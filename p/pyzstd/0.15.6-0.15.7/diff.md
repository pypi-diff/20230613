# Comparing `tmp/pyzstd-0.15.6.tar.gz` & `tmp/pyzstd-0.15.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzstd-0.15.6.tar", last modified: Wed Apr  5 05:28:58 2023, max compression
+gzip compressed data, was "pyzstd-0.15.7.tar", last modified: Fri Apr 21 12:31:15 2023, max compression
```

## Comparing `pyzstd-0.15.6.tar` & `pyzstd-0.15.7.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.702915 pyzstd-0.15.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-05 05:28:47.000000 pyzstd-0.15.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-05 05:28:47.000000 pyzstd-0.15.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-05 05:28:58.702915 pyzstd-0.15.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-05 05:28:47.000000 pyzstd-0.15.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-04-05 05:28:47.000000 pyzstd-0.15.6/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-05 05:28:47.000000 pyzstd-0.15.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.686915 pyzstd-0.15.6/pyzstd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-05 05:28:58.000000 pyzstd-0.15.6/pyzstd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-05 05:28:58.000000 pyzstd-0.15.6/pyzstd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 05:28:58.000000 pyzstd-0.15.6/pyzstd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 05:28:58.000000 pyzstd-0.15.6/pyzstd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 05:28:58.702915 pyzstd-0.15.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-05 05:28:47.000000 pyzstd-0.15.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.686915 pyzstd-0.15.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-04-05 05:28:47.000000 pyzstd-0.15.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-04-05 05:28:47.000000 pyzstd-0.15.6/src/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-04-05 05:28:47.000000 pyzstd-0.15.6/src/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.686915 pyzstd-0.15.6/src/bin_ext/
--rw-r--r--   0 runner    (1001) docker     (123)   124577 2023-04-05 05:28:47.000000 pyzstd-0.15.6/src/bin_ext/_zstdmodule.c
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-05 05:28:47.000000 pyzstd-0.15.6/src/bin_ext/build_cffi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.686915 pyzstd-0.15.6/src/c/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-05 05:28:47.000000 pyzstd-0.15.6/src/c/c_pyzstd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.686915 pyzstd-0.15.6/src/cffi/
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-05 05:28:47.000000 pyzstd-0.15.6/src/cffi/cffi_pyzstd.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:47.000000 pyzstd-0.15.6/src/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.686915 pyzstd-0.15.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:47.000000 pyzstd-0.15.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   208121 2023-04-05 05:28:47.000000 pyzstd-0.15.6/tests/test_zstd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.682915 pyzstd-0.15.6/zstd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.690914 pyzstd-0.15.6/zstd/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/BUCK
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.690914 pyzstd-0.15.6/zstd/lib/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/allocations.h
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/bits.h
--rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/debug.c
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/error_private.c
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/error_private.h
--rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/fse.h
--rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/huf.h
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/mem.h
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/pool.c
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/portability_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/threading.c
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/threading.h
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)   212896 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/zstd_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/zstd_deps.h
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/zstd_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/common/zstd_trace.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.694915 pyzstd-0.15.6/zstd/lib/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/clevels.h
--rw-r--r--   0 runner    (1001) docker     (123)    24096 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/hist.c
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/hist.h
--rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)   312776 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    64416 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_compress_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_compress_literals.c
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_compress_literals.h
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_compress_sequences.c
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_compress_sequences.h
--rw-r--r--   0 runner    (1001) docker     (123)    28499 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_compress_superblock.c
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_compress_superblock.h
--rw-r--r--   0 runner    (1001) docker     (123)    27872 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_cwksp.h
--rw-r--r--   0 runner    (1001) docker     (123)    34479 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_double_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_double_fast.h
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_fast.h
--rw-r--r--   0 runner    (1001) docker     (123)   101952 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_lazy.c
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_lazy.h
--rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_ldm.c
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_ldm.h
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_ldm_geartab.h
--rw-r--r--   0 runner    (1001) docker     (123)    67459 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_opt.c
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstd_opt.h
--rw-r--r--   0 runner    (1001) docker     (123)    81334 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstdmt_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/compress/zstdmt_compress.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.698915 pyzstd-0.15.6/zstd/lib/decompress/
--rw-r--r--   0 runner    (1001) docker     (123)    73701 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/decompress/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/decompress/huf_decompress_amd64.S
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/decompress/zstd_ddict.c
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/decompress/zstd_ddict.h
--rw-r--r--   0 runner    (1001) docker     (123)    99701 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/decompress/zstd_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    99641 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/decompress/zstd_decompress_block.c
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/decompress/zstd_decompress_block.h
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/decompress/zstd_decompress_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.698915 pyzstd-0.15.6/zstd/lib/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/deprecated/zbuff.h
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/deprecated/zbuff_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/deprecated/zbuff_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/deprecated/zbuff_decompress.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.698915 pyzstd-0.15.6/zstd/lib/dictBuilder/
--rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dictBuilder/cover.c
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dictBuilder/cover.h
--rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dictBuilder/divsufsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dictBuilder/divsufsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    28561 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dictBuilder/fastcover.c
--rw-r--r--   0 runner    (1001) docker     (123)    44008 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dictBuilder/zdict.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.686915 pyzstd-0.15.6/zstd/lib/dll/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.698915 pyzstd-0.15.6/zstd/lib/dll/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dll/example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dll/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dll/example/build_package.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dll/example/fullbench-dll.sln
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/dll/example/fullbench-dll.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:28:58.702915 pyzstd-0.15.6/zstd/lib/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_legacy.h
--rw-r--r--   0 runner    (1001) docker     (123)    69465 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v01.c
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v01.h
--rw-r--r--   0 runner    (1001) docker     (123)   125639 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v02.c
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v02.h
--rw-r--r--   0 runner    (1001) docker     (123)   111749 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v03.c
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v03.h
--rw-r--r--   0 runner    (1001) docker     (123)   132791 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v04.c
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v04.h
--rw-r--r--   0 runner    (1001) docker     (123)   153658 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v05.c
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v05.h
--rw-r--r--   0 runner    (1001) docker     (123)   163699 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v06.c
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v06.h
--rw-r--r--   0 runner    (1001) docker     (123)   182559 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v07.c
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/legacy/zstd_v07.h
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/libzstd.mk
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/libzstd.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/module.modulemap
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/zdict.h
--rw-r--r--   0 runner    (1001) docker     (123)   171378 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/zstd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-05 05:28:49.000000 pyzstd-0.15.6/zstd/lib/zstd_errors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.536491 pyzstd-0.15.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-21 12:31:05.000000 pyzstd-0.15.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 12:31:05.000000 pyzstd-0.15.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-21 12:31:15.536491 pyzstd-0.15.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-21 12:31:05.000000 pyzstd-0.15.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-04-21 12:31:05.000000 pyzstd-0.15.7/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-21 12:31:05.000000 pyzstd-0.15.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/pyzstd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-21 12:31:15.000000 pyzstd-0.15.7/pyzstd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-21 12:31:15.000000 pyzstd-0.15.7/pyzstd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:31:15.000000 pyzstd-0.15.7/pyzstd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 12:31:15.000000 pyzstd-0.15.7/pyzstd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:31:15.536491 pyzstd-0.15.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-04-21 12:31:05.000000 pyzstd-0.15.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    25771 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/src/bin_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)   130735 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/bin_ext/_zstdmodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/bin_ext/build_cffi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/src/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/c/c_pyzstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/src/cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)    70341 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/cffi/cffi_pyzstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:05.000000 pyzstd-0.15.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   217042 2023-04-21 12:31:05.000000 pyzstd-0.15.7/tests/test_zstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.516491 pyzstd-0.15.7/zstd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.524491 pyzstd-0.15.7/zstd/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/BUCK
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.524491 pyzstd-0.15.7/zstd/lib/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/allocations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/bits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/debug.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/error_private.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/fse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/huf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/pool.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/portability_macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/threading.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/threading.h
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)   212896 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/zstd_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/zstd_deps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/zstd_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/zstd_trace.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/clevels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24096 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/hist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/hist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)   312776 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    64416 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_literals.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_literals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_sequences.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_sequences.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28499 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_superblock.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_superblock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27872 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_cwksp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34479 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_double_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_double_fast.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_fast.h
+-rw-r--r--   0 runner    (1001) docker     (123)   101952 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_lazy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_lazy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_ldm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_ldm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_ldm_geartab.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67459 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_opt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_opt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    81334 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstdmt_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstdmt_compress.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/decompress/
+-rw-r--r--   0 runner    (1001) docker     (123)    73701 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/huf_decompress_amd64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_ddict.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_ddict.h
+-rw-r--r--   0 runner    (1001) docker     (123)    99701 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    99641 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_block.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/deprecated/zbuff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/deprecated/zbuff_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/deprecated/zbuff_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/deprecated/zbuff_decompress.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/dictBuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/cover.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/cover.h
+-rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/divsufsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/divsufsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28561 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/fastcover.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44008 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/zdict.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.516491 pyzstd-0.15.7/zstd/lib/dll/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/dll/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/build_package.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/fullbench-dll.sln
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/fullbench-dll.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.536491 pyzstd-0.15.7/zstd/lib/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_legacy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69465 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v01.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v01.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125639 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v02.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v02.h
+-rw-r--r--   0 runner    (1001) docker     (123)   111749 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v03.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v03.h
+-rw-r--r--   0 runner    (1001) docker     (123)   132791 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v04.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v04.h
+-rw-r--r--   0 runner    (1001) docker     (123)   153658 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v05.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v05.h
+-rw-r--r--   0 runner    (1001) docker     (123)   163699 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v06.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v06.h
+-rw-r--r--   0 runner    (1001) docker     (123)   182559 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v07.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v07.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/libzstd.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/libzstd.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/module.modulemap
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/zdict.h
+-rw-r--r--   0 runner    (1001) docker     (123)   171378 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/zstd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/zstd_errors.h
```

### Comparing `pyzstd-0.15.6/LICENSE` & `pyzstd-0.15.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/PKG-INFO` & `pyzstd-0.15.7/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: pyzstd
-Version: 0.15.6
-Summary: Python bindings to Zstandard (zstd) compression library, the API style is similar to Python's bz2/lzma/zlib modules.
-Home-page: https://github.com/animalize/pyzstd
-Author: Ma Lin
-Author-email: malincns@163.com
-License: The 3-Clause BSD License
-Keywords: zstandard zstd compression decompression compress decompress
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: System :: Archiving :: Compression
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.5
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Introduction
 ------------
 
 Pyzstd module provides classes and functions for compressing and decompressing data, using Facebook's `Zstandard <http://www.zstd.net>`_ (or zstd as short name) algorithm.
 
 The API style is similar to Python's bz2/lzma/zlib modules.
 
@@ -41,77 +17,87 @@
 Documentation: https://pyzstd.readthedocs.io/en/latest
 
 GitHub: https://github.com/animalize/pyzstd
 
 
 Release note
 ------------
+**0.15.7  (Apr 21, 2023)**
+
+ZstdDict class changes:
+
+#. Fix these advanced compression parameters may be ignored when loading a dictionary: ``windowLog``, ``hashLog``, ``chainLog``, ``searchLog``, ``minMatch``, ``targetLength``, ``strategy``, ``enableLongDistanceMatching``, ``ldmHashLog``, ``ldmMinMatch``, ``ldmBucketSizeLog``, ``ldmHashRateLog``, and some non-public parameters.
+
+#. When compressing, load undigested dictionary instead of digested dictionary by default. Loading again an undigested is slower, see `differences <https://pyzstd.readthedocs.io/en/latest/#ZstdDict.as_digested_dict>`_.
+
+#. Add `.as_prefix <https://pyzstd.readthedocs.io/en/latest/#ZstdDict.as_prefix>`_ attribute. Can use zstd as a `patching engine <https://pyzstd.readthedocs.io/en/latest/#patching-engine>`_.
+
 **0.15.6  (Apr 5, 2023)**
 
-Update bundled zstd source code from v1.5.4 to `v1.5.5 <https://github.com/facebook/zstd/releases/tag/v1.5.5>`_.
+Upgrade zstd source code from v1.5.4 to `v1.5.5 <https://github.com/facebook/zstd/releases/tag/v1.5.5>`_.
 
 **0.15.4  (Feb 24, 2023)**
 
-#. Update bundled zstd source code from v1.5.2 to `v1.5.4 <https://github.com/facebook/zstd/releases/tag/v1.5.4>`_. v1.5.3 is a non-public release.
+#. Upgrade zstd source code from v1.5.2 to `v1.5.4 <https://github.com/facebook/zstd/releases/tag/v1.5.4>`_. v1.5.3 is a non-public release.
 
-#. Support ``pyproject.toml`` build mechanism (PEP-517). Note that specifying build options in old way may be invalid, see `doc <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
+#. Support ``pyproject.toml`` build mechanism (PEP-517). Note that specifying build options in old way may be invalid, see `build commands <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
 
 #. Support "multi-phase initialization" (PEP-489) on CPython 3.11+, can work with CPython sub-interpreters in the future. Currently this build option is disabled by default.
 
 #. Add a command line interface (CLI).
 
 **0.15.3  (Aug 3, 2022)**
 
 Fix ``ZstdError`` object can't be pickled.
 
 **0.15.2  (Jan 22, 2022)**
 
-Update bundled zstd source code from v1.5.1 to `v1.5.2 <https://github.com/facebook/zstd/releases/tag/v1.5.2>`_.
+Upgrade zstd source code from v1.5.1 to `v1.5.2 <https://github.com/facebook/zstd/releases/tag/v1.5.2>`_.
 
 **0.15.1  (Dec 25, 2021)**
 
-#. Update bundled zstd source code from v1.5.0 to `v1.5.1 <https://github.com/facebook/zstd/releases/tag/v1.5.1>`_.
+#. Upgrade zstd source code from v1.5.0 to `v1.5.1 <https://github.com/facebook/zstd/releases/tag/v1.5.1>`_.
 
 #. Fix ``ZstdFile.write()`` / ``train_dict()`` / ``finalize_dict()`` may use wrong length for some buffer protocol objects, see `this issue <https://github.com/animalize/pyzstd/issues/4>`_.
 
 #. Two behavior changes:
 
     * Setting ``CParameter.nbWorkers`` to ``1`` now means "1-thread multi-threaded mode", rather than "single-threaded mode".
 
     * If the underlying zstd library doesn't support multi-threaded compression, no longer automatically fallback to "single-threaded mode", now raise a ``ZstdError`` exception.
 
 #. Add a module level variable `zstd_support_multithread <https://pyzstd.readthedocs.io/en/latest/#zstd_support_multithread>`_.
 
-#. Add a setup.py option ``--avx2``, see `this note <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
+#. Add a setup.py option ``--avx2``, see `build options <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
 
 **0.15.0  (May 18, 2021)**
 
-#. Update bundled zstd source code from v1.4.9 to `v1.5.0 <https://github.com/facebook/zstd/releases/tag/v1.5.0>`_.
+#. Upgrade zstd source code from v1.4.9 to `v1.5.0 <https://github.com/facebook/zstd/releases/tag/v1.5.0>`_.
 
 #. Some improvements, no API changes.
 
 **0.14.4  (Mar 24, 2021)**
 
 #. Add a CFFI implementation that can work with PyPy.
 
 #. Allow dynamically link to zstd library.
 
 **0.14.3  (Mar 4, 2021)**
 
-Update bundled zstd source code from v1.4.8 to `v1.4.9 <https://github.com/facebook/zstd/releases/tag/v1.4.9>`_.
+Upgrade zstd source code from v1.4.8 to `v1.4.9 <https://github.com/facebook/zstd/releases/tag/v1.4.9>`_.
 
 **0.14.2  (Feb 24, 2021)**
 
 #. Add two convenient functions: `compress_stream() <https://pyzstd.readthedocs.io/en/latest/#compress_stream>`_, `decompress_stream() <https://pyzstd.readthedocs.io/en/latest/#decompress_stream>`_.
 
 #. Some improvements.
 
 **0.14.1  (Dec 19, 2020)**
 
-#. Update bundled zstd source code from v1.4.5 to `v1.4.8 <https://github.com/facebook/zstd/releases/tag/v1.4.8>`_.
+#. Upgrade zstd source code from v1.4.5 to `v1.4.8 <https://github.com/facebook/zstd/releases/tag/v1.4.8>`_.
 
     * v1.4.6 is a non-public release for Linux kernel.
 
     * v1.4.8 is a hotfix for `v1.4.7 <https://github.com/facebook/zstd/releases/tag/v1.4.7>`_.
 
 #. Some improvements, no API changes.
 
@@ -137,8 +123,8 @@
 
 It seems the API is stable.
 
 **0.2.4  (Sep 2, 2020)**
 
 The first version upload to PyPI.
 
-Includes zstd `v1.4.5 <https://github.com/facebook/zstd/releases/tag/v1.4.5>`_ source code.
+Includes zstd `v1.4.5 <https://github.com/facebook/zstd/releases/tag/v1.4.5>`_ source code.
```

### Comparing `pyzstd-0.15.6/index.rst` & `pyzstd-0.15.7/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,4407 +28,4800 @@
 000001b0: 2e0a 2a20 4861 7320 6120 4346 4649 2069  ..* Has a CFFI i
 000001c0: 6d70 6c65 6d65 6e74 6174 696f 6e20 7468  mplementation th
 000001d0: 6174 2063 616e 2077 6f72 6b20 7769 7468  at can work with
 000001e0: 2050 7950 792e 0a2a 2048 6173 2061 2063   PyPy..* Has a c
 000001f0: 6f6d 6d61 6e64 206c 696e 6520 696e 7465  ommand line inte
 00000200: 7266 6163 652c 2060 6070 7974 686f 6e20  rface, ``python 
 00000210: 2d6d 2070 797a 7374 6420 2d2d 6865 6c70  -m pyzstd --help
-00000220: 6060 2e20 282a 4164 6465 6420 696e 2076  ``. (*Added in v
-00000230: 6572 7369 6f6e 2030 2e31 352e 342a 290a  ersion 0.15.4*).
-00000240: 0a4c 696e 6b73 3a20 6047 6974 4875 6220  .Links: `GitHub 
-00000250: 7061 6765 203c 6874 7470 733a 2f2f 6769  page <https://gi
-00000260: 7468 7562 2e63 6f6d 2f61 6e69 6d61 6c69  thub.com/animali
-00000270: 7a65 2f70 797a 7374 643e 605f 2c20 6050  ze/pyzstd>`_, `P
-00000280: 7950 4920 7061 6765 203c 6874 7470 733a  yPI page <https:
-00000290: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000002a0: 6374 2f70 797a 7374 643e 605f 2e0a 0a46  ct/pyzstd>`_...F
-000002b0: 6561 7475 7265 7320 6f66 207a 7374 643a  eatures of zstd:
-000002c0: 0a0a 2a20 4661 7374 2063 6f6d 7072 6573  ..* Fast compres
-000002d0: 7369 6f6e 2061 6e64 2064 6563 6f6d 7072  sion and decompr
-000002e0: 6573 7369 6f6e 2073 7065 6564 2e0a 2a20  ession speed..* 
-000002f0: 4966 2075 7365 203a 7265 663a 606d 756c  If use :ref:`mul
-00000300: 7469 2d74 6872 6561 6465 6420 636f 6d70  ti-threaded comp
-00000310: 7265 7373 696f 6e3c 6d74 5f63 6f6d 7072  ression<mt_compr
-00000320: 6573 7369 6f6e 3e60 2c20 7468 6520 636f  ession>`, the co
-00000330: 6d70 7265 7373 696f 6e20 7370 6565 6420  mpression speed 
-00000340: 696d 7072 6f76 6573 2073 6967 6e69 6669  improves signifi
-00000350: 6361 6e74 6c79 2e0a 2a20 4966 2075 7365  cantly..* If use
-00000360: 2070 7265 2d74 7261 696e 6564 203a 7265   pre-trained :re
-00000370: 663a 6064 6963 7469 6f6e 6172 793c 7a73  f:`dictionary<zs
-00000380: 7464 5f64 6963 743e 602c 2074 6865 2063  td_dict>`, the c
-00000390: 6f6d 7072 6573 7369 6f6e 2072 6174 696f  ompression ratio
-000003a0: 206f 6e20 736d 616c 6c20 6461 7461 2028   on small data (
-000003b0: 6120 6665 7720 4b69 4229 2069 6d70 726f  a few KiB) impro
-000003c0: 7665 7320 6472 616d 6174 6963 616c 6c79  ves dramatically
-000003d0: 2e0a 2a20 3a72 6566 3a60 4672 616d 6520  ..* :ref:`Frame 
-000003e0: 616e 6420 626c 6f63 6b3c 6672 616d 655f  and block<frame_
-000003f0: 626c 6f63 6b3e 6020 616c 6c6f 7720 7468  block>` allow th
-00000400: 6520 7573 6520 6d6f 7265 2066 6c65 7869  e use more flexi
-00000410: 626c 652c 2073 7569 7461 626c 6520 666f  ble, suitable fo
-00000420: 7220 6d61 6e79 2073 6365 6e61 7269 6f73  r many scenarios
-00000430: 2e0a 0a2e 2e20 6e6f 7465 3a3a 0a20 2020  ..... note::.   
-00000440: 2054 776f 206f 7468 6572 207a 7374 6420   Two other zstd 
-00000450: 6d6f 6475 6c65 7320 6f6e 2050 7950 493a  modules on PyPI:
-00000460: 0a0a 2020 2020 2a20 607a 7374 6420 3c68  ..    * `zstd <h
-00000470: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000480: 7072 6f6a 6563 742f 7a73 7464 2f3e 605f  project/zstd/>`_
-00000490: 2c20 6120 7665 7279 2073 696d 706c 6520  , a very simple 
-000004a0: 6d6f 6475 6c65 2e0a 2020 2020 2a20 607a  module..    * `z
-000004b0: 7374 616e 6461 7264 203c 6874 7470 733a  standard <https:
-000004c0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000004d0: 6374 2f7a 7374 616e 6461 7264 2f3e 605f  ct/zstandard/>`_
-000004e0: 2c20 7072 6f76 6964 6573 2072 6963 6820  , provides rich 
-000004f0: 4150 492e 0a0a 4578 6365 7074 696f 6e0a  API...Exception.
-00000500: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 7079  ---------.... py
-00000510: 3a65 7863 6570 7469 6f6e 3a3a 205a 7374  :exception:: Zst
-00000520: 6445 7272 6f72 0a0a 2020 2020 5468 6973  dError..    This
-00000530: 2065 7863 6570 7469 6f6e 2069 7320 7261   exception is ra
-00000540: 6973 6564 2077 6865 6e20 616e 2065 7272  ised when an err
-00000550: 6f72 206f 6363 7572 7320 7768 656e 2063  or occurs when c
-00000560: 616c 6c69 6e67 2074 6865 2075 6e64 6572  alling the under
-00000570: 6c79 696e 6720 7a73 7464 206c 6962 7261  lying zstd libra
-00000580: 7279 2e0a 0a0a 5369 6d70 6c65 2063 6f6d  ry....Simple com
-00000590: 7072 6573 7369 6f6e 2f64 6563 6f6d 7072  pression/decompr
-000005a0: 6573 7369 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d  ession.---------
-000005b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005c0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2054 6869  -------..    Thi
-000005d0: 7320 7365 6374 696f 6e20 636f 6e74 6169  s section contai
-000005e0: 6e73 3a0a 0a20 2020 2020 2020 202a 2066  ns:..        * f
-000005f0: 756e 6374 696f 6e20 3a70 793a 6675 6e63  unction :py:func
-00000600: 3a60 636f 6d70 7265 7373 600a 2020 2020  :`compress`.    
-00000610: 2020 2020 2a20 6675 6e63 7469 6f6e 203a      * function :
-00000620: 7079 3a66 756e 633a 6064 6563 6f6d 7072  py:func:`decompr
-00000630: 6573 7360 0a0a 2020 2020 2e2e 2068 696e  ess`..    .. hin
-00000640: 743a 3a0a 2020 2020 2020 2020 4966 2074  t::.        If t
-00000650: 6865 7265 2061 7265 2061 2062 6967 206e  here are a big n
-00000660: 756d 6265 7220 6f66 2073 616d 6520 7479  umber of same ty
-00000670: 7065 2069 6e64 6976 6964 7561 6c20 6461  pe individual da
-00000680: 7461 2c20 7265 7573 6520 7468 6573 6520  ta, reuse these 
-00000690: 6f62 6a65 6374 7320 6d61 7920 656c 696d  objects may elim
-000006a0: 696e 6174 6520 7468 6520 736d 616c 6c20  inate the small 
-000006b0: 6f76 6572 6865 6164 206f 6620 6372 6561  overhead of crea
-000006c0: 7469 6e67 2063 6f6e 7465 7874 202f 2073  ting context / s
-000006d0: 6574 7469 6e67 2070 6172 616d 6574 6572  etting parameter
-000006e0: 7320 2f20 6c6f 6164 696e 6720 6469 6374  s / loading dict
-000006f0: 696f 6e61 7279 2e0a 0a20 2020 2020 2020  ionary...       
-00000700: 202a 203a 7079 3a63 6c61 7373 3a60 5a73   * :py:class:`Zs
-00000710: 7464 436f 6d70 7265 7373 6f72 600a 2020  tdCompressor`.  
-00000720: 2020 2020 2020 2a20 3a70 793a 636c 6173        * :py:clas
-00000730: 733a 6052 6963 684d 656d 5a73 7464 436f  s:`RichMemZstdCo
-00000740: 6d70 7265 7373 6f72 600a 0a0a 2e2e 2070  mpressor`..... p
-00000750: 793a 6675 6e63 7469 6f6e 3a3a 2063 6f6d  y:function:: com
-00000760: 7072 6573 7328 6461 7461 2c20 6c65 7665  press(data, leve
-00000770: 6c5f 6f72 5f6f 7074 696f 6e3d 4e6f 6e65  l_or_option=None
-00000780: 2c20 7a73 7464 5f64 6963 743d 4e6f 6e65  , zstd_dict=None
-00000790: 290a 0a20 2020 2043 6f6d 7072 6573 7320  )..    Compress 
-000007a0: 2a64 6174 612a 2c20 7265 7475 726e 2074  *data*, return t
-000007b0: 6865 2063 6f6d 7072 6573 7365 6420 6461  he compressed da
-000007c0: 7461 2e0a 0a20 2020 2043 6f6d 7072 6573  ta...    Compres
-000007d0: 7369 6e67 2060 6062 2727 6060 2077 696c  sing ``b''`` wil
-000007e0: 6c20 6765 7420 616e 2065 6d70 7479 2063  l get an empty c
-000007f0: 6f6e 7465 6e74 2066 7261 6d65 2028 3920  ontent frame (9 
-00000800: 6279 7465 7320 6f72 206d 6f72 6529 2e0a  bytes or more)..
-00000810: 0a20 2020 203a 7079 3a66 756e 633a 6072  .    :py:func:`r
-00000820: 6963 686d 656d 5f63 6f6d 7072 6573 7360  ichmem_compress`
-00000830: 2066 756e 6374 696f 6e20 6973 2066 6173   function is fas
-00000840: 7465 7220 696e 2073 6f6d 6520 6361 7365  ter in some case
-00000850: 732e 0a0a 2020 2020 3a70 6172 616d 2064  s...    :param d
-00000860: 6174 613a 2044 6174 6120 746f 2062 6520  ata: Data to be 
-00000870: 636f 6d70 7265 7373 6564 2e0a 2020 2020  compressed..    
-00000880: 3a74 7970 6520 6461 7461 3a20 6279 7465  :type data: byte
-00000890: 732d 6c69 6b65 206f 626a 6563 740a 2020  s-like object.  
-000008a0: 2020 3a70 6172 616d 206c 6576 656c 5f6f    :param level_o
-000008b0: 725f 6f70 7469 6f6e 3a20 5768 656e 2069  r_option: When i
-000008c0: 7427 7320 616e 2060 6069 6e74 6060 206f  t's an ``int`` o
-000008d0: 626a 6563 742c 2069 7420 7265 7072 6573  bject, it repres
-000008e0: 656e 7473 203a 7265 663a 6063 6f6d 7072  ents :ref:`compr
-000008f0: 6573 7369 6f6e 206c 6576 656c 3c63 6f6d  ession level<com
-00000900: 7072 6573 7369 6f6e 5f6c 6576 656c 3e60  pression_level>`
-00000910: 2e20 5768 656e 2069 7427 7320 6120 6060  . When it's a ``
-00000920: 6469 6374 6060 206f 626a 6563 742c 2069  dict`` object, i
-00000930: 7420 636f 6e74 6169 6e73 203a 7265 663a  t contains :ref:
-00000940: 6061 6476 616e 6365 6420 636f 6d70 7265  `advanced compre
-00000950: 7373 696f 6e20 7061 7261 6d65 7465 7273  ssion parameters
-00000960: 3c43 5061 7261 6d65 7465 723e 602e 2054  <CParameter>`. T
-00000970: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
-00000980: 2060 604e 6f6e 6560 6020 6d65 616e 7320   ``None`` means 
-00000990: 746f 2075 7365 207a 7374 6427 7320 6465  to use zstd's de
-000009a0: 6661 756c 7420 636f 6d70 7265 7373 696f  fault compressio
-000009b0: 6e20 6c65 7665 6c2f 7061 7261 6d65 7465  n level/paramete
-000009c0: 7273 2e0a 2020 2020 3a74 7970 6520 6c65  rs..    :type le
-000009d0: 7665 6c5f 6f72 5f6f 7074 696f 6e3a 2069  vel_or_option: i
-000009e0: 6e74 206f 7220 6469 6374 0a20 2020 203a  nt or dict.    :
-000009f0: 7061 7261 6d20 7a73 7464 5f64 6963 743a  param zstd_dict:
-00000a00: 2050 7265 2d74 7261 696e 6564 2064 6963   Pre-trained dic
-00000a10: 7469 6f6e 6172 7920 666f 7220 636f 6d70  tionary for comp
-00000a20: 7265 7373 696f 6e2e 0a20 2020 203a 7479  ression..    :ty
-00000a30: 7065 207a 7374 645f 6469 6374 3a20 5a73  pe zstd_dict: Zs
-00000a40: 7464 4469 6374 0a20 2020 203a 7265 7475  tdDict.    :retu
-00000a50: 726e 3a20 436f 6d70 7265 7373 6564 2064  rn: Compressed d
-00000a60: 6174 610a 2020 2020 3a72 7479 7065 3a20  ata.    :rtype: 
-00000a70: 6279 7465 730a 0a2e 2e20 736f 7572 6365  bytes.... source
-00000a80: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-00000a90: 2020 2023 2069 6e74 2063 6f6d 7072 6573     # int compres
-00000aa0: 7369 6f6e 206c 6576 656c 0a20 2020 2063  sion level.    c
-00000ab0: 6f6d 7072 6573 7365 645f 6461 7420 3d20  ompressed_dat = 
-00000ac0: 636f 6d70 7265 7373 2872 6177 5f64 6174  compress(raw_dat
-00000ad0: 2c20 3130 290a 0a20 2020 2023 2064 6963  , 10)..    # dic
-00000ae0: 7420 6f70 7469 6f6e 2c20 7573 6520 3620  t option, use 6 
-00000af0: 7468 7265 6164 7320 746f 2063 6f6d 7072  threads to compr
-00000b00: 6573 732c 2061 6e64 2061 7070 656e 6420  ess, and append 
-00000b10: 6120 342d 6279 7465 2063 6865 636b 7375  a 4-byte checksu
-00000b20: 6d2e 0a20 2020 206f 7074 696f 6e20 3d20  m..    option = 
-00000b30: 7b43 5061 7261 6d65 7465 722e 636f 6d70  {CParameter.comp
-00000b40: 7265 7373 696f 6e4c 6576 656c 203a 2031  ressionLevel : 1
-00000b50: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00000b60: 2043 5061 7261 6d65 7465 722e 6e62 576f   CParameter.nbWo
-00000b70: 726b 6572 7320 3a20 362c 0a20 2020 2020  rkers : 6,.     
-00000b80: 2020 2020 2020 2020 2043 5061 7261 6d65           CParame
-00000b90: 7465 722e 6368 6563 6b73 756d 466c 6167  ter.checksumFlag
-00000ba0: 203a 2031 7d0a 2020 2020 636f 6d70 7265   : 1}.    compre
-00000bb0: 7373 6564 5f64 6174 203d 2063 6f6d 7072  ssed_dat = compr
-00000bc0: 6573 7328 7261 775f 6461 742c 206f 7074  ess(raw_dat, opt
-00000bd0: 696f 6e29 0a0a 0a2e 2e20 7079 3a66 756e  ion)..... py:fun
-00000be0: 6374 696f 6e3a 3a20 6465 636f 6d70 7265  ction:: decompre
-00000bf0: 7373 2864 6174 612c 207a 7374 645f 6469  ss(data, zstd_di
-00000c00: 6374 3d4e 6f6e 652c 206f 7074 696f 6e3d  ct=None, option=
-00000c10: 4e6f 6e65 290a 0a20 2020 2044 6563 6f6d  None)..    Decom
-00000c20: 7072 6573 7320 2a64 6174 612a 2c20 7265  press *data*, re
-00000c30: 7475 726e 2074 6865 2064 6563 6f6d 7072  turn the decompr
-00000c40: 6573 7365 6420 6461 7461 2e0a 0a20 2020  essed data...   
-00000c50: 2053 7570 706f 7274 206d 756c 7469 706c   Support multipl
-00000c60: 6520 636f 6e63 6174 656e 6174 6564 203a  e concatenated :
-00000c70: 7265 663a 6066 7261 6d65 733c 6672 616d  ref:`frames<fram
-00000c80: 655f 626c 6f63 6b3e 602e 0a0a 2020 2020  e_block>`...    
-00000c90: 3a70 6172 616d 2064 6174 613a 2044 6174  :param data: Dat
-00000ca0: 6120 746f 2062 6520 6465 636f 6d70 7265  a to be decompre
-00000cb0: 7373 6564 2e0a 2020 2020 3a74 7970 6520  ssed..    :type 
-00000cc0: 6461 7461 3a20 6279 7465 732d 6c69 6b65  data: bytes-like
-00000cd0: 206f 626a 6563 740a 2020 2020 3a70 6172   object.    :par
-00000ce0: 616d 207a 7374 645f 6469 6374 3a20 5072  am zstd_dict: Pr
-00000cf0: 652d 7472 6169 6e65 6420 6469 6374 696f  e-trained dictio
-00000d00: 6e61 7279 2066 6f72 2064 6563 6f6d 7072  nary for decompr
-00000d10: 6573 7369 6f6e 2e0a 2020 2020 3a74 7970  ession..    :typ
-00000d20: 6520 7a73 7464 5f64 6963 743a 205a 7374  e zstd_dict: Zst
-00000d30: 6444 6963 740a 2020 2020 3a70 6172 616d  dDict.    :param
-00000d40: 206f 7074 696f 6e3a 2041 2060 6064 6963   option: A ``dic
-00000d50: 7460 6020 6f62 6a65 6374 2074 6861 7420  t`` object that 
-00000d60: 636f 6e74 6169 6e73 203a 7079 3a72 6566  contains :py:ref
-00000d70: 3a60 6164 7661 6e63 6564 2064 6563 6f6d  :`advanced decom
-00000d80: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
-00000d90: 6572 733c 4450 6172 616d 6574 6572 3e60  ers<DParameter>`
-00000da0: 2e20 5468 6520 6465 6661 756c 7420 7661  . The default va
-00000db0: 6c75 6520 6060 4e6f 6e65 6060 206d 6561  lue ``None`` mea
-00000dc0: 6e73 2074 6f20 7573 6520 7a73 7464 2773  ns to use zstd's
-00000dd0: 2064 6566 6175 6c74 2064 6563 6f6d 7072   default decompr
-00000de0: 6573 7369 6f6e 2070 6172 616d 6574 6572  ession parameter
-00000df0: 732e 0a20 2020 203a 7479 7065 206f 7074  s..    :type opt
-00000e00: 696f 6e3a 2064 6963 740a 2020 2020 3a72  ion: dict.    :r
-00000e10: 6574 7572 6e3a 2044 6563 6f6d 7072 6573  eturn: Decompres
-00000e20: 7365 6420 6461 7461 0a20 2020 203a 7274  sed data.    :rt
-00000e30: 7970 653a 2062 7974 6573 0a20 2020 203a  ype: bytes.    :
-00000e40: 7261 6973 6573 205a 7374 6445 7272 6f72  raises ZstdError
-00000e50: 3a20 4966 2064 6563 6f6d 7072 6573 7369  : If decompressi
-00000e60: 6f6e 2066 6169 6c73 2e0a 0a0a 5269 6368  on fails....Rich
-00000e70: 206d 656d 6f72 7920 636f 6d70 7265 7373   memory compress
-00000e80: 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ion.------------
-00000e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020  -----------..   
-00000ea0: 2043 6f6d 7072 6573 7320 6461 7461 2075   Compress data u
-00000eb0: 7369 6e67 203a 7265 663a 6072 6963 6820  sing :ref:`rich 
-00000ec0: 6d65 6d6f 7279 206d 6f64 653c 7269 6368  memory mode<rich
-00000ed0: 5f6d 656d 3e60 2e20 5468 6973 206d 6f64  _mem>`. This mod
-00000ee0: 6520 616c 6c6f 6361 7465 7320 6d6f 7265  e allocates more
-00000ef0: 206d 656d 6f72 7920 666f 7220 6f75 7470   memory for outp
-00000f00: 7574 2062 7566 6665 722c 2069 7427 7320  ut buffer, it's 
-00000f10: 6661 7374 6572 2069 6e20 736f 6d65 2063  faster in some c
-00000f20: 6173 6573 2e0a 0a20 2020 2054 6869 7320  ases...    This 
-00000f30: 7365 6374 696f 6e20 636f 6e74 6169 6e73  section contains
-00000f40: 3a0a 0a20 2020 2020 2020 202a 2066 756e  :..        * fun
-00000f50: 6374 696f 6e20 3a70 793a 6675 6e63 3a60  ction :py:func:`
-00000f60: 7269 6368 6d65 6d5f 636f 6d70 7265 7373  richmem_compress
-00000f70: 600a 2020 2020 2020 2020 2a20 636c 6173  `.        * clas
-00000f80: 7320 3a70 793a 636c 6173 733a 6052 6963  s :py:class:`Ric
-00000f90: 684d 656d 5a73 7464 436f 6d70 7265 7373  hMemZstdCompress
-00000fa0: 6f72 602c 2061 2072 6575 7361 626c 6520  or`, a reusable 
-00000fb0: 636f 6d70 7265 7373 6f72 2e0a 0a2e 2e20  compressor..... 
-00000fc0: 7079 3a66 756e 6374 696f 6e3a 3a20 7269  py:function:: ri
-00000fd0: 6368 6d65 6d5f 636f 6d70 7265 7373 2864  chmem_compress(d
-00000fe0: 6174 612c 206c 6576 656c 5f6f 725f 6f70  ata, level_or_op
-00000ff0: 7469 6f6e 3d4e 6f6e 652c 207a 7374 645f  tion=None, zstd_
-00001000: 6469 6374 3d4e 6f6e 6529 0a0a 2020 2020  dict=None)..    
-00001010: 5573 6520 3a72 6566 3a60 7269 6368 206d  Use :ref:`rich m
-00001020: 656d 6f72 7920 6d6f 6465 3c72 6963 685f  emory mode<rich_
-00001030: 6d65 6d3e 6020 746f 2063 6f6d 7072 6573  mem>` to compres
-00001040: 7320 2a64 6174 612a 2e20 4974 2773 2066  s *data*. It's f
-00001050: 6173 7465 7220 7468 616e 203a 7079 3a66  aster than :py:f
-00001060: 756e 633a 6063 6f6d 7072 6573 7360 2069  unc:`compress` i
-00001070: 6e20 736f 6d65 2063 6173 6573 2c20 6275  n some cases, bu
-00001080: 7420 616c 6c6f 6361 7465 7320 6d6f 7265  t allocates more
-00001090: 206d 656d 6f72 792e 0a0a 2020 2020 5468   memory...    Th
-000010a0: 6520 7061 7261 6d65 7465 7273 2061 7265  e parameters are
-000010b0: 2074 6865 2073 616d 6520 6173 203a 7079   the same as :py
-000010c0: 3a66 756e 633a 6063 6f6d 7072 6573 7360  :func:`compress`
-000010d0: 2066 756e 6374 696f 6e2e 0a0a 2020 2020   function...    
-000010e0: 436f 6d70 7265 7373 696e 6720 6060 6227  Compressing ``b'
-000010f0: 2760 6020 7769 6c6c 2067 6574 2061 6e20  '`` will get an 
-00001100: 656d 7074 7920 636f 6e74 656e 7420 6672  empty content fr
-00001110: 616d 6520 2839 2062 7974 6573 206f 7220  ame (9 bytes or 
-00001120: 6d6f 7265 292e 0a0a 0a2e 2e20 7079 3a63  more)...... py:c
-00001130: 6c61 7373 3a3a 2052 6963 684d 656d 5a73  lass:: RichMemZs
-00001140: 7464 436f 6d70 7265 7373 6f72 0a0a 2020  tdCompressor..  
-00001150: 2020 4120 7265 7573 6162 6c65 2063 6f6d    A reusable com
-00001160: 7072 6573 736f 7220 7573 696e 6720 3a72  pressor using :r
-00001170: 6566 3a60 7269 6368 206d 656d 6f72 7920  ef:`rich memory 
-00001180: 6d6f 6465 3c72 6963 685f 6d65 6d3e 602e  mode<rich_mem>`.
-00001190: 2049 7420 6361 6e20 6265 2072 6575 7365   It can be reuse
-000011a0: 6420 666f 7220 6269 6720 6e75 6d62 6572  d for big number
-000011b0: 206f 6620 7361 6d65 2074 7970 6520 696e   of same type in
-000011c0: 6469 7669 6475 616c 2064 6174 612e 0a0a  dividual data...
-000011d0: 2020 2020 5369 6e63 6520 6974 2063 616e      Since it can
-000011e0: 206f 6e6c 7920 6765 6e65 7261 7465 7320   only generates 
-000011f0: 696e 6469 7669 6475 616c 203a 7265 663a  individual :ref:
-00001200: 6066 7261 6d65 733c 6672 616d 655f 626c  `frames<frame_bl
-00001210: 6f63 6b3e 602c 2069 7427 7320 6e6f 7420  ock>`, it's not 
-00001220: 7375 6974 6162 6c65 2066 6f72 2073 7472  suitable for str
-00001230: 6561 6d69 6e67 2063 6f6d 7072 6573 7369  eaming compressi
-00001240: 6f6e 2c20 6f74 6865 7277 6973 6520 7468  on, otherwise th
-00001250: 6520 636f 6d70 7265 7373 696f 6e20 7261  e compression ra
-00001260: 7469 6f20 7769 6c6c 2062 6520 7265 6475  tio will be redu
-00001270: 6365 642c 2061 6e64 2073 6f6d 6520 7072  ced, and some pr
-00001280: 6f67 7261 6d73 2063 616e 2774 2064 6563  ograms can't dec
-00001290: 6f6d 7072 6573 7320 6d75 6c74 6970 6c65  ompress multiple
-000012a0: 2066 7261 6d65 7320 6461 7461 2e20 466f   frames data. Fo
-000012b0: 7220 7374 7265 616d 696e 6720 636f 6d70  r streaming comp
-000012c0: 7265 7373 696f 6e2c 2073 6565 203a 7265  ression, see :re
-000012d0: 663a 6074 6869 7320 7365 6374 696f 6e3c  f:`this section<
-000012e0: 7374 7265 616d 5f63 6f6d 7072 6573 7369  stream_compressi
-000012f0: 6f6e 3e60 2e0a 0a20 2020 2054 6872 6561  on>`...    Threa
-00001300: 642d 7361 6665 2061 7420 6d65 7468 6f64  d-safe at method
-00001310: 206c 6576 656c 2e0a 0a20 2020 202e 2e20   level...    .. 
-00001320: 7079 3a6d 6574 686f 643a 3a20 5f5f 696e  py:method:: __in
-00001330: 6974 5f5f 2873 656c 662c 206c 6576 656c  it__(self, level
-00001340: 5f6f 725f 6f70 7469 6f6e 3d4e 6f6e 652c  _or_option=None,
-00001350: 207a 7374 645f 6469 6374 3d4e 6f6e 6529   zstd_dict=None)
-00001360: 0a0a 2020 2020 2020 2020 5468 6520 7061  ..        The pa
-00001370: 7261 6d65 7465 7273 2061 7265 2074 6865  rameters are the
-00001380: 2073 616d 6520 6173 203a 7079 3a6d 6574   same as :py:met
-00001390: 683a 605a 7374 6443 6f6d 7072 6573 736f  h:`ZstdCompresso
-000013a0: 722e 5f5f 696e 6974 5f5f 6020 6d65 7468  r.__init__` meth
-000013b0: 6f64 2e0a 0a20 2020 202e 2e20 7079 3a6d  od...    .. py:m
-000013c0: 6574 686f 643a 3a20 636f 6d70 7265 7373  ethod:: compress
-000013d0: 2873 656c 662c 2064 6174 6129 0a0a 2020  (self, data)..  
-000013e0: 2020 2020 2020 436f 6d70 7265 7373 202a        Compress *
-000013f0: 6461 7461 2a20 7573 696e 6720 3a72 6566  data* using :ref
-00001400: 3a60 7269 6368 206d 656d 6f72 7920 6d6f  :`rich memory mo
-00001410: 6465 3c72 6963 685f 6d65 6d3e 602c 2072  de<rich_mem>`, r
-00001420: 6574 7572 6e20 6120 7369 6e67 6c65 207a  eturn a single z
-00001430: 7374 6420 3a72 6566 3a60 6672 616d 653c  std :ref:`frame<
-00001440: 6672 616d 655f 626c 6f63 6b3e 602e 0a0a  frame_block>`...
-00001450: 2020 2020 2020 2020 436f 6d70 7265 7373          Compress
-00001460: 696e 6720 6060 6227 2760 6020 7769 6c6c  ing ``b''`` will
-00001470: 2067 6574 2061 6e20 656d 7074 7920 636f   get an empty co
-00001480: 6e74 656e 7420 6672 616d 6520 2839 2062  ntent frame (9 b
-00001490: 7974 6573 206f 7220 6d6f 7265 292e 0a0a  ytes or more)...
-000014a0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-000014b0: 6174 613a 2044 6174 6120 746f 2062 6520  ata: Data to be 
-000014c0: 636f 6d70 7265 7373 6564 2e0a 2020 2020  compressed..    
-000014d0: 2020 2020 3a74 7970 6520 6461 7461 3a20      :type data: 
-000014e0: 6279 7465 732d 6c69 6b65 206f 626a 6563  bytes-like objec
-000014f0: 740a 2020 2020 2020 2020 3a72 6574 7572  t.        :retur
-00001500: 6e3a 2041 2073 696e 676c 6520 7a73 7464  n: A single zstd
-00001510: 2066 7261 6d65 2e0a 2020 2020 2020 2020   frame..        
-00001520: 3a72 7479 7065 3a20 6279 7465 730a 0a20  :rtype: bytes.. 
-00001530: 2020 202e 2e20 736f 7572 6365 636f 6465     .. sourcecode
-00001540: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-00001550: 2020 2063 203d 2052 6963 684d 656d 5a73     c = RichMemZs
-00001560: 7464 436f 6d70 7265 7373 6f72 2829 0a20  tdCompressor(). 
-00001570: 2020 2020 2020 2066 7261 6d65 3120 3d20         frame1 = 
-00001580: 632e 636f 6d70 7265 7373 2872 6177 5f64  c.compress(raw_d
-00001590: 6174 3129 0a20 2020 2020 2020 2066 7261  at1).        fra
-000015a0: 6d65 3220 3d20 632e 636f 6d70 7265 7373  me2 = c.compress
-000015b0: 2872 6177 5f64 6174 3229 0a0a 0a2e 2e20  (raw_dat2)..... 
-000015c0: 5f73 7472 6561 6d5f 636f 6d70 7265 7373  _stream_compress
-000015d0: 696f 6e3a 0a0a 5374 7265 616d 696e 6720  ion:..Streaming 
-000015e0: 636f 6d70 7265 7373 696f 6e0a 2d2d 2d2d  compression.----
-000015f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001600: 2d0a 0a20 2020 2054 6869 7320 7365 6374  -..    This sect
-00001610: 696f 6e20 636f 6e74 6169 6e73 3a0a 0a20  ion contains:.. 
-00001620: 2020 2020 2020 202a 2066 756e 6374 696f         * functio
-00001630: 6e20 3a70 793a 6675 6e63 3a60 636f 6d70  n :py:func:`comp
-00001640: 7265 7373 5f73 7472 6561 6d60 2c20 6120  ress_stream`, a 
-00001650: 6661 7374 2061 6e64 2063 6f6e 7665 6e69  fast and conveni
-00001660: 656e 7420 6675 6e63 7469 6f6e 2e0a 2020  ent function..  
-00001670: 2020 2020 2020 2a20 636c 6173 7320 3a70        * class :p
-00001680: 793a 636c 6173 733a 605a 7374 6443 6f6d  y:class:`ZstdCom
-00001690: 7072 6573 736f 7260 2c20 7369 6d69 6c61  pressor`, simila
-000016a0: 7220 746f 2063 6f6d 7072 6573 736f 7273  r to compressors
-000016b0: 2069 6e20 5079 7468 6f6e 2073 7461 6e64   in Python stand
-000016c0: 6172 6420 6c69 6272 6172 792e 0a0a 2020  ard library...  
-000016d0: 2020 4974 2077 6f75 6c64 2062 6520 6e69    It would be ni
-000016e0: 6365 2074 6f20 6b6e 6f77 2073 6f6d 6520  ce to know some 
-000016f0: 6b6e 6f77 6c65 6467 6520 6162 6f75 7420  knowledge about 
-00001700: 7a73 7464 2064 6174 612c 2073 6565 203a  zstd data, see :
-00001710: 7265 663a 6066 7261 6d65 2061 6e64 2062  ref:`frame and b
-00001720: 6c6f 636b 3c66 7261 6d65 5f62 6c6f 636b  lock<frame_block
-00001730: 3e60 2e0a 0a2e 2e20 7079 3a66 756e 6374  >`..... py:funct
-00001740: 696f 6e3a 3a20 636f 6d70 7265 7373 5f73  ion:: compress_s
-00001750: 7472 6561 6d28 696e 7075 745f 7374 7265  tream(input_stre
-00001760: 616d 2c20 6f75 7470 7574 5f73 7472 6561  am, output_strea
-00001770: 6d2c 202a 2c20 6c65 7665 6c5f 6f72 5f6f  m, *, level_or_o
-00001780: 7074 696f 6e3d 4e6f 6e65 2c20 7a73 7464  ption=None, zstd
-00001790: 5f64 6963 743d 4e6f 6e65 2c20 706c 6564  _dict=None, pled
-000017a0: 6765 645f 696e 7075 745f 7369 7a65 3d4e  ged_input_size=N
-000017b0: 6f6e 652c 2072 6561 645f 7369 7a65 3d31  one, read_size=1
-000017c0: 3331 5f30 3732 2c20 7772 6974 655f 7369  31_072, write_si
-000017d0: 7a65 3d31 3331 5f35 3931 2c20 6361 6c6c  ze=131_591, call
-000017e0: 6261 636b 3d4e 6f6e 6529 0a0a 2020 2020  back=None)..    
-000017f0: 4120 6661 7374 2061 6e64 2063 6f6e 7665  A fast and conve
-00001800: 6e69 656e 7420 6675 6e63 7469 6f6e 2c20  nient function, 
-00001810: 636f 6d70 7265 7373 6573 202a 696e 7075  compresses *inpu
-00001820: 745f 7374 7265 616d 2a20 616e 6420 7772  t_stream* and wr
-00001830: 6974 6573 2074 6865 2063 6f6d 7072 6573  ites the compres
-00001840: 7365 6420 6461 7461 2074 6f20 2a6f 7574  sed data to *out
-00001850: 7075 745f 7374 7265 616d 2a2c 2069 7420  put_stream*, it 
-00001860: 646f 6573 6e27 7420 636c 6f73 6520 7468  doesn't close th
-00001870: 6520 7374 7265 616d 732e 0a0a 2020 2020  e streams...    
-00001880: 4966 2069 6e70 7574 2073 7472 6561 6d20  If input stream 
-00001890: 6973 2060 6062 2727 6060 2c20 6e6f 7468  is ``b''``, noth
-000018a0: 696e 6720 7769 6c6c 2062 6520 7772 6974  ing will be writ
-000018b0: 7465 6e20 746f 206f 7574 7075 7420 7374  ten to output st
-000018c0: 7265 616d 2e0a 0a20 2020 2054 6869 7320  ream...    This 
-000018d0: 6675 6e63 7469 6f6e 2074 7269 6573 2074  function tries t
-000018e0: 6f20 7a65 726f 2d63 6f70 7920 6173 206d  o zero-copy as m
-000018f0: 7563 6820 6173 2070 6f73 7369 626c 652e  uch as possible.
-00001900: 2049 6620 7468 6520 4f53 2068 6173 2072   If the OS has r
-00001910: 6561 6420 7072 6566 6574 6368 696e 6720  ead prefetching 
-00001920: 616e 6420 7772 6974 6520 6275 6666 6572  and write buffer
-00001930: 2c20 6974 206d 6179 2070 6572 666f 726d  , it may perform
-00001940: 2074 6865 2074 6173 6b73 2028 7265 6164   the tasks (read
-00001950: 2f63 6f6d 7072 6573 732f 7772 6974 6529  /compress/write)
-00001960: 2069 6e20 7061 7261 6c6c 656c 2074 6f20   in parallel to 
-00001970: 736f 6d65 2064 6567 7265 652e 0a0a 2020  some degree...  
-00001980: 2020 5468 6520 6465 6661 756c 7420 7661    The default va
-00001990: 6c75 6573 206f 6620 2a72 6561 645f 7369  lues of *read_si
-000019a0: 7a65 2a20 616e 6420 2a77 7269 7465 5f73  ze* and *write_s
-000019b0: 697a 652a 2070 6172 616d 6574 6572 7320  ize* parameters 
-000019c0: 6172 6520 7468 6520 6275 6666 6572 2073  are the buffer s
-000019d0: 697a 6573 2072 6563 6f6d 6d65 6e64 6564  izes recommended
-000019e0: 2062 7920 7a73 7464 2c20 696e 6372 6561   by zstd, increa
-000019f0: 7369 6e67 2074 6865 6d20 6d61 7920 6265  sing them may be
-00001a00: 2066 6173 7465 722c 2061 6e64 2072 6564   faster, and red
-00001a10: 7563 6573 2074 6865 206e 756d 6265 7220  uces the number 
-00001a20: 6f66 2063 616c 6c62 6163 6b20 6675 6e63  of callback func
-00001a30: 7469 6f6e 2063 616c 6c73 2e0a 0a20 2020  tion calls...   
-00001a40: 202e 2e20 7665 7273 696f 6e61 6464 6564   .. versionadded
-00001a50: 3a3a 2030 2e31 342e 320a 0a20 2020 203a  :: 0.14.2..    :
-00001a60: 7061 7261 6d20 696e 7075 745f 7374 7265  param input_stre
-00001a70: 616d 3a20 496e 7075 7420 7374 7265 616d  am: Input stream
-00001a80: 2074 6861 7420 6861 7320 6120 602e 7265   that has a `.re
-00001a90: 6164 696e 746f 2862 2920 3c68 7474 7073  adinto(b) <https
-00001aa0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00001ab0: 7267 2f33 2f6c 6962 7261 7279 2f69 6f2e  rg/3/library/io.
-00001ac0: 6874 6d6c 2369 6f2e 5261 7749 4f42 6173  html#io.RawIOBas
-00001ad0: 652e 7265 6164 696e 746f 3e60 5f20 6d65  e.readinto>`_ me
-00001ae0: 7468 6f64 2e0a 2020 2020 3a70 6172 616d  thod..    :param
-00001af0: 206f 7574 7075 745f 7374 7265 616d 3a20   output_stream: 
-00001b00: 4f75 7470 7574 2073 7472 6561 6d20 7468  Output stream th
-00001b10: 6174 2068 6173 2061 2060 2e77 7269 7465  at has a `.write
-00001b20: 2862 2920 3c68 7474 7073 3a2f 2f64 6f63  (b) <https://doc
-00001b30: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-00001b40: 6962 7261 7279 2f69 6f2e 6874 6d6c 2369  ibrary/io.html#i
-00001b50: 6f2e 5261 7749 4f42 6173 652e 7772 6974  o.RawIOBase.writ
-00001b60: 653e 605f 206d 6574 686f 642e 2049 6620  e>`_ method. If 
-00001b70: 7573 6520 2a63 616c 6c62 6163 6b2a 2066  use *callback* f
-00001b80: 756e 6374 696f 6e2c 2074 6869 7320 7061  unction, this pa
-00001b90: 7261 6d65 7465 7220 6361 6e20 6265 2060  rameter can be `
-00001ba0: 604e 6f6e 6560 602e 0a20 2020 203a 7061  `None``..    :pa
-00001bb0: 7261 6d20 6c65 7665 6c5f 6f72 5f6f 7074  ram level_or_opt
-00001bc0: 696f 6e3a 2057 6865 6e20 6974 2773 2061  ion: When it's a
-00001bd0: 6e20 6060 696e 7460 6020 6f62 6a65 6374  n ``int`` object
-00001be0: 2c20 6974 2072 6570 7265 7365 6e74 7320  , it represents 
-00001bf0: 3a72 6566 3a60 636f 6d70 7265 7373 696f  :ref:`compressio
-00001c00: 6e20 6c65 7665 6c3c 636f 6d70 7265 7373  n level<compress
-00001c10: 696f 6e5f 6c65 7665 6c3e 602e 2057 6865  ion_level>`. Whe
-00001c20: 6e20 6974 2773 2061 2060 6064 6963 7460  n it's a ``dict`
-00001c30: 6020 6f62 6a65 6374 2c20 6974 2063 6f6e  ` object, it con
-00001c40: 7461 696e 7320 3a72 6566 3a60 6164 7661  tains :ref:`adva
-00001c50: 6e63 6564 2063 6f6d 7072 6573 7369 6f6e  nced compression
-00001c60: 2070 6172 616d 6574 6572 733c 4350 6172   parameters<CPar
-00001c70: 616d 6574 6572 3e60 2e20 5468 6520 6465  ameter>`. The de
-00001c80: 6661 756c 7420 7661 6c75 6520 6060 4e6f  fault value ``No
-00001c90: 6e65 6060 206d 6561 6e73 2074 6f20 7573  ne`` means to us
-00001ca0: 6520 7a73 7464 2773 2064 6566 6175 6c74  e zstd's default
-00001cb0: 2063 6f6d 7072 6573 7369 6f6e 206c 6576   compression lev
-00001cc0: 656c 2f70 6172 616d 6574 6572 732e 0a20  el/parameters.. 
-00001cd0: 2020 203a 7479 7065 206c 6576 656c 5f6f     :type level_o
-00001ce0: 725f 6f70 7469 6f6e 3a20 696e 7420 6f72  r_option: int or
-00001cf0: 2064 6963 740a 2020 2020 3a70 6172 616d   dict.    :param
-00001d00: 207a 7374 645f 6469 6374 3a20 5072 652d   zstd_dict: Pre-
-00001d10: 7472 6169 6e65 6420 6469 6374 696f 6e61  trained dictiona
-00001d20: 7279 2066 6f72 2063 6f6d 7072 6573 7369  ry for compressi
-00001d30: 6f6e 2e0a 2020 2020 3a74 7970 6520 7a73  on..    :type zs
-00001d40: 7464 5f64 6963 743a 205a 7374 6444 6963  td_dict: ZstdDic
-00001d50: 740a 2020 2020 3a70 6172 616d 2070 6c65  t.    :param ple
-00001d60: 6467 6564 5f69 6e70 7574 5f73 697a 653a  dged_input_size:
-00001d70: 2049 6620 7365 7420 7468 6973 2070 6172   If set this par
-00001d80: 616d 6574 6572 2074 6f20 7468 6520 7369  ameter to the si
-00001d90: 7a65 206f 6620 696e 7075 7420 6461 7461  ze of input data
-00001da0: 2c20 7468 6520 3a72 6566 3a60 7369 7a65  , the :ref:`size
-00001db0: 3c63 6f6e 7465 6e74 5f73 697a 653e 6020  <content_size>` 
-00001dc0: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
-00001dd0: 696e 746f 2074 6865 2066 7261 6d65 2068  into the frame h
-00001de0: 6561 6465 722e 2049 6620 7468 6520 6163  eader. If the ac
-00001df0: 7475 616c 2069 6e70 7574 2064 6174 6120  tual input data 
-00001e00: 646f 6573 6e27 7420 6d61 7463 6820 6974  doesn't match it
-00001e10: 2c20 6120 3a70 793a 636c 6173 733a 605a  , a :py:class:`Z
-00001e20: 7374 6445 7272 6f72 6020 6578 6365 7074  stdError` except
-00001e30: 696f 6e20 7769 6c6c 2062 6520 7261 6973  ion will be rais
-00001e40: 6564 2e20 4974 206d 6179 2069 6e63 7265  ed. It may incre
-00001e50: 6173 6520 636f 6d70 7265 7373 696f 6e20  ase compression 
-00001e60: 7261 7469 6f20 736c 6967 6874 6c79 2c20  ratio slightly, 
-00001e70: 616e 6420 6865 6c70 2064 6563 6f6d 7072  and help decompr
-00001e80: 6573 7369 6f6e 2063 6f64 6520 746f 2061  ession code to a
-00001e90: 6c6c 6f63 6174 6520 6f75 7470 7574 2062  llocate output b
-00001ea0: 7566 6665 7220 6661 7374 6572 2e0a 2020  uffer faster..  
-00001eb0: 2020 3a74 7970 6520 706c 6564 6765 645f    :type pledged_
-00001ec0: 696e 7075 745f 7369 7a65 3a20 696e 740a  input_size: int.
-00001ed0: 2020 2020 3a70 6172 616d 2072 6561 645f      :param read_
-00001ee0: 7369 7a65 3a20 496e 7075 7420 6275 6666  size: Input buff
-00001ef0: 6572 2073 697a 652c 2069 6e20 6279 7465  er size, in byte
-00001f00: 732e 0a20 2020 203a 7479 7065 2072 6561  s..    :type rea
-00001f10: 645f 7369 7a65 3a20 696e 740a 2020 2020  d_size: int.    
-00001f20: 3a70 6172 616d 2077 7269 7465 5f73 697a  :param write_siz
-00001f30: 653a 204f 7574 7075 7420 6275 6666 6572  e: Output buffer
-00001f40: 2073 697a 652c 2069 6e20 6279 7465 732e   size, in bytes.
-00001f50: 0a20 2020 203a 7479 7065 2077 7269 7465  .    :type write
-00001f60: 5f73 697a 653a 2069 6e74 0a20 2020 203a  _size: int.    :
-00001f70: 7061 7261 6d20 6361 6c6c 6261 636b 3a20  param callback: 
-00001f80: 4120 6361 6c6c 6261 636b 2066 756e 6374  A callback funct
-00001f90: 696f 6e20 7468 6174 2061 6363 6570 7473  ion that accepts
-00001fa0: 2066 6f75 7220 7061 7261 6d65 7465 7273   four parameters
-00001fb0: 3a20 6060 2874 6f74 616c 5f69 6e70 7574  : ``(total_input
-00001fc0: 2c20 746f 7461 6c5f 6f75 7470 7574 2c20  , total_output, 
-00001fd0: 7265 6164 5f64 6174 612c 2077 7269 7465  read_data, write
-00001fe0: 5f64 6174 6129 6060 2e20 5468 6520 6669  _data)``. The fi
-00001ff0: 7273 7420 7477 6f20 6172 6520 6060 696e  rst two are ``in
-00002000: 7460 6020 6f62 6a65 6374 732e 2054 6865  t`` objects. The
-00002010: 206c 6173 7420 7477 6f20 6172 6520 7265   last two are re
-00002020: 6164 6f6e 6c79 2060 6d65 6d6f 7279 7669  adonly `memoryvi
-00002030: 6577 203c 6874 7470 733a 2f2f 646f 6373  ew <https://docs
-00002040: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-00002050: 6272 6172 792f 7374 6474 7970 6573 2e68  brary/stdtypes.h
-00002060: 746d 6c23 6d65 6d6f 7279 2d76 6965 7773  tml#memory-views
-00002070: 3e60 5f20 6f62 6a65 6374 732c 2069 6620  >`_ objects, if 
-00002080: 7761 6e74 2074 6f20 7265 6665 7265 6e63  want to referenc
-00002090: 6520 7468 6520 6461 7461 2028 6f72 2069  e the data (or i
-000020a0: 7473 2073 6c69 6365 2920 6f75 7473 6964  ts slice) outsid
-000020b0: 6520 7468 6520 6361 6c6c 6261 636b 2066  e the callback f
-000020c0: 756e 6374 696f 6e2c 2060 636f 6e76 6572  unction, `conver
-000020d0: 7420 3c68 7474 7073 3a2f 2f64 6f63 732e  t <https://docs.
-000020e0: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
-000020f0: 7261 7279 2f73 7464 7479 7065 732e 6874  rary/stdtypes.ht
-00002100: 6d6c 236d 656d 6f72 7976 6965 772e 746f  ml#memoryview.to
-00002110: 6279 7465 733e 605f 2074 6865 6d20 746f  bytes>`_ them to
-00002120: 2060 6062 7974 6573 6060 206f 626a 6563   ``bytes`` objec
-00002130: 7473 2e20 4966 2069 6e70 7574 2073 7472  ts. If input str
-00002140: 6561 6d20 6973 2060 6062 2727 6060 2c20  eam is ``b''``, 
-00002150: 7468 6520 6361 6c6c 6261 636b 2066 756e  the callback fun
-00002160: 6374 696f 6e20 7769 6c6c 206e 6f74 2062  ction will not b
-00002170: 6520 6361 6c6c 6564 2e0a 2020 2020 3a74  e called..    :t
-00002180: 7970 6520 6361 6c6c 6261 636b 3a20 6361  ype callback: ca
-00002190: 6c6c 6162 6c65 0a20 2020 203a 7265 7475  llable.    :retu
-000021a0: 726e 3a20 4120 322d 6974 656d 2074 7570  rn: A 2-item tup
-000021b0: 6c65 2c20 6060 2874 6f74 616c 5f69 6e70  le, ``(total_inp
-000021c0: 7574 2c20 746f 7461 6c5f 6f75 7470 7574  ut, total_output
-000021d0: 2960 602c 2074 6865 2069 7465 6d73 2061  )``, the items a
-000021e0: 7265 2060 6069 6e74 6060 206f 626a 6563  re ``int`` objec
-000021f0: 7473 2e0a 0a20 2020 202e 2e20 736f 7572  ts...    .. sour
-00002200: 6365 636f 6465 3a3a 2070 7974 686f 6e0a  cecode:: python.
-00002210: 0a20 2020 2020 2020 2023 2063 6f6d 7072  .        # compr
-00002220: 6573 7320 616e 2069 6e70 7574 2066 696c  ess an input fil
-00002230: 652c 2061 6e64 2077 7269 7465 2074 6f20  e, and write to 
-00002240: 616e 206f 7574 7075 7420 6669 6c65 2e0a  an output file..
-00002250: 2020 2020 2020 2020 7769 7468 2069 6f2e          with io.
-00002260: 6f70 656e 2869 6e70 7574 5f66 696c 655f  open(input_file_
-00002270: 7061 7468 2c20 2772 6227 2920 6173 2069  path, 'rb') as i
-00002280: 6668 3a0a 2020 2020 2020 2020 2020 2020  fh:.            
-00002290: 7769 7468 2069 6f2e 6f70 656e 286f 7574  with io.open(out
-000022a0: 7075 745f 6669 6c65 5f70 6174 682c 2027  put_file_path, '
-000022b0: 7762 2729 2061 7320 6f66 683a 0a20 2020  wb') as ofh:.   
-000022c0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-000022d0: 7072 6573 735f 7374 7265 616d 2869 6668  press_stream(ifh
-000022e0: 2c20 6f66 682c 206c 6576 656c 5f6f 725f  , ofh, level_or_
-000022f0: 6f70 7469 6f6e 3d35 290a 0a20 2020 2020  option=5)..     
-00002300: 2020 2023 2063 6f6d 7072 6573 7320 6120     # compress a 
-00002310: 6279 7465 7320 6f62 6a65 6374 2c20 616e  bytes object, an
-00002320: 6420 7772 6974 6520 746f 2061 2066 696c  d write to a fil
-00002330: 652e 0a20 2020 2020 2020 2077 6974 6820  e..        with 
-00002340: 696f 2e42 7974 6573 494f 2872 6177 5f64  io.BytesIO(raw_d
-00002350: 6174 2920 6173 2062 693a 0a20 2020 2020  at) as bi:.     
-00002360: 2020 2020 2020 2077 6974 6820 696f 2e6f         with io.o
-00002370: 7065 6e28 6f75 7470 7574 5f66 696c 655f  pen(output_file_
-00002380: 7061 7468 2c20 2777 6227 2920 6173 206f  path, 'wb') as o
-00002390: 6668 3a0a 2020 2020 2020 2020 2020 2020  fh:.            
-000023a0: 2020 2020 636f 6d70 7265 7373 5f73 7472      compress_str
-000023b0: 6561 6d28 6269 2c20 6f66 682c 2070 6c65  eam(bi, ofh, ple
-000023c0: 6467 6564 5f69 6e70 7574 5f73 697a 653d  dged_input_size=
-000023d0: 6c65 6e28 7261 775f 6461 7429 290a 0a20  len(raw_dat)).. 
-000023e0: 2020 2020 2020 2023 2043 6f6d 7072 6573         # Compres
-000023f0: 7320 616e 2069 6e70 7574 2066 696c 652c  s an input file,
-00002400: 206f 6274 6169 6e20 6120 6279 7465 7320   obtain a bytes 
-00002410: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-00002420: 2320 4974 2773 2066 6173 7465 7220 7468  # It's faster th
-00002430: 616e 2072 6561 6469 6e67 2061 2066 696c  an reading a fil
-00002440: 6520 616e 6420 636f 6d70 7265 7373 696e  e and compressin
-00002450: 6720 6974 2069 6e0a 2020 2020 2020 2020  g it in.        
-00002460: 2320 6d65 6d6f 7279 2c20 7465 7374 6564  # memory, tested
-00002470: 206f 6e20 5562 756e 7475 2850 7974 686f   on Ubuntu(Pytho
-00002480: 6e33 2e38 292f 5769 6e64 6f77 7328 5079  n3.8)/Windows(Py
-00002490: 7468 6f6e 332e 3929 2e0a 2020 2020 2020  thon3.9)..      
-000024a0: 2020 2320 4d61 7962 6520 7468 6520 4f53    # Maybe the OS
-000024b0: 2068 6173 2070 7265 6665 7463 6869 6e67   has prefetching
-000024c0: 2c20 6974 2063 616e 2072 6561 6420 616e  , it can read an
-000024d0: 6420 636f 6d70 7265 7373 0a20 2020 2020  d compress.     
-000024e0: 2020 2023 2064 6174 6120 696e 2070 6172     # data in par
-000024f0: 616c 6c65 6c20 746f 2073 6f6d 6520 6465  allel to some de
-00002500: 6772 6565 2c20 7265 6164 696e 6720 6669  gree, reading fi
-00002510: 6c65 2066 726f 6d20 4844 440a 2020 2020  le from HDD.    
-00002520: 2020 2020 2320 6973 2074 6865 2062 6f74      # is the bot
-00002530: 746c 656e 6563 6b20 696e 2074 6869 7320  tleneck in this 
-00002540: 6361 7365 2e0a 2020 2020 2020 2020 7769  case..        wi
-00002550: 7468 2069 6f2e 6f70 656e 2869 6e70 7574  th io.open(input
-00002560: 5f66 696c 655f 7061 7468 2c20 2772 6227  _file_path, 'rb'
-00002570: 2920 6173 2069 6668 3a0a 2020 2020 2020  ) as ifh:.      
-00002580: 2020 2020 2020 7769 7468 2069 6f2e 4279        with io.By
-00002590: 7465 7349 4f28 2920 6173 2062 6f3a 0a20  tesIO() as bo:. 
-000025a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000025b0: 6f6d 7072 6573 735f 7374 7265 616d 2869  ompress_stream(i
-000025c0: 6668 2c20 626f 290a 2020 2020 2020 2020  fh, bo).        
-000025d0: 2020 2020 2020 2020 636f 6d70 7265 7373          compress
-000025e0: 6564 5f64 6174 203d 2062 6f2e 6765 7476  ed_dat = bo.getv
-000025f0: 616c 7565 2829 0a0a 2020 2020 2020 2020  alue()..        
-00002600: 2320 5072 696e 7420 7072 6f67 7265 7373  # Print progress
-00002610: 2075 7369 6e67 2063 616c 6c62 6163 6b20   using callback 
-00002620: 6675 6e63 7469 6f6e 0a20 2020 2020 2020  function.       
-00002630: 2064 6566 2063 6f6d 7072 6573 735f 7072   def compress_pr
-00002640: 696e 745f 7072 6f67 7265 7373 2869 6e70  int_progress(inp
-00002650: 7574 5f66 696c 655f 7061 7468 2c20 6f75  ut_file_path, ou
-00002660: 7470 7574 5f66 696c 655f 7061 7468 293a  tput_file_path):
-00002670: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
-00002680: 7574 5f66 696c 655f 7369 7a65 203d 206f  ut_file_size = o
-00002690: 732e 7061 7468 2e67 6574 7369 7a65 2869  s.path.getsize(i
-000026a0: 6e70 7574 5f66 696c 655f 7061 7468 290a  nput_file_path).
-000026b0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-000026c0: 2066 756e 6328 746f 7461 6c5f 696e 7075   func(total_inpu
-000026d0: 742c 2074 6f74 616c 5f6f 7574 7075 742c  t, total_output,
-000026e0: 2072 6561 645f 6461 7461 2c20 7772 6974   read_data, writ
-000026f0: 655f 6461 7461 293a 0a20 2020 2020 2020  e_data):.       
-00002700: 2020 2020 2020 2020 2023 2049 6620 696e           # If in
-00002710: 7075 7420 7374 7265 616d 2069 7320 656d  put stream is em
-00002720: 7074 792c 2074 6865 2063 616c 6c62 6163  pty, the callbac
-00002730: 6b20 6675 6e63 7469 6f6e 0a20 2020 2020  k function.     
-00002740: 2020 2020 2020 2020 2020 2023 2077 696c             # wil
-00002750: 6c20 6e6f 7420 6265 2063 616c 6c65 642e  l not be called.
-00002760: 2053 6f20 6e6f 205a 6572 6f44 6976 6973   So no ZeroDivis
-00002770: 696f 6e45 7272 6f72 2068 6572 652e 0a20  ionError here.. 
-00002780: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00002790: 6572 6365 6e74 203d 2031 3030 202a 2074  ercent = 100 * t
-000027a0: 6f74 616c 5f69 6e70 7574 202f 2069 6e70  otal_input / inp
-000027b0: 7574 5f66 696c 655f 7369 7a65 0a20 2020  ut_file_size.   
-000027c0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000027d0: 6e74 2866 2750 726f 6772 6573 733a 207b  nt(f'Progress: {
-000027e0: 7065 7263 656e 743a 2e31 667d 2527 2c20  percent:.1f}%', 
-000027f0: 656e 643d 275c 7227 290a 0a20 2020 2020  end='\r')..     
-00002800: 2020 2020 2020 2077 6974 6820 696f 2e6f         with io.o
-00002810: 7065 6e28 696e 7075 745f 6669 6c65 5f70  pen(input_file_p
-00002820: 6174 682c 2027 7262 2729 2061 7320 6966  ath, 'rb') as if
-00002830: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-00002840: 2020 2077 6974 6820 696f 2e6f 7065 6e28     with io.open(
-00002850: 6f75 7470 7574 5f66 696c 655f 7061 7468  output_file_path
-00002860: 2c20 2777 6227 2920 6173 206f 6668 3a0a  , 'wb') as ofh:.
-00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002880: 2020 2020 636f 6d70 7265 7373 5f73 7472      compress_str
-00002890: 6561 6d28 6966 682c 206f 6668 2c20 6361  eam(ifh, ofh, ca
-000028a0: 6c6c 6261 636b 3d66 756e 6329 0a0a 0a2e  llback=func)....
-000028b0: 2e20 7079 3a63 6c61 7373 3a3a 205a 7374  . py:class:: Zst
-000028c0: 6443 6f6d 7072 6573 736f 720a 0a20 2020  dCompressor..   
-000028d0: 2041 2073 7472 6561 6d69 6e67 2063 6f6d   A streaming com
-000028e0: 7072 6573 736f 722e 2049 7427 7320 7468  pressor. It's th
-000028f0: 7265 6164 2d73 6166 6520 6174 206d 6574  read-safe at met
-00002900: 686f 6420 6c65 7665 6c2e 0a0a 2020 2020  hod level...    
-00002910: 2e2e 2070 793a 6d65 7468 6f64 3a3a 205f  .. py:method:: _
-00002920: 5f69 6e69 745f 5f28 7365 6c66 2c20 6c65  _init__(self, le
-00002930: 7665 6c5f 6f72 5f6f 7074 696f 6e3d 4e6f  vel_or_option=No
-00002940: 6e65 2c20 7a73 7464 5f64 6963 743d 4e6f  ne, zstd_dict=No
-00002950: 6e65 290a 0a20 2020 2020 2020 2049 6e69  ne)..        Ini
-00002960: 7469 616c 697a 6520 6120 5a73 7464 436f  tialize a ZstdCo
-00002970: 6d70 7265 7373 6f72 206f 626a 6563 742e  mpressor object.
-00002980: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00002990: 206c 6576 656c 5f6f 725f 6f70 7469 6f6e   level_or_option
-000029a0: 3a20 5768 656e 2069 7427 7320 616e 2060  : When it's an `
-000029b0: 6069 6e74 6060 206f 626a 6563 742c 2069  `int`` object, i
-000029c0: 7420 7265 7072 6573 656e 7473 2074 6865  t represents the
-000029d0: 203a 7265 663a 6063 6f6d 7072 6573 7369   :ref:`compressi
-000029e0: 6f6e 206c 6576 656c 3c63 6f6d 7072 6573  on level<compres
-000029f0: 7369 6f6e 5f6c 6576 656c 3e60 2e20 5768  sion_level>`. Wh
-00002a00: 656e 2069 7427 7320 6120 6060 6469 6374  en it's a ``dict
-00002a10: 6060 206f 626a 6563 742c 2069 7420 636f  `` object, it co
-00002a20: 6e74 6169 6e73 203a 7265 663a 6061 6476  ntains :ref:`adv
-00002a30: 616e 6365 6420 636f 6d70 7265 7373 696f  anced compressio
-00002a40: 6e20 7061 7261 6d65 7465 7273 3c43 5061  n parameters<CPa
-00002a50: 7261 6d65 7465 723e 602e 2054 6865 2064  rameter>`. The d
-00002a60: 6566 6175 6c74 2076 616c 7565 2060 604e  efault value ``N
-00002a70: 6f6e 6560 6020 6d65 616e 7320 746f 2075  one`` means to u
-00002a80: 7365 207a 7374 6427 7320 6465 6661 756c  se zstd's defaul
-00002a90: 7420 636f 6d70 7265 7373 696f 6e20 6c65  t compression le
-00002aa0: 7665 6c2f 7061 7261 6d65 7465 7273 2e0a  vel/parameters..
-00002ab0: 2020 2020 2020 2020 3a74 7970 6520 6c65          :type le
-00002ac0: 7665 6c5f 6f72 5f6f 7074 696f 6e3a 2069  vel_or_option: i
-00002ad0: 6e74 206f 7220 6469 6374 0a20 2020 2020  nt or dict.     
-00002ae0: 2020 203a 7061 7261 6d20 7a73 7464 5f64     :param zstd_d
-00002af0: 6963 743a 2050 7265 2d74 7261 696e 6564  ict: Pre-trained
-00002b00: 2064 6963 7469 6f6e 6172 7920 666f 7220   dictionary for 
-00002b10: 636f 6d70 7265 7373 696f 6e2e 0a20 2020  compression..   
-00002b20: 2020 2020 203a 7479 7065 207a 7374 645f       :type zstd_
-00002b30: 6469 6374 3a20 5a73 7464 4469 6374 0a0a  dict: ZstdDict..
-00002b40: 2020 2020 2e2e 2070 793a 6d65 7468 6f64      .. py:method
-00002b50: 3a3a 2063 6f6d 7072 6573 7328 7365 6c66  :: compress(self
-00002b60: 2c20 6461 7461 2c20 6d6f 6465 3d5a 7374  , data, mode=Zst
-00002b70: 6443 6f6d 7072 6573 736f 722e 434f 4e54  dCompressor.CONT
-00002b80: 494e 5545 290a 0a20 2020 2020 2020 2050  INUE)..        P
-00002b90: 726f 7669 6465 2064 6174 6120 746f 2074  rovide data to t
-00002ba0: 6865 2063 6f6d 7072 6573 736f 7220 6f62  he compressor ob
-00002bb0: 6a65 6374 2e0a 0a20 2020 2020 2020 203a  ject...        :
-00002bc0: 7061 7261 6d20 6461 7461 3a20 4461 7461  param data: Data
-00002bd0: 2074 6f20 6265 2063 6f6d 7072 6573 7365   to be compresse
-00002be0: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
-00002bf0: 2064 6174 613a 2062 7974 6573 2d6c 696b   data: bytes-lik
-00002c00: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
-00002c10: 203a 7061 7261 6d20 6d6f 6465 3a20 4361   :param mode: Ca
-00002c20: 6e20 6265 2074 6865 7365 2033 2076 616c  n be these 3 val
-00002c30: 7565 733a 203a 7079 3a61 7474 723a 605a  ues: :py:attr:`Z
-00002c40: 7374 6443 6f6d 7072 6573 736f 722e 434f  stdCompressor.CO
-00002c50: 4e54 494e 5545 602c 203a 7079 3a61 7474  NTINUE`, :py:att
-00002c60: 723a 605a 7374 6443 6f6d 7072 6573 736f  r:`ZstdCompresso
-00002c70: 722e 464c 5553 485f 424c 4f43 4b60 2c20  r.FLUSH_BLOCK`, 
-00002c80: 3a70 793a 6174 7472 3a60 5a73 7464 436f  :py:attr:`ZstdCo
-00002c90: 6d70 7265 7373 6f72 2e46 4c55 5348 5f46  mpressor.FLUSH_F
-00002ca0: 5241 4d45 602e 0a20 2020 2020 2020 203a  RAME`..        :
-00002cb0: 7265 7475 726e 3a20 4120 6368 756e 6b20  return: A chunk 
-00002cc0: 6f66 2063 6f6d 7072 6573 7365 6420 6461  of compressed da
-00002cd0: 7461 2069 6620 706f 7373 6962 6c65 2c20  ta if possible, 
-00002ce0: 6f72 2060 6062 2727 6060 206f 7468 6572  or ``b''`` other
-00002cf0: 7769 7365 2e0a 2020 2020 2020 2020 3a72  wise..        :r
-00002d00: 7479 7065 3a20 6279 7465 730a 0a20 2020  type: bytes..   
-00002d10: 202e 2e20 7079 3a6d 6574 686f 643a 3a20   .. py:method:: 
-00002d20: 666c 7573 6828 7365 6c66 2c20 6d6f 6465  flush(self, mode
-00002d30: 3d5a 7374 6443 6f6d 7072 6573 736f 722e  =ZstdCompressor.
-00002d40: 464c 5553 485f 4652 414d 4529 0a0a 2020  FLUSH_FRAME)..  
-00002d50: 2020 2020 2020 466c 7573 6820 616e 7920        Flush any 
-00002d60: 7265 6d61 696e 696e 6720 6461 7461 2069  remaining data i
-00002d70: 6e20 696e 7465 726e 616c 2062 7566 6665  n internal buffe
-00002d80: 722e 0a0a 2020 2020 2020 2020 5369 6e63  r...        Sinc
-00002d90: 6520 7a73 7464 2064 6174 6120 636f 6e73  e zstd data cons
-00002da0: 6973 7473 206f 6620 6f6e 6520 6f72 206d  ists of one or m
-00002db0: 6f72 6520 696e 6465 7065 6e64 656e 7420  ore independent 
-00002dc0: 6672 616d 6573 2c20 7468 6520 636f 6d70  frames, the comp
-00002dd0: 7265 7373 6f72 206f 626a 6563 7420 6361  ressor object ca
-00002de0: 6e20 7374 696c 6c20 6265 2075 7365 6420  n still be used 
-00002df0: 6166 7465 7220 7468 6973 206d 6574 686f  after this metho
-00002e00: 6420 6973 2063 616c 6c65 642e 0a0a 2020  d is called...  
-00002e10: 2020 2020 2020 2a2a 4e6f 7465 2a2a 3a20        **Note**: 
-00002e20: 4162 7573 6520 6f66 2074 6869 7320 6d65  Abuse of this me
-00002e30: 7468 6f64 2077 696c 6c20 7265 6475 6365  thod will reduce
-00002e40: 2063 6f6d 7072 6573 7369 6f6e 2072 6174   compression rat
-00002e50: 696f 2c20 616e 6420 736f 6d65 2070 726f  io, and some pro
-00002e60: 6772 616d 7320 6361 6e20 6f6e 6c79 2064  grams can only d
-00002e70: 6563 6f6d 7072 6573 7320 7369 6e67 6c65  ecompress single
-00002e80: 2066 7261 6d65 2064 6174 612e 2055 7365   frame data. Use
-00002e90: 2069 7420 6f6e 6c79 2077 6865 6e20 6e65   it only when ne
-00002ea0: 6365 7373 6172 792e 0a0a 2020 2020 2020  cessary...      
-00002eb0: 2020 3a70 6172 616d 206d 6f64 653a 2043    :param mode: C
-00002ec0: 616e 2062 6520 7468 6573 6520 3220 7661  an be these 2 va
-00002ed0: 6c75 6573 3a20 3a70 793a 6174 7472 3a60  lues: :py:attr:`
-00002ee0: 5a73 7464 436f 6d70 7265 7373 6f72 2e46  ZstdCompressor.F
-00002ef0: 4c55 5348 5f46 5241 4d45 602c 203a 7079  LUSH_FRAME`, :py
-00002f00: 3a61 7474 723a 605a 7374 6443 6f6d 7072  :attr:`ZstdCompr
-00002f10: 6573 736f 722e 464c 5553 485f 424c 4f43  essor.FLUSH_BLOC
-00002f20: 4b60 2e0a 2020 2020 2020 2020 3a72 6574  K`..        :ret
-00002f30: 7572 6e3a 2046 6c75 7368 6564 2064 6174  urn: Flushed dat
-00002f40: 612e 0a20 2020 2020 2020 203a 7274 7970  a..        :rtyp
-00002f50: 653a 2062 7974 6573 0a0a 2020 2020 2e2e  e: bytes..    ..
-00002f60: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
-00002f70: 6c61 7374 5f6d 6f64 650a 0a20 2020 2020  last_mode..     
-00002f80: 2020 2054 6865 206c 6173 7420 6d6f 6465     The last mode
-00002f90: 2075 7365 6420 746f 2074 6869 7320 636f   used to this co
-00002fa0: 6d70 7265 7373 6f72 2c20 6974 7320 7661  mpressor, its va
-00002fb0: 6c75 6520 6361 6e20 6265 203a 7079 3a61  lue can be :py:a
-00002fc0: 7474 723a 607e 5a73 7464 436f 6d70 7265  ttr:`~ZstdCompre
-00002fd0: 7373 6f72 2e43 4f4e 5449 4e55 4560 2c20  ssor.CONTINUE`, 
-00002fe0: 3a70 793a 6174 7472 3a60 7e5a 7374 6443  :py:attr:`~ZstdC
-00002ff0: 6f6d 7072 6573 736f 722e 464c 5553 485f  ompressor.FLUSH_
-00003000: 424c 4f43 4b60 2c20 3a70 793a 6174 7472  BLOCK`, :py:attr
-00003010: 3a60 7e5a 7374 6443 6f6d 7072 6573 736f  :`~ZstdCompresso
-00003020: 722e 464c 5553 485f 4652 414d 4560 2e20  r.FLUSH_FRAME`. 
-00003030: 496e 6974 6961 6c69 7a65 6420 746f 203a  Initialized to :
-00003040: 7079 3a61 7474 723a 607e 5a73 7464 436f  py:attr:`~ZstdCo
-00003050: 6d70 7265 7373 6f72 2e46 4c55 5348 5f46  mpressor.FLUSH_F
-00003060: 5241 4d45 602e 0a0a 2020 2020 2020 2020  RAME`...        
-00003070: 4974 2063 616e 2062 6520 7573 6564 2074  It can be used t
-00003080: 6f20 6765 7420 7468 6520 6375 7272 656e  o get the curren
-00003090: 7420 7374 6174 6520 6f66 2061 2063 6f6d  t state of a com
-000030a0: 7072 6573 736f 722c 2073 7563 6820 6173  pressor, such as
-000030b0: 2c20 6461 7461 2066 6c75 7368 6564 2c20  , data flushed, 
-000030c0: 6120 6672 616d 6520 656e 6465 642e 0a0a  a frame ended...
-000030d0: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
-000030e0: 7574 653a 3a20 434f 4e54 494e 5545 0a0a  ute:: CONTINUE..
-000030f0: 2020 2020 2020 2020 5573 6564 2066 6f72          Used for
-00003100: 202a 6d6f 6465 2a20 7061 7261 6d65 7465   *mode* paramete
-00003110: 7220 696e 203a 7079 3a6d 6574 683a 607e  r in :py:meth:`~
-00003120: 5a73 7464 436f 6d70 7265 7373 6f72 2e63  ZstdCompressor.c
-00003130: 6f6d 7072 6573 7360 206d 6574 686f 642e  ompress` method.
-00003140: 0a0a 2020 2020 2020 2020 436f 6c6c 6563  ..        Collec
-00003150: 7420 6d6f 7265 2064 6174 612c 2065 6e63  t more data, enc
-00003160: 6f64 6572 2064 6563 6964 6573 2077 6865  oder decides whe
-00003170: 6e20 746f 206f 7574 7075 7420 636f 6d70  n to output comp
-00003180: 7265 7373 6564 2072 6573 756c 742c 2066  ressed result, f
-00003190: 6f72 206f 7074 696d 616c 2063 6f6d 7072  or optimal compr
-000031a0: 6573 7369 6f6e 2072 6174 696f 2e20 5573  ession ratio. Us
-000031b0: 7561 6c6c 7920 7573 6564 2066 6f72 2074  ually used for t
-000031c0: 7261 6469 7469 6f6e 616c 2073 7472 6561  raditional strea
-000031d0: 6d69 6e67 2063 6f6d 7072 6573 7369 6f6e  ming compression
-000031e0: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
-000031f0: 7269 6275 7465 3a3a 2046 4c55 5348 5f42  ribute:: FLUSH_B
-00003200: 4c4f 434b 0a0a 2020 2020 2020 2020 5573  LOCK..        Us
-00003210: 6564 2066 6f72 202a 6d6f 6465 2a20 7061  ed for *mode* pa
-00003220: 7261 6d65 7465 7220 696e 203a 7079 3a6d  rameter in :py:m
-00003230: 6574 683a 607e 5a73 7464 436f 6d70 7265  eth:`~ZstdCompre
-00003240: 7373 6f72 2e63 6f6d 7072 6573 7360 2c20  ssor.compress`, 
-00003250: 3a70 793a 6d65 7468 3a60 7e5a 7374 6443  :py:meth:`~ZstdC
-00003260: 6f6d 7072 6573 736f 722e 666c 7573 6860  ompressor.flush`
-00003270: 206d 6574 686f 6473 2e0a 0a20 2020 2020   methods...     
-00003280: 2020 2046 6c75 7368 2061 6e79 2072 656d     Flush any rem
-00003290: 6169 6e69 6e67 2064 6174 612c 2062 7574  aining data, but
-000032a0: 2064 6f6e 2774 2063 6c6f 7365 2074 6865   don't close the
-000032b0: 2063 7572 7265 6e74 203a 7265 663a 6066   current :ref:`f
-000032c0: 7261 6d65 3c66 7261 6d65 5f62 6c6f 636b  rame<frame_block
-000032d0: 3e60 2e20 5573 7561 6c6c 7920 7573 6564  >`. Usually used
-000032e0: 2066 6f72 2063 6f6d 6d75 6e69 6361 7469   for communicati
-000032f0: 6f6e 2073 6365 6e61 7269 6f73 2e0a 0a20  on scenarios... 
-00003300: 2020 2020 2020 2049 6620 7468 6572 6520         If there 
-00003310: 6973 2064 6174 612c 2069 7420 6372 6561  is data, it crea
-00003320: 7465 7320 6174 206c 6561 7374 206f 6e65  tes at least one
-00003330: 206e 6577 203a 7265 663a 6062 6c6f 636b   new :ref:`block
-00003340: 3c66 7261 6d65 5f62 6c6f 636b 3e60 2c20  <frame_block>`, 
-00003350: 7468 6174 2063 616e 2062 6520 6465 636f  that can be deco
-00003360: 6465 6420 696d 6d65 6469 6174 656c 7920  ded immediately 
-00003370: 6f6e 2072 6563 6570 7469 6f6e 2e20 4966  on reception. If
-00003380: 206e 6f20 7265 6d61 696e 696e 6720 6461   no remaining da
-00003390: 7461 2c20 6e6f 2062 6c6f 636b 2069 7320  ta, no block is 
-000033a0: 6372 6561 7465 642c 2072 6574 7572 6e20  created, return 
-000033b0: 6060 6227 2760 602e 0a0a 2020 2020 2020  ``b''``...      
-000033c0: 2020 2a2a 4e6f 7465 2a2a 3a20 4162 7573    **Note**: Abus
-000033d0: 6520 6f66 2074 6869 7320 6d6f 6465 2077  e of this mode w
-000033e0: 696c 6c20 7265 6475 6365 2063 6f6d 7072  ill reduce compr
-000033f0: 6573 7369 6f6e 2072 6174 696f 2e20 5573  ession ratio. Us
-00003400: 6520 6974 206f 6e6c 7920 7768 656e 206e  e it only when n
-00003410: 6563 6573 7361 7279 2e0a 0a20 2020 202e  ecessary...    .
-00003420: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
-00003430: 2046 4c55 5348 5f46 5241 4d45 0a0a 2020   FLUSH_FRAME..  
-00003440: 2020 2020 2020 5573 6564 2066 6f72 202a        Used for *
-00003450: 6d6f 6465 2a20 7061 7261 6d65 7465 7220  mode* parameter 
-00003460: 696e 203a 7079 3a6d 6574 683a 607e 5a73  in :py:meth:`~Zs
-00003470: 7464 436f 6d70 7265 7373 6f72 2e63 6f6d  tdCompressor.com
-00003480: 7072 6573 7360 2c20 3a70 793a 6d65 7468  press`, :py:meth
-00003490: 3a60 7e5a 7374 6443 6f6d 7072 6573 736f  :`~ZstdCompresso
-000034a0: 722e 666c 7573 6860 206d 6574 686f 6473  r.flush` methods
-000034b0: 2e0a 0a20 2020 2020 2020 2046 6c75 7368  ...        Flush
-000034c0: 2061 6e79 2072 656d 6169 6e69 6e67 2064   any remaining d
-000034d0: 6174 612c 2061 6e64 2063 6c6f 7365 2074  ata, and close t
-000034e0: 6865 2063 7572 7265 6e74 203a 7265 663a  he current :ref:
-000034f0: 6066 7261 6d65 3c66 7261 6d65 5f62 6c6f  `frame<frame_blo
-00003500: 636b 3e60 2e20 5573 7561 6c6c 7920 7573  ck>`. Usually us
-00003510: 6564 2066 6f72 2074 7261 6469 7469 6f6e  ed for tradition
-00003520: 616c 2066 6c75 7368 2e0a 0a20 2020 2020  al flush...     
-00003530: 2020 2053 696e 6365 207a 7374 6420 6461     Since zstd da
-00003540: 7461 2063 6f6e 7369 7374 7320 6f66 206f  ta consists of o
-00003550: 6e65 206f 7220 6d6f 7265 2069 6e64 6570  ne or more indep
-00003560: 656e 6465 6e74 2066 7261 6d65 732c 2064  endent frames, d
-00003570: 6174 6120 6361 6e20 7374 696c 6c20 6265  ata can still be
-00003580: 2070 726f 7669 6465 6420 6166 7465 7220   provided after 
-00003590: 6120 6672 616d 6520 6973 2063 6c6f 7365  a frame is close
-000035a0: 642e 0a0a 2020 2020 2020 2020 2a2a 4e6f  d...        **No
-000035b0: 7465 2a2a 3a20 4162 7573 6520 6f66 2074  te**: Abuse of t
-000035c0: 6869 7320 6d6f 6465 2077 696c 6c20 7265  his mode will re
-000035d0: 6475 6365 2063 6f6d 7072 6573 7369 6f6e  duce compression
-000035e0: 2072 6174 696f 2c20 616e 6420 736f 6d65   ratio, and some
-000035f0: 2070 726f 6772 616d 7320 6361 6e20 6f6e   programs can on
-00003600: 6c79 2064 6563 6f6d 7072 6573 7320 7369  ly decompress si
-00003610: 6e67 6c65 2066 7261 6d65 2064 6174 612e  ngle frame data.
-00003620: 2055 7365 2069 7420 6f6e 6c79 2077 6865   Use it only whe
-00003630: 6e20 6e65 6365 7373 6172 792e 0a0a 2020  n necessary...  
-00003640: 2020 2e2e 2073 6f75 7263 6563 6f64 653a    .. sourcecode:
-00003650: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-00003660: 2020 6320 3d20 5a73 7464 436f 6d70 7265    c = ZstdCompre
-00003670: 7373 6f72 2829 0a0a 2020 2020 2020 2020  ssor()..        
-00003680: 2320 7472 6164 6974 696f 6e61 6c20 7374  # traditional st
-00003690: 7265 616d 696e 6720 636f 6d70 7265 7373  reaming compress
-000036a0: 696f 6e0a 2020 2020 2020 2020 6461 7431  ion.        dat1
-000036b0: 203d 2063 2e63 6f6d 7072 6573 7328 6227   = c.compress(b'
-000036c0: 3132 3334 3536 2729 0a20 2020 2020 2020  123456').       
-000036d0: 2064 6174 3220 3d20 632e 636f 6d70 7265   dat2 = c.compre
-000036e0: 7373 2862 2761 6263 6465 6627 290a 2020  ss(b'abcdef').  
-000036f0: 2020 2020 2020 6461 7433 203d 2063 2e66        dat3 = c.f
-00003700: 6c75 7368 2829 0a0a 2020 2020 2020 2020  lush()..        
-00003710: 2320 7573 6520 2e63 6f6d 7072 6573 7328  # use .compress(
-00003720: 2920 6d65 7468 6f64 2077 6974 6820 6d6f  ) method with mo
-00003730: 6465 2061 7267 756d 656e 740a 2020 2020  de argument.    
-00003740: 2020 2020 636f 6d70 7265 7373 6564 5f64      compressed_d
-00003750: 6174 3120 3d20 632e 636f 6d70 7265 7373  at1 = c.compress
-00003760: 2872 6177 5f64 6174 312c 2063 2e46 4c55  (raw_dat1, c.FLU
-00003770: 5348 5f42 4c4f 434b 290a 2020 2020 2020  SH_BLOCK).      
-00003780: 2020 636f 6d70 7265 7373 6564 5f64 6174    compressed_dat
-00003790: 3220 3d20 632e 636f 6d70 7265 7373 2872  2 = c.compress(r
-000037a0: 6177 5f64 6174 322c 2063 2e46 4c55 5348  aw_dat2, c.FLUSH
-000037b0: 5f46 5241 4d45 290a 0a20 2020 202e 2e20  _FRAME)..    .. 
-000037c0: 6869 6e74 3a3a 2057 6879 203a 7079 3a6d  hint:: Why :py:m
-000037d0: 6574 683a 605a 7374 6443 6f6d 7072 6573  eth:`ZstdCompres
-000037e0: 736f 722e 636f 6d70 7265 7373 6020 6d65  sor.compress` me
-000037f0: 7468 6f64 2068 6173 2061 202a 6d6f 6465  thod has a *mode
-00003800: 2a20 7061 7261 6d65 7465 723f 0a0a 2020  * parameter?..  
-00003810: 2020 2020 2020 232e 2057 6865 6e20 7265        #. When re
-00003820: 7573 6520 3a70 793a 636c 6173 733a 605a  use :py:class:`Z
-00003830: 7374 6443 6f6d 7072 6573 736f 7260 206f  stdCompressor` o
-00003840: 626a 6563 7420 666f 7220 6269 6720 6e75  bject for big nu
-00003850: 6d62 6572 206f 6620 7361 6d65 2074 7970  mber of same typ
-00003860: 6520 696e 6469 7669 6475 616c 2064 6174  e individual dat
-00003870: 612c 206d 616b 6520 6f70 6572 6174 696f  a, make operatio
-00003880: 6e20 6d6f 7265 2063 6f6e 7665 6e69 656e  n more convenien
-00003890: 742e 2054 6865 206f 626a 6563 7420 6973  t. The object is
-000038a0: 2074 6872 6561 642d 7361 6665 2061 7420   thread-safe at 
-000038b0: 6d65 7468 6f64 206c 6576 656c 2e0a 2020  method level..  
-000038c0: 2020 2020 2020 232e 2049 6620 6461 7461        #. If data
-000038d0: 2069 7320 6765 6e65 7261 7465 6420 6279   is generated by
-000038e0: 2061 2073 696e 676c 6520 3a70 793a 6174   a single :py:at
-000038f0: 7472 3a60 7e5a 7374 6443 6f6d 7072 6573  tr:`~ZstdCompres
-00003900: 736f 722e 464c 5553 485f 4652 414d 4560  sor.FLUSH_FRAME`
-00003910: 206d 6f64 652c 2074 6865 2073 697a 6520   mode, the size 
-00003920: 6f66 2075 6e63 6f6d 7072 6573 7365 6420  of uncompressed 
-00003930: 6461 7461 2077 696c 6c20 6265 2072 6563  data will be rec
-00003940: 6f72 6465 6420 696e 2066 7261 6d65 2068  orded in frame h
-00003950: 6561 6465 722e 0a0a 0a53 7472 6561 6d69  eader....Streami
-00003960: 6e67 2064 6563 6f6d 7072 6573 7369 6f6e  ng decompression
-00003970: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-00003980: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020 5468  --------..    Th
-00003990: 6973 2073 6563 7469 6f6e 2063 6f6e 7461  is section conta
-000039a0: 696e 733a 0a0a 2020 2020 2020 2020 2a20  ins:..        * 
-000039b0: 6675 6e63 7469 6f6e 203a 7079 3a66 756e  function :py:fun
-000039c0: 633a 6064 6563 6f6d 7072 6573 735f 7374  c:`decompress_st
-000039d0: 7265 616d 602c 2061 2066 6173 7420 616e  ream`, a fast an
-000039e0: 6420 636f 6e76 656e 6965 6e74 2066 756e  d convenient fun
-000039f0: 6374 696f 6e2e 0a20 2020 2020 2020 202a  ction..        *
-00003a00: 2063 6c61 7373 203a 7079 3a63 6c61 7373   class :py:class
-00003a10: 3a60 5a73 7464 4465 636f 6d70 7265 7373  :`ZstdDecompress
-00003a20: 6f72 602c 2073 696d 696c 6172 2074 6f20  or`, similar to 
-00003a30: 6465 636f 6d70 7265 7373 6f72 7320 696e  decompressors in
-00003a40: 2050 7974 686f 6e20 7374 616e 6461 7264   Python standard
-00003a50: 206c 6962 7261 7279 2e0a 2020 2020 2020   library..      
-00003a60: 2020 2a20 636c 6173 7320 3a70 793a 636c    * class :py:cl
-00003a70: 6173 733a 6045 6e64 6c65 7373 5a73 7464  ass:`EndlessZstd
-00003a80: 4465 636f 6d70 7265 7373 6f72 602c 2061  Decompressor`, a
-00003a90: 2064 6563 6f6d 7072 6573 736f 7220 6163   decompressor ac
-00003aa0: 6365 7074 7320 6d75 6c74 6970 6c65 2063  cepts multiple c
-00003ab0: 6f6e 6361 7465 6e61 7465 6420 3a72 6566  oncatenated :ref
-00003ac0: 3a60 6672 616d 6573 3c66 7261 6d65 5f62  :`frames<frame_b
-00003ad0: 6c6f 636b 3e60 2e0a 0a2e 2e20 7079 3a66  lock>`..... py:f
-00003ae0: 756e 6374 696f 6e3a 3a20 6465 636f 6d70  unction:: decomp
-00003af0: 7265 7373 5f73 7472 6561 6d28 696e 7075  ress_stream(inpu
-00003b00: 745f 7374 7265 616d 2c20 6f75 7470 7574  t_stream, output
-00003b10: 5f73 7472 6561 6d2c 202a 2c20 7a73 7464  _stream, *, zstd
-00003b20: 5f64 6963 743d 4e6f 6e65 2c20 6f70 7469  _dict=None, opti
-00003b30: 6f6e 3d4e 6f6e 652c 2072 6561 645f 7369  on=None, read_si
-00003b40: 7a65 3d31 3331 5f30 3735 2c20 7772 6974  ze=131_075, writ
-00003b50: 655f 7369 7a65 3d31 3331 5f30 3732 2c20  e_size=131_072, 
-00003b60: 6361 6c6c 6261 636b 3d4e 6f6e 6529 0a0a  callback=None)..
-00003b70: 2020 2020 4120 6661 7374 2061 6e64 2063      A fast and c
-00003b80: 6f6e 7665 6e69 656e 7420 6675 6e63 7469  onvenient functi
-00003b90: 6f6e 2c20 6465 636f 6d70 7265 7373 6573  on, decompresses
-00003ba0: 202a 696e 7075 745f 7374 7265 616d 2a20   *input_stream* 
-00003bb0: 616e 6420 7772 6974 6573 2074 6865 2064  and writes the d
-00003bc0: 6563 6f6d 7072 6573 7365 6420 6461 7461  ecompressed data
-00003bd0: 2074 6f20 2a6f 7574 7075 745f 7374 7265   to *output_stre
-00003be0: 616d 2a2c 2069 7420 646f 6573 6e27 7420  am*, it doesn't 
-00003bf0: 636c 6f73 6520 7468 6520 7374 7265 616d  close the stream
-00003c00: 732e 0a0a 2020 2020 5375 7070 6f72 7473  s...    Supports
-00003c10: 206d 756c 7469 706c 6520 636f 6e63 6174   multiple concat
-00003c20: 656e 6174 6564 203a 7265 663a 6066 7261  enated :ref:`fra
-00003c30: 6d65 733c 6672 616d 655f 626c 6f63 6b3e  mes<frame_block>
-00003c40: 602e 0a0a 2020 2020 5468 6973 2066 756e  `...    This fun
-00003c50: 6374 696f 6e20 7472 6965 7320 746f 207a  ction tries to z
-00003c60: 6572 6f2d 636f 7079 2061 7320 6d75 6368  ero-copy as much
-00003c70: 2061 7320 706f 7373 6962 6c65 2e20 4966   as possible. If
-00003c80: 2074 6865 204f 5320 6861 7320 7265 6164   the OS has read
-00003c90: 2070 7265 6665 7463 6869 6e67 2061 6e64   prefetching and
-00003ca0: 2077 7269 7465 2062 7566 6665 722c 2069   write buffer, i
-00003cb0: 7420 6d61 7920 7065 7266 6f72 6d20 7468  t may perform th
-00003cc0: 6520 7461 736b 7320 2872 6561 642f 6465  e tasks (read/de
-00003cd0: 636f 6d70 7265 7373 2f77 7269 7465 2920  compress/write) 
-00003ce0: 696e 2070 6172 616c 6c65 6c20 746f 2073  in parallel to s
-00003cf0: 6f6d 6520 6465 6772 6565 2e0a 0a20 2020  ome degree...   
-00003d00: 2054 6865 2064 6566 6175 6c74 2076 616c   The default val
-00003d10: 7565 7320 6f66 202a 7265 6164 5f73 697a  ues of *read_siz
-00003d20: 652a 2061 6e64 202a 7772 6974 655f 7369  e* and *write_si
-00003d30: 7a65 2a20 7061 7261 6d65 7465 7273 2061  ze* parameters a
-00003d40: 7265 2074 6865 2062 7566 6665 7220 7369  re the buffer si
-00003d50: 7a65 7320 7265 636f 6d6d 656e 6465 6420  zes recommended 
-00003d60: 6279 207a 7374 642c 2069 6e63 7265 6173  by zstd, increas
-00003d70: 696e 6720 7468 656d 206d 6179 2062 6520  ing them may be 
-00003d80: 6661 7374 6572 2c20 616e 6420 7265 6475  faster, and redu
-00003d90: 6365 7320 7468 6520 6e75 6d62 6572 206f  ces the number o
-00003da0: 6620 6361 6c6c 6261 636b 2066 756e 6374  f callback funct
-00003db0: 696f 6e20 6361 6c6c 732e 0a0a 2020 2020  ion calls...    
-00003dc0: 2e2e 2076 6572 7369 6f6e 6164 6465 643a  .. versionadded:
-00003dd0: 3a20 302e 3134 2e32 0a0a 2020 2020 3a70  : 0.14.2..    :p
-00003de0: 6172 616d 2069 6e70 7574 5f73 7472 6561  aram input_strea
-00003df0: 6d3a 2049 6e70 7574 2073 7472 6561 6d20  m: Input stream 
-00003e00: 7468 6174 2068 6173 2061 2060 2e72 6561  that has a `.rea
-00003e10: 6469 6e74 6f28 6229 203c 6874 7470 733a  dinto(b) <https:
-00003e20: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00003e30: 672f 332f 6c69 6272 6172 792f 696f 2e68  g/3/library/io.h
-00003e40: 746d 6c23 696f 2e52 6177 494f 4261 7365  tml#io.RawIOBase
-00003e50: 2e72 6561 6469 6e74 6f3e 605f 206d 6574  .readinto>`_ met
-00003e60: 686f 642e 0a20 2020 203a 7061 7261 6d20  hod..    :param 
-00003e70: 6f75 7470 7574 5f73 7472 6561 6d3a 204f  output_stream: O
-00003e80: 7574 7075 7420 7374 7265 616d 2074 6861  utput stream tha
-00003e90: 7420 6861 7320 6120 602e 7772 6974 6528  t has a `.write(
-00003ea0: 6229 203c 6874 7470 733a 2f2f 646f 6373  b) <https://docs
-00003eb0: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-00003ec0: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
-00003ed0: 2e52 6177 494f 4261 7365 2e77 7269 7465  .RawIOBase.write
-00003ee0: 3e60 5f20 6d65 7468 6f64 2e20 4966 2075  >`_ method. If u
-00003ef0: 7365 202a 6361 6c6c 6261 636b 2a20 6675  se *callback* fu
-00003f00: 6e63 7469 6f6e 2c20 7468 6973 2070 6172  nction, this par
-00003f10: 616d 6574 6572 2063 616e 2062 6520 6060  ameter can be ``
-00003f20: 4e6f 6e65 6060 2e0a 2020 2020 3a70 6172  None``..    :par
-00003f30: 616d 207a 7374 645f 6469 6374 3a20 5072  am zstd_dict: Pr
-00003f40: 652d 7472 6169 6e65 6420 6469 6374 696f  e-trained dictio
-00003f50: 6e61 7279 2066 6f72 2064 6563 6f6d 7072  nary for decompr
-00003f60: 6573 7369 6f6e 2e0a 2020 2020 3a74 7970  ession..    :typ
-00003f70: 6520 7a73 7464 5f64 6963 743a 205a 7374  e zstd_dict: Zst
-00003f80: 6444 6963 740a 2020 2020 3a70 6172 616d  dDict.    :param
-00003f90: 206f 7074 696f 6e3a 2041 2060 6064 6963   option: A ``dic
-00003fa0: 7460 6020 6f62 6a65 6374 2c20 636f 6e74  t`` object, cont
-00003fb0: 6169 6e73 203a 7265 663a 6061 6476 616e  ains :ref:`advan
-00003fc0: 6365 6420 6465 636f 6d70 7265 7373 696f  ced decompressio
-00003fd0: 6e20 7061 7261 6d65 7465 7273 3c44 5061  n parameters<DPa
-00003fe0: 7261 6d65 7465 723e 602e 0a20 2020 203a  rameter>`..    :
-00003ff0: 7479 7065 206f 7074 696f 6e3a 2064 6963  type option: dic
-00004000: 740a 2020 2020 3a70 6172 616d 2072 6561  t.    :param rea
-00004010: 645f 7369 7a65 3a20 496e 7075 7420 6275  d_size: Input bu
-00004020: 6666 6572 2073 697a 652c 2069 6e20 6279  ffer size, in by
-00004030: 7465 732e 0a20 2020 203a 7479 7065 2072  tes..    :type r
-00004040: 6561 645f 7369 7a65 3a20 696e 740a 2020  ead_size: int.  
-00004050: 2020 3a70 6172 616d 2077 7269 7465 5f73    :param write_s
-00004060: 697a 653a 204f 7574 7075 7420 6275 6666  ize: Output buff
-00004070: 6572 2073 697a 652c 2069 6e20 6279 7465  er size, in byte
-00004080: 732e 0a20 2020 203a 7479 7065 2077 7269  s..    :type wri
-00004090: 7465 5f73 697a 653a 2069 6e74 0a20 2020  te_size: int.   
-000040a0: 203a 7061 7261 6d20 6361 6c6c 6261 636b   :param callback
-000040b0: 3a20 4120 6361 6c6c 6261 636b 2066 756e  : A callback fun
-000040c0: 6374 696f 6e20 7468 6174 2061 6363 6570  ction that accep
-000040d0: 7473 2066 6f75 7220 7061 7261 6d65 7465  ts four paramete
-000040e0: 7273 3a20 6060 2874 6f74 616c 5f69 6e70  rs: ``(total_inp
-000040f0: 7574 2c20 746f 7461 6c5f 6f75 7470 7574  ut, total_output
-00004100: 2c20 7265 6164 5f64 6174 612c 2077 7269  , read_data, wri
-00004110: 7465 5f64 6174 6129 6060 2e20 5468 6520  te_data)``. The 
-00004120: 6669 7273 7420 7477 6f20 6172 6520 6060  first two are ``
-00004130: 696e 7460 6020 6f62 6a65 6374 732e 2054  int`` objects. T
-00004140: 6865 206c 6173 7420 7477 6f20 6172 6520  he last two are 
-00004150: 7265 6164 6f6e 6c79 2060 6d65 6d6f 7279  readonly `memory
-00004160: 7669 6577 203c 6874 7470 733a 2f2f 646f  view <https://do
-00004170: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-00004180: 6c69 6272 6172 792f 7374 6474 7970 6573  library/stdtypes
-00004190: 2e68 746d 6c23 6d65 6d6f 7279 2d76 6965  .html#memory-vie
-000041a0: 7773 3e60 5f20 6f62 6a65 6374 732c 2069  ws>`_ objects, i
-000041b0: 6620 7761 6e74 2074 6f20 7265 6665 7265  f want to refere
-000041c0: 6e63 6520 7468 6520 6461 7461 2028 6f72  nce the data (or
-000041d0: 2069 7473 2073 6c69 6365 2920 6f75 7473   its slice) outs
-000041e0: 6964 6520 7468 6520 6361 6c6c 6261 636b  ide the callback
-000041f0: 2066 756e 6374 696f 6e2c 2060 636f 6e76   function, `conv
-00004200: 6572 7420 3c68 7474 7073 3a2f 2f64 6f63  ert <https://doc
-00004210: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-00004220: 6962 7261 7279 2f73 7464 7479 7065 732e  ibrary/stdtypes.
-00004230: 6874 6d6c 236d 656d 6f72 7976 6965 772e  html#memoryview.
-00004240: 746f 6279 7465 733e 605f 2074 6865 6d20  tobytes>`_ them 
-00004250: 746f 2060 6062 7974 6573 6060 206f 626a  to ``bytes`` obj
-00004260: 6563 7473 2e20 4966 2069 6e70 7574 2073  ects. If input s
-00004270: 7472 6561 6d20 6973 2060 6062 2727 6060  tream is ``b''``
-00004280: 2c20 7468 6520 6361 6c6c 6261 636b 2066  , the callback f
-00004290: 756e 6374 696f 6e20 7769 6c6c 206e 6f74  unction will not
-000042a0: 2062 6520 6361 6c6c 6564 2e0a 2020 2020   be called..    
-000042b0: 3a74 7970 6520 6361 6c6c 6261 636b 3a20  :type callback: 
-000042c0: 6361 6c6c 6162 6c65 0a20 2020 203a 7265  callable.    :re
-000042d0: 7475 726e 3a20 4120 322d 6974 656d 2074  turn: A 2-item t
-000042e0: 7570 6c65 2c20 6060 2874 6f74 616c 5f69  uple, ``(total_i
-000042f0: 6e70 7574 2c20 746f 7461 6c5f 6f75 7470  nput, total_outp
-00004300: 7574 2960 602c 2074 6865 2069 7465 6d73  ut)``, the items
-00004310: 2061 7265 2060 6069 6e74 6060 206f 626a   are ``int`` obj
-00004320: 6563 7473 2e0a 2020 2020 3a72 6169 7365  ects..    :raise
-00004330: 7320 5a73 7464 4572 726f 723a 2049 6620  s ZstdError: If 
-00004340: 6465 636f 6d70 7265 7373 696f 6e20 6661  decompression fa
-00004350: 696c 732e 0a0a 2020 2020 2e2e 2073 6f75  ils...    .. sou
-00004360: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
-00004370: 0a0a 2020 2020 2020 2020 2320 6465 636f  ..        # deco
-00004380: 6d70 7265 7373 2061 6e20 696e 7075 7420  mpress an input 
-00004390: 6669 6c65 2c20 616e 6420 7772 6974 6520  file, and write 
-000043a0: 746f 2061 6e20 6f75 7470 7574 2066 696c  to an output fil
-000043b0: 652e 0a20 2020 2020 2020 2077 6974 6820  e..        with 
-000043c0: 696f 2e6f 7065 6e28 696e 7075 745f 6669  io.open(input_fi
-000043d0: 6c65 5f70 6174 682c 2027 7262 2729 2061  le_path, 'rb') a
-000043e0: 7320 6966 683a 0a20 2020 2020 2020 2020  s ifh:.         
-000043f0: 2020 2077 6974 6820 696f 2e6f 7065 6e28     with io.open(
-00004400: 6f75 7470 7574 5f66 696c 655f 7061 7468  output_file_path
-00004410: 2c20 2777 6227 2920 6173 206f 6668 3a0a  , 'wb') as ofh:.
-00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 6465 636f 6d70 7265 7373 5f73 7472 6561  decompress_strea
-00004440: 6d28 6966 682c 206f 6668 290a 0a20 2020  m(ifh, ofh)..   
-00004450: 2020 2020 2023 2064 6563 6f6d 7072 6573       # decompres
-00004460: 7320 6120 6279 7465 7320 6f62 6a65 6374  s a bytes object
-00004470: 2c20 616e 6420 7772 6974 6520 746f 2061  , and write to a
-00004480: 2066 696c 652e 0a20 2020 2020 2020 2077   file..        w
-00004490: 6974 6820 696f 2e42 7974 6573 494f 2863  ith io.BytesIO(c
-000044a0: 6f6d 7072 6573 7365 645f 6461 7429 2061  ompressed_dat) a
-000044b0: 7320 6269 3a0a 2020 2020 2020 2020 2020  s bi:.          
-000044c0: 2020 7769 7468 2069 6f2e 6f70 656e 286f    with io.open(o
-000044d0: 7574 7075 745f 6669 6c65 5f70 6174 682c  utput_file_path,
-000044e0: 2027 7762 2729 2061 7320 6f66 683a 0a20   'wb') as ofh:. 
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004500: 6563 6f6d 7072 6573 735f 7374 7265 616d  ecompress_stream
-00004510: 2862 692c 206f 6668 290a 0a20 2020 2020  (bi, ofh)..     
-00004520: 2020 2023 2044 6563 6f6d 7072 6573 7320     # Decompress 
-00004530: 616e 2069 6e70 7574 2066 696c 652c 206f  an input file, o
-00004540: 6274 6169 6e20 6120 6279 7465 7320 6f62  btain a bytes ob
-00004550: 6a65 6374 2e0a 2020 2020 2020 2020 2320  ject..        # 
-00004560: 4974 2773 2066 6173 7465 7220 7468 616e  It's faster than
-00004570: 2072 6561 6469 6e67 2061 2066 696c 6520   reading a file 
-00004580: 616e 6420 6465 636f 6d70 7265 7373 696e  and decompressin
-00004590: 6720 6974 2069 6e0a 2020 2020 2020 2020  g it in.        
-000045a0: 2320 6d65 6d6f 7279 2c20 7465 7374 6564  # memory, tested
-000045b0: 206f 6e20 5562 756e 7475 2850 7974 686f   on Ubuntu(Pytho
-000045c0: 6e33 2e38 292f 5769 6e64 6f77 7328 5079  n3.8)/Windows(Py
-000045d0: 7468 6f6e 332e 3929 2e0a 2020 2020 2020  thon3.9)..      
-000045e0: 2020 2320 4d61 7962 6520 7468 6520 4f53    # Maybe the OS
-000045f0: 2068 6173 2070 7265 6665 7463 6869 6e67   has prefetching
-00004600: 2c20 6974 2063 616e 2072 6561 6420 616e  , it can read an
-00004610: 6420 6465 636f 6d70 7265 7373 0a20 2020  d decompress.   
-00004620: 2020 2020 2023 2064 6174 6120 696e 2070       # data in p
-00004630: 6172 616c 6c65 6c20 746f 2073 6f6d 6520  arallel to some 
-00004640: 6465 6772 6565 2c20 7265 6164 696e 6720  degree, reading 
-00004650: 6669 6c65 2066 726f 6d20 4844 440a 2020  file from HDD.  
-00004660: 2020 2020 2020 2320 6973 2074 6865 2062        # is the b
-00004670: 6f74 746c 656e 6563 6b20 696e 2074 6869  ottleneck in thi
-00004680: 7320 6361 7365 2e0a 2020 2020 2020 2020  s case..        
-00004690: 7769 7468 2069 6f2e 6f70 656e 2869 6e70  with io.open(inp
-000046a0: 7574 5f66 696c 655f 7061 7468 2c20 2772  ut_file_path, 'r
-000046b0: 6227 2920 6173 2069 6668 3a0a 2020 2020  b') as ifh:.    
-000046c0: 2020 2020 2020 2020 7769 7468 2069 6f2e          with io.
-000046d0: 4279 7465 7349 4f28 2920 6173 2062 6f3a  BytesIO() as bo:
-000046e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000046f0: 2064 6563 6f6d 7072 6573 735f 7374 7265   decompress_stre
-00004700: 616d 2869 6668 2c20 626f 290a 2020 2020  am(ifh, bo).    
-00004710: 2020 2020 2020 2020 2020 2020 6465 636f              deco
-00004720: 6d70 7265 7373 6564 5f64 6174 203d 2062  mpressed_dat = b
-00004730: 6f2e 6765 7476 616c 7565 2829 0a0a 2020  o.getvalue()..  
-00004740: 2020 2020 2020 2320 5072 696e 7420 7072        # Print pr
-00004750: 6f67 7265 7373 2075 7369 6e67 2063 616c  ogress using cal
-00004760: 6c62 6163 6b20 6675 6e63 7469 6f6e 0a20  lback function. 
-00004770: 2020 2020 2020 2064 6566 2064 6563 6f6d         def decom
-00004780: 7072 6573 735f 7072 696e 745f 7072 6f67  press_print_prog
-00004790: 7265 7373 2869 6e70 7574 5f66 696c 655f  ress(input_file_
-000047a0: 7061 7468 2c20 6f75 7470 7574 5f66 696c  path, output_fil
-000047b0: 655f 7061 7468 293a 0a20 2020 2020 2020  e_path):.       
-000047c0: 2020 2020 2069 6e70 7574 5f66 696c 655f       input_file_
-000047d0: 7369 7a65 203d 206f 732e 7061 7468 2e67  size = os.path.g
-000047e0: 6574 7369 7a65 2869 6e70 7574 5f66 696c  etsize(input_fil
-000047f0: 655f 7061 7468 290a 0a20 2020 2020 2020  e_path)..       
-00004800: 2020 2020 2064 6566 2066 756e 6328 746f       def func(to
-00004810: 7461 6c5f 696e 7075 742c 2074 6f74 616c  tal_input, total
-00004820: 5f6f 7574 7075 742c 2072 6561 645f 6461  _output, read_da
-00004830: 7461 2c20 7772 6974 655f 6461 7461 293a  ta, write_data):
-00004840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004850: 2023 2049 6620 696e 7075 7420 7374 7265   # If input stre
-00004860: 616d 2069 7320 656d 7074 792c 2074 6865  am is empty, the
-00004870: 2063 616c 6c62 6163 6b20 6675 6e63 7469   callback functi
-00004880: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-00004890: 2020 2023 2077 696c 6c20 6e6f 7420 6265     # will not be
-000048a0: 2063 616c 6c65 642e 2053 6f20 6e6f 205a   called. So no Z
-000048b0: 6572 6f44 6976 6973 696f 6e45 7272 6f72  eroDivisionError
-000048c0: 2068 6572 652e 0a20 2020 2020 2020 2020   here..         
-000048d0: 2020 2020 2020 2070 6572 6365 6e74 203d         percent =
-000048e0: 2031 3030 202a 2074 6f74 616c 5f69 6e70   100 * total_inp
-000048f0: 7574 202f 2069 6e70 7574 5f66 696c 655f  ut / input_file_
-00004900: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
-00004910: 2020 2020 2070 7269 6e74 2866 2750 726f       print(f'Pro
-00004920: 6772 6573 733a 207b 7065 7263 656e 743a  gress: {percent:
-00004930: 2e31 667d 2527 2c20 656e 643d 275c 7227  .1f}%', end='\r'
-00004940: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
-00004950: 6974 6820 696f 2e6f 7065 6e28 696e 7075  ith io.open(inpu
-00004960: 745f 6669 6c65 5f70 6174 682c 2027 7262  t_file_path, 'rb
-00004970: 2729 2061 7320 6966 683a 0a20 2020 2020  ') as ifh:.     
-00004980: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00004990: 696f 2e6f 7065 6e28 6f75 7470 7574 5f66  io.open(output_f
-000049a0: 696c 655f 7061 7468 2c20 2777 6227 2920  ile_path, 'wb') 
-000049b0: 6173 206f 6668 3a0a 2020 2020 2020 2020  as ofh:.        
-000049c0: 2020 2020 2020 2020 2020 2020 6465 636f              deco
-000049d0: 6d70 7265 7373 5f73 7472 6561 6d28 6966  mpress_stream(if
-000049e0: 682c 206f 6668 2c20 6361 6c6c 6261 636b  h, ofh, callback
-000049f0: 3d66 756e 6329 0a0a 0a2e 2e20 7079 3a63  =func)..... py:c
-00004a00: 6c61 7373 3a3a 205a 7374 6444 6563 6f6d  lass:: ZstdDecom
-00004a10: 7072 6573 736f 720a 0a20 2020 2041 2073  pressor..    A s
-00004a20: 7472 6561 6d69 6e67 2064 6563 6f6d 7072  treaming decompr
-00004a30: 6573 736f 722e 0a0a 2020 2020 4166 7465  essor...    Afte
-00004a40: 7220 6120 3a72 6566 3a60 6672 616d 653c  r a :ref:`frame<
-00004a50: 6672 616d 655f 626c 6f63 6b3e 6020 6973  frame_block>` is
-00004a60: 2064 6563 6f6d 7072 6573 7365 642c 2069   decompressed, i
-00004a70: 7420 7374 6f70 7320 616e 6420 7365 7473  t stops and sets
-00004a80: 203a 7079 3a61 7474 723a 607e 5a73 7464   :py:attr:`~Zstd
-00004a90: 4465 636f 6d70 7265 7373 6f72 2e65 6f66  Decompressor.eof
-00004aa0: 6020 666c 6167 2074 6f20 6060 5472 7565  ` flag to ``True
-00004ab0: 6060 2e0a 0a20 2020 2046 6f72 206d 756c  ``...    For mul
-00004ac0: 7469 706c 6520 6672 616d 6573 2064 6174  tiple frames dat
-00004ad0: 612c 2075 7365 203a 7079 3a63 6c61 7373  a, use :py:class
-00004ae0: 3a60 456e 646c 6573 735a 7374 6444 6563  :`EndlessZstdDec
-00004af0: 6f6d 7072 6573 736f 7260 2e0a 0a20 2020  ompressor`...   
-00004b00: 2054 6872 6561 642d 7361 6665 2061 7420   Thread-safe at 
-00004b10: 6d65 7468 6f64 206c 6576 656c 2e0a 0a20  method level... 
-00004b20: 2020 202e 2e20 7079 3a6d 6574 686f 643a     .. py:method:
-00004b30: 3a20 5f5f 696e 6974 5f5f 2873 656c 662c  : __init__(self,
-00004b40: 207a 7374 645f 6469 6374 3d4e 6f6e 652c   zstd_dict=None,
-00004b50: 206f 7074 696f 6e3d 4e6f 6e65 290a 0a20   option=None).. 
-00004b60: 2020 2020 2020 2049 6e69 7469 616c 697a         Initializ
-00004b70: 6520 6120 5a73 7464 4465 636f 6d70 7265  e a ZstdDecompre
-00004b80: 7373 6f72 206f 626a 6563 742e 0a0a 2020  ssor object...  
-00004b90: 2020 2020 2020 3a70 6172 616d 207a 7374        :param zst
-00004ba0: 645f 6469 6374 3a20 5072 652d 7472 6169  d_dict: Pre-trai
-00004bb0: 6e65 6420 6469 6374 696f 6e61 7279 2066  ned dictionary f
-00004bc0: 6f72 2064 6563 6f6d 7072 6573 7369 6f6e  or decompression
-00004bd0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00004be0: 7a73 7464 5f64 6963 743a 205a 7374 6444  zstd_dict: ZstdD
-00004bf0: 6963 740a 2020 2020 2020 2020 3a70 6172  ict.        :par
-00004c00: 616d 2064 6963 7420 6f70 7469 6f6e 3a20  am dict option: 
-00004c10: 4120 6060 6469 6374 6060 206f 626a 6563  A ``dict`` objec
-00004c20: 7420 7468 6174 2063 6f6e 7461 696e 7320  t that contains 
-00004c30: 3a72 6566 3a60 6164 7661 6e63 6564 2064  :ref:`advanced d
-00004c40: 6563 6f6d 7072 6573 7369 6f6e 2070 6172  ecompression par
-00004c50: 616d 6574 6572 733c 4450 6172 616d 6574  ameters<DParamet
-00004c60: 6572 3e60 2e20 5468 6520 6465 6661 756c  er>`. The defaul
-00004c70: 7420 7661 6c75 6520 6060 4e6f 6e65 6060  t value ``None``
-00004c80: 206d 6561 6e73 2074 6f20 7573 6520 7a73   means to use zs
-00004c90: 7464 2773 2064 6566 6175 6c74 2064 6563  td's default dec
-00004ca0: 6f6d 7072 6573 7369 6f6e 2070 6172 616d  ompression param
-00004cb0: 6574 6572 732e 0a0a 2020 2020 2e2e 2070  eters...    .. p
-00004cc0: 793a 6d65 7468 6f64 3a3a 2064 6563 6f6d  y:method:: decom
-00004cd0: 7072 6573 7328 7365 6c66 2c20 6461 7461  press(self, data
-00004ce0: 2c20 6d61 785f 6c65 6e67 7468 3d2d 3129  , max_length=-1)
-00004cf0: 0a0a 2020 2020 2020 2020 4465 636f 6d70  ..        Decomp
-00004d00: 7265 7373 202a 6461 7461 2a2c 2072 6574  ress *data*, ret
-00004d10: 7572 6e69 6e67 2064 6563 6f6d 7072 6573  urning decompres
-00004d20: 7365 6420 6461 7461 2061 7320 6120 6060  sed data as a ``
-00004d30: 6279 7465 7360 6020 6f62 6a65 6374 2e0a  bytes`` object..
-00004d40: 0a20 2020 2020 2020 2041 6674 6572 2061  .        After a
-00004d50: 203a 7265 663a 6066 7261 6d65 3c66 7261   :ref:`frame<fra
-00004d60: 6d65 5f62 6c6f 636b 3e60 2069 7320 6465  me_block>` is de
-00004d70: 636f 6d70 7265 7373 6564 2c20 6974 2073  compressed, it s
-00004d80: 746f 7073 2061 6e64 2073 6574 7320 3a70  tops and sets :p
-00004d90: 793a 6174 7472 3a60 7e5a 7374 6444 6563  y:attr:`~ZstdDec
-00004da0: 6f6d 7072 6573 736f 722e 656f 6660 2066  ompressor.eof` f
-00004db0: 6c61 6720 746f 2060 6054 7275 6560 602e  lag to ``True``.
-00004dc0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00004dd0: 2064 6174 613a 2044 6174 6120 746f 2062   data: Data to b
-00004de0: 6520 6465 636f 6d70 7265 7373 6564 2e0a  e decompressed..
-00004df0: 2020 2020 2020 2020 3a74 7970 6520 6461          :type da
-00004e00: 7461 3a20 6279 7465 732d 6c69 6b65 206f  ta: bytes-like o
-00004e10: 626a 6563 740a 2020 2020 2020 2020 3a70  bject.        :p
-00004e20: 6172 616d 2069 6e74 206d 6178 5f6c 656e  aram int max_len
-00004e30: 6774 683a 204d 6178 696d 756d 2073 697a  gth: Maximum siz
-00004e40: 6520 6f66 2072 6574 7572 6e65 6420 6461  e of returned da
-00004e50: 7461 2e20 5768 656e 2069 7427 7320 6e65  ta. When it's ne
-00004e60: 6761 7469 7665 2c20 7468 6520 6f75 7470  gative, the outp
-00004e70: 7574 2073 697a 6520 6973 2075 6e6c 696d  ut size is unlim
-00004e80: 6974 6564 2e20 5768 656e 2069 7427 7320  ited. When it's 
-00004e90: 6e6f 6e2d 6e65 6761 7469 7665 2c20 7265  non-negative, re
-00004ea0: 7475 726e 7320 6174 206d 6f73 7420 2a6d  turns at most *m
-00004eb0: 6178 5f6c 656e 6774 682a 2062 7974 6573  ax_length* bytes
-00004ec0: 206f 6620 6465 636f 6d70 7265 7373 6564   of decompressed
-00004ed0: 2064 6174 612e 2049 6620 7468 6973 206c   data. If this l
-00004ee0: 696d 6974 2069 7320 7265 6163 6865 6420  imit is reached 
-00004ef0: 616e 6420 6675 7274 6865 7220 6f75 7470  and further outp
-00004f00: 7574 2063 616e 2028 6f72 206d 6179 2920  ut can (or may) 
-00004f10: 6265 2070 726f 6475 6365 642c 2074 6865  be produced, the
-00004f20: 203a 7079 3a61 7474 723a 607e 5a73 7464   :py:attr:`~Zstd
-00004f30: 4465 636f 6d70 7265 7373 6f72 2e6e 6565  Decompressor.nee
-00004f40: 6473 5f69 6e70 7574 6020 6174 7472 6962  ds_input` attrib
-00004f50: 7574 6520 7769 6c6c 2062 6520 7365 7420  ute will be set 
-00004f60: 746f 2060 6046 616c 7365 6060 2e20 496e  to ``False``. In
-00004f70: 2074 6869 7320 6361 7365 2c20 7468 6520   this case, the 
-00004f80: 6e65 7874 2063 616c 6c20 746f 2074 6869  next call to thi
-00004f90: 7320 6d65 7468 6f64 206d 6179 2070 726f  s method may pro
-00004fa0: 7669 6465 202a 6461 7461 2a20 6173 2060  vide *data* as `
-00004fb0: 6062 2727 6060 2074 6f20 6f62 7461 696e  `b''`` to obtain
-00004fc0: 206d 6f72 6520 6f66 2074 6865 206f 7574   more of the out
-00004fd0: 7075 742e 0a0a 2020 2020 2e2e 2070 793a  put...    .. py:
-00004fe0: 6174 7472 6962 7574 653a 3a20 6e65 6564  attribute:: need
-00004ff0: 735f 696e 7075 740a 0a20 2020 2020 2020  s_input..       
-00005000: 2049 6620 7468 6520 2a6d 6178 5f6c 656e   If the *max_len
-00005010: 6774 682a 206f 7574 7075 7420 6c69 6d69  gth* output limi
-00005020: 7420 696e 203a 7079 3a6d 6574 683a 607e  t in :py:meth:`~
-00005030: 5a73 7464 4465 636f 6d70 7265 7373 6f72  ZstdDecompressor
-00005040: 2e64 6563 6f6d 7072 6573 7360 206d 6574  .decompress` met
-00005050: 686f 6420 6861 7320 6265 656e 2072 6561  hod has been rea
-00005060: 6368 6564 2c20 616e 6420 7468 6520 6465  ched, and the de
-00005070: 636f 6d70 7265 7373 6f72 2068 6173 2028  compressor has (
-00005080: 6f72 206d 6179 2068 6173 2920 756e 636f  or may has) unco
-00005090: 6e73 756d 6564 2069 6e70 7574 2064 6174  nsumed input dat
-000050a0: 612c 2069 7420 7769 6c6c 2062 6520 7365  a, it will be se
-000050b0: 7420 746f 2060 6046 616c 7365 6060 2e20  t to ``False``. 
-000050c0: 496e 2074 6869 7320 6361 7365 2c20 7061  In this case, pa
-000050d0: 7373 2060 6062 2727 6060 2074 6f20 3a70  ss ``b''`` to :p
-000050e0: 793a 6d65 7468 3a60 7e5a 7374 6444 6563  y:meth:`~ZstdDec
-000050f0: 6f6d 7072 6573 736f 722e 6465 636f 6d70  ompressor.decomp
-00005100: 7265 7373 6020 6d65 7468 6f64 206d 6179  ress` method may
-00005110: 206f 7574 7075 7420 6675 7274 6865 7220   output further 
-00005120: 6461 7461 2e0a 0a20 2020 2020 2020 2049  data...        I
-00005130: 6620 6967 6e6f 7265 2074 6869 7320 6174  f ignore this at
-00005140: 7472 6962 7574 6520 7768 656e 2074 6865  tribute when the
-00005150: 7265 2069 7320 756e 636f 6e73 756d 6564  re is unconsumed
-00005160: 2069 6e70 7574 2064 6174 612c 2074 6865   input data, the
-00005170: 7265 2077 696c 6c20 6265 2061 206c 6974  re will be a lit
-00005180: 746c 6520 7065 7266 6f72 6d61 6e63 6520  tle performance 
-00005190: 6c6f 7373 2062 6563 6175 7365 206f 6620  loss because of 
-000051a0: 6578 7472 6120 6d65 6d6f 7279 2063 6f70  extra memory cop
-000051b0: 792e 0a0a 2020 2020 2e2e 2070 793a 6174  y...    .. py:at
-000051c0: 7472 6962 7574 653a 3a20 656f 660a 0a20  tribute:: eof.. 
-000051d0: 2020 2020 2020 2060 6054 7275 6560 6020         ``True`` 
-000051e0: 6d65 616e 7320 7468 6520 656e 6420 6f66  means the end of
-000051f0: 2074 6865 2066 6972 7374 2066 7261 6d65   the first frame
-00005200: 2068 6173 2062 6565 6e20 7265 6163 6865   has been reache
-00005210: 642e 2049 6620 6465 636f 6d70 7265 7373  d. If decompress
-00005220: 2064 6174 6120 6166 7465 7220 7468 6174   data after that
-00005230: 2c20 616e 2060 6045 4f46 4572 726f 7260  , an ``EOFError`
-00005240: 6020 6578 6365 7074 696f 6e20 7769 6c6c  ` exception will
-00005250: 2062 6520 7261 6973 6564 2e0a 0a20 2020   be raised...   
-00005260: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
-00005270: 3a3a 2075 6e75 7365 645f 6461 7461 0a0a  :: unused_data..
-00005280: 2020 2020 2020 2020 4120 6279 7465 7320          A bytes 
-00005290: 6f62 6a65 6374 2e20 5768 656e 205a 7374  object. When Zst
-000052a0: 6444 6563 6f6d 7072 6573 736f 7220 6f62  dDecompressor ob
-000052b0: 6a65 6374 2073 746f 7073 2061 6674 6572  ject stops after
-000052c0: 2064 6563 6f6d 7072 6573 7369 6e67 2061   decompressing a
-000052d0: 2066 7261 6d65 2c20 756e 7573 6564 2069   frame, unused i
-000052e0: 6e70 7574 2064 6174 6120 6166 7465 7220  nput data after 
-000052f0: 7468 6520 6669 7273 7420 6672 616d 652e  the first frame.
-00005300: 204f 7468 6572 7769 7365 2074 6869 7320   Otherwise this 
-00005310: 7769 6c6c 2062 6520 6060 6227 2760 602e  will be ``b''``.
-00005320: 0a0a 2020 2020 2e2e 2073 6f75 7263 6563  ..    .. sourcec
-00005330: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
-00005340: 2020 2020 2020 2320 2d2d 2d20 756e 6c69        # --- unli
-00005350: 6d69 7465 6420 6f75 7470 7574 202d 2d2d  mited output ---
-00005360: 0a20 2020 2020 2020 2064 3120 3d20 5a73  .        d1 = Zs
-00005370: 7464 4465 636f 6d70 7265 7373 6f72 2829  tdDecompressor()
-00005380: 0a0a 2020 2020 2020 2020 6465 636f 6d70  ..        decomp
-00005390: 7265 7373 6564 5f64 6174 3120 3d20 6431  ressed_dat1 = d1
-000053a0: 2e64 6563 6f6d 7072 6573 7328 6461 7431  .decompress(dat1
-000053b0: 290a 2020 2020 2020 2020 6465 636f 6d70  ).        decomp
-000053c0: 7265 7373 6564 5f64 6174 3220 3d20 6431  ressed_dat2 = d1
-000053d0: 2e64 6563 6f6d 7072 6573 7328 6461 7432  .decompress(dat2
-000053e0: 290a 2020 2020 2020 2020 6465 636f 6d70  ).        decomp
-000053f0: 7265 7373 6564 5f64 6174 3320 3d20 6431  ressed_dat3 = d1
-00005400: 2e64 6563 6f6d 7072 6573 7328 6461 7433  .decompress(dat3
-00005410: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00005420: 7420 6431 2e65 6f66 2c20 2764 6174 6120  t d1.eof, 'data 
-00005430: 6973 2061 6e20 696e 636f 6d70 6c65 7465  is an incomplete
-00005440: 207a 7374 6420 6672 616d 652e 270a 0a20   zstd frame.'.. 
-00005450: 2020 2020 2020 2023 202d 2d2d 206c 696d         # --- lim
-00005460: 6974 6564 206f 7574 7075 7420 2d2d 2d0a  ited output ---.
-00005470: 2020 2020 2020 2020 6432 203d 205a 7374          d2 = Zst
-00005480: 6444 6563 6f6d 7072 6573 736f 7228 290a  dDecompressor().
-00005490: 0a20 2020 2020 2020 2077 6869 6c65 2054  .        while T
-000054a0: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
-000054b0: 2069 6620 6432 2e6e 6565 6473 5f69 6e70   if d2.needs_inp
-000054c0: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
-000054d0: 2020 2020 6461 7420 3d20 7265 6164 5f69      dat = read_i
-000054e0: 6e70 7574 2832 2a31 3032 342a 3130 3234  nput(2*1024*1024
-000054f0: 2920 2320 7265 6164 2032 204d 6942 2069  ) # read 2 MiB i
-00005500: 6e70 7574 2064 6174 610a 2020 2020 2020  nput data.      
-00005510: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00005520: 2064 6174 3a20 2320 696e 7075 7420 7374   dat: # input st
-00005530: 7265 616d 2065 6e64 730a 2020 2020 2020  ream ends.      
-00005540: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00005550: 6973 6520 4578 6365 7074 696f 6e28 2749  ise Exception('I
-00005560: 6e70 7574 2073 7472 6561 6d20 656e 6473  nput stream ends
-00005570: 2c20 6275 7420 7468 6520 656e 6420 6f66  , but the end of
-00005580: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055a0: 2020 2020 2020 2027 7468 6520 6669 7273         'the firs
-000055b0: 7420 6672 616d 6520 6973 206e 6f74 2072  t frame is not r
-000055c0: 6561 6368 6564 2e27 290a 2020 2020 2020  eached.').      
-000055d0: 2020 2020 2020 656c 7365 3a20 2320 6d61        else: # ma
-000055e0: 7962 6520 7468 6572 6520 6973 2075 6e63  ybe there is unc
-000055f0: 6f6e 7375 6d65 6420 696e 7075 7420 6461  onsumed input da
-00005600: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
-00005610: 2020 2064 6174 203d 2062 2727 0a0a 2020     dat = b''..  
-00005620: 2020 2020 2020 2020 2020 6368 756e 6b20            chunk 
-00005630: 3d20 6432 2e64 6563 6f6d 7072 6573 7328  = d2.decompress(
-00005640: 6461 742c 2031 302a 3130 3234 2a31 3032  dat, 10*1024*102
-00005650: 3429 2023 206c 696d 6974 206f 7574 7075  4) # limit outpu
-00005660: 7420 6275 6666 6572 2074 6f20 3130 204d  t buffer to 10 M
-00005670: 6942 0a20 2020 2020 2020 2020 2020 2077  iB.            w
-00005680: 7269 7465 5f6f 7574 7075 7428 6368 756e  rite_output(chun
-00005690: 6b29 0a0a 2020 2020 2020 2020 2020 2020  k)..            
-000056a0: 6966 2064 322e 656f 663a 2023 2072 6561  if d2.eof: # rea
-000056b0: 6368 2074 6865 2065 6e64 206f 6620 7468  ch the end of th
-000056c0: 6520 6669 7273 7420 6672 616d 650a 2020  e first frame.  
-000056d0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-000056e0: 6561 6b0a 0a0a 2e2e 2070 793a 636c 6173  eak..... py:clas
-000056f0: 733a 3a20 456e 646c 6573 735a 7374 6444  s:: EndlessZstdD
-00005700: 6563 6f6d 7072 6573 736f 720a 0a20 2020  ecompressor..   
-00005710: 2041 2073 7472 6561 6d69 6e67 2064 6563   A streaming dec
-00005720: 6f6d 7072 6573 736f 722e 0a0a 2020 2020  ompressor...    
-00005730: 4974 2064 6f65 736e 2774 2073 746f 7020  It doesn't stop 
-00005740: 6166 7465 7220 6120 3a72 6566 3a60 6672  after a :ref:`fr
-00005750: 616d 653c 6672 616d 655f 626c 6f63 6b3e  ame<frame_block>
-00005760: 6020 6973 2064 6563 6f6d 7072 6573 7365  ` is decompresse
-00005770: 642c 2063 616e 2062 6520 7573 6564 2074  d, can be used t
-00005780: 6f20 6465 636f 6d70 7265 7373 206d 756c  o decompress mul
-00005790: 7469 706c 6520 636f 6e63 6174 656e 6174  tiple concatenat
-000057a0: 6564 2066 7261 6d65 732e 0a0a 2020 2020  ed frames...    
-000057b0: 5468 7265 6164 2d73 6166 6520 6174 206d  Thread-safe at m
-000057c0: 6574 686f 6420 6c65 7665 6c2e 0a0a 2020  ethod level...  
-000057d0: 2020 2e2e 2070 793a 6d65 7468 6f64 3a3a    .. py:method::
-000057e0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-000057f0: 7a73 7464 5f64 6963 743d 4e6f 6e65 2c20  zstd_dict=None, 
-00005800: 6f70 7469 6f6e 3d4e 6f6e 6529 0a0a 2020  option=None)..  
-00005810: 2020 2020 2020 5468 6520 7061 7261 6d65        The parame
-00005820: 7465 7273 2061 7265 2074 6865 2073 616d  ters are the sam
-00005830: 6520 6173 203a 7079 3a6d 6574 683a 605a  e as :py:meth:`Z
-00005840: 7374 6444 6563 6f6d 7072 6573 736f 722e  stdDecompressor.
-00005850: 5f5f 696e 6974 5f5f 6020 6d65 7468 6f64  __init__` method
-00005860: 2e0a 0a20 2020 202e 2e20 7079 3a6d 6574  ...    .. py:met
-00005870: 686f 643a 3a20 6465 636f 6d70 7265 7373  hod:: decompress
-00005880: 2873 656c 662c 2064 6174 612c 206d 6178  (self, data, max
-00005890: 5f6c 656e 6774 683d 2d31 290a 0a20 2020  _length=-1)..   
-000058a0: 2020 2020 2054 6865 2070 6172 616d 6574       The paramet
-000058b0: 6572 7320 6172 6520 7468 6520 7361 6d65  ers are the same
-000058c0: 2061 7320 3a70 793a 6d65 7468 3a60 5a73   as :py:meth:`Zs
-000058d0: 7464 4465 636f 6d70 7265 7373 6f72 2e64  tdDecompressor.d
-000058e0: 6563 6f6d 7072 6573 7360 206d 6574 686f  ecompress` metho
-000058f0: 642e 0a0a 2020 2020 2020 2020 4166 7465  d...        Afte
-00005900: 7220 6465 636f 6d70 7265 7373 696e 6720  r decompressing 
-00005910: 6120 6672 616d 652c 2069 7420 646f 6573  a frame, it does
-00005920: 6e27 7420 7374 6f70 206c 696b 6520 3a70  n't stop like :p
-00005930: 793a 6d65 7468 3a60 5a73 7464 4465 636f  y:meth:`ZstdDeco
-00005940: 6d70 7265 7373 6f72 2e64 6563 6f6d 7072  mpressor.decompr
-00005950: 6573 7360 2e0a 0a20 2020 202e 2e20 7079  ess`...    .. py
-00005960: 3a61 7474 7269 6275 7465 3a3a 206e 6565  :attribute:: nee
-00005970: 6473 5f69 6e70 7574 0a0a 2020 2020 2020  ds_input..      
-00005980: 2020 4974 2773 2074 6865 2073 616d 6520    It's the same 
-00005990: 6173 203a 7079 3a61 7474 723a 605a 7374  as :py:attr:`Zst
-000059a0: 6444 6563 6f6d 7072 6573 736f 722e 6e65  dDecompressor.ne
-000059b0: 6564 735f 696e 7075 7460 2e0a 0a20 2020  eds_input`...   
-000059c0: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
-000059d0: 3a3a 2061 745f 6672 616d 655f 6564 6765  :: at_frame_edge
-000059e0: 0a0a 2020 2020 2020 2020 6060 5472 7565  ..        ``True
-000059f0: 6060 2077 6865 6e20 626f 7468 2074 6865  `` when both the
-00005a00: 2069 6e70 7574 2061 6e64 206f 7574 7075   input and outpu
-00005a10: 7420 7374 7265 616d 7320 6172 6520 6174  t streams are at
-00005a20: 2061 203a 7265 663a 6066 7261 6d65 3c66   a :ref:`frame<f
-00005a30: 7261 6d65 5f62 6c6f 636b 3e60 2065 6467  rame_block>` edg
-00005a40: 652c 206f 7220 7468 6520 6465 636f 6d70  e, or the decomp
-00005a50: 7265 7373 6f72 206a 7573 7420 6265 2069  ressor just be i
-00005a60: 6e69 7469 616c 697a 6564 2e0a 0a20 2020  nitialized...   
-00005a70: 2020 2020 2054 6869 7320 666c 6167 2063       This flag c
-00005a80: 6f75 6c64 2062 6520 7573 6564 2074 6f20  ould be used to 
-00005a90: 6368 6563 6b20 6461 7461 2069 6e74 6567  check data integ
-00005aa0: 7269 7479 2069 6e20 736f 6d65 2063 6173  rity in some cas
-00005ab0: 6573 2e0a 0a20 2020 202e 2e20 736f 7572  es...    .. sour
-00005ac0: 6365 636f 6465 3a3a 2070 7974 686f 6e0a  cecode:: python.
-00005ad0: 0a20 2020 2020 2020 2023 202d 2d2d 2073  .        # --- s
-00005ae0: 7472 6561 6d69 6e67 2064 6563 6f6d 7072  treaming decompr
-00005af0: 6573 7369 6f6e 2c20 756e 6c69 6d69 7465  ession, unlimite
-00005b00: 6420 6f75 7470 7574 202d 2d2d 0a20 2020  d output ---.   
-00005b10: 2020 2020 2064 3120 3d20 456e 646c 6573       d1 = Endles
-00005b20: 735a 7374 6444 6563 6f6d 7072 6573 736f  sZstdDecompresso
-00005b30: 7228 290a 0a20 2020 2020 2020 2064 6563  r()..        dec
-00005b40: 6f6d 7072 6573 7365 645f 6461 7431 203d  ompressed_dat1 =
-00005b50: 2064 312e 6465 636f 6d70 7265 7373 2864   d1.decompress(d
-00005b60: 6174 3129 0a20 2020 2020 2020 2064 6563  at1).        dec
-00005b70: 6f6d 7072 6573 7365 645f 6461 7432 203d  ompressed_dat2 =
-00005b80: 2064 312e 6465 636f 6d70 7265 7373 2864   d1.decompress(d
-00005b90: 6174 3229 0a20 2020 2020 2020 2064 6563  at2).        dec
-00005ba0: 6f6d 7072 6573 7365 645f 6461 7433 203d  ompressed_dat3 =
-00005bb0: 2064 312e 6465 636f 6d70 7265 7373 2864   d1.decompress(d
-00005bc0: 6174 3329 0a0a 2020 2020 2020 2020 6173  at3)..        as
-00005bd0: 7365 7274 2064 312e 6174 5f66 7261 6d65  sert d1.at_frame
-00005be0: 5f65 6467 652c 2027 6461 7461 2065 6e64  _edge, 'data end
-00005bf0: 7320 696e 2061 6e20 696e 636f 6d70 6c65  s in an incomple
-00005c00: 7465 2066 7261 6d65 2e27 0a0a 2020 2020  te frame.'..    
-00005c10: 2020 2020 2320 2d2d 2d20 7374 7265 616d      # --- stream
-00005c20: 696e 6720 6465 636f 6d70 7265 7373 696f  ing decompressio
-00005c30: 6e2c 206c 696d 6974 6564 206f 7574 7075  n, limited outpu
-00005c40: 7420 2d2d 2d0a 2020 2020 2020 2020 6432  t ---.        d2
-00005c50: 203d 2045 6e64 6c65 7373 5a73 7464 4465   = EndlessZstdDe
-00005c60: 636f 6d70 7265 7373 6f72 2829 0a0a 2020  compressor()..  
-00005c70: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-00005c80: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00005c90: 2064 322e 6e65 6564 735f 696e 7075 743a   d2.needs_input:
-00005ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005cb0: 2064 6174 203d 2072 6561 645f 696e 7075   dat = read_inpu
-00005cc0: 7428 322a 3130 3234 2a31 3032 3429 2023  t(2*1024*1024) #
-00005cd0: 2072 6561 6420 3220 4d69 4220 696e 7075   read 2 MiB inpu
-00005ce0: 7420 6461 7461 0a20 2020 2020 2020 2020  t data.         
-00005cf0: 2020 2020 2020 2069 6620 6e6f 7420 6461         if not da
-00005d00: 743a 2023 2069 6e70 7574 2073 7472 6561  t: # input strea
-00005d10: 6d20 656e 6473 0a20 2020 2020 2020 2020  m ends.         
-00005d20: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00005d30: 7420 6432 2e61 745f 6672 616d 655f 6564  t d2.at_frame_ed
-00005d40: 6765 3a0a 2020 2020 2020 2020 2020 2020  ge:.            
-00005d50: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00005d60: 6520 4578 6365 7074 696f 6e28 2764 6174  e Exception('dat
-00005d70: 6120 656e 6473 2069 6e20 616e 2069 6e63  a ends in an inc
-00005d80: 6f6d 706c 6574 6520 6672 616d 652e 2729  omplete frame.')
-00005d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005da0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-00005db0: 2020 2020 2020 2065 6c73 653a 2023 206d         else: # m
-00005dc0: 6179 6265 2074 6865 7265 2069 7320 756e  aybe there is un
-00005dd0: 636f 6e73 756d 6564 2069 6e70 7574 2064  consumed input d
-00005de0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-00005df0: 2020 2020 6461 7420 3d20 6227 270a 0a20      dat = b''.. 
-00005e00: 2020 2020 2020 2020 2020 2063 6875 6e6b             chunk
-00005e10: 203d 2064 322e 6465 636f 6d70 7265 7373   = d2.decompress
-00005e20: 2864 6174 2c20 3130 2a31 3032 342a 3130  (dat, 10*1024*10
-00005e30: 3234 2920 2320 6c69 6d69 7420 6f75 7470  24) # limit outp
-00005e40: 7574 2062 7566 6665 7220 746f 2031 3020  ut buffer to 10 
-00005e50: 4d69 420a 2020 2020 2020 2020 2020 2020  MiB.            
-00005e60: 7772 6974 655f 6f75 7470 7574 2863 6875  write_output(chu
-00005e70: 6e6b 290a 0a20 2020 202e 2e20 6869 6e74  nk)..    .. hint
-00005e80: 3a3a 2057 6879 203a 7079 3a63 6c61 7373  :: Why :py:class
-00005e90: 3a60 456e 646c 6573 735a 7374 6444 6563  :`EndlessZstdDec
-00005ea0: 6f6d 7072 6573 736f 7260 2064 6f65 736e  ompressor` doesn
-00005eb0: 2774 2073 746f 7020 6174 2066 7261 6d65  't stop at frame
-00005ec0: 2065 6467 6573 3f0a 0a20 2020 2020 2020   edges?..       
-00005ed0: 2049 6620 736f 2c20 756e 7573 6564 2069   If so, unused i
-00005ee0: 6e70 7574 2064 6174 6120 6166 7465 7220  nput data after 
-00005ef0: 616e 2065 6467 6520 7769 6c6c 2062 6520  an edge will be 
-00005f00: 636f 7069 6564 2074 6f20 616e 2069 6e74  copied to an int
-00005f10: 6572 6e61 6c20 6275 6666 6572 2c20 7468  ernal buffer, th
-00005f20: 6973 206d 6179 2062 6520 6120 7065 7266  is may be a perf
-00005f30: 6f72 6d61 6e63 6520 6f76 6572 6865 6164  ormance overhead
-00005f40: 2e0a 0a20 2020 2020 2020 2049 6620 7761  ...        If wa
-00005f50: 6e74 2074 6f20 7374 6f70 2061 7420 6672  nt to stop at fr
-00005f60: 616d 6520 6564 6765 732c 2077 7269 7465  ame edges, write
-00005f70: 2061 2077 7261 7070 6572 2075 7369 6e67   a wrapper using
-00005f80: 203a 7079 3a63 6c61 7373 3a60 5a73 7464   :py:class:`Zstd
-00005f90: 4465 636f 6d70 7265 7373 6f72 6020 636c  Decompressor` cl
-00005fa0: 6173 732e 2041 6e64 2064 6f6e 2774 2066  ass. And don't f
-00005fb0: 6565 6420 746f 6f20 6d75 6368 2064 6174  eed too much dat
-00005fc0: 6120 6576 6572 7920 7469 6d65 2c20 7468  a every time, th
-00005fd0: 6520 6f76 6572 6865 6164 206f 6620 636f  e overhead of co
-00005fe0: 7079 696e 6720 756e 7573 6564 2069 6e70  pying unused inp
-00005ff0: 7574 2064 6174 6120 746f 203a 7079 3a61  ut data to :py:a
-00006000: 7474 723a 605a 7374 6444 6563 6f6d 7072  ttr:`ZstdDecompr
-00006010: 6573 736f 722e 756e 7573 6564 5f64 6174  essor.unused_dat
-00006020: 6160 2061 7474 7269 6275 7465 2073 7469  a` attribute sti
-00006030: 6c6c 2065 7869 7374 732e 0a0a 0a2e 2e20  ll exists...... 
-00006040: 5f7a 7374 645f 6469 6374 3a0a 0a44 6963  _zstd_dict:..Dic
-00006050: 7469 6f6e 6172 790a 2d2d 2d2d 2d2d 2d2d  tionary.--------
-00006060: 2d2d 0a0a 2020 2020 5468 6973 2073 6563  --..    This sec
-00006070: 7469 6f6e 2063 6f6e 7461 696e 733a 0a0a  tion contains:..
-00006080: 2020 2020 2020 2020 2a20 636c 6173 7320          * class 
-00006090: 3a70 793a 636c 6173 733a 605a 7374 6444  :py:class:`ZstdD
-000060a0: 6963 7460 0a20 2020 2020 2020 202a 2066  ict`.        * f
-000060b0: 756e 6374 696f 6e20 3a70 793a 6675 6e63  unction :py:func
-000060c0: 3a60 7472 6169 6e5f 6469 6374 600a 2020  :`train_dict`.  
-000060d0: 2020 2020 2020 2a20 6675 6e63 7469 6f6e        * function
-000060e0: 203a 7079 3a66 756e 633a 6066 696e 616c   :py:func:`final
-000060f0: 697a 655f 6469 6374 600a 0a2e 2e20 6e6f  ize_dict`.... no
-00006100: 7465 3a3a 0a20 2020 2049 6620 7573 6520  te::.    If use 
-00006110: 7072 652d 7472 6169 6e65 6420 7a73 7464  pre-trained zstd
-00006120: 2064 6963 7469 6f6e 6172 792c 2074 6865   dictionary, the
-00006130: 2063 6f6d 7072 6573 7369 6f6e 2072 6174   compression rat
-00006140: 696f 2061 6368 6965 7661 626c 6520 6f6e  io achievable on
-00006150: 2073 6d61 6c6c 2064 6174 6120 2861 2066   small data (a f
-00006160: 6577 204b 6942 2920 696d 7072 6f76 6573  ew KiB) improves
-00006170: 2064 7261 6d61 7469 6361 6c6c 792e 0a0a   dramatically...
-00006180: 2020 2020 2a2a 4174 7465 6e74 696f 6e2a      **Attention*
-00006190: 2a0a 0a20 2020 2020 2020 2023 2e20 4966  *..        #. If
-000061a0: 2079 6f75 206c 6f73 6520 6120 7a73 7464   you lose a zstd
-000061b0: 2064 6963 7469 6f6e 6172 792c 2074 6865   dictionary, the
-000061c0: 6e20 6361 6e27 7420 6465 636f 6d70 7265  n can't decompre
-000061d0: 7373 2074 6865 2063 6f72 7265 7370 6f6e  ss the correspon
-000061e0: 6469 6e67 2064 6174 612e 0a20 2020 2020  ding data..     
-000061f0: 2020 2023 2e20 5a73 7464 2064 6963 7469     #. Zstd dicti
-00006200: 6f6e 6172 7920 6861 7320 6e65 676c 6967  onary has neglig
-00006210: 6962 6c65 2065 6666 6563 7420 6f6e 206c  ible effect on l
-00006220: 6172 6765 2064 6174 6120 286d 756c 7469  arge data (multi
-00006230: 2d4d 6942 2920 636f 6d70 7265 7373 696f  -MiB) compressio
-00006240: 6e2e 0a20 2020 2020 2020 2023 2e20 5468  n..        #. Th
-00006250: 6572 6520 6973 2061 2070 6f73 7369 6269  ere is a possibi
-00006260: 6c69 7479 2074 6861 7420 7468 6520 6469  lity that the di
-00006270: 6374 696f 6e61 7279 2063 6f6e 7465 6e74  ctionary content
-00006280: 2063 6f75 6c64 2062 6520 6d61 6c69 6369   could be malici
-00006290: 6f75 736c 7920 7461 6d70 6572 6564 2062  ously tampered b
-000062a0: 7920 6120 7468 6972 6420 7061 7274 792e  y a third party.
-000062b0: 0a0a 2020 2020 2a2a 4261 636b 6772 6f75  ..    **Backgrou
-000062c0: 6e64 2a2a 0a0a 2020 2020 5468 6520 736d  nd**..    The sm
-000062d0: 616c 6c65 7220 7468 6520 616d 6f75 6e74  aller the amount
-000062e0: 206f 6620 6461 7461 2074 6f20 636f 6d70   of data to comp
-000062f0: 7265 7373 2c20 7468 6520 6d6f 7265 2064  ress, the more d
-00006300: 6966 6669 6375 6c74 2069 7420 6973 2074  ifficult it is t
-00006310: 6f20 636f 6d70 7265 7373 2e20 5468 6973  o compress. This
-00006320: 2070 726f 626c 656d 2069 7320 636f 6d6d   problem is comm
-00006330: 6f6e 2074 6f20 616c 6c20 636f 6d70 7265  on to all compre
-00006340: 7373 696f 6e20 616c 676f 7269 7468 6d73  ssion algorithms
-00006350: 2c20 616e 6420 7265 6173 6f6e 2069 732c  , and reason is,
-00006360: 2063 6f6d 7072 6573 7369 6f6e 2061 6c67   compression alg
-00006370: 6f72 6974 686d 7320 6c65 6172 6e20 6672  orithms learn fr
-00006380: 6f6d 2070 6173 7420 6461 7461 2068 6f77  om past data how
-00006390: 2074 6f20 636f 6d70 7265 7373 2066 7574   to compress fut
-000063a0: 7572 6520 6461 7461 2e20 4275 7420 6174  ure data. But at
-000063b0: 2074 6865 2062 6567 696e 6e69 6e67 206f   the beginning o
-000063c0: 6620 6120 6e65 7720 6461 7461 2073 6574  f a new data set
-000063d0: 2c20 7468 6572 6520 6973 206e 6f20 2270  , there is no "p
-000063e0: 6173 7422 2074 6f20 6275 696c 6420 7570  ast" to build up
-000063f0: 6f6e 2e0a 0a20 2020 205a 7374 6420 7472  on...    Zstd tr
-00006400: 6169 6e69 6e67 206d 6f64 6520 6361 6e20  aining mode can 
-00006410: 6265 2075 7365 6420 746f 2074 756e 6520  be used to tune 
-00006420: 7468 6520 616c 676f 7269 7468 6d20 666f  the algorithm fo
-00006430: 7220 6120 7365 6c65 6374 6564 2074 7970  r a selected typ
-00006440: 6520 6f66 2064 6174 612e 2054 7261 696e  e of data. Train
-00006450: 696e 6720 6973 2061 6368 6965 7665 6420  ing is achieved 
-00006460: 6279 2070 726f 7669 6469 6e67 2069 7420  by providing it 
-00006470: 7769 7468 2061 2066 6577 2073 616d 706c  with a few sampl
-00006480: 6573 2028 6f6e 6520 6669 6c65 2070 6572  es (one file per
-00006490: 2073 616d 706c 6529 2e20 5468 6520 7265   sample). The re
-000064a0: 7375 6c74 206f 6620 7468 6973 2074 7261  sult of this tra
-000064b0: 696e 696e 6720 6973 2073 746f 7265 6420  ining is stored 
-000064c0: 696e 2061 2066 696c 6520 6361 6c6c 6564  in a file called
-000064d0: 2022 6469 6374 696f 6e61 7279 222c 2077   "dictionary", w
-000064e0: 6869 6368 206d 7573 7420 6265 206c 6f61  hich must be loa
-000064f0: 6465 6420 6265 666f 7265 2063 6f6d 7072  ded before compr
-00006500: 6573 7369 6f6e 2061 6e64 2064 6563 6f6d  ession and decom
-00006510: 7072 6573 7369 6f6e 2e0a 0a20 2020 2053  pression...    S
-00006520: 6565 2074 6865 2046 4151 2069 6e20 6074  ee the FAQ in `t
-00006530: 6869 7320 6669 6c65 203c 6874 7470 733a  his file <https:
-00006540: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6163  //github.com/fac
-00006550: 6562 6f6f 6b2f 7a73 7464 2f62 6c6f 622f  ebook/zstd/blob/
-00006560: 6465 762f 6c69 622f 7a64 6963 742e 683e  dev/lib/zdict.h>
-00006570: 605f 2066 6f72 2064 6574 6169 6c73 2e0a  `_ for details..
-00006580: 0a20 2020 202a 2a41 6476 616e 6365 6420  .    **Advanced 
-00006590: 6469 6374 696f 6e61 7279 2074 7261 696e  dictionary train
-000065a0: 696e 672a 2a0a 0a20 2020 2050 797a 7374  ing**..    Pyzst
-000065b0: 6420 6d6f 6475 6c65 206f 6e6c 7920 7573  d module only us
-000065c0: 6573 207a 7374 6420 6c69 6272 6172 7927  es zstd library'
-000065d0: 7320 7374 6162 6c65 2041 5049 2e20 5468  s stable API. Th
-000065e0: 6520 7374 6162 6c65 2041 5049 206f 6e6c  e stable API onl
-000065f0: 7920 6578 706f 7365 7320 7477 6f20 6469  y exposes two di
-00006600: 6374 696f 6e61 7279 2074 7261 696e 696e  ctionary trainin
-00006610: 6720 6675 6e63 7469 6f6e 7320 7468 6174  g functions that
-00006620: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
-00006630: 6f20 3a70 793a 6675 6e63 3a60 7472 6169  o :py:func:`trai
-00006640: 6e5f 6469 6374 6020 616e 6420 3a70 793a  n_dict` and :py:
-00006650: 6675 6e63 3a60 6669 6e61 6c69 7a65 5f64  func:`finalize_d
-00006660: 6963 7460 2e0a 0a20 2020 2049 6620 7761  ict`...    If wa
-00006670: 6e74 2074 6f20 6164 6a75 7374 2061 6476  nt to adjust adv
-00006680: 616e 6365 6420 7472 6169 6e69 6e67 2070  anced training p
-00006690: 6172 616d 6574 6572 732c 2079 6f75 206d  arameters, you m
-000066a0: 6179 2075 7365 207a 7374 6427 7320 434c  ay use zstd's CL
-000066b0: 4920 7072 6f67 7261 6d20 286e 6f74 2070  I program (not p
-000066c0: 797a 7374 6420 6d6f 6475 6c65 2773 2043  yzstd module's C
-000066d0: 4c49 292c 2069 7420 6861 7320 656e 7472  LI), it has entr
-000066e0: 6965 7320 746f 207a 7374 6420 6c69 6272  ies to zstd libr
-000066f0: 6172 7927 7320 6578 7065 7269 6d65 6e74  ary's experiment
-00006700: 616c 2041 5049 2e0a 0a2e 2e20 7079 3a63  al API..... py:c
-00006710: 6c61 7373 3a3a 205a 7374 6444 6963 740a  lass:: ZstdDict.
-00006720: 0a20 2020 2052 6570 7265 7365 6e74 7320  .    Represents 
-00006730: 6120 7a73 7464 2064 6963 7469 6f6e 6172  a zstd dictionar
-00006740: 792c 2063 616e 2062 6520 7573 6564 2066  y, can be used f
-00006750: 6f72 2063 6f6d 7072 6573 7369 6f6e 2f64  or compression/d
-00006760: 6563 6f6d 7072 6573 7369 6f6e 2e0a 0a20  ecompression... 
-00006770: 2020 2049 7420 6861 7320 616e 2069 6e74     It has an int
-00006780: 6572 6e61 6c20 6361 6368 6520 666f 7220  ernal cache for 
-00006790: 636f 7374 6c79 2064 6967 6573 7469 6e67  costly digesting
-000067a0: 2c20 736f 2069 7427 7320 7265 636f 6d6d  , so it's recomm
-000067b0: 656e 6465 6420 746f 2072 6575 7365 2060  ended to reuse `
-000067c0: 605a 7374 6444 6963 7460 6020 6f62 6a65  `ZstdDict`` obje
-000067d0: 6374 2066 6f72 2074 6865 2073 616d 6520  ct for the same 
-000067e0: 6469 6374 696f 6e61 7279 2e0a 0a20 2020  dictionary...   
-000067f0: 2049 7427 7320 7468 7265 6164 2d73 6166   It's thread-saf
-00006800: 652c 2061 6e64 2063 616e 2062 6520 7368  e, and can be sh
-00006810: 6172 6564 2062 7920 6d75 6c74 6970 6c65  ared by multiple
-00006820: 203a 7079 3a63 6c61 7373 3a60 5a73 7464   :py:class:`Zstd
-00006830: 436f 6d70 7265 7373 6f72 6020 2f20 3a70  Compressor` / :p
-00006840: 793a 636c 6173 733a 605a 7374 6444 6563  y:class:`ZstdDec
-00006850: 6f6d 7072 6573 736f 7260 206f 626a 6563  ompressor` objec
-00006860: 7473 2e0a 0a20 2020 202e 2e20 7079 3a6d  ts...    .. py:m
-00006870: 6574 686f 643a 3a20 5f5f 696e 6974 5f5f  ethod:: __init__
-00006880: 2873 656c 662c 2064 6963 745f 636f 6e74  (self, dict_cont
-00006890: 656e 742c 2069 735f 7261 773d 4661 6c73  ent, is_raw=Fals
-000068a0: 6529 0a0a 2020 2020 2020 2020 496e 6974  e)..        Init
-000068b0: 6961 6c69 7a65 2061 205a 7374 6444 6963  ialize a ZstdDic
-000068c0: 7420 6f62 6a65 6374 2e0a 0a20 2020 2020  t object...     
-000068d0: 2020 203a 7061 7261 6d20 6469 6374 5f63     :param dict_c
-000068e0: 6f6e 7465 6e74 3a20 4469 6374 696f 6e61  ontent: Dictiona
-000068f0: 7279 2773 2063 6f6e 7465 6e74 2e0a 2020  ry's content..  
-00006900: 2020 2020 2020 3a74 7970 6520 6469 6374        :type dict
-00006910: 5f63 6f6e 7465 6e74 3a20 6279 7465 732d  _content: bytes-
-00006920: 6c69 6b65 206f 626a 6563 740a 2020 2020  like object.    
-00006930: 2020 2020 3a70 6172 616d 2069 735f 7261      :param is_ra
-00006940: 773a 2054 6869 7320 7061 7261 6d65 7465  w: This paramete
-00006950: 7220 6973 2066 6f72 2061 6476 616e 6365  r is for advance
-00006960: 6420 7573 6572 2e20 6060 5472 7565 6060  d user. ``True``
-00006970: 206d 6561 6e73 202a 6469 6374 5f63 6f6e   means *dict_con
-00006980: 7465 6e74 2a20 6172 6775 6d65 6e74 2069  tent* argument i
-00006990: 7320 6120 2272 6177 2063 6f6e 7465 6e74  s a "raw content
-000069a0: 2220 6469 6374 696f 6e61 7279 2c20 6672  " dictionary, fr
-000069b0: 6565 206f 6620 616e 7920 666f 726d 6174  ee of any format
-000069c0: 2072 6573 7472 6963 7469 6f6e 2e20 6060   restriction. ``
-000069d0: 4661 6c73 6560 6020 6d65 616e 7320 2a64  False`` means *d
-000069e0: 6963 745f 636f 6e74 656e 742a 2061 7267  ict_content* arg
-000069f0: 756d 656e 7420 6973 2061 6e20 6f72 6469  ument is an ordi
-00006a00: 6e61 7279 207a 7374 6420 6469 6374 696f  nary zstd dictio
-00006a10: 6e61 7279 2c20 7761 7320 6372 6561 7465  nary, was create
-00006a20: 6420 6279 207a 7374 6420 6675 6e63 7469  d by zstd functi
-00006a30: 6f6e 732c 2066 6f6c 6c6f 7720 6120 7370  ons, follow a sp
-00006a40: 6563 6966 6965 6420 666f 726d 6174 2e0a  ecified format..
-00006a50: 2020 2020 2020 2020 3a74 7970 6520 6973          :type is
-00006a60: 5f72 6177 3a20 626f 6f6c 0a0a 2020 2020  _raw: bool..    
-00006a70: 2e2e 2070 793a 6174 7472 6962 7574 653a  .. py:attribute:
-00006a80: 3a20 6469 6374 5f63 6f6e 7465 6e74 0a0a  : dict_content..
-00006a90: 2020 2020 2020 2020 5468 6520 636f 6e74          The cont
-00006aa0: 656e 7420 6f66 207a 7374 6420 6469 6374  ent of zstd dict
-00006ab0: 696f 6e61 7279 2c20 6120 6060 6279 7465  ionary, a ``byte
-00006ac0: 7360 6020 6f62 6a65 6374 2e20 4974 2773  s`` object. It's
-00006ad0: 2074 6865 2073 616d 6520 6173 202a 6469   the same as *di
-00006ae0: 6374 5f63 6f6e 7465 6e74 2a20 6172 6775  ct_content* argu
-00006af0: 6d65 6e74 2069 6e20 3a70 793a 6d65 7468  ment in :py:meth
-00006b00: 3a60 7e5a 7374 6444 6963 742e 5f5f 696e  :`~ZstdDict.__in
-00006b10: 6974 5f5f 6020 6d65 7468 6f64 2e20 4974  it__` method. It
-00006b20: 2063 616e 2062 6520 7573 6564 2077 6974   can be used wit
-00006b30: 6820 6f74 6865 7220 7072 6f67 7261 6d73  h other programs
-00006b40: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
-00006b50: 7269 6275 7465 3a3a 2064 6963 745f 6964  ribute:: dict_id
-00006b60: 0a0a 2020 2020 2020 2020 4944 206f 6620  ..        ID of 
-00006b70: 7a73 7464 2064 6963 7469 6f6e 6172 792c  zstd dictionary,
-00006b80: 2061 2033 322d 6269 7420 756e 7369 676e   a 32-bit unsign
-00006b90: 6564 2069 6e74 6567 6572 2076 616c 7565  ed integer value
-00006ba0: 2e20 5365 6520 3a72 6566 3a60 7468 6973  . See :ref:`this
-00006bb0: 206e 6f74 653c 6469 6374 5f69 643e 6020   note<dict_id>` 
-00006bc0: 666f 7220 6465 7461 696c 732e 0a0a 2020  for details...  
-00006bd0: 2020 2020 2020 4e6f 6e2d 7a65 726f 206d        Non-zero m
-00006be0: 6561 6e73 206f 7264 696e 6172 7920 6469  eans ordinary di
-00006bf0: 6374 696f 6e61 7279 2c20 7761 7320 6372  ctionary, was cr
-00006c00: 6561 7465 6420 6279 207a 7374 6420 6675  eated by zstd fu
-00006c10: 6e63 7469 6f6e 732c 2066 6f6c 6c6f 7720  nctions, follow 
-00006c20: 6120 7370 6563 6966 6965 6420 666f 726d  a specified form
-00006c30: 6174 2e0a 0a20 2020 2020 2020 2060 6030  at...        ``0
-00006c40: 6060 206d 6561 6e73 2061 2022 7261 7720  `` means a "raw 
-00006c50: 636f 6e74 656e 7422 2064 6963 7469 6f6e  content" diction
-00006c60: 6172 792c 2066 7265 6520 6f66 2061 6e79  ary, free of any
-00006c70: 2066 6f72 6d61 7420 7265 7374 7269 6374   format restrict
-00006c80: 696f 6e2c 2075 7365 6420 666f 7220 6164  ion, used for ad
-00006c90: 7661 6e63 6564 2075 7365 722e 2028 4e6f  vanced user. (No
-00006ca0: 7465 2074 6861 7420 7468 6520 6d65 616e  te that the mean
-00006cb0: 696e 6720 6f66 2060 6030 6060 2069 7320  ing of ``0`` is 
-00006cc0: 6469 6666 6572 656e 7420 6672 6f6d 2060  different from `
-00006cd0: 6064 6963 7469 6f6e 6172 795f 6964 6060  `dictionary_id``
-00006ce0: 2069 6e20 3a70 793a 6675 6e63 3a60 6765   in :py:func:`ge
-00006cf0: 745f 6672 616d 655f 696e 666f 6020 6675  t_frame_info` fu
-00006d00: 6e63 7469 6f6e 2e29 0a0a 2020 2020 2e2e  nction.)..    ..
-00006d10: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
-00006d20: 7468 6f6e 0a0a 2020 2020 2020 2020 2320  thon..        # 
-00006d30: 6c6f 6164 2061 207a 7374 6420 6469 6374  load a zstd dict
-00006d40: 696f 6e61 7279 2066 726f 6d20 6669 6c65  ionary from file
-00006d50: 0a20 2020 2020 2020 2077 6974 6820 696f  .        with io
-00006d60: 2e6f 7065 6e28 6469 6374 5f70 6174 682c  .open(dict_path,
-00006d70: 2027 7262 2729 2061 7320 663a 0a20 2020   'rb') as f:.   
-00006d80: 2020 2020 2020 2020 2066 696c 655f 636f           file_co
-00006d90: 6e74 656e 7420 3d20 662e 7265 6164 2829  ntent = f.read()
-00006da0: 0a20 2020 2020 2020 207a 6420 3d20 5a73  .        zd = Zs
-00006db0: 7464 4469 6374 2866 696c 655f 636f 6e74  tdDict(file_cont
-00006dc0: 656e 7429 0a0a 2020 2020 2020 2020 2320  ent)..        # 
-00006dd0: 7573 6520 7468 6520 6469 6374 696f 6e61  use the dictiona
-00006de0: 7279 2074 6f20 636f 6d70 7265 7373 0a20  ry to compress. 
-00006df0: 2020 2020 2020 2063 6f6d 7072 6573 7365         compresse
-00006e00: 645f 6461 7420 3d20 636f 6d70 7265 7373  d_dat = compress
-00006e10: 2872 6177 5f64 6174 2c20 7a73 7464 5f64  (raw_dat, zstd_d
-00006e20: 6963 743d 7a64 290a 0a0a 2e2e 2070 793a  ict=zd)..... py:
-00006e30: 6675 6e63 7469 6f6e 3a3a 2074 7261 696e  function:: train
-00006e40: 5f64 6963 7428 7361 6d70 6c65 732c 2064  _dict(samples, d
-00006e50: 6963 745f 7369 7a65 290a 0a20 2020 2054  ict_size)..    T
-00006e60: 7261 696e 2061 207a 7374 6420 6469 6374  rain a zstd dict
-00006e70: 696f 6e61 7279 2e0a 0a20 2020 2053 6565  ionary...    See
-00006e80: 2074 6865 2046 4151 2069 6e20 6074 6869   the FAQ in `thi
-00006e90: 7320 6669 6c65 203c 6874 7470 733a 2f2f  s file <https://
-00006ea0: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
-00006eb0: 6f6f 6b2f 7a73 7464 2f62 6c6f 622f 7265  ook/zstd/blob/re
-00006ec0: 6c65 6173 652f 6c69 622f 7a64 6963 742e  lease/lib/zdict.
-00006ed0: 683e 605f 2066 6f72 2064 6574 6169 6c73  h>`_ for details
-00006ee0: 2e0a 0a20 2020 203a 7061 7261 6d20 7361  ...    :param sa
-00006ef0: 6d70 6c65 733a 2041 6e20 6974 6572 6162  mples: An iterab
-00006f00: 6c65 206f 6620 7361 6d70 6c65 732c 2061  le of samples, a
-00006f10: 2073 616d 706c 6520 6973 2061 2062 7974   sample is a byt
-00006f20: 6573 2d6c 696b 6520 6f62 6a65 6374 2072  es-like object r
-00006f30: 6570 7265 7365 6e74 7320 6120 6669 6c65  epresents a file
-00006f40: 2e0a 2020 2020 3a74 7970 6520 7361 6d70  ..    :type samp
-00006f50: 6c65 733a 2069 7465 7261 626c 650a 2020  les: iterable.  
-00006f60: 2020 3a70 6172 616d 2069 6e74 2064 6963    :param int dic
-00006f70: 745f 7369 7a65 3a20 5265 7475 726e 6564  t_size: Returned
-00006f80: 207a 7374 6420 6469 6374 696f 6e61 7279   zstd dictionary
-00006f90: 2773 202a 2a6d 6178 696d 756d 2a2a 2073  's **maximum** s
-00006fa0: 697a 652c 2069 6e20 6279 7465 732e 0a20  ize, in bytes.. 
-00006fb0: 2020 203a 7265 7475 726e 3a20 5472 6169     :return: Trai
-00006fc0: 6e65 6420 7a73 7464 2064 6963 7469 6f6e  ned zstd diction
-00006fd0: 6172 792e 2049 6620 7761 6e74 2074 6f20  ary. If want to 
-00006fe0: 7361 7665 2074 6865 2064 6963 7469 6f6e  save the diction
-00006ff0: 6172 7920 746f 2061 2066 696c 652c 2073  ary to a file, s
-00007000: 6176 6520 7468 6520 3a70 793a 6174 7472  ave the :py:attr
-00007010: 3a60 5a73 7464 4469 6374 2e64 6963 745f  :`ZstdDict.dict_
-00007020: 636f 6e74 656e 7460 2061 7474 7269 6275  content` attribu
-00007030: 7465 2e0a 2020 2020 3a72 7479 7065 3a20  te..    :rtype: 
-00007040: 5a73 7464 4469 6374 0a0a 2020 2020 2e2e  ZstdDict..    ..
-00007050: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
-00007060: 7468 6f6e 0a0a 2020 2020 2020 2020 6465  thon..        de
-00007070: 6620 7361 6d70 6c65 7328 293a 0a20 2020  f samples():.   
-00007080: 2020 2020 2020 2020 2072 6f6f 7464 6972           rootdir
-00007090: 203d 2072 2245 3a5c 6461 7461 220a 0a20   = r"E:\data".. 
-000070a0: 2020 2020 2020 2020 2020 2023 204e 6f74             # Not
-000070b0: 6520 7468 6174 2074 6865 206f 7264 6572  e that the order
-000070c0: 206f 6620 7468 6520 6669 6c65 7320 6d61   of the files ma
-000070d0: 7920 6265 2064 6966 6665 7265 6e74 2c0a  y be different,.
-000070e0: 2020 2020 2020 2020 2020 2020 2320 7468              # th
-000070f0: 6572 6566 6f72 6520 7468 6520 6765 6e65  erefore the gene
-00007100: 7261 7465 6420 6469 6374 696f 6e61 7279  rated dictionary
-00007110: 206d 6179 2062 6520 6469 6666 6572 656e   may be differen
-00007120: 742e 0a20 2020 2020 2020 2020 2020 2066  t..            f
-00007130: 6f72 2070 6172 656e 742c 2064 6972 6e61  or parent, dirna
-00007140: 6d65 732c 2066 696c 656e 616d 6573 2069  mes, filenames i
-00007150: 6e20 6f73 2e77 616c 6b28 726f 6f74 6469  n os.walk(rootdi
-00007160: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00007170: 2020 2020 666f 7220 6669 6c65 6e61 6d65      for filename
-00007180: 2069 6e20 6669 6c65 6e61 6d65 733a 0a20   in filenames:. 
-00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071a0: 2020 2070 6174 6820 3d20 6f73 2e70 6174     path = os.pat
-000071b0: 682e 6a6f 696e 2870 6172 656e 742c 2066  h.join(parent, f
-000071c0: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
-000071d0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-000071e0: 6820 696f 2e6f 7065 6e28 7061 7468 2c20  h io.open(path, 
-000071f0: 2772 6227 2920 6173 2066 3a0a 2020 2020  'rb') as f:.    
-00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007210: 2020 2020 6461 7420 3d20 662e 7265 6164      dat = f.read
-00007220: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00007230: 2020 2020 2020 2079 6965 6c64 2064 6174         yield dat
-00007240: 0a0a 2020 2020 2020 2020 6469 6320 3d20  ..        dic = 
-00007250: 7079 7a73 7464 2e74 7261 696e 5f64 6963  pyzstd.train_dic
-00007260: 7428 7361 6d70 6c65 7328 292c 2031 3030  t(samples(), 100
-00007270: 2a31 3032 3429 0a0a 2e2e 2070 793a 6675  *1024).... py:fu
-00007280: 6e63 7469 6f6e 3a3a 2066 696e 616c 697a  nction:: finaliz
-00007290: 655f 6469 6374 287a 7374 645f 6469 6374  e_dict(zstd_dict
-000072a0: 2c20 7361 6d70 6c65 732c 2064 6963 745f  , samples, dict_
-000072b0: 7369 7a65 2c20 6c65 7665 6c29 0a0a 2020  size, level)..  
-000072c0: 2020 4769 7665 6e20 6120 6375 7374 6f6d    Given a custom
-000072d0: 2063 6f6e 7465 6e74 2061 7320 6120 6261   content as a ba
-000072e0: 7369 7320 666f 7220 6469 6374 696f 6e61  sis for dictiona
-000072f0: 7279 2c20 616e 6420 6120 7365 7420 6f66  ry, and a set of
-00007300: 2073 616d 706c 6573 2c20 6669 6e61 6c69   samples, finali
-00007310: 7a65 2064 6963 7469 6f6e 6172 7920 6279  ze dictionary by
-00007320: 2061 6464 696e 6720 6865 6164 6572 7320   adding headers 
-00007330: 616e 6420 7374 6174 6973 7469 6373 2061  and statistics a
-00007340: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-00007350: 7a73 7464 2064 6963 7469 6f6e 6172 7920  zstd dictionary 
-00007360: 666f 726d 6174 2e0a 0a20 2020 2053 6565  format...    See
-00007370: 2074 6865 2046 4151 2069 6e20 6074 6869   the FAQ in `thi
-00007380: 7320 6669 6c65 203c 6874 7470 733a 2f2f  s file <https://
-00007390: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
-000073a0: 6f6f 6b2f 7a73 7464 2f62 6c6f 622f 7265  ook/zstd/blob/re
-000073b0: 6c65 6173 652f 6c69 622f 7a64 6963 742e  lease/lib/zdict.
-000073c0: 683e 605f 2066 6f72 2064 6574 6169 6c73  h>`_ for details
-000073d0: 2e0a 0a20 2020 203a 7061 7261 6d20 7a73  ...    :param zs
-000073e0: 7464 5f64 6963 743a 2041 2062 6173 6973  td_dict: A basis
-000073f0: 2064 6963 7469 6f6e 6172 792e 0a20 2020   dictionary..   
-00007400: 203a 7479 7065 207a 7374 645f 6469 6374   :type zstd_dict
-00007410: 3a20 5a73 7464 4469 6374 0a20 2020 203a  : ZstdDict.    :
-00007420: 7061 7261 6d20 7361 6d70 6c65 733a 2041  param samples: A
-00007430: 6e20 6974 6572 6162 6c65 206f 6620 7361  n iterable of sa
-00007440: 6d70 6c65 732c 2061 2073 616d 706c 6520  mples, a sample 
-00007450: 6973 2061 2062 7974 6573 2d6c 696b 6520  is a bytes-like 
-00007460: 6f62 6a65 6374 2072 6570 7265 7365 6e74  object represent
-00007470: 7320 6120 6669 6c65 2e0a 2020 2020 3a74  s a file..    :t
-00007480: 7970 6520 7361 6d70 6c65 733a 2069 7465  ype samples: ite
-00007490: 7261 626c 650a 2020 2020 3a70 6172 616d  rable.    :param
-000074a0: 2069 6e74 2064 6963 745f 7369 7a65 3a20   int dict_size: 
-000074b0: 5265 7475 726e 6564 207a 7374 6420 6469  Returned zstd di
-000074c0: 6374 696f 6e61 7279 2773 202a 2a6d 6178  ctionary's **max
-000074d0: 696d 756d 2a2a 2073 697a 652c 2069 6e20  imum** size, in 
-000074e0: 6279 7465 732e 0a20 2020 203a 7061 7261  bytes..    :para
-000074f0: 6d20 696e 7420 6c65 7665 6c3a 2054 6865  m int level: The
-00007500: 2063 6f6d 7072 6573 7369 6f6e 206c 6576   compression lev
-00007510: 656c 2065 7870 6563 7465 6420 746f 2075  el expected to u
-00007520: 7365 2069 6e20 7072 6f64 7563 7469 6f6e  se in production
-00007530: 2e20 5468 6520 7374 6174 6973 7469 6373  . The statistics
-00007540: 2066 6f72 2065 6163 6820 636f 6d70 7265   for each compre
-00007550: 7373 696f 6e20 6c65 7665 6c20 6469 6666  ssion level diff
-00007560: 6572 2c20 736f 2074 756e 696e 6720 7468  er, so tuning th
-00007570: 6520 6469 6374 696f 6e61 7279 2066 6f72  e dictionary for
-00007580: 2074 6865 2063 6f6d 7072 6573 7369 6f6e   the compression
-00007590: 206c 6576 656c 2063 616e 2068 656c 7020   level can help 
-000075a0: 7175 6974 6520 6120 6269 742e 0a20 2020  quite a bit..   
-000075b0: 203a 7265 7475 726e 3a20 4669 6e61 6c69   :return: Finali
-000075c0: 7a65 6420 7a73 7464 2064 6963 7469 6f6e  zed zstd diction
-000075d0: 6172 792e 2049 6620 7761 6e74 2074 6f20  ary. If want to 
-000075e0: 7361 7665 2074 6865 2064 6963 7469 6f6e  save the diction
-000075f0: 6172 7920 746f 2061 2066 696c 652c 2073  ary to a file, s
-00007600: 6176 6520 7468 6520 3a70 793a 6174 7472  ave the :py:attr
-00007610: 3a60 5a73 7464 4469 6374 2e64 6963 745f  :`ZstdDict.dict_
-00007620: 636f 6e74 656e 7460 2061 7474 7269 6275  content` attribu
-00007630: 7465 2e0a 2020 2020 3a72 7479 7065 3a20  te..    :rtype: 
-00007640: 5a73 7464 4469 6374 0a0a 0a4d 6f64 756c  ZstdDict...Modul
-00007650: 652d 6c65 7665 6c20 6675 6e63 7469 6f6e  e-level function
-00007660: 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s.--------------
-00007670: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020 5468  --------..    Th
-00007680: 6973 2073 6563 7469 6f6e 2063 6f6e 7461  is section conta
-00007690: 696e 733a 0a0a 2020 2020 2020 2020 2a20  ins:..        * 
-000076a0: 6675 6e63 7469 6f6e 203a 7079 3a66 756e  function :py:fun
-000076b0: 633a 6067 6574 5f66 7261 6d65 5f69 6e66  c:`get_frame_inf
-000076c0: 6f60 2c20 6765 7420 6672 616d 6520 696e  o`, get frame in
-000076d0: 666f 726d 6174 696f 6e20 6672 6f6d 2061  formation from a
-000076e0: 2066 7261 6d65 2068 6561 6465 722e 0a20   frame header.. 
-000076f0: 2020 2020 2020 202a 2066 756e 6374 696f         * functio
-00007700: 6e20 3a70 793a 6675 6e63 3a60 6765 745f  n :py:func:`get_
-00007710: 6672 616d 655f 7369 7a65 602c 2067 6574  frame_size`, get
-00007720: 2061 2066 7261 6d65 2773 2073 697a 652e   a frame's size.
-00007730: 0a0a 2e2e 2070 793a 6675 6e63 7469 6f6e  .... py:function
-00007740: 3a3a 2067 6574 5f66 7261 6d65 5f69 6e66  :: get_frame_inf
-00007750: 6f28 6672 616d 655f 6275 6666 6572 290a  o(frame_buffer).
-00007760: 0a20 2020 2047 6574 207a 7374 6420 6672  .    Get zstd fr
-00007770: 616d 6520 696e 666f 726d 6174 696f 6e20  ame information 
-00007780: 6672 6f6d 2061 2066 7261 6d65 2068 6561  from a frame hea
-00007790: 6465 722e 0a0a 2020 2020 5265 7475 726e  der...    Return
-000077a0: 2061 2032 2d69 7465 6d20 6e61 6d65 6474   a 2-item namedt
-000077b0: 7570 6c65 3a20 2864 6563 6f6d 7072 6573  uple: (decompres
-000077c0: 7365 645f 7369 7a65 2c20 6469 6374 696f  sed_size, dictio
-000077d0: 6e61 7279 5f69 6429 0a0a 2020 2020 4966  nary_id)..    If
-000077e0: 2060 6064 6563 6f6d 7072 6573 7365 645f   ``decompressed_
-000077f0: 7369 7a65 6060 2069 7320 6060 4e6f 6e65  size`` is ``None
-00007800: 6060 2c20 6465 636f 6d70 7265 7373 6564  ``, decompressed
-00007810: 2073 697a 6520 6973 2075 6e6b 6e6f 776e   size is unknown
-00007820: 2e0a 0a20 2020 2060 6064 6963 7469 6f6e  ...    ``diction
-00007830: 6172 795f 6964 6060 2069 7320 6120 3332  ary_id`` is a 32
-00007840: 2d62 6974 2075 6e73 6967 6e65 6420 696e  -bit unsigned in
-00007850: 7465 6765 7220 7661 6c75 652e 2060 6030  teger value. ``0
-00007860: 6060 206d 6561 6e73 2064 6963 7469 6f6e  `` means diction
-00007870: 6172 7920 4944 2077 6173 206e 6f74 2072  ary ID was not r
-00007880: 6563 6f72 6465 6420 696e 2066 7261 6d65  ecorded in frame
-00007890: 2068 6561 6465 722c 2074 6865 2066 7261   header, the fra
-000078a0: 6d65 206d 6179 206f 7220 6d61 7920 6e6f  me may or may no
-000078b0: 7420 6e65 6564 2061 2064 6963 7469 6f6e  t need a diction
-000078c0: 6172 7920 746f 2062 6520 6465 636f 6465  ary to be decode
-000078d0: 642c 2061 6e64 2074 6865 2049 4420 6f66  d, and the ID of
-000078e0: 2073 7563 6820 6120 6469 6374 696f 6e61   such a dictiona
-000078f0: 7279 2069 7320 6e6f 7420 7370 6563 6966  ry is not specif
-00007900: 6965 642e 2028 4e6f 7465 2074 6861 7420  ied. (Note that 
-00007910: 7468 6520 6d65 616e 696e 6720 6f66 2060  the meaning of `
-00007920: 6030 6060 2069 7320 6469 6666 6572 656e  `0`` is differen
-00007930: 7420 6672 6f6d 203a 7079 3a61 7474 723a  t from :py:attr:
-00007940: 605a 7374 6444 6963 742e 6469 6374 5f69  `ZstdDict.dict_i
-00007950: 6460 2061 7474 7269 6275 7465 2e29 0a0a  d` attribute.)..
-00007960: 2020 2020 4974 2773 2070 6f73 7369 626c      It's possibl
-00007970: 6520 746f 2061 7070 656e 6420 6d6f 7265  e to append more
-00007980: 2069 7465 6d73 2074 6f20 7468 6520 6e61   items to the na
-00007990: 6d65 6474 7570 6c65 2069 6e20 7468 6520  medtuple in the 
-000079a0: 6675 7475 7265 2e0a 0a20 2020 203a 7061  future...    :pa
-000079b0: 7261 6d20 6672 616d 655f 6275 6666 6572  ram frame_buffer
-000079c0: 3a20 4974 2073 686f 756c 6420 7374 6172  : It should star
-000079d0: 7473 2066 726f 6d20 7468 6520 6265 6769  ts from the begi
-000079e0: 6e6e 696e 6720 6f66 2061 2066 7261 6d65  nning of a frame
-000079f0: 2c20 616e 6420 636f 6e74 6169 6e73 2061  , and contains a
-00007a00: 7420 6c65 6173 7420 7468 6520 6672 616d  t least the fram
-00007a10: 6520 6865 6164 6572 2028 3620 746f 2031  e header (6 to 1
-00007a20: 3820 6279 7465 7329 2e0a 2020 2020 3a74  8 bytes)..    :t
-00007a30: 7970 6520 6672 616d 655f 6275 6666 6572  ype frame_buffer
-00007a40: 3a20 6279 7465 732d 6c69 6b65 206f 626a  : bytes-like obj
-00007a50: 6563 740a 2020 2020 3a72 6574 7572 6e3a  ect.    :return:
-00007a60: 2049 6e66 6f72 6d61 7469 6f6e 2061 626f   Information abo
-00007a70: 7574 2061 2066 7261 6d65 2e0a 2020 2020  ut a frame..    
-00007a80: 3a72 7479 7065 3a20 6e61 6d65 6474 7570  :rtype: namedtup
-00007a90: 6c65 0a20 2020 203a 7261 6973 6573 205a  le.    :raises Z
-00007aa0: 7374 6445 7272 6f72 3a20 5768 656e 2070  stdError: When p
-00007ab0: 6172 7369 6e67 2074 6865 2066 7261 6d65  arsing the frame
-00007ac0: 2068 6561 6465 7220 6661 696c 732e 0a0a   header fails...
-00007ad0: 2e2e 2073 6f75 7263 6563 6f64 653a 3a20  .. sourcecode:: 
-00007ae0: 7079 7468 6f6e 0a0a 2020 2020 3e3e 3e20  python..    >>> 
-00007af0: 7079 7a73 7464 2e67 6574 5f66 7261 6d65  pyzstd.get_frame
-00007b00: 5f69 6e66 6f28 636f 6d70 7265 7373 6564  _info(compressed
-00007b10: 5f64 6174 5b3a 3230 5d29 0a20 2020 2066  _dat[:20]).    f
-00007b20: 7261 6d65 5f69 6e66 6f28 6465 636f 6d70  rame_info(decomp
-00007b30: 7265 7373 6564 5f73 697a 653d 3638 3733  ressed_size=6873
-00007b40: 3739 2c20 6469 6374 696f 6e61 7279 5f69  79, dictionary_i
-00007b50: 643d 3130 3430 3939 3232 3638 290a 0a0a  d=1040992268)...
-00007b60: 2e2e 2070 793a 6675 6e63 7469 6f6e 3a3a  .. py:function::
-00007b70: 2067 6574 5f66 7261 6d65 5f73 697a 6528   get_frame_size(
-00007b80: 6672 616d 655f 6275 6666 6572 290a 0a20  frame_buffer).. 
-00007b90: 2020 2047 6574 2074 6865 2073 697a 6520     Get the size 
-00007ba0: 6f66 2061 207a 7374 6420 6672 616d 652c  of a zstd frame,
-00007bb0: 2069 6e63 6c75 6469 6e67 2066 7261 6d65   including frame
-00007bc0: 2068 6561 6465 7220 616e 6420 342d 6279   header and 4-by
-00007bd0: 7465 2063 6865 636b 7375 6d20 6966 2069  te checksum if i
-00007be0: 7420 6861 732e 0a0a 2020 2020 4974 2077  t has...    It w
-00007bf0: 696c 6c20 6974 6572 6174 6520 616c 6c20  ill iterate all 
-00007c00: 626c 6f63 6b73 2720 6865 6164 6572 2077  blocks' header w
-00007c10: 6974 6869 6e20 6120 6672 616d 652c 2074  ithin a frame, t
-00007c20: 6f20 6163 6375 6d75 6c61 7465 2074 6865  o accumulate the
-00007c30: 2066 7261 6d65 2773 2073 697a 652e 0a0a   frame's size...
-00007c40: 2020 2020 3a70 6172 616d 2066 7261 6d65      :param frame
-00007c50: 5f62 7566 6665 723a 2049 7420 7368 6f75  _buffer: It shou
-00007c60: 6c64 2073 7461 7274 7320 6672 6f6d 2074  ld starts from t
-00007c70: 6865 2062 6567 696e 6e69 6e67 206f 6620  he beginning of 
-00007c80: 6120 6672 616d 652c 2061 6e64 2063 6f6e  a frame, and con
-00007c90: 7461 696e 7320 6174 206c 6561 7374 206f  tains at least o
-00007ca0: 6e65 2063 6f6d 706c 6574 6520 6672 616d  ne complete fram
-00007cb0: 652e 0a20 2020 203a 7479 7065 2066 7261  e..    :type fra
-00007cc0: 6d65 5f62 7566 6665 723a 2062 7974 6573  me_buffer: bytes
-00007cd0: 2d6c 696b 6520 6f62 6a65 6374 0a20 2020  -like object.   
-00007ce0: 203a 7265 7475 726e 3a20 5468 6520 7369   :return: The si
-00007cf0: 7a65 206f 6620 6120 7a73 7464 2066 7261  ze of a zstd fra
-00007d00: 6d65 2e0a 2020 2020 3a72 7479 7065 3a20  me..    :rtype: 
-00007d10: 696e 740a 2020 2020 3a72 6169 7365 7320  int.    :raises 
-00007d20: 5a73 7464 4572 726f 723a 2057 6865 6e20  ZstdError: When 
-00007d30: 6974 2066 6169 6c73 2e0a 0a2e 2e20 736f  it fails..... so
-00007d40: 7572 6365 636f 6465 3a3a 2070 7974 686f  urcecode:: pytho
-00007d50: 6e0a 0a20 2020 203e 3e3e 2070 797a 7374  n..    >>> pyzst
-00007d60: 642e 6765 745f 6672 616d 655f 7369 7a65  d.get_frame_size
-00007d70: 2863 6f6d 7072 6573 7365 645f 6461 7429  (compressed_dat)
-00007d80: 0a20 2020 2032 3532 3837 340a 0a0a 4d6f  .    252874...Mo
-00007d90: 6475 6c65 2d6c 6576 656c 2076 6172 6961  dule-level varia
-00007da0: 626c 6573 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  bles.-----------
-00007db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020  -----------..   
-00007dc0: 2054 6869 7320 7365 6374 696f 6e20 636f   This section co
-00007dd0: 6e74 6169 6e73 3a0a 0a20 2020 2020 2020  ntains:..       
-00007de0: 202a 203a 7079 3a64 6174 613a 607a 7374   * :py:data:`zst
-00007df0: 645f 7665 7273 696f 6e60 2c20 6120 6060  d_version`, a ``
-00007e00: 7374 7260 602e 0a20 2020 2020 2020 202a  str``..        *
-00007e10: 203a 7079 3a64 6174 613a 607a 7374 645f   :py:data:`zstd_
-00007e20: 7665 7273 696f 6e5f 696e 666f 602c 2061  version_info`, a
-00007e30: 2060 6074 7570 6c65 6060 2e0a 2020 2020   ``tuple``..    
-00007e40: 2020 2020 2a20 3a70 793a 6461 7461 3a60      * :py:data:`
-00007e50: 636f 6d70 7265 7373 696f 6e4c 6576 656c  compressionLevel
-00007e60: 5f76 616c 7565 7360 2c20 736f 6d65 2076  _values`, some v
-00007e70: 616c 7565 7320 6465 6669 6e65 6420 6279  alues defined by
-00007e80: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-00007e90: 7a73 7464 206c 6962 7261 7279 2e0a 2020  zstd library..  
-00007ea0: 2020 2020 2020 2a20 3a70 793a 6461 7461        * :py:data
-00007eb0: 3a60 7a73 7464 5f73 7570 706f 7274 5f6d  :`zstd_support_m
-00007ec0: 756c 7469 7468 7265 6164 602c 2077 6865  ultithread`, whe
-00007ed0: 7468 6572 2074 6865 2075 6e64 6572 6c79  ther the underly
-00007ee0: 696e 6720 7a73 7464 206c 6962 7261 7279  ing zstd library
-00007ef0: 2073 7570 706f 7274 7320 6d75 6c74 692d   supports multi-
-00007f00: 7468 7265 6164 6564 2063 6f6d 7072 6573  threaded compres
-00007f10: 7369 6f6e 2e0a 0a2e 2e20 7079 3a64 6174  sion..... py:dat
-00007f20: 613a 3a20 7a73 7464 5f76 6572 7369 6f6e  a:: zstd_version
-00007f30: 0a0a 2020 2020 556e 6465 726c 7969 6e67  ..    Underlying
-00007f40: 207a 7374 6420 6c69 6272 6172 7927 7320   zstd library's 
-00007f50: 7665 7273 696f 6e2c 2060 6073 7472 6060  version, ``str``
-00007f60: 2066 6f72 6d2e 0a0a 2e2e 2073 6f75 7263   form..... sourc
-00007f70: 6563 6f64 653a 3a20 7079 7468 6f6e 0a0a  ecode:: python..
-00007f80: 2020 2020 3e3e 3e20 7079 7a73 7464 2e7a      >>> pyzstd.z
-00007f90: 7374 645f 7665 7273 696f 6e0a 2020 2020  std_version.    
-00007fa0: 2731 2e34 2e35 270a 0a0a 2e2e 2070 793a  '1.4.5'..... py:
-00007fb0: 6461 7461 3a3a 207a 7374 645f 7665 7273  data:: zstd_vers
-00007fc0: 696f 6e5f 696e 666f 0a0a 2020 2020 556e  ion_info..    Un
-00007fd0: 6465 726c 7969 6e67 207a 7374 6420 6c69  derlying zstd li
-00007fe0: 6272 6172 7927 7320 7665 7273 696f 6e2c  brary's version,
-00007ff0: 2060 6074 7570 6c65 6060 2066 6f72 6d2e   ``tuple`` form.
-00008000: 0a0a 2e2e 2073 6f75 7263 6563 6f64 653a  .... sourcecode:
-00008010: 3a20 7079 7468 6f6e 0a0a 2020 2020 3e3e  : python..    >>
-00008020: 3e20 7079 7a73 7464 2e7a 7374 645f 7665  > pyzstd.zstd_ve
-00008030: 7273 696f 6e5f 696e 666f 0a20 2020 2028  rsion_info.    (
-00008040: 312c 2034 2c20 3529 0a0a 0a2e 2e20 7079  1, 4, 5)..... py
-00008050: 3a64 6174 613a 3a20 636f 6d70 7265 7373  :data:: compress
-00008060: 696f 6e4c 6576 656c 5f76 616c 7565 730a  ionLevel_values.
-00008070: 0a20 2020 2041 2033 2d69 7465 6d20 6e61  .    A 3-item na
-00008080: 6d65 6474 7570 6c65 2c20 7661 6c75 6573  medtuple, values
-00008090: 2064 6566 696e 6564 2062 7920 7468 6520   defined by the 
-000080a0: 756e 6465 726c 7969 6e67 207a 7374 6420  underlying zstd 
-000080b0: 6c69 6272 6172 792c 2073 6565 203a 7265  library, see :re
-000080c0: 663a 6063 6f6d 7072 6573 7369 6f6e 206c  f:`compression l
-000080d0: 6576 656c 3c63 6f6d 7072 6573 7369 6f6e  evel<compression
-000080e0: 5f6c 6576 656c 3e60 2066 6f72 2064 6574  _level>` for det
-000080f0: 6169 6c73 2e0a 0a20 2020 2060 6064 6566  ails...    ``def
-00008100: 6175 6c74 6060 2069 7320 6465 6661 756c  ault`` is defaul
-00008110: 7420 636f 6d70 7265 7373 696f 6e20 6c65  t compression le
-00008120: 7665 6c2c 2069 7420 6973 2075 7365 6420  vel, it is used 
-00008130: 7768 656e 2063 6f6d 7072 6573 7369 6f6e  when compression
-00008140: 206c 6576 656c 2069 7320 7365 7420 746f   level is set to
-00008150: 2060 6030 6060 206f 7220 6e6f 7420 7365   ``0`` or not se
-00008160: 742e 0a0a 2020 2020 6060 6d69 6e60 602f  t...    ``min``/
-00008170: 6060 6d61 7860 6020 6172 6520 6d69 6e69  ``max`` are mini
-00008180: 6d75 6d2f 6d61 7869 6d75 6d20 6176 6169  mum/maximum avai
-00008190: 6c61 626c 6520 7661 6c75 6573 206f 6620  lable values of 
-000081a0: 636f 6d70 7265 7373 696f 6e20 6c65 7665  compression leve
-000081b0: 6c2c 2062 6f74 6820 696e 636c 7573 6976  l, both inclusiv
-000081c0: 652e 0a0a 2e2e 2073 6f75 7263 6563 6f64  e..... sourcecod
-000081d0: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-000081e0: 3e3e 3e20 7079 7a73 7464 2e63 6f6d 7072  >>> pyzstd.compr
-000081f0: 6573 7369 6f6e 4c65 7665 6c5f 7661 6c75  essionLevel_valu
-00008200: 6573 2020 2320 3133 3130 3732 203d 2031  es  # 131072 = 1
-00008210: 3238 2a31 3032 340a 2020 2020 7661 6c75  28*1024.    valu
-00008220: 6573 2864 6566 6175 6c74 3d33 2c20 6d69  es(default=3, mi
-00008230: 6e3d 2d31 3331 3037 322c 206d 6178 3d32  n=-131072, max=2
-00008240: 3229 0a0a 0a2e 2e20 7079 3a64 6174 613a  2)..... py:data:
-00008250: 3a20 7a73 7464 5f73 7570 706f 7274 5f6d  : zstd_support_m
-00008260: 756c 7469 7468 7265 6164 0a0a 2020 2020  ultithread..    
-00008270: 5768 6574 6865 7220 7468 6520 756e 6465  Whether the unde
-00008280: 726c 7969 6e67 207a 7374 6420 6c69 6272  rlying zstd libr
-00008290: 6172 7920 7761 7320 636f 6d70 696c 6564  ary was compiled
-000082a0: 2077 6974 6820 3a72 6566 3a60 6d75 6c74   with :ref:`mult
-000082b0: 692d 7468 7265 6164 6564 2063 6f6d 7072  i-threaded compr
-000082c0: 6573 7369 6f6e 3c6d 745f 636f 6d70 7265  ession<mt_compre
-000082d0: 7373 696f 6e3e 6020 7375 7070 6f72 742e  ssion>` support.
-000082e0: 0a0a 2020 2020 4974 2773 2061 6c6d 6f73  ..    It's almos
-000082f0: 7420 616c 7761 7973 2060 6054 7275 6560  t always ``True`
-00008300: 602e 0a0a 2020 2020 4974 2773 2060 6046  `...    It's ``F
-00008310: 616c 7365 6060 2077 6865 6e20 6479 6e61  alse`` when dyna
-00008320: 6d69 6361 6c6c 7920 6c69 6e6b 6564 2074  mically linked t
-00008330: 6f20 7a73 7464 206c 6962 7261 7279 2074  o zstd library t
-00008340: 6861 7420 636f 6d70 696c 6564 2077 6974  hat compiled wit
-00008350: 686f 7574 206d 756c 7469 2d74 6872 6561  hout multi-threa
-00008360: 6465 6420 7375 7070 6f72 742e 204f 7264  ded support. Ord
-00008370: 696e 6172 7920 7573 6572 7320 7769 6c6c  inary users will
-00008380: 206e 6f74 206d 6565 7420 7468 6973 2073   not meet this s
-00008390: 6974 7561 7469 6f6e 2e0a 0a2e 2e20 7665  ituation..... ve
-000083a0: 7273 696f 6e61 6464 6564 3a3a 2030 2e31  rsionadded:: 0.1
-000083b0: 352e 310a 0a2e 2e20 736f 7572 6365 636f  5.1.... sourceco
-000083c0: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
-000083d0: 203e 3e3e 2070 797a 7374 642e 7a73 7464   >>> pyzstd.zstd
-000083e0: 5f73 7570 706f 7274 5f6d 756c 7469 7468  _support_multith
-000083f0: 7265 6164 0a20 2020 2054 7275 650a 0a0a  read.    True...
-00008400: 5a73 7464 4669 6c65 2063 6c61 7373 2061  ZstdFile class a
-00008410: 6e64 206f 7065 6e28 2920 6675 6e63 7469  nd open() functi
-00008420: 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  on.-------------
-00008430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008440: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020  ----------..    
-00008450: 5468 6973 2073 6563 7469 6f6e 2063 6f6e  This section con
-00008460: 7461 696e 733a 0a0a 2020 2020 2020 2020  tains:..        
-00008470: 2a20 636c 6173 7320 3a70 793a 636c 6173  * class :py:clas
-00008480: 733a 605a 7374 6446 696c 6560 2c20 6f70  s:`ZstdFile`, op
-00008490: 656e 2061 207a 7374 642d 636f 6d70 7265  en a zstd-compre
-000084a0: 7373 6564 2066 696c 6520 696e 2062 696e  ssed file in bin
-000084b0: 6172 7920 6d6f 6465 2e0a 2020 2020 2020  ary mode..      
-000084c0: 2020 2a20 6675 6e63 7469 6f6e 203a 7079    * function :py
-000084d0: 3a66 756e 633a 606f 7065 6e60 2c20 6f70  :func:`open`, op
-000084e0: 656e 2061 207a 7374 642d 636f 6d70 7265  en a zstd-compre
-000084f0: 7373 6564 2066 696c 6520 696e 2062 696e  ssed file in bin
-00008500: 6172 7920 6f72 2074 6578 7420 6d6f 6465  ary or text mode
-00008510: 2e0a 0a2e 2e20 7079 3a63 6c61 7373 3a3a  ..... py:class::
-00008520: 205a 7374 6446 696c 650a 0a20 2020 204f   ZstdFile..    O
-00008530: 7065 6e20 6120 7a73 7464 2d63 6f6d 7072  pen a zstd-compr
-00008540: 6573 7365 6420 6669 6c65 2069 6e20 6269  essed file in bi
-00008550: 6e61 7279 206d 6f64 652e 0a0a 2020 2020  nary mode...    
-00008560: 5468 6973 2063 6c61 7373 2069 7320 7665  This class is ve
-00008570: 7279 2073 696d 696c 6172 2074 6f20 6062  ry similar to `b
-00008580: 7a32 2e42 5a32 4669 6c65 203c 6874 7470  z2.BZ2File <http
-00008590: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-000085a0: 6f72 672f 332f 6c69 6272 6172 792f 627a  org/3/library/bz
-000085b0: 322e 6874 6d6c 2362 7a32 2e42 5a32 4669  2.html#bz2.BZ2Fi
-000085c0: 6c65 3e60 5f20 2f20 2060 677a 6970 2e47  le>`_ /  `gzip.G
-000085d0: 7a69 7046 696c 6520 3c68 7474 7073 3a2f  zipFile <https:/
-000085e0: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
-000085f0: 2f33 2f6c 6962 7261 7279 2f67 7a69 702e  /3/library/gzip.
-00008600: 6874 6d6c 2367 7a69 702e 477a 6970 4669  html#gzip.GzipFi
-00008610: 6c65 3e60 5f20 2f20 606c 7a6d 612e 4c5a  le>`_ / `lzma.LZ
-00008620: 4d41 4669 6c65 203c 6874 7470 733a 2f2f  MAFile <https://
-00008630: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-00008640: 332f 6c69 6272 6172 792f 6c7a 6d61 2e68  3/library/lzma.h
-00008650: 746d 6c23 6c7a 6d61 2e4c 5a4d 4146 696c  tml#lzma.LZMAFil
-00008660: 653e 605f 2063 6c61 7373 6573 2069 6e20  e>`_ classes in 
-00008670: 5079 7468 6f6e 2073 7461 6e64 6172 6420  Python standard 
-00008680: 6c69 6272 6172 792e 0a0a 2020 2020 4c69  library...    Li
-00008690: 6b65 2042 5a32 4669 6c65 2f47 7a69 7046  ke BZ2File/GzipF
-000086a0: 696c 652f 4c5a 4d41 4669 6c65 2063 6c61  ile/LZMAFile cla
-000086b0: 7373 6573 2c20 5a73 7464 4669 6c65 2069  sses, ZstdFile i
-000086c0: 7320 6e6f 7420 7468 7265 6164 2d73 6166  s not thread-saf
-000086d0: 652c 2073 6f20 6966 2079 6f75 206e 6565  e, so if you nee
-000086e0: 6420 746f 2075 7365 2061 2073 696e 676c  d to use a singl
-000086f0: 6520 5a73 7464 4669 6c65 206f 626a 6563  e ZstdFile objec
-00008700: 7420 6672 6f6d 206d 756c 7469 706c 6520  t from multiple 
-00008710: 7468 7265 6164 732c 2069 7420 6973 206e  threads, it is n
-00008720: 6563 6573 7361 7279 2074 6f20 7072 6f74  ecessary to prot
-00008730: 6563 7420 6974 2077 6974 6820 6120 6c6f  ect it with a lo
-00008740: 636b 2e0a 0a20 2020 2049 7420 6361 6e20  ck...    It can 
-00008750: 6265 2075 7365 6420 7769 7468 2050 7974  be used with Pyt
-00008760: 686f 6e27 7320 6060 7461 7266 696c 6560  hon's ``tarfile`
-00008770: 6020 6d6f 6475 6c65 2c20 7365 6520 3a72  ` module, see :r
-00008780: 6566 3a60 7468 6973 206e 6f74 653c 7769  ef:`this note<wi
-00008790: 7468 5f74 6172 6669 6c65 3e60 2e0a 0a20  th_tarfile>`... 
-000087a0: 2020 202e 2e20 7079 3a6d 6574 686f 643a     .. py:method:
-000087b0: 3a20 5f5f 696e 6974 5f5f 2873 656c 662c  : __init__(self,
-000087c0: 2066 696c 656e 616d 652c 206d 6f64 653d   filename, mode=
-000087d0: 2272 222c 202a 2c20 6c65 7665 6c5f 6f72  "r", *, level_or
-000087e0: 5f6f 7074 696f 6e3d 4e6f 6e65 2c20 7a73  _option=None, zs
-000087f0: 7464 5f64 6963 743d 4e6f 6e65 290a 0a20  td_dict=None).. 
-00008800: 2020 2020 2020 2054 6865 202a 6669 6c65         The *file
-00008810: 6e61 6d65 2a20 7061 7261 6d65 7465 7220  name* parameter 
-00008820: 6361 6e20 6265 2061 6e20 6578 6973 7469  can be an existi
-00008830: 6e67 2060 6669 6c65 206f 626a 6563 7420  ng `file object 
-00008840: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
-00008850: 7468 6f6e 2e6f 7267 2f33 2f67 6c6f 7373  thon.org/3/gloss
-00008860: 6172 792e 6874 6d6c 2374 6572 6d2d 6669  ary.html#term-fi
-00008870: 6c65 2d6f 626a 6563 743e 605f 2074 6f20  le-object>`_ to 
-00008880: 7772 6170 2c20 6f72 2074 6865 206e 616d  wrap, or the nam
-00008890: 6520 6f66 2074 6865 2066 696c 6520 746f  e of the file to
-000088a0: 206f 7065 6e20 2861 7320 6120 6060 7374   open (as a ``st
-000088b0: 7260 602c 2060 6062 7974 6573 6060 206f  r``, ``bytes`` o
-000088c0: 7220 6070 6174 682d 6c69 6b65 203c 6874  r `path-like <ht
-000088d0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-000088e0: 6e2e 6f72 672f 332f 676c 6f73 7361 7279  n.org/3/glossary
-000088f0: 2e68 746d 6c23 7465 726d 2d70 6174 682d  .html#term-path-
-00008900: 6c69 6b65 2d6f 626a 6563 743e 605f 206f  like-object>`_ o
-00008910: 626a 6563 7429 2e20 5768 656e 2077 7261  bject). When wra
-00008920: 7070 696e 6720 616e 2065 7869 7374 696e  pping an existin
-00008930: 6720 6669 6c65 206f 626a 6563 742c 2074  g file object, t
-00008940: 6865 2077 7261 7070 6564 2066 696c 6520  he wrapped file 
-00008950: 7769 6c6c 206e 6f74 2062 6520 636c 6f73  will not be clos
-00008960: 6564 2077 6865 6e20 7468 6520 5a73 7464  ed when the Zstd
-00008970: 4669 6c65 2069 7320 636c 6f73 6564 2e0a  File is closed..
-00008980: 0a20 2020 2020 2020 2054 6865 202a 6d6f  .        The *mo
-00008990: 6465 2a20 7061 7261 6d65 7465 7220 6361  de* parameter ca
-000089a0: 6e20 6265 2065 6974 6865 7220 2272 2220  n be either "r" 
-000089b0: 666f 7220 7265 6164 696e 6720 2864 6566  for reading (def
-000089c0: 6175 6c74 292c 2022 7722 2066 6f72 206f  ault), "w" for o
-000089d0: 7665 7277 7269 7469 6e67 2c20 2278 2220  verwriting, "x" 
-000089e0: 666f 7220 6578 636c 7573 6976 6520 6372  for exclusive cr
-000089f0: 6561 7469 6f6e 2c20 6f72 2022 6122 2066  eation, or "a" f
-00008a00: 6f72 2061 7070 656e 6469 6e67 2e20 5468  or appending. Th
-00008a10: 6573 6520 6361 6e20 6571 7569 7661 6c65  ese can equivale
-00008a20: 6e74 6c79 2062 6520 6769 7665 6e20 6173  ntly be given as
-00008a30: 2022 7262 222c 2022 7762 222c 2022 7862   "rb", "wb", "xb
-00008a40: 2220 616e 6420 2261 6222 2072 6573 7065  " and "ab" respe
-00008a50: 6374 6976 656c 792e 0a0a 2020 2020 2020  ctively...      
-00008a60: 2020 4966 2069 6e20 7265 6164 696e 6720    If in reading 
-00008a70: 6d6f 6465 2028 6465 636f 6d70 7265 7373  mode (decompress
-00008a80: 696f 6e29 3a0a 0a20 2020 2020 2020 2020  ion):..         
-00008a90: 2020 202a 2054 6865 202a 6c65 7665 6c5f     * The *level_
-00008aa0: 6f72 5f6f 7074 696f 6e2a 2070 6172 616d  or_option* param
-00008ab0: 6574 6572 2063 616e 206f 6e6c 7920 6265  eter can only be
-00008ac0: 2061 2060 6064 6963 7460 6020 6f62 6a65   a ``dict`` obje
-00008ad0: 6374 2c20 7468 6174 2072 6570 7265 7365  ct, that represe
-00008ae0: 6e74 7320 6465 636f 6d70 7265 7373 696f  nts decompressio
-00008af0: 6e20 6f70 7469 6f6e 2e20 4974 2064 6f65  n option. It doe
-00008b00: 736e 2774 2073 7570 706f 7274 2060 6069  sn't support ``i
-00008b10: 6e74 6060 2074 7970 6520 636f 6d70 7265  nt`` type compre
-00008b20: 7373 696f 6e20 6c65 7665 6c20 696e 2074  ssion level in t
-00008b30: 6869 7320 6361 7365 2e0a 2020 2020 2020  his case..      
-00008b40: 2020 2020 2020 2a20 5468 6520 696e 7075        * The inpu
-00008b50: 7420 6669 6c65 206d 6179 2062 6520 7468  t file may be th
-00008b60: 6520 636f 6e63 6174 656e 6174 696f 6e20  e concatenation 
-00008b70: 6f66 206d 756c 7469 706c 6520 3a72 6566  of multiple :ref
-00008b80: 3a60 6672 616d 6573 3c66 7261 6d65 5f62  :`frames<frame_b
-00008b90: 6c6f 636b 3e60 2e0a 0a20 2020 2049 6e20  lock>`...    In 
-00008ba0: 7772 6974 696e 6720 6d6f 6465 2028 636f  writing mode (co
-00008bb0: 6d70 7265 7373 696f 6e29 2c20 7468 6573  mpression), thes
-00008bc0: 6520 6d65 7468 6f64 7320 6172 6520 6176  e methods are av
-00008bd0: 6169 6c61 626c 653a 0a0a 2020 2020 2020  ailable:..      
-00008be0: 2020 2a20 602e 7772 6974 6528 6229 203c    * `.write(b) <
-00008bf0: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-00008c00: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
-00008c10: 792f 696f 2e68 746d 6c23 696f 2e42 7566  y/io.html#io.Buf
-00008c20: 6665 7265 6449 4f42 6173 652e 7772 6974  feredIOBase.writ
-00008c30: 653e 605f 0a20 2020 2020 2020 202a 2060  e>`_.        * `
-00008c40: 2e66 6c75 7368 2829 203c 6874 7470 733a  .flush() <https:
-00008c50: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00008c60: 672f 332f 6c69 6272 6172 792f 696f 2e68  g/3/library/io.h
-00008c70: 746d 6c23 696f 2e49 4f42 6173 652e 666c  tml#io.IOBase.fl
-00008c80: 7573 683e 605f 2c20 666c 7573 6820 746f  ush>`_, flush to
-00008c90: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-00008ca0: 7374 7265 616d 2e20 4974 2075 7365 7320  stream. It uses 
-00008cb0: 3a70 793a 6174 7472 3a60 5a73 7464 436f  :py:attr:`ZstdCo
-00008cc0: 6d70 7265 7373 6f72 2e46 4c55 5348 5f42  mpressor.FLUSH_B
-00008cd0: 4c4f 434b 6020 6d6f 6465 2c20 6162 7573  LOCK` mode, abus
-00008ce0: 6520 6f66 2074 6869 7320 6d65 7468 6f64  e of this method
-00008cf0: 2077 696c 6c20 7265 6475 6365 2063 6f6d   will reduce com
-00008d00: 7072 6573 7369 6f6e 2072 6174 696f 2c20  pression ratio, 
-00008d10: 7573 6520 6974 206f 6e6c 7920 7768 656e  use it only when
-00008d20: 206e 6563 6573 7361 7279 2e20 4966 2074   necessary. If t
-00008d30: 6865 2070 726f 6772 616d 2069 7320 696e  he program is in
-00008d40: 7465 7272 7570 7465 6420 6166 7465 7277  terrupted afterw
-00008d50: 6172 6473 2c20 616c 6c20 6461 7461 2063  ards, all data c
-00008d60: 616e 2062 6520 7265 636f 7665 7265 642e  an be recovered.
-00008d70: 2054 6f20 656e 7375 7265 2073 6176 696e   To ensure savin
-00008d80: 6720 746f 2064 6973 6b2c 2061 6c73 6f20  g to disk, also 
-00008d90: 6e65 6564 2060 6f73 2e66 7379 6e63 2866  need `os.fsync(f
-00008da0: 6429 203c 6874 7470 733a 2f2f 646f 6373  d) <https://docs
-00008db0: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-00008dc0: 6272 6172 792f 6f73 2e68 746d 6c23 6f73  brary/os.html#os
-00008dd0: 2e66 7379 6e63 3e60 5f2e 2020 282a 496d  .fsync>`_.  (*Im
-00008de0: 706c 656d 656e 7465 6420 696e 2076 6572  plemented in ver
-00008df0: 7369 6f6e 2030 2e31 352e 312a 290a 0a20  sion 0.15.1*).. 
-00008e00: 2020 2049 6e20 7265 6164 696e 6720 6d6f     In reading mo
-00008e10: 6465 2028 6465 636f 6d70 7265 7373 696f  de (decompressio
-00008e20: 6e29 2c20 7468 6573 6520 6d65 7468 6f64  n), these method
-00008e30: 7320 616e 6420 7374 6174 656d 656e 7420  s and statement 
-00008e40: 6172 6520 6176 6169 6c61 626c 653a 0a0a  are available:..
-00008e50: 2020 2020 2020 2020 2a20 602e 7265 6164          * `.read
-00008e60: 2873 697a 653d 2d31 2920 3c68 7474 7073  (size=-1) <https
-00008e70: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00008e80: 7267 2f33 2f6c 6962 7261 7279 2f69 6f2e  rg/3/library/io.
-00008e90: 6874 6d6c 2369 6f2e 4275 6666 6572 6564  html#io.Buffered
-00008ea0: 5265 6164 6572 2e72 6561 643e 605f 0a20  Reader.read>`_. 
-00008eb0: 2020 2020 2020 202a 2060 2e72 6561 6431         * `.read1
-00008ec0: 2873 697a 653d 2d31 2920 3c68 7474 7073  (size=-1) <https
-00008ed0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00008ee0: 7267 2f33 2f6c 6962 7261 7279 2f69 6f2e  rg/3/library/io.
-00008ef0: 6874 6d6c 2369 6f2e 4275 6666 6572 6564  html#io.Buffered
-00008f00: 5265 6164 6572 2e72 6561 6431 3e60 5f0a  Reader.read1>`_.
-00008f10: 2020 2020 2020 2020 2a20 602e 7265 6164          * `.read
-00008f20: 696e 746f 2862 2920 3c68 7474 7073 3a2f  into(b) <https:/
-00008f30: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
-00008f40: 2f33 2f6c 6962 7261 7279 2f69 6f2e 6874  /3/library/io.ht
-00008f50: 6d6c 2369 6f2e 4275 6666 6572 6564 494f  ml#io.BufferedIO
-00008f60: 4261 7365 2e72 6561 6469 6e74 6f3e 605f  Base.readinto>`_
-00008f70: 0a20 2020 2020 2020 202a 2060 2e72 6561  .        * `.rea
-00008f80: 6469 6e74 6f31 2862 2920 3c68 7474 7073  dinto1(b) <https
-00008f90: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00008fa0: 7267 2f33 2f6c 6962 7261 7279 2f69 6f2e  rg/3/library/io.
-00008fb0: 6874 6d6c 2369 6f2e 4275 6666 6572 6564  html#io.Buffered
-00008fc0: 494f 4261 7365 2e72 6561 6469 6e74 6f31  IOBase.readinto1
-00008fd0: 3e60 5f0a 2020 2020 2020 2020 2a20 602e  >`_.        * `.
-00008fe0: 7265 6164 6c69 6e65 2873 697a 653d 2d31  readline(size=-1
-00008ff0: 2920 3c68 7474 7073 3a2f 2f64 6f63 732e  ) <https://docs.
-00009000: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
-00009010: 7261 7279 2f69 6f2e 6874 6d6c 2369 6f2e  rary/io.html#io.
-00009020: 494f 4261 7365 2e72 6561 646c 696e 653e  IOBase.readline>
-00009030: 605f 0a20 2020 2020 2020 202a 2060 2e73  `_.        * `.s
-00009040: 6565 6b28 6f66 6673 6574 2c20 7768 656e  eek(offset, when
-00009050: 6365 3d69 6f2e 5345 454b 5f53 4554 2920  ce=io.SEEK_SET) 
-00009060: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
-00009070: 7468 6f6e 2e6f 7267 2f33 2f6c 6962 7261  thon.org/3/libra
-00009080: 7279 2f69 6f2e 6874 6d6c 2369 6f2e 494f  ry/io.html#io.IO
-00009090: 4261 7365 2e73 6565 6b3e 605f 2c20 6e6f  Base.seek>`_, no
-000090a0: 7465 2074 6861 7420 6966 2060 602e 7365  te that if ``.se
-000090b0: 656b 2829 6060 2074 6f20 2270 7265 7669  ek()`` to "previ
-000090c0: 6f75 7320 706f 7369 7469 6f6e 2220 6f72  ous position" or
-000090d0: 2022 706f 7369 7469 6f6e 2072 656c 6174   "position relat
-000090e0: 6976 6520 746f 2045 4f46 2028 7468 6520  ive to EOF (the 
-000090f0: 6669 7273 7420 7469 6d65 2922 2c20 7468  first time)", th
-00009100: 6520 6465 636f 6d70 7265 7373 696f 6e20  e decompression 
-00009110: 6861 7320 746f 2062 6520 7265 7374 6172  has to be restar
-00009120: 7465 6420 6672 6f6d 207a 6572 6f2e 0a20  ted from zero.. 
-00009130: 2020 2020 2020 202a 2060 2e70 6565 6b28         * `.peek(
-00009140: 7369 7a65 3d2d 3129 203c 6874 7470 733a  size=-1) <https:
-00009150: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00009160: 672f 332f 6c69 6272 6172 792f 696f 2e68  g/3/library/io.h
-00009170: 746d 6c23 696f 2e42 7566 6665 7265 6452  tml#io.BufferedR
-00009180: 6561 6465 722e 7065 656b 3e60 5f0a 2020  eader.peek>`_.  
-00009190: 2020 2020 2020 2a20 6049 7465 7261 7469        * `Iterati
-000091a0: 6f6e 203c 6874 7470 733a 2f2f 646f 6373  on <https://docs
-000091b0: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-000091c0: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
-000091d0: 2e49 4f42 6173 653e 605f 2c20 7969 656c  .IOBase>`_, yiel
-000091e0: 6420 6c69 6e65 732c 206c 696e 6520 7465  d lines, line te
-000091f0: 726d 696e 6174 6f72 2069 7320 6060 6227  rminator is ``b'
-00009200: 5c6e 2760 602e 0a0a 2020 2020 496e 2062  \n'``...    In b
-00009210: 6f74 6820 7265 6164 696e 6720 616e 6420  oth reading and 
-00009220: 7772 6974 696e 6720 6d6f 6465 732c 2074  writing modes, t
-00009230: 6865 7365 206d 6574 686f 6473 2061 6e64  hese methods and
-00009240: 2070 726f 7065 7274 7920 6172 6520 6176   property are av
-00009250: 6169 6c61 626c 653a 0a0a 2020 2020 2020  ailable:..      
-00009260: 2020 2a20 602e 636c 6f73 6528 2920 3c68    * `.close() <h
-00009270: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
-00009280: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
-00009290: 2f69 6f2e 6874 6d6c 2369 6f2e 494f 4261  /io.html#io.IOBa
-000092a0: 7365 2e63 6c6f 7365 3e60 5f0a 2020 2020  se.close>`_.    
-000092b0: 2020 2020 2a20 602e 7465 6c6c 2829 203c      * `.tell() <
-000092c0: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-000092d0: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
-000092e0: 792f 696f 2e68 746d 6c23 696f 2e49 4f42  y/io.html#io.IOB
-000092f0: 6173 652e 7465 6c6c 3e60 5f0a 2020 2020  ase.tell>`_.    
-00009300: 2020 2020 2a20 602e 6669 6c65 6e6f 2829      * `.fileno()
-00009310: 203c 6874 7470 733a 2f2f 646f 6373 2e70   <https://docs.p
-00009320: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
-00009330: 6172 792f 696f 2e68 746d 6c23 696f 2e49  ary/io.html#io.I
-00009340: 4f42 6173 652e 6669 6c65 6e6f 3e60 5f0a  OBase.fileno>`_.
-00009350: 2020 2020 2020 2020 2a20 602e 636c 6f73          * `.clos
-00009360: 6564 203c 6874 7470 733a 2f2f 646f 6373  ed <https://docs
-00009370: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-00009380: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
-00009390: 2e49 4f42 6173 652e 636c 6f73 6564 3e60  .IOBase.closed>`
-000093a0: 5f20 2861 2070 726f 7065 7274 7920 6174  _ (a property at
-000093b0: 7472 6962 7574 6529 0a20 2020 2020 2020  tribute).       
-000093c0: 202a 2060 2e77 7269 7461 626c 6528 2920   * `.writable() 
-000093d0: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
-000093e0: 7468 6f6e 2e6f 7267 2f33 2f6c 6962 7261  thon.org/3/libra
-000093f0: 7279 2f69 6f2e 6874 6d6c 2369 6f2e 494f  ry/io.html#io.IO
-00009400: 4261 7365 2e77 7269 7461 626c 653e 605f  Base.writable>`_
-00009410: 0a20 2020 2020 2020 202a 2060 2e72 6561  .        * `.rea
-00009420: 6461 626c 6528 2920 3c68 7474 7073 3a2f  dable() <https:/
-00009430: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
-00009440: 2f33 2f6c 6962 7261 7279 2f69 6f2e 6874  /3/library/io.ht
-00009450: 6d6c 2369 6f2e 494f 4261 7365 2e72 6561  ml#io.IOBase.rea
-00009460: 6461 626c 653e 605f 0a20 2020 2020 2020  dable>`_.       
-00009470: 202a 2060 2e73 6565 6b61 626c 6528 2920   * `.seekable() 
-00009480: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
-00009490: 7468 6f6e 2e6f 7267 2f33 2f6c 6962 7261  thon.org/3/libra
-000094a0: 7279 2f69 6f2e 6874 6d6c 2369 6f2e 494f  ry/io.html#io.IO
-000094b0: 4261 7365 2e73 6565 6b61 626c 653e 605f  Base.seekable>`_
-000094c0: 0a0a 2e2e 2070 793a 6675 6e63 7469 6f6e  .... py:function
-000094d0: 3a3a 206f 7065 6e28 6669 6c65 6e61 6d65  :: open(filename
-000094e0: 2c20 6d6f 6465 3d22 7262 222c 202a 2c20  , mode="rb", *, 
-000094f0: 6c65 7665 6c5f 6f72 5f6f 7074 696f 6e3d  level_or_option=
-00009500: 4e6f 6e65 2c20 7a73 7464 5f64 6963 743d  None, zstd_dict=
-00009510: 4e6f 6e65 2c20 656e 636f 6469 6e67 3d4e  None, encoding=N
-00009520: 6f6e 652c 2065 7272 6f72 733d 4e6f 6e65  one, errors=None
-00009530: 2c20 6e65 776c 696e 653d 4e6f 6e65 290a  , newline=None).
-00009540: 0a20 2020 204f 7065 6e20 6120 7a73 7464  .    Open a zstd
-00009550: 2d63 6f6d 7072 6573 7365 6420 6669 6c65  -compressed file
-00009560: 2069 6e20 6269 6e61 7279 206f 7220 7465   in binary or te
-00009570: 7874 206d 6f64 652c 2072 6574 7572 6e69  xt mode, returni
-00009580: 6e67 2061 2066 696c 6520 6f62 6a65 6374  ng a file object
-00009590: 2e0a 0a20 2020 2054 6869 7320 6675 6e63  ...    This func
-000095a0: 7469 6f6e 2069 7320 7665 7279 2073 696d  tion is very sim
-000095b0: 696c 6172 2074 6f20 6062 7a32 2e6f 7065  ilar to `bz2.ope
-000095c0: 6e28 2920 3c68 7474 7073 3a2f 2f64 6f63  n() <https://doc
-000095d0: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-000095e0: 6962 7261 7279 2f62 7a32 2e68 746d 6c23  ibrary/bz2.html#
-000095f0: 627a 322e 6f70 656e 3e60 5f20 2f20 6067  bz2.open>`_ / `g
-00009600: 7a69 702e 6f70 656e 2829 203c 6874 7470  zip.open() <http
-00009610: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-00009620: 6f72 672f 332f 6c69 6272 6172 792f 677a  org/3/library/gz
-00009630: 6970 2e68 746d 6c23 677a 6970 2e6f 7065  ip.html#gzip.ope
-00009640: 6e3e 605f 202f 2060 6c7a 6d61 2e6f 7065  n>`_ / `lzma.ope
-00009650: 6e28 2920 3c68 7474 7073 3a2f 2f64 6f63  n() <https://doc
-00009660: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-00009670: 6962 7261 7279 2f6c 7a6d 612e 6874 6d6c  ibrary/lzma.html
-00009680: 236c 7a6d 612e 6f70 656e 3e60 5f20 6675  #lzma.open>`_ fu
-00009690: 6e63 7469 6f6e 7320 696e 2050 7974 686f  nctions in Pytho
-000096a0: 6e20 7374 616e 6461 7264 206c 6962 7261  n standard libra
-000096b0: 7279 2e0a 0a20 2020 2054 6865 202a 6669  ry...    The *fi
-000096c0: 6c65 6e61 6d65 2a20 7061 7261 6d65 7465  lename* paramete
-000096d0: 7220 6361 6e20 6265 2061 6e20 6578 6973  r can be an exis
-000096e0: 7469 6e67 2060 6669 6c65 206f 626a 6563  ting `file objec
-000096f0: 7420 3c68 7474 7073 3a2f 2f64 6f63 732e  t <https://docs.
-00009700: 7079 7468 6f6e 2e6f 7267 2f33 2f67 6c6f  python.org/3/glo
-00009710: 7373 6172 792e 6874 6d6c 2374 6572 6d2d  ssary.html#term-
-00009720: 6669 6c65 2d6f 626a 6563 743e 605f 2074  file-object>`_ t
-00009730: 6f20 7772 6170 2c20 6f72 2074 6865 206e  o wrap, or the n
-00009740: 616d 6520 6f66 2074 6865 2066 696c 6520  ame of the file 
-00009750: 746f 206f 7065 6e20 2861 7320 6120 6060  to open (as a ``
-00009760: 7374 7260 602c 2060 6062 7974 6573 6060  str``, ``bytes``
-00009770: 206f 7220 6070 6174 682d 6c69 6b65 203c   or `path-like <
-00009780: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-00009790: 686f 6e2e 6f72 672f 332f 676c 6f73 7361  hon.org/3/glossa
-000097a0: 7279 2e68 746d 6c23 7465 726d 2d70 6174  ry.html#term-pat
-000097b0: 682d 6c69 6b65 2d6f 626a 6563 743e 605f  h-like-object>`_
-000097c0: 206f 626a 6563 7429 2e20 5768 656e 2077   object). When w
-000097d0: 7261 7070 696e 6720 616e 2065 7869 7374  rapping an exist
-000097e0: 696e 6720 6669 6c65 206f 626a 6563 742c  ing file object,
-000097f0: 2074 6865 2077 7261 7070 6564 2066 696c   the wrapped fil
-00009800: 6520 7769 6c6c 206e 6f74 2062 6520 636c  e will not be cl
-00009810: 6f73 6564 2077 6865 6e20 7468 6520 7265  osed when the re
-00009820: 7475 726e 6564 2066 696c 6520 6f62 6a65  turned file obje
-00009830: 6374 2069 7320 636c 6f73 6564 2e0a 0a20  ct is closed... 
-00009840: 2020 2054 6865 202a 6d6f 6465 2a20 7061     The *mode* pa
-00009850: 7261 6d65 7465 7220 6361 6e20 6265 2061  rameter can be a
-00009860: 6e79 206f 6620 2272 222c 2022 7262 222c  ny of "r", "rb",
-00009870: 2022 7722 2c20 2277 6222 2c20 2278 222c   "w", "wb", "x",
-00009880: 2022 7862 222c 2022 6122 206f 7220 2261   "xb", "a" or "a
-00009890: 6222 2066 6f72 2062 696e 6172 7920 6d6f  b" for binary mo
-000098a0: 6465 2c20 6f72 2022 7274 222c 2022 7774  de, or "rt", "wt
-000098b0: 222c 2022 7874 222c 206f 7220 2261 7422  ", "xt", or "at"
-000098c0: 2066 6f72 2074 6578 7420 6d6f 6465 2e20   for text mode. 
-000098d0: 5468 6520 6465 6661 756c 7420 6973 2022  The default is "
-000098e0: 7262 222e 0a0a 2020 2020 4966 2069 6e20  rb"...    If in 
-000098f0: 7265 6164 696e 6720 6d6f 6465 2028 6465  reading mode (de
-00009900: 636f 6d70 7265 7373 696f 6e29 2c20 7468  compression), th
-00009910: 6520 2a6c 6576 656c 5f6f 725f 6f70 7469  e *level_or_opti
-00009920: 6f6e 2a20 7061 7261 6d65 7465 7220 6361  on* parameter ca
-00009930: 6e20 6f6e 6c79 2062 6520 6120 6060 6469  n only be a ``di
-00009940: 6374 6060 206f 626a 6563 742c 2074 6861  ct`` object, tha
-00009950: 7420 7265 7072 6573 656e 7473 2064 6563  t represents dec
-00009960: 6f6d 7072 6573 7369 6f6e 206f 7074 696f  ompression optio
-00009970: 6e2e 2049 7420 646f 6573 6e27 7420 7375  n. It doesn't su
-00009980: 7070 6f72 7420 6060 696e 7460 6020 7479  pport ``int`` ty
-00009990: 7065 2063 6f6d 7072 6573 7369 6f6e 206c  pe compression l
-000099a0: 6576 656c 2069 6e20 7468 6973 2063 6173  evel in this cas
-000099b0: 652e 0a0a 2020 2020 496e 2062 696e 6172  e...    In binar
-000099c0: 7920 6d6f 6465 2c20 6120 3a70 793a 636c  y mode, a :py:cl
-000099d0: 6173 733a 605a 7374 6446 696c 6560 206f  ass:`ZstdFile` o
-000099e0: 626a 6563 7420 6973 2072 6574 7572 6e65  bject is returne
-000099f0: 642e 0a0a 2020 2020 496e 2074 6578 7420  d...    In text 
-00009a00: 6d6f 6465 2c20 6120 3a70 793a 636c 6173  mode, a :py:clas
-00009a10: 733a 605a 7374 6446 696c 6560 206f 626a  s:`ZstdFile` obj
-00009a20: 6563 7420 6973 2063 7265 6174 6564 2c20  ect is created, 
-00009a30: 616e 6420 7772 6170 7065 6420 696e 2061  and wrapped in a
-00009a40: 6e20 6069 6f2e 5465 7874 494f 5772 6170  n `io.TextIOWrap
-00009a50: 7065 7220 3c68 7474 7073 3a2f 2f64 6f63  per <https://doc
-00009a60: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-00009a70: 6962 7261 7279 2f69 6f2e 6874 6d6c 2369  ibrary/io.html#i
-00009a80: 6f2e 5465 7874 494f 5772 6170 7065 723e  o.TextIOWrapper>
-00009a90: 605f 206f 626a 6563 7420 7769 7468 2074  `_ object with t
-00009aa0: 6865 2073 7065 6369 6669 6564 2065 6e63  he specified enc
-00009ab0: 6f64 696e 672c 2065 7272 6f72 2068 616e  oding, error han
-00009ac0: 646c 696e 6720 6265 6861 7669 6f72 2c20  dling behavior, 
-00009ad0: 616e 6420 6c69 6e65 2065 6e64 696e 6728  and line ending(
-00009ae0: 7329 2e0a 0a41 6476 616e 6365 6420 7061  s)...Advanced pa
-00009af0: 7261 6d65 7465 7273 0a2d 2d2d 2d2d 2d2d  rameters.-------
-00009b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020  ------------..  
-00009b10: 2020 5468 6973 2073 6563 7469 6f6e 2063    This section c
-00009b20: 6f6e 7461 696e 7320 636c 6173 7320 3a70  ontains class :p
-00009b30: 793a 636c 6173 733a 6043 5061 7261 6d65  y:class:`CParame
-00009b40: 7465 7260 2c20 3a70 793a 636c 6173 733a  ter`, :py:class:
-00009b50: 6044 5061 7261 6d65 7465 7260 2c20 3a70  `DParameter`, :p
-00009b60: 793a 636c 6173 733a 6053 7472 6174 6567  y:class:`Strateg
-00009b70: 7960 2c20 7468 6579 2061 7265 2073 7562  y`, they are sub
-00009b80: 636c 6173 7365 7320 6f66 2060 6049 6e74  classes of ``Int
-00009b90: 456e 756d 6060 2c20 7573 6564 2066 6f72  Enum``, used for
-00009ba0: 2073 6574 7469 6e67 2061 6476 616e 6365   setting advance
-00009bb0: 6420 7061 7261 6d65 7465 7273 2e0a 0a20  d parameters... 
-00009bc0: 2020 203a 7079 3a63 6c61 7373 3a60 4350     :py:class:`CP
-00009bd0: 6172 616d 6574 6572 6020 636c 6173 7327  arameter` class'
-00009be0: 2061 7474 7269 6275 7465 733a 0a0a 2020   attributes:..  
-00009bf0: 2020 2020 2020 2d20 436f 6d70 7265 7373        - Compress
-00009c00: 696f 6e20 6c65 7665 6c20 283a 7079 3a61  ion level (:py:a
-00009c10: 7474 723a 607e 4350 6172 616d 6574 6572  ttr:`~CParameter
-00009c20: 2e63 6f6d 7072 6573 7369 6f6e 4c65 7665  .compressionLeve
-00009c30: 6c60 290a 2020 2020 2020 2020 2d20 436f  l`).        - Co
-00009c40: 6d70 7265 7373 2061 6c67 6f72 6974 686d  mpress algorithm
-00009c50: 2070 6172 616d 6574 6572 7320 283a 7079   parameters (:py
-00009c60: 3a61 7474 723a 607e 4350 6172 616d 6574  :attr:`~CParamet
-00009c70: 6572 2e77 696e 646f 774c 6f67 602c 203a  er.windowLog`, :
-00009c80: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
-00009c90: 6574 6572 2e68 6173 684c 6f67 602c 203a  eter.hashLog`, :
-00009ca0: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
-00009cb0: 6574 6572 2e63 6861 696e 4c6f 6760 2c20  eter.chainLog`, 
-00009cc0: 3a70 793a 6174 7472 3a60 7e43 5061 7261  :py:attr:`~CPara
-00009cd0: 6d65 7465 722e 7365 6172 6368 4c6f 6760  meter.searchLog`
-00009ce0: 2c20 3a70 793a 6174 7472 3a60 7e43 5061  , :py:attr:`~CPa
-00009cf0: 7261 6d65 7465 722e 6d69 6e4d 6174 6368  rameter.minMatch
-00009d00: 602c 203a 7079 3a61 7474 723a 607e 4350  `, :py:attr:`~CP
-00009d10: 6172 616d 6574 6572 2e74 6172 6765 744c  arameter.targetL
-00009d20: 656e 6774 6860 2c20 3a70 793a 6174 7472  ength`, :py:attr
-00009d30: 3a60 7e43 5061 7261 6d65 7465 722e 7374  :`~CParameter.st
-00009d40: 7261 7465 6779 6029 0a20 2020 2020 2020  rategy`).       
-00009d50: 202d 204c 6f6e 6720 6469 7374 616e 6365   - Long distance
-00009d60: 206d 6174 6368 696e 6720 283a 7079 3a61   matching (:py:a
-00009d70: 7474 723a 607e 4350 6172 616d 6574 6572  ttr:`~CParameter
-00009d80: 2e65 6e61 626c 654c 6f6e 6744 6973 7461  .enableLongDista
-00009d90: 6e63 654d 6174 6368 696e 6760 2c20 3a70  nceMatching`, :p
-00009da0: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
-00009db0: 7465 722e 6c64 6d48 6173 684c 6f67 602c  ter.ldmHashLog`,
-00009dc0: 203a 7079 3a61 7474 723a 607e 4350 6172   :py:attr:`~CPar
-00009dd0: 616d 6574 6572 2e6c 646d 4d69 6e4d 6174  ameter.ldmMinMat
-00009de0: 6368 602c 203a 7079 3a61 7474 723a 607e  ch`, :py:attr:`~
-00009df0: 4350 6172 616d 6574 6572 2e6c 646d 4275  CParameter.ldmBu
-00009e00: 636b 6574 5369 7a65 4c6f 6760 2c20 3a70  cketSizeLog`, :p
-00009e10: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
-00009e20: 7465 722e 6c64 6d48 6173 6852 6174 654c  ter.ldmHashRateL
-00009e30: 6f67 6029 0a20 2020 2020 2020 202d 204d  og`).        - M
-00009e40: 6973 6320 283a 7079 3a61 7474 723a 607e  isc (:py:attr:`~
-00009e50: 4350 6172 616d 6574 6572 2e63 6f6e 7465  CParameter.conte
-00009e60: 6e74 5369 7a65 466c 6167 602c 203a 7079  ntSizeFlag`, :py
-00009e70: 3a61 7474 723a 607e 4350 6172 616d 6574  :attr:`~CParamet
-00009e80: 6572 2e63 6865 636b 7375 6d46 6c61 6760  er.checksumFlag`
-00009e90: 2c20 3a70 793a 6174 7472 3a60 7e43 5061  , :py:attr:`~CPa
-00009ea0: 7261 6d65 7465 722e 6469 6374 4944 466c  rameter.dictIDFl
-00009eb0: 6167 6029 0a20 2020 2020 2020 202d 204d  ag`).        - M
-00009ec0: 756c 7469 2d74 6872 6561 6465 6420 636f  ulti-threaded co
-00009ed0: 6d70 7265 7373 696f 6e20 283a 7079 3a61  mpression (:py:a
-00009ee0: 7474 723a 607e 4350 6172 616d 6574 6572  ttr:`~CParameter
-00009ef0: 2e6e 6257 6f72 6b65 7273 602c 203a 7079  .nbWorkers`, :py
-00009f00: 3a61 7474 723a 607e 4350 6172 616d 6574  :attr:`~CParamet
-00009f10: 6572 2e6a 6f62 5369 7a65 602c 203a 7079  er.jobSize`, :py
-00009f20: 3a61 7474 723a 607e 4350 6172 616d 6574  :attr:`~CParamet
-00009f30: 6572 2e6f 7665 726c 6170 4c6f 6760 290a  er.overlapLog`).
-00009f40: 0a20 2020 203a 7079 3a63 6c61 7373 3a60  .    :py:class:`
-00009f50: 4450 6172 616d 6574 6572 6020 636c 6173  DParameter` clas
-00009f60: 7327 2061 7474 7269 6275 7465 3a0a 0a20  s' attribute:.. 
-00009f70: 2020 2020 2020 202d 2044 6563 6f6d 7072         - Decompr
-00009f80: 6573 7369 6f6e 2070 6172 616d 6574 6572  ession parameter
-00009f90: 2028 3a70 793a 6174 7472 3a60 7e44 5061   (:py:attr:`~DPa
-00009fa0: 7261 6d65 7465 722e 7769 6e64 6f77 4c6f  rameter.windowLo
-00009fb0: 674d 6178 6029 0a0a 2020 2020 3a70 793a  gMax`)..    :py:
-00009fc0: 636c 6173 733a 6053 7472 6174 6567 7960  class:`Strategy`
-00009fd0: 2063 6c61 7373 2720 6174 7472 6962 7574   class' attribut
-00009fe0: 6573 3a0a 0a20 2020 2020 2020 203a 7079  es:..        :py
-00009ff0: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
-0000a000: 2e66 6173 7460 2c20 3a70 793a 6174 7472  .fast`, :py:attr
-0000a010: 3a60 7e53 7472 6174 6567 792e 6466 6173  :`~Strategy.dfas
-0000a020: 7460 2c20 3a70 793a 6174 7472 3a60 7e53  t`, :py:attr:`~S
-0000a030: 7472 6174 6567 792e 6772 6565 6479 602c  trategy.greedy`,
-0000a040: 203a 7079 3a61 7474 723a 607e 5374 7261   :py:attr:`~Stra
-0000a050: 7465 6779 2e6c 617a 7960 2c20 3a70 793a  tegy.lazy`, :py:
-0000a060: 6174 7472 3a60 7e53 7472 6174 6567 792e  attr:`~Strategy.
-0000a070: 6c61 7a79 3260 2c20 3a70 793a 6174 7472  lazy2`, :py:attr
-0000a080: 3a60 7e53 7472 6174 6567 792e 6274 6c61  :`~Strategy.btla
-0000a090: 7a79 3260 2c20 3a70 793a 6174 7472 3a60  zy2`, :py:attr:`
-0000a0a0: 7e53 7472 6174 6567 792e 6274 6f70 7460  ~Strategy.btopt`
-0000a0b0: 2c20 3a70 793a 6174 7472 3a60 7e53 7472  , :py:attr:`~Str
-0000a0c0: 6174 6567 792e 6274 756c 7472 6160 2c20  ategy.btultra`, 
-0000a0d0: 3a70 793a 6174 7472 3a60 7e53 7472 6174  :py:attr:`~Strat
-0000a0e0: 6567 792e 6274 756c 7472 6132 602e 0a0a  egy.btultra2`...
-0000a0f0: 2e2e 205f 4350 6172 616d 6574 6572 3a0a  .. _CParameter:.
-0000a100: 0a2e 2e20 7079 3a63 6c61 7373 3a3a 2043  ... py:class:: C
-0000a110: 5061 7261 6d65 7465 7228 496e 7445 6e75  Parameter(IntEnu
-0000a120: 6d29 0a0a 2020 2020 4164 7661 6e63 6564  m)..    Advanced
-0000a130: 2063 6f6d 7072 6573 7369 6f6e 2070 6172   compression par
-0000a140: 616d 6574 6572 732e 0a0a 2020 2020 5768  ameters...    Wh
-0000a150: 656e 2075 7369 6e67 2c20 7075 7420 7468  en using, put th
-0000a160: 6520 7061 7261 6d65 7465 7273 2069 6e20  e parameters in 
-0000a170: 6120 6060 6469 6374 6060 206f 626a 6563  a ``dict`` objec
-0000a180: 742c 2074 6865 206b 6579 2069 7320 6120  t, the key is a 
-0000a190: 3a70 793a 636c 6173 733a 6043 5061 7261  :py:class:`CPara
-0000a1a0: 6d65 7465 7260 206e 616d 652c 2074 6865  meter` name, the
-0000a1b0: 2076 616c 7565 2069 7320 6120 3332 2d62   value is a 32-b
-0000a1c0: 6974 2073 6967 6e65 6420 696e 7465 6765  it signed intege
-0000a1d0: 7220 7661 6c75 652e 0a0a 2020 2020 2e2e  r value...    ..
-0000a1e0: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
-0000a1f0: 7468 6f6e 0a0a 2020 2020 2020 2020 6f70  thon..        op
-0000a200: 7469 6f6e 203d 207b 4350 6172 616d 6574  tion = {CParamet
-0000a210: 6572 2e63 6f6d 7072 6573 7369 6f6e 4c65  er.compressionLe
-0000a220: 7665 6c20 3a20 3130 2c0a 2020 2020 2020  vel : 10,.      
-0000a230: 2020 2020 2020 2020 2020 2020 4350 6172              CPar
-0000a240: 616d 6574 6572 2e63 6865 636b 7375 6d46  ameter.checksumF
-0000a250: 6c61 6720 3a20 317d 0a0a 2020 2020 2020  lag : 1}..      
-0000a260: 2020 2320 7573 6564 2077 6974 6820 636f    # used with co
-0000a270: 6d70 7265 7373 2829 2066 756e 6374 696f  mpress() functio
-0000a280: 6e0a 2020 2020 2020 2020 636f 6d70 7265  n.        compre
-0000a290: 7373 6564 5f64 6174 203d 2063 6f6d 7072  ssed_dat = compr
-0000a2a0: 6573 7328 7261 775f 6461 742c 206f 7074  ess(raw_dat, opt
-0000a2b0: 696f 6e29 0a0a 2020 2020 2020 2020 2320  ion)..        # 
-0000a2c0: 7573 6564 2077 6974 6820 5a73 7464 436f  used with ZstdCo
-0000a2d0: 6d70 7265 7373 6f72 206f 626a 6563 740a  mpressor object.
-0000a2e0: 2020 2020 2020 2020 6320 3d20 5a73 7464          c = Zstd
-0000a2f0: 436f 6d70 7265 7373 6f72 286c 6576 656c  Compressor(level
-0000a300: 5f6f 725f 6f70 7469 6f6e 3d6f 7074 696f  _or_option=optio
-0000a310: 6e29 0a20 2020 2020 2020 2063 6f6d 7072  n).        compr
-0000a320: 6573 7365 645f 6461 7431 203d 2063 2e63  essed_dat1 = c.c
-0000a330: 6f6d 7072 6573 7328 7261 775f 6461 7429  ompress(raw_dat)
-0000a340: 0a20 2020 2020 2020 2063 6f6d 7072 6573  .        compres
-0000a350: 7365 645f 6461 7432 203d 2063 2e66 6c75  sed_dat2 = c.flu
-0000a360: 7368 2829 0a0a 2020 2020 5061 7261 6d65  sh()..    Parame
-0000a370: 7465 7220 7661 6c75 6520 7368 6f75 6c64  ter value should
-0000a380: 2062 656c 6f6e 6720 746f 2061 6e20 696e   belong to an in
-0000a390: 7465 7276 616c 2077 6974 6820 6c6f 7765  terval with lowe
-0000a3a0: 7220 616e 6420 7570 7065 7220 626f 756e  r and upper boun
-0000a3b0: 6473 2c20 6f74 6865 7277 6973 6520 7468  ds, otherwise th
-0000a3c0: 6579 2077 696c 6c20 6569 7468 6572 2074  ey will either t
-0000a3d0: 7269 6767 6572 2061 6e20 6572 726f 7220  rigger an error 
-0000a3e0: 6f72 2062 6520 636c 616d 7065 6420 7369  or be clamped si
-0000a3f0: 6c65 6e74 6c79 2e0a 0a20 2020 2054 6865  lently...    The
-0000a400: 2063 6f6e 7374 616e 7420 7661 6c75 6573   constant values
-0000a410: 206d 656e 7469 6f6e 6564 2062 656c 6f77   mentioned below
-0000a420: 2061 7265 2064 6566 696e 6564 2069 6e20   are defined in 
-0000a430: 607a 7374 642e 6820 3c68 7474 7073 3a2f  `zstd.h <https:/
-0000a440: 2f67 6974 6875 622e 636f 6d2f 6661 6365  /github.com/face
-0000a450: 626f 6f6b 2f7a 7374 642f 626c 6f62 2f72  book/zstd/blob/r
-0000a460: 656c 6561 7365 2f6c 6962 2f7a 7374 642e  elease/lib/zstd.
-0000a470: 683e 605f 2c20 6e6f 7465 2074 6861 7420  h>`_, note that 
-0000a480: 7468 6573 6520 7661 6c75 6573 206d 6179  these values may
-0000a490: 2062 6520 6469 6666 6572 656e 7420 696e   be different in
-0000a4a0: 2064 6966 6665 7265 6e74 207a 7374 6420   different zstd 
-0000a4b0: 7665 7273 696f 6e73 2e0a 0a20 2020 202e  versions...    .
-0000a4c0: 2e20 7079 3a6d 6574 686f 643a 3a20 626f  . py:method:: bo
-0000a4d0: 756e 6473 2873 656c 6629 0a0a 2020 2020  unds(self)..    
-0000a4e0: 2020 2020 5265 7475 726e 206c 6f77 6572      Return lower
-0000a4f0: 2061 6e64 2075 7070 6572 2062 6f75 6e64   and upper bound
-0000a500: 7320 6f66 2061 2070 6172 616d 6574 6572  s of a parameter
-0000a510: 2c20 626f 7468 2069 6e63 6c75 7369 7665  , both inclusive
-0000a520: 2e0a 0a20 2020 2020 2020 202e 2e20 736f  ...        .. so
-0000a530: 7572 6365 636f 6465 3a3a 2070 7974 686f  urcecode:: pytho
-0000a540: 6e0a 0a20 2020 2020 2020 2020 2020 203e  n..            >
-0000a550: 3e3e 2043 5061 7261 6d65 7465 722e 636f  >> CParameter.co
-0000a560: 6d70 7265 7373 696f 6e4c 6576 656c 2e62  mpressionLevel.b
-0000a570: 6f75 6e64 7328 290a 2020 2020 2020 2020  ounds().        
-0000a580: 2020 2020 282d 3133 3130 3732 2c20 3232      (-131072, 22
-0000a590: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
-0000a5a0: 3e20 4350 6172 616d 6574 6572 2e77 696e  > CParameter.win
-0000a5b0: 646f 774c 6f67 2e62 6f75 6e64 7328 290a  dowLog.bounds().
-0000a5c0: 2020 2020 2020 2020 2020 2020 2831 302c              (10,
-0000a5d0: 2033 3129 0a20 2020 2020 2020 2020 2020   31).           
-0000a5e0: 203e 3e3e 2043 5061 7261 6d65 7465 722e   >>> CParameter.
-0000a5f0: 656e 6162 6c65 4c6f 6e67 4469 7374 616e  enableLongDistan
-0000a600: 6365 4d61 7463 6869 6e67 2e62 6f75 6e64  ceMatching.bound
-0000a610: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000a620: 2830 2c20 3129 0a0a 2020 2020 2e2e 2070  (0, 1)..    .. p
-0000a630: 793a 6174 7472 6962 7574 653a 3a20 636f  y:attribute:: co
-0000a640: 6d70 7265 7373 696f 6e4c 6576 656c 0a0a  mpressionLevel..
-0000a650: 2020 2020 2020 2020 5365 7420 636f 6d70          Set comp
-0000a660: 7265 7373 696f 6e20 7061 7261 6d65 7465  ression paramete
-0000a670: 7273 2061 6363 6f72 6469 6e67 2074 6f20  rs according to 
-0000a680: 7072 652d 6465 6669 6e65 6420 636f 6d70  pre-defined comp
-0000a690: 7265 7373 696f 6e4c 6576 656c 2074 6162  ressionLevel tab
-0000a6a0: 6c65 2c20 7365 6520 3a72 6566 3a60 636f  le, see :ref:`co
-0000a6b0: 6d70 7265 7373 696f 6e20 6c65 7665 6c3c  mpression level<
-0000a6c0: 636f 6d70 7265 7373 696f 6e5f 6c65 7665  compression_leve
-0000a6d0: 6c3e 6020 666f 7220 6465 7461 696c 732e  l>` for details.
-0000a6e0: 0a0a 2020 2020 2020 2020 5365 7474 696e  ..        Settin
-0000a6f0: 6720 6120 636f 6d70 7265 7373 696f 6e20  g a compression 
-0000a700: 6c65 7665 6c20 646f 6573 206e 6f74 2073  level does not s
-0000a710: 6574 2061 6c6c 206f 7468 6572 2063 6f6d  et all other com
-0000a720: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
-0000a730: 6572 7320 746f 2064 6566 6175 6c74 2e20  ers to default. 
-0000a740: 5365 7474 696e 6720 7468 6973 2077 696c  Setting this wil
-0000a750: 6c20 6479 6e61 6d69 6361 6c6c 7920 696d  l dynamically im
-0000a760: 7061 6374 2074 6865 2063 6f6d 7072 6573  pact the compres
-0000a770: 7369 6f6e 2070 6172 616d 6574 6572 7320  sion parameters 
-0000a780: 7768 6963 6820 6861 7665 206e 6f74 2062  which have not b
-0000a790: 6565 6e20 6d61 6e75 616c 6c79 2073 6574  een manually set
-0000a7a0: 2c20 7468 6520 6d61 6e75 616c 6c79 2073  , the manually s
-0000a7b0: 6574 206f 6e65 7320 7769 6c6c 2022 7374  et ones will "st
-0000a7c0: 6963 6b22 2e0a 0a20 2020 202e 2e20 7079  ick"...    .. py
-0000a7d0: 3a61 7474 7269 6275 7465 3a3a 2077 696e  :attribute:: win
-0000a7e0: 646f 774c 6f67 0a0a 2020 2020 2020 2020  dowLog..        
-0000a7f0: 4d61 7869 6d75 6d20 616c 6c6f 7765 6420  Maximum allowed 
-0000a800: 6261 636b 2d72 6566 6572 656e 6365 2064  back-reference d
-0000a810: 6973 7461 6e63 652c 2065 7870 7265 7373  istance, express
-0000a820: 6564 2061 7320 706f 7765 7220 6f66 2032  ed as power of 2
-0000a830: 2c20 6060 3120 3c3c 2077 696e 646f 774c  , ``1 << windowL
-0000a840: 6f67 6060 2062 7974 6573 2e0a 0a20 2020  og`` bytes...   
-0000a850: 2020 2020 204c 6172 6765 7220 7661 6c75       Larger valu
-0000a860: 6573 2072 6571 7569 7269 6e67 206d 6f72  es requiring mor
-0000a870: 6520 6d65 6d6f 7279 2061 6e64 2074 7970  e memory and typ
-0000a880: 6963 616c 6c79 2063 6f6d 7072 6573 7369  ically compressi
-0000a890: 6e67 206d 6f72 652e 0a0a 2020 2020 2020  ng more...      
-0000a8a0: 2020 5468 6973 2077 696c 6c20 7365 7420    This will set 
-0000a8b0: 6120 6d65 6d6f 7279 2062 7564 6765 7420  a memory budget 
-0000a8c0: 666f 7220 7374 7265 616d 696e 6720 6465  for streaming de
-0000a8d0: 636f 6d70 7265 7373 696f 6e2e 2055 7369  compression. Usi
-0000a8e0: 6e67 2061 2076 616c 7565 2067 7265 6174  ng a value great
-0000a8f0: 6572 2074 6861 6e20 6060 5a53 5444 5f57  er than ``ZSTD_W
-0000a900: 494e 444f 574c 4f47 5f4c 494d 4954 5f44  INDOWLOG_LIMIT_D
-0000a910: 4546 4155 4c54 6060 2072 6571 7569 7265  EFAULT`` require
-0000a920: 7320 6578 706c 6963 6974 6c79 2061 6c6c  s explicitly all
-0000a930: 6f77 696e 6720 7375 6368 2073 697a 6520  owing such size 
-0000a940: 6174 2073 7472 6561 6d69 6e67 2064 6563  at streaming dec
-0000a950: 6f6d 7072 6573 7369 6f6e 2073 7461 6765  ompression stage
-0000a960: 2c20 7365 6520 3a70 793a 6174 7472 3a60  , see :py:attr:`
-0000a970: 4450 6172 616d 6574 6572 2e77 696e 646f  DParameter.windo
-0000a980: 774c 6f67 4d61 7860 2e20 6060 5a53 5444  wLogMax`. ``ZSTD
-0000a990: 5f57 494e 444f 574c 4f47 5f4c 494d 4954  _WINDOWLOG_LIMIT
-0000a9a0: 5f44 4546 4155 4c54 6060 2069 7320 3237  _DEFAULT`` is 27
-0000a9b0: 2069 6e20 7a73 7464 2076 312e 322b 2c20   in zstd v1.2+, 
-0000a9c0: 6d65 616e 7320 3132 3820 4d69 4220 2831  means 128 MiB (1
-0000a9d0: 203c 3c20 3237 292e 0a0a 2020 2020 2020   << 27)...      
-0000a9e0: 2020 4d75 7374 2062 6520 636c 616d 7065    Must be clampe
-0000a9f0: 6420 6265 7477 6565 6e20 6060 5a53 5444  d between ``ZSTD
-0000aa00: 5f57 494e 444f 574c 4f47 5f4d 494e 6060  _WINDOWLOG_MIN``
-0000aa10: 2061 6e64 2060 605a 5354 445f 5749 4e44   and ``ZSTD_WIND
-0000aa20: 4f57 4c4f 475f 4d41 5860 602e 0a0a 2020  OWLOG_MAX``...  
-0000aa30: 2020 2020 2020 5370 6563 6961 6c3a 2076        Special: v
-0000aa40: 616c 7565 2060 6030 6060 206d 6561 6e73  alue ``0`` means
-0000aa50: 2022 7573 6520 6465 6661 756c 7420 7769   "use default wi
-0000aa60: 6e64 6f77 4c6f 6722 2c20 7468 656e 2074  ndowLog", then t
-0000aa70: 6865 2076 616c 7565 2069 7320 6479 6e61  he value is dyna
-0000aa80: 6d69 6361 6c6c 7920 7365 742c 2073 6565  mically set, see
-0000aa90: 2022 5722 2063 6f6c 756d 6e20 696e 2060   "W" column in `
-0000aaa0: 7468 6973 2074 6162 6c65 203c 6874 7470  this table <http
-0000aab0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-0000aac0: 6163 6562 6f6f 6b2f 7a73 7464 2f62 6c6f  acebook/zstd/blo
-0000aad0: 622f 7265 6c65 6173 652f 6c69 622f 636f  b/release/lib/co
-0000aae0: 6d70 7265 7373 2f63 6c65 7665 6c73 2e68  mpress/clevels.h
-0000aaf0: 3e60 5f2e 0a0a 2020 2020 2e2e 2070 793a  >`_...    .. py:
-0000ab00: 6174 7472 6962 7574 653a 3a20 6861 7368  attribute:: hash
-0000ab10: 4c6f 670a 0a20 2020 2020 2020 2053 697a  Log..        Siz
-0000ab20: 6520 6f66 2074 6865 2069 6e69 7469 616c  e of the initial
-0000ab30: 2070 726f 6265 2074 6162 6c65 2c20 6173   probe table, as
-0000ab40: 2061 2070 6f77 6572 206f 6620 322c 2072   a power of 2, r
-0000ab50: 6573 756c 7469 6e67 206d 656d 6f72 7920  esulting memory 
-0000ab60: 7573 6167 6520 6973 2060 6031 203c 3c20  usage is ``1 << 
-0000ab70: 2868 6173 684c 6f67 2b32 2960 6020 6279  (hashLog+2)`` by
-0000ab80: 7465 732e 0a0a 2020 2020 2020 2020 4d75  tes...        Mu
-0000ab90: 7374 2062 6520 636c 616d 7065 6420 6265  st be clamped be
-0000aba0: 7477 6565 6e20 6060 5a53 5444 5f48 4153  tween ``ZSTD_HAS
-0000abb0: 484c 4f47 5f4d 494e 6060 2061 6e64 2060  HLOG_MIN`` and `
-0000abc0: 605a 5354 445f 4841 5348 4c4f 475f 4d41  `ZSTD_HASHLOG_MA
-0000abd0: 5860 602e 0a0a 2020 2020 2020 2020 4c61  X``...        La
-0000abe0: 7267 6572 2074 6162 6c65 7320 696d 7072  rger tables impr
-0000abf0: 6f76 6520 636f 6d70 7265 7373 696f 6e20  ove compression 
-0000ac00: 7261 7469 6f20 6f66 2073 7472 6174 6567  ratio of strateg
-0000ac10: 6965 7320 3c3d 203a 7079 3a61 7474 723a  ies <= :py:attr:
-0000ac20: 607e 5374 7261 7465 6779 2e64 6661 7374  `~Strategy.dfast
-0000ac30: 602c 2061 6e64 2069 6d70 726f 7665 2073  `, and improve s
-0000ac40: 7065 6564 206f 6620 7374 7261 7465 6769  peed of strategi
-0000ac50: 6573 203e 203a 7079 3a61 7474 723a 607e  es > :py:attr:`~
-0000ac60: 5374 7261 7465 6779 2e64 6661 7374 602e  Strategy.dfast`.
-0000ac70: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
-0000ac80: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
-0000ac90: 6561 6e73 2022 7573 6520 6465 6661 756c  eans "use defaul
-0000aca0: 7420 6861 7368 4c6f 6722 2c20 7468 656e  t hashLog", then
-0000acb0: 2074 6865 2076 616c 7565 2069 7320 6479   the value is dy
-0000acc0: 6e61 6d69 6361 6c6c 7920 7365 742c 2073  namically set, s
-0000acd0: 6565 2022 4822 2063 6f6c 756d 6e20 696e  ee "H" column in
-0000ace0: 2060 7468 6973 2074 6162 6c65 203c 6874   `this table <ht
-0000acf0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000ad00: 2f66 6163 6562 6f6f 6b2f 7a73 7464 2f62  /facebook/zstd/b
-0000ad10: 6c6f 622f 7265 6c65 6173 652f 6c69 622f  lob/release/lib/
-0000ad20: 636f 6d70 7265 7373 2f63 6c65 7665 6c73  compress/clevels
-0000ad30: 2e68 3e60 5f2e 0a0a 2020 2020 2e2e 2070  .h>`_...    .. p
-0000ad40: 793a 6174 7472 6962 7574 653a 3a20 6368  y:attribute:: ch
-0000ad50: 6169 6e4c 6f67 0a0a 2020 2020 2020 2020  ainLog..        
-0000ad60: 5369 7a65 206f 6620 7468 6520 6d75 6c74  Size of the mult
-0000ad70: 692d 7072 6f62 6520 7365 6172 6368 2074  i-probe search t
-0000ad80: 6162 6c65 2c20 6173 2061 2070 6f77 6572  able, as a power
-0000ad90: 206f 6620 322c 2072 6573 756c 7469 6e67   of 2, resulting
-0000ada0: 206d 656d 6f72 7920 7573 6167 6520 6973   memory usage is
-0000adb0: 2060 6031 203c 3c20 2863 6861 696e 4c6f   ``1 << (chainLo
-0000adc0: 672b 3229 6060 2062 7974 6573 2e0a 0a20  g+2)`` bytes... 
-0000add0: 2020 2020 2020 204d 7573 7420 6265 2063         Must be c
-0000ade0: 6c61 6d70 6564 2062 6574 7765 656e 2060  lamped between `
-0000adf0: 605a 5354 445f 4348 4149 4e4c 4f47 5f4d  `ZSTD_CHAINLOG_M
-0000ae00: 494e 6060 2061 6e64 2060 605a 5354 445f  IN`` and ``ZSTD_
-0000ae10: 4348 4149 4e4c 4f47 5f4d 4158 6060 2e0a  CHAINLOG_MAX``..
-0000ae20: 0a20 2020 2020 2020 204c 6172 6765 7220  .        Larger 
-0000ae30: 7461 626c 6573 2072 6573 756c 7420 696e  tables result in
-0000ae40: 2062 6574 7465 7220 616e 6420 736c 6f77   better and slow
-0000ae50: 6572 2063 6f6d 7072 6573 7369 6f6e 2e0a  er compression..
-0000ae60: 0a20 2020 2020 2020 2054 6869 7320 7061  .        This pa
-0000ae70: 7261 6d65 7465 7220 6973 2075 7365 6c65  rameter is usele
-0000ae80: 7373 2066 6f72 203a 7079 3a61 7474 723a  ss for :py:attr:
-0000ae90: 607e 5374 7261 7465 6779 2e66 6173 7460  `~Strategy.fast`
-0000aea0: 2073 7472 6174 6567 792e 0a0a 2020 2020   strategy...    
-0000aeb0: 2020 2020 4974 2773 2073 7469 6c6c 2075      It's still u
-0000aec0: 7365 6675 6c20 7768 656e 2075 7369 6e67  seful when using
-0000aed0: 203a 7079 3a61 7474 723a 607e 5374 7261   :py:attr:`~Stra
-0000aee0: 7465 6779 2e64 6661 7374 6020 7374 7261  tegy.dfast` stra
-0000aef0: 7465 6779 2c20 696e 2077 6869 6368 2063  tegy, in which c
-0000af00: 6173 6520 6974 2064 6566 696e 6573 2061  ase it defines a
-0000af10: 2073 6563 6f6e 6461 7279 2070 726f 6265   secondary probe
-0000af20: 2074 6162 6c65 2e0a 0a20 2020 2020 2020   table...       
-0000af30: 2053 7065 6369 616c 3a20 7661 6c75 6520   Special: value 
-0000af40: 6060 3060 6020 6d65 616e 7320 2275 7365  ``0`` means "use
-0000af50: 2064 6566 6175 6c74 2063 6861 696e 4c6f   default chainLo
-0000af60: 6722 2c20 7468 656e 2074 6865 2076 616c  g", then the val
-0000af70: 7565 2069 7320 6479 6e61 6d69 6361 6c6c  ue is dynamicall
-0000af80: 7920 7365 742c 2073 6565 2022 4322 2063  y set, see "C" c
-0000af90: 6f6c 756d 6e20 696e 2060 7468 6973 2074  olumn in `this t
-0000afa0: 6162 6c65 203c 6874 7470 733a 2f2f 6769  able <https://gi
-0000afb0: 7468 7562 2e63 6f6d 2f66 6163 6562 6f6f  thub.com/faceboo
-0000afc0: 6b2f 7a73 7464 2f62 6c6f 622f 7265 6c65  k/zstd/blob/rele
-0000afd0: 6173 652f 6c69 622f 636f 6d70 7265 7373  ase/lib/compress
-0000afe0: 2f63 6c65 7665 6c73 2e68 3e60 5f2e 0a0a  /clevels.h>`_...
-0000aff0: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
-0000b000: 7574 653a 3a20 7365 6172 6368 4c6f 670a  ute:: searchLog.
-0000b010: 0a20 2020 2020 2020 204e 756d 6265 7220  .        Number 
-0000b020: 6f66 2073 6561 7263 6820 6174 7465 6d70  of search attemp
-0000b030: 7473 2c20 6173 2061 2070 6f77 6572 206f  ts, as a power o
-0000b040: 6620 322e 0a0a 2020 2020 2020 2020 4d6f  f 2...        Mo
-0000b050: 7265 2061 7474 656d 7074 7320 7265 7375  re attempts resu
-0000b060: 6c74 2069 6e20 6265 7474 6572 2061 6e64  lt in better and
-0000b070: 2073 6c6f 7765 7220 636f 6d70 7265 7373   slower compress
-0000b080: 696f 6e2e 0a0a 2020 2020 2020 2020 5468  ion...        Th
-0000b090: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
-0000b0a0: 7573 656c 6573 7320 666f 7220 3a70 793a  useless for :py:
-0000b0b0: 6174 7472 3a60 7e53 7472 6174 6567 792e  attr:`~Strategy.
-0000b0c0: 6661 7374 6020 616e 6420 3a70 793a 6174  fast` and :py:at
-0000b0d0: 7472 3a60 7e53 7472 6174 6567 792e 6466  tr:`~Strategy.df
-0000b0e0: 6173 7460 2073 7472 6174 6567 6965 732e  ast` strategies.
-0000b0f0: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
-0000b100: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
-0000b110: 6561 6e73 2022 7573 6520 6465 6661 756c  eans "use defaul
-0000b120: 7420 7365 6172 6368 4c6f 6722 2c20 7468  t searchLog", th
-0000b130: 656e 2074 6865 2076 616c 7565 2069 7320  en the value is 
-0000b140: 6479 6e61 6d69 6361 6c6c 7920 7365 742c  dynamically set,
-0000b150: 2073 6565 2022 5322 2063 6f6c 756d 6e20   see "S" column 
-0000b160: 696e 2060 7468 6973 2074 6162 6c65 203c  in `this table <
-0000b170: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000b180: 6f6d 2f66 6163 6562 6f6f 6b2f 7a73 7464  om/facebook/zstd
-0000b190: 2f62 6c6f 622f 7265 6c65 6173 652f 6c69  /blob/release/li
-0000b1a0: 622f 636f 6d70 7265 7373 2f63 6c65 7665  b/compress/cleve
-0000b1b0: 6c73 2e68 3e60 5f2e 0a0a 2020 2020 2e2e  ls.h>`_...    ..
-0000b1c0: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
-0000b1d0: 6d69 6e4d 6174 6368 0a0a 2020 2020 2020  minMatch..      
-0000b1e0: 2020 4d69 6e69 6d75 6d20 7369 7a65 206f    Minimum size o
-0000b1f0: 6620 7365 6172 6368 6564 206d 6174 6368  f searched match
-0000b200: 6573 2e0a 0a20 2020 2020 2020 204e 6f74  es...        Not
-0000b210: 6520 7468 6174 205a 7374 616e 6461 7264  e that Zstandard
-0000b220: 2063 616e 2073 7469 6c6c 2066 696e 6420   can still find 
-0000b230: 6d61 7463 6865 7320 6f66 2073 6d61 6c6c  matches of small
-0000b240: 6572 2073 697a 652c 2069 7420 6a75 7374  er size, it just
-0000b250: 2074 7765 616b 7320 6974 7320 7365 6172   tweaks its sear
-0000b260: 6368 2061 6c67 6f72 6974 686d 2074 6f20  ch algorithm to 
-0000b270: 6c6f 6f6b 2066 6f72 2074 6869 7320 7369  look for this si
-0000b280: 7a65 2061 6e64 206c 6172 6765 722e 0a0a  ze and larger...
-0000b290: 2020 2020 2020 2020 4c61 7267 6572 2076          Larger v
-0000b2a0: 616c 7565 7320 696e 6372 6561 7365 2063  alues increase c
-0000b2b0: 6f6d 7072 6573 7369 6f6e 2061 6e64 2064  ompression and d
-0000b2c0: 6563 6f6d 7072 6573 7369 6f6e 2073 7065  ecompression spe
-0000b2d0: 6564 2c20 6275 7420 6465 6372 6561 7365  ed, but decrease
-0000b2e0: 2072 6174 696f 2e0a 0a20 2020 2020 2020   ratio...       
-0000b2f0: 204d 7573 7420 6265 2063 6c61 6d70 6564   Must be clamped
-0000b300: 2062 6574 7765 656e 2060 605a 5354 445f   between ``ZSTD_
-0000b310: 4d49 4e4d 4154 4348 5f4d 494e 6060 2061  MINMATCH_MIN`` a
-0000b320: 6e64 2060 605a 5354 445f 4d49 4e4d 4154  nd ``ZSTD_MINMAT
-0000b330: 4348 5f4d 4158 6060 2e0a 0a20 2020 2020  CH_MAX``...     
-0000b340: 2020 204e 6f74 6520 7468 6174 2063 7572     Note that cur
-0000b350: 7265 6e74 6c79 2c20 666f 7220 616c 6c20  rently, for all 
-0000b360: 7374 7261 7465 6769 6573 203c 203a 7079  strategies < :py
-0000b370: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
-0000b380: 2e62 746f 7074 602c 2065 6666 6563 7469  .btopt`, effecti
-0000b390: 7665 206d 696e 696d 756d 2069 7320 6060  ve minimum is ``
-0000b3a0: 3460 602c 2066 6f72 2061 6c6c 2073 7472  4``, for all str
-0000b3b0: 6174 6567 6965 7320 3e20 3a70 793a 6174  ategies > :py:at
-0000b3c0: 7472 3a60 7e53 7472 6174 6567 792e 6661  tr:`~Strategy.fa
-0000b3d0: 7374 602c 2065 6666 6563 7469 7665 206d  st`, effective m
-0000b3e0: 6178 696d 756d 2069 7320 6060 3660 602e  aximum is ``6``.
-0000b3f0: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
-0000b400: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
-0000b410: 6561 6e73 2022 7573 6520 6465 6661 756c  eans "use defaul
-0000b420: 7420 6d69 6e4d 6174 6368 4c65 6e67 7468  t minMatchLength
-0000b430: 222c 2074 6865 6e20 7468 6520 7661 6c75  ", then the valu
-0000b440: 6520 6973 2064 796e 616d 6963 616c 6c79  e is dynamically
-0000b450: 2073 6574 2c20 7365 6520 224c 2220 636f   set, see "L" co
-0000b460: 6c75 6d6e 2069 6e20 6074 6869 7320 7461  lumn in `this ta
-0000b470: 626c 6520 3c68 7474 7073 3a2f 2f67 6974  ble <https://git
-0000b480: 6875 622e 636f 6d2f 6661 6365 626f 6f6b  hub.com/facebook
-0000b490: 2f7a 7374 642f 626c 6f62 2f72 656c 6561  /zstd/blob/relea
-0000b4a0: 7365 2f6c 6962 2f63 6f6d 7072 6573 732f  se/lib/compress/
-0000b4b0: 636c 6576 656c 732e 683e 605f 2e0a 0a20  clevels.h>`_... 
-0000b4c0: 2020 202e 2e20 7079 3a61 7474 7269 6275     .. py:attribu
-0000b4d0: 7465 3a3a 2074 6172 6765 744c 656e 6774  te:: targetLengt
-0000b4e0: 680a 0a20 2020 2020 2020 2049 6d70 6163  h..        Impac
-0000b4f0: 7420 6f66 2074 6869 7320 6669 656c 6420  t of this field 
-0000b500: 6465 7065 6e64 7320 6f6e 2073 7472 6174  depends on strat
-0000b510: 6567 792e 0a0a 2020 2020 2020 2020 466f  egy...        Fo
-0000b520: 7220 7374 7261 7465 6769 6573 203a 7079  r strategies :py
-0000b530: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
-0000b540: 2e62 746f 7074 602c 203a 7079 3a61 7474  .btopt`, :py:att
-0000b550: 723a 607e 5374 7261 7465 6779 2e62 7475  r:`~Strategy.btu
-0000b560: 6c74 7261 6020 2620 3a70 793a 6174 7472  ltra` & :py:attr
-0000b570: 3a60 7e53 7472 6174 6567 792e 6274 756c  :`~Strategy.btul
-0000b580: 7472 6132 603a 0a0a 2020 2020 2020 2020  tra2`:..        
-0000b590: 2020 2020 4c65 6e67 7468 206f 6620 4d61      Length of Ma
-0000b5a0: 7463 6820 636f 6e73 6964 6572 6564 2022  tch considered "
-0000b5b0: 676f 6f64 2065 6e6f 7567 6822 2074 6f20  good enough" to 
-0000b5c0: 7374 6f70 2073 6561 7263 682e 0a0a 2020  stop search...  
-0000b5d0: 2020 2020 2020 2020 2020 4c61 7267 6572            Larger
-0000b5e0: 2076 616c 7565 7320 6d61 6b65 2063 6f6d   values make com
-0000b5f0: 7072 6573 7369 6f6e 2073 7472 6f6e 6765  pression stronge
-0000b600: 722c 2061 6e64 2073 6c6f 7765 722e 0a0a  r, and slower...
-0000b610: 2020 2020 2020 2020 466f 7220 7374 7261          For stra
-0000b620: 7465 6779 203a 7079 3a61 7474 723a 607e  tegy :py:attr:`~
-0000b630: 5374 7261 7465 6779 2e66 6173 7460 3a0a  Strategy.fast`:.
-0000b640: 0a20 2020 2020 2020 2020 2020 2044 6973  .            Dis
-0000b650: 7461 6e63 6520 6265 7477 6565 6e20 6d61  tance between ma
-0000b660: 7463 6820 7361 6d70 6c69 6e67 2e0a 0a20  tch sampling... 
-0000b670: 2020 2020 2020 2020 2020 204c 6172 6765             Large
-0000b680: 7220 7661 6c75 6573 206d 616b 6520 636f  r values make co
-0000b690: 6d70 7265 7373 696f 6e20 6661 7374 6572  mpression faster
-0000b6a0: 2c20 616e 6420 7765 616b 6572 2e0a 0a20  , and weaker... 
-0000b6b0: 2020 2020 2020 2053 7065 6369 616c 3a20         Special: 
-0000b6c0: 7661 6c75 6520 6060 3060 6020 6d65 616e  value ``0`` mean
-0000b6d0: 7320 2275 7365 2064 6566 6175 6c74 2074  s "use default t
-0000b6e0: 6172 6765 744c 656e 6774 6822 2c20 7468  argetLength", th
-0000b6f0: 656e 2074 6865 2076 616c 7565 2069 7320  en the value is 
-0000b700: 6479 6e61 6d69 6361 6c6c 7920 7365 742c  dynamically set,
-0000b710: 2073 6565 2022 544c 2220 636f 6c75 6d6e   see "TL" column
-0000b720: 2069 6e20 6074 6869 7320 7461 626c 6520   in `this table 
-0000b730: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-0000b740: 636f 6d2f 6661 6365 626f 6f6b 2f7a 7374  com/facebook/zst
-0000b750: 642f 626c 6f62 2f72 656c 6561 7365 2f6c  d/blob/release/l
-0000b760: 6962 2f63 6f6d 7072 6573 732f 636c 6576  ib/compress/clev
-0000b770: 656c 732e 683e 605f 2e0a 0a20 2020 202e  els.h>`_...    .
-0000b780: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
-0000b790: 2073 7472 6174 6567 790a 0a20 2020 2020   strategy..     
-0000b7a0: 2020 2053 6565 203a 7079 3a61 7474 723a     See :py:attr:
-0000b7b0: 6053 7472 6174 6567 7960 2063 6c61 7373  `Strategy` class
-0000b7c0: 2064 6566 696e 6974 696f 6e2e 0a0a 2020   definition...  
-0000b7d0: 2020 2020 2020 5468 6520 6869 6768 6572        The higher
-0000b7e0: 2074 6865 2076 616c 7565 206f 6620 7365   the value of se
-0000b7f0: 6c65 6374 6564 2073 7472 6174 6567 792c  lected strategy,
-0000b800: 2074 6865 206d 6f72 6520 636f 6d70 6c65   the more comple
-0000b810: 7820 6974 2069 732c 2072 6573 756c 7469  x it is, resulti
-0000b820: 6e67 2069 6e20 7374 726f 6e67 6572 2061  ng in stronger a
-0000b830: 6e64 2073 6c6f 7765 7220 636f 6d70 7265  nd slower compre
-0000b840: 7373 696f 6e2e 0a0a 2020 2020 2020 2020  ssion...        
-0000b850: 5370 6563 6961 6c3a 2076 616c 7565 2060  Special: value `
-0000b860: 6030 6060 206d 6561 6e73 2022 7573 6520  `0`` means "use 
-0000b870: 6465 6661 756c 7420 7374 7261 7465 6779  default strategy
-0000b880: 222c 2074 6865 6e20 7468 6520 7661 6c75  ", then the valu
-0000b890: 6520 6973 2064 796e 616d 6963 616c 6c79  e is dynamically
-0000b8a0: 2073 6574 2c20 7365 6520 2273 7472 6174   set, see "strat
-0000b8b0: 2220 636f 6c75 6d6e 2069 6e20 6074 6869  " column in `thi
-0000b8c0: 7320 7461 626c 6520 3c68 7474 7073 3a2f  s table <https:/
-0000b8d0: 2f67 6974 6875 622e 636f 6d2f 6661 6365  /github.com/face
-0000b8e0: 626f 6f6b 2f7a 7374 642f 626c 6f62 2f72  book/zstd/blob/r
-0000b8f0: 656c 6561 7365 2f6c 6962 2f63 6f6d 7072  elease/lib/compr
-0000b900: 6573 732f 636c 6576 656c 732e 683e 605f  ess/clevels.h>`_
-0000b910: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
-0000b920: 7269 6275 7465 3a3a 2065 6e61 626c 654c  ribute:: enableL
-0000b930: 6f6e 6744 6973 7461 6e63 654d 6174 6368  ongDistanceMatch
-0000b940: 696e 670a 0a20 2020 2020 2020 2045 6e61  ing..        Ena
-0000b950: 626c 6520 6c6f 6e67 2064 6973 7461 6e63  ble long distanc
-0000b960: 6520 6d61 7463 6869 6e67 2e0a 0a20 2020  e matching...   
-0000b970: 2020 2020 2044 6566 6175 6c74 2076 616c       Default val
-0000b980: 7565 2069 7320 6060 3060 602c 2063 616e  ue is ``0``, can
-0000b990: 2062 6520 6060 3160 602e 0a0a 2020 2020   be ``1``...    
-0000b9a0: 2020 2020 5468 6973 2070 6172 616d 6574      This paramet
-0000b9b0: 6572 2069 7320 6465 7369 676e 6564 2074  er is designed t
-0000b9c0: 6f20 696d 7072 6f76 6520 636f 6d70 7265  o improve compre
-0000b9d0: 7373 696f 6e20 7261 7469 6f2c 2066 6f72  ssion ratio, for
-0000b9e0: 206c 6172 6765 2069 6e70 7574 732c 2062   large inputs, b
-0000b9f0: 7920 6669 6e64 696e 6720 6c61 7267 6520  y finding large 
-0000ba00: 6d61 7463 6865 7320 6174 206c 6f6e 6720  matches at long 
-0000ba10: 6469 7374 616e 6365 2e20 4974 2069 6e63  distance. It inc
-0000ba20: 7265 6173 6573 206d 656d 6f72 7920 7573  reases memory us
-0000ba30: 6167 6520 616e 6420 7769 6e64 6f77 2073  age and window s
-0000ba40: 697a 652e 0a0a 2020 2020 2020 2020 4e6f  ize...        No
-0000ba50: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
-0000ba60: 2a20 456e 6162 6c69 6e67 2074 6869 7320  * Enabling this 
-0000ba70: 7061 7261 6d65 7465 7220 696e 6372 6561  parameter increa
-0000ba80: 7365 7320 6465 6661 756c 7420 3a70 793a  ses default :py:
-0000ba90: 6174 7472 3a60 7e43 5061 7261 6d65 7465  attr:`~CParamete
-0000baa0: 722e 7769 6e64 6f77 4c6f 6760 2074 6f20  r.windowLog` to 
-0000bab0: 3132 3820 4d69 4220 6578 6365 7074 2077  128 MiB except w
-0000bac0: 6865 6e20 6578 7072 6573 736c 7920 7365  hen expressly se
-0000bad0: 7420 746f 2061 2064 6966 6665 7265 6e74  t to a different
-0000bae0: 2076 616c 7565 2e0a 2020 2020 2020 2020   value..        
-0000baf0: 2020 2020 2a20 5468 6973 2077 696c 6c20      * This will 
-0000bb00: 6265 2065 6e61 626c 6564 2062 7920 6465  be enabled by de
-0000bb10: 6661 756c 7420 6966 203a 7079 3a61 7474  fault if :py:att
-0000bb20: 723a 607e 4350 6172 616d 6574 6572 2e77  r:`~CParameter.w
-0000bb30: 696e 646f 774c 6f67 6020 3e3d 2031 3238  indowLog` >= 128
-0000bb40: 204d 6942 2061 6e64 2063 6f6d 7072 6573   MiB and compres
-0000bb50: 7369 6f6e 2073 7472 6174 6567 7920 3e3d  sion strategy >=
-0000bb60: 203a 7079 3a61 7474 723a 607e 5374 7261   :py:attr:`~Stra
-0000bb70: 7465 6779 2e62 746f 7074 6020 2863 6f6d  tegy.btopt` (com
-0000bb80: 7072 6573 7369 6f6e 206c 6576 656c 2031  pression level 1
-0000bb90: 362b 292e 0a0a 2020 2020 2e2e 2070 793a  6+)...    .. py:
-0000bba0: 6174 7472 6962 7574 653a 3a20 6c64 6d48  attribute:: ldmH
-0000bbb0: 6173 684c 6f67 0a0a 2020 2020 2020 2020  ashLog..        
-0000bbc0: 5369 7a65 206f 6620 7468 6520 7461 626c  Size of the tabl
-0000bbd0: 6520 666f 7220 6c6f 6e67 2064 6973 7461  e for long dista
-0000bbe0: 6e63 6520 6d61 7463 6869 6e67 2c20 6173  nce matching, as
-0000bbf0: 2061 2070 6f77 6572 206f 6620 322e 0a0a   a power of 2...
-0000bc00: 2020 2020 2020 2020 4c61 7267 6572 2076          Larger v
-0000bc10: 616c 7565 7320 696e 6372 6561 7365 206d  alues increase m
-0000bc20: 656d 6f72 7920 7573 6167 6520 616e 6420  emory usage and 
-0000bc30: 636f 6d70 7265 7373 696f 6e20 7261 7469  compression rati
-0000bc40: 6f2c 2062 7574 2064 6563 7265 6173 6520  o, but decrease 
-0000bc50: 636f 6d70 7265 7373 696f 6e20 7370 6565  compression spee
-0000bc60: 642e 0a0a 2020 2020 2020 2020 4d75 7374  d...        Must
-0000bc70: 2062 6520 636c 616d 7065 6420 6265 7477   be clamped betw
-0000bc80: 6565 6e20 6060 5a53 5444 5f48 4153 484c  een ``ZSTD_HASHL
-0000bc90: 4f47 5f4d 494e 6060 2061 6e64 2060 605a  OG_MIN`` and ``Z
-0000bca0: 5354 445f 4841 5348 4c4f 475f 4d41 5860  STD_HASHLOG_MAX`
-0000bcb0: 602c 2064 6566 6175 6c74 3a20 3a70 793a  `, default: :py:
-0000bcc0: 6174 7472 3a60 7e43 5061 7261 6d65 7465  attr:`~CParamete
-0000bcd0: 722e 7769 6e64 6f77 4c6f 6760 202d 2037  r.windowLog` - 7
-0000bce0: 2e0a 0a20 2020 2020 2020 2053 7065 6369  ...        Speci
-0000bcf0: 616c 3a20 7661 6c75 6520 6060 3060 6020  al: value ``0`` 
-0000bd00: 6d65 616e 7320 2261 7574 6f6d 6174 6963  means "automatic
-0000bd10: 616c 6c79 2064 6574 6572 6d69 6e65 2068  ally determine h
-0000bd20: 6173 686c 6f67 222e 0a0a 2020 2020 2e2e  ashlog"...    ..
-0000bd30: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
-0000bd40: 6c64 6d4d 696e 4d61 7463 680a 0a20 2020  ldmMinMatch..   
-0000bd50: 2020 2020 204d 696e 696d 756d 206d 6174       Minimum mat
-0000bd60: 6368 2073 697a 6520 666f 7220 6c6f 6e67  ch size for long
-0000bd70: 2064 6973 7461 6e63 6520 6d61 7463 6865   distance matche
-0000bd80: 722e 0a0a 2020 2020 2020 2020 4c61 7267  r...        Larg
-0000bd90: 6572 2f74 6f6f 2073 6d61 6c6c 2076 616c  er/too small val
-0000bda0: 7565 7320 7573 7561 6c6c 7920 6465 6372  ues usually decr
-0000bdb0: 6561 7365 2063 6f6d 7072 6573 7369 6f6e  ease compression
-0000bdc0: 2072 6174 696f 2e0a 0a20 2020 2020 2020   ratio...       
-0000bdd0: 204d 7573 7420 6265 2063 6c61 6d70 6564   Must be clamped
-0000bde0: 2062 6574 7765 656e 2060 605a 5354 445f   between ``ZSTD_
-0000bdf0: 4c44 4d5f 4d49 4e4d 4154 4348 5f4d 494e  LDM_MINMATCH_MIN
-0000be00: 6060 2061 6e64 2060 605a 5354 445f 4c44  `` and ``ZSTD_LD
-0000be10: 4d5f 4d49 4e4d 4154 4348 5f4d 4158 6060  M_MINMATCH_MAX``
-0000be20: 2e0a 0a20 2020 2020 2020 2053 7065 6369  ...        Speci
-0000be30: 616c 3a20 7661 6c75 6520 6060 3060 6020  al: value ``0`` 
-0000be40: 6d65 616e 7320 2275 7365 2064 6566 6175  means "use defau
-0000be50: 6c74 2076 616c 7565 2220 2864 6566 6175  lt value" (defau
-0000be60: 6c74 3a20 3634 292e 0a0a 2020 2020 2e2e  lt: 64)...    ..
-0000be70: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
-0000be80: 6c64 6d42 7563 6b65 7453 697a 654c 6f67  ldmBucketSizeLog
-0000be90: 0a0a 2020 2020 2020 2020 4c6f 6720 7369  ..        Log si
-0000bea0: 7a65 206f 6620 6561 6368 2062 7563 6b65  ze of each bucke
-0000beb0: 7420 696e 2074 6865 204c 444d 2068 6173  t in the LDM has
-0000bec0: 6820 7461 626c 6520 666f 7220 636f 6c6c  h table for coll
-0000bed0: 6973 696f 6e20 7265 736f 6c75 7469 6f6e  ision resolution
-0000bee0: 2e0a 0a20 2020 2020 2020 204c 6172 6765  ...        Large
-0000bef0: 7220 7661 6c75 6573 2069 6d70 726f 7665  r values improve
-0000bf00: 2063 6f6c 6c69 7369 6f6e 2072 6573 6f6c   collision resol
-0000bf10: 7574 696f 6e20 6275 7420 6465 6372 6561  ution but decrea
-0000bf20: 7365 2063 6f6d 7072 6573 7369 6f6e 2073  se compression s
-0000bf30: 7065 6564 2e0a 0a20 2020 2020 2020 2054  peed...        T
-0000bf40: 6865 206d 6178 696d 756d 2076 616c 7565  he maximum value
-0000bf50: 2069 7320 6060 5a53 5444 5f4c 444d 5f42   is ``ZSTD_LDM_B
-0000bf60: 5543 4b45 5453 495a 454c 4f47 5f4d 4158  UCKETSIZELOG_MAX
-0000bf70: 6060 2e0a 0a20 2020 2020 2020 2053 7065  ``...        Spe
-0000bf80: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
-0000bf90: 6020 6d65 616e 7320 2275 7365 2064 6566  ` means "use def
-0000bfa0: 6175 6c74 2076 616c 7565 2220 2864 6566  ault value" (def
-0000bfb0: 6175 6c74 3a20 3329 2e0a 0a20 2020 202e  ault: 3)...    .
-0000bfc0: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
-0000bfd0: 206c 646d 4861 7368 5261 7465 4c6f 670a   ldmHashRateLog.
-0000bfe0: 0a20 2020 2020 2020 2046 7265 7175 656e  .        Frequen
-0000bff0: 6379 206f 6620 696e 7365 7274 696e 672f  cy of inserting/
-0000c000: 6c6f 6f6b 696e 6720 7570 2065 6e74 7269  looking up entri
-0000c010: 6573 2069 6e74 6f20 7468 6520 4c44 4d20  es into the LDM 
-0000c020: 6861 7368 2074 6162 6c65 2e0a 0a20 2020  hash table...   
-0000c030: 2020 2020 204d 7573 7420 6265 2063 6c61       Must be cla
-0000c040: 6d70 6564 2062 6574 7765 656e 2030 2061  mped between 0 a
-0000c050: 6e64 2060 6028 5a53 5444 5f57 494e 444f  nd ``(ZSTD_WINDO
-0000c060: 574c 4f47 5f4d 4158 202d 205a 5354 445f  WLOG_MAX - ZSTD_
-0000c070: 4841 5348 4c4f 475f 4d49 4e29 6060 2e0a  HASHLOG_MIN)``..
-0000c080: 0a20 2020 2020 2020 2044 6566 6175 6c74  .        Default
-0000c090: 2069 7320 4d41 5828 302c 2028 3a70 793a   is MAX(0, (:py:
-0000c0a0: 6174 7472 3a60 7e43 5061 7261 6d65 7465  attr:`~CParamete
-0000c0b0: 722e 7769 6e64 6f77 4c6f 6760 202d 203a  r.windowLog` - :
-0000c0c0: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
-0000c0d0: 6574 6572 2e6c 646d 4861 7368 4c6f 6760  eter.ldmHashLog`
-0000c0e0: 2929 2c20 6f70 7469 6d69 7a69 6e67 2068  )), optimizing h
-0000c0f0: 6173 6820 7461 626c 6520 7573 6167 652e  ash table usage.
-0000c100: 0a0a 2020 2020 2020 2020 4c61 7267 6572  ..        Larger
-0000c110: 2076 616c 7565 7320 696d 7072 6f76 6520   values improve 
-0000c120: 636f 6d70 7265 7373 696f 6e20 7370 6565  compression spee
-0000c130: 642e 0a0a 2020 2020 2020 2020 4465 7669  d...        Devi
-0000c140: 6174 696e 6720 6661 7220 6672 6f6d 2064  ating far from d
-0000c150: 6566 6175 6c74 2076 616c 7565 2077 696c  efault value wil
-0000c160: 6c20 6c69 6b65 6c79 2072 6573 756c 7420  l likely result 
-0000c170: 696e 2061 2063 6f6d 7072 6573 7369 6f6e  in a compression
-0000c180: 2072 6174 696f 2064 6563 7265 6173 652e   ratio decrease.
-0000c190: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
-0000c1a0: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
-0000c1b0: 6561 6e73 2022 6175 746f 6d61 7469 6361  eans "automatica
-0000c1c0: 6c6c 7920 6465 7465 726d 696e 6520 6861  lly determine ha
-0000c1d0: 7368 5261 7465 4c6f 6722 2e0a 0a20 2020  shRateLog"...   
-0000c1e0: 202e 2e20 5f63 6f6e 7465 6e74 5f73 697a   .. _content_siz
-0000c1f0: 653a 0a0a 2020 2020 2e2e 2070 793a 6174  e:..    .. py:at
-0000c200: 7472 6962 7574 653a 3a20 636f 6e74 656e  tribute:: conten
-0000c210: 7453 697a 6546 6c61 670a 0a20 2020 2020  tSizeFlag..     
-0000c220: 2020 2055 6e63 6f6d 7072 6573 7365 6420     Uncompressed 
-0000c230: 636f 6e74 656e 7420 7369 7a65 2077 696c  content size wil
-0000c240: 6c20 6265 2077 7269 7474 656e 2069 6e74  l be written int
-0000c250: 6f20 6672 616d 6520 6865 6164 6572 2077  o frame header w
-0000c260: 6865 6e65 7665 7220 6b6e 6f77 6e2e 0a0a  henever known...
-0000c270: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
-0000c280: 7661 6c75 6520 6973 2060 6031 6060 2c20  value is ``1``, 
-0000c290: 6361 6e20 6265 2060 6030 6060 2e0a 0a20  can be ``0``... 
-0000c2a0: 2020 2020 2020 2049 6e20 7472 6164 6974         In tradit
-0000c2b0: 696f 6e61 6c20 7374 7265 616d 696e 6720  ional streaming 
-0000c2c0: 636f 6d70 7265 7373 696f 6e2c 2063 6f6e  compression, con
-0000c2d0: 7465 6e74 2073 697a 6520 6973 2075 6e6b  tent size is unk
-0000c2e0: 6e6f 776e 2e0a 0a20 2020 2020 2020 2049  nown...        I
-0000c2f0: 6e20 7468 6573 6520 636f 6d70 7265 7373  n these compress
-0000c300: 696f 6e73 2c20 7468 6520 636f 6e74 656e  ions, the conten
-0000c310: 7420 7369 7a65 2069 7320 6b6e 6f77 6e3a  t size is known:
-0000c320: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
-0000c330: 3a70 793a 6675 6e63 3a60 636f 6d70 7265  :py:func:`compre
-0000c340: 7373 6020 6675 6e63 7469 6f6e 0a20 2020  ss` function.   
-0000c350: 2020 2020 2020 2020 202a 203a 7079 3a66           * :py:f
-0000c360: 756e 633a 6072 6963 686d 656d 5f63 6f6d  unc:`richmem_com
-0000c370: 7072 6573 7360 2066 756e 6374 696f 6e0a  press` function.
-0000c380: 2020 2020 2020 2020 2020 2020 2a20 3a70              * :p
-0000c390: 793a 636c 6173 733a 605a 7374 6443 6f6d  y:class:`ZstdCom
-0000c3a0: 7072 6573 736f 7260 2063 6c61 7373 2075  pressor` class u
-0000c3b0: 7369 6e67 2061 2073 696e 676c 6520 3a70  sing a single :p
-0000c3c0: 793a 6174 7472 3a60 7e5a 7374 6443 6f6d  y:attr:`~ZstdCom
-0000c3d0: 7072 6573 736f 722e 464c 5553 485f 4652  pressor.FLUSH_FR
-0000c3e0: 414d 4560 206d 6f64 650a 2020 2020 2020  AME` mode.      
-0000c3f0: 2020 2020 2020 2a20 3a70 793a 636c 6173        * :py:clas
-0000c400: 733a 6052 6963 684d 656d 5a73 7464 436f  s:`RichMemZstdCo
-0000c410: 6d70 7265 7373 6f72 6020 636c 6173 730a  mpressor` class.
-0000c420: 2020 2020 2020 2020 2020 2020 2a20 3a70              * :p
-0000c430: 793a 6675 6e63 3a60 636f 6d70 7265 7373  y:func:`compress
-0000c440: 5f73 7472 6561 6d60 2066 756e 6374 696f  _stream` functio
-0000c450: 6e20 7365 7474 696e 6720 2a70 6c65 6467  n setting *pledg
-0000c460: 6564 5f69 6e70 7574 5f73 697a 652a 2070  ed_input_size* p
-0000c470: 6172 616d 6574 6572 0a0a 2020 2020 2020  arameter..      
-0000c480: 2020 5468 6520 6669 656c 6420 696e 2066    The field in f
-0000c490: 7261 6d65 2068 6561 6465 7220 6973 2031  rame header is 1
-0000c4a0: 2f32 2f34 2f38 2062 7974 6573 2c20 6465  /2/4/8 bytes, de
-0000c4b0: 7065 6e64 696e 6720 6f6e 2073 697a 6520  pending on size 
-0000c4c0: 7661 6c75 652e 2049 7420 6d61 7920 6865  value. It may he
-0000c4d0: 6c70 2064 6563 6f6d 7072 6573 7369 6f6e  lp decompression
-0000c4e0: 2063 6f64 6520 746f 2061 6c6c 6f63 6174   code to allocat
-0000c4f0: 6520 6f75 7470 7574 2062 7566 6665 7220  e output buffer 
-0000c500: 6661 7374 6572 2e0a 0a20 2020 2020 2020  faster...       
-0000c510: 205c 2a20 3a70 793a 636c 6173 733a 605a   \* :py:class:`Z
-0000c520: 7374 6443 6f6d 7072 6573 736f 7260 2068  stdCompressor` h
-0000c530: 6173 2061 6e20 756e 646f 6375 6d65 6e74  as an undocument
-0000c540: 6564 206d 6574 686f 6420 746f 2073 6574  ed method to set
-0000c550: 2074 6865 2073 697a 652c 2060 6068 656c   the size, ``hel
-0000c560: 7028 5a73 7464 436f 6d70 7265 7373 6f72  p(ZstdCompressor
-0000c570: 2e5f 7365 745f 706c 6564 6765 645f 696e  ._set_pledged_in
-0000c580: 7075 745f 7369 7a65 2960 6020 746f 2073  put_size)`` to s
-0000c590: 6565 2074 6865 2075 7361 6765 2e0a 0a20  ee the usage... 
-0000c5a0: 2020 202e 2e20 7079 3a61 7474 7269 6275     .. py:attribu
-0000c5b0: 7465 3a3a 2063 6865 636b 7375 6d46 6c61  te:: checksumFla
-0000c5c0: 670a 0a20 2020 2020 2020 2041 2034 2d62  g..        A 4-b
-0000c5d0: 7974 6520 6368 6563 6b73 756d 206f 6620  yte checksum of 
-0000c5e0: 756e 636f 6d70 7265 7373 6564 2063 6f6e  uncompressed con
-0000c5f0: 7465 6e74 2069 7320 7772 6974 7465 6e20  tent is written 
-0000c600: 6174 2074 6865 2065 6e64 206f 6620 6672  at the end of fr
-0000c610: 616d 652e 0a0a 2020 2020 2020 2020 4465  ame...        De
-0000c620: 6661 756c 7420 7661 6c75 6520 6973 2060  fault value is `
-0000c630: 6030 6060 2c20 6361 6e20 6265 2060 6031  `0``, can be ``1
-0000c640: 6060 2e0a 0a20 2020 2020 2020 205a 7374  ``...        Zst
-0000c650: 6427 7320 6465 636f 6d70 7265 7373 696f  d's decompressio
-0000c660: 6e20 636f 6465 2076 6572 6966 6965 7320  n code verifies 
-0000c670: 6974 2e20 4966 2063 6865 636b 7375 6d20  it. If checksum 
-0000c680: 6d69 736d 6174 6368 2c20 7261 6973 6573  mismatch, raises
-0000c690: 2061 203a 7079 3a63 6c61 7373 3a60 5a73   a :py:class:`Zs
-0000c6a0: 7464 4572 726f 7260 2065 7863 6570 7469  tdError` excepti
-0000c6b0: 6f6e 2c20 7769 7468 2061 206d 6573 7361  on, with a messa
-0000c6c0: 6765 206c 696b 6520 2252 6573 746f 7265  ge like "Restore
-0000c6d0: 6420 6461 7461 2064 6f65 736e 2774 206d  d data doesn't m
-0000c6e0: 6174 6368 2063 6865 636b 7375 6d22 2e0a  atch checksum"..
-0000c6f0: 0a20 2020 202e 2e20 7079 3a61 7474 7269  .    .. py:attri
-0000c700: 6275 7465 3a3a 2064 6963 7449 4446 6c61  bute:: dictIDFla
-0000c710: 670a 0a20 2020 2020 2020 2057 6865 6e20  g..        When 
-0000c720: 6170 706c 6963 6162 6c65 2c20 6469 6374  applicable, dict
-0000c730: 696f 6e61 7279 2773 2049 4420 6973 2077  ionary's ID is w
-0000c740: 7269 7474 656e 2069 6e74 6f20 6672 616d  ritten into fram
-0000c750: 6520 6865 6164 6572 2e20 5365 6520 3a72  e header. See :r
-0000c760: 6566 3a60 7468 6973 206e 6f74 653c 6469  ef:`this note<di
-0000c770: 6374 5f69 643e 6020 666f 7220 6465 7461  ct_id>` for deta
-0000c780: 696c 732e 0a0a 2020 2020 2020 2020 4465  ils...        De
-0000c790: 6661 756c 7420 7661 6c75 6520 6973 2060  fault value is `
-0000c7a0: 6031 6060 2c20 6361 6e20 6265 2060 6030  `1``, can be ``0
-0000c7b0: 6060 2e0a 0a20 2020 202e 2e20 7079 3a61  ``...    .. py:a
-0000c7c0: 7474 7269 6275 7465 3a3a 206e 6257 6f72  ttribute:: nbWor
-0000c7d0: 6b65 7273 0a0a 2020 2020 2020 2020 5365  kers..        Se
-0000c7e0: 6c65 6374 2068 6f77 206d 616e 7920 7468  lect how many th
-0000c7f0: 7265 6164 7320 7769 6c6c 2062 6520 7370  reads will be sp
-0000c800: 6177 6e65 6420 746f 2063 6f6d 7072 6573  awned to compres
-0000c810: 7320 696e 2070 6172 616c 6c65 6c2e 0a0a  s in parallel...
-0000c820: 2020 2020 2020 2020 5768 656e 206e 6257          When nbW
-0000c830: 6f72 6b65 7273 203e 3d20 6060 3160 602c  orkers >= ``1``,
-0000c840: 2065 6e61 626c 6573 206d 756c 7469 2d74   enables multi-t
-0000c850: 6872 6561 6465 6420 636f 6d70 7265 7373  hreaded compress
-0000c860: 696f 6e2c 2060 6031 6060 206d 6561 6e73  ion, ``1`` means
-0000c870: 2022 312d 7468 7265 6164 206d 756c 7469   "1-thread multi
-0000c880: 2d74 6872 6561 6465 6420 6d6f 6465 222e  -threaded mode".
-0000c890: 2053 6565 203a 7265 663a 607a 7374 6420   See :ref:`zstd 
-0000c8a0: 6d75 6c74 692d 7468 7265 6164 6564 2063  multi-threaded c
-0000c8b0: 6f6d 7072 6573 7369 6f6e 3c6d 745f 636f  ompression<mt_co
-0000c8c0: 6d70 7265 7373 696f 6e3e 6020 666f 7220  mpression>` for 
-0000c8d0: 6465 7461 696c 732e 0a0a 2020 2020 2020  details...      
-0000c8e0: 2020 4d6f 7265 2077 6f72 6b65 7273 2069    More workers i
-0000c8f0: 6d70 726f 7665 2073 7065 6564 2c20 6275  mprove speed, bu
-0000c900: 7420 616c 736f 2069 6e63 7265 6173 6520  t also increase 
-0000c910: 6d65 6d6f 7279 2075 7361 6765 2e0a 0a20  memory usage... 
-0000c920: 2020 2020 2020 2060 6030 6060 2028 6465         ``0`` (de
-0000c930: 6661 756c 7429 206d 6561 6e73 2022 7369  fault) means "si
-0000c940: 6e67 6c65 2d74 6872 6561 6465 6420 6d6f  ngle-threaded mo
-0000c950: 6465 222c 206e 6f20 776f 726b 6572 2069  de", no worker i
-0000c960: 7320 7370 6177 6e65 642c 2063 6f6d 7072  s spawned, compr
-0000c970: 6573 7369 6f6e 2069 7320 7065 7266 6f72  ession is perfor
-0000c980: 6d65 6420 696e 7369 6465 2063 616c 6c65  med inside calle
-0000c990: 7227 7320 7468 7265 6164 2e0a 0a20 2020  r's thread...   
-0000c9a0: 202e 2e20 7665 7273 696f 6e63 6861 6e67   .. versionchang
-0000c9b0: 6564 3a3a 2030 2e31 352e 310a 2020 2020  ed:: 0.15.1.    
-0000c9c0: 2020 2020 5365 7474 696e 6720 746f 2060      Setting to `
-0000c9d0: 6031 6060 206d 6561 6e73 2022 312d 7468  `1`` means "1-th
-0000c9e0: 7265 6164 206d 756c 7469 2d74 6872 6561  read multi-threa
-0000c9f0: 6465 6420 6d6f 6465 222c 2069 6e73 7465  ded mode", inste
-0000ca00: 6164 206f 6620 2273 696e 676c 652d 7468  ad of "single-th
-0000ca10: 7265 6164 6564 206d 6f64 6522 2e0a 0a20  readed mode"... 
-0000ca20: 2020 202e 2e20 7079 3a61 7474 7269 6275     .. py:attribu
-0000ca30: 7465 3a3a 206a 6f62 5369 7a65 0a0a 2020  te:: jobSize..  
-0000ca40: 2020 2020 2020 5369 7a65 206f 6620 6120        Size of a 
-0000ca50: 636f 6d70 7265 7373 696f 6e20 6a6f 622c  compression job,
-0000ca60: 2069 6e20 6279 7465 732e 0a0a 2020 2020   in bytes...    
-0000ca70: 2020 2020 5468 6973 2076 616c 7565 2069      This value i
-0000ca80: 7320 656e 666f 7263 6564 206f 6e6c 7920  s enforced only 
-0000ca90: 7768 656e 203a 7079 3a61 7474 723a 607e  when :py:attr:`~
-0000caa0: 4350 6172 616d 6574 6572 2e6e 6257 6f72  CParameter.nbWor
-0000cab0: 6b65 7273 6020 3e3d 2031 2e0a 0a20 2020  kers` >= 1...   
-0000cac0: 2020 2020 2045 6163 6820 636f 6d70 7265       Each compre
-0000cad0: 7373 696f 6e20 6a6f 6220 6973 2063 6f6d  ssion job is com
-0000cae0: 706c 6574 6564 2069 6e20 7061 7261 6c6c  pleted in parall
-0000caf0: 656c 2c20 736f 2074 6869 7320 7661 6c75  el, so this valu
-0000cb00: 6520 6361 6e20 696e 6469 7265 6374 6c79  e can indirectly
-0000cb10: 2069 6d70 6163 7420 7468 6520 6e75 6d62   impact the numb
-0000cb20: 6572 206f 6620 6163 7469 7665 2074 6872  er of active thr
-0000cb30: 6561 6473 2e0a 0a20 2020 2020 2020 2060  eads...        `
-0000cb40: 6030 6060 206d 6561 6e73 2064 6566 6175  `0`` means defau
-0000cb50: 6c74 2c20 7768 6963 6820 6973 2064 796e  lt, which is dyn
-0000cb60: 616d 6963 616c 6c79 2064 6574 6572 6d69  amically determi
-0000cb70: 6e65 6420 6261 7365 6420 6f6e 2063 6f6d  ned based on com
-0000cb80: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
-0000cb90: 6572 732e 0a0a 2020 2020 2020 2020 4e6f  ers...        No
-0000cba0: 6e2d 7a65 726f 2076 616c 7565 2077 696c  n-zero value wil
-0000cbb0: 6c20 6265 2073 696c 656e 746c 7920 636c  l be silently cl
-0000cbc0: 616d 7065 6420 746f 3a0a 0a20 2020 2020  amped to:..     
-0000cbd0: 2020 202a 206d 696e 696d 756d 2076 616c     * minimum val
-0000cbe0: 7565 3a20 6060 6d61 7828 6f76 6572 6c61  ue: ``max(overla
-0000cbf0: 705f 7369 7a65 2c20 3531 325f 4b69 4229  p_size, 512_KiB)
-0000cc00: 6060 2e20 6f76 6572 6c61 705f 7369 7a65  ``. overlap_size
-0000cc10: 2069 7320 7370 6563 6966 6965 6420 6279   is specified by
-0000cc20: 203a 7079 3a61 7474 723a 607e 4350 6172   :py:attr:`~CPar
-0000cc30: 616d 6574 6572 2e6f 7665 726c 6170 4c6f  ameter.overlapLo
-0000cc40: 6760 2070 6172 616d 6574 6572 2e0a 2020  g` parameter..  
-0000cc50: 2020 2020 2020 2a20 6d61 7869 6d75 6d20        * maximum 
-0000cc60: 7661 6c75 653a 2060 6035 3132 5f4d 6942  value: ``512_MiB
-0000cc70: 2069 6620 3332 5f62 6974 5f62 7569 6c64   if 32_bit_build
-0000cc80: 2065 6c73 6520 3130 3234 5f4d 6942 6060   else 1024_MiB``
-0000cc90: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
-0000cca0: 7269 6275 7465 3a3a 206f 7665 726c 6170  ribute:: overlap
-0000ccb0: 4c6f 670a 0a20 2020 2020 2020 2043 6f6e  Log..        Con
-0000ccc0: 7472 6f6c 2074 6865 206f 7665 726c 6170  trol the overlap
-0000ccd0: 2073 697a 652c 2061 7320 6120 6672 6163   size, as a frac
-0000cce0: 7469 6f6e 206f 6620 7769 6e64 6f77 2073  tion of window s
-0000ccf0: 697a 652e 2028 5468 6520 2277 696e 646f  ize. (The "windo
-0000cd00: 7720 7369 7a65 2220 6865 7265 2069 7320  w size" here is 
-0000cd10: 6e6f 7420 7374 7269 6374 203a 7079 3a61  not strict :py:a
-0000cd20: 7474 723a 607e 4350 6172 616d 6574 6572  ttr:`~CParameter
-0000cd30: 2e77 696e 646f 774c 6f67 602c 2073 6565  .windowLog`, see
-0000cd40: 207a 7374 6420 736f 7572 6365 2063 6f64   zstd source cod
-0000cd50: 652e 290a 0a20 2020 2020 2020 2054 6869  e.)..        Thi
-0000cd60: 7320 7661 6c75 6520 6973 2065 6e66 6f72  s value is enfor
-0000cd70: 6365 6420 6f6e 6c79 2077 6865 6e20 3a70  ced only when :p
-0000cd80: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
-0000cd90: 7465 722e 6e62 576f 726b 6572 7360 203e  ter.nbWorkers` >
-0000cda0: 3d20 312e 0a0a 2020 2020 2020 2020 5468  = 1...        Th
-0000cdb0: 6520 6f76 6572 6c61 7020 7369 7a65 2069  e overlap size i
-0000cdc0: 7320 616e 2061 6d6f 756e 7420 6f66 2064  s an amount of d
-0000cdd0: 6174 6120 7265 6c6f 6164 6564 2066 726f  ata reloaded fro
-0000cde0: 6d20 7072 6576 696f 7573 206a 6f62 2061  m previous job a
-0000cdf0: 7420 7468 6520 6265 6769 6e6e 696e 6720  t the beginning 
-0000ce00: 6f66 2061 206e 6577 206a 6f62 2e20 4974  of a new job. It
-0000ce10: 2068 656c 7073 2070 7265 7365 7276 6520   helps preserve 
-0000ce20: 636f 6d70 7265 7373 696f 6e20 7261 7469  compression rati
-0000ce30: 6f2c 2077 6869 6c65 2065 6163 6820 6a6f  o, while each jo
-0000ce40: 6220 6973 2063 6f6d 7072 6573 7365 6420  b is compressed 
-0000ce50: 696e 2070 6172 616c 6c65 6c2e 204c 6172  in parallel. Lar
-0000ce60: 6765 7220 7661 6c75 6573 2069 6e63 7265  ger values incre
-0000ce70: 6173 6520 636f 6d70 7265 7373 696f 6e20  ase compression 
-0000ce80: 7261 7469 6f2c 2062 7574 2064 6563 7265  ratio, but decre
-0000ce90: 6173 6520 7370 6565 642e 0a0a 2020 2020  ase speed...    
-0000cea0: 2020 2020 506f 7373 6962 6c65 2076 616c      Possible val
-0000ceb0: 7565 7320 7261 6e67 6520 6672 6f6d 2030  ues range from 0
-0000cec0: 2074 6f20 393a 0a0a 2020 2020 2020 2020   to 9:..        
-0000ced0: 2d20 3020 6d65 616e 7320 2264 6566 6175  - 0 means "defau
-0000cee0: 6c74 2220 3a20 5468 6520 7661 6c75 6520  lt" : The value 
-0000cef0: 7769 6c6c 2062 6520 6465 7465 726d 696e  will be determin
-0000cf00: 6564 2062 7920 7468 6520 6c69 6272 6172  ed by the librar
-0000cf10: 792e 2054 6865 2076 616c 7565 2076 6172  y. The value var
-0000cf20: 6965 7320 6265 7477 6565 6e20 3620 616e  ies between 6 an
-0000cf30: 6420 392c 2064 6570 656e 6469 6e67 206f  d 9, depending o
-0000cf40: 6e20 3a70 793a 6174 7472 3a60 7e43 5061  n :py:attr:`~CPa
-0000cf50: 7261 6d65 7465 722e 7374 7261 7465 6779  rameter.strategy
-0000cf60: 602e 0a20 2020 2020 2020 202d 2031 206d  `..        - 1 m
-0000cf70: 6561 6e73 2022 6e6f 206f 7665 726c 6170  eans "no overlap
-0000cf80: 220a 2020 2020 2020 2020 2d20 3920 6d65  ".        - 9 me
-0000cf90: 616e 7320 2266 756c 6c20 6f76 6572 6c61  ans "full overla
-0000cfa0: 7022 2c20 7573 696e 6720 6120 6675 6c6c  p", using a full
-0000cfb0: 2077 696e 646f 7720 7369 7a65 2e0a 0a20   window size... 
-0000cfc0: 2020 2020 2020 2045 6163 6820 696e 7465         Each inte
-0000cfd0: 726d 6564 6961 7465 2072 616e 6b20 696e  rmediate rank in
-0000cfe0: 6372 6561 7365 732f 6465 6372 6561 7365  creases/decrease
-0000cff0: 7320 6c6f 6164 2073 697a 6520 6279 2061  s load size by a
-0000d000: 2066 6163 746f 7220 323a 0a0a 2020 2020   factor 2:..    
-0000d010: 2020 2020 393a 2066 756c 6c20 7769 6e64      9: full wind
-0000d020: 6f77 3b20 2038 3a20 772f 323b 2020 373a  ow;  8: w/2;  7:
-0000d030: 2077 2f34 3b20 2036 3a20 772f 383b 2020   w/4;  6: w/8;  
-0000d040: 353a 2077 2f31 363b 2020 343a 2077 2f33  5: w/16;  4: w/3
-0000d050: 323b 2020 333a 2077 2f36 343b 2020 323a  2;  3: w/64;  2:
-0000d060: 2077 2f31 3238 3b20 2031 3a20 6e6f 206f   w/128;  1: no o
-0000d070: 7665 726c 6170 3b20 2030 3a20 6465 6661  verlap;  0: defa
-0000d080: 756c 742e 0a0a 0a2e 2e20 5f44 5061 7261  ult...... _DPara
-0000d090: 6d65 7465 723a 0a0a 2e2e 2070 793a 636c  meter:.... py:cl
-0000d0a0: 6173 733a 3a20 4450 6172 616d 6574 6572  ass:: DParameter
-0000d0b0: 2849 6e74 456e 756d 290a 0a20 2020 2041  (IntEnum)..    A
-0000d0c0: 6476 616e 6365 6420 6465 636f 6d70 7265  dvanced decompre
-0000d0d0: 7373 696f 6e20 7061 7261 6d65 7465 7273  ssion parameters
-0000d0e0: 2e0a 0a20 2020 2057 6865 6e20 7573 696e  ...    When usin
-0000d0f0: 672c 2070 7574 2074 6865 2070 6172 616d  g, put the param
-0000d100: 6574 6572 7320 696e 2061 2060 6064 6963  eters in a ``dic
-0000d110: 7460 6020 6f62 6a65 6374 2c20 7468 6520  t`` object, the 
-0000d120: 6b65 7920 6973 2061 203a 7079 3a63 6c61  key is a :py:cla
-0000d130: 7373 3a60 4450 6172 616d 6574 6572 6020  ss:`DParameter` 
-0000d140: 6e61 6d65 2c20 7468 6520 7661 6c75 6520  name, the value 
-0000d150: 6973 2061 2033 322d 6269 7420 7369 676e  is a 32-bit sign
-0000d160: 6564 2069 6e74 6567 6572 2076 616c 7565  ed integer value
-0000d170: 2e0a 0a20 2020 202e 2e20 736f 7572 6365  ...    .. source
-0000d180: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-0000d190: 2020 2020 2020 2023 2073 6574 206d 656d         # set mem
-0000d1a0: 6f72 7920 616c 6c6f 6361 7469 6f6e 206c  ory allocation l
-0000d1b0: 696d 6974 2074 6f20 3136 204d 6942 2028  imit to 16 MiB (
-0000d1c0: 3120 3c3c 2032 3429 0a20 2020 2020 2020  1 << 24).       
-0000d1d0: 206f 7074 696f 6e20 3d20 7b44 5061 7261   option = {DPara
-0000d1e0: 6d65 7465 722e 7769 6e64 6f77 4c6f 674d  meter.windowLogM
-0000d1f0: 6178 203a 2032 347d 0a0a 2020 2020 2020  ax : 24}..      
-0000d200: 2020 2320 7573 6564 2077 6974 6820 6465    # used with de
-0000d210: 636f 6d70 7265 7373 2829 2066 756e 6374  compress() funct
-0000d220: 696f 6e0a 2020 2020 2020 2020 6465 636f  ion.        deco
-0000d230: 6d70 7265 7373 6564 5f64 6174 203d 2064  mpressed_dat = d
-0000d240: 6563 6f6d 7072 6573 7328 6461 742c 206f  ecompress(dat, o
-0000d250: 7074 696f 6e3d 6f70 7469 6f6e 290a 0a20  ption=option).. 
-0000d260: 2020 2020 2020 2023 2075 7365 6420 7769         # used wi
-0000d270: 7468 205a 7374 6444 6563 6f6d 7072 6573  th ZstdDecompres
-0000d280: 736f 7220 6f62 6a65 6374 0a20 2020 2020  sor object.     
-0000d290: 2020 2064 203d 205a 7374 6444 6563 6f6d     d = ZstdDecom
-0000d2a0: 7072 6573 736f 7228 6f70 7469 6f6e 3d6f  pressor(option=o
-0000d2b0: 7074 696f 6e29 0a20 2020 2020 2020 2064  ption).        d
-0000d2c0: 6563 6f6d 7072 6573 7365 645f 6461 7420  ecompressed_dat 
-0000d2d0: 3d20 642e 6465 636f 6d70 7265 7373 2864  = d.decompress(d
-0000d2e0: 6174 290a 0a20 2020 2050 6172 616d 6574  at)..    Paramet
-0000d2f0: 6572 2076 616c 7565 2073 686f 756c 6420  er value should 
-0000d300: 6265 6c6f 6e67 2074 6f20 616e 2069 6e74  belong to an int
-0000d310: 6572 7661 6c20 7769 7468 206c 6f77 6572  erval with lower
-0000d320: 2061 6e64 2075 7070 6572 2062 6f75 6e64   and upper bound
-0000d330: 732c 206f 7468 6572 7769 7365 2074 6865  s, otherwise the
-0000d340: 7920 7769 6c6c 2065 6974 6865 7220 7472  y will either tr
-0000d350: 6967 6765 7220 616e 2065 7272 6f72 206f  igger an error o
-0000d360: 7220 6265 2063 6c61 6d70 6564 2073 696c  r be clamped sil
-0000d370: 656e 746c 792e 0a0a 2020 2020 5468 6520  ently...    The 
-0000d380: 636f 6e73 7461 6e74 2076 616c 7565 7320  constant values 
-0000d390: 6d65 6e74 696f 6e65 6420 6265 6c6f 7720  mentioned below 
-0000d3a0: 6172 6520 6465 6669 6e65 6420 696e 2060  are defined in `
-0000d3b0: 7a73 7464 2e68 203c 6874 7470 733a 2f2f  zstd.h <https://
-0000d3c0: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
-0000d3d0: 6f6f 6b2f 7a73 7464 2f62 6c6f 622f 7265  ook/zstd/blob/re
-0000d3e0: 6c65 6173 652f 6c69 622f 7a73 7464 2e68  lease/lib/zstd.h
-0000d3f0: 3e60 5f2c 206e 6f74 6520 7468 6174 2074  >`_, note that t
-0000d400: 6865 7365 2076 616c 7565 7320 6d61 7920  hese values may 
-0000d410: 6265 2064 6966 6665 7265 6e74 2069 6e20  be different in 
-0000d420: 6469 6666 6572 656e 7420 7a73 7464 2076  different zstd v
-0000d430: 6572 7369 6f6e 732e 0a0a 2020 2020 2e2e  ersions...    ..
-0000d440: 2070 793a 6d65 7468 6f64 3a3a 2062 6f75   py:method:: bou
-0000d450: 6e64 7328 7365 6c66 290a 0a20 2020 2020  nds(self)..     
-0000d460: 2020 2052 6574 7572 6e20 6c6f 7765 7220     Return lower 
-0000d470: 616e 6420 7570 7065 7220 626f 756e 6473  and upper bounds
-0000d480: 206f 6620 6120 7061 7261 6d65 7465 722c   of a parameter,
-0000d490: 2062 6f74 6820 696e 636c 7573 6976 652e   both inclusive.
-0000d4a0: 0a0a 2020 2020 2020 2020 2e2e 2073 6f75  ..        .. sou
-0000d4b0: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
-0000d4c0: 0a0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-0000d4d0: 3e20 4450 6172 616d 6574 6572 2e77 696e  > DParameter.win
-0000d4e0: 646f 774c 6f67 4d61 782e 626f 756e 6473  dowLogMax.bounds
-0000d4f0: 2829 0a20 2020 2020 2020 2020 2020 2028  ().            (
-0000d500: 3130 2c20 3331 290a 0a20 2020 202e 2e20  10, 31)..    .. 
-0000d510: 7079 3a61 7474 7269 6275 7465 3a3a 2077  py:attribute:: w
-0000d520: 696e 646f 774c 6f67 4d61 780a 0a20 2020  indowLogMax..   
-0000d530: 2020 2020 2053 656c 6563 7420 6120 7369       Select a si
-0000d540: 7a65 206c 696d 6974 2028 696e 2070 6f77  ze limit (in pow
-0000d550: 6572 206f 6620 3229 2062 6579 6f6e 6420  er of 2) beyond 
-0000d560: 7768 6963 6820 7468 6520 7374 7265 616d  which the stream
-0000d570: 696e 6720 4150 4920 7769 6c6c 2072 6566  ing API will ref
-0000d580: 7573 6520 746f 2061 6c6c 6f63 6174 6520  use to allocate 
-0000d590: 6d65 6d6f 7279 2062 7566 6665 7220 696e  memory buffer in
-0000d5a0: 206f 7264 6572 2074 6f20 7072 6f74 6563   order to protec
-0000d5b0: 7420 7468 6520 686f 7374 2066 726f 6d20  t the host from 
-0000d5c0: 756e 7265 6173 6f6e 6162 6c65 206d 656d  unreasonable mem
-0000d5d0: 6f72 7920 7265 7175 6972 656d 656e 7473  ory requirements
-0000d5e0: 2e0a 0a20 2020 2020 2020 2049 6620 6120  ...        If a 
-0000d5f0: 3a72 6566 3a60 6672 616d 653c 6672 616d  :ref:`frame<fram
-0000d600: 655f 626c 6f63 6b3e 6020 7265 7175 6972  e_block>` requir
-0000d610: 6573 206d 6f72 6520 6d65 6d6f 7279 2074  es more memory t
-0000d620: 6861 6e20 7468 6520 7365 7420 7661 6c75  han the set valu
-0000d630: 652c 2072 6169 7365 7320 6120 3a70 793a  e, raises a :py:
-0000d640: 636c 6173 733a 605a 7374 6445 7272 6f72  class:`ZstdError
-0000d650: 6020 6578 6365 7074 696f 6e2c 2077 6974  ` exception, wit
-0000d660: 6820 6120 6d65 7373 6167 6520 6c69 6b65  h a message like
-0000d670: 2022 4672 616d 6520 7265 7175 6972 6573   "Frame requires
-0000d680: 2074 6f6f 206d 7563 6820 6d65 6d6f 7279   too much memory
-0000d690: 2066 6f72 2064 6563 6f64 696e 6722 2e0a   for decoding"..
-0000d6a0: 0a20 2020 2020 2020 2054 6869 7320 7061  .        This pa
-0000d6b0: 7261 6d65 7465 7220 6973 206f 6e6c 7920  rameter is only 
-0000d6c0: 7573 6566 756c 2069 6e20 7374 7265 616d  useful in stream
-0000d6d0: 696e 6720 6d6f 6465 2c20 7369 6e63 6520  ing mode, since 
-0000d6e0: 6e6f 2069 6e74 6572 6e61 6c20 6275 6666  no internal buff
-0000d6f0: 6572 2069 7320 616c 6c6f 6361 7465 6420  er is allocated 
-0000d700: 696e 2073 696e 676c 652d 7061 7373 206d  in single-pass m
-0000d710: 6f64 652e 203a 7079 3a66 756e 633a 6064  ode. :py:func:`d
-0000d720: 6563 6f6d 7072 6573 7360 2066 756e 6374  ecompress` funct
-0000d730: 696f 6e20 6d61 7920 7573 6520 7374 7265  ion may use stre
-0000d740: 616d 696e 6720 6d6f 6465 206f 7220 7369  aming mode or si
-0000d750: 6e67 6c65 2d70 6173 7320 6d6f 6465 2e0a  ngle-pass mode..
-0000d760: 0a20 2020 2020 2020 2042 7920 6465 6661  .        By defa
-0000d770: 756c 742c 2061 2064 6563 6f6d 7072 6573  ult, a decompres
-0000d780: 7369 6f6e 2063 6f6e 7465 7874 2061 6363  sion context acc
-0000d790: 6570 7473 2077 696e 646f 7720 7369 7a65  epts window size
-0000d7a0: 7320 3c3d 2060 6028 3120 3c3c 205a 5354  s <= ``(1 << ZST
-0000d7b0: 445f 5749 4e44 4f57 4c4f 475f 4c49 4d49  D_WINDOWLOG_LIMI
-0000d7c0: 545f 4445 4641 554c 5429 6060 2c20 7468  T_DEFAULT)``, th
-0000d7d0: 6520 636f 6e73 7461 6e74 2069 7320 6060  e constant is ``
-0000d7e0: 3237 6060 2069 6e20 7a73 7464 2076 312e  27`` in zstd v1.
-0000d7f0: 322b 2c20 6d65 616e 7320 3132 3820 4d69  2+, means 128 Mi
-0000d800: 4220 2831 203c 3c20 3237 292e 2049 6620  B (1 << 27). If 
-0000d810: 6672 616d 6520 7265 7175 6573 7465 6420  frame requested 
-0000d820: 7769 6e64 6f77 2073 697a 6520 6973 2067  window size is g
-0000d830: 7265 6174 6572 2074 6861 6e20 7468 6973  reater than this
-0000d840: 2076 616c 7565 2c20 6e65 6564 2074 6f20   value, need to 
-0000d850: 6578 706c 6963 6974 6c79 2073 6574 2074  explicitly set t
-0000d860: 6869 7320 7061 7261 6d65 7465 722e 0a0a  his parameter...
-0000d870: 2020 2020 2020 2020 5370 6563 6961 6c3a          Special:
-0000d880: 2076 616c 7565 2060 6030 6060 206d 6561   value ``0`` mea
-0000d890: 6e73 2022 7573 6520 6465 6661 756c 7420  ns "use default 
-0000d8a0: 6d61 7869 6d75 6d20 7769 6e64 6f77 4c6f  maximum windowLo
-0000d8b0: 6722 2e0a 0a0a 2e2e 2070 793a 636c 6173  g"...... py:clas
-0000d8c0: 733a 3a20 5374 7261 7465 6779 2849 6e74  s:: Strategy(Int
-0000d8d0: 456e 756d 290a 0a20 2020 2055 7365 6420  Enum)..    Used 
-0000d8e0: 666f 7220 3a70 793a 6174 7472 3a60 4350  for :py:attr:`CP
-0000d8f0: 6172 616d 6574 6572 2e73 7472 6174 6567  arameter.strateg
-0000d900: 7960 2e0a 0a20 2020 2043 6f6d 7072 6573  y`...    Compres
-0000d910: 7369 6f6e 2073 7472 6174 6567 6965 732c  sion strategies,
-0000d920: 206c 6973 7465 6420 6672 6f6d 2066 6173   listed from fas
-0000d930: 7465 7374 2074 6f20 7374 726f 6e67 6573  test to stronges
-0000d940: 742e 0a0a 2020 2020 4e6f 7465 203a 206e  t...    Note : n
-0000d950: 6577 2073 7472 6174 6567 6965 7320 2a2a  ew strategies **
-0000d960: 6d69 6768 742a 2a20 6265 2061 6464 6564  might** be added
-0000d970: 2069 6e20 7468 6520 6675 7475 7265 2c20   in the future, 
-0000d980: 6f6e 6c79 2074 6865 206f 7264 6572 2028  only the order (
-0000d990: 6672 6f6d 2066 6173 7420 746f 2073 7472  from fast to str
-0000d9a0: 6f6e 6729 2069 7320 6775 6172 616e 7465  ong) is guarante
-0000d9b0: 6564 2e0a 0a20 2020 202e 2e20 7079 3a61  ed...    .. py:a
-0000d9c0: 7474 7269 6275 7465 3a3a 2066 6173 740a  ttribute:: fast.
-0000d9d0: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
-0000d9e0: 7574 653a 3a20 6466 6173 740a 2020 2020  ute:: dfast.    
-0000d9f0: 2e2e 2070 793a 6174 7472 6962 7574 653a  .. py:attribute:
-0000da00: 3a20 6772 6565 6479 0a20 2020 202e 2e20  : greedy.    .. 
-0000da10: 7079 3a61 7474 7269 6275 7465 3a3a 206c  py:attribute:: l
-0000da20: 617a 790a 2020 2020 2e2e 2070 793a 6174  azy.    .. py:at
-0000da30: 7472 6962 7574 653a 3a20 6c61 7a79 320a  tribute:: lazy2.
-0000da40: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
-0000da50: 7574 653a 3a20 6274 6c61 7a79 320a 2020  ute:: btlazy2.  
-0000da60: 2020 2e2e 2070 793a 6174 7472 6962 7574    .. py:attribut
-0000da70: 653a 3a20 6274 6f70 740a 2020 2020 2e2e  e:: btopt.    ..
-0000da80: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
-0000da90: 6274 756c 7472 610a 2020 2020 2e2e 2070  btultra.    .. p
-0000daa0: 793a 6174 7472 6962 7574 653a 3a20 6274  y:attribute:: bt
-0000dab0: 756c 7472 6132 0a0a 2020 2020 2e2e 2073  ultra2..    .. s
-0000dac0: 6f75 7263 6563 6f64 653a 3a20 7079 7468  ourcecode:: pyth
-0000dad0: 6f6e 0a0a 2020 2020 2020 2020 6f70 7469  on..        opti
-0000dae0: 6f6e 203d 207b 4350 6172 616d 6574 6572  on = {CParameter
-0000daf0: 2e73 7472 6174 6567 7920 3a20 5374 7261  .strategy : Stra
-0000db00: 7465 6779 2e6c 617a 7932 2c0a 2020 2020  tegy.lazy2,.    
-0000db10: 2020 2020 2020 2020 2020 2020 2020 4350                CP
-0000db20: 6172 616d 6574 6572 2e63 6865 636b 7375  arameter.checksu
-0000db30: 6d46 6c61 6720 3a20 317d 0a20 2020 2020  mFlag : 1}.     
-0000db40: 2020 2063 6f6d 7072 6573 7365 645f 6461     compressed_da
-0000db50: 7420 3d20 636f 6d70 7265 7373 2872 6177  t = compress(raw
-0000db60: 5f64 6174 2c20 6f70 7469 6f6e 290a 0a0a  _dat, option)...
-0000db70: 496e 666f 726d 6174 6976 6520 6e6f 7465  Informative note
-0000db80: 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s.--------------
-0000db90: 2d2d 2d0a 0a43 6f6d 7072 6573 7369 6f6e  ---..Compression
-0000dba0: 206c 6576 656c 0a3e 3e3e 3e3e 3e3e 3e3e   level.>>>>>>>>>
-0000dbb0: 3e3e 3e3e 3e3e 3e3e 0a0a 2e2e 205f 636f  >>>>>>>>.... _co
-0000dbc0: 6d70 7265 7373 696f 6e5f 6c65 7665 6c3a  mpression_level:
-0000dbd0: 0a0a 2e2e 206e 6f74 653a 3a20 436f 6d70  .... note:: Comp
-0000dbe0: 7265 7373 696f 6e20 6c65 7665 6c0a 0a20  ression level.. 
-0000dbf0: 2020 2043 6f6d 7072 6573 7369 6f6e 206c     Compression l
-0000dc00: 6576 656c 2069 7320 616e 2069 6e74 6567  evel is an integ
-0000dc10: 6572 3a0a 0a20 2020 202a 2060 6031 6060  er:..    * ``1``
-0000dc20: 2074 6f20 6060 3232 6060 2028 6375 7272   to ``22`` (curr
-0000dc30: 656e 746c 7929 2c20 7265 6775 6c61 7220  ently), regular 
-0000dc40: 6c65 7665 6c73 2e20 4c65 7665 6c73 203e  levels. Levels >
-0000dc50: 3d20 3230 2c20 6c61 6265 6c65 6420 2a75  = 20, labeled *u
-0000dc60: 6c74 7261 2a2c 2073 686f 756c 6420 6265  ltra*, should be
-0000dc70: 2075 7365 6420 7769 7468 2063 6175 7469   used with cauti
-0000dc80: 6f6e 2c20 6173 2074 6865 7920 7265 7175  on, as they requ
-0000dc90: 6972 6520 6d6f 7265 206d 656d 6f72 792e  ire more memory.
-0000dca0: 0a20 2020 202a 2060 6030 6060 206d 6561  .    * ``0`` mea
-0000dcb0: 6e73 2075 7365 2074 6865 2064 6566 6175  ns use the defau
-0000dcc0: 6c74 206c 6576 656c 2c20 7768 6963 6820  lt level, which 
-0000dcd0: 6973 2063 7572 7265 6e74 6c79 2060 6033  is currently ``3
-0000dce0: 6060 2064 6566 696e 6564 2062 7920 7468  `` defined by th
-0000dcf0: 6520 756e 6465 726c 7969 6e67 207a 7374  e underlying zst
-0000dd00: 6420 6c69 6272 6172 792e 0a20 2020 202a  d library..    *
-0000dd10: 2060 602d 3133 3130 3732 6060 2074 6f20   ``-131072`` to 
-0000dd20: 6060 2d31 6060 2c20 6e65 6761 7469 7665  ``-1``, negative
-0000dd30: 206c 6576 656c 7320 6578 7465 6e64 2074   levels extend t
-0000dd40: 6865 2072 616e 6765 206f 6620 7370 6565  he range of spee
-0000dd50: 6420 7673 2072 6174 696f 2070 7265 6665  d vs ratio prefe
-0000dd60: 7265 6e63 6573 2e20 5468 6520 6c6f 7765  rences. The lowe
-0000dd70: 7220 7468 6520 6c65 7665 6c2c 2074 6865  r the level, the
-0000dd80: 2066 6173 7465 7220 7468 6520 7370 6565   faster the spee
-0000dd90: 642c 2062 7574 2061 7420 7468 6520 636f  d, but at the co
-0000dda0: 7374 206f 6620 636f 6d70 7265 7373 696f  st of compressio
-0000ddb0: 6e20 7261 7469 6f2e 2031 3331 3037 3220  n ratio. 131072 
-0000ddc0: 3d20 3132 382a 3130 3234 2e0a 0a20 2020  = 128*1024...   
-0000ddd0: 203a 7079 3a64 6174 613a 6063 6f6d 7072   :py:data:`compr
-0000dde0: 6573 7369 6f6e 4c65 7665 6c5f 7661 6c75  essionLevel_valu
-0000ddf0: 6573 6020 6172 6520 736f 6d65 2076 616c  es` are some val
-0000de00: 7565 7320 6465 6669 6e65 6420 6279 2074  ues defined by t
-0000de10: 6865 2075 6e64 6572 6c79 696e 6720 7a73  he underlying zs
-0000de20: 7464 206c 6962 7261 7279 2e0a 0a20 2020  td library...   
-0000de30: 202a 2a46 6f72 2061 6476 616e 6365 6420   **For advanced 
-0000de40: 7573 6572 2a2a 0a0a 2020 2020 436f 6d70  user**..    Comp
-0000de50: 7265 7373 696f 6e20 6c65 7665 6c73 2061  ression levels a
-0000de60: 7265 206a 7573 7420 6e75 6d62 6572 7320  re just numbers 
-0000de70: 7468 6174 206d 6170 2074 6f20 6120 7365  that map to a se
-0000de80: 7420 6f66 2063 6f6d 7072 6573 7369 6f6e  t of compression
-0000de90: 2070 6172 616d 6574 6572 732c 2073 6565   parameters, see
-0000dea0: 2060 7468 6973 2074 6162 6c65 203c 6874   `this table <ht
-0000deb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000dec0: 2f66 6163 6562 6f6f 6b2f 7a73 7464 2f62  /facebook/zstd/b
-0000ded0: 6c6f 622f 7265 6c65 6173 652f 6c69 622f  lob/release/lib/
-0000dee0: 636f 6d70 7265 7373 2f63 6c65 7665 6c73  compress/clevels
-0000def0: 2e68 3e60 5f20 666f 7220 6f76 6572 7669  .h>`_ for overvi
-0000df00: 6577 2e20 5468 6520 7061 7261 6d65 7465  ew. The paramete
-0000df10: 7273 206d 6179 2062 6520 6164 6a75 7374  rs may be adjust
-0000df20: 6564 2062 7920 7468 6520 756e 6465 726c  ed by the underl
-0000df30: 7969 6e67 207a 7374 6420 6c69 6272 6172  ying zstd librar
-0000df40: 7920 6166 7465 7220 6761 7468 6572 696e  y after gatherin
-0000df50: 6720 736f 6d65 2069 6e66 6f72 6d61 7469  g some informati
-0000df60: 6f6e 2c20 7375 6368 2061 7320 6461 7461  on, such as data
-0000df70: 2073 697a 652c 2075 7369 6e67 2064 6963   size, using dic
-0000df80: 7469 6f6e 6172 7920 6f72 206e 6f74 2e0a  tionary or not..
-0000df90: 0a20 2020 2053 6574 7469 6e67 2061 2063  .    Setting a c
-0000dfa0: 6f6d 7072 6573 7369 6f6e 206c 6576 656c  ompression level
-0000dfb0: 2064 6f65 7320 6e6f 7420 7365 7420 616c   does not set al
-0000dfc0: 6c20 6f74 6865 7220 3a72 6566 3a60 636f  l other :ref:`co
-0000dfd0: 6d70 7265 7373 696f 6e20 7061 7261 6d65  mpression parame
-0000dfe0: 7465 7273 3c43 5061 7261 6d65 7465 723e  ters<CParameter>
-0000dff0: 6020 746f 2064 6566 6175 6c74 2e20 5365  ` to default. Se
-0000e000: 7474 696e 6720 7468 6973 2077 696c 6c20  tting this will 
-0000e010: 6479 6e61 6d69 6361 6c6c 7920 696d 7061  dynamically impa
-0000e020: 6374 2074 6865 2063 6f6d 7072 6573 7369  ct the compressi
-0000e030: 6f6e 2070 6172 616d 6574 6572 7320 7768  on parameters wh
-0000e040: 6963 6820 6861 7665 206e 6f74 2062 6565  ich have not bee
-0000e050: 6e20 6d61 6e75 616c 6c79 2073 6574 2c20  n manually set, 
-0000e060: 7468 6520 6d61 6e75 616c 6c79 2073 6574  the manually set
-0000e070: 206f 6e65 7320 7769 6c6c 2022 7374 6963   ones will "stic
-0000e080: 6b22 2e0a 0a0a 4672 616d 6520 616e 6420  k"....Frame and 
-0000e090: 626c 6f63 6b0a 3e3e 3e3e 3e3e 3e3e 3e3e  block.>>>>>>>>>>
-0000e0a0: 3e3e 3e3e 3e0a 0a2e 2e20 5f66 7261 6d65  >>>>>.... _frame
-0000e0b0: 5f62 6c6f 636b 3a0a 0a2e 2e20 6e6f 7465  _block:.... note
-0000e0c0: 3a3a 2046 7261 6d65 2061 6e64 2062 6c6f  :: Frame and blo
-0000e0d0: 636b 0a0a 2020 2020 2a2a 4672 616d 652a  ck..    **Frame*
-0000e0e0: 2a0a 0a20 2020 205a 7374 6420 6461 7461  *..    Zstd data
-0000e0f0: 2063 6f6e 7369 7374 7320 6f66 206f 6e65   consists of one
-0000e100: 206f 7220 6d6f 7265 2069 6e64 6570 656e   or more indepen
-0000e110: 6465 6e74 2022 6672 616d 6573 222e 2054  dent "frames". T
-0000e120: 6865 2064 6563 6f6d 7072 6573 7365 6420  he decompressed 
-0000e130: 636f 6e74 656e 7420 6f66 206d 756c 7469  content of multi
-0000e140: 706c 6520 636f 6e63 6174 656e 6174 6564  ple concatenated
-0000e150: 2066 7261 6d65 7320 6973 2074 6865 2063   frames is the c
-0000e160: 6f6e 6361 7465 6e61 7469 6f6e 206f 6620  oncatenation of 
-0000e170: 6561 6368 2066 7261 6d65 2064 6563 6f6d  each frame decom
-0000e180: 7072 6573 7365 6420 636f 6e74 656e 742e  pressed content.
-0000e190: 0a0a 2020 2020 4120 6672 616d 6520 6973  ..    A frame is
-0000e1a0: 2063 6f6d 706c 6574 656c 7920 696e 6465   completely inde
-0000e1b0: 7065 6e64 656e 742c 2068 6173 2061 2066  pendent, has a f
-0000e1c0: 7261 6d65 2068 6561 6465 722c 2061 6e64  rame header, and
-0000e1d0: 2061 2073 6574 206f 6620 7061 7261 6d65   a set of parame
-0000e1e0: 7465 7273 2077 6869 6368 2074 656c 6c73  ters which tells
-0000e1f0: 2074 6865 2064 6563 6f64 6572 2068 6f77   the decoder how
-0000e200: 2074 6f20 6465 636f 6d70 7265 7373 2069   to decompress i
-0000e210: 742e 0a0a 2020 2020 496e 2061 6464 6974  t...    In addit
-0000e220: 696f 6e20 746f 206e 6f72 6d61 6c20 6672  ion to normal fr
-0000e230: 616d 652c 2074 6865 7265 2069 7320 6073  ame, there is `s
-0000e240: 6b69 7070 6162 6c65 2066 7261 6d65 203c  kippable frame <
-0000e250: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000e260: 6f6d 2f66 6163 6562 6f6f 6b2f 7a73 7464  om/facebook/zstd
-0000e270: 2f62 6c6f 622f 7265 6c65 6173 652f 646f  /blob/release/do
-0000e280: 632f 7a73 7464 5f63 6f6d 7072 6573 7369  c/zstd_compressi
-0000e290: 6f6e 5f66 6f72 6d61 742e 6d64 2373 6b69  on_format.md#ski
-0000e2a0: 7070 6162 6c65 2d66 7261 6d65 733e 605f  ppable-frames>`_
-0000e2b0: 2074 6861 7420 6361 6e20 636f 6e74 6169   that can contai
-0000e2c0: 6e20 616e 7920 7573 6572 2d64 6566 696e  n any user-defin
-0000e2d0: 6564 2064 6174 612c 2073 6b69 7070 6162  ed data, skippab
-0000e2e0: 6c65 2066 7261 6d65 2077 696c 6c20 6265  le frame will be
-0000e2f0: 2064 6563 6f6d 7072 6573 7365 6420 746f   decompressed to
-0000e300: 2060 6062 2727 6060 2e0a 0a20 2020 202a   ``b''``...    *
-0000e310: 2a42 6c6f 636b 2a2a 0a0a 2020 2020 4120  *Block**..    A 
-0000e320: 6672 616d 6520 656e 6361 7073 756c 6174  frame encapsulat
-0000e330: 6573 206f 6e65 206f 7220 6d75 6c74 6970  es one or multip
-0000e340: 6c65 2022 626c 6f63 6b73 222e 2042 6c6f  le "blocks". Blo
-0000e350: 636b 2068 6173 2061 2067 7561 7261 6e74  ck has a guarant
-0000e360: 6565 6420 6d61 7869 6d75 6d20 7369 7a65  eed maximum size
-0000e370: 2028 3320 6279 7465 7320 626c 6f63 6b20   (3 bytes block 
-0000e380: 6865 6164 6572 202b 2031 3238 204b 6942  header + 128 KiB
-0000e390: 292c 2074 6865 2061 6374 7561 6c20 6d61  ), the actual ma
-0000e3a0: 7869 6d75 6d20 7369 7a65 2064 6570 656e  ximum size depen
-0000e3b0: 6473 206f 6e20 6672 616d 6520 7061 7261  ds on frame para
-0000e3c0: 6d65 7465 7273 2e0a 0a20 2020 2055 6e6c  meters...    Unl
-0000e3d0: 696b 6520 696e 6465 7065 6e64 656e 7420  ike independent 
-0000e3e0: 6672 616d 6573 2c20 6561 6368 2062 6c6f  frames, each blo
-0000e3f0: 636b 2064 6570 656e 6473 206f 6e20 7072  ck depends on pr
-0000e400: 6576 696f 7573 2062 6c6f 636b 7320 666f  evious blocks fo
-0000e410: 7220 7072 6f70 6572 2064 6563 6f64 696e  r proper decodin
-0000e420: 672c 2062 7574 2064 6f65 736e 2774 206e  g, but doesn't n
-0000e430: 6565 6420 7468 6520 666f 6c6c 6f77 696e  eed the followin
-0000e440: 6720 626c 6f63 6b73 2c20 6120 636f 6d70  g blocks, a comp
-0000e450: 6c65 7465 2062 6c6f 636b 2063 616e 2062  lete block can b
-0000e460: 6520 6675 6c6c 7920 6465 636f 6d70 7265  e fully decompre
-0000e470: 7373 6564 2e20 536f 2066 6c75 7368 696e  ssed. So flushin
-0000e480: 6720 626c 6f63 6b20 6d61 7920 6265 2075  g block may be u
-0000e490: 7365 6420 696e 2063 6f6d 6d75 6e69 6361  sed in communica
-0000e4a0: 7469 6f6e 2073 6365 6e61 7269 6f73 2c20  tion scenarios, 
-0000e4b0: 7365 6520 3a70 793a 6174 7472 3a60 5a73  see :py:attr:`Zs
-0000e4c0: 7464 436f 6d70 7265 7373 6f72 2e46 4c55  tdCompressor.FLU
-0000e4d0: 5348 5f42 4c4f 434b 602e 0a0a 2020 2020  SH_BLOCK`...    
-0000e4e0: 2e2e 2061 7474 656e 7469 6f6e 3a3a 0a0a  .. attention::..
-0000e4f0: 2020 2020 2020 2020 496e 2073 6f6d 6520          In some 
-0000e500: 606c 616e 6775 6167 6520 6269 6e64 696e  `language bindin
-0000e510: 6773 203c 6874 7470 733a 2f2f 6661 6365  gs <https://face
-0000e520: 626f 6f6b 2e67 6974 6875 622e 696f 2f7a  book.github.io/z
-0000e530: 7374 642f 236f 7468 6572 2d6c 616e 6775  std/#other-langu
-0000e540: 6167 6573 3e60 5f2c 2064 6563 6f6d 7072  ages>`_, decompr
-0000e550: 6573 7328 2920 6675 6e63 7469 6f6e 2064  ess() function d
-0000e560: 6f65 736e 2774 2073 7570 706f 7274 206d  oesn't support m
-0000e570: 756c 7469 706c 6520 6672 616d 6573 2c20  ultiple frames, 
-0000e580: 6f72 2f61 6e64 2064 6f65 736e 2774 2073  or/and doesn't s
-0000e590: 7570 706f 7274 2061 2066 7261 6d65 2077  upport a frame w
-0000e5a0: 6974 6820 756e 6b6e 6f77 6e20 3a72 6566  ith unknown :ref
-0000e5b0: 3a60 636f 6e74 656e 7420 7369 7a65 3c63  :`content size<c
-0000e5c0: 6f6e 7465 6e74 5f73 697a 653e 602c 2070  ontent_size>`, p
-0000e5d0: 6179 2061 7474 656e 7469 6f6e 2077 6865  ay attention whe
-0000e5e0: 6e20 636f 6d70 7265 7373 696e 6720 6461  n compressing da
-0000e5f0: 7461 2066 6f72 206f 7468 6572 206c 616e  ta for other lan
-0000e600: 6775 6167 6520 6269 6e64 696e 6773 2e0a  guage bindings..
-0000e610: 0a0a 4d75 6c74 692d 7468 7265 6164 6564  ..Multi-threaded
-0000e620: 2063 6f6d 7072 6573 7369 6f6e 0a3e 3e3e   compression.>>>
-0000e630: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
-0000e640: 3e3e 3e3e 3e3e 3e0a 0a2e 2e20 5f6d 745f  >>>>>>>.... _mt_
-0000e650: 636f 6d70 7265 7373 696f 6e3a 0a0a 2e2e  compression:....
-0000e660: 206e 6f74 653a 3a20 4d75 6c74 692d 7468   note:: Multi-th
-0000e670: 7265 6164 6564 2063 6f6d 7072 6573 7369  readed compressi
-0000e680: 6f6e 0a0a 2020 2020 5a73 7464 206c 6962  on..    Zstd lib
-0000e690: 7261 7279 2073 7570 706f 7274 7320 6d75  rary supports mu
-0000e6a0: 6c74 692d 7468 7265 6164 6564 2063 6f6d  lti-threaded com
-0000e6b0: 7072 6573 7369 6f6e 2e20 5365 7420 3a70  pression. Set :p
-0000e6c0: 793a 6174 7472 3a60 4350 6172 616d 6574  y:attr:`CParamet
-0000e6d0: 6572 2e6e 6257 6f72 6b65 7273 6020 7061  er.nbWorkers` pa
-0000e6e0: 7261 6d65 7465 7220 3e3d 2060 6031 6060  rameter >= ``1``
-0000e6f0: 2074 6f20 656e 6162 6c65 206d 756c 7469   to enable multi
-0000e700: 2d74 6872 6561 6465 6420 636f 6d70 7265  -threaded compre
-0000e710: 7373 696f 6e2c 2060 6031 6060 206d 6561  ssion, ``1`` mea
-0000e720: 6e73 2022 312d 7468 7265 6164 206d 756c  ns "1-thread mul
-0000e730: 7469 2d74 6872 6561 6465 6420 6d6f 6465  ti-threaded mode
-0000e740: 222e 0a0a 2020 2020 5468 6520 7468 7265  "...    The thre
-0000e750: 6164 7320 6172 6520 7370 6177 6e65 6420  ads are spawned 
-0000e760: 6279 2074 6865 2075 6e64 6572 6c79 696e  by the underlyin
-0000e770: 6720 7a73 7464 206c 6962 7261 7279 2c20  g zstd library, 
-0000e780: 6e6f 7420 6279 2070 797a 7374 6420 6d6f  not by pyzstd mo
-0000e790: 6475 6c65 2e0a 0a20 2020 202e 2e20 736f  dule...    .. so
-0000e7a0: 7572 6365 636f 6465 3a3a 2070 7974 686f  urcecode:: pytho
-0000e7b0: 6e0a 0a20 2020 2020 2020 2023 2075 7365  n..        # use
-0000e7c0: 2034 2074 6872 6561 6473 2074 6f20 636f   4 threads to co
-0000e7d0: 6d70 7265 7373 0a20 2020 2020 2020 206f  mpress.        o
+00000220: 6060 2e0a 0a4c 696e 6b73 3a20 6047 6974  ``...Links: `Git
+00000230: 4875 6220 7061 6765 203c 6874 7470 733a  Hub page <https:
+00000240: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6e69  //github.com/ani
+00000250: 6d61 6c69 7a65 2f70 797a 7374 643e 605f  malize/pyzstd>`_
+00000260: 2c20 6050 7950 4920 7061 6765 203c 6874  , `PyPI page <ht
+00000270: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000280: 726f 6a65 6374 2f70 797a 7374 643e 605f  roject/pyzstd>`_
+00000290: 2e0a 0a46 6561 7475 7265 7320 6f66 207a  ...Features of z
+000002a0: 7374 643a 0a0a 2a20 4661 7374 2063 6f6d  std:..* Fast com
+000002b0: 7072 6573 7369 6f6e 2061 6e64 2064 6563  pression and dec
+000002c0: 6f6d 7072 6573 7369 6f6e 2073 7065 6564  ompression speed
+000002d0: 2e0a 2a20 4966 2075 7365 203a 7265 663a  ..* If use :ref:
+000002e0: 606d 756c 7469 2d74 6872 6561 6465 6420  `multi-threaded 
+000002f0: 636f 6d70 7265 7373 696f 6e3c 6d74 5f63  compression<mt_c
+00000300: 6f6d 7072 6573 7369 6f6e 3e60 2c20 7468  ompression>`, th
+00000310: 6520 636f 6d70 7265 7373 696f 6e20 7370  e compression sp
+00000320: 6565 6420 696d 7072 6f76 6573 2073 6967  eed improves sig
+00000330: 6e69 6669 6361 6e74 6c79 2e0a 2a20 4966  nificantly..* If
+00000340: 2075 7365 2070 7265 2d74 7261 696e 6564   use pre-trained
+00000350: 203a 7265 663a 6064 6963 7469 6f6e 6172   :ref:`dictionar
+00000360: 793c 7a73 7464 5f64 6963 743e 602c 2074  y<zstd_dict>`, t
+00000370: 6865 2063 6f6d 7072 6573 7369 6f6e 2072  he compression r
+00000380: 6174 696f 206f 6e20 736d 616c 6c20 6461  atio on small da
+00000390: 7461 2028 6120 6665 7720 4b69 4229 2069  ta (a few KiB) i
+000003a0: 6d70 726f 7665 7320 6472 616d 6174 6963  mproves dramatic
+000003b0: 616c 6c79 2e0a 2a20 3a72 6566 3a60 4672  ally..* :ref:`Fr
+000003c0: 616d 6520 616e 6420 626c 6f63 6b3c 6672  ame and block<fr
+000003d0: 616d 655f 626c 6f63 6b3e 6020 616c 6c6f  ame_block>` allo
+000003e0: 7720 7468 6520 7573 6520 6d6f 7265 2066  w the use more f
+000003f0: 6c65 7869 626c 652c 2073 7569 7461 626c  lexible, suitabl
+00000400: 6520 666f 7220 6d61 6e79 2073 6365 6e61  e for many scena
+00000410: 7269 6f73 2e0a 2a20 4361 6e20 6265 2075  rios..* Can be u
+00000420: 7365 6420 6173 2061 203a 7265 663a 6070  sed as a :ref:`p
+00000430: 6174 6368 696e 6720 656e 6769 6e65 3c70  atching engine<p
+00000440: 6174 6368 696e 675f 656e 6769 6e65 3e60  atching_engine>`
+00000450: 2e0a 0a2e 2e20 6e6f 7465 3a3a 0a20 2020  ..... note::.   
+00000460: 2054 776f 206f 7468 6572 207a 7374 6420   Two other zstd 
+00000470: 6d6f 6475 6c65 7320 6f6e 2050 7950 493a  modules on PyPI:
+00000480: 0a0a 2020 2020 2a20 607a 7374 6420 3c68  ..    * `zstd <h
+00000490: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000004a0: 7072 6f6a 6563 742f 7a73 7464 2f3e 605f  project/zstd/>`_
+000004b0: 2c20 6120 7665 7279 2073 696d 706c 6520  , a very simple 
+000004c0: 6d6f 6475 6c65 2e0a 2020 2020 2a20 607a  module..    * `z
+000004d0: 7374 616e 6461 7264 203c 6874 7470 733a  standard <https:
+000004e0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+000004f0: 6374 2f7a 7374 616e 6461 7264 2f3e 605f  ct/zstandard/>`_
+00000500: 2c20 7072 6f76 6964 6573 2072 6963 6820  , provides rich 
+00000510: 4150 492e 0a0a 4578 6365 7074 696f 6e0a  API...Exception.
+00000520: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 7079  ---------.... py
+00000530: 3a65 7863 6570 7469 6f6e 3a3a 205a 7374  :exception:: Zst
+00000540: 6445 7272 6f72 0a0a 2020 2020 5468 6973  dError..    This
+00000550: 2065 7863 6570 7469 6f6e 2069 7320 7261   exception is ra
+00000560: 6973 6564 2077 6865 6e20 616e 2065 7272  ised when an err
+00000570: 6f72 206f 6363 7572 7320 7768 656e 2063  or occurs when c
+00000580: 616c 6c69 6e67 2074 6865 2075 6e64 6572  alling the under
+00000590: 6c79 696e 6720 7a73 7464 206c 6962 7261  lying zstd libra
+000005a0: 7279 2e0a 0a0a 5369 6d70 6c65 2063 6f6d  ry....Simple com
+000005b0: 7072 6573 7369 6f6e 2f64 6563 6f6d 7072  pression/decompr
+000005c0: 6573 7369 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d  ession.---------
+000005d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000005e0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2054 6869  -------..    Thi
+000005f0: 7320 7365 6374 696f 6e20 636f 6e74 6169  s section contai
+00000600: 6e73 3a0a 0a20 2020 2020 2020 202a 2066  ns:..        * f
+00000610: 756e 6374 696f 6e20 3a70 793a 6675 6e63  unction :py:func
+00000620: 3a60 636f 6d70 7265 7373 600a 2020 2020  :`compress`.    
+00000630: 2020 2020 2a20 6675 6e63 7469 6f6e 203a      * function :
+00000640: 7079 3a66 756e 633a 6064 6563 6f6d 7072  py:func:`decompr
+00000650: 6573 7360 0a0a 2020 2020 2e2e 2068 696e  ess`..    .. hin
+00000660: 743a 3a0a 2020 2020 2020 2020 4966 2074  t::.        If t
+00000670: 6865 7265 2061 7265 2061 2062 6967 206e  here are a big n
+00000680: 756d 6265 7220 6f66 2073 616d 6520 7479  umber of same ty
+00000690: 7065 2069 6e64 6976 6964 7561 6c20 6461  pe individual da
+000006a0: 7461 2c20 7265 7573 6520 7468 6573 6520  ta, reuse these 
+000006b0: 6f62 6a65 6374 7320 6d61 7920 656c 696d  objects may elim
+000006c0: 696e 6174 6520 7468 6520 736d 616c 6c20  inate the small 
+000006d0: 6f76 6572 6865 6164 206f 6620 6372 6561  overhead of crea
+000006e0: 7469 6e67 2063 6f6e 7465 7874 202f 2073  ting context / s
+000006f0: 6574 7469 6e67 2070 6172 616d 6574 6572  etting parameter
+00000700: 7320 2f20 6c6f 6164 696e 6720 6469 6374  s / loading dict
+00000710: 696f 6e61 7279 2e0a 0a20 2020 2020 2020  ionary...       
+00000720: 202a 203a 7079 3a63 6c61 7373 3a60 5a73   * :py:class:`Zs
+00000730: 7464 436f 6d70 7265 7373 6f72 600a 2020  tdCompressor`.  
+00000740: 2020 2020 2020 2a20 3a70 793a 636c 6173        * :py:clas
+00000750: 733a 6052 6963 684d 656d 5a73 7464 436f  s:`RichMemZstdCo
+00000760: 6d70 7265 7373 6f72 600a 0a0a 2e2e 2070  mpressor`..... p
+00000770: 793a 6675 6e63 7469 6f6e 3a3a 2063 6f6d  y:function:: com
+00000780: 7072 6573 7328 6461 7461 2c20 6c65 7665  press(data, leve
+00000790: 6c5f 6f72 5f6f 7074 696f 6e3d 4e6f 6e65  l_or_option=None
+000007a0: 2c20 7a73 7464 5f64 6963 743d 4e6f 6e65  , zstd_dict=None
+000007b0: 290a 0a20 2020 2043 6f6d 7072 6573 7320  )..    Compress 
+000007c0: 2a64 6174 612a 2c20 7265 7475 726e 2074  *data*, return t
+000007d0: 6865 2063 6f6d 7072 6573 7365 6420 6461  he compressed da
+000007e0: 7461 2e0a 0a20 2020 2043 6f6d 7072 6573  ta...    Compres
+000007f0: 7369 6e67 2060 6062 2727 6060 2077 696c  sing ``b''`` wil
+00000800: 6c20 6765 7420 616e 2065 6d70 7479 2063  l get an empty c
+00000810: 6f6e 7465 6e74 2066 7261 6d65 2028 3920  ontent frame (9 
+00000820: 6279 7465 7320 6f72 206d 6f72 6529 2e0a  bytes or more)..
+00000830: 0a20 2020 203a 7079 3a66 756e 633a 6072  .    :py:func:`r
+00000840: 6963 686d 656d 5f63 6f6d 7072 6573 7360  ichmem_compress`
+00000850: 2066 756e 6374 696f 6e20 6973 2066 6173   function is fas
+00000860: 7465 7220 696e 2073 6f6d 6520 6361 7365  ter in some case
+00000870: 732e 0a0a 2020 2020 3a70 6172 616d 2064  s...    :param d
+00000880: 6174 613a 2044 6174 6120 746f 2062 6520  ata: Data to be 
+00000890: 636f 6d70 7265 7373 6564 2e0a 2020 2020  compressed..    
+000008a0: 3a74 7970 6520 6461 7461 3a20 6279 7465  :type data: byte
+000008b0: 732d 6c69 6b65 206f 626a 6563 740a 2020  s-like object.  
+000008c0: 2020 3a70 6172 616d 206c 6576 656c 5f6f    :param level_o
+000008d0: 725f 6f70 7469 6f6e 3a20 5768 656e 2069  r_option: When i
+000008e0: 7427 7320 616e 2060 6069 6e74 6060 206f  t's an ``int`` o
+000008f0: 626a 6563 742c 2069 7420 7265 7072 6573  bject, it repres
+00000900: 656e 7473 203a 7265 663a 6063 6f6d 7072  ents :ref:`compr
+00000910: 6573 7369 6f6e 206c 6576 656c 3c63 6f6d  ession level<com
+00000920: 7072 6573 7369 6f6e 5f6c 6576 656c 3e60  pression_level>`
+00000930: 2e20 5768 656e 2069 7427 7320 6120 6060  . When it's a ``
+00000940: 6469 6374 6060 206f 626a 6563 742c 2069  dict`` object, i
+00000950: 7420 636f 6e74 6169 6e73 203a 7265 663a  t contains :ref:
+00000960: 6061 6476 616e 6365 6420 636f 6d70 7265  `advanced compre
+00000970: 7373 696f 6e20 7061 7261 6d65 7465 7273  ssion parameters
+00000980: 3c43 5061 7261 6d65 7465 723e 602e 2054  <CParameter>`. T
+00000990: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
+000009a0: 2060 604e 6f6e 6560 6020 6d65 616e 7320   ``None`` means 
+000009b0: 746f 2075 7365 207a 7374 6427 7320 6465  to use zstd's de
+000009c0: 6661 756c 7420 636f 6d70 7265 7373 696f  fault compressio
+000009d0: 6e20 6c65 7665 6c2f 7061 7261 6d65 7465  n level/paramete
+000009e0: 7273 2e0a 2020 2020 3a74 7970 6520 6c65  rs..    :type le
+000009f0: 7665 6c5f 6f72 5f6f 7074 696f 6e3a 2069  vel_or_option: i
+00000a00: 6e74 206f 7220 6469 6374 0a20 2020 203a  nt or dict.    :
+00000a10: 7061 7261 6d20 7a73 7464 5f64 6963 743a  param zstd_dict:
+00000a20: 2050 7265 2d74 7261 696e 6564 2064 6963   Pre-trained dic
+00000a30: 7469 6f6e 6172 7920 666f 7220 636f 6d70  tionary for comp
+00000a40: 7265 7373 696f 6e2e 0a20 2020 203a 7479  ression..    :ty
+00000a50: 7065 207a 7374 645f 6469 6374 3a20 5a73  pe zstd_dict: Zs
+00000a60: 7464 4469 6374 0a20 2020 203a 7265 7475  tdDict.    :retu
+00000a70: 726e 3a20 436f 6d70 7265 7373 6564 2064  rn: Compressed d
+00000a80: 6174 610a 2020 2020 3a72 7479 7065 3a20  ata.    :rtype: 
+00000a90: 6279 7465 730a 0a2e 2e20 736f 7572 6365  bytes.... source
+00000aa0: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
+00000ab0: 2020 2023 2069 6e74 2063 6f6d 7072 6573     # int compres
+00000ac0: 7369 6f6e 206c 6576 656c 0a20 2020 2063  sion level.    c
+00000ad0: 6f6d 7072 6573 7365 645f 6461 7420 3d20  ompressed_dat = 
+00000ae0: 636f 6d70 7265 7373 2872 6177 5f64 6174  compress(raw_dat
+00000af0: 2c20 3130 290a 0a20 2020 2023 2064 6963  , 10)..    # dic
+00000b00: 7420 6f70 7469 6f6e 2c20 7573 6520 3620  t option, use 6 
+00000b10: 7468 7265 6164 7320 746f 2063 6f6d 7072  threads to compr
+00000b20: 6573 732c 2061 6e64 2061 7070 656e 6420  ess, and append 
+00000b30: 6120 342d 6279 7465 2063 6865 636b 7375  a 4-byte checksu
+00000b40: 6d2e 0a20 2020 206f 7074 696f 6e20 3d20  m..    option = 
+00000b50: 7b43 5061 7261 6d65 7465 722e 636f 6d70  {CParameter.comp
+00000b60: 7265 7373 696f 6e4c 6576 656c 203a 2031  ressionLevel : 1
+00000b70: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00000b80: 2043 5061 7261 6d65 7465 722e 6e62 576f   CParameter.nbWo
+00000b90: 726b 6572 7320 3a20 362c 0a20 2020 2020  rkers : 6,.     
+00000ba0: 2020 2020 2020 2020 2043 5061 7261 6d65           CParame
+00000bb0: 7465 722e 6368 6563 6b73 756d 466c 6167  ter.checksumFlag
+00000bc0: 203a 2031 7d0a 2020 2020 636f 6d70 7265   : 1}.    compre
+00000bd0: 7373 6564 5f64 6174 203d 2063 6f6d 7072  ssed_dat = compr
+00000be0: 6573 7328 7261 775f 6461 742c 206f 7074  ess(raw_dat, opt
+00000bf0: 696f 6e29 0a0a 0a2e 2e20 7079 3a66 756e  ion)..... py:fun
+00000c00: 6374 696f 6e3a 3a20 6465 636f 6d70 7265  ction:: decompre
+00000c10: 7373 2864 6174 612c 207a 7374 645f 6469  ss(data, zstd_di
+00000c20: 6374 3d4e 6f6e 652c 206f 7074 696f 6e3d  ct=None, option=
+00000c30: 4e6f 6e65 290a 0a20 2020 2044 6563 6f6d  None)..    Decom
+00000c40: 7072 6573 7320 2a64 6174 612a 2c20 7265  press *data*, re
+00000c50: 7475 726e 2074 6865 2064 6563 6f6d 7072  turn the decompr
+00000c60: 6573 7365 6420 6461 7461 2e0a 0a20 2020  essed data...   
+00000c70: 2053 7570 706f 7274 206d 756c 7469 706c   Support multipl
+00000c80: 6520 636f 6e63 6174 656e 6174 6564 203a  e concatenated :
+00000c90: 7265 663a 6066 7261 6d65 733c 6672 616d  ref:`frames<fram
+00000ca0: 655f 626c 6f63 6b3e 602e 0a0a 2020 2020  e_block>`...    
+00000cb0: 3a70 6172 616d 2064 6174 613a 2044 6174  :param data: Dat
+00000cc0: 6120 746f 2062 6520 6465 636f 6d70 7265  a to be decompre
+00000cd0: 7373 6564 2e0a 2020 2020 3a74 7970 6520  ssed..    :type 
+00000ce0: 6461 7461 3a20 6279 7465 732d 6c69 6b65  data: bytes-like
+00000cf0: 206f 626a 6563 740a 2020 2020 3a70 6172   object.    :par
+00000d00: 616d 207a 7374 645f 6469 6374 3a20 5072  am zstd_dict: Pr
+00000d10: 652d 7472 6169 6e65 6420 6469 6374 696f  e-trained dictio
+00000d20: 6e61 7279 2066 6f72 2064 6563 6f6d 7072  nary for decompr
+00000d30: 6573 7369 6f6e 2e0a 2020 2020 3a74 7970  ession..    :typ
+00000d40: 6520 7a73 7464 5f64 6963 743a 205a 7374  e zstd_dict: Zst
+00000d50: 6444 6963 740a 2020 2020 3a70 6172 616d  dDict.    :param
+00000d60: 206f 7074 696f 6e3a 2041 2060 6064 6963   option: A ``dic
+00000d70: 7460 6020 6f62 6a65 6374 2074 6861 7420  t`` object that 
+00000d80: 636f 6e74 6169 6e73 203a 7079 3a72 6566  contains :py:ref
+00000d90: 3a60 6164 7661 6e63 6564 2064 6563 6f6d  :`advanced decom
+00000da0: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
+00000db0: 6572 733c 4450 6172 616d 6574 6572 3e60  ers<DParameter>`
+00000dc0: 2e20 5468 6520 6465 6661 756c 7420 7661  . The default va
+00000dd0: 6c75 6520 6060 4e6f 6e65 6060 206d 6561  lue ``None`` mea
+00000de0: 6e73 2074 6f20 7573 6520 7a73 7464 2773  ns to use zstd's
+00000df0: 2064 6566 6175 6c74 2064 6563 6f6d 7072   default decompr
+00000e00: 6573 7369 6f6e 2070 6172 616d 6574 6572  ession parameter
+00000e10: 732e 0a20 2020 203a 7479 7065 206f 7074  s..    :type opt
+00000e20: 696f 6e3a 2064 6963 740a 2020 2020 3a72  ion: dict.    :r
+00000e30: 6574 7572 6e3a 2044 6563 6f6d 7072 6573  eturn: Decompres
+00000e40: 7365 6420 6461 7461 0a20 2020 203a 7274  sed data.    :rt
+00000e50: 7970 653a 2062 7974 6573 0a20 2020 203a  ype: bytes.    :
+00000e60: 7261 6973 6573 205a 7374 6445 7272 6f72  raises ZstdError
+00000e70: 3a20 4966 2064 6563 6f6d 7072 6573 7369  : If decompressi
+00000e80: 6f6e 2066 6169 6c73 2e0a 0a0a 5269 6368  on fails....Rich
+00000e90: 206d 656d 6f72 7920 636f 6d70 7265 7373   memory compress
+00000ea0: 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ion.------------
+00000eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020  -----------..   
+00000ec0: 2043 6f6d 7072 6573 7320 6461 7461 2075   Compress data u
+00000ed0: 7369 6e67 203a 7265 663a 6072 6963 6820  sing :ref:`rich 
+00000ee0: 6d65 6d6f 7279 206d 6f64 653c 7269 6368  memory mode<rich
+00000ef0: 5f6d 656d 3e60 2e20 5468 6973 206d 6f64  _mem>`. This mod
+00000f00: 6520 616c 6c6f 6361 7465 7320 6d6f 7265  e allocates more
+00000f10: 206d 656d 6f72 7920 666f 7220 6f75 7470   memory for outp
+00000f20: 7574 2062 7566 6665 722c 2069 7427 7320  ut buffer, it's 
+00000f30: 6661 7374 6572 2069 6e20 736f 6d65 2063  faster in some c
+00000f40: 6173 6573 2e0a 0a20 2020 2054 6869 7320  ases...    This 
+00000f50: 7365 6374 696f 6e20 636f 6e74 6169 6e73  section contains
+00000f60: 3a0a 0a20 2020 2020 2020 202a 2066 756e  :..        * fun
+00000f70: 6374 696f 6e20 3a70 793a 6675 6e63 3a60  ction :py:func:`
+00000f80: 7269 6368 6d65 6d5f 636f 6d70 7265 7373  richmem_compress
+00000f90: 600a 2020 2020 2020 2020 2a20 636c 6173  `.        * clas
+00000fa0: 7320 3a70 793a 636c 6173 733a 6052 6963  s :py:class:`Ric
+00000fb0: 684d 656d 5a73 7464 436f 6d70 7265 7373  hMemZstdCompress
+00000fc0: 6f72 602c 2061 2072 6575 7361 626c 6520  or`, a reusable 
+00000fd0: 636f 6d70 7265 7373 6f72 2e0a 0a2e 2e20  compressor..... 
+00000fe0: 7079 3a66 756e 6374 696f 6e3a 3a20 7269  py:function:: ri
+00000ff0: 6368 6d65 6d5f 636f 6d70 7265 7373 2864  chmem_compress(d
+00001000: 6174 612c 206c 6576 656c 5f6f 725f 6f70  ata, level_or_op
+00001010: 7469 6f6e 3d4e 6f6e 652c 207a 7374 645f  tion=None, zstd_
+00001020: 6469 6374 3d4e 6f6e 6529 0a0a 2020 2020  dict=None)..    
+00001030: 5573 6520 3a72 6566 3a60 7269 6368 206d  Use :ref:`rich m
+00001040: 656d 6f72 7920 6d6f 6465 3c72 6963 685f  emory mode<rich_
+00001050: 6d65 6d3e 6020 746f 2063 6f6d 7072 6573  mem>` to compres
+00001060: 7320 2a64 6174 612a 2e20 4974 2773 2066  s *data*. It's f
+00001070: 6173 7465 7220 7468 616e 203a 7079 3a66  aster than :py:f
+00001080: 756e 633a 6063 6f6d 7072 6573 7360 2069  unc:`compress` i
+00001090: 6e20 736f 6d65 2063 6173 6573 2c20 6275  n some cases, bu
+000010a0: 7420 616c 6c6f 6361 7465 7320 6d6f 7265  t allocates more
+000010b0: 206d 656d 6f72 792e 0a0a 2020 2020 5468   memory...    Th
+000010c0: 6520 7061 7261 6d65 7465 7273 2061 7265  e parameters are
+000010d0: 2074 6865 2073 616d 6520 6173 203a 7079   the same as :py
+000010e0: 3a66 756e 633a 6063 6f6d 7072 6573 7360  :func:`compress`
+000010f0: 2066 756e 6374 696f 6e2e 0a0a 2020 2020   function...    
+00001100: 436f 6d70 7265 7373 696e 6720 6060 6227  Compressing ``b'
+00001110: 2760 6020 7769 6c6c 2067 6574 2061 6e20  '`` will get an 
+00001120: 656d 7074 7920 636f 6e74 656e 7420 6672  empty content fr
+00001130: 616d 6520 2839 2062 7974 6573 206f 7220  ame (9 bytes or 
+00001140: 6d6f 7265 292e 0a0a 0a2e 2e20 7079 3a63  more)...... py:c
+00001150: 6c61 7373 3a3a 2052 6963 684d 656d 5a73  lass:: RichMemZs
+00001160: 7464 436f 6d70 7265 7373 6f72 0a0a 2020  tdCompressor..  
+00001170: 2020 4120 7265 7573 6162 6c65 2063 6f6d    A reusable com
+00001180: 7072 6573 736f 7220 7573 696e 6720 3a72  pressor using :r
+00001190: 6566 3a60 7269 6368 206d 656d 6f72 7920  ef:`rich memory 
+000011a0: 6d6f 6465 3c72 6963 685f 6d65 6d3e 602e  mode<rich_mem>`.
+000011b0: 2049 7420 6361 6e20 6265 2072 6575 7365   It can be reuse
+000011c0: 6420 666f 7220 6269 6720 6e75 6d62 6572  d for big number
+000011d0: 206f 6620 7361 6d65 2074 7970 6520 696e   of same type in
+000011e0: 6469 7669 6475 616c 2064 6174 612e 0a0a  dividual data...
+000011f0: 2020 2020 5369 6e63 6520 6974 2063 616e      Since it can
+00001200: 206f 6e6c 7920 6765 6e65 7261 7465 7320   only generates 
+00001210: 696e 6469 7669 6475 616c 203a 7265 663a  individual :ref:
+00001220: 6066 7261 6d65 733c 6672 616d 655f 626c  `frames<frame_bl
+00001230: 6f63 6b3e 602c 2069 7427 7320 6e6f 7420  ock>`, it's not 
+00001240: 7375 6974 6162 6c65 2066 6f72 2073 7472  suitable for str
+00001250: 6561 6d69 6e67 2063 6f6d 7072 6573 7369  eaming compressi
+00001260: 6f6e 2c20 6f74 6865 7277 6973 6520 7468  on, otherwise th
+00001270: 6520 636f 6d70 7265 7373 696f 6e20 7261  e compression ra
+00001280: 7469 6f20 7769 6c6c 2062 6520 7265 6475  tio will be redu
+00001290: 6365 642c 2061 6e64 2073 6f6d 6520 7072  ced, and some pr
+000012a0: 6f67 7261 6d73 2063 616e 2774 2064 6563  ograms can't dec
+000012b0: 6f6d 7072 6573 7320 6d75 6c74 6970 6c65  ompress multiple
+000012c0: 2066 7261 6d65 7320 6461 7461 2e20 466f   frames data. Fo
+000012d0: 7220 7374 7265 616d 696e 6720 636f 6d70  r streaming comp
+000012e0: 7265 7373 696f 6e2c 2073 6565 203a 7265  ression, see :re
+000012f0: 663a 6074 6869 7320 7365 6374 696f 6e3c  f:`this section<
+00001300: 7374 7265 616d 5f63 6f6d 7072 6573 7369  stream_compressi
+00001310: 6f6e 3e60 2e0a 0a20 2020 2054 6872 6561  on>`...    Threa
+00001320: 642d 7361 6665 2061 7420 6d65 7468 6f64  d-safe at method
+00001330: 206c 6576 656c 2e0a 0a20 2020 202e 2e20   level...    .. 
+00001340: 7079 3a6d 6574 686f 643a 3a20 5f5f 696e  py:method:: __in
+00001350: 6974 5f5f 2873 656c 662c 206c 6576 656c  it__(self, level
+00001360: 5f6f 725f 6f70 7469 6f6e 3d4e 6f6e 652c  _or_option=None,
+00001370: 207a 7374 645f 6469 6374 3d4e 6f6e 6529   zstd_dict=None)
+00001380: 0a0a 2020 2020 2020 2020 5468 6520 7061  ..        The pa
+00001390: 7261 6d65 7465 7273 2061 7265 2074 6865  rameters are the
+000013a0: 2073 616d 6520 6173 203a 7079 3a6d 6574   same as :py:met
+000013b0: 683a 605a 7374 6443 6f6d 7072 6573 736f  h:`ZstdCompresso
+000013c0: 722e 5f5f 696e 6974 5f5f 6020 6d65 7468  r.__init__` meth
+000013d0: 6f64 2e0a 0a20 2020 202e 2e20 7079 3a6d  od...    .. py:m
+000013e0: 6574 686f 643a 3a20 636f 6d70 7265 7373  ethod:: compress
+000013f0: 2873 656c 662c 2064 6174 6129 0a0a 2020  (self, data)..  
+00001400: 2020 2020 2020 436f 6d70 7265 7373 202a        Compress *
+00001410: 6461 7461 2a20 7573 696e 6720 3a72 6566  data* using :ref
+00001420: 3a60 7269 6368 206d 656d 6f72 7920 6d6f  :`rich memory mo
+00001430: 6465 3c72 6963 685f 6d65 6d3e 602c 2072  de<rich_mem>`, r
+00001440: 6574 7572 6e20 6120 7369 6e67 6c65 207a  eturn a single z
+00001450: 7374 6420 3a72 6566 3a60 6672 616d 653c  std :ref:`frame<
+00001460: 6672 616d 655f 626c 6f63 6b3e 602e 0a0a  frame_block>`...
+00001470: 2020 2020 2020 2020 436f 6d70 7265 7373          Compress
+00001480: 696e 6720 6060 6227 2760 6020 7769 6c6c  ing ``b''`` will
+00001490: 2067 6574 2061 6e20 656d 7074 7920 636f   get an empty co
+000014a0: 6e74 656e 7420 6672 616d 6520 2839 2062  ntent frame (9 b
+000014b0: 7974 6573 206f 7220 6d6f 7265 292e 0a0a  ytes or more)...
+000014c0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+000014d0: 6174 613a 2044 6174 6120 746f 2062 6520  ata: Data to be 
+000014e0: 636f 6d70 7265 7373 6564 2e0a 2020 2020  compressed..    
+000014f0: 2020 2020 3a74 7970 6520 6461 7461 3a20      :type data: 
+00001500: 6279 7465 732d 6c69 6b65 206f 626a 6563  bytes-like objec
+00001510: 740a 2020 2020 2020 2020 3a72 6574 7572  t.        :retur
+00001520: 6e3a 2041 2073 696e 676c 6520 7a73 7464  n: A single zstd
+00001530: 2066 7261 6d65 2e0a 2020 2020 2020 2020   frame..        
+00001540: 3a72 7479 7065 3a20 6279 7465 730a 0a20  :rtype: bytes.. 
+00001550: 2020 202e 2e20 736f 7572 6365 636f 6465     .. sourcecode
+00001560: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+00001570: 2020 2063 203d 2052 6963 684d 656d 5a73     c = RichMemZs
+00001580: 7464 436f 6d70 7265 7373 6f72 2829 0a20  tdCompressor(). 
+00001590: 2020 2020 2020 2066 7261 6d65 3120 3d20         frame1 = 
+000015a0: 632e 636f 6d70 7265 7373 2872 6177 5f64  c.compress(raw_d
+000015b0: 6174 3129 0a20 2020 2020 2020 2066 7261  at1).        fra
+000015c0: 6d65 3220 3d20 632e 636f 6d70 7265 7373  me2 = c.compress
+000015d0: 2872 6177 5f64 6174 3229 0a0a 0a2e 2e20  (raw_dat2)..... 
+000015e0: 5f73 7472 6561 6d5f 636f 6d70 7265 7373  _stream_compress
+000015f0: 696f 6e3a 0a0a 5374 7265 616d 696e 6720  ion:..Streaming 
+00001600: 636f 6d70 7265 7373 696f 6e0a 2d2d 2d2d  compression.----
+00001610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001620: 2d0a 0a20 2020 2054 6869 7320 7365 6374  -..    This sect
+00001630: 696f 6e20 636f 6e74 6169 6e73 3a0a 0a20  ion contains:.. 
+00001640: 2020 2020 2020 202a 2066 756e 6374 696f         * functio
+00001650: 6e20 3a70 793a 6675 6e63 3a60 636f 6d70  n :py:func:`comp
+00001660: 7265 7373 5f73 7472 6561 6d60 2c20 6120  ress_stream`, a 
+00001670: 6661 7374 2061 6e64 2063 6f6e 7665 6e69  fast and conveni
+00001680: 656e 7420 6675 6e63 7469 6f6e 2e0a 2020  ent function..  
+00001690: 2020 2020 2020 2a20 636c 6173 7320 3a70        * class :p
+000016a0: 793a 636c 6173 733a 605a 7374 6443 6f6d  y:class:`ZstdCom
+000016b0: 7072 6573 736f 7260 2c20 7369 6d69 6c61  pressor`, simila
+000016c0: 7220 746f 2063 6f6d 7072 6573 736f 7273  r to compressors
+000016d0: 2069 6e20 5079 7468 6f6e 2073 7461 6e64   in Python stand
+000016e0: 6172 6420 6c69 6272 6172 792e 0a0a 2020  ard library...  
+000016f0: 2020 4974 2077 6f75 6c64 2062 6520 6e69    It would be ni
+00001700: 6365 2074 6f20 6b6e 6f77 2073 6f6d 6520  ce to know some 
+00001710: 6b6e 6f77 6c65 6467 6520 6162 6f75 7420  knowledge about 
+00001720: 7a73 7464 2064 6174 612c 2073 6565 203a  zstd data, see :
+00001730: 7265 663a 6066 7261 6d65 2061 6e64 2062  ref:`frame and b
+00001740: 6c6f 636b 3c66 7261 6d65 5f62 6c6f 636b  lock<frame_block
+00001750: 3e60 2e0a 0a2e 2e20 7079 3a66 756e 6374  >`..... py:funct
+00001760: 696f 6e3a 3a20 636f 6d70 7265 7373 5f73  ion:: compress_s
+00001770: 7472 6561 6d28 696e 7075 745f 7374 7265  tream(input_stre
+00001780: 616d 2c20 6f75 7470 7574 5f73 7472 6561  am, output_strea
+00001790: 6d2c 202a 2c20 6c65 7665 6c5f 6f72 5f6f  m, *, level_or_o
+000017a0: 7074 696f 6e3d 4e6f 6e65 2c20 7a73 7464  ption=None, zstd
+000017b0: 5f64 6963 743d 4e6f 6e65 2c20 706c 6564  _dict=None, pled
+000017c0: 6765 645f 696e 7075 745f 7369 7a65 3d4e  ged_input_size=N
+000017d0: 6f6e 652c 2072 6561 645f 7369 7a65 3d31  one, read_size=1
+000017e0: 3331 5f30 3732 2c20 7772 6974 655f 7369  31_072, write_si
+000017f0: 7a65 3d31 3331 5f35 3931 2c20 6361 6c6c  ze=131_591, call
+00001800: 6261 636b 3d4e 6f6e 6529 0a0a 2020 2020  back=None)..    
+00001810: 4120 6661 7374 2061 6e64 2063 6f6e 7665  A fast and conve
+00001820: 6e69 656e 7420 6675 6e63 7469 6f6e 2c20  nient function, 
+00001830: 636f 6d70 7265 7373 6573 202a 696e 7075  compresses *inpu
+00001840: 745f 7374 7265 616d 2a20 616e 6420 7772  t_stream* and wr
+00001850: 6974 6573 2074 6865 2063 6f6d 7072 6573  ites the compres
+00001860: 7365 6420 6461 7461 2074 6f20 2a6f 7574  sed data to *out
+00001870: 7075 745f 7374 7265 616d 2a2c 2069 7420  put_stream*, it 
+00001880: 646f 6573 6e27 7420 636c 6f73 6520 7468  doesn't close th
+00001890: 6520 7374 7265 616d 732e 0a0a 2020 2020  e streams...    
+000018a0: 4966 2069 6e70 7574 2073 7472 6561 6d20  If input stream 
+000018b0: 6973 2060 6062 2727 6060 2c20 6e6f 7468  is ``b''``, noth
+000018c0: 696e 6720 7769 6c6c 2062 6520 7772 6974  ing will be writ
+000018d0: 7465 6e20 746f 206f 7574 7075 7420 7374  ten to output st
+000018e0: 7265 616d 2e0a 0a20 2020 2054 6869 7320  ream...    This 
+000018f0: 6675 6e63 7469 6f6e 2074 7269 6573 2074  function tries t
+00001900: 6f20 7a65 726f 2d63 6f70 7920 6173 206d  o zero-copy as m
+00001910: 7563 6820 6173 2070 6f73 7369 626c 652e  uch as possible.
+00001920: 2049 6620 7468 6520 4f53 2068 6173 2072   If the OS has r
+00001930: 6561 6420 7072 6566 6574 6368 696e 6720  ead prefetching 
+00001940: 616e 6420 7772 6974 6520 6275 6666 6572  and write buffer
+00001950: 2c20 6974 206d 6179 2070 6572 666f 726d  , it may perform
+00001960: 2074 6865 2074 6173 6b73 2028 7265 6164   the tasks (read
+00001970: 2f63 6f6d 7072 6573 732f 7772 6974 6529  /compress/write)
+00001980: 2069 6e20 7061 7261 6c6c 656c 2074 6f20   in parallel to 
+00001990: 736f 6d65 2064 6567 7265 652e 0a0a 2020  some degree...  
+000019a0: 2020 5468 6520 6465 6661 756c 7420 7661    The default va
+000019b0: 6c75 6573 206f 6620 2a72 6561 645f 7369  lues of *read_si
+000019c0: 7a65 2a20 616e 6420 2a77 7269 7465 5f73  ze* and *write_s
+000019d0: 697a 652a 2070 6172 616d 6574 6572 7320  ize* parameters 
+000019e0: 6172 6520 7468 6520 6275 6666 6572 2073  are the buffer s
+000019f0: 697a 6573 2072 6563 6f6d 6d65 6e64 6564  izes recommended
+00001a00: 2062 7920 7a73 7464 2c20 696e 6372 6561   by zstd, increa
+00001a10: 7369 6e67 2074 6865 6d20 6d61 7920 6265  sing them may be
+00001a20: 2066 6173 7465 722c 2061 6e64 2072 6564   faster, and red
+00001a30: 7563 6573 2074 6865 206e 756d 6265 7220  uces the number 
+00001a40: 6f66 2063 616c 6c62 6163 6b20 6675 6e63  of callback func
+00001a50: 7469 6f6e 2063 616c 6c73 2e0a 0a20 2020  tion calls...   
+00001a60: 202e 2e20 7665 7273 696f 6e61 6464 6564   .. versionadded
+00001a70: 3a3a 2030 2e31 342e 320a 0a20 2020 203a  :: 0.14.2..    :
+00001a80: 7061 7261 6d20 696e 7075 745f 7374 7265  param input_stre
+00001a90: 616d 3a20 496e 7075 7420 7374 7265 616d  am: Input stream
+00001aa0: 2074 6861 7420 6861 7320 6120 602e 7265   that has a `.re
+00001ab0: 6164 696e 746f 2862 2920 3c68 7474 7073  adinto(b) <https
+00001ac0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00001ad0: 7267 2f33 2f6c 6962 7261 7279 2f69 6f2e  rg/3/library/io.
+00001ae0: 6874 6d6c 2369 6f2e 5261 7749 4f42 6173  html#io.RawIOBas
+00001af0: 652e 7265 6164 696e 746f 3e60 5f20 6d65  e.readinto>`_ me
+00001b00: 7468 6f64 2e0a 2020 2020 3a70 6172 616d  thod..    :param
+00001b10: 206f 7574 7075 745f 7374 7265 616d 3a20   output_stream: 
+00001b20: 4f75 7470 7574 2073 7472 6561 6d20 7468  Output stream th
+00001b30: 6174 2068 6173 2061 2060 2e77 7269 7465  at has a `.write
+00001b40: 2862 2920 3c68 7474 7073 3a2f 2f64 6f63  (b) <https://doc
+00001b50: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+00001b60: 6962 7261 7279 2f69 6f2e 6874 6d6c 2369  ibrary/io.html#i
+00001b70: 6f2e 5261 7749 4f42 6173 652e 7772 6974  o.RawIOBase.writ
+00001b80: 653e 605f 206d 6574 686f 642e 2049 6620  e>`_ method. If 
+00001b90: 7573 6520 2a63 616c 6c62 6163 6b2a 2066  use *callback* f
+00001ba0: 756e 6374 696f 6e2c 2074 6869 7320 7061  unction, this pa
+00001bb0: 7261 6d65 7465 7220 6361 6e20 6265 2060  rameter can be `
+00001bc0: 604e 6f6e 6560 602e 0a20 2020 203a 7061  `None``..    :pa
+00001bd0: 7261 6d20 6c65 7665 6c5f 6f72 5f6f 7074  ram level_or_opt
+00001be0: 696f 6e3a 2057 6865 6e20 6974 2773 2061  ion: When it's a
+00001bf0: 6e20 6060 696e 7460 6020 6f62 6a65 6374  n ``int`` object
+00001c00: 2c20 6974 2072 6570 7265 7365 6e74 7320  , it represents 
+00001c10: 3a72 6566 3a60 636f 6d70 7265 7373 696f  :ref:`compressio
+00001c20: 6e20 6c65 7665 6c3c 636f 6d70 7265 7373  n level<compress
+00001c30: 696f 6e5f 6c65 7665 6c3e 602e 2057 6865  ion_level>`. Whe
+00001c40: 6e20 6974 2773 2061 2060 6064 6963 7460  n it's a ``dict`
+00001c50: 6020 6f62 6a65 6374 2c20 6974 2063 6f6e  ` object, it con
+00001c60: 7461 696e 7320 3a72 6566 3a60 6164 7661  tains :ref:`adva
+00001c70: 6e63 6564 2063 6f6d 7072 6573 7369 6f6e  nced compression
+00001c80: 2070 6172 616d 6574 6572 733c 4350 6172   parameters<CPar
+00001c90: 616d 6574 6572 3e60 2e20 5468 6520 6465  ameter>`. The de
+00001ca0: 6661 756c 7420 7661 6c75 6520 6060 4e6f  fault value ``No
+00001cb0: 6e65 6060 206d 6561 6e73 2074 6f20 7573  ne`` means to us
+00001cc0: 6520 7a73 7464 2773 2064 6566 6175 6c74  e zstd's default
+00001cd0: 2063 6f6d 7072 6573 7369 6f6e 206c 6576   compression lev
+00001ce0: 656c 2f70 6172 616d 6574 6572 732e 0a20  el/parameters.. 
+00001cf0: 2020 203a 7479 7065 206c 6576 656c 5f6f     :type level_o
+00001d00: 725f 6f70 7469 6f6e 3a20 696e 7420 6f72  r_option: int or
+00001d10: 2064 6963 740a 2020 2020 3a70 6172 616d   dict.    :param
+00001d20: 207a 7374 645f 6469 6374 3a20 5072 652d   zstd_dict: Pre-
+00001d30: 7472 6169 6e65 6420 6469 6374 696f 6e61  trained dictiona
+00001d40: 7279 2066 6f72 2063 6f6d 7072 6573 7369  ry for compressi
+00001d50: 6f6e 2e0a 2020 2020 3a74 7970 6520 7a73  on..    :type zs
+00001d60: 7464 5f64 6963 743a 205a 7374 6444 6963  td_dict: ZstdDic
+00001d70: 740a 2020 2020 3a70 6172 616d 2070 6c65  t.    :param ple
+00001d80: 6467 6564 5f69 6e70 7574 5f73 697a 653a  dged_input_size:
+00001d90: 2049 6620 7365 7420 7468 6973 2070 6172   If set this par
+00001da0: 616d 6574 6572 2074 6f20 7468 6520 7369  ameter to the si
+00001db0: 7a65 206f 6620 696e 7075 7420 6461 7461  ze of input data
+00001dc0: 2c20 7468 6520 3a72 6566 3a60 7369 7a65  , the :ref:`size
+00001dd0: 3c63 6f6e 7465 6e74 5f73 697a 653e 6020  <content_size>` 
+00001de0: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
+00001df0: 696e 746f 2074 6865 2066 7261 6d65 2068  into the frame h
+00001e00: 6561 6465 722e 2049 6620 7468 6520 6163  eader. If the ac
+00001e10: 7475 616c 2069 6e70 7574 2064 6174 6120  tual input data 
+00001e20: 646f 6573 6e27 7420 6d61 7463 6820 6974  doesn't match it
+00001e30: 2c20 6120 3a70 793a 636c 6173 733a 605a  , a :py:class:`Z
+00001e40: 7374 6445 7272 6f72 6020 6578 6365 7074  stdError` except
+00001e50: 696f 6e20 7769 6c6c 2062 6520 7261 6973  ion will be rais
+00001e60: 6564 2e20 4974 206d 6179 2069 6e63 7265  ed. It may incre
+00001e70: 6173 6520 636f 6d70 7265 7373 696f 6e20  ase compression 
+00001e80: 7261 7469 6f20 736c 6967 6874 6c79 2c20  ratio slightly, 
+00001e90: 616e 6420 6865 6c70 2064 6563 6f6d 7072  and help decompr
+00001ea0: 6573 7369 6f6e 2063 6f64 6520 746f 2061  ession code to a
+00001eb0: 6c6c 6f63 6174 6520 6f75 7470 7574 2062  llocate output b
+00001ec0: 7566 6665 7220 6661 7374 6572 2e0a 2020  uffer faster..  
+00001ed0: 2020 3a74 7970 6520 706c 6564 6765 645f    :type pledged_
+00001ee0: 696e 7075 745f 7369 7a65 3a20 696e 740a  input_size: int.
+00001ef0: 2020 2020 3a70 6172 616d 2072 6561 645f      :param read_
+00001f00: 7369 7a65 3a20 496e 7075 7420 6275 6666  size: Input buff
+00001f10: 6572 2073 697a 652c 2069 6e20 6279 7465  er size, in byte
+00001f20: 732e 0a20 2020 203a 7479 7065 2072 6561  s..    :type rea
+00001f30: 645f 7369 7a65 3a20 696e 740a 2020 2020  d_size: int.    
+00001f40: 3a70 6172 616d 2077 7269 7465 5f73 697a  :param write_siz
+00001f50: 653a 204f 7574 7075 7420 6275 6666 6572  e: Output buffer
+00001f60: 2073 697a 652c 2069 6e20 6279 7465 732e   size, in bytes.
+00001f70: 0a20 2020 203a 7479 7065 2077 7269 7465  .    :type write
+00001f80: 5f73 697a 653a 2069 6e74 0a20 2020 203a  _size: int.    :
+00001f90: 7061 7261 6d20 6361 6c6c 6261 636b 3a20  param callback: 
+00001fa0: 4120 6361 6c6c 6261 636b 2066 756e 6374  A callback funct
+00001fb0: 696f 6e20 7468 6174 2061 6363 6570 7473  ion that accepts
+00001fc0: 2066 6f75 7220 7061 7261 6d65 7465 7273   four parameters
+00001fd0: 3a20 6060 2874 6f74 616c 5f69 6e70 7574  : ``(total_input
+00001fe0: 2c20 746f 7461 6c5f 6f75 7470 7574 2c20  , total_output, 
+00001ff0: 7265 6164 5f64 6174 612c 2077 7269 7465  read_data, write
+00002000: 5f64 6174 6129 6060 2e20 5468 6520 6669  _data)``. The fi
+00002010: 7273 7420 7477 6f20 6172 6520 6060 696e  rst two are ``in
+00002020: 7460 6020 6f62 6a65 6374 732e 2054 6865  t`` objects. The
+00002030: 206c 6173 7420 7477 6f20 6172 6520 7265   last two are re
+00002040: 6164 6f6e 6c79 2060 6d65 6d6f 7279 7669  adonly `memoryvi
+00002050: 6577 203c 6874 7470 733a 2f2f 646f 6373  ew <https://docs
+00002060: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+00002070: 6272 6172 792f 7374 6474 7970 6573 2e68  brary/stdtypes.h
+00002080: 746d 6c23 6d65 6d6f 7279 2d76 6965 7773  tml#memory-views
+00002090: 3e60 5f20 6f62 6a65 6374 732c 2069 6620  >`_ objects, if 
+000020a0: 7761 6e74 2074 6f20 7265 6665 7265 6e63  want to referenc
+000020b0: 6520 7468 6520 6461 7461 2028 6f72 2069  e the data (or i
+000020c0: 7473 2073 6c69 6365 2920 6f75 7473 6964  ts slice) outsid
+000020d0: 6520 7468 6520 6361 6c6c 6261 636b 2066  e the callback f
+000020e0: 756e 6374 696f 6e2c 2060 636f 6e76 6572  unction, `conver
+000020f0: 7420 3c68 7474 7073 3a2f 2f64 6f63 732e  t <https://docs.
+00002100: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+00002110: 7261 7279 2f73 7464 7479 7065 732e 6874  rary/stdtypes.ht
+00002120: 6d6c 236d 656d 6f72 7976 6965 772e 746f  ml#memoryview.to
+00002130: 6279 7465 733e 605f 2074 6865 6d20 746f  bytes>`_ them to
+00002140: 2060 6062 7974 6573 6060 206f 626a 6563   ``bytes`` objec
+00002150: 7473 2e20 4966 2069 6e70 7574 2073 7472  ts. If input str
+00002160: 6561 6d20 6973 2060 6062 2727 6060 2c20  eam is ``b''``, 
+00002170: 7468 6520 6361 6c6c 6261 636b 2066 756e  the callback fun
+00002180: 6374 696f 6e20 7769 6c6c 206e 6f74 2062  ction will not b
+00002190: 6520 6361 6c6c 6564 2e0a 2020 2020 3a74  e called..    :t
+000021a0: 7970 6520 6361 6c6c 6261 636b 3a20 6361  ype callback: ca
+000021b0: 6c6c 6162 6c65 0a20 2020 203a 7265 7475  llable.    :retu
+000021c0: 726e 3a20 4120 322d 6974 656d 2074 7570  rn: A 2-item tup
+000021d0: 6c65 2c20 6060 2874 6f74 616c 5f69 6e70  le, ``(total_inp
+000021e0: 7574 2c20 746f 7461 6c5f 6f75 7470 7574  ut, total_output
+000021f0: 2960 602c 2074 6865 2069 7465 6d73 2061  )``, the items a
+00002200: 7265 2060 6069 6e74 6060 206f 626a 6563  re ``int`` objec
+00002210: 7473 2e0a 0a20 2020 202e 2e20 736f 7572  ts...    .. sour
+00002220: 6365 636f 6465 3a3a 2070 7974 686f 6e0a  cecode:: python.
+00002230: 0a20 2020 2020 2020 2023 2063 6f6d 7072  .        # compr
+00002240: 6573 7320 616e 2069 6e70 7574 2066 696c  ess an input fil
+00002250: 652c 2061 6e64 2077 7269 7465 2074 6f20  e, and write to 
+00002260: 616e 206f 7574 7075 7420 6669 6c65 2e0a  an output file..
+00002270: 2020 2020 2020 2020 7769 7468 2069 6f2e          with io.
+00002280: 6f70 656e 2869 6e70 7574 5f66 696c 655f  open(input_file_
+00002290: 7061 7468 2c20 2772 6227 2920 6173 2069  path, 'rb') as i
+000022a0: 6668 3a0a 2020 2020 2020 2020 2020 2020  fh:.            
+000022b0: 7769 7468 2069 6f2e 6f70 656e 286f 7574  with io.open(out
+000022c0: 7075 745f 6669 6c65 5f70 6174 682c 2027  put_file_path, '
+000022d0: 7762 2729 2061 7320 6f66 683a 0a20 2020  wb') as ofh:.   
+000022e0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+000022f0: 7072 6573 735f 7374 7265 616d 2869 6668  press_stream(ifh
+00002300: 2c20 6f66 682c 206c 6576 656c 5f6f 725f  , ofh, level_or_
+00002310: 6f70 7469 6f6e 3d35 290a 0a20 2020 2020  option=5)..     
+00002320: 2020 2023 2063 6f6d 7072 6573 7320 6120     # compress a 
+00002330: 6279 7465 7320 6f62 6a65 6374 2c20 616e  bytes object, an
+00002340: 6420 7772 6974 6520 746f 2061 2066 696c  d write to a fil
+00002350: 652e 0a20 2020 2020 2020 2077 6974 6820  e..        with 
+00002360: 696f 2e42 7974 6573 494f 2872 6177 5f64  io.BytesIO(raw_d
+00002370: 6174 2920 6173 2062 693a 0a20 2020 2020  at) as bi:.     
+00002380: 2020 2020 2020 2077 6974 6820 696f 2e6f         with io.o
+00002390: 7065 6e28 6f75 7470 7574 5f66 696c 655f  pen(output_file_
+000023a0: 7061 7468 2c20 2777 6227 2920 6173 206f  path, 'wb') as o
+000023b0: 6668 3a0a 2020 2020 2020 2020 2020 2020  fh:.            
+000023c0: 2020 2020 636f 6d70 7265 7373 5f73 7472      compress_str
+000023d0: 6561 6d28 6269 2c20 6f66 682c 2070 6c65  eam(bi, ofh, ple
+000023e0: 6467 6564 5f69 6e70 7574 5f73 697a 653d  dged_input_size=
+000023f0: 6c65 6e28 7261 775f 6461 7429 290a 0a20  len(raw_dat)).. 
+00002400: 2020 2020 2020 2023 2043 6f6d 7072 6573         # Compres
+00002410: 7320 616e 2069 6e70 7574 2066 696c 652c  s an input file,
+00002420: 206f 6274 6169 6e20 6120 6279 7465 7320   obtain a bytes 
+00002430: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+00002440: 2320 4974 2773 2066 6173 7465 7220 7468  # It's faster th
+00002450: 616e 2072 6561 6469 6e67 2061 2066 696c  an reading a fil
+00002460: 6520 616e 6420 636f 6d70 7265 7373 696e  e and compressin
+00002470: 6720 6974 2069 6e0a 2020 2020 2020 2020  g it in.        
+00002480: 2320 6d65 6d6f 7279 2c20 7465 7374 6564  # memory, tested
+00002490: 206f 6e20 5562 756e 7475 2850 7974 686f   on Ubuntu(Pytho
+000024a0: 6e33 2e38 292f 5769 6e64 6f77 7328 5079  n3.8)/Windows(Py
+000024b0: 7468 6f6e 332e 3929 2e0a 2020 2020 2020  thon3.9)..      
+000024c0: 2020 2320 4d61 7962 6520 7468 6520 4f53    # Maybe the OS
+000024d0: 2068 6173 2070 7265 6665 7463 6869 6e67   has prefetching
+000024e0: 2c20 6974 2063 616e 2072 6561 6420 616e  , it can read an
+000024f0: 6420 636f 6d70 7265 7373 0a20 2020 2020  d compress.     
+00002500: 2020 2023 2064 6174 6120 696e 2070 6172     # data in par
+00002510: 616c 6c65 6c20 746f 2073 6f6d 6520 6465  allel to some de
+00002520: 6772 6565 2c20 7265 6164 696e 6720 6669  gree, reading fi
+00002530: 6c65 2066 726f 6d20 4844 440a 2020 2020  le from HDD.    
+00002540: 2020 2020 2320 6973 2074 6865 2062 6f74      # is the bot
+00002550: 746c 656e 6563 6b20 696e 2074 6869 7320  tleneck in this 
+00002560: 6361 7365 2e0a 2020 2020 2020 2020 7769  case..        wi
+00002570: 7468 2069 6f2e 6f70 656e 2869 6e70 7574  th io.open(input
+00002580: 5f66 696c 655f 7061 7468 2c20 2772 6227  _file_path, 'rb'
+00002590: 2920 6173 2069 6668 3a0a 2020 2020 2020  ) as ifh:.      
+000025a0: 2020 2020 2020 7769 7468 2069 6f2e 4279        with io.By
+000025b0: 7465 7349 4f28 2920 6173 2062 6f3a 0a20  tesIO() as bo:. 
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000025d0: 6f6d 7072 6573 735f 7374 7265 616d 2869  ompress_stream(i
+000025e0: 6668 2c20 626f 290a 2020 2020 2020 2020  fh, bo).        
+000025f0: 2020 2020 2020 2020 636f 6d70 7265 7373          compress
+00002600: 6564 5f64 6174 203d 2062 6f2e 6765 7476  ed_dat = bo.getv
+00002610: 616c 7565 2829 0a0a 2020 2020 2020 2020  alue()..        
+00002620: 2320 5072 696e 7420 7072 6f67 7265 7373  # Print progress
+00002630: 2075 7369 6e67 2063 616c 6c62 6163 6b20   using callback 
+00002640: 6675 6e63 7469 6f6e 0a20 2020 2020 2020  function.       
+00002650: 2064 6566 2063 6f6d 7072 6573 735f 7072   def compress_pr
+00002660: 696e 745f 7072 6f67 7265 7373 2869 6e70  int_progress(inp
+00002670: 7574 5f66 696c 655f 7061 7468 2c20 6f75  ut_file_path, ou
+00002680: 7470 7574 5f66 696c 655f 7061 7468 293a  tput_file_path):
+00002690: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
+000026a0: 7574 5f66 696c 655f 7369 7a65 203d 206f  ut_file_size = o
+000026b0: 732e 7061 7468 2e67 6574 7369 7a65 2869  s.path.getsize(i
+000026c0: 6e70 7574 5f66 696c 655f 7061 7468 290a  nput_file_path).
+000026d0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+000026e0: 2066 756e 6328 746f 7461 6c5f 696e 7075   func(total_inpu
+000026f0: 742c 2074 6f74 616c 5f6f 7574 7075 742c  t, total_output,
+00002700: 2072 6561 645f 6461 7461 2c20 7772 6974   read_data, writ
+00002710: 655f 6461 7461 293a 0a20 2020 2020 2020  e_data):.       
+00002720: 2020 2020 2020 2020 2023 2049 6620 696e           # If in
+00002730: 7075 7420 7374 7265 616d 2069 7320 656d  put stream is em
+00002740: 7074 792c 2074 6865 2063 616c 6c62 6163  pty, the callbac
+00002750: 6b20 6675 6e63 7469 6f6e 0a20 2020 2020  k function.     
+00002760: 2020 2020 2020 2020 2020 2023 2077 696c             # wil
+00002770: 6c20 6e6f 7420 6265 2063 616c 6c65 642e  l not be called.
+00002780: 2053 6f20 6e6f 205a 6572 6f44 6976 6973   So no ZeroDivis
+00002790: 696f 6e45 7272 6f72 2068 6572 652e 0a20  ionError here.. 
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000027b0: 6572 6365 6e74 203d 2031 3030 202a 2074  ercent = 100 * t
+000027c0: 6f74 616c 5f69 6e70 7574 202f 2069 6e70  otal_input / inp
+000027d0: 7574 5f66 696c 655f 7369 7a65 0a20 2020  ut_file_size.   
+000027e0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000027f0: 6e74 2866 2750 726f 6772 6573 733a 207b  nt(f'Progress: {
+00002800: 7065 7263 656e 743a 2e31 667d 2527 2c20  percent:.1f}%', 
+00002810: 656e 643d 275c 7227 290a 0a20 2020 2020  end='\r')..     
+00002820: 2020 2020 2020 2077 6974 6820 696f 2e6f         with io.o
+00002830: 7065 6e28 696e 7075 745f 6669 6c65 5f70  pen(input_file_p
+00002840: 6174 682c 2027 7262 2729 2061 7320 6966  ath, 'rb') as if
+00002850: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+00002860: 2020 2077 6974 6820 696f 2e6f 7065 6e28     with io.open(
+00002870: 6f75 7470 7574 5f66 696c 655f 7061 7468  output_file_path
+00002880: 2c20 2777 6227 2920 6173 206f 6668 3a0a  , 'wb') as ofh:.
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 636f 6d70 7265 7373 5f73 7472      compress_str
+000028b0: 6561 6d28 6966 682c 206f 6668 2c20 6361  eam(ifh, ofh, ca
+000028c0: 6c6c 6261 636b 3d66 756e 6329 0a0a 0a2e  llback=func)....
+000028d0: 2e20 7079 3a63 6c61 7373 3a3a 205a 7374  . py:class:: Zst
+000028e0: 6443 6f6d 7072 6573 736f 720a 0a20 2020  dCompressor..   
+000028f0: 2041 2073 7472 6561 6d69 6e67 2063 6f6d   A streaming com
+00002900: 7072 6573 736f 722e 2049 7427 7320 7468  pressor. It's th
+00002910: 7265 6164 2d73 6166 6520 6174 206d 6574  read-safe at met
+00002920: 686f 6420 6c65 7665 6c2e 0a0a 2020 2020  hod level...    
+00002930: 2e2e 2070 793a 6d65 7468 6f64 3a3a 205f  .. py:method:: _
+00002940: 5f69 6e69 745f 5f28 7365 6c66 2c20 6c65  _init__(self, le
+00002950: 7665 6c5f 6f72 5f6f 7074 696f 6e3d 4e6f  vel_or_option=No
+00002960: 6e65 2c20 7a73 7464 5f64 6963 743d 4e6f  ne, zstd_dict=No
+00002970: 6e65 290a 0a20 2020 2020 2020 2049 6e69  ne)..        Ini
+00002980: 7469 616c 697a 6520 6120 5a73 7464 436f  tialize a ZstdCo
+00002990: 6d70 7265 7373 6f72 206f 626a 6563 742e  mpressor object.
+000029a0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000029b0: 206c 6576 656c 5f6f 725f 6f70 7469 6f6e   level_or_option
+000029c0: 3a20 5768 656e 2069 7427 7320 616e 2060  : When it's an `
+000029d0: 6069 6e74 6060 206f 626a 6563 742c 2069  `int`` object, i
+000029e0: 7420 7265 7072 6573 656e 7473 2074 6865  t represents the
+000029f0: 203a 7265 663a 6063 6f6d 7072 6573 7369   :ref:`compressi
+00002a00: 6f6e 206c 6576 656c 3c63 6f6d 7072 6573  on level<compres
+00002a10: 7369 6f6e 5f6c 6576 656c 3e60 2e20 5768  sion_level>`. Wh
+00002a20: 656e 2069 7427 7320 6120 6060 6469 6374  en it's a ``dict
+00002a30: 6060 206f 626a 6563 742c 2069 7420 636f  `` object, it co
+00002a40: 6e74 6169 6e73 203a 7265 663a 6061 6476  ntains :ref:`adv
+00002a50: 616e 6365 6420 636f 6d70 7265 7373 696f  anced compressio
+00002a60: 6e20 7061 7261 6d65 7465 7273 3c43 5061  n parameters<CPa
+00002a70: 7261 6d65 7465 723e 602e 2054 6865 2064  rameter>`. The d
+00002a80: 6566 6175 6c74 2076 616c 7565 2060 604e  efault value ``N
+00002a90: 6f6e 6560 6020 6d65 616e 7320 746f 2075  one`` means to u
+00002aa0: 7365 207a 7374 6427 7320 6465 6661 756c  se zstd's defaul
+00002ab0: 7420 636f 6d70 7265 7373 696f 6e20 6c65  t compression le
+00002ac0: 7665 6c2f 7061 7261 6d65 7465 7273 2e0a  vel/parameters..
+00002ad0: 2020 2020 2020 2020 3a74 7970 6520 6c65          :type le
+00002ae0: 7665 6c5f 6f72 5f6f 7074 696f 6e3a 2069  vel_or_option: i
+00002af0: 6e74 206f 7220 6469 6374 0a20 2020 2020  nt or dict.     
+00002b00: 2020 203a 7061 7261 6d20 7a73 7464 5f64     :param zstd_d
+00002b10: 6963 743a 2050 7265 2d74 7261 696e 6564  ict: Pre-trained
+00002b20: 2064 6963 7469 6f6e 6172 7920 666f 7220   dictionary for 
+00002b30: 636f 6d70 7265 7373 696f 6e2e 0a20 2020  compression..   
+00002b40: 2020 2020 203a 7479 7065 207a 7374 645f       :type zstd_
+00002b50: 6469 6374 3a20 5a73 7464 4469 6374 0a0a  dict: ZstdDict..
+00002b60: 2020 2020 2e2e 2070 793a 6d65 7468 6f64      .. py:method
+00002b70: 3a3a 2063 6f6d 7072 6573 7328 7365 6c66  :: compress(self
+00002b80: 2c20 6461 7461 2c20 6d6f 6465 3d5a 7374  , data, mode=Zst
+00002b90: 6443 6f6d 7072 6573 736f 722e 434f 4e54  dCompressor.CONT
+00002ba0: 494e 5545 290a 0a20 2020 2020 2020 2050  INUE)..        P
+00002bb0: 726f 7669 6465 2064 6174 6120 746f 2074  rovide data to t
+00002bc0: 6865 2063 6f6d 7072 6573 736f 7220 6f62  he compressor ob
+00002bd0: 6a65 6374 2e0a 0a20 2020 2020 2020 203a  ject...        :
+00002be0: 7061 7261 6d20 6461 7461 3a20 4461 7461  param data: Data
+00002bf0: 2074 6f20 6265 2063 6f6d 7072 6573 7365   to be compresse
+00002c00: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
+00002c10: 2064 6174 613a 2062 7974 6573 2d6c 696b   data: bytes-lik
+00002c20: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00002c30: 203a 7061 7261 6d20 6d6f 6465 3a20 4361   :param mode: Ca
+00002c40: 6e20 6265 2074 6865 7365 2033 2076 616c  n be these 3 val
+00002c50: 7565 733a 203a 7079 3a61 7474 723a 605a  ues: :py:attr:`Z
+00002c60: 7374 6443 6f6d 7072 6573 736f 722e 434f  stdCompressor.CO
+00002c70: 4e54 494e 5545 602c 203a 7079 3a61 7474  NTINUE`, :py:att
+00002c80: 723a 605a 7374 6443 6f6d 7072 6573 736f  r:`ZstdCompresso
+00002c90: 722e 464c 5553 485f 424c 4f43 4b60 2c20  r.FLUSH_BLOCK`, 
+00002ca0: 3a70 793a 6174 7472 3a60 5a73 7464 436f  :py:attr:`ZstdCo
+00002cb0: 6d70 7265 7373 6f72 2e46 4c55 5348 5f46  mpressor.FLUSH_F
+00002cc0: 5241 4d45 602e 0a20 2020 2020 2020 203a  RAME`..        :
+00002cd0: 7265 7475 726e 3a20 4120 6368 756e 6b20  return: A chunk 
+00002ce0: 6f66 2063 6f6d 7072 6573 7365 6420 6461  of compressed da
+00002cf0: 7461 2069 6620 706f 7373 6962 6c65 2c20  ta if possible, 
+00002d00: 6f72 2060 6062 2727 6060 206f 7468 6572  or ``b''`` other
+00002d10: 7769 7365 2e0a 2020 2020 2020 2020 3a72  wise..        :r
+00002d20: 7479 7065 3a20 6279 7465 730a 0a20 2020  type: bytes..   
+00002d30: 202e 2e20 7079 3a6d 6574 686f 643a 3a20   .. py:method:: 
+00002d40: 666c 7573 6828 7365 6c66 2c20 6d6f 6465  flush(self, mode
+00002d50: 3d5a 7374 6443 6f6d 7072 6573 736f 722e  =ZstdCompressor.
+00002d60: 464c 5553 485f 4652 414d 4529 0a0a 2020  FLUSH_FRAME)..  
+00002d70: 2020 2020 2020 466c 7573 6820 616e 7920        Flush any 
+00002d80: 7265 6d61 696e 696e 6720 6461 7461 2069  remaining data i
+00002d90: 6e20 696e 7465 726e 616c 2062 7566 6665  n internal buffe
+00002da0: 722e 0a0a 2020 2020 2020 2020 5369 6e63  r...        Sinc
+00002db0: 6520 7a73 7464 2064 6174 6120 636f 6e73  e zstd data cons
+00002dc0: 6973 7473 206f 6620 6f6e 6520 6f72 206d  ists of one or m
+00002dd0: 6f72 6520 696e 6465 7065 6e64 656e 7420  ore independent 
+00002de0: 6672 616d 6573 2c20 7468 6520 636f 6d70  frames, the comp
+00002df0: 7265 7373 6f72 206f 626a 6563 7420 6361  ressor object ca
+00002e00: 6e20 7374 696c 6c20 6265 2075 7365 6420  n still be used 
+00002e10: 6166 7465 7220 7468 6973 206d 6574 686f  after this metho
+00002e20: 6420 6973 2063 616c 6c65 642e 0a0a 2020  d is called...  
+00002e30: 2020 2020 2020 2a2a 4e6f 7465 2a2a 3a20        **Note**: 
+00002e40: 4162 7573 6520 6f66 2074 6869 7320 6d65  Abuse of this me
+00002e50: 7468 6f64 2077 696c 6c20 7265 6475 6365  thod will reduce
+00002e60: 2063 6f6d 7072 6573 7369 6f6e 2072 6174   compression rat
+00002e70: 696f 2c20 616e 6420 736f 6d65 2070 726f  io, and some pro
+00002e80: 6772 616d 7320 6361 6e20 6f6e 6c79 2064  grams can only d
+00002e90: 6563 6f6d 7072 6573 7320 7369 6e67 6c65  ecompress single
+00002ea0: 2066 7261 6d65 2064 6174 612e 2055 7365   frame data. Use
+00002eb0: 2069 7420 6f6e 6c79 2077 6865 6e20 6e65   it only when ne
+00002ec0: 6365 7373 6172 792e 0a0a 2020 2020 2020  cessary...      
+00002ed0: 2020 3a70 6172 616d 206d 6f64 653a 2043    :param mode: C
+00002ee0: 616e 2062 6520 7468 6573 6520 3220 7661  an be these 2 va
+00002ef0: 6c75 6573 3a20 3a70 793a 6174 7472 3a60  lues: :py:attr:`
+00002f00: 5a73 7464 436f 6d70 7265 7373 6f72 2e46  ZstdCompressor.F
+00002f10: 4c55 5348 5f46 5241 4d45 602c 203a 7079  LUSH_FRAME`, :py
+00002f20: 3a61 7474 723a 605a 7374 6443 6f6d 7072  :attr:`ZstdCompr
+00002f30: 6573 736f 722e 464c 5553 485f 424c 4f43  essor.FLUSH_BLOC
+00002f40: 4b60 2e0a 2020 2020 2020 2020 3a72 6574  K`..        :ret
+00002f50: 7572 6e3a 2046 6c75 7368 6564 2064 6174  urn: Flushed dat
+00002f60: 612e 0a20 2020 2020 2020 203a 7274 7970  a..        :rtyp
+00002f70: 653a 2062 7974 6573 0a0a 2020 2020 2e2e  e: bytes..    ..
+00002f80: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
+00002f90: 6c61 7374 5f6d 6f64 650a 0a20 2020 2020  last_mode..     
+00002fa0: 2020 2054 6865 206c 6173 7420 6d6f 6465     The last mode
+00002fb0: 2075 7365 6420 746f 2074 6869 7320 636f   used to this co
+00002fc0: 6d70 7265 7373 6f72 2c20 6974 7320 7661  mpressor, its va
+00002fd0: 6c75 6520 6361 6e20 6265 203a 7079 3a61  lue can be :py:a
+00002fe0: 7474 723a 607e 5a73 7464 436f 6d70 7265  ttr:`~ZstdCompre
+00002ff0: 7373 6f72 2e43 4f4e 5449 4e55 4560 2c20  ssor.CONTINUE`, 
+00003000: 3a70 793a 6174 7472 3a60 7e5a 7374 6443  :py:attr:`~ZstdC
+00003010: 6f6d 7072 6573 736f 722e 464c 5553 485f  ompressor.FLUSH_
+00003020: 424c 4f43 4b60 2c20 3a70 793a 6174 7472  BLOCK`, :py:attr
+00003030: 3a60 7e5a 7374 6443 6f6d 7072 6573 736f  :`~ZstdCompresso
+00003040: 722e 464c 5553 485f 4652 414d 4560 2e20  r.FLUSH_FRAME`. 
+00003050: 496e 6974 6961 6c69 7a65 6420 746f 203a  Initialized to :
+00003060: 7079 3a61 7474 723a 607e 5a73 7464 436f  py:attr:`~ZstdCo
+00003070: 6d70 7265 7373 6f72 2e46 4c55 5348 5f46  mpressor.FLUSH_F
+00003080: 5241 4d45 602e 0a0a 2020 2020 2020 2020  RAME`...        
+00003090: 4974 2063 616e 2062 6520 7573 6564 2074  It can be used t
+000030a0: 6f20 6765 7420 7468 6520 6375 7272 656e  o get the curren
+000030b0: 7420 7374 6174 6520 6f66 2061 2063 6f6d  t state of a com
+000030c0: 7072 6573 736f 722c 2073 7563 6820 6173  pressor, such as
+000030d0: 2c20 6461 7461 2066 6c75 7368 6564 2c20  , data flushed, 
+000030e0: 6120 6672 616d 6520 656e 6465 642e 0a0a  a frame ended...
+000030f0: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
+00003100: 7574 653a 3a20 434f 4e54 494e 5545 0a0a  ute:: CONTINUE..
+00003110: 2020 2020 2020 2020 5573 6564 2066 6f72          Used for
+00003120: 202a 6d6f 6465 2a20 7061 7261 6d65 7465   *mode* paramete
+00003130: 7220 696e 203a 7079 3a6d 6574 683a 607e  r in :py:meth:`~
+00003140: 5a73 7464 436f 6d70 7265 7373 6f72 2e63  ZstdCompressor.c
+00003150: 6f6d 7072 6573 7360 206d 6574 686f 642e  ompress` method.
+00003160: 0a0a 2020 2020 2020 2020 436f 6c6c 6563  ..        Collec
+00003170: 7420 6d6f 7265 2064 6174 612c 2065 6e63  t more data, enc
+00003180: 6f64 6572 2064 6563 6964 6573 2077 6865  oder decides whe
+00003190: 6e20 746f 206f 7574 7075 7420 636f 6d70  n to output comp
+000031a0: 7265 7373 6564 2072 6573 756c 742c 2066  ressed result, f
+000031b0: 6f72 206f 7074 696d 616c 2063 6f6d 7072  or optimal compr
+000031c0: 6573 7369 6f6e 2072 6174 696f 2e20 5573  ession ratio. Us
+000031d0: 7561 6c6c 7920 7573 6564 2066 6f72 2074  ually used for t
+000031e0: 7261 6469 7469 6f6e 616c 2073 7472 6561  raditional strea
+000031f0: 6d69 6e67 2063 6f6d 7072 6573 7369 6f6e  ming compression
+00003200: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
+00003210: 7269 6275 7465 3a3a 2046 4c55 5348 5f42  ribute:: FLUSH_B
+00003220: 4c4f 434b 0a0a 2020 2020 2020 2020 5573  LOCK..        Us
+00003230: 6564 2066 6f72 202a 6d6f 6465 2a20 7061  ed for *mode* pa
+00003240: 7261 6d65 7465 7220 696e 203a 7079 3a6d  rameter in :py:m
+00003250: 6574 683a 607e 5a73 7464 436f 6d70 7265  eth:`~ZstdCompre
+00003260: 7373 6f72 2e63 6f6d 7072 6573 7360 2c20  ssor.compress`, 
+00003270: 3a70 793a 6d65 7468 3a60 7e5a 7374 6443  :py:meth:`~ZstdC
+00003280: 6f6d 7072 6573 736f 722e 666c 7573 6860  ompressor.flush`
+00003290: 206d 6574 686f 6473 2e0a 0a20 2020 2020   methods...     
+000032a0: 2020 2046 6c75 7368 2061 6e79 2072 656d     Flush any rem
+000032b0: 6169 6e69 6e67 2064 6174 612c 2062 7574  aining data, but
+000032c0: 2064 6f6e 2774 2063 6c6f 7365 2074 6865   don't close the
+000032d0: 2063 7572 7265 6e74 203a 7265 663a 6066   current :ref:`f
+000032e0: 7261 6d65 3c66 7261 6d65 5f62 6c6f 636b  rame<frame_block
+000032f0: 3e60 2e20 5573 7561 6c6c 7920 7573 6564  >`. Usually used
+00003300: 2066 6f72 2063 6f6d 6d75 6e69 6361 7469   for communicati
+00003310: 6f6e 2073 6365 6e61 7269 6f73 2e0a 0a20  on scenarios... 
+00003320: 2020 2020 2020 2049 6620 7468 6572 6520         If there 
+00003330: 6973 2064 6174 612c 2069 7420 6372 6561  is data, it crea
+00003340: 7465 7320 6174 206c 6561 7374 206f 6e65  tes at least one
+00003350: 206e 6577 203a 7265 663a 6062 6c6f 636b   new :ref:`block
+00003360: 3c66 7261 6d65 5f62 6c6f 636b 3e60 2c20  <frame_block>`, 
+00003370: 7468 6174 2063 616e 2062 6520 6465 636f  that can be deco
+00003380: 6465 6420 696d 6d65 6469 6174 656c 7920  ded immediately 
+00003390: 6f6e 2072 6563 6570 7469 6f6e 2e20 4966  on reception. If
+000033a0: 206e 6f20 7265 6d61 696e 696e 6720 6461   no remaining da
+000033b0: 7461 2c20 6e6f 2062 6c6f 636b 2069 7320  ta, no block is 
+000033c0: 6372 6561 7465 642c 2072 6574 7572 6e20  created, return 
+000033d0: 6060 6227 2760 602e 0a0a 2020 2020 2020  ``b''``...      
+000033e0: 2020 2a2a 4e6f 7465 2a2a 3a20 4162 7573    **Note**: Abus
+000033f0: 6520 6f66 2074 6869 7320 6d6f 6465 2077  e of this mode w
+00003400: 696c 6c20 7265 6475 6365 2063 6f6d 7072  ill reduce compr
+00003410: 6573 7369 6f6e 2072 6174 696f 2e20 5573  ession ratio. Us
+00003420: 6520 6974 206f 6e6c 7920 7768 656e 206e  e it only when n
+00003430: 6563 6573 7361 7279 2e0a 0a20 2020 202e  ecessary...    .
+00003440: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
+00003450: 2046 4c55 5348 5f46 5241 4d45 0a0a 2020   FLUSH_FRAME..  
+00003460: 2020 2020 2020 5573 6564 2066 6f72 202a        Used for *
+00003470: 6d6f 6465 2a20 7061 7261 6d65 7465 7220  mode* parameter 
+00003480: 696e 203a 7079 3a6d 6574 683a 607e 5a73  in :py:meth:`~Zs
+00003490: 7464 436f 6d70 7265 7373 6f72 2e63 6f6d  tdCompressor.com
+000034a0: 7072 6573 7360 2c20 3a70 793a 6d65 7468  press`, :py:meth
+000034b0: 3a60 7e5a 7374 6443 6f6d 7072 6573 736f  :`~ZstdCompresso
+000034c0: 722e 666c 7573 6860 206d 6574 686f 6473  r.flush` methods
+000034d0: 2e0a 0a20 2020 2020 2020 2046 6c75 7368  ...        Flush
+000034e0: 2061 6e79 2072 656d 6169 6e69 6e67 2064   any remaining d
+000034f0: 6174 612c 2061 6e64 2063 6c6f 7365 2074  ata, and close t
+00003500: 6865 2063 7572 7265 6e74 203a 7265 663a  he current :ref:
+00003510: 6066 7261 6d65 3c66 7261 6d65 5f62 6c6f  `frame<frame_blo
+00003520: 636b 3e60 2e20 5573 7561 6c6c 7920 7573  ck>`. Usually us
+00003530: 6564 2066 6f72 2074 7261 6469 7469 6f6e  ed for tradition
+00003540: 616c 2066 6c75 7368 2e0a 0a20 2020 2020  al flush...     
+00003550: 2020 2053 696e 6365 207a 7374 6420 6461     Since zstd da
+00003560: 7461 2063 6f6e 7369 7374 7320 6f66 206f  ta consists of o
+00003570: 6e65 206f 7220 6d6f 7265 2069 6e64 6570  ne or more indep
+00003580: 656e 6465 6e74 2066 7261 6d65 732c 2064  endent frames, d
+00003590: 6174 6120 6361 6e20 7374 696c 6c20 6265  ata can still be
+000035a0: 2070 726f 7669 6465 6420 6166 7465 7220   provided after 
+000035b0: 6120 6672 616d 6520 6973 2063 6c6f 7365  a frame is close
+000035c0: 642e 0a0a 2020 2020 2020 2020 2a2a 4e6f  d...        **No
+000035d0: 7465 2a2a 3a20 4162 7573 6520 6f66 2074  te**: Abuse of t
+000035e0: 6869 7320 6d6f 6465 2077 696c 6c20 7265  his mode will re
+000035f0: 6475 6365 2063 6f6d 7072 6573 7369 6f6e  duce compression
+00003600: 2072 6174 696f 2c20 616e 6420 736f 6d65   ratio, and some
+00003610: 2070 726f 6772 616d 7320 6361 6e20 6f6e   programs can on
+00003620: 6c79 2064 6563 6f6d 7072 6573 7320 7369  ly decompress si
+00003630: 6e67 6c65 2066 7261 6d65 2064 6174 612e  ngle frame data.
+00003640: 2055 7365 2069 7420 6f6e 6c79 2077 6865   Use it only whe
+00003650: 6e20 6e65 6365 7373 6172 792e 0a0a 2020  n necessary...  
+00003660: 2020 2e2e 2073 6f75 7263 6563 6f64 653a    .. sourcecode:
+00003670: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+00003680: 2020 6320 3d20 5a73 7464 436f 6d70 7265    c = ZstdCompre
+00003690: 7373 6f72 2829 0a0a 2020 2020 2020 2020  ssor()..        
+000036a0: 2320 7472 6164 6974 696f 6e61 6c20 7374  # traditional st
+000036b0: 7265 616d 696e 6720 636f 6d70 7265 7373  reaming compress
+000036c0: 696f 6e0a 2020 2020 2020 2020 6461 7431  ion.        dat1
+000036d0: 203d 2063 2e63 6f6d 7072 6573 7328 6227   = c.compress(b'
+000036e0: 3132 3334 3536 2729 0a20 2020 2020 2020  123456').       
+000036f0: 2064 6174 3220 3d20 632e 636f 6d70 7265   dat2 = c.compre
+00003700: 7373 2862 2761 6263 6465 6627 290a 2020  ss(b'abcdef').  
+00003710: 2020 2020 2020 6461 7433 203d 2063 2e66        dat3 = c.f
+00003720: 6c75 7368 2829 0a0a 2020 2020 2020 2020  lush()..        
+00003730: 2320 7573 6520 2e63 6f6d 7072 6573 7328  # use .compress(
+00003740: 2920 6d65 7468 6f64 2077 6974 6820 6d6f  ) method with mo
+00003750: 6465 2061 7267 756d 656e 740a 2020 2020  de argument.    
+00003760: 2020 2020 636f 6d70 7265 7373 6564 5f64      compressed_d
+00003770: 6174 3120 3d20 632e 636f 6d70 7265 7373  at1 = c.compress
+00003780: 2872 6177 5f64 6174 312c 2063 2e46 4c55  (raw_dat1, c.FLU
+00003790: 5348 5f42 4c4f 434b 290a 2020 2020 2020  SH_BLOCK).      
+000037a0: 2020 636f 6d70 7265 7373 6564 5f64 6174    compressed_dat
+000037b0: 3220 3d20 632e 636f 6d70 7265 7373 2872  2 = c.compress(r
+000037c0: 6177 5f64 6174 322c 2063 2e46 4c55 5348  aw_dat2, c.FLUSH
+000037d0: 5f46 5241 4d45 290a 0a20 2020 202e 2e20  _FRAME)..    .. 
+000037e0: 6869 6e74 3a3a 2057 6879 203a 7079 3a6d  hint:: Why :py:m
+000037f0: 6574 683a 605a 7374 6443 6f6d 7072 6573  eth:`ZstdCompres
+00003800: 736f 722e 636f 6d70 7265 7373 6020 6d65  sor.compress` me
+00003810: 7468 6f64 2068 6173 2061 202a 6d6f 6465  thod has a *mode
+00003820: 2a20 7061 7261 6d65 7465 723f 0a0a 2020  * parameter?..  
+00003830: 2020 2020 2020 232e 2057 6865 6e20 7265        #. When re
+00003840: 7573 6520 3a70 793a 636c 6173 733a 605a  use :py:class:`Z
+00003850: 7374 6443 6f6d 7072 6573 736f 7260 206f  stdCompressor` o
+00003860: 626a 6563 7420 666f 7220 6269 6720 6e75  bject for big nu
+00003870: 6d62 6572 206f 6620 7361 6d65 2074 7970  mber of same typ
+00003880: 6520 696e 6469 7669 6475 616c 2064 6174  e individual dat
+00003890: 612c 206d 616b 6520 6f70 6572 6174 696f  a, make operatio
+000038a0: 6e20 6d6f 7265 2063 6f6e 7665 6e69 656e  n more convenien
+000038b0: 742e 2054 6865 206f 626a 6563 7420 6973  t. The object is
+000038c0: 2074 6872 6561 642d 7361 6665 2061 7420   thread-safe at 
+000038d0: 6d65 7468 6f64 206c 6576 656c 2e0a 2020  method level..  
+000038e0: 2020 2020 2020 232e 2049 6620 6461 7461        #. If data
+000038f0: 2069 7320 6765 6e65 7261 7465 6420 6279   is generated by
+00003900: 2061 2073 696e 676c 6520 3a70 793a 6174   a single :py:at
+00003910: 7472 3a60 7e5a 7374 6443 6f6d 7072 6573  tr:`~ZstdCompres
+00003920: 736f 722e 464c 5553 485f 4652 414d 4560  sor.FLUSH_FRAME`
+00003930: 206d 6f64 652c 2074 6865 2073 697a 6520   mode, the size 
+00003940: 6f66 2075 6e63 6f6d 7072 6573 7365 6420  of uncompressed 
+00003950: 6461 7461 2077 696c 6c20 6265 2072 6563  data will be rec
+00003960: 6f72 6465 6420 696e 2066 7261 6d65 2068  orded in frame h
+00003970: 6561 6465 722e 0a0a 0a53 7472 6561 6d69  eader....Streami
+00003980: 6e67 2064 6563 6f6d 7072 6573 7369 6f6e  ng decompression
+00003990: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+000039a0: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020 5468  --------..    Th
+000039b0: 6973 2073 6563 7469 6f6e 2063 6f6e 7461  is section conta
+000039c0: 696e 733a 0a0a 2020 2020 2020 2020 2a20  ins:..        * 
+000039d0: 6675 6e63 7469 6f6e 203a 7079 3a66 756e  function :py:fun
+000039e0: 633a 6064 6563 6f6d 7072 6573 735f 7374  c:`decompress_st
+000039f0: 7265 616d 602c 2061 2066 6173 7420 616e  ream`, a fast an
+00003a00: 6420 636f 6e76 656e 6965 6e74 2066 756e  d convenient fun
+00003a10: 6374 696f 6e2e 0a20 2020 2020 2020 202a  ction..        *
+00003a20: 2063 6c61 7373 203a 7079 3a63 6c61 7373   class :py:class
+00003a30: 3a60 5a73 7464 4465 636f 6d70 7265 7373  :`ZstdDecompress
+00003a40: 6f72 602c 2073 696d 696c 6172 2074 6f20  or`, similar to 
+00003a50: 6465 636f 6d70 7265 7373 6f72 7320 696e  decompressors in
+00003a60: 2050 7974 686f 6e20 7374 616e 6461 7264   Python standard
+00003a70: 206c 6962 7261 7279 2e0a 2020 2020 2020   library..      
+00003a80: 2020 2a20 636c 6173 7320 3a70 793a 636c    * class :py:cl
+00003a90: 6173 733a 6045 6e64 6c65 7373 5a73 7464  ass:`EndlessZstd
+00003aa0: 4465 636f 6d70 7265 7373 6f72 602c 2061  Decompressor`, a
+00003ab0: 2064 6563 6f6d 7072 6573 736f 7220 6163   decompressor ac
+00003ac0: 6365 7074 7320 6d75 6c74 6970 6c65 2063  cepts multiple c
+00003ad0: 6f6e 6361 7465 6e61 7465 6420 3a72 6566  oncatenated :ref
+00003ae0: 3a60 6672 616d 6573 3c66 7261 6d65 5f62  :`frames<frame_b
+00003af0: 6c6f 636b 3e60 2e0a 0a2e 2e20 7079 3a66  lock>`..... py:f
+00003b00: 756e 6374 696f 6e3a 3a20 6465 636f 6d70  unction:: decomp
+00003b10: 7265 7373 5f73 7472 6561 6d28 696e 7075  ress_stream(inpu
+00003b20: 745f 7374 7265 616d 2c20 6f75 7470 7574  t_stream, output
+00003b30: 5f73 7472 6561 6d2c 202a 2c20 7a73 7464  _stream, *, zstd
+00003b40: 5f64 6963 743d 4e6f 6e65 2c20 6f70 7469  _dict=None, opti
+00003b50: 6f6e 3d4e 6f6e 652c 2072 6561 645f 7369  on=None, read_si
+00003b60: 7a65 3d31 3331 5f30 3735 2c20 7772 6974  ze=131_075, writ
+00003b70: 655f 7369 7a65 3d31 3331 5f30 3732 2c20  e_size=131_072, 
+00003b80: 6361 6c6c 6261 636b 3d4e 6f6e 6529 0a0a  callback=None)..
+00003b90: 2020 2020 4120 6661 7374 2061 6e64 2063      A fast and c
+00003ba0: 6f6e 7665 6e69 656e 7420 6675 6e63 7469  onvenient functi
+00003bb0: 6f6e 2c20 6465 636f 6d70 7265 7373 6573  on, decompresses
+00003bc0: 202a 696e 7075 745f 7374 7265 616d 2a20   *input_stream* 
+00003bd0: 616e 6420 7772 6974 6573 2074 6865 2064  and writes the d
+00003be0: 6563 6f6d 7072 6573 7365 6420 6461 7461  ecompressed data
+00003bf0: 2074 6f20 2a6f 7574 7075 745f 7374 7265   to *output_stre
+00003c00: 616d 2a2c 2069 7420 646f 6573 6e27 7420  am*, it doesn't 
+00003c10: 636c 6f73 6520 7468 6520 7374 7265 616d  close the stream
+00003c20: 732e 0a0a 2020 2020 5375 7070 6f72 7473  s...    Supports
+00003c30: 206d 756c 7469 706c 6520 636f 6e63 6174   multiple concat
+00003c40: 656e 6174 6564 203a 7265 663a 6066 7261  enated :ref:`fra
+00003c50: 6d65 733c 6672 616d 655f 626c 6f63 6b3e  mes<frame_block>
+00003c60: 602e 0a0a 2020 2020 5468 6973 2066 756e  `...    This fun
+00003c70: 6374 696f 6e20 7472 6965 7320 746f 207a  ction tries to z
+00003c80: 6572 6f2d 636f 7079 2061 7320 6d75 6368  ero-copy as much
+00003c90: 2061 7320 706f 7373 6962 6c65 2e20 4966   as possible. If
+00003ca0: 2074 6865 204f 5320 6861 7320 7265 6164   the OS has read
+00003cb0: 2070 7265 6665 7463 6869 6e67 2061 6e64   prefetching and
+00003cc0: 2077 7269 7465 2062 7566 6665 722c 2069   write buffer, i
+00003cd0: 7420 6d61 7920 7065 7266 6f72 6d20 7468  t may perform th
+00003ce0: 6520 7461 736b 7320 2872 6561 642f 6465  e tasks (read/de
+00003cf0: 636f 6d70 7265 7373 2f77 7269 7465 2920  compress/write) 
+00003d00: 696e 2070 6172 616c 6c65 6c20 746f 2073  in parallel to s
+00003d10: 6f6d 6520 6465 6772 6565 2e0a 0a20 2020  ome degree...   
+00003d20: 2054 6865 2064 6566 6175 6c74 2076 616c   The default val
+00003d30: 7565 7320 6f66 202a 7265 6164 5f73 697a  ues of *read_siz
+00003d40: 652a 2061 6e64 202a 7772 6974 655f 7369  e* and *write_si
+00003d50: 7a65 2a20 7061 7261 6d65 7465 7273 2061  ze* parameters a
+00003d60: 7265 2074 6865 2062 7566 6665 7220 7369  re the buffer si
+00003d70: 7a65 7320 7265 636f 6d6d 656e 6465 6420  zes recommended 
+00003d80: 6279 207a 7374 642c 2069 6e63 7265 6173  by zstd, increas
+00003d90: 696e 6720 7468 656d 206d 6179 2062 6520  ing them may be 
+00003da0: 6661 7374 6572 2c20 616e 6420 7265 6475  faster, and redu
+00003db0: 6365 7320 7468 6520 6e75 6d62 6572 206f  ces the number o
+00003dc0: 6620 6361 6c6c 6261 636b 2066 756e 6374  f callback funct
+00003dd0: 696f 6e20 6361 6c6c 732e 0a0a 2020 2020  ion calls...    
+00003de0: 2e2e 2076 6572 7369 6f6e 6164 6465 643a  .. versionadded:
+00003df0: 3a20 302e 3134 2e32 0a0a 2020 2020 3a70  : 0.14.2..    :p
+00003e00: 6172 616d 2069 6e70 7574 5f73 7472 6561  aram input_strea
+00003e10: 6d3a 2049 6e70 7574 2073 7472 6561 6d20  m: Input stream 
+00003e20: 7468 6174 2068 6173 2061 2060 2e72 6561  that has a `.rea
+00003e30: 6469 6e74 6f28 6229 203c 6874 7470 733a  dinto(b) <https:
+00003e40: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
+00003e50: 672f 332f 6c69 6272 6172 792f 696f 2e68  g/3/library/io.h
+00003e60: 746d 6c23 696f 2e52 6177 494f 4261 7365  tml#io.RawIOBase
+00003e70: 2e72 6561 6469 6e74 6f3e 605f 206d 6574  .readinto>`_ met
+00003e80: 686f 642e 0a20 2020 203a 7061 7261 6d20  hod..    :param 
+00003e90: 6f75 7470 7574 5f73 7472 6561 6d3a 204f  output_stream: O
+00003ea0: 7574 7075 7420 7374 7265 616d 2074 6861  utput stream tha
+00003eb0: 7420 6861 7320 6120 602e 7772 6974 6528  t has a `.write(
+00003ec0: 6229 203c 6874 7470 733a 2f2f 646f 6373  b) <https://docs
+00003ed0: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+00003ee0: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
+00003ef0: 2e52 6177 494f 4261 7365 2e77 7269 7465  .RawIOBase.write
+00003f00: 3e60 5f20 6d65 7468 6f64 2e20 4966 2075  >`_ method. If u
+00003f10: 7365 202a 6361 6c6c 6261 636b 2a20 6675  se *callback* fu
+00003f20: 6e63 7469 6f6e 2c20 7468 6973 2070 6172  nction, this par
+00003f30: 616d 6574 6572 2063 616e 2062 6520 6060  ameter can be ``
+00003f40: 4e6f 6e65 6060 2e0a 2020 2020 3a70 6172  None``..    :par
+00003f50: 616d 207a 7374 645f 6469 6374 3a20 5072  am zstd_dict: Pr
+00003f60: 652d 7472 6169 6e65 6420 6469 6374 696f  e-trained dictio
+00003f70: 6e61 7279 2066 6f72 2064 6563 6f6d 7072  nary for decompr
+00003f80: 6573 7369 6f6e 2e0a 2020 2020 3a74 7970  ession..    :typ
+00003f90: 6520 7a73 7464 5f64 6963 743a 205a 7374  e zstd_dict: Zst
+00003fa0: 6444 6963 740a 2020 2020 3a70 6172 616d  dDict.    :param
+00003fb0: 206f 7074 696f 6e3a 2041 2060 6064 6963   option: A ``dic
+00003fc0: 7460 6020 6f62 6a65 6374 2c20 636f 6e74  t`` object, cont
+00003fd0: 6169 6e73 203a 7265 663a 6061 6476 616e  ains :ref:`advan
+00003fe0: 6365 6420 6465 636f 6d70 7265 7373 696f  ced decompressio
+00003ff0: 6e20 7061 7261 6d65 7465 7273 3c44 5061  n parameters<DPa
+00004000: 7261 6d65 7465 723e 602e 0a20 2020 203a  rameter>`..    :
+00004010: 7479 7065 206f 7074 696f 6e3a 2064 6963  type option: dic
+00004020: 740a 2020 2020 3a70 6172 616d 2072 6561  t.    :param rea
+00004030: 645f 7369 7a65 3a20 496e 7075 7420 6275  d_size: Input bu
+00004040: 6666 6572 2073 697a 652c 2069 6e20 6279  ffer size, in by
+00004050: 7465 732e 0a20 2020 203a 7479 7065 2072  tes..    :type r
+00004060: 6561 645f 7369 7a65 3a20 696e 740a 2020  ead_size: int.  
+00004070: 2020 3a70 6172 616d 2077 7269 7465 5f73    :param write_s
+00004080: 697a 653a 204f 7574 7075 7420 6275 6666  ize: Output buff
+00004090: 6572 2073 697a 652c 2069 6e20 6279 7465  er size, in byte
+000040a0: 732e 0a20 2020 203a 7479 7065 2077 7269  s..    :type wri
+000040b0: 7465 5f73 697a 653a 2069 6e74 0a20 2020  te_size: int.   
+000040c0: 203a 7061 7261 6d20 6361 6c6c 6261 636b   :param callback
+000040d0: 3a20 4120 6361 6c6c 6261 636b 2066 756e  : A callback fun
+000040e0: 6374 696f 6e20 7468 6174 2061 6363 6570  ction that accep
+000040f0: 7473 2066 6f75 7220 7061 7261 6d65 7465  ts four paramete
+00004100: 7273 3a20 6060 2874 6f74 616c 5f69 6e70  rs: ``(total_inp
+00004110: 7574 2c20 746f 7461 6c5f 6f75 7470 7574  ut, total_output
+00004120: 2c20 7265 6164 5f64 6174 612c 2077 7269  , read_data, wri
+00004130: 7465 5f64 6174 6129 6060 2e20 5468 6520  te_data)``. The 
+00004140: 6669 7273 7420 7477 6f20 6172 6520 6060  first two are ``
+00004150: 696e 7460 6020 6f62 6a65 6374 732e 2054  int`` objects. T
+00004160: 6865 206c 6173 7420 7477 6f20 6172 6520  he last two are 
+00004170: 7265 6164 6f6e 6c79 2060 6d65 6d6f 7279  readonly `memory
+00004180: 7669 6577 203c 6874 7470 733a 2f2f 646f  view <https://do
+00004190: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+000041a0: 6c69 6272 6172 792f 7374 6474 7970 6573  library/stdtypes
+000041b0: 2e68 746d 6c23 6d65 6d6f 7279 2d76 6965  .html#memory-vie
+000041c0: 7773 3e60 5f20 6f62 6a65 6374 732c 2069  ws>`_ objects, i
+000041d0: 6620 7761 6e74 2074 6f20 7265 6665 7265  f want to refere
+000041e0: 6e63 6520 7468 6520 6461 7461 2028 6f72  nce the data (or
+000041f0: 2069 7473 2073 6c69 6365 2920 6f75 7473   its slice) outs
+00004200: 6964 6520 7468 6520 6361 6c6c 6261 636b  ide the callback
+00004210: 2066 756e 6374 696f 6e2c 2060 636f 6e76   function, `conv
+00004220: 6572 7420 3c68 7474 7073 3a2f 2f64 6f63  ert <https://doc
+00004230: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+00004240: 6962 7261 7279 2f73 7464 7479 7065 732e  ibrary/stdtypes.
+00004250: 6874 6d6c 236d 656d 6f72 7976 6965 772e  html#memoryview.
+00004260: 746f 6279 7465 733e 605f 2074 6865 6d20  tobytes>`_ them 
+00004270: 746f 2060 6062 7974 6573 6060 206f 626a  to ``bytes`` obj
+00004280: 6563 7473 2e20 4966 2069 6e70 7574 2073  ects. If input s
+00004290: 7472 6561 6d20 6973 2060 6062 2727 6060  tream is ``b''``
+000042a0: 2c20 7468 6520 6361 6c6c 6261 636b 2066  , the callback f
+000042b0: 756e 6374 696f 6e20 7769 6c6c 206e 6f74  unction will not
+000042c0: 2062 6520 6361 6c6c 6564 2e0a 2020 2020   be called..    
+000042d0: 3a74 7970 6520 6361 6c6c 6261 636b 3a20  :type callback: 
+000042e0: 6361 6c6c 6162 6c65 0a20 2020 203a 7265  callable.    :re
+000042f0: 7475 726e 3a20 4120 322d 6974 656d 2074  turn: A 2-item t
+00004300: 7570 6c65 2c20 6060 2874 6f74 616c 5f69  uple, ``(total_i
+00004310: 6e70 7574 2c20 746f 7461 6c5f 6f75 7470  nput, total_outp
+00004320: 7574 2960 602c 2074 6865 2069 7465 6d73  ut)``, the items
+00004330: 2061 7265 2060 6069 6e74 6060 206f 626a   are ``int`` obj
+00004340: 6563 7473 2e0a 2020 2020 3a72 6169 7365  ects..    :raise
+00004350: 7320 5a73 7464 4572 726f 723a 2049 6620  s ZstdError: If 
+00004360: 6465 636f 6d70 7265 7373 696f 6e20 6661  decompression fa
+00004370: 696c 732e 0a0a 2020 2020 2e2e 2073 6f75  ils...    .. sou
+00004380: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
+00004390: 0a0a 2020 2020 2020 2020 2320 6465 636f  ..        # deco
+000043a0: 6d70 7265 7373 2061 6e20 696e 7075 7420  mpress an input 
+000043b0: 6669 6c65 2c20 616e 6420 7772 6974 6520  file, and write 
+000043c0: 746f 2061 6e20 6f75 7470 7574 2066 696c  to an output fil
+000043d0: 652e 0a20 2020 2020 2020 2077 6974 6820  e..        with 
+000043e0: 696f 2e6f 7065 6e28 696e 7075 745f 6669  io.open(input_fi
+000043f0: 6c65 5f70 6174 682c 2027 7262 2729 2061  le_path, 'rb') a
+00004400: 7320 6966 683a 0a20 2020 2020 2020 2020  s ifh:.         
+00004410: 2020 2077 6974 6820 696f 2e6f 7065 6e28     with io.open(
+00004420: 6f75 7470 7574 5f66 696c 655f 7061 7468  output_file_path
+00004430: 2c20 2777 6227 2920 6173 206f 6668 3a0a  , 'wb') as ofh:.
+00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004450: 6465 636f 6d70 7265 7373 5f73 7472 6561  decompress_strea
+00004460: 6d28 6966 682c 206f 6668 290a 0a20 2020  m(ifh, ofh)..   
+00004470: 2020 2020 2023 2064 6563 6f6d 7072 6573       # decompres
+00004480: 7320 6120 6279 7465 7320 6f62 6a65 6374  s a bytes object
+00004490: 2c20 616e 6420 7772 6974 6520 746f 2061  , and write to a
+000044a0: 2066 696c 652e 0a20 2020 2020 2020 2077   file..        w
+000044b0: 6974 6820 696f 2e42 7974 6573 494f 2863  ith io.BytesIO(c
+000044c0: 6f6d 7072 6573 7365 645f 6461 7429 2061  ompressed_dat) a
+000044d0: 7320 6269 3a0a 2020 2020 2020 2020 2020  s bi:.          
+000044e0: 2020 7769 7468 2069 6f2e 6f70 656e 286f    with io.open(o
+000044f0: 7574 7075 745f 6669 6c65 5f70 6174 682c  utput_file_path,
+00004500: 2027 7762 2729 2061 7320 6f66 683a 0a20   'wb') as ofh:. 
+00004510: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00004520: 6563 6f6d 7072 6573 735f 7374 7265 616d  ecompress_stream
+00004530: 2862 692c 206f 6668 290a 0a20 2020 2020  (bi, ofh)..     
+00004540: 2020 2023 2044 6563 6f6d 7072 6573 7320     # Decompress 
+00004550: 616e 2069 6e70 7574 2066 696c 652c 206f  an input file, o
+00004560: 6274 6169 6e20 6120 6279 7465 7320 6f62  btain a bytes ob
+00004570: 6a65 6374 2e0a 2020 2020 2020 2020 2320  ject..        # 
+00004580: 4974 2773 2066 6173 7465 7220 7468 616e  It's faster than
+00004590: 2072 6561 6469 6e67 2061 2066 696c 6520   reading a file 
+000045a0: 616e 6420 6465 636f 6d70 7265 7373 696e  and decompressin
+000045b0: 6720 6974 2069 6e0a 2020 2020 2020 2020  g it in.        
+000045c0: 2320 6d65 6d6f 7279 2c20 7465 7374 6564  # memory, tested
+000045d0: 206f 6e20 5562 756e 7475 2850 7974 686f   on Ubuntu(Pytho
+000045e0: 6e33 2e38 292f 5769 6e64 6f77 7328 5079  n3.8)/Windows(Py
+000045f0: 7468 6f6e 332e 3929 2e0a 2020 2020 2020  thon3.9)..      
+00004600: 2020 2320 4d61 7962 6520 7468 6520 4f53    # Maybe the OS
+00004610: 2068 6173 2070 7265 6665 7463 6869 6e67   has prefetching
+00004620: 2c20 6974 2063 616e 2072 6561 6420 616e  , it can read an
+00004630: 6420 6465 636f 6d70 7265 7373 0a20 2020  d decompress.   
+00004640: 2020 2020 2023 2064 6174 6120 696e 2070       # data in p
+00004650: 6172 616c 6c65 6c20 746f 2073 6f6d 6520  arallel to some 
+00004660: 6465 6772 6565 2c20 7265 6164 696e 6720  degree, reading 
+00004670: 6669 6c65 2066 726f 6d20 4844 440a 2020  file from HDD.  
+00004680: 2020 2020 2020 2320 6973 2074 6865 2062        # is the b
+00004690: 6f74 746c 656e 6563 6b20 696e 2074 6869  ottleneck in thi
+000046a0: 7320 6361 7365 2e0a 2020 2020 2020 2020  s case..        
+000046b0: 7769 7468 2069 6f2e 6f70 656e 2869 6e70  with io.open(inp
+000046c0: 7574 5f66 696c 655f 7061 7468 2c20 2772  ut_file_path, 'r
+000046d0: 6227 2920 6173 2069 6668 3a0a 2020 2020  b') as ifh:.    
+000046e0: 2020 2020 2020 2020 7769 7468 2069 6f2e          with io.
+000046f0: 4279 7465 7349 4f28 2920 6173 2062 6f3a  BytesIO() as bo:
+00004700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004710: 2064 6563 6f6d 7072 6573 735f 7374 7265   decompress_stre
+00004720: 616d 2869 6668 2c20 626f 290a 2020 2020  am(ifh, bo).    
+00004730: 2020 2020 2020 2020 2020 2020 6465 636f              deco
+00004740: 6d70 7265 7373 6564 5f64 6174 203d 2062  mpressed_dat = b
+00004750: 6f2e 6765 7476 616c 7565 2829 0a0a 2020  o.getvalue()..  
+00004760: 2020 2020 2020 2320 5072 696e 7420 7072        # Print pr
+00004770: 6f67 7265 7373 2075 7369 6e67 2063 616c  ogress using cal
+00004780: 6c62 6163 6b20 6675 6e63 7469 6f6e 0a20  lback function. 
+00004790: 2020 2020 2020 2064 6566 2064 6563 6f6d         def decom
+000047a0: 7072 6573 735f 7072 696e 745f 7072 6f67  press_print_prog
+000047b0: 7265 7373 2869 6e70 7574 5f66 696c 655f  ress(input_file_
+000047c0: 7061 7468 2c20 6f75 7470 7574 5f66 696c  path, output_fil
+000047d0: 655f 7061 7468 293a 0a20 2020 2020 2020  e_path):.       
+000047e0: 2020 2020 2069 6e70 7574 5f66 696c 655f       input_file_
+000047f0: 7369 7a65 203d 206f 732e 7061 7468 2e67  size = os.path.g
+00004800: 6574 7369 7a65 2869 6e70 7574 5f66 696c  etsize(input_fil
+00004810: 655f 7061 7468 290a 0a20 2020 2020 2020  e_path)..       
+00004820: 2020 2020 2064 6566 2066 756e 6328 746f       def func(to
+00004830: 7461 6c5f 696e 7075 742c 2074 6f74 616c  tal_input, total
+00004840: 5f6f 7574 7075 742c 2072 6561 645f 6461  _output, read_da
+00004850: 7461 2c20 7772 6974 655f 6461 7461 293a  ta, write_data):
+00004860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004870: 2023 2049 6620 696e 7075 7420 7374 7265   # If input stre
+00004880: 616d 2069 7320 656d 7074 792c 2074 6865  am is empty, the
+00004890: 2063 616c 6c62 6163 6b20 6675 6e63 7469   callback functi
+000048a0: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+000048b0: 2020 2023 2077 696c 6c20 6e6f 7420 6265     # will not be
+000048c0: 2063 616c 6c65 642e 2053 6f20 6e6f 205a   called. So no Z
+000048d0: 6572 6f44 6976 6973 696f 6e45 7272 6f72  eroDivisionError
+000048e0: 2068 6572 652e 0a20 2020 2020 2020 2020   here..         
+000048f0: 2020 2020 2020 2070 6572 6365 6e74 203d         percent =
+00004900: 2031 3030 202a 2074 6f74 616c 5f69 6e70   100 * total_inp
+00004910: 7574 202f 2069 6e70 7574 5f66 696c 655f  ut / input_file_
+00004920: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
+00004930: 2020 2020 2070 7269 6e74 2866 2750 726f       print(f'Pro
+00004940: 6772 6573 733a 207b 7065 7263 656e 743a  gress: {percent:
+00004950: 2e31 667d 2527 2c20 656e 643d 275c 7227  .1f}%', end='\r'
+00004960: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
+00004970: 6974 6820 696f 2e6f 7065 6e28 696e 7075  ith io.open(inpu
+00004980: 745f 6669 6c65 5f70 6174 682c 2027 7262  t_file_path, 'rb
+00004990: 2729 2061 7320 6966 683a 0a20 2020 2020  ') as ifh:.     
+000049a0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+000049b0: 696f 2e6f 7065 6e28 6f75 7470 7574 5f66  io.open(output_f
+000049c0: 696c 655f 7061 7468 2c20 2777 6227 2920  ile_path, 'wb') 
+000049d0: 6173 206f 6668 3a0a 2020 2020 2020 2020  as ofh:.        
+000049e0: 2020 2020 2020 2020 2020 2020 6465 636f              deco
+000049f0: 6d70 7265 7373 5f73 7472 6561 6d28 6966  mpress_stream(if
+00004a00: 682c 206f 6668 2c20 6361 6c6c 6261 636b  h, ofh, callback
+00004a10: 3d66 756e 6329 0a0a 0a2e 2e20 7079 3a63  =func)..... py:c
+00004a20: 6c61 7373 3a3a 205a 7374 6444 6563 6f6d  lass:: ZstdDecom
+00004a30: 7072 6573 736f 720a 0a20 2020 2041 2073  pressor..    A s
+00004a40: 7472 6561 6d69 6e67 2064 6563 6f6d 7072  treaming decompr
+00004a50: 6573 736f 722e 0a0a 2020 2020 4166 7465  essor...    Afte
+00004a60: 7220 6120 3a72 6566 3a60 6672 616d 653c  r a :ref:`frame<
+00004a70: 6672 616d 655f 626c 6f63 6b3e 6020 6973  frame_block>` is
+00004a80: 2064 6563 6f6d 7072 6573 7365 642c 2069   decompressed, i
+00004a90: 7420 7374 6f70 7320 616e 6420 7365 7473  t stops and sets
+00004aa0: 203a 7079 3a61 7474 723a 607e 5a73 7464   :py:attr:`~Zstd
+00004ab0: 4465 636f 6d70 7265 7373 6f72 2e65 6f66  Decompressor.eof
+00004ac0: 6020 666c 6167 2074 6f20 6060 5472 7565  ` flag to ``True
+00004ad0: 6060 2e0a 0a20 2020 2046 6f72 206d 756c  ``...    For mul
+00004ae0: 7469 706c 6520 6672 616d 6573 2064 6174  tiple frames dat
+00004af0: 612c 2075 7365 203a 7079 3a63 6c61 7373  a, use :py:class
+00004b00: 3a60 456e 646c 6573 735a 7374 6444 6563  :`EndlessZstdDec
+00004b10: 6f6d 7072 6573 736f 7260 2e0a 0a20 2020  ompressor`...   
+00004b20: 2054 6872 6561 642d 7361 6665 2061 7420   Thread-safe at 
+00004b30: 6d65 7468 6f64 206c 6576 656c 2e0a 0a20  method level... 
+00004b40: 2020 202e 2e20 7079 3a6d 6574 686f 643a     .. py:method:
+00004b50: 3a20 5f5f 696e 6974 5f5f 2873 656c 662c  : __init__(self,
+00004b60: 207a 7374 645f 6469 6374 3d4e 6f6e 652c   zstd_dict=None,
+00004b70: 206f 7074 696f 6e3d 4e6f 6e65 290a 0a20   option=None).. 
+00004b80: 2020 2020 2020 2049 6e69 7469 616c 697a         Initializ
+00004b90: 6520 6120 5a73 7464 4465 636f 6d70 7265  e a ZstdDecompre
+00004ba0: 7373 6f72 206f 626a 6563 742e 0a0a 2020  ssor object...  
+00004bb0: 2020 2020 2020 3a70 6172 616d 207a 7374        :param zst
+00004bc0: 645f 6469 6374 3a20 5072 652d 7472 6169  d_dict: Pre-trai
+00004bd0: 6e65 6420 6469 6374 696f 6e61 7279 2066  ned dictionary f
+00004be0: 6f72 2064 6563 6f6d 7072 6573 7369 6f6e  or decompression
+00004bf0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00004c00: 7a73 7464 5f64 6963 743a 205a 7374 6444  zstd_dict: ZstdD
+00004c10: 6963 740a 2020 2020 2020 2020 3a70 6172  ict.        :par
+00004c20: 616d 2064 6963 7420 6f70 7469 6f6e 3a20  am dict option: 
+00004c30: 4120 6060 6469 6374 6060 206f 626a 6563  A ``dict`` objec
+00004c40: 7420 7468 6174 2063 6f6e 7461 696e 7320  t that contains 
+00004c50: 3a72 6566 3a60 6164 7661 6e63 6564 2064  :ref:`advanced d
+00004c60: 6563 6f6d 7072 6573 7369 6f6e 2070 6172  ecompression par
+00004c70: 616d 6574 6572 733c 4450 6172 616d 6574  ameters<DParamet
+00004c80: 6572 3e60 2e20 5468 6520 6465 6661 756c  er>`. The defaul
+00004c90: 7420 7661 6c75 6520 6060 4e6f 6e65 6060  t value ``None``
+00004ca0: 206d 6561 6e73 2074 6f20 7573 6520 7a73   means to use zs
+00004cb0: 7464 2773 2064 6566 6175 6c74 2064 6563  td's default dec
+00004cc0: 6f6d 7072 6573 7369 6f6e 2070 6172 616d  ompression param
+00004cd0: 6574 6572 732e 0a0a 2020 2020 2e2e 2070  eters...    .. p
+00004ce0: 793a 6d65 7468 6f64 3a3a 2064 6563 6f6d  y:method:: decom
+00004cf0: 7072 6573 7328 7365 6c66 2c20 6461 7461  press(self, data
+00004d00: 2c20 6d61 785f 6c65 6e67 7468 3d2d 3129  , max_length=-1)
+00004d10: 0a0a 2020 2020 2020 2020 4465 636f 6d70  ..        Decomp
+00004d20: 7265 7373 202a 6461 7461 2a2c 2072 6574  ress *data*, ret
+00004d30: 7572 6e69 6e67 2064 6563 6f6d 7072 6573  urning decompres
+00004d40: 7365 6420 6461 7461 2061 7320 6120 6060  sed data as a ``
+00004d50: 6279 7465 7360 6020 6f62 6a65 6374 2e0a  bytes`` object..
+00004d60: 0a20 2020 2020 2020 2041 6674 6572 2061  .        After a
+00004d70: 203a 7265 663a 6066 7261 6d65 3c66 7261   :ref:`frame<fra
+00004d80: 6d65 5f62 6c6f 636b 3e60 2069 7320 6465  me_block>` is de
+00004d90: 636f 6d70 7265 7373 6564 2c20 6974 2073  compressed, it s
+00004da0: 746f 7073 2061 6e64 2073 6574 7320 3a70  tops and sets :p
+00004db0: 793a 6174 7472 3a60 7e5a 7374 6444 6563  y:attr:`~ZstdDec
+00004dc0: 6f6d 7072 6573 736f 722e 656f 6660 2066  ompressor.eof` f
+00004dd0: 6c61 6720 746f 2060 6054 7275 6560 602e  lag to ``True``.
+00004de0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00004df0: 2064 6174 613a 2044 6174 6120 746f 2062   data: Data to b
+00004e00: 6520 6465 636f 6d70 7265 7373 6564 2e0a  e decompressed..
+00004e10: 2020 2020 2020 2020 3a74 7970 6520 6461          :type da
+00004e20: 7461 3a20 6279 7465 732d 6c69 6b65 206f  ta: bytes-like o
+00004e30: 626a 6563 740a 2020 2020 2020 2020 3a70  bject.        :p
+00004e40: 6172 616d 2069 6e74 206d 6178 5f6c 656e  aram int max_len
+00004e50: 6774 683a 204d 6178 696d 756d 2073 697a  gth: Maximum siz
+00004e60: 6520 6f66 2072 6574 7572 6e65 6420 6461  e of returned da
+00004e70: 7461 2e20 5768 656e 2069 7427 7320 6e65  ta. When it's ne
+00004e80: 6761 7469 7665 2c20 7468 6520 6f75 7470  gative, the outp
+00004e90: 7574 2073 697a 6520 6973 2075 6e6c 696d  ut size is unlim
+00004ea0: 6974 6564 2e20 5768 656e 2069 7427 7320  ited. When it's 
+00004eb0: 6e6f 6e2d 6e65 6761 7469 7665 2c20 7265  non-negative, re
+00004ec0: 7475 726e 7320 6174 206d 6f73 7420 2a6d  turns at most *m
+00004ed0: 6178 5f6c 656e 6774 682a 2062 7974 6573  ax_length* bytes
+00004ee0: 206f 6620 6465 636f 6d70 7265 7373 6564   of decompressed
+00004ef0: 2064 6174 612e 2049 6620 7468 6973 206c   data. If this l
+00004f00: 696d 6974 2069 7320 7265 6163 6865 6420  imit is reached 
+00004f10: 616e 6420 6675 7274 6865 7220 6f75 7470  and further outp
+00004f20: 7574 2063 616e 2028 6f72 206d 6179 2920  ut can (or may) 
+00004f30: 6265 2070 726f 6475 6365 642c 2074 6865  be produced, the
+00004f40: 203a 7079 3a61 7474 723a 607e 5a73 7464   :py:attr:`~Zstd
+00004f50: 4465 636f 6d70 7265 7373 6f72 2e6e 6565  Decompressor.nee
+00004f60: 6473 5f69 6e70 7574 6020 6174 7472 6962  ds_input` attrib
+00004f70: 7574 6520 7769 6c6c 2062 6520 7365 7420  ute will be set 
+00004f80: 746f 2060 6046 616c 7365 6060 2e20 496e  to ``False``. In
+00004f90: 2074 6869 7320 6361 7365 2c20 7468 6520   this case, the 
+00004fa0: 6e65 7874 2063 616c 6c20 746f 2074 6869  next call to thi
+00004fb0: 7320 6d65 7468 6f64 206d 6179 2070 726f  s method may pro
+00004fc0: 7669 6465 202a 6461 7461 2a20 6173 2060  vide *data* as `
+00004fd0: 6062 2727 6060 2074 6f20 6f62 7461 696e  `b''`` to obtain
+00004fe0: 206d 6f72 6520 6f66 2074 6865 206f 7574   more of the out
+00004ff0: 7075 742e 0a0a 2020 2020 2e2e 2070 793a  put...    .. py:
+00005000: 6174 7472 6962 7574 653a 3a20 6e65 6564  attribute:: need
+00005010: 735f 696e 7075 740a 0a20 2020 2020 2020  s_input..       
+00005020: 2049 6620 7468 6520 2a6d 6178 5f6c 656e   If the *max_len
+00005030: 6774 682a 206f 7574 7075 7420 6c69 6d69  gth* output limi
+00005040: 7420 696e 203a 7079 3a6d 6574 683a 607e  t in :py:meth:`~
+00005050: 5a73 7464 4465 636f 6d70 7265 7373 6f72  ZstdDecompressor
+00005060: 2e64 6563 6f6d 7072 6573 7360 206d 6574  .decompress` met
+00005070: 686f 6420 6861 7320 6265 656e 2072 6561  hod has been rea
+00005080: 6368 6564 2c20 616e 6420 7468 6520 6465  ched, and the de
+00005090: 636f 6d70 7265 7373 6f72 2068 6173 2028  compressor has (
+000050a0: 6f72 206d 6179 2068 6173 2920 756e 636f  or may has) unco
+000050b0: 6e73 756d 6564 2069 6e70 7574 2064 6174  nsumed input dat
+000050c0: 612c 2069 7420 7769 6c6c 2062 6520 7365  a, it will be se
+000050d0: 7420 746f 2060 6046 616c 7365 6060 2e20  t to ``False``. 
+000050e0: 496e 2074 6869 7320 6361 7365 2c20 7061  In this case, pa
+000050f0: 7373 2060 6062 2727 6060 2074 6f20 3a70  ss ``b''`` to :p
+00005100: 793a 6d65 7468 3a60 7e5a 7374 6444 6563  y:meth:`~ZstdDec
+00005110: 6f6d 7072 6573 736f 722e 6465 636f 6d70  ompressor.decomp
+00005120: 7265 7373 6020 6d65 7468 6f64 206d 6179  ress` method may
+00005130: 206f 7574 7075 7420 6675 7274 6865 7220   output further 
+00005140: 6461 7461 2e0a 0a20 2020 2020 2020 2049  data...        I
+00005150: 6620 6967 6e6f 7265 2074 6869 7320 6174  f ignore this at
+00005160: 7472 6962 7574 6520 7768 656e 2074 6865  tribute when the
+00005170: 7265 2069 7320 756e 636f 6e73 756d 6564  re is unconsumed
+00005180: 2069 6e70 7574 2064 6174 612c 2074 6865   input data, the
+00005190: 7265 2077 696c 6c20 6265 2061 206c 6974  re will be a lit
+000051a0: 746c 6520 7065 7266 6f72 6d61 6e63 6520  tle performance 
+000051b0: 6c6f 7373 2062 6563 6175 7365 206f 6620  loss because of 
+000051c0: 6578 7472 6120 6d65 6d6f 7279 2063 6f70  extra memory cop
+000051d0: 792e 0a0a 2020 2020 2e2e 2070 793a 6174  y...    .. py:at
+000051e0: 7472 6962 7574 653a 3a20 656f 660a 0a20  tribute:: eof.. 
+000051f0: 2020 2020 2020 2060 6054 7275 6560 6020         ``True`` 
+00005200: 6d65 616e 7320 7468 6520 656e 6420 6f66  means the end of
+00005210: 2074 6865 2066 6972 7374 2066 7261 6d65   the first frame
+00005220: 2068 6173 2062 6565 6e20 7265 6163 6865   has been reache
+00005230: 642e 2049 6620 6465 636f 6d70 7265 7373  d. If decompress
+00005240: 2064 6174 6120 6166 7465 7220 7468 6174   data after that
+00005250: 2c20 616e 2060 6045 4f46 4572 726f 7260  , an ``EOFError`
+00005260: 6020 6578 6365 7074 696f 6e20 7769 6c6c  ` exception will
+00005270: 2062 6520 7261 6973 6564 2e0a 0a20 2020   be raised...   
+00005280: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+00005290: 3a3a 2075 6e75 7365 645f 6461 7461 0a0a  :: unused_data..
+000052a0: 2020 2020 2020 2020 4120 6279 7465 7320          A bytes 
+000052b0: 6f62 6a65 6374 2e20 5768 656e 205a 7374  object. When Zst
+000052c0: 6444 6563 6f6d 7072 6573 736f 7220 6f62  dDecompressor ob
+000052d0: 6a65 6374 2073 746f 7073 2061 6674 6572  ject stops after
+000052e0: 2064 6563 6f6d 7072 6573 7369 6e67 2061   decompressing a
+000052f0: 2066 7261 6d65 2c20 756e 7573 6564 2069   frame, unused i
+00005300: 6e70 7574 2064 6174 6120 6166 7465 7220  nput data after 
+00005310: 7468 6520 6669 7273 7420 6672 616d 652e  the first frame.
+00005320: 204f 7468 6572 7769 7365 2074 6869 7320   Otherwise this 
+00005330: 7769 6c6c 2062 6520 6060 6227 2760 602e  will be ``b''``.
+00005340: 0a0a 2020 2020 2e2e 2073 6f75 7263 6563  ..    .. sourcec
+00005350: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00005360: 2020 2020 2020 2320 2d2d 2d20 756e 6c69        # --- unli
+00005370: 6d69 7465 6420 6f75 7470 7574 202d 2d2d  mited output ---
+00005380: 0a20 2020 2020 2020 2064 3120 3d20 5a73  .        d1 = Zs
+00005390: 7464 4465 636f 6d70 7265 7373 6f72 2829  tdDecompressor()
+000053a0: 0a0a 2020 2020 2020 2020 6465 636f 6d70  ..        decomp
+000053b0: 7265 7373 6564 5f64 6174 3120 3d20 6431  ressed_dat1 = d1
+000053c0: 2e64 6563 6f6d 7072 6573 7328 6461 7431  .decompress(dat1
+000053d0: 290a 2020 2020 2020 2020 6465 636f 6d70  ).        decomp
+000053e0: 7265 7373 6564 5f64 6174 3220 3d20 6431  ressed_dat2 = d1
+000053f0: 2e64 6563 6f6d 7072 6573 7328 6461 7432  .decompress(dat2
+00005400: 290a 2020 2020 2020 2020 6465 636f 6d70  ).        decomp
+00005410: 7265 7373 6564 5f64 6174 3320 3d20 6431  ressed_dat3 = d1
+00005420: 2e64 6563 6f6d 7072 6573 7328 6461 7433  .decompress(dat3
+00005430: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00005440: 7420 6431 2e65 6f66 2c20 2764 6174 6120  t d1.eof, 'data 
+00005450: 6973 2061 6e20 696e 636f 6d70 6c65 7465  is an incomplete
+00005460: 207a 7374 6420 6672 616d 652e 270a 0a20   zstd frame.'.. 
+00005470: 2020 2020 2020 2023 202d 2d2d 206c 696d         # --- lim
+00005480: 6974 6564 206f 7574 7075 7420 2d2d 2d0a  ited output ---.
+00005490: 2020 2020 2020 2020 6432 203d 205a 7374          d2 = Zst
+000054a0: 6444 6563 6f6d 7072 6573 736f 7228 290a  dDecompressor().
+000054b0: 0a20 2020 2020 2020 2077 6869 6c65 2054  .        while T
+000054c0: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
+000054d0: 2069 6620 6432 2e6e 6565 6473 5f69 6e70   if d2.needs_inp
+000054e0: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
+000054f0: 2020 2020 6461 7420 3d20 7265 6164 5f69      dat = read_i
+00005500: 6e70 7574 2832 2a31 3032 342a 3130 3234  nput(2*1024*1024
+00005510: 2920 2320 7265 6164 2032 204d 6942 2069  ) # read 2 MiB i
+00005520: 6e70 7574 2064 6174 610a 2020 2020 2020  nput data.      
+00005530: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00005540: 2064 6174 3a20 2320 696e 7075 7420 7374   dat: # input st
+00005550: 7265 616d 2065 6e64 730a 2020 2020 2020  ream ends.      
+00005560: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00005570: 6973 6520 4578 6365 7074 696f 6e28 2749  ise Exception('I
+00005580: 6e70 7574 2073 7472 6561 6d20 656e 6473  nput stream ends
+00005590: 2c20 6275 7420 7468 6520 656e 6420 6f66  , but the end of
+000055a0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055c0: 2020 2020 2020 2027 7468 6520 6669 7273         'the firs
+000055d0: 7420 6672 616d 6520 6973 206e 6f74 2072  t frame is not r
+000055e0: 6561 6368 6564 2e27 290a 2020 2020 2020  eached.').      
+000055f0: 2020 2020 2020 656c 7365 3a20 2320 6d61        else: # ma
+00005600: 7962 6520 7468 6572 6520 6973 2075 6e63  ybe there is unc
+00005610: 6f6e 7375 6d65 6420 696e 7075 7420 6461  onsumed input da
+00005620: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
+00005630: 2020 2064 6174 203d 2062 2727 0a0a 2020     dat = b''..  
+00005640: 2020 2020 2020 2020 2020 6368 756e 6b20            chunk 
+00005650: 3d20 6432 2e64 6563 6f6d 7072 6573 7328  = d2.decompress(
+00005660: 6461 742c 2031 302a 3130 3234 2a31 3032  dat, 10*1024*102
+00005670: 3429 2023 206c 696d 6974 206f 7574 7075  4) # limit outpu
+00005680: 7420 6275 6666 6572 2074 6f20 3130 204d  t buffer to 10 M
+00005690: 6942 0a20 2020 2020 2020 2020 2020 2077  iB.            w
+000056a0: 7269 7465 5f6f 7574 7075 7428 6368 756e  rite_output(chun
+000056b0: 6b29 0a0a 2020 2020 2020 2020 2020 2020  k)..            
+000056c0: 6966 2064 322e 656f 663a 2023 2072 6561  if d2.eof: # rea
+000056d0: 6368 2074 6865 2065 6e64 206f 6620 7468  ch the end of th
+000056e0: 6520 6669 7273 7420 6672 616d 650a 2020  e first frame.  
+000056f0: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00005700: 6561 6b0a 0a0a 2e2e 2070 793a 636c 6173  eak..... py:clas
+00005710: 733a 3a20 456e 646c 6573 735a 7374 6444  s:: EndlessZstdD
+00005720: 6563 6f6d 7072 6573 736f 720a 0a20 2020  ecompressor..   
+00005730: 2041 2073 7472 6561 6d69 6e67 2064 6563   A streaming dec
+00005740: 6f6d 7072 6573 736f 722e 0a0a 2020 2020  ompressor...    
+00005750: 4974 2064 6f65 736e 2774 2073 746f 7020  It doesn't stop 
+00005760: 6166 7465 7220 6120 3a72 6566 3a60 6672  after a :ref:`fr
+00005770: 616d 653c 6672 616d 655f 626c 6f63 6b3e  ame<frame_block>
+00005780: 6020 6973 2064 6563 6f6d 7072 6573 7365  ` is decompresse
+00005790: 642c 2063 616e 2062 6520 7573 6564 2074  d, can be used t
+000057a0: 6f20 6465 636f 6d70 7265 7373 206d 756c  o decompress mul
+000057b0: 7469 706c 6520 636f 6e63 6174 656e 6174  tiple concatenat
+000057c0: 6564 2066 7261 6d65 732e 0a0a 2020 2020  ed frames...    
+000057d0: 5468 7265 6164 2d73 6166 6520 6174 206d  Thread-safe at m
+000057e0: 6574 686f 6420 6c65 7665 6c2e 0a0a 2020  ethod level...  
+000057f0: 2020 2e2e 2070 793a 6d65 7468 6f64 3a3a    .. py:method::
+00005800: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00005810: 7a73 7464 5f64 6963 743d 4e6f 6e65 2c20  zstd_dict=None, 
+00005820: 6f70 7469 6f6e 3d4e 6f6e 6529 0a0a 2020  option=None)..  
+00005830: 2020 2020 2020 5468 6520 7061 7261 6d65        The parame
+00005840: 7465 7273 2061 7265 2074 6865 2073 616d  ters are the sam
+00005850: 6520 6173 203a 7079 3a6d 6574 683a 605a  e as :py:meth:`Z
+00005860: 7374 6444 6563 6f6d 7072 6573 736f 722e  stdDecompressor.
+00005870: 5f5f 696e 6974 5f5f 6020 6d65 7468 6f64  __init__` method
+00005880: 2e0a 0a20 2020 202e 2e20 7079 3a6d 6574  ...    .. py:met
+00005890: 686f 643a 3a20 6465 636f 6d70 7265 7373  hod:: decompress
+000058a0: 2873 656c 662c 2064 6174 612c 206d 6178  (self, data, max
+000058b0: 5f6c 656e 6774 683d 2d31 290a 0a20 2020  _length=-1)..   
+000058c0: 2020 2020 2054 6865 2070 6172 616d 6574       The paramet
+000058d0: 6572 7320 6172 6520 7468 6520 7361 6d65  ers are the same
+000058e0: 2061 7320 3a70 793a 6d65 7468 3a60 5a73   as :py:meth:`Zs
+000058f0: 7464 4465 636f 6d70 7265 7373 6f72 2e64  tdDecompressor.d
+00005900: 6563 6f6d 7072 6573 7360 206d 6574 686f  ecompress` metho
+00005910: 642e 0a0a 2020 2020 2020 2020 4166 7465  d...        Afte
+00005920: 7220 6465 636f 6d70 7265 7373 696e 6720  r decompressing 
+00005930: 6120 6672 616d 652c 2069 7420 646f 6573  a frame, it does
+00005940: 6e27 7420 7374 6f70 206c 696b 6520 3a70  n't stop like :p
+00005950: 793a 6d65 7468 3a60 5a73 7464 4465 636f  y:meth:`ZstdDeco
+00005960: 6d70 7265 7373 6f72 2e64 6563 6f6d 7072  mpressor.decompr
+00005970: 6573 7360 2e0a 0a20 2020 202e 2e20 7079  ess`...    .. py
+00005980: 3a61 7474 7269 6275 7465 3a3a 206e 6565  :attribute:: nee
+00005990: 6473 5f69 6e70 7574 0a0a 2020 2020 2020  ds_input..      
+000059a0: 2020 4974 2773 2074 6865 2073 616d 6520    It's the same 
+000059b0: 6173 203a 7079 3a61 7474 723a 605a 7374  as :py:attr:`Zst
+000059c0: 6444 6563 6f6d 7072 6573 736f 722e 6e65  dDecompressor.ne
+000059d0: 6564 735f 696e 7075 7460 2e0a 0a20 2020  eds_input`...   
+000059e0: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+000059f0: 3a3a 2061 745f 6672 616d 655f 6564 6765  :: at_frame_edge
+00005a00: 0a0a 2020 2020 2020 2020 6060 5472 7565  ..        ``True
+00005a10: 6060 2077 6865 6e20 626f 7468 2074 6865  `` when both the
+00005a20: 2069 6e70 7574 2061 6e64 206f 7574 7075   input and outpu
+00005a30: 7420 7374 7265 616d 7320 6172 6520 6174  t streams are at
+00005a40: 2061 203a 7265 663a 6066 7261 6d65 3c66   a :ref:`frame<f
+00005a50: 7261 6d65 5f62 6c6f 636b 3e60 2065 6467  rame_block>` edg
+00005a60: 652c 206f 7220 7468 6520 6465 636f 6d70  e, or the decomp
+00005a70: 7265 7373 6f72 206a 7573 7420 6265 2069  ressor just be i
+00005a80: 6e69 7469 616c 697a 6564 2e0a 0a20 2020  nitialized...   
+00005a90: 2020 2020 2054 6869 7320 666c 6167 2063       This flag c
+00005aa0: 6f75 6c64 2062 6520 7573 6564 2074 6f20  ould be used to 
+00005ab0: 6368 6563 6b20 6461 7461 2069 6e74 6567  check data integ
+00005ac0: 7269 7479 2069 6e20 736f 6d65 2063 6173  rity in some cas
+00005ad0: 6573 2e0a 0a20 2020 202e 2e20 736f 7572  es...    .. sour
+00005ae0: 6365 636f 6465 3a3a 2070 7974 686f 6e0a  cecode:: python.
+00005af0: 0a20 2020 2020 2020 2023 202d 2d2d 2073  .        # --- s
+00005b00: 7472 6561 6d69 6e67 2064 6563 6f6d 7072  treaming decompr
+00005b10: 6573 7369 6f6e 2c20 756e 6c69 6d69 7465  ession, unlimite
+00005b20: 6420 6f75 7470 7574 202d 2d2d 0a20 2020  d output ---.   
+00005b30: 2020 2020 2064 3120 3d20 456e 646c 6573       d1 = Endles
+00005b40: 735a 7374 6444 6563 6f6d 7072 6573 736f  sZstdDecompresso
+00005b50: 7228 290a 0a20 2020 2020 2020 2064 6563  r()..        dec
+00005b60: 6f6d 7072 6573 7365 645f 6461 7431 203d  ompressed_dat1 =
+00005b70: 2064 312e 6465 636f 6d70 7265 7373 2864   d1.decompress(d
+00005b80: 6174 3129 0a20 2020 2020 2020 2064 6563  at1).        dec
+00005b90: 6f6d 7072 6573 7365 645f 6461 7432 203d  ompressed_dat2 =
+00005ba0: 2064 312e 6465 636f 6d70 7265 7373 2864   d1.decompress(d
+00005bb0: 6174 3229 0a20 2020 2020 2020 2064 6563  at2).        dec
+00005bc0: 6f6d 7072 6573 7365 645f 6461 7433 203d  ompressed_dat3 =
+00005bd0: 2064 312e 6465 636f 6d70 7265 7373 2864   d1.decompress(d
+00005be0: 6174 3329 0a0a 2020 2020 2020 2020 6173  at3)..        as
+00005bf0: 7365 7274 2064 312e 6174 5f66 7261 6d65  sert d1.at_frame
+00005c00: 5f65 6467 652c 2027 6461 7461 2065 6e64  _edge, 'data end
+00005c10: 7320 696e 2061 6e20 696e 636f 6d70 6c65  s in an incomple
+00005c20: 7465 2066 7261 6d65 2e27 0a0a 2020 2020  te frame.'..    
+00005c30: 2020 2020 2320 2d2d 2d20 7374 7265 616d      # --- stream
+00005c40: 696e 6720 6465 636f 6d70 7265 7373 696f  ing decompressio
+00005c50: 6e2c 206c 696d 6974 6564 206f 7574 7075  n, limited outpu
+00005c60: 7420 2d2d 2d0a 2020 2020 2020 2020 6432  t ---.        d2
+00005c70: 203d 2045 6e64 6c65 7373 5a73 7464 4465   = EndlessZstdDe
+00005c80: 636f 6d70 7265 7373 6f72 2829 0a0a 2020  compressor()..  
+00005c90: 2020 2020 2020 7768 696c 6520 5472 7565        while True
+00005ca0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00005cb0: 2064 322e 6e65 6564 735f 696e 7075 743a   d2.needs_input:
+00005cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005cd0: 2064 6174 203d 2072 6561 645f 696e 7075   dat = read_inpu
+00005ce0: 7428 322a 3130 3234 2a31 3032 3429 2023  t(2*1024*1024) #
+00005cf0: 2072 6561 6420 3220 4d69 4220 696e 7075   read 2 MiB inpu
+00005d00: 7420 6461 7461 0a20 2020 2020 2020 2020  t data.         
+00005d10: 2020 2020 2020 2069 6620 6e6f 7420 6461         if not da
+00005d20: 743a 2023 2069 6e70 7574 2073 7472 6561  t: # input strea
+00005d30: 6d20 656e 6473 0a20 2020 2020 2020 2020  m ends.         
+00005d40: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00005d50: 7420 6432 2e61 745f 6672 616d 655f 6564  t d2.at_frame_ed
+00005d60: 6765 3a0a 2020 2020 2020 2020 2020 2020  ge:.            
+00005d70: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00005d80: 6520 4578 6365 7074 696f 6e28 2764 6174  e Exception('dat
+00005d90: 6120 656e 6473 2069 6e20 616e 2069 6e63  a ends in an inc
+00005da0: 6f6d 706c 6574 6520 6672 616d 652e 2729  omplete frame.')
+00005db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005dc0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+00005dd0: 2020 2020 2020 2065 6c73 653a 2023 206d         else: # m
+00005de0: 6179 6265 2074 6865 7265 2069 7320 756e  aybe there is un
+00005df0: 636f 6e73 756d 6564 2069 6e70 7574 2064  consumed input d
+00005e00: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+00005e10: 2020 2020 6461 7420 3d20 6227 270a 0a20      dat = b''.. 
+00005e20: 2020 2020 2020 2020 2020 2063 6875 6e6b             chunk
+00005e30: 203d 2064 322e 6465 636f 6d70 7265 7373   = d2.decompress
+00005e40: 2864 6174 2c20 3130 2a31 3032 342a 3130  (dat, 10*1024*10
+00005e50: 3234 2920 2320 6c69 6d69 7420 6f75 7470  24) # limit outp
+00005e60: 7574 2062 7566 6665 7220 746f 2031 3020  ut buffer to 10 
+00005e70: 4d69 420a 2020 2020 2020 2020 2020 2020  MiB.            
+00005e80: 7772 6974 655f 6f75 7470 7574 2863 6875  write_output(chu
+00005e90: 6e6b 290a 0a20 2020 202e 2e20 6869 6e74  nk)..    .. hint
+00005ea0: 3a3a 2057 6879 203a 7079 3a63 6c61 7373  :: Why :py:class
+00005eb0: 3a60 456e 646c 6573 735a 7374 6444 6563  :`EndlessZstdDec
+00005ec0: 6f6d 7072 6573 736f 7260 2064 6f65 736e  ompressor` doesn
+00005ed0: 2774 2073 746f 7020 6174 2066 7261 6d65  't stop at frame
+00005ee0: 2065 6467 6573 3f0a 0a20 2020 2020 2020   edges?..       
+00005ef0: 2049 6620 736f 2c20 756e 7573 6564 2069   If so, unused i
+00005f00: 6e70 7574 2064 6174 6120 6166 7465 7220  nput data after 
+00005f10: 616e 2065 6467 6520 7769 6c6c 2062 6520  an edge will be 
+00005f20: 636f 7069 6564 2074 6f20 616e 2069 6e74  copied to an int
+00005f30: 6572 6e61 6c20 6275 6666 6572 2c20 7468  ernal buffer, th
+00005f40: 6973 206d 6179 2062 6520 6120 7065 7266  is may be a perf
+00005f50: 6f72 6d61 6e63 6520 6f76 6572 6865 6164  ormance overhead
+00005f60: 2e0a 0a20 2020 2020 2020 2049 6620 7761  ...        If wa
+00005f70: 6e74 2074 6f20 7374 6f70 2061 7420 6672  nt to stop at fr
+00005f80: 616d 6520 6564 6765 732c 2077 7269 7465  ame edges, write
+00005f90: 2061 2077 7261 7070 6572 2075 7369 6e67   a wrapper using
+00005fa0: 203a 7079 3a63 6c61 7373 3a60 5a73 7464   :py:class:`Zstd
+00005fb0: 4465 636f 6d70 7265 7373 6f72 6020 636c  Decompressor` cl
+00005fc0: 6173 732e 2041 6e64 2064 6f6e 2774 2066  ass. And don't f
+00005fd0: 6565 6420 746f 6f20 6d75 6368 2064 6174  eed too much dat
+00005fe0: 6120 6576 6572 7920 7469 6d65 2c20 7468  a every time, th
+00005ff0: 6520 6f76 6572 6865 6164 206f 6620 636f  e overhead of co
+00006000: 7079 696e 6720 756e 7573 6564 2069 6e70  pying unused inp
+00006010: 7574 2064 6174 6120 746f 203a 7079 3a61  ut data to :py:a
+00006020: 7474 723a 605a 7374 6444 6563 6f6d 7072  ttr:`ZstdDecompr
+00006030: 6573 736f 722e 756e 7573 6564 5f64 6174  essor.unused_dat
+00006040: 6160 2061 7474 7269 6275 7465 2073 7469  a` attribute sti
+00006050: 6c6c 2065 7869 7374 732e 0a0a 0a2e 2e20  ll exists...... 
+00006060: 5f7a 7374 645f 6469 6374 3a0a 0a44 6963  _zstd_dict:..Dic
+00006070: 7469 6f6e 6172 790a 2d2d 2d2d 2d2d 2d2d  tionary.--------
+00006080: 2d2d 0a0a 2020 2020 5468 6973 2073 6563  --..    This sec
+00006090: 7469 6f6e 2063 6f6e 7461 696e 733a 0a0a  tion contains:..
+000060a0: 2020 2020 2020 2020 2a20 636c 6173 7320          * class 
+000060b0: 3a70 793a 636c 6173 733a 605a 7374 6444  :py:class:`ZstdD
+000060c0: 6963 7460 0a20 2020 2020 2020 202a 2066  ict`.        * f
+000060d0: 756e 6374 696f 6e20 3a70 793a 6675 6e63  unction :py:func
+000060e0: 3a60 7472 6169 6e5f 6469 6374 600a 2020  :`train_dict`.  
+000060f0: 2020 2020 2020 2a20 6675 6e63 7469 6f6e        * function
+00006100: 203a 7079 3a66 756e 633a 6066 696e 616c   :py:func:`final
+00006110: 697a 655f 6469 6374 600a 0a2e 2e20 6e6f  ize_dict`.... no
+00006120: 7465 3a3a 0a20 2020 2049 6620 7573 6520  te::.    If use 
+00006130: 7072 652d 7472 6169 6e65 6420 7a73 7464  pre-trained zstd
+00006140: 2064 6963 7469 6f6e 6172 792c 2074 6865   dictionary, the
+00006150: 2063 6f6d 7072 6573 7369 6f6e 2072 6174   compression rat
+00006160: 696f 2061 6368 6965 7661 626c 6520 6f6e  io achievable on
+00006170: 2073 6d61 6c6c 2064 6174 6120 2861 2066   small data (a f
+00006180: 6577 204b 6942 2920 696d 7072 6f76 6573  ew KiB) improves
+00006190: 2064 7261 6d61 7469 6361 6c6c 792e 0a0a   dramatically...
+000061a0: 2020 2020 2a2a 4261 636b 6772 6f75 6e64      **Background
+000061b0: 2a2a 0a0a 2020 2020 5468 6520 736d 616c  **..    The smal
+000061c0: 6c65 7220 7468 6520 616d 6f75 6e74 206f  ler the amount o
+000061d0: 6620 6461 7461 2074 6f20 636f 6d70 7265  f data to compre
+000061e0: 7373 2c20 7468 6520 6d6f 7265 2064 6966  ss, the more dif
+000061f0: 6669 6375 6c74 2069 7420 6973 2074 6f20  ficult it is to 
+00006200: 636f 6d70 7265 7373 2e20 5468 6973 2070  compress. This p
+00006210: 726f 626c 656d 2069 7320 636f 6d6d 6f6e  roblem is common
+00006220: 2074 6f20 616c 6c20 636f 6d70 7265 7373   to all compress
+00006230: 696f 6e20 616c 676f 7269 7468 6d73 2c20  ion algorithms, 
+00006240: 616e 6420 7265 6173 6f6e 2069 732c 2063  and reason is, c
+00006250: 6f6d 7072 6573 7369 6f6e 2061 6c67 6f72  ompression algor
+00006260: 6974 686d 7320 6c65 6172 6e20 6672 6f6d  ithms learn from
+00006270: 2070 6173 7420 6461 7461 2068 6f77 2074   past data how t
+00006280: 6f20 636f 6d70 7265 7373 2066 7574 7572  o compress futur
+00006290: 6520 6461 7461 2e20 4275 7420 6174 2074  e data. But at t
+000062a0: 6865 2062 6567 696e 6e69 6e67 206f 6620  he beginning of 
+000062b0: 6120 6e65 7720 6461 7461 2073 6574 2c20  a new data set, 
+000062c0: 7468 6572 6520 6973 206e 6f20 2270 6173  there is no "pas
+000062d0: 7422 2074 6f20 6275 696c 6420 7570 6f6e  t" to build upon
+000062e0: 2e0a 0a20 2020 205a 7374 6420 7472 6169  ...    Zstd trai
+000062f0: 6e69 6e67 206d 6f64 6520 6361 6e20 6265  ning mode can be
+00006300: 2075 7365 6420 746f 2074 756e 6520 7468   used to tune th
+00006310: 6520 616c 676f 7269 7468 6d20 666f 7220  e algorithm for 
+00006320: 6120 7365 6c65 6374 6564 2074 7970 6520  a selected type 
+00006330: 6f66 2064 6174 612e 2054 7261 696e 696e  of data. Trainin
+00006340: 6720 6973 2061 6368 6965 7665 6420 6279  g is achieved by
+00006350: 2070 726f 7669 6469 6e67 2069 7420 7769   providing it wi
+00006360: 7468 2061 2066 6577 2073 616d 706c 6573  th a few samples
+00006370: 2028 6f6e 6520 6669 6c65 2070 6572 2073   (one file per s
+00006380: 616d 706c 6529 2e20 5468 6520 7265 7375  ample). The resu
+00006390: 6c74 206f 6620 7468 6973 2074 7261 696e  lt of this train
+000063a0: 696e 6720 6973 2073 746f 7265 6420 696e  ing is stored in
+000063b0: 2061 2066 696c 6520 6361 6c6c 6564 2022   a file called "
+000063c0: 6469 6374 696f 6e61 7279 222c 2077 6869  dictionary", whi
+000063d0: 6368 206d 7573 7420 6265 206c 6f61 6465  ch must be loade
+000063e0: 6420 6265 666f 7265 2063 6f6d 7072 6573  d before compres
+000063f0: 7369 6f6e 2061 6e64 2064 6563 6f6d 7072  sion and decompr
+00006400: 6573 7369 6f6e 2e0a 0a20 2020 2053 6565  ession...    See
+00006410: 2074 6865 2046 4151 2069 6e20 6074 6869   the FAQ in `thi
+00006420: 7320 6669 6c65 203c 6874 7470 733a 2f2f  s file <https://
+00006430: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
+00006440: 6f6f 6b2f 7a73 7464 2f62 6c6f 622f 6465  ook/zstd/blob/de
+00006450: 762f 6c69 622f 7a64 6963 742e 683e 605f  v/lib/zdict.h>`_
+00006460: 2066 6f72 2064 6574 6169 6c73 2e0a 0a20   for details... 
+00006470: 2020 202e 2e20 6174 7465 6e74 696f 6e3a     .. attention:
+00006480: 3a0a 0a20 2020 2020 2020 2023 2e20 4966  :..        #. If
+00006490: 2079 6f75 206c 6f73 6520 6120 7a73 7464   you lose a zstd
+000064a0: 2064 6963 7469 6f6e 6172 792c 2074 6865   dictionary, the
+000064b0: 6e20 6361 6e27 7420 6465 636f 6d70 7265  n can't decompre
+000064c0: 7373 2074 6865 2063 6f72 7265 7370 6f6e  ss the correspon
+000064d0: 6469 6e67 2064 6174 612e 0a20 2020 2020  ding data..     
+000064e0: 2020 2023 2e20 5a73 7464 2064 6963 7469     #. Zstd dicti
+000064f0: 6f6e 6172 7920 6861 7320 6e65 676c 6967  onary has neglig
+00006500: 6962 6c65 2065 6666 6563 7420 6f6e 206c  ible effect on l
+00006510: 6172 6765 2064 6174 6120 286d 756c 7469  arge data (multi
+00006520: 2d4d 6942 2920 636f 6d70 7265 7373 696f  -MiB) compressio
+00006530: 6e2e 2049 6620 7761 6e74 2074 6f20 7573  n. If want to us
+00006540: 6520 6c61 7267 6520 6469 6374 696f 6e61  e large dictiona
+00006550: 7279 2063 6f6e 7465 6e74 2c20 7365 6520  ry content, see 
+00006560: 7072 6566 6978 283a 7079 3a61 7474 723a  prefix(:py:attr:
+00006570: 605a 7374 6444 6963 742e 6173 5f70 7265  `ZstdDict.as_pre
+00006580: 6669 7860 292e 0a20 2020 2020 2020 2023  fix`)..        #
+00006590: 2e20 5468 6572 6520 6973 2061 2070 6f73  . There is a pos
+000065a0: 7369 6269 6c69 7479 2074 6861 7420 7468  sibility that th
+000065b0: 6520 6469 6374 696f 6e61 7279 2063 6f6e  e dictionary con
+000065c0: 7465 6e74 2063 6f75 6c64 2062 6520 6d61  tent could be ma
+000065d0: 6c69 6369 6f75 736c 7920 7461 6d70 6572  liciously tamper
+000065e0: 6564 2062 7920 6120 7468 6972 6420 7061  ed by a third pa
+000065f0: 7274 792e 0a0a 2020 2020 2a2a 4164 7661  rty...    **Adva
+00006600: 6e63 6564 2064 6963 7469 6f6e 6172 7920  nced dictionary 
+00006610: 7472 6169 6e69 6e67 2a2a 0a0a 2020 2020  training**..    
+00006620: 5079 7a73 7464 206d 6f64 756c 6520 6f6e  Pyzstd module on
+00006630: 6c79 2075 7365 7320 7a73 7464 206c 6962  ly uses zstd lib
+00006640: 7261 7279 2773 2073 7461 626c 6520 4150  rary's stable AP
+00006650: 492e 2054 6865 2073 7461 626c 6520 4150  I. The stable AP
+00006660: 4920 6f6e 6c79 2065 7870 6f73 6573 2074  I only exposes t
+00006670: 776f 2064 6963 7469 6f6e 6172 7920 7472  wo dictionary tr
+00006680: 6169 6e69 6e67 2066 756e 6374 696f 6e73  aining functions
+00006690: 2074 6861 7420 636f 7272 6573 706f 6e64   that correspond
+000066a0: 696e 6720 746f 203a 7079 3a66 756e 633a  ing to :py:func:
+000066b0: 6074 7261 696e 5f64 6963 7460 2061 6e64  `train_dict` and
+000066c0: 203a 7079 3a66 756e 633a 6066 696e 616c   :py:func:`final
+000066d0: 697a 655f 6469 6374 602e 0a0a 2020 2020  ize_dict`...    
+000066e0: 4966 2077 616e 7420 746f 2061 646a 7573  If want to adjus
+000066f0: 7420 6164 7661 6e63 6564 2074 7261 696e  t advanced train
+00006700: 696e 6720 7061 7261 6d65 7465 7273 2c20  ing parameters, 
+00006710: 796f 7520 6d61 7920 7573 6520 7a73 7464  you may use zstd
+00006720: 2773 2043 4c49 2070 726f 6772 616d 2028  's CLI program (
+00006730: 6e6f 7420 7079 7a73 7464 206d 6f64 756c  not pyzstd modul
+00006740: 6527 7320 434c 4929 2c20 6974 2068 6173  e's CLI), it has
+00006750: 2065 6e74 7269 6573 2074 6f20 7a73 7464   entries to zstd
+00006760: 206c 6962 7261 7279 2773 2065 7870 6572   library's exper
+00006770: 696d 656e 7461 6c20 4150 492e 0a0a 2e2e  imental API.....
+00006780: 2070 793a 636c 6173 733a 3a20 5a73 7464   py:class:: Zstd
+00006790: 4469 6374 0a0a 2020 2020 5265 7072 6573  Dict..    Repres
+000067a0: 656e 7473 2061 207a 7374 6420 6469 6374  ents a zstd dict
+000067b0: 696f 6e61 7279 2c20 6361 6e20 6265 2075  ionary, can be u
+000067c0: 7365 6420 666f 7220 636f 6d70 7265 7373  sed for compress
+000067d0: 696f 6e2f 6465 636f 6d70 7265 7373 696f  ion/decompressio
+000067e0: 6e2e 0a0a 2020 2020 4974 2773 2074 6872  n...    It's thr
+000067f0: 6561 642d 7361 6665 2c20 616e 6420 6361  ead-safe, and ca
+00006800: 6e20 6265 2073 6861 7265 6420 6279 206d  n be shared by m
+00006810: 756c 7469 706c 6520 3a70 793a 636c 6173  ultiple :py:clas
+00006820: 733a 605a 7374 6443 6f6d 7072 6573 736f  s:`ZstdCompresso
+00006830: 7260 202f 203a 7079 3a63 6c61 7373 3a60  r` / :py:class:`
+00006840: 5a73 7464 4465 636f 6d70 7265 7373 6f72  ZstdDecompressor
+00006850: 6020 6f62 6a65 6374 732e 0a0a 2020 2020  ` objects...    
+00006860: 2e2e 2073 6f75 7263 6563 6f64 653a 3a20  .. sourcecode:: 
+00006870: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+00006880: 2320 6c6f 6164 2061 207a 7374 6420 6469  # load a zstd di
+00006890: 6374 696f 6e61 7279 2066 726f 6d20 6669  ctionary from fi
+000068a0: 6c65 0a20 2020 2020 2020 2077 6974 6820  le.        with 
+000068b0: 696f 2e6f 7065 6e28 6469 6374 5f70 6174  io.open(dict_pat
+000068c0: 682c 2027 7262 2729 2061 7320 663a 0a20  h, 'rb') as f:. 
+000068d0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+000068e0: 636f 6e74 656e 7420 3d20 662e 7265 6164  content = f.read
+000068f0: 2829 0a20 2020 2020 2020 207a 6420 3d20  ().        zd = 
+00006900: 5a73 7464 4469 6374 2866 696c 655f 636f  ZstdDict(file_co
+00006910: 6e74 656e 7429 0a0a 2020 2020 2020 2020  ntent)..        
+00006920: 2320 7573 6520 7468 6520 6469 6374 696f  # use the dictio
+00006930: 6e61 7279 2074 6f20 636f 6d70 7265 7373  nary to compress
+00006940: 2e0a 2020 2020 2020 2020 2320 6966 2075  ..        # if u
+00006950: 7365 2074 6865 2073 616d 6520 6469 6374  se the same dict
+00006960: 696f 6e61 7279 2066 6f72 2063 6f6d 7072  ionary for compr
+00006970: 6573 7369 6f6e 2072 6570 6561 7465 646c  ession repeatedl
+00006980: 792c 2072 6575 7369 6e67 0a20 2020 2020  y, reusing.     
+00006990: 2020 2023 2061 2063 6f6d 7072 6573 736f     # a compresso
+000069a0: 7220 6f62 6a65 6374 2069 7320 6661 7374  r object is fast
+000069b0: 6572 2c20 7365 6520 2e61 735f 756e 6469  er, see .as_undi
+000069c0: 6765 7374 6564 5f64 6963 7420 646f 632e  gested_dict doc.
+000069d0: 0a20 2020 2020 2020 2063 6f6d 7072 6573  .        compres
+000069e0: 7365 645f 6461 7420 3d20 636f 6d70 7265  sed_dat = compre
+000069f0: 7373 2872 6177 5f64 6174 2c20 7a73 7464  ss(raw_dat, zstd
+00006a00: 5f64 6963 743d 7a64 290a 0a20 2020 2020  _dict=zd)..     
+00006a10: 2020 2023 2075 7365 2074 6865 2064 6963     # use the dic
+00006a20: 7469 6f6e 6172 7920 746f 2064 6563 6f6d  tionary to decom
+00006a30: 7072 6573 730a 2020 2020 2020 2020 6465  press.        de
+00006a40: 636f 6d70 7265 7373 6564 5f64 6174 203d  compressed_dat =
+00006a50: 2064 6563 6f6d 7072 6573 7328 636f 6d70   decompress(comp
+00006a60: 7265 7373 6564 5f64 6174 2c20 7a73 7464  ressed_dat, zstd
+00006a70: 5f64 6963 743d 7a64 290a 0a20 2020 202e  _dict=zd)..    .
+00006a80: 2e20 7665 7273 696f 6e63 6861 6e67 6564  . versionchanged
+00006a90: 3a3a 2030 2e31 352e 370a 2020 2020 2020  :: 0.15.7.      
+00006aa0: 2020 5768 656e 2063 6f6d 7072 6573 7369    When compressi
+00006ab0: 6e67 2c20 6c6f 6164 2075 6e64 6967 6573  ng, load undiges
+00006ac0: 7465 6420 6469 6374 696f 6e61 7279 2069  ted dictionary i
+00006ad0: 6e73 7465 6164 206f 6620 6469 6765 7374  nstead of digest
+00006ae0: 6564 2064 6963 7469 6f6e 6172 7920 6279  ed dictionary by
+00006af0: 2064 6566 6175 6c74 2c20 7365 6520 3a70   default, see :p
+00006b00: 793a 6174 7472 3a60 7e5a 7374 6444 6963  y:attr:`~ZstdDic
+00006b10: 742e 6173 5f64 6967 6573 7465 645f 6469  t.as_digested_di
+00006b20: 6374 602e 2041 6c73 6f20 6164 6420 6060  ct`. Also add ``
+00006b30: 2e5f 5f6c 656e 5f5f 2829 6060 206d 6574  .__len__()`` met
+00006b40: 686f 6420 7468 6174 2072 6574 7572 6e69  hod that returni
+00006b50: 6e67 2063 6f6e 7465 6e74 2073 697a 652e  ng content size.
+00006b60: 0a0a 2020 2020 2e2e 2070 793a 6d65 7468  ..    .. py:meth
+00006b70: 6f64 3a3a 205f 5f69 6e69 745f 5f28 7365  od:: __init__(se
+00006b80: 6c66 2c20 6469 6374 5f63 6f6e 7465 6e74  lf, dict_content
+00006b90: 2c20 6973 5f72 6177 3d46 616c 7365 290a  , is_raw=False).
+00006ba0: 0a20 2020 2020 2020 2049 6e69 7469 616c  .        Initial
+00006bb0: 697a 6520 6120 5a73 7464 4469 6374 206f  ize a ZstdDict o
+00006bc0: 626a 6563 742e 0a0a 2020 2020 2020 2020  bject...        
+00006bd0: 3a70 6172 616d 2064 6963 745f 636f 6e74  :param dict_cont
+00006be0: 656e 743a 2044 6963 7469 6f6e 6172 7927  ent: Dictionary'
+00006bf0: 7320 636f 6e74 656e 742e 0a20 2020 2020  s content..     
+00006c00: 2020 203a 7479 7065 2064 6963 745f 636f     :type dict_co
+00006c10: 6e74 656e 743a 2062 7974 6573 2d6c 696b  ntent: bytes-lik
+00006c20: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00006c30: 203a 7061 7261 6d20 6973 5f72 6177 3a20   :param is_raw: 
+00006c40: 5468 6973 2070 6172 616d 6574 6572 2069  This parameter i
+00006c50: 7320 666f 7220 6164 7661 6e63 6564 2075  s for advanced u
+00006c60: 7365 722e 2060 6054 7275 6560 6020 6d65  ser. ``True`` me
+00006c70: 616e 7320 2a64 6963 745f 636f 6e74 656e  ans *dict_conten
+00006c80: 742a 2061 7267 756d 656e 7420 6973 2061  t* argument is a
+00006c90: 2022 7261 7720 636f 6e74 656e 7422 2064   "raw content" d
+00006ca0: 6963 7469 6f6e 6172 792c 2066 7265 6520  ictionary, free 
+00006cb0: 6f66 2061 6e79 2066 6f72 6d61 7420 7265  of any format re
+00006cc0: 7374 7269 6374 696f 6e2e 2060 6046 616c  striction. ``Fal
+00006cd0: 7365 6060 206d 6561 6e73 202a 6469 6374  se`` means *dict
+00006ce0: 5f63 6f6e 7465 6e74 2a20 6172 6775 6d65  _content* argume
+00006cf0: 6e74 2069 7320 616e 206f 7264 696e 6172  nt is an ordinar
+00006d00: 7920 7a73 7464 2064 6963 7469 6f6e 6172  y zstd dictionar
+00006d10: 792c 2077 6173 2063 7265 6174 6564 2062  y, was created b
+00006d20: 7920 7a73 7464 2066 756e 6374 696f 6e73  y zstd functions
+00006d30: 2c20 666f 6c6c 6f77 2061 2073 7065 6369  , follow a speci
+00006d40: 6669 6564 2066 6f72 6d61 742e 0a20 2020  fied format..   
+00006d50: 2020 2020 203a 7479 7065 2069 735f 7261       :type is_ra
+00006d60: 773a 2062 6f6f 6c0a 0a20 2020 202e 2e20  w: bool..    .. 
+00006d70: 7079 3a61 7474 7269 6275 7465 3a3a 2064  py:attribute:: d
+00006d80: 6963 745f 636f 6e74 656e 740a 0a20 2020  ict_content..   
+00006d90: 2020 2020 2054 6865 2063 6f6e 7465 6e74       The content
+00006da0: 206f 6620 7a73 7464 2064 6963 7469 6f6e   of zstd diction
+00006db0: 6172 792c 2061 2060 6062 7974 6573 6060  ary, a ``bytes``
+00006dc0: 206f 626a 6563 742e 2049 7427 7320 7468   object. It's th
+00006dd0: 6520 7361 6d65 2061 7320 2a64 6963 745f  e same as *dict_
+00006de0: 636f 6e74 656e 742a 2061 7267 756d 656e  content* argumen
+00006df0: 7420 696e 203a 7079 3a6d 6574 683a 607e  t in :py:meth:`~
+00006e00: 5a73 7464 4469 6374 2e5f 5f69 6e69 745f  ZstdDict.__init_
+00006e10: 5f60 206d 6574 686f 642e 2049 7420 6361  _` method. It ca
+00006e20: 6e20 6265 2075 7365 6420 7769 7468 206f  n be used with o
+00006e30: 7468 6572 2070 726f 6772 616d 732e 0a0a  ther programs...
+00006e40: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
+00006e50: 7574 653a 3a20 6469 6374 5f69 640a 0a20  ute:: dict_id.. 
+00006e60: 2020 2020 2020 2049 4420 6f66 207a 7374         ID of zst
+00006e70: 6420 6469 6374 696f 6e61 7279 2c20 6120  d dictionary, a 
+00006e80: 3332 2d62 6974 2075 6e73 6967 6e65 6420  32-bit unsigned 
+00006e90: 696e 7465 6765 7220 7661 6c75 652e 2053  integer value. S
+00006ea0: 6565 203a 7265 663a 6074 6869 7320 6e6f  ee :ref:`this no
+00006eb0: 7465 3c64 6963 745f 6964 3e60 2066 6f72  te<dict_id>` for
+00006ec0: 2064 6574 6169 6c73 2e0a 0a20 2020 2020   details...     
+00006ed0: 2020 204e 6f6e 2d7a 6572 6f20 6d65 616e     Non-zero mean
+00006ee0: 7320 6f72 6469 6e61 7279 2064 6963 7469  s ordinary dicti
+00006ef0: 6f6e 6172 792c 2077 6173 2063 7265 6174  onary, was creat
+00006f00: 6564 2062 7920 7a73 7464 2066 756e 6374  ed by zstd funct
+00006f10: 696f 6e73 2c20 666f 6c6c 6f77 2061 2073  ions, follow a s
+00006f20: 7065 6369 6669 6564 2066 6f72 6d61 742e  pecified format.
+00006f30: 0a0a 2020 2020 2020 2020 6060 3060 6020  ..        ``0`` 
+00006f40: 6d65 616e 7320 6120 2272 6177 2063 6f6e  means a "raw con
+00006f50: 7465 6e74 2220 6469 6374 696f 6e61 7279  tent" dictionary
+00006f60: 2c20 6672 6565 206f 6620 616e 7920 666f  , free of any fo
+00006f70: 726d 6174 2072 6573 7472 6963 7469 6f6e  rmat restriction
+00006f80: 2c20 7573 6564 2066 6f72 2061 6476 616e  , used for advan
+00006f90: 6365 6420 7573 6572 2e20 284e 6f74 6520  ced user. (Note 
+00006fa0: 7468 6174 2074 6865 206d 6561 6e69 6e67  that the meaning
+00006fb0: 206f 6620 6060 3060 6020 6973 2064 6966   of ``0`` is dif
+00006fc0: 6665 7265 6e74 2066 726f 6d20 6060 6469  ferent from ``di
+00006fd0: 6374 696f 6e61 7279 5f69 6460 6020 696e  ctionary_id`` in
+00006fe0: 203a 7079 3a66 756e 633a 6067 6574 5f66   :py:func:`get_f
+00006ff0: 7261 6d65 5f69 6e66 6f60 2066 756e 6374  rame_info` funct
+00007000: 696f 6e2e 290a 0a20 2020 202e 2e20 7079  ion.)..    .. py
+00007010: 3a61 7474 7269 6275 7465 3a3a 2061 735f  :attribute:: as_
+00007020: 6469 6765 7374 6564 5f64 6963 740a 0a20  digested_dict.. 
+00007030: 2020 2020 2020 204c 6f61 6420 6173 2061         Load as a
+00007040: 2064 6967 6573 7465 6420 6469 6374 696f   digested dictio
+00007050: 6e61 7279 2c20 7365 6520 6265 6c6f 772e  nary, see below.
+00007060: 0a0a 2020 2020 2020 2020 2e2e 2076 6572  ..        .. ver
+00007070: 7369 6f6e 6164 6465 643a 3a20 302e 3135  sionadded:: 0.15
+00007080: 2e37 0a0a 2020 2020 2e2e 2070 793a 6174  .7..    .. py:at
+00007090: 7472 6962 7574 653a 3a20 6173 5f75 6e64  tribute:: as_und
+000070a0: 6967 6573 7465 645f 6469 6374 0a0a 2020  igested_dict..  
+000070b0: 2020 2020 2020 4c6f 6164 2061 7320 616e        Load as an
+000070c0: 2075 6e64 6967 6573 7465 6420 6469 6374   undigested dict
+000070d0: 696f 6e61 7279 2e0a 0a20 2020 2020 2020  ionary...       
+000070e0: 2044 6967 6573 7469 6e67 2064 6963 7469   Digesting dicti
+000070f0: 6f6e 6172 7920 6973 2061 2063 6f73 746c  onary is a costl
+00007100: 7920 6f70 6572 6174 696f 6e2e 2054 6865  y operation. The
+00007110: 7365 2074 776f 2061 7474 7269 6275 7465  se two attribute
+00007120: 7320 6361 6e20 636f 6e74 726f 6c20 686f  s can control ho
+00007130: 7720 7468 6520 6469 6374 696f 6e61 7279  w the dictionary
+00007140: 2069 7320 6c6f 6164 6564 2074 6f20 636f   is loaded to co
+00007150: 6d70 7265 7373 6f72 2c20 6279 2070 6173  mpressor, by pas
+00007160: 7369 6e67 2074 6865 6d20 6173 2060 7a73  sing them as `zs
+00007170: 7464 5f64 6963 7460 2061 7267 756d 656e  td_dict` argumen
+00007180: 743a 2060 6063 6f6d 7072 6573 7328 6461  t: ``compress(da
+00007190: 742c 207a 7374 645f 6469 6374 3d7a 642e  t, zstd_dict=zd.
+000071a0: 6173 5f64 6967 6573 7465 645f 6469 6374  as_digested_dict
+000071b0: 2960 600a 0a20 2020 2020 2020 2049 6620  )``..        If 
+000071c0: 646f 6e27 7420 7370 6563 6966 7920 7468  don't specify th
+000071d0: 6573 6520 7477 6f20 6174 7472 6962 7574  ese two attribut
+000071e0: 6573 2c20 7573 6520 2a2a 756e 6469 6765  es, use **undige
+000071f0: 7374 6564 2a2a 2064 6963 7469 6f6e 6172  sted** dictionar
+00007200: 7920 666f 7220 636f 6d70 7265 7373 696f  y for compressio
+00007210: 6e20 6279 2064 6566 6175 6c74 3a20 6060  n by default: ``
+00007220: 636f 6d70 7265 7373 2864 6174 2c20 7a73  compress(dat, zs
+00007230: 7464 5f64 6963 743d 7a64 2960 600a 0a20  td_dict=zd)``.. 
+00007240: 2020 2020 2020 202e 2e20 6c69 7374 2d74         .. list-t
+00007250: 6162 6c65 3a3a 2044 6966 6665 7265 6e63  able:: Differenc
+00007260: 6520 666f 7220 636f 6d70 7265 7373 696f  e for compressio
+00007270: 6e0a 2020 2020 2020 2020 2020 2020 3a77  n.            :w
+00007280: 6964 7468 733a 2031 3220 3132 2031 320a  idths: 12 12 12.
+00007290: 2020 2020 2020 2020 2020 2020 3a68 6561              :hea
+000072a0: 6465 722d 726f 7773 3a20 310a 0a20 2020  der-rows: 1..   
+000072b0: 2020 2020 2020 2020 202a 202d 0a20 2020           * -.   
+000072c0: 2020 2020 2020 2020 2020 202d 207c 2044             - | D
+000072d0: 6967 6573 7465 640a 2020 2020 2020 2020  igested.        
+000072e0: 2020 2020 2020 2020 7c20 6469 6374 696f          | dictio
+000072f0: 6e61 7279 0a20 2020 2020 2020 2020 2020  nary.           
+00007300: 2020 202d 207c 2055 6e64 6967 6573 7465     - | Undigeste
+00007310: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00007320: 2020 7c20 6469 6374 696f 6e61 7279 0a20    | dictionary. 
+00007330: 2020 2020 2020 2020 2020 202a 202d 207c             * - |
+00007340: 2053 6f6d 6520 6164 7661 6e63 6564 0a20   Some advanced. 
+00007350: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007360: 2070 6172 616d 6574 6572 7320 6f66 0a20   parameters of. 
+00007370: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007380: 2063 6f6d 7072 6573 736f 7220 6d61 790a   compressor may.
+00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073a0: 7c20 6265 206f 7665 7272 6964 6465 6e0a  | be overridden.
+000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073c0: 7c20 6279 2064 6963 7469 6f6e 6172 7927  | by dictionary'
+000073d0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000073e0: 2020 7c20 7061 7261 6d65 7465 7273 0a20    | parameters. 
+000073f0: 2020 2020 2020 2020 2020 2020 202d 207c               - |
+00007400: 2060 6077 696e 646f 774c 6f67 6060 2c20   ``windowLog``, 
+00007410: 6060 6861 7368 4c6f 6760 602c 0a20 2020  ``hashLog``,.   
+00007420: 2020 2020 2020 2020 2020 2020 207c 2060               | `
+00007430: 6063 6861 696e 4c6f 6760 602c 2060 6073  `chainLog``, ``s
+00007440: 6561 7263 684c 6f67 6060 2c0a 2020 2020  earchLog``,.    
+00007450: 2020 2020 2020 2020 2020 2020 7c20 6060              | ``
+00007460: 6d69 6e4d 6174 6368 6060 2c20 6060 7461  minMatch``, ``ta
+00007470: 7267 6574 4c65 6e67 7468 6060 2c0a 2020  rgetLength``,.  
+00007480: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00007490: 6060 7374 7261 7465 6779 6060 2c0a 2020  ``strategy``,.  
+000074a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000074b0: 6060 656e 6162 6c65 4c6f 6e67 4469 7374  ``enableLongDist
+000074c0: 616e 6365 4d61 7463 6869 6e67 6060 2c0a  anceMatching``,.
+000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074e0: 7c20 6060 6c64 6d48 6173 684c 6f67 6060  | ``ldmHashLog``
+000074f0: 2c20 6060 6c64 6d4d 696e 4d61 7463 6860  , ``ldmMinMatch`
+00007500: 602c 0a20 2020 2020 2020 2020 2020 2020  `,.             
+00007510: 2020 207c 2060 606c 646d 4275 636b 6574     | ``ldmBucket
+00007520: 5369 7a65 4c6f 6760 602c 0a20 2020 2020  SizeLog``,.     
+00007530: 2020 2020 2020 2020 2020 207c 2060 606c             | ``l
+00007540: 646d 4861 7368 5261 7465 4c6f 6760 602c  dmHashRateLog``,
+00007550: 2061 6e64 2073 6f6d 650a 2020 2020 2020   and some.      
+00007560: 2020 2020 2020 2020 2020 7c20 6e6f 6e2d            | non-
+00007570: 7075 626c 6963 2070 6172 616d 6574 6572  public parameter
+00007580: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+00007590: 202d 204e 6f0a 2020 2020 2020 2020 2020   - No.          
+000075a0: 2020 2a20 2d20 7c20 5a73 7464 4469 6374    * - | ZstdDict
+000075b0: 2068 6173 0a20 2020 2020 2020 2020 2020   has.           
+000075c0: 2020 2020 207c 2069 6e74 6572 6e61 6c20       | internal 
+000075d0: 6361 6368 650a 2020 2020 2020 2020 2020  cache.          
+000075e0: 2020 2020 2020 7c20 666f 7220 7468 6973        | for this
+000075f0: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
+00007600: 207c 2059 6573 2e20 4974 2773 2066 6173   | Yes. It's fas
+00007610: 7465 7220 7768 656e 0a20 2020 2020 2020  ter when.       
+00007620: 2020 2020 2020 2020 207c 206c 6f61 6469           | loadi
+00007630: 6e67 2061 6761 696e 2061 2064 6967 6573  ng again a diges
+00007640: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+00007650: 2020 2020 7c20 6469 6374 696f 6e61 7279      | dictionary
+00007660: 2077 6974 6820 7468 6520 7361 6d65 0a20   with the same. 
+00007670: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007680: 2063 6f6d 7072 6573 7369 6f6e 206c 6576   compression lev
+00007690: 656c 2e0a 2020 2020 2020 2020 2020 2020  el..            
+000076a0: 2020 2d20 7c20 4e6f 2e20 4966 206c 6f61    - | No. If loa
+000076b0: 6420 616e 2075 6e64 6967 6573 7465 640a  d an undigested.
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 7c20 6469 6374 696f 6e61 7279 206d 756c  | dictionary mul
+000076e0: 7469 706c 6520 7469 6d65 732c 0a20 2020  tiple times,.   
+000076f0: 2020 2020 2020 2020 2020 2020 207c 2063               | c
+00007700: 6f6e 7369 6465 7220 7265 7573 696e 6720  onsider reusing 
+00007710: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00007720: 2020 7c20 636f 6d70 7265 7373 6f72 206f    | compressor o
+00007730: 626a 6563 742e 0a0a 2020 2020 2020 2020  bject...        
+00007740: 466f 7220 6465 636f 6d70 7265 7373 696f  For decompressio
+00007750: 6e2c 2074 6865 7920 6861 7665 2074 6865  n, they have the
+00007760: 2073 616d 6520 6566 6665 6374 2e20 5079   same effect. Py
+00007770: 7a73 7464 2075 7365 7320 2a2a 6469 6765  zstd uses **dige
+00007780: 7374 6564 2a2a 2064 6963 7469 6f6e 6172  sted** dictionar
+00007790: 7920 666f 7220 6465 636f 6d70 7265 7373  y for decompress
+000077a0: 696f 6e20 6279 2064 6566 6175 6c74 2c20  ion by default, 
+000077b0: 7768 6963 6820 6973 2066 6173 7465 7220  which is faster 
+000077c0: 7768 656e 206c 6f61 6469 6e67 2061 6761  when loading aga
+000077d0: 696e 3a20 6060 6465 636f 6d70 7265 7373  in: ``decompress
+000077e0: 2864 6174 2c20 7a73 7464 5f64 6963 743d  (dat, zstd_dict=
+000077f0: 7a64 2960 600a 0a20 2020 2020 2020 202e  zd)``..        .
+00007800: 2e20 7665 7273 696f 6e61 6464 6564 3a3a  . versionadded::
+00007810: 2030 2e31 352e 370a 0a20 2020 202e 2e20   0.15.7..    .. 
+00007820: 7079 3a61 7474 7269 6275 7465 3a3a 2061  py:attribute:: a
+00007830: 735f 7072 6566 6978 0a0a 2020 2020 2020  s_prefix..      
+00007840: 2020 4c6f 6164 2074 6865 2064 6963 7469    Load the dicti
+00007850: 6f6e 6172 7920 636f 6e74 656e 7420 746f  onary content to
+00007860: 2063 6f6d 7072 6573 736f 722f 6465 636f   compressor/deco
+00007870: 6d70 7265 7373 6f72 2061 7320 6120 2270  mpressor as a "p
+00007880: 7265 6669 7822 2c20 6279 2070 6173 7369  refix", by passi
+00007890: 6e67 2074 6869 7320 6174 7472 6962 7574  ng this attribut
+000078a0: 6520 6173 2060 7a73 7464 5f64 6963 7460  e as `zstd_dict`
+000078b0: 2061 7267 756d 656e 743a 2060 6063 6f6d   argument: ``com
+000078c0: 7072 6573 7328 6461 742c 207a 7374 645f  press(dat, zstd_
+000078d0: 6469 6374 3d7a 642e 6173 5f70 7265 6669  dict=zd.as_prefi
+000078e0: 7829 6060 0a0a 2020 2020 2020 2020 5072  x)``..        Pr
+000078f0: 6566 6978 2063 616e 2062 6520 7573 6564  efix can be used
+00007900: 2066 6f72 203a 7265 663a 6070 6174 6368   for :ref:`patch
+00007910: 696e 6720 656e 6769 6e65 3c70 6174 6368  ing engine<patch
+00007920: 696e 675f 656e 6769 6e65 3e60 2073 6365  ing_engine>` sce
+00007930: 6e61 7269 6f2e 0a0a 2020 2020 2020 2020  nario...        
+00007940: 232e 2050 7265 6669 7820 6973 2063 6f6d  #. Prefix is com
+00007950: 7061 7469 626c 6520 7769 7468 2022 6c6f  patible with "lo
+00007960: 6e67 2064 6973 7461 6e63 6520 6d61 7463  ng distance matc
+00007970: 6869 6e67 222c 2077 6869 6c65 2064 6963  hing", while dic
+00007980: 7469 6f6e 6172 7920 6973 206e 6f74 2e0a  tionary is not..
+00007990: 2020 2020 2020 2020 232e 2050 7265 6669          #. Prefi
+000079a0: 7820 6f6e 6c79 2077 6f72 6b20 666f 7220  x only work for 
+000079b0: 7468 6520 6669 7273 7420 6672 616d 652c  the first frame,
+000079c0: 2074 6865 6e20 7468 6520 636f 6d70 7265   then the compre
+000079d0: 7373 6f72 2f64 6563 6f6d 7072 6573 736f  ssor/decompresso
+000079e0: 7220 7769 6c6c 2072 6574 7572 6e20 746f  r will return to
+000079f0: 206e 6f20 7072 6566 6978 2073 7461 7465   no prefix state
+00007a00: 2e20 5468 6973 2069 7320 6469 6666 6572  . This is differ
+00007a10: 656e 7420 6672 6f6d 2064 6963 7469 6f6e  ent from diction
+00007a20: 6172 7920 7468 6174 2063 616e 2062 6520  ary that can be 
+00007a30: 7573 6564 2066 6f72 2061 6c6c 2073 7562  used for all sub
+00007a40: 7365 7175 656e 7420 6672 616d 6573 2e0a  sequent frames..
+00007a50: 2020 2020 2020 2020 232e 2057 6865 6e20          #. When 
+00007a60: 6465 636f 6d70 7265 7373 696e 672c 206d  decompressing, m
+00007a70: 7573 7420 7573 6520 7468 6520 7361 6d65  ust use the same
+00007a80: 2070 7265 6669 7820 6173 2077 6865 6e20   prefix as when 
+00007a90: 636f 6d70 7265 7373 696e 672e 0a20 2020  compressing..   
+00007aa0: 2020 2020 2023 2e20 4c6f 6164 696e 6720       #. Loading 
+00007ab0: 7072 6566 6978 2074 6f20 636f 6d70 7265  prefix to compre
+00007ac0: 7373 6f72 2069 7320 636f 7374 6c79 2e0a  ssor is costly..
+00007ad0: 2020 2020 2020 2020 232e 204c 6f61 6469          #. Loadi
+00007ae0: 6e67 2070 7265 6669 7820 746f 2064 6563  ng prefix to dec
+00007af0: 6f6d 7072 6573 736f 7220 6973 206e 6f74  ompressor is not
+00007b00: 2063 6f73 746c 792e 0a0a 2020 2020 2020   costly...      
+00007b10: 2020 2e2e 2076 6572 7369 6f6e 6164 6465    .. versionadde
+00007b20: 643a 3a20 302e 3135 2e37 0a0a 0a2e 2e20  d:: 0.15.7..... 
+00007b30: 7079 3a66 756e 6374 696f 6e3a 3a20 7472  py:function:: tr
+00007b40: 6169 6e5f 6469 6374 2873 616d 706c 6573  ain_dict(samples
+00007b50: 2c20 6469 6374 5f73 697a 6529 0a0a 2020  , dict_size)..  
+00007b60: 2020 5472 6169 6e20 6120 7a73 7464 2064    Train a zstd d
+00007b70: 6963 7469 6f6e 6172 792e 0a0a 2020 2020  ictionary...    
+00007b80: 5365 6520 7468 6520 4641 5120 696e 2060  See the FAQ in `
+00007b90: 7468 6973 2066 696c 6520 3c68 7474 7073  this file <https
+00007ba0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
+00007bb0: 6365 626f 6f6b 2f7a 7374 642f 626c 6f62  cebook/zstd/blob
+00007bc0: 2f72 656c 6561 7365 2f6c 6962 2f7a 6469  /release/lib/zdi
+00007bd0: 6374 2e68 3e60 5f20 666f 7220 6465 7461  ct.h>`_ for deta
+00007be0: 696c 732e 0a0a 2020 2020 3a70 6172 616d  ils...    :param
+00007bf0: 2073 616d 706c 6573 3a20 416e 2069 7465   samples: An ite
+00007c00: 7261 626c 6520 6f66 2073 616d 706c 6573  rable of samples
+00007c10: 2c20 6120 7361 6d70 6c65 2069 7320 6120  , a sample is a 
+00007c20: 6279 7465 732d 6c69 6b65 206f 626a 6563  bytes-like objec
+00007c30: 7420 7265 7072 6573 656e 7473 2061 2066  t represents a f
+00007c40: 696c 652e 0a20 2020 203a 7479 7065 2073  ile..    :type s
+00007c50: 616d 706c 6573 3a20 6974 6572 6162 6c65  amples: iterable
+00007c60: 0a20 2020 203a 7061 7261 6d20 696e 7420  .    :param int 
+00007c70: 6469 6374 5f73 697a 653a 2052 6574 7572  dict_size: Retur
+00007c80: 6e65 6420 7a73 7464 2064 6963 7469 6f6e  ned zstd diction
+00007c90: 6172 7927 7320 2a2a 6d61 7869 6d75 6d2a  ary's **maximum*
+00007ca0: 2a20 7369 7a65 2c20 696e 2062 7974 6573  * size, in bytes
+00007cb0: 2e0a 2020 2020 3a72 6574 7572 6e3a 2054  ..    :return: T
+00007cc0: 7261 696e 6564 207a 7374 6420 6469 6374  rained zstd dict
+00007cd0: 696f 6e61 7279 2e20 4966 2077 616e 7420  ionary. If want 
+00007ce0: 746f 2073 6176 6520 7468 6520 6469 6374  to save the dict
+00007cf0: 696f 6e61 7279 2074 6f20 6120 6669 6c65  ionary to a file
+00007d00: 2c20 7361 7665 2074 6865 203a 7079 3a61  , save the :py:a
+00007d10: 7474 723a 605a 7374 6444 6963 742e 6469  ttr:`ZstdDict.di
+00007d20: 6374 5f63 6f6e 7465 6e74 6020 6174 7472  ct_content` attr
+00007d30: 6962 7574 652e 0a20 2020 203a 7274 7970  ibute..    :rtyp
+00007d40: 653a 205a 7374 6444 6963 740a 0a20 2020  e: ZstdDict..   
+00007d50: 202e 2e20 736f 7572 6365 636f 6465 3a3a   .. sourcecode::
+00007d60: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+00007d70: 2064 6566 2073 616d 706c 6573 2829 3a0a   def samples():.
+00007d80: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+00007d90: 6469 7220 3d20 7222 453a 5c64 6174 6122  dir = r"E:\data"
+00007da0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00007db0: 4e6f 7465 2074 6861 7420 7468 6520 6f72  Note that the or
+00007dc0: 6465 7220 6f66 2074 6865 2066 696c 6573  der of the files
+00007dd0: 206d 6179 2062 6520 6469 6666 6572 656e   may be differen
+00007de0: 742c 0a20 2020 2020 2020 2020 2020 2023  t,.            #
+00007df0: 2074 6865 7265 666f 7265 2074 6865 2067   therefore the g
+00007e00: 656e 6572 6174 6564 2064 6963 7469 6f6e  enerated diction
+00007e10: 6172 7920 6d61 7920 6265 2064 6966 6665  ary may be diffe
+00007e20: 7265 6e74 2e0a 2020 2020 2020 2020 2020  rent..          
+00007e30: 2020 666f 7220 7061 7265 6e74 2c20 6469    for parent, di
+00007e40: 726e 616d 6573 2c20 6669 6c65 6e61 6d65  rnames, filename
+00007e50: 7320 696e 206f 732e 7761 6c6b 2872 6f6f  s in os.walk(roo
+00007e60: 7464 6972 293a 0a20 2020 2020 2020 2020  tdir):.         
+00007e70: 2020 2020 2020 2066 6f72 2066 696c 656e         for filen
+00007e80: 616d 6520 696e 2066 696c 656e 616d 6573  ame in filenames
+00007e90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007ea0: 2020 2020 2020 7061 7468 203d 206f 732e        path = os.
+00007eb0: 7061 7468 2e6a 6f69 6e28 7061 7265 6e74  path.join(parent
+00007ec0: 2c20 6669 6c65 6e61 6d65 290a 2020 2020  , filename).    
+00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ee0: 7769 7468 2069 6f2e 6f70 656e 2870 6174  with io.open(pat
+00007ef0: 682c 2027 7262 2729 2061 7320 663a 0a20  h, 'rb') as f:. 
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 2020 2020 2020 2064 6174 203d 2066 2e72         dat = f.r
+00007f20: 6561 6428 290a 2020 2020 2020 2020 2020  ead().          
+00007f30: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
+00007f40: 6461 740a 0a20 2020 2020 2020 2064 6963  dat..        dic
+00007f50: 203d 2070 797a 7374 642e 7472 6169 6e5f   = pyzstd.train_
+00007f60: 6469 6374 2873 616d 706c 6573 2829 2c20  dict(samples(), 
+00007f70: 3130 302a 3130 3234 290a 0a2e 2e20 7079  100*1024).... py
+00007f80: 3a66 756e 6374 696f 6e3a 3a20 6669 6e61  :function:: fina
+00007f90: 6c69 7a65 5f64 6963 7428 7a73 7464 5f64  lize_dict(zstd_d
+00007fa0: 6963 742c 2073 616d 706c 6573 2c20 6469  ict, samples, di
+00007fb0: 6374 5f73 697a 652c 206c 6576 656c 290a  ct_size, level).
+00007fc0: 0a20 2020 2047 6976 656e 2061 2063 7573  .    Given a cus
+00007fd0: 746f 6d20 636f 6e74 656e 7420 6173 2061  tom content as a
+00007fe0: 2062 6173 6973 2066 6f72 2064 6963 7469   basis for dicti
+00007ff0: 6f6e 6172 792c 2061 6e64 2061 2073 6574  onary, and a set
+00008000: 206f 6620 7361 6d70 6c65 732c 2066 696e   of samples, fin
+00008010: 616c 697a 6520 6469 6374 696f 6e61 7279  alize dictionary
+00008020: 2062 7920 6164 6469 6e67 2068 6561 6465   by adding heade
+00008030: 7273 2061 6e64 2073 7461 7469 7374 6963  rs and statistic
+00008040: 7320 6163 636f 7264 696e 6720 746f 2074  s according to t
+00008050: 6865 207a 7374 6420 6469 6374 696f 6e61  he zstd dictiona
+00008060: 7279 2066 6f72 6d61 742e 0a0a 2020 2020  ry format...    
+00008070: 5365 6520 7468 6520 4641 5120 696e 2060  See the FAQ in `
+00008080: 7468 6973 2066 696c 6520 3c68 7474 7073  this file <https
+00008090: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
+000080a0: 6365 626f 6f6b 2f7a 7374 642f 626c 6f62  cebook/zstd/blob
+000080b0: 2f72 656c 6561 7365 2f6c 6962 2f7a 6469  /release/lib/zdi
+000080c0: 6374 2e68 3e60 5f20 666f 7220 6465 7461  ct.h>`_ for deta
+000080d0: 696c 732e 0a0a 2020 2020 3a70 6172 616d  ils...    :param
+000080e0: 207a 7374 645f 6469 6374 3a20 4120 6261   zstd_dict: A ba
+000080f0: 7369 7320 6469 6374 696f 6e61 7279 2e0a  sis dictionary..
+00008100: 2020 2020 3a74 7970 6520 7a73 7464 5f64      :type zstd_d
+00008110: 6963 743a 205a 7374 6444 6963 740a 2020  ict: ZstdDict.  
+00008120: 2020 3a70 6172 616d 2073 616d 706c 6573    :param samples
+00008130: 3a20 416e 2069 7465 7261 626c 6520 6f66  : An iterable of
+00008140: 2073 616d 706c 6573 2c20 6120 7361 6d70   samples, a samp
+00008150: 6c65 2069 7320 6120 6279 7465 732d 6c69  le is a bytes-li
+00008160: 6b65 206f 626a 6563 7420 7265 7072 6573  ke object repres
+00008170: 656e 7473 2061 2066 696c 652e 0a20 2020  ents a file..   
+00008180: 203a 7479 7065 2073 616d 706c 6573 3a20   :type samples: 
+00008190: 6974 6572 6162 6c65 0a20 2020 203a 7061  iterable.    :pa
+000081a0: 7261 6d20 696e 7420 6469 6374 5f73 697a  ram int dict_siz
+000081b0: 653a 2052 6574 7572 6e65 6420 7a73 7464  e: Returned zstd
+000081c0: 2064 6963 7469 6f6e 6172 7927 7320 2a2a   dictionary's **
+000081d0: 6d61 7869 6d75 6d2a 2a20 7369 7a65 2c20  maximum** size, 
+000081e0: 696e 2062 7974 6573 2e0a 2020 2020 3a70  in bytes..    :p
+000081f0: 6172 616d 2069 6e74 206c 6576 656c 3a20  aram int level: 
+00008200: 5468 6520 636f 6d70 7265 7373 696f 6e20  The compression 
+00008210: 6c65 7665 6c20 6578 7065 6374 6564 2074  level expected t
+00008220: 6f20 7573 6520 696e 2070 726f 6475 6374  o use in product
+00008230: 696f 6e2e 2054 6865 2073 7461 7469 7374  ion. The statist
+00008240: 6963 7320 666f 7220 6561 6368 2063 6f6d  ics for each com
+00008250: 7072 6573 7369 6f6e 206c 6576 656c 2064  pression level d
+00008260: 6966 6665 722c 2073 6f20 7475 6e69 6e67  iffer, so tuning
+00008270: 2074 6865 2064 6963 7469 6f6e 6172 7920   the dictionary 
+00008280: 666f 7220 7468 6520 636f 6d70 7265 7373  for the compress
+00008290: 696f 6e20 6c65 7665 6c20 6361 6e20 6865  ion level can he
+000082a0: 6c70 2071 7569 7465 2061 2062 6974 2e0a  lp quite a bit..
+000082b0: 2020 2020 3a72 6574 7572 6e3a 2046 696e      :return: Fin
+000082c0: 616c 697a 6564 207a 7374 6420 6469 6374  alized zstd dict
+000082d0: 696f 6e61 7279 2e20 4966 2077 616e 7420  ionary. If want 
+000082e0: 746f 2073 6176 6520 7468 6520 6469 6374  to save the dict
+000082f0: 696f 6e61 7279 2074 6f20 6120 6669 6c65  ionary to a file
+00008300: 2c20 7361 7665 2074 6865 203a 7079 3a61  , save the :py:a
+00008310: 7474 723a 605a 7374 6444 6963 742e 6469  ttr:`ZstdDict.di
+00008320: 6374 5f63 6f6e 7465 6e74 6020 6174 7472  ct_content` attr
+00008330: 6962 7574 652e 0a20 2020 203a 7274 7970  ibute..    :rtyp
+00008340: 653a 205a 7374 6444 6963 740a 0a0a 4d6f  e: ZstdDict...Mo
+00008350: 6475 6c65 2d6c 6576 656c 2066 756e 6374  dule-level funct
+00008360: 696f 6e73 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ions.-----------
+00008370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020  -----------..   
+00008380: 2054 6869 7320 7365 6374 696f 6e20 636f   This section co
+00008390: 6e74 6169 6e73 3a0a 0a20 2020 2020 2020  ntains:..       
+000083a0: 202a 2066 756e 6374 696f 6e20 3a70 793a   * function :py:
+000083b0: 6675 6e63 3a60 6765 745f 6672 616d 655f  func:`get_frame_
+000083c0: 696e 666f 602c 2067 6574 2066 7261 6d65  info`, get frame
+000083d0: 2069 6e66 6f72 6d61 7469 6f6e 2066 726f   information fro
+000083e0: 6d20 6120 6672 616d 6520 6865 6164 6572  m a frame header
+000083f0: 2e0a 2020 2020 2020 2020 2a20 6675 6e63  ..        * func
+00008400: 7469 6f6e 203a 7079 3a66 756e 633a 6067  tion :py:func:`g
+00008410: 6574 5f66 7261 6d65 5f73 697a 6560 2c20  et_frame_size`, 
+00008420: 6765 7420 6120 6672 616d 6527 7320 7369  get a frame's si
+00008430: 7a65 2e0a 0a2e 2e20 7079 3a66 756e 6374  ze..... py:funct
+00008440: 696f 6e3a 3a20 6765 745f 6672 616d 655f  ion:: get_frame_
+00008450: 696e 666f 2866 7261 6d65 5f62 7566 6665  info(frame_buffe
+00008460: 7229 0a0a 2020 2020 4765 7420 7a73 7464  r)..    Get zstd
+00008470: 2066 7261 6d65 2069 6e66 6f72 6d61 7469   frame informati
+00008480: 6f6e 2066 726f 6d20 6120 6672 616d 6520  on from a frame 
+00008490: 6865 6164 6572 2e0a 0a20 2020 2052 6574  header...    Ret
+000084a0: 7572 6e20 6120 322d 6974 656d 206e 616d  urn a 2-item nam
+000084b0: 6564 7475 706c 653a 2028 6465 636f 6d70  edtuple: (decomp
+000084c0: 7265 7373 6564 5f73 697a 652c 2064 6963  ressed_size, dic
+000084d0: 7469 6f6e 6172 795f 6964 290a 0a20 2020  tionary_id)..   
+000084e0: 2049 6620 6060 6465 636f 6d70 7265 7373   If ``decompress
+000084f0: 6564 5f73 697a 6560 6020 6973 2060 604e  ed_size`` is ``N
+00008500: 6f6e 6560 602c 2064 6563 6f6d 7072 6573  one``, decompres
+00008510: 7365 6420 7369 7a65 2069 7320 756e 6b6e  sed size is unkn
+00008520: 6f77 6e2e 0a0a 2020 2020 6060 6469 6374  own...    ``dict
+00008530: 696f 6e61 7279 5f69 6460 6020 6973 2061  ionary_id`` is a
+00008540: 2033 322d 6269 7420 756e 7369 676e 6564   32-bit unsigned
+00008550: 2069 6e74 6567 6572 2076 616c 7565 2e20   integer value. 
+00008560: 6060 3060 6020 6d65 616e 7320 6469 6374  ``0`` means dict
+00008570: 696f 6e61 7279 2049 4420 7761 7320 6e6f  ionary ID was no
+00008580: 7420 7265 636f 7264 6564 2069 6e20 6672  t recorded in fr
+00008590: 616d 6520 6865 6164 6572 2c20 7468 6520  ame header, the 
+000085a0: 6672 616d 6520 6d61 7920 6f72 206d 6179  frame may or may
+000085b0: 206e 6f74 206e 6565 6420 6120 6469 6374   not need a dict
+000085c0: 696f 6e61 7279 2074 6f20 6265 2064 6563  ionary to be dec
+000085d0: 6f64 6564 2c20 616e 6420 7468 6520 4944  oded, and the ID
+000085e0: 206f 6620 7375 6368 2061 2064 6963 7469   of such a dicti
+000085f0: 6f6e 6172 7920 6973 206e 6f74 2073 7065  onary is not spe
+00008600: 6369 6669 6564 2e20 284e 6f74 6520 7468  cified. (Note th
+00008610: 6174 2074 6865 206d 6561 6e69 6e67 206f  at the meaning o
+00008620: 6620 6060 3060 6020 6973 2064 6966 6665  f ``0`` is diffe
+00008630: 7265 6e74 2066 726f 6d20 3a70 793a 6174  rent from :py:at
+00008640: 7472 3a60 5a73 7464 4469 6374 2e64 6963  tr:`ZstdDict.dic
+00008650: 745f 6964 6020 6174 7472 6962 7574 652e  t_id` attribute.
+00008660: 290a 0a20 2020 2049 7427 7320 706f 7373  )..    It's poss
+00008670: 6962 6c65 2074 6f20 6170 7065 6e64 206d  ible to append m
+00008680: 6f72 6520 6974 656d 7320 746f 2074 6865  ore items to the
+00008690: 206e 616d 6564 7475 706c 6520 696e 2074   namedtuple in t
+000086a0: 6865 2066 7574 7572 652e 0a0a 2020 2020  he future...    
+000086b0: 3a70 6172 616d 2066 7261 6d65 5f62 7566  :param frame_buf
+000086c0: 6665 723a 2049 7420 7368 6f75 6c64 2073  fer: It should s
+000086d0: 7461 7274 7320 6672 6f6d 2074 6865 2062  tarts from the b
+000086e0: 6567 696e 6e69 6e67 206f 6620 6120 6672  eginning of a fr
+000086f0: 616d 652c 2061 6e64 2063 6f6e 7461 696e  ame, and contain
+00008700: 7320 6174 206c 6561 7374 2074 6865 2066  s at least the f
+00008710: 7261 6d65 2068 6561 6465 7220 2836 2074  rame header (6 t
+00008720: 6f20 3138 2062 7974 6573 292e 0a20 2020  o 18 bytes)..   
+00008730: 203a 7479 7065 2066 7261 6d65 5f62 7566   :type frame_buf
+00008740: 6665 723a 2062 7974 6573 2d6c 696b 6520  fer: bytes-like 
+00008750: 6f62 6a65 6374 0a20 2020 203a 7265 7475  object.    :retu
+00008760: 726e 3a20 496e 666f 726d 6174 696f 6e20  rn: Information 
+00008770: 6162 6f75 7420 6120 6672 616d 652e 0a20  about a frame.. 
+00008780: 2020 203a 7274 7970 653a 206e 616d 6564     :rtype: named
+00008790: 7475 706c 650a 2020 2020 3a72 6169 7365  tuple.    :raise
+000087a0: 7320 5a73 7464 4572 726f 723a 2057 6865  s ZstdError: Whe
+000087b0: 6e20 7061 7273 696e 6720 7468 6520 6672  n parsing the fr
+000087c0: 616d 6520 6865 6164 6572 2066 6169 6c73  ame header fails
+000087d0: 2e0a 0a2e 2e20 736f 7572 6365 636f 6465  ..... sourcecode
+000087e0: 3a3a 2070 7974 686f 6e0a 0a20 2020 203e  :: python..    >
+000087f0: 3e3e 2070 797a 7374 642e 6765 745f 6672  >> pyzstd.get_fr
+00008800: 616d 655f 696e 666f 2863 6f6d 7072 6573  ame_info(compres
+00008810: 7365 645f 6461 745b 3a32 305d 290a 2020  sed_dat[:20]).  
+00008820: 2020 6672 616d 655f 696e 666f 2864 6563    frame_info(dec
+00008830: 6f6d 7072 6573 7365 645f 7369 7a65 3d36  ompressed_size=6
+00008840: 3837 3337 392c 2064 6963 7469 6f6e 6172  87379, dictionar
+00008850: 795f 6964 3d31 3034 3039 3932 3236 3829  y_id=1040992268)
+00008860: 0a0a 0a2e 2e20 7079 3a66 756e 6374 696f  ..... py:functio
+00008870: 6e3a 3a20 6765 745f 6672 616d 655f 7369  n:: get_frame_si
+00008880: 7a65 2866 7261 6d65 5f62 7566 6665 7229  ze(frame_buffer)
+00008890: 0a0a 2020 2020 4765 7420 7468 6520 7369  ..    Get the si
+000088a0: 7a65 206f 6620 6120 7a73 7464 2066 7261  ze of a zstd fra
+000088b0: 6d65 2c20 696e 636c 7564 696e 6720 6672  me, including fr
+000088c0: 616d 6520 6865 6164 6572 2061 6e64 2034  ame header and 4
+000088d0: 2d62 7974 6520 6368 6563 6b73 756d 2069  -byte checksum i
+000088e0: 6620 6974 2068 6173 2e0a 0a20 2020 2049  f it has...    I
+000088f0: 7420 7769 6c6c 2069 7465 7261 7465 2061  t will iterate a
+00008900: 6c6c 2062 6c6f 636b 7327 2068 6561 6465  ll blocks' heade
+00008910: 7220 7769 7468 696e 2061 2066 7261 6d65  r within a frame
+00008920: 2c20 746f 2061 6363 756d 756c 6174 6520  , to accumulate 
+00008930: 7468 6520 6672 616d 6527 7320 7369 7a65  the frame's size
+00008940: 2e0a 0a20 2020 203a 7061 7261 6d20 6672  ...    :param fr
+00008950: 616d 655f 6275 6666 6572 3a20 4974 2073  ame_buffer: It s
+00008960: 686f 756c 6420 7374 6172 7473 2066 726f  hould starts fro
+00008970: 6d20 7468 6520 6265 6769 6e6e 696e 6720  m the beginning 
+00008980: 6f66 2061 2066 7261 6d65 2c20 616e 6420  of a frame, and 
+00008990: 636f 6e74 6169 6e73 2061 7420 6c65 6173  contains at leas
+000089a0: 7420 6f6e 6520 636f 6d70 6c65 7465 2066  t one complete f
+000089b0: 7261 6d65 2e0a 2020 2020 3a74 7970 6520  rame..    :type 
+000089c0: 6672 616d 655f 6275 6666 6572 3a20 6279  frame_buffer: by
+000089d0: 7465 732d 6c69 6b65 206f 626a 6563 740a  tes-like object.
+000089e0: 2020 2020 3a72 6574 7572 6e3a 2054 6865      :return: The
+000089f0: 2073 697a 6520 6f66 2061 207a 7374 6420   size of a zstd 
+00008a00: 6672 616d 652e 0a20 2020 203a 7274 7970  frame..    :rtyp
+00008a10: 653a 2069 6e74 0a20 2020 203a 7261 6973  e: int.    :rais
+00008a20: 6573 205a 7374 6445 7272 6f72 3a20 5768  es ZstdError: Wh
+00008a30: 656e 2069 7420 6661 696c 732e 0a0a 2e2e  en it fails.....
+00008a40: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
+00008a50: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 7079  thon..    >>> py
+00008a60: 7a73 7464 2e67 6574 5f66 7261 6d65 5f73  zstd.get_frame_s
+00008a70: 697a 6528 636f 6d70 7265 7373 6564 5f64  ize(compressed_d
+00008a80: 6174 290a 2020 2020 3235 3238 3734 0a0a  at).    252874..
+00008a90: 0a4d 6f64 756c 652d 6c65 7665 6c20 7661  .Module-level va
+00008aa0: 7269 6162 6c65 730a 2d2d 2d2d 2d2d 2d2d  riables.--------
+00008ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00008ac0: 2020 2020 5468 6973 2073 6563 7469 6f6e      This section
+00008ad0: 2063 6f6e 7461 696e 733a 0a0a 2020 2020   contains:..    
+00008ae0: 2020 2020 2a20 3a70 793a 6461 7461 3a60      * :py:data:`
+00008af0: 7a73 7464 5f76 6572 7369 6f6e 602c 2061  zstd_version`, a
+00008b00: 2060 6073 7472 6060 2e0a 2020 2020 2020   ``str``..      
+00008b10: 2020 2a20 3a70 793a 6461 7461 3a60 7a73    * :py:data:`zs
+00008b20: 7464 5f76 6572 7369 6f6e 5f69 6e66 6f60  td_version_info`
+00008b30: 2c20 6120 6060 7475 706c 6560 602e 0a20  , a ``tuple``.. 
+00008b40: 2020 2020 2020 202a 203a 7079 3a64 6174         * :py:dat
+00008b50: 613a 6063 6f6d 7072 6573 7369 6f6e 4c65  a:`compressionLe
+00008b60: 7665 6c5f 7661 6c75 6573 602c 2073 6f6d  vel_values`, som
+00008b70: 6520 7661 6c75 6573 2064 6566 696e 6564  e values defined
+00008b80: 2062 7920 7468 6520 756e 6465 726c 7969   by the underlyi
+00008b90: 6e67 207a 7374 6420 6c69 6272 6172 792e  ng zstd library.
+00008ba0: 0a20 2020 2020 2020 202a 203a 7079 3a64  .        * :py:d
+00008bb0: 6174 613a 607a 7374 645f 7375 7070 6f72  ata:`zstd_suppor
+00008bc0: 745f 6d75 6c74 6974 6872 6561 6460 2c20  t_multithread`, 
+00008bd0: 7768 6574 6865 7220 7468 6520 756e 6465  whether the unde
+00008be0: 726c 7969 6e67 207a 7374 6420 6c69 6272  rlying zstd libr
+00008bf0: 6172 7920 7375 7070 6f72 7473 206d 756c  ary supports mul
+00008c00: 7469 2d74 6872 6561 6465 6420 636f 6d70  ti-threaded comp
+00008c10: 7265 7373 696f 6e2e 0a0a 2e2e 2070 793a  ression..... py:
+00008c20: 6461 7461 3a3a 207a 7374 645f 7665 7273  data:: zstd_vers
+00008c30: 696f 6e0a 0a20 2020 2055 6e64 6572 6c79  ion..    Underly
+00008c40: 696e 6720 7a73 7464 206c 6962 7261 7279  ing zstd library
+00008c50: 2773 2076 6572 7369 6f6e 2c20 6060 7374  's version, ``st
+00008c60: 7260 6020 666f 726d 2e0a 0a2e 2e20 736f  r`` form..... so
+00008c70: 7572 6365 636f 6465 3a3a 2070 7974 686f  urcecode:: pytho
+00008c80: 6e0a 0a20 2020 203e 3e3e 2070 797a 7374  n..    >>> pyzst
+00008c90: 642e 7a73 7464 5f76 6572 7369 6f6e 0a20  d.zstd_version. 
+00008ca0: 2020 2027 312e 342e 3527 0a0a 0a2e 2e20     '1.4.5'..... 
+00008cb0: 7079 3a64 6174 613a 3a20 7a73 7464 5f76  py:data:: zstd_v
+00008cc0: 6572 7369 6f6e 5f69 6e66 6f0a 0a20 2020  ersion_info..   
+00008cd0: 2055 6e64 6572 6c79 696e 6720 7a73 7464   Underlying zstd
+00008ce0: 206c 6962 7261 7279 2773 2076 6572 7369   library's versi
+00008cf0: 6f6e 2c20 6060 7475 706c 6560 6020 666f  on, ``tuple`` fo
+00008d00: 726d 2e0a 0a2e 2e20 736f 7572 6365 636f  rm..... sourceco
+00008d10: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
+00008d20: 203e 3e3e 2070 797a 7374 642e 7a73 7464   >>> pyzstd.zstd
+00008d30: 5f76 6572 7369 6f6e 5f69 6e66 6f0a 2020  _version_info.  
+00008d40: 2020 2831 2c20 342c 2035 290a 0a0a 2e2e    (1, 4, 5).....
+00008d50: 2070 793a 6461 7461 3a3a 2063 6f6d 7072   py:data:: compr
+00008d60: 6573 7369 6f6e 4c65 7665 6c5f 7661 6c75  essionLevel_valu
+00008d70: 6573 0a0a 2020 2020 4120 332d 6974 656d  es..    A 3-item
+00008d80: 206e 616d 6564 7475 706c 652c 2076 616c   namedtuple, val
+00008d90: 7565 7320 6465 6669 6e65 6420 6279 2074  ues defined by t
+00008da0: 6865 2075 6e64 6572 6c79 696e 6720 7a73  he underlying zs
+00008db0: 7464 206c 6962 7261 7279 2c20 7365 6520  td library, see 
+00008dc0: 3a72 6566 3a60 636f 6d70 7265 7373 696f  :ref:`compressio
+00008dd0: 6e20 6c65 7665 6c3c 636f 6d70 7265 7373  n level<compress
+00008de0: 696f 6e5f 6c65 7665 6c3e 6020 666f 7220  ion_level>` for 
+00008df0: 6465 7461 696c 732e 0a0a 2020 2020 6060  details...    ``
+00008e00: 6465 6661 756c 7460 6020 6973 2064 6566  default`` is def
+00008e10: 6175 6c74 2063 6f6d 7072 6573 7369 6f6e  ault compression
+00008e20: 206c 6576 656c 2c20 6974 2069 7320 7573   level, it is us
+00008e30: 6564 2077 6865 6e20 636f 6d70 7265 7373  ed when compress
+00008e40: 696f 6e20 6c65 7665 6c20 6973 2073 6574  ion level is set
+00008e50: 2074 6f20 6060 3060 6020 6f72 206e 6f74   to ``0`` or not
+00008e60: 2073 6574 2e0a 0a20 2020 2060 606d 696e   set...    ``min
+00008e70: 6060 2f60 606d 6178 6060 2061 7265 206d  ``/``max`` are m
+00008e80: 696e 696d 756d 2f6d 6178 696d 756d 2061  inimum/maximum a
+00008e90: 7661 696c 6162 6c65 2076 616c 7565 7320  vailable values 
+00008ea0: 6f66 2063 6f6d 7072 6573 7369 6f6e 206c  of compression l
+00008eb0: 6576 656c 2c20 626f 7468 2069 6e63 6c75  evel, both inclu
+00008ec0: 7369 7665 2e0a 0a2e 2e20 736f 7572 6365  sive..... source
+00008ed0: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
+00008ee0: 2020 203e 3e3e 2070 797a 7374 642e 636f     >>> pyzstd.co
+00008ef0: 6d70 7265 7373 696f 6e4c 6576 656c 5f76  mpressionLevel_v
+00008f00: 616c 7565 7320 2023 2031 3331 3037 3220  alues  # 131072 
+00008f10: 3d20 3132 382a 3130 3234 0a20 2020 2076  = 128*1024.    v
+00008f20: 616c 7565 7328 6465 6661 756c 743d 332c  alues(default=3,
+00008f30: 206d 696e 3d2d 3133 3130 3732 2c20 6d61   min=-131072, ma
+00008f40: 783d 3232 290a 0a0a 2e2e 2070 793a 6461  x=22)..... py:da
+00008f50: 7461 3a3a 207a 7374 645f 7375 7070 6f72  ta:: zstd_suppor
+00008f60: 745f 6d75 6c74 6974 6872 6561 640a 0a20  t_multithread.. 
+00008f70: 2020 2057 6865 7468 6572 2074 6865 2075     Whether the u
+00008f80: 6e64 6572 6c79 696e 6720 7a73 7464 206c  nderlying zstd l
+00008f90: 6962 7261 7279 2077 6173 2063 6f6d 7069  ibrary was compi
+00008fa0: 6c65 6420 7769 7468 203a 7265 663a 606d  led with :ref:`m
+00008fb0: 756c 7469 2d74 6872 6561 6465 6420 636f  ulti-threaded co
+00008fc0: 6d70 7265 7373 696f 6e3c 6d74 5f63 6f6d  mpression<mt_com
+00008fd0: 7072 6573 7369 6f6e 3e60 2073 7570 706f  pression>` suppo
+00008fe0: 7274 2e0a 0a20 2020 2049 7427 7320 616c  rt...    It's al
+00008ff0: 6d6f 7374 2061 6c77 6179 7320 6060 5472  most always ``Tr
+00009000: 7565 6060 2e0a 0a20 2020 2049 7427 7320  ue``...    It's 
+00009010: 6060 4661 6c73 6560 6020 7768 656e 2064  ``False`` when d
+00009020: 796e 616d 6963 616c 6c79 206c 696e 6b65  ynamically linke
+00009030: 6420 746f 207a 7374 6420 6c69 6272 6172  d to zstd librar
+00009040: 7920 7468 6174 2063 6f6d 7069 6c65 6420  y that compiled 
+00009050: 7769 7468 6f75 7420 6d75 6c74 692d 7468  without multi-th
+00009060: 7265 6164 6564 2073 7570 706f 7274 2e20  readed support. 
+00009070: 4f72 6469 6e61 7279 2075 7365 7273 2077  Ordinary users w
+00009080: 696c 6c20 6e6f 7420 6d65 6574 2074 6869  ill not meet thi
+00009090: 7320 7369 7475 6174 696f 6e2e 0a0a 2e2e  s situation.....
+000090a0: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
+000090b0: 302e 3135 2e31 0a0a 2e2e 2073 6f75 7263  0.15.1.... sourc
+000090c0: 6563 6f64 653a 3a20 7079 7468 6f6e 0a0a  ecode:: python..
+000090d0: 2020 2020 3e3e 3e20 7079 7a73 7464 2e7a      >>> pyzstd.z
+000090e0: 7374 645f 7375 7070 6f72 745f 6d75 6c74  std_support_mult
+000090f0: 6974 6872 6561 640a 2020 2020 5472 7565  ithread.    True
+00009100: 0a0a 0a5a 7374 6446 696c 6520 636c 6173  ...ZstdFile clas
+00009110: 7320 616e 6420 6f70 656e 2829 2066 756e  s and open() fun
+00009120: 6374 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d  ction.----------
+00009130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20  -------------.. 
+00009150: 2020 2054 6869 7320 7365 6374 696f 6e20     This section 
+00009160: 636f 6e74 6169 6e73 3a0a 0a20 2020 2020  contains:..     
+00009170: 2020 202a 2063 6c61 7373 203a 7079 3a63     * class :py:c
+00009180: 6c61 7373 3a60 5a73 7464 4669 6c65 602c  lass:`ZstdFile`,
+00009190: 206f 7065 6e20 6120 7a73 7464 2d63 6f6d   open a zstd-com
+000091a0: 7072 6573 7365 6420 6669 6c65 2069 6e20  pressed file in 
+000091b0: 6269 6e61 7279 206d 6f64 652e 0a20 2020  binary mode..   
+000091c0: 2020 2020 202a 2066 756e 6374 696f 6e20       * function 
+000091d0: 3a70 793a 6675 6e63 3a60 6f70 656e 602c  :py:func:`open`,
+000091e0: 206f 7065 6e20 6120 7a73 7464 2d63 6f6d   open a zstd-com
+000091f0: 7072 6573 7365 6420 6669 6c65 2069 6e20  pressed file in 
+00009200: 6269 6e61 7279 206f 7220 7465 7874 206d  binary or text m
+00009210: 6f64 652e 0a0a 2e2e 2070 793a 636c 6173  ode..... py:clas
+00009220: 733a 3a20 5a73 7464 4669 6c65 0a0a 2020  s:: ZstdFile..  
+00009230: 2020 4f70 656e 2061 207a 7374 642d 636f    Open a zstd-co
+00009240: 6d70 7265 7373 6564 2066 696c 6520 696e  mpressed file in
+00009250: 2062 696e 6172 7920 6d6f 6465 2e0a 0a20   binary mode... 
+00009260: 2020 2054 6869 7320 636c 6173 7320 6973     This class is
+00009270: 2076 6572 7920 7369 6d69 6c61 7220 746f   very similar to
+00009280: 2060 627a 322e 425a 3246 696c 6520 3c68   `bz2.BZ2File <h
+00009290: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
+000092a0: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
+000092b0: 2f62 7a32 2e68 746d 6c23 627a 322e 425a  /bz2.html#bz2.BZ
+000092c0: 3246 696c 653e 605f 202f 2020 6067 7a69  2File>`_ /  `gzi
+000092d0: 702e 477a 6970 4669 6c65 203c 6874 7470  p.GzipFile <http
+000092e0: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+000092f0: 6f72 672f 332f 6c69 6272 6172 792f 677a  org/3/library/gz
+00009300: 6970 2e68 746d 6c23 677a 6970 2e47 7a69  ip.html#gzip.Gzi
+00009310: 7046 696c 653e 605f 202f 2060 6c7a 6d61  pFile>`_ / `lzma
+00009320: 2e4c 5a4d 4146 696c 6520 3c68 7474 7073  .LZMAFile <https
+00009330: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00009340: 7267 2f33 2f6c 6962 7261 7279 2f6c 7a6d  rg/3/library/lzm
+00009350: 612e 6874 6d6c 236c 7a6d 612e 4c5a 4d41  a.html#lzma.LZMA
+00009360: 4669 6c65 3e60 5f20 636c 6173 7365 7320  File>`_ classes 
+00009370: 696e 2050 7974 686f 6e20 7374 616e 6461  in Python standa
+00009380: 7264 206c 6962 7261 7279 2e0a 0a20 2020  rd library...   
+00009390: 204c 696b 6520 425a 3246 696c 652f 477a   Like BZ2File/Gz
+000093a0: 6970 4669 6c65 2f4c 5a4d 4146 696c 6520  ipFile/LZMAFile 
+000093b0: 636c 6173 7365 732c 205a 7374 6446 696c  classes, ZstdFil
+000093c0: 6520 6973 206e 6f74 2074 6872 6561 642d  e is not thread-
+000093d0: 7361 6665 2c20 736f 2069 6620 796f 7520  safe, so if you 
+000093e0: 6e65 6564 2074 6f20 7573 6520 6120 7369  need to use a si
+000093f0: 6e67 6c65 205a 7374 6446 696c 6520 6f62  ngle ZstdFile ob
+00009400: 6a65 6374 2066 726f 6d20 6d75 6c74 6970  ject from multip
+00009410: 6c65 2074 6872 6561 6473 2c20 6974 2069  le threads, it i
+00009420: 7320 6e65 6365 7373 6172 7920 746f 2070  s necessary to p
+00009430: 726f 7465 6374 2069 7420 7769 7468 2061  rotect it with a
+00009440: 206c 6f63 6b2e 0a0a 2020 2020 4974 2063   lock...    It c
+00009450: 616e 2062 6520 7573 6564 2077 6974 6820  an be used with 
+00009460: 5079 7468 6f6e 2773 2060 6074 6172 6669  Python's ``tarfi
+00009470: 6c65 6060 206d 6f64 756c 652c 2073 6565  le`` module, see
+00009480: 203a 7265 663a 6074 6869 7320 6e6f 7465   :ref:`this note
+00009490: 3c77 6974 685f 7461 7266 696c 653e 602e  <with_tarfile>`.
+000094a0: 0a0a 2020 2020 2e2e 2070 793a 6d65 7468  ..    .. py:meth
+000094b0: 6f64 3a3a 205f 5f69 6e69 745f 5f28 7365  od:: __init__(se
+000094c0: 6c66 2c20 6669 6c65 6e61 6d65 2c20 6d6f  lf, filename, mo
+000094d0: 6465 3d22 7222 2c20 2a2c 206c 6576 656c  de="r", *, level
+000094e0: 5f6f 725f 6f70 7469 6f6e 3d4e 6f6e 652c  _or_option=None,
+000094f0: 207a 7374 645f 6469 6374 3d4e 6f6e 6529   zstd_dict=None)
+00009500: 0a0a 2020 2020 2020 2020 5468 6520 2a66  ..        The *f
+00009510: 696c 656e 616d 652a 2070 6172 616d 6574  ilename* paramet
+00009520: 6572 2063 616e 2062 6520 616e 2065 7869  er can be an exi
+00009530: 7374 696e 6720 6066 696c 6520 6f62 6a65  sting `file obje
+00009540: 6374 203c 6874 7470 733a 2f2f 646f 6373  ct <https://docs
+00009550: 2e70 7974 686f 6e2e 6f72 672f 332f 676c  .python.org/3/gl
+00009560: 6f73 7361 7279 2e68 746d 6c23 7465 726d  ossary.html#term
+00009570: 2d66 696c 652d 6f62 6a65 6374 3e60 5f20  -file-object>`_ 
+00009580: 746f 2077 7261 702c 206f 7220 7468 6520  to wrap, or the 
+00009590: 6e61 6d65 206f 6620 7468 6520 6669 6c65  name of the file
+000095a0: 2074 6f20 6f70 656e 2028 6173 2061 2060   to open (as a `
+000095b0: 6073 7472 6060 2c20 6060 6279 7465 7360  `str``, ``bytes`
+000095c0: 6020 6f72 2060 7061 7468 2d6c 696b 6520  ` or `path-like 
+000095d0: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
+000095e0: 7468 6f6e 2e6f 7267 2f33 2f67 6c6f 7373  thon.org/3/gloss
+000095f0: 6172 792e 6874 6d6c 2374 6572 6d2d 7061  ary.html#term-pa
+00009600: 7468 2d6c 696b 652d 6f62 6a65 6374 3e60  th-like-object>`
+00009610: 5f20 6f62 6a65 6374 292e 2057 6865 6e20  _ object). When 
+00009620: 7772 6170 7069 6e67 2061 6e20 6578 6973  wrapping an exis
+00009630: 7469 6e67 2066 696c 6520 6f62 6a65 6374  ting file object
+00009640: 2c20 7468 6520 7772 6170 7065 6420 6669  , the wrapped fi
+00009650: 6c65 2077 696c 6c20 6e6f 7420 6265 2063  le will not be c
+00009660: 6c6f 7365 6420 7768 656e 2074 6865 205a  losed when the Z
+00009670: 7374 6446 696c 6520 6973 2063 6c6f 7365  stdFile is close
+00009680: 642e 0a0a 2020 2020 2020 2020 5468 6520  d...        The 
+00009690: 2a6d 6f64 652a 2070 6172 616d 6574 6572  *mode* parameter
+000096a0: 2063 616e 2062 6520 6569 7468 6572 2022   can be either "
+000096b0: 7222 2066 6f72 2072 6561 6469 6e67 2028  r" for reading (
+000096c0: 6465 6661 756c 7429 2c20 2277 2220 666f  default), "w" fo
+000096d0: 7220 6f76 6572 7772 6974 696e 672c 2022  r overwriting, "
+000096e0: 7822 2066 6f72 2065 7863 6c75 7369 7665  x" for exclusive
+000096f0: 2063 7265 6174 696f 6e2c 206f 7220 2261   creation, or "a
+00009700: 2220 666f 7220 6170 7065 6e64 696e 672e  " for appending.
+00009710: 2054 6865 7365 2063 616e 2065 7175 6976   These can equiv
+00009720: 616c 656e 746c 7920 6265 2067 6976 656e  alently be given
+00009730: 2061 7320 2272 6222 2c20 2277 6222 2c20   as "rb", "wb", 
+00009740: 2278 6222 2061 6e64 2022 6162 2220 7265  "xb" and "ab" re
+00009750: 7370 6563 7469 7665 6c79 2e0a 0a20 2020  spectively...   
+00009760: 2020 2020 2049 6620 696e 2072 6561 6469       If in readi
+00009770: 6e67 206d 6f64 6520 2864 6563 6f6d 7072  ng mode (decompr
+00009780: 6573 7369 6f6e 293a 0a0a 2020 2020 2020  ession):..      
+00009790: 2020 2020 2020 2a20 5468 6520 2a6c 6576        * The *lev
+000097a0: 656c 5f6f 725f 6f70 7469 6f6e 2a20 7061  el_or_option* pa
+000097b0: 7261 6d65 7465 7220 6361 6e20 6f6e 6c79  rameter can only
+000097c0: 2062 6520 6120 6060 6469 6374 6060 206f   be a ``dict`` o
+000097d0: 626a 6563 742c 2074 6861 7420 7265 7072  bject, that repr
+000097e0: 6573 656e 7473 2064 6563 6f6d 7072 6573  esents decompres
+000097f0: 7369 6f6e 206f 7074 696f 6e2e 2049 7420  sion option. It 
+00009800: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+00009810: 6060 696e 7460 6020 7479 7065 2063 6f6d  ``int`` type com
+00009820: 7072 6573 7369 6f6e 206c 6576 656c 2069  pression level i
+00009830: 6e20 7468 6973 2063 6173 652e 0a20 2020  n this case..   
+00009840: 2020 2020 2020 2020 202a 2054 6865 2069           * The i
+00009850: 6e70 7574 2066 696c 6520 6d61 7920 6265  nput file may be
+00009860: 2074 6865 2063 6f6e 6361 7465 6e61 7469   the concatenati
+00009870: 6f6e 206f 6620 6d75 6c74 6970 6c65 203a  on of multiple :
+00009880: 7265 663a 6066 7261 6d65 733c 6672 616d  ref:`frames<fram
+00009890: 655f 626c 6f63 6b3e 602e 0a0a 2020 2020  e_block>`...    
+000098a0: 496e 2077 7269 7469 6e67 206d 6f64 6520  In writing mode 
+000098b0: 2863 6f6d 7072 6573 7369 6f6e 292c 2074  (compression), t
+000098c0: 6865 7365 206d 6574 686f 6473 2061 7265  hese methods are
+000098d0: 2061 7661 696c 6162 6c65 3a0a 0a20 2020   available:..   
+000098e0: 2020 2020 202a 2060 2e77 7269 7465 2862       * `.write(b
+000098f0: 2920 3c68 7474 7073 3a2f 2f64 6f63 732e  ) <https://docs.
+00009900: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+00009910: 7261 7279 2f69 6f2e 6874 6d6c 2369 6f2e  rary/io.html#io.
+00009920: 4275 6666 6572 6564 494f 4261 7365 2e77  BufferedIOBase.w
+00009930: 7269 7465 3e60 5f0a 2020 2020 2020 2020  rite>`_.        
+00009940: 2a20 602e 666c 7573 6828 2920 3c68 7474  * `.flush() <htt
+00009950: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00009960: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f69  .org/3/library/i
+00009970: 6f2e 6874 6d6c 2369 6f2e 494f 4261 7365  o.html#io.IOBase
+00009980: 2e66 6c75 7368 3e60 5f2c 2066 6c75 7368  .flush>`_, flush
+00009990: 2074 6f20 7468 6520 756e 6465 726c 7969   to the underlyi
+000099a0: 6e67 2073 7472 6561 6d2e 2049 7420 7573  ng stream. It us
+000099b0: 6573 203a 7079 3a61 7474 723a 605a 7374  es :py:attr:`Zst
+000099c0: 6443 6f6d 7072 6573 736f 722e 464c 5553  dCompressor.FLUS
+000099d0: 485f 424c 4f43 4b60 206d 6f64 652c 2061  H_BLOCK` mode, a
+000099e0: 6275 7365 206f 6620 7468 6973 206d 6574  buse of this met
+000099f0: 686f 6420 7769 6c6c 2072 6564 7563 6520  hod will reduce 
+00009a00: 636f 6d70 7265 7373 696f 6e20 7261 7469  compression rati
+00009a10: 6f2c 2075 7365 2069 7420 6f6e 6c79 2077  o, use it only w
+00009a20: 6865 6e20 6e65 6365 7373 6172 792e 2049  hen necessary. I
+00009a30: 6620 7468 6520 7072 6f67 7261 6d20 6973  f the program is
+00009a40: 2069 6e74 6572 7275 7074 6564 2061 6674   interrupted aft
+00009a50: 6572 7761 7264 732c 2061 6c6c 2064 6174  erwards, all dat
+00009a60: 6120 6361 6e20 6265 2072 6563 6f76 6572  a can be recover
+00009a70: 6564 2e20 546f 2065 6e73 7572 6520 7361  ed. To ensure sa
+00009a80: 7669 6e67 2074 6f20 6469 736b 2c20 616c  ving to disk, al
+00009a90: 736f 206e 6565 6420 606f 732e 6673 796e  so need `os.fsyn
+00009aa0: 6328 6664 2920 3c68 7474 7073 3a2f 2f64  c(fd) <https://d
+00009ab0: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
+00009ac0: 2f6c 6962 7261 7279 2f6f 732e 6874 6d6c  /library/os.html
+00009ad0: 236f 732e 6673 796e 633e 605f 2e20 2028  #os.fsync>`_.  (
+00009ae0: 2a49 6d70 6c65 6d65 6e74 6564 2069 6e20  *Implemented in 
+00009af0: 7665 7273 696f 6e20 302e 3135 2e31 2a29  version 0.15.1*)
+00009b00: 0a0a 2020 2020 496e 2072 6561 6469 6e67  ..    In reading
+00009b10: 206d 6f64 6520 2864 6563 6f6d 7072 6573   mode (decompres
+00009b20: 7369 6f6e 292c 2074 6865 7365 206d 6574  sion), these met
+00009b30: 686f 6473 2061 6e64 2073 7461 7465 6d65  hods and stateme
+00009b40: 6e74 2061 7265 2061 7661 696c 6162 6c65  nt are available
+00009b50: 3a0a 0a20 2020 2020 2020 202a 2060 2e72  :..        * `.r
+00009b60: 6561 6428 7369 7a65 3d2d 3129 203c 6874  ead(size=-1) <ht
+00009b70: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00009b80: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00009b90: 696f 2e68 746d 6c23 696f 2e42 7566 6665  io.html#io.Buffe
+00009ba0: 7265 6452 6561 6465 722e 7265 6164 3e60  redReader.read>`
+00009bb0: 5f0a 2020 2020 2020 2020 2a20 602e 7265  _.        * `.re
+00009bc0: 6164 3128 7369 7a65 3d2d 3129 203c 6874  ad1(size=-1) <ht
+00009bd0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00009be0: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00009bf0: 696f 2e68 746d 6c23 696f 2e42 7566 6665  io.html#io.Buffe
+00009c00: 7265 6452 6561 6465 722e 7265 6164 313e  redReader.read1>
+00009c10: 605f 0a20 2020 2020 2020 202a 2060 2e72  `_.        * `.r
+00009c20: 6561 6469 6e74 6f28 6229 203c 6874 7470  eadinto(b) <http
+00009c30: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+00009c40: 6f72 672f 332f 6c69 6272 6172 792f 696f  org/3/library/io
+00009c50: 2e68 746d 6c23 696f 2e42 7566 6665 7265  .html#io.Buffere
+00009c60: 6449 4f42 6173 652e 7265 6164 696e 746f  dIOBase.readinto
+00009c70: 3e60 5f0a 2020 2020 2020 2020 2a20 602e  >`_.        * `.
+00009c80: 7265 6164 696e 746f 3128 6229 203c 6874  readinto1(b) <ht
+00009c90: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00009ca0: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00009cb0: 696f 2e68 746d 6c23 696f 2e42 7566 6665  io.html#io.Buffe
+00009cc0: 7265 6449 4f42 6173 652e 7265 6164 696e  redIOBase.readin
+00009cd0: 746f 313e 605f 0a20 2020 2020 2020 202a  to1>`_.        *
+00009ce0: 2060 2e72 6561 646c 696e 6528 7369 7a65   `.readline(size
+00009cf0: 3d2d 3129 203c 6874 7470 733a 2f2f 646f  =-1) <https://do
+00009d00: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+00009d10: 6c69 6272 6172 792f 696f 2e68 746d 6c23  library/io.html#
+00009d20: 696f 2e49 4f42 6173 652e 7265 6164 6c69  io.IOBase.readli
+00009d30: 6e65 3e60 5f0a 2020 2020 2020 2020 2a20  ne>`_.        * 
+00009d40: 602e 7365 656b 286f 6666 7365 742c 2077  `.seek(offset, w
+00009d50: 6865 6e63 653d 696f 2e53 4545 4b5f 5345  hence=io.SEEK_SE
+00009d60: 5429 203c 6874 7470 733a 2f2f 646f 6373  T) <https://docs
+00009d70: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+00009d80: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
+00009d90: 2e49 4f42 6173 652e 7365 656b 3e60 5f2c  .IOBase.seek>`_,
+00009da0: 206e 6f74 6520 7468 6174 2069 6620 6060   note that if ``
+00009db0: 2e73 6565 6b28 2960 6020 746f 2022 7072  .seek()`` to "pr
+00009dc0: 6576 696f 7573 2070 6f73 6974 696f 6e22  evious position"
+00009dd0: 206f 7220 2270 6f73 6974 696f 6e20 7265   or "position re
+00009de0: 6c61 7469 7665 2074 6f20 454f 4620 2874  lative to EOF (t
+00009df0: 6865 2066 6972 7374 2074 696d 6529 222c  he first time)",
+00009e00: 2074 6865 2064 6563 6f6d 7072 6573 7369   the decompressi
+00009e10: 6f6e 2068 6173 2074 6f20 6265 2072 6573  on has to be res
+00009e20: 7461 7274 6564 2066 726f 6d20 7a65 726f  tarted from zero
+00009e30: 2e0a 2020 2020 2020 2020 2a20 602e 7065  ..        * `.pe
+00009e40: 656b 2873 697a 653d 2d31 2920 3c68 7474  ek(size=-1) <htt
+00009e50: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00009e60: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f69  .org/3/library/i
+00009e70: 6f2e 6874 6d6c 2369 6f2e 4275 6666 6572  o.html#io.Buffer
+00009e80: 6564 5265 6164 6572 2e70 6565 6b3e 605f  edReader.peek>`_
+00009e90: 0a20 2020 2020 2020 202a 2060 4974 6572  .        * `Iter
+00009ea0: 6174 696f 6e20 3c68 7474 7073 3a2f 2f64  ation <https://d
+00009eb0: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
+00009ec0: 2f6c 6962 7261 7279 2f69 6f2e 6874 6d6c  /library/io.html
+00009ed0: 2369 6f2e 494f 4261 7365 3e60 5f2c 2079  #io.IOBase>`_, y
+00009ee0: 6965 6c64 206c 696e 6573 2c20 6c69 6e65  ield lines, line
+00009ef0: 2074 6572 6d69 6e61 746f 7220 6973 2060   terminator is `
+00009f00: 6062 275c 6e27 6060 2e0a 0a20 2020 2049  `b'\n'``...    I
+00009f10: 6e20 626f 7468 2072 6561 6469 6e67 2061  n both reading a
+00009f20: 6e64 2077 7269 7469 6e67 206d 6f64 6573  nd writing modes
+00009f30: 2c20 7468 6573 6520 6d65 7468 6f64 7320  , these methods 
+00009f40: 616e 6420 7072 6f70 6572 7479 2061 7265  and property are
+00009f50: 2061 7661 696c 6162 6c65 3a0a 0a20 2020   available:..   
+00009f60: 2020 2020 202a 2060 2e63 6c6f 7365 2829       * `.close()
+00009f70: 203c 6874 7470 733a 2f2f 646f 6373 2e70   <https://docs.p
+00009f80: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
+00009f90: 6172 792f 696f 2e68 746d 6c23 696f 2e49  ary/io.html#io.I
+00009fa0: 4f42 6173 652e 636c 6f73 653e 605f 0a20  OBase.close>`_. 
+00009fb0: 2020 2020 2020 202a 2060 2e74 656c 6c28         * `.tell(
+00009fc0: 2920 3c68 7474 7073 3a2f 2f64 6f63 732e  ) <https://docs.
+00009fd0: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+00009fe0: 7261 7279 2f69 6f2e 6874 6d6c 2369 6f2e  rary/io.html#io.
+00009ff0: 494f 4261 7365 2e74 656c 6c3e 605f 0a20  IOBase.tell>`_. 
+0000a000: 2020 2020 2020 202a 2060 2e66 696c 656e         * `.filen
+0000a010: 6f28 2920 3c68 7474 7073 3a2f 2f64 6f63  o() <https://doc
+0000a020: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+0000a030: 6962 7261 7279 2f69 6f2e 6874 6d6c 2369  ibrary/io.html#i
+0000a040: 6f2e 494f 4261 7365 2e66 696c 656e 6f3e  o.IOBase.fileno>
+0000a050: 605f 0a20 2020 2020 2020 202a 2060 2e63  `_.        * `.c
+0000a060: 6c6f 7365 6420 3c68 7474 7073 3a2f 2f64  losed <https://d
+0000a070: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
+0000a080: 2f6c 6962 7261 7279 2f69 6f2e 6874 6d6c  /library/io.html
+0000a090: 2369 6f2e 494f 4261 7365 2e63 6c6f 7365  #io.IOBase.close
+0000a0a0: 643e 605f 2028 6120 7072 6f70 6572 7479  d>`_ (a property
+0000a0b0: 2061 7474 7269 6275 7465 290a 2020 2020   attribute).    
+0000a0c0: 2020 2020 2a20 602e 7772 6974 6162 6c65      * `.writable
+0000a0d0: 2829 203c 6874 7470 733a 2f2f 646f 6373  () <https://docs
+0000a0e0: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+0000a0f0: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
+0000a100: 2e49 4f42 6173 652e 7772 6974 6162 6c65  .IOBase.writable
+0000a110: 3e60 5f0a 2020 2020 2020 2020 2a20 602e  >`_.        * `.
+0000a120: 7265 6164 6162 6c65 2829 203c 6874 7470  readable() <http
+0000a130: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+0000a140: 6f72 672f 332f 6c69 6272 6172 792f 696f  org/3/library/io
+0000a150: 2e68 746d 6c23 696f 2e49 4f42 6173 652e  .html#io.IOBase.
+0000a160: 7265 6164 6162 6c65 3e60 5f0a 2020 2020  readable>`_.    
+0000a170: 2020 2020 2a20 602e 7365 656b 6162 6c65      * `.seekable
+0000a180: 2829 203c 6874 7470 733a 2f2f 646f 6373  () <https://docs
+0000a190: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+0000a1a0: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
+0000a1b0: 2e49 4f42 6173 652e 7365 656b 6162 6c65  .IOBase.seekable
+0000a1c0: 3e60 5f0a 0a2e 2e20 7079 3a66 756e 6374  >`_.... py:funct
+0000a1d0: 696f 6e3a 3a20 6f70 656e 2866 696c 656e  ion:: open(filen
+0000a1e0: 616d 652c 206d 6f64 653d 2272 6222 2c20  ame, mode="rb", 
+0000a1f0: 2a2c 206c 6576 656c 5f6f 725f 6f70 7469  *, level_or_opti
+0000a200: 6f6e 3d4e 6f6e 652c 207a 7374 645f 6469  on=None, zstd_di
+0000a210: 6374 3d4e 6f6e 652c 2065 6e63 6f64 696e  ct=None, encodin
+0000a220: 673d 4e6f 6e65 2c20 6572 726f 7273 3d4e  g=None, errors=N
+0000a230: 6f6e 652c 206e 6577 6c69 6e65 3d4e 6f6e  one, newline=Non
+0000a240: 6529 0a0a 2020 2020 4f70 656e 2061 207a  e)..    Open a z
+0000a250: 7374 642d 636f 6d70 7265 7373 6564 2066  std-compressed f
+0000a260: 696c 6520 696e 2062 696e 6172 7920 6f72  ile in binary or
+0000a270: 2074 6578 7420 6d6f 6465 2c20 7265 7475   text mode, retu
+0000a280: 726e 696e 6720 6120 6669 6c65 206f 626a  rning a file obj
+0000a290: 6563 742e 0a0a 2020 2020 5468 6973 2066  ect...    This f
+0000a2a0: 756e 6374 696f 6e20 6973 2076 6572 7920  unction is very 
+0000a2b0: 7369 6d69 6c61 7220 746f 2060 627a 322e  similar to `bz2.
+0000a2c0: 6f70 656e 2829 203c 6874 7470 733a 2f2f  open() <https://
+0000a2d0: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+0000a2e0: 332f 6c69 6272 6172 792f 627a 322e 6874  3/library/bz2.ht
+0000a2f0: 6d6c 2362 7a32 2e6f 7065 6e3e 605f 202f  ml#bz2.open>`_ /
+0000a300: 2060 677a 6970 2e6f 7065 6e28 2920 3c68   `gzip.open() <h
+0000a310: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
+0000a320: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
+0000a330: 2f67 7a69 702e 6874 6d6c 2367 7a69 702e  /gzip.html#gzip.
+0000a340: 6f70 656e 3e60 5f20 2f20 606c 7a6d 612e  open>`_ / `lzma.
+0000a350: 6f70 656e 2829 203c 6874 7470 733a 2f2f  open() <https://
+0000a360: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+0000a370: 332f 6c69 6272 6172 792f 6c7a 6d61 2e68  3/library/lzma.h
+0000a380: 746d 6c23 6c7a 6d61 2e6f 7065 6e3e 605f  tml#lzma.open>`_
+0000a390: 2066 756e 6374 696f 6e73 2069 6e20 5079   functions in Py
+0000a3a0: 7468 6f6e 2073 7461 6e64 6172 6420 6c69  thon standard li
+0000a3b0: 6272 6172 792e 0a0a 2020 2020 5468 6520  brary...    The 
+0000a3c0: 2a66 696c 656e 616d 652a 2070 6172 616d  *filename* param
+0000a3d0: 6574 6572 2063 616e 2062 6520 616e 2065  eter can be an e
+0000a3e0: 7869 7374 696e 6720 6066 696c 6520 6f62  xisting `file ob
+0000a3f0: 6a65 6374 203c 6874 7470 733a 2f2f 646f  ject <https://do
+0000a400: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+0000a410: 676c 6f73 7361 7279 2e68 746d 6c23 7465  glossary.html#te
+0000a420: 726d 2d66 696c 652d 6f62 6a65 6374 3e60  rm-file-object>`
+0000a430: 5f20 746f 2077 7261 702c 206f 7220 7468  _ to wrap, or th
+0000a440: 6520 6e61 6d65 206f 6620 7468 6520 6669  e name of the fi
+0000a450: 6c65 2074 6f20 6f70 656e 2028 6173 2061  le to open (as a
+0000a460: 2060 6073 7472 6060 2c20 6060 6279 7465   ``str``, ``byte
+0000a470: 7360 6020 6f72 2060 7061 7468 2d6c 696b  s`` or `path-lik
+0000a480: 6520 3c68 7474 7073 3a2f 2f64 6f63 732e  e <https://docs.
+0000a490: 7079 7468 6f6e 2e6f 7267 2f33 2f67 6c6f  python.org/3/glo
+0000a4a0: 7373 6172 792e 6874 6d6c 2374 6572 6d2d  ssary.html#term-
+0000a4b0: 7061 7468 2d6c 696b 652d 6f62 6a65 6374  path-like-object
+0000a4c0: 3e60 5f20 6f62 6a65 6374 292e 2057 6865  >`_ object). Whe
+0000a4d0: 6e20 7772 6170 7069 6e67 2061 6e20 6578  n wrapping an ex
+0000a4e0: 6973 7469 6e67 2066 696c 6520 6f62 6a65  isting file obje
+0000a4f0: 6374 2c20 7468 6520 7772 6170 7065 6420  ct, the wrapped 
+0000a500: 6669 6c65 2077 696c 6c20 6e6f 7420 6265  file will not be
+0000a510: 2063 6c6f 7365 6420 7768 656e 2074 6865   closed when the
+0000a520: 2072 6574 7572 6e65 6420 6669 6c65 206f   returned file o
+0000a530: 626a 6563 7420 6973 2063 6c6f 7365 642e  bject is closed.
+0000a540: 0a0a 2020 2020 5468 6520 2a6d 6f64 652a  ..    The *mode*
+0000a550: 2070 6172 616d 6574 6572 2063 616e 2062   parameter can b
+0000a560: 6520 616e 7920 6f66 2022 7222 2c20 2272  e any of "r", "r
+0000a570: 6222 2c20 2277 222c 2022 7762 222c 2022  b", "w", "wb", "
+0000a580: 7822 2c20 2278 6222 2c20 2261 2220 6f72  x", "xb", "a" or
+0000a590: 2022 6162 2220 666f 7220 6269 6e61 7279   "ab" for binary
+0000a5a0: 206d 6f64 652c 206f 7220 2272 7422 2c20   mode, or "rt", 
+0000a5b0: 2277 7422 2c20 2278 7422 2c20 6f72 2022  "wt", "xt", or "
+0000a5c0: 6174 2220 666f 7220 7465 7874 206d 6f64  at" for text mod
+0000a5d0: 652e 2054 6865 2064 6566 6175 6c74 2069  e. The default i
+0000a5e0: 7320 2272 6222 2e0a 0a20 2020 2049 6620  s "rb"...    If 
+0000a5f0: 696e 2072 6561 6469 6e67 206d 6f64 6520  in reading mode 
+0000a600: 2864 6563 6f6d 7072 6573 7369 6f6e 292c  (decompression),
+0000a610: 2074 6865 202a 6c65 7665 6c5f 6f72 5f6f   the *level_or_o
+0000a620: 7074 696f 6e2a 2070 6172 616d 6574 6572  ption* parameter
+0000a630: 2063 616e 206f 6e6c 7920 6265 2061 2060   can only be a `
+0000a640: 6064 6963 7460 6020 6f62 6a65 6374 2c20  `dict`` object, 
+0000a650: 7468 6174 2072 6570 7265 7365 6e74 7320  that represents 
+0000a660: 6465 636f 6d70 7265 7373 696f 6e20 6f70  decompression op
+0000a670: 7469 6f6e 2e20 4974 2064 6f65 736e 2774  tion. It doesn't
+0000a680: 2073 7570 706f 7274 2060 6069 6e74 6060   support ``int``
+0000a690: 2074 7970 6520 636f 6d70 7265 7373 696f   type compressio
+0000a6a0: 6e20 6c65 7665 6c20 696e 2074 6869 7320  n level in this 
+0000a6b0: 6361 7365 2e0a 0a20 2020 2049 6e20 6269  case...    In bi
+0000a6c0: 6e61 7279 206d 6f64 652c 2061 203a 7079  nary mode, a :py
+0000a6d0: 3a63 6c61 7373 3a60 5a73 7464 4669 6c65  :class:`ZstdFile
+0000a6e0: 6020 6f62 6a65 6374 2069 7320 7265 7475  ` object is retu
+0000a6f0: 726e 6564 2e0a 0a20 2020 2049 6e20 7465  rned...    In te
+0000a700: 7874 206d 6f64 652c 2061 203a 7079 3a63  xt mode, a :py:c
+0000a710: 6c61 7373 3a60 5a73 7464 4669 6c65 6020  lass:`ZstdFile` 
+0000a720: 6f62 6a65 6374 2069 7320 6372 6561 7465  object is create
+0000a730: 642c 2061 6e64 2077 7261 7070 6564 2069  d, and wrapped i
+0000a740: 6e20 616e 2060 696f 2e54 6578 7449 4f57  n an `io.TextIOW
+0000a750: 7261 7070 6572 203c 6874 7470 733a 2f2f  rapper <https://
+0000a760: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+0000a770: 332f 6c69 6272 6172 792f 696f 2e68 746d  3/library/io.htm
+0000a780: 6c23 696f 2e54 6578 7449 4f57 7261 7070  l#io.TextIOWrapp
+0000a790: 6572 3e60 5f20 6f62 6a65 6374 2077 6974  er>`_ object wit
+0000a7a0: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
+0000a7b0: 656e 636f 6469 6e67 2c20 6572 726f 7220  encoding, error 
+0000a7c0: 6861 6e64 6c69 6e67 2062 6568 6176 696f  handling behavio
+0000a7d0: 722c 2061 6e64 206c 696e 6520 656e 6469  r, and line endi
+0000a7e0: 6e67 2873 292e 0a0a 4164 7661 6e63 6564  ng(s)...Advanced
+0000a7f0: 2070 6172 616d 6574 6572 730a 2d2d 2d2d   parameters.----
+0000a800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+0000a810: 0a20 2020 2054 6869 7320 7365 6374 696f  .    This sectio
+0000a820: 6e20 636f 6e74 6169 6e73 2063 6c61 7373  n contains class
+0000a830: 203a 7079 3a63 6c61 7373 3a60 4350 6172   :py:class:`CPar
+0000a840: 616d 6574 6572 602c 203a 7079 3a63 6c61  ameter`, :py:cla
+0000a850: 7373 3a60 4450 6172 616d 6574 6572 602c  ss:`DParameter`,
+0000a860: 203a 7079 3a63 6c61 7373 3a60 5374 7261   :py:class:`Stra
+0000a870: 7465 6779 602c 2074 6865 7920 6172 6520  tegy`, they are 
+0000a880: 7375 6263 6c61 7373 6573 206f 6620 6060  subclasses of ``
+0000a890: 496e 7445 6e75 6d60 602c 2075 7365 6420  IntEnum``, used 
+0000a8a0: 666f 7220 7365 7474 696e 6720 6164 7661  for setting adva
+0000a8b0: 6e63 6564 2070 6172 616d 6574 6572 732e  nced parameters.
+0000a8c0: 0a0a 2020 2020 3a70 793a 636c 6173 733a  ..    :py:class:
+0000a8d0: 6043 5061 7261 6d65 7465 7260 2063 6c61  `CParameter` cla
+0000a8e0: 7373 2720 6174 7472 6962 7574 6573 3a0a  ss' attributes:.
+0000a8f0: 0a20 2020 2020 2020 202d 2043 6f6d 7072  .        - Compr
+0000a900: 6573 7369 6f6e 206c 6576 656c 2028 3a70  ession level (:p
+0000a910: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
+0000a920: 7465 722e 636f 6d70 7265 7373 696f 6e4c  ter.compressionL
+0000a930: 6576 656c 6029 0a20 2020 2020 2020 202d  evel`).        -
+0000a940: 2043 6f6d 7072 6573 7320 616c 676f 7269   Compress algori
+0000a950: 7468 6d20 7061 7261 6d65 7465 7273 2028  thm parameters (
+0000a960: 3a70 793a 6174 7472 3a60 7e43 5061 7261  :py:attr:`~CPara
+0000a970: 6d65 7465 722e 7769 6e64 6f77 4c6f 6760  meter.windowLog`
+0000a980: 2c20 3a70 793a 6174 7472 3a60 7e43 5061  , :py:attr:`~CPa
+0000a990: 7261 6d65 7465 722e 6861 7368 4c6f 6760  rameter.hashLog`
+0000a9a0: 2c20 3a70 793a 6174 7472 3a60 7e43 5061  , :py:attr:`~CPa
+0000a9b0: 7261 6d65 7465 722e 6368 6169 6e4c 6f67  rameter.chainLog
+0000a9c0: 602c 203a 7079 3a61 7474 723a 607e 4350  `, :py:attr:`~CP
+0000a9d0: 6172 616d 6574 6572 2e73 6561 7263 684c  arameter.searchL
+0000a9e0: 6f67 602c 203a 7079 3a61 7474 723a 607e  og`, :py:attr:`~
+0000a9f0: 4350 6172 616d 6574 6572 2e6d 696e 4d61  CParameter.minMa
+0000aa00: 7463 6860 2c20 3a70 793a 6174 7472 3a60  tch`, :py:attr:`
+0000aa10: 7e43 5061 7261 6d65 7465 722e 7461 7267  ~CParameter.targ
+0000aa20: 6574 4c65 6e67 7468 602c 203a 7079 3a61  etLength`, :py:a
+0000aa30: 7474 723a 607e 4350 6172 616d 6574 6572  ttr:`~CParameter
+0000aa40: 2e73 7472 6174 6567 7960 290a 2020 2020  .strategy`).    
+0000aa50: 2020 2020 2d20 4c6f 6e67 2064 6973 7461      - Long dista
+0000aa60: 6e63 6520 6d61 7463 6869 6e67 2028 3a70  nce matching (:p
+0000aa70: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
+0000aa80: 7465 722e 656e 6162 6c65 4c6f 6e67 4469  ter.enableLongDi
+0000aa90: 7374 616e 6365 4d61 7463 6869 6e67 602c  stanceMatching`,
+0000aaa0: 203a 7079 3a61 7474 723a 607e 4350 6172   :py:attr:`~CPar
+0000aab0: 616d 6574 6572 2e6c 646d 4861 7368 4c6f  ameter.ldmHashLo
+0000aac0: 6760 2c20 3a70 793a 6174 7472 3a60 7e43  g`, :py:attr:`~C
+0000aad0: 5061 7261 6d65 7465 722e 6c64 6d4d 696e  Parameter.ldmMin
+0000aae0: 4d61 7463 6860 2c20 3a70 793a 6174 7472  Match`, :py:attr
+0000aaf0: 3a60 7e43 5061 7261 6d65 7465 722e 6c64  :`~CParameter.ld
+0000ab00: 6d42 7563 6b65 7453 697a 654c 6f67 602c  mBucketSizeLog`,
+0000ab10: 203a 7079 3a61 7474 723a 607e 4350 6172   :py:attr:`~CPar
+0000ab20: 616d 6574 6572 2e6c 646d 4861 7368 5261  ameter.ldmHashRa
+0000ab30: 7465 4c6f 6760 290a 2020 2020 2020 2020  teLog`).        
+0000ab40: 2d20 4d69 7363 2028 3a70 793a 6174 7472  - Misc (:py:attr
+0000ab50: 3a60 7e43 5061 7261 6d65 7465 722e 636f  :`~CParameter.co
+0000ab60: 6e74 656e 7453 697a 6546 6c61 6760 2c20  ntentSizeFlag`, 
+0000ab70: 3a70 793a 6174 7472 3a60 7e43 5061 7261  :py:attr:`~CPara
+0000ab80: 6d65 7465 722e 6368 6563 6b73 756d 466c  meter.checksumFl
+0000ab90: 6167 602c 203a 7079 3a61 7474 723a 607e  ag`, :py:attr:`~
+0000aba0: 4350 6172 616d 6574 6572 2e64 6963 7449  CParameter.dictI
+0000abb0: 4446 6c61 6760 290a 2020 2020 2020 2020  DFlag`).        
+0000abc0: 2d20 4d75 6c74 692d 7468 7265 6164 6564  - Multi-threaded
+0000abd0: 2063 6f6d 7072 6573 7369 6f6e 2028 3a70   compression (:p
+0000abe0: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
+0000abf0: 7465 722e 6e62 576f 726b 6572 7360 2c20  ter.nbWorkers`, 
+0000ac00: 3a70 793a 6174 7472 3a60 7e43 5061 7261  :py:attr:`~CPara
+0000ac10: 6d65 7465 722e 6a6f 6253 697a 6560 2c20  meter.jobSize`, 
+0000ac20: 3a70 793a 6174 7472 3a60 7e43 5061 7261  :py:attr:`~CPara
+0000ac30: 6d65 7465 722e 6f76 6572 6c61 704c 6f67  meter.overlapLog
+0000ac40: 6029 0a0a 2020 2020 3a70 793a 636c 6173  `)..    :py:clas
+0000ac50: 733a 6044 5061 7261 6d65 7465 7260 2063  s:`DParameter` c
+0000ac60: 6c61 7373 2720 6174 7472 6962 7574 653a  lass' attribute:
+0000ac70: 0a0a 2020 2020 2020 2020 2d20 4465 636f  ..        - Deco
+0000ac80: 6d70 7265 7373 696f 6e20 7061 7261 6d65  mpression parame
+0000ac90: 7465 7220 283a 7079 3a61 7474 723a 607e  ter (:py:attr:`~
+0000aca0: 4450 6172 616d 6574 6572 2e77 696e 646f  DParameter.windo
+0000acb0: 774c 6f67 4d61 7860 290a 0a20 2020 203a  wLogMax`)..    :
+0000acc0: 7079 3a63 6c61 7373 3a60 5374 7261 7465  py:class:`Strate
+0000acd0: 6779 6020 636c 6173 7327 2061 7474 7269  gy` class' attri
+0000ace0: 6275 7465 733a 0a0a 2020 2020 2020 2020  butes:..        
+0000acf0: 3a70 793a 6174 7472 3a60 7e53 7472 6174  :py:attr:`~Strat
+0000ad00: 6567 792e 6661 7374 602c 203a 7079 3a61  egy.fast`, :py:a
+0000ad10: 7474 723a 607e 5374 7261 7465 6779 2e64  ttr:`~Strategy.d
+0000ad20: 6661 7374 602c 203a 7079 3a61 7474 723a  fast`, :py:attr:
+0000ad30: 607e 5374 7261 7465 6779 2e67 7265 6564  `~Strategy.greed
+0000ad40: 7960 2c20 3a70 793a 6174 7472 3a60 7e53  y`, :py:attr:`~S
+0000ad50: 7472 6174 6567 792e 6c61 7a79 602c 203a  trategy.lazy`, :
+0000ad60: 7079 3a61 7474 723a 607e 5374 7261 7465  py:attr:`~Strate
+0000ad70: 6779 2e6c 617a 7932 602c 203a 7079 3a61  gy.lazy2`, :py:a
+0000ad80: 7474 723a 607e 5374 7261 7465 6779 2e62  ttr:`~Strategy.b
+0000ad90: 746c 617a 7932 602c 203a 7079 3a61 7474  tlazy2`, :py:att
+0000ada0: 723a 607e 5374 7261 7465 6779 2e62 746f  r:`~Strategy.bto
+0000adb0: 7074 602c 203a 7079 3a61 7474 723a 607e  pt`, :py:attr:`~
+0000adc0: 5374 7261 7465 6779 2e62 7475 6c74 7261  Strategy.btultra
+0000add0: 602c 203a 7079 3a61 7474 723a 607e 5374  `, :py:attr:`~St
+0000ade0: 7261 7465 6779 2e62 7475 6c74 7261 3260  rategy.btultra2`
+0000adf0: 2e0a 0a2e 2e20 5f43 5061 7261 6d65 7465  ..... _CParamete
+0000ae00: 723a 0a0a 2e2e 2070 793a 636c 6173 733a  r:.... py:class:
+0000ae10: 3a20 4350 6172 616d 6574 6572 2849 6e74  : CParameter(Int
+0000ae20: 456e 756d 290a 0a20 2020 2041 6476 616e  Enum)..    Advan
+0000ae30: 6365 6420 636f 6d70 7265 7373 696f 6e20  ced compression 
+0000ae40: 7061 7261 6d65 7465 7273 2e0a 0a20 2020  parameters...   
+0000ae50: 2057 6865 6e20 7573 696e 672c 2070 7574   When using, put
+0000ae60: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
+0000ae70: 696e 2061 2060 6064 6963 7460 6020 6f62  in a ``dict`` ob
+0000ae80: 6a65 6374 2c20 7468 6520 6b65 7920 6973  ject, the key is
+0000ae90: 2061 203a 7079 3a63 6c61 7373 3a60 4350   a :py:class:`CP
+0000aea0: 6172 616d 6574 6572 6020 6e61 6d65 2c20  arameter` name, 
+0000aeb0: 7468 6520 7661 6c75 6520 6973 2061 2033  the value is a 3
+0000aec0: 322d 6269 7420 7369 676e 6564 2069 6e74  2-bit signed int
+0000aed0: 6567 6572 2076 616c 7565 2e0a 0a20 2020  eger value...   
+0000aee0: 202e 2e20 736f 7572 6365 636f 6465 3a3a   .. sourcecode::
+0000aef0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+0000af00: 206f 7074 696f 6e20 3d20 7b43 5061 7261   option = {CPara
+0000af10: 6d65 7465 722e 636f 6d70 7265 7373 696f  meter.compressio
+0000af20: 6e4c 6576 656c 203a 2031 302c 0a20 2020  nLevel : 10,.   
+0000af30: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+0000af40: 5061 7261 6d65 7465 722e 6368 6563 6b73  Parameter.checks
+0000af50: 756d 466c 6167 203a 2031 7d0a 0a20 2020  umFlag : 1}..   
+0000af60: 2020 2020 2023 2075 7365 6420 7769 7468       # used with
+0000af70: 2063 6f6d 7072 6573 7328 2920 6675 6e63   compress() func
+0000af80: 7469 6f6e 0a20 2020 2020 2020 2063 6f6d  tion.        com
+0000af90: 7072 6573 7365 645f 6461 7420 3d20 636f  pressed_dat = co
+0000afa0: 6d70 7265 7373 2872 6177 5f64 6174 2c20  mpress(raw_dat, 
+0000afb0: 6f70 7469 6f6e 290a 0a20 2020 2020 2020  option)..       
+0000afc0: 2023 2075 7365 6420 7769 7468 205a 7374   # used with Zst
+0000afd0: 6443 6f6d 7072 6573 736f 7220 6f62 6a65  dCompressor obje
+0000afe0: 6374 0a20 2020 2020 2020 2063 203d 205a  ct.        c = Z
+0000aff0: 7374 6443 6f6d 7072 6573 736f 7228 6c65  stdCompressor(le
+0000b000: 7665 6c5f 6f72 5f6f 7074 696f 6e3d 6f70  vel_or_option=op
+0000b010: 7469 6f6e 290a 2020 2020 2020 2020 636f  tion).        co
+0000b020: 6d70 7265 7373 6564 5f64 6174 3120 3d20  mpressed_dat1 = 
+0000b030: 632e 636f 6d70 7265 7373 2872 6177 5f64  c.compress(raw_d
+0000b040: 6174 290a 2020 2020 2020 2020 636f 6d70  at).        comp
+0000b050: 7265 7373 6564 5f64 6174 3220 3d20 632e  ressed_dat2 = c.
+0000b060: 666c 7573 6828 290a 0a20 2020 2050 6172  flush()..    Par
+0000b070: 616d 6574 6572 2076 616c 7565 2073 686f  ameter value sho
+0000b080: 756c 6420 6265 6c6f 6e67 2074 6f20 616e  uld belong to an
+0000b090: 2069 6e74 6572 7661 6c20 7769 7468 206c   interval with l
+0000b0a0: 6f77 6572 2061 6e64 2075 7070 6572 2062  ower and upper b
+0000b0b0: 6f75 6e64 732c 206f 7468 6572 7769 7365  ounds, otherwise
+0000b0c0: 2074 6865 7920 7769 6c6c 2065 6974 6865   they will eithe
+0000b0d0: 7220 7472 6967 6765 7220 616e 2065 7272  r trigger an err
+0000b0e0: 6f72 206f 7220 6265 2063 6c61 6d70 6564  or or be clamped
+0000b0f0: 2073 696c 656e 746c 792e 0a0a 2020 2020   silently...    
+0000b100: 5468 6520 636f 6e73 7461 6e74 2076 616c  The constant val
+0000b110: 7565 7320 6d65 6e74 696f 6e65 6420 6265  ues mentioned be
+0000b120: 6c6f 7720 6172 6520 6465 6669 6e65 6420  low are defined 
+0000b130: 696e 2060 7a73 7464 2e68 203c 6874 7470  in `zstd.h <http
+0000b140: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
+0000b150: 6163 6562 6f6f 6b2f 7a73 7464 2f62 6c6f  acebook/zstd/blo
+0000b160: 622f 7265 6c65 6173 652f 6c69 622f 7a73  b/release/lib/zs
+0000b170: 7464 2e68 3e60 5f2c 206e 6f74 6520 7468  td.h>`_, note th
+0000b180: 6174 2074 6865 7365 2076 616c 7565 7320  at these values 
+0000b190: 6d61 7920 6265 2064 6966 6665 7265 6e74  may be different
+0000b1a0: 2069 6e20 6469 6666 6572 656e 7420 7a73   in different zs
+0000b1b0: 7464 2076 6572 7369 6f6e 732e 0a0a 2020  td versions...  
+0000b1c0: 2020 2e2e 2070 793a 6d65 7468 6f64 3a3a    .. py:method::
+0000b1d0: 2062 6f75 6e64 7328 7365 6c66 290a 0a20   bounds(self).. 
+0000b1e0: 2020 2020 2020 2052 6574 7572 6e20 6c6f         Return lo
+0000b1f0: 7765 7220 616e 6420 7570 7065 7220 626f  wer and upper bo
+0000b200: 756e 6473 206f 6620 6120 7061 7261 6d65  unds of a parame
+0000b210: 7465 722c 2062 6f74 6820 696e 636c 7573  ter, both inclus
+0000b220: 6976 652e 0a0a 2020 2020 2020 2020 2e2e  ive...        ..
+0000b230: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
+0000b240: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
+0000b250: 2020 3e3e 3e20 4350 6172 616d 6574 6572    >>> CParameter
+0000b260: 2e63 6f6d 7072 6573 7369 6f6e 4c65 7665  .compressionLeve
+0000b270: 6c2e 626f 756e 6473 2829 0a20 2020 2020  l.bounds().     
+0000b280: 2020 2020 2020 2028 2d31 3331 3037 322c         (-131072,
+0000b290: 2032 3229 0a20 2020 2020 2020 2020 2020   22).           
+0000b2a0: 203e 3e3e 2043 5061 7261 6d65 7465 722e   >>> CParameter.
+0000b2b0: 7769 6e64 6f77 4c6f 672e 626f 756e 6473  windowLog.bounds
+0000b2c0: 2829 0a20 2020 2020 2020 2020 2020 2028  ().            (
+0000b2d0: 3130 2c20 3331 290a 2020 2020 2020 2020  10, 31).        
+0000b2e0: 2020 2020 3e3e 3e20 4350 6172 616d 6574      >>> CParamet
+0000b2f0: 6572 2e65 6e61 626c 654c 6f6e 6744 6973  er.enableLongDis
+0000b300: 7461 6e63 654d 6174 6368 696e 672e 626f  tanceMatching.bo
+0000b310: 756e 6473 2829 0a20 2020 2020 2020 2020  unds().         
+0000b320: 2020 2028 302c 2031 290a 0a20 2020 202e     (0, 1)..    .
+0000b330: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
+0000b340: 2063 6f6d 7072 6573 7369 6f6e 4c65 7665   compressionLeve
+0000b350: 6c0a 0a20 2020 2020 2020 2053 6574 2063  l..        Set c
+0000b360: 6f6d 7072 6573 7369 6f6e 2070 6172 616d  ompression param
+0000b370: 6574 6572 7320 6163 636f 7264 696e 6720  eters according 
+0000b380: 746f 2070 7265 2d64 6566 696e 6564 2063  to pre-defined c
+0000b390: 6f6d 7072 6573 7369 6f6e 4c65 7665 6c20  ompressionLevel 
+0000b3a0: 7461 626c 652c 2073 6565 203a 7265 663a  table, see :ref:
+0000b3b0: 6063 6f6d 7072 6573 7369 6f6e 206c 6576  `compression lev
+0000b3c0: 656c 3c63 6f6d 7072 6573 7369 6f6e 5f6c  el<compression_l
+0000b3d0: 6576 656c 3e60 2066 6f72 2064 6574 6169  evel>` for detai
+0000b3e0: 6c73 2e0a 0a20 2020 2020 2020 2053 6574  ls...        Set
+0000b3f0: 7469 6e67 2061 2063 6f6d 7072 6573 7369  ting a compressi
+0000b400: 6f6e 206c 6576 656c 2064 6f65 7320 6e6f  on level does no
+0000b410: 7420 7365 7420 616c 6c20 6f74 6865 7220  t set all other 
+0000b420: 636f 6d70 7265 7373 696f 6e20 7061 7261  compression para
+0000b430: 6d65 7465 7273 2074 6f20 6465 6661 756c  meters to defaul
+0000b440: 742e 2053 6574 7469 6e67 2074 6869 7320  t. Setting this 
+0000b450: 7769 6c6c 2064 796e 616d 6963 616c 6c79  will dynamically
+0000b460: 2069 6d70 6163 7420 7468 6520 636f 6d70   impact the comp
+0000b470: 7265 7373 696f 6e20 7061 7261 6d65 7465  ression paramete
+0000b480: 7273 2077 6869 6368 2068 6176 6520 6e6f  rs which have no
+0000b490: 7420 6265 656e 206d 616e 7561 6c6c 7920  t been manually 
+0000b4a0: 7365 742c 2074 6865 206d 616e 7561 6c6c  set, the manuall
+0000b4b0: 7920 7365 7420 6f6e 6573 2077 696c 6c20  y set ones will 
+0000b4c0: 2273 7469 636b 222e 0a0a 2020 2020 2e2e  "stick"...    ..
+0000b4d0: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
+0000b4e0: 7769 6e64 6f77 4c6f 670a 0a20 2020 2020  windowLog..     
+0000b4f0: 2020 204d 6178 696d 756d 2061 6c6c 6f77     Maximum allow
+0000b500: 6564 2062 6163 6b2d 7265 6665 7265 6e63  ed back-referenc
+0000b510: 6520 6469 7374 616e 6365 2c20 6578 7072  e distance, expr
+0000b520: 6573 7365 6420 6173 2070 6f77 6572 206f  essed as power o
+0000b530: 6620 322c 2060 6031 203c 3c20 7769 6e64  f 2, ``1 << wind
+0000b540: 6f77 4c6f 6760 6020 6279 7465 732e 0a0a  owLog`` bytes...
+0000b550: 2020 2020 2020 2020 4c61 7267 6572 2076          Larger v
+0000b560: 616c 7565 7320 7265 7175 6972 696e 6720  alues requiring 
+0000b570: 6d6f 7265 206d 656d 6f72 7920 616e 6420  more memory and 
+0000b580: 7479 7069 6361 6c6c 7920 636f 6d70 7265  typically compre
+0000b590: 7373 696e 6720 6d6f 7265 2e0a 0a20 2020  ssing more...   
+0000b5a0: 2020 2020 2054 6869 7320 7769 6c6c 2073       This will s
+0000b5b0: 6574 2061 206d 656d 6f72 7920 6275 6467  et a memory budg
+0000b5c0: 6574 2066 6f72 2073 7472 6561 6d69 6e67  et for streaming
+0000b5d0: 2064 6563 6f6d 7072 6573 7369 6f6e 2e20   decompression. 
+0000b5e0: 5573 696e 6720 6120 7661 6c75 6520 6772  Using a value gr
+0000b5f0: 6561 7465 7220 7468 616e 2060 605a 5354  eater than ``ZST
+0000b600: 445f 5749 4e44 4f57 4c4f 475f 4c49 4d49  D_WINDOWLOG_LIMI
+0000b610: 545f 4445 4641 554c 5460 6020 7265 7175  T_DEFAULT`` requ
+0000b620: 6972 6573 2065 7870 6c69 6369 746c 7920  ires explicitly 
+0000b630: 616c 6c6f 7769 6e67 2073 7563 6820 7369  allowing such si
+0000b640: 7a65 2061 7420 7374 7265 616d 696e 6720  ze at streaming 
+0000b650: 6465 636f 6d70 7265 7373 696f 6e20 7374  decompression st
+0000b660: 6167 652c 2073 6565 203a 7079 3a61 7474  age, see :py:att
+0000b670: 723a 6044 5061 7261 6d65 7465 722e 7769  r:`DParameter.wi
+0000b680: 6e64 6f77 4c6f 674d 6178 602e 2060 605a  ndowLogMax`. ``Z
+0000b690: 5354 445f 5749 4e44 4f57 4c4f 475f 4c49  STD_WINDOWLOG_LI
+0000b6a0: 4d49 545f 4445 4641 554c 5460 6020 6973  MIT_DEFAULT`` is
+0000b6b0: 2032 3720 696e 207a 7374 6420 7631 2e32   27 in zstd v1.2
+0000b6c0: 2b2c 206d 6561 6e73 2031 3238 204d 6942  +, means 128 MiB
+0000b6d0: 2028 3120 3c3c 2032 3729 2e0a 0a20 2020   (1 << 27)...   
+0000b6e0: 2020 2020 204d 7573 7420 6265 2063 6c61       Must be cla
+0000b6f0: 6d70 6564 2062 6574 7765 656e 2060 605a  mped between ``Z
+0000b700: 5354 445f 5749 4e44 4f57 4c4f 475f 4d49  STD_WINDOWLOG_MI
+0000b710: 4e60 6020 616e 6420 6060 5a53 5444 5f57  N`` and ``ZSTD_W
+0000b720: 494e 444f 574c 4f47 5f4d 4158 6060 2e0a  INDOWLOG_MAX``..
+0000b730: 0a20 2020 2020 2020 2053 7065 6369 616c  .        Special
+0000b740: 3a20 7661 6c75 6520 6060 3060 6020 6d65  : value ``0`` me
+0000b750: 616e 7320 2275 7365 2064 6566 6175 6c74  ans "use default
+0000b760: 2077 696e 646f 774c 6f67 222c 2074 6865   windowLog", the
+0000b770: 6e20 7468 6520 7661 6c75 6520 6973 2064  n the value is d
+0000b780: 796e 616d 6963 616c 6c79 2073 6574 2c20  ynamically set, 
+0000b790: 7365 6520 2257 2220 636f 6c75 6d6e 2069  see "W" column i
+0000b7a0: 6e20 6074 6869 7320 7461 626c 6520 3c68  n `this table <h
+0000b7b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000b7c0: 6d2f 6661 6365 626f 6f6b 2f7a 7374 642f  m/facebook/zstd/
+0000b7d0: 626c 6f62 2f72 656c 6561 7365 2f6c 6962  blob/release/lib
+0000b7e0: 2f63 6f6d 7072 6573 732f 636c 6576 656c  /compress/clevel
+0000b7f0: 732e 683e 605f 2e0a 0a20 2020 202e 2e20  s.h>`_...    .. 
+0000b800: 7079 3a61 7474 7269 6275 7465 3a3a 2068  py:attribute:: h
+0000b810: 6173 684c 6f67 0a0a 2020 2020 2020 2020  ashLog..        
+0000b820: 5369 7a65 206f 6620 7468 6520 696e 6974  Size of the init
+0000b830: 6961 6c20 7072 6f62 6520 7461 626c 652c  ial probe table,
+0000b840: 2061 7320 6120 706f 7765 7220 6f66 2032   as a power of 2
+0000b850: 2c20 7265 7375 6c74 696e 6720 6d65 6d6f  , resulting memo
+0000b860: 7279 2075 7361 6765 2069 7320 6060 3120  ry usage is ``1 
+0000b870: 3c3c 2028 6861 7368 4c6f 672b 3229 6060  << (hashLog+2)``
+0000b880: 2062 7974 6573 2e0a 0a20 2020 2020 2020   bytes...       
+0000b890: 204d 7573 7420 6265 2063 6c61 6d70 6564   Must be clamped
+0000b8a0: 2062 6574 7765 656e 2060 605a 5354 445f   between ``ZSTD_
+0000b8b0: 4841 5348 4c4f 475f 4d49 4e60 6020 616e  HASHLOG_MIN`` an
+0000b8c0: 6420 6060 5a53 5444 5f48 4153 484c 4f47  d ``ZSTD_HASHLOG
+0000b8d0: 5f4d 4158 6060 2e0a 0a20 2020 2020 2020  _MAX``...       
+0000b8e0: 204c 6172 6765 7220 7461 626c 6573 2069   Larger tables i
+0000b8f0: 6d70 726f 7665 2063 6f6d 7072 6573 7369  mprove compressi
+0000b900: 6f6e 2072 6174 696f 206f 6620 7374 7261  on ratio of stra
+0000b910: 7465 6769 6573 203c 3d20 3a70 793a 6174  tegies <= :py:at
+0000b920: 7472 3a60 7e53 7472 6174 6567 792e 6466  tr:`~Strategy.df
+0000b930: 6173 7460 2c20 616e 6420 696d 7072 6f76  ast`, and improv
+0000b940: 6520 7370 6565 6420 6f66 2073 7472 6174  e speed of strat
+0000b950: 6567 6965 7320 3e20 3a70 793a 6174 7472  egies > :py:attr
+0000b960: 3a60 7e53 7472 6174 6567 792e 6466 6173  :`~Strategy.dfas
+0000b970: 7460 2e0a 0a20 2020 2020 2020 2053 7065  t`...        Spe
+0000b980: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
+0000b990: 6020 6d65 616e 7320 2275 7365 2064 6566  ` means "use def
+0000b9a0: 6175 6c74 2068 6173 684c 6f67 222c 2074  ault hashLog", t
+0000b9b0: 6865 6e20 7468 6520 7661 6c75 6520 6973  hen the value is
+0000b9c0: 2064 796e 616d 6963 616c 6c79 2073 6574   dynamically set
+0000b9d0: 2c20 7365 6520 2248 2220 636f 6c75 6d6e  , see "H" column
+0000b9e0: 2069 6e20 6074 6869 7320 7461 626c 6520   in `this table 
+0000b9f0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+0000ba00: 636f 6d2f 6661 6365 626f 6f6b 2f7a 7374  com/facebook/zst
+0000ba10: 642f 626c 6f62 2f72 656c 6561 7365 2f6c  d/blob/release/l
+0000ba20: 6962 2f63 6f6d 7072 6573 732f 636c 6576  ib/compress/clev
+0000ba30: 656c 732e 683e 605f 2e0a 0a20 2020 202e  els.h>`_...    .
+0000ba40: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
+0000ba50: 2063 6861 696e 4c6f 670a 0a20 2020 2020   chainLog..     
+0000ba60: 2020 2053 697a 6520 6f66 2074 6865 206d     Size of the m
+0000ba70: 756c 7469 2d70 726f 6265 2073 6561 7263  ulti-probe searc
+0000ba80: 6820 7461 626c 652c 2061 7320 6120 706f  h table, as a po
+0000ba90: 7765 7220 6f66 2032 2c20 7265 7375 6c74  wer of 2, result
+0000baa0: 696e 6720 6d65 6d6f 7279 2075 7361 6765  ing memory usage
+0000bab0: 2069 7320 6060 3120 3c3c 2028 6368 6169   is ``1 << (chai
+0000bac0: 6e4c 6f67 2b32 2960 6020 6279 7465 732e  nLog+2)`` bytes.
+0000bad0: 0a0a 2020 2020 2020 2020 4d75 7374 2062  ..        Must b
+0000bae0: 6520 636c 616d 7065 6420 6265 7477 6565  e clamped betwee
+0000baf0: 6e20 6060 5a53 5444 5f43 4841 494e 4c4f  n ``ZSTD_CHAINLO
+0000bb00: 475f 4d49 4e60 6020 616e 6420 6060 5a53  G_MIN`` and ``ZS
+0000bb10: 5444 5f43 4841 494e 4c4f 475f 4d41 5860  TD_CHAINLOG_MAX`
+0000bb20: 602e 0a0a 2020 2020 2020 2020 4c61 7267  `...        Larg
+0000bb30: 6572 2074 6162 6c65 7320 7265 7375 6c74  er tables result
+0000bb40: 2069 6e20 6265 7474 6572 2061 6e64 2073   in better and s
+0000bb50: 6c6f 7765 7220 636f 6d70 7265 7373 696f  lower compressio
+0000bb60: 6e2e 0a0a 2020 2020 2020 2020 5468 6973  n...        This
+0000bb70: 2070 6172 616d 6574 6572 2069 7320 7573   parameter is us
+0000bb80: 656c 6573 7320 666f 7220 3a70 793a 6174  eless for :py:at
+0000bb90: 7472 3a60 7e53 7472 6174 6567 792e 6661  tr:`~Strategy.fa
+0000bba0: 7374 6020 7374 7261 7465 6779 2e0a 0a20  st` strategy... 
+0000bbb0: 2020 2020 2020 2049 7427 7320 7374 696c         It's stil
+0000bbc0: 6c20 7573 6566 756c 2077 6865 6e20 7573  l useful when us
+0000bbd0: 696e 6720 3a70 793a 6174 7472 3a60 7e53  ing :py:attr:`~S
+0000bbe0: 7472 6174 6567 792e 6466 6173 7460 2073  trategy.dfast` s
+0000bbf0: 7472 6174 6567 792c 2069 6e20 7768 6963  trategy, in whic
+0000bc00: 6820 6361 7365 2069 7420 6465 6669 6e65  h case it define
+0000bc10: 7320 6120 7365 636f 6e64 6172 7920 7072  s a secondary pr
+0000bc20: 6f62 6520 7461 626c 652e 0a0a 2020 2020  obe table...    
+0000bc30: 2020 2020 5370 6563 6961 6c3a 2076 616c      Special: val
+0000bc40: 7565 2060 6030 6060 206d 6561 6e73 2022  ue ``0`` means "
+0000bc50: 7573 6520 6465 6661 756c 7420 6368 6169  use default chai
+0000bc60: 6e4c 6f67 222c 2074 6865 6e20 7468 6520  nLog", then the 
+0000bc70: 7661 6c75 6520 6973 2064 796e 616d 6963  value is dynamic
+0000bc80: 616c 6c79 2073 6574 2c20 7365 6520 2243  ally set, see "C
+0000bc90: 2220 636f 6c75 6d6e 2069 6e20 6074 6869  " column in `thi
+0000bca0: 7320 7461 626c 6520 3c68 7474 7073 3a2f  s table <https:/
+0000bcb0: 2f67 6974 6875 622e 636f 6d2f 6661 6365  /github.com/face
+0000bcc0: 626f 6f6b 2f7a 7374 642f 626c 6f62 2f72  book/zstd/blob/r
+0000bcd0: 656c 6561 7365 2f6c 6962 2f63 6f6d 7072  elease/lib/compr
+0000bce0: 6573 732f 636c 6576 656c 732e 683e 605f  ess/clevels.h>`_
+0000bcf0: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
+0000bd00: 7269 6275 7465 3a3a 2073 6561 7263 684c  ribute:: searchL
+0000bd10: 6f67 0a0a 2020 2020 2020 2020 4e75 6d62  og..        Numb
+0000bd20: 6572 206f 6620 7365 6172 6368 2061 7474  er of search att
+0000bd30: 656d 7074 732c 2061 7320 6120 706f 7765  empts, as a powe
+0000bd40: 7220 6f66 2032 2e0a 0a20 2020 2020 2020  r of 2...       
+0000bd50: 204d 6f72 6520 6174 7465 6d70 7473 2072   More attempts r
+0000bd60: 6573 756c 7420 696e 2062 6574 7465 7220  esult in better 
+0000bd70: 616e 6420 736c 6f77 6572 2063 6f6d 7072  and slower compr
+0000bd80: 6573 7369 6f6e 2e0a 0a20 2020 2020 2020  ession...       
+0000bd90: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
+0000bda0: 6973 2075 7365 6c65 7373 2066 6f72 203a  is useless for :
+0000bdb0: 7079 3a61 7474 723a 607e 5374 7261 7465  py:attr:`~Strate
+0000bdc0: 6779 2e66 6173 7460 2061 6e64 203a 7079  gy.fast` and :py
+0000bdd0: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
+0000bde0: 2e64 6661 7374 6020 7374 7261 7465 6769  .dfast` strategi
+0000bdf0: 6573 2e0a 0a20 2020 2020 2020 2053 7065  es...        Spe
+0000be00: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
+0000be10: 6020 6d65 616e 7320 2275 7365 2064 6566  ` means "use def
+0000be20: 6175 6c74 2073 6561 7263 684c 6f67 222c  ault searchLog",
+0000be30: 2074 6865 6e20 7468 6520 7661 6c75 6520   then the value 
+0000be40: 6973 2064 796e 616d 6963 616c 6c79 2073  is dynamically s
+0000be50: 6574 2c20 7365 6520 2253 2220 636f 6c75  et, see "S" colu
+0000be60: 6d6e 2069 6e20 6074 6869 7320 7461 626c  mn in `this tabl
+0000be70: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
+0000be80: 622e 636f 6d2f 6661 6365 626f 6f6b 2f7a  b.com/facebook/z
+0000be90: 7374 642f 626c 6f62 2f72 656c 6561 7365  std/blob/release
+0000bea0: 2f6c 6962 2f63 6f6d 7072 6573 732f 636c  /lib/compress/cl
+0000beb0: 6576 656c 732e 683e 605f 2e0a 0a20 2020  evels.h>`_...   
+0000bec0: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+0000bed0: 3a3a 206d 696e 4d61 7463 680a 0a20 2020  :: minMatch..   
+0000bee0: 2020 2020 204d 696e 696d 756d 2073 697a       Minimum siz
+0000bef0: 6520 6f66 2073 6561 7263 6865 6420 6d61  e of searched ma
+0000bf00: 7463 6865 732e 0a0a 2020 2020 2020 2020  tches...        
+0000bf10: 4e6f 7465 2074 6861 7420 5a73 7461 6e64  Note that Zstand
+0000bf20: 6172 6420 6361 6e20 7374 696c 6c20 6669  ard can still fi
+0000bf30: 6e64 206d 6174 6368 6573 206f 6620 736d  nd matches of sm
+0000bf40: 616c 6c65 7220 7369 7a65 2c20 6974 206a  aller size, it j
+0000bf50: 7573 7420 7477 6561 6b73 2069 7473 2073  ust tweaks its s
+0000bf60: 6561 7263 6820 616c 676f 7269 7468 6d20  earch algorithm 
+0000bf70: 746f 206c 6f6f 6b20 666f 7220 7468 6973  to look for this
+0000bf80: 2073 697a 6520 616e 6420 6c61 7267 6572   size and larger
+0000bf90: 2e0a 0a20 2020 2020 2020 204c 6172 6765  ...        Large
+0000bfa0: 7220 7661 6c75 6573 2069 6e63 7265 6173  r values increas
+0000bfb0: 6520 636f 6d70 7265 7373 696f 6e20 616e  e compression an
+0000bfc0: 6420 6465 636f 6d70 7265 7373 696f 6e20  d decompression 
+0000bfd0: 7370 6565 642c 2062 7574 2064 6563 7265  speed, but decre
+0000bfe0: 6173 6520 7261 7469 6f2e 0a0a 2020 2020  ase ratio...    
+0000bff0: 2020 2020 4d75 7374 2062 6520 636c 616d      Must be clam
+0000c000: 7065 6420 6265 7477 6565 6e20 6060 5a53  ped between ``ZS
+0000c010: 5444 5f4d 494e 4d41 5443 485f 4d49 4e60  TD_MINMATCH_MIN`
+0000c020: 6020 616e 6420 6060 5a53 5444 5f4d 494e  ` and ``ZSTD_MIN
+0000c030: 4d41 5443 485f 4d41 5860 602e 0a0a 2020  MATCH_MAX``...  
+0000c040: 2020 2020 2020 4e6f 7465 2074 6861 7420        Note that 
+0000c050: 6375 7272 656e 746c 792c 2066 6f72 2061  currently, for a
+0000c060: 6c6c 2073 7472 6174 6567 6965 7320 3c20  ll strategies < 
+0000c070: 3a70 793a 6174 7472 3a60 7e53 7472 6174  :py:attr:`~Strat
+0000c080: 6567 792e 6274 6f70 7460 2c20 6566 6665  egy.btopt`, effe
+0000c090: 6374 6976 6520 6d69 6e69 6d75 6d20 6973  ctive minimum is
+0000c0a0: 2060 6034 6060 2c20 666f 7220 616c 6c20   ``4``, for all 
+0000c0b0: 7374 7261 7465 6769 6573 203e 203a 7079  strategies > :py
+0000c0c0: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
+0000c0d0: 2e66 6173 7460 2c20 6566 6665 6374 6976  .fast`, effectiv
+0000c0e0: 6520 6d61 7869 6d75 6d20 6973 2060 6036  e maximum is ``6
+0000c0f0: 6060 2e0a 0a20 2020 2020 2020 2053 7065  ``...        Spe
+0000c100: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
+0000c110: 6020 6d65 616e 7320 2275 7365 2064 6566  ` means "use def
+0000c120: 6175 6c74 206d 696e 4d61 7463 684c 656e  ault minMatchLen
+0000c130: 6774 6822 2c20 7468 656e 2074 6865 2076  gth", then the v
+0000c140: 616c 7565 2069 7320 6479 6e61 6d69 6361  alue is dynamica
+0000c150: 6c6c 7920 7365 742c 2073 6565 2022 4c22  lly set, see "L"
+0000c160: 2063 6f6c 756d 6e20 696e 2060 7468 6973   column in `this
+0000c170: 2074 6162 6c65 203c 6874 7470 733a 2f2f   table <https://
+0000c180: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
+0000c190: 6f6f 6b2f 7a73 7464 2f62 6c6f 622f 7265  ook/zstd/blob/re
+0000c1a0: 6c65 6173 652f 6c69 622f 636f 6d70 7265  lease/lib/compre
+0000c1b0: 7373 2f63 6c65 7665 6c73 2e68 3e60 5f2e  ss/clevels.h>`_.
+0000c1c0: 0a0a 2020 2020 2e2e 2070 793a 6174 7472  ..    .. py:attr
+0000c1d0: 6962 7574 653a 3a20 7461 7267 6574 4c65  ibute:: targetLe
+0000c1e0: 6e67 7468 0a0a 2020 2020 2020 2020 496d  ngth..        Im
+0000c1f0: 7061 6374 206f 6620 7468 6973 2066 6965  pact of this fie
+0000c200: 6c64 2064 6570 656e 6473 206f 6e20 7374  ld depends on st
+0000c210: 7261 7465 6779 2e0a 0a20 2020 2020 2020  rategy...       
+0000c220: 2046 6f72 2073 7472 6174 6567 6965 7320   For strategies 
+0000c230: 3a70 793a 6174 7472 3a60 7e53 7472 6174  :py:attr:`~Strat
+0000c240: 6567 792e 6274 6f70 7460 2c20 3a70 793a  egy.btopt`, :py:
+0000c250: 6174 7472 3a60 7e53 7472 6174 6567 792e  attr:`~Strategy.
+0000c260: 6274 756c 7472 6160 2026 203a 7079 3a61  btultra` & :py:a
+0000c270: 7474 723a 607e 5374 7261 7465 6779 2e62  ttr:`~Strategy.b
+0000c280: 7475 6c74 7261 3260 3a0a 0a20 2020 2020  tultra2`:..     
+0000c290: 2020 2020 2020 204c 656e 6774 6820 6f66         Length of
+0000c2a0: 204d 6174 6368 2063 6f6e 7369 6465 7265   Match considere
+0000c2b0: 6420 2267 6f6f 6420 656e 6f75 6768 2220  d "good enough" 
+0000c2c0: 746f 2073 746f 7020 7365 6172 6368 2e0a  to stop search..
+0000c2d0: 0a20 2020 2020 2020 2020 2020 204c 6172  .            Lar
+0000c2e0: 6765 7220 7661 6c75 6573 206d 616b 6520  ger values make 
+0000c2f0: 636f 6d70 7265 7373 696f 6e20 7374 726f  compression stro
+0000c300: 6e67 6572 2c20 616e 6420 736c 6f77 6572  nger, and slower
+0000c310: 2e0a 0a20 2020 2020 2020 2046 6f72 2073  ...        For s
+0000c320: 7472 6174 6567 7920 3a70 793a 6174 7472  trategy :py:attr
+0000c330: 3a60 7e53 7472 6174 6567 792e 6661 7374  :`~Strategy.fast
+0000c340: 603a 0a0a 2020 2020 2020 2020 2020 2020  `:..            
+0000c350: 4469 7374 616e 6365 2062 6574 7765 656e  Distance between
+0000c360: 206d 6174 6368 2073 616d 706c 696e 672e   match sampling.
+0000c370: 0a0a 2020 2020 2020 2020 2020 2020 4c61  ..            La
+0000c380: 7267 6572 2076 616c 7565 7320 6d61 6b65  rger values make
+0000c390: 2063 6f6d 7072 6573 7369 6f6e 2066 6173   compression fas
+0000c3a0: 7465 722c 2061 6e64 2077 6561 6b65 722e  ter, and weaker.
+0000c3b0: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
+0000c3c0: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
+0000c3d0: 6561 6e73 2022 7573 6520 6465 6661 756c  eans "use defaul
+0000c3e0: 7420 7461 7267 6574 4c65 6e67 7468 222c  t targetLength",
+0000c3f0: 2074 6865 6e20 7468 6520 7661 6c75 6520   then the value 
+0000c400: 6973 2064 796e 616d 6963 616c 6c79 2073  is dynamically s
+0000c410: 6574 2c20 7365 6520 2254 4c22 2063 6f6c  et, see "TL" col
+0000c420: 756d 6e20 696e 2060 7468 6973 2074 6162  umn in `this tab
+0000c430: 6c65 203c 6874 7470 733a 2f2f 6769 7468  le <https://gith
+0000c440: 7562 2e63 6f6d 2f66 6163 6562 6f6f 6b2f  ub.com/facebook/
+0000c450: 7a73 7464 2f62 6c6f 622f 7265 6c65 6173  zstd/blob/releas
+0000c460: 652f 6c69 622f 636f 6d70 7265 7373 2f63  e/lib/compress/c
+0000c470: 6c65 7665 6c73 2e68 3e60 5f2e 0a0a 2020  levels.h>`_...  
+0000c480: 2020 2e2e 2070 793a 6174 7472 6962 7574    .. py:attribut
+0000c490: 653a 3a20 7374 7261 7465 6779 0a0a 2020  e:: strategy..  
+0000c4a0: 2020 2020 2020 5365 6520 3a70 793a 6174        See :py:at
+0000c4b0: 7472 3a60 5374 7261 7465 6779 6020 636c  tr:`Strategy` cl
+0000c4c0: 6173 7320 6465 6669 6e69 7469 6f6e 2e0a  ass definition..
+0000c4d0: 0a20 2020 2020 2020 2054 6865 2068 6967  .        The hig
+0000c4e0: 6865 7220 7468 6520 7661 6c75 6520 6f66  her the value of
+0000c4f0: 2073 656c 6563 7465 6420 7374 7261 7465   selected strate
+0000c500: 6779 2c20 7468 6520 6d6f 7265 2063 6f6d  gy, the more com
+0000c510: 706c 6578 2069 7420 6973 2c20 7265 7375  plex it is, resu
+0000c520: 6c74 696e 6720 696e 2073 7472 6f6e 6765  lting in stronge
+0000c530: 7220 616e 6420 736c 6f77 6572 2063 6f6d  r and slower com
+0000c540: 7072 6573 7369 6f6e 2e0a 0a20 2020 2020  pression...     
+0000c550: 2020 2053 7065 6369 616c 3a20 7661 6c75     Special: valu
+0000c560: 6520 6060 3060 6020 6d65 616e 7320 2275  e ``0`` means "u
+0000c570: 7365 2064 6566 6175 6c74 2073 7472 6174  se default strat
+0000c580: 6567 7922 2c20 7468 656e 2074 6865 2076  egy", then the v
+0000c590: 616c 7565 2069 7320 6479 6e61 6d69 6361  alue is dynamica
+0000c5a0: 6c6c 7920 7365 742c 2073 6565 2022 7374  lly set, see "st
+0000c5b0: 7261 7422 2063 6f6c 756d 6e20 696e 2060  rat" column in `
+0000c5c0: 7468 6973 2074 6162 6c65 203c 6874 7470  this table <http
+0000c5d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
+0000c5e0: 6163 6562 6f6f 6b2f 7a73 7464 2f62 6c6f  acebook/zstd/blo
+0000c5f0: 622f 7265 6c65 6173 652f 6c69 622f 636f  b/release/lib/co
+0000c600: 6d70 7265 7373 2f63 6c65 7665 6c73 2e68  mpress/clevels.h
+0000c610: 3e60 5f2e 0a0a 2020 2020 2e2e 2070 793a  >`_...    .. py:
+0000c620: 6174 7472 6962 7574 653a 3a20 656e 6162  attribute:: enab
+0000c630: 6c65 4c6f 6e67 4469 7374 616e 6365 4d61  leLongDistanceMa
+0000c640: 7463 6869 6e67 0a0a 2020 2020 2020 2020  tching..        
+0000c650: 456e 6162 6c65 206c 6f6e 6720 6469 7374  Enable long dist
+0000c660: 616e 6365 206d 6174 6368 696e 672e 0a0a  ance matching...
+0000c670: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
+0000c680: 7661 6c75 6520 6973 2060 6030 6060 2c20  value is ``0``, 
+0000c690: 6361 6e20 6265 2060 6031 6060 2e0a 0a20  can be ``1``... 
+0000c6a0: 2020 2020 2020 2054 6869 7320 7061 7261         This para
+0000c6b0: 6d65 7465 7220 6973 2064 6573 6967 6e65  meter is designe
+0000c6c0: 6420 746f 2069 6d70 726f 7665 2063 6f6d  d to improve com
+0000c6d0: 7072 6573 7369 6f6e 2072 6174 696f 2c20  pression ratio, 
+0000c6e0: 666f 7220 6c61 7267 6520 696e 7075 7473  for large inputs
+0000c6f0: 2c20 6279 2066 696e 6469 6e67 206c 6172  , by finding lar
+0000c700: 6765 206d 6174 6368 6573 2061 7420 6c6f  ge matches at lo
+0000c710: 6e67 2064 6973 7461 6e63 652e 2049 7420  ng distance. It 
+0000c720: 696e 6372 6561 7365 7320 6d65 6d6f 7279  increases memory
+0000c730: 2075 7361 6765 2061 6e64 2077 696e 646f   usage and windo
+0000c740: 7720 7369 7a65 2e0a 0a20 2020 2020 2020  w size...       
+0000c750: 204e 6f74 653a 0a20 2020 2020 2020 2020   Note:.         
+0000c760: 2020 202a 2045 6e61 626c 696e 6720 7468     * Enabling th
+0000c770: 6973 2070 6172 616d 6574 6572 2069 6e63  is parameter inc
+0000c780: 7265 6173 6573 2064 6566 6175 6c74 203a  reases default :
+0000c790: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
+0000c7a0: 6574 6572 2e77 696e 646f 774c 6f67 6020  eter.windowLog` 
+0000c7b0: 746f 2031 3238 204d 6942 2065 7863 6570  to 128 MiB excep
+0000c7c0: 7420 7768 656e 2065 7870 7265 7373 6c79  t when expressly
+0000c7d0: 2073 6574 2074 6f20 6120 6469 6666 6572   set to a differ
+0000c7e0: 656e 7420 7661 6c75 652e 0a20 2020 2020  ent value..     
+0000c7f0: 2020 2020 2020 202a 2054 6869 7320 7769         * This wi
+0000c800: 6c6c 2062 6520 656e 6162 6c65 6420 6279  ll be enabled by
+0000c810: 2064 6566 6175 6c74 2069 6620 3a70 793a   default if :py:
+0000c820: 6174 7472 3a60 7e43 5061 7261 6d65 7465  attr:`~CParamete
+0000c830: 722e 7769 6e64 6f77 4c6f 6760 203e 3d20  r.windowLog` >= 
+0000c840: 3132 3820 4d69 4220 616e 6420 636f 6d70  128 MiB and comp
+0000c850: 7265 7373 696f 6e20 7374 7261 7465 6779  ression strategy
+0000c860: 203e 3d20 3a70 793a 6174 7472 3a60 7e53   >= :py:attr:`~S
+0000c870: 7472 6174 6567 792e 6274 6f70 7460 2028  trategy.btopt` (
+0000c880: 636f 6d70 7265 7373 696f 6e20 6c65 7665  compression leve
+0000c890: 6c20 3136 2b29 2e0a 0a20 2020 202e 2e20  l 16+)...    .. 
+0000c8a0: 7079 3a61 7474 7269 6275 7465 3a3a 206c  py:attribute:: l
+0000c8b0: 646d 4861 7368 4c6f 670a 0a20 2020 2020  dmHashLog..     
+0000c8c0: 2020 2053 697a 6520 6f66 2074 6865 2074     Size of the t
+0000c8d0: 6162 6c65 2066 6f72 206c 6f6e 6720 6469  able for long di
+0000c8e0: 7374 616e 6365 206d 6174 6368 696e 672c  stance matching,
+0000c8f0: 2061 7320 6120 706f 7765 7220 6f66 2032   as a power of 2
+0000c900: 2e0a 0a20 2020 2020 2020 204c 6172 6765  ...        Large
+0000c910: 7220 7661 6c75 6573 2069 6e63 7265 6173  r values increas
+0000c920: 6520 6d65 6d6f 7279 2075 7361 6765 2061  e memory usage a
+0000c930: 6e64 2063 6f6d 7072 6573 7369 6f6e 2072  nd compression r
+0000c940: 6174 696f 2c20 6275 7420 6465 6372 6561  atio, but decrea
+0000c950: 7365 2063 6f6d 7072 6573 7369 6f6e 2073  se compression s
+0000c960: 7065 6564 2e0a 0a20 2020 2020 2020 204d  peed...        M
+0000c970: 7573 7420 6265 2063 6c61 6d70 6564 2062  ust be clamped b
+0000c980: 6574 7765 656e 2060 605a 5354 445f 4841  etween ``ZSTD_HA
+0000c990: 5348 4c4f 475f 4d49 4e60 6020 616e 6420  SHLOG_MIN`` and 
+0000c9a0: 6060 5a53 5444 5f48 4153 484c 4f47 5f4d  ``ZSTD_HASHLOG_M
+0000c9b0: 4158 6060 2c20 6465 6661 756c 743a 203a  AX``, default: :
+0000c9c0: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
+0000c9d0: 6574 6572 2e77 696e 646f 774c 6f67 6020  eter.windowLog` 
+0000c9e0: 2d20 372e 0a0a 2020 2020 2020 2020 5370  - 7...        Sp
+0000c9f0: 6563 6961 6c3a 2076 616c 7565 2060 6030  ecial: value ``0
+0000ca00: 6060 206d 6561 6e73 2022 6175 746f 6d61  `` means "automa
+0000ca10: 7469 6361 6c6c 7920 6465 7465 726d 696e  tically determin
+0000ca20: 6520 6861 7368 6c6f 6722 2e0a 0a20 2020  e hashlog"...   
+0000ca30: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+0000ca40: 3a3a 206c 646d 4d69 6e4d 6174 6368 0a0a  :: ldmMinMatch..
+0000ca50: 2020 2020 2020 2020 4d69 6e69 6d75 6d20          Minimum 
+0000ca60: 6d61 7463 6820 7369 7a65 2066 6f72 206c  match size for l
+0000ca70: 6f6e 6720 6469 7374 616e 6365 206d 6174  ong distance mat
+0000ca80: 6368 6572 2e0a 0a20 2020 2020 2020 204c  cher...        L
+0000ca90: 6172 6765 722f 746f 6f20 736d 616c 6c20  arger/too small 
+0000caa0: 7661 6c75 6573 2075 7375 616c 6c79 2064  values usually d
+0000cab0: 6563 7265 6173 6520 636f 6d70 7265 7373  ecrease compress
+0000cac0: 696f 6e20 7261 7469 6f2e 0a0a 2020 2020  ion ratio...    
+0000cad0: 2020 2020 4d75 7374 2062 6520 636c 616d      Must be clam
+0000cae0: 7065 6420 6265 7477 6565 6e20 6060 5a53  ped between ``ZS
+0000caf0: 5444 5f4c 444d 5f4d 494e 4d41 5443 485f  TD_LDM_MINMATCH_
+0000cb00: 4d49 4e60 6020 616e 6420 6060 5a53 5444  MIN`` and ``ZSTD
+0000cb10: 5f4c 444d 5f4d 494e 4d41 5443 485f 4d41  _LDM_MINMATCH_MA
+0000cb20: 5860 602e 0a0a 2020 2020 2020 2020 5370  X``...        Sp
+0000cb30: 6563 6961 6c3a 2076 616c 7565 2060 6030  ecial: value ``0
+0000cb40: 6060 206d 6561 6e73 2022 7573 6520 6465  `` means "use de
+0000cb50: 6661 756c 7420 7661 6c75 6522 2028 6465  fault value" (de
+0000cb60: 6661 756c 743a 2036 3429 2e0a 0a20 2020  fault: 64)...   
+0000cb70: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+0000cb80: 3a3a 206c 646d 4275 636b 6574 5369 7a65  :: ldmBucketSize
+0000cb90: 4c6f 670a 0a20 2020 2020 2020 204c 6f67  Log..        Log
+0000cba0: 2073 697a 6520 6f66 2065 6163 6820 6275   size of each bu
+0000cbb0: 636b 6574 2069 6e20 7468 6520 4c44 4d20  cket in the LDM 
+0000cbc0: 6861 7368 2074 6162 6c65 2066 6f72 2063  hash table for c
+0000cbd0: 6f6c 6c69 7369 6f6e 2072 6573 6f6c 7574  ollision resolut
+0000cbe0: 696f 6e2e 0a0a 2020 2020 2020 2020 4c61  ion...        La
+0000cbf0: 7267 6572 2076 616c 7565 7320 696d 7072  rger values impr
+0000cc00: 6f76 6520 636f 6c6c 6973 696f 6e20 7265  ove collision re
+0000cc10: 736f 6c75 7469 6f6e 2062 7574 2064 6563  solution but dec
+0000cc20: 7265 6173 6520 636f 6d70 7265 7373 696f  rease compressio
+0000cc30: 6e20 7370 6565 642e 0a0a 2020 2020 2020  n speed...      
+0000cc40: 2020 5468 6520 6d61 7869 6d75 6d20 7661    The maximum va
+0000cc50: 6c75 6520 6973 2060 605a 5354 445f 4c44  lue is ``ZSTD_LD
+0000cc60: 4d5f 4255 434b 4554 5349 5a45 4c4f 475f  M_BUCKETSIZELOG_
+0000cc70: 4d41 5860 602e 0a0a 2020 2020 2020 2020  MAX``...        
+0000cc80: 5370 6563 6961 6c3a 2076 616c 7565 2060  Special: value `
+0000cc90: 6030 6060 206d 6561 6e73 2022 7573 6520  `0`` means "use 
+0000cca0: 6465 6661 756c 7420 7661 6c75 6522 2028  default value" (
+0000ccb0: 6465 6661 756c 743a 2033 292e 0a0a 2020  default: 3)...  
+0000ccc0: 2020 2e2e 2070 793a 6174 7472 6962 7574    .. py:attribut
+0000ccd0: 653a 3a20 6c64 6d48 6173 6852 6174 654c  e:: ldmHashRateL
+0000cce0: 6f67 0a0a 2020 2020 2020 2020 4672 6571  og..        Freq
+0000ccf0: 7565 6e63 7920 6f66 2069 6e73 6572 7469  uency of inserti
+0000cd00: 6e67 2f6c 6f6f 6b69 6e67 2075 7020 656e  ng/looking up en
+0000cd10: 7472 6965 7320 696e 746f 2074 6865 204c  tries into the L
+0000cd20: 444d 2068 6173 6820 7461 626c 652e 0a0a  DM hash table...
+0000cd30: 2020 2020 2020 2020 4d75 7374 2062 6520          Must be 
+0000cd40: 636c 616d 7065 6420 6265 7477 6565 6e20  clamped between 
+0000cd50: 3020 616e 6420 6060 285a 5354 445f 5749  0 and ``(ZSTD_WI
+0000cd60: 4e44 4f57 4c4f 475f 4d41 5820 2d20 5a53  NDOWLOG_MAX - ZS
+0000cd70: 5444 5f48 4153 484c 4f47 5f4d 494e 2960  TD_HASHLOG_MIN)`
+0000cd80: 602e 0a0a 2020 2020 2020 2020 4465 6661  `...        Defa
+0000cd90: 756c 7420 6973 204d 4158 2830 2c20 283a  ult is MAX(0, (:
+0000cda0: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
+0000cdb0: 6574 6572 2e77 696e 646f 774c 6f67 6020  eter.windowLog` 
+0000cdc0: 2d20 3a70 793a 6174 7472 3a60 7e43 5061  - :py:attr:`~CPa
+0000cdd0: 7261 6d65 7465 722e 6c64 6d48 6173 684c  rameter.ldmHashL
+0000cde0: 6f67 6029 292c 206f 7074 696d 697a 696e  og`)), optimizin
+0000cdf0: 6720 6861 7368 2074 6162 6c65 2075 7361  g hash table usa
+0000ce00: 6765 2e0a 0a20 2020 2020 2020 204c 6172  ge...        Lar
+0000ce10: 6765 7220 7661 6c75 6573 2069 6d70 726f  ger values impro
+0000ce20: 7665 2063 6f6d 7072 6573 7369 6f6e 2073  ve compression s
+0000ce30: 7065 6564 2e0a 0a20 2020 2020 2020 2044  peed...        D
+0000ce40: 6576 6961 7469 6e67 2066 6172 2066 726f  eviating far fro
+0000ce50: 6d20 6465 6661 756c 7420 7661 6c75 6520  m default value 
+0000ce60: 7769 6c6c 206c 696b 656c 7920 7265 7375  will likely resu
+0000ce70: 6c74 2069 6e20 6120 636f 6d70 7265 7373  lt in a compress
+0000ce80: 696f 6e20 7261 7469 6f20 6465 6372 6561  ion ratio decrea
+0000ce90: 7365 2e0a 0a20 2020 2020 2020 2053 7065  se...        Spe
+0000cea0: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
+0000ceb0: 6020 6d65 616e 7320 2261 7574 6f6d 6174  ` means "automat
+0000cec0: 6963 616c 6c79 2064 6574 6572 6d69 6e65  ically determine
+0000ced0: 2068 6173 6852 6174 654c 6f67 222e 0a0a   hashRateLog"...
+0000cee0: 2020 2020 2e2e 205f 636f 6e74 656e 745f      .. _content_
+0000cef0: 7369 7a65 3a0a 0a20 2020 202e 2e20 7079  size:..    .. py
+0000cf00: 3a61 7474 7269 6275 7465 3a3a 2063 6f6e  :attribute:: con
+0000cf10: 7465 6e74 5369 7a65 466c 6167 0a0a 2020  tentSizeFlag..  
+0000cf20: 2020 2020 2020 556e 636f 6d70 7265 7373        Uncompress
+0000cf30: 6564 2063 6f6e 7465 6e74 2073 697a 6520  ed content size 
+0000cf40: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
+0000cf50: 696e 746f 2066 7261 6d65 2068 6561 6465  into frame heade
+0000cf60: 7220 7768 656e 6576 6572 206b 6e6f 776e  r whenever known
+0000cf70: 2e0a 0a20 2020 2020 2020 2044 6566 6175  ...        Defau
+0000cf80: 6c74 2076 616c 7565 2069 7320 6060 3160  lt value is ``1`
+0000cf90: 602c 2063 616e 2062 6520 6060 3060 602e  `, can be ``0``.
+0000cfa0: 0a0a 2020 2020 2020 2020 496e 2074 7261  ..        In tra
+0000cfb0: 6469 7469 6f6e 616c 2073 7472 6561 6d69  ditional streami
+0000cfc0: 6e67 2063 6f6d 7072 6573 7369 6f6e 2c20  ng compression, 
+0000cfd0: 636f 6e74 656e 7420 7369 7a65 2069 7320  content size is 
+0000cfe0: 756e 6b6e 6f77 6e2e 0a0a 2020 2020 2020  unknown...      
+0000cff0: 2020 496e 2074 6865 7365 2063 6f6d 7072    In these compr
+0000d000: 6573 7369 6f6e 732c 2074 6865 2063 6f6e  essions, the con
+0000d010: 7465 6e74 2073 697a 6520 6973 206b 6e6f  tent size is kno
+0000d020: 776e 3a0a 0a20 2020 2020 2020 2020 2020  wn:..           
+0000d030: 202a 203a 7079 3a66 756e 633a 6063 6f6d   * :py:func:`com
+0000d040: 7072 6573 7360 2066 756e 6374 696f 6e0a  press` function.
+0000d050: 2020 2020 2020 2020 2020 2020 2a20 3a70              * :p
+0000d060: 793a 6675 6e63 3a60 7269 6368 6d65 6d5f  y:func:`richmem_
+0000d070: 636f 6d70 7265 7373 6020 6675 6e63 7469  compress` functi
+0000d080: 6f6e 0a20 2020 2020 2020 2020 2020 202a  on.            *
+0000d090: 203a 7079 3a63 6c61 7373 3a60 5a73 7464   :py:class:`Zstd
+0000d0a0: 436f 6d70 7265 7373 6f72 6020 636c 6173  Compressor` clas
+0000d0b0: 7320 7573 696e 6720 6120 7369 6e67 6c65  s using a single
+0000d0c0: 203a 7079 3a61 7474 723a 607e 5a73 7464   :py:attr:`~Zstd
+0000d0d0: 436f 6d70 7265 7373 6f72 2e46 4c55 5348  Compressor.FLUSH
+0000d0e0: 5f46 5241 4d45 6020 6d6f 6465 0a20 2020  _FRAME` mode.   
+0000d0f0: 2020 2020 2020 2020 202a 203a 7079 3a63           * :py:c
+0000d100: 6c61 7373 3a60 5269 6368 4d65 6d5a 7374  lass:`RichMemZst
+0000d110: 6443 6f6d 7072 6573 736f 7260 2063 6c61  dCompressor` cla
+0000d120: 7373 0a20 2020 2020 2020 2020 2020 202a  ss.            *
+0000d130: 203a 7079 3a66 756e 633a 6063 6f6d 7072   :py:func:`compr
+0000d140: 6573 735f 7374 7265 616d 6020 6675 6e63  ess_stream` func
+0000d150: 7469 6f6e 2073 6574 7469 6e67 202a 706c  tion setting *pl
+0000d160: 6564 6765 645f 696e 7075 745f 7369 7a65  edged_input_size
+0000d170: 2a20 7061 7261 6d65 7465 720a 0a20 2020  * parameter..   
+0000d180: 2020 2020 2054 6865 2066 6965 6c64 2069       The field i
+0000d190: 6e20 6672 616d 6520 6865 6164 6572 2069  n frame header i
+0000d1a0: 7320 312f 322f 342f 3820 6279 7465 732c  s 1/2/4/8 bytes,
+0000d1b0: 2064 6570 656e 6469 6e67 206f 6e20 7369   depending on si
+0000d1c0: 7a65 2076 616c 7565 2e20 4974 206d 6179  ze value. It may
+0000d1d0: 2068 656c 7020 6465 636f 6d70 7265 7373   help decompress
+0000d1e0: 696f 6e20 636f 6465 2074 6f20 616c 6c6f  ion code to allo
+0000d1f0: 6361 7465 206f 7574 7075 7420 6275 6666  cate output buff
+0000d200: 6572 2066 6173 7465 722e 0a0a 2020 2020  er faster...    
+0000d210: 2020 2020 5c2a 203a 7079 3a63 6c61 7373      \* :py:class
+0000d220: 3a60 5a73 7464 436f 6d70 7265 7373 6f72  :`ZstdCompressor
+0000d230: 6020 6861 7320 616e 2075 6e64 6f63 756d  ` has an undocum
+0000d240: 656e 7465 6420 6d65 7468 6f64 2074 6f20  ented method to 
+0000d250: 7365 7420 7468 6520 7369 7a65 2c20 6060  set the size, ``
+0000d260: 6865 6c70 285a 7374 6443 6f6d 7072 6573  help(ZstdCompres
+0000d270: 736f 722e 5f73 6574 5f70 6c65 6467 6564  sor._set_pledged
+0000d280: 5f69 6e70 7574 5f73 697a 6529 6060 2074  _input_size)`` t
+0000d290: 6f20 7365 6520 7468 6520 7573 6167 652e  o see the usage.
+0000d2a0: 0a0a 2020 2020 2e2e 2070 793a 6174 7472  ..    .. py:attr
+0000d2b0: 6962 7574 653a 3a20 6368 6563 6b73 756d  ibute:: checksum
+0000d2c0: 466c 6167 0a0a 2020 2020 2020 2020 4120  Flag..        A 
+0000d2d0: 342d 6279 7465 2063 6865 636b 7375 6d20  4-byte checksum 
+0000d2e0: 6f66 2075 6e63 6f6d 7072 6573 7365 6420  of uncompressed 
+0000d2f0: 636f 6e74 656e 7420 6973 2077 7269 7474  content is writt
+0000d300: 656e 2061 7420 7468 6520 656e 6420 6f66  en at the end of
+0000d310: 2066 7261 6d65 2e0a 0a20 2020 2020 2020   frame...       
+0000d320: 2044 6566 6175 6c74 2076 616c 7565 2069   Default value i
+0000d330: 7320 6060 3060 602c 2063 616e 2062 6520  s ``0``, can be 
+0000d340: 6060 3160 602e 0a0a 2020 2020 2020 2020  ``1``...        
+0000d350: 5a73 7464 2773 2064 6563 6f6d 7072 6573  Zstd's decompres
+0000d360: 7369 6f6e 2063 6f64 6520 7665 7269 6669  sion code verifi
+0000d370: 6573 2069 742e 2049 6620 6368 6563 6b73  es it. If checks
+0000d380: 756d 206d 6973 6d61 7463 682c 2072 6169  um mismatch, rai
+0000d390: 7365 7320 6120 3a70 793a 636c 6173 733a  ses a :py:class:
+0000d3a0: 605a 7374 6445 7272 6f72 6020 6578 6365  `ZstdError` exce
+0000d3b0: 7074 696f 6e2c 2077 6974 6820 6120 6d65  ption, with a me
+0000d3c0: 7373 6167 6520 6c69 6b65 2022 5265 7374  ssage like "Rest
+0000d3d0: 6f72 6564 2064 6174 6120 646f 6573 6e27  ored data doesn'
+0000d3e0: 7420 6d61 7463 6820 6368 6563 6b73 756d  t match checksum
+0000d3f0: 222e 0a0a 2020 2020 2e2e 2070 793a 6174  "...    .. py:at
+0000d400: 7472 6962 7574 653a 3a20 6469 6374 4944  tribute:: dictID
+0000d410: 466c 6167 0a0a 2020 2020 2020 2020 5768  Flag..        Wh
+0000d420: 656e 2061 7070 6c69 6361 626c 652c 2064  en applicable, d
+0000d430: 6963 7469 6f6e 6172 7927 7320 4944 2069  ictionary's ID i
+0000d440: 7320 7772 6974 7465 6e20 696e 746f 2066  s written into f
+0000d450: 7261 6d65 2068 6561 6465 722e 2053 6565  rame header. See
+0000d460: 203a 7265 663a 6074 6869 7320 6e6f 7465   :ref:`this note
+0000d470: 3c64 6963 745f 6964 3e60 2066 6f72 2064  <dict_id>` for d
+0000d480: 6574 6169 6c73 2e0a 0a20 2020 2020 2020  etails...       
+0000d490: 2044 6566 6175 6c74 2076 616c 7565 2069   Default value i
+0000d4a0: 7320 6060 3160 602c 2063 616e 2062 6520  s ``1``, can be 
+0000d4b0: 6060 3060 602e 0a0a 2020 2020 2e2e 2070  ``0``...    .. p
+0000d4c0: 793a 6174 7472 6962 7574 653a 3a20 6e62  y:attribute:: nb
+0000d4d0: 576f 726b 6572 730a 0a20 2020 2020 2020  Workers..       
+0000d4e0: 2053 656c 6563 7420 686f 7720 6d61 6e79   Select how many
+0000d4f0: 2074 6872 6561 6473 2077 696c 6c20 6265   threads will be
+0000d500: 2073 7061 776e 6564 2074 6f20 636f 6d70   spawned to comp
+0000d510: 7265 7373 2069 6e20 7061 7261 6c6c 656c  ress in parallel
+0000d520: 2e0a 0a20 2020 2020 2020 2057 6865 6e20  ...        When 
+0000d530: 6e62 576f 726b 6572 7320 3e3d 2060 6031  nbWorkers >= ``1
+0000d540: 6060 2c20 656e 6162 6c65 7320 6d75 6c74  ``, enables mult
+0000d550: 692d 7468 7265 6164 6564 2063 6f6d 7072  i-threaded compr
+0000d560: 6573 7369 6f6e 2c20 6060 3160 6020 6d65  ession, ``1`` me
+0000d570: 616e 7320 2231 2d74 6872 6561 6420 6d75  ans "1-thread mu
+0000d580: 6c74 692d 7468 7265 6164 6564 206d 6f64  lti-threaded mod
+0000d590: 6522 2e20 5365 6520 3a72 6566 3a60 7a73  e". See :ref:`zs
+0000d5a0: 7464 206d 756c 7469 2d74 6872 6561 6465  td multi-threade
+0000d5b0: 6420 636f 6d70 7265 7373 696f 6e3c 6d74  d compression<mt
+0000d5c0: 5f63 6f6d 7072 6573 7369 6f6e 3e60 2066  _compression>` f
+0000d5d0: 6f72 2064 6574 6169 6c73 2e0a 0a20 2020  or details...   
+0000d5e0: 2020 2020 204d 6f72 6520 776f 726b 6572       More worker
+0000d5f0: 7320 696d 7072 6f76 6520 7370 6565 642c  s improve speed,
+0000d600: 2062 7574 2061 6c73 6f20 696e 6372 6561   but also increa
+0000d610: 7365 206d 656d 6f72 7920 7573 6167 652e  se memory usage.
+0000d620: 0a0a 2020 2020 2020 2020 6060 3060 6020  ..        ``0`` 
+0000d630: 2864 6566 6175 6c74 2920 6d65 616e 7320  (default) means 
+0000d640: 2273 696e 676c 652d 7468 7265 6164 6564  "single-threaded
+0000d650: 206d 6f64 6522 2c20 6e6f 2077 6f72 6b65   mode", no worke
+0000d660: 7220 6973 2073 7061 776e 6564 2c20 636f  r is spawned, co
+0000d670: 6d70 7265 7373 696f 6e20 6973 2070 6572  mpression is per
+0000d680: 666f 726d 6564 2069 6e73 6964 6520 6361  formed inside ca
+0000d690: 6c6c 6572 2773 2074 6872 6561 642e 0a0a  ller's thread...
+0000d6a0: 2020 2020 2e2e 2076 6572 7369 6f6e 6368      .. versionch
+0000d6b0: 616e 6765 643a 3a20 302e 3135 2e31 0a20  anged:: 0.15.1. 
+0000d6c0: 2020 2020 2020 2053 6574 7469 6e67 2074         Setting t
+0000d6d0: 6f20 6060 3160 6020 6d65 616e 7320 2231  o ``1`` means "1
+0000d6e0: 2d74 6872 6561 6420 6d75 6c74 692d 7468  -thread multi-th
+0000d6f0: 7265 6164 6564 206d 6f64 6522 2c20 696e  readed mode", in
+0000d700: 7374 6561 6420 6f66 2022 7369 6e67 6c65  stead of "single
+0000d710: 2d74 6872 6561 6465 6420 6d6f 6465 222e  -threaded mode".
+0000d720: 0a0a 2020 2020 2e2e 2070 793a 6174 7472  ..    .. py:attr
+0000d730: 6962 7574 653a 3a20 6a6f 6253 697a 650a  ibute:: jobSize.
+0000d740: 0a20 2020 2020 2020 2053 697a 6520 6f66  .        Size of
+0000d750: 2061 2063 6f6d 7072 6573 7369 6f6e 206a   a compression j
+0000d760: 6f62 2c20 696e 2062 7974 6573 2e0a 0a20  ob, in bytes... 
+0000d770: 2020 2020 2020 2054 6869 7320 7661 6c75         This valu
+0000d780: 6520 6973 2065 6e66 6f72 6365 6420 6f6e  e is enforced on
+0000d790: 6c79 2077 6865 6e20 3a70 793a 6174 7472  ly when :py:attr
+0000d7a0: 3a60 7e43 5061 7261 6d65 7465 722e 6e62  :`~CParameter.nb
+0000d7b0: 576f 726b 6572 7360 203e 3d20 312e 0a0a  Workers` >= 1...
+0000d7c0: 2020 2020 2020 2020 4561 6368 2063 6f6d          Each com
+0000d7d0: 7072 6573 7369 6f6e 206a 6f62 2069 7320  pression job is 
+0000d7e0: 636f 6d70 6c65 7465 6420 696e 2070 6172  completed in par
+0000d7f0: 616c 6c65 6c2c 2073 6f20 7468 6973 2076  allel, so this v
+0000d800: 616c 7565 2063 616e 2069 6e64 6972 6563  alue can indirec
+0000d810: 746c 7920 696d 7061 6374 2074 6865 206e  tly impact the n
+0000d820: 756d 6265 7220 6f66 2061 6374 6976 6520  umber of active 
+0000d830: 7468 7265 6164 732e 0a0a 2020 2020 2020  threads...      
+0000d840: 2020 6060 3060 6020 6d65 616e 7320 6465    ``0`` means de
+0000d850: 6661 756c 742c 2077 6869 6368 2069 7320  fault, which is 
+0000d860: 6479 6e61 6d69 6361 6c6c 7920 6465 7465  dynamically dete
+0000d870: 726d 696e 6564 2062 6173 6564 206f 6e20  rmined based on 
+0000d880: 636f 6d70 7265 7373 696f 6e20 7061 7261  compression para
+0000d890: 6d65 7465 7273 2e0a 0a20 2020 2020 2020  meters...       
+0000d8a0: 204e 6f6e 2d7a 6572 6f20 7661 6c75 6520   Non-zero value 
+0000d8b0: 7769 6c6c 2062 6520 7369 6c65 6e74 6c79  will be silently
+0000d8c0: 2063 6c61 6d70 6564 2074 6f3a 0a0a 2020   clamped to:..  
+0000d8d0: 2020 2020 2020 2a20 6d69 6e69 6d75 6d20        * minimum 
+0000d8e0: 7661 6c75 653a 2060 606d 6178 286f 7665  value: ``max(ove
+0000d8f0: 726c 6170 5f73 697a 652c 2035 3132 5f4b  rlap_size, 512_K
+0000d900: 6942 2960 602e 206f 7665 726c 6170 5f73  iB)``. overlap_s
+0000d910: 697a 6520 6973 2073 7065 6369 6669 6564  ize is specified
+0000d920: 2062 7920 3a70 793a 6174 7472 3a60 7e43   by :py:attr:`~C
+0000d930: 5061 7261 6d65 7465 722e 6f76 6572 6c61  Parameter.overla
+0000d940: 704c 6f67 6020 7061 7261 6d65 7465 722e  pLog` parameter.
+0000d950: 0a20 2020 2020 2020 202a 206d 6178 696d  .        * maxim
+0000d960: 756d 2076 616c 7565 3a20 6060 3531 325f  um value: ``512_
+0000d970: 4d69 4220 6966 2033 325f 6269 745f 6275  MiB if 32_bit_bu
+0000d980: 696c 6420 656c 7365 2031 3032 345f 4d69  ild else 1024_Mi
+0000d990: 4260 602e 0a0a 2020 2020 2e2e 2070 793a  B``...    .. py:
+0000d9a0: 6174 7472 6962 7574 653a 3a20 6f76 6572  attribute:: over
+0000d9b0: 6c61 704c 6f67 0a0a 2020 2020 2020 2020  lapLog..        
+0000d9c0: 436f 6e74 726f 6c20 7468 6520 6f76 6572  Control the over
+0000d9d0: 6c61 7020 7369 7a65 2c20 6173 2061 2066  lap size, as a f
+0000d9e0: 7261 6374 696f 6e20 6f66 2077 696e 646f  raction of windo
+0000d9f0: 7720 7369 7a65 2e20 2854 6865 2022 7769  w size. (The "wi
+0000da00: 6e64 6f77 2073 697a 6522 2068 6572 6520  ndow size" here 
+0000da10: 6973 206e 6f74 2073 7472 6963 7420 3a70  is not strict :p
+0000da20: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
+0000da30: 7465 722e 7769 6e64 6f77 4c6f 6760 2c20  ter.windowLog`, 
+0000da40: 7365 6520 7a73 7464 2073 6f75 7263 6520  see zstd source 
+0000da50: 636f 6465 2e29 0a0a 2020 2020 2020 2020  code.)..        
+0000da60: 5468 6973 2076 616c 7565 2069 7320 656e  This value is en
+0000da70: 666f 7263 6564 206f 6e6c 7920 7768 656e  forced only when
+0000da80: 203a 7079 3a61 7474 723a 607e 4350 6172   :py:attr:`~CPar
+0000da90: 616d 6574 6572 2e6e 6257 6f72 6b65 7273  ameter.nbWorkers
+0000daa0: 6020 3e3d 2031 2e0a 0a20 2020 2020 2020  ` >= 1...       
+0000dab0: 2054 6865 206f 7665 726c 6170 2073 697a   The overlap siz
+0000dac0: 6520 6973 2061 6e20 616d 6f75 6e74 206f  e is an amount o
+0000dad0: 6620 6461 7461 2072 656c 6f61 6465 6420  f data reloaded 
+0000dae0: 6672 6f6d 2070 7265 7669 6f75 7320 6a6f  from previous jo
+0000daf0: 6220 6174 2074 6865 2062 6567 696e 6e69  b at the beginni
+0000db00: 6e67 206f 6620 6120 6e65 7720 6a6f 622e  ng of a new job.
+0000db10: 2049 7420 6865 6c70 7320 7072 6573 6572   It helps preser
+0000db20: 7665 2063 6f6d 7072 6573 7369 6f6e 2072  ve compression r
+0000db30: 6174 696f 2c20 7768 696c 6520 6561 6368  atio, while each
+0000db40: 206a 6f62 2069 7320 636f 6d70 7265 7373   job is compress
+0000db50: 6564 2069 6e20 7061 7261 6c6c 656c 2e20  ed in parallel. 
+0000db60: 4c61 7267 6572 2076 616c 7565 7320 696e  Larger values in
+0000db70: 6372 6561 7365 2063 6f6d 7072 6573 7369  crease compressi
+0000db80: 6f6e 2072 6174 696f 2c20 6275 7420 6465  on ratio, but de
+0000db90: 6372 6561 7365 2073 7065 6564 2e0a 0a20  crease speed... 
+0000dba0: 2020 2020 2020 2050 6f73 7369 626c 6520         Possible 
+0000dbb0: 7661 6c75 6573 2072 616e 6765 2066 726f  values range fro
+0000dbc0: 6d20 3020 746f 2039 3a0a 0a20 2020 2020  m 0 to 9:..     
+0000dbd0: 2020 202d 2030 206d 6561 6e73 2022 6465     - 0 means "de
+0000dbe0: 6661 756c 7422 203a 2054 6865 2076 616c  fault" : The val
+0000dbf0: 7565 2077 696c 6c20 6265 2064 6574 6572  ue will be deter
+0000dc00: 6d69 6e65 6420 6279 2074 6865 206c 6962  mined by the lib
+0000dc10: 7261 7279 2e20 5468 6520 7661 6c75 6520  rary. The value 
+0000dc20: 7661 7269 6573 2062 6574 7765 656e 2036  varies between 6
+0000dc30: 2061 6e64 2039 2c20 6465 7065 6e64 696e   and 9, dependin
+0000dc40: 6720 6f6e 203a 7079 3a61 7474 723a 607e  g on :py:attr:`~
+0000dc50: 4350 6172 616d 6574 6572 2e73 7472 6174  CParameter.strat
+0000dc60: 6567 7960 2e0a 2020 2020 2020 2020 2d20  egy`..        - 
+0000dc70: 3120 6d65 616e 7320 226e 6f20 6f76 6572  1 means "no over
+0000dc80: 6c61 7022 0a20 2020 2020 2020 202d 2039  lap".        - 9
+0000dc90: 206d 6561 6e73 2022 6675 6c6c 206f 7665   means "full ove
+0000dca0: 726c 6170 222c 2075 7369 6e67 2061 2066  rlap", using a f
+0000dcb0: 756c 6c20 7769 6e64 6f77 2073 697a 652e  ull window size.
+0000dcc0: 0a0a 2020 2020 2020 2020 4561 6368 2069  ..        Each i
+0000dcd0: 6e74 6572 6d65 6469 6174 6520 7261 6e6b  ntermediate rank
+0000dce0: 2069 6e63 7265 6173 6573 2f64 6563 7265   increases/decre
+0000dcf0: 6173 6573 206c 6f61 6420 7369 7a65 2062  ases load size b
+0000dd00: 7920 6120 6661 6374 6f72 2032 3a0a 0a20  y a factor 2:.. 
+0000dd10: 2020 2020 2020 2039 3a20 6675 6c6c 2077         9: full w
+0000dd20: 696e 646f 773b 2020 383a 2077 2f32 3b20  indow;  8: w/2; 
+0000dd30: 2037 3a20 772f 343b 2020 363a 2077 2f38   7: w/4;  6: w/8
+0000dd40: 3b20 2035 3a20 772f 3136 3b20 2034 3a20  ;  5: w/16;  4: 
+0000dd50: 772f 3332 3b20 2033 3a20 772f 3634 3b20  w/32;  3: w/64; 
+0000dd60: 2032 3a20 772f 3132 383b 2020 313a 206e   2: w/128;  1: n
+0000dd70: 6f20 6f76 6572 6c61 703b 2020 303a 2064  o overlap;  0: d
+0000dd80: 6566 6175 6c74 2e0a 0a0a 2e2e 205f 4450  efault...... _DP
+0000dd90: 6172 616d 6574 6572 3a0a 0a2e 2e20 7079  arameter:.... py
+0000dda0: 3a63 6c61 7373 3a3a 2044 5061 7261 6d65  :class:: DParame
+0000ddb0: 7465 7228 496e 7445 6e75 6d29 0a0a 2020  ter(IntEnum)..  
+0000ddc0: 2020 4164 7661 6e63 6564 2064 6563 6f6d    Advanced decom
+0000ddd0: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
+0000dde0: 6572 732e 0a0a 2020 2020 5768 656e 2075  ers...    When u
+0000ddf0: 7369 6e67 2c20 7075 7420 7468 6520 7061  sing, put the pa
+0000de00: 7261 6d65 7465 7273 2069 6e20 6120 6060  rameters in a ``
+0000de10: 6469 6374 6060 206f 626a 6563 742c 2074  dict`` object, t
+0000de20: 6865 206b 6579 2069 7320 6120 3a70 793a  he key is a :py:
+0000de30: 636c 6173 733a 6044 5061 7261 6d65 7465  class:`DParamete
+0000de40: 7260 206e 616d 652c 2074 6865 2076 616c  r` name, the val
+0000de50: 7565 2069 7320 6120 3332 2d62 6974 2073  ue is a 32-bit s
+0000de60: 6967 6e65 6420 696e 7465 6765 7220 7661  igned integer va
+0000de70: 6c75 652e 0a0a 2020 2020 2e2e 2073 6f75  lue...    .. sou
+0000de80: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
+0000de90: 0a0a 2020 2020 2020 2020 2320 7365 7420  ..        # set 
+0000dea0: 6d65 6d6f 7279 2061 6c6c 6f63 6174 696f  memory allocatio
+0000deb0: 6e20 6c69 6d69 7420 746f 2031 3620 4d69  n limit to 16 Mi
+0000dec0: 4220 2831 203c 3c20 3234 290a 2020 2020  B (1 << 24).    
+0000ded0: 2020 2020 6f70 7469 6f6e 203d 207b 4450      option = {DP
+0000dee0: 6172 616d 6574 6572 2e77 696e 646f 774c  arameter.windowL
+0000def0: 6f67 4d61 7820 3a20 3234 7d0a 0a20 2020  ogMax : 24}..   
+0000df00: 2020 2020 2023 2075 7365 6420 7769 7468       # used with
+0000df10: 2064 6563 6f6d 7072 6573 7328 2920 6675   decompress() fu
+0000df20: 6e63 7469 6f6e 0a20 2020 2020 2020 2064  nction.        d
+0000df30: 6563 6f6d 7072 6573 7365 645f 6461 7420  ecompressed_dat 
+0000df40: 3d20 6465 636f 6d70 7265 7373 2864 6174  = decompress(dat
+0000df50: 2c20 6f70 7469 6f6e 3d6f 7074 696f 6e29  , option=option)
+0000df60: 0a0a 2020 2020 2020 2020 2320 7573 6564  ..        # used
+0000df70: 2077 6974 6820 5a73 7464 4465 636f 6d70   with ZstdDecomp
+0000df80: 7265 7373 6f72 206f 626a 6563 740a 2020  ressor object.  
+0000df90: 2020 2020 2020 6420 3d20 5a73 7464 4465        d = ZstdDe
+0000dfa0: 636f 6d70 7265 7373 6f72 286f 7074 696f  compressor(optio
+0000dfb0: 6e3d 6f70 7469 6f6e 290a 2020 2020 2020  n=option).      
+0000dfc0: 2020 6465 636f 6d70 7265 7373 6564 5f64    decompressed_d
+0000dfd0: 6174 203d 2064 2e64 6563 6f6d 7072 6573  at = d.decompres
+0000dfe0: 7328 6461 7429 0a0a 2020 2020 5061 7261  s(dat)..    Para
+0000dff0: 6d65 7465 7220 7661 6c75 6520 7368 6f75  meter value shou
+0000e000: 6c64 2062 656c 6f6e 6720 746f 2061 6e20  ld belong to an 
+0000e010: 696e 7465 7276 616c 2077 6974 6820 6c6f  interval with lo
+0000e020: 7765 7220 616e 6420 7570 7065 7220 626f  wer and upper bo
+0000e030: 756e 6473 2c20 6f74 6865 7277 6973 6520  unds, otherwise 
+0000e040: 7468 6579 2077 696c 6c20 6569 7468 6572  they will either
+0000e050: 2074 7269 6767 6572 2061 6e20 6572 726f   trigger an erro
+0000e060: 7220 6f72 2062 6520 636c 616d 7065 6420  r or be clamped 
+0000e070: 7369 6c65 6e74 6c79 2e0a 0a20 2020 2054  silently...    T
+0000e080: 6865 2063 6f6e 7374 616e 7420 7661 6c75  he constant valu
+0000e090: 6573 206d 656e 7469 6f6e 6564 2062 656c  es mentioned bel
+0000e0a0: 6f77 2061 7265 2064 6566 696e 6564 2069  ow are defined i
+0000e0b0: 6e20 607a 7374 642e 6820 3c68 7474 7073  n `zstd.h <https
+0000e0c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
+0000e0d0: 6365 626f 6f6b 2f7a 7374 642f 626c 6f62  cebook/zstd/blob
+0000e0e0: 2f72 656c 6561 7365 2f6c 6962 2f7a 7374  /release/lib/zst
+0000e0f0: 642e 683e 605f 2c20 6e6f 7465 2074 6861  d.h>`_, note tha
+0000e100: 7420 7468 6573 6520 7661 6c75 6573 206d  t these values m
+0000e110: 6179 2062 6520 6469 6666 6572 656e 7420  ay be different 
+0000e120: 696e 2064 6966 6665 7265 6e74 207a 7374  in different zst
+0000e130: 6420 7665 7273 696f 6e73 2e0a 0a20 2020  d versions...   
+0000e140: 202e 2e20 7079 3a6d 6574 686f 643a 3a20   .. py:method:: 
+0000e150: 626f 756e 6473 2873 656c 6629 0a0a 2020  bounds(self)..  
+0000e160: 2020 2020 2020 5265 7475 726e 206c 6f77        Return low
+0000e170: 6572 2061 6e64 2075 7070 6572 2062 6f75  er and upper bou
+0000e180: 6e64 7320 6f66 2061 2070 6172 616d 6574  nds of a paramet
+0000e190: 6572 2c20 626f 7468 2069 6e63 6c75 7369  er, both inclusi
+0000e1a0: 7665 2e0a 0a20 2020 2020 2020 202e 2e20  ve...        .. 
+0000e1b0: 736f 7572 6365 636f 6465 3a3a 2070 7974  sourcecode:: pyt
+0000e1c0: 686f 6e0a 0a20 2020 2020 2020 2020 2020  hon..           
+0000e1d0: 203e 3e3e 2044 5061 7261 6d65 7465 722e   >>> DParameter.
+0000e1e0: 7769 6e64 6f77 4c6f 674d 6178 2e62 6f75  windowLogMax.bou
+0000e1f0: 6e64 7328 290a 2020 2020 2020 2020 2020  nds().          
+0000e200: 2020 2831 302c 2033 3129 0a0a 2020 2020    (10, 31)..    
+0000e210: 2e2e 2070 793a 6174 7472 6962 7574 653a  .. py:attribute:
+0000e220: 3a20 7769 6e64 6f77 4c6f 674d 6178 0a0a  : windowLogMax..
+0000e230: 2020 2020 2020 2020 5365 6c65 6374 2061          Select a
+0000e240: 2073 697a 6520 6c69 6d69 7420 2869 6e20   size limit (in 
+0000e250: 706f 7765 7220 6f66 2032 2920 6265 796f  power of 2) beyo
+0000e260: 6e64 2077 6869 6368 2074 6865 2073 7472  nd which the str
+0000e270: 6561 6d69 6e67 2041 5049 2077 696c 6c20  eaming API will 
+0000e280: 7265 6675 7365 2074 6f20 616c 6c6f 6361  refuse to alloca
+0000e290: 7465 206d 656d 6f72 7920 6275 6666 6572  te memory buffer
+0000e2a0: 2069 6e20 6f72 6465 7220 746f 2070 726f   in order to pro
+0000e2b0: 7465 6374 2074 6865 2068 6f73 7420 6672  tect the host fr
+0000e2c0: 6f6d 2075 6e72 6561 736f 6e61 626c 6520  om unreasonable 
+0000e2d0: 6d65 6d6f 7279 2072 6571 7569 7265 6d65  memory requireme
+0000e2e0: 6e74 732e 0a0a 2020 2020 2020 2020 4966  nts...        If
+0000e2f0: 2061 203a 7265 663a 6066 7261 6d65 3c66   a :ref:`frame<f
+0000e300: 7261 6d65 5f62 6c6f 636b 3e60 2072 6571  rame_block>` req
+0000e310: 7569 7265 7320 6d6f 7265 206d 656d 6f72  uires more memor
+0000e320: 7920 7468 616e 2074 6865 2073 6574 2076  y than the set v
+0000e330: 616c 7565 2c20 7261 6973 6573 2061 203a  alue, raises a :
+0000e340: 7079 3a63 6c61 7373 3a60 5a73 7464 4572  py:class:`ZstdEr
+0000e350: 726f 7260 2065 7863 6570 7469 6f6e 2c20  ror` exception, 
+0000e360: 7769 7468 2061 206d 6573 7361 6765 206c  with a message l
+0000e370: 696b 6520 2246 7261 6d65 2072 6571 7569  ike "Frame requi
+0000e380: 7265 7320 746f 6f20 6d75 6368 206d 656d  res too much mem
+0000e390: 6f72 7920 666f 7220 6465 636f 6469 6e67  ory for decoding
+0000e3a0: 222e 0a0a 2020 2020 2020 2020 5468 6973  "...        This
+0000e3b0: 2070 6172 616d 6574 6572 2069 7320 6f6e   parameter is on
+0000e3c0: 6c79 2075 7365 6675 6c20 696e 2073 7472  ly useful in str
+0000e3d0: 6561 6d69 6e67 206d 6f64 652c 2073 696e  eaming mode, sin
+0000e3e0: 6365 206e 6f20 696e 7465 726e 616c 2062  ce no internal b
+0000e3f0: 7566 6665 7220 6973 2061 6c6c 6f63 6174  uffer is allocat
+0000e400: 6564 2069 6e20 7369 6e67 6c65 2d70 6173  ed in single-pas
+0000e410: 7320 6d6f 6465 2e20 3a70 793a 6675 6e63  s mode. :py:func
+0000e420: 3a60 6465 636f 6d70 7265 7373 6020 6675  :`decompress` fu
+0000e430: 6e63 7469 6f6e 206d 6179 2075 7365 2073  nction may use s
+0000e440: 7472 6561 6d69 6e67 206d 6f64 6520 6f72  treaming mode or
+0000e450: 2073 696e 676c 652d 7061 7373 206d 6f64   single-pass mod
+0000e460: 652e 0a0a 2020 2020 2020 2020 4279 2064  e...        By d
+0000e470: 6566 6175 6c74 2c20 6120 6465 636f 6d70  efault, a decomp
+0000e480: 7265 7373 696f 6e20 636f 6e74 6578 7420  ression context 
+0000e490: 6163 6365 7074 7320 7769 6e64 6f77 2073  accepts window s
+0000e4a0: 697a 6573 203c 3d20 6060 2831 203c 3c20  izes <= ``(1 << 
+0000e4b0: 5a53 5444 5f57 494e 444f 574c 4f47 5f4c  ZSTD_WINDOWLOG_L
+0000e4c0: 494d 4954 5f44 4546 4155 4c54 2960 602c  IMIT_DEFAULT)``,
+0000e4d0: 2074 6865 2063 6f6e 7374 616e 7420 6973   the constant is
+0000e4e0: 2060 6032 3760 6020 696e 207a 7374 6420   ``27`` in zstd 
+0000e4f0: 7631 2e32 2b2c 206d 6561 6e73 2031 3238  v1.2+, means 128
+0000e500: 204d 6942 2028 3120 3c3c 2032 3729 2e20   MiB (1 << 27). 
+0000e510: 4966 2066 7261 6d65 2072 6571 7565 7374  If frame request
+0000e520: 6564 2077 696e 646f 7720 7369 7a65 2069  ed window size i
+0000e530: 7320 6772 6561 7465 7220 7468 616e 2074  s greater than t
+0000e540: 6869 7320 7661 6c75 652c 206e 6565 6420  his value, need 
+0000e550: 746f 2065 7870 6c69 6369 746c 7920 7365  to explicitly se
+0000e560: 7420 7468 6973 2070 6172 616d 6574 6572  t this parameter
+0000e570: 2e0a 0a20 2020 2020 2020 2053 7065 6369  ...        Speci
+0000e580: 616c 3a20 7661 6c75 6520 6060 3060 6020  al: value ``0`` 
+0000e590: 6d65 616e 7320 2275 7365 2064 6566 6175  means "use defau
+0000e5a0: 6c74 206d 6178 696d 756d 2077 696e 646f  lt maximum windo
+0000e5b0: 774c 6f67 222e 0a0a 0a2e 2e20 7079 3a63  wLog"...... py:c
+0000e5c0: 6c61 7373 3a3a 2053 7472 6174 6567 7928  lass:: Strategy(
+0000e5d0: 496e 7445 6e75 6d29 0a0a 2020 2020 5573  IntEnum)..    Us
+0000e5e0: 6564 2066 6f72 203a 7079 3a61 7474 723a  ed for :py:attr:
+0000e5f0: 6043 5061 7261 6d65 7465 722e 7374 7261  `CParameter.stra
+0000e600: 7465 6779 602e 0a0a 2020 2020 436f 6d70  tegy`...    Comp
+0000e610: 7265 7373 696f 6e20 7374 7261 7465 6769  ression strategi
+0000e620: 6573 2c20 6c69 7374 6564 2066 726f 6d20  es, listed from 
+0000e630: 6661 7374 6573 7420 746f 2073 7472 6f6e  fastest to stron
+0000e640: 6765 7374 2e0a 0a20 2020 204e 6f74 6520  gest...    Note 
+0000e650: 3a20 6e65 7720 7374 7261 7465 6769 6573  : new strategies
+0000e660: 202a 2a6d 6967 6874 2a2a 2062 6520 6164   **might** be ad
+0000e670: 6465 6420 696e 2074 6865 2066 7574 7572  ded in the futur
+0000e680: 652c 206f 6e6c 7920 7468 6520 6f72 6465  e, only the orde
+0000e690: 7220 2866 726f 6d20 6661 7374 2074 6f20  r (from fast to 
+0000e6a0: 7374 726f 6e67 2920 6973 2067 7561 7261  strong) is guara
+0000e6b0: 6e74 6565 642e 0a0a 2020 2020 2e2e 2070  nteed...    .. p
+0000e6c0: 793a 6174 7472 6962 7574 653a 3a20 6661  y:attribute:: fa
+0000e6d0: 7374 0a20 2020 202e 2e20 7079 3a61 7474  st.    .. py:att
+0000e6e0: 7269 6275 7465 3a3a 2064 6661 7374 0a20  ribute:: dfast. 
+0000e6f0: 2020 202e 2e20 7079 3a61 7474 7269 6275     .. py:attribu
+0000e700: 7465 3a3a 2067 7265 6564 790a 2020 2020  te:: greedy.    
+0000e710: 2e2e 2070 793a 6174 7472 6962 7574 653a  .. py:attribute:
+0000e720: 3a20 6c61 7a79 0a20 2020 202e 2e20 7079  : lazy.    .. py
+0000e730: 3a61 7474 7269 6275 7465 3a3a 206c 617a  :attribute:: laz
+0000e740: 7932 0a20 2020 202e 2e20 7079 3a61 7474  y2.    .. py:att
+0000e750: 7269 6275 7465 3a3a 2062 746c 617a 7932  ribute:: btlazy2
+0000e760: 0a20 2020 202e 2e20 7079 3a61 7474 7269  .    .. py:attri
+0000e770: 6275 7465 3a3a 2062 746f 7074 0a20 2020  bute:: btopt.   
+0000e780: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+0000e790: 3a3a 2062 7475 6c74 7261 0a20 2020 202e  :: btultra.    .
+0000e7a0: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
+0000e7b0: 2062 7475 6c74 7261 320a 0a20 2020 202e   btultra2..    .
+0000e7c0: 2e20 736f 7572 6365 636f 6465 3a3a 2070  . sourcecode:: p
+0000e7d0: 7974 686f 6e0a 0a20 2020 2020 2020 206f  ython..        o
 0000e7e0: 7074 696f 6e20 3d20 7b43 5061 7261 6d65  ption = {CParame
-0000e7f0: 7465 722e 6e62 576f 726b 6572 7320 3a20  ter.nbWorkers : 
-0000e800: 347d 0a20 2020 2020 2020 2063 6f6d 7072  4}.        compr
-0000e810: 6573 7365 645f 6461 7420 3d20 636f 6d70  essed_dat = comp
-0000e820: 7265 7373 2872 6177 5f64 6174 2c20 6f70  ress(raw_dat, op
-0000e830: 7469 6f6e 290a 0a20 2020 2054 6865 2064  tion)..    The d
-0000e840: 6174 6120 7769 6c6c 2062 6520 7370 6c69  ata will be spli
-0000e850: 7420 696e 746f 2070 6f72 7469 6f6e 7320  t into portions 
-0000e860: 616e 6420 636f 6d70 7265 7373 6564 2069  and compressed i
-0000e870: 6e20 7061 7261 6c6c 656c 2e20 5468 6520  n parallel. The 
-0000e880: 706f 7274 696f 6e20 7369 7a65 2063 616e  portion size can
-0000e890: 2062 6520 7370 6563 6966 6965 6420 6279   be specified by
-0000e8a0: 203a 7079 3a61 7474 723a 6043 5061 7261   :py:attr:`CPara
-0000e8b0: 6d65 7465 722e 6a6f 6253 697a 6560 2070  meter.jobSize` p
-0000e8c0: 6172 616d 6574 6572 2c20 7468 6520 6f76  arameter, the ov
-0000e8d0: 6572 6c61 7020 7369 7a65 2063 616e 2062  erlap size can b
-0000e8e0: 6520 7370 6563 6966 6965 6420 6279 203a  e specified by :
-0000e8f0: 7079 3a61 7474 723a 6043 5061 7261 6d65  py:attr:`CParame
-0000e900: 7465 722e 6f76 6572 6c61 704c 6f67 6020  ter.overlapLog` 
-0000e910: 7061 7261 6d65 7465 722c 2075 7375 616c  parameter, usual
-0000e920: 6c79 2064 6f6e 2774 206e 6565 6420 746f  ly don't need to
-0000e930: 2073 6574 2074 6865 7365 2e0a 0a20 2020   set these...   
-0000e940: 2054 6865 206d 756c 7469 2d74 6872 6561   The multi-threa
-0000e950: 6465 6420 6f75 7470 7574 2077 696c 6c20  ded output will 
-0000e960: 6265 2064 6966 6665 7265 6e74 2074 6861  be different tha
-0000e970: 6e20 7468 6520 7369 6e67 6c65 2d74 6872  n the single-thr
-0000e980: 6561 6465 6420 6f75 7470 7574 2e20 486f  eaded output. Ho
-0000e990: 7765 7665 722c 2062 6f74 6820 6172 6520  wever, both are 
-0000e9a0: 6465 7465 726d 696e 6973 7469 632c 2061  deterministic, a
-0000e9b0: 6e64 2074 6865 206d 756c 7469 2d74 6872  nd the multi-thr
-0000e9c0: 6561 6465 6420 6f75 7470 7574 2070 726f  eaded output pro
-0000e9d0: 6475 6365 7320 7468 6520 7361 6d65 2063  duces the same c
-0000e9e0: 6f6d 7072 6573 7365 6420 6461 7461 206e  ompressed data n
-0000e9f0: 6f20 6d61 7474 6572 2068 6f77 206d 616e  o matter how man
-0000ea00: 7920 7468 7265 6164 7320 7573 6564 2e0a  y threads used..
-0000ea10: 0a20 2020 2054 6865 206d 756c 7469 2d74  .    The multi-t
-0000ea20: 6872 6561 6465 6420 6f75 7470 7574 2069  hreaded output i
-0000ea30: 7320 6120 7369 6e67 6c65 203a 7265 663a  s a single :ref:
-0000ea40: 6066 7261 6d65 3c66 7261 6d65 5f62 6c6f  `frame<frame_blo
-0000ea50: 636b 3e60 2c20 6974 2773 206c 6172 6765  ck>`, it's large
-0000ea60: 7220 6120 6c69 7474 6c65 2e20 436f 6d70  r a little. Comp
-0000ea70: 7265 7373 696e 6720 6120 3532 302e 3538  ressing a 520.58
-0000ea80: 204d 6942 2064 6174 612c 2073 696e 676c   MiB data, singl
-0000ea90: 652d 7468 7265 6164 6564 206f 7574 7075  e-threaded outpu
-0000eaa0: 7420 6973 2032 3733 2e35 3520 4d69 422c  t is 273.55 MiB,
-0000eab0: 206d 756c 7469 2d74 6872 6561 6465 6420   multi-threaded 
-0000eac0: 6f75 7470 7574 2069 7320 3237 342e 3333  output is 274.33
-0000ead0: 204d 6942 2e0a 0a20 2020 202e 2e20 6869   MiB...    .. hi
-0000eae0: 6e74 3a3a 0a20 2020 2020 2020 2055 7369  nt::.        Usi
-0000eaf0: 6e67 2022 4350 5520 7068 7973 6963 616c  ng "CPU physical
-0000eb00: 2063 6f72 6573 206e 756d 6265 7222 2061   cores number" a
-0000eb10: 7320 7468 7265 6164 7320 6e75 6d62 6572  s threads number
-0000eb20: 206d 6179 2062 6520 7468 6520 6661 7374   may be the fast
-0000eb30: 6573 742c 2074 6f20 6765 7420 7468 6520  est, to get the 
-0000eb40: 6e75 6d62 6572 206e 6565 6420 746f 2069  number need to i
-0000eb50: 6e73 7461 6c6c 2074 6869 7264 2d70 6172  nstall third-par
-0000eb60: 7479 206d 6f64 756c 652e 2060 6f73 2e63  ty module. `os.c
-0000eb70: 7075 5f63 6f75 6e74 2829 203c 6874 7470  pu_count() <http
-0000eb80: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-0000eb90: 6f72 672f 332f 6c69 6272 6172 792f 6f73  org/3/library/os
-0000eba0: 2e68 746d 6c23 6f73 2e63 7075 5f63 6f75  .html#os.cpu_cou
-0000ebb0: 6e74 3e60 5f20 6361 6e20 6f6e 6c79 2067  nt>`_ can only g
-0000ebc0: 6574 2022 4350 5520 6c6f 6769 6361 6c20  et "CPU logical 
-0000ebd0: 636f 7265 7320 6e75 6d62 6572 2220 2868  cores number" (h
-0000ebe0: 7970 6572 2d74 6872 6561 6469 6e67 2063  yper-threading c
-0000ebf0: 6170 6162 696c 6974 7929 2e0a 0a0a 5269  apability)....Ri
-0000ec00: 6368 206d 656d 6f72 7920 6d6f 6465 0a3e  ch memory mode.>
-0000ec10: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e0a  >>>>>>>>>>>>>>>.
-0000ec20: 0a2e 2e20 5f72 6963 685f 6d65 6d3a 0a0a  ... _rich_mem:..
-0000ec30: 2e2e 206e 6f74 653a 3a20 5269 6368 206d  .. note:: Rich m
-0000ec40: 656d 6f72 7920 6d6f 6465 0a0a 2020 2020  emory mode..    
-0000ec50: 7079 7a73 7464 206d 6f64 756c 6520 6861  pyzstd module ha
-0000ec60: 7320 6120 2272 6963 6820 6d65 6d6f 7279  s a "rich memory
-0000ec70: 206d 6f64 6522 2066 6f72 2063 6f6d 7072   mode" for compr
-0000ec80: 6573 7369 6f6e 2e20 4974 2061 6c6c 6f63  ession. It alloc
-0000ec90: 6174 6573 206d 6f72 6520 6d65 6d6f 7279  ates more memory
-0000eca0: 2066 6f72 206f 7574 7075 7420 6275 6666   for output buff
-0000ecb0: 6572 2c20 616e 6420 6661 7374 6572 2069  er, and faster i
-0000ecc0: 6e20 736f 6d65 2063 6173 6573 2e20 5375  n some cases. Su
-0000ecd0: 6974 6162 6c65 2066 6f72 2065 7874 7265  itable for extre
-0000ece0: 6d65 6c79 2066 6173 7420 636f 6d70 7265  mely fast compre
-0000ecf0: 7373 696f 6e20 7363 656e 6172 696f 732e  ssion scenarios.
-0000ed00: 0a0a 2020 2020 5468 6572 6520 6973 2061  ..    There is a
-0000ed10: 203a 7079 3a66 756e 633a 6072 6963 686d   :py:func:`richm
-0000ed20: 656d 5f63 6f6d 7072 6573 7360 2066 756e  em_compress` fun
-0000ed30: 6374 696f 6e2c 2061 203a 7079 3a63 6c61  ction, a :py:cla
-0000ed40: 7373 3a60 5269 6368 4d65 6d5a 7374 6443  ss:`RichMemZstdC
-0000ed50: 6f6d 7072 6573 736f 7260 2063 6c61 7373  ompressor` class
-0000ed60: 2e0a 0a20 2020 2043 7572 7265 6e74 6c79  ...    Currently
-0000ed70: 2069 7420 776f 6e27 7420 6265 2066 6173   it won't be fas
-0000ed80: 7465 7220 7768 656e 2075 7369 6e67 203a  ter when using :
-0000ed90: 7265 663a 607a 7374 6420 6d75 6c74 692d  ref:`zstd multi-
-0000eda0: 7468 7265 6164 6564 2063 6f6d 7072 6573  threaded compres
-0000edb0: 7369 6f6e 203c 6d74 5f63 6f6d 7072 6573  sion <mt_compres
-0000edc0: 7369 6f6e 3e60 2c20 6974 2077 696c 6c20  sion>`, it will 
-0000edd0: 6973 7375 6520 6120 6060 5265 736f 7572  issue a ``Resour
-0000ede0: 6365 5761 726e 696e 6773 6060 2069 6e20  ceWarnings`` in 
-0000edf0: 7468 6973 2063 6173 652e 0a0a 2020 2020  this case...    
-0000ee00: 4566 6665 6374 733a 0a0a 2020 2020 2a20  Effects:..    * 
-0000ee10: 5468 6520 6f75 7470 7574 2062 7566 6665  The output buffe
-0000ee20: 7220 6973 206c 6172 6765 7220 7468 616e  r is larger than
-0000ee30: 2069 6e70 7574 2064 6174 6120 6120 6c69   input data a li
-0000ee40: 7474 6c65 2e0a 2020 2020 2a20 4966 2069  ttle..    * If i
-0000ee50: 6e70 7574 2064 6174 6120 6973 206c 6172  nput data is lar
-0000ee60: 6765 7220 7468 616e 207e 3331 2e38 4b42  ger than ~31.8KB
-0000ee70: 2c20 7570 2074 6f20 3232 2520 6661 7374  , up to 22% fast
-0000ee80: 6572 2e20 5468 6520 6c6f 7765 7220 7468  er. The lower th
-0000ee90: 6520 636f 6d70 7265 7373 696f 6e20 6c65  e compression le
-0000eea0: 7665 6c2c 2074 6865 206d 7563 6820 6661  vel, the much fa
-0000eeb0: 7374 6572 2069 7420 6973 2075 7375 616c  ster it is usual
-0000eec0: 6c79 2e0a 0a20 2020 2057 6865 6e20 6e6f  ly...    When no
-0000eed0: 7420 7573 696e 6720 7468 6973 206d 6f64  t using this mod
-0000eee0: 652c 2074 6865 206f 7574 7075 7420 6275  e, the output bu
-0000eef0: 6666 6572 2067 726f 7773 2060 6772 6164  ffer grows `grad
-0000ef00: 7561 6c6c 7920 3c68 7474 7073 3a2f 2f67  ually <https://g
-0000ef10: 6974 6875 622e 636f 6d2f 616e 696d 616c  ithub.com/animal
-0000ef20: 697a 652f 7079 7a73 7464 2f62 6c6f 622f  ize/pyzstd/blob/
-0000ef30: 302e 3134 2e32 2f73 7263 2f5f 7a73 7464  0.14.2/src/_zstd
-0000ef40: 6d6f 6475 6c65 2e63 234c 3133 352d 4c31  module.c#L135-L1
-0000ef50: 3630 3e60 5f2c 2069 6e20 6f72 6465 7220  60>`_, in order 
-0000ef60: 6e6f 7420 746f 2061 6c6c 6f63 6174 6520  not to allocate 
-0000ef70: 746f 6f20 6d75 6368 206d 656d 6f72 792e  too much memory.
-0000ef80: 2054 6865 206e 6567 6174 6976 6520 6566   The negative ef
-0000ef90: 6665 6374 2069 7320 7468 6174 2070 797a  fect is that pyz
-0000efa0: 7374 6420 6d6f 6475 6c65 2075 7375 616c  std module usual
-0000efb0: 6c79 206e 6565 6420 746f 2063 616c 6c20  ly need to call 
-0000efc0: 7468 6520 756e 6465 726c 7969 6e67 207a  the underlying z
-0000efd0: 7374 6420 6c69 6272 6172 7927 7320 636f  std library's co
-0000efe0: 6d70 7265 7373 2066 756e 6374 696f 6e20  mpress function 
-0000eff0: 6d75 6c74 6970 6c65 2074 696d 6573 2e0a  multiple times..
-0000f000: 0a20 2020 2057 6865 6e20 7573 696e 6720  .    When using 
-0000f010: 7468 6973 206d 6f64 652c 2074 6865 2073  this mode, the s
-0000f020: 697a 6520 6f66 206f 7574 7075 7420 6275  ize of output bu
-0000f030: 6666 6572 2069 7320 7072 6f76 6964 6564  ffer is provided
-0000f040: 2062 7920 5a53 5444 5f63 6f6d 7072 6573   by ZSTD_compres
-0000f050: 7342 6f75 6e64 2829 2066 756e 6374 696f  sBound() functio
-0000f060: 6e2c 2077 6869 6368 2069 7320 6c61 7267  n, which is larg
-0000f070: 6572 2074 6861 6e20 696e 7075 7420 6461  er than input da
-0000f080: 7461 2061 206c 6974 746c 6520 286d 6178  ta a little (max
-0000f090: 696d 756d 2063 6f6d 7072 6573 7365 6420  imum compressed 
-0000f0a0: 7369 7a65 2069 6e20 776f 7273 7420 6361  size in worst ca
-0000f0b0: 7365 2073 696e 676c 652d 7061 7373 2073  se single-pass s
-0000f0c0: 6365 6e61 7269 6f29 2e20 466f 7220 6120  cenario). For a 
-0000f0d0: 3130 3020 4d69 4220 696e 7075 7420 6461  100 MiB input da
-0000f0e0: 7461 2c20 7468 6520 616c 6c6f 6361 7465  ta, the allocate
-0000f0f0: 6420 6f75 7470 7574 2062 7566 6665 7220  d output buffer 
-0000f100: 6973 2028 3130 3020 4d69 4220 2b20 3430  is (100 MiB + 40
-0000f110: 3020 4b69 4229 2e20 5468 6520 756e 6465  0 KiB). The unde
-0000f120: 726c 7969 6e67 207a 7374 6420 6c69 6272  rlying zstd libr
-0000f130: 6172 7920 6176 6f69 6473 2065 7874 7261  ary avoids extra
-0000f140: 206d 656d 6f72 7920 636f 7079 2066 6f72   memory copy for
-0000f150: 2074 6869 7320 6f75 7470 7574 2062 7566   this output buf
-0000f160: 6665 7220 7369 7a65 2e0a 0a20 2020 202e  fer size...    .
-0000f170: 2e20 736f 7572 6365 636f 6465 3a3a 2070  . sourcecode:: p
-0000f180: 7974 686f 6e0a 0a20 2020 2020 2020 2023  ython..        #
-0000f190: 2075 7365 2072 6963 686d 656d 5f63 6f6d   use richmem_com
-0000f1a0: 7072 6573 7328 2920 6675 6e63 7469 6f6e  press() function
-0000f1b0: 0a20 2020 2020 2020 2063 6f6d 7072 6573  .        compres
-0000f1c0: 7365 645f 6461 7420 3d20 7269 6368 6d65  sed_dat = richme
-0000f1d0: 6d5f 636f 6d70 7265 7373 2872 6177 5f64  m_compress(raw_d
-0000f1e0: 6174 290a 0a20 2020 2020 2020 2023 2072  at)..        # r
-0000f1f0: 6575 7365 2052 6963 684d 656d 5a73 7464  euse RichMemZstd
-0000f200: 436f 6d70 7265 7373 6f72 206f 626a 6563  Compressor objec
-0000f210: 740a 2020 2020 2020 2020 6320 3d20 5269  t.        c = Ri
-0000f220: 6368 4d65 6d5a 7374 6443 6f6d 7072 6573  chMemZstdCompres
-0000f230: 736f 7228 290a 2020 2020 2020 2020 6672  sor().        fr
-0000f240: 616d 6531 203d 2063 2e63 6f6d 7072 6573  ame1 = c.compres
-0000f250: 7328 7261 775f 6461 7431 290a 2020 2020  s(raw_dat1).    
-0000f260: 2020 2020 6672 616d 6532 203d 2063 2e63      frame2 = c.c
-0000f270: 6f6d 7072 6573 7328 7261 775f 6461 7432  ompress(raw_dat2
-0000f280: 290a 0a20 2020 2043 6f6d 7072 6573 7369  )..    Compressi
-0000f290: 6e67 2061 2035 3230 2e35 3820 4d69 4220  ng a 520.58 MiB 
-0000f2a0: 6461 7461 2c20 6974 2061 6363 656c 6572  data, it acceler
-0000f2b0: 6174 6573 2066 726f 6d20 352e 3430 2073  ates from 5.40 s
-0000f2c0: 6563 6f6e 6473 2074 6f20 342e 3632 2073  econds to 4.62 s
-0000f2d0: 6563 6f6e 6473 2e0a 0a0a 5573 6520 7769  econds....Use wi
-0000f2e0: 7468 2074 6172 6669 6c65 206d 6f64 756c  th tarfile modul
-0000f2f0: 650a 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  e.>>>>>>>>>>>>>>
-0000f300: 3e3e 3e3e 3e3e 3e3e 3e0a 0a2e 2e20 5f77  >>>>>>>>>.... _w
-0000f310: 6974 685f 7461 7266 696c 653a 0a0a 2e2e  ith_tarfile:....
-0000f320: 206e 6f74 653a 3a20 5573 6520 7769 7468   note:: Use with
-0000f330: 2074 6172 6669 6c65 206d 6f64 756c 650a   tarfile module.
-0000f340: 0a20 2020 2050 7974 686f 6e27 7320 6074  .    Python's `t
-0000f350: 6172 6669 6c65 203c 6874 7470 733a 2f2f  arfile <https://
-0000f360: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-0000f370: 332f 6c69 6272 6172 792f 7461 7266 696c  3/library/tarfil
-0000f380: 652e 6874 6d6c 3e60 5f20 6d6f 6475 6c65  e.html>`_ module
-0000f390: 2073 7570 706f 7274 7320 6172 6269 7472   supports arbitr
-0000f3a0: 6172 7920 636f 6d70 7265 7373 696f 6e20  ary compression 
-0000f3b0: 616c 676f 7269 7468 6d73 2062 7920 7072  algorithms by pr
-0000f3c0: 6f76 6964 696e 6720 6120 6669 6c65 206f  oviding a file o
-0000f3d0: 626a 6563 742e 0a0a 2020 2020 5468 6973  bject...    This
-0000f3e0: 2063 6f64 6520 656e 6361 7073 756c 6174   code encapsulat
-0000f3f0: 6573 2061 2060 605a 7374 6454 6172 4669  es a ``ZstdTarFi
-0000f400: 6c65 6060 2063 6c61 7373 2075 7369 6e67  le`` class using
-0000f410: 203a 7079 3a63 6c61 7373 3a60 5a73 7464   :py:class:`Zstd
-0000f420: 4669 6c65 602c 2069 7420 6361 6e20 6265  File`, it can be
-0000f430: 2075 7365 6420 6c69 6b65 2060 7461 7266   used like `tarf
-0000f440: 696c 652e 5461 7246 696c 6520 3c68 7474  ile.TarFile <htt
-0000f450: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
-0000f460: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f74  .org/3/library/t
-0000f470: 6172 6669 6c65 2e68 746d 6c23 7461 7266  arfile.html#tarf
-0000f480: 696c 652e 5461 7246 696c 653e 605f 2063  ile.TarFile>`_ c
-0000f490: 6c61 7373 3a0a 0a20 2020 202e 2e20 736f  lass:..    .. so
-0000f4a0: 7572 6365 636f 6465 3a3a 2070 7974 686f  urcecode:: pytho
-0000f4b0: 6e0a 0a20 2020 2020 2020 2069 6d70 6f72  n..        impor
-0000f4c0: 7420 7461 7266 696c 650a 0a20 2020 2020  t tarfile..     
-0000f4d0: 2020 2023 2077 6865 6e20 7573 696e 6720     # when using 
-0000f4e0: 7265 6164 206d 6f64 6520 2864 6563 6f6d  read mode (decom
-0000f4f0: 7072 6573 7369 6f6e 292c 2074 6865 206c  pression), the l
-0000f500: 6576 656c 5f6f 725f 6f70 7469 6f6e 2070  evel_or_option p
-0000f510: 6172 616d 6574 6572 0a20 2020 2020 2020  arameter.       
-0000f520: 2023 2063 616e 206f 6e6c 7920 6265 2061   # can only be a
-0000f530: 2064 6963 7420 6f62 6a65 6374 2c20 7468   dict object, th
-0000f540: 6174 2072 6570 7265 7365 6e74 7320 6465  at represents de
-0000f550: 636f 6d70 7265 7373 696f 6e20 6f70 7469  compression opti
-0000f560: 6f6e 2e20 4974 0a20 2020 2020 2020 2023  on. It.        #
-0000f570: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-0000f580: 2069 6e74 2074 7970 6520 636f 6d70 7265   int type compre
-0000f590: 7373 696f 6e20 6c65 7665 6c20 696e 2074  ssion level in t
-0000f5a0: 6869 7320 6361 7365 2e0a 0a20 2020 2020  his case...     
-0000f5b0: 2020 2063 6c61 7373 205a 7374 6454 6172     class ZstdTar
-0000f5c0: 4669 6c65 2874 6172 6669 6c65 2e54 6172  File(tarfile.Tar
-0000f5d0: 4669 6c65 293a 0a20 2020 2020 2020 2020  File):.         
-0000f5e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000f5f0: 7365 6c66 2c20 6e61 6d65 2c20 6d6f 6465  self, name, mode
-0000f600: 3d27 7227 2c20 2a2c 206c 6576 656c 5f6f  ='r', *, level_o
-0000f610: 725f 6f70 7469 6f6e 3d4e 6f6e 652c 207a  r_option=None, z
-0000f620: 7374 645f 6469 6374 3d4e 6f6e 652c 202a  std_dict=None, *
-0000f630: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-0000f640: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
-0000f650: 7374 645f 6669 6c65 203d 205a 7374 6446  std_file = ZstdF
-0000f660: 696c 6528 6e61 6d65 2c20 6d6f 6465 2c0a  ile(name, mode,.
-0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f690: 2020 2020 2020 2020 2020 6c65 7665 6c5f            level_
-0000f6a0: 6f72 5f6f 7074 696f 6e3d 6c65 7665 6c5f  or_option=level_
-0000f6b0: 6f72 5f6f 7074 696f 6e2c 0a20 2020 2020  or_option,.     
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6e0: 2020 2020 207a 7374 645f 6469 6374 3d7a       zstd_dict=z
-0000f6f0: 7374 645f 6469 6374 290a 2020 2020 2020  std_dict).      
-0000f700: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000f710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f720: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-0000f730: 745f 5f28 6669 6c65 6f62 6a3d 7365 6c66  t__(fileobj=self
-0000f740: 2e7a 7374 645f 6669 6c65 2c20 6d6f 6465  .zstd_file, mode
-0000f750: 3d6d 6f64 652c 202a 2a6b 7761 7267 7329  =mode, **kwargs)
-0000f760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f770: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-0000f780: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f790: 662e 7a73 7464 5f66 696c 652e 636c 6f73  f.zstd_file.clos
-0000f7a0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000f7b0: 2020 2020 2020 2020 7261 6973 650a 0a20          raise.. 
-0000f7c0: 2020 2020 2020 2020 2020 2064 6566 2063             def c
-0000f7d0: 6c6f 7365 2873 656c 6629 3a0a 2020 2020  lose(self):.    
-0000f7e0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-0000f7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f800: 2020 2020 2073 7570 6572 2829 2e63 6c6f       super().clo
-0000f810: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
-0000f820: 2020 2020 2066 696e 616c 6c79 3a0a 2020       finally:.  
-0000f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f840: 2020 7365 6c66 2e7a 7374 645f 6669 6c65    self.zstd_file
-0000f850: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
-0000f860: 2020 2320 7772 6974 6520 2e74 6172 2e7a    # write .tar.z
-0000f870: 7374 2066 696c 6520 2863 6f6d 7072 6573  st file (compres
-0000f880: 7369 6f6e 290a 2020 2020 2020 2020 7769  sion).        wi
-0000f890: 7468 205a 7374 6454 6172 4669 6c65 2827  th ZstdTarFile('
-0000f8a0: 6172 6368 6976 652e 7461 722e 7a73 7427  archive.tar.zst'
-0000f8b0: 2c20 6d6f 6465 3d27 7727 2c20 6c65 7665  , mode='w', leve
-0000f8c0: 6c5f 6f72 5f6f 7074 696f 6e3d 3529 2061  l_or_option=5) a
-0000f8d0: 7320 7461 723a 0a20 2020 2020 2020 2020  s tar:.         
-0000f8e0: 2020 2023 2064 6f20 736f 6d65 7468 696e     # do somethin
-0000f8f0: 670a 0a20 2020 2020 2020 2023 2072 6561  g..        # rea
-0000f900: 6420 2e74 6172 2e7a 7374 2066 696c 6520  d .tar.zst file 
-0000f910: 2864 6563 6f6d 7072 6573 7369 6f6e 290a  (decompression).
-0000f920: 2020 2020 2020 2020 7769 7468 205a 7374          with Zst
-0000f930: 6454 6172 4669 6c65 2827 6172 6368 6976  dTarFile('archiv
-0000f940: 652e 7461 722e 7a73 7427 2c20 6d6f 6465  e.tar.zst', mode
-0000f950: 3d27 7227 2920 6173 2074 6172 3a0a 2020  ='r') as tar:.  
-0000f960: 2020 2020 2020 2020 2020 2320 646f 2073            # do s
-0000f970: 6f6d 6574 6869 6e67 0a0a 2020 2020 5768  omething..    Wh
-0000f980: 656e 2074 6865 2061 626f 7665 2063 6f64  en the above cod
-0000f990: 6520 6973 2069 6e20 7265 6164 206d 6f64  e is in read mod
-0000f9a0: 6520 2864 6563 6f6d 7072 6573 7369 6f6e  e (decompression
-0000f9b0: 292c 2061 6e64 2073 656c 6563 7469 7665  ), and selective
-0000f9c0: 6c79 2072 6561 6420 6669 6c65 7320 6d75  ly read files mu
-0000f9d0: 6c74 6970 6c65 2074 696d 6573 2c20 6974  ltiple times, it
-0000f9e0: 206d 6179 2073 6565 6b20 746f 2070 7265   may seek to pre
-0000f9f0: 7669 6f75 7320 706f 7369 7469 6f6e 732c  vious positions,
-0000fa00: 2074 6865 6e20 7468 6520 6465 636f 6d70   then the decomp
-0000fa10: 7265 7373 696f 6e20 6861 7320 746f 2062  ression has to b
-0000fa20: 6520 7265 7374 6172 7465 6420 6672 6f6d  e restarted from
-0000fa30: 207a 6572 6f2e 2049 6620 7468 6973 2073   zero. If this s
-0000fa40: 6c6f 7773 2064 6f77 6e20 7468 6520 6f70  lows down the op
-0000fa50: 6572 6174 696f 6e73 2c20 7468 6520 6172  erations, the ar
-0000fa60: 6368 6976 6520 6361 6e20 6265 2064 6563  chive can be dec
-0000fa70: 6f6d 7072 6573 7365 6420 746f 2061 2074  ompressed to a t
-0000fa80: 656d 706f 7261 7279 2066 696c 652c 2061  emporary file, a
-0000fa90: 6e64 2072 6561 6420 6672 6f6d 2069 742e  nd read from it.
-0000faa0: 2054 6869 7320 636f 6465 2065 6e63 6170   This code encap
-0000fab0: 7375 6c61 7465 7320 7468 6520 7072 6f63  sulates the proc
-0000fac0: 6573 733a 0a0a 2020 2020 2e2e 2073 6f75  ess:..    .. sou
-0000fad0: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
-0000fae0: 0a0a 2020 2020 2020 2020 696d 706f 7274  ..        import
-0000faf0: 2063 6f6e 7465 7874 6c69 620a 2020 2020   contextlib.    
-0000fb00: 2020 2020 696d 706f 7274 2069 6f0a 2020      import io.  
-0000fb10: 2020 2020 2020 696d 706f 7274 2074 6172        import tar
-0000fb20: 6669 6c65 0a20 2020 2020 2020 2069 6d70  file.        imp
-0000fb30: 6f72 7420 7465 6d70 6669 6c65 0a20 2020  ort tempfile.   
-0000fb40: 2020 2020 2066 726f 6d20 7079 7a73 7464       from pyzstd
-0000fb50: 2069 6d70 6f72 7420 6465 636f 6d70 7265   import decompre
-0000fb60: 7373 5f73 7472 6561 6d0a 0a20 2020 2020  ss_stream..     
-0000fb70: 2020 2040 636f 6e74 6578 746c 6962 2e63     @contextlib.c
-0000fb80: 6f6e 7465 7874 6d61 6e61 6765 720a 2020  ontextmanager.  
-0000fb90: 2020 2020 2020 6465 6620 5a73 7464 5461        def ZstdTa
-0000fba0: 7252 6561 6465 7228 6e61 6d65 2c20 2a2c  rReader(name, *,
-0000fbb0: 207a 7374 645f 6469 6374 3d4e 6f6e 652c   zstd_dict=None,
-0000fbc0: 206f 7074 696f 6e3d 4e6f 6e65 2c20 2a2a   option=None, **
-0000fbd0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-0000fbe0: 2020 2020 2077 6974 6820 696f 2e6f 7065       with io.ope
-0000fbf0: 6e28 6e61 6d65 2c20 2772 6227 2920 6173  n(name, 'rb') as
-0000fc00: 2069 6668 3a0a 2020 2020 2020 2020 2020   ifh:.          
-0000fc10: 2020 2020 2020 7769 7468 2074 656d 7066        with tempf
-0000fc20: 696c 652e 5465 6d70 6f72 6172 7946 696c  ile.TemporaryFil
-0000fc30: 6528 2920 6173 2074 6d70 5f66 696c 653a  e() as tmp_file:
-0000fc40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc50: 2020 2020 2064 6563 6f6d 7072 6573 735f       decompress_
-0000fc60: 7374 7265 616d 2869 6668 2c20 746d 705f  stream(ifh, tmp_
-0000fc70: 6669 6c65 2c0a 2020 2020 2020 2020 2020  file,.          
-0000fc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc90: 2020 2020 2020 2020 2020 2020 7a73 7464              zstd
-0000fca0: 5f64 6963 743d 7a73 7464 5f64 6963 742c  _dict=zstd_dict,
-0000fcb0: 206f 7074 696f 6e3d 6f70 7469 6f6e 290a   option=option).
-0000fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcd0: 2020 2020 746d 705f 6669 6c65 2e73 6565      tmp_file.see
-0000fce0: 6b28 3029 0a20 2020 2020 2020 2020 2020  k(0).           
-0000fcf0: 2020 2020 2020 2020 2077 6974 6820 7461           with ta
-0000fd00: 7266 696c 652e 5461 7246 696c 6528 6669  rfile.TarFile(fi
-0000fd10: 6c65 6f62 6a3d 746d 705f 6669 6c65 2c20  leobj=tmp_file, 
-0000fd20: 2a2a 6b77 6172 6773 2920 6173 2074 6172  **kwargs) as tar
-0000fd30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fd40: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-0000fd50: 7461 720a 0a20 2020 2020 2020 2077 6974  tar..        wit
-0000fd60: 6820 5a73 7464 5461 7252 6561 6465 7228  h ZstdTarReader(
-0000fd70: 2761 7263 6869 7665 2e74 6172 2e7a 7374  'archive.tar.zst
-0000fd80: 2729 2061 7320 7461 723a 0a20 2020 2020  ') as tar:.     
-0000fd90: 2020 2020 2020 2023 2064 6f20 736f 6d65         # do some
-0000fda0: 7468 696e 670a 0a0a 5a73 7464 2064 6963  thing...Zstd dic
-0000fdb0: 7469 6f6e 6172 7920 4944 0a3e 3e3e 3e3e  tionary ID.>>>>>
-0000fdc0: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e0a 0a2e  >>>>>>>>>>>>>...
-0000fdd0: 2e20 5f64 6963 745f 6964 3a0a 0a2e 2e20  . _dict_id:.... 
-0000fde0: 6e6f 7465 3a3a 205a 7374 6420 6469 6374  note:: Zstd dict
-0000fdf0: 696f 6e61 7279 2049 440a 0a20 2020 2044  ionary ID..    D
-0000fe00: 6963 7469 6f6e 6172 7920 4944 2069 7320  ictionary ID is 
-0000fe10: 6120 3332 2d62 6974 2075 6e73 6967 6e65  a 32-bit unsigne
-0000fe20: 6420 696e 7465 6765 7220 7661 6c75 652e  d integer value.
-0000fe30: 2044 6563 6f64 6572 2075 7365 7320 6974   Decoder uses it
-0000fe40: 2074 6f20 6368 6563 6b20 6966 2074 6865   to check if the
-0000fe50: 2063 6f72 7265 6374 2064 6963 7469 6f6e   correct diction
-0000fe60: 6172 7920 6973 2075 7365 642e 0a0a 2020  ary is used...  
-0000fe70: 2020 4163 636f 7264 696e 6720 746f 207a    According to z
-0000fe80: 7374 6420 6469 6374 696f 6e61 7279 2066  std dictionary f
-0000fe90: 6f72 6d61 7420 6073 7065 6369 6669 6361  ormat `specifica
-0000fea0: 7469 6f6e 203c 6874 7470 733a 2f2f 6769  tion <https://gi
-0000feb0: 7468 7562 2e63 6f6d 2f66 6163 6562 6f6f  thub.com/faceboo
-0000fec0: 6b2f 7a73 7464 2f62 6c6f 622f 7265 6c65  k/zstd/blob/rele
-0000fed0: 6173 652f 646f 632f 7a73 7464 5f63 6f6d  ase/doc/zstd_com
-0000fee0: 7072 6573 7369 6f6e 5f66 6f72 6d61 742e  pression_format.
-0000fef0: 6d64 2364 6963 7469 6f6e 6172 792d 666f  md#dictionary-fo
-0000ff00: 726d 6174 3e60 5f2c 2069 6620 6120 6469  rmat>`_, if a di
-0000ff10: 6374 696f 6e61 7279 2069 7320 676f 696e  ctionary is goin
-0000ff20: 6720 746f 2062 6520 6469 7374 7269 6275  g to be distribu
-0000ff30: 7465 6420 696e 2070 7562 6c69 632c 2074  ted in public, t
-0000ff40: 6865 2066 6f6c 6c6f 7769 6e67 2072 616e  he following ran
-0000ff50: 6765 7320 6172 6520 7265 7365 7276 6564  ges are reserved
-0000ff60: 2066 6f72 2066 7574 7572 6520 7265 6769   for future regi
-0000ff70: 7374 7261 7220 616e 6420 7368 616c 6c20  strar and shall 
-0000ff80: 6e6f 7420 6265 2075 7365 643a 0a0a 2020  not be used:..  
-0000ff90: 2020 2020 2020 2d20 6c6f 7720 7261 6e67        - low rang
-0000ffa0: 653a 203c 3d20 3332 3736 370a 2020 2020  e: <= 32767.    
-0000ffb0: 2020 2020 2d20 6869 6768 2072 616e 6765      - high range
-0000ffc0: 3a20 3e3d 2032 5e33 310a 0a20 2020 204f  : >= 2^31..    O
-0000ffd0: 7574 7369 6465 206f 6620 7468 6573 6520  utside of these 
-0000ffe0: 7261 6e67 6573 2c20 616e 7920 7661 6c75  ranges, any valu
-0000fff0: 6520 696e 2028 3332 3736 3720 3c20 7620  e in (32767 < v 
-00010000: 3c20 325e 3331 2920 6361 6e20 6265 2075  < 2^31) can be u
-00010010: 7365 6420 6672 6565 6c79 2c20 6576 656e  sed freely, even
-00010020: 2069 6e20 7075 626c 6963 2065 6e76 6972   in public envir
-00010030: 6f6e 6d65 6e74 2e0a 0a20 2020 2049 6e20  onment...    In 
-00010040: 7a73 7464 2066 7261 6d65 2068 6561 6465  zstd frame heade
-00010050: 722c 2074 6865 2060 4469 6374 696f 6e61  r, the `Dictiona
-00010060: 7279 5f49 4420 3c68 7474 7073 3a2f 2f67  ry_ID <https://g
-00010070: 6974 6875 622e 636f 6d2f 6661 6365 626f  ithub.com/facebo
-00010080: 6f6b 2f7a 7374 642f 626c 6f62 2f72 656c  ok/zstd/blob/rel
-00010090: 6561 7365 2f64 6f63 2f7a 7374 645f 636f  ease/doc/zstd_co
-000100a0: 6d70 7265 7373 696f 6e5f 666f 726d 6174  mpression_format
-000100b0: 2e6d 6423 6469 6374 696f 6e61 7279 5f69  .md#dictionary_i
-000100c0: 643e 605f 2066 6965 6c64 2063 616e 2062  d>`_ field can b
-000100d0: 6520 302f 312f 322f 3420 6279 7465 732e  e 0/1/2/4 bytes.
-000100e0: 2049 6620 7468 6520 7661 6c75 6520 6973   If the value is
-000100f0: 2073 6d61 6c6c 2c20 7468 6973 2063 616e   small, this can
-00010100: 2073 6176 6520 327e 3320 6279 7465 732e   save 2~3 bytes.
-00010110: 204f 7220 646f 6e27 7420 7772 6974 6520   Or don't write 
-00010120: 7468 6520 4944 2062 7920 7365 7474 696e  the ID by settin
-00010130: 6720 3a70 793a 6174 7472 3a60 4350 6172  g :py:attr:`CPar
-00010140: 616d 6574 6572 2e64 6963 7449 4446 6c61  ameter.dictIDFla
-00010150: 6760 2070 6172 616d 6574 6572 2e0a 0a20  g` parameter... 
-00010160: 2020 2070 797a 7374 6420 6d6f 6475 6c65     pyzstd module
-00010170: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-00010180: 2073 7065 6369 6679 696e 6720 4944 2077   specifying ID w
-00010190: 6865 6e20 7472 6169 6e69 6e67 2064 6963  hen training dic
-000101a0: 7469 6f6e 6172 7920 6375 7272 656e 746c  tionary currentl
-000101b0: 792e 2049 6620 7761 6e74 2074 6f20 7370  y. If want to sp
-000101c0: 6563 6966 7920 7468 6520 4944 2c20 6d6f  ecify the ID, mo
-000101d0: 6469 6679 2074 6865 2064 6963 7469 6f6e  dify the diction
-000101e0: 6172 7920 636f 6e74 656e 7420 6163 636f  ary content acco
-000101f0: 7264 696e 6720 746f 2066 6f72 6d61 7420  rding to format 
-00010200: 7370 6563 6966 6963 6174 696f 6e2c 2061  specification, a
-00010210: 6e64 2074 616b 6520 7468 6520 636f 7272  nd take the corr
-00010220: 6573 706f 6e64 696e 6720 7269 736b 732e  esponding risks.
-00010230: 0a0a 2020 2020 2a2a 4174 7465 6e74 696f  ..    **Attentio
-00010240: 6e2a 2a0a 0a20 2020 2049 6e20 3a70 793a  n**..    In :py:
-00010250: 636c 6173 733a 605a 7374 6444 6963 7460  class:`ZstdDict`
-00010260: 2063 6c61 7373 2c20 3a70 793a 6174 7472   class, :py:attr
-00010270: 3a60 5a73 7464 4469 6374 2e64 6963 745f  :`ZstdDict.dict_
-00010280: 6964 6020 6174 7472 6962 7574 6520 3d3d  id` attribute ==
-00010290: 2030 206d 6561 6e73 2074 6865 2064 6963   0 means the dic
-000102a0: 7469 6f6e 6172 7920 6973 2061 2022 7261  tionary is a "ra
-000102b0: 7720 636f 6e74 656e 7422 2064 6963 7469  w content" dicti
-000102c0: 6f6e 6172 792c 2066 7265 6520 6f66 2061  onary, free of a
-000102d0: 6e79 2066 6f72 6d61 7420 7265 7374 7269  ny format restri
-000102e0: 6374 696f 6e2c 2075 7365 6420 666f 7220  ction, used for 
-000102f0: 6164 7661 6e63 6564 2075 7365 722e 204e  advanced user. N
-00010300: 6f6e 2d7a 6572 6f20 6d65 616e 7320 6974  on-zero means it
-00010310: 2773 2061 6e20 6f72 6469 6e61 7279 2064  's an ordinary d
-00010320: 6963 7469 6f6e 6172 792c 2077 6173 2063  ictionary, was c
-00010330: 7265 6174 6564 2062 7920 7a73 7464 2066  reated by zstd f
-00010340: 756e 6374 696f 6e73 2c20 666f 6c6c 6f77  unctions, follow
-00010350: 2074 6865 2066 6f72 6d61 7420 7370 6563   the format spec
-00010360: 6966 6963 6174 696f 6e2e 0a0a 2020 2020  ification...    
-00010370: 496e 203a 7079 3a66 756e 633a 6067 6574  In :py:func:`get
-00010380: 5f66 7261 6d65 5f69 6e66 6f60 2066 756e  _frame_info` fun
-00010390: 6374 696f 6e2c 2060 6064 6963 7469 6f6e  ction, ``diction
-000103a0: 6172 795f 6964 6060 203d 3d20 3020 6d65  ary_id`` == 0 me
-000103b0: 616e 7320 6469 6374 696f 6e61 7279 2049  ans dictionary I
-000103c0: 4420 7761 7320 6e6f 7420 7265 636f 7264  D was not record
-000103d0: 6564 2069 6e20 7468 6520 6672 616d 6520  ed in the frame 
-000103e0: 6865 6164 6572 2c20 7468 6520 6672 616d  header, the fram
-000103f0: 6520 6d61 7920 6f72 206d 6179 206e 6f74  e may or may not
-00010400: 206e 6565 6420 6120 6469 6374 696f 6e61   need a dictiona
-00010410: 7279 2074 6f20 6265 2064 6563 6f64 6564  ry to be decoded
-00010420: 2c20 616e 6420 7468 6520 4944 206f 6620  , and the ID of 
-00010430: 7375 6368 2061 2064 6963 7469 6f6e 6172  such a dictionar
-00010440: 7920 6973 206e 6f74 2073 7065 6369 6669  y is not specifi
-00010450: 6564 2e0a 0a0a 4275 696c 6420 7079 7a73  ed....Build pyzs
-00010460: 7464 206d 6f64 756c 6520 7769 7468 206f  td module with o
-00010470: 7074 696f 6e73 0a3e 3e3e 3e3e 3e3e 3e3e  ptions.>>>>>>>>>
-00010480: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
-00010490: 3e3e 3e3e 3e3e 3e0a 0a2e 2e20 5f62 7569  >>>>>>>.... _bui
-000104a0: 6c64 5f70 797a 7374 643a 0a0a 2e2e 206e  ld_pyzstd:.... n
-000104b0: 6f74 653a 3a20 4275 696c 6420 7079 7a73  ote:: Build pyzs
-000104c0: 7464 206d 6f64 756c 6520 7769 7468 206f  td module with o
-000104d0: 7074 696f 6e73 0a0a 2020 2020 31ef b88f  ptions..    1...
-000104e0: e283 a320 4966 2070 726f 7669 6465 2060  ... If provide `
-000104f0: 602d 2d61 7678 3260 6020 6275 696c 6420  `--avx2`` build 
-00010500: 6f70 7469 6f6e 2c20 6974 2077 696c 6c20  option, it will 
-00010510: 6275 696c 6420 7769 7468 2041 5658 322f  build with AVX2/
-00010520: 424d 4932 2069 6e73 7472 7563 7469 6f6e  BMI2 instruction
-00010530: 732e 2049 6e20 4d53 5643 2062 7569 6c64  s. In MSVC build
-00010540: 2028 7374 6174 6963 206c 696e 6b29 2c20   (static link), 
-00010550: 7468 6973 2062 7269 6e67 7320 736f 6d65  this brings some
-00010560: 2070 6572 666f 726d 616e 6365 2069 6d70   performance imp
-00010570: 726f 7665 6d65 6e74 732e 2049 6e20 4743  rovements. In GC
-00010580: 432f 434c 414e 4720 6275 696c 6473 2c20  C/CLANG builds, 
-00010590: 6e6f 2073 6967 6e69 6669 6361 6e74 2069  no significant i
-000105a0: 6d70 726f 7665 6d65 6e74 2c20 6f72 2077  mprovement, or w
-000105b0: 6f72 7365 2e0a 0a20 2020 202e 2e20 736f  orse...    .. so
-000105c0: 7572 6365 636f 6465 3a3a 2073 6865 6c6c  urcecode:: shell
-000105d0: 0a0a 2020 2020 2020 2020 2320 f09f 9fa0  ..        # ....
-000105e0: 2070 797a 7374 6420 302e 3135 2e34 2b20   pyzstd 0.15.4+ 
-000105f0: 616e 6420 7069 7020 3232 2e31 2b20 7375  and pip 22.1+ su
-00010600: 7070 6f72 7420 5045 502d 3531 373a 0a20  pport PEP-517:. 
-00010610: 2020 2020 2020 2023 2062 7569 6c64 2061         # build a
-00010620: 6e64 2069 6e73 7461 6c6c 0a20 2020 2020  nd install.     
-00010630: 2020 2070 6970 2069 6e73 7461 6c6c 202d     pip install -
-00010640: 2d63 6f6e 6669 672d 7365 7474 696e 6773  -config-settings
-00010650: 3d22 2d2d 6275 696c 642d 6f70 7469 6f6e  ="--build-option
-00010660: 3d2d 2d61 7678 3222 202d 7620 7079 7a73  =--avx2" -v pyzs
-00010670: 7464 2d30 2e31 352e 342e 7461 722e 677a  td-0.15.4.tar.gz
-00010680: 0a20 2020 2020 2020 2023 2062 7569 6c64  .        # build
-00010690: 2061 2072 6564 6973 7472 6962 7574 6162   a redistributab
-000106a0: 6c65 2077 6865 656c 0a20 2020 2020 2020  le wheel.       
-000106b0: 2070 6970 2077 6865 656c 202d 2d63 6f6e   pip wheel --con
-000106c0: 6669 672d 7365 7474 696e 6773 3d22 2d2d  fig-settings="--
-000106d0: 6275 696c 642d 6f70 7469 6f6e 3d2d 2d61  build-option=--a
-000106e0: 7678 3222 202d 7620 7079 7a73 7464 2d30  vx2" -v pyzstd-0
-000106f0: 2e31 352e 342e 7461 722e 677a 0a20 2020  .15.4.tar.gz.   
-00010700: 2020 2020 2023 20f0 9f9f a020 6c65 6761       # .... lega
-00010710: 6379 2063 6f6d 6d61 6e64 733a 0a20 2020  cy commands:.   
-00010720: 2020 2020 2023 2062 7569 6c64 2061 6e64       # build and
-00010730: 2069 6e73 7461 6c6c 0a20 2020 2020 2020   install.       
-00010740: 2070 7974 686f 6e20 7365 7475 702e 7079   python setup.py
-00010750: 2069 6e73 7461 6c6c 202d 2d61 7678 320a   install --avx2.
-00010760: 2020 2020 2020 2020 2320 6275 696c 6420          # build 
-00010770: 6120 7265 6469 7374 7269 6275 7461 626c  a redistributabl
-00010780: 6520 7768 6565 6c0a 2020 2020 2020 2020  e wheel.        
-00010790: 7079 7468 6f6e 2073 6574 7570 2e70 7920  python setup.py 
-000107a0: 6264 6973 745f 7768 6565 6c20 2d2d 6176  bdist_wheel --av
-000107b0: 7832 0a0a 2020 2020 32ef b88f e283 a320  x2..    2...... 
-000107c0: 5079 7a73 7464 206d 6f64 756c 6520 7375  Pyzstd module su
-000107d0: 7070 6f72 7473 3a0a 0a20 2020 2020 2020  pports:..       
-000107e0: 202a 2044 796e 616d 6963 616c 6c79 206c   * Dynamically l
-000107f0: 696e 6b20 746f 207a 7374 6420 6c69 6272  ink to zstd libr
-00010800: 6172 7920 2870 726f 7669 6465 6420 6279  ary (provided by
-00010810: 2073 7973 7465 6d20 6f72 2061 2044 4c4c   system or a DLL
-00010820: 206c 6962 7261 7279 292c 2074 6865 6e20   library), then 
-00010830: 7468 6520 7a73 7464 2073 6f75 7263 6520  the zstd source 
-00010840: 636f 6465 2069 6e20 6060 7a73 7464 6060  code in ``zstd``
-00010850: 2066 6f6c 6465 7220 7769 6c6c 2062 6520   folder will be 
-00010860: 6967 6e6f 7265 642e 0a20 2020 2020 2020  ignored..       
-00010870: 202a 2050 726f 7669 6465 2061 2060 4346   * Provide a `CF
-00010880: 4649 203c 6874 7470 733a 2f2f 646f 632e  FI <https://doc.
-00010890: 7079 7079 2e6f 7267 2f65 6e2f 6c61 7465  pypy.org/en/late
-000108a0: 7374 2f65 7874 656e 6469 6e67 2e68 746d  st/extending.htm
-000108b0: 6c23 6366 6669 3e60 5f20 696d 706c 656d  l#cffi>`_ implem
-000108c0: 656e 7461 7469 6f6e 2074 6861 7420 6361  entation that ca
-000108d0: 6e20 776f 726b 2077 6974 6820 5079 5079  n work with PyPy
-000108e0: 2e0a 0a20 2020 204f 6e20 4350 7974 686f  ...    On CPytho
-000108f0: 6e2c 2070 726f 7669 6465 2074 6865 7365  n, provide these
-00010900: 2062 7569 6c64 206f 7074 696f 6e73 3a0a   build options:.
-00010910: 0a20 2020 2020 2020 2023 2e20 6e6f 206f  .        #. no o
-00010920: 7074 696f 6e3a 2043 2069 6d70 6c65 6d65  ption: C impleme
-00010930: 6e74 6174 696f 6e2c 2073 7461 7469 6361  ntation, statica
-00010940: 6c6c 7920 6c69 6e6b 2074 6f20 7a73 7464  lly link to zstd
-00010950: 206c 6962 7261 7279 2e0a 2020 2020 2020   library..      
-00010960: 2020 232e 2060 602d 2d64 796e 616d 6963    #. ``--dynamic
-00010970: 2d6c 696e 6b2d 7a73 7464 6060 3a20 4320  -link-zstd``: C 
-00010980: 696d 706c 656d 656e 7461 7469 6f6e 2c20  implementation, 
-00010990: 6479 6e61 6d69 6361 6c6c 7920 6c69 6e6b  dynamically link
-000109a0: 2074 6f20 7a73 7464 206c 6962 7261 7279   to zstd library
-000109b0: 2e0a 2020 2020 2020 2020 232e 2060 602d  ..        #. ``-
-000109c0: 2d63 6666 6960 603a 2043 4646 4920 696d  -cffi``: CFFI im
-000109d0: 706c 656d 656e 7461 7469 6f6e 2028 736c  plementation (sl
-000109e0: 6f77 6572 292c 2073 7461 7469 6361 6c6c  ower), staticall
-000109f0: 7920 6c69 6e6b 2074 6f20 7a73 7464 206c  y link to zstd l
-00010a00: 6962 7261 7279 2e0a 2020 2020 2020 2020  ibrary..        
-00010a10: 232e 2060 602d 2d63 6666 6920 2d2d 6479  #. ``--cffi --dy
-00010a20: 6e61 6d69 632d 6c69 6e6b 2d7a 7374 6460  namic-link-zstd`
-00010a30: 603a 2043 4646 4920 696d 706c 656d 656e  `: CFFI implemen
-00010a40: 7461 7469 6f6e 2028 736c 6f77 6572 292c  tation (slower),
-00010a50: 2064 796e 616d 6963 616c 6c79 206c 696e   dynamically lin
-00010a60: 6b20 746f 207a 7374 6420 6c69 6272 6172  k to zstd librar
-00010a70: 792e 0a0a 2020 2020 4f6e 2050 7950 792c  y...    On PyPy,
-00010a80: 206f 6e6c 7920 4346 4649 2069 6d70 6c65   only CFFI imple
-00010a90: 6d65 6e74 6174 696f 6e20 6361 6e20 6265  mentation can be
-00010aa0: 2075 7365 642c 2073 6f20 6060 2d2d 6366   used, so ``--cf
-00010ab0: 6669 6060 2069 7320 6164 6465 6420 696d  fi`` is added im
-00010ac0: 706c 6963 6974 6c79 2e20 6060 2d2d 6479  plicitly. ``--dy
-00010ad0: 6e61 6d69 632d 6c69 6e6b 2d7a 7374 6460  namic-link-zstd`
-00010ae0: 6020 6973 206f 7074 696f 6e61 6c2e 0a0a  ` is optional...
-00010af0: 2020 2020 2e2e 2073 6f75 7263 6563 6f64      .. sourcecod
-00010b00: 653a 3a20 7368 656c 6c0a 0a20 2020 2020  e:: shell..     
-00010b10: 2020 2023 20f0 9f9f a020 7079 7a73 7464     # .... pyzstd
-00010b20: 2030 2e31 352e 342b 2061 6e64 2070 6970   0.15.4+ and pip
-00010b30: 2032 322e 312b 2073 7570 706f 7274 2050   22.1+ support P
-00010b40: 4550 2d35 3137 3a0a 2020 2020 2020 2020  EP-517:.        
-00010b50: 2320 6275 696c 6420 616e 6420 696e 7374  # build and inst
-00010b60: 616c 6c0a 2020 2020 2020 2020 7069 7033  all.        pip3
-00010b70: 2069 6e73 7461 6c6c 202d 2d63 6f6e 6669   install --confi
-00010b80: 672d 7365 7474 696e 6773 3d22 2d2d 6275  g-settings="--bu
-00010b90: 696c 642d 6f70 7469 6f6e 3d2d 2d64 796e  ild-option=--dyn
-00010ba0: 616d 6963 2d6c 696e 6b2d 7a73 7464 2220  amic-link-zstd" 
-00010bb0: 2d76 2070 797a 7374 642d 302e 3135 2e34  -v pyzstd-0.15.4
-00010bc0: 2e74 6172 2e67 7a0a 2020 2020 2020 2020  .tar.gz.        
-00010bd0: 2320 6275 696c 6420 6120 7265 6469 7374  # build a redist
-00010be0: 7269 6275 7461 626c 6520 7768 6565 6c0a  ributable wheel.
-00010bf0: 2020 2020 2020 2020 7069 7033 2077 6865          pip3 whe
-00010c00: 656c 202d 2d63 6f6e 6669 672d 7365 7474  el --config-sett
-00010c10: 696e 6773 3d22 2d2d 6275 696c 642d 6f70  ings="--build-op
-00010c20: 7469 6f6e 3d2d 2d64 796e 616d 6963 2d6c  tion=--dynamic-l
-00010c30: 696e 6b2d 7a73 7464 2220 2d76 2070 797a  ink-zstd" -v pyz
-00010c40: 7374 642d 302e 3135 2e34 2e74 6172 2e67  std-0.15.4.tar.g
-00010c50: 7a0a 2020 2020 2020 2020 2320 7370 6563  z.        # spec
-00010c60: 6966 7920 6d6f 7265 2074 6861 6e20 6f6e  ify more than on
-00010c70: 6520 6f70 7469 6f6e 0a20 2020 2020 2020  e option.       
-00010c80: 2070 6970 3320 7768 6565 6c20 2d2d 636f   pip3 wheel --co
-00010c90: 6e66 6967 2d73 6574 7469 6e67 733d 222d  nfig-settings="-
-00010ca0: 2d62 7569 6c64 2d6f 7074 696f 6e3d 2d2d  -build-option=--
-00010cb0: 6479 6e61 6d69 632d 6c69 6e6b 2d7a 7374  dynamic-link-zst
-00010cc0: 6420 2d2d 6366 6669 2220 2d76 2070 797a  d --cffi" -v pyz
-00010cd0: 7374 642d 302e 3135 2e34 2e74 6172 2e67  std-0.15.4.tar.g
-00010ce0: 7a0a 2020 2020 2020 2020 2320 f09f 9fa0  z.        # ....
-00010cf0: 206c 6567 6163 7920 636f 6d6d 616e 6473   legacy commands
-00010d00: 3a0a 2020 2020 2020 2020 2320 6275 696c  :.        # buil
-00010d10: 6420 616e 6420 696e 7374 616c 6c0a 2020  d and install.  
-00010d20: 2020 2020 2020 7079 7468 6f6e 3320 7365        python3 se
-00010d30: 7475 702e 7079 2069 6e73 7461 6c6c 202d  tup.py install -
-00010d40: 2d64 796e 616d 6963 2d6c 696e 6b2d 7a73  -dynamic-link-zs
-00010d50: 7464 0a20 2020 2020 2020 2023 2062 7569  td.        # bui
-00010d60: 6c64 2061 2072 6564 6973 7472 6962 7574  ld a redistribut
-00010d70: 6162 6c65 2077 6865 656c 0a20 2020 2020  able wheel.     
-00010d80: 2020 2070 7974 686f 6e33 2073 6574 7570     python3 setup
-00010d90: 2e70 7920 6264 6973 745f 7768 6565 6c20  .py bdist_wheel 
-00010da0: 2d2d 6479 6e61 6d69 632d 6c69 6e6b 2d7a  --dynamic-link-z
-00010db0: 7374 640a 0a20 2020 2053 6f6d 6520 6e6f  std..    Some no
-00010dc0: 7465 733a 0a0a 2020 2020 2020 2020 2a20  tes:..        * 
-00010dd0: 5468 6520 7768 6565 6c73 206f 6e20 6050  The wheels on `P
-00010de0: 7950 4920 3c68 7474 7073 3a2f 2f70 7970  yPI <https://pyp
-00010df0: 692e 6f72 672f 7072 6f6a 6563 742f 7079  i.org/project/py
-00010e00: 7a73 7464 3e60 5f20 7573 6520 7374 6174  zstd>`_ use stat
-00010e10: 6963 206c 696e 6b69 6e67 2c20 7468 6520  ic linking, the 
-00010e20: 7061 636b 6167 6573 206f 6e20 6041 6e61  packages on `Ana
-00010e30: 636f 6e64 6120 3c68 7474 7073 3a2f 2f61  conda <https://a
-00010e40: 6e61 636f 6e64 612e 6f72 672f 636f 6e64  naconda.org/cond
-00010e50: 612d 666f 7267 652f 7079 7a73 7464 3e60  a-forge/pyzstd>`
-00010e60: 5f20 7573 6520 6479 6e61 6d69 6320 6c69  _ use dynamic li
-00010e70: 6e6b 696e 672e 0a20 2020 2020 2020 202a  nking..        *
-00010e80: 204e 6f20 6d61 7474 6572 2073 7461 7469   No matter stati
-00010e90: 6320 6f72 2064 796e 616d 6963 206c 696e  c or dynamic lin
-00010ea0: 6b69 6e67 2c20 7079 7a73 7464 206d 6f64  king, pyzstd mod
-00010eb0: 756c 6520 7265 7175 6972 6573 207a 7374  ule requires zst
-00010ec0: 6420 7631 2e34 2e30 2b2e 0a20 2020 2020  d v1.4.0+..     
-00010ed0: 2020 202a 2053 7461 7469 6320 6c69 6e6b     * Static link
-00010ee0: 696e 673a 2055 7365 207a 7374 6427 7320  ing: Use zstd's 
-00010ef0: 6f66 6669 6369 616c 2072 656c 6561 7365  official release
-00010f00: 2077 6974 686f 7574 2061 6e79 2063 6861   without any cha
-00010f10: 6e67 652e 2049 6620 7761 6e74 2074 6f20  nge. If want to 
-00010f20: 7570 6772 6164 6520 6f72 2064 6f77 6e67  upgrade or downg
-00010f30: 7261 6465 2074 6865 207a 7374 6420 6c69  rade the zstd li
-00010f40: 6272 6172 792c 206a 7573 7420 7265 706c  brary, just repl
-00010f50: 6163 6520 6060 7a73 7464 6060 2066 6f6c  ace ``zstd`` fol
-00010f60: 6465 722e 0a20 2020 2020 2020 202a 2044  der..        * D
-00010f70: 796e 616d 6963 206c 696e 6b69 6e67 3a20  ynamic linking: 
-00010f80: 4966 206e 6577 207a 7374 6420 4150 4920  If new zstd API 
-00010f90: 6973 2075 7365 6420 6174 2063 6f6d 7069  is used at compi
-00010fa0: 6c65 2d74 696d 652c 206c 696e 6b69 6e67  le-time, linking
-00010fb0: 2074 6f20 6c6f 7765 7220 7665 7273 696f   to lower versio
-00010fc0: 6e20 7275 6e2d 7469 6d65 207a 7374 6420  n run-time zstd 
-00010fd0: 6c69 6272 6172 7920 7769 6c6c 2066 6169  library will fai
-00010fe0: 6c2e 2055 7365 2076 312e 352e 3020 6e65  l. Use v1.5.0 ne
-00010ff0: 7720 4150 4920 6966 2070 6f73 7369 626c  w API if possibl
-00011000: 652e 0a0a 2020 2020 4f6e 2057 696e 646f  e...    On Windo
-00011010: 7773 2c20 7468 6572 6520 6973 206e 6f20  ws, there is no 
-00011020: 7379 7374 656d 2d77 6964 6520 7a73 7464  system-wide zstd
-00011030: 206c 6962 7261 7279 2e20 5079 7a73 7464   library. Pyzstd
-00011040: 206d 6f64 756c 6520 6361 6e20 6479 6e61   module can dyna
-00011050: 6d69 6361 6c6c 7920 6c69 6e6b 2074 6f20  mically link to 
-00011060: 6120 444c 4c20 6c69 6272 6172 792c 206d  a DLL library, m
-00011070: 6f64 6966 7920 6060 7365 7475 702e 7079  odify ``setup.py
-00011080: 6060 3a0a 0a20 2020 202e 2e20 736f 7572  ``:..    .. sour
-00011090: 6365 636f 6465 3a3a 2070 7974 686f 6e0a  cecode:: python.
-000110a0: 0a20 2020 2020 2020 2023 2045 3a5c 7a73  .        # E:\zs
-000110b0: 7464 5f64 6c6c 2066 6f6c 6465 7220 6861  td_dll folder ha
-000110c0: 7320 7a73 7464 2e68 202f 207a 6469 6374  s zstd.h / zdict
-000110d0: 2e68 202f 206c 6962 7a73 7464 2e6c 6962  .h / libzstd.lib
-000110e0: 2074 6861 740a 2020 2020 2020 2020 2320   that.        # 
-000110f0: 616c 6f6e 6720 7769 7468 206c 6962 7a73  along with libzs
-00011100: 7464 2e64 6c6c 0a20 2020 2020 2020 2069  td.dll.        i
-00011110: 6620 4459 4e41 4d49 435f 4c49 4e4b 3a0a  f DYNAMIC_LINK:.
-00011120: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-00011130: 6773 203d 207b 0a20 2020 2020 2020 2020  gs = {.         
-00011140: 2020 2027 696e 636c 7564 655f 6469 7273     'include_dirs
-00011150: 273a 205b 2745 3a5c 7a73 7464 5f64 6c6c  ': ['E:\zstd_dll
-00011160: 275d 2c20 2320 2e68 2064 6972 6563 746f  '], # .h directo
-00011170: 7279 0a20 2020 2020 2020 2020 2020 2027  ry.            '
-00011180: 6c69 6272 6172 795f 6469 7273 273a 205b  library_dirs': [
-00011190: 2745 3a5c 7a73 7464 5f64 6c6c 275d 2c20  'E:\zstd_dll'], 
-000111a0: 2320 2e6c 6962 2064 6972 6563 746f 7279  # .lib directory
-000111b0: 0a20 2020 2020 2020 2020 2020 2027 6c69  .            'li
-000111c0: 6272 6172 6965 7327 3a20 5b27 6c69 627a  braries': ['libz
-000111d0: 7374 6427 5d2c 2020 2020 2020 2020 2320  std'],        # 
-000111e0: 6c69 6220 6e61 6d65 2c20 6e6f 7420 6669  lib name, not fi
-000111f0: 6c65 6e61 6d65 2c20 666f 7220 7468 6520  lename, for the 
-00011200: 6c69 6e6b 6572 2e0a 2020 2020 2020 2020  linker..        
-00011210: 2020 2020 2e2e 2e0a 0a20 2020 2041 6e64      .....    And
-00011220: 2070 7574 2060 606c 6962 7a73 7464 2e64   put ``libzstd.d
-00011230: 6c6c 6060 2069 6e74 6f20 6f6e 6520 6f66  ll`` into one of
-00011240: 2074 6865 7365 2064 6972 6563 746f 7269   these directori
-00011250: 6573 3a0a 0a20 2020 2020 2020 202a 2044  es:..        * D
-00011260: 6972 6563 746f 7279 2061 6464 6564 2062  irectory added b
-00011270: 7920 606f 732e 6164 645f 646c 6c5f 6469  y `os.add_dll_di
-00011280: 7265 6374 6f72 7928 2920 3c68 7474 7073  rectory() <https
-00011290: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-000112a0: 7267 2f33 2f6c 6962 7261 7279 2f6f 732e  rg/3/library/os.
-000112b0: 6874 6d6c 236f 732e 6164 645f 646c 6c5f  html#os.add_dll_
-000112c0: 6469 7265 6374 6f72 793e 605f 2066 756e  directory>`_ fun
-000112d0: 6374 696f 6e2e 0a20 2020 2020 2020 202a  ction..        *
-000112e0: 2050 7974 686f 6e27 7320 726f 6f74 2064   Python's root d
-000112f0: 6972 6563 746f 7279 2074 6861 7420 6861  irectory that ha
-00011300: 7320 7079 7468 6f6e 2e65 7865 2e0a 2020  s python.exe..  
-00011310: 2020 2020 2020 2a20 2553 7973 7465 6d52        * %SystemR
-00011320: 6f6f 7425 5c53 7973 7465 6d33 320a 0a20  oot%\System32.. 
-00011330: 2020 204e 6f74 6520 7468 6174 2074 6865     Note that the
-00011340: 2061 626f 7665 206c 6973 7420 646f 6573   above list does
-00011350: 6e27 7420 696e 636c 7564 6520 7468 6520  n't include the 
-00011360: 6375 7272 656e 7420 776f 726b 696e 6720  current working 
-00011370: 6469 7265 6374 6f72 7920 616e 6420 2550  directory and %P
-00011380: 4154 4825 2064 6972 6563 746f 7269 6573  ATH% directories
-00011390: 2e0a 0a20 2020 2033 efb8 8fe2 83a3 2055  ...    3...... U
-000113a0: 7365 2022 6d75 6c74 692d 7068 6173 6520  se "multi-phase 
-000113b0: 696e 6974 6961 6c69 7a61 7469 6f6e 2220  initialization" 
-000113c0: 6f6e 2043 5079 7468 6f6e 2e0a 0a20 2020  on CPython...   
-000113d0: 2049 6620 7072 6f76 6964 6520 6060 2d2d   If provide ``--
-000113e0: 6d75 6c74 692d 7068 6173 652d 696e 6974  multi-phase-init
-000113f0: 6060 2062 7569 6c64 206f 7074 696f 6e2c  `` build option,
-00011400: 2069 7420 7769 6c6c 2062 7569 6c64 2077   it will build w
-00011410: 6974 6820 226d 756c 7469 2d70 6861 7365  ith "multi-phase
-00011420: 2069 6e69 7469 616c 697a 6174 696f 6e22   initialization"
-00011430: 2028 6050 4550 2d34 3839 203c 6874 7470   (`PEP-489 <http
-00011440: 733a 2f2f 7065 7073 2e70 7974 686f 6e2e  s://peps.python.
-00011450: 6f72 672f 7065 702d 3034 3839 2f3e 605f  org/pep-0489/>`_
-00011460: 2920 6f6e 2043 5079 7468 6f6e 2033 2e31  ) on CPython 3.1
-00011470: 312b 2e0a 0a20 2020 2053 696e 6365 2069  1+...    Since i
-00011480: 7420 6164 6473 2061 2074 696e 7920 6f76  t adds a tiny ov
-00011490: 6572 6865 6164 2c20 6974 2773 2064 6973  erhead, it's dis
-000114a0: 6162 6c65 6420 6279 2064 6566 6175 6c74  abled by default
-000114b0: 2e20 4974 2063 616e 2062 6520 656e 6162  . It can be enab
-000114c0: 6c65 6420 6166 7465 7220 4350 7974 686f  led after CPytho
-000114d0: 6e27 7320 6073 7562 2d69 6e74 6572 7072  n's `sub-interpr
-000114e0: 6574 6572 7320 3c68 7474 7073 3a2f 2f70  eters <https://p
-000114f0: 6570 732e 7079 7468 6f6e 2e6f 7267 2f70  eps.python.org/p
-00011500: 6570 2d30 3535 342f 3e60 5f20 6973 206d  ep-0554/>`_ is m
-00011510: 6174 7572 652e 0a                        ature..
+0000e7f0: 7465 722e 7374 7261 7465 6779 203a 2053  ter.strategy : S
+0000e800: 7472 6174 6567 792e 6c61 7a79 322c 0a20  trategy.lazy2,. 
+0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e820: 2043 5061 7261 6d65 7465 722e 6368 6563   CParameter.chec
+0000e830: 6b73 756d 466c 6167 203a 2031 7d0a 2020  ksumFlag : 1}.  
+0000e840: 2020 2020 2020 636f 6d70 7265 7373 6564        compressed
+0000e850: 5f64 6174 203d 2063 6f6d 7072 6573 7328  _dat = compress(
+0000e860: 7261 775f 6461 742c 206f 7074 696f 6e29  raw_dat, option)
+0000e870: 0a0a 0a49 6e66 6f72 6d61 7469 7665 206e  ...Informative n
+0000e880: 6f74 6573 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  otes.-----------
+0000e890: 2d2d 2d2d 2d2d 0a0a 436f 6d70 7265 7373  ------..Compress
+0000e8a0: 696f 6e20 6c65 7665 6c0a 3e3e 3e3e 3e3e  ion level.>>>>>>
+0000e8b0: 3e3e 3e3e 3e3e 3e3e 3e3e 3e0a 0a2e 2e20  >>>>>>>>>>>.... 
+0000e8c0: 5f63 6f6d 7072 6573 7369 6f6e 5f6c 6576  _compression_lev
+0000e8d0: 656c 3a0a 0a2e 2e20 6e6f 7465 3a3a 2043  el:.... note:: C
+0000e8e0: 6f6d 7072 6573 7369 6f6e 206c 6576 656c  ompression level
+0000e8f0: 0a0a 2020 2020 436f 6d70 7265 7373 696f  ..    Compressio
+0000e900: 6e20 6c65 7665 6c20 6973 2061 6e20 696e  n level is an in
+0000e910: 7465 6765 723a 0a0a 2020 2020 2a20 6060  teger:..    * ``
+0000e920: 3160 6020 746f 2060 6032 3260 6020 2863  1`` to ``22`` (c
+0000e930: 7572 7265 6e74 6c79 292c 2072 6567 756c  urrently), regul
+0000e940: 6172 206c 6576 656c 732e 204c 6576 656c  ar levels. Level
+0000e950: 7320 3e3d 2032 302c 206c 6162 656c 6564  s >= 20, labeled
+0000e960: 202a 756c 7472 612a 2c20 7368 6f75 6c64   *ultra*, should
+0000e970: 2062 6520 7573 6564 2077 6974 6820 6361   be used with ca
+0000e980: 7574 696f 6e2c 2061 7320 7468 6579 2072  ution, as they r
+0000e990: 6571 7569 7265 206d 6f72 6520 6d65 6d6f  equire more memo
+0000e9a0: 7279 2e0a 2020 2020 2a20 6060 3060 6020  ry..    * ``0`` 
+0000e9b0: 6d65 616e 7320 7573 6520 7468 6520 6465  means use the de
+0000e9c0: 6661 756c 7420 6c65 7665 6c2c 2077 6869  fault level, whi
+0000e9d0: 6368 2069 7320 6375 7272 656e 746c 7920  ch is currently 
+0000e9e0: 6060 3360 6020 6465 6669 6e65 6420 6279  ``3`` defined by
+0000e9f0: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
+0000ea00: 7a73 7464 206c 6962 7261 7279 2e0a 2020  zstd library..  
+0000ea10: 2020 2a20 6060 2d31 3331 3037 3260 6020    * ``-131072`` 
+0000ea20: 746f 2060 602d 3160 602c 206e 6567 6174  to ``-1``, negat
+0000ea30: 6976 6520 6c65 7665 6c73 2065 7874 656e  ive levels exten
+0000ea40: 6420 7468 6520 7261 6e67 6520 6f66 2073  d the range of s
+0000ea50: 7065 6564 2076 7320 7261 7469 6f20 7072  peed vs ratio pr
+0000ea60: 6566 6572 656e 6365 732e 2054 6865 206c  eferences. The l
+0000ea70: 6f77 6572 2074 6865 206c 6576 656c 2c20  ower the level, 
+0000ea80: 7468 6520 6661 7374 6572 2074 6865 2073  the faster the s
+0000ea90: 7065 6564 2c20 6275 7420 6174 2074 6865  peed, but at the
+0000eaa0: 2063 6f73 7420 6f66 2063 6f6d 7072 6573   cost of compres
+0000eab0: 7369 6f6e 2072 6174 696f 2e20 3133 3130  sion ratio. 1310
+0000eac0: 3732 203d 2031 3238 2a31 3032 342e 0a0a  72 = 128*1024...
+0000ead0: 2020 2020 3a70 793a 6461 7461 3a60 636f      :py:data:`co
+0000eae0: 6d70 7265 7373 696f 6e4c 6576 656c 5f76  mpressionLevel_v
+0000eaf0: 616c 7565 7360 2061 7265 2073 6f6d 6520  alues` are some 
+0000eb00: 7661 6c75 6573 2064 6566 696e 6564 2062  values defined b
+0000eb10: 7920 7468 6520 756e 6465 726c 7969 6e67  y the underlying
+0000eb20: 207a 7374 6420 6c69 6272 6172 792e 0a0a   zstd library...
+0000eb30: 2020 2020 2a2a 466f 7220 6164 7661 6e63      **For advanc
+0000eb40: 6564 2075 7365 722a 2a0a 0a20 2020 2043  ed user**..    C
+0000eb50: 6f6d 7072 6573 7369 6f6e 206c 6576 656c  ompression level
+0000eb60: 7320 6172 6520 6a75 7374 206e 756d 6265  s are just numbe
+0000eb70: 7273 2074 6861 7420 6d61 7020 746f 2061  rs that map to a
+0000eb80: 2073 6574 206f 6620 636f 6d70 7265 7373   set of compress
+0000eb90: 696f 6e20 7061 7261 6d65 7465 7273 2c20  ion parameters, 
+0000eba0: 7365 6520 6074 6869 7320 7461 626c 6520  see `this table 
+0000ebb0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+0000ebc0: 636f 6d2f 6661 6365 626f 6f6b 2f7a 7374  com/facebook/zst
+0000ebd0: 642f 626c 6f62 2f72 656c 6561 7365 2f6c  d/blob/release/l
+0000ebe0: 6962 2f63 6f6d 7072 6573 732f 636c 6576  ib/compress/clev
+0000ebf0: 656c 732e 683e 605f 2066 6f72 206f 7665  els.h>`_ for ove
+0000ec00: 7276 6965 772e 2054 6865 2070 6172 616d  rview. The param
+0000ec10: 6574 6572 7320 6d61 7920 6265 2061 646a  eters may be adj
+0000ec20: 7573 7465 6420 6279 2074 6865 2075 6e64  usted by the und
+0000ec30: 6572 6c79 696e 6720 7a73 7464 206c 6962  erlying zstd lib
+0000ec40: 7261 7279 2061 6674 6572 2067 6174 6865  rary after gathe
+0000ec50: 7269 6e67 2073 6f6d 6520 696e 666f 726d  ring some inform
+0000ec60: 6174 696f 6e2c 2073 7563 6820 6173 2064  ation, such as d
+0000ec70: 6174 6120 7369 7a65 2c20 7573 696e 6720  ata size, using 
+0000ec80: 6469 6374 696f 6e61 7279 206f 7220 6e6f  dictionary or no
+0000ec90: 742e 0a0a 2020 2020 5365 7474 696e 6720  t...    Setting 
+0000eca0: 6120 636f 6d70 7265 7373 696f 6e20 6c65  a compression le
+0000ecb0: 7665 6c20 646f 6573 206e 6f74 2073 6574  vel does not set
+0000ecc0: 2061 6c6c 206f 7468 6572 203a 7265 663a   all other :ref:
+0000ecd0: 6063 6f6d 7072 6573 7369 6f6e 2070 6172  `compression par
+0000ece0: 616d 6574 6572 733c 4350 6172 616d 6574  ameters<CParamet
+0000ecf0: 6572 3e60 2074 6f20 6465 6661 756c 742e  er>` to default.
+0000ed00: 2053 6574 7469 6e67 2074 6869 7320 7769   Setting this wi
+0000ed10: 6c6c 2064 796e 616d 6963 616c 6c79 2069  ll dynamically i
+0000ed20: 6d70 6163 7420 7468 6520 636f 6d70 7265  mpact the compre
+0000ed30: 7373 696f 6e20 7061 7261 6d65 7465 7273  ssion parameters
+0000ed40: 2077 6869 6368 2068 6176 6520 6e6f 7420   which have not 
+0000ed50: 6265 656e 206d 616e 7561 6c6c 7920 7365  been manually se
+0000ed60: 742c 2074 6865 206d 616e 7561 6c6c 7920  t, the manually 
+0000ed70: 7365 7420 6f6e 6573 2077 696c 6c20 2273  set ones will "s
+0000ed80: 7469 636b 222e 0a0a 0a46 7261 6d65 2061  tick"....Frame a
+0000ed90: 6e64 2062 6c6f 636b 0a3e 3e3e 3e3e 3e3e  nd block.>>>>>>>
+0000eda0: 3e3e 3e3e 3e3e 3e3e 0a0a 2e2e 205f 6672  >>>>>>>>.... _fr
+0000edb0: 616d 655f 626c 6f63 6b3a 0a0a 2e2e 206e  ame_block:.... n
+0000edc0: 6f74 653a 3a20 4672 616d 6520 616e 6420  ote:: Frame and 
+0000edd0: 626c 6f63 6b0a 0a20 2020 202a 2a46 7261  block..    **Fra
+0000ede0: 6d65 2a2a 0a0a 2020 2020 5a73 7464 2064  me**..    Zstd d
+0000edf0: 6174 6120 636f 6e73 6973 7473 206f 6620  ata consists of 
+0000ee00: 6f6e 6520 6f72 206d 6f72 6520 696e 6465  one or more inde
+0000ee10: 7065 6e64 656e 7420 2266 7261 6d65 7322  pendent "frames"
+0000ee20: 2e20 5468 6520 6465 636f 6d70 7265 7373  . The decompress
+0000ee30: 6564 2063 6f6e 7465 6e74 206f 6620 6d75  ed content of mu
+0000ee40: 6c74 6970 6c65 2063 6f6e 6361 7465 6e61  ltiple concatena
+0000ee50: 7465 6420 6672 616d 6573 2069 7320 7468  ted frames is th
+0000ee60: 6520 636f 6e63 6174 656e 6174 696f 6e20  e concatenation 
+0000ee70: 6f66 2065 6163 6820 6672 616d 6520 6465  of each frame de
+0000ee80: 636f 6d70 7265 7373 6564 2063 6f6e 7465  compressed conte
+0000ee90: 6e74 2e0a 0a20 2020 2041 2066 7261 6d65  nt...    A frame
+0000eea0: 2069 7320 636f 6d70 6c65 7465 6c79 2069   is completely i
+0000eeb0: 6e64 6570 656e 6465 6e74 2c20 6861 7320  ndependent, has 
+0000eec0: 6120 6672 616d 6520 6865 6164 6572 2c20  a frame header, 
+0000eed0: 616e 6420 6120 7365 7420 6f66 2070 6172  and a set of par
+0000eee0: 616d 6574 6572 7320 7768 6963 6820 7465  ameters which te
+0000eef0: 6c6c 7320 7468 6520 6465 636f 6465 7220  lls the decoder 
+0000ef00: 686f 7720 746f 2064 6563 6f6d 7072 6573  how to decompres
+0000ef10: 7320 6974 2e0a 0a20 2020 2049 6e20 6164  s it...    In ad
+0000ef20: 6469 7469 6f6e 2074 6f20 6e6f 726d 616c  dition to normal
+0000ef30: 2066 7261 6d65 2c20 7468 6572 6520 6973   frame, there is
+0000ef40: 2060 736b 6970 7061 626c 6520 6672 616d   `skippable fram
+0000ef50: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
+0000ef60: 622e 636f 6d2f 6661 6365 626f 6f6b 2f7a  b.com/facebook/z
+0000ef70: 7374 642f 626c 6f62 2f72 656c 6561 7365  std/blob/release
+0000ef80: 2f64 6f63 2f7a 7374 645f 636f 6d70 7265  /doc/zstd_compre
+0000ef90: 7373 696f 6e5f 666f 726d 6174 2e6d 6423  ssion_format.md#
+0000efa0: 736b 6970 7061 626c 652d 6672 616d 6573  skippable-frames
+0000efb0: 3e60 5f20 7468 6174 2063 616e 2063 6f6e  >`_ that can con
+0000efc0: 7461 696e 2061 6e79 2075 7365 722d 6465  tain any user-de
+0000efd0: 6669 6e65 6420 6461 7461 2c20 736b 6970  fined data, skip
+0000efe0: 7061 626c 6520 6672 616d 6520 7769 6c6c  pable frame will
+0000eff0: 2062 6520 6465 636f 6d70 7265 7373 6564   be decompressed
+0000f000: 2074 6f20 6060 6227 2760 602e 0a0a 2020   to ``b''``...  
+0000f010: 2020 2a2a 426c 6f63 6b2a 2a0a 0a20 2020    **Block**..   
+0000f020: 2041 2066 7261 6d65 2065 6e63 6170 7375   A frame encapsu
+0000f030: 6c61 7465 7320 6f6e 6520 6f72 206d 756c  lates one or mul
+0000f040: 7469 706c 6520 2262 6c6f 636b 7322 2e20  tiple "blocks". 
+0000f050: 426c 6f63 6b20 6861 7320 6120 6775 6172  Block has a guar
+0000f060: 616e 7465 6564 206d 6178 696d 756d 2073  anteed maximum s
+0000f070: 697a 6520 2833 2062 7974 6573 2062 6c6f  ize (3 bytes blo
+0000f080: 636b 2068 6561 6465 7220 2b20 3132 3820  ck header + 128 
+0000f090: 4b69 4229 2c20 7468 6520 6163 7475 616c  KiB), the actual
+0000f0a0: 206d 6178 696d 756d 2073 697a 6520 6465   maximum size de
+0000f0b0: 7065 6e64 7320 6f6e 2066 7261 6d65 2070  pends on frame p
+0000f0c0: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
+0000f0d0: 556e 6c69 6b65 2069 6e64 6570 656e 6465  Unlike independe
+0000f0e0: 6e74 2066 7261 6d65 732c 2065 6163 6820  nt frames, each 
+0000f0f0: 626c 6f63 6b20 6465 7065 6e64 7320 6f6e  block depends on
+0000f100: 2070 7265 7669 6f75 7320 626c 6f63 6b73   previous blocks
+0000f110: 2066 6f72 2070 726f 7065 7220 6465 636f   for proper deco
+0000f120: 6469 6e67 2c20 6275 7420 646f 6573 6e27  ding, but doesn'
+0000f130: 7420 6e65 6564 2074 6865 2066 6f6c 6c6f  t need the follo
+0000f140: 7769 6e67 2062 6c6f 636b 732c 2061 2063  wing blocks, a c
+0000f150: 6f6d 706c 6574 6520 626c 6f63 6b20 6361  omplete block ca
+0000f160: 6e20 6265 2066 756c 6c79 2064 6563 6f6d  n be fully decom
+0000f170: 7072 6573 7365 642e 2053 6f20 666c 7573  pressed. So flus
+0000f180: 6869 6e67 2062 6c6f 636b 206d 6179 2062  hing block may b
+0000f190: 6520 7573 6564 2069 6e20 636f 6d6d 756e  e used in commun
+0000f1a0: 6963 6174 696f 6e20 7363 656e 6172 696f  ication scenario
+0000f1b0: 732c 2073 6565 203a 7079 3a61 7474 723a  s, see :py:attr:
+0000f1c0: 605a 7374 6443 6f6d 7072 6573 736f 722e  `ZstdCompressor.
+0000f1d0: 464c 5553 485f 424c 4f43 4b60 2e0a 0a20  FLUSH_BLOCK`... 
+0000f1e0: 2020 202e 2e20 6174 7465 6e74 696f 6e3a     .. attention:
+0000f1f0: 3a0a 0a20 2020 2020 2020 2049 6e20 736f  :..        In so
+0000f200: 6d65 2060 6c61 6e67 7561 6765 2062 696e  me `language bin
+0000f210: 6469 6e67 7320 3c68 7474 7073 3a2f 2f66  dings <https://f
+0000f220: 6163 6562 6f6f 6b2e 6769 7468 7562 2e69  acebook.github.i
+0000f230: 6f2f 7a73 7464 2f23 6f74 6865 722d 6c61  o/zstd/#other-la
+0000f240: 6e67 7561 6765 733e 605f 2c20 6465 636f  nguages>`_, deco
+0000f250: 6d70 7265 7373 2829 2066 756e 6374 696f  mpress() functio
+0000f260: 6e20 646f 6573 6e27 7420 7375 7070 6f72  n doesn't suppor
+0000f270: 7420 6d75 6c74 6970 6c65 2066 7261 6d65  t multiple frame
+0000f280: 732c 206f 722f 616e 6420 646f 6573 6e27  s, or/and doesn'
+0000f290: 7420 7375 7070 6f72 7420 6120 6672 616d  t support a fram
+0000f2a0: 6520 7769 7468 2075 6e6b 6e6f 776e 203a  e with unknown :
+0000f2b0: 7265 663a 6063 6f6e 7465 6e74 2073 697a  ref:`content siz
+0000f2c0: 653c 636f 6e74 656e 745f 7369 7a65 3e60  e<content_size>`
+0000f2d0: 2c20 7061 7920 6174 7465 6e74 696f 6e20  , pay attention 
+0000f2e0: 7768 656e 2063 6f6d 7072 6573 7369 6e67  when compressing
+0000f2f0: 2064 6174 6120 666f 7220 6f74 6865 7220   data for other 
+0000f300: 6c61 6e67 7561 6765 2062 696e 6469 6e67  language binding
+0000f310: 732e 0a0a 0a4d 756c 7469 2d74 6872 6561  s....Multi-threa
+0000f320: 6465 6420 636f 6d70 7265 7373 696f 6e0a  ded compression.
+0000f330: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
+0000f340: 3e3e 3e3e 3e3e 3e3e 3e3e 0a0a 2e2e 205f  >>>>>>>>>>.... _
+0000f350: 6d74 5f63 6f6d 7072 6573 7369 6f6e 3a0a  mt_compression:.
+0000f360: 0a2e 2e20 6e6f 7465 3a3a 204d 756c 7469  ... note:: Multi
+0000f370: 2d74 6872 6561 6465 6420 636f 6d70 7265  -threaded compre
+0000f380: 7373 696f 6e0a 0a20 2020 205a 7374 6420  ssion..    Zstd 
+0000f390: 6c69 6272 6172 7920 7375 7070 6f72 7473  library supports
+0000f3a0: 206d 756c 7469 2d74 6872 6561 6465 6420   multi-threaded 
+0000f3b0: 636f 6d70 7265 7373 696f 6e2e 2053 6574  compression. Set
+0000f3c0: 203a 7079 3a61 7474 723a 6043 5061 7261   :py:attr:`CPara
+0000f3d0: 6d65 7465 722e 6e62 576f 726b 6572 7360  meter.nbWorkers`
+0000f3e0: 2070 6172 616d 6574 6572 203e 3d20 6060   parameter >= ``
+0000f3f0: 3160 6020 746f 2065 6e61 626c 6520 6d75  1`` to enable mu
+0000f400: 6c74 692d 7468 7265 6164 6564 2063 6f6d  lti-threaded com
+0000f410: 7072 6573 7369 6f6e 2c20 6060 3160 6020  pression, ``1`` 
+0000f420: 6d65 616e 7320 2231 2d74 6872 6561 6420  means "1-thread 
+0000f430: 6d75 6c74 692d 7468 7265 6164 6564 206d  multi-threaded m
+0000f440: 6f64 6522 2e0a 0a20 2020 2054 6865 2074  ode"...    The t
+0000f450: 6872 6561 6473 2061 7265 2073 7061 776e  hreads are spawn
+0000f460: 6564 2062 7920 7468 6520 756e 6465 726c  ed by the underl
+0000f470: 7969 6e67 207a 7374 6420 6c69 6272 6172  ying zstd librar
+0000f480: 792c 206e 6f74 2062 7920 7079 7a73 7464  y, not by pyzstd
+0000f490: 206d 6f64 756c 652e 0a0a 2020 2020 2e2e   module...    ..
+0000f4a0: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
+0000f4b0: 7468 6f6e 0a0a 2020 2020 2020 2020 2320  thon..        # 
+0000f4c0: 7573 6520 3420 7468 7265 6164 7320 746f  use 4 threads to
+0000f4d0: 2063 6f6d 7072 6573 730a 2020 2020 2020   compress.      
+0000f4e0: 2020 6f70 7469 6f6e 203d 207b 4350 6172    option = {CPar
+0000f4f0: 616d 6574 6572 2e6e 6257 6f72 6b65 7273  ameter.nbWorkers
+0000f500: 203a 2034 7d0a 2020 2020 2020 2020 636f   : 4}.        co
+0000f510: 6d70 7265 7373 6564 5f64 6174 203d 2063  mpressed_dat = c
+0000f520: 6f6d 7072 6573 7328 7261 775f 6461 742c  ompress(raw_dat,
+0000f530: 206f 7074 696f 6e29 0a0a 2020 2020 5468   option)..    Th
+0000f540: 6520 6461 7461 2077 696c 6c20 6265 2073  e data will be s
+0000f550: 706c 6974 2069 6e74 6f20 706f 7274 696f  plit into portio
+0000f560: 6e73 2061 6e64 2063 6f6d 7072 6573 7365  ns and compresse
+0000f570: 6420 696e 2070 6172 616c 6c65 6c2e 2054  d in parallel. T
+0000f580: 6865 2070 6f72 7469 6f6e 2073 697a 6520  he portion size 
+0000f590: 6361 6e20 6265 2073 7065 6369 6669 6564  can be specified
+0000f5a0: 2062 7920 3a70 793a 6174 7472 3a60 4350   by :py:attr:`CP
+0000f5b0: 6172 616d 6574 6572 2e6a 6f62 5369 7a65  arameter.jobSize
+0000f5c0: 6020 7061 7261 6d65 7465 722c 2074 6865  ` parameter, the
+0000f5d0: 206f 7665 726c 6170 2073 697a 6520 6361   overlap size ca
+0000f5e0: 6e20 6265 2073 7065 6369 6669 6564 2062  n be specified b
+0000f5f0: 7920 3a70 793a 6174 7472 3a60 4350 6172  y :py:attr:`CPar
+0000f600: 616d 6574 6572 2e6f 7665 726c 6170 4c6f  ameter.overlapLo
+0000f610: 6760 2070 6172 616d 6574 6572 2c20 7573  g` parameter, us
+0000f620: 7561 6c6c 7920 646f 6e27 7420 6e65 6564  ually don't need
+0000f630: 2074 6f20 7365 7420 7468 6573 652e 0a0a   to set these...
+0000f640: 2020 2020 5468 6520 6d75 6c74 692d 7468      The multi-th
+0000f650: 7265 6164 6564 206f 7574 7075 7420 7769  readed output wi
+0000f660: 6c6c 2062 6520 6469 6666 6572 656e 7420  ll be different 
+0000f670: 7468 616e 2074 6865 2073 696e 676c 652d  than the single-
+0000f680: 7468 7265 6164 6564 206f 7574 7075 742e  threaded output.
+0000f690: 2048 6f77 6576 6572 2c20 626f 7468 2061   However, both a
+0000f6a0: 7265 2064 6574 6572 6d69 6e69 7374 6963  re deterministic
+0000f6b0: 2c20 616e 6420 7468 6520 6d75 6c74 692d  , and the multi-
+0000f6c0: 7468 7265 6164 6564 206f 7574 7075 7420  threaded output 
+0000f6d0: 7072 6f64 7563 6573 2074 6865 2073 616d  produces the sam
+0000f6e0: 6520 636f 6d70 7265 7373 6564 2064 6174  e compressed dat
+0000f6f0: 6120 6e6f 206d 6174 7465 7220 686f 7720  a no matter how 
+0000f700: 6d61 6e79 2074 6872 6561 6473 2075 7365  many threads use
+0000f710: 642e 0a0a 2020 2020 5468 6520 6d75 6c74  d...    The mult
+0000f720: 692d 7468 7265 6164 6564 206f 7574 7075  i-threaded outpu
+0000f730: 7420 6973 2061 2073 696e 676c 6520 3a72  t is a single :r
+0000f740: 6566 3a60 6672 616d 653c 6672 616d 655f  ef:`frame<frame_
+0000f750: 626c 6f63 6b3e 602c 2069 7427 7320 6c61  block>`, it's la
+0000f760: 7267 6572 2061 206c 6974 746c 652e 2043  rger a little. C
+0000f770: 6f6d 7072 6573 7369 6e67 2061 2035 3230  ompressing a 520
+0000f780: 2e35 3820 4d69 4220 6461 7461 2c20 7369  .58 MiB data, si
+0000f790: 6e67 6c65 2d74 6872 6561 6465 6420 6f75  ngle-threaded ou
+0000f7a0: 7470 7574 2069 7320 3237 332e 3535 204d  tput is 273.55 M
+0000f7b0: 6942 2c20 6d75 6c74 692d 7468 7265 6164  iB, multi-thread
+0000f7c0: 6564 206f 7574 7075 7420 6973 2032 3734  ed output is 274
+0000f7d0: 2e33 3320 4d69 422e 0a0a 2020 2020 2e2e  .33 MiB...    ..
+0000f7e0: 2068 696e 743a 3a0a 2020 2020 2020 2020   hint::.        
+0000f7f0: 5573 696e 6720 2243 5055 2070 6879 7369  Using "CPU physi
+0000f800: 6361 6c20 636f 7265 7320 6e75 6d62 6572  cal cores number
+0000f810: 2220 6173 2074 6872 6561 6473 206e 756d  " as threads num
+0000f820: 6265 7220 6d61 7920 6265 2074 6865 2066  ber may be the f
+0000f830: 6173 7465 7374 2c20 746f 2067 6574 2074  astest, to get t
+0000f840: 6865 206e 756d 6265 7220 6e65 6564 2074  he number need t
+0000f850: 6f20 696e 7374 616c 6c20 7468 6972 642d  o install third-
+0000f860: 7061 7274 7920 6d6f 6475 6c65 2e20 606f  party module. `o
+0000f870: 732e 6370 755f 636f 756e 7428 2920 3c68  s.cpu_count() <h
+0000f880: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
+0000f890: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
+0000f8a0: 2f6f 732e 6874 6d6c 236f 732e 6370 755f  /os.html#os.cpu_
+0000f8b0: 636f 756e 743e 605f 2063 616e 206f 6e6c  count>`_ can onl
+0000f8c0: 7920 6765 7420 2243 5055 206c 6f67 6963  y get "CPU logic
+0000f8d0: 616c 2063 6f72 6573 206e 756d 6265 7222  al cores number"
+0000f8e0: 2028 6879 7065 722d 7468 7265 6164 696e   (hyper-threadin
+0000f8f0: 6720 6361 7061 6269 6c69 7479 292e 0a0a  g capability)...
+0000f900: 0a52 6963 6820 6d65 6d6f 7279 206d 6f64  .Rich memory mod
+0000f910: 650a 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  e.>>>>>>>>>>>>>>
+0000f920: 3e3e 0a0a 2e2e 205f 7269 6368 5f6d 656d  >>.... _rich_mem
+0000f930: 3a0a 0a2e 2e20 6e6f 7465 3a3a 2052 6963  :.... note:: Ric
+0000f940: 6820 6d65 6d6f 7279 206d 6f64 650a 0a20  h memory mode.. 
+0000f950: 2020 2070 797a 7374 6420 6d6f 6475 6c65     pyzstd module
+0000f960: 2068 6173 2061 2022 7269 6368 206d 656d   has a "rich mem
+0000f970: 6f72 7920 6d6f 6465 2220 666f 7220 636f  ory mode" for co
+0000f980: 6d70 7265 7373 696f 6e2e 2049 7420 616c  mpression. It al
+0000f990: 6c6f 6361 7465 7320 6d6f 7265 206d 656d  locates more mem
+0000f9a0: 6f72 7920 666f 7220 6f75 7470 7574 2062  ory for output b
+0000f9b0: 7566 6665 722c 2061 6e64 2066 6173 7465  uffer, and faste
+0000f9c0: 7220 696e 2073 6f6d 6520 6361 7365 732e  r in some cases.
+0000f9d0: 2053 7569 7461 626c 6520 666f 7220 6578   Suitable for ex
+0000f9e0: 7472 656d 656c 7920 6661 7374 2063 6f6d  tremely fast com
+0000f9f0: 7072 6573 7369 6f6e 2073 6365 6e61 7269  pression scenari
+0000fa00: 6f73 2e0a 0a20 2020 2054 6865 7265 2069  os...    There i
+0000fa10: 7320 6120 3a70 793a 6675 6e63 3a60 7269  s a :py:func:`ri
+0000fa20: 6368 6d65 6d5f 636f 6d70 7265 7373 6020  chmem_compress` 
+0000fa30: 6675 6e63 7469 6f6e 2c20 6120 3a70 793a  function, a :py:
+0000fa40: 636c 6173 733a 6052 6963 684d 656d 5a73  class:`RichMemZs
+0000fa50: 7464 436f 6d70 7265 7373 6f72 6020 636c  tdCompressor` cl
+0000fa60: 6173 732e 0a0a 2020 2020 4375 7272 656e  ass...    Curren
+0000fa70: 746c 7920 6974 2077 6f6e 2774 2062 6520  tly it won't be 
+0000fa80: 6661 7374 6572 2077 6865 6e20 7573 696e  faster when usin
+0000fa90: 6720 3a72 6566 3a60 7a73 7464 206d 756c  g :ref:`zstd mul
+0000faa0: 7469 2d74 6872 6561 6465 6420 636f 6d70  ti-threaded comp
+0000fab0: 7265 7373 696f 6e20 3c6d 745f 636f 6d70  ression <mt_comp
+0000fac0: 7265 7373 696f 6e3e 602c 2069 7420 7769  ression>`, it wi
+0000fad0: 6c6c 2069 7373 7565 2061 2060 6052 6573  ll issue a ``Res
+0000fae0: 6f75 7263 6557 6172 6e69 6e67 7360 6020  ourceWarnings`` 
+0000faf0: 696e 2074 6869 7320 6361 7365 2e0a 0a20  in this case... 
+0000fb00: 2020 2045 6666 6563 7473 3a0a 0a20 2020     Effects:..   
+0000fb10: 202a 2054 6865 206f 7574 7075 7420 6275   * The output bu
+0000fb20: 6666 6572 2069 7320 6c61 7267 6572 2074  ffer is larger t
+0000fb30: 6861 6e20 696e 7075 7420 6461 7461 2061  han input data a
+0000fb40: 206c 6974 746c 652e 0a20 2020 202a 2049   little..    * I
+0000fb50: 6620 696e 7075 7420 6461 7461 2069 7320  f input data is 
+0000fb60: 6c61 7267 6572 2074 6861 6e20 7e33 312e  larger than ~31.
+0000fb70: 384b 422c 2075 7020 746f 2032 3225 2066  8KB, up to 22% f
+0000fb80: 6173 7465 722e 2054 6865 206c 6f77 6572  aster. The lower
+0000fb90: 2074 6865 2063 6f6d 7072 6573 7369 6f6e   the compression
+0000fba0: 206c 6576 656c 2c20 7468 6520 6d75 6368   level, the much
+0000fbb0: 2066 6173 7465 7220 6974 2069 7320 7573   faster it is us
+0000fbc0: 7561 6c6c 792e 0a0a 2020 2020 5768 656e  ually...    When
+0000fbd0: 206e 6f74 2075 7369 6e67 2074 6869 7320   not using this 
+0000fbe0: 6d6f 6465 2c20 7468 6520 6f75 7470 7574  mode, the output
+0000fbf0: 2062 7566 6665 7220 6772 6f77 7320 6067   buffer grows `g
+0000fc00: 7261 6475 616c 6c79 203c 6874 7470 733a  radually <https:
+0000fc10: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6e69  //github.com/ani
+0000fc20: 6d61 6c69 7a65 2f70 797a 7374 642f 626c  malize/pyzstd/bl
+0000fc30: 6f62 2f30 2e31 352e 372f 7372 632f 6269  ob/0.15.7/src/bi
+0000fc40: 6e5f 6578 742f 5f7a 7374 646d 6f64 756c  n_ext/_zstdmodul
+0000fc50: 652e 6323 4c32 3138 2d4c 3234 333e 605f  e.c#L218-L243>`_
+0000fc60: 2c20 696e 206f 7264 6572 206e 6f74 2074  , in order not t
+0000fc70: 6f20 616c 6c6f 6361 7465 2074 6f6f 206d  o allocate too m
+0000fc80: 7563 6820 6d65 6d6f 7279 2e20 5468 6520  uch memory. The 
+0000fc90: 6e65 6761 7469 7665 2065 6666 6563 7420  negative effect 
+0000fca0: 6973 2074 6861 7420 7079 7a73 7464 206d  is that pyzstd m
+0000fcb0: 6f64 756c 6520 7573 7561 6c6c 7920 6e65  odule usually ne
+0000fcc0: 6564 2074 6f20 6361 6c6c 2074 6865 2075  ed to call the u
+0000fcd0: 6e64 6572 6c79 696e 6720 7a73 7464 206c  nderlying zstd l
+0000fce0: 6962 7261 7279 2773 2063 6f6d 7072 6573  ibrary's compres
+0000fcf0: 7320 6675 6e63 7469 6f6e 206d 756c 7469  s function multi
+0000fd00: 706c 6520 7469 6d65 732e 0a0a 2020 2020  ple times...    
+0000fd10: 5768 656e 2075 7369 6e67 2074 6869 7320  When using this 
+0000fd20: 6d6f 6465 2c20 7468 6520 7369 7a65 206f  mode, the size o
+0000fd30: 6620 6f75 7470 7574 2062 7566 6665 7220  f output buffer 
+0000fd40: 6973 2070 726f 7669 6465 6420 6279 205a  is provided by Z
+0000fd50: 5354 445f 636f 6d70 7265 7373 426f 756e  STD_compressBoun
+0000fd60: 6428 2920 6675 6e63 7469 6f6e 2c20 7768  d() function, wh
+0000fd70: 6963 6820 6973 206c 6172 6765 7220 7468  ich is larger th
+0000fd80: 616e 2069 6e70 7574 2064 6174 6120 6120  an input data a 
+0000fd90: 6c69 7474 6c65 2028 6d61 7869 6d75 6d20  little (maximum 
+0000fda0: 636f 6d70 7265 7373 6564 2073 697a 6520  compressed size 
+0000fdb0: 696e 2077 6f72 7374 2063 6173 6520 7369  in worst case si
+0000fdc0: 6e67 6c65 2d70 6173 7320 7363 656e 6172  ngle-pass scenar
+0000fdd0: 696f 292e 2046 6f72 2061 2031 3030 204d  io). For a 100 M
+0000fde0: 6942 2069 6e70 7574 2064 6174 612c 2074  iB input data, t
+0000fdf0: 6865 2061 6c6c 6f63 6174 6564 206f 7574  he allocated out
+0000fe00: 7075 7420 6275 6666 6572 2069 7320 2831  put buffer is (1
+0000fe10: 3030 204d 6942 202b 2034 3030 204b 6942  00 MiB + 400 KiB
+0000fe20: 292e 2054 6865 2075 6e64 6572 6c79 696e  ). The underlyin
+0000fe30: 6720 7a73 7464 206c 6962 7261 7279 2061  g zstd library a
+0000fe40: 766f 6964 7320 6578 7472 6120 6d65 6d6f  voids extra memo
+0000fe50: 7279 2063 6f70 7920 666f 7220 7468 6973  ry copy for this
+0000fe60: 206f 7574 7075 7420 6275 6666 6572 2073   output buffer s
+0000fe70: 697a 652e 0a0a 2020 2020 2e2e 2073 6f75  ize...    .. sou
+0000fe80: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
+0000fe90: 0a0a 2020 2020 2020 2020 2320 7573 6520  ..        # use 
+0000fea0: 7269 6368 6d65 6d5f 636f 6d70 7265 7373  richmem_compress
+0000feb0: 2829 2066 756e 6374 696f 6e0a 2020 2020  () function.    
+0000fec0: 2020 2020 636f 6d70 7265 7373 6564 5f64      compressed_d
+0000fed0: 6174 203d 2072 6963 686d 656d 5f63 6f6d  at = richmem_com
+0000fee0: 7072 6573 7328 7261 775f 6461 7429 0a0a  press(raw_dat)..
+0000fef0: 2020 2020 2020 2020 2320 7265 7573 6520          # reuse 
+0000ff00: 5269 6368 4d65 6d5a 7374 6443 6f6d 7072  RichMemZstdCompr
+0000ff10: 6573 736f 7220 6f62 6a65 6374 0a20 2020  essor object.   
+0000ff20: 2020 2020 2063 203d 2052 6963 684d 656d       c = RichMem
+0000ff30: 5a73 7464 436f 6d70 7265 7373 6f72 2829  ZstdCompressor()
+0000ff40: 0a20 2020 2020 2020 2066 7261 6d65 3120  .        frame1 
+0000ff50: 3d20 632e 636f 6d70 7265 7373 2872 6177  = c.compress(raw
+0000ff60: 5f64 6174 3129 0a20 2020 2020 2020 2066  _dat1).        f
+0000ff70: 7261 6d65 3220 3d20 632e 636f 6d70 7265  rame2 = c.compre
+0000ff80: 7373 2872 6177 5f64 6174 3229 0a0a 2020  ss(raw_dat2)..  
+0000ff90: 2020 436f 6d70 7265 7373 696e 6720 6120    Compressing a 
+0000ffa0: 3532 302e 3538 204d 6942 2064 6174 612c  520.58 MiB data,
+0000ffb0: 2069 7420 6163 6365 6c65 7261 7465 7320   it accelerates 
+0000ffc0: 6672 6f6d 2035 2e34 3020 7365 636f 6e64  from 5.40 second
+0000ffd0: 7320 746f 2034 2e36 3220 7365 636f 6e64  s to 4.62 second
+0000ffe0: 732e 0a0a 0a55 7365 2077 6974 6820 7461  s....Use with ta
+0000fff0: 7266 696c 6520 6d6f 6475 6c65 0a3e 3e3e  rfile module.>>>
+00010000: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
+00010010: 3e3e 3e3e 0a0a 2e2e 205f 7769 7468 5f74  >>>>.... _with_t
+00010020: 6172 6669 6c65 3a0a 0a2e 2e20 6e6f 7465  arfile:.... note
+00010030: 3a3a 2055 7365 2077 6974 6820 7461 7266  :: Use with tarf
+00010040: 696c 6520 6d6f 6475 6c65 0a0a 2020 2020  ile module..    
+00010050: 5079 7468 6f6e 2773 2060 7461 7266 696c  Python's `tarfil
+00010060: 6520 3c68 7474 7073 3a2f 2f64 6f63 732e  e <https://docs.
+00010070: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+00010080: 7261 7279 2f74 6172 6669 6c65 2e68 746d  rary/tarfile.htm
+00010090: 6c3e 605f 206d 6f64 756c 6520 7375 7070  l>`_ module supp
+000100a0: 6f72 7473 2061 7262 6974 7261 7279 2063  orts arbitrary c
+000100b0: 6f6d 7072 6573 7369 6f6e 2061 6c67 6f72  ompression algor
+000100c0: 6974 686d 7320 6279 2070 726f 7669 6469  ithms by providi
+000100d0: 6e67 2061 2066 696c 6520 6f62 6a65 6374  ng a file object
+000100e0: 2e0a 0a20 2020 2054 6869 7320 636f 6465  ...    This code
+000100f0: 2065 6e63 6170 7375 6c61 7465 7320 6120   encapsulates a 
+00010100: 6060 5a73 7464 5461 7246 696c 6560 6020  ``ZstdTarFile`` 
+00010110: 636c 6173 7320 7573 696e 6720 3a70 793a  class using :py:
+00010120: 636c 6173 733a 605a 7374 6446 696c 6560  class:`ZstdFile`
+00010130: 2c20 6974 2063 616e 2062 6520 7573 6564  , it can be used
+00010140: 206c 696b 6520 6074 6172 6669 6c65 2e54   like `tarfile.T
+00010150: 6172 4669 6c65 203c 6874 7470 733a 2f2f  arFile <https://
+00010160: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+00010170: 332f 6c69 6272 6172 792f 7461 7266 696c  3/library/tarfil
+00010180: 652e 6874 6d6c 2374 6172 6669 6c65 2e54  e.html#tarfile.T
+00010190: 6172 4669 6c65 3e60 5f20 636c 6173 733a  arFile>`_ class:
+000101a0: 0a0a 2020 2020 2e2e 2073 6f75 7263 6563  ..    .. sourcec
+000101b0: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+000101c0: 2020 2020 2020 696d 706f 7274 2074 6172        import tar
+000101d0: 6669 6c65 0a0a 2020 2020 2020 2020 2320  file..        # 
+000101e0: 7768 656e 2075 7369 6e67 2072 6561 6420  when using read 
+000101f0: 6d6f 6465 2028 6465 636f 6d70 7265 7373  mode (decompress
+00010200: 696f 6e29 2c20 7468 6520 6c65 7665 6c5f  ion), the level_
+00010210: 6f72 5f6f 7074 696f 6e20 7061 7261 6d65  or_option parame
+00010220: 7465 720a 2020 2020 2020 2020 2320 6361  ter.        # ca
+00010230: 6e20 6f6e 6c79 2062 6520 6120 6469 6374  n only be a dict
+00010240: 206f 626a 6563 742c 2074 6861 7420 7265   object, that re
+00010250: 7072 6573 656e 7473 2064 6563 6f6d 7072  presents decompr
+00010260: 6573 7369 6f6e 206f 7074 696f 6e2e 2049  ession option. I
+00010270: 740a 2020 2020 2020 2020 2320 646f 6573  t.        # does
+00010280: 6e27 7420 7375 7070 6f72 7420 696e 7420  n't support int 
+00010290: 7479 7065 2063 6f6d 7072 6573 7369 6f6e  type compression
+000102a0: 206c 6576 656c 2069 6e20 7468 6973 2063   level in this c
+000102b0: 6173 652e 0a0a 2020 2020 2020 2020 636c  ase...        cl
+000102c0: 6173 7320 5a73 7464 5461 7246 696c 6528  ass ZstdTarFile(
+000102d0: 7461 7266 696c 652e 5461 7246 696c 6529  tarfile.TarFile)
+000102e0: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+000102f0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00010300: 206e 616d 652c 206d 6f64 653d 2772 272c   name, mode='r',
+00010310: 202a 2c20 6c65 7665 6c5f 6f72 5f6f 7074   *, level_or_opt
+00010320: 696f 6e3d 4e6f 6e65 2c20 7a73 7464 5f64  ion=None, zstd_d
+00010330: 6963 743d 4e6f 6e65 2c20 2a2a 6b77 6172  ict=None, **kwar
+00010340: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
+00010350: 2020 2020 2073 656c 662e 7a73 7464 5f66       self.zstd_f
+00010360: 696c 6520 3d20 5a73 7464 4669 6c65 286e  ile = ZstdFile(n
+00010370: 616d 652c 206d 6f64 652c 0a20 2020 2020  ame, mode,.     
+00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103a0: 2020 2020 206c 6576 656c 5f6f 725f 6f70       level_or_op
+000103b0: 7469 6f6e 3d6c 6576 656c 5f6f 725f 6f70  tion=level_or_op
+000103c0: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103f0: 7a73 7464 5f64 6963 743d 7a73 7464 5f64  zstd_dict=zstd_d
+00010400: 6963 7429 0a20 2020 2020 2020 2020 2020  ict).           
+00010410: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00010420: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00010430: 7065 7228 292e 5f5f 696e 6974 5f5f 2866  per().__init__(f
+00010440: 696c 656f 626a 3d73 656c 662e 7a73 7464  ileobj=self.zstd
+00010450: 5f66 696c 652c 206d 6f64 653d 6d6f 6465  _file, mode=mode
+00010460: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+00010470: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00010480: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+00010490: 2020 2020 2020 2020 7365 6c66 2e7a 7374          self.zst
+000104a0: 645f 6669 6c65 2e63 6c6f 7365 2829 0a20  d_file.close(). 
+000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104c0: 2020 2072 6169 7365 0a0a 2020 2020 2020     raise..      
+000104d0: 2020 2020 2020 6465 6620 636c 6f73 6528        def close(
+000104e0: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
+000104f0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010510: 7375 7065 7228 292e 636c 6f73 6528 290a  super().close().
+00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010530: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
+00010540: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010550: 662e 7a73 7464 5f66 696c 652e 636c 6f73  f.zstd_file.clos
+00010560: 6528 290a 0a20 2020 2020 2020 2023 2077  e()..        # w
+00010570: 7269 7465 202e 7461 722e 7a73 7420 6669  rite .tar.zst fi
+00010580: 6c65 2028 636f 6d70 7265 7373 696f 6e29  le (compression)
+00010590: 0a20 2020 2020 2020 2077 6974 6820 5a73  .        with Zs
+000105a0: 7464 5461 7246 696c 6528 2761 7263 6869  tdTarFile('archi
+000105b0: 7665 2e74 6172 2e7a 7374 272c 206d 6f64  ve.tar.zst', mod
+000105c0: 653d 2777 272c 206c 6576 656c 5f6f 725f  e='w', level_or_
+000105d0: 6f70 7469 6f6e 3d35 2920 6173 2074 6172  option=5) as tar
+000105e0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+000105f0: 646f 2073 6f6d 6574 6869 6e67 0a0a 2020  do something..  
+00010600: 2020 2020 2020 2320 7265 6164 202e 7461        # read .ta
+00010610: 722e 7a73 7420 6669 6c65 2028 6465 636f  r.zst file (deco
+00010620: 6d70 7265 7373 696f 6e29 0a20 2020 2020  mpression).     
+00010630: 2020 2077 6974 6820 5a73 7464 5461 7246     with ZstdTarF
+00010640: 696c 6528 2761 7263 6869 7665 2e74 6172  ile('archive.tar
+00010650: 2e7a 7374 272c 206d 6f64 653d 2772 2729  .zst', mode='r')
+00010660: 2061 7320 7461 723a 0a20 2020 2020 2020   as tar:.       
+00010670: 2020 2020 2023 2064 6f20 736f 6d65 7468       # do someth
+00010680: 696e 670a 0a20 2020 2057 6865 6e20 7468  ing..    When th
+00010690: 6520 6162 6f76 6520 636f 6465 2069 7320  e above code is 
+000106a0: 696e 2072 6561 6420 6d6f 6465 2028 6465  in read mode (de
+000106b0: 636f 6d70 7265 7373 696f 6e29 2c20 616e  compression), an
+000106c0: 6420 7365 6c65 6374 6976 656c 7920 7265  d selectively re
+000106d0: 6164 2066 696c 6573 206d 756c 7469 706c  ad files multipl
+000106e0: 6520 7469 6d65 732c 2069 7420 6d61 7920  e times, it may 
+000106f0: 7365 656b 2074 6f20 7072 6576 696f 7573  seek to previous
+00010700: 2070 6f73 6974 696f 6e73 2c20 7468 656e   positions, then
+00010710: 2074 6865 2064 6563 6f6d 7072 6573 7369   the decompressi
+00010720: 6f6e 2068 6173 2074 6f20 6265 2072 6573  on has to be res
+00010730: 7461 7274 6564 2066 726f 6d20 7a65 726f  tarted from zero
+00010740: 2e20 4966 2074 6869 7320 736c 6f77 7320  . If this slows 
+00010750: 646f 776e 2074 6865 206f 7065 7261 7469  down the operati
+00010760: 6f6e 732c 2074 6865 2061 7263 6869 7665  ons, the archive
+00010770: 2063 616e 2062 6520 6465 636f 6d70 7265   can be decompre
+00010780: 7373 6564 2074 6f20 6120 7465 6d70 6f72  ssed to a tempor
+00010790: 6172 7920 6669 6c65 2c20 616e 6420 7265  ary file, and re
+000107a0: 6164 2066 726f 6d20 6974 2e20 5468 6973  ad from it. This
+000107b0: 2063 6f64 6520 656e 6361 7073 756c 6174   code encapsulat
+000107c0: 6573 2074 6865 2070 726f 6365 7373 3a0a  es the process:.
+000107d0: 0a20 2020 202e 2e20 736f 7572 6365 636f  .    .. sourceco
+000107e0: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
+000107f0: 2020 2020 2069 6d70 6f72 7420 636f 6e74       import cont
+00010800: 6578 746c 6962 0a20 2020 2020 2020 2069  extlib.        i
+00010810: 6d70 6f72 7420 696f 0a20 2020 2020 2020  mport io.       
+00010820: 2069 6d70 6f72 7420 7461 7266 696c 650a   import tarfile.
+00010830: 2020 2020 2020 2020 696d 706f 7274 2074          import t
+00010840: 656d 7066 696c 650a 2020 2020 2020 2020  empfile.        
+00010850: 6672 6f6d 2070 797a 7374 6420 696d 706f  from pyzstd impo
+00010860: 7274 2064 6563 6f6d 7072 6573 735f 7374  rt decompress_st
+00010870: 7265 616d 0a0a 2020 2020 2020 2020 4063  ream..        @c
+00010880: 6f6e 7465 7874 6c69 622e 636f 6e74 6578  ontextlib.contex
+00010890: 746d 616e 6167 6572 0a20 2020 2020 2020  tmanager.       
+000108a0: 2064 6566 205a 7374 6454 6172 5265 6164   def ZstdTarRead
+000108b0: 6572 286e 616d 652c 202a 2c20 7a73 7464  er(name, *, zstd
+000108c0: 5f64 6963 743d 4e6f 6e65 2c20 6f70 7469  _dict=None, opti
+000108d0: 6f6e 3d4e 6f6e 652c 202a 2a6b 7761 7267  on=None, **kwarg
+000108e0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+000108f0: 7769 7468 2069 6f2e 6f70 656e 286e 616d  with io.open(nam
+00010900: 652c 2027 7262 2729 2061 7320 6966 683a  e, 'rb') as ifh:
+00010910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010920: 2077 6974 6820 7465 6d70 6669 6c65 2e54   with tempfile.T
+00010930: 656d 706f 7261 7279 4669 6c65 2829 2061  emporaryFile() a
+00010940: 7320 746d 705f 6669 6c65 3a0a 2020 2020  s tmp_file:.    
+00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010960: 6465 636f 6d70 7265 7373 5f73 7472 6561  decompress_strea
+00010970: 6d28 6966 682c 2074 6d70 5f66 696c 652c  m(ifh, tmp_file,
+00010980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109a0: 2020 2020 2020 207a 7374 645f 6469 6374         zstd_dict
+000109b0: 3d7a 7374 645f 6469 6374 2c20 6f70 7469  =zstd_dict, opti
+000109c0: 6f6e 3d6f 7074 696f 6e29 0a20 2020 2020  on=option).     
+000109d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000109e0: 6d70 5f66 696c 652e 7365 656b 2830 290a  mp_file.seek(0).
+000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a00: 2020 2020 7769 7468 2074 6172 6669 6c65      with tarfile
+00010a10: 2e54 6172 4669 6c65 2866 696c 656f 626a  .TarFile(fileobj
+00010a20: 3d74 6d70 5f66 696c 652c 202a 2a6b 7761  =tmp_file, **kwa
+00010a30: 7267 7329 2061 7320 7461 723a 0a20 2020  rgs) as tar:.   
+00010a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a50: 2020 2020 2079 6965 6c64 2074 6172 0a0a       yield tar..
+00010a60: 2020 2020 2020 2020 7769 7468 205a 7374          with Zst
+00010a70: 6454 6172 5265 6164 6572 2827 6172 6368  dTarReader('arch
+00010a80: 6976 652e 7461 722e 7a73 7427 2920 6173  ive.tar.zst') as
+00010a90: 2074 6172 3a0a 2020 2020 2020 2020 2020   tar:.          
+00010aa0: 2020 2320 646f 2073 6f6d 6574 6869 6e67    # do something
+00010ab0: 0a0a 0a5a 7374 6420 6469 6374 696f 6e61  ...Zstd dictiona
+00010ac0: 7279 2049 440a 3e3e 3e3e 3e3e 3e3e 3e3e  ry ID.>>>>>>>>>>
+00010ad0: 3e3e 3e3e 3e3e 3e3e 0a0a 2e2e 205f 6469  >>>>>>>>.... _di
+00010ae0: 6374 5f69 643a 0a0a 2e2e 206e 6f74 653a  ct_id:.... note:
+00010af0: 3a20 5a73 7464 2064 6963 7469 6f6e 6172  : Zstd dictionar
+00010b00: 7920 4944 0a0a 2020 2020 4469 6374 696f  y ID..    Dictio
+00010b10: 6e61 7279 2049 4420 6973 2061 2033 322d  nary ID is a 32-
+00010b20: 6269 7420 756e 7369 676e 6564 2069 6e74  bit unsigned int
+00010b30: 6567 6572 2076 616c 7565 2e20 4465 636f  eger value. Deco
+00010b40: 6465 7220 7573 6573 2069 7420 746f 2063  der uses it to c
+00010b50: 6865 636b 2069 6620 7468 6520 636f 7272  heck if the corr
+00010b60: 6563 7420 6469 6374 696f 6e61 7279 2069  ect dictionary i
+00010b70: 7320 7573 6564 2e0a 0a20 2020 2041 6363  s used...    Acc
+00010b80: 6f72 6469 6e67 2074 6f20 7a73 7464 2064  ording to zstd d
+00010b90: 6963 7469 6f6e 6172 7920 666f 726d 6174  ictionary format
+00010ba0: 2060 7370 6563 6966 6963 6174 696f 6e20   `specification 
+00010bb0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+00010bc0: 636f 6d2f 6661 6365 626f 6f6b 2f7a 7374  com/facebook/zst
+00010bd0: 642f 626c 6f62 2f72 656c 6561 7365 2f64  d/blob/release/d
+00010be0: 6f63 2f7a 7374 645f 636f 6d70 7265 7373  oc/zstd_compress
+00010bf0: 696f 6e5f 666f 726d 6174 2e6d 6423 6469  ion_format.md#di
+00010c00: 6374 696f 6e61 7279 2d66 6f72 6d61 743e  ctionary-format>
+00010c10: 605f 2c20 6966 2061 2064 6963 7469 6f6e  `_, if a diction
+00010c20: 6172 7920 6973 2067 6f69 6e67 2074 6f20  ary is going to 
+00010c30: 6265 2064 6973 7472 6962 7574 6564 2069  be distributed i
+00010c40: 6e20 7075 626c 6963 2c20 7468 6520 666f  n public, the fo
+00010c50: 6c6c 6f77 696e 6720 7261 6e67 6573 2061  llowing ranges a
+00010c60: 7265 2072 6573 6572 7665 6420 666f 7220  re reserved for 
+00010c70: 6675 7475 7265 2072 6567 6973 7472 6172  future registrar
+00010c80: 2061 6e64 2073 6861 6c6c 206e 6f74 2062   and shall not b
+00010c90: 6520 7573 6564 3a0a 0a20 2020 2020 2020  e used:..       
+00010ca0: 202d 206c 6f77 2072 616e 6765 3a20 3c3d   - low range: <=
+00010cb0: 2033 3237 3637 0a20 2020 2020 2020 202d   32767.        -
+00010cc0: 2068 6967 6820 7261 6e67 653a 203e 3d20   high range: >= 
+00010cd0: 325e 3331 0a0a 2020 2020 4f75 7473 6964  2^31..    Outsid
+00010ce0: 6520 6f66 2074 6865 7365 2072 616e 6765  e of these range
+00010cf0: 732c 2061 6e79 2076 616c 7565 2069 6e20  s, any value in 
+00010d00: 2833 3237 3637 203c 2076 203c 2032 5e33  (32767 < v < 2^3
+00010d10: 3129 2063 616e 2062 6520 7573 6564 2066  1) can be used f
+00010d20: 7265 656c 792c 2065 7665 6e20 696e 2070  reely, even in p
+00010d30: 7562 6c69 6320 656e 7669 726f 6e6d 656e  ublic environmen
+00010d40: 742e 0a0a 2020 2020 496e 207a 7374 6420  t...    In zstd 
+00010d50: 6672 616d 6520 6865 6164 6572 2c20 7468  frame header, th
+00010d60: 6520 6044 6963 7469 6f6e 6172 795f 4944  e `Dictionary_ID
+00010d70: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
+00010d80: 2e63 6f6d 2f66 6163 6562 6f6f 6b2f 7a73  .com/facebook/zs
+00010d90: 7464 2f62 6c6f 622f 7265 6c65 6173 652f  td/blob/release/
+00010da0: 646f 632f 7a73 7464 5f63 6f6d 7072 6573  doc/zstd_compres
+00010db0: 7369 6f6e 5f66 6f72 6d61 742e 6d64 2364  sion_format.md#d
+00010dc0: 6963 7469 6f6e 6172 795f 6964 3e60 5f20  ictionary_id>`_ 
+00010dd0: 6669 656c 6420 6361 6e20 6265 2030 2f31  field can be 0/1
+00010de0: 2f32 2f34 2062 7974 6573 2e20 4966 2074  /2/4 bytes. If t
+00010df0: 6865 2076 616c 7565 2069 7320 736d 616c  he value is smal
+00010e00: 6c2c 2074 6869 7320 6361 6e20 7361 7665  l, this can save
+00010e10: 2032 7e33 2062 7974 6573 2e20 4f72 2064   2~3 bytes. Or d
+00010e20: 6f6e 2774 2077 7269 7465 2074 6865 2049  on't write the I
+00010e30: 4420 6279 2073 6574 7469 6e67 203a 7079  D by setting :py
+00010e40: 3a61 7474 723a 6043 5061 7261 6d65 7465  :attr:`CParamete
+00010e50: 722e 6469 6374 4944 466c 6167 6020 7061  r.dictIDFlag` pa
+00010e60: 7261 6d65 7465 722e 0a0a 2020 2020 7079  rameter...    py
+00010e70: 7a73 7464 206d 6f64 756c 6520 646f 6573  zstd module does
+00010e80: 6e27 7420 7375 7070 6f72 7420 7370 6563  n't support spec
+00010e90: 6966 7969 6e67 2049 4420 7768 656e 2074  ifying ID when t
+00010ea0: 7261 696e 696e 6720 6469 6374 696f 6e61  raining dictiona
+00010eb0: 7279 2063 7572 7265 6e74 6c79 2e20 4966  ry currently. If
+00010ec0: 2077 616e 7420 746f 2073 7065 6369 6679   want to specify
+00010ed0: 2074 6865 2049 442c 206d 6f64 6966 7920   the ID, modify 
+00010ee0: 7468 6520 6469 6374 696f 6e61 7279 2063  the dictionary c
+00010ef0: 6f6e 7465 6e74 2061 6363 6f72 6469 6e67  ontent according
+00010f00: 2074 6f20 666f 726d 6174 2073 7065 6369   to format speci
+00010f10: 6669 6361 7469 6f6e 2c20 616e 6420 7461  fication, and ta
+00010f20: 6b65 2074 6865 2063 6f72 7265 7370 6f6e  ke the correspon
+00010f30: 6469 6e67 2072 6973 6b73 2e0a 0a20 2020  ding risks...   
+00010f40: 202a 2a41 7474 656e 7469 6f6e 2a2a 0a0a   **Attention**..
+00010f50: 2020 2020 496e 203a 7079 3a63 6c61 7373      In :py:class
+00010f60: 3a60 5a73 7464 4469 6374 6020 636c 6173  :`ZstdDict` clas
+00010f70: 732c 203a 7079 3a61 7474 723a 605a 7374  s, :py:attr:`Zst
+00010f80: 6444 6963 742e 6469 6374 5f69 6460 2061  dDict.dict_id` a
+00010f90: 7474 7269 6275 7465 203d 3d20 3020 6d65  ttribute == 0 me
+00010fa0: 616e 7320 7468 6520 6469 6374 696f 6e61  ans the dictiona
+00010fb0: 7279 2069 7320 6120 2272 6177 2063 6f6e  ry is a "raw con
+00010fc0: 7465 6e74 2220 6469 6374 696f 6e61 7279  tent" dictionary
+00010fd0: 2c20 6672 6565 206f 6620 616e 7920 666f  , free of any fo
+00010fe0: 726d 6174 2072 6573 7472 6963 7469 6f6e  rmat restriction
+00010ff0: 2c20 7573 6564 2066 6f72 2061 6476 616e  , used for advan
+00011000: 6365 6420 7573 6572 2e20 4e6f 6e2d 7a65  ced user. Non-ze
+00011010: 726f 206d 6561 6e73 2069 7427 7320 616e  ro means it's an
+00011020: 206f 7264 696e 6172 7920 6469 6374 696f   ordinary dictio
+00011030: 6e61 7279 2c20 7761 7320 6372 6561 7465  nary, was create
+00011040: 6420 6279 207a 7374 6420 6675 6e63 7469  d by zstd functi
+00011050: 6f6e 732c 2066 6f6c 6c6f 7720 7468 6520  ons, follow the 
+00011060: 666f 726d 6174 2073 7065 6369 6669 6361  format specifica
+00011070: 7469 6f6e 2e0a 0a20 2020 2049 6e20 3a70  tion...    In :p
+00011080: 793a 6675 6e63 3a60 6765 745f 6672 616d  y:func:`get_fram
+00011090: 655f 696e 666f 6020 6675 6e63 7469 6f6e  e_info` function
+000110a0: 2c20 6060 6469 6374 696f 6e61 7279 5f69  , ``dictionary_i
+000110b0: 6460 6020 3d3d 2030 206d 6561 6e73 2064  d`` == 0 means d
+000110c0: 6963 7469 6f6e 6172 7920 4944 2077 6173  ictionary ID was
+000110d0: 206e 6f74 2072 6563 6f72 6465 6420 696e   not recorded in
+000110e0: 2074 6865 2066 7261 6d65 2068 6561 6465   the frame heade
+000110f0: 722c 2074 6865 2066 7261 6d65 206d 6179  r, the frame may
+00011100: 206f 7220 6d61 7920 6e6f 7420 6e65 6564   or may not need
+00011110: 2061 2064 6963 7469 6f6e 6172 7920 746f   a dictionary to
+00011120: 2062 6520 6465 636f 6465 642c 2061 6e64   be decoded, and
+00011130: 2074 6865 2049 4420 6f66 2073 7563 6820   the ID of such 
+00011140: 6120 6469 6374 696f 6e61 7279 2069 7320  a dictionary is 
+00011150: 6e6f 7420 7370 6563 6966 6965 642e 0a0a  not specified...
+00011160: 0a55 7365 207a 7374 6420 6173 2061 2070  .Use zstd as a p
+00011170: 6174 6368 696e 6720 656e 6769 6e65 0a3e  atching engine.>
+00011180: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
+00011190: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 0a0a 2e2e  >>>>>>>>>>>>....
+000111a0: 205f 7061 7463 6869 6e67 5f65 6e67 696e   _patching_engin
+000111b0: 653a 0a0a 2e2e 206e 6f74 653a 3a20 5573  e:.... note:: Us
+000111c0: 6520 7a73 7464 2061 7320 6120 7061 7463  e zstd as a patc
+000111d0: 6869 6e67 2065 6e67 696e 650a 0a20 2020  hing engine..   
+000111e0: 205a 7374 6420 6361 6e20 6265 2075 7365   Zstd can be use
+000111f0: 6420 6173 2061 2067 7265 6174 2060 7061  d as a great `pa
+00011200: 7463 6869 6e67 2065 6e67 696e 6520 3c68  tching engine <h
+00011210: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00011220: 6d2f 6661 6365 626f 6f6b 2f7a 7374 642f  m/facebook/zstd/
+00011230: 7769 6b69 2f5a 7374 616e 6461 7264 2d61  wiki/Zstandard-a
+00011240: 732d 612d 7061 7463 6869 6e67 2d65 6e67  s-a-patching-eng
+00011250: 696e 653e 605f 2c20 616c 7468 6f75 6768  ine>`_, although
+00011260: 2069 7420 6861 7320 736f 6d65 206c 696d   it has some lim
+00011270: 6974 6174 696f 6e73 2e0a 0a20 2020 2049  itations...    I
+00011280: 6e20 7468 6973 2070 6172 7469 6375 6c61  n this particula
+00011290: 7220 7363 656e 6172 696f 2c20 7061 7373  r scenario, pass
+000112a0: 203a 7079 3a61 7474 723a 605a 7374 6444   :py:attr:`ZstdD
+000112b0: 6963 742e 6173 5f70 7265 6669 7860 2061  ict.as_prefix` a
+000112c0: 7320 607a 7374 645f 6469 6374 6020 6172  s `zstd_dict` ar
+000112d0: 6775 6d65 6e74 2e20 2250 7265 6669 7822  gument. "Prefix"
+000112e0: 2069 7320 7369 6d69 6c61 7220 746f 2022   is similar to "
+000112f0: 7261 7720 636f 6e74 656e 7422 2064 6963  raw content" dic
+00011300: 7469 6f6e 6172 792c 2062 7574 207a 7374  tionary, but zst
+00011310: 6420 696e 7465 726e 616c 6c79 2068 616e  d internally han
+00011320: 646c 6573 2074 6865 6d20 6469 6666 6572  dles them differ
+00011330: 656e 746c 792c 2073 6565 2060 7468 6973  ently, see `this
+00011340: 2069 7373 7565 203c 6874 7470 733a 2f2f   issue <https://
+00011350: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
+00011360: 6f6f 6b2f 7a73 7464 2f69 7373 7565 732f  ook/zstd/issues/
+00011370: 3238 3335 3e60 5f2e 0a0a 2020 2020 4573  2835>`_...    Es
+00011380: 7365 6e74 6961 6c6c 792c 2070 7265 6669  sentially, prefi
+00011390: 7820 6973 206c 696b 6520 6265 696e 6720  x is like being 
+000113a0: 706c 6163 6564 2062 6566 6f72 6520 7468  placed before th
+000113b0: 6520 6461 7461 2074 6f20 6265 2063 6f6d  e data to be com
+000113c0: 7072 6573 7365 642e 2053 6565 2022 5a53  pressed. See "ZS
+000113d0: 5444 5f63 5f64 6574 6572 6d69 6e69 7374  TD_c_determinist
+000113e0: 6963 5265 6650 7265 6669 7822 2069 6e20  icRefPrefix" in 
+000113f0: 6074 6869 7320 6669 6c65 203c 6874 7470  `this file <http
+00011400: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
+00011410: 6163 6562 6f6f 6b2f 7a73 7464 2f62 6c6f  acebook/zstd/blo
+00011420: 622f 7265 6c65 6173 652f 6c69 622f 7a73  b/release/lib/zs
+00011430: 7464 2e68 3e60 5f2e 0a0a 2020 2020 312c  td.h>`_...    1,
+00011440: 2047 656e 6572 6174 696e 6720 6120 7061   Generating a pa
+00011450: 7463 6820 2863 6f6d 7072 6573 7329 0a0a  tch (compress)..
+00011460: 2020 2020 4173 7375 6d69 6e67 2056 4552      Assuming VER
+00011470: 5f31 2061 6e64 2056 4552 5f32 2061 7265  _1 and VER_2 are
+00011480: 2074 776f 2076 6572 7369 6f6e 732e 0a0a   two versions...
+00011490: 2020 2020 4c65 7420 7468 6520 2277 696e      Let the "win
+000114a0: 646f 7722 2063 6f76 6572 2074 6865 206c  dow" cover the l
+000114b0: 6f6e 6765 7374 2076 6572 7369 6f6e 2c20  ongest version, 
+000114c0: 6279 2073 6574 7469 6e67 203a 7079 3a61  by setting :py:a
+000114d0: 7474 723a 6043 5061 7261 6d65 7465 722e  ttr:`CParameter.
+000114e0: 7769 6e64 6f77 4c6f 6760 2e20 416e 6420  windowLog`. And 
+000114f0: 656e 6162 6c65 2022 6c6f 6e67 2064 6973  enable "long dis
+00011500: 7461 6e63 6520 6d61 7463 6869 6e67 2220  tance matching" 
+00011510: 6279 2073 6574 7469 6e67 203a 7079 3a61  by setting :py:a
+00011520: 7474 723a 6043 5061 7261 6d65 7465 722e  ttr:`CParameter.
+00011530: 656e 6162 6c65 4c6f 6e67 4469 7374 616e  enableLongDistan
+00011540: 6365 4d61 7463 6869 6e67 6020 746f 2031  ceMatching` to 1
+00011550: 2e20 5468 6520 6060 2d2d 7061 7463 682d  . The ``--patch-
+00011560: 6672 6f6d 6060 206f 7074 696f 6e20 6f66  from`` option of
+00011570: 207a 7374 6420 434c 4920 616c 736f 2075   zstd CLI also u
+00011580: 7365 7320 6f74 6865 7220 7061 7261 6d65  ses other parame
+00011590: 7465 7273 2c20 6275 7420 7468 6573 6520  ters, but these 
+000115a0: 7477 6f20 6d61 7474 6572 2074 6865 206d  two matter the m
+000115b0: 6f73 742e 0a0a 2020 2020 5468 6520 7661  ost...    The va
+000115c0: 6c69 6420 7661 6c75 6520 6f66 2060 7769  lid value of `wi
+000115d0: 6e64 6f77 4c6f 6760 2069 7320 5b31 302c  ndowLog` is [10,
+000115e0: 3330 5d20 696e 2033 322d 6269 7420 6275  30] in 32-bit bu
+000115f0: 696c 642c 205b 3130 2c33 315d 2069 6e20  ild, [10,31] in 
+00011600: 3634 2d62 6974 2062 7569 6c64 2e20 536f  64-bit build. So
+00011610: 2069 6e20 3634 2d62 6974 2062 7569 6c64   in 64-bit build
+00011620: 2c20 6974 2068 6173 2061 2060 3247 6942  , it has a `2GiB
+00011630: 206c 656e 6774 6820 6c69 6d69 7420 3c68   length limit <h
+00011640: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00011650: 6d2f 6661 6365 626f 6f6b 2f7a 7374 642f  m/facebook/zstd/
+00011660: 6973 7375 6573 2f32 3137 333e 605f 2e20  issues/2173>`_. 
+00011670: 5374 7269 6374 6c79 2073 7065 616b 696e  Strictly speakin
+00011680: 672c 2074 6865 206c 696d 6974 2069 7320  g, the limit is 
+00011690: 2832 4769 4220 2d20 7e31 3030 4b69 4229  (2GiB - ~100KiB)
+000116a0: 2e20 5768 656e 2074 6869 7320 6c69 6d69  . When this limi
+000116b0: 7420 6973 2065 7863 6565 6465 642c 2074  t is exceeded, t
+000116c0: 6865 2070 6174 6368 2062 6563 6f6d 6573  he patch becomes
+000116d0: 2076 6572 7920 6c61 7267 6520 616e 6420   very large and 
+000116e0: 6c6f 7365 7320 7468 6520 6d65 616e 696e  loses the meanin
+000116f0: 6720 6f66 2061 2070 6174 6368 2e0a 0a20  g of a patch... 
+00011700: 2020 202e 2e20 736f 7572 6365 636f 6465     .. sourcecode
+00011710: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+00011720: 2020 2023 2075 7365 2056 4552 5f31 2061     # use VER_1 a
+00011730: 7320 7072 6566 6978 2e0a 2020 2020 2020  s prefix..      
+00011740: 2020 7631 203d 205a 7374 6444 6963 7428    v1 = ZstdDict(
+00011750: 5645 525f 312c 2069 735f 7261 773d 5472  VER_1, is_raw=Tr
+00011760: 7565 290a 0a20 2020 2020 2020 2023 206c  ue)..        # l
+00011770: 6574 2074 6865 2077 696e 646f 7720 636f  et the window co
+00011780: 7665 7220 7468 6520 6c6f 6e67 6573 7420  ver the longest 
+00011790: 7665 7273 696f 6e2e 0a20 2020 2020 2020  version..       
+000117a0: 2023 2064 6f6e 2774 2066 6f72 6765 7420   # don't forget 
+000117b0: 746f 2063 6c61 6d70 2077 696e 646f 774c  to clamp windowL
+000117c0: 6f67 2074 6f20 7661 6c69 6420 7261 6e67  og to valid rang
+000117d0: 652e 0a20 2020 2020 2020 2023 2065 6e61  e..        # ena
+000117e0: 626c 6520 226c 6f6e 6720 6469 7374 616e  ble "long distan
+000117f0: 6365 206d 6174 6368 696e 6722 2e0a 2020  ce matching"..  
+00011800: 2020 2020 2020 7769 6e64 6f77 4c6f 6720        windowLog 
+00011810: 3d20 6d61 7828 6c65 6e28 5645 525f 3129  = max(len(VER_1)
+00011820: 2c20 6c65 6e28 5645 525f 3229 292e 6269  , len(VER_2)).bi
+00011830: 745f 6c65 6e67 7468 2829 0a20 2020 2020  t_length().     
+00011840: 2020 206f 7074 696f 6e20 3d20 7b43 5061     option = {CPa
+00011850: 7261 6d65 7465 722e 7769 6e64 6f77 4c6f  rameter.windowLo
+00011860: 673a 2077 696e 646f 774c 6f67 2c0a 2020  g: windowLog,.  
+00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011880: 4350 6172 616d 6574 6572 2e65 6e61 626c  CParameter.enabl
+00011890: 654c 6f6e 6744 6973 7461 6e63 654d 6174  eLongDistanceMat
+000118a0: 6368 696e 673a 2031 7d0a 0a20 2020 2020  ching: 1}..     
+000118b0: 2020 2023 2067 6574 2061 2073 6d61 6c6c     # get a small
+000118c0: 2050 4154 4348 0a20 2020 2020 2020 2050   PATCH.        P
+000118d0: 4154 4348 203d 2063 6f6d 7072 6573 7328  ATCH = compress(
+000118e0: 5645 525f 322c 206c 6576 656c 5f6f 725f  VER_2, level_or_
+000118f0: 6f70 7469 6f6e 3d6f 7074 696f 6e2c 207a  option=option, z
+00011900: 7374 645f 6469 6374 3d76 312e 6173 5f70  std_dict=v1.as_p
+00011910: 7265 6669 7829 0a0a 2020 2020 322c 2041  refix)..    2, A
+00011920: 7070 6c79 696e 6720 7468 6520 7061 7463  pplying the patc
+00011930: 6820 2864 6563 6f6d 7072 6573 7329 0a0a  h (decompress)..
+00011940: 2020 2020 5072 6566 6978 2069 7320 6e6f      Prefix is no
+00011950: 7420 6469 6374 696f 6e61 7279 2c20 736f  t dictionary, so
+00011960: 2074 6865 2066 7261 6d65 2068 6561 6465   the frame heade
+00011970: 7220 646f 6573 6e27 7420 7265 636f 7264  r doesn't record
+00011980: 2061 203a 7265 663a 6064 6963 7469 6f6e   a :ref:`diction
+00011990: 6172 7920 6964 3c64 6963 745f 6964 3e60  ary id<dict_id>`
+000119a0: 2e20 5768 656e 2064 6563 6f6d 7072 6573  . When decompres
+000119b0: 7369 6e67 2c20 6d75 7374 2075 7365 2074  sing, must use t
+000119c0: 6865 2073 616d 6520 7072 6566 6978 2061  he same prefix a
+000119d0: 7320 7768 656e 2063 6f6d 7072 6573 7369  s when compressi
+000119e0: 6e67 2e20 4f74 6865 7277 6973 6520 5a73  ng. Otherwise Zs
+000119f0: 7464 4572 726f 7220 6578 6365 7074 696f  tdError exceptio
+00011a00: 6e20 6d61 7920 6265 2072 6169 7365 6420  n may be raised 
+00011a10: 7769 7468 2061 206d 6573 7361 6765 206c  with a message l
+00011a20: 696b 6520 2244 6174 6120 636f 7272 7570  ike "Data corrup
+00011a30: 7469 6f6e 2064 6574 6563 7465 6422 2e0a  tion detected"..
+00011a40: 0a20 2020 2044 6563 6f6d 7072 6573 7369  .    Decompressi
+00011a50: 6e67 2072 6571 7569 7265 7320 6120 7769  ng requires a wi
+00011a60: 6e64 6f77 206f 6620 7468 6520 7361 6d65  ndow of the same
+00011a70: 2073 697a 6520 6173 2077 6865 6e20 636f   size as when co
+00011a80: 6d70 7265 7373 696e 672c 2074 6869 7320  mpressing, this 
+00011a90: 6d61 7920 6265 2061 2070 726f 626c 656d  may be a problem
+00011aa0: 2066 6f72 2073 6d61 6c6c 2052 414d 2064   for small RAM d
+00011ab0: 6576 6963 652e 2049 6620 7468 6520 7769  evice. If the wi
+00011ac0: 6e64 6f77 2069 7320 6c61 7267 6572 2074  ndow is larger t
+00011ad0: 6861 6e20 3132 384d 6942 2c20 6e65 6564  han 128MiB, need
+00011ae0: 2074 6f20 6578 706c 6963 6974 6c79 2073   to explicitly s
+00011af0: 6574 203a 7079 3a61 7474 723a 6044 5061  et :py:attr:`DPa
+00011b00: 7261 6d65 7465 722e 7769 6e64 6f77 4c6f  rameter.windowLo
+00011b10: 674d 6178 6020 746f 2061 6c6c 6f77 206c  gMax` to allow l
+00011b20: 6172 6765 7220 7769 6e64 6f77 2e0a 0a20  arger window... 
+00011b30: 2020 202e 2e20 736f 7572 6365 636f 6465     .. sourcecode
+00011b40: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+00011b50: 2020 2023 2075 7365 2056 4552 5f31 2061     # use VER_1 a
+00011b60: 7320 7072 6566 6978 0a20 2020 2020 2020  s prefix.       
+00011b70: 2076 3120 3d20 5a73 7464 4469 6374 2856   v1 = ZstdDict(V
+00011b80: 4552 5f31 2c20 6973 5f72 6177 3d54 7275  ER_1, is_raw=Tru
+00011b90: 6529 0a0a 2020 2020 2020 2020 2320 616c  e)..        # al
+00011ba0: 6c6f 7720 6c61 7267 6520 7769 6e64 6f77  low large window
+00011bb0: 2c20 7468 6520 6163 7475 616c 2077 696e  , the actual win
+00011bc0: 646f 774c 6f67 2069 7320 6672 6f6d 2066  dowLog is from f
+00011bd0: 7261 6d65 2068 6561 6465 722e 0a20 2020  rame header..   
+00011be0: 2020 2020 206f 7074 696f 6e20 3d20 7b44       option = {D
+00011bf0: 5061 7261 6d65 7465 722e 7769 6e64 6f77  Parameter.window
+00011c00: 4c6f 674d 6178 3a20 3331 7d0a 0a20 2020  LogMax: 31}..   
+00011c10: 2020 2020 2023 2067 6574 2056 4552 5f32       # get VER_2
+00011c20: 2066 726f 6d20 2856 4552 5f31 202b 2050   from (VER_1 + P
+00011c30: 4154 4348 290a 2020 2020 2020 2020 5645  ATCH).        VE
+00011c40: 525f 3220 3d20 6465 636f 6d70 7265 7373  R_2 = decompress
+00011c50: 2850 4154 4348 2c20 7a73 7464 5f64 6963  (PATCH, zstd_dic
+00011c60: 743d 7631 2e61 735f 7072 6566 6978 2c20  t=v1.as_prefix, 
+00011c70: 6f70 7469 6f6e 3d6f 7074 696f 6e29 0a0a  option=option)..
+00011c80: 0a42 7569 6c64 2070 797a 7374 6420 6d6f  .Build pyzstd mo
+00011c90: 6475 6c65 2077 6974 6820 6f70 7469 6f6e  dule with option
+00011ca0: 730a 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  s.>>>>>>>>>>>>>>
+00011cb0: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
+00011cc0: 3e3e 0a0a 2e2e 205f 6275 696c 645f 7079  >>.... _build_py
+00011cd0: 7a73 7464 3a0a 0a2e 2e20 6e6f 7465 3a3a  zstd:.... note::
+00011ce0: 2042 7569 6c64 2070 797a 7374 6420 6d6f   Build pyzstd mo
+00011cf0: 6475 6c65 2077 6974 6820 6f70 7469 6f6e  dule with option
+00011d00: 730a 0a20 2020 2031 efb8 8fe2 83a3 2049  s..    1...... I
+00011d10: 6620 7072 6f76 6964 6520 6060 2d2d 6176  f provide ``--av
+00011d20: 7832 6060 2062 7569 6c64 206f 7074 696f  x2`` build optio
+00011d30: 6e2c 2069 7420 7769 6c6c 2062 7569 6c64  n, it will build
+00011d40: 2077 6974 6820 4156 5832 2f42 4d49 3220   with AVX2/BMI2 
+00011d50: 696e 7374 7275 6374 696f 6e73 2e20 496e  instructions. In
+00011d60: 204d 5356 4320 6275 696c 6420 2873 7461   MSVC build (sta
+00011d70: 7469 6320 6c69 6e6b 292c 2074 6869 7320  tic link), this 
+00011d80: 6272 696e 6773 2073 6f6d 6520 7065 7266  brings some perf
+00011d90: 6f72 6d61 6e63 6520 696d 7072 6f76 656d  ormance improvem
+00011da0: 656e 7473 2e20 4743 432f 434c 414e 4720  ents. GCC/CLANG 
+00011db0: 6275 696c 6473 2061 6c72 6561 6479 2064  builds already d
+00011dc0: 796e 616d 6963 616c 6c79 2064 6973 7061  ynamically dispa
+00011dd0: 7463 6820 736f 6d65 2066 756e 6374 696f  tch some functio
+00011de0: 6e73 2066 6f72 2042 4d49 3220 696e 7374  ns for BMI2 inst
+00011df0: 7275 6374 696f 6e73 2c20 736f 206e 6f20  ructions, so no 
+00011e00: 7369 676e 6966 6963 616e 7420 696d 7072  significant impr
+00011e10: 6f76 656d 656e 742e 0a0a 2020 2020 2e2e  ovement...    ..
+00011e20: 2073 6f75 7263 6563 6f64 653a 3a20 7368   sourcecode:: sh
+00011e30: 656c 6c0a 0a20 2020 2020 2020 2023 20f0  ell..        # .
+00011e40: 9f9f a020 7079 7a73 7464 2030 2e31 352e  ... pyzstd 0.15.
+00011e50: 342b 2061 6e64 2070 6970 2032 322e 312b  4+ and pip 22.1+
+00011e60: 2073 7570 706f 7274 2050 4550 2d35 3137   support PEP-517
+00011e70: 3a0a 2020 2020 2020 2020 2320 6275 696c  :.        # buil
+00011e80: 6420 616e 6420 696e 7374 616c 6c0a 2020  d and install.  
+00011e90: 2020 2020 2020 7069 7020 696e 7374 616c        pip instal
+00011ea0: 6c20 2d2d 636f 6e66 6967 2d73 6574 7469  l --config-setti
+00011eb0: 6e67 733d 222d 2d62 7569 6c64 2d6f 7074  ngs="--build-opt
+00011ec0: 696f 6e3d 2d2d 6176 7832 2220 2d76 2070  ion=--avx2" -v p
+00011ed0: 797a 7374 642d 302e 3135 2e34 2e74 6172  yzstd-0.15.4.tar
+00011ee0: 2e67 7a0a 2020 2020 2020 2020 2320 6275  .gz.        # bu
+00011ef0: 696c 6420 6120 7265 6469 7374 7269 6275  ild a redistribu
+00011f00: 7461 626c 6520 7768 6565 6c0a 2020 2020  table wheel.    
+00011f10: 2020 2020 7069 7020 7768 6565 6c20 2d2d      pip wheel --
+00011f20: 636f 6e66 6967 2d73 6574 7469 6e67 733d  config-settings=
+00011f30: 222d 2d62 7569 6c64 2d6f 7074 696f 6e3d  "--build-option=
+00011f40: 2d2d 6176 7832 2220 2d76 2070 797a 7374  --avx2" -v pyzst
+00011f50: 642d 302e 3135 2e34 2e74 6172 2e67 7a0a  d-0.15.4.tar.gz.
+00011f60: 2020 2020 2020 2020 2320 f09f 9fa0 206c          # .... l
+00011f70: 6567 6163 7920 636f 6d6d 616e 6473 3a0a  egacy commands:.
+00011f80: 2020 2020 2020 2020 2320 6275 696c 6420          # build 
+00011f90: 616e 6420 696e 7374 616c 6c0a 2020 2020  and install.    
+00011fa0: 2020 2020 7079 7468 6f6e 2073 6574 7570      python setup
+00011fb0: 2e70 7920 696e 7374 616c 6c20 2d2d 6176  .py install --av
+00011fc0: 7832 0a20 2020 2020 2020 2023 2062 7569  x2.        # bui
+00011fd0: 6c64 2061 2072 6564 6973 7472 6962 7574  ld a redistribut
+00011fe0: 6162 6c65 2077 6865 656c 0a20 2020 2020  able wheel.     
+00011ff0: 2020 2070 7974 686f 6e20 7365 7475 702e     python setup.
+00012000: 7079 2062 6469 7374 5f77 6865 656c 202d  py bdist_wheel -
+00012010: 2d61 7678 320a 0a20 2020 2032 efb8 8fe2  -avx2..    2....
+00012020: 83a3 2050 797a 7374 6420 6d6f 6475 6c65  .. Pyzstd module
+00012030: 2073 7570 706f 7274 733a 0a0a 2020 2020   supports:..    
+00012040: 2020 2020 2a20 4479 6e61 6d69 6361 6c6c      * Dynamicall
+00012050: 7920 6c69 6e6b 2074 6f20 7a73 7464 206c  y link to zstd l
+00012060: 6962 7261 7279 2028 7072 6f76 6964 6564  ibrary (provided
+00012070: 2062 7920 7379 7374 656d 206f 7220 6120   by system or a 
+00012080: 444c 4c20 6c69 6272 6172 7929 2c20 7468  DLL library), th
+00012090: 656e 2074 6865 207a 7374 6420 736f 7572  en the zstd sour
+000120a0: 6365 2063 6f64 6520 696e 2060 607a 7374  ce code in ``zst
+000120b0: 6460 6020 666f 6c64 6572 2077 696c 6c20  d`` folder will 
+000120c0: 6265 2069 676e 6f72 6564 2e0a 2020 2020  be ignored..    
+000120d0: 2020 2020 2a20 5072 6f76 6964 6520 6120      * Provide a 
+000120e0: 6043 4646 4920 3c68 7474 7073 3a2f 2f64  `CFFI <https://d
+000120f0: 6f63 2e70 7970 792e 6f72 672f 656e 2f6c  oc.pypy.org/en/l
+00012100: 6174 6573 742f 6578 7465 6e64 696e 672e  atest/extending.
+00012110: 6874 6d6c 2363 6666 693e 605f 2069 6d70  html#cffi>`_ imp
+00012120: 6c65 6d65 6e74 6174 696f 6e20 7468 6174  lementation that
+00012130: 2063 616e 2077 6f72 6b20 7769 7468 2050   can work with P
+00012140: 7950 792e 0a0a 2020 2020 4f6e 2043 5079  yPy...    On CPy
+00012150: 7468 6f6e 2c20 7072 6f76 6964 6520 7468  thon, provide th
+00012160: 6573 6520 6275 696c 6420 6f70 7469 6f6e  ese build option
+00012170: 733a 0a0a 2020 2020 2020 2020 232e 206e  s:..        #. n
+00012180: 6f20 6f70 7469 6f6e 3a20 4320 696d 706c  o option: C impl
+00012190: 656d 656e 7461 7469 6f6e 2c20 7374 6174  ementation, stat
+000121a0: 6963 616c 6c79 206c 696e 6b20 746f 207a  ically link to z
+000121b0: 7374 6420 6c69 6272 6172 792e 0a20 2020  std library..   
+000121c0: 2020 2020 2023 2e20 6060 2d2d 6479 6e61       #. ``--dyna
+000121d0: 6d69 632d 6c69 6e6b 2d7a 7374 6460 603a  mic-link-zstd``:
+000121e0: 2043 2069 6d70 6c65 6d65 6e74 6174 696f   C implementatio
+000121f0: 6e2c 2064 796e 616d 6963 616c 6c79 206c  n, dynamically l
+00012200: 696e 6b20 746f 207a 7374 6420 6c69 6272  ink to zstd libr
+00012210: 6172 792e 0a20 2020 2020 2020 2023 2e20  ary..        #. 
+00012220: 6060 2d2d 6366 6669 6060 3a20 4346 4649  ``--cffi``: CFFI
+00012230: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00012240: 2873 6c6f 7765 7229 2c20 7374 6174 6963  (slower), static
+00012250: 616c 6c79 206c 696e 6b20 746f 207a 7374  ally link to zst
+00012260: 6420 6c69 6272 6172 792e 0a20 2020 2020  d library..     
+00012270: 2020 2023 2e20 6060 2d2d 6366 6669 202d     #. ``--cffi -
+00012280: 2d64 796e 616d 6963 2d6c 696e 6b2d 7a73  -dynamic-link-zs
+00012290: 7464 6060 3a20 4346 4649 2069 6d70 6c65  td``: CFFI imple
+000122a0: 6d65 6e74 6174 696f 6e20 2873 6c6f 7765  mentation (slowe
+000122b0: 7229 2c20 6479 6e61 6d69 6361 6c6c 7920  r), dynamically 
+000122c0: 6c69 6e6b 2074 6f20 7a73 7464 206c 6962  link to zstd lib
+000122d0: 7261 7279 2e0a 0a20 2020 204f 6e20 5079  rary...    On Py
+000122e0: 5079 2c20 6f6e 6c79 2043 4646 4920 696d  Py, only CFFI im
+000122f0: 706c 656d 656e 7461 7469 6f6e 2063 616e  plementation can
+00012300: 2062 6520 7573 6564 2c20 736f 2060 602d   be used, so ``-
+00012310: 2d63 6666 6960 6020 6973 2061 6464 6564  -cffi`` is added
+00012320: 2069 6d70 6c69 6369 746c 792e 2060 602d   implicitly. ``-
+00012330: 2d64 796e 616d 6963 2d6c 696e 6b2d 7a73  -dynamic-link-zs
+00012340: 7464 6060 2069 7320 6f70 7469 6f6e 616c  td`` is optional
+00012350: 2e0a 0a20 2020 202e 2e20 736f 7572 6365  ...    .. source
+00012360: 636f 6465 3a3a 2073 6865 6c6c 0a0a 2020  code:: shell..  
+00012370: 2020 2020 2020 2320 f09f 9fa0 2070 797a        # .... pyz
+00012380: 7374 6420 302e 3135 2e34 2b20 616e 6420  std 0.15.4+ and 
+00012390: 7069 7020 3232 2e31 2b20 7375 7070 6f72  pip 22.1+ suppor
+000123a0: 7420 5045 502d 3531 373a 0a20 2020 2020  t PEP-517:.     
+000123b0: 2020 2023 2062 7569 6c64 2061 6e64 2069     # build and i
+000123c0: 6e73 7461 6c6c 0a20 2020 2020 2020 2070  nstall.        p
+000123d0: 6970 3320 696e 7374 616c 6c20 2d2d 636f  ip3 install --co
+000123e0: 6e66 6967 2d73 6574 7469 6e67 733d 222d  nfig-settings="-
+000123f0: 2d62 7569 6c64 2d6f 7074 696f 6e3d 2d2d  -build-option=--
+00012400: 6479 6e61 6d69 632d 6c69 6e6b 2d7a 7374  dynamic-link-zst
+00012410: 6422 202d 7620 7079 7a73 7464 2d30 2e31  d" -v pyzstd-0.1
+00012420: 352e 342e 7461 722e 677a 0a20 2020 2020  5.4.tar.gz.     
+00012430: 2020 2023 2062 7569 6c64 2061 2072 6564     # build a red
+00012440: 6973 7472 6962 7574 6162 6c65 2077 6865  istributable whe
+00012450: 656c 0a20 2020 2020 2020 2070 6970 3320  el.        pip3 
+00012460: 7768 6565 6c20 2d2d 636f 6e66 6967 2d73  wheel --config-s
+00012470: 6574 7469 6e67 733d 222d 2d62 7569 6c64  ettings="--build
+00012480: 2d6f 7074 696f 6e3d 2d2d 6479 6e61 6d69  -option=--dynami
+00012490: 632d 6c69 6e6b 2d7a 7374 6422 202d 7620  c-link-zstd" -v 
+000124a0: 7079 7a73 7464 2d30 2e31 352e 342e 7461  pyzstd-0.15.4.ta
+000124b0: 722e 677a 0a20 2020 2020 2020 2023 2073  r.gz.        # s
+000124c0: 7065 6369 6679 206d 6f72 6520 7468 616e  pecify more than
+000124d0: 206f 6e65 206f 7074 696f 6e0a 2020 2020   one option.    
+000124e0: 2020 2020 7069 7033 2077 6865 656c 202d      pip3 wheel -
+000124f0: 2d63 6f6e 6669 672d 7365 7474 696e 6773  -config-settings
+00012500: 3d22 2d2d 6275 696c 642d 6f70 7469 6f6e  ="--build-option
+00012510: 3d2d 2d64 796e 616d 6963 2d6c 696e 6b2d  =--dynamic-link-
+00012520: 7a73 7464 202d 2d63 6666 6922 202d 7620  zstd --cffi" -v 
+00012530: 7079 7a73 7464 2d30 2e31 352e 342e 7461  pyzstd-0.15.4.ta
+00012540: 722e 677a 0a20 2020 2020 2020 2023 20f0  r.gz.        # .
+00012550: 9f9f a020 6c65 6761 6379 2063 6f6d 6d61  ... legacy comma
+00012560: 6e64 733a 0a20 2020 2020 2020 2023 2062  nds:.        # b
+00012570: 7569 6c64 2061 6e64 2069 6e73 7461 6c6c  uild and install
+00012580: 0a20 2020 2020 2020 2070 7974 686f 6e33  .        python3
+00012590: 2073 6574 7570 2e70 7920 696e 7374 616c   setup.py instal
+000125a0: 6c20 2d2d 6479 6e61 6d69 632d 6c69 6e6b  l --dynamic-link
+000125b0: 2d7a 7374 640a 2020 2020 2020 2020 2320  -zstd.        # 
+000125c0: 6275 696c 6420 6120 7265 6469 7374 7269  build a redistri
+000125d0: 6275 7461 626c 6520 7768 6565 6c0a 2020  butable wheel.  
+000125e0: 2020 2020 2020 7079 7468 6f6e 3320 7365        python3 se
+000125f0: 7475 702e 7079 2062 6469 7374 5f77 6865  tup.py bdist_whe
+00012600: 656c 202d 2d64 796e 616d 6963 2d6c 696e  el --dynamic-lin
+00012610: 6b2d 7a73 7464 0a0a 2020 2020 536f 6d65  k-zstd..    Some
+00012620: 206e 6f74 6573 3a0a 0a20 2020 2020 2020   notes:..       
+00012630: 202a 2054 6865 2077 6865 656c 7320 6f6e   * The wheels on
+00012640: 2060 5079 5049 203c 6874 7470 733a 2f2f   `PyPI <https://
+00012650: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00012660: 2f70 797a 7374 643e 605f 2075 7365 2073  /pyzstd>`_ use s
+00012670: 7461 7469 6320 6c69 6e6b 696e 672c 2074  tatic linking, t
+00012680: 6865 2070 6163 6b61 6765 7320 6f6e 2060  he packages on `
+00012690: 416e 6163 6f6e 6461 203c 6874 7470 733a  Anaconda <https:
+000126a0: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f63  //anaconda.org/c
+000126b0: 6f6e 6461 2d66 6f72 6765 2f70 797a 7374  onda-forge/pyzst
+000126c0: 643e 605f 2075 7365 2064 796e 616d 6963  d>`_ use dynamic
+000126d0: 206c 696e 6b69 6e67 2e0a 2020 2020 2020   linking..      
+000126e0: 2020 2a20 4e6f 206d 6174 7465 7220 7374    * No matter st
+000126f0: 6174 6963 206f 7220 6479 6e61 6d69 6320  atic or dynamic 
+00012700: 6c69 6e6b 696e 672c 2070 797a 7374 6420  linking, pyzstd 
+00012710: 6d6f 6475 6c65 2072 6571 7569 7265 7320  module requires 
+00012720: 7a73 7464 2076 312e 342e 302b 2e0a 2020  zstd v1.4.0+..  
+00012730: 2020 2020 2020 2a20 5374 6174 6963 206c        * Static l
+00012740: 696e 6b69 6e67 3a20 5573 6520 7a73 7464  inking: Use zstd
+00012750: 2773 206f 6666 6963 6961 6c20 7265 6c65  's official rele
+00012760: 6173 6520 7769 7468 6f75 7420 616e 7920  ase without any 
+00012770: 6368 616e 6765 2e20 4966 2077 616e 7420  change. If want 
+00012780: 746f 2075 7067 7261 6465 206f 7220 646f  to upgrade or do
+00012790: 776e 6772 6164 6520 7468 6520 7a73 7464  wngrade the zstd
+000127a0: 206c 6962 7261 7279 2c20 6a75 7374 2072   library, just r
+000127b0: 6570 6c61 6365 2060 607a 7374 6460 6020  eplace ``zstd`` 
+000127c0: 666f 6c64 6572 2e0a 2020 2020 2020 2020  folder..        
+000127d0: 2a20 4479 6e61 6d69 6320 6c69 6e6b 696e  * Dynamic linkin
+000127e0: 673a 2049 6620 6e65 7720 7a73 7464 2041  g: If new zstd A
+000127f0: 5049 2069 7320 7573 6564 2061 7420 636f  PI is used at co
+00012800: 6d70 696c 652d 7469 6d65 2c20 6c69 6e6b  mpile-time, link
+00012810: 696e 6720 746f 206c 6f77 6572 2076 6572  ing to lower ver
+00012820: 7369 6f6e 2072 756e 2d74 696d 6520 7a73  sion run-time zs
+00012830: 7464 206c 6962 7261 7279 2077 696c 6c20  td library will 
+00012840: 6661 696c 2e20 5573 6520 7631 2e35 2e30  fail. Use v1.5.0
+00012850: 206e 6577 2041 5049 2069 6620 706f 7373   new API if poss
+00012860: 6962 6c65 2e0a 0a20 2020 204f 6e20 5769  ible...    On Wi
+00012870: 6e64 6f77 732c 2074 6865 7265 2069 7320  ndows, there is 
+00012880: 6e6f 2073 7973 7465 6d2d 7769 6465 207a  no system-wide z
+00012890: 7374 6420 6c69 6272 6172 792e 2050 797a  std library. Pyz
+000128a0: 7374 6420 6d6f 6475 6c65 2063 616e 2064  std module can d
+000128b0: 796e 616d 6963 616c 6c79 206c 696e 6b20  ynamically link 
+000128c0: 746f 2061 2044 4c4c 206c 6962 7261 7279  to a DLL library
+000128d0: 2c20 6d6f 6469 6679 2060 6073 6574 7570  , modify ``setup
+000128e0: 2e70 7960 603a 0a0a 2020 2020 2e2e 2073  .py``:..    .. s
+000128f0: 6f75 7263 6563 6f64 653a 3a20 7079 7468  ourcecode:: pyth
+00012900: 6f6e 0a0a 2020 2020 2020 2020 2320 453a  on..        # E:
+00012910: 5c7a 7374 645f 646c 6c20 666f 6c64 6572  \zstd_dll folder
+00012920: 2068 6173 207a 7374 642e 6820 2f20 7a64   has zstd.h / zd
+00012930: 6963 742e 6820 2f20 6c69 627a 7374 642e  ict.h / libzstd.
+00012940: 6c69 6220 7468 6174 0a20 2020 2020 2020  lib that.       
+00012950: 2023 2061 6c6f 6e67 2077 6974 6820 6c69   # along with li
+00012960: 627a 7374 642e 646c 6c0a 2020 2020 2020  bzstd.dll.      
+00012970: 2020 6966 2044 594e 414d 4943 5f4c 494e    if DYNAMIC_LIN
+00012980: 4b3a 0a20 2020 2020 2020 2020 2020 206b  K:.            k
+00012990: 7761 7267 7320 3d20 7b0a 2020 2020 2020  wargs = {.      
+000129a0: 2020 2020 2020 2769 6e63 6c75 6465 5f64        'include_d
+000129b0: 6972 7327 3a20 5b27 453a 5c7a 7374 645f  irs': ['E:\zstd_
+000129c0: 646c 6c27 5d2c 2023 202e 6820 6469 7265  dll'], # .h dire
+000129d0: 6374 6f72 790a 2020 2020 2020 2020 2020  ctory.          
+000129e0: 2020 276c 6962 7261 7279 5f64 6972 7327    'library_dirs'
+000129f0: 3a20 5b27 453a 5c7a 7374 645f 646c 6c27  : ['E:\zstd_dll'
+00012a00: 5d2c 2023 202e 6c69 6220 6469 7265 6374  ], # .lib direct
+00012a10: 6f72 790a 2020 2020 2020 2020 2020 2020  ory.            
+00012a20: 276c 6962 7261 7269 6573 273a 205b 276c  'libraries': ['l
+00012a30: 6962 7a73 7464 275d 2c20 2020 2020 2020  ibzstd'],       
+00012a40: 2023 206c 6962 206e 616d 652c 206e 6f74   # lib name, not
+00012a50: 2066 696c 656e 616d 652c 2066 6f72 2074   filename, for t
+00012a60: 6865 206c 696e 6b65 722e 0a20 2020 2020  he linker..     
+00012a70: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
+00012a80: 416e 6420 7075 7420 6060 6c69 627a 7374  And put ``libzst
+00012a90: 642e 646c 6c60 6020 696e 746f 206f 6e65  d.dll`` into one
+00012aa0: 206f 6620 7468 6573 6520 6469 7265 6374   of these direct
+00012ab0: 6f72 6965 733a 0a0a 2020 2020 2020 2020  ories:..        
+00012ac0: 2a20 4469 7265 6374 6f72 7920 6164 6465  * Directory adde
+00012ad0: 6420 6279 2060 6f73 2e61 6464 5f64 6c6c  d by `os.add_dll
+00012ae0: 5f64 6972 6563 746f 7279 2829 203c 6874  _directory() <ht
+00012af0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00012b00: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00012b10: 6f73 2e68 746d 6c23 6f73 2e61 6464 5f64  os.html#os.add_d
+00012b20: 6c6c 5f64 6972 6563 746f 7279 3e60 5f20  ll_directory>`_ 
+00012b30: 6675 6e63 7469 6f6e 2e20 2854 6865 2075  function. (The u
+00012b40: 6e69 742d 7465 7374 7320 616e 6420 7468  nit-tests and th
+00012b50: 6520 434c 4920 6361 6e27 7420 7574 696c  e CLI can't util
+00012b60: 697a 6520 7468 6973 290a 2020 2020 2020  ize this).      
+00012b70: 2020 2a20 5079 7468 6f6e 2773 2072 6f6f    * Python's roo
+00012b80: 7420 6469 7265 6374 6f72 7920 7468 6174  t directory that
+00012b90: 2068 6173 2070 7974 686f 6e2e 6578 652e   has python.exe.
+00012ba0: 0a20 2020 2020 2020 202a 2025 5379 7374  .        * %Syst
+00012bb0: 656d 526f 6f74 255c 5379 7374 656d 3332  emRoot%\System32
+00012bc0: 0a0a 2020 2020 4e6f 7465 2074 6861 7420  ..    Note that 
+00012bd0: 7468 6520 6162 6f76 6520 6c69 7374 2064  the above list d
+00012be0: 6f65 736e 2774 2069 6e63 6c75 6465 2074  oesn't include t
+00012bf0: 6865 2063 7572 7265 6e74 2077 6f72 6b69  he current worki
+00012c00: 6e67 2064 6972 6563 746f 7279 2061 6e64  ng directory and
+00012c10: 2025 5041 5448 2520 6469 7265 6374 6f72   %PATH% director
+00012c20: 6965 732e 0a0a 2020 2020 33ef b88f e283  ies...    3.....
+00012c30: a320 5573 6520 226d 756c 7469 2d70 6861  . Use "multi-pha
+00012c40: 7365 2069 6e69 7469 616c 697a 6174 696f  se initializatio
+00012c50: 6e22 206f 6e20 4350 7974 686f 6e2e 0a0a  n" on CPython...
+00012c60: 2020 2020 4966 2070 726f 7669 6465 2060      If provide `
+00012c70: 602d 2d6d 756c 7469 2d70 6861 7365 2d69  `--multi-phase-i
+00012c80: 6e69 7460 6020 6275 696c 6420 6f70 7469  nit`` build opti
+00012c90: 6f6e 2c20 6974 2077 696c 6c20 6275 696c  on, it will buil
+00012ca0: 6420 7769 7468 2022 6d75 6c74 692d 7068  d with "multi-ph
+00012cb0: 6173 6520 696e 6974 6961 6c69 7a61 7469  ase initializati
+00012cc0: 6f6e 2220 2860 5045 502d 3438 3920 3c68  on" (`PEP-489 <h
+00012cd0: 7474 7073 3a2f 2f70 6570 732e 7079 7468  ttps://peps.pyth
+00012ce0: 6f6e 2e6f 7267 2f70 6570 2d30 3438 392f  on.org/pep-0489/
+00012cf0: 3e60 5f29 206f 6e20 4350 7974 686f 6e20  >`_) on CPython 
+00012d00: 332e 3131 2b2e 0a0a 2020 2020 5369 6e63  3.11+...    Sinc
+00012d10: 6520 6974 2061 6464 7320 6120 7469 6e79  e it adds a tiny
+00012d20: 206f 7665 7268 6561 642c 2069 7427 7320   overhead, it's 
+00012d30: 6469 7361 626c 6564 2062 7920 6465 6661  disabled by defa
+00012d40: 756c 742e 2049 7420 6361 6e20 6265 2065  ult. It can be e
+00012d50: 6e61 626c 6564 2061 6674 6572 2043 5079  nabled after CPy
+00012d60: 7468 6f6e 2773 2060 7375 622d 696e 7465  thon's `sub-inte
+00012d70: 7270 7265 7465 7273 203c 6874 7470 733a  rpreters <https:
+00012d80: 2f2f 7065 7073 2e70 7974 686f 6e2e 6f72  //peps.python.or
+00012d90: 672f 7065 702d 3035 3534 2f3e 605f 2069  g/pep-0554/>`_ i
+00012da0: 7320 6d61 7475 7265 2e0a                 s mature..
```

### Comparing `pyzstd-0.15.6/pyzstd.egg-info/PKG-INFO` & `pyzstd-0.15.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pyzstd
-Version: 0.15.6
+Version: 0.15.7
 Summary: Python bindings to Zstandard (zstd) compression library, the API style is similar to Python's bz2/lzma/zlib modules.
 Home-page: https://github.com/animalize/pyzstd
 Author: Ma Lin
 Author-email: malincns@163.com
 License: The 3-Clause BSD License
 Keywords: zstandard zstd compression decompression compress decompress
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Archiving :: Compression
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
@@ -41,77 +43,87 @@
 Documentation: https://pyzstd.readthedocs.io/en/latest
 
 GitHub: https://github.com/animalize/pyzstd
 
 
 Release note
 ------------
+**0.15.7  (Apr 21, 2023)**
+
+ZstdDict class changes:
+
+#. Fix these advanced compression parameters may be ignored when loading a dictionary: ``windowLog``, ``hashLog``, ``chainLog``, ``searchLog``, ``minMatch``, ``targetLength``, ``strategy``, ``enableLongDistanceMatching``, ``ldmHashLog``, ``ldmMinMatch``, ``ldmBucketSizeLog``, ``ldmHashRateLog``, and some non-public parameters.
+
+#. When compressing, load undigested dictionary instead of digested dictionary by default. Loading again an undigested is slower, see `differences <https://pyzstd.readthedocs.io/en/latest/#ZstdDict.as_digested_dict>`_.
+
+#. Add `.as_prefix <https://pyzstd.readthedocs.io/en/latest/#ZstdDict.as_prefix>`_ attribute. Can use zstd as a `patching engine <https://pyzstd.readthedocs.io/en/latest/#patching-engine>`_.
+
 **0.15.6  (Apr 5, 2023)**
 
-Update bundled zstd source code from v1.5.4 to `v1.5.5 <https://github.com/facebook/zstd/releases/tag/v1.5.5>`_.
+Upgrade zstd source code from v1.5.4 to `v1.5.5 <https://github.com/facebook/zstd/releases/tag/v1.5.5>`_.
 
 **0.15.4  (Feb 24, 2023)**
 
-#. Update bundled zstd source code from v1.5.2 to `v1.5.4 <https://github.com/facebook/zstd/releases/tag/v1.5.4>`_. v1.5.3 is a non-public release.
+#. Upgrade zstd source code from v1.5.2 to `v1.5.4 <https://github.com/facebook/zstd/releases/tag/v1.5.4>`_. v1.5.3 is a non-public release.
 
-#. Support ``pyproject.toml`` build mechanism (PEP-517). Note that specifying build options in old way may be invalid, see `doc <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
+#. Support ``pyproject.toml`` build mechanism (PEP-517). Note that specifying build options in old way may be invalid, see `build commands <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
 
 #. Support "multi-phase initialization" (PEP-489) on CPython 3.11+, can work with CPython sub-interpreters in the future. Currently this build option is disabled by default.
 
 #. Add a command line interface (CLI).
 
 **0.15.3  (Aug 3, 2022)**
 
 Fix ``ZstdError`` object can't be pickled.
 
 **0.15.2  (Jan 22, 2022)**
 
-Update bundled zstd source code from v1.5.1 to `v1.5.2 <https://github.com/facebook/zstd/releases/tag/v1.5.2>`_.
+Upgrade zstd source code from v1.5.1 to `v1.5.2 <https://github.com/facebook/zstd/releases/tag/v1.5.2>`_.
 
 **0.15.1  (Dec 25, 2021)**
 
-#. Update bundled zstd source code from v1.5.0 to `v1.5.1 <https://github.com/facebook/zstd/releases/tag/v1.5.1>`_.
+#. Upgrade zstd source code from v1.5.0 to `v1.5.1 <https://github.com/facebook/zstd/releases/tag/v1.5.1>`_.
 
 #. Fix ``ZstdFile.write()`` / ``train_dict()`` / ``finalize_dict()`` may use wrong length for some buffer protocol objects, see `this issue <https://github.com/animalize/pyzstd/issues/4>`_.
 
 #. Two behavior changes:
 
     * Setting ``CParameter.nbWorkers`` to ``1`` now means "1-thread multi-threaded mode", rather than "single-threaded mode".
 
     * If the underlying zstd library doesn't support multi-threaded compression, no longer automatically fallback to "single-threaded mode", now raise a ``ZstdError`` exception.
 
 #. Add a module level variable `zstd_support_multithread <https://pyzstd.readthedocs.io/en/latest/#zstd_support_multithread>`_.
 
-#. Add a setup.py option ``--avx2``, see `this note <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
+#. Add a setup.py option ``--avx2``, see `build options <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
 
 **0.15.0  (May 18, 2021)**
 
-#. Update bundled zstd source code from v1.4.9 to `v1.5.0 <https://github.com/facebook/zstd/releases/tag/v1.5.0>`_.
+#. Upgrade zstd source code from v1.4.9 to `v1.5.0 <https://github.com/facebook/zstd/releases/tag/v1.5.0>`_.
 
 #. Some improvements, no API changes.
 
 **0.14.4  (Mar 24, 2021)**
 
 #. Add a CFFI implementation that can work with PyPy.
 
 #. Allow dynamically link to zstd library.
 
 **0.14.3  (Mar 4, 2021)**
 
-Update bundled zstd source code from v1.4.8 to `v1.4.9 <https://github.com/facebook/zstd/releases/tag/v1.4.9>`_.
+Upgrade zstd source code from v1.4.8 to `v1.4.9 <https://github.com/facebook/zstd/releases/tag/v1.4.9>`_.
 
 **0.14.2  (Feb 24, 2021)**
 
 #. Add two convenient functions: `compress_stream() <https://pyzstd.readthedocs.io/en/latest/#compress_stream>`_, `decompress_stream() <https://pyzstd.readthedocs.io/en/latest/#decompress_stream>`_.
 
 #. Some improvements.
 
 **0.14.1  (Dec 19, 2020)**
 
-#. Update bundled zstd source code from v1.4.5 to `v1.4.8 <https://github.com/facebook/zstd/releases/tag/v1.4.8>`_.
+#. Upgrade zstd source code from v1.4.5 to `v1.4.8 <https://github.com/facebook/zstd/releases/tag/v1.4.8>`_.
 
     * v1.4.6 is a non-public release for Linux kernel.
 
     * v1.4.8 is a hotfix for `v1.4.7 <https://github.com/facebook/zstd/releases/tag/v1.4.7>`_.
 
 #. Some improvements, no API changes.
```

### Comparing `pyzstd-0.15.6/pyzstd.egg-info/SOURCES.txt` & `pyzstd-0.15.7/pyzstd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/setup.py` & `pyzstd-0.15.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,34 +45,43 @@
     else:
         return False
 
 class pyzstd_build_ext(build_ext):
     PYZSTD_AVX2 = False
     PYZSTD_DEBUG = False
     PYZSTD_WARNING_AS_ERROR = False
+    PYZSTD_CONFIG_MSG = ''
 
     def build_extensions(self):
+        # Print build config message in actual build
+        print(self.PYZSTD_CONFIG_MSG, flush=True)
+
         # Accept assembly files
         self.compiler.src_extensions.extend(['.s', '.S'])
         # Build debug build
         self.debug = self.PYZSTD_DEBUG
 
         for extension in self.extensions:
             if self.compiler.compiler_type in ('unix', 'mingw32', 'cygwin'):
                 # -g0:
                 #   Level 0 produces no debug information at all. This reduces
                 #   the size of GCC wheels. By default CPython won't print any
                 #   C stack trace, so -g0 and -g2 are same for most users.
-                more_options = ['-g0']
+                # -flto:
+                #   This option runs the standard link-time optimizer. To use the
+                #   link-time optimizer, -flto and optimization options should be
+                #   specified at compile time and during the final link.
+                more_options = ['-g0', '-flto']
                 if self.PYZSTD_AVX2:
                     instrs = ['-mavx2', '-mbmi', '-mbmi2', '-mlzcnt']
                     more_options.extend(instrs)
                 if self.PYZSTD_WARNING_AS_ERROR:
                     more_options.append('-Werror')
                 extension.extra_compile_args.extend(more_options)
+                extension.extra_link_args.extend(['-g0', '-flto'])
             elif self.compiler.compiler_type == 'msvc':
                 # Remove .S source files, they use gcc/clang syntax.
                 extension.sources = [i for i in extension.sources
                                         if not fnmatch.fnmatch(i, '*.[sS]')]
 
                 # /Ob3: More aggressive inlining than /Ob2.
                 # /GF:  Eliminates duplicate strings.
@@ -85,40 +94,73 @@
                     more_options.append('/arch:AVX2')
                 if self.PYZSTD_WARNING_AS_ERROR:
                     more_options.append('/WX')
                 extension.extra_compile_args.extend(more_options)
         super().build_extensions()
 
 def do_setup():
+    # read stuff
     long_description, module_version = read_stuff()
 
+    # parse options
     pyzstd_build_ext.PYZSTD_AVX2 = has_option('--avx2')
     pyzstd_build_ext.PYZSTD_DEBUG = has_option('--debug')
     pyzstd_build_ext.PYZSTD_WARNING_AS_ERROR = has_option('--warning-as-error')
 
     DYNAMIC_LINK = has_option('--dynamic-link-zstd')
     CFFI = has_option('--cffi') or platform.python_implementation() == 'PyPy'
     MULTI_PHASE_INIT = has_option('--multi-phase-init')
 
+    # build config message
+    pyzstd_build_ext.PYZSTD_CONFIG_MSG = \
+               ('+--------------------------------------------+\n'
+                '|             Pyzstd build config            |\n'
+                '+-------------------------+------------------+\n'
+                '| Pyzstd version          | {!s:<16} |\n'
+                '+-------------------------+------------------+\n'
+                '| Implementation          | {!s:<16} |\n'
+                '+-------------------------+------------------+\n'
+                '| Enable multi-phase-init | {!s:<16} |\n'
+                '+-------------------------+------------------+\n'
+                '| Link to zstd library    | {!s:<16} |\n'
+                '+-------------------------+------------------+\n'
+                '| Enable AVX2/BMI2        | {!s:<16} |\n'
+                '+-------------------------+------------------+\n'
+                '| Debug build             | {!s:<16} |\n'
+                '+-------------------------+------------------+\n'
+                '| Warning as error        | {!s:<16} |\n'
+                '+-------------------------+------------------+').format(
+                    module_version,
+                    'CFFI' if CFFI else 'C',
+                    'Not for CFFI' if CFFI else MULTI_PHASE_INIT,
+                    'Dynamically link' if DYNAMIC_LINK else 'Statically link',
+                    pyzstd_build_ext.PYZSTD_AVX2,
+                    pyzstd_build_ext.PYZSTD_DEBUG,
+                    pyzstd_build_ext.PYZSTD_WARNING_AS_ERROR)
+
     if DYNAMIC_LINK:
         kwargs = {
             'include_dirs': [],    # .h directory
             'library_dirs': [],    # .lib directory
             'libraries': ['zstd'], # lib name, not filename, for the linker.
             'sources': [],
             'define_macros': []
         }
     else:  # statically link to zstd lib
         kwargs = {
-            'include_dirs': ['zstd/lib', 'zstd/lib/dictBuilder'],
+            'include_dirs': ['zstd/lib',
+                             # for zstd 1.4.x:
+                             'zstd/lib/common',
+                             'zstd/lib/dictBuilder'],
             'library_dirs': [],
             'libraries': [],
             'sources': get_zstd_files_list(),
-            'define_macros': [('ZSTD_MULTITHREAD', None),
-                              ('PYZSTD_STATIC_LINK', None)]
+            'define_macros': [('PYZSTD_STATIC_LINK', None),
+                              # enable multi-threaded compression
+                              ('ZSTD_MULTITHREAD', None)]
         }
 
     if CFFI:
         # packages
         packages = ['pyzstd', 'pyzstd.cffi']
 
         # binary extension
@@ -139,16 +181,17 @@
             kwargs['define_macros'].append(('USE_MULTI_PHASE_INIT', None))
 
         binary_extension = Extension(**kwargs)
 
     setup(
         name='pyzstd',
         version=module_version,
-        description=("Python bindings to Zstandard (zstd) compression library, "
-                     "the API style is similar to Python's bz2/lzma/zlib modules."),
+        description=("Python bindings to Zstandard (zstd) compression "
+                     "library, the API style is similar to Python's "
+                     "bz2/lzma/zlib modules."),
         long_description=long_description,
         long_description_content_type='text/x-rst',
         author='Ma Lin',
         author_email='malincns@163.com',
         url='https://github.com/animalize/pyzstd',
         license='The 3-Clause BSD License',
         python_requires='>=3.5',
@@ -156,14 +199,16 @@
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Developers",
             "Topic :: System :: Archiving :: Compression",
             "License :: OSI Approved :: BSD License",
             "Programming Language :: Python :: Implementation :: CPython",
             "Programming Language :: Python :: Implementation :: PyPy",
+            "Programming Language :: Python :: 3.5",
+            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
         ],
         keywords='zstandard zstd compression decompression compress decompress',
```

### Comparing `pyzstd-0.15.6/src/__init__.py` & `pyzstd-0.15.7/src/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,23 @@
     try:
         # Import CFFI implementation
         from .cffi.cffi_pyzstd import *
         from .cffi.cffi_pyzstd import _train_dict, _finalize_dict, \
                                       _ZSTD_DStreamInSize
     except ImportError:
         raise ImportError(
-            "pyzstd module: Neither C implementation nor CFFI implementation "
-            "can be imported. If pyzstd module is dynamically linked to zstd "
-            "library, make sure not to remove zstd library, and the run-time "
-            "zstd library's version can't be lower than that at compile-time.")
+            "\n\npyzstd module: Can't import compiled .so/.pyd file.\n"
+            "1, If pyzstd module is dynamically linked to zstd library: Make sure\n"
+            "   not to remove zstd library, and the run-time zstd library's version\n"
+            "   can't be lower than that at compile-time; On Windows, the directory\n"
+            "   that has libzstd.dll should be added by os.add_dll_directory() function.\n"
+            "2, Please install pyzstd module through pip, to ensure that compiled\n"
+            "   .so/.pyd file matches the architecture/OS/Python.\n")
 
-__version__ = '0.15.6'
+__version__ = '0.15.7'
 
 __doc__ = '''\
 Python bindings to Zstandard (zstd) compression library, the API style is
 similar to Python's bz2/lzma/zlib modules.
 
 Command line interface of this module: python -m pyzstd --help
 
@@ -324,17 +327,14 @@
         zstd_dict: A ZstdDict object, pre-trained dictionary for compression /
             decompression.
         """
         self._fp = None
         self._closefp = False
         self._mode = _MODE_CLOSED
 
-        if not isinstance(zstd_dict, (type(None), ZstdDict)):
-            raise TypeError("zstd_dict argument should be a ZstdDict object.")
-
         # Read or write mode
         if mode in ("r", "rb"):
             if not isinstance(level_or_option, (type(None), dict)):
                 msg = ("In read mode (decompression), level_or_option argument "
                        "should be a dict object, that represents decompression "
                        "option. It doesn't support int type compression level "
                        "in this case.")
```

### Comparing `pyzstd-0.15.6/src/__init__.pyi` & `pyzstd-0.15.7/src/__init__.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -55,98 +55,105 @@
     def bounds(self) -> Tuple[int, int]: ...
 
 class DParameter(IntEnum):
     windowLogMax: int
 
     def bounds(self) -> Tuple[int, int]: ...
 
+ZstdDictInfo = Tuple['ZstdDict', int]
 class ZstdDict:
     dict_content: bytes
     dict_id: int
 
+    as_digested_dict: ZstdDictInfo
+    as_undigested_dict: ZstdDictInfo
+    as_prefix: ZstdDictInfo
+
     def __init__(self,
                  dict_content,
                  is_raw: bool = False) -> None: ...
 
+    def __len__(self) -> int: ...
+
 class ZstdCompressor:
     CONTINUE: ClassVar[int]
     FLUSH_BLOCK: ClassVar[int]
     FLUSH_FRAME: ClassVar[int]
 
     last_mode: Union[ZstdCompressor.CONTINUE, ZstdCompressor.FLUSH_BLOCK, ZstdCompressor.FLUSH_FRAME]
 
     def __init__(self,
                  level_or_option: Union[None, int, Dict[CParameter, int]] = None,
-                 zstd_dict: Optional[ZstdDict] = None) -> None: ...
+                 zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None) -> None: ...
 
     def compress(self,
                  data,
                  mode: Union[ZstdCompressor.CONTINUE, ZstdCompressor.FLUSH_BLOCK, ZstdCompressor.FLUSH_FRAME] = ZstdCompressor.CONTINUE) -> bytes: ...
 
     def flush(self,
               mode: Union[ZstdCompressor.FLUSH_BLOCK, ZstdCompressor.FLUSH_FRAME] = ZstdCompressor.FLUSH_FRAME) -> bytes: ...
 
     def _set_pledged_input_size(self, size: Union[int, None]) -> None: ...
 
 class RichMemZstdCompressor:
     def __init__(self,
                  level_or_option: Union[None, int, Dict[CParameter, int]] = None,
-                 zstd_dict: Optional[ZstdDict] = None) -> None: ...
+                 zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None) -> None: ...
 
     def compress(self, data) -> bytes: ...
 
 class ZstdDecompressor:
     needs_input: bool
     eof: bool
     unused_data: bytes
 
     def __init__(self,
-                 zstd_dict: Optional[ZstdDict] = None,
+                 zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
                  option: Optional[Dict[DParameter, int]] = None) -> None: ...
 
     def decompress(self,
                    data: ByteString,
                    max_length: int = -1) -> bytes: ...
 
 class EndlessZstdDecompressor:
     needs_input: bool
     at_frame_edge: bool
 
     def __init__(self,
-                 zstd_dict: Optional[ZstdDict] = None,
+                 zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
                  option: Optional[Dict[DParameter, int]] = None) -> None: ...
 
     def decompress(self,
                    data: ByteString,
                    max_length: int = -1) -> bytes: ...
 
 class ZstdError(Exception):
     ...
 
 def compress(data,
              level_or_option: Union[None, int, Dict[CParameter, int]] = None,
-             zstd_dict: Optional[ZstdDict] = None) -> bytes: ...
+             zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None) -> bytes: ...
 
 def richmem_compress(data,
                      level_or_option: Union[None, int, Dict[CParameter, int]] = None,
-                     zstd_dict: Optional[ZstdDict] = None) -> bytes: ...
+                     zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None) -> bytes: ...
 
 def decompress(data: ByteString,
-               zstd_dict: Optional[ZstdDict] = None,
+               zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
                option: Optional[Dict[DParameter, int]] = None) -> bytes: ...
 
 def compress_stream(input_stream: BinaryIO, output_stream: Union[BinaryIO, None], *,
                     level_or_option: Union[None, int, Dict[CParameter, int]] = None,
-                    zstd_dict: Optional[ZstdDict] = None,
+                    zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
                     pledged_input_size: Optional[int] = None,
                     read_size: int = 131_072, write_size: int = 131_591,
                     callback: Optional[Callable[[int, int, memoryview, memoryview], None]] = None) -> Tuple[int, int]: ...
 
 def decompress_stream(input_stream: BinaryIO, output_stream: Union[BinaryIO, None], *,
-                      zstd_dict: Optional[ZstdDict] = None,
+                      zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
                       option: Optional[Dict[DParameter, int]] = None,
                       read_size: int = 131_075, write_size: int = 131_072,
                       callback: Optional[Callable[[int, int, memoryview, memoryview], None]] = None) -> Tuple[int, int]: ...
 
 def train_dict(samples: Iterable,
                dict_size: int) -> ZstdDict: ...
 
@@ -165,15 +172,15 @@
 
 class ZstdFile(io.BufferedIOBase):
     def __init__(self,
                  filename: Union[str, bytes, PathLike, BinaryIO],
                  mode: str = "r",
                  *,
                  level_or_option: Union[None, int, Dict[CParameter, int], Dict[DParameter, int]] = None,
-                 zstd_dict: Optional[ZstdDict] = None) -> None: ...
+                 zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None) -> None: ...
     def close(self) -> None: ...
 
     def write(self, data) -> int: ...
     def flush(self) -> None: ...
 
     def read(self, size: int = -1) -> bytes: ...
     def read1(self, size: int = -1) -> bytes: ...
@@ -199,31 +206,31 @@
                     "wt", "at", "xt"] # write
 
 @overload
 def open(filename: Union[str, bytes, PathLike, BinaryIO],
          mode: _BinaryMode = "rb",
          *,
          level_or_option: Union[None, int, Dict[CParameter, int], Dict[DParameter, int]] = None,
-         zstd_dict: Optional[ZstdDict] = None,
+         zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
          encoding: None = None,
          errors: None = None,
          newline: None = None) -> ZstdFile: ...
 
 @overload
 def open(filename: Union[str, bytes, PathLike, BinaryIO],
          mode: _TextMode = ...,
          *,
          level_or_option: Union[None, int, Dict[CParameter, int], Dict[DParameter, int]] = None,
-         zstd_dict: Optional[ZstdDict] = None,
+         zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
          encoding: Optional[str] = None,
          errors: Optional[str] = None,
          newline: Optional[str] = None) -> TextIO: ...
 
 @overload
 def open(filename: Union[str, bytes, PathLike, BinaryIO],
          mode: str = "rb",
          *,
          level_or_option: Union[None, int, Dict[CParameter, int], Dict[DParameter, int]] = None,
-         zstd_dict: Optional[ZstdDict] = None,
+         zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
          encoding: Optional[str] = None,
          errors: Optional[str] = None,
          newline: Optional[str] = None) -> Union[ZstdFile, TextIO]: ...
```

### Comparing `pyzstd-0.15.6/src/__main__.py` & `pyzstd-0.15.7/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/src/bin_ext/_zstdmodule.c` & `pyzstd-0.15.7/src/bin_ext/_zstdmodule.c`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 
     /* Thread lock for compressing */
     PyThread_type_lock lock;
 
     /* (nbWorker >= 1) ? 1 : 0 */
     int use_multithread;
 
+    /* Compression level */
+    int compression_level;
+
     /* __init__ has been called, 0 or 1. */
     int inited;
 
 #ifdef USE_MULTI_PHASE_INIT
     _zstd_state *module_state;
 #endif
 } ZstdCompressor;
@@ -531,15 +534,15 @@
 {
     {ZSTD_d_windowLogMax, "windowLogMax"}
 };
 
 /* Format an user friendly error message. */
 FORCE_NO_INLINE void
 set_parameter_error(const _zstd_state* const state, int is_compress,
-                    Py_ssize_t pos, int key_v, int value_v)
+                    int key_v, int value_v)
 {
     ParameterInfo const *list;
     int list_size;
     char const *name;
     char *type;
     ZSTD_bounds bounds;
     int i;
@@ -563,15 +566,15 @@
             break;
         }
     }
 
     /* Unknown parameter */
     if (name == NULL) {
         PyOS_snprintf(pos_msg, sizeof(pos_msg),
-                      "the %zdth parameter (key %d)", pos, key_v);
+                      "unknown parameter (key %d)", key_v);
         name = pos_msg;
     }
 
     /* Get parameter bounds */
     if (is_compress) {
         bounds = ZSTD_cParam_getBounds(key_v);
     } else {
@@ -667,14 +670,20 @@
     ERR_GET_D_BOUNDS,
     ERR_SET_C_LEVEL,
 
     ERR_TRAIN_DICT,
     ERR_FINALIZE_DICT
 } error_type;
 
+typedef enum {
+    DICT_TYPE_DIGESTED = 0,
+    DICT_TYPE_UNDIGESTED = 1,
+    DICT_TYPE_PREFIX = 2
+} dictionary_type;
+
 /* Format error message and set ZstdError. */
 FORCE_NO_INLINE void
 set_zstd_error(const _zstd_state* const state,
                const error_type type, const size_t zstd_ret)
 {
     char buf[128];
     char *msg;
@@ -689,18 +698,18 @@
         msg = "Unable to compress zstd data: %s";
         break;
     case ERR_SET_PLEDGED_INPUT_SIZE:
         msg = "Unable to set pledged uncompressed content size: %s";
         break;
 
     case ERR_LOAD_D_DICT:
-        msg = "Unable to load zstd dictionary for decompression: %s";
+        msg = "Unable to load zstd dictionary or prefix for decompression: %s";
         break;
     case ERR_LOAD_C_DICT:
-        msg = "Unable to load zstd dictionary for compression: %s";
+        msg = "Unable to load zstd dictionary or prefix for compression: %s";
         break;
 
     case ERR_GET_C_BOUNDS:
         msg = "Unable to get zstd compression parameter bounds: %s";
         break;
     case ERR_GET_D_BOUNDS:
         msg = "Unable to get zstd decompression parameter bounds: %s";
@@ -757,16 +766,16 @@
         cdict = ZSTD_createCDict(PyBytes_AS_STRING(self->dict_content),
                                  Py_SIZE(self->dict_content), compressionLevel);
         Py_END_ALLOW_THREADS
 
         if (cdict == NULL) {
             STATE_FROM_OBJ(self);
             PyErr_SetString(MS_MEMBER(ZstdError),
-                            "Failed to get ZSTD_CDict instance from zstd "
-                            "dictionary content.");
+                            "Failed to create ZSTD_CDict instance from zstd "
+                            "dictionary content. Maybe the content is corrupted.");
             goto error;
         }
 
         /* Put ZSTD_CDict instance into PyCapsule object */
         capsule = PyCapsule_New(cdict, NULL, capsule_free_cdict);
         if (capsule == NULL) {
             ZSTD_freeCDict(cdict);
@@ -792,37 +801,62 @@
     RELEASE_LOCK(self);
     return cdict;
 }
 
 static inline ZSTD_DDict *
 _get_DDict(ZstdDict *self)
 {
-    return self->d_dict;
+    ZSTD_DDict *ret;
+
+    /* Already created */
+    if (self->d_dict != NULL) {
+        return self->d_dict;
+    }
+
+    ACQUIRE_LOCK(self);
+    if (self->d_dict == NULL) {
+        /* Create ZSTD_DDict instance from dictionary content */
+        Py_BEGIN_ALLOW_THREADS
+        self->d_dict = ZSTD_createDDict(PyBytes_AS_STRING(self->dict_content),
+                                        Py_SIZE(self->dict_content));
+        Py_END_ALLOW_THREADS
+
+        if (self->d_dict == NULL) {
+            STATE_FROM_OBJ(self);
+            PyErr_SetString(MS_MEMBER(ZstdError),
+                            "Failed to create ZSTD_DDict instance from zstd "
+                            "dictionary content. Maybe the content is corrupted.");
+        }
+    }
+
+    /* Don't lose any exception */
+    ret = self->d_dict;
+    RELEASE_LOCK(self);
+
+    return ret;
 }
 
-/* Set compressLevel or compression parameters to compression context. */
+/* Set compressLevel or compression parameters to compression context */
 static int
-set_c_parameters(ZstdCompressor *self,
-                 PyObject *level_or_option,
-                 int *compress_level)
+set_c_parameters(ZstdCompressor *self, PyObject *level_or_option)
 {
     size_t zstd_ret;
     STATE_FROM_OBJ(self);
 
     /* Integer compression level */
     if (PyLong_Check(level_or_option)) {
         int level = _PyLong_AsInt(level_or_option);
         if (level == -1 && PyErr_Occurred()) {
             PyErr_SetString(PyExc_ValueError,
                             "Compression level should be 32-bit signed int value.");
             return -1;
         }
 
-        /* Save to *compress_level for generating ZSTD_CDICT */
-        *compress_level = level;
+        /* Save for generating ZSTD_CDICT */
+        self->compression_level = level;
 
         /* Set compressionLevel to compression context */
         zstd_ret = ZSTD_CCtx_setParameter(self->cctx,
                                           ZSTD_c_compressionLevel,
                                           level);
 
         /* Check error */
@@ -851,88 +885,136 @@
             const int key_v = _PyLong_AsInt(key);
             if (key_v == -1 && PyErr_Occurred()) {
                 PyErr_SetString(PyExc_ValueError,
                                 "Key of option dict should be 32-bit signed int value.");
                 return -1;
             }
 
-            int value_v = _PyLong_AsInt(value);
+            const int value_v = _PyLong_AsInt(value);
             if (value_v == -1 && PyErr_Occurred()) {
                 PyErr_SetString(PyExc_ValueError,
                                 "Value of option dict should be 32-bit signed int value.");
                 return -1;
             }
 
             if (key_v == ZSTD_c_compressionLevel) {
-                /* Save to *compress_level for generating ZSTD_CDICT */
-                *compress_level = value_v;
+                /* Save for generating ZSTD_CDICT */
+                self->compression_level = value_v;
             } else if (key_v == ZSTD_c_nbWorkers) {
                 /* From zstd library doc:
                    1. When nbWorkers >= 1, triggers asynchronous mode when
                       used with ZSTD_compressStream2().
                    2, Default value is `0`, aka "single-threaded mode" : no
                       worker is spawned, compression is performed inside
                       caller's thread, all invocations are blocking. */
-                if (value_v > 0) {
+                if (value_v != 0) {
                     self->use_multithread = 1;
                 }
             }
 
             /* Set parameter to compression context */
             zstd_ret = ZSTD_CCtx_setParameter(self->cctx, key_v, value_v);
             if (ZSTD_isError(zstd_ret)) {
-                set_parameter_error(MODULE_STATE, 1, pos, key_v, value_v);
+                set_parameter_error(MODULE_STATE, 1, key_v, value_v);
                 return -1;
             }
         }
         return 0;
     }
 
     /* Wrong type */
     PyErr_SetString(PyExc_TypeError, "level_or_option argument wrong type.");
     return -1;
 }
 
-/* Load dictionary (ZSTD_CDict instance) to compression context (ZSTD_CCtx instance). */
+/* Load dictionary or prefix to compression context */
 static int
-load_c_dict(ZstdCompressor *self, PyObject *dict, int compress_level)
+load_c_dict(ZstdCompressor *self, PyObject *dict)
 {
     size_t zstd_ret;
-    ZSTD_CDict *c_dict;
     STATE_FROM_OBJ(self);
-    int ret;
+    ZstdDict *zd;
+    int type, ret;
 
-    /* Check dict type */
+    /* Check ZstdDict */
     ret = PyObject_IsInstance(dict, (PyObject*)MS_MEMBER(ZstdDict_type));
     if (ret < 0) {
         return -1;
-    } else if (ret == 0) {
-        PyErr_SetString(PyExc_TypeError,
-                        "zstd_dict argument should be ZstdDict object.");
-        return -1;
+    } else if (ret > 0) {
+        /* When compressing, use undigested dictionary by default. */
+        zd = (ZstdDict*)dict;
+        type = DICT_TYPE_UNDIGESTED;
+        goto load;
     }
 
-    /* Get ZSTD_CDict */
-    c_dict = _get_CDict((ZstdDict*)dict, compress_level);
-    if (c_dict == NULL) {
-        return -1;
+    /* Check (ZstdDict, type) */
+    if (PyTuple_CheckExact(dict) && PyTuple_GET_SIZE(dict) == 2) {
+        /* Check ZstdDict */
+        ret = PyObject_IsInstance(PyTuple_GET_ITEM(dict, 0),
+                                  (PyObject*)MS_MEMBER(ZstdDict_type));
+        if (ret < 0) {
+            return -1;
+        } else if (ret > 0) {
+            /* type == -1 may indicate an error. */
+            type = _PyLong_AsInt(PyTuple_GET_ITEM(dict, 1));
+            if (type == DICT_TYPE_DIGESTED ||
+                type == DICT_TYPE_UNDIGESTED ||
+                type == DICT_TYPE_PREFIX)
+            {
+                assert(type >= 0);
+                zd = (ZstdDict*)PyTuple_GET_ITEM(dict, 0);
+                goto load;
+            }
+        }
     }
 
-    /* Reference a prepared dictionary */
-    zstd_ret = ZSTD_CCtx_refCDict(self->cctx, c_dict);
+    /* Wrong type */
+    PyErr_SetString(PyExc_TypeError,
+                    "zstd_dict argument should be ZstdDict object.");
+    return -1;
+
+load:
+    if (type == DICT_TYPE_DIGESTED) {
+        /* Get ZSTD_CDict */
+        ZSTD_CDict *c_dict = _get_CDict(zd, self->compression_level);
+        if (c_dict == NULL) {
+            return -1;
+        }
+        /* Reference a prepared dictionary.
+           It overrides some compression context's parameters. */
+        zstd_ret = ZSTD_CCtx_refCDict(self->cctx, c_dict);
+    } else if (type == DICT_TYPE_UNDIGESTED) {
+        /* Load a dictionary.
+           It doesn't override compression context's parameters. */
+        zstd_ret = ZSTD_CCtx_loadDictionary(
+                            self->cctx,
+                            PyBytes_AS_STRING(zd->dict_content),
+                            Py_SIZE(zd->dict_content));
+    } else if (type == DICT_TYPE_PREFIX) {
+        /* Load a prefix */
+        zstd_ret = ZSTD_CCtx_refPrefix(
+                            self->cctx,
+                            PyBytes_AS_STRING(zd->dict_content),
+                            Py_SIZE(zd->dict_content));
+    } else {
+        /* Impossible code path */
+        PyErr_SetString(PyExc_SystemError,
+                        "load_c_dict() impossible code path");
+        return -1;
+    }
 
     /* Check error */
     if (ZSTD_isError(zstd_ret)) {
         set_zstd_error(MODULE_STATE, ERR_LOAD_C_DICT, zstd_ret);
         return -1;
     }
     return 0;
 }
 
-/* Set decompression parameters to decompression context. */
+/* Set decompression parameters to decompression context */
 static int
 set_d_parameters(ZstdDecompressor *self, PyObject *option)
 {
     size_t zstd_ret;
     PyObject *key, *value;
     Py_ssize_t pos;
     STATE_FROM_OBJ(self);
@@ -969,48 +1051,94 @@
         }
 
         /* Set parameter to compression context */
         zstd_ret = ZSTD_DCtx_setParameter(self->dctx, key_v, value_v);
 
         /* Check error */
         if (ZSTD_isError(zstd_ret)) {
-            set_parameter_error(MODULE_STATE, 0, pos, key_v, value_v);
+            set_parameter_error(MODULE_STATE, 0, key_v, value_v);
             return -1;
         }
     }
     return 0;
 }
 
-/* Load dictionary (ZSTD_DDict instance) to decompression context (ZSTD_DCtx instance). */
+/* Load dictionary or prefix to decompression context */
 static int
 load_d_dict(ZstdDecompressor *self, PyObject *dict)
 {
     size_t zstd_ret;
-    ZSTD_DDict *d_dict;
     STATE_FROM_OBJ(self);
-    int ret;
+    ZstdDict *zd;
+    int type, ret;
 
-    /* Check dict type */
+    /* Check ZstdDict */
     ret = PyObject_IsInstance(dict, (PyObject*)MS_MEMBER(ZstdDict_type));
     if (ret < 0) {
         return -1;
-    } else if (ret == 0) {
-        PyErr_SetString(PyExc_TypeError,
-                        "zstd_dict argument should be ZstdDict object.");
-        return -1;
+    } else if (ret > 0) {
+        /* When decompressing, use digested dictionary by default. */
+        zd = (ZstdDict*)dict;
+        type = DICT_TYPE_DIGESTED;
+        goto load;
     }
 
-    /* Get ZSTD_DDict */
-    d_dict = _get_DDict((ZstdDict*)dict);
-    if (d_dict == NULL) {
-        return -1;
+    /* Check (ZstdDict, type) */
+    if (PyTuple_CheckExact(dict) && PyTuple_GET_SIZE(dict) == 2) {
+        /* Check ZstdDict */
+        ret = PyObject_IsInstance(PyTuple_GET_ITEM(dict, 0),
+                                  (PyObject*)MS_MEMBER(ZstdDict_type));
+        if (ret < 0) {
+            return -1;
+        } else if (ret > 0) {
+            /* type == -1 may indicate an error. */
+            type = _PyLong_AsInt(PyTuple_GET_ITEM(dict, 1));
+            if (type == DICT_TYPE_DIGESTED ||
+                type == DICT_TYPE_UNDIGESTED ||
+                type == DICT_TYPE_PREFIX)
+            {
+                assert(type >= 0);
+                zd = (ZstdDict*)PyTuple_GET_ITEM(dict, 0);
+                goto load;
+            }
+        }
     }
 
-    /* Reference a decompress dictionary */
-    zstd_ret = ZSTD_DCtx_refDDict(self->dctx, d_dict);
+    /* Wrong type */
+    PyErr_SetString(PyExc_TypeError,
+                    "zstd_dict argument should be ZstdDict object.");
+    return -1;
+
+load:
+    if (type == DICT_TYPE_DIGESTED) {
+        /* Get ZSTD_DDict */
+        ZSTD_DDict *d_dict = _get_DDict(zd);
+        if (d_dict == NULL) {
+            return -1;
+        }
+        /* Reference a prepared dictionary */
+        zstd_ret = ZSTD_DCtx_refDDict(self->dctx, d_dict);
+    } else if (type == DICT_TYPE_UNDIGESTED) {
+        /* Load a dictionary */
+        zstd_ret = ZSTD_DCtx_loadDictionary(
+                            self->dctx,
+                            PyBytes_AS_STRING(zd->dict_content),
+                            Py_SIZE(zd->dict_content));
+    } else if (type == DICT_TYPE_PREFIX) {
+        /* Load a prefix */
+        zstd_ret = ZSTD_DCtx_refPrefix(
+                            self->dctx,
+                            PyBytes_AS_STRING(zd->dict_content),
+                            Py_SIZE(zd->dict_content));
+    } else {
+        /* Impossible code path */
+        PyErr_SetString(PyExc_SystemError,
+                        "load_d_dict() impossible code path");
+        return -1;
+    }
 
     /* Check error */
     if (ZSTD_isError(zstd_ret)) {
         set_zstd_error(MODULE_STATE, ERR_LOAD_D_DICT, zstd_ret);
         return -1;
     }
     return 0;
@@ -1121,31 +1249,17 @@
        at least 8 bytes */
     if (Py_SIZE(self->dict_content) < 8) {
         PyErr_SetString(PyExc_ValueError,
                         "Zstd dictionary content should at least 8 bytes.");
         return -1;
     }
 
-    /* Create ZSTD_DDict instance from dictionary content, also check content
-       integrity to some degree. */
-    Py_BEGIN_ALLOW_THREADS
-    self->d_dict = ZSTD_createDDict(PyBytes_AS_STRING(self->dict_content),
-                                    Py_SIZE(self->dict_content));
-    Py_END_ALLOW_THREADS
-
-    if (self->d_dict == NULL) {
-        STATE_FROM_OBJ(self);
-        PyErr_SetString(MS_MEMBER(ZstdError),
-                        "Failed to get ZSTD_DDict instance from zstd "
-                        "dictionary content. Maybe the content is corrupted.");
-        return -1;
-    }
-
     /* Get dict_id, 0 means "raw content" dictionary. */
-    self->dict_id = ZSTD_getDictID_fromDDict(self->d_dict);
+    self->dict_id = ZSTD_getDictID_fromDict(PyBytes_AS_STRING(self->dict_content),
+                                            Py_SIZE(self->dict_content));
 
     /* Check validity for ordinary dictionary */
     if (!is_raw && self->dict_id == 0) {
         char *msg = "The dict_content argument is not a valid zstd "
                     "dictionary. The first 4 bytes of a valid zstd dictionary "
                     "should be a magic number: b'\\x37\\xA4\\x30\\xEC'.\n"
                     "If you are an advanced user, and can be sure that "
@@ -1160,18 +1274,18 @@
 
 static PyObject *
 ZstdDict_reduce(ZstdDict *self)
 {
     /* return Py_BuildValue("O(O)", Py_TYPE(self), self->dict_content); */
 
     PyErr_SetString(PyExc_TypeError,
-                    "Intentionally not supporting pickle. If need to save zstd "
-                    "dictionary to disk, please save .dict_content attribute, "
-                    "it's a bytes object. So that the zstd dictionary can be "
-                    "used with other programs.");
+                    "ZstdDict object intentionally doesn't support pickle. If need "
+                    "to save zstd dictionary to disk, please save .dict_content "
+                    "attribute, it's a bytes object. So that the zstd dictionary "
+                    "can be used with other programs.");
     return NULL;
 }
 
 static PyMethodDef ZstdDict_methods[] = {
     {"__reduce__", (PyCFunction)ZstdDict_reduce,
      METH_NOARGS, reduce_cannot_pickle_doc},
 
@@ -1215,22 +1329,88 @@
 
 static PyMemberDef ZstdDict_members[] = {
     {"dict_id", T_UINT, offsetof(ZstdDict, dict_id), READONLY, ZstdDict_dictid_doc},
     {"dict_content", T_OBJECT_EX, offsetof(ZstdDict, dict_content), READONLY, ZstdDict_dictcontent_doc},
     {NULL}
 };
 
+PyDoc_STRVAR(ZstdDict_as_digested_dict_doc,
+"Load as a digested dictionary to compressor, by passing this attribute as\n"
+"zstd_dict argument: compress(dat, zstd_dict=zd.as_digested_dict)\n"
+"1, Some advanced compression parameters of compressor may be overridden\n"
+"   by parameters of digested dictionary.\n"
+"2, ZstdDict has a digested dictionaries cache for each compression level.\n"
+"   It's faster when loading again a digested dictionary with the same\n"
+"   compression level.\n"
+"3, No need to use this for decompression.");
+
+static PyObject *
+ZstdDict_as_digested_dict_get(ZstdDict *self, void *Py_UNUSED(ignored))
+{
+    return Py_BuildValue("Oi", self, DICT_TYPE_DIGESTED);
+}
+
+PyDoc_STRVAR(ZstdDict_as_undigested_dict_doc,
+"Load as an undigested dictionary to compressor, by passing this attribute as\n"
+"zstd_dict argument: compress(dat, zstd_dict=zd.as_undigested_dict)\n"
+"1, The advanced compression parameters of compressor will not be overridden.\n"
+"2, Loading an undigested dictionary is costly. If load an undigested dictionary\n"
+"   multiple times, consider reusing a compressor object.\n"
+"3, No need to use this for decompression.");
+
+static PyObject *
+ZstdDict_as_undigested_dict_get(ZstdDict *self, void *Py_UNUSED(ignored))
+{
+    return Py_BuildValue("Oi", self, DICT_TYPE_UNDIGESTED);
+}
+
+PyDoc_STRVAR(ZstdDict_as_prefix_doc,
+"Load as a prefix to compressor/decompressor, by passing this attribute as\n"
+"zstd_dict argument: compress(dat, zstd_dict=zd.as_prefix)\n"
+"1, Prefix is compatible with long distance matching, while dictionary is not.\n"
+"2, It only works for the first frame, then the compressor/decompressor will\n"
+"   return to no prefix state.\n"
+"3, When decompressing, must use the same prefix as when compressing.");
+
+static PyObject *
+ZstdDict_as_prefix_get(ZstdDict *self, void *Py_UNUSED(ignored))
+{
+    return Py_BuildValue("Oi", self, DICT_TYPE_PREFIX);
+}
+
+static PyGetSetDef ZstdDict_getset[] = {
+    {"as_digested_dict", (getter)ZstdDict_as_digested_dict_get,
+     NULL, ZstdDict_as_digested_dict_doc},
+
+    {"as_undigested_dict", (getter)ZstdDict_as_undigested_dict_get,
+     NULL, ZstdDict_as_undigested_dict_doc},
+
+    {"as_prefix", (getter)ZstdDict_as_prefix_get,
+     NULL, ZstdDict_as_prefix_doc},
+
+    {NULL},
+};
+
+static Py_ssize_t
+ZstdDict_length(ZstdDict *self)
+{
+    assert(PyBytes_Check(self->dict_content));
+    return Py_SIZE(self->dict_content);
+}
+
 static PyType_Slot zstddict_slots[] = {
     {Py_tp_methods, ZstdDict_methods},
     {Py_tp_members, ZstdDict_members},
+    {Py_tp_getset, ZstdDict_getset},
     {Py_tp_new, ZstdDict_new},
     {Py_tp_dealloc, ZstdDict_dealloc},
     {Py_tp_init, ZstdDict_init},
     {Py_tp_str, ZstdDict_str},
     {Py_tp_doc, (char*)ZstdDict_dict_doc},
+    {Py_sq_length, ZstdDict_length},
     {0, 0}
 };
 
 static PyType_Spec zstddict_type_spec = {
     .name = "pyzstd.ZstdDict",
     .basicsize = sizeof(ZstdDict),
     .flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
@@ -1490,14 +1670,15 @@
     self = (ZstdCompressor*)type->tp_alloc(type, 0);
     if (self == NULL) {
         goto error;
     }
 
     assert(self->dict == NULL);
     assert(self->use_multithread == 0);
+    assert(self->compression_level == 0);
     assert(self->inited == 0);
 
     /* Keep this first. Set module state to self. */
     SET_STATE_TO_OBJ(type, self);
 
     /* Compression context */
     self->cctx = ZSTD_createCCtx();
@@ -1557,16 +1738,14 @@
 static int
 ZstdCompressor_init(ZstdCompressor *self, PyObject *args, PyObject *kwargs)
 {
     static char *kwlist[] = {"level_or_option", "zstd_dict", NULL};
     PyObject *level_or_option = Py_None;
     PyObject *zstd_dict = Py_None;
 
-    int compress_level = 0; /* 0 means use zstd's default compression level */
-
     if (!PyArg_ParseTupleAndKeywords(args, kwargs,
                                      "|OO:ZstdCompressor.__init__", kwlist,
                                      &level_or_option, &zstd_dict)) {
         return -1;
     }
 
     /* Only called once */
@@ -1574,22 +1753,22 @@
         PyErr_SetString(PyExc_RuntimeError, init_twice_msg);
         return -1;
     }
     self->inited = 1;
 
     /* Set compressLevel/option to compression context */
     if (level_or_option != Py_None) {
-        if (set_c_parameters(self, level_or_option, &compress_level) < 0) {
+        if (set_c_parameters(self, level_or_option) < 0) {
             return -1;
         }
     }
 
     /* Load dictionary to compression context */
     if (zstd_dict != Py_None) {
-        if (load_c_dict(self, zstd_dict, compress_level) < 0) {
+        if (load_c_dict(self, zstd_dict) < 0) {
             return -1;
         }
 
         /* Py_INCREF the dict */
         Py_INCREF(zstd_dict);
         self->dict = zstd_dict;
     }
@@ -1957,16 +2136,14 @@
 static int
 RichMemZstdCompressor_init(ZstdCompressor *self, PyObject *args, PyObject *kwargs)
 {
     static char *kwlist[] = {"level_or_option", "zstd_dict", NULL};
     PyObject *level_or_option = Py_None;
     PyObject *zstd_dict = Py_None;
 
-    int compress_level = 0; /* 0 means use zstd's default compression level */
-
     if (!PyArg_ParseTupleAndKeywords(args, kwargs,
                                      "|OO:RichMemZstdCompressor.__init__", kwlist,
                                      &level_or_option, &zstd_dict)) {
         return -1;
     }
 
     /* Only called once */
@@ -1974,15 +2151,15 @@
         PyErr_SetString(PyExc_RuntimeError, init_twice_msg);
         return -1;
     }
     self->inited = 1;
 
     /* Set compressLevel/option to compression context */
     if (level_or_option != Py_None) {
-        if (set_c_parameters(self, level_or_option, &compress_level) < 0) {
+        if (set_c_parameters(self, level_or_option) < 0) {
             return -1;
         }
     }
 
     /* Check effective condition */
     if (self->use_multithread) {
         char *msg = "Currently \"rich memory mode\" has no effect on "
@@ -1992,15 +2169,15 @@
         if (PyErr_WarnEx(PyExc_ResourceWarning, msg, 1) < 0) {
             return -1;
         }
     }
 
     /* Load dictionary to compression context */
     if (zstd_dict != Py_None) {
-        if (load_c_dict(self, zstd_dict, compress_level) < 0) {
+        if (load_c_dict(self, zstd_dict) < 0) {
             return -1;
         }
 
         /* Py_INCREF the dict */
         Py_INCREF(zstd_dict);
         self->dict = zstd_dict;
     }
@@ -2346,18 +2523,18 @@
             self->input_buffer_size = new_size;
 
             /* Set begin & end position */
             self->in_begin = 0;
             self->in_end = used_now;
         } else if (avail_now < (size_t) data.len) {
             /* Move unconsumed data to the beginning.
-               dst < src, so using memcpy() is safe. */
-            memcpy(self->input_buffer,
-                   self->input_buffer + self->in_begin,
-                   used_now);
+               Overlap is possbile, so use memmove(). */
+            memmove(self->input_buffer,
+                    self->input_buffer + self->in_begin,
+                    used_now);
 
             /* Set begin & end position */
             self->in_begin = 0;
             self->in_end = used_now;
         }
 
         /* Copy data to input buffer */
@@ -3219,15 +3396,14 @@
     /* If fails, modify value in __init__.pyi and doc. */
     assert(read_size == 131072);
     assert(write_size == 131591);
 
     size_t zstd_ret;
     PyObject *temp;
     ZstdCompressor self = {0};
-    int compress_level = 0; /* 0 means use zstd's default compression level */
     uint64_t pledged_size_value = ZSTD_CONTENTSIZE_UNKNOWN;
     ZSTD_inBuffer in = {.src = NULL};
     ZSTD_outBuffer out = {.dst = NULL};
     PyObject *in_memoryview = NULL;
     uint64_t total_input_size = 0;
     uint64_t total_output_size = 0;
     STATE_FROM_MODULE(module);
@@ -3289,21 +3465,21 @@
         goto error;
     }
 #ifdef USE_MULTI_PHASE_INIT
     self.module_state = MODULE_STATE;
 #endif
 
     if (level_or_option != Py_None) {
-        if (set_c_parameters(&self, level_or_option, &compress_level) < 0) {
+        if (set_c_parameters(&self, level_or_option) < 0) {
             goto error;
         }
     }
 
     if (zstd_dict != Py_None) {
-        if (load_c_dict(&self, zstd_dict, compress_level) < 0) {
+        if (load_c_dict(&self, zstd_dict) < 0) {
             goto error;
         }
     }
 
     if (pledged_size_value != ZSTD_CONTENTSIZE_UNKNOWN) {
         zstd_ret = ZSTD_CCtx_setPledgedSrcSize(self.cctx, pledged_size_value);
         if (ZSTD_isError(zstd_ret)) {
```

### Comparing `pyzstd-0.15.6/src/bin_ext/build_cffi.py` & `pyzstd-0.15.7/src/bin_ext/build_cffi.py`

 * *Files 10% similar despite different names*

```diff
@@ -123,20 +123,25 @@
 size_t ZSTD_CStreamOutSize(void);
 size_t ZSTD_DStreamInSize(void);
 size_t ZSTD_DStreamOutSize(void);
 
 ZSTD_CDict* ZSTD_createCDict(const void* dictBuffer, size_t dictSize,
                              int compressionLevel);
 size_t ZSTD_CCtx_refCDict(ZSTD_CCtx* cctx, const ZSTD_CDict* cdict);
+size_t ZSTD_CCtx_loadDictionary(ZSTD_CCtx* cctx, const void* dict, size_t dictSize);
 size_t ZSTD_freeCDict(ZSTD_CDict* CDict);
+size_t ZSTD_CCtx_refPrefix(ZSTD_CCtx* cctx, const void* prefix, size_t prefixSize);
 
 ZSTD_DDict* ZSTD_createDDict(const void* dictBuffer, size_t dictSize);
 size_t ZSTD_DCtx_refDDict(ZSTD_DCtx* dctx, const ZSTD_DDict* ddict);
+size_t ZSTD_DCtx_loadDictionary(ZSTD_DCtx* dctx, const void* dict, size_t dictSize);
 size_t ZSTD_freeDDict(ZSTD_DDict* ddict);
-unsigned ZSTD_getDictID_fromDDict(const ZSTD_DDict* ddict);
+size_t ZSTD_DCtx_refPrefix(ZSTD_DCtx* dctx, const void* prefix, size_t prefixSize);
+
+unsigned ZSTD_getDictID_fromDict(const void* dict, size_t dictSize);
 
 ZSTD_CCtx* ZSTD_createCCtx(void);
 size_t ZSTD_freeCCtx(ZSTD_CCtx* cctx);
 size_t ZSTD_CCtx_reset(ZSTD_CCtx* cctx, ZSTD_ResetDirective reset);
 size_t ZSTD_CCtx_setPledgedSrcSize(ZSTD_CCtx* cctx, unsigned long long pledgedSrcSize);
 size_t ZSTD_compressStream2(ZSTD_CCtx* cctx,
                             ZSTD_outBuffer* output,
@@ -163,15 +168,15 @@
 } ZDICT_params_t;
 
 size_t ZDICT_finalizeDictionary(void* dstDictBuffer, size_t maxDictSize,
                                 const void* dictContent, size_t dictContentSize,
                                 const void* samplesBuffer, const size_t* samplesSizes, unsigned nbSamples,
                                 ZDICT_params_t parameters);
 
-int pyzstd_static_link;
+extern int pyzstd_static_link;
 """)
 
 source = """
 #include "zstd.h"
 #include "zdict.h"
 
 #if ZSTD_VERSION_NUMBER < 10400
@@ -198,16 +203,16 @@
 int ZSTD_defaultCLevel(void)
 {
     return ZSTD_CLEVEL_DEFAULT;
 }
 #endif
 
 #ifdef PYZSTD_STATIC_LINK
-pyzstd_static_link = 1;
+int pyzstd_static_link = 1;
 #else
-pyzstd_static_link = 0;
+int pyzstd_static_link = 0;
 #endif
 """
 
 def get_extension(**kwargs):
     ffibuilder.set_source(source=source, **kwargs)
     return ffibuilder.distutils_extension()
```

### Comparing `pyzstd-0.15.6/src/c/c_pyzstd.py` & `pyzstd-0.15.7/src/c/c_pyzstd.py`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/src/cffi/cffi_pyzstd.py` & `pyzstd-0.15.7/src/cffi/cffi_pyzstd.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,14 +233,18 @@
             ffi.memmove(final+posi, block, len(block))
             posi += len(block)
         # The last block
         ffi.memmove(final+posi, self.list[-1], out.pos)
 
         return bytes(ffi.buffer(final))
 
+_DICT_TYPE_DIGESTED = 0
+_DICT_TYPE_UNDIGESTED = 1
+_DICT_TYPE_PREFIX = 2
+
 class ZstdDict:
     """Zstd dictionary, used for compression/decompression."""
 
     def __init__(self, dict_content, is_raw=False) -> None:
         """Initialize a ZstdDict object.
 
         Parameters
@@ -248,38 +252,32 @@
         is_raw:       This parameter is for advanced user. True means dict_content
                       argument is a "raw content" dictionary, free of any format
                       restriction. False means dict_content argument is an ordinary
                       zstd dictionary, was created by zstd functions, follow a
                       specified format.
         """
         self.__cdicts = {}
+        self.__ddict = ffi.NULL
         self.__lock = Lock()
 
         # Check dict_content's type
         try:
             self.__dict_content = bytes(dict_content)
         except:
             raise TypeError("dict_content argument should be bytes-like object.")
 
         # Both ordinary dictionary and "raw content" dictionary should
         # at least 8 bytes
         if len(self.__dict_content) < 8:
             raise ValueError('Zstd dictionary content should at least 8 bytes.')
 
-        # Create ZSTD_DDict instance from dictionary content, also check content
-        # integrity to some degree.
-        self.__ddict = m.ZSTD_createDDict(ffi.from_buffer(self.__dict_content),
-                                          len(self.__dict_content))
-        if self.__ddict == ffi.NULL:
-            msg = ("Failed to get ZSTD_DDict instance from zstd "
-                   "dictionary content. Maybe the content is corrupted.")
-            raise ZstdError(msg)
-
         # Get dict_id, 0 means "raw content" dictionary.
-        self.__dict_id = m.ZSTD_getDictID_fromDDict(self.__ddict)
+        self.__dict_id = m.ZSTD_getDictID_fromDict(
+                                    ffi.from_buffer(self.__dict_content),
+                                    len(self.__dict_content))
 
         # Check validity for ordinary dictionary
         if not is_raw and self.__dict_id == 0:
             msg = ('The dict_content argument is not a valid zstd '
                    'dictionary. The first 4 bytes of a valid zstd dictionary '
                    'should be a magic number: b"\\x37\\xA4\\x30\\xEC".\n'
                    'If you are an advanced user, and can be sure that '
@@ -316,43 +314,96 @@
         a specified format.
 
         0 means a "raw content" dictionary, free of any format restriction, used
         for advanced user.
         """
         return self.__dict_id
 
+    @property
+    def as_digested_dict(self):
+        """Load as a digested dictionary to compressor, by passing this attribute as
+        zstd_dict argument: compress(dat, zstd_dict=zd.as_digested_dict)
+        1, Some advanced compression parameters of compressor may be overridden
+           by parameters of digested dictionary.
+        2, ZstdDict has a digested dictionaries cache for each compression level.
+           It's faster when loading again a digested dictionary with the same
+           compression level.
+        3, No need to use this for decompression.
+        """
+        return (self, _DICT_TYPE_DIGESTED)
+
+    @property
+    def as_undigested_dict(self):
+        """Load as an undigested dictionary to compressor, by passing this attribute as
+        zstd_dict argument: compress(dat, zstd_dict=zd.as_undigested_dict)
+        1, The advanced compression parameters of compressor will not be overridden.
+        2, Loading an undigested dictionary is costly. If load an undigested dictionary
+           multiple times, consider reusing a compressor object.
+        3, No need to use this for decompression.
+        """
+        return (self, _DICT_TYPE_UNDIGESTED)
+
+    @property
+    def as_prefix(self):
+        """Load as a prefix to compressor/decompressor, by passing this attribute as
+        zstd_dict argument: compress(dat, zstd_dict=zd.as_prefix)
+        1, Prefix is compatible with long distance matching, while dictionary is not.
+        2, It only works for the first frame, then the compressor/decompressor will
+           return to no prefix state.
+        3, When decompressing, must use the same prefix as when compressing.
+        """
+        return (self, _DICT_TYPE_PREFIX)
+
     def __str__(self):
         return '<ZstdDict dict_id=%d dict_size=%d>' % \
                (self.__dict_id, len(self.__dict_content))
 
+    def __len__(self):
+        return len(self.__dict_content)
+
     def __reduce__(self):
-        msg = ("Intentionally not supporting pickle. If need to save zstd "
-               "dictionary to disk, please save .dict_content attribute, "
-               "it's a bytes object. So that the zstd dictionary can be "
-               "used with other programs.")
+        msg = ("ZstdDict object intentionally doesn't support pickle. If need "
+               "to save zstd dictionary to disk, please save .dict_content "
+               "attribute, it's a bytes object. So that the zstd dictionary "
+               "can be used with other programs.")
         raise TypeError(msg)
 
     def _get_cdict(self, level):
         with self.__lock:
             # Already cached
             if level in self.__cdicts:
                 cdict = self.__cdicts[level]
             else:
                 # Create ZSTD_CDict instance
                 cdict = m.ZSTD_createCDict(ffi.from_buffer(self.__dict_content),
                                            len(self.__dict_content), level)
                 if cdict == ffi.NULL:
-                    msg = ("Failed to get ZSTD_CDict instance from zstd "
-                           "dictionary content.")
+                    msg = ("Failed to create ZSTD_CDict instance from zstd "
+                           "dictionary content. Maybe the content is corrupted.")
                     raise ZstdError(msg)
                 self.__cdicts[level] = cdict
             return cdict
 
     def _get_ddict(self):
-        return self.__ddict
+        # Already created
+        if self.__ddict != ffi.NULL:
+            return self.__ddict
+
+        with self.__lock:
+            # Create ZSTD_DDict instance from dictionary content
+            self.__ddict = m.ZSTD_createDDict(
+                                    ffi.from_buffer(self.__dict_content),
+                                    len(self.__dict_content))
+
+            if self.__ddict == ffi.NULL:
+                msg = ("Failed to create ZSTD_DDict instance from zstd "
+                       "dictionary content. Maybe the content is corrupted.")
+                raise ZstdError(msg)
+
+            return self.__ddict
 
 class _ErrorType:
     ERR_DECOMPRESS=0
     ERR_COMPRESS=1
     ERR_SET_PLEDGED_INPUT_SIZE=2
 
     ERR_LOAD_D_DICT=3
@@ -366,16 +417,16 @@
     ERR_FINALIZE_DICT=9
 
     _TYPE_MSG = (
         "Unable to decompress zstd data: %s",
         "Unable to compress zstd data: %s",
         "Unable to set pledged uncompressed content size: %s",
 
-        "Unable to load zstd dictionary for decompression: %s",
-        "Unable to load zstd dictionary for compression: %s",
+        "Unable to load zstd dictionary or prefix for decompression: %s",
+        "Unable to load zstd dictionary or prefix for compression: %s",
 
         "Unable to get zstd compression parameter bounds: %s",
         "Unable to get zstd decompression parameter bounds: %s",
         "Unable to set zstd compression level: %s",
 
         "Unable to train zstd dictionary: %s",
         "Unable to finalize zstd dictionary: %s")
@@ -387,15 +438,15 @@
 def _set_zstd_error(type, zstd_ret):
     assert m.ZSTD_isError(zstd_ret)
 
     msg = _ErrorType.get_type_msg(type) % \
           ffi.string(m.ZSTD_getErrorName(zstd_ret)).decode('utf-8')
     raise ZstdError(msg)
 
-def _set_parameter_error(is_compress, pos, key, value):
+def _set_parameter_error(is_compress, key, value):
     COMPRESS_PARAMETERS = \
     {m.ZSTD_c_compressionLevel: "compressionLevel",
      m.ZSTD_c_windowLog:        "windowLog",
      m.ZSTD_c_hashLog:          "hashLog",
      m.ZSTD_c_chainLog:         "chainLog",
      m.ZSTD_c_searchLog:        "searchLog",
      m.ZSTD_c_minMatch:         "minMatch",
@@ -425,15 +476,15 @@
         parameters = DECOMPRESS_PARAMETERS
         type_msg = "decompression"
 
     # Find parameter's name
     name = parameters.get(key)
     # Unknown parameter
     if name is None:
-        name = 'the %dth parameter (key %d)' % (pos, key)
+        name = 'unknown parameter (key %d)' % key
 
     # Get parameter bounds
     if is_compress:
         bounds = m.ZSTD_cParam_getBounds(key)
     else:
         bounds = m.ZSTD_dParam_getBounds(key)
     if m.ZSTD_isError(bounds.error):
@@ -470,81 +521,135 @@
 
         return level_or_option, False
 
     if isinstance(level_or_option, dict):
         level = 0  # 0 means use zstd's default compression level
         use_multithread = False
 
-        for posi, (key, value) in enumerate(level_or_option.items(), 1):
+        for key, value in level_or_option.items():
             # Check key type
             if type(key) == DParameter:
                 raise TypeError("Key of compression option dict should "
                                 "NOT be DParameter.")
 
             # Both key & value should be 32-bit signed int
             _check_int32_value(key, "Key of option dict")
             _check_int32_value(value, "Value of option dict")
 
             if key == m.ZSTD_c_compressionLevel:
                 level = value
             elif key == m.ZSTD_c_nbWorkers:
-                if value > 0:
+                if value != 0:
                     use_multithread = True
 
             # Set parameter
             zstd_ret = m.ZSTD_CCtx_setParameter(cctx, key, value)
             if m.ZSTD_isError(zstd_ret):
-                _set_parameter_error(True, posi, key, value)
+                _set_parameter_error(True, key, value)
 
         return level, use_multithread
 
     raise TypeError("level_or_option argument wrong type.")
 
 def _set_d_parameters(dctx, option):
     if not isinstance(option, dict):
         raise TypeError("option argument should be dict object.")
 
-    for posi, (key, value) in enumerate(option.items(), 1):
+    for key, value in option.items():
         # Check key type
         if type(key) == CParameter:
             raise TypeError("Key of decompression option dict should "
                             "NOT be CParameter.")
 
         # Both key & value should be 32-bit signed int
         _check_int32_value(key, "Key of option dict")
         _check_int32_value(value, "Value of option dict")
 
         # Set parameter
         zstd_ret = m.ZSTD_DCtx_setParameter(dctx, key, value)
         if m.ZSTD_isError(zstd_ret):
-            _set_parameter_error(False, posi, key, value)
+            _set_parameter_error(False, key, value)
 
 def _load_c_dict(cctx, zstd_dict, level):
-    # Check dict type
-    if not isinstance(zstd_dict, ZstdDict):
+    if isinstance(zstd_dict, ZstdDict):
+        # When compressing, use undigested dictionary by default.
+        zd = zstd_dict
+        type = _DICT_TYPE_UNDIGESTED
+    elif isinstance(zstd_dict, tuple) and \
+         len(zstd_dict) == 2 and \
+         isinstance(zstd_dict[0], ZstdDict) and \
+         zstd_dict[1] in {_DICT_TYPE_DIGESTED,
+                          _DICT_TYPE_UNDIGESTED,
+                          _DICT_TYPE_PREFIX}:
+        zd = zstd_dict[0]
+        type = zstd_dict[1]
+    else:
         raise TypeError("zstd_dict argument should be ZstdDict object.")
 
-    # Get ZSTD_CDict
-    c_dict = zstd_dict._get_cdict(level)
+    if type == _DICT_TYPE_DIGESTED:
+        # Get ZSTD_CDict
+        c_dict = zd._get_cdict(level)
+        # Reference a prepared dictionary.
+        # It overrides some compression context's parameters.
+        zstd_ret = m.ZSTD_CCtx_refCDict(cctx, c_dict)
+    elif type == _DICT_TYPE_UNDIGESTED:
+        # Load a dictionary.
+        # It doesn't override compression context's parameters.
+        zstd_ret = m.ZSTD_CCtx_loadDictionary(
+                                    cctx,
+                                    ffi.from_buffer(zd.dict_content),
+                                    len(zd.dict_content))
+    elif type == _DICT_TYPE_PREFIX:
+        # Reference as prefix
+        zstd_ret = m.ZSTD_CCtx_refPrefix(
+                                    cctx,
+                                    ffi.from_buffer(zd.dict_content),
+                                    len(zd.dict_content))
+    else:
+        raise SystemError('_load_c_dict() impossible code path')
 
-    # Reference a prepared dictionary
-    zstd_ret = m.ZSTD_CCtx_refCDict(cctx, c_dict)
     if m.ZSTD_isError(zstd_ret):
         _set_zstd_error(_ErrorType.ERR_LOAD_C_DICT, zstd_ret)
 
 def _load_d_dict(dctx, zstd_dict):
-    # Check dict type
-    if not isinstance(zstd_dict, ZstdDict):
+    if isinstance(zstd_dict, ZstdDict):
+        # When decompressing, use digested dictionary by default.
+        zd = zstd_dict
+        type = _DICT_TYPE_DIGESTED
+    elif isinstance(zstd_dict, tuple) and \
+         len(zstd_dict) == 2 and \
+         isinstance(zstd_dict[0], ZstdDict) and \
+         zstd_dict[1] in {_DICT_TYPE_DIGESTED,
+                          _DICT_TYPE_UNDIGESTED,
+                          _DICT_TYPE_PREFIX}:
+        zd = zstd_dict[0]
+        type = zstd_dict[1]
+    else:
         raise TypeError("zstd_dict argument should be ZstdDict object.")
 
-    # Get ZSTD_DDict
-    d_dict = zstd_dict._get_ddict()
+    if type == _DICT_TYPE_DIGESTED:
+        # Get ZSTD_DDict
+        d_dict = zd._get_ddict()
+        # Reference a prepared dictionary
+        zstd_ret = m.ZSTD_DCtx_refDDict(dctx, d_dict)
+    elif type == _DICT_TYPE_UNDIGESTED:
+        # Load a dictionary
+        zstd_ret = m.ZSTD_DCtx_loadDictionary(
+                                    dctx,
+                                    ffi.from_buffer(zd.dict_content),
+                                    len(zd.dict_content))
+    elif type == _DICT_TYPE_PREFIX:
+        # Reference as prefix
+        zstd_ret = m.ZSTD_DCtx_refPrefix(
+                                    dctx,
+                                    ffi.from_buffer(zd.dict_content),
+                                    len(zd.dict_content))
+    else:
+        raise SystemError('_load_d_dict() impossible code path')
 
-    # Reference a prepared dictionary
-    zstd_ret = m.ZSTD_DCtx_refDDict(dctx, d_dict)
     if m.ZSTD_isError(zstd_ret):
         _set_zstd_error(_ErrorType.ERR_LOAD_D_DICT, zstd_ret)
 
 class _Compressor:
     def __init__(self, level_or_option=None, zstd_dict=None):
         self._use_multithread = False
         self._lock = Lock()
@@ -561,16 +666,16 @@
         # Compression context
         self._cctx = m.ZSTD_createCCtx()
         if self._cctx == ffi.NULL:
             raise ZstdError("Unable to create ZSTD_CCtx instance.")
 
         # Set compressLevel/option to compression context
         if level_or_option is not None:
-            level, self._use_multithread = _set_c_parameters(self._cctx,
-                                                             level_or_option)
+            level, self._use_multithread = \
+                  _set_c_parameters(self._cctx, level_or_option)
 
         # Load dictionary to compression context
         if zstd_dict is not None:
             _load_c_dict(self._cctx, zstd_dict, level)
             self.__dict = zstd_dict
 
     def __del__(self):
@@ -1343,15 +1448,16 @@
     try:
         # Initialize & set ZstdCompressor
         cctx = m.ZSTD_createCCtx()
         if cctx == ffi.NULL:
             raise ZstdError("Unable to create ZSTD_CCtx instance.")
 
         if level_or_option is not None:
-            level, use_multithread = _set_c_parameters(cctx, level_or_option)
+            level, use_multithread = \
+                _set_c_parameters(cctx, level_or_option)
         if zstd_dict is not None:
             _load_c_dict(cctx, zstd_dict, level)
 
         if pledged_input_size is not None:
             zstd_ret = m.ZSTD_CCtx_setPledgedSrcSize(cctx, pledged_input_size)
             if m.ZSTD_isError(zstd_ret):
                 _set_zstd_error(_ErrorType.ERR_COMPRESS, zstd_ret)
```

### Comparing `pyzstd-0.15.6/tests/test_zstd.py` & `pyzstd-0.15.7/tests/test_zstd.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,58 @@
 import io
 import os
 import re
 import sys
 import array
 import pathlib
 import pickle
+import platform
 import random
 import subprocess
 import tempfile
 import unittest
 
 import pyzstd
 from pyzstd import ZstdCompressor, RichMemZstdCompressor, \
                    ZstdDecompressor, EndlessZstdDecompressor, ZstdError, \
                    CParameter, DParameter, Strategy, \
                    compress, compress_stream, richmem_compress, \
                    decompress, decompress_stream, \
                    ZstdDict, train_dict, finalize_dict, \
                    zstd_version, zstd_version_info, zstd_support_multithread, \
                    compressionLevel_values, get_frame_info, get_frame_size, \
-                   ZstdFile, open
+                   ZstdFile, open, __version__ as pyzstd_version
 
-PYZSTD_CONFIG = pyzstd.PYZSTD_CONFIG
+PYZSTD_CONFIG = pyzstd.PYZSTD_CONFIG # type: ignore
 if PYZSTD_CONFIG[1] == 'c':
-    from pyzstd.c import _zstd
+    from pyzstd.c import _zstd       # type: ignore
+
+build_info = ('Pyzstd build information:\n'
+              ' - Environment:\n'
+              '   * Machine type: {}\n'
+              '   * Bit build: {}\n'
+              '   * OS: {}\n'
+              ' - Pyzstd:\n'
+              '   * Pyzstd version: {}\n'
+              '   * Implementation: {}\n'
+              '   * Enable multi-phase init: {}\n'
+              ' - Zstd:\n'
+              '   * Zstd version: {}\n'
+              '   * Link to zstd library: {}\n'
+              '   * Enable multi-threaded compression: {}\n').format(
+                    platform.machine(), # Environment
+                    PYZSTD_CONFIG[0],
+                    platform.system(),
+                    pyzstd_version,     # Pyzstd
+                    PYZSTD_CONFIG[1].upper(),
+                    PYZSTD_CONFIG[3],
+                    zstd_version,       # Zstd
+                    'Statically link' if PYZSTD_CONFIG[2] else 'Dynamically link',
+                    zstd_support_multithread)
+print(build_info, flush=True)
 
 DECOMPRESSED_DAT = None
 COMPRESSED_DAT = None
 
 DECOMPRESSED_100_PLUS_32KB = None
 COMPRESSED_100_PLUS_32KB = None
 
@@ -89,14 +114,15 @@
         sample = [b'%s = %d' % (random.choice(words), random.randrange(100))
                   for j in range(20)]
         sample = b'\n'.join(sample)
 
         lst.append(sample)
     global SAMPLES
     SAMPLES = lst
+    assert len(SAMPLES) > 10
 
     global TRAINED_DICT
     TRAINED_DICT = train_dict(SAMPLES, 3*1024)
     assert len(TRAINED_DICT.dict_content) <= 3*1024
 
 class FunctionsTestCase(unittest.TestCase):
 
@@ -340,22 +366,28 @@
 
     def test_ZstdDict(self):
         ZstdDict(b'12345678', True)
         zd = ZstdDict(b'12345678', is_raw=True)
 
         self.assertEqual(type(zd.dict_content), bytes)
         self.assertEqual(zd.dict_id, 0)
+        self.assertEqual(zd.as_digested_dict[1], 0)
+        self.assertEqual(zd.as_undigested_dict[1], 1)
+        self.assertEqual(zd.as_prefix[1], 2)
 
         # name
         self.assertIn('.ZstdDict', str(type(zd)))
 
         # doesn't support pickle
         with self.assertRaisesRegex(TypeError,
                                     r'save \.dict_content attribute'):
             pickle.dumps(zd)
+        with self.assertRaisesRegex(TypeError,
+                                    r'save \.dict_content attribute'):
+            pickle.dumps(zd.as_prefix)
 
         # supports subclass
         class SubClass(ZstdDict):
             pass
 
     def test_Strategy(self):
         # class attributes
@@ -545,34 +577,46 @@
             with self.assertRaises(ZstdError):
                 ZstdCompressor({CParameter.nbWorkers:4})
             with self.assertRaises(ZstdError):
                 ZstdCompressor({CParameter.jobSize:4})
             with self.assertRaises(ZstdError):
                 ZstdCompressor({CParameter.overlapLog:4})
 
-        # unknown parameter
-        with self.assertRaisesRegex(ZstdError,
-                      r'the 2th parameter \(key 654321\).*?invalid. \(zstd v'):
-            ZstdCompressor({CParameter.compressionLevel:3,
-                            654321:-12345})
-
     def test_decompress_parameters(self):
         d = {DParameter.windowLogMax : 15}
         EndlessZstdDecompressor(option=d)
 
         # larger than signed int, ValueError
         d1 = d.copy()
         d1[DParameter.windowLogMax] = 2**31
         self.assertRaises(ValueError, EndlessZstdDecompressor, None, d1)
 
         # value out of bounds, ZstdError
         d2 = d.copy()
         d2[DParameter.windowLogMax] = 32
         self.assertRaises(ZstdError, EndlessZstdDecompressor, None, d2)
 
+    def test_unknown_compression_parameter(self):
+        KEY = 100001234
+        option = {CParameter.compressionLevel: 10,
+                  KEY: 200000000}
+        pattern = r'Zstd compression parameter.*?"unknown parameter \(key %d\)"' \
+                  % KEY
+        with self.assertRaisesRegex(ZstdError, pattern):
+            ZstdCompressor(option)
+
+    def test_unknown_decompression_parameter(self):
+        KEY = 100001234
+        option = {DParameter.windowLogMax: DParameter.windowLogMax.bounds()[1],
+                  KEY: 200000000}
+        pattern = r'Zstd decompression parameter.*?"unknown parameter \(key %d\)"' \
+                  % KEY
+        with self.assertRaisesRegex(ZstdError, pattern):
+            ZstdDecompressor(option=option)
+
     @unittest.skipIf(not zstd_support_multithread,
                      "zstd build doesn't support multi-threaded compression")
     def test_zstd_multithread_compress(self):
         size = 40*1024*1024
         b = THIS_FILE_BYTES * (size // len(THIS_FILE_BYTES))
 
         option = {CParameter.compressionLevel : 4,
@@ -1722,16 +1766,39 @@
         with self.assertRaises(TypeError):
             ZstdDict(desk333=345)
 
     def test_invalid_dict(self):
         DICT_MAGIC = 0xEC30A437.to_bytes(4, byteorder='little')
         dict_content = DICT_MAGIC + b'abcdefghighlmnopqrstuvwxyz'
 
+        # corrupted
+        zd = ZstdDict(dict_content, is_raw=False)
+        with self.assertRaisesRegex(ZstdError, r'ZSTD_CDict.*?corrupted'):
+            ZstdCompressor(zstd_dict=zd.as_digested_dict)
         with self.assertRaisesRegex(ZstdError, r'ZSTD_DDict.*?corrupted'):
-            ZstdDict(dict_content, is_raw=False)
+            ZstdDecompressor(zd)
+
+        # wrong type
+        with self.assertRaisesRegex(TypeError, r'should be ZstdDict object'):
+            ZstdCompressor(zstd_dict=(zd, b'123'))
+        with self.assertRaisesRegex(TypeError, r'should be ZstdDict object'):
+            ZstdCompressor(zstd_dict=(zd, 1, 2))
+        with self.assertRaisesRegex(TypeError, r'should be ZstdDict object'):
+            ZstdCompressor(zstd_dict=(zd, -1))
+        with self.assertRaisesRegex(TypeError, r'should be ZstdDict object'):
+            ZstdCompressor(zstd_dict=(zd, 3))
+
+        with self.assertRaisesRegex(TypeError, r'should be ZstdDict object'):
+            ZstdDecompressor(zstd_dict=(zd, b'123'))
+        with self.assertRaisesRegex(TypeError, r'should be ZstdDict object'):
+            ZstdDecompressor((zd, 1, 2))
+        with self.assertRaisesRegex(TypeError, r'should be ZstdDict object'):
+            ZstdDecompressor((zd, -1))
+        with self.assertRaisesRegex(TypeError, r'should be ZstdDict object'):
+            ZstdDecompressor((zd, 3))
 
     def test_train_dict(self):
         DICT_SIZE1 = 3*1024
 
         global TRAINED_DICT
         TRAINED_DICT = pyzstd.train_dict(SAMPLES, DICT_SIZE1)
         ZstdDict(TRAINED_DICT.dict_content, False)
@@ -1906,14 +1973,77 @@
             pyzstd._finalize_dict(TRAINED_DICT.dict_content,
                                   concatenation, wrong_size_lst, 300*1024, 5)
 
         # correct size list
         pyzstd._finalize_dict(TRAINED_DICT.dict_content,
                               concatenation, correct_size_lst, 300*1024, 5)
 
+    def test_as_prefix(self):
+        # V1
+        V1 = THIS_FILE_BYTES
+        zd = ZstdDict(V1, True)
+
+        # V2
+        mid = len(V1) // 2
+        V2 = V1[:mid] + \
+             (b'a' if V1[mid] != b'a' else b'b') + \
+             V1[mid+1:]
+
+        # compress
+        dat = richmem_compress(V2, zstd_dict=zd.as_prefix)
+        self.assertEqual(get_frame_info(dat).dictionary_id, 0)
+
+        # decompress
+        self.assertEqual(decompress(dat, zd.as_prefix), V2)
+
+        # use wrong prefix
+        zd2 = ZstdDict(SAMPLES[0], True)
+        try:
+            decompressed = decompress(dat, zd2.as_prefix)
+        except ZstdError: # expected
+            pass
+        else:
+            self.assertNotEqual(decompressed, V2)
+
+        # read only attribute
+        with self.assertRaises(AttributeError):
+            zd.as_prefix = b'1234'
+
+    def test_as_digested_dict(self):
+        zd = TRAINED_DICT
+
+        # test .as_digested_dict
+        dat = richmem_compress(SAMPLES[0], zstd_dict=zd.as_digested_dict)
+        self.assertEqual(decompress(dat, zd.as_digested_dict), SAMPLES[0])
+        with self.assertRaises(AttributeError):
+            zd.as_digested_dict = b'1234'
+
+        # test .as_undigested_dict
+        dat = richmem_compress(SAMPLES[0], zstd_dict=zd.as_undigested_dict)
+        self.assertEqual(decompress(dat, zd.as_undigested_dict), SAMPLES[0])
+        with self.assertRaises(AttributeError):
+            zd.as_undigested_dict = b'1234'
+
+    def test_advanced_compression_parameters(self):
+        option = {CParameter.compressionLevel: 6,
+                  CParameter.windowLog: 20,
+                  CParameter.enableLongDistanceMatching: 1}
+
+        # automatically select
+        dat = richmem_compress(SAMPLES[0], option, TRAINED_DICT)
+        self.assertEqual(decompress(dat, TRAINED_DICT), SAMPLES[0])
+
+        # explicitly select
+        dat = richmem_compress(SAMPLES[0], option, TRAINED_DICT.as_digested_dict)
+        self.assertEqual(decompress(dat, TRAINED_DICT), SAMPLES[0])
+
+    def test_len(self):
+        self.assertEqual(len(TRAINED_DICT), len(TRAINED_DICT.dict_content))
+        self.assertIn(str(len(TRAINED_DICT)), str(TRAINED_DICT))
+
 class OutputBufferTestCase(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         KB = 1024
         MB = 1024 * 1024
 
@@ -2805,22 +2935,39 @@
 
     def test_tell_bad_args(self):
         f = ZstdFile(BytesIO(COMPRESSED_100_PLUS_32KB))
         f.close()
         self.assertRaises(ValueError, f.tell)
 
     def test_file_dict(self):
+        # default
         bi = BytesIO()
         with ZstdFile(bi, 'w', zstd_dict=TRAINED_DICT) as f:
             f.write(SAMPLES[0])
-
         bi.seek(0)
         with ZstdFile(bi, zstd_dict=TRAINED_DICT) as f:
             dat = f.read()
+        self.assertEqual(dat, SAMPLES[0])
 
+        # .as_(un)digested_dict
+        bi = BytesIO()
+        with ZstdFile(bi, 'w', zstd_dict=TRAINED_DICT.as_digested_dict) as f:
+            f.write(SAMPLES[0])
+        bi.seek(0)
+        with ZstdFile(bi, zstd_dict=TRAINED_DICT.as_undigested_dict) as f:
+            dat = f.read()
+        self.assertEqual(dat, SAMPLES[0])
+
+    def test_file_prefix(self):
+        bi = BytesIO()
+        with ZstdFile(bi, 'w', zstd_dict=TRAINED_DICT.as_prefix) as f:
+            f.write(SAMPLES[0])
+        bi.seek(0)
+        with ZstdFile(bi, zstd_dict=TRAINED_DICT.as_prefix) as f:
+            dat = f.read()
         self.assertEqual(dat, SAMPLES[0])
 
     def test_UnsupportedOperation(self):
         # 1
         with ZstdFile(BytesIO(), 'r') as f:
             with self.assertRaises(io.UnsupportedOperation):
                 f.write(b'1234')
@@ -3030,22 +3177,47 @@
             with self.assertRaises(FileExistsError):
                 with open(TESTFN, mode):
                     pass
 
         os.remove(TESTFN)
 
     def test_open_dict(self):
+        # default
         bi = BytesIO()
         with open(bi, 'w', zstd_dict=TRAINED_DICT) as f:
             f.write(SAMPLES[0])
-
         bi.seek(0)
         with open(bi, zstd_dict=TRAINED_DICT) as f:
             dat = f.read()
+        self.assertEqual(dat, SAMPLES[0])
+
+        # .as_(un)digested_dict
+        bi = BytesIO()
+        with open(bi, 'w', zstd_dict=TRAINED_DICT.as_digested_dict) as f:
+            f.write(SAMPLES[0])
+        bi.seek(0)
+        with open(bi, zstd_dict=TRAINED_DICT.as_undigested_dict) as f:
+            dat = f.read()
+        self.assertEqual(dat, SAMPLES[0])
 
+        # invalid dictionary
+        bi = BytesIO()
+        with self.assertRaisesRegex(TypeError, 'zstd_dict'):
+            open(bi, 'w', zstd_dict={1:2, 2:3})
+
+        with self.assertRaisesRegex(TypeError, 'zstd_dict'):
+            open(bi, 'w', zstd_dict=b'1234567890')
+
+    def test_open_prefix(self):
+        bi = BytesIO()
+        with open(bi, 'w', zstd_dict=TRAINED_DICT.as_prefix) as f:
+            f.write(SAMPLES[0])
+        bi.seek(0)
+        with open(bi, zstd_dict=TRAINED_DICT.as_prefix) as f:
+            dat = f.read()
         self.assertEqual(dat, SAMPLES[0])
 
     def test_buffer_protocol(self):
         # don't use len() for buffer protocol objects
         arr = array.array("i", range(1000))
         LENGTH = len(arr) * arr.itemsize
 
@@ -3099,14 +3271,16 @@
             compress_stream(123, b1)
         with self.assertRaisesRegex(TypeError, r'output_stream'):
             compress_stream(b1, 123)
         with self.assertRaisesRegex(TypeError, r'level_or_option'):
             compress_stream(b1, b2, level_or_option='3')
         with self.assertRaisesRegex(TypeError, r'zstd_dict'):
             compress_stream(b1, b2, zstd_dict={})
+        with self.assertRaisesRegex(TypeError, r'zstd_dict'):
+            compress_stream(b1, b2, zstd_dict=b'1234567890')
         with self.assertRaisesRegex(ValueError, r'pledged_input_size'):
             compress_stream(b1, b2, pledged_input_size=-1)
         with self.assertRaisesRegex(ValueError, r'pledged_input_size'):
             compress_stream(b1, b2, pledged_input_size=2**64+1)
         with self.assertRaisesRegex(ValueError, r'read_size'):
             compress_stream(b1, b2, read_size=-1)
         with self.assertRaises(OverflowError):
@@ -3185,14 +3359,16 @@
         b2 = BytesIO()
         with self.assertRaisesRegex(TypeError, r'input_stream'):
             decompress_stream(123, b1)
         with self.assertRaisesRegex(TypeError, r'output_stream'):
             decompress_stream(b1, 123)
         with self.assertRaisesRegex(TypeError, r'zstd_dict'):
             decompress_stream(b1, b2, zstd_dict={})
+        with self.assertRaisesRegex(TypeError, r'zstd_dict'):
+            decompress_stream(b1, b2, zstd_dict=b'1234567890')
         with self.assertRaisesRegex(TypeError, r'option'):
             decompress_stream(b1, b2, option=3)
         with self.assertRaisesRegex(ValueError, r'read_size'):
             decompress_stream(b1, b2, read_size=-1)
         with self.assertRaises(OverflowError):
             decompress_stream(b1, b2, write_size=2**64+1)
         with self.assertRaisesRegex(TypeError, r'callback'):
@@ -3293,14 +3469,55 @@
         def cb(a,b,c,d):
             self.fail('callback function should not be called')
         # callback function will not be called for empty input,
         # it's a promised behavior.
         compress_stream(io.BytesIO(b''), io.BytesIO(), callback=cb)
         decompress_stream(io.BytesIO(b''), io.BytesIO(), callback=cb)
 
+    def test_stream_dict(self):
+        zd = ZstdDict(THIS_FILE_BYTES, True)
+
+        # default
+        with BytesIO(THIS_FILE_BYTES) as bi, BytesIO() as bo:
+            ret = compress_stream(bi, bo, zstd_dict=zd)
+            compressed = bo.getvalue()
+        self.assertEqual(ret, (len(THIS_FILE_BYTES), len(compressed)))
+
+        with BytesIO(compressed) as bi, BytesIO() as bo:
+            ret = decompress_stream(bi, bo, zstd_dict=zd)
+            decompressed = bo.getvalue()
+        self.assertEqual(ret, (len(compressed), len(decompressed)))
+        self.assertEqual(decompressed, THIS_FILE_BYTES)
+
+        # .as_(un)digested_dict
+        with BytesIO(THIS_FILE_BYTES) as bi, BytesIO() as bo:
+            ret = compress_stream(bi, bo, zstd_dict=zd.as_undigested_dict)
+            compressed = bo.getvalue()
+        self.assertEqual(ret, (len(THIS_FILE_BYTES), len(compressed)))
+
+        with BytesIO(compressed) as bi, BytesIO() as bo:
+            ret = decompress_stream(bi, bo, zstd_dict=zd.as_digested_dict)
+            decompressed = bo.getvalue()
+        self.assertEqual(ret, (len(compressed), len(decompressed)))
+        self.assertEqual(decompressed, THIS_FILE_BYTES)
+
+    def test_stream_prefix(self):
+        zd = ZstdDict(THIS_FILE_BYTES, True)
+
+        with BytesIO(THIS_FILE_BYTES) as bi, BytesIO() as bo:
+            ret = compress_stream(bi, bo, zstd_dict=zd.as_prefix)
+            compressed = bo.getvalue()
+        self.assertEqual(ret, (len(THIS_FILE_BYTES), len(compressed)))
+
+        with BytesIO(compressed) as bi, BytesIO() as bo:
+            ret = decompress_stream(bi, bo, zstd_dict=zd.as_prefix)
+            decompressed = bo.getvalue()
+        self.assertEqual(ret, (len(compressed), len(decompressed)))
+        self.assertEqual(decompressed, THIS_FILE_BYTES)
+
 class CLITestCase(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.tempdir = tempfile.TemporaryDirectory()
         cls.dir_name = cls.tempdir.name
 
         cls.samples_path = os.path.join(cls.dir_name, 'samples').rstrip(os.sep)
```

### Comparing `pyzstd-0.15.6/zstd/lib/BUCK` & `pyzstd-0.15.7/zstd/lib/BUCK`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/Makefile` & `pyzstd-0.15.7/zstd/lib/Makefile`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/README.md` & `pyzstd-0.15.7/zstd/lib/README.md`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/allocations.h` & `pyzstd-0.15.7/zstd/lib/common/allocations.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/bits.h` & `pyzstd-0.15.7/zstd/lib/common/bits.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/bitstream.h` & `pyzstd-0.15.7/zstd/lib/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/compiler.h` & `pyzstd-0.15.7/zstd/lib/common/compiler.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/cpu.h` & `pyzstd-0.15.7/zstd/lib/common/cpu.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/debug.c` & `pyzstd-0.15.7/zstd/lib/common/debug.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/debug.h` & `pyzstd-0.15.7/zstd/lib/common/debug.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/entropy_common.c` & `pyzstd-0.15.7/zstd/lib/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/error_private.c` & `pyzstd-0.15.7/zstd/lib/common/error_private.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/error_private.h` & `pyzstd-0.15.7/zstd/lib/common/error_private.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/fse.h` & `pyzstd-0.15.7/zstd/lib/common/fse.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/fse_decompress.c` & `pyzstd-0.15.7/zstd/lib/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/huf.h` & `pyzstd-0.15.7/zstd/lib/common/huf.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/mem.h` & `pyzstd-0.15.7/zstd/lib/common/mem.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/pool.c` & `pyzstd-0.15.7/zstd/lib/common/pool.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/pool.h` & `pyzstd-0.15.7/zstd/lib/common/pool.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/portability_macros.h` & `pyzstd-0.15.7/zstd/lib/common/portability_macros.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/threading.c` & `pyzstd-0.15.7/zstd/lib/common/threading.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/threading.h` & `pyzstd-0.15.7/zstd/lib/common/threading.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/xxhash.c` & `pyzstd-0.15.7/zstd/lib/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/xxhash.h` & `pyzstd-0.15.7/zstd/lib/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/zstd_common.c` & `pyzstd-0.15.7/zstd/lib/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/zstd_deps.h` & `pyzstd-0.15.7/zstd/lib/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/zstd_internal.h` & `pyzstd-0.15.7/zstd/lib/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/common/zstd_trace.h` & `pyzstd-0.15.7/zstd/lib/common/zstd_trace.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/clevels.h` & `pyzstd-0.15.7/zstd/lib/compress/clevels.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/fse_compress.c` & `pyzstd-0.15.7/zstd/lib/compress/fse_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/hist.c` & `pyzstd-0.15.7/zstd/lib/compress/hist.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/hist.h` & `pyzstd-0.15.7/zstd/lib/compress/hist.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/huf_compress.c` & `pyzstd-0.15.7/zstd/lib/compress/huf_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_compress.c` & `pyzstd-0.15.7/zstd/lib/compress/zstd_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_compress_internal.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_internal.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_compress_literals.c` & `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_literals.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_compress_literals.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_literals.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_compress_sequences.c` & `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_sequences.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_compress_sequences.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_sequences.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_compress_superblock.c` & `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_superblock.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_compress_superblock.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_superblock.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_cwksp.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_cwksp.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_double_fast.c` & `pyzstd-0.15.7/zstd/lib/compress/zstd_double_fast.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_double_fast.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_double_fast.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_fast.c` & `pyzstd-0.15.7/zstd/lib/compress/zstd_fast.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_fast.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_fast.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_lazy.c` & `pyzstd-0.15.7/zstd/lib/compress/zstd_lazy.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_lazy.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_lazy.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_ldm.c` & `pyzstd-0.15.7/zstd/lib/compress/zstd_ldm.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_ldm.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_ldm.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_ldm_geartab.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_ldm_geartab.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_opt.c` & `pyzstd-0.15.7/zstd/lib/compress/zstd_opt.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstd_opt.h` & `pyzstd-0.15.7/zstd/lib/compress/zstd_opt.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstdmt_compress.c` & `pyzstd-0.15.7/zstd/lib/compress/zstdmt_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/compress/zstdmt_compress.h` & `pyzstd-0.15.7/zstd/lib/compress/zstdmt_compress.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/decompress/huf_decompress.c` & `pyzstd-0.15.7/zstd/lib/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/decompress/huf_decompress_amd64.S` & `pyzstd-0.15.7/zstd/lib/decompress/huf_decompress_amd64.S`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/decompress/zstd_ddict.c` & `pyzstd-0.15.7/zstd/lib/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/decompress/zstd_ddict.h` & `pyzstd-0.15.7/zstd/lib/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/decompress/zstd_decompress.c` & `pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/decompress/zstd_decompress_block.c` & `pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/decompress/zstd_decompress_block.h` & `pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/decompress/zstd_decompress_internal.h` & `pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/deprecated/zbuff.h` & `pyzstd-0.15.7/zstd/lib/deprecated/zbuff.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/deprecated/zbuff_common.c` & `pyzstd-0.15.7/zstd/lib/deprecated/zbuff_common.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/deprecated/zbuff_compress.c` & `pyzstd-0.15.7/zstd/lib/deprecated/zbuff_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/deprecated/zbuff_decompress.c` & `pyzstd-0.15.7/zstd/lib/deprecated/zbuff_decompress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dictBuilder/cover.c` & `pyzstd-0.15.7/zstd/lib/dictBuilder/cover.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dictBuilder/cover.h` & `pyzstd-0.15.7/zstd/lib/dictBuilder/cover.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dictBuilder/divsufsort.c` & `pyzstd-0.15.7/zstd/lib/dictBuilder/divsufsort.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dictBuilder/divsufsort.h` & `pyzstd-0.15.7/zstd/lib/dictBuilder/divsufsort.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dictBuilder/fastcover.c` & `pyzstd-0.15.7/zstd/lib/dictBuilder/fastcover.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dictBuilder/zdict.c` & `pyzstd-0.15.7/zstd/lib/dictBuilder/zdict.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dll/example/Makefile` & `pyzstd-0.15.7/zstd/lib/dll/example/Makefile`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dll/example/README.md` & `pyzstd-0.15.7/zstd/lib/dll/example/README.md`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dll/example/build_package.bat` & `pyzstd-0.15.7/zstd/lib/dll/example/build_package.bat`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dll/example/fullbench-dll.sln` & `pyzstd-0.15.7/zstd/lib/dll/example/fullbench-dll.sln`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/dll/example/fullbench-dll.vcxproj` & `pyzstd-0.15.7/zstd/lib/dll/example/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_legacy.h` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_legacy.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v01.c` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v01.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v01.h` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v01.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v02.c` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v02.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v02.h` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v02.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v03.c` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v03.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v03.h` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v03.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v04.c` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v04.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v04.h` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v04.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v05.c` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v05.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v05.h` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v05.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v06.c` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v06.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v06.h` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v06.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v07.c` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v07.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/legacy/zstd_v07.h` & `pyzstd-0.15.7/zstd/lib/legacy/zstd_v07.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/libzstd.mk` & `pyzstd-0.15.7/zstd/lib/libzstd.mk`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/module.modulemap` & `pyzstd-0.15.7/zstd/lib/module.modulemap`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/zdict.h` & `pyzstd-0.15.7/zstd/lib/zdict.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/zstd.h` & `pyzstd-0.15.7/zstd/lib/zstd.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.6/zstd/lib/zstd_errors.h` & `pyzstd-0.15.7/zstd/lib/zstd_errors.h`

 * *Files identical despite different names*

