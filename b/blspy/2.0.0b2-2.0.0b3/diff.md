# Comparing `tmp/blspy-2.0.0b2.tar.gz` & `tmp/blspy-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blspy-2.0.0b2.tar", last modified: Mon Jun 12 17:02:03 2023, max compression
+gzip compressed data, was "blspy-2.0.0b3.tar", last modified: Tue Jun 13 16:43:59 2023, max compression
```

## Comparing `blspy-2.0.0b2.tar` & `blspy-2.0.0b3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.757443 blspy-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.745443 blspy-2.0.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.github/workflows/build-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.github/workflows/js-bindings.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-12 17:01:54.000000 blspy-2.0.0b2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-12 17:01:54.000000 blspy-2.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-12 17:01:54.000000 blspy-2.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-12 17:02:03.757443 blspy-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-12 17:01:54.000000 blspy-2.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/blspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/cmake_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-12 17:01:54.000000 blspy-2.0.0b2/cmake_modules/Findsodium.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-06-12 17:01:54.000000 blspy-2.0.0b2/emsdk_build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/js-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/blsjs.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/jsbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   126728 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/js-bindings/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/PrivateKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/PublicKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/Signature.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/karma.test.js
--rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/typings.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.753443 blspy-2.0.0b2/js-bindings/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/G1ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/G1ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/G2ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/G2ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/JSWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/PrivateKeyWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/PrivateKeyWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/SchemeMPLWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/SchemeMPLWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/UtilWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/UtilWrapper.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      219 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 17:01:54.000000 blspy-2.0.0b2/lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 17:01:54.000000 blspy-2.0.0b2/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 17:01:54.000000 blspy-2.0.0b2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.753443 blspy-2.0.0b2/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    29858 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/pythonbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.753443 blspy-2.0.0b2/python-impl/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/bls12381.py
--rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21950 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/hash_to_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/hd_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/impl-test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/op_swu_g2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:02:03.757443 blspy-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-12 17:01:54.000000 blspy-2.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.757443 blspy-2.0.0b2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/bls.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/bls.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   261840 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/blstasm.lib
--rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/elements.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/elements.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/hdkeys.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/hkdf.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/privatekey.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/privatekey.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/schemes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/schemes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/test-bench.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/test-utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    55932 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.431975 blspy-2.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.419975 blspy-2.0.0b3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.423975 blspy-2.0.0b3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.github/workflows/build-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.github/workflows/js-bindings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-13 16:43:49.000000 blspy-2.0.0b3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-13 16:43:49.000000 blspy-2.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-13 16:43:49.000000 blspy-2.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-13 16:43:59.431975 blspy-2.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-13 16:43:49.000000 blspy-2.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.423975 blspy-2.0.0b3/blspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.423975 blspy-2.0.0b3/cmake_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-13 16:43:49.000000 blspy-2.0.0b3/cmake_modules/Findsodium.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-06-13 16:43:49.000000 blspy-2.0.0b3/emsdk_build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.423975 blspy-2.0.0b3/js-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/blsjs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/jsbindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   126728 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.427975 blspy-2.0.0b3/js-bindings/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/PrivateKey.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/PublicKey.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/Signature.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/karma.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/typings.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.427975 blspy-2.0.0b3/js-bindings/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/G1ElementWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/G1ElementWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/G2ElementWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/G2ElementWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/JSWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/PrivateKeyWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/PrivateKeyWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/SchemeMPLWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/SchemeMPLWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/UtilWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/UtilWrapper.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      219 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-13 16:43:49.000000 blspy-2.0.0b3/lgtm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 16:43:49.000000 blspy-2.0.0b3/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 16:43:49.000000 blspy-2.0.0b3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.427975 blspy-2.0.0b3/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29858 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/pythonbindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.427975 blspy-2.0.0b3/python-impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/bls12381.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21950 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/hash_to_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/hd_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/impl-test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/op_swu_g2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:43:59.431975 blspy-2.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-13 16:43:49.000000 blspy-2.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.431975 blspy-2.0.0b3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/bls.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/bls.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   261840 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/blstasm.lib
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/elements.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/elements.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/hdkeys.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/hkdf.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/privatekey.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/privatekey.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/schemes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/schemes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/test-bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/test-utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    56462 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/util.hpp
```

### Comparing `blspy-2.0.0b2/.github/workflows/build-test.yaml` & `blspy-2.0.0b3/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/.github/workflows/build-wheels.yml` & `blspy-2.0.0b3/.github/workflows/build-wheels.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/.github/workflows/js-bindings.yml` & `blspy-2.0.0b3/.github/workflows/js-bindings.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/.github/workflows/stale-issue.yml` & `blspy-2.0.0b3/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/CMakeLists.txt` & `blspy-2.0.0b3/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   GIT_TAG f73a3fe1afdc4e37ac5fe0ddd401bf521f6bba65
 )
 set(SODIUM_PCH "on" CACHE STRING "")
 set(SODIUM_DISABLE_TESTS "on" CACHE STRING "")
 set(SODIUM_CHIA_MINIMAL "on" CACHE STRING "")
 FetchContent_MakeAvailable(Sodium)
 
