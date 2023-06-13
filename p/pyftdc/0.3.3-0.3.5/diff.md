# Comparing `tmp/pyftdc-0.3.3.tar.gz` & `tmp/pyftdc-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftdc-0.3.3.tar", last modified: Wed Apr 19 17:19:26 2023, max compression
+gzip compressed data, was "pyftdc-0.3.5.tar", last modified: Tue Jun 13 19:39:19 2023, max compression
```

## Comparing `pyftdc-0.3.3.tar` & `pyftdc-0.3.5.tar`

### file list

```diff
@@ -1,300 +1,300 @@
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.630099 pyftdc-0.3.3/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1109 2023-04-19 15:22:46.000000 pyftdc-0.3.3/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2182 2023-03-29 21:01:49.000000 pyftdc-0.3.3/LICENSE
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      444 2023-03-29 21:01:49.000000 pyftdc-0.3.3/MANIFEST.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8130 2023-04-19 17:19:26.629880 pyftdc-0.3.3/PKG-INFO
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7595 2023-03-29 21:01:49.000000 pyftdc-0.3.3/README.md
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.588911 pyftdc-0.3.3/extern/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1386 2023-03-29 21:01:49.000000 pyftdc-0.3.3/extern/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.591259 pyftdc-0.3.3/pybind11/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1304 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.appveyor.yml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      996 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.clang-format
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2210 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.clang-tidy
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2196 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.cmake-format.yaml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      487 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.gitignore
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3477 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       62 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/.readthedocs.yml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    10999 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1684 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/LICENSE
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      256 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/MANIFEST.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7656 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/README.rst
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.594809 pyftdc-0.3.3/pybind11/docs/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      653 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/Doxyfile
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.594972 pyftdc-0.3.3/pybind11/docs/_static/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      254 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/_static/theme_overrides.css
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.595962 pyftdc-0.3.3/pybind11/docs/advanced/
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.597237 pyftdc-0.3.3/pybind11/docs/advanced/cast/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3937 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3409 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14283 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3889 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1556 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12433 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9703 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9363 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    48319 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8453 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17806 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    26827 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12446 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.597914 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      278 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17447 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9030 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5710 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6367 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9368 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/basics.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2962 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/benchmark.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3168 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/benchmark.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    99067 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/changelog.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    16451 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/classes.rst
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.598150 pyftdc-0.3.3/pybind11/docs/cmake/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      273 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/cmake/index.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    26267 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/compiling.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12082 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/conf.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14599 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/faq.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      613 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/index.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3277 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/installing.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3079 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/limitations.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    58510 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    44653 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    87708 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    41121 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    85853 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2647 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/reference.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4414 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/release.rst
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      130 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/requirements.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    23491 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.586228 pyftdc-0.3.3/pybind11/include/
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.601153 pyftdc-0.3.3/pybind11/include/pybind11/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    23920 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/attr.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7069 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    64793 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/cast.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8907 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      120 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/common.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2096 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.602259 pyftdc-0.3.3/pybind11/include/pybind11/detail/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    28526 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    51655 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5491 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17971 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    24196 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    44414 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1513 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    31441 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12175 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/embed.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5589 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/eval.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4755 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/functional.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6848 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/gil.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8851 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    78036 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9781 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/operators.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2181 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/options.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)   125927 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    80901 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.602398 pyftdc-0.3.3/pybind11/include/pybind11/stl/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3551 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14438 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/stl.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    26992 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2575 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/noxfile.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.603554 pyftdc-0.3.3/pybind11/pybind11/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      216 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/__init__.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1158 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/__main__.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      202 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/_version.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      137 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/_version.pyi
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      662 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/commands.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/py.typed
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17483 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2038 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pybind11/setup_helpers.pyi
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      957 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/pyproject.toml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1910 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/setup.cfg
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5057 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/setup.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.617337 pyftdc-0.3.3/pybind11/tests/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    21095 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4841 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/conftest.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    11734 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/constructor_stats.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1781 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1022 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/env.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.617749 pyftdc-0.3.3/pybind11/tests/extra_python_package/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7578 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.618053 pyftdc-0.3.3/pybind11/tests/extra_setuptools/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4221 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2847 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/local_bindings.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5743 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/object.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6264 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3686 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3018 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      693 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/pytest.ini
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      877 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/requirements.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      855 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_async.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      558 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_async.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8567 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5055 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_buffers.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    15872 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    18372 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4118 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6573 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_call_policies.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9243 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6044 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_callbacks.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3370 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5727 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_chrono.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    23812 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_class.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14508 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_class.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.618641 pyftdc-0.3.3/pybind11/tests/test_cmake_build/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2639 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      673 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.618809 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1171 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.618952 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1293 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.619096 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1685 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      152 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.619258 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1353 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.619439 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1163 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.619600 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1368 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      273 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4254 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      650 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_const_name.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5934 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1522 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    10718 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4646 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_copy_move.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7210 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4088 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1259 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1114 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2816 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1630 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    18169 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eigen.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    28283 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.620488 pyftdc-0.3.3/pybind11/tests/test_embed/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1798 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      733 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      543 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14173 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      280 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      300 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5722 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_enum.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9132 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_enum.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3168 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eval.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1183 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eval.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      143 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_eval_call.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    10197 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      399 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_exceptions.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9038 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_exceptions.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    18419 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    16731 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1673 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3128 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4122 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7958 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_iostream.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9236 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    13998 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4401 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8101 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    21327 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    17804 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4021 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_modules.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2843 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_modules.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12305 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    12034 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    19774 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20339 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20154 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14036 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4461 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9710 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2777 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1907 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9463 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4392 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     6646 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2286 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_pickling.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20878 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    19010 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_pytypes.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20580 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8059 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    19040 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9620 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    20722 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_stl.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    11662 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_stl.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4622 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8071 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     4597 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      765 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1855 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_thread.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      875 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_thread.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      603 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_union.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      172 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_union.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    23102 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    13146 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3226 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2657 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.622988 pyftdc-0.3.3/pybind11/tools/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2350 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     3105 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    10378 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 jorge.imperial   (502) staff       (20)     1423 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/check-style.sh
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      952 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1122 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/libsize.py
--rwxr-xr-x   0 jorge.imperial   (502) staff       (20)     1306 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/make_changelog.py
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14579 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7063 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9673 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     7447 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       94 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/pyproject.toml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1951 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/setup_global.py.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1089 2023-03-29 21:01:49.000000 pyftdc-0.3.3/pybind11/tools/setup_main.py.in
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      679 2023-04-19 17:18:48.000000 pyftdc-0.3.3/pyproject.toml
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       38 2023-04-19 17:19:26.630141 pyftdc-0.3.3/setup.cfg
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5492 2023-04-19 15:22:46.000000 pyftdc-0.3.3/setup.py
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.625841 pyftdc-0.3.3/src/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    13508 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/BinaryBSON.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2236 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/CSVWriter.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      354 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/ChunkMetric.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      177 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/ConstDataRangeCursor.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     5987 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/Dataset.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8622 2023-04-01 15:17:09.000000 pyftdc-0.3.3/src/FTDCParser.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      351 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/FileParsedData.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1911 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/JSONWriter.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2744 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/MetricsToWTMap.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2680 2023-03-31 02:42:43.000000 pyftdc-0.3.3/src/ParserState.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       62 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/ParserTask.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2240 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/ParserTasksList.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       68 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/SampleLocation.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       65 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/WriterTask.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      643 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/WriterTaskList.cpp
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.628738 pyftdc-0.3.3/src/include/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      894 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/include/BinaryBSON.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      447 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/CSVWriter.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      813 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/include/ChunkMetric.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      633 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/ConstDataRangeCursor.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     2131 2023-04-11 21:35:43.000000 pyftdc-0.3.3/src/include/Dataset.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1158 2023-04-01 15:17:09.000000 pyftdc-0.3.3/src/include/FTDCParser.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      753 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/FileParsedData.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      444 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/JSONWriter.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      271 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/Metrics.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      976 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/MetricsToWTMap.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1420 2023-03-31 02:42:43.000000 pyftdc-0.3.3/src/include/ParserState.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      593 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/ParserTask.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      625 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/ParserTasksList.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      468 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/SampleLocation.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      261 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/Timestamp.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      392 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/WriterTask.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)      676 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/WriterTaskList.h
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     1470 2023-03-29 21:01:49.000000 pyftdc-0.3.3/src/include/bson_value.h
-drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-04-19 17:19:26.629679 pyftdc-0.3.3/src/pyftdc.egg-info/
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     8130 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/PKG-INFO
--rw-r--r--   0 jorge.imperial   (502) staff       (20)     9039 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/SOURCES.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/dependency_links.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2023-04-19 15:22:46.000000 pyftdc-0.3.3/src/pyftdc.egg-info/not-zip-safe
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       20 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/requires.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)       15 2023-04-19 17:19:26.000000 pyftdc-0.3.3/src/pyftdc.egg-info/top_level.txt
--rw-r--r--   0 jorge.imperial   (502) staff       (20)    14741 2023-04-19 15:22:46.000000 pyftdc-0.3.3/src/python.cpp
--rw-r--r--   0 jorge.imperial   (502) staff       (20)        6 2023-04-19 17:18:36.000000 pyftdc-0.3.3/version.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.185943 pyftdc-0.3.5/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1017 2023-05-28 00:31:08.000000 pyftdc-0.3.5/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2182 2023-03-29 21:01:49.000000 pyftdc-0.3.5/LICENSE
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      432 2023-05-28 00:31:08.000000 pyftdc-0.3.5/MANIFEST.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8161 2023-06-13 19:39:19.185784 pyftdc-0.3.5/PKG-INFO
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7595 2023-03-29 21:01:49.000000 pyftdc-0.3.5/README.md
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.127315 pyftdc-0.3.5/extern/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1386 2023-03-29 21:01:49.000000 pyftdc-0.3.5/extern/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.130100 pyftdc-0.3.5/pybind11/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1304 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/.appveyor.yml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      996 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/.clang-format
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2210 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/.clang-tidy
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2196 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/.cmake-format.yaml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      487 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/.gitignore
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3477 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       62 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/.readthedocs.yml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    10999 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1684 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/LICENSE
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      256 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/MANIFEST.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7656 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/README.rst
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.135023 pyftdc-0.3.5/pybind11/docs/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      653 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/Doxyfile
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.135205 pyftdc-0.3.5/pybind11/docs/_static/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      254 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/_static/theme_overrides.css
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.136702 pyftdc-0.3.5/pybind11/docs/advanced/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.138095 pyftdc-0.3.5/pybind11/docs/advanced/cast/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3937 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3409 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14283 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3889 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1556 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12433 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9703 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9363 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    48319 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8453 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17806 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    26827 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12446 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.138858 pyftdc-0.3.5/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      278 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17447 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9030 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5710 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6367 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9368 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/basics.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2962 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/benchmark.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3168 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/benchmark.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    99067 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/changelog.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    16451 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/classes.rst
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.139032 pyftdc-0.3.5/pybind11/docs/cmake/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      273 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    26267 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/compiling.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12082 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/conf.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14599 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/faq.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      613 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/index.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3277 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/installing.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3079 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/limitations.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    58510 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    44653 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    87708 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    41121 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    85853 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2647 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/reference.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4414 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/release.rst
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      130 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/requirements.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    23491 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.124924 pyftdc-0.3.5/pybind11/include/
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.142462 pyftdc-0.3.5/pybind11/include/pybind11/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    23920 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7069 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    64793 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8907 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      120 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/common.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2096 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.143673 pyftdc-0.3.5/pybind11/include/pybind11/detail/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    28526 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    51655 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5491 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17971 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    24196 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    44414 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1513 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    31441 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12175 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5589 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4755 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6848 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8851 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    78036 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9781 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2181 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/options.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)   125927 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    80901 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.144050 pyftdc-0.3.5/pybind11/include/pybind11/stl/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3551 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14438 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    26992 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2575 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/noxfile.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.150230 pyftdc-0.3.5/pybind11/pybind11/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      216 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/pybind11/__init__.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1158 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/pybind11/__main__.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      202 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/pybind11/_version.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      137 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/pybind11/_version.pyi
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      662 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/pybind11/commands.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/pybind11/py.typed
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17483 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2038 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/pybind11/setup_helpers.pyi
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      957 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/pyproject.toml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1910 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/setup.cfg
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5057 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/setup.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.171066 pyftdc-0.3.5/pybind11/tests/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    21095 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4841 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/conftest.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    11734 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1781 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1022 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/env.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.171398 pyftdc-0.3.5/pybind11/tests/extra_python_package/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7578 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.171802 pyftdc-0.3.5/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        0 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4221 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2847 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/local_bindings.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5743 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/object.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6264 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3686 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3018 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      693 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/pytest.ini
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      877 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/requirements.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      855 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_async.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      558 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_async.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8567 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5055 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_buffers.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    15872 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    18372 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4118 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6573 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9243 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6044 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3370 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5727 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_chrono.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    23812 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_class.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14508 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_class.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.172574 pyftdc-0.3.5/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2639 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      673 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.172737 pyftdc-0.3.5/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1171 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.172923 pyftdc-0.3.5/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1293 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.173116 pyftdc-0.3.5/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1685 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      152 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.173297 pyftdc-0.3.5/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1353 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.173532 pyftdc-0.3.5/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1163 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.173790 pyftdc-0.3.5/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1368 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      273 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4254 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      650 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_const_name.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5934 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1522 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    10718 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4646 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7210 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4088 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1259 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1114 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2816 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1630 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    18169 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_eigen.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    28283 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_eigen.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.174929 pyftdc-0.3.5/pybind11/tests/test_embed/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1798 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      733 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      543 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14173 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      280 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      300 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5722 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9132 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_enum.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3168 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1183 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_eval.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      143 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    10197 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      399 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9038 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    18419 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    16731 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1673 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3128 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4122 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7958 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_iostream.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9236 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    13998 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4401 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8101 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    21327 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    17804 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4021 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2843 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_modules.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12305 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    12034 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    19774 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20339 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20154 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14036 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4461 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9710 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2777 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1907 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9463 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4392 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6646 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2286 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_pickling.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20878 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    19010 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20580 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8059 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    19040 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9620 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    20722 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    11662 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_stl.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4622 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8071 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     4597 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      765 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1855 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      875 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_thread.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      603 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_union.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      172 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_union.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    23102 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    13146 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3226 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2657 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.178088 pyftdc-0.3.5/pybind11/tools/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2350 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     3105 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    10378 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 jorge.imperial   (502) staff       (20)     1423 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/check-style.sh
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      952 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1122 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/libsize.py
+-rwxr-xr-x   0 jorge.imperial   (502) staff       (20)     1306 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/make_changelog.py
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    14579 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7063 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9673 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     7447 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       94 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/pyproject.toml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1951 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1089 2023-03-29 21:01:49.000000 pyftdc-0.3.5/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      710 2023-06-13 18:34:37.000000 pyftdc-0.3.5/pyproject.toml
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       38 2023-06-13 19:39:19.185990 pyftdc-0.3.5/setup.cfg
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     6197 2023-05-28 00:31:08.000000 pyftdc-0.3.5/setup.py
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.181215 pyftdc-0.3.5/src/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    13508 2023-04-11 21:35:43.000000 pyftdc-0.3.5/src/BinaryBSON.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2236 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/CSVWriter.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      354 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/ChunkMetric.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      177 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/ConstDataRangeCursor.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     5988 2023-06-13 18:34:37.000000 pyftdc-0.3.5/src/Dataset.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8622 2023-04-01 15:17:09.000000 pyftdc-0.3.5/src/FTDCParser.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      351 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/FileParsedData.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1911 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/JSONWriter.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2744 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/MetricsToWTMap.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2680 2023-03-31 02:42:43.000000 pyftdc-0.3.5/src/ParserState.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       62 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/ParserTask.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2240 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/ParserTasksList.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       68 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/SampleLocation.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       65 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/WriterTask.cpp
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      643 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/WriterTaskList.cpp
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.184561 pyftdc-0.3.5/src/include/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      894 2023-04-11 21:35:43.000000 pyftdc-0.3.5/src/include/BinaryBSON.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      447 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/CSVWriter.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      813 2023-04-11 21:35:43.000000 pyftdc-0.3.5/src/include/ChunkMetric.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      633 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/ConstDataRangeCursor.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     2131 2023-04-11 21:35:43.000000 pyftdc-0.3.5/src/include/Dataset.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1158 2023-04-01 15:17:09.000000 pyftdc-0.3.5/src/include/FTDCParser.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      753 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/FileParsedData.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      444 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/JSONWriter.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      271 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/Metrics.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      976 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/MetricsToWTMap.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1420 2023-03-31 02:42:43.000000 pyftdc-0.3.5/src/include/ParserState.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      593 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/ParserTask.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      625 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/ParserTasksList.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      468 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/SampleLocation.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      261 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/Timestamp.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      392 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/WriterTask.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)      676 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/WriterTaskList.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     1470 2023-03-29 21:01:49.000000 pyftdc-0.3.5/src/include/bson_value.h
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       28 2023-06-13 19:39:19.000000 pyftdc-0.3.5/src/include/version.h
+drwxr-xr-x   0 jorge.imperial   (502) staff       (20)        0 2023-06-13 19:39:19.185596 pyftdc-0.3.5/src/pyftdc.egg-info/
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     8161 2023-06-13 19:39:19.000000 pyftdc-0.3.5/src/pyftdc.egg-info/PKG-INFO
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)     9049 2023-06-13 19:39:19.000000 pyftdc-0.3.5/src/pyftdc.egg-info/SOURCES.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2023-06-13 19:39:19.000000 pyftdc-0.3.5/src/pyftdc.egg-info/dependency_links.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)        1 2023-04-19 15:22:46.000000 pyftdc-0.3.5/src/pyftdc.egg-info/not-zip-safe
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       20 2023-06-13 19:39:19.000000 pyftdc-0.3.5/src/pyftdc.egg-info/requires.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)       15 2023-06-13 19:39:19.000000 pyftdc-0.3.5/src/pyftdc.egg-info/top_level.txt
+-rw-r--r--   0 jorge.imperial   (502) staff       (20)    15512 2023-05-28 00:31:08.000000 pyftdc-0.3.5/src/python.cpp
```

### Comparing `pyftdc-0.3.3/CMakeLists.txt` & `pyftdc-0.3.5/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 cmake_minimum_required(VERSION 3.15)
 project(pyftdc)
 
 set(CMAKE_CXX_STANDARD 17)
 