-set(BLST_GIT_TAG "origin/master")
+set(BLST_GIT_TAG "a8cd361c9f671577aeab3f074098443af92a53fc")
 set(BLST_REPOSITORY "https://github.com/supranational/blst")
 
 message(STATUS "blst will be built from: ${BLST_GIT_TAG} and repository ${BLST_REPOSITORY}")
 
 FetchContent_Declare(
   blst
   GIT_REPOSITORY ${BLST_REPOSITORY}
```

### Comparing `blspy-2.0.0b2/LICENSE` & `blspy-2.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/PKG-INFO` & `blspy-2.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blspy
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: BLS signatures in c++ (python bindings)
 Home-page: https://github.com/Chia-Network/bls-signatures
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blspy-2.0.0b2/README.md` & `blspy-2.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/blspy.egg-info/PKG-INFO` & `blspy-2.0.0b3/blspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blspy
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: BLS signatures in c++ (python bindings)
 Home-page: https://github.com/Chia-Network/bls-signatures
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blspy-2.0.0b2/blspy.egg-info/SOURCES.txt` & `blspy-2.0.0b3/blspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/cmake_modules/Findsodium.cmake` & `blspy-2.0.0b3/cmake_modules/Findsodium.cmake`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/CMakeLists.txt` & `blspy-2.0.0b3/js-bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/README.md` & `blspy-2.0.0b3/js-bindings/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/blsjs.d.ts` & `blspy-2.0.0b3/js-bindings/blsjs.d.ts`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/helpers.cpp` & `blspy-2.0.0b3/js-bindings/helpers.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/helpers.h` & `blspy-2.0.0b3/js-bindings/helpers.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/jsbindings.cpp` & `blspy-2.0.0b3/js-bindings/jsbindings.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/package-lock.json` & `blspy-2.0.0b3/js-bindings/package-lock.json`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/package.json` & `blspy-2.0.0b3/js-bindings/package.json`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/tests/PrivateKey.spec.js` & `blspy-2.0.0b3/js-bindings/tests/PrivateKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/tests/PublicKey.spec.js` & `blspy-2.0.0b3/js-bindings/tests/PublicKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/tests/Signature.spec.js` & `blspy-2.0.0b3/js-bindings/tests/Signature.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/tests/karma.conf.js` & `blspy-2.0.0b3/js-bindings/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/tests/test.js` & `blspy-2.0.0b3/js-bindings/tests/test.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/tests/typings.spec.ts` & `blspy-2.0.0b3/js-bindings/tests/typings.spec.ts`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/tests/yarn.lock` & `blspy-2.0.0b3/js-bindings/tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/G1ElementWrapper.cpp` & `blspy-2.0.0b3/js-bindings/wrappers/G1ElementWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/G1ElementWrapper.h` & `blspy-2.0.0b3/js-bindings/wrappers/G1ElementWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/G2ElementWrapper.cpp` & `blspy-2.0.0b3/js-bindings/wrappers/G2ElementWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/G2ElementWrapper.h` & `blspy-2.0.0b3/js-bindings/wrappers/G2ElementWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/JSWrapper.h` & `blspy-2.0.0b3/js-bindings/wrappers/JSWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/PrivateKeyWrapper.cpp` & `blspy-2.0.0b3/js-bindings/wrappers/PrivateKeyWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/PrivateKeyWrapper.h` & `blspy-2.0.0b3/js-bindings/wrappers/PrivateKeyWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/SchemeMPLWrapper.cpp` & `blspy-2.0.0b3/js-bindings/wrappers/SchemeMPLWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/SchemeMPLWrapper.h` & `blspy-2.0.0b3/js-bindings/wrappers/SchemeMPLWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/UtilWrapper.cpp` & `blspy-2.0.0b3/js-bindings/wrappers/UtilWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/js-bindings/wrappers/UtilWrapper.h` & `blspy-2.0.0b3/js-bindings/wrappers/UtilWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-bindings/README.md` & `blspy-2.0.0b3/python-bindings/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-bindings/benchmark.py` & `blspy-2.0.0b3/python-bindings/benchmark.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-bindings/pythonbindings.cpp` & `blspy-2.0.0b3/python-bindings/pythonbindings.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-bindings/test.py` & `blspy-2.0.0b3/python-bindings/test.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/README.md` & `blspy-2.0.0b3/python-impl/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/bls12381.py` & `blspy-2.0.0b3/python-impl/bls12381.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/ec.py` & `blspy-2.0.0b3/python-impl/ec.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/fields.py` & `blspy-2.0.0b3/python-impl/fields.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/hash_to_field.py` & `blspy-2.0.0b3/python-impl/hash_to_field.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/hd_keys.py` & `blspy-2.0.0b3/python-impl/hd_keys.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/hkdf.py` & `blspy-2.0.0b3/python-impl/hkdf.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/impl-test.py` & `blspy-2.0.0b3/python-impl/impl-test.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/op_swu_g2.py` & `blspy-2.0.0b3/python-impl/op_swu_g2.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/pairing.py` & `blspy-2.0.0b3/python-impl/pairing.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/private_key.py` & `blspy-2.0.0b3/python-impl/private_key.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/schemes.py` & `blspy-2.0.0b3/python-impl/schemes.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/python-impl/util.py` & `blspy-2.0.0b3/python-impl/util.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/setup.py` & `blspy-2.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/CMakeLists.txt` & `blspy-2.0.0b3/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/bls.cpp` & `blspy-2.0.0b3/src/bls.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/bls.hpp` & `blspy-2.0.0b3/src/bls.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/blstasm.lib` & `blspy-2.0.0b3/src/blstasm.lib`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/elements.cpp` & `blspy-2.0.0b3/src/elements.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -189,22 +189,22 @@
 std::ostream& operator<<(std::ostream& os, const G1Element& ele)
 {
     return os << Util::HexStr(ele.Serialize());
 }
 
 G1Element& operator+=(G1Element& a, const G1Element& b)
 {
-    blst_p1_add(&(a.p), &(a.p), &(b.p));
+    blst_p1_add_or_double(&(a.p), &(a.p), &(b.p));
     return a;
 }
 
 G1Element operator+(const G1Element& a, const G1Element& b)
 {
     G1Element ans;
-    blst_p1_add(&(ans.p), &(a.p), &(b.p));
+    blst_p1_add_or_double(&(ans.p), &(a.p), &(b.p));
     return ans;
 }
 
 G1Element operator*(const G1Element& a, const blst_scalar& k)
 {
     G1Element ans;
     byte* bte = Util::SecAlloc<byte>(32);
@@ -356,22 +356,22 @@
 std::ostream& operator<<(std::ostream& os, const G2Element& s)
 {
     return os << Util::HexStr(s.Serialize());
 }
 
 G2Element& operator+=(G2Element& a, const G2Element& b)
 {
-    blst_p2_add(&(a.q), &(a.q), &(b.q));
+    blst_p2_add_or_double(&(a.q), &(a.q), &(b.q));
     return a;
 }
 
 G2Element operator+(const G2Element& a, const G2Element& b)
 {
     G2Element ans;
-    blst_p2_add(&(ans.q), &(a.q), &(b.q));
+    blst_p2_add_or_double(&(ans.q), &(a.q), &(b.q));
     return ans;
 }
 
 G2Element operator*(const G2Element& a, const blst_scalar& k)
 {
     G2Element ans;
     byte* bte = Util::SecAlloc<byte>(32);
```

### Comparing `blspy-2.0.0b2/src/elements.hpp` & `blspy-2.0.0b3/src/elements.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/hdkeys.hpp` & `blspy-2.0.0b3/src/hdkeys.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/hkdf.hpp` & `blspy-2.0.0b3/src/hkdf.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/privatekey.cpp` & `blspy-2.0.0b3/src/privatekey.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/privatekey.hpp` & `blspy-2.0.0b3/src/privatekey.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/schemes.cpp` & `blspy-2.0.0b3/src/schemes.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/schemes.hpp` & `blspy-2.0.0b3/src/schemes.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/test-bench.cpp` & `blspy-2.0.0b3/src/test-bench.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/test-utils.hpp` & `blspy-2.0.0b3/src/test-utils.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b2/src/test.cpp` & `blspy-2.0.0b3/src/test.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -798,14 +798,29 @@
             PopSchemeMPL().FastAggregateVerify(pks_as_g1, msg, aggSig) ==
             false);
         REQUIRE(pks_as_bytes.size() == 0);
         REQUIRE(
             PopSchemeMPL().FastAggregateVerify(
                 pks_as_bytes, msg, aggSig.Serialize()) == false);
     }
+    SECTION("Aggregate same sig element")
+    {
+        vector<uint8_t> message = {100, 2, 254, 88, 90, 45, 23};
+
+        vector<uint8_t> seed(32, 0x50);
+
+        PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
+
+        G1Element pk1 = sk1.GetG1Element();
+
+        G2Element sig1Aug = AugSchemeMPL().Sign(sk1, message);
+        G2Element aggSigAug = AugSchemeMPL().Aggregate({sig1Aug, sig1Aug});
+        REQUIRE(AugSchemeMPL().AggregateVerify(
+            {pk1, pk1}, vector<vector<uint8_t>>{message, message}, aggSigAug));
+    }
 }
 
 TEST_CASE("Agg sks")
 {
     SECTION("Should create aggregates with agg sk (basic scheme)")
     {
         const vector<uint8_t> message = {100, 2, 254, 88, 90, 45, 23};
```

### Comparing `blspy-2.0.0b2/src/util.hpp` & `blspy-2.0.0b3/src/util.hpp`

 * *Files identical despite different names*