-# Get version from file
-file(READ "version.txt" file_version)
-
-message( "---------------------- library ${PROJECT_NAME} version: " ${file_version}  "----------------------------")
+message( "---------------------- library ${PROJECT_NAME} ----------------------------")
 
 add_subdirectory(extern)
 add_subdirectory(pybind11)
 #add_subdirectory(Boost_tests)
 
 pybind11_add_module(${PROJECT_NAME}
         src/python.cpp
```

### Comparing `pyftdc-0.3.3/LICENSE` & `pyftdc-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/PKG-INFO` & `pyftdc-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyftdc
-Version: 0.3.3
-Summary: A small example package
+Version: 0.3.5
+Summary: A parser for MongoDB FTDC files, with Python bindings.
 Author: Jorge Imperial
 Author-email: Jorge Imperial <jlimperial@protonmail.com>
 Project-URL: Homepage, https://gitlab.com/jimper/mongo_ftdc
 Project-URL: Bug Tracker, https://gitlab.com/jimper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyftdc-0.3.3/README.md` & `pyftdc-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/extern/CMakeLists.txt` & `pyftdc-0.3.5/extern/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/.appveyor.yml` & `pyftdc-0.3.5/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/.clang-format` & `pyftdc-0.3.5/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/.clang-tidy` & `pyftdc-0.3.5/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/.cmake-format.yaml` & `pyftdc-0.3.5/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/.pre-commit-config.yaml` & `pyftdc-0.3.5/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/LICENSE` & `pyftdc-0.3.5/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/README.rst` & `pyftdc-0.3.5/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/Doxyfile` & `pyftdc-0.3.5/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/cast/chrono.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/cast/custom.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/cast/eigen.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/cast/functional.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/cast/index.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/cast/overview.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/cast/stl.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/cast/strings.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/classes.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/embedding.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/exceptions.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/functions.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/misc.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/pycpp/numpy.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/pycpp/object.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/pycpp/utilities.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/advanced/smart_ptrs.rst` & `pyftdc-0.3.5/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/basics.rst` & `pyftdc-0.3.5/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/benchmark.py` & `pyftdc-0.3.5/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/benchmark.rst` & `pyftdc-0.3.5/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/changelog.rst` & `pyftdc-0.3.5/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/classes.rst` & `pyftdc-0.3.5/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/compiling.rst` & `pyftdc-0.3.5/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/conf.py` & `pyftdc-0.3.5/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/faq.rst` & `pyftdc-0.3.5/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/index.rst` & `pyftdc-0.3.5/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/installing.rst` & `pyftdc-0.3.5/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/limitations.rst` & `pyftdc-0.3.5/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/pybind11-logo.png` & `pyftdc-0.3.5/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python1.png` & `pyftdc-0.3.5/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python1.svg` & `pyftdc-0.3.5/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python2.png` & `pyftdc-0.3.5/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/pybind11_vs_boost_python2.svg` & `pyftdc-0.3.5/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/reference.rst` & `pyftdc-0.3.5/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/release.rst` & `pyftdc-0.3.5/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/docs/upgrade.rst` & `pyftdc-0.3.5/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/attr.h` & `pyftdc-0.3.5/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/buffer_info.h` & `pyftdc-0.3.5/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/cast.h` & `pyftdc-0.3.5/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/chrono.h` & `pyftdc-0.3.5/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/complex.h` & `pyftdc-0.3.5/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/detail/class.h` & `pyftdc-0.3.5/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/detail/common.h` & `pyftdc-0.3.5/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/detail/descr.h` & `pyftdc-0.3.5/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/detail/init.h` & `pyftdc-0.3.5/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/detail/internals.h` & `pyftdc-0.3.5/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/detail/type_caster_base.h` & `pyftdc-0.3.5/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/detail/typeid.h` & `pyftdc-0.3.5/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/eigen.h` & `pyftdc-0.3.5/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/embed.h` & `pyftdc-0.3.5/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/eval.h` & `pyftdc-0.3.5/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/functional.h` & `pyftdc-0.3.5/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/gil.h` & `pyftdc-0.3.5/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/iostream.h` & `pyftdc-0.3.5/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/numpy.h` & `pyftdc-0.3.5/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/operators.h` & `pyftdc-0.3.5/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/options.h` & `pyftdc-0.3.5/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/pybind11.h` & `pyftdc-0.3.5/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/pytypes.h` & `pyftdc-0.3.5/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/stl/filesystem.h` & `pyftdc-0.3.5/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/stl.h` & `pyftdc-0.3.5/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/include/pybind11/stl_bind.h` & `pyftdc-0.3.5/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/noxfile.py` & `pyftdc-0.3.5/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/pybind11/__main__.py` & `pyftdc-0.3.5/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/pybind11/commands.py` & `pyftdc-0.3.5/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/pybind11/setup_helpers.py` & `pyftdc-0.3.5/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/pybind11/setup_helpers.pyi` & `pyftdc-0.3.5/pybind11/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/pyproject.toml` & `pyftdc-0.3.5/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/setup.cfg` & `pyftdc-0.3.5/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/setup.py` & `pyftdc-0.3.5/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/conftest.py` & `pyftdc-0.3.5/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/constructor_stats.h` & `pyftdc-0.3.5/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/cross_module_gil_utils.cpp` & `pyftdc-0.3.5/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/env.py` & `pyftdc-0.3.5/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/extra_python_package/test_files.py` & `pyftdc-0.3.5/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/extra_setuptools/test_setuphelper.py` & `pyftdc-0.3.5/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/local_bindings.h` & `pyftdc-0.3.5/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/object.h` & `pyftdc-0.3.5/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/pybind11_cross_module_tests.cpp` & `pyftdc-0.3.5/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/pybind11_tests.cpp` & `pyftdc-0.3.5/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/pybind11_tests.h` & `pyftdc-0.3.5/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/pytest.ini` & `pyftdc-0.3.5/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/requirements.txt` & `pyftdc-0.3.5/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_async.cpp` & `pyftdc-0.3.5/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_async.py` & `pyftdc-0.3.5/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_buffers.cpp` & `pyftdc-0.3.5/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_buffers.py` & `pyftdc-0.3.5/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_builtin_casters.cpp` & `pyftdc-0.3.5/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_builtin_casters.py` & `pyftdc-0.3.5/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_call_policies.cpp` & `pyftdc-0.3.5/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_call_policies.py` & `pyftdc-0.3.5/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_callbacks.cpp` & `pyftdc-0.3.5/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_callbacks.py` & `pyftdc-0.3.5/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_chrono.cpp` & `pyftdc-0.3.5/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_chrono.py` & `pyftdc-0.3.5/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_class.cpp` & `pyftdc-0.3.5/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_class.py` & `pyftdc-0.3.5/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_cmake_build/embed.cpp` & `pyftdc-0.3.5/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_const_name.cpp` & `pyftdc-0.3.5/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_const_name.py` & `pyftdc-0.3.5/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_constants_and_functions.cpp` & `pyftdc-0.3.5/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_constants_and_functions.py` & `pyftdc-0.3.5/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_copy_move.cpp` & `pyftdc-0.3.5/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_copy_move.py` & `pyftdc-0.3.5/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_custom_type_casters.cpp` & `pyftdc-0.3.5/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_custom_type_casters.py` & `pyftdc-0.3.5/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_custom_type_setup.cpp` & `pyftdc-0.3.5/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_custom_type_setup.py` & `pyftdc-0.3.5/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_docstring_options.cpp` & `pyftdc-0.3.5/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_docstring_options.py` & `pyftdc-0.3.5/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_eigen.cpp` & `pyftdc-0.3.5/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_eigen.py` & `pyftdc-0.3.5/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_embed/CMakeLists.txt` & `pyftdc-0.3.5/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_embed/catch.cpp` & `pyftdc-0.3.5/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_embed/external_module.cpp` & `pyftdc-0.3.5/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_embed/test_interpreter.cpp` & `pyftdc-0.3.5/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_enum.cpp` & `pyftdc-0.3.5/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_enum.py` & `pyftdc-0.3.5/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_eval.cpp` & `pyftdc-0.3.5/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_eval.py` & `pyftdc-0.3.5/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_exceptions.cpp` & `pyftdc-0.3.5/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_exceptions.py` & `pyftdc-0.3.5/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_factory_constructors.cpp` & `pyftdc-0.3.5/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_factory_constructors.py` & `pyftdc-0.3.5/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_gil_scoped.cpp` & `pyftdc-0.3.5/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_gil_scoped.py` & `pyftdc-0.3.5/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_iostream.cpp` & `pyftdc-0.3.5/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_iostream.py` & `pyftdc-0.3.5/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_kwargs_and_defaults.cpp` & `pyftdc-0.3.5/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_kwargs_and_defaults.py` & `pyftdc-0.3.5/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_local_bindings.cpp` & `pyftdc-0.3.5/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_local_bindings.py` & `pyftdc-0.3.5/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_methods_and_attributes.cpp` & `pyftdc-0.3.5/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_methods_and_attributes.py` & `pyftdc-0.3.5/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_modules.cpp` & `pyftdc-0.3.5/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_modules.py` & `pyftdc-0.3.5/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_multiple_inheritance.cpp` & `pyftdc-0.3.5/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_multiple_inheritance.py` & `pyftdc-0.3.5/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_numpy_array.cpp` & `pyftdc-0.3.5/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_numpy_array.py` & `pyftdc-0.3.5/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_numpy_dtypes.cpp` & `pyftdc-0.3.5/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_numpy_dtypes.py` & `pyftdc-0.3.5/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_numpy_vectorize.cpp` & `pyftdc-0.3.5/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_numpy_vectorize.py` & `pyftdc-0.3.5/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_opaque_types.cpp` & `pyftdc-0.3.5/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_opaque_types.py` & `pyftdc-0.3.5/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_operator_overloading.cpp` & `pyftdc-0.3.5/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_operator_overloading.py` & `pyftdc-0.3.5/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_pickling.cpp` & `pyftdc-0.3.5/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_pickling.py` & `pyftdc-0.3.5/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_pytypes.cpp` & `pyftdc-0.3.5/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_pytypes.py` & `pyftdc-0.3.5/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_sequences_and_iterators.cpp` & `pyftdc-0.3.5/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_sequences_and_iterators.py` & `pyftdc-0.3.5/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_smart_ptr.cpp` & `pyftdc-0.3.5/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_smart_ptr.py` & `pyftdc-0.3.5/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_stl.cpp` & `pyftdc-0.3.5/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_stl.py` & `pyftdc-0.3.5/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_stl_binders.cpp` & `pyftdc-0.3.5/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_stl_binders.py` & `pyftdc-0.3.5/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_tagbased_polymorphic.cpp` & `pyftdc-0.3.5/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_tagbased_polymorphic.py` & `pyftdc-0.3.5/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_thread.cpp` & `pyftdc-0.3.5/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_thread.py` & `pyftdc-0.3.5/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_union.cpp` & `pyftdc-0.3.5/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_virtual_functions.cpp` & `pyftdc-0.3.5/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/test_virtual_functions.py` & `pyftdc-0.3.5/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/valgrind-numpy-scipy.supp` & `pyftdc-0.3.5/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tests/valgrind-python.supp` & `pyftdc-0.3.5/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/FindCatch.cmake` & `pyftdc-0.3.5/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/FindEigen3.cmake` & `pyftdc-0.3.5/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/FindPythonLibsNew.cmake` & `pyftdc-0.3.5/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/check-style.sh` & `pyftdc-0.3.5/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/cmake_uninstall.cmake.in` & `pyftdc-0.3.5/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/libsize.py` & `pyftdc-0.3.5/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/make_changelog.py` & `pyftdc-0.3.5/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/pybind11Common.cmake` & `pyftdc-0.3.5/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/pybind11Config.cmake.in` & `pyftdc-0.3.5/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/pybind11NewTools.cmake` & `pyftdc-0.3.5/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/pybind11Tools.cmake` & `pyftdc-0.3.5/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/setup_global.py.in` & `pyftdc-0.3.5/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pybind11/tools/setup_main.py.in` & `pyftdc-0.3.5/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/pyproject.toml` & `pyftdc-0.3.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 ]
 build-backend = "setuptools.build_meta"
  
 
 # Project
 [project]
 name = "pyftdc"
-version = "0.3.3"
+version = "0.3.5"
 authors = [
     { name="Jorge Imperial", email="jlimperial@protonmail.com" },
 ]
-description = "A small example package"
+description = "A parser for MongoDB FTDC files, with Python bindings."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyftdc-0.3.3/setup.py` & `pyftdc-0.3.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,41 @@
+import codecs
 import os
 import re
 import subprocess
 import sys
 
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
 
-with open('version.txt') as f:
-    __version__ = f.readline().rstrip()
-    f.close()
+
+def read(rel_path):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+        return fp.read()
+
+
+rel_path = "./pyproject.toml"
+
+try:
+    for line in read(rel_path).splitlines():
+        if line.startswith('version'):
+            # toml file is of the form 'version = "version"'
+            tokens = line.split()
+            delim = '"' if '"' in tokens[2] else "'"
+            __version__ = tokens[2].split(delim)[1]
+
+            with open("src/include/version.h", "wt") as f:
+                f.write(f'#define PYFTDC_VERSION {__version__}')
+                f.close()
+
+
+            break
+except FileNotFoundError:
+    raise RuntimeError(f'======================Unable to find version string in {rel_path}.')
 
 # Convert distutils Windows platform specifiers to CMake -A arguments
 PLAT_TO_CMAKE = {
     "win32": "Win32",
     "win-amd64": "x64",
     "win-arm32": "ARM",
     "win-arm64": "ARM64",
```

### Comparing `pyftdc-0.3.3/src/BinaryBSON.cpp` & `pyftdc-0.3.5/src/BinaryBSON.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/CSVWriter.cpp` & `pyftdc-0.3.5/src/CSVWriter.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/Dataset.cpp` & `pyftdc-0.3.5/src/Dataset.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         return nullptr;
 
     auto metrics = new std::vector<uint64_t>;
 
     if (samplesInDataset == 0)
         samplesInDataset = parserState->getSamplesCount();
 
-    spdlog::info("Metric: '{}' Reserving space for {} samples.", metricName, samplesInDataset);
+    spdlog::debug("Metric: '{}' Reserving space for {} samples.", metricName, samplesInDataset);
     metrics->reserve(samplesInDataset);
 
     for (auto b : parserState->getBinBSONArray()) {
         auto chunkMetric = b->getMetric(index);
         metrics->insert(metrics->end(),
                         chunkMetric->getValues(),
                         chunkMetric->getValues() + chunkMetric->getSampleCount());
```

### Comparing `pyftdc-0.3.3/src/FTDCParser.cpp` & `pyftdc-0.3.5/src/FTDCParser.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/JSONWriter.cpp` & `pyftdc-0.3.5/src/JSONWriter.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/MetricsToWTMap.cpp` & `pyftdc-0.3.5/src/MetricsToWTMap.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/ParserState.cpp` & `pyftdc-0.3.5/src/ParserState.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/ParserTasksList.cpp` & `pyftdc-0.3.5/src/ParserTasksList.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/WriterTaskList.cpp` & `pyftdc-0.3.5/src/WriterTaskList.cpp`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/BinaryBSON.h` & `pyftdc-0.3.5/src/include/BinaryBSON.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/ChunkMetric.h` & `pyftdc-0.3.5/src/include/ChunkMetric.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/ConstDataRangeCursor.h` & `pyftdc-0.3.5/src/include/ConstDataRangeCursor.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/Dataset.h` & `pyftdc-0.3.5/src/include/Dataset.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/FTDCParser.h` & `pyftdc-0.3.5/src/include/FTDCParser.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/FileParsedData.h` & `pyftdc-0.3.5/src/include/FileParsedData.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/MetricsToWTMap.h` & `pyftdc-0.3.5/src/include/MetricsToWTMap.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/ParserState.h` & `pyftdc-0.3.5/src/include/ParserState.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/ParserTask.h` & `pyftdc-0.3.5/src/include/ParserTask.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/ParserTasksList.h` & `pyftdc-0.3.5/src/include/ParserTasksList.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/WriterTaskList.h` & `pyftdc-0.3.5/src/include/WriterTaskList.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/include/bson_value.h` & `pyftdc-0.3.5/src/include/bson_value.h`

 * *Files identical despite different names*

### Comparing `pyftdc-0.3.3/src/pyftdc.egg-info/PKG-INFO` & `pyftdc-0.3.5/src/pyftdc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyftdc
-Version: 0.3.3
-Summary: A small example package
+Version: 0.3.5
+Summary: A parser for MongoDB FTDC files, with Python bindings.
 Author: Jorge Imperial
 Author-email: Jorge Imperial <jlimperial@protonmail.com>
 Project-URL: Homepage, https://gitlab.com/jimper/mongo_ftdc
 Project-URL: Bug Tracker, https://gitlab.com/jimper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyftdc-0.3.3/src/pyftdc.egg-info/SOURCES.txt` & `pyftdc-0.3.5/src/pyftdc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-version.txt
 extern/CMakeLists.txt
 pybind11/.appveyor.yml
 pybind11/.clang-format
 pybind11/.clang-tidy
 pybind11/.cmake-format.yaml
 pybind11/.gitignore
 pybind11/.pre-commit-config.yaml
@@ -257,13 +256,14 @@
 src/include/ParserTask.h
 src/include/ParserTasksList.h
 src/include/SampleLocation.h
 src/include/Timestamp.h
 src/include/WriterTask.h
 src/include/WriterTaskList.h
 src/include/bson_value.h
+src/include/version.h
 src/pyftdc.egg-info/PKG-INFO
 src/pyftdc.egg-info/SOURCES.txt
 src/pyftdc.egg-info/dependency_links.txt
 src/pyftdc.egg-info/not-zip-safe
 src/pyftdc.egg-info/requires.txt
 src/pyftdc.egg-info/top_level.txt
```

### Comparing `pyftdc-0.3.3/src/python.cpp` & `pyftdc-0.3.5/src/python.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 using namespace py::literals;
 using namespace ftdcparser;
 namespace fs = std::filesystem;
 
 typedef std::vector<std::string> MetricNames;
 
+#include <version.h>
 
 #define FALSE 0
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
 
 //std::vector<uint64_t> *emptyArray;
@@ -100,14 +101,28 @@
     MetricsPtr
     getMetric(std::string &metric_name,
                           size_t start = INVALID_TIMESTAMP, size_t end = INVALID_TIMESTAMP,
                           bool rated_metric = false) const  {
         return dataSet->getMetric(metric_name, start, end, rated_metric);
     }
 
+    [[nodiscard]]
+    std::vector<MetricsPtr>
+    getMetricsList(std::vector<std::string>& metric_names,
+              size_t start = INVALID_TIMESTAMP, size_t end = INVALID_TIMESTAMP,
+              bool rated_metric = false) const  {
+
+        std::vector<MetricsPtr> metricList;
+        for (auto &name : metric_names) {
+            auto m = this->getMetric(name, start, end, rated_metric);
+            metricList.emplace_back(m);
+        }
+
+        return metricList;
+    }
 
     [[nodiscard]]
     py::array_t<unsigned long>
     getMetricAsNumpyArray(std::string &metric_name,
                           size_t start = INVALID_TIMESTAMP,
                           size_t end = INVALID_TIMESTAMP,
                           bool rated_metric = false) const {
@@ -369,15 +384,21 @@
              py::arg("end") = ::INVALID_TIMESTAMP,
              py::arg("rated_metric") = false)
         .def("get_metrics_list_numpy", &DatasetClass::getMetricListAsNumpyArray,
              "Returns a list of metrics as numpy arrays.",
              py::arg("testMetricNames"),
              py::arg("start") = ::INVALID_TIMESTAMP,
              py::arg("end") = ::INVALID_TIMESTAMP,
-             py::arg("rated_metric") = false);
+             py::arg("rated_metric") = false)
+    .def("get_metrics_list", &DatasetClass::getMetricsList,
+         "Returns a list of metrics.",
+         py::arg("MetricNames"),
+         py::arg("start") = ::INVALID_TIMESTAMP,
+         py::arg("end") = ::INVALID_TIMESTAMP,
+         py::arg("rated_metric") = false);
 
 py::class_<ParserClass>(m, "FTDCParser")
     .def(py::init<>())
     .def("set_verbose", &ParserClass::setVerbose,
          "Set verbose flag", py::arg("verbose"))
     .def("parse_dir", &ParserClass::parseDir,
         "Parses all files in a directory",
@@ -426,13 +447,13 @@
         py::arg("start") = ::INVALID_TIMESTAMP,
         py::arg("end") = ::INVALID_TIMESTAMP,
         py::arg("rated_metric") = false,
         py::arg("transpose") = false);
 
 
 
-#ifdef VERSION_INFO
-m.attr("__version__") = MACRO_STRINGIFY(VERSION_INFO);
+#ifdef PYFTDC_VERSION
+m.attr("__version__") = MACRO_STRINGIFY(PYFTDC_VERSION);
 #else
 m.attr("__version__") = "dev";
 #endif
 } // PYBIND11_MODULE
```

