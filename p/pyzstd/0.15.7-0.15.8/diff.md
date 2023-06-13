# Comparing `tmp/pyzstd-0.15.7.tar.gz` & `tmp/pyzstd-0.15.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzstd-0.15.7.tar", last modified: Fri Apr 21 12:31:15 2023, max compression
+gzip compressed data, was "pyzstd-0.15.8.tar", last modified: Tue Jun 13 10:12:03 2023, max compression
```

## Comparing `pyzstd-0.15.7.tar` & `pyzstd-0.15.8.tar`

### file list

```diff
@@ -1,139 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.536491 pyzstd-0.15.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-21 12:31:05.000000 pyzstd-0.15.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 12:31:05.000000 pyzstd-0.15.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-21 12:31:15.536491 pyzstd-0.15.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-21 12:31:05.000000 pyzstd-0.15.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-04-21 12:31:05.000000 pyzstd-0.15.7/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-21 12:31:05.000000 pyzstd-0.15.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/pyzstd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-21 12:31:15.000000 pyzstd-0.15.7/pyzstd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-21 12:31:15.000000 pyzstd-0.15.7/pyzstd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:31:15.000000 pyzstd-0.15.7/pyzstd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 12:31:15.000000 pyzstd-0.15.7/pyzstd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:31:15.536491 pyzstd-0.15.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-04-21 12:31:05.000000 pyzstd-0.15.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)    25771 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/src/bin_ext/
--rw-r--r--   0 runner    (1001) docker     (123)   130735 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/bin_ext/_zstdmodule.c
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/bin_ext/build_cffi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/src/c/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/c/c_pyzstd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/src/cffi/
--rw-r--r--   0 runner    (1001) docker     (123)    70341 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/cffi/cffi_pyzstd.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:05.000000 pyzstd-0.15.7/src/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.520491 pyzstd-0.15.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:05.000000 pyzstd-0.15.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   217042 2023-04-21 12:31:05.000000 pyzstd-0.15.7/tests/test_zstd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.516491 pyzstd-0.15.7/zstd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.524491 pyzstd-0.15.7/zstd/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/BUCK
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.524491 pyzstd-0.15.7/zstd/lib/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/allocations.h
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/bits.h
--rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/debug.c
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/error_private.c
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/error_private.h
--rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/fse.h
--rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/huf.h
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/mem.h
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/pool.c
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/portability_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/threading.c
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/threading.h
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)   212896 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/zstd_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/zstd_deps.h
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/zstd_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/common/zstd_trace.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/clevels.h
--rw-r--r--   0 runner    (1001) docker     (123)    24096 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/hist.c
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/hist.h
--rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)   312776 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    64416 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_literals.c
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_literals.h
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_sequences.c
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_sequences.h
--rw-r--r--   0 runner    (1001) docker     (123)    28499 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_superblock.c
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_compress_superblock.h
--rw-r--r--   0 runner    (1001) docker     (123)    27872 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_cwksp.h
--rw-r--r--   0 runner    (1001) docker     (123)    34479 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_double_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_double_fast.h
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_fast.h
--rw-r--r--   0 runner    (1001) docker     (123)   101952 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_lazy.c
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_lazy.h
--rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_ldm.c
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_ldm.h
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_ldm_geartab.h
--rw-r--r--   0 runner    (1001) docker     (123)    67459 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_opt.c
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstd_opt.h
--rw-r--r--   0 runner    (1001) docker     (123)    81334 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstdmt_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/compress/zstdmt_compress.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/decompress/
--rw-r--r--   0 runner    (1001) docker     (123)    73701 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/huf_decompress_amd64.S
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_ddict.c
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_ddict.h
--rw-r--r--   0 runner    (1001) docker     (123)    99701 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    99641 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_block.c
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_block.h
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/deprecated/zbuff.h
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/deprecated/zbuff_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/deprecated/zbuff_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/deprecated/zbuff_decompress.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/dictBuilder/
--rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/cover.c
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/cover.h
--rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/divsufsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/divsufsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    28561 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/fastcover.c
--rw-r--r--   0 runner    (1001) docker     (123)    44008 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dictBuilder/zdict.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.516491 pyzstd-0.15.7/zstd/lib/dll/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.532491 pyzstd-0.15.7/zstd/lib/dll/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/build_package.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/fullbench-dll.sln
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/dll/example/fullbench-dll.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:31:15.536491 pyzstd-0.15.7/zstd/lib/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_legacy.h
--rw-r--r--   0 runner    (1001) docker     (123)    69465 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v01.c
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v01.h
--rw-r--r--   0 runner    (1001) docker     (123)   125639 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v02.c
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v02.h
--rw-r--r--   0 runner    (1001) docker     (123)   111749 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v03.c
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v03.h
--rw-r--r--   0 runner    (1001) docker     (123)   132791 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v04.c
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v04.h
--rw-r--r--   0 runner    (1001) docker     (123)   153658 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v05.c
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v05.h
--rw-r--r--   0 runner    (1001) docker     (123)   163699 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v06.c
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v06.h
--rw-r--r--   0 runner    (1001) docker     (123)   182559 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v07.c
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/legacy/zstd_v07.h
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/libzstd.mk
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/libzstd.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/module.modulemap
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/zdict.h
--rw-r--r--   0 runner    (1001) docker     (123)   171378 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/zstd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-21 12:31:06.000000 pyzstd-0.15.7/zstd/lib/zstd_errors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.433651 pyzstd-0.15.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-13 10:11:50.000000 pyzstd-0.15.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-13 10:11:50.000000 pyzstd-0.15.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-13 10:12:03.433651 pyzstd-0.15.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-06-13 10:11:50.000000 pyzstd-0.15.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81554 2023-06-13 10:11:50.000000 pyzstd-0.15.8/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 10:11:50.000000 pyzstd-0.15.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.417651 pyzstd-0.15.8/pyzstd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-13 10:12:03.000000 pyzstd-0.15.8/pyzstd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-13 10:12:03.000000 pyzstd-0.15.8/pyzstd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:12:03.000000 pyzstd-0.15.8/pyzstd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 10:12:03.000000 pyzstd-0.15.8/pyzstd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:12:03.433651 pyzstd-0.15.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-06-13 10:11:50.000000 pyzstd-0.15.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.417651 pyzstd-0.15.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.417651 pyzstd-0.15.8/src/bin_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/bin_ext/compressor.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26746 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/bin_ext/decompressor.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/bin_ext/dict.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/bin_ext/file.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/bin_ext/macro_functions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/bin_ext/pyzstd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26146 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/bin_ext/pyzstd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/bin_ext/pyzstd_build_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/bin_ext/stream.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.417651 pyzstd-0.15.8/src/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/c/c_pyzstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.417651 pyzstd-0.15.8/src/cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)    81128 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/cffi/cffi_pyzstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26229 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/seekable_zstdfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-06-13 10:11:50.000000 pyzstd-0.15.8/src/zstdfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.417651 pyzstd-0.15.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:11:50.000000 pyzstd-0.15.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62761 2023-06-13 10:11:50.000000 pyzstd-0.15.8/tests/test_seekable.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140819 2023-06-13 10:11:50.000000 pyzstd-0.15.8/tests/test_zstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.413651 pyzstd-0.15.8/zstd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.421651 pyzstd-0.15.8/zstd/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/BUCK
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.421651 pyzstd-0.15.8/zstd/lib/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/allocations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/bits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/debug.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/error_private.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/fse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/huf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/pool.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/portability_macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/threading.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/threading.h
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)   212896 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/zstd_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/zstd_deps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/zstd_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/common/zstd_trace.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.425651 pyzstd-0.15.8/zstd/lib/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/clevels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24096 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/hist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/hist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)   312776 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    64416 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_compress_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_compress_literals.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_compress_literals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_compress_sequences.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_compress_sequences.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28499 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_compress_superblock.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_compress_superblock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27872 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_cwksp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34479 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_double_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_double_fast.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_fast.h
+-rw-r--r--   0 runner    (1001) docker     (123)   101952 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_lazy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_lazy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_ldm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_ldm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_ldm_geartab.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67459 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_opt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstd_opt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    81334 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstdmt_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/compress/zstdmt_compress.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.429651 pyzstd-0.15.8/zstd/lib/decompress/
+-rw-r--r--   0 runner    (1001) docker     (123)    73701 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/decompress/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/decompress/huf_decompress_amd64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/decompress/zstd_ddict.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/decompress/zstd_ddict.h
+-rw-r--r--   0 runner    (1001) docker     (123)    99701 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/decompress/zstd_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    99641 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/decompress/zstd_decompress_block.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/decompress/zstd_decompress_block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/decompress/zstd_decompress_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.429651 pyzstd-0.15.8/zstd/lib/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/deprecated/zbuff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/deprecated/zbuff_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/deprecated/zbuff_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/deprecated/zbuff_decompress.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.429651 pyzstd-0.15.8/zstd/lib/dictBuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dictBuilder/cover.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dictBuilder/cover.h
+-rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dictBuilder/divsufsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dictBuilder/divsufsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28561 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dictBuilder/fastcover.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44008 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dictBuilder/zdict.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.413651 pyzstd-0.15.8/zstd/lib/dll/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.429651 pyzstd-0.15.8/zstd/lib/dll/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dll/example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dll/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dll/example/build_package.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dll/example/fullbench-dll.sln
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/dll/example/fullbench-dll.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:12:03.433651 pyzstd-0.15.8/zstd/lib/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_legacy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69465 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v01.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v01.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125639 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v02.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v02.h
+-rw-r--r--   0 runner    (1001) docker     (123)   111749 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v03.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v03.h
+-rw-r--r--   0 runner    (1001) docker     (123)   132791 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v04.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v04.h
+-rw-r--r--   0 runner    (1001) docker     (123)   153658 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v05.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v05.h
+-rw-r--r--   0 runner    (1001) docker     (123)   163699 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v06.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v06.h
+-rw-r--r--   0 runner    (1001) docker     (123)   182559 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v07.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/legacy/zstd_v07.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/libzstd.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/libzstd.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/module.modulemap
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/zdict.h
+-rw-r--r--   0 runner    (1001) docker     (123)   171378 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/zstd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-13 10:11:52.000000 pyzstd-0.15.8/zstd/lib/zstd_errors.h
```

### Comparing `pyzstd-0.15.7/LICENSE` & `pyzstd-0.15.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/PKG-INFO` & `pyzstd-0.15.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyzstd
-Version: 0.15.7
+Version: 0.15.8
 Summary: Python bindings to Zstandard (zstd) compression library, the API style is similar to Python's bz2/lzma/zlib modules.
 Home-page: https://github.com/animalize/pyzstd
 Author: Ma Lin
 Author-email: malincns@163.com
 License: The 3-Clause BSD License
-Keywords: zstandard zstd compression decompression compress decompress
+Keywords: zstandard zstd zst tar file seekable format
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Archiving :: Compression
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3.5
@@ -30,27 +30,38 @@
 Pyzstd module provides classes and functions for compressing and decompressing data, using Facebook's `Zstandard <http://www.zstd.net>`_ (or zstd as short name) algorithm.
 
 The API style is similar to Python's bz2/lzma/zlib modules.
 
 * Includes zstd v1.5.5 source code
 * Can also dynamically link to zstd library provided by system, see `this note <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
 * Has a CFFI implementation that can work with PyPy
+* ``ZstdFile`` class has C language level performance
+* Supports `Zstandard Seekable Format <https://github.com/facebook/zstd/blob/dev/contrib/seekable_format/zstd_seekable_compression_format.md>`__
 * Has a command line interface: ``python -m pyzstd --help``
 
-
 Links
 -----------
 
 Documentation: https://pyzstd.readthedocs.io/en/latest
 
 GitHub: https://github.com/animalize/pyzstd
 
 
 Release note
 ------------
+**0.15.8  (Jun 13, 2023)**
+
+#. Add `SeekableZstdFile <https://pyzstd.readthedocs.io/en/latest/#SeekableZstdFile>`_ class, it's a subclass of ``ZstdFile``, supports `Zstandard Seekable Format <https://github.com/facebook/zstd/blob/dev/contrib/seekable_format/zstd_seekable_compression_format.md>`__.
+
+#. Add *mode* argument to ``ZstdFile.flush()`` method, now it can flush a zstd frame.
+
+#. Add *read_size* and *write_buffer_size* arguments to ``ZstdFile.__init__()`` method, can work with Network File Systems better.
+
+#. Optimize ``ZstdFile`` performance to C language level.
+
 **0.15.7  (Apr 21, 2023)**
 
 ZstdDict class changes:
 
 #. Fix these advanced compression parameters may be ignored when loading a dictionary: ``windowLog``, ``hashLog``, ``chainLog``, ``searchLog``, ``minMatch``, ``targetLength``, ``strategy``, ``enableLongDistanceMatching``, ``ldmHashLog``, ``ldmMinMatch``, ``ldmBucketSizeLog``, ``ldmHashRateLog``, and some non-public parameters.
 
 #. When compressing, load undigested dictionary instead of digested dictionary by default. Loading again an undigested is slower, see `differences <https://pyzstd.readthedocs.io/en/latest/#ZstdDict.as_digested_dict>`_.
```

### Comparing `pyzstd-0.15.7/README.rst` & `pyzstd-0.15.8/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,38 @@
 Pyzstd module provides classes and functions for compressing and decompressing data, using Facebook's `Zstandard <http://www.zstd.net>`_ (or zstd as short name) algorithm.
 
 The API style is similar to Python's bz2/lzma/zlib modules.
 
 * Includes zstd v1.5.5 source code
 * Can also dynamically link to zstd library provided by system, see `this note <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
 * Has a CFFI implementation that can work with PyPy
+* ``ZstdFile`` class has C language level performance
+* Supports `Zstandard Seekable Format <https://github.com/facebook/zstd/blob/dev/contrib/seekable_format/zstd_seekable_compression_format.md>`__
 * Has a command line interface: ``python -m pyzstd --help``
 
-
 Links
 -----------
 
 Documentation: https://pyzstd.readthedocs.io/en/latest
 
 GitHub: https://github.com/animalize/pyzstd
 
 
 Release note
 ------------
+**0.15.8  (Jun 13, 2023)**
+
+#. Add `SeekableZstdFile <https://pyzstd.readthedocs.io/en/latest/#SeekableZstdFile>`_ class, it's a subclass of ``ZstdFile``, supports `Zstandard Seekable Format <https://github.com/facebook/zstd/blob/dev/contrib/seekable_format/zstd_seekable_compression_format.md>`__.
+
+#. Add *mode* argument to ``ZstdFile.flush()`` method, now it can flush a zstd frame.
+
+#. Add *read_size* and *write_buffer_size* arguments to ``ZstdFile.__init__()`` method, can work with Network File Systems better.
+
+#. Optimize ``ZstdFile`` performance to C language level.
+
 **0.15.7  (Apr 21, 2023)**
 
 ZstdDict class changes:
 
 #. Fix these advanced compression parameters may be ignored when loading a dictionary: ``windowLog``, ``hashLog``, ``chainLog``, ``searchLog``, ``minMatch``, ``targetLength``, ``strategy``, ``enableLongDistanceMatching``, ``ldmHashLog``, ``ldmMinMatch``, ``ldmBucketSizeLog``, ``ldmHashRateLog``, and some non-public parameters.
 
 #. When compressing, load undigested dictionary instead of digested dictionary by default. Loading again an undigested is slower, see `differences <https://pyzstd.readthedocs.io/en/latest/#ZstdDict.as_digested_dict>`_.
```

### Comparing `pyzstd-0.15.7/index.rst` & `pyzstd-0.15.8/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -14,4814 +14,5085 @@
 000000d0: 616d 6529 2061 6c67 6f72 6974 686d 2e0a  ame) algorithm..
 000000e0: 0a54 6865 2041 5049 2073 7479 6c65 2069  .The API style i
 000000f0: 7320 7369 6d69 6c61 7220 746f 2050 7974  s similar to Pyt
 00000100: 686f 6e27 7320 627a 322f 6c7a 6d61 2f7a  hon's bz2/lzma/z
 00000110: 6c69 6220 6d6f 6475 6c65 732e 0a0a 2a20  lib modules...* 
 00000120: 496e 636c 7564 6573 2074 6865 206c 6174  Includes the lat
 00000130: 6573 7420 7a73 7464 206c 6962 7261 7279  est zstd library
-00000140: 2073 6f75 7263 6520 636f 6465 2e0a 2a20   source code..* 
-00000150: 4361 6e20 616c 736f 2064 796e 616d 6963  Can also dynamic
-00000160: 616c 6c79 206c 696e 6b20 746f 207a 7374  ally link to zst
-00000170: 6420 6c69 6272 6172 7920 7072 6f76 6964  d library provid
-00000180: 6564 2062 7920 7379 7374 656d 2c20 7365  ed by system, se
-00000190: 6520 3a72 6566 3a60 7468 6973 206e 6f74  e :ref:`this not
-000001a0: 653c 6275 696c 645f 7079 7a73 7464 3e60  e<build_pyzstd>`
-000001b0: 2e0a 2a20 4861 7320 6120 4346 4649 2069  ..* Has a CFFI i
-000001c0: 6d70 6c65 6d65 6e74 6174 696f 6e20 7468  mplementation th
-000001d0: 6174 2063 616e 2077 6f72 6b20 7769 7468  at can work with
-000001e0: 2050 7950 792e 0a2a 2048 6173 2061 2063   PyPy..* Has a c
-000001f0: 6f6d 6d61 6e64 206c 696e 6520 696e 7465  ommand line inte
-00000200: 7266 6163 652c 2060 6070 7974 686f 6e20  rface, ``python 
-00000210: 2d6d 2070 797a 7374 6420 2d2d 6865 6c70  -m pyzstd --help
-00000220: 6060 2e0a 0a4c 696e 6b73 3a20 6047 6974  ``...Links: `Git
-00000230: 4875 6220 7061 6765 203c 6874 7470 733a  Hub page <https:
-00000240: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6e69  //github.com/ani
-00000250: 6d61 6c69 7a65 2f70 797a 7374 643e 605f  malize/pyzstd>`_
-00000260: 2c20 6050 7950 4920 7061 6765 203c 6874  , `PyPI page <ht
-00000270: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000280: 726f 6a65 6374 2f70 797a 7374 643e 605f  roject/pyzstd>`_
-00000290: 2e0a 0a46 6561 7475 7265 7320 6f66 207a  ...Features of z
-000002a0: 7374 643a 0a0a 2a20 4661 7374 2063 6f6d  std:..* Fast com
-000002b0: 7072 6573 7369 6f6e 2061 6e64 2064 6563  pression and dec
-000002c0: 6f6d 7072 6573 7369 6f6e 2073 7065 6564  ompression speed
-000002d0: 2e0a 2a20 4966 2075 7365 203a 7265 663a  ..* If use :ref:
-000002e0: 606d 756c 7469 2d74 6872 6561 6465 6420  `multi-threaded 
-000002f0: 636f 6d70 7265 7373 696f 6e3c 6d74 5f63  compression<mt_c
-00000300: 6f6d 7072 6573 7369 6f6e 3e60 2c20 7468  ompression>`, th
-00000310: 6520 636f 6d70 7265 7373 696f 6e20 7370  e compression sp
-00000320: 6565 6420 696d 7072 6f76 6573 2073 6967  eed improves sig
-00000330: 6e69 6669 6361 6e74 6c79 2e0a 2a20 4966  nificantly..* If
-00000340: 2075 7365 2070 7265 2d74 7261 696e 6564   use pre-trained
-00000350: 203a 7265 663a 6064 6963 7469 6f6e 6172   :ref:`dictionar
-00000360: 793c 7a73 7464 5f64 6963 743e 602c 2074  y<zstd_dict>`, t
-00000370: 6865 2063 6f6d 7072 6573 7369 6f6e 2072  he compression r
-00000380: 6174 696f 206f 6e20 736d 616c 6c20 6461  atio on small da
-00000390: 7461 2028 6120 6665 7720 4b69 4229 2069  ta (a few KiB) i
-000003a0: 6d70 726f 7665 7320 6472 616d 6174 6963  mproves dramatic
-000003b0: 616c 6c79 2e0a 2a20 3a72 6566 3a60 4672  ally..* :ref:`Fr
-000003c0: 616d 6520 616e 6420 626c 6f63 6b3c 6672  ame and block<fr
-000003d0: 616d 655f 626c 6f63 6b3e 6020 616c 6c6f  ame_block>` allo
-000003e0: 7720 7468 6520 7573 6520 6d6f 7265 2066  w the use more f
-000003f0: 6c65 7869 626c 652c 2073 7569 7461 626c  lexible, suitabl
-00000400: 6520 666f 7220 6d61 6e79 2073 6365 6e61  e for many scena
-00000410: 7269 6f73 2e0a 2a20 4361 6e20 6265 2075  rios..* Can be u
-00000420: 7365 6420 6173 2061 203a 7265 663a 6070  sed as a :ref:`p
-00000430: 6174 6368 696e 6720 656e 6769 6e65 3c70  atching engine<p
-00000440: 6174 6368 696e 675f 656e 6769 6e65 3e60  atching_engine>`
-00000450: 2e0a 0a2e 2e20 6e6f 7465 3a3a 0a20 2020  ..... note::.   
-00000460: 2054 776f 206f 7468 6572 207a 7374 6420   Two other zstd 
-00000470: 6d6f 6475 6c65 7320 6f6e 2050 7950 493a  modules on PyPI:
-00000480: 0a0a 2020 2020 2a20 607a 7374 6420 3c68  ..    * `zstd <h
-00000490: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-000004a0: 7072 6f6a 6563 742f 7a73 7464 2f3e 605f  project/zstd/>`_
-000004b0: 2c20 6120 7665 7279 2073 696d 706c 6520  , a very simple 
-000004c0: 6d6f 6475 6c65 2e0a 2020 2020 2a20 607a  module..    * `z
-000004d0: 7374 616e 6461 7264 203c 6874 7470 733a  standard <https:
-000004e0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000004f0: 6374 2f7a 7374 616e 6461 7264 2f3e 605f  ct/zstandard/>`_
-00000500: 2c20 7072 6f76 6964 6573 2072 6963 6820  , provides rich 
-00000510: 4150 492e 0a0a 4578 6365 7074 696f 6e0a  API...Exception.
-00000520: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 7079  ---------.... py
-00000530: 3a65 7863 6570 7469 6f6e 3a3a 205a 7374  :exception:: Zst
-00000540: 6445 7272 6f72 0a0a 2020 2020 5468 6973  dError..    This
-00000550: 2065 7863 6570 7469 6f6e 2069 7320 7261   exception is ra
-00000560: 6973 6564 2077 6865 6e20 616e 2065 7272  ised when an err
-00000570: 6f72 206f 6363 7572 7320 7768 656e 2063  or occurs when c
-00000580: 616c 6c69 6e67 2074 6865 2075 6e64 6572  alling the under
-00000590: 6c79 696e 6720 7a73 7464 206c 6962 7261  lying zstd libra
-000005a0: 7279 2e0a 0a0a 5369 6d70 6c65 2063 6f6d  ry....Simple com
-000005b0: 7072 6573 7369 6f6e 2f64 6563 6f6d 7072  pression/decompr
-000005c0: 6573 7369 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d  ession.---------
-000005d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005e0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2054 6869  -------..    Thi
-000005f0: 7320 7365 6374 696f 6e20 636f 6e74 6169  s section contai
-00000600: 6e73 3a0a 0a20 2020 2020 2020 202a 2066  ns:..        * f
-00000610: 756e 6374 696f 6e20 3a70 793a 6675 6e63  unction :py:func
-00000620: 3a60 636f 6d70 7265 7373 600a 2020 2020  :`compress`.    
-00000630: 2020 2020 2a20 6675 6e63 7469 6f6e 203a      * function :
-00000640: 7079 3a66 756e 633a 6064 6563 6f6d 7072  py:func:`decompr
-00000650: 6573 7360 0a0a 2020 2020 2e2e 2068 696e  ess`..    .. hin
-00000660: 743a 3a0a 2020 2020 2020 2020 4966 2074  t::.        If t
-00000670: 6865 7265 2061 7265 2061 2062 6967 206e  here are a big n
-00000680: 756d 6265 7220 6f66 2073 616d 6520 7479  umber of same ty
-00000690: 7065 2069 6e64 6976 6964 7561 6c20 6461  pe individual da
-000006a0: 7461 2c20 7265 7573 6520 7468 6573 6520  ta, reuse these 
-000006b0: 6f62 6a65 6374 7320 6d61 7920 656c 696d  objects may elim
-000006c0: 696e 6174 6520 7468 6520 736d 616c 6c20  inate the small 
-000006d0: 6f76 6572 6865 6164 206f 6620 6372 6561  overhead of crea
-000006e0: 7469 6e67 2063 6f6e 7465 7874 202f 2073  ting context / s
-000006f0: 6574 7469 6e67 2070 6172 616d 6574 6572  etting parameter
-00000700: 7320 2f20 6c6f 6164 696e 6720 6469 6374  s / loading dict
-00000710: 696f 6e61 7279 2e0a 0a20 2020 2020 2020  ionary...       
-00000720: 202a 203a 7079 3a63 6c61 7373 3a60 5a73   * :py:class:`Zs
-00000730: 7464 436f 6d70 7265 7373 6f72 600a 2020  tdCompressor`.  
-00000740: 2020 2020 2020 2a20 3a70 793a 636c 6173        * :py:clas
-00000750: 733a 6052 6963 684d 656d 5a73 7464 436f  s:`RichMemZstdCo
-00000760: 6d70 7265 7373 6f72 600a 0a0a 2e2e 2070  mpressor`..... p
-00000770: 793a 6675 6e63 7469 6f6e 3a3a 2063 6f6d  y:function:: com
-00000780: 7072 6573 7328 6461 7461 2c20 6c65 7665  press(data, leve
-00000790: 6c5f 6f72 5f6f 7074 696f 6e3d 4e6f 6e65  l_or_option=None
-000007a0: 2c20 7a73 7464 5f64 6963 743d 4e6f 6e65  , zstd_dict=None
-000007b0: 290a 0a20 2020 2043 6f6d 7072 6573 7320  )..    Compress 
-000007c0: 2a64 6174 612a 2c20 7265 7475 726e 2074  *data*, return t
-000007d0: 6865 2063 6f6d 7072 6573 7365 6420 6461  he compressed da
-000007e0: 7461 2e0a 0a20 2020 2043 6f6d 7072 6573  ta...    Compres
-000007f0: 7369 6e67 2060 6062 2727 6060 2077 696c  sing ``b''`` wil
-00000800: 6c20 6765 7420 616e 2065 6d70 7479 2063  l get an empty c
-00000810: 6f6e 7465 6e74 2066 7261 6d65 2028 3920  ontent frame (9 
-00000820: 6279 7465 7320 6f72 206d 6f72 6529 2e0a  bytes or more)..
-00000830: 0a20 2020 203a 7079 3a66 756e 633a 6072  .    :py:func:`r
-00000840: 6963 686d 656d 5f63 6f6d 7072 6573 7360  ichmem_compress`
-00000850: 2066 756e 6374 696f 6e20 6973 2066 6173   function is fas
-00000860: 7465 7220 696e 2073 6f6d 6520 6361 7365  ter in some case
-00000870: 732e 0a0a 2020 2020 3a70 6172 616d 2064  s...    :param d
-00000880: 6174 613a 2044 6174 6120 746f 2062 6520  ata: Data to be 
-00000890: 636f 6d70 7265 7373 6564 2e0a 2020 2020  compressed..    
-000008a0: 3a74 7970 6520 6461 7461 3a20 6279 7465  :type data: byte
-000008b0: 732d 6c69 6b65 206f 626a 6563 740a 2020  s-like object.  
-000008c0: 2020 3a70 6172 616d 206c 6576 656c 5f6f    :param level_o
-000008d0: 725f 6f70 7469 6f6e 3a20 5768 656e 2069  r_option: When i
-000008e0: 7427 7320 616e 2060 6069 6e74 6060 206f  t's an ``int`` o
-000008f0: 626a 6563 742c 2069 7420 7265 7072 6573  bject, it repres
-00000900: 656e 7473 203a 7265 663a 6063 6f6d 7072  ents :ref:`compr
-00000910: 6573 7369 6f6e 206c 6576 656c 3c63 6f6d  ession level<com
-00000920: 7072 6573 7369 6f6e 5f6c 6576 656c 3e60  pression_level>`
-00000930: 2e20 5768 656e 2069 7427 7320 6120 6060  . When it's a ``
-00000940: 6469 6374 6060 206f 626a 6563 742c 2069  dict`` object, i
-00000950: 7420 636f 6e74 6169 6e73 203a 7265 663a  t contains :ref:
-00000960: 6061 6476 616e 6365 6420 636f 6d70 7265  `advanced compre
-00000970: 7373 696f 6e20 7061 7261 6d65 7465 7273  ssion parameters
-00000980: 3c43 5061 7261 6d65 7465 723e 602e 2054  <CParameter>`. T
-00000990: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
-000009a0: 2060 604e 6f6e 6560 6020 6d65 616e 7320   ``None`` means 
-000009b0: 746f 2075 7365 207a 7374 6427 7320 6465  to use zstd's de
-000009c0: 6661 756c 7420 636f 6d70 7265 7373 696f  fault compressio
-000009d0: 6e20 6c65 7665 6c2f 7061 7261 6d65 7465  n level/paramete
-000009e0: 7273 2e0a 2020 2020 3a74 7970 6520 6c65  rs..    :type le
-000009f0: 7665 6c5f 6f72 5f6f 7074 696f 6e3a 2069  vel_or_option: i
-00000a00: 6e74 206f 7220 6469 6374 0a20 2020 203a  nt or dict.    :
-00000a10: 7061 7261 6d20 7a73 7464 5f64 6963 743a  param zstd_dict:
-00000a20: 2050 7265 2d74 7261 696e 6564 2064 6963   Pre-trained dic
-00000a30: 7469 6f6e 6172 7920 666f 7220 636f 6d70  tionary for comp
-00000a40: 7265 7373 696f 6e2e 0a20 2020 203a 7479  ression..    :ty
-00000a50: 7065 207a 7374 645f 6469 6374 3a20 5a73  pe zstd_dict: Zs
-00000a60: 7464 4469 6374 0a20 2020 203a 7265 7475  tdDict.    :retu
-00000a70: 726e 3a20 436f 6d70 7265 7373 6564 2064  rn: Compressed d
-00000a80: 6174 610a 2020 2020 3a72 7479 7065 3a20  ata.    :rtype: 
-00000a90: 6279 7465 730a 0a2e 2e20 736f 7572 6365  bytes.... source
-00000aa0: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-00000ab0: 2020 2023 2069 6e74 2063 6f6d 7072 6573     # int compres
-00000ac0: 7369 6f6e 206c 6576 656c 0a20 2020 2063  sion level.    c
-00000ad0: 6f6d 7072 6573 7365 645f 6461 7420 3d20  ompressed_dat = 
-00000ae0: 636f 6d70 7265 7373 2872 6177 5f64 6174  compress(raw_dat
-00000af0: 2c20 3130 290a 0a20 2020 2023 2064 6963  , 10)..    # dic
-00000b00: 7420 6f70 7469 6f6e 2c20 7573 6520 3620  t option, use 6 
-00000b10: 7468 7265 6164 7320 746f 2063 6f6d 7072  threads to compr
-00000b20: 6573 732c 2061 6e64 2061 7070 656e 6420  ess, and append 
-00000b30: 6120 342d 6279 7465 2063 6865 636b 7375  a 4-byte checksu
-00000b40: 6d2e 0a20 2020 206f 7074 696f 6e20 3d20  m..    option = 
-00000b50: 7b43 5061 7261 6d65 7465 722e 636f 6d70  {CParameter.comp
-00000b60: 7265 7373 696f 6e4c 6576 656c 203a 2031  ressionLevel : 1
-00000b70: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00000b80: 2043 5061 7261 6d65 7465 722e 6e62 576f   CParameter.nbWo
-00000b90: 726b 6572 7320 3a20 362c 0a20 2020 2020  rkers : 6,.     
-00000ba0: 2020 2020 2020 2020 2043 5061 7261 6d65           CParame
-00000bb0: 7465 722e 6368 6563 6b73 756d 466c 6167  ter.checksumFlag
-00000bc0: 203a 2031 7d0a 2020 2020 636f 6d70 7265   : 1}.    compre
-00000bd0: 7373 6564 5f64 6174 203d 2063 6f6d 7072  ssed_dat = compr
-00000be0: 6573 7328 7261 775f 6461 742c 206f 7074  ess(raw_dat, opt
-00000bf0: 696f 6e29 0a0a 0a2e 2e20 7079 3a66 756e  ion)..... py:fun
-00000c00: 6374 696f 6e3a 3a20 6465 636f 6d70 7265  ction:: decompre
-00000c10: 7373 2864 6174 612c 207a 7374 645f 6469  ss(data, zstd_di
-00000c20: 6374 3d4e 6f6e 652c 206f 7074 696f 6e3d  ct=None, option=
-00000c30: 4e6f 6e65 290a 0a20 2020 2044 6563 6f6d  None)..    Decom
-00000c40: 7072 6573 7320 2a64 6174 612a 2c20 7265  press *data*, re
-00000c50: 7475 726e 2074 6865 2064 6563 6f6d 7072  turn the decompr
-00000c60: 6573 7365 6420 6461 7461 2e0a 0a20 2020  essed data...   
-00000c70: 2053 7570 706f 7274 206d 756c 7469 706c   Support multipl
-00000c80: 6520 636f 6e63 6174 656e 6174 6564 203a  e concatenated :
-00000c90: 7265 663a 6066 7261 6d65 733c 6672 616d  ref:`frames<fram
-00000ca0: 655f 626c 6f63 6b3e 602e 0a0a 2020 2020  e_block>`...    
-00000cb0: 3a70 6172 616d 2064 6174 613a 2044 6174  :param data: Dat
-00000cc0: 6120 746f 2062 6520 6465 636f 6d70 7265  a to be decompre
-00000cd0: 7373 6564 2e0a 2020 2020 3a74 7970 6520  ssed..    :type 
-00000ce0: 6461 7461 3a20 6279 7465 732d 6c69 6b65  data: bytes-like
-00000cf0: 206f 626a 6563 740a 2020 2020 3a70 6172   object.    :par
-00000d00: 616d 207a 7374 645f 6469 6374 3a20 5072  am zstd_dict: Pr
-00000d10: 652d 7472 6169 6e65 6420 6469 6374 696f  e-trained dictio
-00000d20: 6e61 7279 2066 6f72 2064 6563 6f6d 7072  nary for decompr
-00000d30: 6573 7369 6f6e 2e0a 2020 2020 3a74 7970  ession..    :typ
-00000d40: 6520 7a73 7464 5f64 6963 743a 205a 7374  e zstd_dict: Zst
-00000d50: 6444 6963 740a 2020 2020 3a70 6172 616d  dDict.    :param
-00000d60: 206f 7074 696f 6e3a 2041 2060 6064 6963   option: A ``dic
-00000d70: 7460 6020 6f62 6a65 6374 2074 6861 7420  t`` object that 
-00000d80: 636f 6e74 6169 6e73 203a 7079 3a72 6566  contains :py:ref
-00000d90: 3a60 6164 7661 6e63 6564 2064 6563 6f6d  :`advanced decom
-00000da0: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
-00000db0: 6572 733c 4450 6172 616d 6574 6572 3e60  ers<DParameter>`
-00000dc0: 2e20 5468 6520 6465 6661 756c 7420 7661  . The default va
-00000dd0: 6c75 6520 6060 4e6f 6e65 6060 206d 6561  lue ``None`` mea
-00000de0: 6e73 2074 6f20 7573 6520 7a73 7464 2773  ns to use zstd's
-00000df0: 2064 6566 6175 6c74 2064 6563 6f6d 7072   default decompr
-00000e00: 6573 7369 6f6e 2070 6172 616d 6574 6572  ession parameter
-00000e10: 732e 0a20 2020 203a 7479 7065 206f 7074  s..    :type opt
-00000e20: 696f 6e3a 2064 6963 740a 2020 2020 3a72  ion: dict.    :r
-00000e30: 6574 7572 6e3a 2044 6563 6f6d 7072 6573  eturn: Decompres
-00000e40: 7365 6420 6461 7461 0a20 2020 203a 7274  sed data.    :rt
-00000e50: 7970 653a 2062 7974 6573 0a20 2020 203a  ype: bytes.    :
-00000e60: 7261 6973 6573 205a 7374 6445 7272 6f72  raises ZstdError
-00000e70: 3a20 4966 2064 6563 6f6d 7072 6573 7369  : If decompressi
-00000e80: 6f6e 2066 6169 6c73 2e0a 0a0a 5269 6368  on fails....Rich
-00000e90: 206d 656d 6f72 7920 636f 6d70 7265 7373   memory compress
-00000ea0: 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ion.------------
-00000eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020  -----------..   
-00000ec0: 2043 6f6d 7072 6573 7320 6461 7461 2075   Compress data u
-00000ed0: 7369 6e67 203a 7265 663a 6072 6963 6820  sing :ref:`rich 
-00000ee0: 6d65 6d6f 7279 206d 6f64 653c 7269 6368  memory mode<rich
-00000ef0: 5f6d 656d 3e60 2e20 5468 6973 206d 6f64  _mem>`. This mod
-00000f00: 6520 616c 6c6f 6361 7465 7320 6d6f 7265  e allocates more
-00000f10: 206d 656d 6f72 7920 666f 7220 6f75 7470   memory for outp
-00000f20: 7574 2062 7566 6665 722c 2069 7427 7320  ut buffer, it's 
-00000f30: 6661 7374 6572 2069 6e20 736f 6d65 2063  faster in some c
-00000f40: 6173 6573 2e0a 0a20 2020 2054 6869 7320  ases...    This 
-00000f50: 7365 6374 696f 6e20 636f 6e74 6169 6e73  section contains
-00000f60: 3a0a 0a20 2020 2020 2020 202a 2066 756e  :..        * fun
-00000f70: 6374 696f 6e20 3a70 793a 6675 6e63 3a60  ction :py:func:`
-00000f80: 7269 6368 6d65 6d5f 636f 6d70 7265 7373  richmem_compress
-00000f90: 600a 2020 2020 2020 2020 2a20 636c 6173  `.        * clas
-00000fa0: 7320 3a70 793a 636c 6173 733a 6052 6963  s :py:class:`Ric
-00000fb0: 684d 656d 5a73 7464 436f 6d70 7265 7373  hMemZstdCompress
-00000fc0: 6f72 602c 2061 2072 6575 7361 626c 6520  or`, a reusable 
-00000fd0: 636f 6d70 7265 7373 6f72 2e0a 0a2e 2e20  compressor..... 
-00000fe0: 7079 3a66 756e 6374 696f 6e3a 3a20 7269  py:function:: ri
-00000ff0: 6368 6d65 6d5f 636f 6d70 7265 7373 2864  chmem_compress(d
-00001000: 6174 612c 206c 6576 656c 5f6f 725f 6f70  ata, level_or_op
-00001010: 7469 6f6e 3d4e 6f6e 652c 207a 7374 645f  tion=None, zstd_
-00001020: 6469 6374 3d4e 6f6e 6529 0a0a 2020 2020  dict=None)..    
-00001030: 5573 6520 3a72 6566 3a60 7269 6368 206d  Use :ref:`rich m
-00001040: 656d 6f72 7920 6d6f 6465 3c72 6963 685f  emory mode<rich_
-00001050: 6d65 6d3e 6020 746f 2063 6f6d 7072 6573  mem>` to compres
-00001060: 7320 2a64 6174 612a 2e20 4974 2773 2066  s *data*. It's f
-00001070: 6173 7465 7220 7468 616e 203a 7079 3a66  aster than :py:f
-00001080: 756e 633a 6063 6f6d 7072 6573 7360 2069  unc:`compress` i
-00001090: 6e20 736f 6d65 2063 6173 6573 2c20 6275  n some cases, bu
-000010a0: 7420 616c 6c6f 6361 7465 7320 6d6f 7265  t allocates more
-000010b0: 206d 656d 6f72 792e 0a0a 2020 2020 5468   memory...    Th
-000010c0: 6520 7061 7261 6d65 7465 7273 2061 7265  e parameters are
-000010d0: 2074 6865 2073 616d 6520 6173 203a 7079   the same as :py
-000010e0: 3a66 756e 633a 6063 6f6d 7072 6573 7360  :func:`compress`
-000010f0: 2066 756e 6374 696f 6e2e 0a0a 2020 2020   function...    
-00001100: 436f 6d70 7265 7373 696e 6720 6060 6227  Compressing ``b'
-00001110: 2760 6020 7769 6c6c 2067 6574 2061 6e20  '`` will get an 
-00001120: 656d 7074 7920 636f 6e74 656e 7420 6672  empty content fr
-00001130: 616d 6520 2839 2062 7974 6573 206f 7220  ame (9 bytes or 
-00001140: 6d6f 7265 292e 0a0a 0a2e 2e20 7079 3a63  more)...... py:c
-00001150: 6c61 7373 3a3a 2052 6963 684d 656d 5a73  lass:: RichMemZs
-00001160: 7464 436f 6d70 7265 7373 6f72 0a0a 2020  tdCompressor..  
-00001170: 2020 4120 7265 7573 6162 6c65 2063 6f6d    A reusable com
-00001180: 7072 6573 736f 7220 7573 696e 6720 3a72  pressor using :r
-00001190: 6566 3a60 7269 6368 206d 656d 6f72 7920  ef:`rich memory 
-000011a0: 6d6f 6465 3c72 6963 685f 6d65 6d3e 602e  mode<rich_mem>`.
-000011b0: 2049 7420 6361 6e20 6265 2072 6575 7365   It can be reuse
-000011c0: 6420 666f 7220 6269 6720 6e75 6d62 6572  d for big number
-000011d0: 206f 6620 7361 6d65 2074 7970 6520 696e   of same type in
-000011e0: 6469 7669 6475 616c 2064 6174 612e 0a0a  dividual data...
-000011f0: 2020 2020 5369 6e63 6520 6974 2063 616e      Since it can
-00001200: 206f 6e6c 7920 6765 6e65 7261 7465 7320   only generates 
-00001210: 696e 6469 7669 6475 616c 203a 7265 663a  individual :ref:
-00001220: 6066 7261 6d65 733c 6672 616d 655f 626c  `frames<frame_bl
-00001230: 6f63 6b3e 602c 2069 7427 7320 6e6f 7420  ock>`, it's not 
-00001240: 7375 6974 6162 6c65 2066 6f72 2073 7472  suitable for str
-00001250: 6561 6d69 6e67 2063 6f6d 7072 6573 7369  eaming compressi
-00001260: 6f6e 2c20 6f74 6865 7277 6973 6520 7468  on, otherwise th
-00001270: 6520 636f 6d70 7265 7373 696f 6e20 7261  e compression ra
-00001280: 7469 6f20 7769 6c6c 2062 6520 7265 6475  tio will be redu
-00001290: 6365 642c 2061 6e64 2073 6f6d 6520 7072  ced, and some pr
-000012a0: 6f67 7261 6d73 2063 616e 2774 2064 6563  ograms can't dec
-000012b0: 6f6d 7072 6573 7320 6d75 6c74 6970 6c65  ompress multiple
-000012c0: 2066 7261 6d65 7320 6461 7461 2e20 466f   frames data. Fo
-000012d0: 7220 7374 7265 616d 696e 6720 636f 6d70  r streaming comp
-000012e0: 7265 7373 696f 6e2c 2073 6565 203a 7265  ression, see :re
-000012f0: 663a 6074 6869 7320 7365 6374 696f 6e3c  f:`this section<
-00001300: 7374 7265 616d 5f63 6f6d 7072 6573 7369  stream_compressi
-00001310: 6f6e 3e60 2e0a 0a20 2020 2054 6872 6561  on>`...    Threa
-00001320: 642d 7361 6665 2061 7420 6d65 7468 6f64  d-safe at method
-00001330: 206c 6576 656c 2e0a 0a20 2020 202e 2e20   level...    .. 
-00001340: 7079 3a6d 6574 686f 643a 3a20 5f5f 696e  py:method:: __in
-00001350: 6974 5f5f 2873 656c 662c 206c 6576 656c  it__(self, level
-00001360: 5f6f 725f 6f70 7469 6f6e 3d4e 6f6e 652c  _or_option=None,
-00001370: 207a 7374 645f 6469 6374 3d4e 6f6e 6529   zstd_dict=None)
-00001380: 0a0a 2020 2020 2020 2020 5468 6520 7061  ..        The pa
-00001390: 7261 6d65 7465 7273 2061 7265 2074 6865  rameters are the
-000013a0: 2073 616d 6520 6173 203a 7079 3a6d 6574   same as :py:met
-000013b0: 683a 605a 7374 6443 6f6d 7072 6573 736f  h:`ZstdCompresso
-000013c0: 722e 5f5f 696e 6974 5f5f 6020 6d65 7468  r.__init__` meth
-000013d0: 6f64 2e0a 0a20 2020 202e 2e20 7079 3a6d  od...    .. py:m
-000013e0: 6574 686f 643a 3a20 636f 6d70 7265 7373  ethod:: compress
-000013f0: 2873 656c 662c 2064 6174 6129 0a0a 2020  (self, data)..  
-00001400: 2020 2020 2020 436f 6d70 7265 7373 202a        Compress *
-00001410: 6461 7461 2a20 7573 696e 6720 3a72 6566  data* using :ref
-00001420: 3a60 7269 6368 206d 656d 6f72 7920 6d6f  :`rich memory mo
-00001430: 6465 3c72 6963 685f 6d65 6d3e 602c 2072  de<rich_mem>`, r
-00001440: 6574 7572 6e20 6120 7369 6e67 6c65 207a  eturn a single z
-00001450: 7374 6420 3a72 6566 3a60 6672 616d 653c  std :ref:`frame<
-00001460: 6672 616d 655f 626c 6f63 6b3e 602e 0a0a  frame_block>`...
-00001470: 2020 2020 2020 2020 436f 6d70 7265 7373          Compress
-00001480: 696e 6720 6060 6227 2760 6020 7769 6c6c  ing ``b''`` will
-00001490: 2067 6574 2061 6e20 656d 7074 7920 636f   get an empty co
-000014a0: 6e74 656e 7420 6672 616d 6520 2839 2062  ntent frame (9 b
-000014b0: 7974 6573 206f 7220 6d6f 7265 292e 0a0a  ytes or more)...
-000014c0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-000014d0: 6174 613a 2044 6174 6120 746f 2062 6520  ata: Data to be 
-000014e0: 636f 6d70 7265 7373 6564 2e0a 2020 2020  compressed..    
-000014f0: 2020 2020 3a74 7970 6520 6461 7461 3a20      :type data: 
-00001500: 6279 7465 732d 6c69 6b65 206f 626a 6563  bytes-like objec
-00001510: 740a 2020 2020 2020 2020 3a72 6574 7572  t.        :retur
-00001520: 6e3a 2041 2073 696e 676c 6520 7a73 7464  n: A single zstd
-00001530: 2066 7261 6d65 2e0a 2020 2020 2020 2020   frame..        
-00001540: 3a72 7479 7065 3a20 6279 7465 730a 0a20  :rtype: bytes.. 
-00001550: 2020 202e 2e20 736f 7572 6365 636f 6465     .. sourcecode
-00001560: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-00001570: 2020 2063 203d 2052 6963 684d 656d 5a73     c = RichMemZs
-00001580: 7464 436f 6d70 7265 7373 6f72 2829 0a20  tdCompressor(). 
-00001590: 2020 2020 2020 2066 7261 6d65 3120 3d20         frame1 = 
-000015a0: 632e 636f 6d70 7265 7373 2872 6177 5f64  c.compress(raw_d
-000015b0: 6174 3129 0a20 2020 2020 2020 2066 7261  at1).        fra
-000015c0: 6d65 3220 3d20 632e 636f 6d70 7265 7373  me2 = c.compress
-000015d0: 2872 6177 5f64 6174 3229 0a0a 0a2e 2e20  (raw_dat2)..... 
-000015e0: 5f73 7472 6561 6d5f 636f 6d70 7265 7373  _stream_compress
-000015f0: 696f 6e3a 0a0a 5374 7265 616d 696e 6720  ion:..Streaming 
-00001600: 636f 6d70 7265 7373 696f 6e0a 2d2d 2d2d  compression.----
-00001610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001620: 2d0a 0a20 2020 2054 6869 7320 7365 6374  -..    This sect
-00001630: 696f 6e20 636f 6e74 6169 6e73 3a0a 0a20  ion contains:.. 
-00001640: 2020 2020 2020 202a 2066 756e 6374 696f         * functio
-00001650: 6e20 3a70 793a 6675 6e63 3a60 636f 6d70  n :py:func:`comp
-00001660: 7265 7373 5f73 7472 6561 6d60 2c20 6120  ress_stream`, a 
-00001670: 6661 7374 2061 6e64 2063 6f6e 7665 6e69  fast and conveni
-00001680: 656e 7420 6675 6e63 7469 6f6e 2e0a 2020  ent function..  
-00001690: 2020 2020 2020 2a20 636c 6173 7320 3a70        * class :p
-000016a0: 793a 636c 6173 733a 605a 7374 6443 6f6d  y:class:`ZstdCom
-000016b0: 7072 6573 736f 7260 2c20 7369 6d69 6c61  pressor`, simila
-000016c0: 7220 746f 2063 6f6d 7072 6573 736f 7273  r to compressors
-000016d0: 2069 6e20 5079 7468 6f6e 2073 7461 6e64   in Python stand
-000016e0: 6172 6420 6c69 6272 6172 792e 0a0a 2020  ard library...  
-000016f0: 2020 4974 2077 6f75 6c64 2062 6520 6e69    It would be ni
-00001700: 6365 2074 6f20 6b6e 6f77 2073 6f6d 6520  ce to know some 
-00001710: 6b6e 6f77 6c65 6467 6520 6162 6f75 7420  knowledge about 
-00001720: 7a73 7464 2064 6174 612c 2073 6565 203a  zstd data, see :
-00001730: 7265 663a 6066 7261 6d65 2061 6e64 2062  ref:`frame and b
-00001740: 6c6f 636b 3c66 7261 6d65 5f62 6c6f 636b  lock<frame_block
-00001750: 3e60 2e0a 0a2e 2e20 7079 3a66 756e 6374  >`..... py:funct
-00001760: 696f 6e3a 3a20 636f 6d70 7265 7373 5f73  ion:: compress_s
-00001770: 7472 6561 6d28 696e 7075 745f 7374 7265  tream(input_stre
-00001780: 616d 2c20 6f75 7470 7574 5f73 7472 6561  am, output_strea
-00001790: 6d2c 202a 2c20 6c65 7665 6c5f 6f72 5f6f  m, *, level_or_o
-000017a0: 7074 696f 6e3d 4e6f 6e65 2c20 7a73 7464  ption=None, zstd
-000017b0: 5f64 6963 743d 4e6f 6e65 2c20 706c 6564  _dict=None, pled
-000017c0: 6765 645f 696e 7075 745f 7369 7a65 3d4e  ged_input_size=N
-000017d0: 6f6e 652c 2072 6561 645f 7369 7a65 3d31  one, read_size=1
-000017e0: 3331 5f30 3732 2c20 7772 6974 655f 7369  31_072, write_si
-000017f0: 7a65 3d31 3331 5f35 3931 2c20 6361 6c6c  ze=131_591, call
-00001800: 6261 636b 3d4e 6f6e 6529 0a0a 2020 2020  back=None)..    
-00001810: 4120 6661 7374 2061 6e64 2063 6f6e 7665  A fast and conve
-00001820: 6e69 656e 7420 6675 6e63 7469 6f6e 2c20  nient function, 
-00001830: 636f 6d70 7265 7373 6573 202a 696e 7075  compresses *inpu
-00001840: 745f 7374 7265 616d 2a20 616e 6420 7772  t_stream* and wr
-00001850: 6974 6573 2074 6865 2063 6f6d 7072 6573  ites the compres
-00001860: 7365 6420 6461 7461 2074 6f20 2a6f 7574  sed data to *out
-00001870: 7075 745f 7374 7265 616d 2a2c 2069 7420  put_stream*, it 
-00001880: 646f 6573 6e27 7420 636c 6f73 6520 7468  doesn't close th
-00001890: 6520 7374 7265 616d 732e 0a0a 2020 2020  e streams...    
-000018a0: 4966 2069 6e70 7574 2073 7472 6561 6d20  If input stream 
-000018b0: 6973 2060 6062 2727 6060 2c20 6e6f 7468  is ``b''``, noth
-000018c0: 696e 6720 7769 6c6c 2062 6520 7772 6974  ing will be writ
-000018d0: 7465 6e20 746f 206f 7574 7075 7420 7374  ten to output st
-000018e0: 7265 616d 2e0a 0a20 2020 2054 6869 7320  ream...    This 
-000018f0: 6675 6e63 7469 6f6e 2074 7269 6573 2074  function tries t
-00001900: 6f20 7a65 726f 2d63 6f70 7920 6173 206d  o zero-copy as m
-00001910: 7563 6820 6173 2070 6f73 7369 626c 652e  uch as possible.
-00001920: 2049 6620 7468 6520 4f53 2068 6173 2072   If the OS has r
-00001930: 6561 6420 7072 6566 6574 6368 696e 6720  ead prefetching 
-00001940: 616e 6420 7772 6974 6520 6275 6666 6572  and write buffer
-00001950: 2c20 6974 206d 6179 2070 6572 666f 726d  , it may perform
-00001960: 2074 6865 2074 6173 6b73 2028 7265 6164   the tasks (read
-00001970: 2f63 6f6d 7072 6573 732f 7772 6974 6529  /compress/write)
-00001980: 2069 6e20 7061 7261 6c6c 656c 2074 6f20   in parallel to 
-00001990: 736f 6d65 2064 6567 7265 652e 0a0a 2020  some degree...  
-000019a0: 2020 5468 6520 6465 6661 756c 7420 7661    The default va
-000019b0: 6c75 6573 206f 6620 2a72 6561 645f 7369  lues of *read_si
-000019c0: 7a65 2a20 616e 6420 2a77 7269 7465 5f73  ze* and *write_s
-000019d0: 697a 652a 2070 6172 616d 6574 6572 7320  ize* parameters 
-000019e0: 6172 6520 7468 6520 6275 6666 6572 2073  are the buffer s
-000019f0: 697a 6573 2072 6563 6f6d 6d65 6e64 6564  izes recommended
-00001a00: 2062 7920 7a73 7464 2c20 696e 6372 6561   by zstd, increa
-00001a10: 7369 6e67 2074 6865 6d20 6d61 7920 6265  sing them may be
-00001a20: 2066 6173 7465 722c 2061 6e64 2072 6564   faster, and red
-00001a30: 7563 6573 2074 6865 206e 756d 6265 7220  uces the number 
-00001a40: 6f66 2063 616c 6c62 6163 6b20 6675 6e63  of callback func
-00001a50: 7469 6f6e 2063 616c 6c73 2e0a 0a20 2020  tion calls...   
-00001a60: 202e 2e20 7665 7273 696f 6e61 6464 6564   .. versionadded
-00001a70: 3a3a 2030 2e31 342e 320a 0a20 2020 203a  :: 0.14.2..    :
-00001a80: 7061 7261 6d20 696e 7075 745f 7374 7265  param input_stre
-00001a90: 616d 3a20 496e 7075 7420 7374 7265 616d  am: Input stream
-00001aa0: 2074 6861 7420 6861 7320 6120 602e 7265   that has a `.re
-00001ab0: 6164 696e 746f 2862 2920 3c68 7474 7073  adinto(b) <https
-00001ac0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00001ad0: 7267 2f33 2f6c 6962 7261 7279 2f69 6f2e  rg/3/library/io.
-00001ae0: 6874 6d6c 2369 6f2e 5261 7749 4f42 6173  html#io.RawIOBas
-00001af0: 652e 7265 6164 696e 746f 3e60 5f20 6d65  e.readinto>`_ me
-00001b00: 7468 6f64 2e0a 2020 2020 3a70 6172 616d  thod..    :param
-00001b10: 206f 7574 7075 745f 7374 7265 616d 3a20   output_stream: 
-00001b20: 4f75 7470 7574 2073 7472 6561 6d20 7468  Output stream th
-00001b30: 6174 2068 6173 2061 2060 2e77 7269 7465  at has a `.write
-00001b40: 2862 2920 3c68 7474 7073 3a2f 2f64 6f63  (b) <https://doc
-00001b50: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-00001b60: 6962 7261 7279 2f69 6f2e 6874 6d6c 2369  ibrary/io.html#i
-00001b70: 6f2e 5261 7749 4f42 6173 652e 7772 6974  o.RawIOBase.writ
-00001b80: 653e 605f 206d 6574 686f 642e 2049 6620  e>`_ method. If 
-00001b90: 7573 6520 2a63 616c 6c62 6163 6b2a 2066  use *callback* f
-00001ba0: 756e 6374 696f 6e2c 2074 6869 7320 7061  unction, this pa
-00001bb0: 7261 6d65 7465 7220 6361 6e20 6265 2060  rameter can be `
-00001bc0: 604e 6f6e 6560 602e 0a20 2020 203a 7061  `None``..    :pa
-00001bd0: 7261 6d20 6c65 7665 6c5f 6f72 5f6f 7074  ram level_or_opt
-00001be0: 696f 6e3a 2057 6865 6e20 6974 2773 2061  ion: When it's a
-00001bf0: 6e20 6060 696e 7460 6020 6f62 6a65 6374  n ``int`` object
-00001c00: 2c20 6974 2072 6570 7265 7365 6e74 7320  , it represents 
-00001c10: 3a72 6566 3a60 636f 6d70 7265 7373 696f  :ref:`compressio
-00001c20: 6e20 6c65 7665 6c3c 636f 6d70 7265 7373  n level<compress
-00001c30: 696f 6e5f 6c65 7665 6c3e 602e 2057 6865  ion_level>`. Whe
-00001c40: 6e20 6974 2773 2061 2060 6064 6963 7460  n it's a ``dict`
-00001c50: 6020 6f62 6a65 6374 2c20 6974 2063 6f6e  ` object, it con
-00001c60: 7461 696e 7320 3a72 6566 3a60 6164 7661  tains :ref:`adva
-00001c70: 6e63 6564 2063 6f6d 7072 6573 7369 6f6e  nced compression
-00001c80: 2070 6172 616d 6574 6572 733c 4350 6172   parameters<CPar
-00001c90: 616d 6574 6572 3e60 2e20 5468 6520 6465  ameter>`. The de
-00001ca0: 6661 756c 7420 7661 6c75 6520 6060 4e6f  fault value ``No
-00001cb0: 6e65 6060 206d 6561 6e73 2074 6f20 7573  ne`` means to us
-00001cc0: 6520 7a73 7464 2773 2064 6566 6175 6c74  e zstd's default
-00001cd0: 2063 6f6d 7072 6573 7369 6f6e 206c 6576   compression lev
-00001ce0: 656c 2f70 6172 616d 6574 6572 732e 0a20  el/parameters.. 
-00001cf0: 2020 203a 7479 7065 206c 6576 656c 5f6f     :type level_o
-00001d00: 725f 6f70 7469 6f6e 3a20 696e 7420 6f72  r_option: int or
-00001d10: 2064 6963 740a 2020 2020 3a70 6172 616d   dict.    :param
-00001d20: 207a 7374 645f 6469 6374 3a20 5072 652d   zstd_dict: Pre-
-00001d30: 7472 6169 6e65 6420 6469 6374 696f 6e61  trained dictiona
-00001d40: 7279 2066 6f72 2063 6f6d 7072 6573 7369  ry for compressi
-00001d50: 6f6e 2e0a 2020 2020 3a74 7970 6520 7a73  on..    :type zs
-00001d60: 7464 5f64 6963 743a 205a 7374 6444 6963  td_dict: ZstdDic
-00001d70: 740a 2020 2020 3a70 6172 616d 2070 6c65  t.    :param ple
-00001d80: 6467 6564 5f69 6e70 7574 5f73 697a 653a  dged_input_size:
-00001d90: 2049 6620 7365 7420 7468 6973 2070 6172   If set this par
-00001da0: 616d 6574 6572 2074 6f20 7468 6520 7369  ameter to the si
-00001db0: 7a65 206f 6620 696e 7075 7420 6461 7461  ze of input data
-00001dc0: 2c20 7468 6520 3a72 6566 3a60 7369 7a65  , the :ref:`size
-00001dd0: 3c63 6f6e 7465 6e74 5f73 697a 653e 6020  <content_size>` 
-00001de0: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
-00001df0: 696e 746f 2074 6865 2066 7261 6d65 2068  into the frame h
-00001e00: 6561 6465 722e 2049 6620 7468 6520 6163  eader. If the ac
-00001e10: 7475 616c 2069 6e70 7574 2064 6174 6120  tual input data 
-00001e20: 646f 6573 6e27 7420 6d61 7463 6820 6974  doesn't match it
-00001e30: 2c20 6120 3a70 793a 636c 6173 733a 605a  , a :py:class:`Z
-00001e40: 7374 6445 7272 6f72 6020 6578 6365 7074  stdError` except
-00001e50: 696f 6e20 7769 6c6c 2062 6520 7261 6973  ion will be rais
-00001e60: 6564 2e20 4974 206d 6179 2069 6e63 7265  ed. It may incre
-00001e70: 6173 6520 636f 6d70 7265 7373 696f 6e20  ase compression 
-00001e80: 7261 7469 6f20 736c 6967 6874 6c79 2c20  ratio slightly, 
-00001e90: 616e 6420 6865 6c70 2064 6563 6f6d 7072  and help decompr
-00001ea0: 6573 7369 6f6e 2063 6f64 6520 746f 2061  ession code to a
-00001eb0: 6c6c 6f63 6174 6520 6f75 7470 7574 2062  llocate output b
-00001ec0: 7566 6665 7220 6661 7374 6572 2e0a 2020  uffer faster..  
-00001ed0: 2020 3a74 7970 6520 706c 6564 6765 645f    :type pledged_
-00001ee0: 696e 7075 745f 7369 7a65 3a20 696e 740a  input_size: int.
-00001ef0: 2020 2020 3a70 6172 616d 2072 6561 645f      :param read_
-00001f00: 7369 7a65 3a20 496e 7075 7420 6275 6666  size: Input buff
-00001f10: 6572 2073 697a 652c 2069 6e20 6279 7465  er size, in byte
-00001f20: 732e 0a20 2020 203a 7479 7065 2072 6561  s..    :type rea
-00001f30: 645f 7369 7a65 3a20 696e 740a 2020 2020  d_size: int.    
-00001f40: 3a70 6172 616d 2077 7269 7465 5f73 697a  :param write_siz
-00001f50: 653a 204f 7574 7075 7420 6275 6666 6572  e: Output buffer
-00001f60: 2073 697a 652c 2069 6e20 6279 7465 732e   size, in bytes.
-00001f70: 0a20 2020 203a 7479 7065 2077 7269 7465  .    :type write
-00001f80: 5f73 697a 653a 2069 6e74 0a20 2020 203a  _size: int.    :
-00001f90: 7061 7261 6d20 6361 6c6c 6261 636b 3a20  param callback: 
-00001fa0: 4120 6361 6c6c 6261 636b 2066 756e 6374  A callback funct
-00001fb0: 696f 6e20 7468 6174 2061 6363 6570 7473  ion that accepts
-00001fc0: 2066 6f75 7220 7061 7261 6d65 7465 7273   four parameters
-00001fd0: 3a20 6060 2874 6f74 616c 5f69 6e70 7574  : ``(total_input
-00001fe0: 2c20 746f 7461 6c5f 6f75 7470 7574 2c20  , total_output, 
-00001ff0: 7265 6164 5f64 6174 612c 2077 7269 7465  read_data, write
-00002000: 5f64 6174 6129 6060 2e20 5468 6520 6669  _data)``. The fi
-00002010: 7273 7420 7477 6f20 6172 6520 6060 696e  rst two are ``in
-00002020: 7460 6020 6f62 6a65 6374 732e 2054 6865  t`` objects. The
-00002030: 206c 6173 7420 7477 6f20 6172 6520 7265   last two are re
-00002040: 6164 6f6e 6c79 2060 6d65 6d6f 7279 7669  adonly `memoryvi
-00002050: 6577 203c 6874 7470 733a 2f2f 646f 6373  ew <https://docs
-00002060: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-00002070: 6272 6172 792f 7374 6474 7970 6573 2e68  brary/stdtypes.h
-00002080: 746d 6c23 6d65 6d6f 7279 2d76 6965 7773  tml#memory-views
-00002090: 3e60 5f20 6f62 6a65 6374 732c 2069 6620  >`_ objects, if 
-000020a0: 7761 6e74 2074 6f20 7265 6665 7265 6e63  want to referenc
-000020b0: 6520 7468 6520 6461 7461 2028 6f72 2069  e the data (or i
-000020c0: 7473 2073 6c69 6365 2920 6f75 7473 6964  ts slice) outsid
-000020d0: 6520 7468 6520 6361 6c6c 6261 636b 2066  e the callback f
-000020e0: 756e 6374 696f 6e2c 2060 636f 6e76 6572  unction, `conver
-000020f0: 7420 3c68 7474 7073 3a2f 2f64 6f63 732e  t <https://docs.
-00002100: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
-00002110: 7261 7279 2f73 7464 7479 7065 732e 6874  rary/stdtypes.ht
-00002120: 6d6c 236d 656d 6f72 7976 6965 772e 746f  ml#memoryview.to
-00002130: 6279 7465 733e 605f 2074 6865 6d20 746f  bytes>`_ them to
-00002140: 2060 6062 7974 6573 6060 206f 626a 6563   ``bytes`` objec
-00002150: 7473 2e20 4966 2069 6e70 7574 2073 7472  ts. If input str
-00002160: 6561 6d20 6973 2060 6062 2727 6060 2c20  eam is ``b''``, 
-00002170: 7468 6520 6361 6c6c 6261 636b 2066 756e  the callback fun
-00002180: 6374 696f 6e20 7769 6c6c 206e 6f74 2062  ction will not b
-00002190: 6520 6361 6c6c 6564 2e0a 2020 2020 3a74  e called..    :t
-000021a0: 7970 6520 6361 6c6c 6261 636b 3a20 6361  ype callback: ca
-000021b0: 6c6c 6162 6c65 0a20 2020 203a 7265 7475  llable.    :retu
-000021c0: 726e 3a20 4120 322d 6974 656d 2074 7570  rn: A 2-item tup
-000021d0: 6c65 2c20 6060 2874 6f74 616c 5f69 6e70  le, ``(total_inp
-000021e0: 7574 2c20 746f 7461 6c5f 6f75 7470 7574  ut, total_output
-000021f0: 2960 602c 2074 6865 2069 7465 6d73 2061  )``, the items a
-00002200: 7265 2060 6069 6e74 6060 206f 626a 6563  re ``int`` objec
-00002210: 7473 2e0a 0a20 2020 202e 2e20 736f 7572  ts...    .. sour
-00002220: 6365 636f 6465 3a3a 2070 7974 686f 6e0a  cecode:: python.
-00002230: 0a20 2020 2020 2020 2023 2063 6f6d 7072  .        # compr
-00002240: 6573 7320 616e 2069 6e70 7574 2066 696c  ess an input fil
-00002250: 652c 2061 6e64 2077 7269 7465 2074 6f20  e, and write to 
-00002260: 616e 206f 7574 7075 7420 6669 6c65 2e0a  an output file..
-00002270: 2020 2020 2020 2020 7769 7468 2069 6f2e          with io.
-00002280: 6f70 656e 2869 6e70 7574 5f66 696c 655f  open(input_file_
-00002290: 7061 7468 2c20 2772 6227 2920 6173 2069  path, 'rb') as i
-000022a0: 6668 3a0a 2020 2020 2020 2020 2020 2020  fh:.            
-000022b0: 7769 7468 2069 6f2e 6f70 656e 286f 7574  with io.open(out
-000022c0: 7075 745f 6669 6c65 5f70 6174 682c 2027  put_file_path, '
-000022d0: 7762 2729 2061 7320 6f66 683a 0a20 2020  wb') as ofh:.   
-000022e0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-000022f0: 7072 6573 735f 7374 7265 616d 2869 6668  press_stream(ifh
-00002300: 2c20 6f66 682c 206c 6576 656c 5f6f 725f  , ofh, level_or_
-00002310: 6f70 7469 6f6e 3d35 290a 0a20 2020 2020  option=5)..     
-00002320: 2020 2023 2063 6f6d 7072 6573 7320 6120     # compress a 
-00002330: 6279 7465 7320 6f62 6a65 6374 2c20 616e  bytes object, an
-00002340: 6420 7772 6974 6520 746f 2061 2066 696c  d write to a fil
-00002350: 652e 0a20 2020 2020 2020 2077 6974 6820  e..        with 
-00002360: 696f 2e42 7974 6573 494f 2872 6177 5f64  io.BytesIO(raw_d
-00002370: 6174 2920 6173 2062 693a 0a20 2020 2020  at) as bi:.     
-00002380: 2020 2020 2020 2077 6974 6820 696f 2e6f         with io.o
-00002390: 7065 6e28 6f75 7470 7574 5f66 696c 655f  pen(output_file_
-000023a0: 7061 7468 2c20 2777 6227 2920 6173 206f  path, 'wb') as o
-000023b0: 6668 3a0a 2020 2020 2020 2020 2020 2020  fh:.            
-000023c0: 2020 2020 636f 6d70 7265 7373 5f73 7472      compress_str
-000023d0: 6561 6d28 6269 2c20 6f66 682c 2070 6c65  eam(bi, ofh, ple
-000023e0: 6467 6564 5f69 6e70 7574 5f73 697a 653d  dged_input_size=
-000023f0: 6c65 6e28 7261 775f 6461 7429 290a 0a20  len(raw_dat)).. 
-00002400: 2020 2020 2020 2023 2043 6f6d 7072 6573         # Compres
-00002410: 7320 616e 2069 6e70 7574 2066 696c 652c  s an input file,
-00002420: 206f 6274 6169 6e20 6120 6279 7465 7320   obtain a bytes 
-00002430: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-00002440: 2320 4974 2773 2066 6173 7465 7220 7468  # It's faster th
-00002450: 616e 2072 6561 6469 6e67 2061 2066 696c  an reading a fil
-00002460: 6520 616e 6420 636f 6d70 7265 7373 696e  e and compressin
-00002470: 6720 6974 2069 6e0a 2020 2020 2020 2020  g it in.        
-00002480: 2320 6d65 6d6f 7279 2c20 7465 7374 6564  # memory, tested
-00002490: 206f 6e20 5562 756e 7475 2850 7974 686f   on Ubuntu(Pytho
-000024a0: 6e33 2e38 292f 5769 6e64 6f77 7328 5079  n3.8)/Windows(Py
-000024b0: 7468 6f6e 332e 3929 2e0a 2020 2020 2020  thon3.9)..      
-000024c0: 2020 2320 4d61 7962 6520 7468 6520 4f53    # Maybe the OS
-000024d0: 2068 6173 2070 7265 6665 7463 6869 6e67   has prefetching
-000024e0: 2c20 6974 2063 616e 2072 6561 6420 616e  , it can read an
-000024f0: 6420 636f 6d70 7265 7373 0a20 2020 2020  d compress.     
-00002500: 2020 2023 2064 6174 6120 696e 2070 6172     # data in par
-00002510: 616c 6c65 6c20 746f 2073 6f6d 6520 6465  allel to some de
-00002520: 6772 6565 2c20 7265 6164 696e 6720 6669  gree, reading fi
-00002530: 6c65 2066 726f 6d20 4844 440a 2020 2020  le from HDD.    
-00002540: 2020 2020 2320 6973 2074 6865 2062 6f74      # is the bot
-00002550: 746c 656e 6563 6b20 696e 2074 6869 7320  tleneck in this 
-00002560: 6361 7365 2e0a 2020 2020 2020 2020 7769  case..        wi
-00002570: 7468 2069 6f2e 6f70 656e 2869 6e70 7574  th io.open(input
-00002580: 5f66 696c 655f 7061 7468 2c20 2772 6227  _file_path, 'rb'
-00002590: 2920 6173 2069 6668 3a0a 2020 2020 2020  ) as ifh:.      
-000025a0: 2020 2020 2020 7769 7468 2069 6f2e 4279        with io.By
-000025b0: 7465 7349 4f28 2920 6173 2062 6f3a 0a20  tesIO() as bo:. 
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000025d0: 6f6d 7072 6573 735f 7374 7265 616d 2869  ompress_stream(i
-000025e0: 6668 2c20 626f 290a 2020 2020 2020 2020  fh, bo).        
-000025f0: 2020 2020 2020 2020 636f 6d70 7265 7373          compress
-00002600: 6564 5f64 6174 203d 2062 6f2e 6765 7476  ed_dat = bo.getv
-00002610: 616c 7565 2829 0a0a 2020 2020 2020 2020  alue()..        
-00002620: 2320 5072 696e 7420 7072 6f67 7265 7373  # Print progress
-00002630: 2075 7369 6e67 2063 616c 6c62 6163 6b20   using callback 
-00002640: 6675 6e63 7469 6f6e 0a20 2020 2020 2020  function.       
-00002650: 2064 6566 2063 6f6d 7072 6573 735f 7072   def compress_pr
-00002660: 696e 745f 7072 6f67 7265 7373 2869 6e70  int_progress(inp
-00002670: 7574 5f66 696c 655f 7061 7468 2c20 6f75  ut_file_path, ou
-00002680: 7470 7574 5f66 696c 655f 7061 7468 293a  tput_file_path):
-00002690: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
-000026a0: 7574 5f66 696c 655f 7369 7a65 203d 206f  ut_file_size = o
-000026b0: 732e 7061 7468 2e67 6574 7369 7a65 2869  s.path.getsize(i
-000026c0: 6e70 7574 5f66 696c 655f 7061 7468 290a  nput_file_path).
-000026d0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-000026e0: 2066 756e 6328 746f 7461 6c5f 696e 7075   func(total_inpu
-000026f0: 742c 2074 6f74 616c 5f6f 7574 7075 742c  t, total_output,
-00002700: 2072 6561 645f 6461 7461 2c20 7772 6974   read_data, writ
-00002710: 655f 6461 7461 293a 0a20 2020 2020 2020  e_data):.       
-00002720: 2020 2020 2020 2020 2023 2049 6620 696e           # If in
-00002730: 7075 7420 7374 7265 616d 2069 7320 656d  put stream is em
-00002740: 7074 792c 2074 6865 2063 616c 6c62 6163  pty, the callbac
-00002750: 6b20 6675 6e63 7469 6f6e 0a20 2020 2020  k function.     
-00002760: 2020 2020 2020 2020 2020 2023 2077 696c             # wil
-00002770: 6c20 6e6f 7420 6265 2063 616c 6c65 642e  l not be called.
-00002780: 2053 6f20 6e6f 205a 6572 6f44 6976 6973   So no ZeroDivis
-00002790: 696f 6e45 7272 6f72 2068 6572 652e 0a20  ionError here.. 
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000027b0: 6572 6365 6e74 203d 2031 3030 202a 2074  ercent = 100 * t
-000027c0: 6f74 616c 5f69 6e70 7574 202f 2069 6e70  otal_input / inp
-000027d0: 7574 5f66 696c 655f 7369 7a65 0a20 2020  ut_file_size.   
-000027e0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000027f0: 6e74 2866 2750 726f 6772 6573 733a 207b  nt(f'Progress: {
-00002800: 7065 7263 656e 743a 2e31 667d 2527 2c20  percent:.1f}%', 
-00002810: 656e 643d 275c 7227 290a 0a20 2020 2020  end='\r')..     
-00002820: 2020 2020 2020 2077 6974 6820 696f 2e6f         with io.o
-00002830: 7065 6e28 696e 7075 745f 6669 6c65 5f70  pen(input_file_p
-00002840: 6174 682c 2027 7262 2729 2061 7320 6966  ath, 'rb') as if
-00002850: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-00002860: 2020 2077 6974 6820 696f 2e6f 7065 6e28     with io.open(
-00002870: 6f75 7470 7574 5f66 696c 655f 7061 7468  output_file_path
-00002880: 2c20 2777 6227 2920 6173 206f 6668 3a0a  , 'wb') as ofh:.
-00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028a0: 2020 2020 636f 6d70 7265 7373 5f73 7472      compress_str
-000028b0: 6561 6d28 6966 682c 206f 6668 2c20 6361  eam(ifh, ofh, ca
-000028c0: 6c6c 6261 636b 3d66 756e 6329 0a0a 0a2e  llback=func)....
-000028d0: 2e20 7079 3a63 6c61 7373 3a3a 205a 7374  . py:class:: Zst
-000028e0: 6443 6f6d 7072 6573 736f 720a 0a20 2020  dCompressor..   
-000028f0: 2041 2073 7472 6561 6d69 6e67 2063 6f6d   A streaming com
-00002900: 7072 6573 736f 722e 2049 7427 7320 7468  pressor. It's th
-00002910: 7265 6164 2d73 6166 6520 6174 206d 6574  read-safe at met
-00002920: 686f 6420 6c65 7665 6c2e 0a0a 2020 2020  hod level...    
-00002930: 2e2e 2070 793a 6d65 7468 6f64 3a3a 205f  .. py:method:: _
-00002940: 5f69 6e69 745f 5f28 7365 6c66 2c20 6c65  _init__(self, le
-00002950: 7665 6c5f 6f72 5f6f 7074 696f 6e3d 4e6f  vel_or_option=No
-00002960: 6e65 2c20 7a73 7464 5f64 6963 743d 4e6f  ne, zstd_dict=No
-00002970: 6e65 290a 0a20 2020 2020 2020 2049 6e69  ne)..        Ini
-00002980: 7469 616c 697a 6520 6120 5a73 7464 436f  tialize a ZstdCo
-00002990: 6d70 7265 7373 6f72 206f 626a 6563 742e  mpressor object.
-000029a0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000029b0: 206c 6576 656c 5f6f 725f 6f70 7469 6f6e   level_or_option
-000029c0: 3a20 5768 656e 2069 7427 7320 616e 2060  : When it's an `
-000029d0: 6069 6e74 6060 206f 626a 6563 742c 2069  `int`` object, i
-000029e0: 7420 7265 7072 6573 656e 7473 2074 6865  t represents the
-000029f0: 203a 7265 663a 6063 6f6d 7072 6573 7369   :ref:`compressi
-00002a00: 6f6e 206c 6576 656c 3c63 6f6d 7072 6573  on level<compres
-00002a10: 7369 6f6e 5f6c 6576 656c 3e60 2e20 5768  sion_level>`. Wh
-00002a20: 656e 2069 7427 7320 6120 6060 6469 6374  en it's a ``dict
-00002a30: 6060 206f 626a 6563 742c 2069 7420 636f  `` object, it co
-00002a40: 6e74 6169 6e73 203a 7265 663a 6061 6476  ntains :ref:`adv
-00002a50: 616e 6365 6420 636f 6d70 7265 7373 696f  anced compressio
-00002a60: 6e20 7061 7261 6d65 7465 7273 3c43 5061  n parameters<CPa
-00002a70: 7261 6d65 7465 723e 602e 2054 6865 2064  rameter>`. The d
-00002a80: 6566 6175 6c74 2076 616c 7565 2060 604e  efault value ``N
-00002a90: 6f6e 6560 6020 6d65 616e 7320 746f 2075  one`` means to u
-00002aa0: 7365 207a 7374 6427 7320 6465 6661 756c  se zstd's defaul
-00002ab0: 7420 636f 6d70 7265 7373 696f 6e20 6c65  t compression le
-00002ac0: 7665 6c2f 7061 7261 6d65 7465 7273 2e0a  vel/parameters..
-00002ad0: 2020 2020 2020 2020 3a74 7970 6520 6c65          :type le
-00002ae0: 7665 6c5f 6f72 5f6f 7074 696f 6e3a 2069  vel_or_option: i
-00002af0: 6e74 206f 7220 6469 6374 0a20 2020 2020  nt or dict.     
-00002b00: 2020 203a 7061 7261 6d20 7a73 7464 5f64     :param zstd_d
-00002b10: 6963 743a 2050 7265 2d74 7261 696e 6564  ict: Pre-trained
-00002b20: 2064 6963 7469 6f6e 6172 7920 666f 7220   dictionary for 
-00002b30: 636f 6d70 7265 7373 696f 6e2e 0a20 2020  compression..   
-00002b40: 2020 2020 203a 7479 7065 207a 7374 645f       :type zstd_
-00002b50: 6469 6374 3a20 5a73 7464 4469 6374 0a0a  dict: ZstdDict..
-00002b60: 2020 2020 2e2e 2070 793a 6d65 7468 6f64      .. py:method
-00002b70: 3a3a 2063 6f6d 7072 6573 7328 7365 6c66  :: compress(self
-00002b80: 2c20 6461 7461 2c20 6d6f 6465 3d5a 7374  , data, mode=Zst
-00002b90: 6443 6f6d 7072 6573 736f 722e 434f 4e54  dCompressor.CONT
-00002ba0: 494e 5545 290a 0a20 2020 2020 2020 2050  INUE)..        P
-00002bb0: 726f 7669 6465 2064 6174 6120 746f 2074  rovide data to t
-00002bc0: 6865 2063 6f6d 7072 6573 736f 7220 6f62  he compressor ob
-00002bd0: 6a65 6374 2e0a 0a20 2020 2020 2020 203a  ject...        :
-00002be0: 7061 7261 6d20 6461 7461 3a20 4461 7461  param data: Data
-00002bf0: 2074 6f20 6265 2063 6f6d 7072 6573 7365   to be compresse
-00002c00: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
-00002c10: 2064 6174 613a 2062 7974 6573 2d6c 696b   data: bytes-lik
-00002c20: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
-00002c30: 203a 7061 7261 6d20 6d6f 6465 3a20 4361   :param mode: Ca
-00002c40: 6e20 6265 2074 6865 7365 2033 2076 616c  n be these 3 val
-00002c50: 7565 733a 203a 7079 3a61 7474 723a 605a  ues: :py:attr:`Z
-00002c60: 7374 6443 6f6d 7072 6573 736f 722e 434f  stdCompressor.CO
-00002c70: 4e54 494e 5545 602c 203a 7079 3a61 7474  NTINUE`, :py:att
-00002c80: 723a 605a 7374 6443 6f6d 7072 6573 736f  r:`ZstdCompresso
-00002c90: 722e 464c 5553 485f 424c 4f43 4b60 2c20  r.FLUSH_BLOCK`, 
-00002ca0: 3a70 793a 6174 7472 3a60 5a73 7464 436f  :py:attr:`ZstdCo
-00002cb0: 6d70 7265 7373 6f72 2e46 4c55 5348 5f46  mpressor.FLUSH_F
-00002cc0: 5241 4d45 602e 0a20 2020 2020 2020 203a  RAME`..        :
-00002cd0: 7265 7475 726e 3a20 4120 6368 756e 6b20  return: A chunk 
-00002ce0: 6f66 2063 6f6d 7072 6573 7365 6420 6461  of compressed da
-00002cf0: 7461 2069 6620 706f 7373 6962 6c65 2c20  ta if possible, 
-00002d00: 6f72 2060 6062 2727 6060 206f 7468 6572  or ``b''`` other
-00002d10: 7769 7365 2e0a 2020 2020 2020 2020 3a72  wise..        :r
-00002d20: 7479 7065 3a20 6279 7465 730a 0a20 2020  type: bytes..   
-00002d30: 202e 2e20 7079 3a6d 6574 686f 643a 3a20   .. py:method:: 
-00002d40: 666c 7573 6828 7365 6c66 2c20 6d6f 6465  flush(self, mode
-00002d50: 3d5a 7374 6443 6f6d 7072 6573 736f 722e  =ZstdCompressor.
-00002d60: 464c 5553 485f 4652 414d 4529 0a0a 2020  FLUSH_FRAME)..  
-00002d70: 2020 2020 2020 466c 7573 6820 616e 7920        Flush any 
-00002d80: 7265 6d61 696e 696e 6720 6461 7461 2069  remaining data i
-00002d90: 6e20 696e 7465 726e 616c 2062 7566 6665  n internal buffe
-00002da0: 722e 0a0a 2020 2020 2020 2020 5369 6e63  r...        Sinc
-00002db0: 6520 7a73 7464 2064 6174 6120 636f 6e73  e zstd data cons
-00002dc0: 6973 7473 206f 6620 6f6e 6520 6f72 206d  ists of one or m
-00002dd0: 6f72 6520 696e 6465 7065 6e64 656e 7420  ore independent 
-00002de0: 6672 616d 6573 2c20 7468 6520 636f 6d70  frames, the comp
-00002df0: 7265 7373 6f72 206f 626a 6563 7420 6361  ressor object ca
-00002e00: 6e20 7374 696c 6c20 6265 2075 7365 6420  n still be used 
-00002e10: 6166 7465 7220 7468 6973 206d 6574 686f  after this metho
-00002e20: 6420 6973 2063 616c 6c65 642e 0a0a 2020  d is called...  
-00002e30: 2020 2020 2020 2a2a 4e6f 7465 2a2a 3a20        **Note**: 
-00002e40: 4162 7573 6520 6f66 2074 6869 7320 6d65  Abuse of this me
-00002e50: 7468 6f64 2077 696c 6c20 7265 6475 6365  thod will reduce
-00002e60: 2063 6f6d 7072 6573 7369 6f6e 2072 6174   compression rat
-00002e70: 696f 2c20 616e 6420 736f 6d65 2070 726f  io, and some pro
-00002e80: 6772 616d 7320 6361 6e20 6f6e 6c79 2064  grams can only d
-00002e90: 6563 6f6d 7072 6573 7320 7369 6e67 6c65  ecompress single
-00002ea0: 2066 7261 6d65 2064 6174 612e 2055 7365   frame data. Use
-00002eb0: 2069 7420 6f6e 6c79 2077 6865 6e20 6e65   it only when ne
-00002ec0: 6365 7373 6172 792e 0a0a 2020 2020 2020  cessary...      
-00002ed0: 2020 3a70 6172 616d 206d 6f64 653a 2043    :param mode: C
-00002ee0: 616e 2062 6520 7468 6573 6520 3220 7661  an be these 2 va
-00002ef0: 6c75 6573 3a20 3a70 793a 6174 7472 3a60  lues: :py:attr:`
-00002f00: 5a73 7464 436f 6d70 7265 7373 6f72 2e46  ZstdCompressor.F
-00002f10: 4c55 5348 5f46 5241 4d45 602c 203a 7079  LUSH_FRAME`, :py
-00002f20: 3a61 7474 723a 605a 7374 6443 6f6d 7072  :attr:`ZstdCompr
-00002f30: 6573 736f 722e 464c 5553 485f 424c 4f43  essor.FLUSH_BLOC
-00002f40: 4b60 2e0a 2020 2020 2020 2020 3a72 6574  K`..        :ret
-00002f50: 7572 6e3a 2046 6c75 7368 6564 2064 6174  urn: Flushed dat
-00002f60: 612e 0a20 2020 2020 2020 203a 7274 7970  a..        :rtyp
-00002f70: 653a 2062 7974 6573 0a0a 2020 2020 2e2e  e: bytes..    ..
-00002f80: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
-00002f90: 6c61 7374 5f6d 6f64 650a 0a20 2020 2020  last_mode..     
-00002fa0: 2020 2054 6865 206c 6173 7420 6d6f 6465     The last mode
-00002fb0: 2075 7365 6420 746f 2074 6869 7320 636f   used to this co
-00002fc0: 6d70 7265 7373 6f72 2c20 6974 7320 7661  mpressor, its va
-00002fd0: 6c75 6520 6361 6e20 6265 203a 7079 3a61  lue can be :py:a
-00002fe0: 7474 723a 607e 5a73 7464 436f 6d70 7265  ttr:`~ZstdCompre
-00002ff0: 7373 6f72 2e43 4f4e 5449 4e55 4560 2c20  ssor.CONTINUE`, 
-00003000: 3a70 793a 6174 7472 3a60 7e5a 7374 6443  :py:attr:`~ZstdC
-00003010: 6f6d 7072 6573 736f 722e 464c 5553 485f  ompressor.FLUSH_
-00003020: 424c 4f43 4b60 2c20 3a70 793a 6174 7472  BLOCK`, :py:attr
-00003030: 3a60 7e5a 7374 6443 6f6d 7072 6573 736f  :`~ZstdCompresso
-00003040: 722e 464c 5553 485f 4652 414d 4560 2e20  r.FLUSH_FRAME`. 
-00003050: 496e 6974 6961 6c69 7a65 6420 746f 203a  Initialized to :
-00003060: 7079 3a61 7474 723a 607e 5a73 7464 436f  py:attr:`~ZstdCo
-00003070: 6d70 7265 7373 6f72 2e46 4c55 5348 5f46  mpressor.FLUSH_F
-00003080: 5241 4d45 602e 0a0a 2020 2020 2020 2020  RAME`...        
-00003090: 4974 2063 616e 2062 6520 7573 6564 2074  It can be used t
-000030a0: 6f20 6765 7420 7468 6520 6375 7272 656e  o get the curren
-000030b0: 7420 7374 6174 6520 6f66 2061 2063 6f6d  t state of a com
-000030c0: 7072 6573 736f 722c 2073 7563 6820 6173  pressor, such as
-000030d0: 2c20 6461 7461 2066 6c75 7368 6564 2c20  , data flushed, 
-000030e0: 6120 6672 616d 6520 656e 6465 642e 0a0a  a frame ended...
-000030f0: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
-00003100: 7574 653a 3a20 434f 4e54 494e 5545 0a0a  ute:: CONTINUE..
-00003110: 2020 2020 2020 2020 5573 6564 2066 6f72          Used for
-00003120: 202a 6d6f 6465 2a20 7061 7261 6d65 7465   *mode* paramete
-00003130: 7220 696e 203a 7079 3a6d 6574 683a 607e  r in :py:meth:`~
-00003140: 5a73 7464 436f 6d70 7265 7373 6f72 2e63  ZstdCompressor.c
-00003150: 6f6d 7072 6573 7360 206d 6574 686f 642e  ompress` method.
-00003160: 0a0a 2020 2020 2020 2020 436f 6c6c 6563  ..        Collec
-00003170: 7420 6d6f 7265 2064 6174 612c 2065 6e63  t more data, enc
-00003180: 6f64 6572 2064 6563 6964 6573 2077 6865  oder decides whe
-00003190: 6e20 746f 206f 7574 7075 7420 636f 6d70  n to output comp
-000031a0: 7265 7373 6564 2072 6573 756c 742c 2066  ressed result, f
-000031b0: 6f72 206f 7074 696d 616c 2063 6f6d 7072  or optimal compr
-000031c0: 6573 7369 6f6e 2072 6174 696f 2e20 5573  ession ratio. Us
-000031d0: 7561 6c6c 7920 7573 6564 2066 6f72 2074  ually used for t
-000031e0: 7261 6469 7469 6f6e 616c 2073 7472 6561  raditional strea
-000031f0: 6d69 6e67 2063 6f6d 7072 6573 7369 6f6e  ming compression
-00003200: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
-00003210: 7269 6275 7465 3a3a 2046 4c55 5348 5f42  ribute:: FLUSH_B
-00003220: 4c4f 434b 0a0a 2020 2020 2020 2020 5573  LOCK..        Us
-00003230: 6564 2066 6f72 202a 6d6f 6465 2a20 7061  ed for *mode* pa
-00003240: 7261 6d65 7465 7220 696e 203a 7079 3a6d  rameter in :py:m
-00003250: 6574 683a 607e 5a73 7464 436f 6d70 7265  eth:`~ZstdCompre
-00003260: 7373 6f72 2e63 6f6d 7072 6573 7360 2c20  ssor.compress`, 
-00003270: 3a70 793a 6d65 7468 3a60 7e5a 7374 6443  :py:meth:`~ZstdC
-00003280: 6f6d 7072 6573 736f 722e 666c 7573 6860  ompressor.flush`
-00003290: 206d 6574 686f 6473 2e0a 0a20 2020 2020   methods...     
-000032a0: 2020 2046 6c75 7368 2061 6e79 2072 656d     Flush any rem
-000032b0: 6169 6e69 6e67 2064 6174 612c 2062 7574  aining data, but
-000032c0: 2064 6f6e 2774 2063 6c6f 7365 2074 6865   don't close the
-000032d0: 2063 7572 7265 6e74 203a 7265 663a 6066   current :ref:`f
-000032e0: 7261 6d65 3c66 7261 6d65 5f62 6c6f 636b  rame<frame_block
-000032f0: 3e60 2e20 5573 7561 6c6c 7920 7573 6564  >`. Usually used
-00003300: 2066 6f72 2063 6f6d 6d75 6e69 6361 7469   for communicati
-00003310: 6f6e 2073 6365 6e61 7269 6f73 2e0a 0a20  on scenarios... 
-00003320: 2020 2020 2020 2049 6620 7468 6572 6520         If there 
-00003330: 6973 2064 6174 612c 2069 7420 6372 6561  is data, it crea
-00003340: 7465 7320 6174 206c 6561 7374 206f 6e65  tes at least one
-00003350: 206e 6577 203a 7265 663a 6062 6c6f 636b   new :ref:`block
-00003360: 3c66 7261 6d65 5f62 6c6f 636b 3e60 2c20  <frame_block>`, 
-00003370: 7468 6174 2063 616e 2062 6520 6465 636f  that can be deco
-00003380: 6465 6420 696d 6d65 6469 6174 656c 7920  ded immediately 
-00003390: 6f6e 2072 6563 6570 7469 6f6e 2e20 4966  on reception. If
-000033a0: 206e 6f20 7265 6d61 696e 696e 6720 6461   no remaining da
-000033b0: 7461 2c20 6e6f 2062 6c6f 636b 2069 7320  ta, no block is 
-000033c0: 6372 6561 7465 642c 2072 6574 7572 6e20  created, return 
-000033d0: 6060 6227 2760 602e 0a0a 2020 2020 2020  ``b''``...      
-000033e0: 2020 2a2a 4e6f 7465 2a2a 3a20 4162 7573    **Note**: Abus
-000033f0: 6520 6f66 2074 6869 7320 6d6f 6465 2077  e of this mode w
-00003400: 696c 6c20 7265 6475 6365 2063 6f6d 7072  ill reduce compr
-00003410: 6573 7369 6f6e 2072 6174 696f 2e20 5573  ession ratio. Us
-00003420: 6520 6974 206f 6e6c 7920 7768 656e 206e  e it only when n
-00003430: 6563 6573 7361 7279 2e0a 0a20 2020 202e  ecessary...    .
-00003440: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
-00003450: 2046 4c55 5348 5f46 5241 4d45 0a0a 2020   FLUSH_FRAME..  
-00003460: 2020 2020 2020 5573 6564 2066 6f72 202a        Used for *
-00003470: 6d6f 6465 2a20 7061 7261 6d65 7465 7220  mode* parameter 
-00003480: 696e 203a 7079 3a6d 6574 683a 607e 5a73  in :py:meth:`~Zs
-00003490: 7464 436f 6d70 7265 7373 6f72 2e63 6f6d  tdCompressor.com
-000034a0: 7072 6573 7360 2c20 3a70 793a 6d65 7468  press`, :py:meth
-000034b0: 3a60 7e5a 7374 6443 6f6d 7072 6573 736f  :`~ZstdCompresso
-000034c0: 722e 666c 7573 6860 206d 6574 686f 6473  r.flush` methods
-000034d0: 2e0a 0a20 2020 2020 2020 2046 6c75 7368  ...        Flush
-000034e0: 2061 6e79 2072 656d 6169 6e69 6e67 2064   any remaining d
-000034f0: 6174 612c 2061 6e64 2063 6c6f 7365 2074  ata, and close t
-00003500: 6865 2063 7572 7265 6e74 203a 7265 663a  he current :ref:
-00003510: 6066 7261 6d65 3c66 7261 6d65 5f62 6c6f  `frame<frame_blo
-00003520: 636b 3e60 2e20 5573 7561 6c6c 7920 7573  ck>`. Usually us
-00003530: 6564 2066 6f72 2074 7261 6469 7469 6f6e  ed for tradition
-00003540: 616c 2066 6c75 7368 2e0a 0a20 2020 2020  al flush...     
-00003550: 2020 2053 696e 6365 207a 7374 6420 6461     Since zstd da
-00003560: 7461 2063 6f6e 7369 7374 7320 6f66 206f  ta consists of o
-00003570: 6e65 206f 7220 6d6f 7265 2069 6e64 6570  ne or more indep
-00003580: 656e 6465 6e74 2066 7261 6d65 732c 2064  endent frames, d
-00003590: 6174 6120 6361 6e20 7374 696c 6c20 6265  ata can still be
-000035a0: 2070 726f 7669 6465 6420 6166 7465 7220   provided after 
-000035b0: 6120 6672 616d 6520 6973 2063 6c6f 7365  a frame is close
-000035c0: 642e 0a0a 2020 2020 2020 2020 2a2a 4e6f  d...        **No
-000035d0: 7465 2a2a 3a20 4162 7573 6520 6f66 2074  te**: Abuse of t
-000035e0: 6869 7320 6d6f 6465 2077 696c 6c20 7265  his mode will re
-000035f0: 6475 6365 2063 6f6d 7072 6573 7369 6f6e  duce compression
-00003600: 2072 6174 696f 2c20 616e 6420 736f 6d65   ratio, and some
-00003610: 2070 726f 6772 616d 7320 6361 6e20 6f6e   programs can on
-00003620: 6c79 2064 6563 6f6d 7072 6573 7320 7369  ly decompress si
-00003630: 6e67 6c65 2066 7261 6d65 2064 6174 612e  ngle frame data.
-00003640: 2055 7365 2069 7420 6f6e 6c79 2077 6865   Use it only whe
-00003650: 6e20 6e65 6365 7373 6172 792e 0a0a 2020  n necessary...  
-00003660: 2020 2e2e 2073 6f75 7263 6563 6f64 653a    .. sourcecode:
-00003670: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-00003680: 2020 6320 3d20 5a73 7464 436f 6d70 7265    c = ZstdCompre
-00003690: 7373 6f72 2829 0a0a 2020 2020 2020 2020  ssor()..        
-000036a0: 2320 7472 6164 6974 696f 6e61 6c20 7374  # traditional st
-000036b0: 7265 616d 696e 6720 636f 6d70 7265 7373  reaming compress
-000036c0: 696f 6e0a 2020 2020 2020 2020 6461 7431  ion.        dat1
-000036d0: 203d 2063 2e63 6f6d 7072 6573 7328 6227   = c.compress(b'
-000036e0: 3132 3334 3536 2729 0a20 2020 2020 2020  123456').       
-000036f0: 2064 6174 3220 3d20 632e 636f 6d70 7265   dat2 = c.compre
-00003700: 7373 2862 2761 6263 6465 6627 290a 2020  ss(b'abcdef').  
-00003710: 2020 2020 2020 6461 7433 203d 2063 2e66        dat3 = c.f
-00003720: 6c75 7368 2829 0a0a 2020 2020 2020 2020  lush()..        
-00003730: 2320 7573 6520 2e63 6f6d 7072 6573 7328  # use .compress(
-00003740: 2920 6d65 7468 6f64 2077 6974 6820 6d6f  ) method with mo
-00003750: 6465 2061 7267 756d 656e 740a 2020 2020  de argument.    
-00003760: 2020 2020 636f 6d70 7265 7373 6564 5f64      compressed_d
-00003770: 6174 3120 3d20 632e 636f 6d70 7265 7373  at1 = c.compress
-00003780: 2872 6177 5f64 6174 312c 2063 2e46 4c55  (raw_dat1, c.FLU
-00003790: 5348 5f42 4c4f 434b 290a 2020 2020 2020  SH_BLOCK).      
-000037a0: 2020 636f 6d70 7265 7373 6564 5f64 6174    compressed_dat
-000037b0: 3220 3d20 632e 636f 6d70 7265 7373 2872  2 = c.compress(r
-000037c0: 6177 5f64 6174 322c 2063 2e46 4c55 5348  aw_dat2, c.FLUSH
-000037d0: 5f46 5241 4d45 290a 0a20 2020 202e 2e20  _FRAME)..    .. 
-000037e0: 6869 6e74 3a3a 2057 6879 203a 7079 3a6d  hint:: Why :py:m
-000037f0: 6574 683a 605a 7374 6443 6f6d 7072 6573  eth:`ZstdCompres
-00003800: 736f 722e 636f 6d70 7265 7373 6020 6d65  sor.compress` me
-00003810: 7468 6f64 2068 6173 2061 202a 6d6f 6465  thod has a *mode
-00003820: 2a20 7061 7261 6d65 7465 723f 0a0a 2020  * parameter?..  
-00003830: 2020 2020 2020 232e 2057 6865 6e20 7265        #. When re
-00003840: 7573 6520 3a70 793a 636c 6173 733a 605a  use :py:class:`Z
-00003850: 7374 6443 6f6d 7072 6573 736f 7260 206f  stdCompressor` o
-00003860: 626a 6563 7420 666f 7220 6269 6720 6e75  bject for big nu
-00003870: 6d62 6572 206f 6620 7361 6d65 2074 7970  mber of same typ
-00003880: 6520 696e 6469 7669 6475 616c 2064 6174  e individual dat
-00003890: 612c 206d 616b 6520 6f70 6572 6174 696f  a, make operatio
-000038a0: 6e20 6d6f 7265 2063 6f6e 7665 6e69 656e  n more convenien
-000038b0: 742e 2054 6865 206f 626a 6563 7420 6973  t. The object is
-000038c0: 2074 6872 6561 642d 7361 6665 2061 7420   thread-safe at 
-000038d0: 6d65 7468 6f64 206c 6576 656c 2e0a 2020  method level..  
-000038e0: 2020 2020 2020 232e 2049 6620 6461 7461        #. If data
-000038f0: 2069 7320 6765 6e65 7261 7465 6420 6279   is generated by
-00003900: 2061 2073 696e 676c 6520 3a70 793a 6174   a single :py:at
-00003910: 7472 3a60 7e5a 7374 6443 6f6d 7072 6573  tr:`~ZstdCompres
-00003920: 736f 722e 464c 5553 485f 4652 414d 4560  sor.FLUSH_FRAME`
-00003930: 206d 6f64 652c 2074 6865 2073 697a 6520   mode, the size 
-00003940: 6f66 2075 6e63 6f6d 7072 6573 7365 6420  of uncompressed 
-00003950: 6461 7461 2077 696c 6c20 6265 2072 6563  data will be rec
-00003960: 6f72 6465 6420 696e 2066 7261 6d65 2068  orded in frame h
-00003970: 6561 6465 722e 0a0a 0a53 7472 6561 6d69  eader....Streami
-00003980: 6e67 2064 6563 6f6d 7072 6573 7369 6f6e  ng decompression
-00003990: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-000039a0: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020 5468  --------..    Th
-000039b0: 6973 2073 6563 7469 6f6e 2063 6f6e 7461  is section conta
-000039c0: 696e 733a 0a0a 2020 2020 2020 2020 2a20  ins:..        * 
-000039d0: 6675 6e63 7469 6f6e 203a 7079 3a66 756e  function :py:fun
-000039e0: 633a 6064 6563 6f6d 7072 6573 735f 7374  c:`decompress_st
-000039f0: 7265 616d 602c 2061 2066 6173 7420 616e  ream`, a fast an
-00003a00: 6420 636f 6e76 656e 6965 6e74 2066 756e  d convenient fun
-00003a10: 6374 696f 6e2e 0a20 2020 2020 2020 202a  ction..        *
-00003a20: 2063 6c61 7373 203a 7079 3a63 6c61 7373   class :py:class
-00003a30: 3a60 5a73 7464 4465 636f 6d70 7265 7373  :`ZstdDecompress
-00003a40: 6f72 602c 2073 696d 696c 6172 2074 6f20  or`, similar to 
-00003a50: 6465 636f 6d70 7265 7373 6f72 7320 696e  decompressors in
-00003a60: 2050 7974 686f 6e20 7374 616e 6461 7264   Python standard
-00003a70: 206c 6962 7261 7279 2e0a 2020 2020 2020   library..      
-00003a80: 2020 2a20 636c 6173 7320 3a70 793a 636c    * class :py:cl
-00003a90: 6173 733a 6045 6e64 6c65 7373 5a73 7464  ass:`EndlessZstd
-00003aa0: 4465 636f 6d70 7265 7373 6f72 602c 2061  Decompressor`, a
-00003ab0: 2064 6563 6f6d 7072 6573 736f 7220 6163   decompressor ac
-00003ac0: 6365 7074 7320 6d75 6c74 6970 6c65 2063  cepts multiple c
-00003ad0: 6f6e 6361 7465 6e61 7465 6420 3a72 6566  oncatenated :ref
-00003ae0: 3a60 6672 616d 6573 3c66 7261 6d65 5f62  :`frames<frame_b
-00003af0: 6c6f 636b 3e60 2e0a 0a2e 2e20 7079 3a66  lock>`..... py:f
-00003b00: 756e 6374 696f 6e3a 3a20 6465 636f 6d70  unction:: decomp
-00003b10: 7265 7373 5f73 7472 6561 6d28 696e 7075  ress_stream(inpu
-00003b20: 745f 7374 7265 616d 2c20 6f75 7470 7574  t_stream, output
-00003b30: 5f73 7472 6561 6d2c 202a 2c20 7a73 7464  _stream, *, zstd
-00003b40: 5f64 6963 743d 4e6f 6e65 2c20 6f70 7469  _dict=None, opti
-00003b50: 6f6e 3d4e 6f6e 652c 2072 6561 645f 7369  on=None, read_si
-00003b60: 7a65 3d31 3331 5f30 3735 2c20 7772 6974  ze=131_075, writ
-00003b70: 655f 7369 7a65 3d31 3331 5f30 3732 2c20  e_size=131_072, 
-00003b80: 6361 6c6c 6261 636b 3d4e 6f6e 6529 0a0a  callback=None)..
-00003b90: 2020 2020 4120 6661 7374 2061 6e64 2063      A fast and c
-00003ba0: 6f6e 7665 6e69 656e 7420 6675 6e63 7469  onvenient functi
-00003bb0: 6f6e 2c20 6465 636f 6d70 7265 7373 6573  on, decompresses
-00003bc0: 202a 696e 7075 745f 7374 7265 616d 2a20   *input_stream* 
-00003bd0: 616e 6420 7772 6974 6573 2074 6865 2064  and writes the d
-00003be0: 6563 6f6d 7072 6573 7365 6420 6461 7461  ecompressed data
-00003bf0: 2074 6f20 2a6f 7574 7075 745f 7374 7265   to *output_stre
-00003c00: 616d 2a2c 2069 7420 646f 6573 6e27 7420  am*, it doesn't 
-00003c10: 636c 6f73 6520 7468 6520 7374 7265 616d  close the stream
-00003c20: 732e 0a0a 2020 2020 5375 7070 6f72 7473  s...    Supports
-00003c30: 206d 756c 7469 706c 6520 636f 6e63 6174   multiple concat
-00003c40: 656e 6174 6564 203a 7265 663a 6066 7261  enated :ref:`fra
-00003c50: 6d65 733c 6672 616d 655f 626c 6f63 6b3e  mes<frame_block>
-00003c60: 602e 0a0a 2020 2020 5468 6973 2066 756e  `...    This fun
-00003c70: 6374 696f 6e20 7472 6965 7320 746f 207a  ction tries to z
-00003c80: 6572 6f2d 636f 7079 2061 7320 6d75 6368  ero-copy as much
-00003c90: 2061 7320 706f 7373 6962 6c65 2e20 4966   as possible. If
-00003ca0: 2074 6865 204f 5320 6861 7320 7265 6164   the OS has read
-00003cb0: 2070 7265 6665 7463 6869 6e67 2061 6e64   prefetching and
-00003cc0: 2077 7269 7465 2062 7566 6665 722c 2069   write buffer, i
-00003cd0: 7420 6d61 7920 7065 7266 6f72 6d20 7468  t may perform th
-00003ce0: 6520 7461 736b 7320 2872 6561 642f 6465  e tasks (read/de
-00003cf0: 636f 6d70 7265 7373 2f77 7269 7465 2920  compress/write) 
-00003d00: 696e 2070 6172 616c 6c65 6c20 746f 2073  in parallel to s
-00003d10: 6f6d 6520 6465 6772 6565 2e0a 0a20 2020  ome degree...   
-00003d20: 2054 6865 2064 6566 6175 6c74 2076 616c   The default val
-00003d30: 7565 7320 6f66 202a 7265 6164 5f73 697a  ues of *read_siz
-00003d40: 652a 2061 6e64 202a 7772 6974 655f 7369  e* and *write_si
-00003d50: 7a65 2a20 7061 7261 6d65 7465 7273 2061  ze* parameters a
-00003d60: 7265 2074 6865 2062 7566 6665 7220 7369  re the buffer si
-00003d70: 7a65 7320 7265 636f 6d6d 656e 6465 6420  zes recommended 
-00003d80: 6279 207a 7374 642c 2069 6e63 7265 6173  by zstd, increas
-00003d90: 696e 6720 7468 656d 206d 6179 2062 6520  ing them may be 
-00003da0: 6661 7374 6572 2c20 616e 6420 7265 6475  faster, and redu
-00003db0: 6365 7320 7468 6520 6e75 6d62 6572 206f  ces the number o
-00003dc0: 6620 6361 6c6c 6261 636b 2066 756e 6374  f callback funct
-00003dd0: 696f 6e20 6361 6c6c 732e 0a0a 2020 2020  ion calls...    
-00003de0: 2e2e 2076 6572 7369 6f6e 6164 6465 643a  .. versionadded:
-00003df0: 3a20 302e 3134 2e32 0a0a 2020 2020 3a70  : 0.14.2..    :p
-00003e00: 6172 616d 2069 6e70 7574 5f73 7472 6561  aram input_strea
-00003e10: 6d3a 2049 6e70 7574 2073 7472 6561 6d20  m: Input stream 
-00003e20: 7468 6174 2068 6173 2061 2060 2e72 6561  that has a `.rea
-00003e30: 6469 6e74 6f28 6229 203c 6874 7470 733a  dinto(b) <https:
-00003e40: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00003e50: 672f 332f 6c69 6272 6172 792f 696f 2e68  g/3/library/io.h
-00003e60: 746d 6c23 696f 2e52 6177 494f 4261 7365  tml#io.RawIOBase
-00003e70: 2e72 6561 6469 6e74 6f3e 605f 206d 6574  .readinto>`_ met
-00003e80: 686f 642e 0a20 2020 203a 7061 7261 6d20  hod..    :param 
-00003e90: 6f75 7470 7574 5f73 7472 6561 6d3a 204f  output_stream: O
-00003ea0: 7574 7075 7420 7374 7265 616d 2074 6861  utput stream tha
-00003eb0: 7420 6861 7320 6120 602e 7772 6974 6528  t has a `.write(
-00003ec0: 6229 203c 6874 7470 733a 2f2f 646f 6373  b) <https://docs
-00003ed0: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-00003ee0: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
-00003ef0: 2e52 6177 494f 4261 7365 2e77 7269 7465  .RawIOBase.write
-00003f00: 3e60 5f20 6d65 7468 6f64 2e20 4966 2075  >`_ method. If u
-00003f10: 7365 202a 6361 6c6c 6261 636b 2a20 6675  se *callback* fu
-00003f20: 6e63 7469 6f6e 2c20 7468 6973 2070 6172  nction, this par
-00003f30: 616d 6574 6572 2063 616e 2062 6520 6060  ameter can be ``
-00003f40: 4e6f 6e65 6060 2e0a 2020 2020 3a70 6172  None``..    :par
-00003f50: 616d 207a 7374 645f 6469 6374 3a20 5072  am zstd_dict: Pr
-00003f60: 652d 7472 6169 6e65 6420 6469 6374 696f  e-trained dictio
-00003f70: 6e61 7279 2066 6f72 2064 6563 6f6d 7072  nary for decompr
-00003f80: 6573 7369 6f6e 2e0a 2020 2020 3a74 7970  ession..    :typ
-00003f90: 6520 7a73 7464 5f64 6963 743a 205a 7374  e zstd_dict: Zst
-00003fa0: 6444 6963 740a 2020 2020 3a70 6172 616d  dDict.    :param
-00003fb0: 206f 7074 696f 6e3a 2041 2060 6064 6963   option: A ``dic
-00003fc0: 7460 6020 6f62 6a65 6374 2c20 636f 6e74  t`` object, cont
-00003fd0: 6169 6e73 203a 7265 663a 6061 6476 616e  ains :ref:`advan
-00003fe0: 6365 6420 6465 636f 6d70 7265 7373 696f  ced decompressio
-00003ff0: 6e20 7061 7261 6d65 7465 7273 3c44 5061  n parameters<DPa
-00004000: 7261 6d65 7465 723e 602e 0a20 2020 203a  rameter>`..    :
-00004010: 7479 7065 206f 7074 696f 6e3a 2064 6963  type option: dic
-00004020: 740a 2020 2020 3a70 6172 616d 2072 6561  t.    :param rea
-00004030: 645f 7369 7a65 3a20 496e 7075 7420 6275  d_size: Input bu
-00004040: 6666 6572 2073 697a 652c 2069 6e20 6279  ffer size, in by
-00004050: 7465 732e 0a20 2020 203a 7479 7065 2072  tes..    :type r
-00004060: 6561 645f 7369 7a65 3a20 696e 740a 2020  ead_size: int.  
-00004070: 2020 3a70 6172 616d 2077 7269 7465 5f73    :param write_s
-00004080: 697a 653a 204f 7574 7075 7420 6275 6666  ize: Output buff
-00004090: 6572 2073 697a 652c 2069 6e20 6279 7465  er size, in byte
-000040a0: 732e 0a20 2020 203a 7479 7065 2077 7269  s..    :type wri
-000040b0: 7465 5f73 697a 653a 2069 6e74 0a20 2020  te_size: int.   
-000040c0: 203a 7061 7261 6d20 6361 6c6c 6261 636b   :param callback
-000040d0: 3a20 4120 6361 6c6c 6261 636b 2066 756e  : A callback fun
-000040e0: 6374 696f 6e20 7468 6174 2061 6363 6570  ction that accep
-000040f0: 7473 2066 6f75 7220 7061 7261 6d65 7465  ts four paramete
-00004100: 7273 3a20 6060 2874 6f74 616c 5f69 6e70  rs: ``(total_inp
-00004110: 7574 2c20 746f 7461 6c5f 6f75 7470 7574  ut, total_output
-00004120: 2c20 7265 6164 5f64 6174 612c 2077 7269  , read_data, wri
-00004130: 7465 5f64 6174 6129 6060 2e20 5468 6520  te_data)``. The 
-00004140: 6669 7273 7420 7477 6f20 6172 6520 6060  first two are ``
-00004150: 696e 7460 6020 6f62 6a65 6374 732e 2054  int`` objects. T
-00004160: 6865 206c 6173 7420 7477 6f20 6172 6520  he last two are 
-00004170: 7265 6164 6f6e 6c79 2060 6d65 6d6f 7279  readonly `memory
-00004180: 7669 6577 203c 6874 7470 733a 2f2f 646f  view <https://do
-00004190: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-000041a0: 6c69 6272 6172 792f 7374 6474 7970 6573  library/stdtypes
-000041b0: 2e68 746d 6c23 6d65 6d6f 7279 2d76 6965  .html#memory-vie
-000041c0: 7773 3e60 5f20 6f62 6a65 6374 732c 2069  ws>`_ objects, i
-000041d0: 6620 7761 6e74 2074 6f20 7265 6665 7265  f want to refere
-000041e0: 6e63 6520 7468 6520 6461 7461 2028 6f72  nce the data (or
-000041f0: 2069 7473 2073 6c69 6365 2920 6f75 7473   its slice) outs
-00004200: 6964 6520 7468 6520 6361 6c6c 6261 636b  ide the callback
-00004210: 2066 756e 6374 696f 6e2c 2060 636f 6e76   function, `conv
-00004220: 6572 7420 3c68 7474 7073 3a2f 2f64 6f63  ert <https://doc
-00004230: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-00004240: 6962 7261 7279 2f73 7464 7479 7065 732e  ibrary/stdtypes.
-00004250: 6874 6d6c 236d 656d 6f72 7976 6965 772e  html#memoryview.
-00004260: 746f 6279 7465 733e 605f 2074 6865 6d20  tobytes>`_ them 
-00004270: 746f 2060 6062 7974 6573 6060 206f 626a  to ``bytes`` obj
-00004280: 6563 7473 2e20 4966 2069 6e70 7574 2073  ects. If input s
-00004290: 7472 6561 6d20 6973 2060 6062 2727 6060  tream is ``b''``
-000042a0: 2c20 7468 6520 6361 6c6c 6261 636b 2066  , the callback f
-000042b0: 756e 6374 696f 6e20 7769 6c6c 206e 6f74  unction will not
-000042c0: 2062 6520 6361 6c6c 6564 2e0a 2020 2020   be called..    
-000042d0: 3a74 7970 6520 6361 6c6c 6261 636b 3a20  :type callback: 
-000042e0: 6361 6c6c 6162 6c65 0a20 2020 203a 7265  callable.    :re
-000042f0: 7475 726e 3a20 4120 322d 6974 656d 2074  turn: A 2-item t
-00004300: 7570 6c65 2c20 6060 2874 6f74 616c 5f69  uple, ``(total_i
-00004310: 6e70 7574 2c20 746f 7461 6c5f 6f75 7470  nput, total_outp
-00004320: 7574 2960 602c 2074 6865 2069 7465 6d73  ut)``, the items
-00004330: 2061 7265 2060 6069 6e74 6060 206f 626a   are ``int`` obj
-00004340: 6563 7473 2e0a 2020 2020 3a72 6169 7365  ects..    :raise
-00004350: 7320 5a73 7464 4572 726f 723a 2049 6620  s ZstdError: If 
-00004360: 6465 636f 6d70 7265 7373 696f 6e20 6661  decompression fa
-00004370: 696c 732e 0a0a 2020 2020 2e2e 2073 6f75  ils...    .. sou
-00004380: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
-00004390: 0a0a 2020 2020 2020 2020 2320 6465 636f  ..        # deco
-000043a0: 6d70 7265 7373 2061 6e20 696e 7075 7420  mpress an input 
-000043b0: 6669 6c65 2c20 616e 6420 7772 6974 6520  file, and write 
-000043c0: 746f 2061 6e20 6f75 7470 7574 2066 696c  to an output fil
-000043d0: 652e 0a20 2020 2020 2020 2077 6974 6820  e..        with 
-000043e0: 696f 2e6f 7065 6e28 696e 7075 745f 6669  io.open(input_fi
-000043f0: 6c65 5f70 6174 682c 2027 7262 2729 2061  le_path, 'rb') a
-00004400: 7320 6966 683a 0a20 2020 2020 2020 2020  s ifh:.         
-00004410: 2020 2077 6974 6820 696f 2e6f 7065 6e28     with io.open(
-00004420: 6f75 7470 7574 5f66 696c 655f 7061 7468  output_file_path
-00004430: 2c20 2777 6227 2920 6173 206f 6668 3a0a  , 'wb') as ofh:.
-00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004450: 6465 636f 6d70 7265 7373 5f73 7472 6561  decompress_strea
-00004460: 6d28 6966 682c 206f 6668 290a 0a20 2020  m(ifh, ofh)..   
-00004470: 2020 2020 2023 2064 6563 6f6d 7072 6573       # decompres
-00004480: 7320 6120 6279 7465 7320 6f62 6a65 6374  s a bytes object
-00004490: 2c20 616e 6420 7772 6974 6520 746f 2061  , and write to a
-000044a0: 2066 696c 652e 0a20 2020 2020 2020 2077   file..        w
-000044b0: 6974 6820 696f 2e42 7974 6573 494f 2863  ith io.BytesIO(c
-000044c0: 6f6d 7072 6573 7365 645f 6461 7429 2061  ompressed_dat) a
-000044d0: 7320 6269 3a0a 2020 2020 2020 2020 2020  s bi:.          
-000044e0: 2020 7769 7468 2069 6f2e 6f70 656e 286f    with io.open(o
-000044f0: 7574 7075 745f 6669 6c65 5f70 6174 682c  utput_file_path,
-00004500: 2027 7762 2729 2061 7320 6f66 683a 0a20   'wb') as ofh:. 
-00004510: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004520: 6563 6f6d 7072 6573 735f 7374 7265 616d  ecompress_stream
-00004530: 2862 692c 206f 6668 290a 0a20 2020 2020  (bi, ofh)..     
-00004540: 2020 2023 2044 6563 6f6d 7072 6573 7320     # Decompress 
-00004550: 616e 2069 6e70 7574 2066 696c 652c 206f  an input file, o
-00004560: 6274 6169 6e20 6120 6279 7465 7320 6f62  btain a bytes ob
-00004570: 6a65 6374 2e0a 2020 2020 2020 2020 2320  ject..        # 
-00004580: 4974 2773 2066 6173 7465 7220 7468 616e  It's faster than
-00004590: 2072 6561 6469 6e67 2061 2066 696c 6520   reading a file 
-000045a0: 616e 6420 6465 636f 6d70 7265 7373 696e  and decompressin
-000045b0: 6720 6974 2069 6e0a 2020 2020 2020 2020  g it in.        
-000045c0: 2320 6d65 6d6f 7279 2c20 7465 7374 6564  # memory, tested
-000045d0: 206f 6e20 5562 756e 7475 2850 7974 686f   on Ubuntu(Pytho
-000045e0: 6e33 2e38 292f 5769 6e64 6f77 7328 5079  n3.8)/Windows(Py
-000045f0: 7468 6f6e 332e 3929 2e0a 2020 2020 2020  thon3.9)..      
-00004600: 2020 2320 4d61 7962 6520 7468 6520 4f53    # Maybe the OS
-00004610: 2068 6173 2070 7265 6665 7463 6869 6e67   has prefetching
-00004620: 2c20 6974 2063 616e 2072 6561 6420 616e  , it can read an
-00004630: 6420 6465 636f 6d70 7265 7373 0a20 2020  d decompress.   
-00004640: 2020 2020 2023 2064 6174 6120 696e 2070       # data in p
-00004650: 6172 616c 6c65 6c20 746f 2073 6f6d 6520  arallel to some 
-00004660: 6465 6772 6565 2c20 7265 6164 696e 6720  degree, reading 
-00004670: 6669 6c65 2066 726f 6d20 4844 440a 2020  file from HDD.  
-00004680: 2020 2020 2020 2320 6973 2074 6865 2062        # is the b
-00004690: 6f74 746c 656e 6563 6b20 696e 2074 6869  ottleneck in thi
-000046a0: 7320 6361 7365 2e0a 2020 2020 2020 2020  s case..        
-000046b0: 7769 7468 2069 6f2e 6f70 656e 2869 6e70  with io.open(inp
-000046c0: 7574 5f66 696c 655f 7061 7468 2c20 2772  ut_file_path, 'r
-000046d0: 6227 2920 6173 2069 6668 3a0a 2020 2020  b') as ifh:.    
-000046e0: 2020 2020 2020 2020 7769 7468 2069 6f2e          with io.
-000046f0: 4279 7465 7349 4f28 2920 6173 2062 6f3a  BytesIO() as bo:
-00004700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004710: 2064 6563 6f6d 7072 6573 735f 7374 7265   decompress_stre
-00004720: 616d 2869 6668 2c20 626f 290a 2020 2020  am(ifh, bo).    
-00004730: 2020 2020 2020 2020 2020 2020 6465 636f              deco
-00004740: 6d70 7265 7373 6564 5f64 6174 203d 2062  mpressed_dat = b
-00004750: 6f2e 6765 7476 616c 7565 2829 0a0a 2020  o.getvalue()..  
-00004760: 2020 2020 2020 2320 5072 696e 7420 7072        # Print pr
-00004770: 6f67 7265 7373 2075 7369 6e67 2063 616c  ogress using cal
-00004780: 6c62 6163 6b20 6675 6e63 7469 6f6e 0a20  lback function. 
-00004790: 2020 2020 2020 2064 6566 2064 6563 6f6d         def decom
-000047a0: 7072 6573 735f 7072 696e 745f 7072 6f67  press_print_prog
-000047b0: 7265 7373 2869 6e70 7574 5f66 696c 655f  ress(input_file_
-000047c0: 7061 7468 2c20 6f75 7470 7574 5f66 696c  path, output_fil
-000047d0: 655f 7061 7468 293a 0a20 2020 2020 2020  e_path):.       
-000047e0: 2020 2020 2069 6e70 7574 5f66 696c 655f       input_file_
-000047f0: 7369 7a65 203d 206f 732e 7061 7468 2e67  size = os.path.g
-00004800: 6574 7369 7a65 2869 6e70 7574 5f66 696c  etsize(input_fil
-00004810: 655f 7061 7468 290a 0a20 2020 2020 2020  e_path)..       
-00004820: 2020 2020 2064 6566 2066 756e 6328 746f       def func(to
-00004830: 7461 6c5f 696e 7075 742c 2074 6f74 616c  tal_input, total
-00004840: 5f6f 7574 7075 742c 2072 6561 645f 6461  _output, read_da
-00004850: 7461 2c20 7772 6974 655f 6461 7461 293a  ta, write_data):
-00004860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004870: 2023 2049 6620 696e 7075 7420 7374 7265   # If input stre
-00004880: 616d 2069 7320 656d 7074 792c 2074 6865  am is empty, the
-00004890: 2063 616c 6c62 6163 6b20 6675 6e63 7469   callback functi
-000048a0: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-000048b0: 2020 2023 2077 696c 6c20 6e6f 7420 6265     # will not be
-000048c0: 2063 616c 6c65 642e 2053 6f20 6e6f 205a   called. So no Z
-000048d0: 6572 6f44 6976 6973 696f 6e45 7272 6f72  eroDivisionError
-000048e0: 2068 6572 652e 0a20 2020 2020 2020 2020   here..         
-000048f0: 2020 2020 2020 2070 6572 6365 6e74 203d         percent =
-00004900: 2031 3030 202a 2074 6f74 616c 5f69 6e70   100 * total_inp
-00004910: 7574 202f 2069 6e70 7574 5f66 696c 655f  ut / input_file_
-00004920: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
-00004930: 2020 2020 2070 7269 6e74 2866 2750 726f       print(f'Pro
-00004940: 6772 6573 733a 207b 7065 7263 656e 743a  gress: {percent:
-00004950: 2e31 667d 2527 2c20 656e 643d 275c 7227  .1f}%', end='\r'
-00004960: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
-00004970: 6974 6820 696f 2e6f 7065 6e28 696e 7075  ith io.open(inpu
-00004980: 745f 6669 6c65 5f70 6174 682c 2027 7262  t_file_path, 'rb
-00004990: 2729 2061 7320 6966 683a 0a20 2020 2020  ') as ifh:.     
-000049a0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-000049b0: 696f 2e6f 7065 6e28 6f75 7470 7574 5f66  io.open(output_f
-000049c0: 696c 655f 7061 7468 2c20 2777 6227 2920  ile_path, 'wb') 
-000049d0: 6173 206f 6668 3a0a 2020 2020 2020 2020  as ofh:.        
-000049e0: 2020 2020 2020 2020 2020 2020 6465 636f              deco
-000049f0: 6d70 7265 7373 5f73 7472 6561 6d28 6966  mpress_stream(if
-00004a00: 682c 206f 6668 2c20 6361 6c6c 6261 636b  h, ofh, callback
-00004a10: 3d66 756e 6329 0a0a 0a2e 2e20 7079 3a63  =func)..... py:c
-00004a20: 6c61 7373 3a3a 205a 7374 6444 6563 6f6d  lass:: ZstdDecom
-00004a30: 7072 6573 736f 720a 0a20 2020 2041 2073  pressor..    A s
-00004a40: 7472 6561 6d69 6e67 2064 6563 6f6d 7072  treaming decompr
-00004a50: 6573 736f 722e 0a0a 2020 2020 4166 7465  essor...    Afte
-00004a60: 7220 6120 3a72 6566 3a60 6672 616d 653c  r a :ref:`frame<
-00004a70: 6672 616d 655f 626c 6f63 6b3e 6020 6973  frame_block>` is
-00004a80: 2064 6563 6f6d 7072 6573 7365 642c 2069   decompressed, i
-00004a90: 7420 7374 6f70 7320 616e 6420 7365 7473  t stops and sets
-00004aa0: 203a 7079 3a61 7474 723a 607e 5a73 7464   :py:attr:`~Zstd
-00004ab0: 4465 636f 6d70 7265 7373 6f72 2e65 6f66  Decompressor.eof
-00004ac0: 6020 666c 6167 2074 6f20 6060 5472 7565  ` flag to ``True
-00004ad0: 6060 2e0a 0a20 2020 2046 6f72 206d 756c  ``...    For mul
-00004ae0: 7469 706c 6520 6672 616d 6573 2064 6174  tiple frames dat
-00004af0: 612c 2075 7365 203a 7079 3a63 6c61 7373  a, use :py:class
-00004b00: 3a60 456e 646c 6573 735a 7374 6444 6563  :`EndlessZstdDec
-00004b10: 6f6d 7072 6573 736f 7260 2e0a 0a20 2020  ompressor`...   
-00004b20: 2054 6872 6561 642d 7361 6665 2061 7420   Thread-safe at 
-00004b30: 6d65 7468 6f64 206c 6576 656c 2e0a 0a20  method level... 
-00004b40: 2020 202e 2e20 7079 3a6d 6574 686f 643a     .. py:method:
-00004b50: 3a20 5f5f 696e 6974 5f5f 2873 656c 662c  : __init__(self,
-00004b60: 207a 7374 645f 6469 6374 3d4e 6f6e 652c   zstd_dict=None,
-00004b70: 206f 7074 696f 6e3d 4e6f 6e65 290a 0a20   option=None).. 
-00004b80: 2020 2020 2020 2049 6e69 7469 616c 697a         Initializ
-00004b90: 6520 6120 5a73 7464 4465 636f 6d70 7265  e a ZstdDecompre
-00004ba0: 7373 6f72 206f 626a 6563 742e 0a0a 2020  ssor object...  
-00004bb0: 2020 2020 2020 3a70 6172 616d 207a 7374        :param zst
-00004bc0: 645f 6469 6374 3a20 5072 652d 7472 6169  d_dict: Pre-trai
-00004bd0: 6e65 6420 6469 6374 696f 6e61 7279 2066  ned dictionary f
-00004be0: 6f72 2064 6563 6f6d 7072 6573 7369 6f6e  or decompression
-00004bf0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00004c00: 7a73 7464 5f64 6963 743a 205a 7374 6444  zstd_dict: ZstdD
-00004c10: 6963 740a 2020 2020 2020 2020 3a70 6172  ict.        :par
-00004c20: 616d 2064 6963 7420 6f70 7469 6f6e 3a20  am dict option: 
-00004c30: 4120 6060 6469 6374 6060 206f 626a 6563  A ``dict`` objec
-00004c40: 7420 7468 6174 2063 6f6e 7461 696e 7320  t that contains 
-00004c50: 3a72 6566 3a60 6164 7661 6e63 6564 2064  :ref:`advanced d
-00004c60: 6563 6f6d 7072 6573 7369 6f6e 2070 6172  ecompression par
-00004c70: 616d 6574 6572 733c 4450 6172 616d 6574  ameters<DParamet
-00004c80: 6572 3e60 2e20 5468 6520 6465 6661 756c  er>`. The defaul
-00004c90: 7420 7661 6c75 6520 6060 4e6f 6e65 6060  t value ``None``
-00004ca0: 206d 6561 6e73 2074 6f20 7573 6520 7a73   means to use zs
-00004cb0: 7464 2773 2064 6566 6175 6c74 2064 6563  td's default dec
-00004cc0: 6f6d 7072 6573 7369 6f6e 2070 6172 616d  ompression param
-00004cd0: 6574 6572 732e 0a0a 2020 2020 2e2e 2070  eters...    .. p
-00004ce0: 793a 6d65 7468 6f64 3a3a 2064 6563 6f6d  y:method:: decom
-00004cf0: 7072 6573 7328 7365 6c66 2c20 6461 7461  press(self, data
-00004d00: 2c20 6d61 785f 6c65 6e67 7468 3d2d 3129  , max_length=-1)
-00004d10: 0a0a 2020 2020 2020 2020 4465 636f 6d70  ..        Decomp
-00004d20: 7265 7373 202a 6461 7461 2a2c 2072 6574  ress *data*, ret
-00004d30: 7572 6e69 6e67 2064 6563 6f6d 7072 6573  urning decompres
-00004d40: 7365 6420 6461 7461 2061 7320 6120 6060  sed data as a ``
-00004d50: 6279 7465 7360 6020 6f62 6a65 6374 2e0a  bytes`` object..
-00004d60: 0a20 2020 2020 2020 2041 6674 6572 2061  .        After a
-00004d70: 203a 7265 663a 6066 7261 6d65 3c66 7261   :ref:`frame<fra
-00004d80: 6d65 5f62 6c6f 636b 3e60 2069 7320 6465  me_block>` is de
-00004d90: 636f 6d70 7265 7373 6564 2c20 6974 2073  compressed, it s
-00004da0: 746f 7073 2061 6e64 2073 6574 7320 3a70  tops and sets :p
-00004db0: 793a 6174 7472 3a60 7e5a 7374 6444 6563  y:attr:`~ZstdDec
-00004dc0: 6f6d 7072 6573 736f 722e 656f 6660 2066  ompressor.eof` f
-00004dd0: 6c61 6720 746f 2060 6054 7275 6560 602e  lag to ``True``.
-00004de0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00004df0: 2064 6174 613a 2044 6174 6120 746f 2062   data: Data to b
-00004e00: 6520 6465 636f 6d70 7265 7373 6564 2e0a  e decompressed..
-00004e10: 2020 2020 2020 2020 3a74 7970 6520 6461          :type da
-00004e20: 7461 3a20 6279 7465 732d 6c69 6b65 206f  ta: bytes-like o
-00004e30: 626a 6563 740a 2020 2020 2020 2020 3a70  bject.        :p
-00004e40: 6172 616d 2069 6e74 206d 6178 5f6c 656e  aram int max_len
-00004e50: 6774 683a 204d 6178 696d 756d 2073 697a  gth: Maximum siz
-00004e60: 6520 6f66 2072 6574 7572 6e65 6420 6461  e of returned da
-00004e70: 7461 2e20 5768 656e 2069 7427 7320 6e65  ta. When it's ne
-00004e80: 6761 7469 7665 2c20 7468 6520 6f75 7470  gative, the outp
-00004e90: 7574 2073 697a 6520 6973 2075 6e6c 696d  ut size is unlim
-00004ea0: 6974 6564 2e20 5768 656e 2069 7427 7320  ited. When it's 
-00004eb0: 6e6f 6e2d 6e65 6761 7469 7665 2c20 7265  non-negative, re
-00004ec0: 7475 726e 7320 6174 206d 6f73 7420 2a6d  turns at most *m
-00004ed0: 6178 5f6c 656e 6774 682a 2062 7974 6573  ax_length* bytes
-00004ee0: 206f 6620 6465 636f 6d70 7265 7373 6564   of decompressed
-00004ef0: 2064 6174 612e 2049 6620 7468 6973 206c   data. If this l
-00004f00: 696d 6974 2069 7320 7265 6163 6865 6420  imit is reached 
-00004f10: 616e 6420 6675 7274 6865 7220 6f75 7470  and further outp
-00004f20: 7574 2063 616e 2028 6f72 206d 6179 2920  ut can (or may) 
-00004f30: 6265 2070 726f 6475 6365 642c 2074 6865  be produced, the
-00004f40: 203a 7079 3a61 7474 723a 607e 5a73 7464   :py:attr:`~Zstd
-00004f50: 4465 636f 6d70 7265 7373 6f72 2e6e 6565  Decompressor.nee
-00004f60: 6473 5f69 6e70 7574 6020 6174 7472 6962  ds_input` attrib
-00004f70: 7574 6520 7769 6c6c 2062 6520 7365 7420  ute will be set 
-00004f80: 746f 2060 6046 616c 7365 6060 2e20 496e  to ``False``. In
-00004f90: 2074 6869 7320 6361 7365 2c20 7468 6520   this case, the 
-00004fa0: 6e65 7874 2063 616c 6c20 746f 2074 6869  next call to thi
-00004fb0: 7320 6d65 7468 6f64 206d 6179 2070 726f  s method may pro
-00004fc0: 7669 6465 202a 6461 7461 2a20 6173 2060  vide *data* as `
-00004fd0: 6062 2727 6060 2074 6f20 6f62 7461 696e  `b''`` to obtain
-00004fe0: 206d 6f72 6520 6f66 2074 6865 206f 7574   more of the out
-00004ff0: 7075 742e 0a0a 2020 2020 2e2e 2070 793a  put...    .. py:
-00005000: 6174 7472 6962 7574 653a 3a20 6e65 6564  attribute:: need
-00005010: 735f 696e 7075 740a 0a20 2020 2020 2020  s_input..       
-00005020: 2049 6620 7468 6520 2a6d 6178 5f6c 656e   If the *max_len
-00005030: 6774 682a 206f 7574 7075 7420 6c69 6d69  gth* output limi
-00005040: 7420 696e 203a 7079 3a6d 6574 683a 607e  t in :py:meth:`~
-00005050: 5a73 7464 4465 636f 6d70 7265 7373 6f72  ZstdDecompressor
-00005060: 2e64 6563 6f6d 7072 6573 7360 206d 6574  .decompress` met
-00005070: 686f 6420 6861 7320 6265 656e 2072 6561  hod has been rea
-00005080: 6368 6564 2c20 616e 6420 7468 6520 6465  ched, and the de
-00005090: 636f 6d70 7265 7373 6f72 2068 6173 2028  compressor has (
-000050a0: 6f72 206d 6179 2068 6173 2920 756e 636f  or may has) unco
-000050b0: 6e73 756d 6564 2069 6e70 7574 2064 6174  nsumed input dat
-000050c0: 612c 2069 7420 7769 6c6c 2062 6520 7365  a, it will be se
-000050d0: 7420 746f 2060 6046 616c 7365 6060 2e20  t to ``False``. 
-000050e0: 496e 2074 6869 7320 6361 7365 2c20 7061  In this case, pa
-000050f0: 7373 2060 6062 2727 6060 2074 6f20 3a70  ss ``b''`` to :p
-00005100: 793a 6d65 7468 3a60 7e5a 7374 6444 6563  y:meth:`~ZstdDec
-00005110: 6f6d 7072 6573 736f 722e 6465 636f 6d70  ompressor.decomp
-00005120: 7265 7373 6020 6d65 7468 6f64 206d 6179  ress` method may
-00005130: 206f 7574 7075 7420 6675 7274 6865 7220   output further 
-00005140: 6461 7461 2e0a 0a20 2020 2020 2020 2049  data...        I
-00005150: 6620 6967 6e6f 7265 2074 6869 7320 6174  f ignore this at
-00005160: 7472 6962 7574 6520 7768 656e 2074 6865  tribute when the
-00005170: 7265 2069 7320 756e 636f 6e73 756d 6564  re is unconsumed
-00005180: 2069 6e70 7574 2064 6174 612c 2074 6865   input data, the
-00005190: 7265 2077 696c 6c20 6265 2061 206c 6974  re will be a lit
-000051a0: 746c 6520 7065 7266 6f72 6d61 6e63 6520  tle performance 
-000051b0: 6c6f 7373 2062 6563 6175 7365 206f 6620  loss because of 
-000051c0: 6578 7472 6120 6d65 6d6f 7279 2063 6f70  extra memory cop
-000051d0: 792e 0a0a 2020 2020 2e2e 2070 793a 6174  y...    .. py:at
-000051e0: 7472 6962 7574 653a 3a20 656f 660a 0a20  tribute:: eof.. 
-000051f0: 2020 2020 2020 2060 6054 7275 6560 6020         ``True`` 
-00005200: 6d65 616e 7320 7468 6520 656e 6420 6f66  means the end of
-00005210: 2074 6865 2066 6972 7374 2066 7261 6d65   the first frame
-00005220: 2068 6173 2062 6565 6e20 7265 6163 6865   has been reache
-00005230: 642e 2049 6620 6465 636f 6d70 7265 7373  d. If decompress
-00005240: 2064 6174 6120 6166 7465 7220 7468 6174   data after that
-00005250: 2c20 616e 2060 6045 4f46 4572 726f 7260  , an ``EOFError`
-00005260: 6020 6578 6365 7074 696f 6e20 7769 6c6c  ` exception will
-00005270: 2062 6520 7261 6973 6564 2e0a 0a20 2020   be raised...   
-00005280: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
-00005290: 3a3a 2075 6e75 7365 645f 6461 7461 0a0a  :: unused_data..
-000052a0: 2020 2020 2020 2020 4120 6279 7465 7320          A bytes 
-000052b0: 6f62 6a65 6374 2e20 5768 656e 205a 7374  object. When Zst
-000052c0: 6444 6563 6f6d 7072 6573 736f 7220 6f62  dDecompressor ob
-000052d0: 6a65 6374 2073 746f 7073 2061 6674 6572  ject stops after
-000052e0: 2064 6563 6f6d 7072 6573 7369 6e67 2061   decompressing a
-000052f0: 2066 7261 6d65 2c20 756e 7573 6564 2069   frame, unused i
-00005300: 6e70 7574 2064 6174 6120 6166 7465 7220  nput data after 
-00005310: 7468 6520 6669 7273 7420 6672 616d 652e  the first frame.
-00005320: 204f 7468 6572 7769 7365 2074 6869 7320   Otherwise this 
-00005330: 7769 6c6c 2062 6520 6060 6227 2760 602e  will be ``b''``.
-00005340: 0a0a 2020 2020 2e2e 2073 6f75 7263 6563  ..    .. sourcec
-00005350: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
-00005360: 2020 2020 2020 2320 2d2d 2d20 756e 6c69        # --- unli
-00005370: 6d69 7465 6420 6f75 7470 7574 202d 2d2d  mited output ---
-00005380: 0a20 2020 2020 2020 2064 3120 3d20 5a73  .        d1 = Zs
-00005390: 7464 4465 636f 6d70 7265 7373 6f72 2829  tdDecompressor()
-000053a0: 0a0a 2020 2020 2020 2020 6465 636f 6d70  ..        decomp
-000053b0: 7265 7373 6564 5f64 6174 3120 3d20 6431  ressed_dat1 = d1
-000053c0: 2e64 6563 6f6d 7072 6573 7328 6461 7431  .decompress(dat1
-000053d0: 290a 2020 2020 2020 2020 6465 636f 6d70  ).        decomp
-000053e0: 7265 7373 6564 5f64 6174 3220 3d20 6431  ressed_dat2 = d1
-000053f0: 2e64 6563 6f6d 7072 6573 7328 6461 7432  .decompress(dat2
-00005400: 290a 2020 2020 2020 2020 6465 636f 6d70  ).        decomp
-00005410: 7265 7373 6564 5f64 6174 3320 3d20 6431  ressed_dat3 = d1
-00005420: 2e64 6563 6f6d 7072 6573 7328 6461 7433  .decompress(dat3
-00005430: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00005440: 7420 6431 2e65 6f66 2c20 2764 6174 6120  t d1.eof, 'data 
-00005450: 6973 2061 6e20 696e 636f 6d70 6c65 7465  is an incomplete
-00005460: 207a 7374 6420 6672 616d 652e 270a 0a20   zstd frame.'.. 
-00005470: 2020 2020 2020 2023 202d 2d2d 206c 696d         # --- lim
-00005480: 6974 6564 206f 7574 7075 7420 2d2d 2d0a  ited output ---.
-00005490: 2020 2020 2020 2020 6432 203d 205a 7374          d2 = Zst
-000054a0: 6444 6563 6f6d 7072 6573 736f 7228 290a  dDecompressor().
-000054b0: 0a20 2020 2020 2020 2077 6869 6c65 2054  .        while T
-000054c0: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
-000054d0: 2069 6620 6432 2e6e 6565 6473 5f69 6e70   if d2.needs_inp
-000054e0: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
-000054f0: 2020 2020 6461 7420 3d20 7265 6164 5f69      dat = read_i
-00005500: 6e70 7574 2832 2a31 3032 342a 3130 3234  nput(2*1024*1024
-00005510: 2920 2320 7265 6164 2032 204d 6942 2069  ) # read 2 MiB i
-00005520: 6e70 7574 2064 6174 610a 2020 2020 2020  nput data.      
-00005530: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00005540: 2064 6174 3a20 2320 696e 7075 7420 7374   dat: # input st
-00005550: 7265 616d 2065 6e64 730a 2020 2020 2020  ream ends.      
-00005560: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00005570: 6973 6520 4578 6365 7074 696f 6e28 2749  ise Exception('I
-00005580: 6e70 7574 2073 7472 6561 6d20 656e 6473  nput stream ends
-00005590: 2c20 6275 7420 7468 6520 656e 6420 6f66  , but the end of
-000055a0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 2020 2020 2020 2027 7468 6520 6669 7273         'the firs
-000055d0: 7420 6672 616d 6520 6973 206e 6f74 2072  t frame is not r
-000055e0: 6561 6368 6564 2e27 290a 2020 2020 2020  eached.').      
-000055f0: 2020 2020 2020 656c 7365 3a20 2320 6d61        else: # ma
-00005600: 7962 6520 7468 6572 6520 6973 2075 6e63  ybe there is unc
-00005610: 6f6e 7375 6d65 6420 696e 7075 7420 6461  onsumed input da
-00005620: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
-00005630: 2020 2064 6174 203d 2062 2727 0a0a 2020     dat = b''..  
-00005640: 2020 2020 2020 2020 2020 6368 756e 6b20            chunk 
-00005650: 3d20 6432 2e64 6563 6f6d 7072 6573 7328  = d2.decompress(
-00005660: 6461 742c 2031 302a 3130 3234 2a31 3032  dat, 10*1024*102
-00005670: 3429 2023 206c 696d 6974 206f 7574 7075  4) # limit outpu
-00005680: 7420 6275 6666 6572 2074 6f20 3130 204d  t buffer to 10 M
-00005690: 6942 0a20 2020 2020 2020 2020 2020 2077  iB.            w
-000056a0: 7269 7465 5f6f 7574 7075 7428 6368 756e  rite_output(chun
-000056b0: 6b29 0a0a 2020 2020 2020 2020 2020 2020  k)..            
-000056c0: 6966 2064 322e 656f 663a 2023 2072 6561  if d2.eof: # rea
-000056d0: 6368 2074 6865 2065 6e64 206f 6620 7468  ch the end of th
-000056e0: 6520 6669 7273 7420 6672 616d 650a 2020  e first frame.  
-000056f0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00005700: 6561 6b0a 0a0a 2e2e 2070 793a 636c 6173  eak..... py:clas
-00005710: 733a 3a20 456e 646c 6573 735a 7374 6444  s:: EndlessZstdD
-00005720: 6563 6f6d 7072 6573 736f 720a 0a20 2020  ecompressor..   
-00005730: 2041 2073 7472 6561 6d69 6e67 2064 6563   A streaming dec
-00005740: 6f6d 7072 6573 736f 722e 0a0a 2020 2020  ompressor...    
-00005750: 4974 2064 6f65 736e 2774 2073 746f 7020  It doesn't stop 
-00005760: 6166 7465 7220 6120 3a72 6566 3a60 6672  after a :ref:`fr
-00005770: 616d 653c 6672 616d 655f 626c 6f63 6b3e  ame<frame_block>
-00005780: 6020 6973 2064 6563 6f6d 7072 6573 7365  ` is decompresse
-00005790: 642c 2063 616e 2062 6520 7573 6564 2074  d, can be used t
-000057a0: 6f20 6465 636f 6d70 7265 7373 206d 756c  o decompress mul
-000057b0: 7469 706c 6520 636f 6e63 6174 656e 6174  tiple concatenat
-000057c0: 6564 2066 7261 6d65 732e 0a0a 2020 2020  ed frames...    
-000057d0: 5468 7265 6164 2d73 6166 6520 6174 206d  Thread-safe at m
-000057e0: 6574 686f 6420 6c65 7665 6c2e 0a0a 2020  ethod level...  
-000057f0: 2020 2e2e 2070 793a 6d65 7468 6f64 3a3a    .. py:method::
-00005800: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00005810: 7a73 7464 5f64 6963 743d 4e6f 6e65 2c20  zstd_dict=None, 
-00005820: 6f70 7469 6f6e 3d4e 6f6e 6529 0a0a 2020  option=None)..  
-00005830: 2020 2020 2020 5468 6520 7061 7261 6d65        The parame
-00005840: 7465 7273 2061 7265 2074 6865 2073 616d  ters are the sam
-00005850: 6520 6173 203a 7079 3a6d 6574 683a 605a  e as :py:meth:`Z
-00005860: 7374 6444 6563 6f6d 7072 6573 736f 722e  stdDecompressor.
-00005870: 5f5f 696e 6974 5f5f 6020 6d65 7468 6f64  __init__` method
-00005880: 2e0a 0a20 2020 202e 2e20 7079 3a6d 6574  ...    .. py:met
-00005890: 686f 643a 3a20 6465 636f 6d70 7265 7373  hod:: decompress
-000058a0: 2873 656c 662c 2064 6174 612c 206d 6178  (self, data, max
-000058b0: 5f6c 656e 6774 683d 2d31 290a 0a20 2020  _length=-1)..   
-000058c0: 2020 2020 2054 6865 2070 6172 616d 6574       The paramet
-000058d0: 6572 7320 6172 6520 7468 6520 7361 6d65  ers are the same
-000058e0: 2061 7320 3a70 793a 6d65 7468 3a60 5a73   as :py:meth:`Zs
-000058f0: 7464 4465 636f 6d70 7265 7373 6f72 2e64  tdDecompressor.d
-00005900: 6563 6f6d 7072 6573 7360 206d 6574 686f  ecompress` metho
-00005910: 642e 0a0a 2020 2020 2020 2020 4166 7465  d...        Afte
-00005920: 7220 6465 636f 6d70 7265 7373 696e 6720  r decompressing 
-00005930: 6120 6672 616d 652c 2069 7420 646f 6573  a frame, it does
-00005940: 6e27 7420 7374 6f70 206c 696b 6520 3a70  n't stop like :p
-00005950: 793a 6d65 7468 3a60 5a73 7464 4465 636f  y:meth:`ZstdDeco
-00005960: 6d70 7265 7373 6f72 2e64 6563 6f6d 7072  mpressor.decompr
-00005970: 6573 7360 2e0a 0a20 2020 202e 2e20 7079  ess`...    .. py
-00005980: 3a61 7474 7269 6275 7465 3a3a 206e 6565  :attribute:: nee
-00005990: 6473 5f69 6e70 7574 0a0a 2020 2020 2020  ds_input..      
-000059a0: 2020 4974 2773 2074 6865 2073 616d 6520    It's the same 
-000059b0: 6173 203a 7079 3a61 7474 723a 605a 7374  as :py:attr:`Zst
-000059c0: 6444 6563 6f6d 7072 6573 736f 722e 6e65  dDecompressor.ne
-000059d0: 6564 735f 696e 7075 7460 2e0a 0a20 2020  eds_input`...   
-000059e0: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
-000059f0: 3a3a 2061 745f 6672 616d 655f 6564 6765  :: at_frame_edge
-00005a00: 0a0a 2020 2020 2020 2020 6060 5472 7565  ..        ``True
-00005a10: 6060 2077 6865 6e20 626f 7468 2074 6865  `` when both the
-00005a20: 2069 6e70 7574 2061 6e64 206f 7574 7075   input and outpu
-00005a30: 7420 7374 7265 616d 7320 6172 6520 6174  t streams are at
-00005a40: 2061 203a 7265 663a 6066 7261 6d65 3c66   a :ref:`frame<f
-00005a50: 7261 6d65 5f62 6c6f 636b 3e60 2065 6467  rame_block>` edg
-00005a60: 652c 206f 7220 7468 6520 6465 636f 6d70  e, or the decomp
-00005a70: 7265 7373 6f72 206a 7573 7420 6265 2069  ressor just be i
-00005a80: 6e69 7469 616c 697a 6564 2e0a 0a20 2020  nitialized...   
-00005a90: 2020 2020 2054 6869 7320 666c 6167 2063       This flag c
-00005aa0: 6f75 6c64 2062 6520 7573 6564 2074 6f20  ould be used to 
-00005ab0: 6368 6563 6b20 6461 7461 2069 6e74 6567  check data integ
-00005ac0: 7269 7479 2069 6e20 736f 6d65 2063 6173  rity in some cas
-00005ad0: 6573 2e0a 0a20 2020 202e 2e20 736f 7572  es...    .. sour
-00005ae0: 6365 636f 6465 3a3a 2070 7974 686f 6e0a  cecode:: python.
-00005af0: 0a20 2020 2020 2020 2023 202d 2d2d 2073  .        # --- s
-00005b00: 7472 6561 6d69 6e67 2064 6563 6f6d 7072  treaming decompr
-00005b10: 6573 7369 6f6e 2c20 756e 6c69 6d69 7465  ession, unlimite
-00005b20: 6420 6f75 7470 7574 202d 2d2d 0a20 2020  d output ---.   
-00005b30: 2020 2020 2064 3120 3d20 456e 646c 6573       d1 = Endles
-00005b40: 735a 7374 6444 6563 6f6d 7072 6573 736f  sZstdDecompresso
-00005b50: 7228 290a 0a20 2020 2020 2020 2064 6563  r()..        dec
-00005b60: 6f6d 7072 6573 7365 645f 6461 7431 203d  ompressed_dat1 =
-00005b70: 2064 312e 6465 636f 6d70 7265 7373 2864   d1.decompress(d
-00005b80: 6174 3129 0a20 2020 2020 2020 2064 6563  at1).        dec
-00005b90: 6f6d 7072 6573 7365 645f 6461 7432 203d  ompressed_dat2 =
-00005ba0: 2064 312e 6465 636f 6d70 7265 7373 2864   d1.decompress(d
-00005bb0: 6174 3229 0a20 2020 2020 2020 2064 6563  at2).        dec
-00005bc0: 6f6d 7072 6573 7365 645f 6461 7433 203d  ompressed_dat3 =
-00005bd0: 2064 312e 6465 636f 6d70 7265 7373 2864   d1.decompress(d
-00005be0: 6174 3329 0a0a 2020 2020 2020 2020 6173  at3)..        as
-00005bf0: 7365 7274 2064 312e 6174 5f66 7261 6d65  sert d1.at_frame
-00005c00: 5f65 6467 652c 2027 6461 7461 2065 6e64  _edge, 'data end
-00005c10: 7320 696e 2061 6e20 696e 636f 6d70 6c65  s in an incomple
-00005c20: 7465 2066 7261 6d65 2e27 0a0a 2020 2020  te frame.'..    
-00005c30: 2020 2020 2320 2d2d 2d20 7374 7265 616d      # --- stream
-00005c40: 696e 6720 6465 636f 6d70 7265 7373 696f  ing decompressio
-00005c50: 6e2c 206c 696d 6974 6564 206f 7574 7075  n, limited outpu
-00005c60: 7420 2d2d 2d0a 2020 2020 2020 2020 6432  t ---.        d2
-00005c70: 203d 2045 6e64 6c65 7373 5a73 7464 4465   = EndlessZstdDe
-00005c80: 636f 6d70 7265 7373 6f72 2829 0a0a 2020  compressor()..  
-00005c90: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-00005ca0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00005cb0: 2064 322e 6e65 6564 735f 696e 7075 743a   d2.needs_input:
-00005cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005cd0: 2064 6174 203d 2072 6561 645f 696e 7075   dat = read_inpu
-00005ce0: 7428 322a 3130 3234 2a31 3032 3429 2023  t(2*1024*1024) #
-00005cf0: 2072 6561 6420 3220 4d69 4220 696e 7075   read 2 MiB inpu
-00005d00: 7420 6461 7461 0a20 2020 2020 2020 2020  t data.         
-00005d10: 2020 2020 2020 2069 6620 6e6f 7420 6461         if not da
-00005d20: 743a 2023 2069 6e70 7574 2073 7472 6561  t: # input strea
-00005d30: 6d20 656e 6473 0a20 2020 2020 2020 2020  m ends.         
-00005d40: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00005d50: 7420 6432 2e61 745f 6672 616d 655f 6564  t d2.at_frame_ed
-00005d60: 6765 3a0a 2020 2020 2020 2020 2020 2020  ge:.            
-00005d70: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00005d80: 6520 4578 6365 7074 696f 6e28 2764 6174  e Exception('dat
-00005d90: 6120 656e 6473 2069 6e20 616e 2069 6e63  a ends in an inc
-00005da0: 6f6d 706c 6574 6520 6672 616d 652e 2729  omplete frame.')
-00005db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005dc0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-00005dd0: 2020 2020 2020 2065 6c73 653a 2023 206d         else: # m
-00005de0: 6179 6265 2074 6865 7265 2069 7320 756e  aybe there is un
-00005df0: 636f 6e73 756d 6564 2069 6e70 7574 2064  consumed input d
-00005e00: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-00005e10: 2020 2020 6461 7420 3d20 6227 270a 0a20      dat = b''.. 
-00005e20: 2020 2020 2020 2020 2020 2063 6875 6e6b             chunk
-00005e30: 203d 2064 322e 6465 636f 6d70 7265 7373   = d2.decompress
-00005e40: 2864 6174 2c20 3130 2a31 3032 342a 3130  (dat, 10*1024*10
-00005e50: 3234 2920 2320 6c69 6d69 7420 6f75 7470  24) # limit outp
-00005e60: 7574 2062 7566 6665 7220 746f 2031 3020  ut buffer to 10 
-00005e70: 4d69 420a 2020 2020 2020 2020 2020 2020  MiB.            
-00005e80: 7772 6974 655f 6f75 7470 7574 2863 6875  write_output(chu
-00005e90: 6e6b 290a 0a20 2020 202e 2e20 6869 6e74  nk)..    .. hint
-00005ea0: 3a3a 2057 6879 203a 7079 3a63 6c61 7373  :: Why :py:class
-00005eb0: 3a60 456e 646c 6573 735a 7374 6444 6563  :`EndlessZstdDec
-00005ec0: 6f6d 7072 6573 736f 7260 2064 6f65 736e  ompressor` doesn
-00005ed0: 2774 2073 746f 7020 6174 2066 7261 6d65  't stop at frame
-00005ee0: 2065 6467 6573 3f0a 0a20 2020 2020 2020   edges?..       
-00005ef0: 2049 6620 736f 2c20 756e 7573 6564 2069   If so, unused i
-00005f00: 6e70 7574 2064 6174 6120 6166 7465 7220  nput data after 
-00005f10: 616e 2065 6467 6520 7769 6c6c 2062 6520  an edge will be 
-00005f20: 636f 7069 6564 2074 6f20 616e 2069 6e74  copied to an int
-00005f30: 6572 6e61 6c20 6275 6666 6572 2c20 7468  ernal buffer, th
-00005f40: 6973 206d 6179 2062 6520 6120 7065 7266  is may be a perf
-00005f50: 6f72 6d61 6e63 6520 6f76 6572 6865 6164  ormance overhead
-00005f60: 2e0a 0a20 2020 2020 2020 2049 6620 7761  ...        If wa
-00005f70: 6e74 2074 6f20 7374 6f70 2061 7420 6672  nt to stop at fr
-00005f80: 616d 6520 6564 6765 732c 2077 7269 7465  ame edges, write
-00005f90: 2061 2077 7261 7070 6572 2075 7369 6e67   a wrapper using
-00005fa0: 203a 7079 3a63 6c61 7373 3a60 5a73 7464   :py:class:`Zstd
-00005fb0: 4465 636f 6d70 7265 7373 6f72 6020 636c  Decompressor` cl
-00005fc0: 6173 732e 2041 6e64 2064 6f6e 2774 2066  ass. And don't f
-00005fd0: 6565 6420 746f 6f20 6d75 6368 2064 6174  eed too much dat
-00005fe0: 6120 6576 6572 7920 7469 6d65 2c20 7468  a every time, th
-00005ff0: 6520 6f76 6572 6865 6164 206f 6620 636f  e overhead of co
-00006000: 7079 696e 6720 756e 7573 6564 2069 6e70  pying unused inp
-00006010: 7574 2064 6174 6120 746f 203a 7079 3a61  ut data to :py:a
-00006020: 7474 723a 605a 7374 6444 6563 6f6d 7072  ttr:`ZstdDecompr
-00006030: 6573 736f 722e 756e 7573 6564 5f64 6174  essor.unused_dat
-00006040: 6160 2061 7474 7269 6275 7465 2073 7469  a` attribute sti
-00006050: 6c6c 2065 7869 7374 732e 0a0a 0a2e 2e20  ll exists...... 
-00006060: 5f7a 7374 645f 6469 6374 3a0a 0a44 6963  _zstd_dict:..Dic
-00006070: 7469 6f6e 6172 790a 2d2d 2d2d 2d2d 2d2d  tionary.--------
-00006080: 2d2d 0a0a 2020 2020 5468 6973 2073 6563  --..    This sec
-00006090: 7469 6f6e 2063 6f6e 7461 696e 733a 0a0a  tion contains:..
-000060a0: 2020 2020 2020 2020 2a20 636c 6173 7320          * class 
-000060b0: 3a70 793a 636c 6173 733a 605a 7374 6444  :py:class:`ZstdD
-000060c0: 6963 7460 0a20 2020 2020 2020 202a 2066  ict`.        * f
-000060d0: 756e 6374 696f 6e20 3a70 793a 6675 6e63  unction :py:func
-000060e0: 3a60 7472 6169 6e5f 6469 6374 600a 2020  :`train_dict`.  
-000060f0: 2020 2020 2020 2a20 6675 6e63 7469 6f6e        * function
-00006100: 203a 7079 3a66 756e 633a 6066 696e 616c   :py:func:`final
-00006110: 697a 655f 6469 6374 600a 0a2e 2e20 6e6f  ize_dict`.... no
-00006120: 7465 3a3a 0a20 2020 2049 6620 7573 6520  te::.    If use 
-00006130: 7072 652d 7472 6169 6e65 6420 7a73 7464  pre-trained zstd
-00006140: 2064 6963 7469 6f6e 6172 792c 2074 6865   dictionary, the
-00006150: 2063 6f6d 7072 6573 7369 6f6e 2072 6174   compression rat
-00006160: 696f 2061 6368 6965 7661 626c 6520 6f6e  io achievable on
-00006170: 2073 6d61 6c6c 2064 6174 6120 2861 2066   small data (a f
-00006180: 6577 204b 6942 2920 696d 7072 6f76 6573  ew KiB) improves
-00006190: 2064 7261 6d61 7469 6361 6c6c 792e 0a0a   dramatically...
-000061a0: 2020 2020 2a2a 4261 636b 6772 6f75 6e64      **Background
-000061b0: 2a2a 0a0a 2020 2020 5468 6520 736d 616c  **..    The smal
-000061c0: 6c65 7220 7468 6520 616d 6f75 6e74 206f  ler the amount o
-000061d0: 6620 6461 7461 2074 6f20 636f 6d70 7265  f data to compre
-000061e0: 7373 2c20 7468 6520 6d6f 7265 2064 6966  ss, the more dif
-000061f0: 6669 6375 6c74 2069 7420 6973 2074 6f20  ficult it is to 
-00006200: 636f 6d70 7265 7373 2e20 5468 6973 2070  compress. This p
-00006210: 726f 626c 656d 2069 7320 636f 6d6d 6f6e  roblem is common
-00006220: 2074 6f20 616c 6c20 636f 6d70 7265 7373   to all compress
-00006230: 696f 6e20 616c 676f 7269 7468 6d73 2c20  ion algorithms, 
-00006240: 616e 6420 7265 6173 6f6e 2069 732c 2063  and reason is, c
-00006250: 6f6d 7072 6573 7369 6f6e 2061 6c67 6f72  ompression algor
-00006260: 6974 686d 7320 6c65 6172 6e20 6672 6f6d  ithms learn from
-00006270: 2070 6173 7420 6461 7461 2068 6f77 2074   past data how t
-00006280: 6f20 636f 6d70 7265 7373 2066 7574 7572  o compress futur
-00006290: 6520 6461 7461 2e20 4275 7420 6174 2074  e data. But at t
-000062a0: 6865 2062 6567 696e 6e69 6e67 206f 6620  he beginning of 
-000062b0: 6120 6e65 7720 6461 7461 2073 6574 2c20  a new data set, 
-000062c0: 7468 6572 6520 6973 206e 6f20 2270 6173  there is no "pas
-000062d0: 7422 2074 6f20 6275 696c 6420 7570 6f6e  t" to build upon
-000062e0: 2e0a 0a20 2020 205a 7374 6420 7472 6169  ...    Zstd trai
-000062f0: 6e69 6e67 206d 6f64 6520 6361 6e20 6265  ning mode can be
-00006300: 2075 7365 6420 746f 2074 756e 6520 7468   used to tune th
-00006310: 6520 616c 676f 7269 7468 6d20 666f 7220  e algorithm for 
-00006320: 6120 7365 6c65 6374 6564 2074 7970 6520  a selected type 
-00006330: 6f66 2064 6174 612e 2054 7261 696e 696e  of data. Trainin
-00006340: 6720 6973 2061 6368 6965 7665 6420 6279  g is achieved by
-00006350: 2070 726f 7669 6469 6e67 2069 7420 7769   providing it wi
-00006360: 7468 2061 2066 6577 2073 616d 706c 6573  th a few samples
-00006370: 2028 6f6e 6520 6669 6c65 2070 6572 2073   (one file per s
-00006380: 616d 706c 6529 2e20 5468 6520 7265 7375  ample). The resu
-00006390: 6c74 206f 6620 7468 6973 2074 7261 696e  lt of this train
-000063a0: 696e 6720 6973 2073 746f 7265 6420 696e  ing is stored in
-000063b0: 2061 2066 696c 6520 6361 6c6c 6564 2022   a file called "
-000063c0: 6469 6374 696f 6e61 7279 222c 2077 6869  dictionary", whi
-000063d0: 6368 206d 7573 7420 6265 206c 6f61 6465  ch must be loade
-000063e0: 6420 6265 666f 7265 2063 6f6d 7072 6573  d before compres
-000063f0: 7369 6f6e 2061 6e64 2064 6563 6f6d 7072  sion and decompr
-00006400: 6573 7369 6f6e 2e0a 0a20 2020 2053 6565  ession...    See
-00006410: 2074 6865 2046 4151 2069 6e20 6074 6869   the FAQ in `thi
-00006420: 7320 6669 6c65 203c 6874 7470 733a 2f2f  s file <https://
-00006430: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
-00006440: 6f6f 6b2f 7a73 7464 2f62 6c6f 622f 6465  ook/zstd/blob/de
-00006450: 762f 6c69 622f 7a64 6963 742e 683e 605f  v/lib/zdict.h>`_
-00006460: 2066 6f72 2064 6574 6169 6c73 2e0a 0a20   for details... 
-00006470: 2020 202e 2e20 6174 7465 6e74 696f 6e3a     .. attention:
-00006480: 3a0a 0a20 2020 2020 2020 2023 2e20 4966  :..        #. If
-00006490: 2079 6f75 206c 6f73 6520 6120 7a73 7464   you lose a zstd
-000064a0: 2064 6963 7469 6f6e 6172 792c 2074 6865   dictionary, the
-000064b0: 6e20 6361 6e27 7420 6465 636f 6d70 7265  n can't decompre
-000064c0: 7373 2074 6865 2063 6f72 7265 7370 6f6e  ss the correspon
-000064d0: 6469 6e67 2064 6174 612e 0a20 2020 2020  ding data..     
-000064e0: 2020 2023 2e20 5a73 7464 2064 6963 7469     #. Zstd dicti
-000064f0: 6f6e 6172 7920 6861 7320 6e65 676c 6967  onary has neglig
-00006500: 6962 6c65 2065 6666 6563 7420 6f6e 206c  ible effect on l
-00006510: 6172 6765 2064 6174 6120 286d 756c 7469  arge data (multi
-00006520: 2d4d 6942 2920 636f 6d70 7265 7373 696f  -MiB) compressio
-00006530: 6e2e 2049 6620 7761 6e74 2074 6f20 7573  n. If want to us
-00006540: 6520 6c61 7267 6520 6469 6374 696f 6e61  e large dictiona
-00006550: 7279 2063 6f6e 7465 6e74 2c20 7365 6520  ry content, see 
-00006560: 7072 6566 6978 283a 7079 3a61 7474 723a  prefix(:py:attr:
-00006570: 605a 7374 6444 6963 742e 6173 5f70 7265  `ZstdDict.as_pre
-00006580: 6669 7860 292e 0a20 2020 2020 2020 2023  fix`)..        #
-00006590: 2e20 5468 6572 6520 6973 2061 2070 6f73  . There is a pos
-000065a0: 7369 6269 6c69 7479 2074 6861 7420 7468  sibility that th
-000065b0: 6520 6469 6374 696f 6e61 7279 2063 6f6e  e dictionary con
-000065c0: 7465 6e74 2063 6f75 6c64 2062 6520 6d61  tent could be ma
-000065d0: 6c69 6369 6f75 736c 7920 7461 6d70 6572  liciously tamper
-000065e0: 6564 2062 7920 6120 7468 6972 6420 7061  ed by a third pa
-000065f0: 7274 792e 0a0a 2020 2020 2a2a 4164 7661  rty...    **Adva
-00006600: 6e63 6564 2064 6963 7469 6f6e 6172 7920  nced dictionary 
-00006610: 7472 6169 6e69 6e67 2a2a 0a0a 2020 2020  training**..    
-00006620: 5079 7a73 7464 206d 6f64 756c 6520 6f6e  Pyzstd module on
-00006630: 6c79 2075 7365 7320 7a73 7464 206c 6962  ly uses zstd lib
-00006640: 7261 7279 2773 2073 7461 626c 6520 4150  rary's stable AP
-00006650: 492e 2054 6865 2073 7461 626c 6520 4150  I. The stable AP
-00006660: 4920 6f6e 6c79 2065 7870 6f73 6573 2074  I only exposes t
-00006670: 776f 2064 6963 7469 6f6e 6172 7920 7472  wo dictionary tr
-00006680: 6169 6e69 6e67 2066 756e 6374 696f 6e73  aining functions
-00006690: 2074 6861 7420 636f 7272 6573 706f 6e64   that correspond
-000066a0: 696e 6720 746f 203a 7079 3a66 756e 633a  ing to :py:func:
-000066b0: 6074 7261 696e 5f64 6963 7460 2061 6e64  `train_dict` and
-000066c0: 203a 7079 3a66 756e 633a 6066 696e 616c   :py:func:`final
-000066d0: 697a 655f 6469 6374 602e 0a0a 2020 2020  ize_dict`...    
-000066e0: 4966 2077 616e 7420 746f 2061 646a 7573  If want to adjus
-000066f0: 7420 6164 7661 6e63 6564 2074 7261 696e  t advanced train
-00006700: 696e 6720 7061 7261 6d65 7465 7273 2c20  ing parameters, 
-00006710: 796f 7520 6d61 7920 7573 6520 7a73 7464  you may use zstd
-00006720: 2773 2043 4c49 2070 726f 6772 616d 2028  's CLI program (
-00006730: 6e6f 7420 7079 7a73 7464 206d 6f64 756c  not pyzstd modul
-00006740: 6527 7320 434c 4929 2c20 6974 2068 6173  e's CLI), it has
-00006750: 2065 6e74 7269 6573 2074 6f20 7a73 7464   entries to zstd
-00006760: 206c 6962 7261 7279 2773 2065 7870 6572   library's exper
-00006770: 696d 656e 7461 6c20 4150 492e 0a0a 2e2e  imental API.....
-00006780: 2070 793a 636c 6173 733a 3a20 5a73 7464   py:class:: Zstd
-00006790: 4469 6374 0a0a 2020 2020 5265 7072 6573  Dict..    Repres
-000067a0: 656e 7473 2061 207a 7374 6420 6469 6374  ents a zstd dict
-000067b0: 696f 6e61 7279 2c20 6361 6e20 6265 2075  ionary, can be u
-000067c0: 7365 6420 666f 7220 636f 6d70 7265 7373  sed for compress
-000067d0: 696f 6e2f 6465 636f 6d70 7265 7373 696f  ion/decompressio
-000067e0: 6e2e 0a0a 2020 2020 4974 2773 2074 6872  n...    It's thr
-000067f0: 6561 642d 7361 6665 2c20 616e 6420 6361  ead-safe, and ca
-00006800: 6e20 6265 2073 6861 7265 6420 6279 206d  n be shared by m
-00006810: 756c 7469 706c 6520 3a70 793a 636c 6173  ultiple :py:clas
-00006820: 733a 605a 7374 6443 6f6d 7072 6573 736f  s:`ZstdCompresso
-00006830: 7260 202f 203a 7079 3a63 6c61 7373 3a60  r` / :py:class:`
-00006840: 5a73 7464 4465 636f 6d70 7265 7373 6f72  ZstdDecompressor
-00006850: 6020 6f62 6a65 6374 732e 0a0a 2020 2020  ` objects...    
-00006860: 2e2e 2073 6f75 7263 6563 6f64 653a 3a20  .. sourcecode:: 
-00006870: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-00006880: 2320 6c6f 6164 2061 207a 7374 6420 6469  # load a zstd di
-00006890: 6374 696f 6e61 7279 2066 726f 6d20 6669  ctionary from fi
-000068a0: 6c65 0a20 2020 2020 2020 2077 6974 6820  le.        with 
-000068b0: 696f 2e6f 7065 6e28 6469 6374 5f70 6174  io.open(dict_pat
-000068c0: 682c 2027 7262 2729 2061 7320 663a 0a20  h, 'rb') as f:. 
-000068d0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-000068e0: 636f 6e74 656e 7420 3d20 662e 7265 6164  content = f.read
-000068f0: 2829 0a20 2020 2020 2020 207a 6420 3d20  ().        zd = 
-00006900: 5a73 7464 4469 6374 2866 696c 655f 636f  ZstdDict(file_co
-00006910: 6e74 656e 7429 0a0a 2020 2020 2020 2020  ntent)..        
-00006920: 2320 7573 6520 7468 6520 6469 6374 696f  # use the dictio
-00006930: 6e61 7279 2074 6f20 636f 6d70 7265 7373  nary to compress
-00006940: 2e0a 2020 2020 2020 2020 2320 6966 2075  ..        # if u
-00006950: 7365 2074 6865 2073 616d 6520 6469 6374  se the same dict
-00006960: 696f 6e61 7279 2066 6f72 2063 6f6d 7072  ionary for compr
-00006970: 6573 7369 6f6e 2072 6570 6561 7465 646c  ession repeatedl
-00006980: 792c 2072 6575 7369 6e67 0a20 2020 2020  y, reusing.     
-00006990: 2020 2023 2061 2063 6f6d 7072 6573 736f     # a compresso
-000069a0: 7220 6f62 6a65 6374 2069 7320 6661 7374  r object is fast
-000069b0: 6572 2c20 7365 6520 2e61 735f 756e 6469  er, see .as_undi
-000069c0: 6765 7374 6564 5f64 6963 7420 646f 632e  gested_dict doc.
-000069d0: 0a20 2020 2020 2020 2063 6f6d 7072 6573  .        compres
-000069e0: 7365 645f 6461 7420 3d20 636f 6d70 7265  sed_dat = compre
-000069f0: 7373 2872 6177 5f64 6174 2c20 7a73 7464  ss(raw_dat, zstd
-00006a00: 5f64 6963 743d 7a64 290a 0a20 2020 2020  _dict=zd)..     
-00006a10: 2020 2023 2075 7365 2074 6865 2064 6963     # use the dic
-00006a20: 7469 6f6e 6172 7920 746f 2064 6563 6f6d  tionary to decom
-00006a30: 7072 6573 730a 2020 2020 2020 2020 6465  press.        de
-00006a40: 636f 6d70 7265 7373 6564 5f64 6174 203d  compressed_dat =
-00006a50: 2064 6563 6f6d 7072 6573 7328 636f 6d70   decompress(comp
-00006a60: 7265 7373 6564 5f64 6174 2c20 7a73 7464  ressed_dat, zstd
-00006a70: 5f64 6963 743d 7a64 290a 0a20 2020 202e  _dict=zd)..    .
-00006a80: 2e20 7665 7273 696f 6e63 6861 6e67 6564  . versionchanged
-00006a90: 3a3a 2030 2e31 352e 370a 2020 2020 2020  :: 0.15.7.      
-00006aa0: 2020 5768 656e 2063 6f6d 7072 6573 7369    When compressi
-00006ab0: 6e67 2c20 6c6f 6164 2075 6e64 6967 6573  ng, load undiges
-00006ac0: 7465 6420 6469 6374 696f 6e61 7279 2069  ted dictionary i
-00006ad0: 6e73 7465 6164 206f 6620 6469 6765 7374  nstead of digest
-00006ae0: 6564 2064 6963 7469 6f6e 6172 7920 6279  ed dictionary by
-00006af0: 2064 6566 6175 6c74 2c20 7365 6520 3a70   default, see :p
-00006b00: 793a 6174 7472 3a60 7e5a 7374 6444 6963  y:attr:`~ZstdDic
-00006b10: 742e 6173 5f64 6967 6573 7465 645f 6469  t.as_digested_di
-00006b20: 6374 602e 2041 6c73 6f20 6164 6420 6060  ct`. Also add ``
-00006b30: 2e5f 5f6c 656e 5f5f 2829 6060 206d 6574  .__len__()`` met
-00006b40: 686f 6420 7468 6174 2072 6574 7572 6e69  hod that returni
-00006b50: 6e67 2063 6f6e 7465 6e74 2073 697a 652e  ng content size.
-00006b60: 0a0a 2020 2020 2e2e 2070 793a 6d65 7468  ..    .. py:meth
-00006b70: 6f64 3a3a 205f 5f69 6e69 745f 5f28 7365  od:: __init__(se
-00006b80: 6c66 2c20 6469 6374 5f63 6f6e 7465 6e74  lf, dict_content
-00006b90: 2c20 6973 5f72 6177 3d46 616c 7365 290a  , is_raw=False).
-00006ba0: 0a20 2020 2020 2020 2049 6e69 7469 616c  .        Initial
-00006bb0: 697a 6520 6120 5a73 7464 4469 6374 206f  ize a ZstdDict o
-00006bc0: 626a 6563 742e 0a0a 2020 2020 2020 2020  bject...        
-00006bd0: 3a70 6172 616d 2064 6963 745f 636f 6e74  :param dict_cont
-00006be0: 656e 743a 2044 6963 7469 6f6e 6172 7927  ent: Dictionary'
-00006bf0: 7320 636f 6e74 656e 742e 0a20 2020 2020  s content..     
-00006c00: 2020 203a 7479 7065 2064 6963 745f 636f     :type dict_co
-00006c10: 6e74 656e 743a 2062 7974 6573 2d6c 696b  ntent: bytes-lik
-00006c20: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
-00006c30: 203a 7061 7261 6d20 6973 5f72 6177 3a20   :param is_raw: 
-00006c40: 5468 6973 2070 6172 616d 6574 6572 2069  This parameter i
-00006c50: 7320 666f 7220 6164 7661 6e63 6564 2075  s for advanced u
-00006c60: 7365 722e 2060 6054 7275 6560 6020 6d65  ser. ``True`` me
-00006c70: 616e 7320 2a64 6963 745f 636f 6e74 656e  ans *dict_conten
-00006c80: 742a 2061 7267 756d 656e 7420 6973 2061  t* argument is a
-00006c90: 2022 7261 7720 636f 6e74 656e 7422 2064   "raw content" d
-00006ca0: 6963 7469 6f6e 6172 792c 2066 7265 6520  ictionary, free 
-00006cb0: 6f66 2061 6e79 2066 6f72 6d61 7420 7265  of any format re
-00006cc0: 7374 7269 6374 696f 6e2e 2060 6046 616c  striction. ``Fal
-00006cd0: 7365 6060 206d 6561 6e73 202a 6469 6374  se`` means *dict
-00006ce0: 5f63 6f6e 7465 6e74 2a20 6172 6775 6d65  _content* argume
-00006cf0: 6e74 2069 7320 616e 206f 7264 696e 6172  nt is an ordinar
-00006d00: 7920 7a73 7464 2064 6963 7469 6f6e 6172  y zstd dictionar
-00006d10: 792c 2077 6173 2063 7265 6174 6564 2062  y, was created b
-00006d20: 7920 7a73 7464 2066 756e 6374 696f 6e73  y zstd functions
-00006d30: 2c20 666f 6c6c 6f77 2061 2073 7065 6369  , follow a speci
-00006d40: 6669 6564 2066 6f72 6d61 742e 0a20 2020  fied format..   
-00006d50: 2020 2020 203a 7479 7065 2069 735f 7261       :type is_ra
-00006d60: 773a 2062 6f6f 6c0a 0a20 2020 202e 2e20  w: bool..    .. 
-00006d70: 7079 3a61 7474 7269 6275 7465 3a3a 2064  py:attribute:: d
-00006d80: 6963 745f 636f 6e74 656e 740a 0a20 2020  ict_content..   
-00006d90: 2020 2020 2054 6865 2063 6f6e 7465 6e74       The content
-00006da0: 206f 6620 7a73 7464 2064 6963 7469 6f6e   of zstd diction
-00006db0: 6172 792c 2061 2060 6062 7974 6573 6060  ary, a ``bytes``
-00006dc0: 206f 626a 6563 742e 2049 7427 7320 7468   object. It's th
-00006dd0: 6520 7361 6d65 2061 7320 2a64 6963 745f  e same as *dict_
-00006de0: 636f 6e74 656e 742a 2061 7267 756d 656e  content* argumen
-00006df0: 7420 696e 203a 7079 3a6d 6574 683a 607e  t in :py:meth:`~
-00006e00: 5a73 7464 4469 6374 2e5f 5f69 6e69 745f  ZstdDict.__init_
-00006e10: 5f60 206d 6574 686f 642e 2049 7420 6361  _` method. It ca
-00006e20: 6e20 6265 2075 7365 6420 7769 7468 206f  n be used with o
-00006e30: 7468 6572 2070 726f 6772 616d 732e 0a0a  ther programs...
-00006e40: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
-00006e50: 7574 653a 3a20 6469 6374 5f69 640a 0a20  ute:: dict_id.. 
-00006e60: 2020 2020 2020 2049 4420 6f66 207a 7374         ID of zst
-00006e70: 6420 6469 6374 696f 6e61 7279 2c20 6120  d dictionary, a 
-00006e80: 3332 2d62 6974 2075 6e73 6967 6e65 6420  32-bit unsigned 
-00006e90: 696e 7465 6765 7220 7661 6c75 652e 2053  integer value. S
-00006ea0: 6565 203a 7265 663a 6074 6869 7320 6e6f  ee :ref:`this no
-00006eb0: 7465 3c64 6963 745f 6964 3e60 2066 6f72  te<dict_id>` for
-00006ec0: 2064 6574 6169 6c73 2e0a 0a20 2020 2020   details...     
-00006ed0: 2020 204e 6f6e 2d7a 6572 6f20 6d65 616e     Non-zero mean
-00006ee0: 7320 6f72 6469 6e61 7279 2064 6963 7469  s ordinary dicti
-00006ef0: 6f6e 6172 792c 2077 6173 2063 7265 6174  onary, was creat
-00006f00: 6564 2062 7920 7a73 7464 2066 756e 6374  ed by zstd funct
-00006f10: 696f 6e73 2c20 666f 6c6c 6f77 2061 2073  ions, follow a s
-00006f20: 7065 6369 6669 6564 2066 6f72 6d61 742e  pecified format.
-00006f30: 0a0a 2020 2020 2020 2020 6060 3060 6020  ..        ``0`` 
-00006f40: 6d65 616e 7320 6120 2272 6177 2063 6f6e  means a "raw con
-00006f50: 7465 6e74 2220 6469 6374 696f 6e61 7279  tent" dictionary
-00006f60: 2c20 6672 6565 206f 6620 616e 7920 666f  , free of any fo
-00006f70: 726d 6174 2072 6573 7472 6963 7469 6f6e  rmat restriction
-00006f80: 2c20 7573 6564 2066 6f72 2061 6476 616e  , used for advan
-00006f90: 6365 6420 7573 6572 2e20 284e 6f74 6520  ced user. (Note 
-00006fa0: 7468 6174 2074 6865 206d 6561 6e69 6e67  that the meaning
-00006fb0: 206f 6620 6060 3060 6020 6973 2064 6966   of ``0`` is dif
-00006fc0: 6665 7265 6e74 2066 726f 6d20 6060 6469  ferent from ``di
-00006fd0: 6374 696f 6e61 7279 5f69 6460 6020 696e  ctionary_id`` in
-00006fe0: 203a 7079 3a66 756e 633a 6067 6574 5f66   :py:func:`get_f
-00006ff0: 7261 6d65 5f69 6e66 6f60 2066 756e 6374  rame_info` funct
-00007000: 696f 6e2e 290a 0a20 2020 202e 2e20 7079  ion.)..    .. py
-00007010: 3a61 7474 7269 6275 7465 3a3a 2061 735f  :attribute:: as_
-00007020: 6469 6765 7374 6564 5f64 6963 740a 0a20  digested_dict.. 
-00007030: 2020 2020 2020 204c 6f61 6420 6173 2061         Load as a
-00007040: 2064 6967 6573 7465 6420 6469 6374 696f   digested dictio
-00007050: 6e61 7279 2c20 7365 6520 6265 6c6f 772e  nary, see below.
-00007060: 0a0a 2020 2020 2020 2020 2e2e 2076 6572  ..        .. ver
-00007070: 7369 6f6e 6164 6465 643a 3a20 302e 3135  sionadded:: 0.15
-00007080: 2e37 0a0a 2020 2020 2e2e 2070 793a 6174  .7..    .. py:at
-00007090: 7472 6962 7574 653a 3a20 6173 5f75 6e64  tribute:: as_und
-000070a0: 6967 6573 7465 645f 6469 6374 0a0a 2020  igested_dict..  
-000070b0: 2020 2020 2020 4c6f 6164 2061 7320 616e        Load as an
-000070c0: 2075 6e64 6967 6573 7465 6420 6469 6374   undigested dict
-000070d0: 696f 6e61 7279 2e0a 0a20 2020 2020 2020  ionary...       
-000070e0: 2044 6967 6573 7469 6e67 2064 6963 7469   Digesting dicti
-000070f0: 6f6e 6172 7920 6973 2061 2063 6f73 746c  onary is a costl
-00007100: 7920 6f70 6572 6174 696f 6e2e 2054 6865  y operation. The
-00007110: 7365 2074 776f 2061 7474 7269 6275 7465  se two attribute
-00007120: 7320 6361 6e20 636f 6e74 726f 6c20 686f  s can control ho
-00007130: 7720 7468 6520 6469 6374 696f 6e61 7279  w the dictionary
-00007140: 2069 7320 6c6f 6164 6564 2074 6f20 636f   is loaded to co
-00007150: 6d70 7265 7373 6f72 2c20 6279 2070 6173  mpressor, by pas
-00007160: 7369 6e67 2074 6865 6d20 6173 2060 7a73  sing them as `zs
-00007170: 7464 5f64 6963 7460 2061 7267 756d 656e  td_dict` argumen
-00007180: 743a 2060 6063 6f6d 7072 6573 7328 6461  t: ``compress(da
-00007190: 742c 207a 7374 645f 6469 6374 3d7a 642e  t, zstd_dict=zd.
-000071a0: 6173 5f64 6967 6573 7465 645f 6469 6374  as_digested_dict
-000071b0: 2960 600a 0a20 2020 2020 2020 2049 6620  )``..        If 
-000071c0: 646f 6e27 7420 7370 6563 6966 7920 7468  don't specify th
-000071d0: 6573 6520 7477 6f20 6174 7472 6962 7574  ese two attribut
-000071e0: 6573 2c20 7573 6520 2a2a 756e 6469 6765  es, use **undige
-000071f0: 7374 6564 2a2a 2064 6963 7469 6f6e 6172  sted** dictionar
-00007200: 7920 666f 7220 636f 6d70 7265 7373 696f  y for compressio
-00007210: 6e20 6279 2064 6566 6175 6c74 3a20 6060  n by default: ``
-00007220: 636f 6d70 7265 7373 2864 6174 2c20 7a73  compress(dat, zs
-00007230: 7464 5f64 6963 743d 7a64 2960 600a 0a20  td_dict=zd)``.. 
-00007240: 2020 2020 2020 202e 2e20 6c69 7374 2d74         .. list-t
-00007250: 6162 6c65 3a3a 2044 6966 6665 7265 6e63  able:: Differenc
-00007260: 6520 666f 7220 636f 6d70 7265 7373 696f  e for compressio
-00007270: 6e0a 2020 2020 2020 2020 2020 2020 3a77  n.            :w
-00007280: 6964 7468 733a 2031 3220 3132 2031 320a  idths: 12 12 12.
-00007290: 2020 2020 2020 2020 2020 2020 3a68 6561              :hea
-000072a0: 6465 722d 726f 7773 3a20 310a 0a20 2020  der-rows: 1..   
-000072b0: 2020 2020 2020 2020 202a 202d 0a20 2020           * -.   
-000072c0: 2020 2020 2020 2020 2020 202d 207c 2044             - | D
-000072d0: 6967 6573 7465 640a 2020 2020 2020 2020  igested.        
-000072e0: 2020 2020 2020 2020 7c20 6469 6374 696f          | dictio
-000072f0: 6e61 7279 0a20 2020 2020 2020 2020 2020  nary.           
-00007300: 2020 202d 207c 2055 6e64 6967 6573 7465     - | Undigeste
-00007310: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00007320: 2020 7c20 6469 6374 696f 6e61 7279 0a20    | dictionary. 
-00007330: 2020 2020 2020 2020 2020 202a 202d 207c             * - |
-00007340: 2053 6f6d 6520 6164 7661 6e63 6564 0a20   Some advanced. 
-00007350: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007360: 2070 6172 616d 6574 6572 7320 6f66 0a20   parameters of. 
-00007370: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007380: 2063 6f6d 7072 6573 736f 7220 6d61 790a   compressor may.
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073a0: 7c20 6265 206f 7665 7272 6964 6465 6e0a  | be overridden.
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 7c20 6279 2064 6963 7469 6f6e 6172 7927  | by dictionary'
-000073d0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-000073e0: 2020 7c20 7061 7261 6d65 7465 7273 0a20    | parameters. 
-000073f0: 2020 2020 2020 2020 2020 2020 202d 207c               - |
-00007400: 2060 6077 696e 646f 774c 6f67 6060 2c20   ``windowLog``, 
-00007410: 6060 6861 7368 4c6f 6760 602c 0a20 2020  ``hashLog``,.   
-00007420: 2020 2020 2020 2020 2020 2020 207c 2060               | `
-00007430: 6063 6861 696e 4c6f 6760 602c 2060 6073  `chainLog``, ``s
-00007440: 6561 7263 684c 6f67 6060 2c0a 2020 2020  earchLog``,.    
-00007450: 2020 2020 2020 2020 2020 2020 7c20 6060              | ``
-00007460: 6d69 6e4d 6174 6368 6060 2c20 6060 7461  minMatch``, ``ta
-00007470: 7267 6574 4c65 6e67 7468 6060 2c0a 2020  rgetLength``,.  
-00007480: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00007490: 6060 7374 7261 7465 6779 6060 2c0a 2020  ``strategy``,.  
-000074a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000074b0: 6060 656e 6162 6c65 4c6f 6e67 4469 7374  ``enableLongDist
-000074c0: 616e 6365 4d61 7463 6869 6e67 6060 2c0a  anceMatching``,.
-000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074e0: 7c20 6060 6c64 6d48 6173 684c 6f67 6060  | ``ldmHashLog``
-000074f0: 2c20 6060 6c64 6d4d 696e 4d61 7463 6860  , ``ldmMinMatch`
-00007500: 602c 0a20 2020 2020 2020 2020 2020 2020  `,.             
-00007510: 2020 207c 2060 606c 646d 4275 636b 6574     | ``ldmBucket
-00007520: 5369 7a65 4c6f 6760 602c 0a20 2020 2020  SizeLog``,.     
-00007530: 2020 2020 2020 2020 2020 207c 2060 606c             | ``l
-00007540: 646d 4861 7368 5261 7465 4c6f 6760 602c  dmHashRateLog``,
-00007550: 2061 6e64 2073 6f6d 650a 2020 2020 2020   and some.      
-00007560: 2020 2020 2020 2020 2020 7c20 6e6f 6e2d            | non-
-00007570: 7075 626c 6963 2070 6172 616d 6574 6572  public parameter
-00007580: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-00007590: 202d 204e 6f0a 2020 2020 2020 2020 2020   - No.          
-000075a0: 2020 2a20 2d20 7c20 5a73 7464 4469 6374    * - | ZstdDict
-000075b0: 2068 6173 0a20 2020 2020 2020 2020 2020   has.           
-000075c0: 2020 2020 207c 2069 6e74 6572 6e61 6c20       | internal 
-000075d0: 6361 6368 650a 2020 2020 2020 2020 2020  cache.          
-000075e0: 2020 2020 2020 7c20 666f 7220 7468 6973        | for this
-000075f0: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
-00007600: 207c 2059 6573 2e20 4974 2773 2066 6173   | Yes. It's fas
-00007610: 7465 7220 7768 656e 0a20 2020 2020 2020  ter when.       
-00007620: 2020 2020 2020 2020 207c 206c 6f61 6469           | loadi
-00007630: 6e67 2061 6761 696e 2061 2064 6967 6573  ng again a diges
-00007640: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
-00007650: 2020 2020 7c20 6469 6374 696f 6e61 7279      | dictionary
-00007660: 2077 6974 6820 7468 6520 7361 6d65 0a20   with the same. 
-00007670: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007680: 2063 6f6d 7072 6573 7369 6f6e 206c 6576   compression lev
-00007690: 656c 2e0a 2020 2020 2020 2020 2020 2020  el..            
-000076a0: 2020 2d20 7c20 4e6f 2e20 4966 206c 6f61    - | No. If loa
-000076b0: 6420 616e 2075 6e64 6967 6573 7465 640a  d an undigested.
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 7c20 6469 6374 696f 6e61 7279 206d 756c  | dictionary mul
-000076e0: 7469 706c 6520 7469 6d65 732c 0a20 2020  tiple times,.   
-000076f0: 2020 2020 2020 2020 2020 2020 207c 2063               | c
-00007700: 6f6e 7369 6465 7220 7265 7573 696e 6720  onsider reusing 
-00007710: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-00007720: 2020 7c20 636f 6d70 7265 7373 6f72 206f    | compressor o
-00007730: 626a 6563 742e 0a0a 2020 2020 2020 2020  bject...        
-00007740: 466f 7220 6465 636f 6d70 7265 7373 696f  For decompressio
-00007750: 6e2c 2074 6865 7920 6861 7665 2074 6865  n, they have the
-00007760: 2073 616d 6520 6566 6665 6374 2e20 5079   same effect. Py
-00007770: 7a73 7464 2075 7365 7320 2a2a 6469 6765  zstd uses **dige
-00007780: 7374 6564 2a2a 2064 6963 7469 6f6e 6172  sted** dictionar
-00007790: 7920 666f 7220 6465 636f 6d70 7265 7373  y for decompress
-000077a0: 696f 6e20 6279 2064 6566 6175 6c74 2c20  ion by default, 
-000077b0: 7768 6963 6820 6973 2066 6173 7465 7220  which is faster 
-000077c0: 7768 656e 206c 6f61 6469 6e67 2061 6761  when loading aga
-000077d0: 696e 3a20 6060 6465 636f 6d70 7265 7373  in: ``decompress
-000077e0: 2864 6174 2c20 7a73 7464 5f64 6963 743d  (dat, zstd_dict=
-000077f0: 7a64 2960 600a 0a20 2020 2020 2020 202e  zd)``..        .
-00007800: 2e20 7665 7273 696f 6e61 6464 6564 3a3a  . versionadded::
-00007810: 2030 2e31 352e 370a 0a20 2020 202e 2e20   0.15.7..    .. 
-00007820: 7079 3a61 7474 7269 6275 7465 3a3a 2061  py:attribute:: a
-00007830: 735f 7072 6566 6978 0a0a 2020 2020 2020  s_prefix..      
-00007840: 2020 4c6f 6164 2074 6865 2064 6963 7469    Load the dicti
-00007850: 6f6e 6172 7920 636f 6e74 656e 7420 746f  onary content to
-00007860: 2063 6f6d 7072 6573 736f 722f 6465 636f   compressor/deco
-00007870: 6d70 7265 7373 6f72 2061 7320 6120 2270  mpressor as a "p
-00007880: 7265 6669 7822 2c20 6279 2070 6173 7369  refix", by passi
-00007890: 6e67 2074 6869 7320 6174 7472 6962 7574  ng this attribut
-000078a0: 6520 6173 2060 7a73 7464 5f64 6963 7460  e as `zstd_dict`
-000078b0: 2061 7267 756d 656e 743a 2060 6063 6f6d   argument: ``com
-000078c0: 7072 6573 7328 6461 742c 207a 7374 645f  press(dat, zstd_
-000078d0: 6469 6374 3d7a 642e 6173 5f70 7265 6669  dict=zd.as_prefi
-000078e0: 7829 6060 0a0a 2020 2020 2020 2020 5072  x)``..        Pr
-000078f0: 6566 6978 2063 616e 2062 6520 7573 6564  efix can be used
-00007900: 2066 6f72 203a 7265 663a 6070 6174 6368   for :ref:`patch
-00007910: 696e 6720 656e 6769 6e65 3c70 6174 6368  ing engine<patch
-00007920: 696e 675f 656e 6769 6e65 3e60 2073 6365  ing_engine>` sce
-00007930: 6e61 7269 6f2e 0a0a 2020 2020 2020 2020  nario...        
-00007940: 232e 2050 7265 6669 7820 6973 2063 6f6d  #. Prefix is com
-00007950: 7061 7469 626c 6520 7769 7468 2022 6c6f  patible with "lo
-00007960: 6e67 2064 6973 7461 6e63 6520 6d61 7463  ng distance matc
-00007970: 6869 6e67 222c 2077 6869 6c65 2064 6963  hing", while dic
-00007980: 7469 6f6e 6172 7920 6973 206e 6f74 2e0a  tionary is not..
-00007990: 2020 2020 2020 2020 232e 2050 7265 6669          #. Prefi
-000079a0: 7820 6f6e 6c79 2077 6f72 6b20 666f 7220  x only work for 
-000079b0: 7468 6520 6669 7273 7420 6672 616d 652c  the first frame,
-000079c0: 2074 6865 6e20 7468 6520 636f 6d70 7265   then the compre
-000079d0: 7373 6f72 2f64 6563 6f6d 7072 6573 736f  ssor/decompresso
-000079e0: 7220 7769 6c6c 2072 6574 7572 6e20 746f  r will return to
-000079f0: 206e 6f20 7072 6566 6978 2073 7461 7465   no prefix state
-00007a00: 2e20 5468 6973 2069 7320 6469 6666 6572  . This is differ
-00007a10: 656e 7420 6672 6f6d 2064 6963 7469 6f6e  ent from diction
-00007a20: 6172 7920 7468 6174 2063 616e 2062 6520  ary that can be 
-00007a30: 7573 6564 2066 6f72 2061 6c6c 2073 7562  used for all sub
-00007a40: 7365 7175 656e 7420 6672 616d 6573 2e0a  sequent frames..
-00007a50: 2020 2020 2020 2020 232e 2057 6865 6e20          #. When 
-00007a60: 6465 636f 6d70 7265 7373 696e 672c 206d  decompressing, m
-00007a70: 7573 7420 7573 6520 7468 6520 7361 6d65  ust use the same
-00007a80: 2070 7265 6669 7820 6173 2077 6865 6e20   prefix as when 
-00007a90: 636f 6d70 7265 7373 696e 672e 0a20 2020  compressing..   
-00007aa0: 2020 2020 2023 2e20 4c6f 6164 696e 6720       #. Loading 
-00007ab0: 7072 6566 6978 2074 6f20 636f 6d70 7265  prefix to compre
-00007ac0: 7373 6f72 2069 7320 636f 7374 6c79 2e0a  ssor is costly..
-00007ad0: 2020 2020 2020 2020 232e 204c 6f61 6469          #. Loadi
-00007ae0: 6e67 2070 7265 6669 7820 746f 2064 6563  ng prefix to dec
-00007af0: 6f6d 7072 6573 736f 7220 6973 206e 6f74  ompressor is not
-00007b00: 2063 6f73 746c 792e 0a0a 2020 2020 2020   costly...      
-00007b10: 2020 2e2e 2076 6572 7369 6f6e 6164 6465    .. versionadde
-00007b20: 643a 3a20 302e 3135 2e37 0a0a 0a2e 2e20  d:: 0.15.7..... 
-00007b30: 7079 3a66 756e 6374 696f 6e3a 3a20 7472  py:function:: tr
-00007b40: 6169 6e5f 6469 6374 2873 616d 706c 6573  ain_dict(samples
-00007b50: 2c20 6469 6374 5f73 697a 6529 0a0a 2020  , dict_size)..  
-00007b60: 2020 5472 6169 6e20 6120 7a73 7464 2064    Train a zstd d
-00007b70: 6963 7469 6f6e 6172 792e 0a0a 2020 2020  ictionary...    
-00007b80: 5365 6520 7468 6520 4641 5120 696e 2060  See the FAQ in `
-00007b90: 7468 6973 2066 696c 6520 3c68 7474 7073  this file <https
-00007ba0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
-00007bb0: 6365 626f 6f6b 2f7a 7374 642f 626c 6f62  cebook/zstd/blob
-00007bc0: 2f72 656c 6561 7365 2f6c 6962 2f7a 6469  /release/lib/zdi
-00007bd0: 6374 2e68 3e60 5f20 666f 7220 6465 7461  ct.h>`_ for deta
-00007be0: 696c 732e 0a0a 2020 2020 3a70 6172 616d  ils...    :param
-00007bf0: 2073 616d 706c 6573 3a20 416e 2069 7465   samples: An ite
-00007c00: 7261 626c 6520 6f66 2073 616d 706c 6573  rable of samples
-00007c10: 2c20 6120 7361 6d70 6c65 2069 7320 6120  , a sample is a 
-00007c20: 6279 7465 732d 6c69 6b65 206f 626a 6563  bytes-like objec
-00007c30: 7420 7265 7072 6573 656e 7473 2061 2066  t represents a f
-00007c40: 696c 652e 0a20 2020 203a 7479 7065 2073  ile..    :type s
-00007c50: 616d 706c 6573 3a20 6974 6572 6162 6c65  amples: iterable
-00007c60: 0a20 2020 203a 7061 7261 6d20 696e 7420  .    :param int 
-00007c70: 6469 6374 5f73 697a 653a 2052 6574 7572  dict_size: Retur
-00007c80: 6e65 6420 7a73 7464 2064 6963 7469 6f6e  ned zstd diction
-00007c90: 6172 7927 7320 2a2a 6d61 7869 6d75 6d2a  ary's **maximum*
-00007ca0: 2a20 7369 7a65 2c20 696e 2062 7974 6573  * size, in bytes
-00007cb0: 2e0a 2020 2020 3a72 6574 7572 6e3a 2054  ..    :return: T
-00007cc0: 7261 696e 6564 207a 7374 6420 6469 6374  rained zstd dict
-00007cd0: 696f 6e61 7279 2e20 4966 2077 616e 7420  ionary. If want 
-00007ce0: 746f 2073 6176 6520 7468 6520 6469 6374  to save the dict
-00007cf0: 696f 6e61 7279 2074 6f20 6120 6669 6c65  ionary to a file
-00007d00: 2c20 7361 7665 2074 6865 203a 7079 3a61  , save the :py:a
-00007d10: 7474 723a 605a 7374 6444 6963 742e 6469  ttr:`ZstdDict.di
-00007d20: 6374 5f63 6f6e 7465 6e74 6020 6174 7472  ct_content` attr
-00007d30: 6962 7574 652e 0a20 2020 203a 7274 7970  ibute..    :rtyp
-00007d40: 653a 205a 7374 6444 6963 740a 0a20 2020  e: ZstdDict..   
-00007d50: 202e 2e20 736f 7572 6365 636f 6465 3a3a   .. sourcecode::
-00007d60: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
-00007d70: 2064 6566 2073 616d 706c 6573 2829 3a0a   def samples():.
-00007d80: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00007d90: 6469 7220 3d20 7222 453a 5c64 6174 6122  dir = r"E:\data"
-00007da0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00007db0: 4e6f 7465 2074 6861 7420 7468 6520 6f72  Note that the or
-00007dc0: 6465 7220 6f66 2074 6865 2066 696c 6573  der of the files
-00007dd0: 206d 6179 2062 6520 6469 6666 6572 656e   may be differen
-00007de0: 742c 0a20 2020 2020 2020 2020 2020 2023  t,.            #
-00007df0: 2074 6865 7265 666f 7265 2074 6865 2067   therefore the g
-00007e00: 656e 6572 6174 6564 2064 6963 7469 6f6e  enerated diction
-00007e10: 6172 7920 6d61 7920 6265 2064 6966 6665  ary may be diffe
-00007e20: 7265 6e74 2e0a 2020 2020 2020 2020 2020  rent..          
-00007e30: 2020 666f 7220 7061 7265 6e74 2c20 6469    for parent, di
-00007e40: 726e 616d 6573 2c20 6669 6c65 6e61 6d65  rnames, filename
-00007e50: 7320 696e 206f 732e 7761 6c6b 2872 6f6f  s in os.walk(roo
-00007e60: 7464 6972 293a 0a20 2020 2020 2020 2020  tdir):.         
-00007e70: 2020 2020 2020 2066 6f72 2066 696c 656e         for filen
-00007e80: 616d 6520 696e 2066 696c 656e 616d 6573  ame in filenames
-00007e90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007ea0: 2020 2020 2020 7061 7468 203d 206f 732e        path = os.
-00007eb0: 7061 7468 2e6a 6f69 6e28 7061 7265 6e74  path.join(parent
-00007ec0: 2c20 6669 6c65 6e61 6d65 290a 2020 2020  , filename).    
-00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 7769 7468 2069 6f2e 6f70 656e 2870 6174  with io.open(pat
-00007ef0: 682c 2027 7262 2729 2061 7320 663a 0a20  h, 'rb') as f:. 
-00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f10: 2020 2020 2020 2064 6174 203d 2066 2e72         dat = f.r
-00007f20: 6561 6428 290a 2020 2020 2020 2020 2020  ead().          
-00007f30: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-00007f40: 6461 740a 0a20 2020 2020 2020 2064 6963  dat..        dic
-00007f50: 203d 2070 797a 7374 642e 7472 6169 6e5f   = pyzstd.train_
-00007f60: 6469 6374 2873 616d 706c 6573 2829 2c20  dict(samples(), 
-00007f70: 3130 302a 3130 3234 290a 0a2e 2e20 7079  100*1024).... py
-00007f80: 3a66 756e 6374 696f 6e3a 3a20 6669 6e61  :function:: fina
-00007f90: 6c69 7a65 5f64 6963 7428 7a73 7464 5f64  lize_dict(zstd_d
-00007fa0: 6963 742c 2073 616d 706c 6573 2c20 6469  ict, samples, di
-00007fb0: 6374 5f73 697a 652c 206c 6576 656c 290a  ct_size, level).
-00007fc0: 0a20 2020 2047 6976 656e 2061 2063 7573  .    Given a cus
-00007fd0: 746f 6d20 636f 6e74 656e 7420 6173 2061  tom content as a
-00007fe0: 2062 6173 6973 2066 6f72 2064 6963 7469   basis for dicti
-00007ff0: 6f6e 6172 792c 2061 6e64 2061 2073 6574  onary, and a set
-00008000: 206f 6620 7361 6d70 6c65 732c 2066 696e   of samples, fin
-00008010: 616c 697a 6520 6469 6374 696f 6e61 7279  alize dictionary
-00008020: 2062 7920 6164 6469 6e67 2068 6561 6465   by adding heade
-00008030: 7273 2061 6e64 2073 7461 7469 7374 6963  rs and statistic
-00008040: 7320 6163 636f 7264 696e 6720 746f 2074  s according to t
-00008050: 6865 207a 7374 6420 6469 6374 696f 6e61  he zstd dictiona
-00008060: 7279 2066 6f72 6d61 742e 0a0a 2020 2020  ry format...    
-00008070: 5365 6520 7468 6520 4641 5120 696e 2060  See the FAQ in `
-00008080: 7468 6973 2066 696c 6520 3c68 7474 7073  this file <https
-00008090: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
-000080a0: 6365 626f 6f6b 2f7a 7374 642f 626c 6f62  cebook/zstd/blob
-000080b0: 2f72 656c 6561 7365 2f6c 6962 2f7a 6469  /release/lib/zdi
-000080c0: 6374 2e68 3e60 5f20 666f 7220 6465 7461  ct.h>`_ for deta
-000080d0: 696c 732e 0a0a 2020 2020 3a70 6172 616d  ils...    :param
-000080e0: 207a 7374 645f 6469 6374 3a20 4120 6261   zstd_dict: A ba
-000080f0: 7369 7320 6469 6374 696f 6e61 7279 2e0a  sis dictionary..
-00008100: 2020 2020 3a74 7970 6520 7a73 7464 5f64      :type zstd_d
-00008110: 6963 743a 205a 7374 6444 6963 740a 2020  ict: ZstdDict.  
-00008120: 2020 3a70 6172 616d 2073 616d 706c 6573    :param samples
-00008130: 3a20 416e 2069 7465 7261 626c 6520 6f66  : An iterable of
-00008140: 2073 616d 706c 6573 2c20 6120 7361 6d70   samples, a samp
-00008150: 6c65 2069 7320 6120 6279 7465 732d 6c69  le is a bytes-li
-00008160: 6b65 206f 626a 6563 7420 7265 7072 6573  ke object repres
-00008170: 656e 7473 2061 2066 696c 652e 0a20 2020  ents a file..   
-00008180: 203a 7479 7065 2073 616d 706c 6573 3a20   :type samples: 
-00008190: 6974 6572 6162 6c65 0a20 2020 203a 7061  iterable.    :pa
-000081a0: 7261 6d20 696e 7420 6469 6374 5f73 697a  ram int dict_siz
-000081b0: 653a 2052 6574 7572 6e65 6420 7a73 7464  e: Returned zstd
-000081c0: 2064 6963 7469 6f6e 6172 7927 7320 2a2a   dictionary's **
-000081d0: 6d61 7869 6d75 6d2a 2a20 7369 7a65 2c20  maximum** size, 
-000081e0: 696e 2062 7974 6573 2e0a 2020 2020 3a70  in bytes..    :p
-000081f0: 6172 616d 2069 6e74 206c 6576 656c 3a20  aram int level: 
-00008200: 5468 6520 636f 6d70 7265 7373 696f 6e20  The compression 
-00008210: 6c65 7665 6c20 6578 7065 6374 6564 2074  level expected t
-00008220: 6f20 7573 6520 696e 2070 726f 6475 6374  o use in product
-00008230: 696f 6e2e 2054 6865 2073 7461 7469 7374  ion. The statist
-00008240: 6963 7320 666f 7220 6561 6368 2063 6f6d  ics for each com
-00008250: 7072 6573 7369 6f6e 206c 6576 656c 2064  pression level d
-00008260: 6966 6665 722c 2073 6f20 7475 6e69 6e67  iffer, so tuning
-00008270: 2074 6865 2064 6963 7469 6f6e 6172 7920   the dictionary 
-00008280: 666f 7220 7468 6520 636f 6d70 7265 7373  for the compress
-00008290: 696f 6e20 6c65 7665 6c20 6361 6e20 6865  ion level can he
-000082a0: 6c70 2071 7569 7465 2061 2062 6974 2e0a  lp quite a bit..
-000082b0: 2020 2020 3a72 6574 7572 6e3a 2046 696e      :return: Fin
-000082c0: 616c 697a 6564 207a 7374 6420 6469 6374  alized zstd dict
-000082d0: 696f 6e61 7279 2e20 4966 2077 616e 7420  ionary. If want 
-000082e0: 746f 2073 6176 6520 7468 6520 6469 6374  to save the dict
-000082f0: 696f 6e61 7279 2074 6f20 6120 6669 6c65  ionary to a file
-00008300: 2c20 7361 7665 2074 6865 203a 7079 3a61  , save the :py:a
-00008310: 7474 723a 605a 7374 6444 6963 742e 6469  ttr:`ZstdDict.di
-00008320: 6374 5f63 6f6e 7465 6e74 6020 6174 7472  ct_content` attr
-00008330: 6962 7574 652e 0a20 2020 203a 7274 7970  ibute..    :rtyp
-00008340: 653a 205a 7374 6444 6963 740a 0a0a 4d6f  e: ZstdDict...Mo
-00008350: 6475 6c65 2d6c 6576 656c 2066 756e 6374  dule-level funct
-00008360: 696f 6e73 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ions.-----------
-00008370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020  -----------..   
-00008380: 2054 6869 7320 7365 6374 696f 6e20 636f   This section co
-00008390: 6e74 6169 6e73 3a0a 0a20 2020 2020 2020  ntains:..       
-000083a0: 202a 2066 756e 6374 696f 6e20 3a70 793a   * function :py:
-000083b0: 6675 6e63 3a60 6765 745f 6672 616d 655f  func:`get_frame_
-000083c0: 696e 666f 602c 2067 6574 2066 7261 6d65  info`, get frame
-000083d0: 2069 6e66 6f72 6d61 7469 6f6e 2066 726f   information fro
-000083e0: 6d20 6120 6672 616d 6520 6865 6164 6572  m a frame header
-000083f0: 2e0a 2020 2020 2020 2020 2a20 6675 6e63  ..        * func
-00008400: 7469 6f6e 203a 7079 3a66 756e 633a 6067  tion :py:func:`g
-00008410: 6574 5f66 7261 6d65 5f73 697a 6560 2c20  et_frame_size`, 
-00008420: 6765 7420 6120 6672 616d 6527 7320 7369  get a frame's si
-00008430: 7a65 2e0a 0a2e 2e20 7079 3a66 756e 6374  ze..... py:funct
-00008440: 696f 6e3a 3a20 6765 745f 6672 616d 655f  ion:: get_frame_
-00008450: 696e 666f 2866 7261 6d65 5f62 7566 6665  info(frame_buffe
-00008460: 7229 0a0a 2020 2020 4765 7420 7a73 7464  r)..    Get zstd
-00008470: 2066 7261 6d65 2069 6e66 6f72 6d61 7469   frame informati
-00008480: 6f6e 2066 726f 6d20 6120 6672 616d 6520  on from a frame 
-00008490: 6865 6164 6572 2e0a 0a20 2020 2052 6574  header...    Ret
-000084a0: 7572 6e20 6120 322d 6974 656d 206e 616d  urn a 2-item nam
-000084b0: 6564 7475 706c 653a 2028 6465 636f 6d70  edtuple: (decomp
-000084c0: 7265 7373 6564 5f73 697a 652c 2064 6963  ressed_size, dic
-000084d0: 7469 6f6e 6172 795f 6964 290a 0a20 2020  tionary_id)..   
-000084e0: 2049 6620 6060 6465 636f 6d70 7265 7373   If ``decompress
-000084f0: 6564 5f73 697a 6560 6020 6973 2060 604e  ed_size`` is ``N
-00008500: 6f6e 6560 602c 2064 6563 6f6d 7072 6573  one``, decompres
-00008510: 7365 6420 7369 7a65 2069 7320 756e 6b6e  sed size is unkn
-00008520: 6f77 6e2e 0a0a 2020 2020 6060 6469 6374  own...    ``dict
-00008530: 696f 6e61 7279 5f69 6460 6020 6973 2061  ionary_id`` is a
-00008540: 2033 322d 6269 7420 756e 7369 676e 6564   32-bit unsigned
-00008550: 2069 6e74 6567 6572 2076 616c 7565 2e20   integer value. 
-00008560: 6060 3060 6020 6d65 616e 7320 6469 6374  ``0`` means dict
-00008570: 696f 6e61 7279 2049 4420 7761 7320 6e6f  ionary ID was no
-00008580: 7420 7265 636f 7264 6564 2069 6e20 6672  t recorded in fr
-00008590: 616d 6520 6865 6164 6572 2c20 7468 6520  ame header, the 
-000085a0: 6672 616d 6520 6d61 7920 6f72 206d 6179  frame may or may
-000085b0: 206e 6f74 206e 6565 6420 6120 6469 6374   not need a dict
-000085c0: 696f 6e61 7279 2074 6f20 6265 2064 6563  ionary to be dec
-000085d0: 6f64 6564 2c20 616e 6420 7468 6520 4944  oded, and the ID
-000085e0: 206f 6620 7375 6368 2061 2064 6963 7469   of such a dicti
-000085f0: 6f6e 6172 7920 6973 206e 6f74 2073 7065  onary is not spe
-00008600: 6369 6669 6564 2e20 284e 6f74 6520 7468  cified. (Note th
-00008610: 6174 2074 6865 206d 6561 6e69 6e67 206f  at the meaning o
-00008620: 6620 6060 3060 6020 6973 2064 6966 6665  f ``0`` is diffe
-00008630: 7265 6e74 2066 726f 6d20 3a70 793a 6174  rent from :py:at
-00008640: 7472 3a60 5a73 7464 4469 6374 2e64 6963  tr:`ZstdDict.dic
-00008650: 745f 6964 6020 6174 7472 6962 7574 652e  t_id` attribute.
-00008660: 290a 0a20 2020 2049 7427 7320 706f 7373  )..    It's poss
-00008670: 6962 6c65 2074 6f20 6170 7065 6e64 206d  ible to append m
-00008680: 6f72 6520 6974 656d 7320 746f 2074 6865  ore items to the
-00008690: 206e 616d 6564 7475 706c 6520 696e 2074   namedtuple in t
-000086a0: 6865 2066 7574 7572 652e 0a0a 2020 2020  he future...    
-000086b0: 3a70 6172 616d 2066 7261 6d65 5f62 7566  :param frame_buf
-000086c0: 6665 723a 2049 7420 7368 6f75 6c64 2073  fer: It should s
-000086d0: 7461 7274 7320 6672 6f6d 2074 6865 2062  tarts from the b
-000086e0: 6567 696e 6e69 6e67 206f 6620 6120 6672  eginning of a fr
-000086f0: 616d 652c 2061 6e64 2063 6f6e 7461 696e  ame, and contain
-00008700: 7320 6174 206c 6561 7374 2074 6865 2066  s at least the f
-00008710: 7261 6d65 2068 6561 6465 7220 2836 2074  rame header (6 t
-00008720: 6f20 3138 2062 7974 6573 292e 0a20 2020  o 18 bytes)..   
-00008730: 203a 7479 7065 2066 7261 6d65 5f62 7566   :type frame_buf
-00008740: 6665 723a 2062 7974 6573 2d6c 696b 6520  fer: bytes-like 
-00008750: 6f62 6a65 6374 0a20 2020 203a 7265 7475  object.    :retu
-00008760: 726e 3a20 496e 666f 726d 6174 696f 6e20  rn: Information 
-00008770: 6162 6f75 7420 6120 6672 616d 652e 0a20  about a frame.. 
-00008780: 2020 203a 7274 7970 653a 206e 616d 6564     :rtype: named
-00008790: 7475 706c 650a 2020 2020 3a72 6169 7365  tuple.    :raise
-000087a0: 7320 5a73 7464 4572 726f 723a 2057 6865  s ZstdError: Whe
-000087b0: 6e20 7061 7273 696e 6720 7468 6520 6672  n parsing the fr
-000087c0: 616d 6520 6865 6164 6572 2066 6169 6c73  ame header fails
-000087d0: 2e0a 0a2e 2e20 736f 7572 6365 636f 6465  ..... sourcecode
-000087e0: 3a3a 2070 7974 686f 6e0a 0a20 2020 203e  :: python..    >
-000087f0: 3e3e 2070 797a 7374 642e 6765 745f 6672  >> pyzstd.get_fr
-00008800: 616d 655f 696e 666f 2863 6f6d 7072 6573  ame_info(compres
-00008810: 7365 645f 6461 745b 3a32 305d 290a 2020  sed_dat[:20]).  
-00008820: 2020 6672 616d 655f 696e 666f 2864 6563    frame_info(dec
-00008830: 6f6d 7072 6573 7365 645f 7369 7a65 3d36  ompressed_size=6
-00008840: 3837 3337 392c 2064 6963 7469 6f6e 6172  87379, dictionar
-00008850: 795f 6964 3d31 3034 3039 3932 3236 3829  y_id=1040992268)
-00008860: 0a0a 0a2e 2e20 7079 3a66 756e 6374 696f  ..... py:functio
-00008870: 6e3a 3a20 6765 745f 6672 616d 655f 7369  n:: get_frame_si
-00008880: 7a65 2866 7261 6d65 5f62 7566 6665 7229  ze(frame_buffer)
-00008890: 0a0a 2020 2020 4765 7420 7468 6520 7369  ..    Get the si
-000088a0: 7a65 206f 6620 6120 7a73 7464 2066 7261  ze of a zstd fra
-000088b0: 6d65 2c20 696e 636c 7564 696e 6720 6672  me, including fr
-000088c0: 616d 6520 6865 6164 6572 2061 6e64 2034  ame header and 4
-000088d0: 2d62 7974 6520 6368 6563 6b73 756d 2069  -byte checksum i
-000088e0: 6620 6974 2068 6173 2e0a 0a20 2020 2049  f it has...    I
-000088f0: 7420 7769 6c6c 2069 7465 7261 7465 2061  t will iterate a
-00008900: 6c6c 2062 6c6f 636b 7327 2068 6561 6465  ll blocks' heade
-00008910: 7220 7769 7468 696e 2061 2066 7261 6d65  r within a frame
-00008920: 2c20 746f 2061 6363 756d 756c 6174 6520  , to accumulate 
-00008930: 7468 6520 6672 616d 6527 7320 7369 7a65  the frame's size
-00008940: 2e0a 0a20 2020 203a 7061 7261 6d20 6672  ...    :param fr
-00008950: 616d 655f 6275 6666 6572 3a20 4974 2073  ame_buffer: It s
-00008960: 686f 756c 6420 7374 6172 7473 2066 726f  hould starts fro
-00008970: 6d20 7468 6520 6265 6769 6e6e 696e 6720  m the beginning 
-00008980: 6f66 2061 2066 7261 6d65 2c20 616e 6420  of a frame, and 
-00008990: 636f 6e74 6169 6e73 2061 7420 6c65 6173  contains at leas
-000089a0: 7420 6f6e 6520 636f 6d70 6c65 7465 2066  t one complete f
-000089b0: 7261 6d65 2e0a 2020 2020 3a74 7970 6520  rame..    :type 
-000089c0: 6672 616d 655f 6275 6666 6572 3a20 6279  frame_buffer: by
-000089d0: 7465 732d 6c69 6b65 206f 626a 6563 740a  tes-like object.
-000089e0: 2020 2020 3a72 6574 7572 6e3a 2054 6865      :return: The
-000089f0: 2073 697a 6520 6f66 2061 207a 7374 6420   size of a zstd 
-00008a00: 6672 616d 652e 0a20 2020 203a 7274 7970  frame..    :rtyp
-00008a10: 653a 2069 6e74 0a20 2020 203a 7261 6973  e: int.    :rais
-00008a20: 6573 205a 7374 6445 7272 6f72 3a20 5768  es ZstdError: Wh
-00008a30: 656e 2069 7420 6661 696c 732e 0a0a 2e2e  en it fails.....
-00008a40: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
-00008a50: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 7079  thon..    >>> py
-00008a60: 7a73 7464 2e67 6574 5f66 7261 6d65 5f73  zstd.get_frame_s
-00008a70: 697a 6528 636f 6d70 7265 7373 6564 5f64  ize(compressed_d
-00008a80: 6174 290a 2020 2020 3235 3238 3734 0a0a  at).    252874..
-00008a90: 0a4d 6f64 756c 652d 6c65 7665 6c20 7661  .Module-level va
-00008aa0: 7269 6162 6c65 730a 2d2d 2d2d 2d2d 2d2d  riables.--------
-00008ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00008ac0: 2020 2020 5468 6973 2073 6563 7469 6f6e      This section
-00008ad0: 2063 6f6e 7461 696e 733a 0a0a 2020 2020   contains:..    
-00008ae0: 2020 2020 2a20 3a70 793a 6461 7461 3a60      * :py:data:`
-00008af0: 7a73 7464 5f76 6572 7369 6f6e 602c 2061  zstd_version`, a
-00008b00: 2060 6073 7472 6060 2e0a 2020 2020 2020   ``str``..      
-00008b10: 2020 2a20 3a70 793a 6461 7461 3a60 7a73    * :py:data:`zs
-00008b20: 7464 5f76 6572 7369 6f6e 5f69 6e66 6f60  td_version_info`
-00008b30: 2c20 6120 6060 7475 706c 6560 602e 0a20  , a ``tuple``.. 
-00008b40: 2020 2020 2020 202a 203a 7079 3a64 6174         * :py:dat
-00008b50: 613a 6063 6f6d 7072 6573 7369 6f6e 4c65  a:`compressionLe
-00008b60: 7665 6c5f 7661 6c75 6573 602c 2073 6f6d  vel_values`, som
-00008b70: 6520 7661 6c75 6573 2064 6566 696e 6564  e values defined
-00008b80: 2062 7920 7468 6520 756e 6465 726c 7969   by the underlyi
-00008b90: 6e67 207a 7374 6420 6c69 6272 6172 792e  ng zstd library.
-00008ba0: 0a20 2020 2020 2020 202a 203a 7079 3a64  .        * :py:d
-00008bb0: 6174 613a 607a 7374 645f 7375 7070 6f72  ata:`zstd_suppor
-00008bc0: 745f 6d75 6c74 6974 6872 6561 6460 2c20  t_multithread`, 
-00008bd0: 7768 6574 6865 7220 7468 6520 756e 6465  whether the unde
-00008be0: 726c 7969 6e67 207a 7374 6420 6c69 6272  rlying zstd libr
-00008bf0: 6172 7920 7375 7070 6f72 7473 206d 756c  ary supports mul
-00008c00: 7469 2d74 6872 6561 6465 6420 636f 6d70  ti-threaded comp
-00008c10: 7265 7373 696f 6e2e 0a0a 2e2e 2070 793a  ression..... py:
-00008c20: 6461 7461 3a3a 207a 7374 645f 7665 7273  data:: zstd_vers
-00008c30: 696f 6e0a 0a20 2020 2055 6e64 6572 6c79  ion..    Underly
-00008c40: 696e 6720 7a73 7464 206c 6962 7261 7279  ing zstd library
-00008c50: 2773 2076 6572 7369 6f6e 2c20 6060 7374  's version, ``st
-00008c60: 7260 6020 666f 726d 2e0a 0a2e 2e20 736f  r`` form..... so
-00008c70: 7572 6365 636f 6465 3a3a 2070 7974 686f  urcecode:: pytho
-00008c80: 6e0a 0a20 2020 203e 3e3e 2070 797a 7374  n..    >>> pyzst
-00008c90: 642e 7a73 7464 5f76 6572 7369 6f6e 0a20  d.zstd_version. 
-00008ca0: 2020 2027 312e 342e 3527 0a0a 0a2e 2e20     '1.4.5'..... 
-00008cb0: 7079 3a64 6174 613a 3a20 7a73 7464 5f76  py:data:: zstd_v
-00008cc0: 6572 7369 6f6e 5f69 6e66 6f0a 0a20 2020  ersion_info..   
-00008cd0: 2055 6e64 6572 6c79 696e 6720 7a73 7464   Underlying zstd
-00008ce0: 206c 6962 7261 7279 2773 2076 6572 7369   library's versi
-00008cf0: 6f6e 2c20 6060 7475 706c 6560 6020 666f  on, ``tuple`` fo
-00008d00: 726d 2e0a 0a2e 2e20 736f 7572 6365 636f  rm..... sourceco
-00008d10: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
-00008d20: 203e 3e3e 2070 797a 7374 642e 7a73 7464   >>> pyzstd.zstd
-00008d30: 5f76 6572 7369 6f6e 5f69 6e66 6f0a 2020  _version_info.  
-00008d40: 2020 2831 2c20 342c 2035 290a 0a0a 2e2e    (1, 4, 5).....
-00008d50: 2070 793a 6461 7461 3a3a 2063 6f6d 7072   py:data:: compr
-00008d60: 6573 7369 6f6e 4c65 7665 6c5f 7661 6c75  essionLevel_valu
-00008d70: 6573 0a0a 2020 2020 4120 332d 6974 656d  es..    A 3-item
-00008d80: 206e 616d 6564 7475 706c 652c 2076 616c   namedtuple, val
-00008d90: 7565 7320 6465 6669 6e65 6420 6279 2074  ues defined by t
-00008da0: 6865 2075 6e64 6572 6c79 696e 6720 7a73  he underlying zs
-00008db0: 7464 206c 6962 7261 7279 2c20 7365 6520  td library, see 
-00008dc0: 3a72 6566 3a60 636f 6d70 7265 7373 696f  :ref:`compressio
-00008dd0: 6e20 6c65 7665 6c3c 636f 6d70 7265 7373  n level<compress
-00008de0: 696f 6e5f 6c65 7665 6c3e 6020 666f 7220  ion_level>` for 
-00008df0: 6465 7461 696c 732e 0a0a 2020 2020 6060  details...    ``
-00008e00: 6465 6661 756c 7460 6020 6973 2064 6566  default`` is def
-00008e10: 6175 6c74 2063 6f6d 7072 6573 7369 6f6e  ault compression
-00008e20: 206c 6576 656c 2c20 6974 2069 7320 7573   level, it is us
-00008e30: 6564 2077 6865 6e20 636f 6d70 7265 7373  ed when compress
-00008e40: 696f 6e20 6c65 7665 6c20 6973 2073 6574  ion level is set
-00008e50: 2074 6f20 6060 3060 6020 6f72 206e 6f74   to ``0`` or not
-00008e60: 2073 6574 2e0a 0a20 2020 2060 606d 696e   set...    ``min
-00008e70: 6060 2f60 606d 6178 6060 2061 7265 206d  ``/``max`` are m
-00008e80: 696e 696d 756d 2f6d 6178 696d 756d 2061  inimum/maximum a
-00008e90: 7661 696c 6162 6c65 2076 616c 7565 7320  vailable values 
-00008ea0: 6f66 2063 6f6d 7072 6573 7369 6f6e 206c  of compression l
-00008eb0: 6576 656c 2c20 626f 7468 2069 6e63 6c75  evel, both inclu
-00008ec0: 7369 7665 2e0a 0a2e 2e20 736f 7572 6365  sive..... source
-00008ed0: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-00008ee0: 2020 203e 3e3e 2070 797a 7374 642e 636f     >>> pyzstd.co
-00008ef0: 6d70 7265 7373 696f 6e4c 6576 656c 5f76  mpressionLevel_v
-00008f00: 616c 7565 7320 2023 2031 3331 3037 3220  alues  # 131072 
-00008f10: 3d20 3132 382a 3130 3234 0a20 2020 2076  = 128*1024.    v
-00008f20: 616c 7565 7328 6465 6661 756c 743d 332c  alues(default=3,
-00008f30: 206d 696e 3d2d 3133 3130 3732 2c20 6d61   min=-131072, ma
-00008f40: 783d 3232 290a 0a0a 2e2e 2070 793a 6461  x=22)..... py:da
-00008f50: 7461 3a3a 207a 7374 645f 7375 7070 6f72  ta:: zstd_suppor
-00008f60: 745f 6d75 6c74 6974 6872 6561 640a 0a20  t_multithread.. 
-00008f70: 2020 2057 6865 7468 6572 2074 6865 2075     Whether the u
-00008f80: 6e64 6572 6c79 696e 6720 7a73 7464 206c  nderlying zstd l
-00008f90: 6962 7261 7279 2077 6173 2063 6f6d 7069  ibrary was compi
-00008fa0: 6c65 6420 7769 7468 203a 7265 663a 606d  led with :ref:`m
-00008fb0: 756c 7469 2d74 6872 6561 6465 6420 636f  ulti-threaded co
-00008fc0: 6d70 7265 7373 696f 6e3c 6d74 5f63 6f6d  mpression<mt_com
-00008fd0: 7072 6573 7369 6f6e 3e60 2073 7570 706f  pression>` suppo
-00008fe0: 7274 2e0a 0a20 2020 2049 7427 7320 616c  rt...    It's al
-00008ff0: 6d6f 7374 2061 6c77 6179 7320 6060 5472  most always ``Tr
-00009000: 7565 6060 2e0a 0a20 2020 2049 7427 7320  ue``...    It's 
-00009010: 6060 4661 6c73 6560 6020 7768 656e 2064  ``False`` when d
-00009020: 796e 616d 6963 616c 6c79 206c 696e 6b65  ynamically linke
-00009030: 6420 746f 207a 7374 6420 6c69 6272 6172  d to zstd librar
-00009040: 7920 7468 6174 2063 6f6d 7069 6c65 6420  y that compiled 
-00009050: 7769 7468 6f75 7420 6d75 6c74 692d 7468  without multi-th
-00009060: 7265 6164 6564 2073 7570 706f 7274 2e20  readed support. 
-00009070: 4f72 6469 6e61 7279 2075 7365 7273 2077  Ordinary users w
-00009080: 696c 6c20 6e6f 7420 6d65 6574 2074 6869  ill not meet thi
-00009090: 7320 7369 7475 6174 696f 6e2e 0a0a 2e2e  s situation.....
-000090a0: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
-000090b0: 302e 3135 2e31 0a0a 2e2e 2073 6f75 7263  0.15.1.... sourc
-000090c0: 6563 6f64 653a 3a20 7079 7468 6f6e 0a0a  ecode:: python..
-000090d0: 2020 2020 3e3e 3e20 7079 7a73 7464 2e7a      >>> pyzstd.z
-000090e0: 7374 645f 7375 7070 6f72 745f 6d75 6c74  std_support_mult
-000090f0: 6974 6872 6561 640a 2020 2020 5472 7565  ithread.    True
-00009100: 0a0a 0a5a 7374 6446 696c 6520 636c 6173  ...ZstdFile clas
-00009110: 7320 616e 6420 6f70 656e 2829 2066 756e  s and open() fun
-00009120: 6374 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d  ction.----------
-00009130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20  -------------.. 
-00009150: 2020 2054 6869 7320 7365 6374 696f 6e20     This section 
-00009160: 636f 6e74 6169 6e73 3a0a 0a20 2020 2020  contains:..     
-00009170: 2020 202a 2063 6c61 7373 203a 7079 3a63     * class :py:c
-00009180: 6c61 7373 3a60 5a73 7464 4669 6c65 602c  lass:`ZstdFile`,
-00009190: 206f 7065 6e20 6120 7a73 7464 2d63 6f6d   open a zstd-com
-000091a0: 7072 6573 7365 6420 6669 6c65 2069 6e20  pressed file in 
-000091b0: 6269 6e61 7279 206d 6f64 652e 0a20 2020  binary mode..   
-000091c0: 2020 2020 202a 2066 756e 6374 696f 6e20       * function 
-000091d0: 3a70 793a 6675 6e63 3a60 6f70 656e 602c  :py:func:`open`,
-000091e0: 206f 7065 6e20 6120 7a73 7464 2d63 6f6d   open a zstd-com
-000091f0: 7072 6573 7365 6420 6669 6c65 2069 6e20  pressed file in 
-00009200: 6269 6e61 7279 206f 7220 7465 7874 206d  binary or text m
-00009210: 6f64 652e 0a0a 2e2e 2070 793a 636c 6173  ode..... py:clas
-00009220: 733a 3a20 5a73 7464 4669 6c65 0a0a 2020  s:: ZstdFile..  
-00009230: 2020 4f70 656e 2061 207a 7374 642d 636f    Open a zstd-co
-00009240: 6d70 7265 7373 6564 2066 696c 6520 696e  mpressed file in
-00009250: 2062 696e 6172 7920 6d6f 6465 2e0a 0a20   binary mode... 
-00009260: 2020 2054 6869 7320 636c 6173 7320 6973     This class is
-00009270: 2076 6572 7920 7369 6d69 6c61 7220 746f   very similar to
-00009280: 2060 627a 322e 425a 3246 696c 6520 3c68   `bz2.BZ2File <h
-00009290: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
-000092a0: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
-000092b0: 2f62 7a32 2e68 746d 6c23 627a 322e 425a  /bz2.html#bz2.BZ
-000092c0: 3246 696c 653e 605f 202f 2020 6067 7a69  2File>`_ /  `gzi
-000092d0: 702e 477a 6970 4669 6c65 203c 6874 7470  p.GzipFile <http
-000092e0: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-000092f0: 6f72 672f 332f 6c69 6272 6172 792f 677a  org/3/library/gz
-00009300: 6970 2e68 746d 6c23 677a 6970 2e47 7a69  ip.html#gzip.Gzi
-00009310: 7046 696c 653e 605f 202f 2060 6c7a 6d61  pFile>`_ / `lzma
-00009320: 2e4c 5a4d 4146 696c 6520 3c68 7474 7073  .LZMAFile <https
-00009330: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00009340: 7267 2f33 2f6c 6962 7261 7279 2f6c 7a6d  rg/3/library/lzm
-00009350: 612e 6874 6d6c 236c 7a6d 612e 4c5a 4d41  a.html#lzma.LZMA
-00009360: 4669 6c65 3e60 5f20 636c 6173 7365 7320  File>`_ classes 
-00009370: 696e 2050 7974 686f 6e20 7374 616e 6461  in Python standa
-00009380: 7264 206c 6962 7261 7279 2e0a 0a20 2020  rd library...   
-00009390: 204c 696b 6520 425a 3246 696c 652f 477a   Like BZ2File/Gz
-000093a0: 6970 4669 6c65 2f4c 5a4d 4146 696c 6520  ipFile/LZMAFile 
-000093b0: 636c 6173 7365 732c 205a 7374 6446 696c  classes, ZstdFil
-000093c0: 6520 6973 206e 6f74 2074 6872 6561 642d  e is not thread-
-000093d0: 7361 6665 2c20 736f 2069 6620 796f 7520  safe, so if you 
-000093e0: 6e65 6564 2074 6f20 7573 6520 6120 7369  need to use a si
-000093f0: 6e67 6c65 205a 7374 6446 696c 6520 6f62  ngle ZstdFile ob
-00009400: 6a65 6374 2066 726f 6d20 6d75 6c74 6970  ject from multip
-00009410: 6c65 2074 6872 6561 6473 2c20 6974 2069  le threads, it i
-00009420: 7320 6e65 6365 7373 6172 7920 746f 2070  s necessary to p
-00009430: 726f 7465 6374 2069 7420 7769 7468 2061  rotect it with a
-00009440: 206c 6f63 6b2e 0a0a 2020 2020 4974 2063   lock...    It c
-00009450: 616e 2062 6520 7573 6564 2077 6974 6820  an be used with 
-00009460: 5079 7468 6f6e 2773 2060 6074 6172 6669  Python's ``tarfi
-00009470: 6c65 6060 206d 6f64 756c 652c 2073 6565  le`` module, see
-00009480: 203a 7265 663a 6074 6869 7320 6e6f 7465   :ref:`this note
-00009490: 3c77 6974 685f 7461 7266 696c 653e 602e  <with_tarfile>`.
-000094a0: 0a0a 2020 2020 2e2e 2070 793a 6d65 7468  ..    .. py:meth
-000094b0: 6f64 3a3a 205f 5f69 6e69 745f 5f28 7365  od:: __init__(se
-000094c0: 6c66 2c20 6669 6c65 6e61 6d65 2c20 6d6f  lf, filename, mo
-000094d0: 6465 3d22 7222 2c20 2a2c 206c 6576 656c  de="r", *, level
-000094e0: 5f6f 725f 6f70 7469 6f6e 3d4e 6f6e 652c  _or_option=None,
-000094f0: 207a 7374 645f 6469 6374 3d4e 6f6e 6529   zstd_dict=None)
-00009500: 0a0a 2020 2020 2020 2020 5468 6520 2a66  ..        The *f
-00009510: 696c 656e 616d 652a 2070 6172 616d 6574  ilename* paramet
-00009520: 6572 2063 616e 2062 6520 616e 2065 7869  er can be an exi
-00009530: 7374 696e 6720 6066 696c 6520 6f62 6a65  sting `file obje
-00009540: 6374 203c 6874 7470 733a 2f2f 646f 6373  ct <https://docs
-00009550: 2e70 7974 686f 6e2e 6f72 672f 332f 676c  .python.org/3/gl
-00009560: 6f73 7361 7279 2e68 746d 6c23 7465 726d  ossary.html#term
-00009570: 2d66 696c 652d 6f62 6a65 6374 3e60 5f20  -file-object>`_ 
-00009580: 746f 2077 7261 702c 206f 7220 7468 6520  to wrap, or the 
-00009590: 6e61 6d65 206f 6620 7468 6520 6669 6c65  name of the file
-000095a0: 2074 6f20 6f70 656e 2028 6173 2061 2060   to open (as a `
-000095b0: 6073 7472 6060 2c20 6060 6279 7465 7360  `str``, ``bytes`
-000095c0: 6020 6f72 2060 7061 7468 2d6c 696b 6520  ` or `path-like 
-000095d0: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
-000095e0: 7468 6f6e 2e6f 7267 2f33 2f67 6c6f 7373  thon.org/3/gloss
-000095f0: 6172 792e 6874 6d6c 2374 6572 6d2d 7061  ary.html#term-pa
-00009600: 7468 2d6c 696b 652d 6f62 6a65 6374 3e60  th-like-object>`
-00009610: 5f20 6f62 6a65 6374 292e 2057 6865 6e20  _ object). When 
-00009620: 7772 6170 7069 6e67 2061 6e20 6578 6973  wrapping an exis
-00009630: 7469 6e67 2066 696c 6520 6f62 6a65 6374  ting file object
-00009640: 2c20 7468 6520 7772 6170 7065 6420 6669  , the wrapped fi
-00009650: 6c65 2077 696c 6c20 6e6f 7420 6265 2063  le will not be c
-00009660: 6c6f 7365 6420 7768 656e 2074 6865 205a  losed when the Z
-00009670: 7374 6446 696c 6520 6973 2063 6c6f 7365  stdFile is close
-00009680: 642e 0a0a 2020 2020 2020 2020 5468 6520  d...        The 
-00009690: 2a6d 6f64 652a 2070 6172 616d 6574 6572  *mode* parameter
-000096a0: 2063 616e 2062 6520 6569 7468 6572 2022   can be either "
-000096b0: 7222 2066 6f72 2072 6561 6469 6e67 2028  r" for reading (
-000096c0: 6465 6661 756c 7429 2c20 2277 2220 666f  default), "w" fo
-000096d0: 7220 6f76 6572 7772 6974 696e 672c 2022  r overwriting, "
-000096e0: 7822 2066 6f72 2065 7863 6c75 7369 7665  x" for exclusive
-000096f0: 2063 7265 6174 696f 6e2c 206f 7220 2261   creation, or "a
-00009700: 2220 666f 7220 6170 7065 6e64 696e 672e  " for appending.
-00009710: 2054 6865 7365 2063 616e 2065 7175 6976   These can equiv
-00009720: 616c 656e 746c 7920 6265 2067 6976 656e  alently be given
-00009730: 2061 7320 2272 6222 2c20 2277 6222 2c20   as "rb", "wb", 
-00009740: 2278 6222 2061 6e64 2022 6162 2220 7265  "xb" and "ab" re
-00009750: 7370 6563 7469 7665 6c79 2e0a 0a20 2020  spectively...   
-00009760: 2020 2020 2049 6620 696e 2072 6561 6469       If in readi
-00009770: 6e67 206d 6f64 6520 2864 6563 6f6d 7072  ng mode (decompr
-00009780: 6573 7369 6f6e 293a 0a0a 2020 2020 2020  ession):..      
-00009790: 2020 2020 2020 2a20 5468 6520 2a6c 6576        * The *lev
-000097a0: 656c 5f6f 725f 6f70 7469 6f6e 2a20 7061  el_or_option* pa
-000097b0: 7261 6d65 7465 7220 6361 6e20 6f6e 6c79  rameter can only
-000097c0: 2062 6520 6120 6060 6469 6374 6060 206f   be a ``dict`` o
-000097d0: 626a 6563 742c 2074 6861 7420 7265 7072  bject, that repr
-000097e0: 6573 656e 7473 2064 6563 6f6d 7072 6573  esents decompres
-000097f0: 7369 6f6e 206f 7074 696f 6e2e 2049 7420  sion option. It 
-00009800: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-00009810: 6060 696e 7460 6020 7479 7065 2063 6f6d  ``int`` type com
-00009820: 7072 6573 7369 6f6e 206c 6576 656c 2069  pression level i
-00009830: 6e20 7468 6973 2063 6173 652e 0a20 2020  n this case..   
-00009840: 2020 2020 2020 2020 202a 2054 6865 2069           * The i
-00009850: 6e70 7574 2066 696c 6520 6d61 7920 6265  nput file may be
-00009860: 2074 6865 2063 6f6e 6361 7465 6e61 7469   the concatenati
-00009870: 6f6e 206f 6620 6d75 6c74 6970 6c65 203a  on of multiple :
-00009880: 7265 663a 6066 7261 6d65 733c 6672 616d  ref:`frames<fram
-00009890: 655f 626c 6f63 6b3e 602e 0a0a 2020 2020  e_block>`...    
-000098a0: 496e 2077 7269 7469 6e67 206d 6f64 6520  In writing mode 
-000098b0: 2863 6f6d 7072 6573 7369 6f6e 292c 2074  (compression), t
-000098c0: 6865 7365 206d 6574 686f 6473 2061 7265  hese methods are
-000098d0: 2061 7661 696c 6162 6c65 3a0a 0a20 2020   available:..   
-000098e0: 2020 2020 202a 2060 2e77 7269 7465 2862       * `.write(b
-000098f0: 2920 3c68 7474 7073 3a2f 2f64 6f63 732e  ) <https://docs.
-00009900: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
-00009910: 7261 7279 2f69 6f2e 6874 6d6c 2369 6f2e  rary/io.html#io.
-00009920: 4275 6666 6572 6564 494f 4261 7365 2e77  BufferedIOBase.w
-00009930: 7269 7465 3e60 5f0a 2020 2020 2020 2020  rite>`_.        
-00009940: 2a20 602e 666c 7573 6828 2920 3c68 7474  * `.flush() <htt
-00009950: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
-00009960: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f69  .org/3/library/i
-00009970: 6f2e 6874 6d6c 2369 6f2e 494f 4261 7365  o.html#io.IOBase
-00009980: 2e66 6c75 7368 3e60 5f2c 2066 6c75 7368  .flush>`_, flush
-00009990: 2074 6f20 7468 6520 756e 6465 726c 7969   to the underlyi
-000099a0: 6e67 2073 7472 6561 6d2e 2049 7420 7573  ng stream. It us
-000099b0: 6573 203a 7079 3a61 7474 723a 605a 7374  es :py:attr:`Zst
-000099c0: 6443 6f6d 7072 6573 736f 722e 464c 5553  dCompressor.FLUS
-000099d0: 485f 424c 4f43 4b60 206d 6f64 652c 2061  H_BLOCK` mode, a
-000099e0: 6275 7365 206f 6620 7468 6973 206d 6574  buse of this met
-000099f0: 686f 6420 7769 6c6c 2072 6564 7563 6520  hod will reduce 
-00009a00: 636f 6d70 7265 7373 696f 6e20 7261 7469  compression rati
-00009a10: 6f2c 2075 7365 2069 7420 6f6e 6c79 2077  o, use it only w
-00009a20: 6865 6e20 6e65 6365 7373 6172 792e 2049  hen necessary. I
-00009a30: 6620 7468 6520 7072 6f67 7261 6d20 6973  f the program is
-00009a40: 2069 6e74 6572 7275 7074 6564 2061 6674   interrupted aft
-00009a50: 6572 7761 7264 732c 2061 6c6c 2064 6174  erwards, all dat
-00009a60: 6120 6361 6e20 6265 2072 6563 6f76 6572  a can be recover
-00009a70: 6564 2e20 546f 2065 6e73 7572 6520 7361  ed. To ensure sa
-00009a80: 7669 6e67 2074 6f20 6469 736b 2c20 616c  ving to disk, al
-00009a90: 736f 206e 6565 6420 606f 732e 6673 796e  so need `os.fsyn
-00009aa0: 6328 6664 2920 3c68 7474 7073 3a2f 2f64  c(fd) <https://d
-00009ab0: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
-00009ac0: 2f6c 6962 7261 7279 2f6f 732e 6874 6d6c  /library/os.html
-00009ad0: 236f 732e 6673 796e 633e 605f 2e20 2028  #os.fsync>`_.  (
-00009ae0: 2a49 6d70 6c65 6d65 6e74 6564 2069 6e20  *Implemented in 
-00009af0: 7665 7273 696f 6e20 302e 3135 2e31 2a29  version 0.15.1*)
-00009b00: 0a0a 2020 2020 496e 2072 6561 6469 6e67  ..    In reading
-00009b10: 206d 6f64 6520 2864 6563 6f6d 7072 6573   mode (decompres
-00009b20: 7369 6f6e 292c 2074 6865 7365 206d 6574  sion), these met
-00009b30: 686f 6473 2061 6e64 2073 7461 7465 6d65  hods and stateme
-00009b40: 6e74 2061 7265 2061 7661 696c 6162 6c65  nt are available
-00009b50: 3a0a 0a20 2020 2020 2020 202a 2060 2e72  :..        * `.r
-00009b60: 6561 6428 7369 7a65 3d2d 3129 203c 6874  ead(size=-1) <ht
-00009b70: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00009b80: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-00009b90: 696f 2e68 746d 6c23 696f 2e42 7566 6665  io.html#io.Buffe
-00009ba0: 7265 6452 6561 6465 722e 7265 6164 3e60  redReader.read>`
-00009bb0: 5f0a 2020 2020 2020 2020 2a20 602e 7265  _.        * `.re
-00009bc0: 6164 3128 7369 7a65 3d2d 3129 203c 6874  ad1(size=-1) <ht
-00009bd0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00009be0: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-00009bf0: 696f 2e68 746d 6c23 696f 2e42 7566 6665  io.html#io.Buffe
-00009c00: 7265 6452 6561 6465 722e 7265 6164 313e  redReader.read1>
-00009c10: 605f 0a20 2020 2020 2020 202a 2060 2e72  `_.        * `.r
-00009c20: 6561 6469 6e74 6f28 6229 203c 6874 7470  eadinto(b) <http
-00009c30: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-00009c40: 6f72 672f 332f 6c69 6272 6172 792f 696f  org/3/library/io
-00009c50: 2e68 746d 6c23 696f 2e42 7566 6665 7265  .html#io.Buffere
-00009c60: 6449 4f42 6173 652e 7265 6164 696e 746f  dIOBase.readinto
-00009c70: 3e60 5f0a 2020 2020 2020 2020 2a20 602e  >`_.        * `.
-00009c80: 7265 6164 696e 746f 3128 6229 203c 6874  readinto1(b) <ht
-00009c90: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00009ca0: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-00009cb0: 696f 2e68 746d 6c23 696f 2e42 7566 6665  io.html#io.Buffe
-00009cc0: 7265 6449 4f42 6173 652e 7265 6164 696e  redIOBase.readin
-00009cd0: 746f 313e 605f 0a20 2020 2020 2020 202a  to1>`_.        *
-00009ce0: 2060 2e72 6561 646c 696e 6528 7369 7a65   `.readline(size
-00009cf0: 3d2d 3129 203c 6874 7470 733a 2f2f 646f  =-1) <https://do
-00009d00: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-00009d10: 6c69 6272 6172 792f 696f 2e68 746d 6c23  library/io.html#
-00009d20: 696f 2e49 4f42 6173 652e 7265 6164 6c69  io.IOBase.readli
-00009d30: 6e65 3e60 5f0a 2020 2020 2020 2020 2a20  ne>`_.        * 
-00009d40: 602e 7365 656b 286f 6666 7365 742c 2077  `.seek(offset, w
-00009d50: 6865 6e63 653d 696f 2e53 4545 4b5f 5345  hence=io.SEEK_SE
-00009d60: 5429 203c 6874 7470 733a 2f2f 646f 6373  T) <https://docs
-00009d70: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-00009d80: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
-00009d90: 2e49 4f42 6173 652e 7365 656b 3e60 5f2c  .IOBase.seek>`_,
-00009da0: 206e 6f74 6520 7468 6174 2069 6620 6060   note that if ``
-00009db0: 2e73 6565 6b28 2960 6020 746f 2022 7072  .seek()`` to "pr
-00009dc0: 6576 696f 7573 2070 6f73 6974 696f 6e22  evious position"
-00009dd0: 206f 7220 2270 6f73 6974 696f 6e20 7265   or "position re
-00009de0: 6c61 7469 7665 2074 6f20 454f 4620 2874  lative to EOF (t
-00009df0: 6865 2066 6972 7374 2074 696d 6529 222c  he first time)",
-00009e00: 2074 6865 2064 6563 6f6d 7072 6573 7369   the decompressi
-00009e10: 6f6e 2068 6173 2074 6f20 6265 2072 6573  on has to be res
-00009e20: 7461 7274 6564 2066 726f 6d20 7a65 726f  tarted from zero
-00009e30: 2e0a 2020 2020 2020 2020 2a20 602e 7065  ..        * `.pe
-00009e40: 656b 2873 697a 653d 2d31 2920 3c68 7474  ek(size=-1) <htt
-00009e50: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
-00009e60: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f69  .org/3/library/i
-00009e70: 6f2e 6874 6d6c 2369 6f2e 4275 6666 6572  o.html#io.Buffer
-00009e80: 6564 5265 6164 6572 2e70 6565 6b3e 605f  edReader.peek>`_
-00009e90: 0a20 2020 2020 2020 202a 2060 4974 6572  .        * `Iter
-00009ea0: 6174 696f 6e20 3c68 7474 7073 3a2f 2f64  ation <https://d
-00009eb0: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
-00009ec0: 2f6c 6962 7261 7279 2f69 6f2e 6874 6d6c  /library/io.html
-00009ed0: 2369 6f2e 494f 4261 7365 3e60 5f2c 2079  #io.IOBase>`_, y
-00009ee0: 6965 6c64 206c 696e 6573 2c20 6c69 6e65  ield lines, line
-00009ef0: 2074 6572 6d69 6e61 746f 7220 6973 2060   terminator is `
-00009f00: 6062 275c 6e27 6060 2e0a 0a20 2020 2049  `b'\n'``...    I
-00009f10: 6e20 626f 7468 2072 6561 6469 6e67 2061  n both reading a
-00009f20: 6e64 2077 7269 7469 6e67 206d 6f64 6573  nd writing modes
-00009f30: 2c20 7468 6573 6520 6d65 7468 6f64 7320  , these methods 
-00009f40: 616e 6420 7072 6f70 6572 7479 2061 7265  and property are
-00009f50: 2061 7661 696c 6162 6c65 3a0a 0a20 2020   available:..   
-00009f60: 2020 2020 202a 2060 2e63 6c6f 7365 2829       * `.close()
-00009f70: 203c 6874 7470 733a 2f2f 646f 6373 2e70   <https://docs.p
-00009f80: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
-00009f90: 6172 792f 696f 2e68 746d 6c23 696f 2e49  ary/io.html#io.I
-00009fa0: 4f42 6173 652e 636c 6f73 653e 605f 0a20  OBase.close>`_. 
-00009fb0: 2020 2020 2020 202a 2060 2e74 656c 6c28         * `.tell(
+00000140: 2073 6f75 7263 6520 636f 6465 0a2a 2043   source code.* C
+00000150: 616e 2061 6c73 6f20 6479 6e61 6d69 6361  an also dynamica
+00000160: 6c6c 7920 6c69 6e6b 2074 6f20 7a73 7464  lly link to zstd
+00000170: 206c 6962 7261 7279 2070 726f 7669 6465   library provide
+00000180: 6420 6279 2073 7973 7465 6d2c 2073 6565  d by system, see
+00000190: 203a 7265 663a 6074 6869 7320 6e6f 7465   :ref:`this note
+000001a0: 3c62 7569 6c64 5f70 797a 7374 643e 602e  <build_pyzstd>`.
+000001b0: 0a2a 2048 6173 2061 2043 4646 4920 696d  .* Has a CFFI im
+000001c0: 706c 656d 656e 7461 7469 6f6e 2074 6861  plementation tha
+000001d0: 7420 6361 6e20 776f 726b 2077 6974 6820  t can work with 
+000001e0: 5079 5079 0a2a 203a 7079 3a63 6c61 7373  PyPy.* :py:class
+000001f0: 3a60 5a73 7464 4669 6c65 6020 636c 6173  :`ZstdFile` clas
+00000200: 7320 6861 7320 4320 6c61 6e67 7561 6765  s has C language
+00000210: 206c 6576 656c 2070 6572 666f 726d 616e   level performan
+00000220: 6365 0a2a 2053 7570 706f 7274 7320 605a  ce.* Supports `Z
+00000230: 7374 616e 6461 7264 2053 6565 6b61 626c  standard Seekabl
+00000240: 6520 466f 726d 6174 203c 6874 7470 733a  e Format <https:
+00000250: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6163  //github.com/fac
+00000260: 6562 6f6f 6b2f 7a73 7464 2f62 6c6f 622f  ebook/zstd/blob/
+00000270: 6465 762f 636f 6e74 7269 622f 7365 656b  dev/contrib/seek
+00000280: 6162 6c65 5f66 6f72 6d61 742f 7a73 7464  able_format/zstd
+00000290: 5f73 6565 6b61 626c 655f 636f 6d70 7265  _seekable_compre
+000002a0: 7373 696f 6e5f 666f 726d 6174 2e6d 643e  ssion_format.md>
+000002b0: 605f 5f0a 2a20 4861 7320 6120 636f 6d6d  `__.* Has a comm
+000002c0: 616e 6420 6c69 6e65 2069 6e74 6572 6661  and line interfa
+000002d0: 6365 2c20 6060 7079 7468 6f6e 202d 6d20  ce, ``python -m 
+000002e0: 7079 7a73 7464 202d 2d68 656c 7060 602e  pyzstd --help``.
+000002f0: 0a0a 4c69 6e6b 733a 2060 4769 7448 7562  ..Links: `GitHub
+00000300: 2070 6167 6520 3c68 7474 7073 3a2f 2f67   page <https://g
+00000310: 6974 6875 622e 636f 6d2f 616e 696d 616c  ithub.com/animal
+00000320: 697a 652f 7079 7a73 7464 3e60 5f2c 2060  ize/pyzstd>`_, `
+00000330: 5079 5049 2070 6167 6520 3c68 7474 7073  PyPI page <https
+00000340: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000350: 6563 742f 7079 7a73 7464 3e60 5f2e 0a0a  ect/pyzstd>`_...
+00000360: 4665 6174 7572 6573 206f 6620 7a73 7464  Features of zstd
+00000370: 3a0a 0a2a 2046 6173 7420 636f 6d70 7265  :..* Fast compre
+00000380: 7373 696f 6e20 616e 6420 6465 636f 6d70  ssion and decomp
+00000390: 7265 7373 696f 6e20 7370 6565 642e 0a2a  ression speed..*
+000003a0: 2049 6620 7573 6520 3a72 6566 3a60 6d75   If use :ref:`mu
+000003b0: 6c74 692d 7468 7265 6164 6564 2063 6f6d  lti-threaded com
+000003c0: 7072 6573 7369 6f6e 3c6d 745f 636f 6d70  pression<mt_comp
+000003d0: 7265 7373 696f 6e3e 602c 2074 6865 2063  ression>`, the c
+000003e0: 6f6d 7072 6573 7369 6f6e 2073 7065 6564  ompression speed
+000003f0: 2069 6d70 726f 7665 7320 7369 676e 6966   improves signif
+00000400: 6963 616e 746c 792e 0a2a 2049 6620 7573  icantly..* If us
+00000410: 6520 7072 652d 7472 6169 6e65 6420 3a72  e pre-trained :r
+00000420: 6566 3a60 6469 6374 696f 6e61 7279 3c7a  ef:`dictionary<z
+00000430: 7374 645f 6469 6374 3e60 2c20 7468 6520  std_dict>`, the 
+00000440: 636f 6d70 7265 7373 696f 6e20 7261 7469  compression rati
+00000450: 6f20 6f6e 2073 6d61 6c6c 2064 6174 6120  o on small data 
+00000460: 2861 2066 6577 204b 6942 2920 696d 7072  (a few KiB) impr
+00000470: 6f76 6573 2064 7261 6d61 7469 6361 6c6c  oves dramaticall
+00000480: 792e 0a2a 203a 7265 663a 6046 7261 6d65  y..* :ref:`Frame
+00000490: 2061 6e64 2062 6c6f 636b 3c66 7261 6d65   and block<frame
+000004a0: 5f62 6c6f 636b 3e60 2061 6c6c 6f77 2074  _block>` allow t
+000004b0: 6865 2075 7365 206d 6f72 6520 666c 6578  he use more flex
+000004c0: 6962 6c65 2c20 7375 6974 6162 6c65 2066  ible, suitable f
+000004d0: 6f72 206d 616e 7920 7363 656e 6172 696f  or many scenario
+000004e0: 732e 0a2a 2043 616e 2062 6520 7573 6564  s..* Can be used
+000004f0: 2061 7320 6120 3a72 6566 3a60 7061 7463   as a :ref:`patc
+00000500: 6869 6e67 2065 6e67 696e 653c 7061 7463  hing engine<patc
+00000510: 6869 6e67 5f65 6e67 696e 653e 602e 0a0a  hing_engine>`...
+00000520: 2e2e 206e 6f74 653a 3a0a 2020 2020 5477  .. note::.    Tw
+00000530: 6f20 6f74 6865 7220 7a73 7464 206d 6f64  o other zstd mod
+00000540: 756c 6573 206f 6e20 5079 5049 3a0a 0a20  ules on PyPI:.. 
+00000550: 2020 202a 2060 7a73 7464 203c 6874 7470     * `zstd <http
+00000560: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000570: 6a65 6374 2f7a 7374 642f 3e60 5f2c 2061  ject/zstd/>`_, a
+00000580: 2076 6572 7920 7369 6d70 6c65 206d 6f64   very simple mod
+00000590: 756c 652e 0a20 2020 202a 2060 7a73 7461  ule..    * `zsta
+000005a0: 6e64 6172 6420 3c68 7474 7073 3a2f 2f70  ndard <https://p
+000005b0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000005c0: 7a73 7461 6e64 6172 642f 3e60 5f2c 2070  zstandard/>`_, p
+000005d0: 726f 7669 6465 7320 7269 6368 2041 5049  rovides rich API
+000005e0: 2e0a 0a45 7863 6570 7469 6f6e 0a2d 2d2d  ...Exception.---
+000005f0: 2d2d 2d2d 2d2d 0a0a 2e2e 2070 793a 6578  ------.... py:ex
+00000600: 6365 7074 696f 6e3a 3a20 5a73 7464 4572  ception:: ZstdEr
+00000610: 726f 720a 0a20 2020 2054 6869 7320 6578  ror..    This ex
+00000620: 6365 7074 696f 6e20 6973 2072 6169 7365  ception is raise
+00000630: 6420 7768 656e 2061 6e20 6572 726f 7220  d when an error 
+00000640: 6f63 6375 7273 2077 6865 6e20 6361 6c6c  occurs when call
+00000650: 696e 6720 7468 6520 756e 6465 726c 7969  ing the underlyi
+00000660: 6e67 207a 7374 6420 6c69 6272 6172 792e  ng zstd library.
+00000670: 2053 7562 636c 6173 7320 6f66 2060 6045   Subclass of ``E
+00000680: 7863 6570 7469 6f6e 6060 2e0a 0a0a 5369  xception``....Si
+00000690: 6d70 6c65 2063 6f6d 7072 6573 7369 6f6e  mple compression
+000006a0: 2f64 6563 6f6d 7072 6573 7369 6f6e 0a2d  /decompression.-
+000006b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+000006d0: 0a20 2020 2054 6869 7320 7365 6374 696f  .    This sectio
+000006e0: 6e20 636f 6e74 6169 6e73 3a0a 0a20 2020  n contains:..   
+000006f0: 2020 2020 202a 2066 756e 6374 696f 6e20       * function 
+00000700: 3a70 793a 6675 6e63 3a60 636f 6d70 7265  :py:func:`compre
+00000710: 7373 600a 2020 2020 2020 2020 2a20 6675  ss`.        * fu
+00000720: 6e63 7469 6f6e 203a 7079 3a66 756e 633a  nction :py:func:
+00000730: 6064 6563 6f6d 7072 6573 7360 0a0a 2020  `decompress`..  
+00000740: 2020 2e2e 2068 696e 743a 3a0a 2020 2020    .. hint::.    
+00000750: 2020 2020 4966 2074 6865 7265 2061 7265      If there are
+00000760: 2061 2062 6967 206e 756d 6265 7220 6f66   a big number of
+00000770: 2073 616d 6520 7479 7065 2069 6e64 6976   same type indiv
+00000780: 6964 7561 6c20 6461 7461 2c20 7265 7573  idual data, reus
+00000790: 6520 7468 6573 6520 6f62 6a65 6374 7320  e these objects 
+000007a0: 6d61 7920 656c 696d 696e 6174 6520 7468  may eliminate th
+000007b0: 6520 736d 616c 6c20 6f76 6572 6865 6164  e small overhead
+000007c0: 206f 6620 6372 6561 7469 6e67 2063 6f6e   of creating con
+000007d0: 7465 7874 202f 2073 6574 7469 6e67 2070  text / setting p
+000007e0: 6172 616d 6574 6572 7320 2f20 6c6f 6164  arameters / load
+000007f0: 696e 6720 6469 6374 696f 6e61 7279 2e0a  ing dictionary..
+00000800: 0a20 2020 2020 2020 202a 203a 7079 3a63  .        * :py:c
+00000810: 6c61 7373 3a60 5a73 7464 436f 6d70 7265  lass:`ZstdCompre
+00000820: 7373 6f72 600a 2020 2020 2020 2020 2a20  ssor`.        * 
+00000830: 3a70 793a 636c 6173 733a 6052 6963 684d  :py:class:`RichM
+00000840: 656d 5a73 7464 436f 6d70 7265 7373 6f72  emZstdCompressor
+00000850: 600a 0a0a 2e2e 2070 793a 6675 6e63 7469  `..... py:functi
+00000860: 6f6e 3a3a 2063 6f6d 7072 6573 7328 6461  on:: compress(da
+00000870: 7461 2c20 6c65 7665 6c5f 6f72 5f6f 7074  ta, level_or_opt
+00000880: 696f 6e3d 4e6f 6e65 2c20 7a73 7464 5f64  ion=None, zstd_d
+00000890: 6963 743d 4e6f 6e65 290a 0a20 2020 2043  ict=None)..    C
+000008a0: 6f6d 7072 6573 7320 2a64 6174 612a 2c20  ompress *data*, 
+000008b0: 7265 7475 726e 2074 6865 2063 6f6d 7072  return the compr
+000008c0: 6573 7365 6420 6461 7461 2e0a 0a20 2020  essed data...   
+000008d0: 2043 6f6d 7072 6573 7369 6e67 2060 6062   Compressing ``b
+000008e0: 2727 6060 2077 696c 6c20 6765 7420 616e  ''`` will get an
+000008f0: 2065 6d70 7479 2063 6f6e 7465 6e74 2066   empty content f
+00000900: 7261 6d65 2028 3920 6279 7465 7320 6f72  rame (9 bytes or
+00000910: 206d 6f72 6529 2e0a 0a20 2020 203a 7079   more)...    :py
+00000920: 3a66 756e 633a 6072 6963 686d 656d 5f63  :func:`richmem_c
+00000930: 6f6d 7072 6573 7360 2066 756e 6374 696f  ompress` functio
+00000940: 6e20 6973 2066 6173 7465 7220 696e 2073  n is faster in s
+00000950: 6f6d 6520 6361 7365 732e 0a0a 2020 2020  ome cases...    
+00000960: 3a70 6172 616d 2064 6174 613a 2044 6174  :param data: Dat
+00000970: 6120 746f 2062 6520 636f 6d70 7265 7373  a to be compress
+00000980: 6564 2e0a 2020 2020 3a74 7970 6520 6461  ed..    :type da
+00000990: 7461 3a20 6279 7465 732d 6c69 6b65 206f  ta: bytes-like o
+000009a0: 626a 6563 740a 2020 2020 3a70 6172 616d  bject.    :param
+000009b0: 206c 6576 656c 5f6f 725f 6f70 7469 6f6e   level_or_option
+000009c0: 3a20 5768 656e 2069 7427 7320 616e 2060  : When it's an `
+000009d0: 6069 6e74 6060 206f 626a 6563 742c 2069  `int`` object, i
+000009e0: 7420 7265 7072 6573 656e 7473 203a 7265  t represents :re
+000009f0: 663a 6063 6f6d 7072 6573 7369 6f6e 206c  f:`compression l
+00000a00: 6576 656c 3c63 6f6d 7072 6573 7369 6f6e  evel<compression
+00000a10: 5f6c 6576 656c 3e60 2e20 5768 656e 2069  _level>`. When i
+00000a20: 7427 7320 6120 6060 6469 6374 6060 206f  t's a ``dict`` o
+00000a30: 626a 6563 742c 2069 7420 636f 6e74 6169  bject, it contai
+00000a40: 6e73 203a 7265 663a 6061 6476 616e 6365  ns :ref:`advance
+00000a50: 6420 636f 6d70 7265 7373 696f 6e20 7061  d compression pa
+00000a60: 7261 6d65 7465 7273 3c43 5061 7261 6d65  rameters<CParame
+00000a70: 7465 723e 602e 2054 6865 2064 6566 6175  ter>`. The defau
+00000a80: 6c74 2076 616c 7565 2060 604e 6f6e 6560  lt value ``None`
+00000a90: 6020 6d65 616e 7320 746f 2075 7365 207a  ` means to use z
+00000aa0: 7374 6427 7320 6465 6661 756c 7420 636f  std's default co
+00000ab0: 6d70 7265 7373 696f 6e20 6c65 7665 6c2f  mpression level/
+00000ac0: 7061 7261 6d65 7465 7273 2e0a 2020 2020  parameters..    
+00000ad0: 3a74 7970 6520 6c65 7665 6c5f 6f72 5f6f  :type level_or_o
+00000ae0: 7074 696f 6e3a 2069 6e74 206f 7220 6469  ption: int or di
+00000af0: 6374 0a20 2020 203a 7061 7261 6d20 7a73  ct.    :param zs
+00000b00: 7464 5f64 6963 743a 2050 7265 2d74 7261  td_dict: Pre-tra
+00000b10: 696e 6564 2064 6963 7469 6f6e 6172 7920  ined dictionary 
+00000b20: 666f 7220 636f 6d70 7265 7373 696f 6e2e  for compression.
+00000b30: 0a20 2020 203a 7479 7065 207a 7374 645f  .    :type zstd_
+00000b40: 6469 6374 3a20 5a73 7464 4469 6374 0a20  dict: ZstdDict. 
+00000b50: 2020 203a 7265 7475 726e 3a20 436f 6d70     :return: Comp
+00000b60: 7265 7373 6564 2064 6174 610a 2020 2020  ressed data.    
+00000b70: 3a72 7479 7065 3a20 6279 7465 730a 0a2e  :rtype: bytes...
+00000b80: 2e20 736f 7572 6365 636f 6465 3a3a 2070  . sourcecode:: p
+00000b90: 7974 686f 6e0a 0a20 2020 2023 2069 6e74  ython..    # int
+00000ba0: 2063 6f6d 7072 6573 7369 6f6e 206c 6576   compression lev
+00000bb0: 656c 0a20 2020 2063 6f6d 7072 6573 7365  el.    compresse
+00000bc0: 645f 6461 7420 3d20 636f 6d70 7265 7373  d_dat = compress
+00000bd0: 2872 6177 5f64 6174 2c20 3130 290a 0a20  (raw_dat, 10).. 
+00000be0: 2020 2023 2064 6963 7420 6f70 7469 6f6e     # dict option
+00000bf0: 2c20 7573 6520 3620 7468 7265 6164 7320  , use 6 threads 
+00000c00: 746f 2063 6f6d 7072 6573 732c 2061 6e64  to compress, and
+00000c10: 2061 7070 656e 6420 6120 342d 6279 7465   append a 4-byte
+00000c20: 2063 6865 636b 7375 6d2e 0a20 2020 206f   checksum..    o
+00000c30: 7074 696f 6e20 3d20 7b43 5061 7261 6d65  ption = {CParame
+00000c40: 7465 722e 636f 6d70 7265 7373 696f 6e4c  ter.compressionL
+00000c50: 6576 656c 203a 2031 302c 0a20 2020 2020  evel : 10,.     
+00000c60: 2020 2020 2020 2020 2043 5061 7261 6d65           CParame
+00000c70: 7465 722e 6e62 576f 726b 6572 7320 3a20  ter.nbWorkers : 
+00000c80: 362c 0a20 2020 2020 2020 2020 2020 2020  6,.             
+00000c90: 2043 5061 7261 6d65 7465 722e 6368 6563   CParameter.chec
+00000ca0: 6b73 756d 466c 6167 203a 2031 7d0a 2020  ksumFlag : 1}.  
+00000cb0: 2020 636f 6d70 7265 7373 6564 5f64 6174    compressed_dat
+00000cc0: 203d 2063 6f6d 7072 6573 7328 7261 775f   = compress(raw_
+00000cd0: 6461 742c 206f 7074 696f 6e29 0a0a 0a2e  dat, option)....
+00000ce0: 2e20 7079 3a66 756e 6374 696f 6e3a 3a20  . py:function:: 
+00000cf0: 6465 636f 6d70 7265 7373 2864 6174 612c  decompress(data,
+00000d00: 207a 7374 645f 6469 6374 3d4e 6f6e 652c   zstd_dict=None,
+00000d10: 206f 7074 696f 6e3d 4e6f 6e65 290a 0a20   option=None).. 
+00000d20: 2020 2044 6563 6f6d 7072 6573 7320 2a64     Decompress *d
+00000d30: 6174 612a 2c20 7265 7475 726e 2074 6865  ata*, return the
+00000d40: 2064 6563 6f6d 7072 6573 7365 6420 6461   decompressed da
+00000d50: 7461 2e0a 0a20 2020 2053 7570 706f 7274  ta...    Support
+00000d60: 206d 756c 7469 706c 6520 636f 6e63 6174   multiple concat
+00000d70: 656e 6174 6564 203a 7265 663a 6066 7261  enated :ref:`fra
+00000d80: 6d65 733c 6672 616d 655f 626c 6f63 6b3e  mes<frame_block>
+00000d90: 602e 0a0a 2020 2020 3a70 6172 616d 2064  `...    :param d
+00000da0: 6174 613a 2044 6174 6120 746f 2062 6520  ata: Data to be 
+00000db0: 6465 636f 6d70 7265 7373 6564 2e0a 2020  decompressed..  
+00000dc0: 2020 3a74 7970 6520 6461 7461 3a20 6279    :type data: by
+00000dd0: 7465 732d 6c69 6b65 206f 626a 6563 740a  tes-like object.
+00000de0: 2020 2020 3a70 6172 616d 207a 7374 645f      :param zstd_
+00000df0: 6469 6374 3a20 5072 652d 7472 6169 6e65  dict: Pre-traine
+00000e00: 6420 6469 6374 696f 6e61 7279 2066 6f72  d dictionary for
+00000e10: 2064 6563 6f6d 7072 6573 7369 6f6e 2e0a   decompression..
+00000e20: 2020 2020 3a74 7970 6520 7a73 7464 5f64      :type zstd_d
+00000e30: 6963 743a 205a 7374 6444 6963 740a 2020  ict: ZstdDict.  
+00000e40: 2020 3a70 6172 616d 206f 7074 696f 6e3a    :param option:
+00000e50: 2041 2060 6064 6963 7460 6020 6f62 6a65   A ``dict`` obje
+00000e60: 6374 2074 6861 7420 636f 6e74 6169 6e73  ct that contains
+00000e70: 203a 7079 3a72 6566 3a60 6164 7661 6e63   :py:ref:`advanc
+00000e80: 6564 2064 6563 6f6d 7072 6573 7369 6f6e  ed decompression
+00000e90: 2070 6172 616d 6574 6572 733c 4450 6172   parameters<DPar
+00000ea0: 616d 6574 6572 3e60 2e20 5468 6520 6465  ameter>`. The de
+00000eb0: 6661 756c 7420 7661 6c75 6520 6060 4e6f  fault value ``No
+00000ec0: 6e65 6060 206d 6561 6e73 2074 6f20 7573  ne`` means to us
+00000ed0: 6520 7a73 7464 2773 2064 6566 6175 6c74  e zstd's default
+00000ee0: 2064 6563 6f6d 7072 6573 7369 6f6e 2070   decompression p
+00000ef0: 6172 616d 6574 6572 732e 0a20 2020 203a  arameters..    :
+00000f00: 7479 7065 206f 7074 696f 6e3a 2064 6963  type option: dic
+00000f10: 740a 2020 2020 3a72 6574 7572 6e3a 2044  t.    :return: D
+00000f20: 6563 6f6d 7072 6573 7365 6420 6461 7461  ecompressed data
+00000f30: 0a20 2020 203a 7274 7970 653a 2062 7974  .    :rtype: byt
+00000f40: 6573 0a20 2020 203a 7261 6973 6573 205a  es.    :raises Z
+00000f50: 7374 6445 7272 6f72 3a20 4966 2064 6563  stdError: If dec
+00000f60: 6f6d 7072 6573 7369 6f6e 2066 6169 6c73  ompression fails
+00000f70: 2e0a 0a0a 5269 6368 206d 656d 6f72 7920  ....Rich memory 
+00000f80: 636f 6d70 7265 7373 696f 6e0a 2d2d 2d2d  compression.----
+00000f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000fa0: 2d2d 2d0a 0a20 2020 2043 6f6d 7072 6573  ---..    Compres
+00000fb0: 7320 6461 7461 2075 7369 6e67 203a 7265  s data using :re
+00000fc0: 663a 6072 6963 6820 6d65 6d6f 7279 206d  f:`rich memory m
+00000fd0: 6f64 653c 7269 6368 5f6d 656d 3e60 2e20  ode<rich_mem>`. 
+00000fe0: 5468 6973 206d 6f64 6520 616c 6c6f 6361  This mode alloca
+00000ff0: 7465 7320 6d6f 7265 206d 656d 6f72 7920  tes more memory 
+00001000: 666f 7220 6f75 7470 7574 2062 7566 6665  for output buffe
+00001010: 722c 2069 7427 7320 6661 7374 6572 2069  r, it's faster i
+00001020: 6e20 736f 6d65 2063 6173 6573 2e0a 0a20  n some cases... 
+00001030: 2020 2054 6869 7320 7365 6374 696f 6e20     This section 
+00001040: 636f 6e74 6169 6e73 3a0a 0a20 2020 2020  contains:..     
+00001050: 2020 202a 2066 756e 6374 696f 6e20 3a70     * function :p
+00001060: 793a 6675 6e63 3a60 7269 6368 6d65 6d5f  y:func:`richmem_
+00001070: 636f 6d70 7265 7373 600a 2020 2020 2020  compress`.      
+00001080: 2020 2a20 636c 6173 7320 3a70 793a 636c    * class :py:cl
+00001090: 6173 733a 6052 6963 684d 656d 5a73 7464  ass:`RichMemZstd
+000010a0: 436f 6d70 7265 7373 6f72 602c 2061 2072  Compressor`, a r
+000010b0: 6575 7361 626c 6520 636f 6d70 7265 7373  eusable compress
+000010c0: 6f72 2e0a 0a2e 2e20 7079 3a66 756e 6374  or..... py:funct
+000010d0: 696f 6e3a 3a20 7269 6368 6d65 6d5f 636f  ion:: richmem_co
+000010e0: 6d70 7265 7373 2864 6174 612c 206c 6576  mpress(data, lev
+000010f0: 656c 5f6f 725f 6f70 7469 6f6e 3d4e 6f6e  el_or_option=Non
+00001100: 652c 207a 7374 645f 6469 6374 3d4e 6f6e  e, zstd_dict=Non
+00001110: 6529 0a0a 2020 2020 5573 6520 3a72 6566  e)..    Use :ref
+00001120: 3a60 7269 6368 206d 656d 6f72 7920 6d6f  :`rich memory mo
+00001130: 6465 3c72 6963 685f 6d65 6d3e 6020 746f  de<rich_mem>` to
+00001140: 2063 6f6d 7072 6573 7320 2a64 6174 612a   compress *data*
+00001150: 2e20 4974 2773 2066 6173 7465 7220 7468  . It's faster th
+00001160: 616e 203a 7079 3a66 756e 633a 6063 6f6d  an :py:func:`com
+00001170: 7072 6573 7360 2069 6e20 736f 6d65 2063  press` in some c
+00001180: 6173 6573 2c20 6275 7420 616c 6c6f 6361  ases, but alloca
+00001190: 7465 7320 6d6f 7265 206d 656d 6f72 792e  tes more memory.
+000011a0: 0a0a 2020 2020 5468 6520 7061 7261 6d65  ..    The parame
+000011b0: 7465 7273 2061 7265 2074 6865 2073 616d  ters are the sam
+000011c0: 6520 6173 203a 7079 3a66 756e 633a 6063  e as :py:func:`c
+000011d0: 6f6d 7072 6573 7360 2066 756e 6374 696f  ompress` functio
+000011e0: 6e2e 0a0a 2020 2020 436f 6d70 7265 7373  n...    Compress
+000011f0: 696e 6720 6060 6227 2760 6020 7769 6c6c  ing ``b''`` will
+00001200: 2067 6574 2061 6e20 656d 7074 7920 636f   get an empty co
+00001210: 6e74 656e 7420 6672 616d 6520 2839 2062  ntent frame (9 b
+00001220: 7974 6573 206f 7220 6d6f 7265 292e 0a0a  ytes or more)...
+00001230: 0a2e 2e20 7079 3a63 6c61 7373 3a3a 2052  ... py:class:: R
+00001240: 6963 684d 656d 5a73 7464 436f 6d70 7265  ichMemZstdCompre
+00001250: 7373 6f72 0a0a 2020 2020 4120 7265 7573  ssor..    A reus
+00001260: 6162 6c65 2063 6f6d 7072 6573 736f 7220  able compressor 
+00001270: 7573 696e 6720 3a72 6566 3a60 7269 6368  using :ref:`rich
+00001280: 206d 656d 6f72 7920 6d6f 6465 3c72 6963   memory mode<ric
+00001290: 685f 6d65 6d3e 602e 2049 7420 6361 6e20  h_mem>`. It can 
+000012a0: 6265 2072 6575 7365 6420 666f 7220 6269  be reused for bi
+000012b0: 6720 6e75 6d62 6572 206f 6620 7361 6d65  g number of same
+000012c0: 2074 7970 6520 696e 6469 7669 6475 616c   type individual
+000012d0: 2064 6174 612e 0a0a 2020 2020 5369 6e63   data...    Sinc
+000012e0: 6520 6974 2063 616e 206f 6e6c 7920 6765  e it can only ge
+000012f0: 6e65 7261 7465 7320 696e 6469 7669 6475  nerates individu
+00001300: 616c 203a 7265 663a 6066 7261 6d65 733c  al :ref:`frames<
+00001310: 6672 616d 655f 626c 6f63 6b3e 602c 2069  frame_block>`, i
+00001320: 7427 7320 6e6f 7420 7375 6974 6162 6c65  t's not suitable
+00001330: 2066 6f72 2073 7472 6561 6d69 6e67 2063   for streaming c
+00001340: 6f6d 7072 6573 7369 6f6e 2c20 6f74 6865  ompression, othe
+00001350: 7277 6973 6520 7468 6520 636f 6d70 7265  rwise the compre
+00001360: 7373 696f 6e20 7261 7469 6f20 7769 6c6c  ssion ratio will
+00001370: 2062 6520 7265 6475 6365 642c 2061 6e64   be reduced, and
+00001380: 2073 6f6d 6520 7072 6f67 7261 6d73 2063   some programs c
+00001390: 616e 2774 2064 6563 6f6d 7072 6573 7320  an't decompress 
+000013a0: 6d75 6c74 6970 6c65 2066 7261 6d65 7320  multiple frames 
+000013b0: 6461 7461 2e20 466f 7220 7374 7265 616d  data. For stream
+000013c0: 696e 6720 636f 6d70 7265 7373 696f 6e2c  ing compression,
+000013d0: 2073 6565 203a 7265 663a 6074 6869 7320   see :ref:`this 
+000013e0: 7365 6374 696f 6e3c 7374 7265 616d 5f63  section<stream_c
+000013f0: 6f6d 7072 6573 7369 6f6e 3e60 2e0a 0a20  ompression>`... 
+00001400: 2020 2054 6872 6561 642d 7361 6665 2061     Thread-safe a
+00001410: 7420 6d65 7468 6f64 206c 6576 656c 2e0a  t method level..
+00001420: 0a20 2020 202e 2e20 7079 3a6d 6574 686f  .    .. py:metho
+00001430: 643a 3a20 5f5f 696e 6974 5f5f 2873 656c  d:: __init__(sel
+00001440: 662c 206c 6576 656c 5f6f 725f 6f70 7469  f, level_or_opti
+00001450: 6f6e 3d4e 6f6e 652c 207a 7374 645f 6469  on=None, zstd_di
+00001460: 6374 3d4e 6f6e 6529 0a0a 2020 2020 2020  ct=None)..      
+00001470: 2020 5468 6520 7061 7261 6d65 7465 7273    The parameters
+00001480: 2061 7265 2074 6865 2073 616d 6520 6173   are the same as
+00001490: 203a 7079 3a6d 6574 683a 605a 7374 6443   :py:meth:`ZstdC
+000014a0: 6f6d 7072 6573 736f 722e 5f5f 696e 6974  ompressor.__init
+000014b0: 5f5f 6020 6d65 7468 6f64 2e0a 0a20 2020  __` method...   
+000014c0: 202e 2e20 7079 3a6d 6574 686f 643a 3a20   .. py:method:: 
+000014d0: 636f 6d70 7265 7373 2873 656c 662c 2064  compress(self, d
+000014e0: 6174 6129 0a0a 2020 2020 2020 2020 436f  ata)..        Co
+000014f0: 6d70 7265 7373 202a 6461 7461 2a20 7573  mpress *data* us
+00001500: 696e 6720 3a72 6566 3a60 7269 6368 206d  ing :ref:`rich m
+00001510: 656d 6f72 7920 6d6f 6465 3c72 6963 685f  emory mode<rich_
+00001520: 6d65 6d3e 602c 2072 6574 7572 6e20 6120  mem>`, return a 
+00001530: 7369 6e67 6c65 207a 7374 6420 3a72 6566  single zstd :ref
+00001540: 3a60 6672 616d 653c 6672 616d 655f 626c  :`frame<frame_bl
+00001550: 6f63 6b3e 602e 0a0a 2020 2020 2020 2020  ock>`...        
+00001560: 436f 6d70 7265 7373 696e 6720 6060 6227  Compressing ``b'
+00001570: 2760 6020 7769 6c6c 2067 6574 2061 6e20  '`` will get an 
+00001580: 656d 7074 7920 636f 6e74 656e 7420 6672  empty content fr
+00001590: 616d 6520 2839 2062 7974 6573 206f 7220  ame (9 bytes or 
+000015a0: 6d6f 7265 292e 0a0a 2020 2020 2020 2020  more)...        
+000015b0: 3a70 6172 616d 2064 6174 613a 2044 6174  :param data: Dat
+000015c0: 6120 746f 2062 6520 636f 6d70 7265 7373  a to be compress
+000015d0: 6564 2e0a 2020 2020 2020 2020 3a74 7970  ed..        :typ
+000015e0: 6520 6461 7461 3a20 6279 7465 732d 6c69  e data: bytes-li
+000015f0: 6b65 206f 626a 6563 740a 2020 2020 2020  ke object.      
+00001600: 2020 3a72 6574 7572 6e3a 2041 2073 696e    :return: A sin
+00001610: 676c 6520 7a73 7464 2066 7261 6d65 2e0a  gle zstd frame..
+00001620: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00001630: 6279 7465 730a 0a20 2020 202e 2e20 736f  bytes..    .. so
+00001640: 7572 6365 636f 6465 3a3a 2070 7974 686f  urcecode:: pytho
+00001650: 6e0a 0a20 2020 2020 2020 2063 203d 2052  n..        c = R
+00001660: 6963 684d 656d 5a73 7464 436f 6d70 7265  ichMemZstdCompre
+00001670: 7373 6f72 2829 0a20 2020 2020 2020 2066  ssor().        f
+00001680: 7261 6d65 3120 3d20 632e 636f 6d70 7265  rame1 = c.compre
+00001690: 7373 2872 6177 5f64 6174 3129 0a20 2020  ss(raw_dat1).   
+000016a0: 2020 2020 2066 7261 6d65 3220 3d20 632e       frame2 = c.
+000016b0: 636f 6d70 7265 7373 2872 6177 5f64 6174  compress(raw_dat
+000016c0: 3229 0a0a 0a2e 2e20 5f73 7472 6561 6d5f  2)..... _stream_
+000016d0: 636f 6d70 7265 7373 696f 6e3a 0a0a 5374  compression:..St
+000016e0: 7265 616d 696e 6720 636f 6d70 7265 7373  reaming compress
+000016f0: 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ion.------------
+00001700: 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020 2054  ---------..    T
+00001710: 6869 7320 7365 6374 696f 6e20 636f 6e74  his section cont
+00001720: 6169 6e73 3a0a 0a20 2020 2020 2020 202a  ains:..        *
+00001730: 2066 756e 6374 696f 6e20 3a70 793a 6675   function :py:fu
+00001740: 6e63 3a60 636f 6d70 7265 7373 5f73 7472  nc:`compress_str
+00001750: 6561 6d60 2c20 6120 6661 7374 2061 6e64  eam`, a fast and
+00001760: 2063 6f6e 7665 6e69 656e 7420 6675 6e63   convenient func
+00001770: 7469 6f6e 2e0a 2020 2020 2020 2020 2a20  tion..        * 
+00001780: 636c 6173 7320 3a70 793a 636c 6173 733a  class :py:class:
+00001790: 605a 7374 6443 6f6d 7072 6573 736f 7260  `ZstdCompressor`
+000017a0: 2c20 7369 6d69 6c61 7220 746f 2063 6f6d  , similar to com
+000017b0: 7072 6573 736f 7273 2069 6e20 5079 7468  pressors in Pyth
+000017c0: 6f6e 2073 7461 6e64 6172 6420 6c69 6272  on standard libr
+000017d0: 6172 792e 0a0a 2020 2020 4974 2077 6f75  ary...    It wou
+000017e0: 6c64 2062 6520 6e69 6365 2074 6f20 6b6e  ld be nice to kn
+000017f0: 6f77 2073 6f6d 6520 6b6e 6f77 6c65 6467  ow some knowledg
+00001800: 6520 6162 6f75 7420 7a73 7464 2064 6174  e about zstd dat
+00001810: 612c 2073 6565 203a 7265 663a 6066 7261  a, see :ref:`fra
+00001820: 6d65 2061 6e64 2062 6c6f 636b 3c66 7261  me and block<fra
+00001830: 6d65 5f62 6c6f 636b 3e60 2e0a 0a2e 2e20  me_block>`..... 
+00001840: 7079 3a66 756e 6374 696f 6e3a 3a20 636f  py:function:: co
+00001850: 6d70 7265 7373 5f73 7472 6561 6d28 696e  mpress_stream(in
+00001860: 7075 745f 7374 7265 616d 2c20 6f75 7470  put_stream, outp
+00001870: 7574 5f73 7472 6561 6d2c 202a 2c20 6c65  ut_stream, *, le
+00001880: 7665 6c5f 6f72 5f6f 7074 696f 6e3d 4e6f  vel_or_option=No
+00001890: 6e65 2c20 7a73 7464 5f64 6963 743d 4e6f  ne, zstd_dict=No
+000018a0: 6e65 2c20 706c 6564 6765 645f 696e 7075  ne, pledged_inpu
+000018b0: 745f 7369 7a65 3d4e 6f6e 652c 2072 6561  t_size=None, rea
+000018c0: 645f 7369 7a65 3d31 3331 5f30 3732 2c20  d_size=131_072, 
+000018d0: 7772 6974 655f 7369 7a65 3d31 3331 5f35  write_size=131_5
+000018e0: 3931 2c20 6361 6c6c 6261 636b 3d4e 6f6e  91, callback=Non
+000018f0: 6529 0a0a 2020 2020 4120 6661 7374 2061  e)..    A fast a
+00001900: 6e64 2063 6f6e 7665 6e69 656e 7420 6675  nd convenient fu
+00001910: 6e63 7469 6f6e 2c20 636f 6d70 7265 7373  nction, compress
+00001920: 6573 202a 696e 7075 745f 7374 7265 616d  es *input_stream
+00001930: 2a20 616e 6420 7772 6974 6573 2074 6865  * and writes the
+00001940: 2063 6f6d 7072 6573 7365 6420 6461 7461   compressed data
+00001950: 2074 6f20 2a6f 7574 7075 745f 7374 7265   to *output_stre
+00001960: 616d 2a2c 2069 7420 646f 6573 6e27 7420  am*, it doesn't 
+00001970: 636c 6f73 6520 7468 6520 7374 7265 616d  close the stream
+00001980: 732e 0a0a 2020 2020 4966 2069 6e70 7574  s...    If input
+00001990: 2073 7472 6561 6d20 6973 2060 6062 2727   stream is ``b''
+000019a0: 6060 2c20 6e6f 7468 696e 6720 7769 6c6c  ``, nothing will
+000019b0: 2062 6520 7772 6974 7465 6e20 746f 206f   be written to o
+000019c0: 7574 7075 7420 7374 7265 616d 2e0a 0a20  utput stream... 
+000019d0: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+000019e0: 2074 7269 6573 2074 6f20 7a65 726f 2d63   tries to zero-c
+000019f0: 6f70 7920 6173 206d 7563 6820 6173 2070  opy as much as p
+00001a00: 6f73 7369 626c 652e 2049 6620 7468 6520  ossible. If the 
+00001a10: 4f53 2068 6173 2072 6561 6420 7072 6566  OS has read pref
+00001a20: 6574 6368 696e 6720 616e 6420 7772 6974  etching and writ
+00001a30: 6520 6275 6666 6572 2c20 6974 206d 6179  e buffer, it may
+00001a40: 2070 6572 666f 726d 2074 6865 2074 6173   perform the tas
+00001a50: 6b73 2028 7265 6164 2f63 6f6d 7072 6573  ks (read/compres
+00001a60: 732f 7772 6974 6529 2069 6e20 7061 7261  s/write) in para
+00001a70: 6c6c 656c 2074 6f20 736f 6d65 2064 6567  llel to some deg
+00001a80: 7265 652e 0a0a 2020 2020 5468 6520 6465  ree...    The de
+00001a90: 6661 756c 7420 7661 6c75 6573 206f 6620  fault values of 
+00001aa0: 2a72 6561 645f 7369 7a65 2a20 616e 6420  *read_size* and 
+00001ab0: 2a77 7269 7465 5f73 697a 652a 2070 6172  *write_size* par
+00001ac0: 616d 6574 6572 7320 6172 6520 7468 6520  ameters are the 
+00001ad0: 6275 6666 6572 2073 697a 6573 2072 6563  buffer sizes rec
+00001ae0: 6f6d 6d65 6e64 6564 2062 7920 7a73 7464  ommended by zstd
+00001af0: 2c20 696e 6372 6561 7369 6e67 2074 6865  , increasing the
+00001b00: 6d20 6d61 7920 6265 2066 6173 7465 722c  m may be faster,
+00001b10: 2061 6e64 2072 6564 7563 6573 2074 6865   and reduces the
+00001b20: 206e 756d 6265 7220 6f66 2063 616c 6c62   number of callb
+00001b30: 6163 6b20 6675 6e63 7469 6f6e 2063 616c  ack function cal
+00001b40: 6c73 2e0a 0a20 2020 202e 2e20 7665 7273  ls...    .. vers
+00001b50: 696f 6e61 6464 6564 3a3a 2030 2e31 342e  ionadded:: 0.14.
+00001b60: 320a 0a20 2020 203a 7061 7261 6d20 696e  2..    :param in
+00001b70: 7075 745f 7374 7265 616d 3a20 496e 7075  put_stream: Inpu
+00001b80: 7420 7374 7265 616d 2074 6861 7420 6861  t stream that ha
+00001b90: 7320 6120 602e 7265 6164 696e 746f 2862  s a `.readinto(b
+00001ba0: 2920 3c68 7474 7073 3a2f 2f64 6f63 732e  ) <https://docs.
+00001bb0: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+00001bc0: 7261 7279 2f69 6f2e 6874 6d6c 2369 6f2e  rary/io.html#io.
+00001bd0: 5261 7749 4f42 6173 652e 7265 6164 696e  RawIOBase.readin
+00001be0: 746f 3e60 5f20 6d65 7468 6f64 2e0a 2020  to>`_ method..  
+00001bf0: 2020 3a70 6172 616d 206f 7574 7075 745f    :param output_
+00001c00: 7374 7265 616d 3a20 4f75 7470 7574 2073  stream: Output s
+00001c10: 7472 6561 6d20 7468 6174 2068 6173 2061  tream that has a
+00001c20: 2060 2e77 7269 7465 2862 2920 3c68 7474   `.write(b) <htt
+00001c30: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00001c40: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f69  .org/3/library/i
+00001c50: 6f2e 6874 6d6c 2369 6f2e 5261 7749 4f42  o.html#io.RawIOB
+00001c60: 6173 652e 7772 6974 653e 605f 206d 6574  ase.write>`_ met
+00001c70: 686f 642e 2049 6620 7573 6520 2a63 616c  hod. If use *cal
+00001c80: 6c62 6163 6b2a 2066 756e 6374 696f 6e2c  lback* function,
+00001c90: 2074 6869 7320 7061 7261 6d65 7465 7220   this parameter 
+00001ca0: 6361 6e20 6265 2060 604e 6f6e 6560 602e  can be ``None``.
+00001cb0: 0a20 2020 203a 7061 7261 6d20 6c65 7665  .    :param leve
+00001cc0: 6c5f 6f72 5f6f 7074 696f 6e3a 2057 6865  l_or_option: Whe
+00001cd0: 6e20 6974 2773 2061 6e20 6060 696e 7460  n it's an ``int`
+00001ce0: 6020 6f62 6a65 6374 2c20 6974 2072 6570  ` object, it rep
+00001cf0: 7265 7365 6e74 7320 3a72 6566 3a60 636f  resents :ref:`co
+00001d00: 6d70 7265 7373 696f 6e20 6c65 7665 6c3c  mpression level<
+00001d10: 636f 6d70 7265 7373 696f 6e5f 6c65 7665  compression_leve
+00001d20: 6c3e 602e 2057 6865 6e20 6974 2773 2061  l>`. When it's a
+00001d30: 2060 6064 6963 7460 6020 6f62 6a65 6374   ``dict`` object
+00001d40: 2c20 6974 2063 6f6e 7461 696e 7320 3a72  , it contains :r
+00001d50: 6566 3a60 6164 7661 6e63 6564 2063 6f6d  ef:`advanced com
+00001d60: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
+00001d70: 6572 733c 4350 6172 616d 6574 6572 3e60  ers<CParameter>`
+00001d80: 2e20 5468 6520 6465 6661 756c 7420 7661  . The default va
+00001d90: 6c75 6520 6060 4e6f 6e65 6060 206d 6561  lue ``None`` mea
+00001da0: 6e73 2074 6f20 7573 6520 7a73 7464 2773  ns to use zstd's
+00001db0: 2064 6566 6175 6c74 2063 6f6d 7072 6573   default compres
+00001dc0: 7369 6f6e 206c 6576 656c 2f70 6172 616d  sion level/param
+00001dd0: 6574 6572 732e 0a20 2020 203a 7479 7065  eters..    :type
+00001de0: 206c 6576 656c 5f6f 725f 6f70 7469 6f6e   level_or_option
+00001df0: 3a20 696e 7420 6f72 2064 6963 740a 2020  : int or dict.  
+00001e00: 2020 3a70 6172 616d 207a 7374 645f 6469    :param zstd_di
+00001e10: 6374 3a20 5072 652d 7472 6169 6e65 6420  ct: Pre-trained 
+00001e20: 6469 6374 696f 6e61 7279 2066 6f72 2063  dictionary for c
+00001e30: 6f6d 7072 6573 7369 6f6e 2e0a 2020 2020  ompression..    
+00001e40: 3a74 7970 6520 7a73 7464 5f64 6963 743a  :type zstd_dict:
+00001e50: 205a 7374 6444 6963 740a 2020 2020 3a70   ZstdDict.    :p
+00001e60: 6172 616d 2070 6c65 6467 6564 5f69 6e70  aram pledged_inp
+00001e70: 7574 5f73 697a 653a 2049 6620 7365 7420  ut_size: If set 
+00001e80: 7468 6973 2070 6172 616d 6574 6572 2074  this parameter t
+00001e90: 6f20 7468 6520 7369 7a65 206f 6620 696e  o the size of in
+00001ea0: 7075 7420 6461 7461 2c20 7468 6520 3a72  put data, the :r
+00001eb0: 6566 3a60 7369 7a65 3c63 6f6e 7465 6e74  ef:`size<content
+00001ec0: 5f73 697a 653e 6020 7769 6c6c 2062 6520  _size>` will be 
+00001ed0: 7772 6974 7465 6e20 696e 746f 2074 6865  written into the
+00001ee0: 2066 7261 6d65 2068 6561 6465 722e 2049   frame header. I
+00001ef0: 6620 7468 6520 6163 7475 616c 2069 6e70  f the actual inp
+00001f00: 7574 2064 6174 6120 646f 6573 6e27 7420  ut data doesn't 
+00001f10: 6d61 7463 6820 6974 2c20 6120 3a70 793a  match it, a :py:
+00001f20: 636c 6173 733a 605a 7374 6445 7272 6f72  class:`ZstdError
+00001f30: 6020 6578 6365 7074 696f 6e20 7769 6c6c  ` exception will
+00001f40: 2062 6520 7261 6973 6564 2e20 4974 206d   be raised. It m
+00001f50: 6179 2069 6e63 7265 6173 6520 636f 6d70  ay increase comp
+00001f60: 7265 7373 696f 6e20 7261 7469 6f20 736c  ression ratio sl
+00001f70: 6967 6874 6c79 2c20 616e 6420 6865 6c70  ightly, and help
+00001f80: 2064 6563 6f6d 7072 6573 7369 6f6e 2063   decompression c
+00001f90: 6f64 6520 746f 2061 6c6c 6f63 6174 6520  ode to allocate 
+00001fa0: 6f75 7470 7574 2062 7566 6665 7220 6661  output buffer fa
+00001fb0: 7374 6572 2e0a 2020 2020 3a74 7970 6520  ster..    :type 
+00001fc0: 706c 6564 6765 645f 696e 7075 745f 7369  pledged_input_si
+00001fd0: 7a65 3a20 696e 740a 2020 2020 3a70 6172  ze: int.    :par
+00001fe0: 616d 2072 6561 645f 7369 7a65 3a20 496e  am read_size: In
+00001ff0: 7075 7420 6275 6666 6572 2073 697a 652c  put buffer size,
+00002000: 2069 6e20 6279 7465 732e 0a20 2020 203a   in bytes..    :
+00002010: 7479 7065 2072 6561 645f 7369 7a65 3a20  type read_size: 
+00002020: 696e 740a 2020 2020 3a70 6172 616d 2077  int.    :param w
+00002030: 7269 7465 5f73 697a 653a 204f 7574 7075  rite_size: Outpu
+00002040: 7420 6275 6666 6572 2073 697a 652c 2069  t buffer size, i
+00002050: 6e20 6279 7465 732e 0a20 2020 203a 7479  n bytes..    :ty
+00002060: 7065 2077 7269 7465 5f73 697a 653a 2069  pe write_size: i
+00002070: 6e74 0a20 2020 203a 7061 7261 6d20 6361  nt.    :param ca
+00002080: 6c6c 6261 636b 3a20 4120 6361 6c6c 6261  llback: A callba
+00002090: 636b 2066 756e 6374 696f 6e20 7468 6174  ck function that
+000020a0: 2061 6363 6570 7473 2066 6f75 7220 7061   accepts four pa
+000020b0: 7261 6d65 7465 7273 3a20 6060 2874 6f74  rameters: ``(tot
+000020c0: 616c 5f69 6e70 7574 2c20 746f 7461 6c5f  al_input, total_
+000020d0: 6f75 7470 7574 2c20 7265 6164 5f64 6174  output, read_dat
+000020e0: 612c 2077 7269 7465 5f64 6174 6129 6060  a, write_data)``
+000020f0: 2e20 5468 6520 6669 7273 7420 7477 6f20  . The first two 
+00002100: 6172 6520 6060 696e 7460 6020 6f62 6a65  are ``int`` obje
+00002110: 6374 732e 2054 6865 206c 6173 7420 7477  cts. The last tw
+00002120: 6f20 6172 6520 7265 6164 6f6e 6c79 2060  o are readonly `
+00002130: 6d65 6d6f 7279 7669 6577 203c 6874 7470  memoryview <http
+00002140: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+00002150: 6f72 672f 332f 6c69 6272 6172 792f 7374  org/3/library/st
+00002160: 6474 7970 6573 2e68 746d 6c23 6d65 6d6f  dtypes.html#memo
+00002170: 7279 2d76 6965 7773 3e60 5f20 6f62 6a65  ry-views>`_ obje
+00002180: 6374 732c 2069 6620 7761 6e74 2074 6f20  cts, if want to 
+00002190: 7265 6665 7265 6e63 6520 7468 6520 6461  reference the da
+000021a0: 7461 2028 6f72 2069 7473 2073 6c69 6365  ta (or its slice
+000021b0: 2920 6f75 7473 6964 6520 7468 6520 6361  ) outside the ca
+000021c0: 6c6c 6261 636b 2066 756e 6374 696f 6e2c  llback function,
+000021d0: 2060 636f 6e76 6572 7420 3c68 7474 7073   `convert <https
+000021e0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+000021f0: 7267 2f33 2f6c 6962 7261 7279 2f73 7464  rg/3/library/std
+00002200: 7479 7065 732e 6874 6d6c 236d 656d 6f72  types.html#memor
+00002210: 7976 6965 772e 746f 6279 7465 733e 605f  yview.tobytes>`_
+00002220: 2074 6865 6d20 746f 2060 6062 7974 6573   them to ``bytes
+00002230: 6060 206f 626a 6563 7473 2e20 4966 2069  `` objects. If i
+00002240: 6e70 7574 2073 7472 6561 6d20 6973 2060  nput stream is `
+00002250: 6062 2727 6060 2c20 7468 6520 6361 6c6c  `b''``, the call
+00002260: 6261 636b 2066 756e 6374 696f 6e20 7769  back function wi
+00002270: 6c6c 206e 6f74 2062 6520 6361 6c6c 6564  ll not be called
+00002280: 2e0a 2020 2020 3a74 7970 6520 6361 6c6c  ..    :type call
+00002290: 6261 636b 3a20 6361 6c6c 6162 6c65 0a20  back: callable. 
+000022a0: 2020 203a 7265 7475 726e 3a20 4120 322d     :return: A 2-
+000022b0: 6974 656d 2074 7570 6c65 2c20 6060 2874  item tuple, ``(t
+000022c0: 6f74 616c 5f69 6e70 7574 2c20 746f 7461  otal_input, tota
+000022d0: 6c5f 6f75 7470 7574 2960 602c 2074 6865  l_output)``, the
+000022e0: 2069 7465 6d73 2061 7265 2060 6069 6e74   items are ``int
+000022f0: 6060 206f 626a 6563 7473 2e0a 0a20 2020  `` objects...   
+00002300: 202e 2e20 736f 7572 6365 636f 6465 3a3a   .. sourcecode::
+00002310: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+00002320: 2023 2063 6f6d 7072 6573 7320 616e 2069   # compress an i
+00002330: 6e70 7574 2066 696c 652c 2061 6e64 2077  nput file, and w
+00002340: 7269 7465 2074 6f20 616e 206f 7574 7075  rite to an outpu
+00002350: 7420 6669 6c65 2e0a 2020 2020 2020 2020  t file..        
+00002360: 7769 7468 2069 6f2e 6f70 656e 2869 6e70  with io.open(inp
+00002370: 7574 5f66 696c 655f 7061 7468 2c20 2772  ut_file_path, 'r
+00002380: 6227 2920 6173 2069 6668 3a0a 2020 2020  b') as ifh:.    
+00002390: 2020 2020 2020 2020 7769 7468 2069 6f2e          with io.
+000023a0: 6f70 656e 286f 7574 7075 745f 6669 6c65  open(output_file
+000023b0: 5f70 6174 682c 2027 7762 2729 2061 7320  _path, 'wb') as 
+000023c0: 6f66 683a 0a20 2020 2020 2020 2020 2020  ofh:.           
+000023d0: 2020 2020 2063 6f6d 7072 6573 735f 7374       compress_st
+000023e0: 7265 616d 2869 6668 2c20 6f66 682c 206c  ream(ifh, ofh, l
+000023f0: 6576 656c 5f6f 725f 6f70 7469 6f6e 3d35  evel_or_option=5
+00002400: 290a 0a20 2020 2020 2020 2023 2063 6f6d  )..        # com
+00002410: 7072 6573 7320 6120 6279 7465 7320 6f62  press a bytes ob
+00002420: 6a65 6374 2c20 616e 6420 7772 6974 6520  ject, and write 
+00002430: 746f 2061 2066 696c 652e 0a20 2020 2020  to a file..     
+00002440: 2020 2077 6974 6820 696f 2e42 7974 6573     with io.Bytes
+00002450: 494f 2872 6177 5f64 6174 2920 6173 2062  IO(raw_dat) as b
+00002460: 693a 0a20 2020 2020 2020 2020 2020 2077  i:.            w
+00002470: 6974 6820 696f 2e6f 7065 6e28 6f75 7470  ith io.open(outp
+00002480: 7574 5f66 696c 655f 7061 7468 2c20 2777  ut_file_path, 'w
+00002490: 6227 2920 6173 206f 6668 3a0a 2020 2020  b') as ofh:.    
+000024a0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+000024b0: 7265 7373 5f73 7472 6561 6d28 6269 2c20  ress_stream(bi, 
+000024c0: 6f66 682c 2070 6c65 6467 6564 5f69 6e70  ofh, pledged_inp
+000024d0: 7574 5f73 697a 653d 6c65 6e28 7261 775f  ut_size=len(raw_
+000024e0: 6461 7429 290a 0a20 2020 2020 2020 2023  dat))..        #
+000024f0: 2043 6f6d 7072 6573 7320 616e 2069 6e70   Compress an inp
+00002500: 7574 2066 696c 652c 206f 6274 6169 6e20  ut file, obtain 
+00002510: 6120 6279 7465 7320 6f62 6a65 6374 2e0a  a bytes object..
+00002520: 2020 2020 2020 2020 2320 4974 2773 2066          # It's f
+00002530: 6173 7465 7220 7468 616e 2072 6561 6469  aster than readi
+00002540: 6e67 2061 2066 696c 6520 616e 6420 636f  ng a file and co
+00002550: 6d70 7265 7373 696e 6720 6974 2069 6e0a  mpressing it in.
+00002560: 2020 2020 2020 2020 2320 6d65 6d6f 7279          # memory
+00002570: 2c20 7465 7374 6564 206f 6e20 5562 756e  , tested on Ubun
+00002580: 7475 2850 7974 686f 6e33 2e38 292f 5769  tu(Python3.8)/Wi
+00002590: 6e64 6f77 7328 5079 7468 6f6e 332e 3929  ndows(Python3.9)
+000025a0: 2e0a 2020 2020 2020 2020 2320 4d61 7962  ..        # Mayb
+000025b0: 6520 7468 6520 4f53 2068 6173 2070 7265  e the OS has pre
+000025c0: 6665 7463 6869 6e67 2c20 6974 2063 616e  fetching, it can
+000025d0: 2072 6561 6420 616e 6420 636f 6d70 7265   read and compre
+000025e0: 7373 0a20 2020 2020 2020 2023 2064 6174  ss.        # dat
+000025f0: 6120 696e 2070 6172 616c 6c65 6c20 746f  a in parallel to
+00002600: 2073 6f6d 6520 6465 6772 6565 2c20 7265   some degree, re
+00002610: 6164 696e 6720 6669 6c65 2066 726f 6d20  ading file from 
+00002620: 4844 440a 2020 2020 2020 2020 2320 6973  HDD.        # is
+00002630: 2074 6865 2062 6f74 746c 656e 6563 6b20   the bottleneck 
+00002640: 696e 2074 6869 7320 6361 7365 2e0a 2020  in this case..  
+00002650: 2020 2020 2020 7769 7468 2069 6f2e 6f70        with io.op
+00002660: 656e 2869 6e70 7574 5f66 696c 655f 7061  en(input_file_pa
+00002670: 7468 2c20 2772 6227 2920 6173 2069 6668  th, 'rb') as ifh
+00002680: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00002690: 7468 2069 6f2e 4279 7465 7349 4f28 2920  th io.BytesIO() 
+000026a0: 6173 2062 6f3a 0a20 2020 2020 2020 2020  as bo:.         
+000026b0: 2020 2020 2020 2063 6f6d 7072 6573 735f         compress_
+000026c0: 7374 7265 616d 2869 6668 2c20 626f 290a  stream(ifh, bo).
+000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026e0: 636f 6d70 7265 7373 6564 5f64 6174 203d  compressed_dat =
+000026f0: 2062 6f2e 6765 7476 616c 7565 2829 0a0a   bo.getvalue()..
+00002700: 2020 2020 2020 2020 2320 5072 696e 7420          # Print 
+00002710: 7072 6f67 7265 7373 2075 7369 6e67 2063  progress using c
+00002720: 616c 6c62 6163 6b20 6675 6e63 7469 6f6e  allback function
+00002730: 0a20 2020 2020 2020 2064 6566 2063 6f6d  .        def com
+00002740: 7072 6573 735f 7072 696e 745f 7072 6f67  press_print_prog
+00002750: 7265 7373 2869 6e70 7574 5f66 696c 655f  ress(input_file_
+00002760: 7061 7468 2c20 6f75 7470 7574 5f66 696c  path, output_fil
+00002770: 655f 7061 7468 293a 0a20 2020 2020 2020  e_path):.       
+00002780: 2020 2020 2069 6e70 7574 5f66 696c 655f       input_file_
+00002790: 7369 7a65 203d 206f 732e 7061 7468 2e67  size = os.path.g
+000027a0: 6574 7369 7a65 2869 6e70 7574 5f66 696c  etsize(input_fil
+000027b0: 655f 7061 7468 290a 0a20 2020 2020 2020  e_path)..       
+000027c0: 2020 2020 2064 6566 2066 756e 6328 746f       def func(to
+000027d0: 7461 6c5f 696e 7075 742c 2074 6f74 616c  tal_input, total
+000027e0: 5f6f 7574 7075 742c 2072 6561 645f 6461  _output, read_da
+000027f0: 7461 2c20 7772 6974 655f 6461 7461 293a  ta, write_data):
+00002800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002810: 2023 2049 6620 696e 7075 7420 7374 7265   # If input stre
+00002820: 616d 2069 7320 656d 7074 792c 2074 6865  am is empty, the
+00002830: 2063 616c 6c62 6163 6b20 6675 6e63 7469   callback functi
+00002840: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00002850: 2020 2023 2077 696c 6c20 6e6f 7420 6265     # will not be
+00002860: 2063 616c 6c65 642e 2053 6f20 6e6f 205a   called. So no Z
+00002870: 6572 6f44 6976 6973 696f 6e45 7272 6f72  eroDivisionError
+00002880: 2068 6572 652e 0a20 2020 2020 2020 2020   here..         
+00002890: 2020 2020 2020 2070 6572 6365 6e74 203d         percent =
+000028a0: 2031 3030 202a 2074 6f74 616c 5f69 6e70   100 * total_inp
+000028b0: 7574 202f 2069 6e70 7574 5f66 696c 655f  ut / input_file_
+000028c0: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
+000028d0: 2020 2020 2070 7269 6e74 2866 2750 726f       print(f'Pro
+000028e0: 6772 6573 733a 207b 7065 7263 656e 743a  gress: {percent:
+000028f0: 2e31 667d 2527 2c20 656e 643d 275c 7227  .1f}%', end='\r'
+00002900: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
+00002910: 6974 6820 696f 2e6f 7065 6e28 696e 7075  ith io.open(inpu
+00002920: 745f 6669 6c65 5f70 6174 682c 2027 7262  t_file_path, 'rb
+00002930: 2729 2061 7320 6966 683a 0a20 2020 2020  ') as ifh:.     
+00002940: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00002950: 696f 2e6f 7065 6e28 6f75 7470 7574 5f66  io.open(output_f
+00002960: 696c 655f 7061 7468 2c20 2777 6227 2920  ile_path, 'wb') 
+00002970: 6173 206f 6668 3a0a 2020 2020 2020 2020  as ofh:.        
+00002980: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00002990: 7265 7373 5f73 7472 6561 6d28 6966 682c  ress_stream(ifh,
+000029a0: 206f 6668 2c20 6361 6c6c 6261 636b 3d66   ofh, callback=f
+000029b0: 756e 6329 0a0a 0a2e 2e20 7079 3a63 6c61  unc)..... py:cla
+000029c0: 7373 3a3a 205a 7374 6443 6f6d 7072 6573  ss:: ZstdCompres
+000029d0: 736f 720a 0a20 2020 2041 2073 7472 6561  sor..    A strea
+000029e0: 6d69 6e67 2063 6f6d 7072 6573 736f 722e  ming compressor.
+000029f0: 2049 7427 7320 7468 7265 6164 2d73 6166   It's thread-saf
+00002a00: 6520 6174 206d 6574 686f 6420 6c65 7665  e at method leve
+00002a10: 6c2e 0a0a 2020 2020 2e2e 2070 793a 6d65  l...    .. py:me
+00002a20: 7468 6f64 3a3a 205f 5f69 6e69 745f 5f28  thod:: __init__(
+00002a30: 7365 6c66 2c20 6c65 7665 6c5f 6f72 5f6f  self, level_or_o
+00002a40: 7074 696f 6e3d 4e6f 6e65 2c20 7a73 7464  ption=None, zstd
+00002a50: 5f64 6963 743d 4e6f 6e65 290a 0a20 2020  _dict=None)..   
+00002a60: 2020 2020 2049 6e69 7469 616c 697a 6520       Initialize 
+00002a70: 6120 5a73 7464 436f 6d70 7265 7373 6f72  a ZstdCompressor
+00002a80: 206f 626a 6563 742e 0a0a 2020 2020 2020   object...      
+00002a90: 2020 3a70 6172 616d 206c 6576 656c 5f6f    :param level_o
+00002aa0: 725f 6f70 7469 6f6e 3a20 5768 656e 2069  r_option: When i
+00002ab0: 7427 7320 616e 2060 6069 6e74 6060 206f  t's an ``int`` o
+00002ac0: 626a 6563 742c 2069 7420 7265 7072 6573  bject, it repres
+00002ad0: 656e 7473 2074 6865 203a 7265 663a 6063  ents the :ref:`c
+00002ae0: 6f6d 7072 6573 7369 6f6e 206c 6576 656c  ompression level
+00002af0: 3c63 6f6d 7072 6573 7369 6f6e 5f6c 6576  <compression_lev
+00002b00: 656c 3e60 2e20 5768 656e 2069 7427 7320  el>`. When it's 
+00002b10: 6120 6060 6469 6374 6060 206f 626a 6563  a ``dict`` objec
+00002b20: 742c 2069 7420 636f 6e74 6169 6e73 203a  t, it contains :
+00002b30: 7265 663a 6061 6476 616e 6365 6420 636f  ref:`advanced co
+00002b40: 6d70 7265 7373 696f 6e20 7061 7261 6d65  mpression parame
+00002b50: 7465 7273 3c43 5061 7261 6d65 7465 723e  ters<CParameter>
+00002b60: 602e 2054 6865 2064 6566 6175 6c74 2076  `. The default v
+00002b70: 616c 7565 2060 604e 6f6e 6560 6020 6d65  alue ``None`` me
+00002b80: 616e 7320 746f 2075 7365 207a 7374 6427  ans to use zstd'
+00002b90: 7320 6465 6661 756c 7420 636f 6d70 7265  s default compre
+00002ba0: 7373 696f 6e20 6c65 7665 6c2f 7061 7261  ssion level/para
+00002bb0: 6d65 7465 7273 2e0a 2020 2020 2020 2020  meters..        
+00002bc0: 3a74 7970 6520 6c65 7665 6c5f 6f72 5f6f  :type level_or_o
+00002bd0: 7074 696f 6e3a 2069 6e74 206f 7220 6469  ption: int or di
+00002be0: 6374 0a20 2020 2020 2020 203a 7061 7261  ct.        :para
+00002bf0: 6d20 7a73 7464 5f64 6963 743a 2050 7265  m zstd_dict: Pre
+00002c00: 2d74 7261 696e 6564 2064 6963 7469 6f6e  -trained diction
+00002c10: 6172 7920 666f 7220 636f 6d70 7265 7373  ary for compress
+00002c20: 696f 6e2e 0a20 2020 2020 2020 203a 7479  ion..        :ty
+00002c30: 7065 207a 7374 645f 6469 6374 3a20 5a73  pe zstd_dict: Zs
+00002c40: 7464 4469 6374 0a0a 2020 2020 2e2e 2070  tdDict..    .. p
+00002c50: 793a 6d65 7468 6f64 3a3a 2063 6f6d 7072  y:method:: compr
+00002c60: 6573 7328 7365 6c66 2c20 6461 7461 2c20  ess(self, data, 
+00002c70: 6d6f 6465 3d5a 7374 6443 6f6d 7072 6573  mode=ZstdCompres
+00002c80: 736f 722e 434f 4e54 494e 5545 290a 0a20  sor.CONTINUE).. 
+00002c90: 2020 2020 2020 2050 726f 7669 6465 2064         Provide d
+00002ca0: 6174 6120 746f 2074 6865 2063 6f6d 7072  ata to the compr
+00002cb0: 6573 736f 7220 6f62 6a65 6374 2e0a 0a20  essor object... 
+00002cc0: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
+00002cd0: 7461 3a20 4461 7461 2074 6f20 6265 2063  ta: Data to be c
+00002ce0: 6f6d 7072 6573 7365 642e 0a20 2020 2020  ompressed..     
+00002cf0: 2020 203a 7479 7065 2064 6174 613a 2062     :type data: b
+00002d00: 7974 6573 2d6c 696b 6520 6f62 6a65 6374  ytes-like object
+00002d10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00002d20: 6d6f 6465 3a20 4361 6e20 6265 2074 6865  mode: Can be the
+00002d30: 7365 2033 2076 616c 7565 733a 203a 7079  se 3 values: :py
+00002d40: 3a61 7474 723a 605a 7374 6443 6f6d 7072  :attr:`ZstdCompr
+00002d50: 6573 736f 722e 434f 4e54 494e 5545 602c  essor.CONTINUE`,
+00002d60: 203a 7079 3a61 7474 723a 605a 7374 6443   :py:attr:`ZstdC
+00002d70: 6f6d 7072 6573 736f 722e 464c 5553 485f  ompressor.FLUSH_
+00002d80: 424c 4f43 4b60 2c20 3a70 793a 6174 7472  BLOCK`, :py:attr
+00002d90: 3a60 5a73 7464 436f 6d70 7265 7373 6f72  :`ZstdCompressor
+00002da0: 2e46 4c55 5348 5f46 5241 4d45 602e 0a20  .FLUSH_FRAME`.. 
+00002db0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00002dc0: 4120 6368 756e 6b20 6f66 2063 6f6d 7072  A chunk of compr
+00002dd0: 6573 7365 6420 6461 7461 2069 6620 706f  essed data if po
+00002de0: 7373 6962 6c65 2c20 6f72 2060 6062 2727  ssible, or ``b''
+00002df0: 6060 206f 7468 6572 7769 7365 2e0a 2020  `` otherwise..  
+00002e00: 2020 2020 2020 3a72 7479 7065 3a20 6279        :rtype: by
+00002e10: 7465 730a 0a20 2020 202e 2e20 7079 3a6d  tes..    .. py:m
+00002e20: 6574 686f 643a 3a20 666c 7573 6828 7365  ethod:: flush(se
+00002e30: 6c66 2c20 6d6f 6465 3d5a 7374 6443 6f6d  lf, mode=ZstdCom
+00002e40: 7072 6573 736f 722e 464c 5553 485f 4652  pressor.FLUSH_FR
+00002e50: 414d 4529 0a0a 2020 2020 2020 2020 466c  AME)..        Fl
+00002e60: 7573 6820 616e 7920 7265 6d61 696e 696e  ush any remainin
+00002e70: 6720 6461 7461 2069 6e20 696e 7465 726e  g data in intern
+00002e80: 616c 2062 7566 6665 722e 0a0a 2020 2020  al buffer...    
+00002e90: 2020 2020 5369 6e63 6520 7a73 7464 2064      Since zstd d
+00002ea0: 6174 6120 636f 6e73 6973 7473 206f 6620  ata consists of 
+00002eb0: 6f6e 6520 6f72 206d 6f72 6520 696e 6465  one or more inde
+00002ec0: 7065 6e64 656e 7420 6672 616d 6573 2c20  pendent frames, 
+00002ed0: 7468 6520 636f 6d70 7265 7373 6f72 206f  the compressor o
+00002ee0: 626a 6563 7420 6361 6e20 7374 696c 6c20  bject can still 
+00002ef0: 6265 2075 7365 6420 6166 7465 7220 7468  be used after th
+00002f00: 6973 206d 6574 686f 6420 6973 2063 616c  is method is cal
+00002f10: 6c65 642e 0a0a 2020 2020 2020 2020 2a2a  led...        **
+00002f20: 4e6f 7465 2a2a 3a20 4162 7573 6520 6f66  Note**: Abuse of
+00002f30: 2074 6869 7320 6d65 7468 6f64 2077 696c   this method wil
+00002f40: 6c20 7265 6475 6365 2063 6f6d 7072 6573  l reduce compres
+00002f50: 7369 6f6e 2072 6174 696f 2c20 616e 6420  sion ratio, and 
+00002f60: 736f 6d65 2070 726f 6772 616d 7320 6361  some programs ca
+00002f70: 6e20 6f6e 6c79 2064 6563 6f6d 7072 6573  n only decompres
+00002f80: 7320 7369 6e67 6c65 2066 7261 6d65 2064  s single frame d
+00002f90: 6174 612e 2055 7365 2069 7420 6f6e 6c79  ata. Use it only
+00002fa0: 2077 6865 6e20 6e65 6365 7373 6172 792e   when necessary.
+00002fb0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00002fc0: 206d 6f64 653a 2043 616e 2062 6520 7468   mode: Can be th
+00002fd0: 6573 6520 3220 7661 6c75 6573 3a20 3a70  ese 2 values: :p
+00002fe0: 793a 6174 7472 3a60 5a73 7464 436f 6d70  y:attr:`ZstdComp
+00002ff0: 7265 7373 6f72 2e46 4c55 5348 5f46 5241  ressor.FLUSH_FRA
+00003000: 4d45 602c 203a 7079 3a61 7474 723a 605a  ME`, :py:attr:`Z
+00003010: 7374 6443 6f6d 7072 6573 736f 722e 464c  stdCompressor.FL
+00003020: 5553 485f 424c 4f43 4b60 2e0a 2020 2020  USH_BLOCK`..    
+00003030: 2020 2020 3a72 6574 7572 6e3a 2046 6c75      :return: Flu
+00003040: 7368 6564 2064 6174 612e 0a20 2020 2020  shed data..     
+00003050: 2020 203a 7274 7970 653a 2062 7974 6573     :rtype: bytes
+00003060: 0a0a 2020 2020 2e2e 2070 793a 6174 7472  ..    .. py:attr
+00003070: 6962 7574 653a 3a20 6c61 7374 5f6d 6f64  ibute:: last_mod
+00003080: 650a 0a20 2020 2020 2020 2054 6865 206c  e..        The l
+00003090: 6173 7420 6d6f 6465 2075 7365 6420 746f  ast mode used to
+000030a0: 2074 6869 7320 636f 6d70 7265 7373 6f72   this compressor
+000030b0: 2c20 6974 7320 7661 6c75 6520 6361 6e20  , its value can 
+000030c0: 6265 203a 7079 3a61 7474 723a 607e 5a73  be :py:attr:`~Zs
+000030d0: 7464 436f 6d70 7265 7373 6f72 2e43 4f4e  tdCompressor.CON
+000030e0: 5449 4e55 4560 2c20 3a70 793a 6174 7472  TINUE`, :py:attr
+000030f0: 3a60 7e5a 7374 6443 6f6d 7072 6573 736f  :`~ZstdCompresso
+00003100: 722e 464c 5553 485f 424c 4f43 4b60 2c20  r.FLUSH_BLOCK`, 
+00003110: 3a70 793a 6174 7472 3a60 7e5a 7374 6443  :py:attr:`~ZstdC
+00003120: 6f6d 7072 6573 736f 722e 464c 5553 485f  ompressor.FLUSH_
+00003130: 4652 414d 4560 2e20 496e 6974 6961 6c69  FRAME`. Initiali
+00003140: 7a65 6420 746f 203a 7079 3a61 7474 723a  zed to :py:attr:
+00003150: 607e 5a73 7464 436f 6d70 7265 7373 6f72  `~ZstdCompressor
+00003160: 2e46 4c55 5348 5f46 5241 4d45 602e 0a0a  .FLUSH_FRAME`...
+00003170: 2020 2020 2020 2020 4974 2063 616e 2062          It can b
+00003180: 6520 7573 6564 2074 6f20 6765 7420 7468  e used to get th
+00003190: 6520 6375 7272 656e 7420 7374 6174 6520  e current state 
+000031a0: 6f66 2061 2063 6f6d 7072 6573 736f 722c  of a compressor,
+000031b0: 2073 7563 6820 6173 2c20 6461 7461 2066   such as, data f
+000031c0: 6c75 7368 6564 2c20 6120 6672 616d 6520  lushed, a frame 
+000031d0: 656e 6465 642e 0a0a 2020 2020 2e2e 2070  ended...    .. p
+000031e0: 793a 6174 7472 6962 7574 653a 3a20 434f  y:attribute:: CO
+000031f0: 4e54 494e 5545 0a0a 2020 2020 2020 2020  NTINUE..        
+00003200: 5573 6564 2066 6f72 202a 6d6f 6465 2a20  Used for *mode* 
+00003210: 7061 7261 6d65 7465 7220 696e 203a 7079  parameter in :py
+00003220: 3a6d 6574 683a 607e 5a73 7464 436f 6d70  :meth:`~ZstdComp
+00003230: 7265 7373 6f72 2e63 6f6d 7072 6573 7360  ressor.compress`
+00003240: 206d 6574 686f 642e 0a0a 2020 2020 2020   method...      
+00003250: 2020 436f 6c6c 6563 7420 6d6f 7265 2064    Collect more d
+00003260: 6174 612c 2065 6e63 6f64 6572 2064 6563  ata, encoder dec
+00003270: 6964 6573 2077 6865 6e20 746f 206f 7574  ides when to out
+00003280: 7075 7420 636f 6d70 7265 7373 6564 2072  put compressed r
+00003290: 6573 756c 742c 2066 6f72 206f 7074 696d  esult, for optim
+000032a0: 616c 2063 6f6d 7072 6573 7369 6f6e 2072  al compression r
+000032b0: 6174 696f 2e20 5573 7561 6c6c 7920 7573  atio. Usually us
+000032c0: 6564 2066 6f72 2074 7261 6469 7469 6f6e  ed for tradition
+000032d0: 616c 2073 7472 6561 6d69 6e67 2063 6f6d  al streaming com
+000032e0: 7072 6573 7369 6f6e 2e0a 0a20 2020 202e  pression...    .
+000032f0: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
+00003300: 2046 4c55 5348 5f42 4c4f 434b 0a0a 2020   FLUSH_BLOCK..  
+00003310: 2020 2020 2020 5573 6564 2066 6f72 202a        Used for *
+00003320: 6d6f 6465 2a20 7061 7261 6d65 7465 7220  mode* parameter 
+00003330: 696e 203a 7079 3a6d 6574 683a 607e 5a73  in :py:meth:`~Zs
+00003340: 7464 436f 6d70 7265 7373 6f72 2e63 6f6d  tdCompressor.com
+00003350: 7072 6573 7360 2c20 3a70 793a 6d65 7468  press`, :py:meth
+00003360: 3a60 7e5a 7374 6443 6f6d 7072 6573 736f  :`~ZstdCompresso
+00003370: 722e 666c 7573 6860 206d 6574 686f 6473  r.flush` methods
+00003380: 2e0a 0a20 2020 2020 2020 2046 6c75 7368  ...        Flush
+00003390: 2061 6e79 2072 656d 6169 6e69 6e67 2064   any remaining d
+000033a0: 6174 612c 2062 7574 2064 6f6e 2774 2063  ata, but don't c
+000033b0: 6c6f 7365 2074 6865 2063 7572 7265 6e74  lose the current
+000033c0: 203a 7265 663a 6066 7261 6d65 3c66 7261   :ref:`frame<fra
+000033d0: 6d65 5f62 6c6f 636b 3e60 2e20 5573 7561  me_block>`. Usua
+000033e0: 6c6c 7920 7573 6564 2066 6f72 2063 6f6d  lly used for com
+000033f0: 6d75 6e69 6361 7469 6f6e 2073 6365 6e61  munication scena
+00003400: 7269 6f73 2e0a 0a20 2020 2020 2020 2049  rios...        I
+00003410: 6620 7468 6572 6520 6973 2064 6174 612c  f there is data,
+00003420: 2069 7420 6372 6561 7465 7320 6174 206c   it creates at l
+00003430: 6561 7374 206f 6e65 206e 6577 203a 7265  east one new :re
+00003440: 663a 6062 6c6f 636b 3c66 7261 6d65 5f62  f:`block<frame_b
+00003450: 6c6f 636b 3e60 2c20 7468 6174 2063 616e  lock>`, that can
+00003460: 2062 6520 6465 636f 6465 6420 696d 6d65   be decoded imme
+00003470: 6469 6174 656c 7920 6f6e 2072 6563 6570  diately on recep
+00003480: 7469 6f6e 2e20 4966 206e 6f20 7265 6d61  tion. If no rema
+00003490: 696e 696e 6720 6461 7461 2c20 6e6f 2062  ining data, no b
+000034a0: 6c6f 636b 2069 7320 6372 6561 7465 642c  lock is created,
+000034b0: 2072 6574 7572 6e20 6060 6227 2760 602e   return ``b''``.
+000034c0: 0a0a 2020 2020 2020 2020 2a2a 4e6f 7465  ..        **Note
+000034d0: 2a2a 3a20 4162 7573 6520 6f66 2074 6869  **: Abuse of thi
+000034e0: 7320 6d6f 6465 2077 696c 6c20 7265 6475  s mode will redu
+000034f0: 6365 2063 6f6d 7072 6573 7369 6f6e 2072  ce compression r
+00003500: 6174 696f 2e20 5573 6520 6974 206f 6e6c  atio. Use it onl
+00003510: 7920 7768 656e 206e 6563 6573 7361 7279  y when necessary
+00003520: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
+00003530: 7269 6275 7465 3a3a 2046 4c55 5348 5f46  ribute:: FLUSH_F
+00003540: 5241 4d45 0a0a 2020 2020 2020 2020 5573  RAME..        Us
+00003550: 6564 2066 6f72 202a 6d6f 6465 2a20 7061  ed for *mode* pa
+00003560: 7261 6d65 7465 7220 696e 203a 7079 3a6d  rameter in :py:m
+00003570: 6574 683a 607e 5a73 7464 436f 6d70 7265  eth:`~ZstdCompre
+00003580: 7373 6f72 2e63 6f6d 7072 6573 7360 2c20  ssor.compress`, 
+00003590: 3a70 793a 6d65 7468 3a60 7e5a 7374 6443  :py:meth:`~ZstdC
+000035a0: 6f6d 7072 6573 736f 722e 666c 7573 6860  ompressor.flush`
+000035b0: 206d 6574 686f 6473 2e0a 0a20 2020 2020   methods...     
+000035c0: 2020 2046 6c75 7368 2061 6e79 2072 656d     Flush any rem
+000035d0: 6169 6e69 6e67 2064 6174 612c 2061 6e64  aining data, and
+000035e0: 2063 6c6f 7365 2074 6865 2063 7572 7265   close the curre
+000035f0: 6e74 203a 7265 663a 6066 7261 6d65 3c66  nt :ref:`frame<f
+00003600: 7261 6d65 5f62 6c6f 636b 3e60 2e20 5573  rame_block>`. Us
+00003610: 7561 6c6c 7920 7573 6564 2066 6f72 2074  ually used for t
+00003620: 7261 6469 7469 6f6e 616c 2066 6c75 7368  raditional flush
+00003630: 2e0a 0a20 2020 2020 2020 2053 696e 6365  ...        Since
+00003640: 207a 7374 6420 6461 7461 2063 6f6e 7369   zstd data consi
+00003650: 7374 7320 6f66 206f 6e65 206f 7220 6d6f  sts of one or mo
+00003660: 7265 2069 6e64 6570 656e 6465 6e74 2066  re independent f
+00003670: 7261 6d65 732c 2064 6174 6120 6361 6e20  rames, data can 
+00003680: 7374 696c 6c20 6265 2070 726f 7669 6465  still be provide
+00003690: 6420 6166 7465 7220 6120 6672 616d 6520  d after a frame 
+000036a0: 6973 2063 6c6f 7365 642e 0a0a 2020 2020  is closed...    
+000036b0: 2020 2020 2a2a 4e6f 7465 2a2a 3a20 4162      **Note**: Ab
+000036c0: 7573 6520 6f66 2074 6869 7320 6d6f 6465  use of this mode
+000036d0: 2077 696c 6c20 7265 6475 6365 2063 6f6d   will reduce com
+000036e0: 7072 6573 7369 6f6e 2072 6174 696f 2c20  pression ratio, 
+000036f0: 616e 6420 736f 6d65 2070 726f 6772 616d  and some program
+00003700: 7320 6361 6e20 6f6e 6c79 2064 6563 6f6d  s can only decom
+00003710: 7072 6573 7320 7369 6e67 6c65 2066 7261  press single fra
+00003720: 6d65 2064 6174 612e 2055 7365 2069 7420  me data. Use it 
+00003730: 6f6e 6c79 2077 6865 6e20 6e65 6365 7373  only when necess
+00003740: 6172 792e 0a0a 2020 2020 2e2e 2073 6f75  ary...    .. sou
+00003750: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
+00003760: 0a0a 2020 2020 2020 2020 6320 3d20 5a73  ..        c = Zs
+00003770: 7464 436f 6d70 7265 7373 6f72 2829 0a0a  tdCompressor()..
+00003780: 2020 2020 2020 2020 2320 7472 6164 6974          # tradit
+00003790: 696f 6e61 6c20 7374 7265 616d 696e 6720  ional streaming 
+000037a0: 636f 6d70 7265 7373 696f 6e0a 2020 2020  compression.    
+000037b0: 2020 2020 6461 7431 203d 2063 2e63 6f6d      dat1 = c.com
+000037c0: 7072 6573 7328 6227 3132 3334 3536 2729  press(b'123456')
+000037d0: 0a20 2020 2020 2020 2064 6174 3220 3d20  .        dat2 = 
+000037e0: 632e 636f 6d70 7265 7373 2862 2761 6263  c.compress(b'abc
+000037f0: 6465 6627 290a 2020 2020 2020 2020 6461  def').        da
+00003800: 7433 203d 2063 2e66 6c75 7368 2829 0a0a  t3 = c.flush()..
+00003810: 2020 2020 2020 2020 2320 7573 6520 2e63          # use .c
+00003820: 6f6d 7072 6573 7328 2920 6d65 7468 6f64  ompress() method
+00003830: 2077 6974 6820 6d6f 6465 2061 7267 756d   with mode argum
+00003840: 656e 740a 2020 2020 2020 2020 636f 6d70  ent.        comp
+00003850: 7265 7373 6564 5f64 6174 3120 3d20 632e  ressed_dat1 = c.
+00003860: 636f 6d70 7265 7373 2872 6177 5f64 6174  compress(raw_dat
+00003870: 312c 2063 2e46 4c55 5348 5f42 4c4f 434b  1, c.FLUSH_BLOCK
+00003880: 290a 2020 2020 2020 2020 636f 6d70 7265  ).        compre
+00003890: 7373 6564 5f64 6174 3220 3d20 632e 636f  ssed_dat2 = c.co
+000038a0: 6d70 7265 7373 2872 6177 5f64 6174 322c  mpress(raw_dat2,
+000038b0: 2063 2e46 4c55 5348 5f46 5241 4d45 290a   c.FLUSH_FRAME).
+000038c0: 0a20 2020 202e 2e20 6869 6e74 3a3a 2057  .    .. hint:: W
+000038d0: 6879 203a 7079 3a6d 6574 683a 605a 7374  hy :py:meth:`Zst
+000038e0: 6443 6f6d 7072 6573 736f 722e 636f 6d70  dCompressor.comp
+000038f0: 7265 7373 6020 6d65 7468 6f64 2068 6173  ress` method has
+00003900: 2061 202a 6d6f 6465 2a20 7061 7261 6d65   a *mode* parame
+00003910: 7465 723f 0a0a 2020 2020 2020 2020 232e  ter?..        #.
+00003920: 2057 6865 6e20 7265 7573 6520 3a70 793a   When reuse :py:
+00003930: 636c 6173 733a 605a 7374 6443 6f6d 7072  class:`ZstdCompr
+00003940: 6573 736f 7260 206f 626a 6563 7420 666f  essor` object fo
+00003950: 7220 6269 6720 6e75 6d62 6572 206f 6620  r big number of 
+00003960: 7361 6d65 2074 7970 6520 696e 6469 7669  same type indivi
+00003970: 6475 616c 2064 6174 612c 206d 616b 6520  dual data, make 
+00003980: 6f70 6572 6174 696f 6e20 6d6f 7265 2063  operation more c
+00003990: 6f6e 7665 6e69 656e 742e 2054 6865 206f  onvenient. The o
+000039a0: 626a 6563 7420 6973 2074 6872 6561 642d  bject is thread-
+000039b0: 7361 6665 2061 7420 6d65 7468 6f64 206c  safe at method l
+000039c0: 6576 656c 2e0a 2020 2020 2020 2020 232e  evel..        #.
+000039d0: 2049 6620 6461 7461 2069 7320 6765 6e65   If data is gene
+000039e0: 7261 7465 6420 6279 2061 2073 696e 676c  rated by a singl
+000039f0: 6520 3a70 793a 6174 7472 3a60 7e5a 7374  e :py:attr:`~Zst
+00003a00: 6443 6f6d 7072 6573 736f 722e 464c 5553  dCompressor.FLUS
+00003a10: 485f 4652 414d 4560 206d 6f64 652c 2074  H_FRAME` mode, t
+00003a20: 6865 2073 697a 6520 6f66 2075 6e63 6f6d  he size of uncom
+00003a30: 7072 6573 7365 6420 6461 7461 2077 696c  pressed data wil
+00003a40: 6c20 6265 2072 6563 6f72 6465 6420 696e  l be recorded in
+00003a50: 2066 7261 6d65 2068 6561 6465 722e 0a0a   frame header...
+00003a60: 0a53 7472 6561 6d69 6e67 2064 6563 6f6d  .Streaming decom
+00003a70: 7072 6573 7369 6f6e 0a2d 2d2d 2d2d 2d2d  pression.-------
+00003a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003a90: 0a0a 2020 2020 5468 6973 2073 6563 7469  ..    This secti
+00003aa0: 6f6e 2063 6f6e 7461 696e 733a 0a0a 2020  on contains:..  
+00003ab0: 2020 2020 2020 2a20 6675 6e63 7469 6f6e        * function
+00003ac0: 203a 7079 3a66 756e 633a 6064 6563 6f6d   :py:func:`decom
+00003ad0: 7072 6573 735f 7374 7265 616d 602c 2061  press_stream`, a
+00003ae0: 2066 6173 7420 616e 6420 636f 6e76 656e   fast and conven
+00003af0: 6965 6e74 2066 756e 6374 696f 6e2e 0a20  ient function.. 
+00003b00: 2020 2020 2020 202a 2063 6c61 7373 203a         * class :
+00003b10: 7079 3a63 6c61 7373 3a60 5a73 7464 4465  py:class:`ZstdDe
+00003b20: 636f 6d70 7265 7373 6f72 602c 2073 696d  compressor`, sim
+00003b30: 696c 6172 2074 6f20 6465 636f 6d70 7265  ilar to decompre
+00003b40: 7373 6f72 7320 696e 2050 7974 686f 6e20  ssors in Python 
+00003b50: 7374 616e 6461 7264 206c 6962 7261 7279  standard library
+00003b60: 2e0a 2020 2020 2020 2020 2a20 636c 6173  ..        * clas
+00003b70: 7320 3a70 793a 636c 6173 733a 6045 6e64  s :py:class:`End
+00003b80: 6c65 7373 5a73 7464 4465 636f 6d70 7265  lessZstdDecompre
+00003b90: 7373 6f72 602c 2061 2064 6563 6f6d 7072  ssor`, a decompr
+00003ba0: 6573 736f 7220 6163 6365 7074 7320 6d75  essor accepts mu
+00003bb0: 6c74 6970 6c65 2063 6f6e 6361 7465 6e61  ltiple concatena
+00003bc0: 7465 6420 3a72 6566 3a60 6672 616d 6573  ted :ref:`frames
+00003bd0: 3c66 7261 6d65 5f62 6c6f 636b 3e60 2e0a  <frame_block>`..
+00003be0: 0a2e 2e20 7079 3a66 756e 6374 696f 6e3a  ... py:function:
+00003bf0: 3a20 6465 636f 6d70 7265 7373 5f73 7472  : decompress_str
+00003c00: 6561 6d28 696e 7075 745f 7374 7265 616d  eam(input_stream
+00003c10: 2c20 6f75 7470 7574 5f73 7472 6561 6d2c  , output_stream,
+00003c20: 202a 2c20 7a73 7464 5f64 6963 743d 4e6f   *, zstd_dict=No
+00003c30: 6e65 2c20 6f70 7469 6f6e 3d4e 6f6e 652c  ne, option=None,
+00003c40: 2072 6561 645f 7369 7a65 3d31 3331 5f30   read_size=131_0
+00003c50: 3735 2c20 7772 6974 655f 7369 7a65 3d31  75, write_size=1
+00003c60: 3331 5f30 3732 2c20 6361 6c6c 6261 636b  31_072, callback
+00003c70: 3d4e 6f6e 6529 0a0a 2020 2020 4120 6661  =None)..    A fa
+00003c80: 7374 2061 6e64 2063 6f6e 7665 6e69 656e  st and convenien
+00003c90: 7420 6675 6e63 7469 6f6e 2c20 6465 636f  t function, deco
+00003ca0: 6d70 7265 7373 6573 202a 696e 7075 745f  mpresses *input_
+00003cb0: 7374 7265 616d 2a20 616e 6420 7772 6974  stream* and writ
+00003cc0: 6573 2074 6865 2064 6563 6f6d 7072 6573  es the decompres
+00003cd0: 7365 6420 6461 7461 2074 6f20 2a6f 7574  sed data to *out
+00003ce0: 7075 745f 7374 7265 616d 2a2c 2069 7420  put_stream*, it 
+00003cf0: 646f 6573 6e27 7420 636c 6f73 6520 7468  doesn't close th
+00003d00: 6520 7374 7265 616d 732e 0a0a 2020 2020  e streams...    
+00003d10: 5375 7070 6f72 7473 206d 756c 7469 706c  Supports multipl
+00003d20: 6520 636f 6e63 6174 656e 6174 6564 203a  e concatenated :
+00003d30: 7265 663a 6066 7261 6d65 733c 6672 616d  ref:`frames<fram
+00003d40: 655f 626c 6f63 6b3e 602e 0a0a 2020 2020  e_block>`...    
+00003d50: 5468 6973 2066 756e 6374 696f 6e20 7472  This function tr
+00003d60: 6965 7320 746f 207a 6572 6f2d 636f 7079  ies to zero-copy
+00003d70: 2061 7320 6d75 6368 2061 7320 706f 7373   as much as poss
+00003d80: 6962 6c65 2e20 4966 2074 6865 204f 5320  ible. If the OS 
+00003d90: 6861 7320 7265 6164 2070 7265 6665 7463  has read prefetc
+00003da0: 6869 6e67 2061 6e64 2077 7269 7465 2062  hing and write b
+00003db0: 7566 6665 722c 2069 7420 6d61 7920 7065  uffer, it may pe
+00003dc0: 7266 6f72 6d20 7468 6520 7461 736b 7320  rform the tasks 
+00003dd0: 2872 6561 642f 6465 636f 6d70 7265 7373  (read/decompress
+00003de0: 2f77 7269 7465 2920 696e 2070 6172 616c  /write) in paral
+00003df0: 6c65 6c20 746f 2073 6f6d 6520 6465 6772  lel to some degr
+00003e00: 6565 2e0a 0a20 2020 2054 6865 2064 6566  ee...    The def
+00003e10: 6175 6c74 2076 616c 7565 7320 6f66 202a  ault values of *
+00003e20: 7265 6164 5f73 697a 652a 2061 6e64 202a  read_size* and *
+00003e30: 7772 6974 655f 7369 7a65 2a20 7061 7261  write_size* para
+00003e40: 6d65 7465 7273 2061 7265 2074 6865 2062  meters are the b
+00003e50: 7566 6665 7220 7369 7a65 7320 7265 636f  uffer sizes reco
+00003e60: 6d6d 656e 6465 6420 6279 207a 7374 642c  mmended by zstd,
+00003e70: 2069 6e63 7265 6173 696e 6720 7468 656d   increasing them
+00003e80: 206d 6179 2062 6520 6661 7374 6572 2c20   may be faster, 
+00003e90: 616e 6420 7265 6475 6365 7320 7468 6520  and reduces the 
+00003ea0: 6e75 6d62 6572 206f 6620 6361 6c6c 6261  number of callba
+00003eb0: 636b 2066 756e 6374 696f 6e20 6361 6c6c  ck function call
+00003ec0: 732e 0a0a 2020 2020 2e2e 2076 6572 7369  s...    .. versi
+00003ed0: 6f6e 6164 6465 643a 3a20 302e 3134 2e32  onadded:: 0.14.2
+00003ee0: 0a0a 2020 2020 3a70 6172 616d 2069 6e70  ..    :param inp
+00003ef0: 7574 5f73 7472 6561 6d3a 2049 6e70 7574  ut_stream: Input
+00003f00: 2073 7472 6561 6d20 7468 6174 2068 6173   stream that has
+00003f10: 2061 2060 2e72 6561 6469 6e74 6f28 6229   a `.readinto(b)
+00003f20: 203c 6874 7470 733a 2f2f 646f 6373 2e70   <https://docs.p
+00003f30: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
+00003f40: 6172 792f 696f 2e68 746d 6c23 696f 2e52  ary/io.html#io.R
+00003f50: 6177 494f 4261 7365 2e72 6561 6469 6e74  awIOBase.readint
+00003f60: 6f3e 605f 206d 6574 686f 642e 0a20 2020  o>`_ method..   
+00003f70: 203a 7061 7261 6d20 6f75 7470 7574 5f73   :param output_s
+00003f80: 7472 6561 6d3a 204f 7574 7075 7420 7374  tream: Output st
+00003f90: 7265 616d 2074 6861 7420 6861 7320 6120  ream that has a 
+00003fa0: 602e 7772 6974 6528 6229 203c 6874 7470  `.write(b) <http
+00003fb0: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+00003fc0: 6f72 672f 332f 6c69 6272 6172 792f 696f  org/3/library/io
+00003fd0: 2e68 746d 6c23 696f 2e52 6177 494f 4261  .html#io.RawIOBa
+00003fe0: 7365 2e77 7269 7465 3e60 5f20 6d65 7468  se.write>`_ meth
+00003ff0: 6f64 2e20 4966 2075 7365 202a 6361 6c6c  od. If use *call
+00004000: 6261 636b 2a20 6675 6e63 7469 6f6e 2c20  back* function, 
+00004010: 7468 6973 2070 6172 616d 6574 6572 2063  this parameter c
+00004020: 616e 2062 6520 6060 4e6f 6e65 6060 2e0a  an be ``None``..
+00004030: 2020 2020 3a70 6172 616d 207a 7374 645f      :param zstd_
+00004040: 6469 6374 3a20 5072 652d 7472 6169 6e65  dict: Pre-traine
+00004050: 6420 6469 6374 696f 6e61 7279 2066 6f72  d dictionary for
+00004060: 2064 6563 6f6d 7072 6573 7369 6f6e 2e0a   decompression..
+00004070: 2020 2020 3a74 7970 6520 7a73 7464 5f64      :type zstd_d
+00004080: 6963 743a 205a 7374 6444 6963 740a 2020  ict: ZstdDict.  
+00004090: 2020 3a70 6172 616d 206f 7074 696f 6e3a    :param option:
+000040a0: 2041 2060 6064 6963 7460 6020 6f62 6a65   A ``dict`` obje
+000040b0: 6374 2c20 636f 6e74 6169 6e73 203a 7265  ct, contains :re
+000040c0: 663a 6061 6476 616e 6365 6420 6465 636f  f:`advanced deco
+000040d0: 6d70 7265 7373 696f 6e20 7061 7261 6d65  mpression parame
+000040e0: 7465 7273 3c44 5061 7261 6d65 7465 723e  ters<DParameter>
+000040f0: 602e 0a20 2020 203a 7479 7065 206f 7074  `..    :type opt
+00004100: 696f 6e3a 2064 6963 740a 2020 2020 3a70  ion: dict.    :p
+00004110: 6172 616d 2072 6561 645f 7369 7a65 3a20  aram read_size: 
+00004120: 496e 7075 7420 6275 6666 6572 2073 697a  Input buffer siz
+00004130: 652c 2069 6e20 6279 7465 732e 0a20 2020  e, in bytes..   
+00004140: 203a 7479 7065 2072 6561 645f 7369 7a65   :type read_size
+00004150: 3a20 696e 740a 2020 2020 3a70 6172 616d  : int.    :param
+00004160: 2077 7269 7465 5f73 697a 653a 204f 7574   write_size: Out
+00004170: 7075 7420 6275 6666 6572 2073 697a 652c  put buffer size,
+00004180: 2069 6e20 6279 7465 732e 0a20 2020 203a   in bytes..    :
+00004190: 7479 7065 2077 7269 7465 5f73 697a 653a  type write_size:
+000041a0: 2069 6e74 0a20 2020 203a 7061 7261 6d20   int.    :param 
+000041b0: 6361 6c6c 6261 636b 3a20 4120 6361 6c6c  callback: A call
+000041c0: 6261 636b 2066 756e 6374 696f 6e20 7468  back function th
+000041d0: 6174 2061 6363 6570 7473 2066 6f75 7220  at accepts four 
+000041e0: 7061 7261 6d65 7465 7273 3a20 6060 2874  parameters: ``(t
+000041f0: 6f74 616c 5f69 6e70 7574 2c20 746f 7461  otal_input, tota
+00004200: 6c5f 6f75 7470 7574 2c20 7265 6164 5f64  l_output, read_d
+00004210: 6174 612c 2077 7269 7465 5f64 6174 6129  ata, write_data)
+00004220: 6060 2e20 5468 6520 6669 7273 7420 7477  ``. The first tw
+00004230: 6f20 6172 6520 6060 696e 7460 6020 6f62  o are ``int`` ob
+00004240: 6a65 6374 732e 2054 6865 206c 6173 7420  jects. The last 
+00004250: 7477 6f20 6172 6520 7265 6164 6f6e 6c79  two are readonly
+00004260: 2060 6d65 6d6f 7279 7669 6577 203c 6874   `memoryview <ht
+00004270: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00004280: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00004290: 7374 6474 7970 6573 2e68 746d 6c23 6d65  stdtypes.html#me
+000042a0: 6d6f 7279 2d76 6965 7773 3e60 5f20 6f62  mory-views>`_ ob
+000042b0: 6a65 6374 732c 2069 6620 7761 6e74 2074  jects, if want t
+000042c0: 6f20 7265 6665 7265 6e63 6520 7468 6520  o reference the 
+000042d0: 6461 7461 2028 6f72 2069 7473 2073 6c69  data (or its sli
+000042e0: 6365 2920 6f75 7473 6964 6520 7468 6520  ce) outside the 
+000042f0: 6361 6c6c 6261 636b 2066 756e 6374 696f  callback functio
+00004300: 6e2c 2060 636f 6e76 6572 7420 3c68 7474  n, `convert <htt
+00004310: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00004320: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f73  .org/3/library/s
+00004330: 7464 7479 7065 732e 6874 6d6c 236d 656d  tdtypes.html#mem
+00004340: 6f72 7976 6965 772e 746f 6279 7465 733e  oryview.tobytes>
+00004350: 605f 2074 6865 6d20 746f 2060 6062 7974  `_ them to ``byt
+00004360: 6573 6060 206f 626a 6563 7473 2e20 4966  es`` objects. If
+00004370: 2069 6e70 7574 2073 7472 6561 6d20 6973   input stream is
+00004380: 2060 6062 2727 6060 2c20 7468 6520 6361   ``b''``, the ca
+00004390: 6c6c 6261 636b 2066 756e 6374 696f 6e20  llback function 
+000043a0: 7769 6c6c 206e 6f74 2062 6520 6361 6c6c  will not be call
+000043b0: 6564 2e0a 2020 2020 3a74 7970 6520 6361  ed..    :type ca
+000043c0: 6c6c 6261 636b 3a20 6361 6c6c 6162 6c65  llback: callable
+000043d0: 0a20 2020 203a 7265 7475 726e 3a20 4120  .    :return: A 
+000043e0: 322d 6974 656d 2074 7570 6c65 2c20 6060  2-item tuple, ``
+000043f0: 2874 6f74 616c 5f69 6e70 7574 2c20 746f  (total_input, to
+00004400: 7461 6c5f 6f75 7470 7574 2960 602c 2074  tal_output)``, t
+00004410: 6865 2069 7465 6d73 2061 7265 2060 6069  he items are ``i
+00004420: 6e74 6060 206f 626a 6563 7473 2e0a 2020  nt`` objects..  
+00004430: 2020 3a72 6169 7365 7320 5a73 7464 4572    :raises ZstdEr
+00004440: 726f 723a 2049 6620 6465 636f 6d70 7265  ror: If decompre
+00004450: 7373 696f 6e20 6661 696c 732e 0a0a 2020  ssion fails...  
+00004460: 2020 2e2e 2073 6f75 7263 6563 6f64 653a    .. sourcecode:
+00004470: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+00004480: 2020 2320 6465 636f 6d70 7265 7373 2061    # decompress a
+00004490: 6e20 696e 7075 7420 6669 6c65 2c20 616e  n input file, an
+000044a0: 6420 7772 6974 6520 746f 2061 6e20 6f75  d write to an ou
+000044b0: 7470 7574 2066 696c 652e 0a20 2020 2020  tput file..     
+000044c0: 2020 2077 6974 6820 696f 2e6f 7065 6e28     with io.open(
+000044d0: 696e 7075 745f 6669 6c65 5f70 6174 682c  input_file_path,
+000044e0: 2027 7262 2729 2061 7320 6966 683a 0a20   'rb') as ifh:. 
+000044f0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00004500: 696f 2e6f 7065 6e28 6f75 7470 7574 5f66  io.open(output_f
+00004510: 696c 655f 7061 7468 2c20 2777 6227 2920  ile_path, 'wb') 
+00004520: 6173 206f 6668 3a0a 2020 2020 2020 2020  as ofh:.        
+00004530: 2020 2020 2020 2020 6465 636f 6d70 7265          decompre
+00004540: 7373 5f73 7472 6561 6d28 6966 682c 206f  ss_stream(ifh, o
+00004550: 6668 290a 0a20 2020 2020 2020 2023 2064  fh)..        # d
+00004560: 6563 6f6d 7072 6573 7320 6120 6279 7465  ecompress a byte
+00004570: 7320 6f62 6a65 6374 2c20 616e 6420 7772  s object, and wr
+00004580: 6974 6520 746f 2061 2066 696c 652e 0a20  ite to a file.. 
+00004590: 2020 2020 2020 2077 6974 6820 696f 2e42         with io.B
+000045a0: 7974 6573 494f 2863 6f6d 7072 6573 7365  ytesIO(compresse
+000045b0: 645f 6461 7429 2061 7320 6269 3a0a 2020  d_dat) as bi:.  
+000045c0: 2020 2020 2020 2020 2020 7769 7468 2069            with i
+000045d0: 6f2e 6f70 656e 286f 7574 7075 745f 6669  o.open(output_fi
+000045e0: 6c65 5f70 6174 682c 2027 7762 2729 2061  le_path, 'wb') a
+000045f0: 7320 6f66 683a 0a20 2020 2020 2020 2020  s ofh:.         
+00004600: 2020 2020 2020 2064 6563 6f6d 7072 6573         decompres
+00004610: 735f 7374 7265 616d 2862 692c 206f 6668  s_stream(bi, ofh
+00004620: 290a 0a20 2020 2020 2020 2023 2044 6563  )..        # Dec
+00004630: 6f6d 7072 6573 7320 616e 2069 6e70 7574  ompress an input
+00004640: 2066 696c 652c 206f 6274 6169 6e20 6120   file, obtain a 
+00004650: 6279 7465 7320 6f62 6a65 6374 2e0a 2020  bytes object..  
+00004660: 2020 2020 2020 2320 4974 2773 2066 6173        # It's fas
+00004670: 7465 7220 7468 616e 2072 6561 6469 6e67  ter than reading
+00004680: 2061 2066 696c 6520 616e 6420 6465 636f   a file and deco
+00004690: 6d70 7265 7373 696e 6720 6974 2069 6e0a  mpressing it in.
+000046a0: 2020 2020 2020 2020 2320 6d65 6d6f 7279          # memory
+000046b0: 2c20 7465 7374 6564 206f 6e20 5562 756e  , tested on Ubun
+000046c0: 7475 2850 7974 686f 6e33 2e38 292f 5769  tu(Python3.8)/Wi
+000046d0: 6e64 6f77 7328 5079 7468 6f6e 332e 3929  ndows(Python3.9)
+000046e0: 2e0a 2020 2020 2020 2020 2320 4d61 7962  ..        # Mayb
+000046f0: 6520 7468 6520 4f53 2068 6173 2070 7265  e the OS has pre
+00004700: 6665 7463 6869 6e67 2c20 6974 2063 616e  fetching, it can
+00004710: 2072 6561 6420 616e 6420 6465 636f 6d70   read and decomp
+00004720: 7265 7373 0a20 2020 2020 2020 2023 2064  ress.        # d
+00004730: 6174 6120 696e 2070 6172 616c 6c65 6c20  ata in parallel 
+00004740: 746f 2073 6f6d 6520 6465 6772 6565 2c20  to some degree, 
+00004750: 7265 6164 696e 6720 6669 6c65 2066 726f  reading file fro
+00004760: 6d20 4844 440a 2020 2020 2020 2020 2320  m HDD.        # 
+00004770: 6973 2074 6865 2062 6f74 746c 656e 6563  is the bottlenec
+00004780: 6b20 696e 2074 6869 7320 6361 7365 2e0a  k in this case..
+00004790: 2020 2020 2020 2020 7769 7468 2069 6f2e          with io.
+000047a0: 6f70 656e 2869 6e70 7574 5f66 696c 655f  open(input_file_
+000047b0: 7061 7468 2c20 2772 6227 2920 6173 2069  path, 'rb') as i
+000047c0: 6668 3a0a 2020 2020 2020 2020 2020 2020  fh:.            
+000047d0: 7769 7468 2069 6f2e 4279 7465 7349 4f28  with io.BytesIO(
+000047e0: 2920 6173 2062 6f3a 0a20 2020 2020 2020  ) as bo:.       
+000047f0: 2020 2020 2020 2020 2064 6563 6f6d 7072           decompr
+00004800: 6573 735f 7374 7265 616d 2869 6668 2c20  ess_stream(ifh, 
+00004810: 626f 290a 2020 2020 2020 2020 2020 2020  bo).            
+00004820: 2020 2020 6465 636f 6d70 7265 7373 6564      decompressed
+00004830: 5f64 6174 203d 2062 6f2e 6765 7476 616c  _dat = bo.getval
+00004840: 7565 2829 0a0a 2020 2020 2020 2020 2320  ue()..        # 
+00004850: 5072 696e 7420 7072 6f67 7265 7373 2075  Print progress u
+00004860: 7369 6e67 2063 616c 6c62 6163 6b20 6675  sing callback fu
+00004870: 6e63 7469 6f6e 0a20 2020 2020 2020 2064  nction.        d
+00004880: 6566 2064 6563 6f6d 7072 6573 735f 7072  ef decompress_pr
+00004890: 696e 745f 7072 6f67 7265 7373 2869 6e70  int_progress(inp
+000048a0: 7574 5f66 696c 655f 7061 7468 2c20 6f75  ut_file_path, ou
+000048b0: 7470 7574 5f66 696c 655f 7061 7468 293a  tput_file_path):
+000048c0: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
+000048d0: 7574 5f66 696c 655f 7369 7a65 203d 206f  ut_file_size = o
+000048e0: 732e 7061 7468 2e67 6574 7369 7a65 2869  s.path.getsize(i
+000048f0: 6e70 7574 5f66 696c 655f 7061 7468 290a  nput_file_path).
+00004900: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+00004910: 2066 756e 6328 746f 7461 6c5f 696e 7075   func(total_inpu
+00004920: 742c 2074 6f74 616c 5f6f 7574 7075 742c  t, total_output,
+00004930: 2072 6561 645f 6461 7461 2c20 7772 6974   read_data, writ
+00004940: 655f 6461 7461 293a 0a20 2020 2020 2020  e_data):.       
+00004950: 2020 2020 2020 2020 2023 2049 6620 696e           # If in
+00004960: 7075 7420 7374 7265 616d 2069 7320 656d  put stream is em
+00004970: 7074 792c 2074 6865 2063 616c 6c62 6163  pty, the callbac
+00004980: 6b20 6675 6e63 7469 6f6e 0a20 2020 2020  k function.     
+00004990: 2020 2020 2020 2020 2020 2023 2077 696c             # wil
+000049a0: 6c20 6e6f 7420 6265 2063 616c 6c65 642e  l not be called.
+000049b0: 2053 6f20 6e6f 205a 6572 6f44 6976 6973   So no ZeroDivis
+000049c0: 696f 6e45 7272 6f72 2068 6572 652e 0a20  ionError here.. 
+000049d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000049e0: 6572 6365 6e74 203d 2031 3030 202a 2074  ercent = 100 * t
+000049f0: 6f74 616c 5f69 6e70 7574 202f 2069 6e70  otal_input / inp
+00004a00: 7574 5f66 696c 655f 7369 7a65 0a20 2020  ut_file_size.   
+00004a10: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00004a20: 6e74 2866 2750 726f 6772 6573 733a 207b  nt(f'Progress: {
+00004a30: 7065 7263 656e 743a 2e31 667d 2527 2c20  percent:.1f}%', 
+00004a40: 656e 643d 275c 7227 290a 0a20 2020 2020  end='\r')..     
+00004a50: 2020 2020 2020 2077 6974 6820 696f 2e6f         with io.o
+00004a60: 7065 6e28 696e 7075 745f 6669 6c65 5f70  pen(input_file_p
+00004a70: 6174 682c 2027 7262 2729 2061 7320 6966  ath, 'rb') as if
+00004a80: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+00004a90: 2020 2077 6974 6820 696f 2e6f 7065 6e28     with io.open(
+00004aa0: 6f75 7470 7574 5f66 696c 655f 7061 7468  output_file_path
+00004ab0: 2c20 2777 6227 2920 6173 206f 6668 3a0a  , 'wb') as ofh:.
+00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ad0: 2020 2020 6465 636f 6d70 7265 7373 5f73      decompress_s
+00004ae0: 7472 6561 6d28 6966 682c 206f 6668 2c20  tream(ifh, ofh, 
+00004af0: 6361 6c6c 6261 636b 3d66 756e 6329 0a0a  callback=func)..
+00004b00: 0a2e 2e20 7079 3a63 6c61 7373 3a3a 205a  ... py:class:: Z
+00004b10: 7374 6444 6563 6f6d 7072 6573 736f 720a  stdDecompressor.
+00004b20: 0a20 2020 2041 2073 7472 6561 6d69 6e67  .    A streaming
+00004b30: 2064 6563 6f6d 7072 6573 736f 722e 0a0a   decompressor...
+00004b40: 2020 2020 4166 7465 7220 6120 3a72 6566      After a :ref
+00004b50: 3a60 6672 616d 653c 6672 616d 655f 626c  :`frame<frame_bl
+00004b60: 6f63 6b3e 6020 6973 2064 6563 6f6d 7072  ock>` is decompr
+00004b70: 6573 7365 642c 2069 7420 7374 6f70 7320  essed, it stops 
+00004b80: 616e 6420 7365 7473 203a 7079 3a61 7474  and sets :py:att
+00004b90: 723a 607e 5a73 7464 4465 636f 6d70 7265  r:`~ZstdDecompre
+00004ba0: 7373 6f72 2e65 6f66 6020 666c 6167 2074  ssor.eof` flag t
+00004bb0: 6f20 6060 5472 7565 6060 2e0a 0a20 2020  o ``True``...   
+00004bc0: 2046 6f72 206d 756c 7469 706c 6520 6672   For multiple fr
+00004bd0: 616d 6573 2064 6174 612c 2075 7365 203a  ames data, use :
+00004be0: 7079 3a63 6c61 7373 3a60 456e 646c 6573  py:class:`Endles
+00004bf0: 735a 7374 6444 6563 6f6d 7072 6573 736f  sZstdDecompresso
+00004c00: 7260 2e0a 0a20 2020 2054 6872 6561 642d  r`...    Thread-
+00004c10: 7361 6665 2061 7420 6d65 7468 6f64 206c  safe at method l
+00004c20: 6576 656c 2e0a 0a20 2020 202e 2e20 7079  evel...    .. py
+00004c30: 3a6d 6574 686f 643a 3a20 5f5f 696e 6974  :method:: __init
+00004c40: 5f5f 2873 656c 662c 207a 7374 645f 6469  __(self, zstd_di
+00004c50: 6374 3d4e 6f6e 652c 206f 7074 696f 6e3d  ct=None, option=
+00004c60: 4e6f 6e65 290a 0a20 2020 2020 2020 2049  None)..        I
+00004c70: 6e69 7469 616c 697a 6520 6120 5a73 7464  nitialize a Zstd
+00004c80: 4465 636f 6d70 7265 7373 6f72 206f 626a  Decompressor obj
+00004c90: 6563 742e 0a0a 2020 2020 2020 2020 3a70  ect...        :p
+00004ca0: 6172 616d 207a 7374 645f 6469 6374 3a20  aram zstd_dict: 
+00004cb0: 5072 652d 7472 6169 6e65 6420 6469 6374  Pre-trained dict
+00004cc0: 696f 6e61 7279 2066 6f72 2064 6563 6f6d  ionary for decom
+00004cd0: 7072 6573 7369 6f6e 2e0a 2020 2020 2020  pression..      
+00004ce0: 2020 3a74 7970 6520 7a73 7464 5f64 6963    :type zstd_dic
+00004cf0: 743a 205a 7374 6444 6963 740a 2020 2020  t: ZstdDict.    
+00004d00: 2020 2020 3a70 6172 616d 2064 6963 7420      :param dict 
+00004d10: 6f70 7469 6f6e 3a20 4120 6060 6469 6374  option: A ``dict
+00004d20: 6060 206f 626a 6563 7420 7468 6174 2063  `` object that c
+00004d30: 6f6e 7461 696e 7320 3a72 6566 3a60 6164  ontains :ref:`ad
+00004d40: 7661 6e63 6564 2064 6563 6f6d 7072 6573  vanced decompres
+00004d50: 7369 6f6e 2070 6172 616d 6574 6572 733c  sion parameters<
+00004d60: 4450 6172 616d 6574 6572 3e60 2e20 5468  DParameter>`. Th
+00004d70: 6520 6465 6661 756c 7420 7661 6c75 6520  e default value 
+00004d80: 6060 4e6f 6e65 6060 206d 6561 6e73 2074  ``None`` means t
+00004d90: 6f20 7573 6520 7a73 7464 2773 2064 6566  o use zstd's def
+00004da0: 6175 6c74 2064 6563 6f6d 7072 6573 7369  ault decompressi
+00004db0: 6f6e 2070 6172 616d 6574 6572 732e 0a0a  on parameters...
+00004dc0: 2020 2020 2e2e 2070 793a 6d65 7468 6f64      .. py:method
+00004dd0: 3a3a 2064 6563 6f6d 7072 6573 7328 7365  :: decompress(se
+00004de0: 6c66 2c20 6461 7461 2c20 6d61 785f 6c65  lf, data, max_le
+00004df0: 6e67 7468 3d2d 3129 0a0a 2020 2020 2020  ngth=-1)..      
+00004e00: 2020 4465 636f 6d70 7265 7373 202a 6461    Decompress *da
+00004e10: 7461 2a2c 2072 6574 7572 6e69 6e67 2064  ta*, returning d
+00004e20: 6563 6f6d 7072 6573 7365 6420 6461 7461  ecompressed data
+00004e30: 2061 7320 6120 6060 6279 7465 7360 6020   as a ``bytes`` 
+00004e40: 6f62 6a65 6374 2e0a 0a20 2020 2020 2020  object...       
+00004e50: 2041 6674 6572 2061 203a 7265 663a 6066   After a :ref:`f
+00004e60: 7261 6d65 3c66 7261 6d65 5f62 6c6f 636b  rame<frame_block
+00004e70: 3e60 2069 7320 6465 636f 6d70 7265 7373  >` is decompress
+00004e80: 6564 2c20 6974 2073 746f 7073 2061 6e64  ed, it stops and
+00004e90: 2073 6574 7320 3a70 793a 6174 7472 3a60   sets :py:attr:`
+00004ea0: 7e5a 7374 6444 6563 6f6d 7072 6573 736f  ~ZstdDecompresso
+00004eb0: 722e 656f 6660 2066 6c61 6720 746f 2060  r.eof` flag to `
+00004ec0: 6054 7275 6560 602e 0a0a 2020 2020 2020  `True``...      
+00004ed0: 2020 3a70 6172 616d 2064 6174 613a 2044    :param data: D
+00004ee0: 6174 6120 746f 2062 6520 6465 636f 6d70  ata to be decomp
+00004ef0: 7265 7373 6564 2e0a 2020 2020 2020 2020  ressed..        
+00004f00: 3a74 7970 6520 6461 7461 3a20 6279 7465  :type data: byte
+00004f10: 732d 6c69 6b65 206f 626a 6563 740a 2020  s-like object.  
+00004f20: 2020 2020 2020 3a70 6172 616d 2069 6e74        :param int
+00004f30: 206d 6178 5f6c 656e 6774 683a 204d 6178   max_length: Max
+00004f40: 696d 756d 2073 697a 6520 6f66 2072 6574  imum size of ret
+00004f50: 7572 6e65 6420 6461 7461 2e20 5768 656e  urned data. When
+00004f60: 2069 7427 7320 6e65 6761 7469 7665 2c20   it's negative, 
+00004f70: 7468 6520 6f75 7470 7574 2073 697a 6520  the output size 
+00004f80: 6973 2075 6e6c 696d 6974 6564 2e20 5768  is unlimited. Wh
+00004f90: 656e 2069 7427 7320 6e6f 6e2d 6e65 6761  en it's non-nega
+00004fa0: 7469 7665 2c20 7265 7475 726e 7320 6174  tive, returns at
+00004fb0: 206d 6f73 7420 2a6d 6178 5f6c 656e 6774   most *max_lengt
+00004fc0: 682a 2062 7974 6573 206f 6620 6465 636f  h* bytes of deco
+00004fd0: 6d70 7265 7373 6564 2064 6174 612e 2049  mpressed data. I
+00004fe0: 6620 7468 6973 206c 696d 6974 2069 7320  f this limit is 
+00004ff0: 7265 6163 6865 6420 616e 6420 6675 7274  reached and furt
+00005000: 6865 7220 6f75 7470 7574 2063 616e 2028  her output can (
+00005010: 6f72 206d 6179 2920 6265 2070 726f 6475  or may) be produ
+00005020: 6365 642c 2074 6865 203a 7079 3a61 7474  ced, the :py:att
+00005030: 723a 607e 5a73 7464 4465 636f 6d70 7265  r:`~ZstdDecompre
+00005040: 7373 6f72 2e6e 6565 6473 5f69 6e70 7574  ssor.needs_input
+00005050: 6020 6174 7472 6962 7574 6520 7769 6c6c  ` attribute will
+00005060: 2062 6520 7365 7420 746f 2060 6046 616c   be set to ``Fal
+00005070: 7365 6060 2e20 496e 2074 6869 7320 6361  se``. In this ca
+00005080: 7365 2c20 7468 6520 6e65 7874 2063 616c  se, the next cal
+00005090: 6c20 746f 2074 6869 7320 6d65 7468 6f64  l to this method
+000050a0: 206d 6179 2070 726f 7669 6465 202a 6461   may provide *da
+000050b0: 7461 2a20 6173 2060 6062 2727 6060 2074  ta* as ``b''`` t
+000050c0: 6f20 6f62 7461 696e 206d 6f72 6520 6f66  o obtain more of
+000050d0: 2074 6865 206f 7574 7075 742e 0a0a 2020   the output...  
+000050e0: 2020 2e2e 2070 793a 6174 7472 6962 7574    .. py:attribut
+000050f0: 653a 3a20 6e65 6564 735f 696e 7075 740a  e:: needs_input.
+00005100: 0a20 2020 2020 2020 2049 6620 7468 6520  .        If the 
+00005110: 2a6d 6178 5f6c 656e 6774 682a 206f 7574  *max_length* out
+00005120: 7075 7420 6c69 6d69 7420 696e 203a 7079  put limit in :py
+00005130: 3a6d 6574 683a 607e 5a73 7464 4465 636f  :meth:`~ZstdDeco
+00005140: 6d70 7265 7373 6f72 2e64 6563 6f6d 7072  mpressor.decompr
+00005150: 6573 7360 206d 6574 686f 6420 6861 7320  ess` method has 
+00005160: 6265 656e 2072 6561 6368 6564 2c20 616e  been reached, an
+00005170: 6420 7468 6520 6465 636f 6d70 7265 7373  d the decompress
+00005180: 6f72 2068 6173 2028 6f72 206d 6179 2068  or has (or may h
+00005190: 6173 2920 756e 636f 6e73 756d 6564 2069  as) unconsumed i
+000051a0: 6e70 7574 2064 6174 612c 2069 7420 7769  nput data, it wi
+000051b0: 6c6c 2062 6520 7365 7420 746f 2060 6046  ll be set to ``F
+000051c0: 616c 7365 6060 2e20 496e 2074 6869 7320  alse``. In this 
+000051d0: 6361 7365 2c20 7061 7373 2060 6062 2727  case, pass ``b''
+000051e0: 6060 2074 6f20 3a70 793a 6d65 7468 3a60  `` to :py:meth:`
+000051f0: 7e5a 7374 6444 6563 6f6d 7072 6573 736f  ~ZstdDecompresso
+00005200: 722e 6465 636f 6d70 7265 7373 6020 6d65  r.decompress` me
+00005210: 7468 6f64 206d 6179 206f 7574 7075 7420  thod may output 
+00005220: 6675 7274 6865 7220 6461 7461 2e0a 0a20  further data... 
+00005230: 2020 2020 2020 2049 6620 6967 6e6f 7265         If ignore
+00005240: 2074 6869 7320 6174 7472 6962 7574 6520   this attribute 
+00005250: 7768 656e 2074 6865 7265 2069 7320 756e  when there is un
+00005260: 636f 6e73 756d 6564 2069 6e70 7574 2064  consumed input d
+00005270: 6174 612c 2074 6865 7265 2077 696c 6c20  ata, there will 
+00005280: 6265 2061 206c 6974 746c 6520 7065 7266  be a little perf
+00005290: 6f72 6d61 6e63 6520 6c6f 7373 2062 6563  ormance loss bec
+000052a0: 6175 7365 206f 6620 6578 7472 6120 6d65  ause of extra me
+000052b0: 6d6f 7279 2063 6f70 792e 0a0a 2020 2020  mory copy...    
+000052c0: 2e2e 2070 793a 6174 7472 6962 7574 653a  .. py:attribute:
+000052d0: 3a20 656f 660a 0a20 2020 2020 2020 2060  : eof..        `
+000052e0: 6054 7275 6560 6020 6d65 616e 7320 7468  `True`` means th
+000052f0: 6520 656e 6420 6f66 2074 6865 2066 6972  e end of the fir
+00005300: 7374 2066 7261 6d65 2068 6173 2062 6565  st frame has bee
+00005310: 6e20 7265 6163 6865 642e 2049 6620 6465  n reached. If de
+00005320: 636f 6d70 7265 7373 2064 6174 6120 6166  compress data af
+00005330: 7465 7220 7468 6174 2c20 616e 2060 6045  ter that, an ``E
+00005340: 4f46 4572 726f 7260 6020 6578 6365 7074  OFError`` except
+00005350: 696f 6e20 7769 6c6c 2062 6520 7261 6973  ion will be rais
+00005360: 6564 2e0a 0a20 2020 202e 2e20 7079 3a61  ed...    .. py:a
+00005370: 7474 7269 6275 7465 3a3a 2075 6e75 7365  ttribute:: unuse
+00005380: 645f 6461 7461 0a0a 2020 2020 2020 2020  d_data..        
+00005390: 4120 6279 7465 7320 6f62 6a65 6374 2e20  A bytes object. 
+000053a0: 5768 656e 205a 7374 6444 6563 6f6d 7072  When ZstdDecompr
+000053b0: 6573 736f 7220 6f62 6a65 6374 2073 746f  essor object sto
+000053c0: 7073 2061 6674 6572 2064 6563 6f6d 7072  ps after decompr
+000053d0: 6573 7369 6e67 2061 2066 7261 6d65 2c20  essing a frame, 
+000053e0: 756e 7573 6564 2069 6e70 7574 2064 6174  unused input dat
+000053f0: 6120 6166 7465 7220 7468 6520 6669 7273  a after the firs
+00005400: 7420 6672 616d 652e 204f 7468 6572 7769  t frame. Otherwi
+00005410: 7365 2074 6869 7320 7769 6c6c 2062 6520  se this will be 
+00005420: 6060 6227 2760 602e 0a0a 2020 2020 2e2e  ``b''``...    ..
+00005430: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
+00005440: 7468 6f6e 0a0a 2020 2020 2020 2020 2320  thon..        # 
+00005450: 2d2d 2d20 756e 6c69 6d69 7465 6420 6f75  --- unlimited ou
+00005460: 7470 7574 202d 2d2d 0a20 2020 2020 2020  tput ---.       
+00005470: 2064 3120 3d20 5a73 7464 4465 636f 6d70   d1 = ZstdDecomp
+00005480: 7265 7373 6f72 2829 0a0a 2020 2020 2020  ressor()..      
+00005490: 2020 6465 636f 6d70 7265 7373 6564 5f64    decompressed_d
+000054a0: 6174 3120 3d20 6431 2e64 6563 6f6d 7072  at1 = d1.decompr
+000054b0: 6573 7328 6461 7431 290a 2020 2020 2020  ess(dat1).      
+000054c0: 2020 6465 636f 6d70 7265 7373 6564 5f64    decompressed_d
+000054d0: 6174 3220 3d20 6431 2e64 6563 6f6d 7072  at2 = d1.decompr
+000054e0: 6573 7328 6461 7432 290a 2020 2020 2020  ess(dat2).      
+000054f0: 2020 6465 636f 6d70 7265 7373 6564 5f64    decompressed_d
+00005500: 6174 3320 3d20 6431 2e64 6563 6f6d 7072  at3 = d1.decompr
+00005510: 6573 7328 6461 7433 290a 0a20 2020 2020  ess(dat3)..     
+00005520: 2020 2061 7373 6572 7420 6431 2e65 6f66     assert d1.eof
+00005530: 2c20 2764 6174 6120 6973 2061 6e20 696e  , 'data is an in
+00005540: 636f 6d70 6c65 7465 207a 7374 6420 6672  complete zstd fr
+00005550: 616d 652e 270a 0a20 2020 2020 2020 2023  ame.'..        #
+00005560: 202d 2d2d 206c 696d 6974 6564 206f 7574   --- limited out
+00005570: 7075 7420 2d2d 2d0a 2020 2020 2020 2020  put ---.        
+00005580: 6432 203d 205a 7374 6444 6563 6f6d 7072  d2 = ZstdDecompr
+00005590: 6573 736f 7228 290a 0a20 2020 2020 2020  essor()..       
+000055a0: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
+000055b0: 2020 2020 2020 2020 2069 6620 6432 2e6e           if d2.n
+000055c0: 6565 6473 5f69 6e70 7574 3a0a 2020 2020  eeds_input:.    
+000055d0: 2020 2020 2020 2020 2020 2020 6461 7420              dat 
+000055e0: 3d20 7265 6164 5f69 6e70 7574 2832 2a31  = read_input(2*1
+000055f0: 3032 342a 3130 3234 2920 2320 7265 6164  024*1024) # read
+00005600: 2032 204d 6942 2069 6e70 7574 2064 6174   2 MiB input dat
+00005610: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00005620: 2020 6966 206e 6f74 2064 6174 3a20 2320    if not dat: # 
+00005630: 696e 7075 7420 7374 7265 616d 2065 6e64  input stream end
+00005640: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00005650: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+00005660: 7074 696f 6e28 2749 6e70 7574 2073 7472  ption('Input str
+00005670: 6561 6d20 656e 6473 2c20 6275 7420 7468  eam ends, but th
+00005680: 6520 656e 6420 6f66 2027 0a20 2020 2020  e end of '.     
+00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000056b0: 7468 6520 6669 7273 7420 6672 616d 6520  the first frame 
+000056c0: 6973 206e 6f74 2072 6561 6368 6564 2e27  is not reached.'
+000056d0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+000056e0: 7365 3a20 2320 6d61 7962 6520 7468 6572  se: # maybe ther
+000056f0: 6520 6973 2075 6e63 6f6e 7375 6d65 6420  e is unconsumed 
+00005700: 696e 7075 7420 6461 7461 0a20 2020 2020  input data.     
+00005710: 2020 2020 2020 2020 2020 2064 6174 203d             dat =
+00005720: 2062 2727 0a0a 2020 2020 2020 2020 2020   b''..          
+00005730: 2020 6368 756e 6b20 3d20 6432 2e64 6563    chunk = d2.dec
+00005740: 6f6d 7072 6573 7328 6461 742c 2031 302a  ompress(dat, 10*
+00005750: 3130 3234 2a31 3032 3429 2023 206c 696d  1024*1024) # lim
+00005760: 6974 206f 7574 7075 7420 6275 6666 6572  it output buffer
+00005770: 2074 6f20 3130 204d 6942 0a20 2020 2020   to 10 MiB.     
+00005780: 2020 2020 2020 2077 7269 7465 5f6f 7574         write_out
+00005790: 7075 7428 6368 756e 6b29 0a0a 2020 2020  put(chunk)..    
+000057a0: 2020 2020 2020 2020 6966 2064 322e 656f          if d2.eo
+000057b0: 663a 2023 2072 6561 6368 2074 6865 2065  f: # reach the e
+000057c0: 6e64 206f 6620 7468 6520 6669 7273 7420  nd of the first 
+000057d0: 6672 616d 650a 2020 2020 2020 2020 2020  frame.          
+000057e0: 2020 2020 2020 6272 6561 6b0a 0a0a 2e2e        break.....
+000057f0: 2070 793a 636c 6173 733a 3a20 456e 646c   py:class:: Endl
+00005800: 6573 735a 7374 6444 6563 6f6d 7072 6573  essZstdDecompres
+00005810: 736f 720a 0a20 2020 2041 2073 7472 6561  sor..    A strea
+00005820: 6d69 6e67 2064 6563 6f6d 7072 6573 736f  ming decompresso
+00005830: 722e 0a0a 2020 2020 4974 2064 6f65 736e  r...    It doesn
+00005840: 2774 2073 746f 7020 6166 7465 7220 6120  't stop after a 
+00005850: 3a72 6566 3a60 6672 616d 653c 6672 616d  :ref:`frame<fram
+00005860: 655f 626c 6f63 6b3e 6020 6973 2064 6563  e_block>` is dec
+00005870: 6f6d 7072 6573 7365 642c 2063 616e 2062  ompressed, can b
+00005880: 6520 7573 6564 2074 6f20 6465 636f 6d70  e used to decomp
+00005890: 7265 7373 206d 756c 7469 706c 6520 636f  ress multiple co
+000058a0: 6e63 6174 656e 6174 6564 2066 7261 6d65  ncatenated frame
+000058b0: 732e 0a0a 2020 2020 5468 7265 6164 2d73  s...    Thread-s
+000058c0: 6166 6520 6174 206d 6574 686f 6420 6c65  afe at method le
+000058d0: 7665 6c2e 0a0a 2020 2020 2e2e 2070 793a  vel...    .. py:
+000058e0: 6d65 7468 6f64 3a3a 205f 5f69 6e69 745f  method:: __init_
+000058f0: 5f28 7365 6c66 2c20 7a73 7464 5f64 6963  _(self, zstd_dic
+00005900: 743d 4e6f 6e65 2c20 6f70 7469 6f6e 3d4e  t=None, option=N
+00005910: 6f6e 6529 0a0a 2020 2020 2020 2020 5468  one)..        Th
+00005920: 6520 7061 7261 6d65 7465 7273 2061 7265  e parameters are
+00005930: 2074 6865 2073 616d 6520 6173 203a 7079   the same as :py
+00005940: 3a6d 6574 683a 605a 7374 6444 6563 6f6d  :meth:`ZstdDecom
+00005950: 7072 6573 736f 722e 5f5f 696e 6974 5f5f  pressor.__init__
+00005960: 6020 6d65 7468 6f64 2e0a 0a20 2020 202e  ` method...    .
+00005970: 2e20 7079 3a6d 6574 686f 643a 3a20 6465  . py:method:: de
+00005980: 636f 6d70 7265 7373 2873 656c 662c 2064  compress(self, d
+00005990: 6174 612c 206d 6178 5f6c 656e 6774 683d  ata, max_length=
+000059a0: 2d31 290a 0a20 2020 2020 2020 2054 6865  -1)..        The
+000059b0: 2070 6172 616d 6574 6572 7320 6172 6520   parameters are 
+000059c0: 7468 6520 7361 6d65 2061 7320 3a70 793a  the same as :py:
+000059d0: 6d65 7468 3a60 5a73 7464 4465 636f 6d70  meth:`ZstdDecomp
+000059e0: 7265 7373 6f72 2e64 6563 6f6d 7072 6573  ressor.decompres
+000059f0: 7360 206d 6574 686f 642e 0a0a 2020 2020  s` method...    
+00005a00: 2020 2020 4166 7465 7220 6465 636f 6d70      After decomp
+00005a10: 7265 7373 696e 6720 6120 6672 616d 652c  ressing a frame,
+00005a20: 2069 7420 646f 6573 6e27 7420 7374 6f70   it doesn't stop
+00005a30: 206c 696b 6520 3a70 793a 6d65 7468 3a60   like :py:meth:`
+00005a40: 5a73 7464 4465 636f 6d70 7265 7373 6f72  ZstdDecompressor
+00005a50: 2e64 6563 6f6d 7072 6573 7360 2e0a 0a20  .decompress`... 
+00005a60: 2020 202e 2e20 7079 3a61 7474 7269 6275     .. py:attribu
+00005a70: 7465 3a3a 206e 6565 6473 5f69 6e70 7574  te:: needs_input
+00005a80: 0a0a 2020 2020 2020 2020 4974 2773 2074  ..        It's t
+00005a90: 6865 2073 616d 6520 6173 203a 7079 3a61  he same as :py:a
+00005aa0: 7474 723a 605a 7374 6444 6563 6f6d 7072  ttr:`ZstdDecompr
+00005ab0: 6573 736f 722e 6e65 6564 735f 696e 7075  essor.needs_inpu
+00005ac0: 7460 2e0a 0a20 2020 202e 2e20 7079 3a61  t`...    .. py:a
+00005ad0: 7474 7269 6275 7465 3a3a 2061 745f 6672  ttribute:: at_fr
+00005ae0: 616d 655f 6564 6765 0a0a 2020 2020 2020  ame_edge..      
+00005af0: 2020 6060 5472 7565 6060 2077 6865 6e20    ``True`` when 
+00005b00: 626f 7468 2074 6865 2069 6e70 7574 2061  both the input a
+00005b10: 6e64 206f 7574 7075 7420 7374 7265 616d  nd output stream
+00005b20: 7320 6172 6520 6174 2061 203a 7265 663a  s are at a :ref:
+00005b30: 6066 7261 6d65 3c66 7261 6d65 5f62 6c6f  `frame<frame_blo
+00005b40: 636b 3e60 2065 6467 652c 206f 7220 7468  ck>` edge, or th
+00005b50: 6520 6465 636f 6d70 7265 7373 6f72 206a  e decompressor j
+00005b60: 7573 7420 6265 2069 6e69 7469 616c 697a  ust be initializ
+00005b70: 6564 2e0a 0a20 2020 2020 2020 2054 6869  ed...        Thi
+00005b80: 7320 666c 6167 2063 6f75 6c64 2062 6520  s flag could be 
+00005b90: 7573 6564 2074 6f20 6368 6563 6b20 6461  used to check da
+00005ba0: 7461 2069 6e74 6567 7269 7479 2069 6e20  ta integrity in 
+00005bb0: 736f 6d65 2063 6173 6573 2e0a 0a20 2020  some cases...   
+00005bc0: 202e 2e20 736f 7572 6365 636f 6465 3a3a   .. sourcecode::
+00005bd0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+00005be0: 2023 202d 2d2d 2073 7472 6561 6d69 6e67   # --- streaming
+00005bf0: 2064 6563 6f6d 7072 6573 7369 6f6e 2c20   decompression, 
+00005c00: 756e 6c69 6d69 7465 6420 6f75 7470 7574  unlimited output
+00005c10: 202d 2d2d 0a20 2020 2020 2020 2064 3120   ---.        d1 
+00005c20: 3d20 456e 646c 6573 735a 7374 6444 6563  = EndlessZstdDec
+00005c30: 6f6d 7072 6573 736f 7228 290a 0a20 2020  ompressor()..   
+00005c40: 2020 2020 2064 6563 6f6d 7072 6573 7365       decompresse
+00005c50: 645f 6461 7431 203d 2064 312e 6465 636f  d_dat1 = d1.deco
+00005c60: 6d70 7265 7373 2864 6174 3129 0a20 2020  mpress(dat1).   
+00005c70: 2020 2020 2064 6563 6f6d 7072 6573 7365       decompresse
+00005c80: 645f 6461 7432 203d 2064 312e 6465 636f  d_dat2 = d1.deco
+00005c90: 6d70 7265 7373 2864 6174 3229 0a20 2020  mpress(dat2).   
+00005ca0: 2020 2020 2064 6563 6f6d 7072 6573 7365       decompresse
+00005cb0: 645f 6461 7433 203d 2064 312e 6465 636f  d_dat3 = d1.deco
+00005cc0: 6d70 7265 7373 2864 6174 3329 0a0a 2020  mpress(dat3)..  
+00005cd0: 2020 2020 2020 6173 7365 7274 2064 312e        assert d1.
+00005ce0: 6174 5f66 7261 6d65 5f65 6467 652c 2027  at_frame_edge, '
+00005cf0: 6461 7461 2065 6e64 7320 696e 2061 6e20  data ends in an 
+00005d00: 696e 636f 6d70 6c65 7465 2066 7261 6d65  incomplete frame
+00005d10: 2e27 0a0a 2020 2020 2020 2020 2320 2d2d  .'..        # --
+00005d20: 2d20 7374 7265 616d 696e 6720 6465 636f  - streaming deco
+00005d30: 6d70 7265 7373 696f 6e2c 206c 696d 6974  mpression, limit
+00005d40: 6564 206f 7574 7075 7420 2d2d 2d0a 2020  ed output ---.  
+00005d50: 2020 2020 2020 6432 203d 2045 6e64 6c65        d2 = Endle
+00005d60: 7373 5a73 7464 4465 636f 6d70 7265 7373  ssZstdDecompress
+00005d70: 6f72 2829 0a0a 2020 2020 2020 2020 7768  or()..        wh
+00005d80: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
+00005d90: 2020 2020 2020 6966 2064 322e 6e65 6564        if d2.need
+00005da0: 735f 696e 7075 743a 0a20 2020 2020 2020  s_input:.       
+00005db0: 2020 2020 2020 2020 2064 6174 203d 2072           dat = r
+00005dc0: 6561 645f 696e 7075 7428 322a 3130 3234  ead_input(2*1024
+00005dd0: 2a31 3032 3429 2023 2072 6561 6420 3220  *1024) # read 2 
+00005de0: 4d69 4220 696e 7075 7420 6461 7461 0a20  MiB input data. 
+00005df0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005e00: 6620 6e6f 7420 6461 743a 2023 2069 6e70  f not dat: # inp
+00005e10: 7574 2073 7472 6561 6d20 656e 6473 0a20  ut stream ends. 
+00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e30: 2020 2069 6620 6e6f 7420 6432 2e61 745f     if not d2.at_
+00005e40: 6672 616d 655f 6564 6765 3a0a 2020 2020  frame_edge:.    
+00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e60: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+00005e70: 696f 6e28 2764 6174 6120 656e 6473 2069  ion('data ends i
+00005e80: 6e20 616e 2069 6e63 6f6d 706c 6574 6520  n an incomplete 
+00005e90: 6672 616d 652e 2729 0a20 2020 2020 2020  frame.').       
+00005ea0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00005eb0: 616b 0a20 2020 2020 2020 2020 2020 2065  ak.            e
+00005ec0: 6c73 653a 2023 206d 6179 6265 2074 6865  lse: # maybe the
+00005ed0: 7265 2069 7320 756e 636f 6e73 756d 6564  re is unconsumed
+00005ee0: 2069 6e70 7574 2064 6174 610a 2020 2020   input data.    
+00005ef0: 2020 2020 2020 2020 2020 2020 6461 7420              dat 
+00005f00: 3d20 6227 270a 0a20 2020 2020 2020 2020  = b''..         
+00005f10: 2020 2063 6875 6e6b 203d 2064 322e 6465     chunk = d2.de
+00005f20: 636f 6d70 7265 7373 2864 6174 2c20 3130  compress(dat, 10
+00005f30: 2a31 3032 342a 3130 3234 2920 2320 6c69  *1024*1024) # li
+00005f40: 6d69 7420 6f75 7470 7574 2062 7566 6665  mit output buffe
+00005f50: 7220 746f 2031 3020 4d69 420a 2020 2020  r to 10 MiB.    
+00005f60: 2020 2020 2020 2020 7772 6974 655f 6f75          write_ou
+00005f70: 7470 7574 2863 6875 6e6b 290a 0a20 2020  tput(chunk)..   
+00005f80: 202e 2e20 6869 6e74 3a3a 2057 6879 203a   .. hint:: Why :
+00005f90: 7079 3a63 6c61 7373 3a60 456e 646c 6573  py:class:`Endles
+00005fa0: 735a 7374 6444 6563 6f6d 7072 6573 736f  sZstdDecompresso
+00005fb0: 7260 2064 6f65 736e 2774 2073 746f 7020  r` doesn't stop 
+00005fc0: 6174 2066 7261 6d65 2065 6467 6573 3f0a  at frame edges?.
+00005fd0: 0a20 2020 2020 2020 2049 6620 736f 2c20  .        If so, 
+00005fe0: 756e 7573 6564 2069 6e70 7574 2064 6174  unused input dat
+00005ff0: 6120 6166 7465 7220 616e 2065 6467 6520  a after an edge 
+00006000: 7769 6c6c 2062 6520 636f 7069 6564 2074  will be copied t
+00006010: 6f20 616e 2069 6e74 6572 6e61 6c20 6275  o an internal bu
+00006020: 6666 6572 2c20 7468 6973 206d 6179 2062  ffer, this may b
+00006030: 6520 6120 7065 7266 6f72 6d61 6e63 6520  e a performance 
+00006040: 6f76 6572 6865 6164 2e0a 0a20 2020 2020  overhead...     
+00006050: 2020 2049 6620 7761 6e74 2074 6f20 7374     If want to st
+00006060: 6f70 2061 7420 6672 616d 6520 6564 6765  op at frame edge
+00006070: 732c 2077 7269 7465 2061 2077 7261 7070  s, write a wrapp
+00006080: 6572 2075 7369 6e67 203a 7079 3a63 6c61  er using :py:cla
+00006090: 7373 3a60 5a73 7464 4465 636f 6d70 7265  ss:`ZstdDecompre
+000060a0: 7373 6f72 6020 636c 6173 732e 2041 6e64  ssor` class. And
+000060b0: 2064 6f6e 2774 2066 6565 6420 746f 6f20   don't feed too 
+000060c0: 6d75 6368 2064 6174 6120 6576 6572 7920  much data every 
+000060d0: 7469 6d65 2c20 7468 6520 6f76 6572 6865  time, the overhe
+000060e0: 6164 206f 6620 636f 7079 696e 6720 756e  ad of copying un
+000060f0: 7573 6564 2069 6e70 7574 2064 6174 6120  used input data 
+00006100: 746f 203a 7079 3a61 7474 723a 605a 7374  to :py:attr:`Zst
+00006110: 6444 6563 6f6d 7072 6573 736f 722e 756e  dDecompressor.un
+00006120: 7573 6564 5f64 6174 6160 2061 7474 7269  used_data` attri
+00006130: 6275 7465 2073 7469 6c6c 2065 7869 7374  bute still exist
+00006140: 732e 0a0a 0a2e 2e20 5f7a 7374 645f 6469  s...... _zstd_di
+00006150: 6374 3a0a 0a44 6963 7469 6f6e 6172 790a  ct:..Dictionary.
+00006160: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020  ----------..    
+00006170: 5468 6973 2073 6563 7469 6f6e 2063 6f6e  This section con
+00006180: 7461 696e 733a 0a0a 2020 2020 2020 2020  tains:..        
+00006190: 2a20 636c 6173 7320 3a70 793a 636c 6173  * class :py:clas
+000061a0: 733a 605a 7374 6444 6963 7460 0a20 2020  s:`ZstdDict`.   
+000061b0: 2020 2020 202a 2066 756e 6374 696f 6e20       * function 
+000061c0: 3a70 793a 6675 6e63 3a60 7472 6169 6e5f  :py:func:`train_
+000061d0: 6469 6374 600a 2020 2020 2020 2020 2a20  dict`.        * 
+000061e0: 6675 6e63 7469 6f6e 203a 7079 3a66 756e  function :py:fun
+000061f0: 633a 6066 696e 616c 697a 655f 6469 6374  c:`finalize_dict
+00006200: 600a 0a2e 2e20 6e6f 7465 3a3a 0a20 2020  `.... note::.   
+00006210: 2049 6620 7573 6520 7072 652d 7472 6169   If use pre-trai
+00006220: 6e65 6420 7a73 7464 2064 6963 7469 6f6e  ned zstd diction
+00006230: 6172 792c 2074 6865 2063 6f6d 7072 6573  ary, the compres
+00006240: 7369 6f6e 2072 6174 696f 2061 6368 6965  sion ratio achie
+00006250: 7661 626c 6520 6f6e 2073 6d61 6c6c 2064  vable on small d
+00006260: 6174 6120 2861 2066 6577 204b 6942 2920  ata (a few KiB) 
+00006270: 696d 7072 6f76 6573 2064 7261 6d61 7469  improves dramati
+00006280: 6361 6c6c 792e 0a0a 2020 2020 2a2a 4261  cally...    **Ba
+00006290: 636b 6772 6f75 6e64 2a2a 0a0a 2020 2020  ckground**..    
+000062a0: 5468 6520 736d 616c 6c65 7220 7468 6520  The smaller the 
+000062b0: 616d 6f75 6e74 206f 6620 6461 7461 2074  amount of data t
+000062c0: 6f20 636f 6d70 7265 7373 2c20 7468 6520  o compress, the 
+000062d0: 6d6f 7265 2064 6966 6669 6375 6c74 2069  more difficult i
+000062e0: 7420 6973 2074 6f20 636f 6d70 7265 7373  t is to compress
+000062f0: 2e20 5468 6973 2070 726f 626c 656d 2069  . This problem i
+00006300: 7320 636f 6d6d 6f6e 2074 6f20 616c 6c20  s common to all 
+00006310: 636f 6d70 7265 7373 696f 6e20 616c 676f  compression algo
+00006320: 7269 7468 6d73 2c20 616e 6420 7265 6173  rithms, and reas
+00006330: 6f6e 2069 732c 2063 6f6d 7072 6573 7369  on is, compressi
+00006340: 6f6e 2061 6c67 6f72 6974 686d 7320 6c65  on algorithms le
+00006350: 6172 6e20 6672 6f6d 2070 6173 7420 6461  arn from past da
+00006360: 7461 2068 6f77 2074 6f20 636f 6d70 7265  ta how to compre
+00006370: 7373 2066 7574 7572 6520 6461 7461 2e20  ss future data. 
+00006380: 4275 7420 6174 2074 6865 2062 6567 696e  But at the begin
+00006390: 6e69 6e67 206f 6620 6120 6e65 7720 6461  ning of a new da
+000063a0: 7461 2073 6574 2c20 7468 6572 6520 6973  ta set, there is
+000063b0: 206e 6f20 2270 6173 7422 2074 6f20 6275   no "past" to bu
+000063c0: 696c 6420 7570 6f6e 2e0a 0a20 2020 205a  ild upon...    Z
+000063d0: 7374 6420 7472 6169 6e69 6e67 206d 6f64  std training mod
+000063e0: 6520 6361 6e20 6265 2075 7365 6420 746f  e can be used to
+000063f0: 2074 756e 6520 7468 6520 616c 676f 7269   tune the algori
+00006400: 7468 6d20 666f 7220 6120 7365 6c65 6374  thm for a select
+00006410: 6564 2074 7970 6520 6f66 2064 6174 612e  ed type of data.
+00006420: 2054 7261 696e 696e 6720 6973 2061 6368   Training is ach
+00006430: 6965 7665 6420 6279 2070 726f 7669 6469  ieved by providi
+00006440: 6e67 2069 7420 7769 7468 2061 2066 6577  ng it with a few
+00006450: 2073 616d 706c 6573 2028 6f6e 6520 6669   samples (one fi
+00006460: 6c65 2070 6572 2073 616d 706c 6529 2e20  le per sample). 
+00006470: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
+00006480: 6973 2074 7261 696e 696e 6720 6973 2073  is training is s
+00006490: 746f 7265 6420 696e 2061 2066 696c 6520  tored in a file 
+000064a0: 6361 6c6c 6564 2022 6469 6374 696f 6e61  called "dictiona
+000064b0: 7279 222c 2077 6869 6368 206d 7573 7420  ry", which must 
+000064c0: 6265 206c 6f61 6465 6420 6265 666f 7265  be loaded before
+000064d0: 2063 6f6d 7072 6573 7369 6f6e 2061 6e64   compression and
+000064e0: 2064 6563 6f6d 7072 6573 7369 6f6e 2e0a   decompression..
+000064f0: 0a20 2020 2053 6565 2074 6865 2046 4151  .    See the FAQ
+00006500: 2069 6e20 6074 6869 7320 6669 6c65 203c   in `this file <
+00006510: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00006520: 6f6d 2f66 6163 6562 6f6f 6b2f 7a73 7464  om/facebook/zstd
+00006530: 2f62 6c6f 622f 6465 762f 6c69 622f 7a64  /blob/dev/lib/zd
+00006540: 6963 742e 683e 605f 2066 6f72 2064 6574  ict.h>`_ for det
+00006550: 6169 6c73 2e0a 0a20 2020 202e 2e20 6174  ails...    .. at
+00006560: 7465 6e74 696f 6e3a 3a0a 0a20 2020 2020  tention::..     
+00006570: 2020 2023 2e20 4966 2079 6f75 206c 6f73     #. If you los
+00006580: 6520 6120 7a73 7464 2064 6963 7469 6f6e  e a zstd diction
+00006590: 6172 792c 2074 6865 6e20 6361 6e27 7420  ary, then can't 
+000065a0: 6465 636f 6d70 7265 7373 2074 6865 2063  decompress the c
+000065b0: 6f72 7265 7370 6f6e 6469 6e67 2064 6174  orresponding dat
+000065c0: 612e 0a20 2020 2020 2020 2023 2e20 5a73  a..        #. Zs
+000065d0: 7464 2064 6963 7469 6f6e 6172 7920 6861  td dictionary ha
+000065e0: 7320 6e65 676c 6967 6962 6c65 2065 6666  s negligible eff
+000065f0: 6563 7420 6f6e 206c 6172 6765 2064 6174  ect on large dat
+00006600: 6120 286d 756c 7469 2d4d 6942 2920 636f  a (multi-MiB) co
+00006610: 6d70 7265 7373 696f 6e2e 2049 6620 7761  mpression. If wa
+00006620: 6e74 2074 6f20 7573 6520 6c61 7267 6520  nt to use large 
+00006630: 6469 6374 696f 6e61 7279 2063 6f6e 7465  dictionary conte
+00006640: 6e74 2c20 7365 6520 7072 6566 6978 283a  nt, see prefix(:
+00006650: 7079 3a61 7474 723a 605a 7374 6444 6963  py:attr:`ZstdDic
+00006660: 742e 6173 5f70 7265 6669 7860 292e 0a20  t.as_prefix`).. 
+00006670: 2020 2020 2020 2023 2e20 5468 6572 6520         #. There 
+00006680: 6973 2061 2070 6f73 7369 6269 6c69 7479  is a possibility
+00006690: 2074 6861 7420 7468 6520 6469 6374 696f   that the dictio
+000066a0: 6e61 7279 2063 6f6e 7465 6e74 2063 6f75  nary content cou
+000066b0: 6c64 2062 6520 6d61 6c69 6369 6f75 736c  ld be maliciousl
+000066c0: 7920 7461 6d70 6572 6564 2062 7920 6120  y tampered by a 
+000066d0: 7468 6972 6420 7061 7274 792e 0a0a 2020  third party...  
+000066e0: 2020 2a2a 4164 7661 6e63 6564 2064 6963    **Advanced dic
+000066f0: 7469 6f6e 6172 7920 7472 6169 6e69 6e67  tionary training
+00006700: 2a2a 0a0a 2020 2020 5079 7a73 7464 206d  **..    Pyzstd m
+00006710: 6f64 756c 6520 6f6e 6c79 2075 7365 7320  odule only uses 
+00006720: 7a73 7464 206c 6962 7261 7279 2773 2073  zstd library's s
+00006730: 7461 626c 6520 4150 492e 2054 6865 2073  table API. The s
+00006740: 7461 626c 6520 4150 4920 6f6e 6c79 2065  table API only e
+00006750: 7870 6f73 6573 2074 776f 2064 6963 7469  xposes two dicti
+00006760: 6f6e 6172 7920 7472 6169 6e69 6e67 2066  onary training f
+00006770: 756e 6374 696f 6e73 2074 6861 7420 636f  unctions that co
+00006780: 7272 6573 706f 6e64 696e 6720 746f 203a  rresponding to :
+00006790: 7079 3a66 756e 633a 6074 7261 696e 5f64  py:func:`train_d
+000067a0: 6963 7460 2061 6e64 203a 7079 3a66 756e  ict` and :py:fun
+000067b0: 633a 6066 696e 616c 697a 655f 6469 6374  c:`finalize_dict
+000067c0: 602e 0a0a 2020 2020 4966 2077 616e 7420  `...    If want 
+000067d0: 746f 2061 646a 7573 7420 6164 7661 6e63  to adjust advanc
+000067e0: 6564 2074 7261 696e 696e 6720 7061 7261  ed training para
+000067f0: 6d65 7465 7273 2c20 796f 7520 6d61 7920  meters, you may 
+00006800: 7573 6520 7a73 7464 2773 2043 4c49 2070  use zstd's CLI p
+00006810: 726f 6772 616d 2028 6e6f 7420 7079 7a73  rogram (not pyzs
+00006820: 7464 206d 6f64 756c 6527 7320 434c 4929  td module's CLI)
+00006830: 2c20 6974 2068 6173 2065 6e74 7269 6573  , it has entries
+00006840: 2074 6f20 7a73 7464 206c 6962 7261 7279   to zstd library
+00006850: 2773 2065 7870 6572 696d 656e 7461 6c20  's experimental 
+00006860: 4150 492e 0a0a 2e2e 2070 793a 636c 6173  API..... py:clas
+00006870: 733a 3a20 5a73 7464 4469 6374 0a0a 2020  s:: ZstdDict..  
+00006880: 2020 5265 7072 6573 656e 7473 2061 207a    Represents a z
+00006890: 7374 6420 6469 6374 696f 6e61 7279 2c20  std dictionary, 
+000068a0: 6361 6e20 6265 2075 7365 6420 666f 7220  can be used for 
+000068b0: 636f 6d70 7265 7373 696f 6e2f 6465 636f  compression/deco
+000068c0: 6d70 7265 7373 696f 6e2e 0a0a 2020 2020  mpression...    
+000068d0: 4974 2773 2074 6872 6561 642d 7361 6665  It's thread-safe
+000068e0: 2c20 616e 6420 6361 6e20 6265 2073 6861  , and can be sha
+000068f0: 7265 6420 6279 206d 756c 7469 706c 6520  red by multiple 
+00006900: 3a70 793a 636c 6173 733a 605a 7374 6443  :py:class:`ZstdC
+00006910: 6f6d 7072 6573 736f 7260 202f 203a 7079  ompressor` / :py
+00006920: 3a63 6c61 7373 3a60 5a73 7464 4465 636f  :class:`ZstdDeco
+00006930: 6d70 7265 7373 6f72 6020 6f62 6a65 6374  mpressor` object
+00006940: 732e 0a0a 2020 2020 2e2e 2073 6f75 7263  s...    .. sourc
+00006950: 6563 6f64 653a 3a20 7079 7468 6f6e 0a0a  ecode:: python..
+00006960: 2020 2020 2020 2020 2320 6c6f 6164 2061          # load a
+00006970: 207a 7374 6420 6469 6374 696f 6e61 7279   zstd dictionary
+00006980: 2066 726f 6d20 6669 6c65 0a20 2020 2020   from file.     
+00006990: 2020 2077 6974 6820 696f 2e6f 7065 6e28     with io.open(
+000069a0: 6469 6374 5f70 6174 682c 2027 7262 2729  dict_path, 'rb')
+000069b0: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
+000069c0: 2020 2066 696c 655f 636f 6e74 656e 7420     file_content 
+000069d0: 3d20 662e 7265 6164 2829 0a20 2020 2020  = f.read().     
+000069e0: 2020 207a 6420 3d20 5a73 7464 4469 6374     zd = ZstdDict
+000069f0: 2866 696c 655f 636f 6e74 656e 7429 0a0a  (file_content)..
+00006a00: 2020 2020 2020 2020 2320 7573 6520 7468          # use th
+00006a10: 6520 6469 6374 696f 6e61 7279 2074 6f20  e dictionary to 
+00006a20: 636f 6d70 7265 7373 2e0a 2020 2020 2020  compress..      
+00006a30: 2020 2320 6966 2075 7365 2061 2064 6963    # if use a dic
+00006a40: 7469 6f6e 6172 7920 666f 7220 636f 6d70  tionary for comp
+00006a50: 7265 7373 6f72 206d 756c 7469 706c 6520  ressor multiple 
+00006a60: 7469 6d65 732c 2072 6575 7369 6e67 0a20  times, reusing. 
+00006a70: 2020 2020 2020 2023 2061 2063 6f6d 7072         # a compr
+00006a80: 6573 736f 7220 6f62 6a65 6374 2069 7320  essor object is 
+00006a90: 6661 7374 6572 2c20 7365 6520 2e61 735f  faster, see .as_
+00006aa0: 756e 6469 6765 7374 6564 5f64 6963 7420  undigested_dict 
+00006ab0: 646f 632e 0a20 2020 2020 2020 2063 6f6d  doc..        com
+00006ac0: 7072 6573 7365 645f 6461 7420 3d20 636f  pressed_dat = co
+00006ad0: 6d70 7265 7373 2872 6177 5f64 6174 2c20  mpress(raw_dat, 
+00006ae0: 7a73 7464 5f64 6963 743d 7a64 290a 0a20  zstd_dict=zd).. 
+00006af0: 2020 2020 2020 2023 2075 7365 2074 6865         # use the
+00006b00: 2064 6963 7469 6f6e 6172 7920 746f 2064   dictionary to d
+00006b10: 6563 6f6d 7072 6573 730a 2020 2020 2020  ecompress.      
+00006b20: 2020 6465 636f 6d70 7265 7373 6564 5f64    decompressed_d
+00006b30: 6174 203d 2064 6563 6f6d 7072 6573 7328  at = decompress(
+00006b40: 636f 6d70 7265 7373 6564 5f64 6174 2c20  compressed_dat, 
+00006b50: 7a73 7464 5f64 6963 743d 7a64 290a 0a20  zstd_dict=zd).. 
+00006b60: 2020 202e 2e20 7665 7273 696f 6e63 6861     .. versioncha
+00006b70: 6e67 6564 3a3a 2030 2e31 352e 370a 2020  nged:: 0.15.7.  
+00006b80: 2020 2020 2020 5768 656e 2063 6f6d 7072        When compr
+00006b90: 6573 7369 6e67 2c20 6c6f 6164 2075 6e64  essing, load und
+00006ba0: 6967 6573 7465 6420 6469 6374 696f 6e61  igested dictiona
+00006bb0: 7279 2069 6e73 7465 6164 206f 6620 6469  ry instead of di
+00006bc0: 6765 7374 6564 2064 6963 7469 6f6e 6172  gested dictionar
+00006bd0: 7920 6279 2064 6566 6175 6c74 2c20 7365  y by default, se
+00006be0: 6520 3a70 793a 6174 7472 3a60 7e5a 7374  e :py:attr:`~Zst
+00006bf0: 6444 6963 742e 6173 5f64 6967 6573 7465  dDict.as_digeste
+00006c00: 645f 6469 6374 602e 2041 6c73 6f20 6164  d_dict`. Also ad
+00006c10: 6420 6060 2e5f 5f6c 656e 5f5f 2829 6060  d ``.__len__()``
+00006c20: 206d 6574 686f 6420 7468 6174 2072 6574   method that ret
+00006c30: 7572 6e69 6e67 2063 6f6e 7465 6e74 2073  urning content s
+00006c40: 697a 652e 0a0a 2020 2020 2e2e 2070 793a  ize...    .. py:
+00006c50: 6d65 7468 6f64 3a3a 205f 5f69 6e69 745f  method:: __init_
+00006c60: 5f28 7365 6c66 2c20 6469 6374 5f63 6f6e  _(self, dict_con
+00006c70: 7465 6e74 2c20 6973 5f72 6177 3d46 616c  tent, is_raw=Fal
+00006c80: 7365 290a 0a20 2020 2020 2020 2049 6e69  se)..        Ini
+00006c90: 7469 616c 697a 6520 6120 5a73 7464 4469  tialize a ZstdDi
+00006ca0: 6374 206f 626a 6563 742e 0a0a 2020 2020  ct object...    
+00006cb0: 2020 2020 3a70 6172 616d 2064 6963 745f      :param dict_
+00006cc0: 636f 6e74 656e 743a 2044 6963 7469 6f6e  content: Diction
+00006cd0: 6172 7927 7320 636f 6e74 656e 742e 0a20  ary's content.. 
+00006ce0: 2020 2020 2020 203a 7479 7065 2064 6963         :type dic
+00006cf0: 745f 636f 6e74 656e 743a 2062 7974 6573  t_content: bytes
+00006d00: 2d6c 696b 6520 6f62 6a65 6374 0a20 2020  -like object.   
+00006d10: 2020 2020 203a 7061 7261 6d20 6973 5f72       :param is_r
+00006d20: 6177 3a20 5468 6973 2070 6172 616d 6574  aw: This paramet
+00006d30: 6572 2069 7320 666f 7220 6164 7661 6e63  er is for advanc
+00006d40: 6564 2075 7365 722e 2060 6054 7275 6560  ed user. ``True`
+00006d50: 6020 6d65 616e 7320 2a64 6963 745f 636f  ` means *dict_co
+00006d60: 6e74 656e 742a 2061 7267 756d 656e 7420  ntent* argument 
+00006d70: 6973 2061 2022 7261 7720 636f 6e74 656e  is a "raw conten
+00006d80: 7422 2064 6963 7469 6f6e 6172 792c 2066  t" dictionary, f
+00006d90: 7265 6520 6f66 2061 6e79 2066 6f72 6d61  ree of any forma
+00006da0: 7420 7265 7374 7269 6374 696f 6e2e 2060  t restriction. `
+00006db0: 6046 616c 7365 6060 206d 6561 6e73 202a  `False`` means *
+00006dc0: 6469 6374 5f63 6f6e 7465 6e74 2a20 6172  dict_content* ar
+00006dd0: 6775 6d65 6e74 2069 7320 616e 206f 7264  gument is an ord
+00006de0: 696e 6172 7920 7a73 7464 2064 6963 7469  inary zstd dicti
+00006df0: 6f6e 6172 792c 2077 6173 2063 7265 6174  onary, was creat
+00006e00: 6564 2062 7920 7a73 7464 2066 756e 6374  ed by zstd funct
+00006e10: 696f 6e73 2c20 666f 6c6c 6f77 2061 2073  ions, follow a s
+00006e20: 7065 6369 6669 6564 2066 6f72 6d61 742e  pecified format.
+00006e30: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
+00006e40: 735f 7261 773a 2062 6f6f 6c0a 0a20 2020  s_raw: bool..   
+00006e50: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+00006e60: 3a3a 2064 6963 745f 636f 6e74 656e 740a  :: dict_content.
+00006e70: 0a20 2020 2020 2020 2054 6865 2063 6f6e  .        The con
+00006e80: 7465 6e74 206f 6620 7a73 7464 2064 6963  tent of zstd dic
+00006e90: 7469 6f6e 6172 792c 2061 2060 6062 7974  tionary, a ``byt
+00006ea0: 6573 6060 206f 626a 6563 742e 2049 7427  es`` object. It'
+00006eb0: 7320 7468 6520 7361 6d65 2061 7320 2a64  s the same as *d
+00006ec0: 6963 745f 636f 6e74 656e 742a 2061 7267  ict_content* arg
+00006ed0: 756d 656e 7420 696e 203a 7079 3a6d 6574  ument in :py:met
+00006ee0: 683a 607e 5a73 7464 4469 6374 2e5f 5f69  h:`~ZstdDict.__i
+00006ef0: 6e69 745f 5f60 206d 6574 686f 642e 2049  nit__` method. I
+00006f00: 7420 6361 6e20 6265 2075 7365 6420 7769  t can be used wi
+00006f10: 7468 206f 7468 6572 2070 726f 6772 616d  th other program
+00006f20: 732e 0a0a 2020 2020 2e2e 2070 793a 6174  s...    .. py:at
+00006f30: 7472 6962 7574 653a 3a20 6469 6374 5f69  tribute:: dict_i
+00006f40: 640a 0a20 2020 2020 2020 2049 4420 6f66  d..        ID of
+00006f50: 207a 7374 6420 6469 6374 696f 6e61 7279   zstd dictionary
+00006f60: 2c20 6120 3332 2d62 6974 2075 6e73 6967  , a 32-bit unsig
+00006f70: 6e65 6420 696e 7465 6765 7220 7661 6c75  ned integer valu
+00006f80: 652e 2053 6565 203a 7265 663a 6074 6869  e. See :ref:`thi
+00006f90: 7320 6e6f 7465 3c64 6963 745f 6964 3e60  s note<dict_id>`
+00006fa0: 2066 6f72 2064 6574 6169 6c73 2e0a 0a20   for details... 
+00006fb0: 2020 2020 2020 204e 6f6e 2d7a 6572 6f20         Non-zero 
+00006fc0: 6d65 616e 7320 6f72 6469 6e61 7279 2064  means ordinary d
+00006fd0: 6963 7469 6f6e 6172 792c 2077 6173 2063  ictionary, was c
+00006fe0: 7265 6174 6564 2062 7920 7a73 7464 2066  reated by zstd f
+00006ff0: 756e 6374 696f 6e73 2c20 666f 6c6c 6f77  unctions, follow
+00007000: 2061 2073 7065 6369 6669 6564 2066 6f72   a specified for
+00007010: 6d61 742e 0a0a 2020 2020 2020 2020 6060  mat...        ``
+00007020: 3060 6020 6d65 616e 7320 6120 2272 6177  0`` means a "raw
+00007030: 2063 6f6e 7465 6e74 2220 6469 6374 696f   content" dictio
+00007040: 6e61 7279 2c20 6672 6565 206f 6620 616e  nary, free of an
+00007050: 7920 666f 726d 6174 2072 6573 7472 6963  y format restric
+00007060: 7469 6f6e 2c20 7573 6564 2066 6f72 2061  tion, used for a
+00007070: 6476 616e 6365 6420 7573 6572 2e20 284e  dvanced user. (N
+00007080: 6f74 6520 7468 6174 2074 6865 206d 6561  ote that the mea
+00007090: 6e69 6e67 206f 6620 6060 3060 6020 6973  ning of ``0`` is
+000070a0: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
+000070b0: 6060 6469 6374 696f 6e61 7279 5f69 6460  ``dictionary_id`
+000070c0: 6020 696e 203a 7079 3a66 756e 633a 6067  ` in :py:func:`g
+000070d0: 6574 5f66 7261 6d65 5f69 6e66 6f60 2066  et_frame_info` f
+000070e0: 756e 6374 696f 6e2e 290a 0a20 2020 202e  unction.)..    .
+000070f0: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
+00007100: 2061 735f 6469 6765 7374 6564 5f64 6963   as_digested_dic
+00007110: 740a 0a20 2020 2020 2020 204c 6f61 6420  t..        Load 
+00007120: 6173 2061 2064 6967 6573 7465 6420 6469  as a digested di
+00007130: 6374 696f 6e61 7279 2c20 7365 6520 6265  ctionary, see be
+00007140: 6c6f 772e 0a0a 2020 2020 2020 2020 2e2e  low...        ..
+00007150: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
+00007160: 302e 3135 2e37 0a0a 2020 2020 2e2e 2070  0.15.7..    .. p
+00007170: 793a 6174 7472 6962 7574 653a 3a20 6173  y:attribute:: as
+00007180: 5f75 6e64 6967 6573 7465 645f 6469 6374  _undigested_dict
+00007190: 0a0a 2020 2020 2020 2020 4c6f 6164 2061  ..        Load a
+000071a0: 7320 616e 2075 6e64 6967 6573 7465 6420  s an undigested 
+000071b0: 6469 6374 696f 6e61 7279 2e0a 0a20 2020  dictionary...   
+000071c0: 2020 2020 2044 6967 6573 7469 6e67 2064       Digesting d
+000071d0: 6963 7469 6f6e 6172 7920 6973 2061 2063  ictionary is a c
+000071e0: 6f73 746c 7920 6f70 6572 6174 696f 6e2e  ostly operation.
+000071f0: 2054 6865 7365 2074 776f 2061 7474 7269   These two attri
+00007200: 6275 7465 7320 6361 6e20 636f 6e74 726f  butes can contro
+00007210: 6c20 686f 7720 7468 6520 6469 6374 696f  l how the dictio
+00007220: 6e61 7279 2069 7320 6c6f 6164 6564 2074  nary is loaded t
+00007230: 6f20 636f 6d70 7265 7373 6f72 2c20 6279  o compressor, by
+00007240: 2070 6173 7369 6e67 2074 6865 6d20 6173   passing them as
+00007250: 2060 7a73 7464 5f64 6963 7460 2061 7267   `zstd_dict` arg
+00007260: 756d 656e 743a 2060 6063 6f6d 7072 6573  ument: ``compres
+00007270: 7328 6461 742c 207a 7374 645f 6469 6374  s(dat, zstd_dict
+00007280: 3d7a 642e 6173 5f64 6967 6573 7465 645f  =zd.as_digested_
+00007290: 6469 6374 2960 600a 0a20 2020 2020 2020  dict)``..       
+000072a0: 2049 6620 646f 6e27 7420 7370 6563 6966   If don't specif
+000072b0: 7920 7468 6573 6520 7477 6f20 6174 7472  y these two attr
+000072c0: 6962 7574 6573 2c20 7573 6520 2a2a 756e  ibutes, use **un
+000072d0: 6469 6765 7374 6564 2a2a 2064 6963 7469  digested** dicti
+000072e0: 6f6e 6172 7920 666f 7220 636f 6d70 7265  onary for compre
+000072f0: 7373 696f 6e20 6279 2064 6566 6175 6c74  ssion by default
+00007300: 3a20 6060 636f 6d70 7265 7373 2864 6174  : ``compress(dat
+00007310: 2c20 7a73 7464 5f64 6963 743d 7a64 2960  , zstd_dict=zd)`
+00007320: 600a 0a20 2020 2020 2020 202e 2e20 6c69  `..        .. li
+00007330: 7374 2d74 6162 6c65 3a3a 2044 6966 6665  st-table:: Diffe
+00007340: 7265 6e63 6520 666f 7220 636f 6d70 7265  rence for compre
+00007350: 7373 696f 6e0a 2020 2020 2020 2020 2020  ssion.          
+00007360: 2020 3a77 6964 7468 733a 2031 3220 3132    :widths: 12 12
+00007370: 2031 320a 2020 2020 2020 2020 2020 2020   12.            
+00007380: 3a68 6561 6465 722d 726f 7773 3a20 310a  :header-rows: 1.
+00007390: 0a20 2020 2020 2020 2020 2020 202a 202d  .            * -
+000073a0: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
+000073b0: 207c 2044 6967 6573 7465 640a 2020 2020   | Digested.    
+000073c0: 2020 2020 2020 2020 2020 2020 7c20 6469              | di
+000073d0: 6374 696f 6e61 7279 0a20 2020 2020 2020  ctionary.       
+000073e0: 2020 2020 2020 202d 207c 2055 6e64 6967         - | Undig
+000073f0: 6573 7465 640a 2020 2020 2020 2020 2020  ested.          
+00007400: 2020 2020 2020 7c20 6469 6374 696f 6e61        | dictiona
+00007410: 7279 0a20 2020 2020 2020 2020 2020 202a  ry.            *
+00007420: 202d 207c 2053 6f6d 6520 6164 7661 6e63   - | Some advanc
+00007430: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+00007440: 2020 207c 2070 6172 616d 6574 6572 7320     | parameters 
+00007450: 6f66 0a20 2020 2020 2020 2020 2020 2020  of.             
+00007460: 2020 207c 2063 6f6d 7072 6573 736f 7220     | compressor 
+00007470: 6d61 790a 2020 2020 2020 2020 2020 2020  may.            
+00007480: 2020 2020 7c20 6265 206f 7665 7272 6964      | be overrid
+00007490: 6465 6e0a 2020 2020 2020 2020 2020 2020  den.            
+000074a0: 2020 2020 7c20 6279 2064 6963 7469 6f6e      | by diction
+000074b0: 6172 7927 730a 2020 2020 2020 2020 2020  ary's.          
+000074c0: 2020 2020 2020 7c20 7061 7261 6d65 7465        | paramete
+000074d0: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
+000074e0: 202d 207c 2060 6077 696e 646f 774c 6f67   - | ``windowLog
+000074f0: 6060 2c20 6060 6861 7368 4c6f 6760 602c  ``, ``hashLog``,
+00007500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007510: 207c 2060 6063 6861 696e 4c6f 6760 602c   | ``chainLog``,
+00007520: 2060 6073 6561 7263 684c 6f67 6060 2c0a   ``searchLog``,.
+00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007540: 7c20 6060 6d69 6e4d 6174 6368 6060 2c20  | ``minMatch``, 
+00007550: 6060 7461 7267 6574 4c65 6e67 7468 6060  ``targetLength``
+00007560: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007570: 2020 7c20 6060 7374 7261 7465 6779 6060    | ``strategy``
+00007580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007590: 2020 7c20 6060 656e 6162 6c65 4c6f 6e67    | ``enableLong
+000075a0: 4469 7374 616e 6365 4d61 7463 6869 6e67  DistanceMatching
+000075b0: 6060 2c0a 2020 2020 2020 2020 2020 2020  ``,.            
+000075c0: 2020 2020 7c20 6060 6c64 6d48 6173 684c      | ``ldmHashL
+000075d0: 6f67 6060 2c20 6060 6c64 6d4d 696e 4d61  og``, ``ldmMinMa
+000075e0: 7463 6860 602c 0a20 2020 2020 2020 2020  tch``,.         
+000075f0: 2020 2020 2020 207c 2060 606c 646d 4275         | ``ldmBu
+00007600: 636b 6574 5369 7a65 4c6f 6760 602c 0a20  cketSizeLog``,. 
+00007610: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007620: 2060 606c 646d 4861 7368 5261 7465 4c6f   ``ldmHashRateLo
+00007630: 6760 602c 2061 6e64 2073 6f6d 650a 2020  g``, and some.  
+00007640: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00007650: 6e6f 6e2d 7075 626c 6963 2070 6172 616d  non-public param
+00007660: 6574 6572 732e 0a20 2020 2020 2020 2020  eters..         
+00007670: 2020 2020 202d 204e 6f0a 2020 2020 2020       - No.      
+00007680: 2020 2020 2020 2a20 2d20 7c20 5a73 7464        * - | Zstd
+00007690: 4469 6374 2068 6173 0a20 2020 2020 2020  Dict has.       
+000076a0: 2020 2020 2020 2020 207c 2069 6e74 6572           | inter
+000076b0: 6e61 6c20 6361 6368 650a 2020 2020 2020  nal cache.      
+000076c0: 2020 2020 2020 2020 2020 7c20 666f 7220            | for 
+000076d0: 7468 6973 0a20 2020 2020 2020 2020 2020  this.           
+000076e0: 2020 202d 207c 2059 6573 2e20 4974 2773     - | Yes. It's
+000076f0: 2066 6173 7465 7220 7768 656e 0a20 2020   faster when.   
+00007700: 2020 2020 2020 2020 2020 2020 207c 206c               | l
+00007710: 6f61 6469 6e67 2061 6761 696e 2061 2064  oading again a d
+00007720: 6967 6573 7465 640a 2020 2020 2020 2020  igested.        
+00007730: 2020 2020 2020 2020 7c20 6469 6374 696f          | dictio
+00007740: 6e61 7279 2077 6974 6820 7468 6520 7361  nary with the sa
+00007750: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
+00007760: 2020 207c 2063 6f6d 7072 6573 7369 6f6e     | compression
+00007770: 206c 6576 656c 2e0a 2020 2020 2020 2020   level..        
+00007780: 2020 2020 2020 2d20 7c20 4e6f 2e20 4966        - | No. If
+00007790: 206c 6f61 6420 616e 2075 6e64 6967 6573   load an undiges
+000077a0: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+000077b0: 2020 2020 7c20 6469 6374 696f 6e61 7279      | dictionary
+000077c0: 206d 756c 7469 706c 6520 7469 6d65 732c   multiple times,
+000077d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000077e0: 207c 2063 6f6e 7369 6465 7220 7265 7573   | consider reus
+000077f0: 696e 6720 610a 2020 2020 2020 2020 2020  ing a.          
+00007800: 2020 2020 2020 7c20 636f 6d70 7265 7373        | compress
+00007810: 6f72 206f 626a 6563 742e 0a0a 2020 2020  or object...    
+00007820: 2020 2020 466f 7220 6465 636f 6d70 7265      For decompre
+00007830: 7373 696f 6e2c 2074 6865 7920 6861 7665  ssion, they have
+00007840: 2074 6865 2073 616d 6520 6566 6665 6374   the same effect
+00007850: 2e20 5079 7a73 7464 2075 7365 7320 2a2a  . Pyzstd uses **
+00007860: 6469 6765 7374 6564 2a2a 2064 6963 7469  digested** dicti
+00007870: 6f6e 6172 7920 666f 7220 6465 636f 6d70  onary for decomp
+00007880: 7265 7373 696f 6e20 6279 2064 6566 6175  ression by defau
+00007890: 6c74 2c20 7768 6963 6820 6973 2066 6173  lt, which is fas
+000078a0: 7465 7220 7768 656e 206c 6f61 6469 6e67  ter when loading
+000078b0: 2061 6761 696e 3a20 6060 6465 636f 6d70   again: ``decomp
+000078c0: 7265 7373 2864 6174 2c20 7a73 7464 5f64  ress(dat, zstd_d
+000078d0: 6963 743d 7a64 2960 600a 0a20 2020 2020  ict=zd)``..     
+000078e0: 2020 202e 2e20 7665 7273 696f 6e61 6464     .. versionadd
+000078f0: 6564 3a3a 2030 2e31 352e 370a 0a20 2020  ed:: 0.15.7..   
+00007900: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+00007910: 3a3a 2061 735f 7072 6566 6978 0a0a 2020  :: as_prefix..  
+00007920: 2020 2020 2020 4c6f 6164 2074 6865 2064        Load the d
+00007930: 6963 7469 6f6e 6172 7920 636f 6e74 656e  ictionary conten
+00007940: 7420 746f 2063 6f6d 7072 6573 736f 722f  t to compressor/
+00007950: 6465 636f 6d70 7265 7373 6f72 2061 7320  decompressor as 
+00007960: 6120 2270 7265 6669 7822 2c20 6279 2070  a "prefix", by p
+00007970: 6173 7369 6e67 2074 6869 7320 6174 7472  assing this attr
+00007980: 6962 7574 6520 6173 2060 7a73 7464 5f64  ibute as `zstd_d
+00007990: 6963 7460 2061 7267 756d 656e 743a 2060  ict` argument: `
+000079a0: 6063 6f6d 7072 6573 7328 6461 742c 207a  `compress(dat, z
+000079b0: 7374 645f 6469 6374 3d7a 642e 6173 5f70  std_dict=zd.as_p
+000079c0: 7265 6669 7829 6060 0a0a 2020 2020 2020  refix)``..      
+000079d0: 2020 5072 6566 6978 2063 616e 2062 6520    Prefix can be 
+000079e0: 7573 6564 2066 6f72 203a 7265 663a 6070  used for :ref:`p
+000079f0: 6174 6368 696e 6720 656e 6769 6e65 3c70  atching engine<p
+00007a00: 6174 6368 696e 675f 656e 6769 6e65 3e60  atching_engine>`
+00007a10: 2073 6365 6e61 7269 6f2e 0a0a 2020 2020   scenario...    
+00007a20: 2020 2020 232e 2050 7265 6669 7820 6973      #. Prefix is
+00007a30: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
+00007a40: 2022 6c6f 6e67 2064 6973 7461 6e63 6520   "long distance 
+00007a50: 6d61 7463 6869 6e67 222c 2077 6869 6c65  matching", while
+00007a60: 2064 6963 7469 6f6e 6172 7920 6973 206e   dictionary is n
+00007a70: 6f74 2e0a 2020 2020 2020 2020 232e 2050  ot..        #. P
+00007a80: 7265 6669 7820 6f6e 6c79 2077 6f72 6b20  refix only work 
+00007a90: 666f 7220 7468 6520 6669 7273 7420 6672  for the first fr
+00007aa0: 616d 652c 2074 6865 6e20 7468 6520 636f  ame, then the co
+00007ab0: 6d70 7265 7373 6f72 2f64 6563 6f6d 7072  mpressor/decompr
+00007ac0: 6573 736f 7220 7769 6c6c 2072 6574 7572  essor will retur
+00007ad0: 6e20 746f 206e 6f20 7072 6566 6978 2073  n to no prefix s
+00007ae0: 7461 7465 2e20 5468 6973 2069 7320 6469  tate. This is di
+00007af0: 6666 6572 656e 7420 6672 6f6d 2064 6963  fferent from dic
+00007b00: 7469 6f6e 6172 7920 7468 6174 2063 616e  tionary that can
+00007b10: 2062 6520 7573 6564 2066 6f72 2061 6c6c   be used for all
+00007b20: 2073 7562 7365 7175 656e 7420 6672 616d   subsequent fram
+00007b30: 6573 2e20 5468 6572 6566 6f72 652c 2062  es. Therefore, b
+00007b40: 6520 6361 7265 6675 6c20 7768 656e 2075  e careful when u
+00007b50: 7369 6e67 2077 6974 6820 5a73 7464 4669  sing with ZstdFi
+00007b60: 6c65 2f53 6565 6b61 626c 655a 7374 6446  le/SeekableZstdF
+00007b70: 696c 652e 0a20 2020 2020 2020 2023 2e20  ile..        #. 
+00007b80: 5768 656e 2064 6563 6f6d 7072 6573 7369  When decompressi
+00007b90: 6e67 2c20 6d75 7374 2075 7365 2074 6865  ng, must use the
+00007ba0: 2073 616d 6520 7072 6566 6978 2061 7320   same prefix as 
+00007bb0: 7768 656e 2063 6f6d 7072 6573 7369 6e67  when compressing
+00007bc0: 2e0a 2020 2020 2020 2020 232e 204c 6f61  ..        #. Loa
+00007bd0: 6469 6e67 2070 7265 6669 7820 746f 2063  ding prefix to c
+00007be0: 6f6d 7072 6573 736f 7220 6973 2063 6f73  ompressor is cos
+00007bf0: 746c 792e 0a20 2020 2020 2020 2023 2e20  tly..        #. 
+00007c00: 4c6f 6164 696e 6720 7072 6566 6978 2074  Loading prefix t
+00007c10: 6f20 6465 636f 6d70 7265 7373 6f72 2069  o decompressor i
+00007c20: 7320 6e6f 7420 636f 7374 6c79 2e0a 0a20  s not costly... 
+00007c30: 2020 2020 2020 202e 2e20 7665 7273 696f         .. versio
+00007c40: 6e61 6464 6564 3a3a 2030 2e31 352e 370a  nadded:: 0.15.7.
+00007c50: 0a0a 2e2e 2070 793a 6675 6e63 7469 6f6e  .... py:function
+00007c60: 3a3a 2074 7261 696e 5f64 6963 7428 7361  :: train_dict(sa
+00007c70: 6d70 6c65 732c 2064 6963 745f 7369 7a65  mples, dict_size
+00007c80: 290a 0a20 2020 2054 7261 696e 2061 207a  )..    Train a z
+00007c90: 7374 6420 6469 6374 696f 6e61 7279 2e0a  std dictionary..
+00007ca0: 0a20 2020 2053 6565 2074 6865 2046 4151  .    See the FAQ
+00007cb0: 2069 6e20 6074 6869 7320 6669 6c65 203c   in `this file <
+00007cc0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00007cd0: 6f6d 2f66 6163 6562 6f6f 6b2f 7a73 7464  om/facebook/zstd
+00007ce0: 2f62 6c6f 622f 7265 6c65 6173 652f 6c69  /blob/release/li
+00007cf0: 622f 7a64 6963 742e 683e 605f 2066 6f72  b/zdict.h>`_ for
+00007d00: 2064 6574 6169 6c73 2e0a 0a20 2020 203a   details...    :
+00007d10: 7061 7261 6d20 7361 6d70 6c65 733a 2041  param samples: A
+00007d20: 6e20 6974 6572 6162 6c65 206f 6620 7361  n iterable of sa
+00007d30: 6d70 6c65 732c 2061 2073 616d 706c 6520  mples, a sample 
+00007d40: 6973 2061 2062 7974 6573 2d6c 696b 6520  is a bytes-like 
+00007d50: 6f62 6a65 6374 2072 6570 7265 7365 6e74  object represent
+00007d60: 7320 6120 6669 6c65 2e0a 2020 2020 3a74  s a file..    :t
+00007d70: 7970 6520 7361 6d70 6c65 733a 2069 7465  ype samples: ite
+00007d80: 7261 626c 650a 2020 2020 3a70 6172 616d  rable.    :param
+00007d90: 2069 6e74 2064 6963 745f 7369 7a65 3a20   int dict_size: 
+00007da0: 5265 7475 726e 6564 207a 7374 6420 6469  Returned zstd di
+00007db0: 6374 696f 6e61 7279 2773 202a 2a6d 6178  ctionary's **max
+00007dc0: 696d 756d 2a2a 2073 697a 652c 2069 6e20  imum** size, in 
+00007dd0: 6279 7465 732e 0a20 2020 203a 7265 7475  bytes..    :retu
+00007de0: 726e 3a20 5472 6169 6e65 6420 7a73 7464  rn: Trained zstd
+00007df0: 2064 6963 7469 6f6e 6172 792e 2049 6620   dictionary. If 
+00007e00: 7761 6e74 2074 6f20 7361 7665 2074 6865  want to save the
+00007e10: 2064 6963 7469 6f6e 6172 7920 746f 2061   dictionary to a
+00007e20: 2066 696c 652c 2073 6176 6520 7468 6520   file, save the 
+00007e30: 3a70 793a 6174 7472 3a60 5a73 7464 4469  :py:attr:`ZstdDi
+00007e40: 6374 2e64 6963 745f 636f 6e74 656e 7460  ct.dict_content`
+00007e50: 2061 7474 7269 6275 7465 2e0a 2020 2020   attribute..    
+00007e60: 3a72 7479 7065 3a20 5a73 7464 4469 6374  :rtype: ZstdDict
+00007e70: 0a0a 2020 2020 2e2e 2073 6f75 7263 6563  ..    .. sourcec
+00007e80: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00007e90: 2020 2020 2020 6465 6620 7361 6d70 6c65        def sample
+00007ea0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00007eb0: 2072 6f6f 7464 6972 203d 2072 2245 3a5c   rootdir = r"E:\
+00007ec0: 6461 7461 220a 0a20 2020 2020 2020 2020  data"..         
+00007ed0: 2020 2023 204e 6f74 6520 7468 6174 2074     # Note that t
+00007ee0: 6865 206f 7264 6572 206f 6620 7468 6520  he order of the 
+00007ef0: 6669 6c65 7320 6d61 7920 6265 2064 6966  files may be dif
+00007f00: 6665 7265 6e74 2c0a 2020 2020 2020 2020  ferent,.        
+00007f10: 2020 2020 2320 7468 6572 6566 6f72 6520      # therefore 
+00007f20: 7468 6520 6765 6e65 7261 7465 6420 6469  the generated di
+00007f30: 6374 696f 6e61 7279 206d 6179 2062 6520  ctionary may be 
+00007f40: 6469 6666 6572 656e 742e 0a20 2020 2020  different..     
+00007f50: 2020 2020 2020 2066 6f72 2070 6172 656e         for paren
+00007f60: 742c 2064 6972 6e61 6d65 732c 2066 696c  t, dirnames, fil
+00007f70: 656e 616d 6573 2069 6e20 6f73 2e77 616c  enames in os.wal
+00007f80: 6b28 726f 6f74 6469 7229 3a0a 2020 2020  k(rootdir):.    
+00007f90: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00007fa0: 6669 6c65 6e61 6d65 2069 6e20 6669 6c65  filename in file
+00007fb0: 6e61 6d65 733a 0a20 2020 2020 2020 2020  names:.         
+00007fc0: 2020 2020 2020 2020 2020 2070 6174 6820             path 
+00007fd0: 3d20 6f73 2e70 6174 682e 6a6f 696e 2870  = os.path.join(p
+00007fe0: 6172 656e 742c 2066 696c 656e 616d 6529  arent, filename)
+00007ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008000: 2020 2020 2077 6974 6820 696f 2e6f 7065       with io.ope
+00008010: 6e28 7061 7468 2c20 2772 6227 2920 6173  n(path, 'rb') as
+00008020: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
+00008030: 2020 2020 2020 2020 2020 2020 6461 7420              dat 
+00008040: 3d20 662e 7265 6164 2829 0a20 2020 2020  = f.read().     
+00008050: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+00008060: 6965 6c64 2064 6174 0a0a 2020 2020 2020  ield dat..      
+00008070: 2020 6469 6320 3d20 7079 7a73 7464 2e74    dic = pyzstd.t
+00008080: 7261 696e 5f64 6963 7428 7361 6d70 6c65  rain_dict(sample
+00008090: 7328 292c 2031 3030 2a31 3032 3429 0a0a  s(), 100*1024)..
+000080a0: 2e2e 2070 793a 6675 6e63 7469 6f6e 3a3a  .. py:function::
+000080b0: 2066 696e 616c 697a 655f 6469 6374 287a   finalize_dict(z
+000080c0: 7374 645f 6469 6374 2c20 7361 6d70 6c65  std_dict, sample
+000080d0: 732c 2064 6963 745f 7369 7a65 2c20 6c65  s, dict_size, le
+000080e0: 7665 6c29 0a0a 2020 2020 4769 7665 6e20  vel)..    Given 
+000080f0: 6120 6375 7374 6f6d 2063 6f6e 7465 6e74  a custom content
+00008100: 2061 7320 6120 6261 7369 7320 666f 7220   as a basis for 
+00008110: 6469 6374 696f 6e61 7279 2c20 616e 6420  dictionary, and 
+00008120: 6120 7365 7420 6f66 2073 616d 706c 6573  a set of samples
+00008130: 2c20 6669 6e61 6c69 7a65 2064 6963 7469  , finalize dicti
+00008140: 6f6e 6172 7920 6279 2061 6464 696e 6720  onary by adding 
+00008150: 6865 6164 6572 7320 616e 6420 7374 6174  headers and stat
+00008160: 6973 7469 6373 2061 6363 6f72 6469 6e67  istics according
+00008170: 2074 6f20 7468 6520 7a73 7464 2064 6963   to the zstd dic
+00008180: 7469 6f6e 6172 7920 666f 726d 6174 2e0a  tionary format..
+00008190: 0a20 2020 2053 6565 2074 6865 2046 4151  .    See the FAQ
+000081a0: 2069 6e20 6074 6869 7320 6669 6c65 203c   in `this file <
+000081b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000081c0: 6f6d 2f66 6163 6562 6f6f 6b2f 7a73 7464  om/facebook/zstd
+000081d0: 2f62 6c6f 622f 7265 6c65 6173 652f 6c69  /blob/release/li
+000081e0: 622f 7a64 6963 742e 683e 605f 2066 6f72  b/zdict.h>`_ for
+000081f0: 2064 6574 6169 6c73 2e0a 0a20 2020 203a   details...    :
+00008200: 7061 7261 6d20 7a73 7464 5f64 6963 743a  param zstd_dict:
+00008210: 2041 2062 6173 6973 2064 6963 7469 6f6e   A basis diction
+00008220: 6172 792e 0a20 2020 203a 7479 7065 207a  ary..    :type z
+00008230: 7374 645f 6469 6374 3a20 5a73 7464 4469  std_dict: ZstdDi
+00008240: 6374 0a20 2020 203a 7061 7261 6d20 7361  ct.    :param sa
+00008250: 6d70 6c65 733a 2041 6e20 6974 6572 6162  mples: An iterab
+00008260: 6c65 206f 6620 7361 6d70 6c65 732c 2061  le of samples, a
+00008270: 2073 616d 706c 6520 6973 2061 2062 7974   sample is a byt
+00008280: 6573 2d6c 696b 6520 6f62 6a65 6374 2072  es-like object r
+00008290: 6570 7265 7365 6e74 7320 6120 6669 6c65  epresents a file
+000082a0: 2e0a 2020 2020 3a74 7970 6520 7361 6d70  ..    :type samp
+000082b0: 6c65 733a 2069 7465 7261 626c 650a 2020  les: iterable.  
+000082c0: 2020 3a70 6172 616d 2069 6e74 2064 6963    :param int dic
+000082d0: 745f 7369 7a65 3a20 5265 7475 726e 6564  t_size: Returned
+000082e0: 207a 7374 6420 6469 6374 696f 6e61 7279   zstd dictionary
+000082f0: 2773 202a 2a6d 6178 696d 756d 2a2a 2073  's **maximum** s
+00008300: 697a 652c 2069 6e20 6279 7465 732e 0a20  ize, in bytes.. 
+00008310: 2020 203a 7061 7261 6d20 696e 7420 6c65     :param int le
+00008320: 7665 6c3a 2054 6865 2063 6f6d 7072 6573  vel: The compres
+00008330: 7369 6f6e 206c 6576 656c 2065 7870 6563  sion level expec
+00008340: 7465 6420 746f 2075 7365 2069 6e20 7072  ted to use in pr
+00008350: 6f64 7563 7469 6f6e 2e20 5468 6520 7374  oduction. The st
+00008360: 6174 6973 7469 6373 2066 6f72 2065 6163  atistics for eac
+00008370: 6820 636f 6d70 7265 7373 696f 6e20 6c65  h compression le
+00008380: 7665 6c20 6469 6666 6572 2c20 736f 2074  vel differ, so t
+00008390: 756e 696e 6720 7468 6520 6469 6374 696f  uning the dictio
+000083a0: 6e61 7279 2066 6f72 2074 6865 2063 6f6d  nary for the com
+000083b0: 7072 6573 7369 6f6e 206c 6576 656c 2063  pression level c
+000083c0: 616e 2068 656c 7020 7175 6974 6520 6120  an help quite a 
+000083d0: 6269 742e 0a20 2020 203a 7265 7475 726e  bit..    :return
+000083e0: 3a20 4669 6e61 6c69 7a65 6420 7a73 7464  : Finalized zstd
+000083f0: 2064 6963 7469 6f6e 6172 792e 2049 6620   dictionary. If 
+00008400: 7761 6e74 2074 6f20 7361 7665 2074 6865  want to save the
+00008410: 2064 6963 7469 6f6e 6172 7920 746f 2061   dictionary to a
+00008420: 2066 696c 652c 2073 6176 6520 7468 6520   file, save the 
+00008430: 3a70 793a 6174 7472 3a60 5a73 7464 4469  :py:attr:`ZstdDi
+00008440: 6374 2e64 6963 745f 636f 6e74 656e 7460  ct.dict_content`
+00008450: 2061 7474 7269 6275 7465 2e0a 2020 2020   attribute..    
+00008460: 3a72 7479 7065 3a20 5a73 7464 4469 6374  :rtype: ZstdDict
+00008470: 0a0a 0a4d 6f64 756c 652d 6c65 7665 6c20  ...Module-level 
+00008480: 6675 6e63 7469 6f6e 730a 2d2d 2d2d 2d2d  functions.------
+00008490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000084a0: 0a0a 2020 2020 5468 6973 2073 6563 7469  ..    This secti
+000084b0: 6f6e 2063 6f6e 7461 696e 733a 0a0a 2020  on contains:..  
+000084c0: 2020 2020 2020 2a20 6675 6e63 7469 6f6e        * function
+000084d0: 203a 7079 3a66 756e 633a 6067 6574 5f66   :py:func:`get_f
+000084e0: 7261 6d65 5f69 6e66 6f60 2c20 6765 7420  rame_info`, get 
+000084f0: 6672 616d 6520 696e 666f 726d 6174 696f  frame informatio
+00008500: 6e20 6672 6f6d 2061 2066 7261 6d65 2068  n from a frame h
+00008510: 6561 6465 722e 0a20 2020 2020 2020 202a  eader..        *
+00008520: 2066 756e 6374 696f 6e20 3a70 793a 6675   function :py:fu
+00008530: 6e63 3a60 6765 745f 6672 616d 655f 7369  nc:`get_frame_si
+00008540: 7a65 602c 2067 6574 2061 2066 7261 6d65  ze`, get a frame
+00008550: 2773 2073 697a 652e 0a0a 2e2e 2070 793a  's size..... py:
+00008560: 6675 6e63 7469 6f6e 3a3a 2067 6574 5f66  function:: get_f
+00008570: 7261 6d65 5f69 6e66 6f28 6672 616d 655f  rame_info(frame_
+00008580: 6275 6666 6572 290a 0a20 2020 2047 6574  buffer)..    Get
+00008590: 207a 7374 6420 6672 616d 6520 696e 666f   zstd frame info
+000085a0: 726d 6174 696f 6e20 6672 6f6d 2061 2066  rmation from a f
+000085b0: 7261 6d65 2068 6561 6465 722e 0a0a 2020  rame header...  
+000085c0: 2020 5265 7475 726e 2061 2032 2d69 7465    Return a 2-ite
+000085d0: 6d20 6e61 6d65 6474 7570 6c65 3a20 2864  m namedtuple: (d
+000085e0: 6563 6f6d 7072 6573 7365 645f 7369 7a65  ecompressed_size
+000085f0: 2c20 6469 6374 696f 6e61 7279 5f69 6429  , dictionary_id)
+00008600: 0a0a 2020 2020 4966 2060 6064 6563 6f6d  ..    If ``decom
+00008610: 7072 6573 7365 645f 7369 7a65 6060 2069  pressed_size`` i
+00008620: 7320 6060 4e6f 6e65 6060 2c20 6465 636f  s ``None``, deco
+00008630: 6d70 7265 7373 6564 2073 697a 6520 6973  mpressed size is
+00008640: 2075 6e6b 6e6f 776e 2e0a 0a20 2020 2060   unknown...    `
+00008650: 6064 6963 7469 6f6e 6172 795f 6964 6060  `dictionary_id``
+00008660: 2069 7320 6120 3332 2d62 6974 2075 6e73   is a 32-bit uns
+00008670: 6967 6e65 6420 696e 7465 6765 7220 7661  igned integer va
+00008680: 6c75 652e 2060 6030 6060 206d 6561 6e73  lue. ``0`` means
+00008690: 2064 6963 7469 6f6e 6172 7920 4944 2077   dictionary ID w
+000086a0: 6173 206e 6f74 2072 6563 6f72 6465 6420  as not recorded 
+000086b0: 696e 2066 7261 6d65 2068 6561 6465 722c  in frame header,
+000086c0: 2074 6865 2066 7261 6d65 206d 6179 206f   the frame may o
+000086d0: 7220 6d61 7920 6e6f 7420 6e65 6564 2061  r may not need a
+000086e0: 2064 6963 7469 6f6e 6172 7920 746f 2062   dictionary to b
+000086f0: 6520 6465 636f 6465 642c 2061 6e64 2074  e decoded, and t
+00008700: 6865 2049 4420 6f66 2073 7563 6820 6120  he ID of such a 
+00008710: 6469 6374 696f 6e61 7279 2069 7320 6e6f  dictionary is no
+00008720: 7420 7370 6563 6966 6965 642e 2028 4e6f  t specified. (No
+00008730: 7465 2074 6861 7420 7468 6520 6d65 616e  te that the mean
+00008740: 696e 6720 6f66 2060 6030 6060 2069 7320  ing of ``0`` is 
+00008750: 6469 6666 6572 656e 7420 6672 6f6d 203a  different from :
+00008760: 7079 3a61 7474 723a 605a 7374 6444 6963  py:attr:`ZstdDic
+00008770: 742e 6469 6374 5f69 6460 2061 7474 7269  t.dict_id` attri
+00008780: 6275 7465 2e29 0a0a 2020 2020 4974 2773  bute.)..    It's
+00008790: 2070 6f73 7369 626c 6520 746f 2061 7070   possible to app
+000087a0: 656e 6420 6d6f 7265 2069 7465 6d73 2074  end more items t
+000087b0: 6f20 7468 6520 6e61 6d65 6474 7570 6c65  o the namedtuple
+000087c0: 2069 6e20 7468 6520 6675 7475 7265 2e0a   in the future..
+000087d0: 0a20 2020 203a 7061 7261 6d20 6672 616d  .    :param fram
+000087e0: 655f 6275 6666 6572 3a20 4974 2073 686f  e_buffer: It sho
+000087f0: 756c 6420 7374 6172 7473 2066 726f 6d20  uld starts from 
+00008800: 7468 6520 6265 6769 6e6e 696e 6720 6f66  the beginning of
+00008810: 2061 2066 7261 6d65 2c20 616e 6420 636f   a frame, and co
+00008820: 6e74 6169 6e73 2061 7420 6c65 6173 7420  ntains at least 
+00008830: 7468 6520 6672 616d 6520 6865 6164 6572  the frame header
+00008840: 2028 3620 746f 2031 3820 6279 7465 7329   (6 to 18 bytes)
+00008850: 2e0a 2020 2020 3a74 7970 6520 6672 616d  ..    :type fram
+00008860: 655f 6275 6666 6572 3a20 6279 7465 732d  e_buffer: bytes-
+00008870: 6c69 6b65 206f 626a 6563 740a 2020 2020  like object.    
+00008880: 3a72 6574 7572 6e3a 2049 6e66 6f72 6d61  :return: Informa
+00008890: 7469 6f6e 2061 626f 7574 2061 2066 7261  tion about a fra
+000088a0: 6d65 2e0a 2020 2020 3a72 7479 7065 3a20  me..    :rtype: 
+000088b0: 6e61 6d65 6474 7570 6c65 0a20 2020 203a  namedtuple.    :
+000088c0: 7261 6973 6573 205a 7374 6445 7272 6f72  raises ZstdError
+000088d0: 3a20 5768 656e 2070 6172 7369 6e67 2074  : When parsing t
+000088e0: 6865 2066 7261 6d65 2068 6561 6465 7220  he frame header 
+000088f0: 6661 696c 732e 0a0a 2e2e 2073 6f75 7263  fails..... sourc
+00008900: 6563 6f64 653a 3a20 7079 7468 6f6e 0a0a  ecode:: python..
+00008910: 2020 2020 3e3e 3e20 7079 7a73 7464 2e67      >>> pyzstd.g
+00008920: 6574 5f66 7261 6d65 5f69 6e66 6f28 636f  et_frame_info(co
+00008930: 6d70 7265 7373 6564 5f64 6174 5b3a 3230  mpressed_dat[:20
+00008940: 5d29 0a20 2020 2066 7261 6d65 5f69 6e66  ]).    frame_inf
+00008950: 6f28 6465 636f 6d70 7265 7373 6564 5f73  o(decompressed_s
+00008960: 697a 653d 3638 3733 3739 2c20 6469 6374  ize=687379, dict
+00008970: 696f 6e61 7279 5f69 643d 3130 3430 3939  ionary_id=104099
+00008980: 3232 3638 290a 0a0a 2e2e 2070 793a 6675  2268)..... py:fu
+00008990: 6e63 7469 6f6e 3a3a 2067 6574 5f66 7261  nction:: get_fra
+000089a0: 6d65 5f73 697a 6528 6672 616d 655f 6275  me_size(frame_bu
+000089b0: 6666 6572 290a 0a20 2020 2047 6574 2074  ffer)..    Get t
+000089c0: 6865 2073 697a 6520 6f66 2061 207a 7374  he size of a zst
+000089d0: 6420 6672 616d 652c 2069 6e63 6c75 6469  d frame, includi
+000089e0: 6e67 2066 7261 6d65 2068 6561 6465 7220  ng frame header 
+000089f0: 616e 6420 342d 6279 7465 2063 6865 636b  and 4-byte check
+00008a00: 7375 6d20 6966 2069 7420 6861 732e 0a0a  sum if it has...
+00008a10: 2020 2020 4974 2077 696c 6c20 6974 6572      It will iter
+00008a20: 6174 6520 616c 6c20 626c 6f63 6b73 2720  ate all blocks' 
+00008a30: 6865 6164 6572 2077 6974 6869 6e20 6120  header within a 
+00008a40: 6672 616d 652c 2074 6f20 6163 6375 6d75  frame, to accumu
+00008a50: 6c61 7465 2074 6865 2066 7261 6d65 2773  late the frame's
+00008a60: 2073 697a 652e 0a0a 2020 2020 3a70 6172   size...    :par
+00008a70: 616d 2066 7261 6d65 5f62 7566 6665 723a  am frame_buffer:
+00008a80: 2049 7420 7368 6f75 6c64 2073 7461 7274   It should start
+00008a90: 7320 6672 6f6d 2074 6865 2062 6567 696e  s from the begin
+00008aa0: 6e69 6e67 206f 6620 6120 6672 616d 652c  ning of a frame,
+00008ab0: 2061 6e64 2063 6f6e 7461 696e 7320 6174   and contains at
+00008ac0: 206c 6561 7374 206f 6e65 2063 6f6d 706c   least one compl
+00008ad0: 6574 6520 6672 616d 652e 0a20 2020 203a  ete frame..    :
+00008ae0: 7479 7065 2066 7261 6d65 5f62 7566 6665  type frame_buffe
+00008af0: 723a 2062 7974 6573 2d6c 696b 6520 6f62  r: bytes-like ob
+00008b00: 6a65 6374 0a20 2020 203a 7265 7475 726e  ject.    :return
+00008b10: 3a20 5468 6520 7369 7a65 206f 6620 6120  : The size of a 
+00008b20: 7a73 7464 2066 7261 6d65 2e0a 2020 2020  zstd frame..    
+00008b30: 3a72 7479 7065 3a20 696e 740a 2020 2020  :rtype: int.    
+00008b40: 3a72 6169 7365 7320 5a73 7464 4572 726f  :raises ZstdErro
+00008b50: 723a 2057 6865 6e20 6974 2066 6169 6c73  r: When it fails
+00008b60: 2e0a 0a2e 2e20 736f 7572 6365 636f 6465  ..... sourcecode
+00008b70: 3a3a 2070 7974 686f 6e0a 0a20 2020 203e  :: python..    >
+00008b80: 3e3e 2070 797a 7374 642e 6765 745f 6672  >> pyzstd.get_fr
+00008b90: 616d 655f 7369 7a65 2863 6f6d 7072 6573  ame_size(compres
+00008ba0: 7365 645f 6461 7429 0a20 2020 2032 3532  sed_dat).    252
+00008bb0: 3837 340a 0a0a 4d6f 6475 6c65 2d6c 6576  874...Module-lev
+00008bc0: 656c 2076 6172 6961 626c 6573 0a2d 2d2d  el variables.---
+00008bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008be0: 2d2d 2d0a 0a20 2020 2054 6869 7320 7365  ---..    This se
+00008bf0: 6374 696f 6e20 636f 6e74 6169 6e73 3a0a  ction contains:.
+00008c00: 0a20 2020 2020 2020 202a 203a 7079 3a64  .        * :py:d
+00008c10: 6174 613a 607a 7374 645f 7665 7273 696f  ata:`zstd_versio
+00008c20: 6e60 2c20 6120 6060 7374 7260 602e 0a20  n`, a ``str``.. 
+00008c30: 2020 2020 2020 202a 203a 7079 3a64 6174         * :py:dat
+00008c40: 613a 607a 7374 645f 7665 7273 696f 6e5f  a:`zstd_version_
+00008c50: 696e 666f 602c 2061 2060 6074 7570 6c65  info`, a ``tuple
+00008c60: 6060 2e0a 2020 2020 2020 2020 2a20 3a70  ``..        * :p
+00008c70: 793a 6461 7461 3a60 636f 6d70 7265 7373  y:data:`compress
+00008c80: 696f 6e4c 6576 656c 5f76 616c 7565 7360  ionLevel_values`
+00008c90: 2c20 736f 6d65 2076 616c 7565 7320 6465  , some values de
+00008ca0: 6669 6e65 6420 6279 2074 6865 2075 6e64  fined by the und
+00008cb0: 6572 6c79 696e 6720 7a73 7464 206c 6962  erlying zstd lib
+00008cc0: 7261 7279 2e0a 2020 2020 2020 2020 2a20  rary..        * 
+00008cd0: 3a70 793a 6461 7461 3a60 7a73 7464 5f73  :py:data:`zstd_s
+00008ce0: 7570 706f 7274 5f6d 756c 7469 7468 7265  upport_multithre
+00008cf0: 6164 602c 2077 6865 7468 6572 2074 6865  ad`, whether the
+00008d00: 2075 6e64 6572 6c79 696e 6720 7a73 7464   underlying zstd
+00008d10: 206c 6962 7261 7279 2073 7570 706f 7274   library support
+00008d20: 7320 6d75 6c74 692d 7468 7265 6164 6564  s multi-threaded
+00008d30: 2063 6f6d 7072 6573 7369 6f6e 2e0a 0a2e   compression....
+00008d40: 2e20 7079 3a64 6174 613a 3a20 7a73 7464  . py:data:: zstd
+00008d50: 5f76 6572 7369 6f6e 0a0a 2020 2020 556e  _version..    Un
+00008d60: 6465 726c 7969 6e67 207a 7374 6420 6c69  derlying zstd li
+00008d70: 6272 6172 7927 7320 7665 7273 696f 6e2c  brary's version,
+00008d80: 2060 6073 7472 6060 2066 6f72 6d2e 0a0a   ``str`` form...
+00008d90: 2e2e 2073 6f75 7263 6563 6f64 653a 3a20  .. sourcecode:: 
+00008da0: 7079 7468 6f6e 0a0a 2020 2020 3e3e 3e20  python..    >>> 
+00008db0: 7079 7a73 7464 2e7a 7374 645f 7665 7273  pyzstd.zstd_vers
+00008dc0: 696f 6e0a 2020 2020 2731 2e34 2e35 270a  ion.    '1.4.5'.
+00008dd0: 0a0a 2e2e 2070 793a 6461 7461 3a3a 207a  .... py:data:: z
+00008de0: 7374 645f 7665 7273 696f 6e5f 696e 666f  std_version_info
+00008df0: 0a0a 2020 2020 556e 6465 726c 7969 6e67  ..    Underlying
+00008e00: 207a 7374 6420 6c69 6272 6172 7927 7320   zstd library's 
+00008e10: 7665 7273 696f 6e2c 2060 6074 7570 6c65  version, ``tuple
+00008e20: 6060 2066 6f72 6d2e 0a0a 2e2e 2073 6f75  `` form..... sou
+00008e30: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
+00008e40: 0a0a 2020 2020 3e3e 3e20 7079 7a73 7464  ..    >>> pyzstd
+00008e50: 2e7a 7374 645f 7665 7273 696f 6e5f 696e  .zstd_version_in
+00008e60: 666f 0a20 2020 2028 312c 2034 2c20 3529  fo.    (1, 4, 5)
+00008e70: 0a0a 0a2e 2e20 7079 3a64 6174 613a 3a20  ..... py:data:: 
+00008e80: 636f 6d70 7265 7373 696f 6e4c 6576 656c  compressionLevel
+00008e90: 5f76 616c 7565 730a 0a20 2020 2041 2033  _values..    A 3
+00008ea0: 2d69 7465 6d20 6e61 6d65 6474 7570 6c65  -item namedtuple
+00008eb0: 2c20 7661 6c75 6573 2064 6566 696e 6564  , values defined
+00008ec0: 2062 7920 7468 6520 756e 6465 726c 7969   by the underlyi
+00008ed0: 6e67 207a 7374 6420 6c69 6272 6172 792c  ng zstd library,
+00008ee0: 2073 6565 203a 7265 663a 6063 6f6d 7072   see :ref:`compr
+00008ef0: 6573 7369 6f6e 206c 6576 656c 3c63 6f6d  ession level<com
+00008f00: 7072 6573 7369 6f6e 5f6c 6576 656c 3e60  pression_level>`
+00008f10: 2066 6f72 2064 6574 6169 6c73 2e0a 0a20   for details... 
+00008f20: 2020 2060 6064 6566 6175 6c74 6060 2069     ``default`` i
+00008f30: 7320 6465 6661 756c 7420 636f 6d70 7265  s default compre
+00008f40: 7373 696f 6e20 6c65 7665 6c2c 2069 7420  ssion level, it 
+00008f50: 6973 2075 7365 6420 7768 656e 2063 6f6d  is used when com
+00008f60: 7072 6573 7369 6f6e 206c 6576 656c 2069  pression level i
+00008f70: 7320 7365 7420 746f 2060 6030 6060 206f  s set to ``0`` o
+00008f80: 7220 6e6f 7420 7365 742e 0a0a 2020 2020  r not set...    
+00008f90: 6060 6d69 6e60 602f 6060 6d61 7860 6020  ``min``/``max`` 
+00008fa0: 6172 6520 6d69 6e69 6d75 6d2f 6d61 7869  are minimum/maxi
+00008fb0: 6d75 6d20 6176 6169 6c61 626c 6520 7661  mum available va
+00008fc0: 6c75 6573 206f 6620 636f 6d70 7265 7373  lues of compress
+00008fd0: 696f 6e20 6c65 7665 6c2c 2062 6f74 6820  ion level, both 
+00008fe0: 696e 636c 7573 6976 652e 0a0a 2e2e 2073  inclusive..... s
+00008ff0: 6f75 7263 6563 6f64 653a 3a20 7079 7468  ourcecode:: pyth
+00009000: 6f6e 0a0a 2020 2020 3e3e 3e20 7079 7a73  on..    >>> pyzs
+00009010: 7464 2e63 6f6d 7072 6573 7369 6f6e 4c65  td.compressionLe
+00009020: 7665 6c5f 7661 6c75 6573 2020 2320 3133  vel_values  # 13
+00009030: 3130 3732 203d 2031 3238 2a31 3032 340a  1072 = 128*1024.
+00009040: 2020 2020 7661 6c75 6573 2864 6566 6175      values(defau
+00009050: 6c74 3d33 2c20 6d69 6e3d 2d31 3331 3037  lt=3, min=-13107
+00009060: 322c 206d 6178 3d32 3229 0a0a 0a2e 2e20  2, max=22)..... 
+00009070: 7079 3a64 6174 613a 3a20 7a73 7464 5f73  py:data:: zstd_s
+00009080: 7570 706f 7274 5f6d 756c 7469 7468 7265  upport_multithre
+00009090: 6164 0a0a 2020 2020 5768 6574 6865 7220  ad..    Whether 
+000090a0: 7468 6520 756e 6465 726c 7969 6e67 207a  the underlying z
+000090b0: 7374 6420 6c69 6272 6172 7920 7761 7320  std library was 
+000090c0: 636f 6d70 696c 6564 2077 6974 6820 3a72  compiled with :r
+000090d0: 6566 3a60 6d75 6c74 692d 7468 7265 6164  ef:`multi-thread
+000090e0: 6564 2063 6f6d 7072 6573 7369 6f6e 3c6d  ed compression<m
+000090f0: 745f 636f 6d70 7265 7373 696f 6e3e 6020  t_compression>` 
+00009100: 7375 7070 6f72 742e 0a0a 2020 2020 4974  support...    It
+00009110: 2773 2061 6c6d 6f73 7420 616c 7761 7973  's almost always
+00009120: 2060 6054 7275 6560 602e 0a0a 2020 2020   ``True``...    
+00009130: 4974 2773 2060 6046 616c 7365 6060 2077  It's ``False`` w
+00009140: 6865 6e20 6479 6e61 6d69 6361 6c6c 7920  hen dynamically 
+00009150: 6c69 6e6b 6564 2074 6f20 7a73 7464 206c  linked to zstd l
+00009160: 6962 7261 7279 2074 6861 7420 636f 6d70  ibrary that comp
+00009170: 696c 6564 2077 6974 686f 7574 206d 756c  iled without mul
+00009180: 7469 2d74 6872 6561 6465 6420 7375 7070  ti-threaded supp
+00009190: 6f72 742e 204f 7264 696e 6172 7920 7573  ort. Ordinary us
+000091a0: 6572 7320 7769 6c6c 206e 6f74 206d 6565  ers will not mee
+000091b0: 7420 7468 6973 2073 6974 7561 7469 6f6e  t this situation
+000091c0: 2e0a 0a2e 2e20 7665 7273 696f 6e61 6464  ..... versionadd
+000091d0: 6564 3a3a 2030 2e31 352e 310a 0a2e 2e20  ed:: 0.15.1.... 
+000091e0: 736f 7572 6365 636f 6465 3a3a 2070 7974  sourcecode:: pyt
+000091f0: 686f 6e0a 0a20 2020 203e 3e3e 2070 797a  hon..    >>> pyz
+00009200: 7374 642e 7a73 7464 5f73 7570 706f 7274  std.zstd_support
+00009210: 5f6d 756c 7469 7468 7265 6164 0a20 2020  _multithread.   
+00009220: 2054 7275 650a 0a0a 5a73 7464 4669 6c65   True...ZstdFile
+00009230: 2063 6c61 7373 2061 6e64 206f 7065 6e28   class and open(
+00009240: 2920 6675 6e63 7469 6f6e 0a2d 2d2d 2d2d  ) function.-----
+00009250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20  -------------.. 
+00009270: 2020 2054 6869 7320 7365 6374 696f 6e20     This section 
+00009280: 636f 6e74 6169 6e73 3a0a 0a20 2020 2020  contains:..     
+00009290: 2020 202a 2063 6c61 7373 203a 7079 3a63     * class :py:c
+000092a0: 6c61 7373 3a60 5a73 7464 4669 6c65 602c  lass:`ZstdFile`,
+000092b0: 206f 7065 6e20 6120 7a73 7464 2d63 6f6d   open a zstd-com
+000092c0: 7072 6573 7365 6420 6669 6c65 2069 6e20  pressed file in 
+000092d0: 6269 6e61 7279 206d 6f64 652e 0a20 2020  binary mode..   
+000092e0: 2020 2020 202a 2066 756e 6374 696f 6e20       * function 
+000092f0: 3a70 793a 6675 6e63 3a60 6f70 656e 602c  :py:func:`open`,
+00009300: 206f 7065 6e20 6120 7a73 7464 2d63 6f6d   open a zstd-com
+00009310: 7072 6573 7365 6420 6669 6c65 2069 6e20  pressed file in 
+00009320: 6269 6e61 7279 206f 7220 7465 7874 206d  binary or text m
+00009330: 6f64 652e 0a0a 2e2e 2070 793a 636c 6173  ode..... py:clas
+00009340: 733a 3a20 5a73 7464 4669 6c65 0a0a 2020  s:: ZstdFile..  
+00009350: 2020 4f70 656e 2061 207a 7374 642d 636f    Open a zstd-co
+00009360: 6d70 7265 7373 6564 2066 696c 6520 696e  mpressed file in
+00009370: 2062 696e 6172 7920 6d6f 6465 2e0a 0a20   binary mode... 
+00009380: 2020 2054 6869 7320 636c 6173 7320 6973     This class is
+00009390: 2076 6572 7920 7369 6d69 6c61 7220 746f   very similar to
+000093a0: 2060 627a 322e 425a 3246 696c 6520 3c68   `bz2.BZ2File <h
+000093b0: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
+000093c0: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
+000093d0: 2f62 7a32 2e68 746d 6c23 627a 322e 425a  /bz2.html#bz2.BZ
+000093e0: 3246 696c 653e 605f 202f 2020 6067 7a69  2File>`_ /  `gzi
+000093f0: 702e 477a 6970 4669 6c65 203c 6874 7470  p.GzipFile <http
+00009400: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+00009410: 6f72 672f 332f 6c69 6272 6172 792f 677a  org/3/library/gz
+00009420: 6970 2e68 746d 6c23 677a 6970 2e47 7a69  ip.html#gzip.Gzi
+00009430: 7046 696c 653e 605f 202f 2060 6c7a 6d61  pFile>`_ / `lzma
+00009440: 2e4c 5a4d 4146 696c 6520 3c68 7474 7073  .LZMAFile <https
+00009450: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00009460: 7267 2f33 2f6c 6962 7261 7279 2f6c 7a6d  rg/3/library/lzm
+00009470: 612e 6874 6d6c 236c 7a6d 612e 4c5a 4d41  a.html#lzma.LZMA
+00009480: 4669 6c65 3e60 5f20 636c 6173 7365 7320  File>`_ classes 
+00009490: 696e 2050 7974 686f 6e20 7374 616e 6461  in Python standa
+000094a0: 7264 206c 6962 7261 7279 2e20 4275 7420  rd library. But 
+000094b0: 7468 6520 7065 7266 6f72 6d61 6e63 6520  the performance 
+000094c0: 6973 206d 7563 6820 6265 7474 6572 2074  is much better t
+000094d0: 6861 6e20 7468 656d 2e0a 0a20 2020 204c  han them...    L
+000094e0: 696b 6520 425a 3246 696c 652f 477a 6970  ike BZ2File/Gzip
+000094f0: 4669 6c65 2f4c 5a4d 4146 696c 6520 636c  File/LZMAFile cl
+00009500: 6173 7365 732c 205a 7374 6446 696c 6520  asses, ZstdFile 
+00009510: 6973 206e 6f74 2074 6872 6561 642d 7361  is not thread-sa
+00009520: 6665 2c20 736f 2069 6620 796f 7520 6e65  fe, so if you ne
+00009530: 6564 2074 6f20 7573 6520 6120 7369 6e67  ed to use a sing
+00009540: 6c65 205a 7374 6446 696c 6520 6f62 6a65  le ZstdFile obje
+00009550: 6374 2066 726f 6d20 6d75 6c74 6970 6c65  ct from multiple
+00009560: 2074 6872 6561 6473 2c20 6974 2069 7320   threads, it is 
+00009570: 6e65 6365 7373 6172 7920 746f 2070 726f  necessary to pro
+00009580: 7465 6374 2069 7420 7769 7468 2061 206c  tect it with a l
+00009590: 6f63 6b2e 0a0a 2020 2020 4974 2063 616e  ock...    It can
+000095a0: 2062 6520 7573 6564 2077 6974 6820 5079   be used with Py
+000095b0: 7468 6f6e 2773 2060 6074 6172 6669 6c65  thon's ``tarfile
+000095c0: 6060 206d 6f64 756c 652c 2073 6565 203a  `` module, see :
+000095d0: 7265 663a 6074 6869 7320 6e6f 7465 3c77  ref:`this note<w
+000095e0: 6974 685f 7461 7266 696c 653e 602e 0a0a  ith_tarfile>`...
+000095f0: 2020 2020 2e2e 2070 793a 6d65 7468 6f64      .. py:method
+00009600: 3a3a 205f 5f69 6e69 745f 5f28 7365 6c66  :: __init__(self
+00009610: 2c20 6669 6c65 6e61 6d65 2c20 6d6f 6465  , filename, mode
+00009620: 3d22 7222 2c20 2a2c 206c 6576 656c 5f6f  ="r", *, level_o
+00009630: 725f 6f70 7469 6f6e 3d4e 6f6e 652c 207a  r_option=None, z
+00009640: 7374 645f 6469 6374 3d4e 6f6e 652c 2072  std_dict=None, r
+00009650: 6561 645f 7369 7a65 3d31 3331 5f30 3735  ead_size=131_075
+00009660: 2c20 7772 6974 655f 6275 6666 6572 5f73  , write_buffer_s
+00009670: 697a 653d 3133 315f 3539 3129 0a0a 2020  ize=131_591)..  
+00009680: 2020 2020 2020 5468 6520 2a66 696c 656e        The *filen
+00009690: 616d 652a 2061 7267 756d 656e 7420 6361  ame* argument ca
+000096a0: 6e20 6265 2061 6e20 6578 6973 7469 6e67  n be an existing
+000096b0: 2060 6669 6c65 206f 626a 6563 7420 3c68   `file object <h
+000096c0: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
+000096d0: 6f6e 2e6f 7267 2f33 2f67 6c6f 7373 6172  on.org/3/glossar
+000096e0: 792e 6874 6d6c 2374 6572 6d2d 6669 6c65  y.html#term-file
+000096f0: 2d6f 626a 6563 743e 605f 2074 6f20 7772  -object>`_ to wr
+00009700: 6170 2c20 6f72 2074 6865 206e 616d 6520  ap, or the name 
+00009710: 6f66 2074 6865 2066 696c 6520 746f 206f  of the file to o
+00009720: 7065 6e20 2861 7320 6120 6060 7374 7260  pen (as a ``str`
+00009730: 602c 2060 6062 7974 6573 6060 206f 7220  `, ``bytes`` or 
+00009740: 6070 6174 682d 6c69 6b65 203c 6874 7470  `path-like <http
+00009750: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+00009760: 6f72 672f 332f 676c 6f73 7361 7279 2e68  org/3/glossary.h
+00009770: 746d 6c23 7465 726d 2d70 6174 682d 6c69  tml#term-path-li
+00009780: 6b65 2d6f 626a 6563 743e 605f 206f 626a  ke-object>`_ obj
+00009790: 6563 7429 2e20 5768 656e 2077 7261 7070  ect). When wrapp
+000097a0: 696e 6720 616e 2065 7869 7374 696e 6720  ing an existing 
+000097b0: 6669 6c65 206f 626a 6563 742c 2074 6865  file object, the
+000097c0: 2077 7261 7070 6564 2066 696c 6520 7769   wrapped file wi
+000097d0: 6c6c 206e 6f74 2062 6520 636c 6f73 6564  ll not be closed
+000097e0: 2077 6865 6e20 7468 6520 5a73 7464 4669   when the ZstdFi
+000097f0: 6c65 2069 7320 636c 6f73 6564 2e0a 0a20  le is closed... 
+00009800: 2020 2020 2020 2054 6865 202a 6d6f 6465         The *mode
+00009810: 2a20 6172 6775 6d65 6e74 2063 616e 2062  * argument can b
+00009820: 6520 6569 7468 6572 2022 7222 2066 6f72  e either "r" for
+00009830: 2072 6561 6469 6e67 2028 6465 6661 756c   reading (defaul
+00009840: 7429 2c20 2277 2220 666f 7220 6f76 6572  t), "w" for over
+00009850: 7772 6974 696e 672c 2022 7822 2066 6f72  writing, "x" for
+00009860: 2065 7863 6c75 7369 7665 2063 7265 6174   exclusive creat
+00009870: 696f 6e2c 206f 7220 2261 2220 666f 7220  ion, or "a" for 
+00009880: 6170 7065 6e64 696e 672e 2054 6865 7365  appending. These
+00009890: 2063 616e 2065 7175 6976 616c 656e 746c   can equivalentl
+000098a0: 7920 6265 2067 6976 656e 2061 7320 2272  y be given as "r
+000098b0: 6222 2c20 2277 6222 2c20 2278 6222 2061  b", "wb", "xb" a
+000098c0: 6e64 2022 6162 2220 7265 7370 6563 7469  nd "ab" respecti
+000098d0: 7665 6c79 2e0a 0a20 2020 2020 2020 2049  vely...        I
+000098e0: 6e20 7265 6164 696e 6720 6d6f 6465 2028  n reading mode (
+000098f0: 6465 636f 6d70 7265 7373 696f 6e29 2c20  decompression), 
+00009900: 2a72 6561 645f 7369 7a65 2a20 6172 6775  *read_size* argu
+00009910: 6d65 6e74 2069 7320 6279 7465 7320 6e75  ment is bytes nu
+00009920: 6d62 6572 2074 6861 7420 7265 6164 2066  mber that read f
+00009930: 726f 6d20 7468 6520 756e 6465 726c 7969  rom the underlyi
+00009940: 6e67 2066 696c 6520 6f62 6a65 6374 2065  ng file object e
+00009950: 6163 6820 7469 6d65 2c20 6465 6661 756c  ach time, defaul
+00009960: 7420 7661 6c75 6520 6973 207a 7374 6427  t value is zstd'
+00009970: 7320 7265 636f 6d6d 656e 6465 6420 7661  s recommended va
+00009980: 6c75 652e 2049 6620 7573 6520 7769 7468  lue. If use with
+00009990: 204e 6574 776f 726b 2046 696c 6520 5379   Network File Sy
+000099a0: 7374 656d 2c20 696e 6372 6561 7369 6e67  stem, increasing
+000099b0: 2069 7420 6d61 7920 6765 7420 6265 7474   it may get bett
+000099c0: 6572 2070 6572 666f 726d 616e 6365 2e0a  er performance..
+000099d0: 0a20 2020 2020 2020 2049 6e20 7772 6974  .        In writ
+000099e0: 696e 6720 6d6f 6465 7320 2863 6f6d 7072  ing modes (compr
+000099f0: 6573 7369 6f6e 292c 202a 7772 6974 655f  ession), *write_
+00009a00: 6275 6666 6572 5f73 697a 652a 2061 7267  buffer_size* arg
+00009a10: 756d 656e 7420 6973 206f 7574 7075 7420  ument is output 
+00009a20: 6275 6666 6572 2773 2073 697a 652c 2064  buffer's size, d
+00009a30: 6566 6175 6c74 2076 616c 7565 2069 7320  efault value is 
+00009a40: 7a73 7464 2773 2072 6563 6f6d 6d65 6e64  zstd's recommend
+00009a50: 6564 2076 616c 7565 2e20 4966 2075 7365  ed value. If use
+00009a60: 2077 6974 6820 4e65 7477 6f72 6b20 4669   with Network Fi
+00009a70: 6c65 2053 7973 7465 6d2c 2069 6e63 7265  le System, incre
+00009a80: 6173 696e 6720 6974 206d 6179 2067 6574  asing it may get
+00009a90: 2062 6574 7465 7220 7065 7266 6f72 6d61   better performa
+00009aa0: 6e63 652e 0a0a 2020 2020 2e2e 2076 6572  nce...    .. ver
+00009ab0: 7369 6f6e 6368 616e 6765 643a 3a20 302e  sionchanged:: 0.
+00009ac0: 3135 2e38 0a20 2020 2020 2020 2041 6464  15.8.        Add
+00009ad0: 202a 7265 6164 5f73 697a 652a 2061 6e64   *read_size* and
+00009ae0: 202a 7772 6974 655f 6275 6666 6572 5f73   *write_buffer_s
+00009af0: 697a 652a 2061 7267 756d 656e 7473 2e0a  ize* arguments..
+00009b00: 0a20 2020 2049 6e20 7265 6164 696e 6720  .    In reading 
+00009b10: 6d6f 6465 2028 6465 636f 6d70 7265 7373  mode (decompress
+00009b20: 696f 6e29 2c20 7468 6573 6520 6d65 7468  ion), these meth
+00009b30: 6f64 7320 616e 6420 7374 6174 656d 656e  ods and statemen
+00009b40: 7420 6172 6520 6176 6169 6c61 626c 653a  t are available:
+00009b50: 0a0a 2020 2020 2020 2020 2a20 602e 7265  ..        * `.re
+00009b60: 6164 2873 697a 653d 2d31 2920 3c68 7474  ad(size=-1) <htt
+00009b70: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00009b80: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f69  .org/3/library/i
+00009b90: 6f2e 6874 6d6c 2369 6f2e 4275 6666 6572  o.html#io.Buffer
+00009ba0: 6564 5265 6164 6572 2e72 6561 643e 605f  edReader.read>`_
+00009bb0: 0a20 2020 2020 2020 202a 2060 2e72 6561  .        * `.rea
+00009bc0: 6431 2873 697a 653d 2d31 2920 3c68 7474  d1(size=-1) <htt
+00009bd0: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00009be0: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f69  .org/3/library/i
+00009bf0: 6f2e 6874 6d6c 2369 6f2e 4275 6666 6572  o.html#io.Buffer
+00009c00: 6564 5265 6164 6572 2e72 6561 6431 3e60  edReader.read1>`
+00009c10: 5f0a 2020 2020 2020 2020 2a20 602e 7265  _.        * `.re
+00009c20: 6164 696e 746f 2862 2920 3c68 7474 7073  adinto(b) <https
+00009c30: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00009c40: 7267 2f33 2f6c 6962 7261 7279 2f69 6f2e  rg/3/library/io.
+00009c50: 6874 6d6c 2369 6f2e 4275 6666 6572 6564  html#io.Buffered
+00009c60: 494f 4261 7365 2e72 6561 6469 6e74 6f3e  IOBase.readinto>
+00009c70: 605f 0a20 2020 2020 2020 202a 2060 2e72  `_.        * `.r
+00009c80: 6561 6469 6e74 6f31 2862 2920 3c68 7474  eadinto1(b) <htt
+00009c90: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00009ca0: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f69  .org/3/library/i
+00009cb0: 6f2e 6874 6d6c 2369 6f2e 4275 6666 6572  o.html#io.Buffer
+00009cc0: 6564 494f 4261 7365 2e72 6561 6469 6e74  edIOBase.readint
+00009cd0: 6f31 3e60 5f0a 2020 2020 2020 2020 2a20  o1>`_.        * 
+00009ce0: 602e 7265 6164 6c69 6e65 2873 697a 653d  `.readline(size=
+00009cf0: 2d31 2920 3c68 7474 7073 3a2f 2f64 6f63  -1) <https://doc
+00009d00: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+00009d10: 6962 7261 7279 2f69 6f2e 6874 6d6c 2369  ibrary/io.html#i
+00009d20: 6f2e 494f 4261 7365 2e72 6561 646c 696e  o.IOBase.readlin
+00009d30: 653e 605f 0a20 2020 2020 2020 202a 2060  e>`_.        * `
+00009d40: 2e73 6565 6b28 6f66 6673 6574 2c20 7768  .seek(offset, wh
+00009d50: 656e 6365 3d69 6f2e 5345 454b 5f53 4554  ence=io.SEEK_SET
+00009d60: 2920 3c68 7474 7073 3a2f 2f64 6f63 732e  ) <https://docs.
+00009d70: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+00009d80: 7261 7279 2f69 6f2e 6874 6d6c 2369 6f2e  rary/io.html#io.
+00009d90: 494f 4261 7365 2e73 6565 6b3e 605f 2c20  IOBase.seek>`_, 
+00009da0: 6e6f 7465 2074 6861 7420 6966 2073 6565  note that if see
+00009db0: 6b20 746f 2061 2070 6f73 6974 696f 6e20  k to a position 
+00009dc0: 6265 666f 7265 2074 6865 2063 7572 7265  before the curre
+00009dd0: 6e74 2070 6f73 6974 696f 6e2c 206f 7220  nt position, or 
+00009de0: 7365 656b 2074 6f20 6120 706f 7369 7469  seek to a positi
+00009df0: 6f6e 2072 656c 6174 6976 6520 746f 2074  on relative to t
+00009e00: 6865 2065 6e64 206f 6620 7468 6520 6669  he end of the fi
+00009e10: 6c65 2028 7468 6520 6669 7273 7420 7469  le (the first ti
+00009e20: 6d65 292c 2074 6865 2064 6563 6f6d 7072  me), the decompr
+00009e30: 6573 7369 6f6e 2068 6173 2074 6f20 6265  ession has to be
+00009e40: 2072 6573 7461 7274 6564 2066 726f 6d20   restarted from 
+00009e50: 7a65 726f 2e20 4966 2073 6565 6b2c 2063  zero. If seek, c
+00009e60: 6f6e 7369 6465 7220 7573 696e 6720 3a70  onsider using :p
+00009e70: 793a 636c 6173 733a 6053 6565 6b61 626c  y:class:`Seekabl
+00009e80: 655a 7374 6446 696c 6560 2063 6c61 7373  eZstdFile` class
+00009e90: 2e0a 2020 2020 2020 2020 2a20 602e 7065  ..        * `.pe
+00009ea0: 656b 2873 697a 653d 2d31 2920 3c68 7474  ek(size=-1) <htt
+00009eb0: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00009ec0: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f69  .org/3/library/i
+00009ed0: 6f2e 6874 6d6c 2369 6f2e 4275 6666 6572  o.html#io.Buffer
+00009ee0: 6564 5265 6164 6572 2e70 6565 6b3e 605f  edReader.peek>`_
+00009ef0: 0a20 2020 2020 2020 202a 2060 4974 6572  .        * `Iter
+00009f00: 6174 696f 6e20 3c68 7474 7073 3a2f 2f64  ation <https://d
+00009f10: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
+00009f20: 2f6c 6962 7261 7279 2f69 6f2e 6874 6d6c  /library/io.html
+00009f30: 2369 6f2e 494f 4261 7365 3e60 5f2c 2079  #io.IOBase>`_, y
+00009f40: 6965 6c64 206c 696e 6573 2c20 6c69 6e65  ield lines, line
+00009f50: 2074 6572 6d69 6e61 746f 7220 6973 2060   terminator is `
+00009f60: 6062 275c 6e27 6060 2e0a 0a20 2020 2049  `b'\n'``...    I
+00009f70: 6e20 7772 6974 696e 6720 6d6f 6465 7320  n writing modes 
+00009f80: 2863 6f6d 7072 6573 7369 6f6e 292c 2074  (compression), t
+00009f90: 6865 7365 206d 6574 686f 6473 2061 7265  hese methods are
+00009fa0: 2061 7661 696c 6162 6c65 3a0a 0a20 2020   available:..   
+00009fb0: 2020 2020 202a 2060 2e77 7269 7465 2862       * `.write(b
 00009fc0: 2920 3c68 7474 7073 3a2f 2f64 6f63 732e  ) <https://docs.
 00009fd0: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
 00009fe0: 7261 7279 2f69 6f2e 6874 6d6c 2369 6f2e  rary/io.html#io.
-00009ff0: 494f 4261 7365 2e74 656c 6c3e 605f 0a20  IOBase.tell>`_. 
-0000a000: 2020 2020 2020 202a 2060 2e66 696c 656e         * `.filen
-0000a010: 6f28 2920 3c68 7474 7073 3a2f 2f64 6f63  o() <https://doc
-0000a020: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-0000a030: 6962 7261 7279 2f69 6f2e 6874 6d6c 2369  ibrary/io.html#i
-0000a040: 6f2e 494f 4261 7365 2e66 696c 656e 6f3e  o.IOBase.fileno>
-0000a050: 605f 0a20 2020 2020 2020 202a 2060 2e63  `_.        * `.c
-0000a060: 6c6f 7365 6420 3c68 7474 7073 3a2f 2f64  losed <https://d
-0000a070: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
-0000a080: 2f6c 6962 7261 7279 2f69 6f2e 6874 6d6c  /library/io.html
-0000a090: 2369 6f2e 494f 4261 7365 2e63 6c6f 7365  #io.IOBase.close
-0000a0a0: 643e 605f 2028 6120 7072 6f70 6572 7479  d>`_ (a property
-0000a0b0: 2061 7474 7269 6275 7465 290a 2020 2020   attribute).    
-0000a0c0: 2020 2020 2a20 602e 7772 6974 6162 6c65      * `.writable
-0000a0d0: 2829 203c 6874 7470 733a 2f2f 646f 6373  () <https://docs
-0000a0e0: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-0000a0f0: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
-0000a100: 2e49 4f42 6173 652e 7772 6974 6162 6c65  .IOBase.writable
-0000a110: 3e60 5f0a 2020 2020 2020 2020 2a20 602e  >`_.        * `.
-0000a120: 7265 6164 6162 6c65 2829 203c 6874 7470  readable() <http
-0000a130: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-0000a140: 6f72 672f 332f 6c69 6272 6172 792f 696f  org/3/library/io
-0000a150: 2e68 746d 6c23 696f 2e49 4f42 6173 652e  .html#io.IOBase.
-0000a160: 7265 6164 6162 6c65 3e60 5f0a 2020 2020  readable>`_.    
-0000a170: 2020 2020 2a20 602e 7365 656b 6162 6c65      * `.seekable
-0000a180: 2829 203c 6874 7470 733a 2f2f 646f 6373  () <https://docs
-0000a190: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-0000a1a0: 6272 6172 792f 696f 2e68 746d 6c23 696f  brary/io.html#io
-0000a1b0: 2e49 4f42 6173 652e 7365 656b 6162 6c65  .IOBase.seekable
-0000a1c0: 3e60 5f0a 0a2e 2e20 7079 3a66 756e 6374  >`_.... py:funct
-0000a1d0: 696f 6e3a 3a20 6f70 656e 2866 696c 656e  ion:: open(filen
-0000a1e0: 616d 652c 206d 6f64 653d 2272 6222 2c20  ame, mode="rb", 
-0000a1f0: 2a2c 206c 6576 656c 5f6f 725f 6f70 7469  *, level_or_opti
-0000a200: 6f6e 3d4e 6f6e 652c 207a 7374 645f 6469  on=None, zstd_di
-0000a210: 6374 3d4e 6f6e 652c 2065 6e63 6f64 696e  ct=None, encodin
-0000a220: 673d 4e6f 6e65 2c20 6572 726f 7273 3d4e  g=None, errors=N
-0000a230: 6f6e 652c 206e 6577 6c69 6e65 3d4e 6f6e  one, newline=Non
-0000a240: 6529 0a0a 2020 2020 4f70 656e 2061 207a  e)..    Open a z
-0000a250: 7374 642d 636f 6d70 7265 7373 6564 2066  std-compressed f
-0000a260: 696c 6520 696e 2062 696e 6172 7920 6f72  ile in binary or
-0000a270: 2074 6578 7420 6d6f 6465 2c20 7265 7475   text mode, retu
-0000a280: 726e 696e 6720 6120 6669 6c65 206f 626a  rning a file obj
-0000a290: 6563 742e 0a0a 2020 2020 5468 6973 2066  ect...    This f
-0000a2a0: 756e 6374 696f 6e20 6973 2076 6572 7920  unction is very 
-0000a2b0: 7369 6d69 6c61 7220 746f 2060 627a 322e  similar to `bz2.
-0000a2c0: 6f70 656e 2829 203c 6874 7470 733a 2f2f  open() <https://
-0000a2d0: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-0000a2e0: 332f 6c69 6272 6172 792f 627a 322e 6874  3/library/bz2.ht
-0000a2f0: 6d6c 2362 7a32 2e6f 7065 6e3e 605f 202f  ml#bz2.open>`_ /
-0000a300: 2060 677a 6970 2e6f 7065 6e28 2920 3c68   `gzip.open() <h
-0000a310: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
-0000a320: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
-0000a330: 2f67 7a69 702e 6874 6d6c 2367 7a69 702e  /gzip.html#gzip.
-0000a340: 6f70 656e 3e60 5f20 2f20 606c 7a6d 612e  open>`_ / `lzma.
-0000a350: 6f70 656e 2829 203c 6874 7470 733a 2f2f  open() <https://
-0000a360: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-0000a370: 332f 6c69 6272 6172 792f 6c7a 6d61 2e68  3/library/lzma.h
-0000a380: 746d 6c23 6c7a 6d61 2e6f 7065 6e3e 605f  tml#lzma.open>`_
-0000a390: 2066 756e 6374 696f 6e73 2069 6e20 5079   functions in Py
-0000a3a0: 7468 6f6e 2073 7461 6e64 6172 6420 6c69  thon standard li
-0000a3b0: 6272 6172 792e 0a0a 2020 2020 5468 6520  brary...    The 
-0000a3c0: 2a66 696c 656e 616d 652a 2070 6172 616d  *filename* param
-0000a3d0: 6574 6572 2063 616e 2062 6520 616e 2065  eter can be an e
-0000a3e0: 7869 7374 696e 6720 6066 696c 6520 6f62  xisting `file ob
-0000a3f0: 6a65 6374 203c 6874 7470 733a 2f2f 646f  ject <https://do
-0000a400: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-0000a410: 676c 6f73 7361 7279 2e68 746d 6c23 7465  glossary.html#te
-0000a420: 726d 2d66 696c 652d 6f62 6a65 6374 3e60  rm-file-object>`
-0000a430: 5f20 746f 2077 7261 702c 206f 7220 7468  _ to wrap, or th
-0000a440: 6520 6e61 6d65 206f 6620 7468 6520 6669  e name of the fi
-0000a450: 6c65 2074 6f20 6f70 656e 2028 6173 2061  le to open (as a
-0000a460: 2060 6073 7472 6060 2c20 6060 6279 7465   ``str``, ``byte
-0000a470: 7360 6020 6f72 2060 7061 7468 2d6c 696b  s`` or `path-lik
-0000a480: 6520 3c68 7474 7073 3a2f 2f64 6f63 732e  e <https://docs.
-0000a490: 7079 7468 6f6e 2e6f 7267 2f33 2f67 6c6f  python.org/3/glo
-0000a4a0: 7373 6172 792e 6874 6d6c 2374 6572 6d2d  ssary.html#term-
-0000a4b0: 7061 7468 2d6c 696b 652d 6f62 6a65 6374  path-like-object
-0000a4c0: 3e60 5f20 6f62 6a65 6374 292e 2057 6865  >`_ object). Whe
-0000a4d0: 6e20 7772 6170 7069 6e67 2061 6e20 6578  n wrapping an ex
-0000a4e0: 6973 7469 6e67 2066 696c 6520 6f62 6a65  isting file obje
-0000a4f0: 6374 2c20 7468 6520 7772 6170 7065 6420  ct, the wrapped 
-0000a500: 6669 6c65 2077 696c 6c20 6e6f 7420 6265  file will not be
-0000a510: 2063 6c6f 7365 6420 7768 656e 2074 6865   closed when the
-0000a520: 2072 6574 7572 6e65 6420 6669 6c65 206f   returned file o
-0000a530: 626a 6563 7420 6973 2063 6c6f 7365 642e  bject is closed.
-0000a540: 0a0a 2020 2020 5468 6520 2a6d 6f64 652a  ..    The *mode*
-0000a550: 2070 6172 616d 6574 6572 2063 616e 2062   parameter can b
-0000a560: 6520 616e 7920 6f66 2022 7222 2c20 2272  e any of "r", "r
-0000a570: 6222 2c20 2277 222c 2022 7762 222c 2022  b", "w", "wb", "
-0000a580: 7822 2c20 2278 6222 2c20 2261 2220 6f72  x", "xb", "a" or
-0000a590: 2022 6162 2220 666f 7220 6269 6e61 7279   "ab" for binary
-0000a5a0: 206d 6f64 652c 206f 7220 2272 7422 2c20   mode, or "rt", 
-0000a5b0: 2277 7422 2c20 2278 7422 2c20 6f72 2022  "wt", "xt", or "
-0000a5c0: 6174 2220 666f 7220 7465 7874 206d 6f64  at" for text mod
-0000a5d0: 652e 2054 6865 2064 6566 6175 6c74 2069  e. The default i
-0000a5e0: 7320 2272 6222 2e0a 0a20 2020 2049 6620  s "rb"...    If 
-0000a5f0: 696e 2072 6561 6469 6e67 206d 6f64 6520  in reading mode 
-0000a600: 2864 6563 6f6d 7072 6573 7369 6f6e 292c  (decompression),
-0000a610: 2074 6865 202a 6c65 7665 6c5f 6f72 5f6f   the *level_or_o
-0000a620: 7074 696f 6e2a 2070 6172 616d 6574 6572  ption* parameter
-0000a630: 2063 616e 206f 6e6c 7920 6265 2061 2060   can only be a `
-0000a640: 6064 6963 7460 6020 6f62 6a65 6374 2c20  `dict`` object, 
-0000a650: 7468 6174 2072 6570 7265 7365 6e74 7320  that represents 
-0000a660: 6465 636f 6d70 7265 7373 696f 6e20 6f70  decompression op
-0000a670: 7469 6f6e 2e20 4974 2064 6f65 736e 2774  tion. It doesn't
-0000a680: 2073 7570 706f 7274 2060 6069 6e74 6060   support ``int``
-0000a690: 2074 7970 6520 636f 6d70 7265 7373 696f   type compressio
-0000a6a0: 6e20 6c65 7665 6c20 696e 2074 6869 7320  n level in this 
-0000a6b0: 6361 7365 2e0a 0a20 2020 2049 6e20 6269  case...    In bi
-0000a6c0: 6e61 7279 206d 6f64 652c 2061 203a 7079  nary mode, a :py
-0000a6d0: 3a63 6c61 7373 3a60 5a73 7464 4669 6c65  :class:`ZstdFile
-0000a6e0: 6020 6f62 6a65 6374 2069 7320 7265 7475  ` object is retu
-0000a6f0: 726e 6564 2e0a 0a20 2020 2049 6e20 7465  rned...    In te
-0000a700: 7874 206d 6f64 652c 2061 203a 7079 3a63  xt mode, a :py:c
-0000a710: 6c61 7373 3a60 5a73 7464 4669 6c65 6020  lass:`ZstdFile` 
-0000a720: 6f62 6a65 6374 2069 7320 6372 6561 7465  object is create
-0000a730: 642c 2061 6e64 2077 7261 7070 6564 2069  d, and wrapped i
-0000a740: 6e20 616e 2060 696f 2e54 6578 7449 4f57  n an `io.TextIOW
-0000a750: 7261 7070 6572 203c 6874 7470 733a 2f2f  rapper <https://
-0000a760: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-0000a770: 332f 6c69 6272 6172 792f 696f 2e68 746d  3/library/io.htm
-0000a780: 6c23 696f 2e54 6578 7449 4f57 7261 7070  l#io.TextIOWrapp
-0000a790: 6572 3e60 5f20 6f62 6a65 6374 2077 6974  er>`_ object wit
-0000a7a0: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
-0000a7b0: 656e 636f 6469 6e67 2c20 6572 726f 7220  encoding, error 
-0000a7c0: 6861 6e64 6c69 6e67 2062 6568 6176 696f  handling behavio
-0000a7d0: 722c 2061 6e64 206c 696e 6520 656e 6469  r, and line endi
-0000a7e0: 6e67 2873 292e 0a0a 4164 7661 6e63 6564  ng(s)...Advanced
-0000a7f0: 2070 6172 616d 6574 6572 730a 2d2d 2d2d   parameters.----
-0000a800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0000a810: 0a20 2020 2054 6869 7320 7365 6374 696f  .    This sectio
-0000a820: 6e20 636f 6e74 6169 6e73 2063 6c61 7373  n contains class
-0000a830: 203a 7079 3a63 6c61 7373 3a60 4350 6172   :py:class:`CPar
-0000a840: 616d 6574 6572 602c 203a 7079 3a63 6c61  ameter`, :py:cla
-0000a850: 7373 3a60 4450 6172 616d 6574 6572 602c  ss:`DParameter`,
-0000a860: 203a 7079 3a63 6c61 7373 3a60 5374 7261   :py:class:`Stra
-0000a870: 7465 6779 602c 2074 6865 7920 6172 6520  tegy`, they are 
-0000a880: 7375 6263 6c61 7373 6573 206f 6620 6060  subclasses of ``
-0000a890: 496e 7445 6e75 6d60 602c 2075 7365 6420  IntEnum``, used 
-0000a8a0: 666f 7220 7365 7474 696e 6720 6164 7661  for setting adva
-0000a8b0: 6e63 6564 2070 6172 616d 6574 6572 732e  nced parameters.
-0000a8c0: 0a0a 2020 2020 3a70 793a 636c 6173 733a  ..    :py:class:
-0000a8d0: 6043 5061 7261 6d65 7465 7260 2063 6c61  `CParameter` cla
-0000a8e0: 7373 2720 6174 7472 6962 7574 6573 3a0a  ss' attributes:.
-0000a8f0: 0a20 2020 2020 2020 202d 2043 6f6d 7072  .        - Compr
-0000a900: 6573 7369 6f6e 206c 6576 656c 2028 3a70  ession level (:p
-0000a910: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
-0000a920: 7465 722e 636f 6d70 7265 7373 696f 6e4c  ter.compressionL
-0000a930: 6576 656c 6029 0a20 2020 2020 2020 202d  evel`).        -
-0000a940: 2043 6f6d 7072 6573 7320 616c 676f 7269   Compress algori
-0000a950: 7468 6d20 7061 7261 6d65 7465 7273 2028  thm parameters (
-0000a960: 3a70 793a 6174 7472 3a60 7e43 5061 7261  :py:attr:`~CPara
-0000a970: 6d65 7465 722e 7769 6e64 6f77 4c6f 6760  meter.windowLog`
-0000a980: 2c20 3a70 793a 6174 7472 3a60 7e43 5061  , :py:attr:`~CPa
-0000a990: 7261 6d65 7465 722e 6861 7368 4c6f 6760  rameter.hashLog`
-0000a9a0: 2c20 3a70 793a 6174 7472 3a60 7e43 5061  , :py:attr:`~CPa
-0000a9b0: 7261 6d65 7465 722e 6368 6169 6e4c 6f67  rameter.chainLog
-0000a9c0: 602c 203a 7079 3a61 7474 723a 607e 4350  `, :py:attr:`~CP
-0000a9d0: 6172 616d 6574 6572 2e73 6561 7263 684c  arameter.searchL
-0000a9e0: 6f67 602c 203a 7079 3a61 7474 723a 607e  og`, :py:attr:`~
-0000a9f0: 4350 6172 616d 6574 6572 2e6d 696e 4d61  CParameter.minMa
-0000aa00: 7463 6860 2c20 3a70 793a 6174 7472 3a60  tch`, :py:attr:`
-0000aa10: 7e43 5061 7261 6d65 7465 722e 7461 7267  ~CParameter.targ
-0000aa20: 6574 4c65 6e67 7468 602c 203a 7079 3a61  etLength`, :py:a
-0000aa30: 7474 723a 607e 4350 6172 616d 6574 6572  ttr:`~CParameter
-0000aa40: 2e73 7472 6174 6567 7960 290a 2020 2020  .strategy`).    
-0000aa50: 2020 2020 2d20 4c6f 6e67 2064 6973 7461      - Long dista
-0000aa60: 6e63 6520 6d61 7463 6869 6e67 2028 3a70  nce matching (:p
-0000aa70: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
-0000aa80: 7465 722e 656e 6162 6c65 4c6f 6e67 4469  ter.enableLongDi
-0000aa90: 7374 616e 6365 4d61 7463 6869 6e67 602c  stanceMatching`,
-0000aaa0: 203a 7079 3a61 7474 723a 607e 4350 6172   :py:attr:`~CPar
-0000aab0: 616d 6574 6572 2e6c 646d 4861 7368 4c6f  ameter.ldmHashLo
-0000aac0: 6760 2c20 3a70 793a 6174 7472 3a60 7e43  g`, :py:attr:`~C
-0000aad0: 5061 7261 6d65 7465 722e 6c64 6d4d 696e  Parameter.ldmMin
-0000aae0: 4d61 7463 6860 2c20 3a70 793a 6174 7472  Match`, :py:attr
-0000aaf0: 3a60 7e43 5061 7261 6d65 7465 722e 6c64  :`~CParameter.ld
-0000ab00: 6d42 7563 6b65 7453 697a 654c 6f67 602c  mBucketSizeLog`,
-0000ab10: 203a 7079 3a61 7474 723a 607e 4350 6172   :py:attr:`~CPar
-0000ab20: 616d 6574 6572 2e6c 646d 4861 7368 5261  ameter.ldmHashRa
-0000ab30: 7465 4c6f 6760 290a 2020 2020 2020 2020  teLog`).        
-0000ab40: 2d20 4d69 7363 2028 3a70 793a 6174 7472  - Misc (:py:attr
-0000ab50: 3a60 7e43 5061 7261 6d65 7465 722e 636f  :`~CParameter.co
-0000ab60: 6e74 656e 7453 697a 6546 6c61 6760 2c20  ntentSizeFlag`, 
-0000ab70: 3a70 793a 6174 7472 3a60 7e43 5061 7261  :py:attr:`~CPara
-0000ab80: 6d65 7465 722e 6368 6563 6b73 756d 466c  meter.checksumFl
-0000ab90: 6167 602c 203a 7079 3a61 7474 723a 607e  ag`, :py:attr:`~
-0000aba0: 4350 6172 616d 6574 6572 2e64 6963 7449  CParameter.dictI
-0000abb0: 4446 6c61 6760 290a 2020 2020 2020 2020  DFlag`).        
-0000abc0: 2d20 4d75 6c74 692d 7468 7265 6164 6564  - Multi-threaded
-0000abd0: 2063 6f6d 7072 6573 7369 6f6e 2028 3a70   compression (:p
-0000abe0: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
-0000abf0: 7465 722e 6e62 576f 726b 6572 7360 2c20  ter.nbWorkers`, 
-0000ac00: 3a70 793a 6174 7472 3a60 7e43 5061 7261  :py:attr:`~CPara
-0000ac10: 6d65 7465 722e 6a6f 6253 697a 6560 2c20  meter.jobSize`, 
-0000ac20: 3a70 793a 6174 7472 3a60 7e43 5061 7261  :py:attr:`~CPara
-0000ac30: 6d65 7465 722e 6f76 6572 6c61 704c 6f67  meter.overlapLog
-0000ac40: 6029 0a0a 2020 2020 3a70 793a 636c 6173  `)..    :py:clas
-0000ac50: 733a 6044 5061 7261 6d65 7465 7260 2063  s:`DParameter` c
-0000ac60: 6c61 7373 2720 6174 7472 6962 7574 653a  lass' attribute:
-0000ac70: 0a0a 2020 2020 2020 2020 2d20 4465 636f  ..        - Deco
-0000ac80: 6d70 7265 7373 696f 6e20 7061 7261 6d65  mpression parame
-0000ac90: 7465 7220 283a 7079 3a61 7474 723a 607e  ter (:py:attr:`~
-0000aca0: 4450 6172 616d 6574 6572 2e77 696e 646f  DParameter.windo
-0000acb0: 774c 6f67 4d61 7860 290a 0a20 2020 203a  wLogMax`)..    :
-0000acc0: 7079 3a63 6c61 7373 3a60 5374 7261 7465  py:class:`Strate
-0000acd0: 6779 6020 636c 6173 7327 2061 7474 7269  gy` class' attri
-0000ace0: 6275 7465 733a 0a0a 2020 2020 2020 2020  butes:..        
-0000acf0: 3a70 793a 6174 7472 3a60 7e53 7472 6174  :py:attr:`~Strat
-0000ad00: 6567 792e 6661 7374 602c 203a 7079 3a61  egy.fast`, :py:a
-0000ad10: 7474 723a 607e 5374 7261 7465 6779 2e64  ttr:`~Strategy.d
-0000ad20: 6661 7374 602c 203a 7079 3a61 7474 723a  fast`, :py:attr:
-0000ad30: 607e 5374 7261 7465 6779 2e67 7265 6564  `~Strategy.greed
-0000ad40: 7960 2c20 3a70 793a 6174 7472 3a60 7e53  y`, :py:attr:`~S
-0000ad50: 7472 6174 6567 792e 6c61 7a79 602c 203a  trategy.lazy`, :
-0000ad60: 7079 3a61 7474 723a 607e 5374 7261 7465  py:attr:`~Strate
-0000ad70: 6779 2e6c 617a 7932 602c 203a 7079 3a61  gy.lazy2`, :py:a
-0000ad80: 7474 723a 607e 5374 7261 7465 6779 2e62  ttr:`~Strategy.b
-0000ad90: 746c 617a 7932 602c 203a 7079 3a61 7474  tlazy2`, :py:att
-0000ada0: 723a 607e 5374 7261 7465 6779 2e62 746f  r:`~Strategy.bto
-0000adb0: 7074 602c 203a 7079 3a61 7474 723a 607e  pt`, :py:attr:`~
-0000adc0: 5374 7261 7465 6779 2e62 7475 6c74 7261  Strategy.btultra
-0000add0: 602c 203a 7079 3a61 7474 723a 607e 5374  `, :py:attr:`~St
-0000ade0: 7261 7465 6779 2e62 7475 6c74 7261 3260  rategy.btultra2`
-0000adf0: 2e0a 0a2e 2e20 5f43 5061 7261 6d65 7465  ..... _CParamete
-0000ae00: 723a 0a0a 2e2e 2070 793a 636c 6173 733a  r:.... py:class:
-0000ae10: 3a20 4350 6172 616d 6574 6572 2849 6e74  : CParameter(Int
-0000ae20: 456e 756d 290a 0a20 2020 2041 6476 616e  Enum)..    Advan
-0000ae30: 6365 6420 636f 6d70 7265 7373 696f 6e20  ced compression 
-0000ae40: 7061 7261 6d65 7465 7273 2e0a 0a20 2020  parameters...   
-0000ae50: 2057 6865 6e20 7573 696e 672c 2070 7574   When using, put
-0000ae60: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
-0000ae70: 696e 2061 2060 6064 6963 7460 6020 6f62  in a ``dict`` ob
-0000ae80: 6a65 6374 2c20 7468 6520 6b65 7920 6973  ject, the key is
-0000ae90: 2061 203a 7079 3a63 6c61 7373 3a60 4350   a :py:class:`CP
-0000aea0: 6172 616d 6574 6572 6020 6e61 6d65 2c20  arameter` name, 
-0000aeb0: 7468 6520 7661 6c75 6520 6973 2061 2033  the value is a 3
-0000aec0: 322d 6269 7420 7369 676e 6564 2069 6e74  2-bit signed int
-0000aed0: 6567 6572 2076 616c 7565 2e0a 0a20 2020  eger value...   
-0000aee0: 202e 2e20 736f 7572 6365 636f 6465 3a3a   .. sourcecode::
-0000aef0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
-0000af00: 206f 7074 696f 6e20 3d20 7b43 5061 7261   option = {CPara
-0000af10: 6d65 7465 722e 636f 6d70 7265 7373 696f  meter.compressio
-0000af20: 6e4c 6576 656c 203a 2031 302c 0a20 2020  nLevel : 10,.   
-0000af30: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-0000af40: 5061 7261 6d65 7465 722e 6368 6563 6b73  Parameter.checks
-0000af50: 756d 466c 6167 203a 2031 7d0a 0a20 2020  umFlag : 1}..   
-0000af60: 2020 2020 2023 2075 7365 6420 7769 7468       # used with
-0000af70: 2063 6f6d 7072 6573 7328 2920 6675 6e63   compress() func
-0000af80: 7469 6f6e 0a20 2020 2020 2020 2063 6f6d  tion.        com
-0000af90: 7072 6573 7365 645f 6461 7420 3d20 636f  pressed_dat = co
-0000afa0: 6d70 7265 7373 2872 6177 5f64 6174 2c20  mpress(raw_dat, 
-0000afb0: 6f70 7469 6f6e 290a 0a20 2020 2020 2020  option)..       
-0000afc0: 2023 2075 7365 6420 7769 7468 205a 7374   # used with Zst
-0000afd0: 6443 6f6d 7072 6573 736f 7220 6f62 6a65  dCompressor obje
-0000afe0: 6374 0a20 2020 2020 2020 2063 203d 205a  ct.        c = Z
-0000aff0: 7374 6443 6f6d 7072 6573 736f 7228 6c65  stdCompressor(le
-0000b000: 7665 6c5f 6f72 5f6f 7074 696f 6e3d 6f70  vel_or_option=op
-0000b010: 7469 6f6e 290a 2020 2020 2020 2020 636f  tion).        co
-0000b020: 6d70 7265 7373 6564 5f64 6174 3120 3d20  mpressed_dat1 = 
-0000b030: 632e 636f 6d70 7265 7373 2872 6177 5f64  c.compress(raw_d
-0000b040: 6174 290a 2020 2020 2020 2020 636f 6d70  at).        comp
-0000b050: 7265 7373 6564 5f64 6174 3220 3d20 632e  ressed_dat2 = c.
-0000b060: 666c 7573 6828 290a 0a20 2020 2050 6172  flush()..    Par
-0000b070: 616d 6574 6572 2076 616c 7565 2073 686f  ameter value sho
-0000b080: 756c 6420 6265 6c6f 6e67 2074 6f20 616e  uld belong to an
-0000b090: 2069 6e74 6572 7661 6c20 7769 7468 206c   interval with l
-0000b0a0: 6f77 6572 2061 6e64 2075 7070 6572 2062  ower and upper b
-0000b0b0: 6f75 6e64 732c 206f 7468 6572 7769 7365  ounds, otherwise
-0000b0c0: 2074 6865 7920 7769 6c6c 2065 6974 6865   they will eithe
-0000b0d0: 7220 7472 6967 6765 7220 616e 2065 7272  r trigger an err
-0000b0e0: 6f72 206f 7220 6265 2063 6c61 6d70 6564  or or be clamped
-0000b0f0: 2073 696c 656e 746c 792e 0a0a 2020 2020   silently...    
-0000b100: 5468 6520 636f 6e73 7461 6e74 2076 616c  The constant val
-0000b110: 7565 7320 6d65 6e74 696f 6e65 6420 6265  ues mentioned be
-0000b120: 6c6f 7720 6172 6520 6465 6669 6e65 6420  low are defined 
-0000b130: 696e 2060 7a73 7464 2e68 203c 6874 7470  in `zstd.h <http
-0000b140: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-0000b150: 6163 6562 6f6f 6b2f 7a73 7464 2f62 6c6f  acebook/zstd/blo
-0000b160: 622f 7265 6c65 6173 652f 6c69 622f 7a73  b/release/lib/zs
-0000b170: 7464 2e68 3e60 5f2c 206e 6f74 6520 7468  td.h>`_, note th
-0000b180: 6174 2074 6865 7365 2076 616c 7565 7320  at these values 
-0000b190: 6d61 7920 6265 2064 6966 6665 7265 6e74  may be different
-0000b1a0: 2069 6e20 6469 6666 6572 656e 7420 7a73   in different zs
-0000b1b0: 7464 2076 6572 7369 6f6e 732e 0a0a 2020  td versions...  
-0000b1c0: 2020 2e2e 2070 793a 6d65 7468 6f64 3a3a    .. py:method::
-0000b1d0: 2062 6f75 6e64 7328 7365 6c66 290a 0a20   bounds(self).. 
-0000b1e0: 2020 2020 2020 2052 6574 7572 6e20 6c6f         Return lo
-0000b1f0: 7765 7220 616e 6420 7570 7065 7220 626f  wer and upper bo
-0000b200: 756e 6473 206f 6620 6120 7061 7261 6d65  unds of a parame
-0000b210: 7465 722c 2062 6f74 6820 696e 636c 7573  ter, both inclus
-0000b220: 6976 652e 0a0a 2020 2020 2020 2020 2e2e  ive...        ..
-0000b230: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
-0000b240: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0000b250: 2020 3e3e 3e20 4350 6172 616d 6574 6572    >>> CParameter
-0000b260: 2e63 6f6d 7072 6573 7369 6f6e 4c65 7665  .compressionLeve
-0000b270: 6c2e 626f 756e 6473 2829 0a20 2020 2020  l.bounds().     
-0000b280: 2020 2020 2020 2028 2d31 3331 3037 322c         (-131072,
-0000b290: 2032 3229 0a20 2020 2020 2020 2020 2020   22).           
-0000b2a0: 203e 3e3e 2043 5061 7261 6d65 7465 722e   >>> CParameter.
-0000b2b0: 7769 6e64 6f77 4c6f 672e 626f 756e 6473  windowLog.bounds
-0000b2c0: 2829 0a20 2020 2020 2020 2020 2020 2028  ().            (
-0000b2d0: 3130 2c20 3331 290a 2020 2020 2020 2020  10, 31).        
-0000b2e0: 2020 2020 3e3e 3e20 4350 6172 616d 6574      >>> CParamet
-0000b2f0: 6572 2e65 6e61 626c 654c 6f6e 6744 6973  er.enableLongDis
-0000b300: 7461 6e63 654d 6174 6368 696e 672e 626f  tanceMatching.bo
-0000b310: 756e 6473 2829 0a20 2020 2020 2020 2020  unds().         
-0000b320: 2020 2028 302c 2031 290a 0a20 2020 202e     (0, 1)..    .
-0000b330: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
-0000b340: 2063 6f6d 7072 6573 7369 6f6e 4c65 7665   compressionLeve
-0000b350: 6c0a 0a20 2020 2020 2020 2053 6574 2063  l..        Set c
-0000b360: 6f6d 7072 6573 7369 6f6e 2070 6172 616d  ompression param
-0000b370: 6574 6572 7320 6163 636f 7264 696e 6720  eters according 
-0000b380: 746f 2070 7265 2d64 6566 696e 6564 2063  to pre-defined c
-0000b390: 6f6d 7072 6573 7369 6f6e 4c65 7665 6c20  ompressionLevel 
-0000b3a0: 7461 626c 652c 2073 6565 203a 7265 663a  table, see :ref:
-0000b3b0: 6063 6f6d 7072 6573 7369 6f6e 206c 6576  `compression lev
-0000b3c0: 656c 3c63 6f6d 7072 6573 7369 6f6e 5f6c  el<compression_l
-0000b3d0: 6576 656c 3e60 2066 6f72 2064 6574 6169  evel>` for detai
-0000b3e0: 6c73 2e0a 0a20 2020 2020 2020 2053 6574  ls...        Set
-0000b3f0: 7469 6e67 2061 2063 6f6d 7072 6573 7369  ting a compressi
-0000b400: 6f6e 206c 6576 656c 2064 6f65 7320 6e6f  on level does no
-0000b410: 7420 7365 7420 616c 6c20 6f74 6865 7220  t set all other 
-0000b420: 636f 6d70 7265 7373 696f 6e20 7061 7261  compression para
-0000b430: 6d65 7465 7273 2074 6f20 6465 6661 756c  meters to defaul
-0000b440: 742e 2053 6574 7469 6e67 2074 6869 7320  t. Setting this 
-0000b450: 7769 6c6c 2064 796e 616d 6963 616c 6c79  will dynamically
-0000b460: 2069 6d70 6163 7420 7468 6520 636f 6d70   impact the comp
-0000b470: 7265 7373 696f 6e20 7061 7261 6d65 7465  ression paramete
-0000b480: 7273 2077 6869 6368 2068 6176 6520 6e6f  rs which have no
-0000b490: 7420 6265 656e 206d 616e 7561 6c6c 7920  t been manually 
-0000b4a0: 7365 742c 2074 6865 206d 616e 7561 6c6c  set, the manuall
-0000b4b0: 7920 7365 7420 6f6e 6573 2077 696c 6c20  y set ones will 
-0000b4c0: 2273 7469 636b 222e 0a0a 2020 2020 2e2e  "stick"...    ..
-0000b4d0: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
-0000b4e0: 7769 6e64 6f77 4c6f 670a 0a20 2020 2020  windowLog..     
-0000b4f0: 2020 204d 6178 696d 756d 2061 6c6c 6f77     Maximum allow
-0000b500: 6564 2062 6163 6b2d 7265 6665 7265 6e63  ed back-referenc
-0000b510: 6520 6469 7374 616e 6365 2c20 6578 7072  e distance, expr
-0000b520: 6573 7365 6420 6173 2070 6f77 6572 206f  essed as power o
-0000b530: 6620 322c 2060 6031 203c 3c20 7769 6e64  f 2, ``1 << wind
-0000b540: 6f77 4c6f 6760 6020 6279 7465 732e 0a0a  owLog`` bytes...
-0000b550: 2020 2020 2020 2020 4c61 7267 6572 2076          Larger v
-0000b560: 616c 7565 7320 7265 7175 6972 696e 6720  alues requiring 
-0000b570: 6d6f 7265 206d 656d 6f72 7920 616e 6420  more memory and 
-0000b580: 7479 7069 6361 6c6c 7920 636f 6d70 7265  typically compre
-0000b590: 7373 696e 6720 6d6f 7265 2e0a 0a20 2020  ssing more...   
-0000b5a0: 2020 2020 2054 6869 7320 7769 6c6c 2073       This will s
-0000b5b0: 6574 2061 206d 656d 6f72 7920 6275 6467  et a memory budg
-0000b5c0: 6574 2066 6f72 2073 7472 6561 6d69 6e67  et for streaming
-0000b5d0: 2064 6563 6f6d 7072 6573 7369 6f6e 2e20   decompression. 
-0000b5e0: 5573 696e 6720 6120 7661 6c75 6520 6772  Using a value gr
-0000b5f0: 6561 7465 7220 7468 616e 2060 605a 5354  eater than ``ZST
-0000b600: 445f 5749 4e44 4f57 4c4f 475f 4c49 4d49  D_WINDOWLOG_LIMI
-0000b610: 545f 4445 4641 554c 5460 6020 7265 7175  T_DEFAULT`` requ
-0000b620: 6972 6573 2065 7870 6c69 6369 746c 7920  ires explicitly 
-0000b630: 616c 6c6f 7769 6e67 2073 7563 6820 7369  allowing such si
-0000b640: 7a65 2061 7420 7374 7265 616d 696e 6720  ze at streaming 
-0000b650: 6465 636f 6d70 7265 7373 696f 6e20 7374  decompression st
-0000b660: 6167 652c 2073 6565 203a 7079 3a61 7474  age, see :py:att
-0000b670: 723a 6044 5061 7261 6d65 7465 722e 7769  r:`DParameter.wi
-0000b680: 6e64 6f77 4c6f 674d 6178 602e 2060 605a  ndowLogMax`. ``Z
-0000b690: 5354 445f 5749 4e44 4f57 4c4f 475f 4c49  STD_WINDOWLOG_LI
-0000b6a0: 4d49 545f 4445 4641 554c 5460 6020 6973  MIT_DEFAULT`` is
-0000b6b0: 2032 3720 696e 207a 7374 6420 7631 2e32   27 in zstd v1.2
-0000b6c0: 2b2c 206d 6561 6e73 2031 3238 204d 6942  +, means 128 MiB
-0000b6d0: 2028 3120 3c3c 2032 3729 2e0a 0a20 2020   (1 << 27)...   
-0000b6e0: 2020 2020 204d 7573 7420 6265 2063 6c61       Must be cla
-0000b6f0: 6d70 6564 2062 6574 7765 656e 2060 605a  mped between ``Z
-0000b700: 5354 445f 5749 4e44 4f57 4c4f 475f 4d49  STD_WINDOWLOG_MI
-0000b710: 4e60 6020 616e 6420 6060 5a53 5444 5f57  N`` and ``ZSTD_W
-0000b720: 494e 444f 574c 4f47 5f4d 4158 6060 2e0a  INDOWLOG_MAX``..
-0000b730: 0a20 2020 2020 2020 2053 7065 6369 616c  .        Special
-0000b740: 3a20 7661 6c75 6520 6060 3060 6020 6d65  : value ``0`` me
-0000b750: 616e 7320 2275 7365 2064 6566 6175 6c74  ans "use default
-0000b760: 2077 696e 646f 774c 6f67 222c 2074 6865   windowLog", the
-0000b770: 6e20 7468 6520 7661 6c75 6520 6973 2064  n the value is d
-0000b780: 796e 616d 6963 616c 6c79 2073 6574 2c20  ynamically set, 
-0000b790: 7365 6520 2257 2220 636f 6c75 6d6e 2069  see "W" column i
-0000b7a0: 6e20 6074 6869 7320 7461 626c 6520 3c68  n `this table <h
-0000b7b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000b7c0: 6d2f 6661 6365 626f 6f6b 2f7a 7374 642f  m/facebook/zstd/
-0000b7d0: 626c 6f62 2f72 656c 6561 7365 2f6c 6962  blob/release/lib
-0000b7e0: 2f63 6f6d 7072 6573 732f 636c 6576 656c  /compress/clevel
-0000b7f0: 732e 683e 605f 2e0a 0a20 2020 202e 2e20  s.h>`_...    .. 
-0000b800: 7079 3a61 7474 7269 6275 7465 3a3a 2068  py:attribute:: h
-0000b810: 6173 684c 6f67 0a0a 2020 2020 2020 2020  ashLog..        
-0000b820: 5369 7a65 206f 6620 7468 6520 696e 6974  Size of the init
-0000b830: 6961 6c20 7072 6f62 6520 7461 626c 652c  ial probe table,
-0000b840: 2061 7320 6120 706f 7765 7220 6f66 2032   as a power of 2
-0000b850: 2c20 7265 7375 6c74 696e 6720 6d65 6d6f  , resulting memo
-0000b860: 7279 2075 7361 6765 2069 7320 6060 3120  ry usage is ``1 
-0000b870: 3c3c 2028 6861 7368 4c6f 672b 3229 6060  << (hashLog+2)``
-0000b880: 2062 7974 6573 2e0a 0a20 2020 2020 2020   bytes...       
-0000b890: 204d 7573 7420 6265 2063 6c61 6d70 6564   Must be clamped
-0000b8a0: 2062 6574 7765 656e 2060 605a 5354 445f   between ``ZSTD_
-0000b8b0: 4841 5348 4c4f 475f 4d49 4e60 6020 616e  HASHLOG_MIN`` an
-0000b8c0: 6420 6060 5a53 5444 5f48 4153 484c 4f47  d ``ZSTD_HASHLOG
-0000b8d0: 5f4d 4158 6060 2e0a 0a20 2020 2020 2020  _MAX``...       
-0000b8e0: 204c 6172 6765 7220 7461 626c 6573 2069   Larger tables i
-0000b8f0: 6d70 726f 7665 2063 6f6d 7072 6573 7369  mprove compressi
-0000b900: 6f6e 2072 6174 696f 206f 6620 7374 7261  on ratio of stra
-0000b910: 7465 6769 6573 203c 3d20 3a70 793a 6174  tegies <= :py:at
-0000b920: 7472 3a60 7e53 7472 6174 6567 792e 6466  tr:`~Strategy.df
-0000b930: 6173 7460 2c20 616e 6420 696d 7072 6f76  ast`, and improv
-0000b940: 6520 7370 6565 6420 6f66 2073 7472 6174  e speed of strat
-0000b950: 6567 6965 7320 3e20 3a70 793a 6174 7472  egies > :py:attr
-0000b960: 3a60 7e53 7472 6174 6567 792e 6466 6173  :`~Strategy.dfas
-0000b970: 7460 2e0a 0a20 2020 2020 2020 2053 7065  t`...        Spe
-0000b980: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
-0000b990: 6020 6d65 616e 7320 2275 7365 2064 6566  ` means "use def
-0000b9a0: 6175 6c74 2068 6173 684c 6f67 222c 2074  ault hashLog", t
-0000b9b0: 6865 6e20 7468 6520 7661 6c75 6520 6973  hen the value is
-0000b9c0: 2064 796e 616d 6963 616c 6c79 2073 6574   dynamically set
-0000b9d0: 2c20 7365 6520 2248 2220 636f 6c75 6d6e  , see "H" column
-0000b9e0: 2069 6e20 6074 6869 7320 7461 626c 6520   in `this table 
-0000b9f0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-0000ba00: 636f 6d2f 6661 6365 626f 6f6b 2f7a 7374  com/facebook/zst
-0000ba10: 642f 626c 6f62 2f72 656c 6561 7365 2f6c  d/blob/release/l
-0000ba20: 6962 2f63 6f6d 7072 6573 732f 636c 6576  ib/compress/clev
-0000ba30: 656c 732e 683e 605f 2e0a 0a20 2020 202e  els.h>`_...    .
-0000ba40: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
-0000ba50: 2063 6861 696e 4c6f 670a 0a20 2020 2020   chainLog..     
-0000ba60: 2020 2053 697a 6520 6f66 2074 6865 206d     Size of the m
-0000ba70: 756c 7469 2d70 726f 6265 2073 6561 7263  ulti-probe searc
-0000ba80: 6820 7461 626c 652c 2061 7320 6120 706f  h table, as a po
-0000ba90: 7765 7220 6f66 2032 2c20 7265 7375 6c74  wer of 2, result
-0000baa0: 696e 6720 6d65 6d6f 7279 2075 7361 6765  ing memory usage
-0000bab0: 2069 7320 6060 3120 3c3c 2028 6368 6169   is ``1 << (chai
-0000bac0: 6e4c 6f67 2b32 2960 6020 6279 7465 732e  nLog+2)`` bytes.
-0000bad0: 0a0a 2020 2020 2020 2020 4d75 7374 2062  ..        Must b
-0000bae0: 6520 636c 616d 7065 6420 6265 7477 6565  e clamped betwee
-0000baf0: 6e20 6060 5a53 5444 5f43 4841 494e 4c4f  n ``ZSTD_CHAINLO
-0000bb00: 475f 4d49 4e60 6020 616e 6420 6060 5a53  G_MIN`` and ``ZS
-0000bb10: 5444 5f43 4841 494e 4c4f 475f 4d41 5860  TD_CHAINLOG_MAX`
-0000bb20: 602e 0a0a 2020 2020 2020 2020 4c61 7267  `...        Larg
-0000bb30: 6572 2074 6162 6c65 7320 7265 7375 6c74  er tables result
-0000bb40: 2069 6e20 6265 7474 6572 2061 6e64 2073   in better and s
-0000bb50: 6c6f 7765 7220 636f 6d70 7265 7373 696f  lower compressio
-0000bb60: 6e2e 0a0a 2020 2020 2020 2020 5468 6973  n...        This
-0000bb70: 2070 6172 616d 6574 6572 2069 7320 7573   parameter is us
-0000bb80: 656c 6573 7320 666f 7220 3a70 793a 6174  eless for :py:at
-0000bb90: 7472 3a60 7e53 7472 6174 6567 792e 6661  tr:`~Strategy.fa
-0000bba0: 7374 6020 7374 7261 7465 6779 2e0a 0a20  st` strategy... 
-0000bbb0: 2020 2020 2020 2049 7427 7320 7374 696c         It's stil
-0000bbc0: 6c20 7573 6566 756c 2077 6865 6e20 7573  l useful when us
-0000bbd0: 696e 6720 3a70 793a 6174 7472 3a60 7e53  ing :py:attr:`~S
-0000bbe0: 7472 6174 6567 792e 6466 6173 7460 2073  trategy.dfast` s
-0000bbf0: 7472 6174 6567 792c 2069 6e20 7768 6963  trategy, in whic
-0000bc00: 6820 6361 7365 2069 7420 6465 6669 6e65  h case it define
-0000bc10: 7320 6120 7365 636f 6e64 6172 7920 7072  s a secondary pr
-0000bc20: 6f62 6520 7461 626c 652e 0a0a 2020 2020  obe table...    
-0000bc30: 2020 2020 5370 6563 6961 6c3a 2076 616c      Special: val
-0000bc40: 7565 2060 6030 6060 206d 6561 6e73 2022  ue ``0`` means "
-0000bc50: 7573 6520 6465 6661 756c 7420 6368 6169  use default chai
-0000bc60: 6e4c 6f67 222c 2074 6865 6e20 7468 6520  nLog", then the 
-0000bc70: 7661 6c75 6520 6973 2064 796e 616d 6963  value is dynamic
-0000bc80: 616c 6c79 2073 6574 2c20 7365 6520 2243  ally set, see "C
-0000bc90: 2220 636f 6c75 6d6e 2069 6e20 6074 6869  " column in `thi
-0000bca0: 7320 7461 626c 6520 3c68 7474 7073 3a2f  s table <https:/
-0000bcb0: 2f67 6974 6875 622e 636f 6d2f 6661 6365  /github.com/face
-0000bcc0: 626f 6f6b 2f7a 7374 642f 626c 6f62 2f72  book/zstd/blob/r
-0000bcd0: 656c 6561 7365 2f6c 6962 2f63 6f6d 7072  elease/lib/compr
-0000bce0: 6573 732f 636c 6576 656c 732e 683e 605f  ess/clevels.h>`_
-0000bcf0: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
-0000bd00: 7269 6275 7465 3a3a 2073 6561 7263 684c  ribute:: searchL
-0000bd10: 6f67 0a0a 2020 2020 2020 2020 4e75 6d62  og..        Numb
-0000bd20: 6572 206f 6620 7365 6172 6368 2061 7474  er of search att
-0000bd30: 656d 7074 732c 2061 7320 6120 706f 7765  empts, as a powe
-0000bd40: 7220 6f66 2032 2e0a 0a20 2020 2020 2020  r of 2...       
-0000bd50: 204d 6f72 6520 6174 7465 6d70 7473 2072   More attempts r
-0000bd60: 6573 756c 7420 696e 2062 6574 7465 7220  esult in better 
-0000bd70: 616e 6420 736c 6f77 6572 2063 6f6d 7072  and slower compr
-0000bd80: 6573 7369 6f6e 2e0a 0a20 2020 2020 2020  ession...       
-0000bd90: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
-0000bda0: 6973 2075 7365 6c65 7373 2066 6f72 203a  is useless for :
-0000bdb0: 7079 3a61 7474 723a 607e 5374 7261 7465  py:attr:`~Strate
-0000bdc0: 6779 2e66 6173 7460 2061 6e64 203a 7079  gy.fast` and :py
-0000bdd0: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
-0000bde0: 2e64 6661 7374 6020 7374 7261 7465 6769  .dfast` strategi
-0000bdf0: 6573 2e0a 0a20 2020 2020 2020 2053 7065  es...        Spe
-0000be00: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
-0000be10: 6020 6d65 616e 7320 2275 7365 2064 6566  ` means "use def
-0000be20: 6175 6c74 2073 6561 7263 684c 6f67 222c  ault searchLog",
-0000be30: 2074 6865 6e20 7468 6520 7661 6c75 6520   then the value 
-0000be40: 6973 2064 796e 616d 6963 616c 6c79 2073  is dynamically s
-0000be50: 6574 2c20 7365 6520 2253 2220 636f 6c75  et, see "S" colu
-0000be60: 6d6e 2069 6e20 6074 6869 7320 7461 626c  mn in `this tabl
-0000be70: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
-0000be80: 622e 636f 6d2f 6661 6365 626f 6f6b 2f7a  b.com/facebook/z
-0000be90: 7374 642f 626c 6f62 2f72 656c 6561 7365  std/blob/release
-0000bea0: 2f6c 6962 2f63 6f6d 7072 6573 732f 636c  /lib/compress/cl
-0000beb0: 6576 656c 732e 683e 605f 2e0a 0a20 2020  evels.h>`_...   
-0000bec0: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
-0000bed0: 3a3a 206d 696e 4d61 7463 680a 0a20 2020  :: minMatch..   
-0000bee0: 2020 2020 204d 696e 696d 756d 2073 697a       Minimum siz
-0000bef0: 6520 6f66 2073 6561 7263 6865 6420 6d61  e of searched ma
-0000bf00: 7463 6865 732e 0a0a 2020 2020 2020 2020  tches...        
-0000bf10: 4e6f 7465 2074 6861 7420 5a73 7461 6e64  Note that Zstand
-0000bf20: 6172 6420 6361 6e20 7374 696c 6c20 6669  ard can still fi
-0000bf30: 6e64 206d 6174 6368 6573 206f 6620 736d  nd matches of sm
-0000bf40: 616c 6c65 7220 7369 7a65 2c20 6974 206a  aller size, it j
-0000bf50: 7573 7420 7477 6561 6b73 2069 7473 2073  ust tweaks its s
-0000bf60: 6561 7263 6820 616c 676f 7269 7468 6d20  earch algorithm 
-0000bf70: 746f 206c 6f6f 6b20 666f 7220 7468 6973  to look for this
-0000bf80: 2073 697a 6520 616e 6420 6c61 7267 6572   size and larger
-0000bf90: 2e0a 0a20 2020 2020 2020 204c 6172 6765  ...        Large
-0000bfa0: 7220 7661 6c75 6573 2069 6e63 7265 6173  r values increas
-0000bfb0: 6520 636f 6d70 7265 7373 696f 6e20 616e  e compression an
-0000bfc0: 6420 6465 636f 6d70 7265 7373 696f 6e20  d decompression 
-0000bfd0: 7370 6565 642c 2062 7574 2064 6563 7265  speed, but decre
-0000bfe0: 6173 6520 7261 7469 6f2e 0a0a 2020 2020  ase ratio...    
-0000bff0: 2020 2020 4d75 7374 2062 6520 636c 616d      Must be clam
-0000c000: 7065 6420 6265 7477 6565 6e20 6060 5a53  ped between ``ZS
-0000c010: 5444 5f4d 494e 4d41 5443 485f 4d49 4e60  TD_MINMATCH_MIN`
-0000c020: 6020 616e 6420 6060 5a53 5444 5f4d 494e  ` and ``ZSTD_MIN
-0000c030: 4d41 5443 485f 4d41 5860 602e 0a0a 2020  MATCH_MAX``...  
-0000c040: 2020 2020 2020 4e6f 7465 2074 6861 7420        Note that 
-0000c050: 6375 7272 656e 746c 792c 2066 6f72 2061  currently, for a
-0000c060: 6c6c 2073 7472 6174 6567 6965 7320 3c20  ll strategies < 
-0000c070: 3a70 793a 6174 7472 3a60 7e53 7472 6174  :py:attr:`~Strat
-0000c080: 6567 792e 6274 6f70 7460 2c20 6566 6665  egy.btopt`, effe
-0000c090: 6374 6976 6520 6d69 6e69 6d75 6d20 6973  ctive minimum is
-0000c0a0: 2060 6034 6060 2c20 666f 7220 616c 6c20   ``4``, for all 
-0000c0b0: 7374 7261 7465 6769 6573 203e 203a 7079  strategies > :py
-0000c0c0: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
-0000c0d0: 2e66 6173 7460 2c20 6566 6665 6374 6976  .fast`, effectiv
-0000c0e0: 6520 6d61 7869 6d75 6d20 6973 2060 6036  e maximum is ``6
-0000c0f0: 6060 2e0a 0a20 2020 2020 2020 2053 7065  ``...        Spe
-0000c100: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
-0000c110: 6020 6d65 616e 7320 2275 7365 2064 6566  ` means "use def
-0000c120: 6175 6c74 206d 696e 4d61 7463 684c 656e  ault minMatchLen
-0000c130: 6774 6822 2c20 7468 656e 2074 6865 2076  gth", then the v
-0000c140: 616c 7565 2069 7320 6479 6e61 6d69 6361  alue is dynamica
-0000c150: 6c6c 7920 7365 742c 2073 6565 2022 4c22  lly set, see "L"
-0000c160: 2063 6f6c 756d 6e20 696e 2060 7468 6973   column in `this
-0000c170: 2074 6162 6c65 203c 6874 7470 733a 2f2f   table <https://
-0000c180: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
-0000c190: 6f6f 6b2f 7a73 7464 2f62 6c6f 622f 7265  ook/zstd/blob/re
-0000c1a0: 6c65 6173 652f 6c69 622f 636f 6d70 7265  lease/lib/compre
-0000c1b0: 7373 2f63 6c65 7665 6c73 2e68 3e60 5f2e  ss/clevels.h>`_.
-0000c1c0: 0a0a 2020 2020 2e2e 2070 793a 6174 7472  ..    .. py:attr
-0000c1d0: 6962 7574 653a 3a20 7461 7267 6574 4c65  ibute:: targetLe
-0000c1e0: 6e67 7468 0a0a 2020 2020 2020 2020 496d  ngth..        Im
-0000c1f0: 7061 6374 206f 6620 7468 6973 2066 6965  pact of this fie
-0000c200: 6c64 2064 6570 656e 6473 206f 6e20 7374  ld depends on st
-0000c210: 7261 7465 6779 2e0a 0a20 2020 2020 2020  rategy...       
-0000c220: 2046 6f72 2073 7472 6174 6567 6965 7320   For strategies 
-0000c230: 3a70 793a 6174 7472 3a60 7e53 7472 6174  :py:attr:`~Strat
-0000c240: 6567 792e 6274 6f70 7460 2c20 3a70 793a  egy.btopt`, :py:
-0000c250: 6174 7472 3a60 7e53 7472 6174 6567 792e  attr:`~Strategy.
-0000c260: 6274 756c 7472 6160 2026 203a 7079 3a61  btultra` & :py:a
-0000c270: 7474 723a 607e 5374 7261 7465 6779 2e62  ttr:`~Strategy.b
-0000c280: 7475 6c74 7261 3260 3a0a 0a20 2020 2020  tultra2`:..     
-0000c290: 2020 2020 2020 204c 656e 6774 6820 6f66         Length of
-0000c2a0: 204d 6174 6368 2063 6f6e 7369 6465 7265   Match considere
-0000c2b0: 6420 2267 6f6f 6420 656e 6f75 6768 2220  d "good enough" 
-0000c2c0: 746f 2073 746f 7020 7365 6172 6368 2e0a  to stop search..
-0000c2d0: 0a20 2020 2020 2020 2020 2020 204c 6172  .            Lar
-0000c2e0: 6765 7220 7661 6c75 6573 206d 616b 6520  ger values make 
-0000c2f0: 636f 6d70 7265 7373 696f 6e20 7374 726f  compression stro
-0000c300: 6e67 6572 2c20 616e 6420 736c 6f77 6572  nger, and slower
-0000c310: 2e0a 0a20 2020 2020 2020 2046 6f72 2073  ...        For s
-0000c320: 7472 6174 6567 7920 3a70 793a 6174 7472  trategy :py:attr
-0000c330: 3a60 7e53 7472 6174 6567 792e 6661 7374  :`~Strategy.fast
-0000c340: 603a 0a0a 2020 2020 2020 2020 2020 2020  `:..            
-0000c350: 4469 7374 616e 6365 2062 6574 7765 656e  Distance between
-0000c360: 206d 6174 6368 2073 616d 706c 696e 672e   match sampling.
-0000c370: 0a0a 2020 2020 2020 2020 2020 2020 4c61  ..            La
-0000c380: 7267 6572 2076 616c 7565 7320 6d61 6b65  rger values make
-0000c390: 2063 6f6d 7072 6573 7369 6f6e 2066 6173   compression fas
-0000c3a0: 7465 722c 2061 6e64 2077 6561 6b65 722e  ter, and weaker.
-0000c3b0: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
-0000c3c0: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
-0000c3d0: 6561 6e73 2022 7573 6520 6465 6661 756c  eans "use defaul
-0000c3e0: 7420 7461 7267 6574 4c65 6e67 7468 222c  t targetLength",
-0000c3f0: 2074 6865 6e20 7468 6520 7661 6c75 6520   then the value 
-0000c400: 6973 2064 796e 616d 6963 616c 6c79 2073  is dynamically s
-0000c410: 6574 2c20 7365 6520 2254 4c22 2063 6f6c  et, see "TL" col
-0000c420: 756d 6e20 696e 2060 7468 6973 2074 6162  umn in `this tab
-0000c430: 6c65 203c 6874 7470 733a 2f2f 6769 7468  le <https://gith
-0000c440: 7562 2e63 6f6d 2f66 6163 6562 6f6f 6b2f  ub.com/facebook/
-0000c450: 7a73 7464 2f62 6c6f 622f 7265 6c65 6173  zstd/blob/releas
-0000c460: 652f 6c69 622f 636f 6d70 7265 7373 2f63  e/lib/compress/c
-0000c470: 6c65 7665 6c73 2e68 3e60 5f2e 0a0a 2020  levels.h>`_...  
-0000c480: 2020 2e2e 2070 793a 6174 7472 6962 7574    .. py:attribut
-0000c490: 653a 3a20 7374 7261 7465 6779 0a0a 2020  e:: strategy..  
-0000c4a0: 2020 2020 2020 5365 6520 3a70 793a 6174        See :py:at
-0000c4b0: 7472 3a60 5374 7261 7465 6779 6020 636c  tr:`Strategy` cl
-0000c4c0: 6173 7320 6465 6669 6e69 7469 6f6e 2e0a  ass definition..
-0000c4d0: 0a20 2020 2020 2020 2054 6865 2068 6967  .        The hig
-0000c4e0: 6865 7220 7468 6520 7661 6c75 6520 6f66  her the value of
-0000c4f0: 2073 656c 6563 7465 6420 7374 7261 7465   selected strate
-0000c500: 6779 2c20 7468 6520 6d6f 7265 2063 6f6d  gy, the more com
-0000c510: 706c 6578 2069 7420 6973 2c20 7265 7375  plex it is, resu
-0000c520: 6c74 696e 6720 696e 2073 7472 6f6e 6765  lting in stronge
-0000c530: 7220 616e 6420 736c 6f77 6572 2063 6f6d  r and slower com
-0000c540: 7072 6573 7369 6f6e 2e0a 0a20 2020 2020  pression...     
-0000c550: 2020 2053 7065 6369 616c 3a20 7661 6c75     Special: valu
-0000c560: 6520 6060 3060 6020 6d65 616e 7320 2275  e ``0`` means "u
-0000c570: 7365 2064 6566 6175 6c74 2073 7472 6174  se default strat
-0000c580: 6567 7922 2c20 7468 656e 2074 6865 2076  egy", then the v
-0000c590: 616c 7565 2069 7320 6479 6e61 6d69 6361  alue is dynamica
-0000c5a0: 6c6c 7920 7365 742c 2073 6565 2022 7374  lly set, see "st
-0000c5b0: 7261 7422 2063 6f6c 756d 6e20 696e 2060  rat" column in `
-0000c5c0: 7468 6973 2074 6162 6c65 203c 6874 7470  this table <http
-0000c5d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-0000c5e0: 6163 6562 6f6f 6b2f 7a73 7464 2f62 6c6f  acebook/zstd/blo
-0000c5f0: 622f 7265 6c65 6173 652f 6c69 622f 636f  b/release/lib/co
-0000c600: 6d70 7265 7373 2f63 6c65 7665 6c73 2e68  mpress/clevels.h
-0000c610: 3e60 5f2e 0a0a 2020 2020 2e2e 2070 793a  >`_...    .. py:
-0000c620: 6174 7472 6962 7574 653a 3a20 656e 6162  attribute:: enab
-0000c630: 6c65 4c6f 6e67 4469 7374 616e 6365 4d61  leLongDistanceMa
-0000c640: 7463 6869 6e67 0a0a 2020 2020 2020 2020  tching..        
-0000c650: 456e 6162 6c65 206c 6f6e 6720 6469 7374  Enable long dist
-0000c660: 616e 6365 206d 6174 6368 696e 672e 0a0a  ance matching...
-0000c670: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
-0000c680: 7661 6c75 6520 6973 2060 6030 6060 2c20  value is ``0``, 
-0000c690: 6361 6e20 6265 2060 6031 6060 2e0a 0a20  can be ``1``... 
-0000c6a0: 2020 2020 2020 2054 6869 7320 7061 7261         This para
-0000c6b0: 6d65 7465 7220 6973 2064 6573 6967 6e65  meter is designe
-0000c6c0: 6420 746f 2069 6d70 726f 7665 2063 6f6d  d to improve com
-0000c6d0: 7072 6573 7369 6f6e 2072 6174 696f 2c20  pression ratio, 
-0000c6e0: 666f 7220 6c61 7267 6520 696e 7075 7473  for large inputs
-0000c6f0: 2c20 6279 2066 696e 6469 6e67 206c 6172  , by finding lar
-0000c700: 6765 206d 6174 6368 6573 2061 7420 6c6f  ge matches at lo
-0000c710: 6e67 2064 6973 7461 6e63 652e 2049 7420  ng distance. It 
-0000c720: 696e 6372 6561 7365 7320 6d65 6d6f 7279  increases memory
-0000c730: 2075 7361 6765 2061 6e64 2077 696e 646f   usage and windo
-0000c740: 7720 7369 7a65 2e0a 0a20 2020 2020 2020  w size...       
-0000c750: 204e 6f74 653a 0a20 2020 2020 2020 2020   Note:.         
-0000c760: 2020 202a 2045 6e61 626c 696e 6720 7468     * Enabling th
-0000c770: 6973 2070 6172 616d 6574 6572 2069 6e63  is parameter inc
-0000c780: 7265 6173 6573 2064 6566 6175 6c74 203a  reases default :
-0000c790: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
-0000c7a0: 6574 6572 2e77 696e 646f 774c 6f67 6020  eter.windowLog` 
-0000c7b0: 746f 2031 3238 204d 6942 2065 7863 6570  to 128 MiB excep
-0000c7c0: 7420 7768 656e 2065 7870 7265 7373 6c79  t when expressly
-0000c7d0: 2073 6574 2074 6f20 6120 6469 6666 6572   set to a differ
-0000c7e0: 656e 7420 7661 6c75 652e 0a20 2020 2020  ent value..     
-0000c7f0: 2020 2020 2020 202a 2054 6869 7320 7769         * This wi
-0000c800: 6c6c 2062 6520 656e 6162 6c65 6420 6279  ll be enabled by
-0000c810: 2064 6566 6175 6c74 2069 6620 3a70 793a   default if :py:
-0000c820: 6174 7472 3a60 7e43 5061 7261 6d65 7465  attr:`~CParamete
-0000c830: 722e 7769 6e64 6f77 4c6f 6760 203e 3d20  r.windowLog` >= 
-0000c840: 3132 3820 4d69 4220 616e 6420 636f 6d70  128 MiB and comp
-0000c850: 7265 7373 696f 6e20 7374 7261 7465 6779  ression strategy
-0000c860: 203e 3d20 3a70 793a 6174 7472 3a60 7e53   >= :py:attr:`~S
-0000c870: 7472 6174 6567 792e 6274 6f70 7460 2028  trategy.btopt` (
-0000c880: 636f 6d70 7265 7373 696f 6e20 6c65 7665  compression leve
-0000c890: 6c20 3136 2b29 2e0a 0a20 2020 202e 2e20  l 16+)...    .. 
-0000c8a0: 7079 3a61 7474 7269 6275 7465 3a3a 206c  py:attribute:: l
-0000c8b0: 646d 4861 7368 4c6f 670a 0a20 2020 2020  dmHashLog..     
-0000c8c0: 2020 2053 697a 6520 6f66 2074 6865 2074     Size of the t
-0000c8d0: 6162 6c65 2066 6f72 206c 6f6e 6720 6469  able for long di
-0000c8e0: 7374 616e 6365 206d 6174 6368 696e 672c  stance matching,
-0000c8f0: 2061 7320 6120 706f 7765 7220 6f66 2032   as a power of 2
-0000c900: 2e0a 0a20 2020 2020 2020 204c 6172 6765  ...        Large
-0000c910: 7220 7661 6c75 6573 2069 6e63 7265 6173  r values increas
-0000c920: 6520 6d65 6d6f 7279 2075 7361 6765 2061  e memory usage a
-0000c930: 6e64 2063 6f6d 7072 6573 7369 6f6e 2072  nd compression r
-0000c940: 6174 696f 2c20 6275 7420 6465 6372 6561  atio, but decrea
-0000c950: 7365 2063 6f6d 7072 6573 7369 6f6e 2073  se compression s
-0000c960: 7065 6564 2e0a 0a20 2020 2020 2020 204d  peed...        M
-0000c970: 7573 7420 6265 2063 6c61 6d70 6564 2062  ust be clamped b
-0000c980: 6574 7765 656e 2060 605a 5354 445f 4841  etween ``ZSTD_HA
-0000c990: 5348 4c4f 475f 4d49 4e60 6020 616e 6420  SHLOG_MIN`` and 
-0000c9a0: 6060 5a53 5444 5f48 4153 484c 4f47 5f4d  ``ZSTD_HASHLOG_M
-0000c9b0: 4158 6060 2c20 6465 6661 756c 743a 203a  AX``, default: :
-0000c9c0: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
-0000c9d0: 6574 6572 2e77 696e 646f 774c 6f67 6020  eter.windowLog` 
-0000c9e0: 2d20 372e 0a0a 2020 2020 2020 2020 5370  - 7...        Sp
-0000c9f0: 6563 6961 6c3a 2076 616c 7565 2060 6030  ecial: value ``0
-0000ca00: 6060 206d 6561 6e73 2022 6175 746f 6d61  `` means "automa
-0000ca10: 7469 6361 6c6c 7920 6465 7465 726d 696e  tically determin
-0000ca20: 6520 6861 7368 6c6f 6722 2e0a 0a20 2020  e hashlog"...   
-0000ca30: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
-0000ca40: 3a3a 206c 646d 4d69 6e4d 6174 6368 0a0a  :: ldmMinMatch..
-0000ca50: 2020 2020 2020 2020 4d69 6e69 6d75 6d20          Minimum 
-0000ca60: 6d61 7463 6820 7369 7a65 2066 6f72 206c  match size for l
-0000ca70: 6f6e 6720 6469 7374 616e 6365 206d 6174  ong distance mat
-0000ca80: 6368 6572 2e0a 0a20 2020 2020 2020 204c  cher...        L
-0000ca90: 6172 6765 722f 746f 6f20 736d 616c 6c20  arger/too small 
-0000caa0: 7661 6c75 6573 2075 7375 616c 6c79 2064  values usually d
-0000cab0: 6563 7265 6173 6520 636f 6d70 7265 7373  ecrease compress
-0000cac0: 696f 6e20 7261 7469 6f2e 0a0a 2020 2020  ion ratio...    
-0000cad0: 2020 2020 4d75 7374 2062 6520 636c 616d      Must be clam
-0000cae0: 7065 6420 6265 7477 6565 6e20 6060 5a53  ped between ``ZS
-0000caf0: 5444 5f4c 444d 5f4d 494e 4d41 5443 485f  TD_LDM_MINMATCH_
-0000cb00: 4d49 4e60 6020 616e 6420 6060 5a53 5444  MIN`` and ``ZSTD
-0000cb10: 5f4c 444d 5f4d 494e 4d41 5443 485f 4d41  _LDM_MINMATCH_MA
-0000cb20: 5860 602e 0a0a 2020 2020 2020 2020 5370  X``...        Sp
-0000cb30: 6563 6961 6c3a 2076 616c 7565 2060 6030  ecial: value ``0
-0000cb40: 6060 206d 6561 6e73 2022 7573 6520 6465  `` means "use de
-0000cb50: 6661 756c 7420 7661 6c75 6522 2028 6465  fault value" (de
-0000cb60: 6661 756c 743a 2036 3429 2e0a 0a20 2020  fault: 64)...   
-0000cb70: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
-0000cb80: 3a3a 206c 646d 4275 636b 6574 5369 7a65  :: ldmBucketSize
-0000cb90: 4c6f 670a 0a20 2020 2020 2020 204c 6f67  Log..        Log
-0000cba0: 2073 697a 6520 6f66 2065 6163 6820 6275   size of each bu
-0000cbb0: 636b 6574 2069 6e20 7468 6520 4c44 4d20  cket in the LDM 
-0000cbc0: 6861 7368 2074 6162 6c65 2066 6f72 2063  hash table for c
-0000cbd0: 6f6c 6c69 7369 6f6e 2072 6573 6f6c 7574  ollision resolut
-0000cbe0: 696f 6e2e 0a0a 2020 2020 2020 2020 4c61  ion...        La
-0000cbf0: 7267 6572 2076 616c 7565 7320 696d 7072  rger values impr
-0000cc00: 6f76 6520 636f 6c6c 6973 696f 6e20 7265  ove collision re
-0000cc10: 736f 6c75 7469 6f6e 2062 7574 2064 6563  solution but dec
-0000cc20: 7265 6173 6520 636f 6d70 7265 7373 696f  rease compressio
-0000cc30: 6e20 7370 6565 642e 0a0a 2020 2020 2020  n speed...      
-0000cc40: 2020 5468 6520 6d61 7869 6d75 6d20 7661    The maximum va
-0000cc50: 6c75 6520 6973 2060 605a 5354 445f 4c44  lue is ``ZSTD_LD
-0000cc60: 4d5f 4255 434b 4554 5349 5a45 4c4f 475f  M_BUCKETSIZELOG_
-0000cc70: 4d41 5860 602e 0a0a 2020 2020 2020 2020  MAX``...        
-0000cc80: 5370 6563 6961 6c3a 2076 616c 7565 2060  Special: value `
-0000cc90: 6030 6060 206d 6561 6e73 2022 7573 6520  `0`` means "use 
-0000cca0: 6465 6661 756c 7420 7661 6c75 6522 2028  default value" (
-0000ccb0: 6465 6661 756c 743a 2033 292e 0a0a 2020  default: 3)...  
-0000ccc0: 2020 2e2e 2070 793a 6174 7472 6962 7574    .. py:attribut
-0000ccd0: 653a 3a20 6c64 6d48 6173 6852 6174 654c  e:: ldmHashRateL
-0000cce0: 6f67 0a0a 2020 2020 2020 2020 4672 6571  og..        Freq
-0000ccf0: 7565 6e63 7920 6f66 2069 6e73 6572 7469  uency of inserti
-0000cd00: 6e67 2f6c 6f6f 6b69 6e67 2075 7020 656e  ng/looking up en
-0000cd10: 7472 6965 7320 696e 746f 2074 6865 204c  tries into the L
-0000cd20: 444d 2068 6173 6820 7461 626c 652e 0a0a  DM hash table...
-0000cd30: 2020 2020 2020 2020 4d75 7374 2062 6520          Must be 
-0000cd40: 636c 616d 7065 6420 6265 7477 6565 6e20  clamped between 
-0000cd50: 3020 616e 6420 6060 285a 5354 445f 5749  0 and ``(ZSTD_WI
-0000cd60: 4e44 4f57 4c4f 475f 4d41 5820 2d20 5a53  NDOWLOG_MAX - ZS
-0000cd70: 5444 5f48 4153 484c 4f47 5f4d 494e 2960  TD_HASHLOG_MIN)`
-0000cd80: 602e 0a0a 2020 2020 2020 2020 4465 6661  `...        Defa
-0000cd90: 756c 7420 6973 204d 4158 2830 2c20 283a  ult is MAX(0, (:
-0000cda0: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
-0000cdb0: 6574 6572 2e77 696e 646f 774c 6f67 6020  eter.windowLog` 
-0000cdc0: 2d20 3a70 793a 6174 7472 3a60 7e43 5061  - :py:attr:`~CPa
-0000cdd0: 7261 6d65 7465 722e 6c64 6d48 6173 684c  rameter.ldmHashL
-0000cde0: 6f67 6029 292c 206f 7074 696d 697a 696e  og`)), optimizin
-0000cdf0: 6720 6861 7368 2074 6162 6c65 2075 7361  g hash table usa
-0000ce00: 6765 2e0a 0a20 2020 2020 2020 204c 6172  ge...        Lar
-0000ce10: 6765 7220 7661 6c75 6573 2069 6d70 726f  ger values impro
-0000ce20: 7665 2063 6f6d 7072 6573 7369 6f6e 2073  ve compression s
-0000ce30: 7065 6564 2e0a 0a20 2020 2020 2020 2044  peed...        D
-0000ce40: 6576 6961 7469 6e67 2066 6172 2066 726f  eviating far fro
-0000ce50: 6d20 6465 6661 756c 7420 7661 6c75 6520  m default value 
-0000ce60: 7769 6c6c 206c 696b 656c 7920 7265 7375  will likely resu
-0000ce70: 6c74 2069 6e20 6120 636f 6d70 7265 7373  lt in a compress
-0000ce80: 696f 6e20 7261 7469 6f20 6465 6372 6561  ion ratio decrea
-0000ce90: 7365 2e0a 0a20 2020 2020 2020 2053 7065  se...        Spe
-0000cea0: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
-0000ceb0: 6020 6d65 616e 7320 2261 7574 6f6d 6174  ` means "automat
-0000cec0: 6963 616c 6c79 2064 6574 6572 6d69 6e65  ically determine
-0000ced0: 2068 6173 6852 6174 654c 6f67 222e 0a0a   hashRateLog"...
-0000cee0: 2020 2020 2e2e 205f 636f 6e74 656e 745f      .. _content_
-0000cef0: 7369 7a65 3a0a 0a20 2020 202e 2e20 7079  size:..    .. py
-0000cf00: 3a61 7474 7269 6275 7465 3a3a 2063 6f6e  :attribute:: con
-0000cf10: 7465 6e74 5369 7a65 466c 6167 0a0a 2020  tentSizeFlag..  
-0000cf20: 2020 2020 2020 556e 636f 6d70 7265 7373        Uncompress
-0000cf30: 6564 2063 6f6e 7465 6e74 2073 697a 6520  ed content size 
-0000cf40: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
-0000cf50: 696e 746f 2066 7261 6d65 2068 6561 6465  into frame heade
-0000cf60: 7220 7768 656e 6576 6572 206b 6e6f 776e  r whenever known
-0000cf70: 2e0a 0a20 2020 2020 2020 2044 6566 6175  ...        Defau
-0000cf80: 6c74 2076 616c 7565 2069 7320 6060 3160  lt value is ``1`
-0000cf90: 602c 2063 616e 2062 6520 6060 3060 602e  `, can be ``0``.
-0000cfa0: 0a0a 2020 2020 2020 2020 496e 2074 7261  ..        In tra
-0000cfb0: 6469 7469 6f6e 616c 2073 7472 6561 6d69  ditional streami
-0000cfc0: 6e67 2063 6f6d 7072 6573 7369 6f6e 2c20  ng compression, 
-0000cfd0: 636f 6e74 656e 7420 7369 7a65 2069 7320  content size is 
-0000cfe0: 756e 6b6e 6f77 6e2e 0a0a 2020 2020 2020  unknown...      
-0000cff0: 2020 496e 2074 6865 7365 2063 6f6d 7072    In these compr
-0000d000: 6573 7369 6f6e 732c 2074 6865 2063 6f6e  essions, the con
-0000d010: 7465 6e74 2073 697a 6520 6973 206b 6e6f  tent size is kno
-0000d020: 776e 3a0a 0a20 2020 2020 2020 2020 2020  wn:..           
-0000d030: 202a 203a 7079 3a66 756e 633a 6063 6f6d   * :py:func:`com
-0000d040: 7072 6573 7360 2066 756e 6374 696f 6e0a  press` function.
-0000d050: 2020 2020 2020 2020 2020 2020 2a20 3a70              * :p
-0000d060: 793a 6675 6e63 3a60 7269 6368 6d65 6d5f  y:func:`richmem_
-0000d070: 636f 6d70 7265 7373 6020 6675 6e63 7469  compress` functi
-0000d080: 6f6e 0a20 2020 2020 2020 2020 2020 202a  on.            *
-0000d090: 203a 7079 3a63 6c61 7373 3a60 5a73 7464   :py:class:`Zstd
-0000d0a0: 436f 6d70 7265 7373 6f72 6020 636c 6173  Compressor` clas
-0000d0b0: 7320 7573 696e 6720 6120 7369 6e67 6c65  s using a single
-0000d0c0: 203a 7079 3a61 7474 723a 607e 5a73 7464   :py:attr:`~Zstd
-0000d0d0: 436f 6d70 7265 7373 6f72 2e46 4c55 5348  Compressor.FLUSH
-0000d0e0: 5f46 5241 4d45 6020 6d6f 6465 0a20 2020  _FRAME` mode.   
-0000d0f0: 2020 2020 2020 2020 202a 203a 7079 3a63           * :py:c
-0000d100: 6c61 7373 3a60 5269 6368 4d65 6d5a 7374  lass:`RichMemZst
-0000d110: 6443 6f6d 7072 6573 736f 7260 2063 6c61  dCompressor` cla
-0000d120: 7373 0a20 2020 2020 2020 2020 2020 202a  ss.            *
-0000d130: 203a 7079 3a66 756e 633a 6063 6f6d 7072   :py:func:`compr
-0000d140: 6573 735f 7374 7265 616d 6020 6675 6e63  ess_stream` func
-0000d150: 7469 6f6e 2073 6574 7469 6e67 202a 706c  tion setting *pl
-0000d160: 6564 6765 645f 696e 7075 745f 7369 7a65  edged_input_size
-0000d170: 2a20 7061 7261 6d65 7465 720a 0a20 2020  * parameter..   
-0000d180: 2020 2020 2054 6865 2066 6965 6c64 2069       The field i
-0000d190: 6e20 6672 616d 6520 6865 6164 6572 2069  n frame header i
-0000d1a0: 7320 312f 322f 342f 3820 6279 7465 732c  s 1/2/4/8 bytes,
-0000d1b0: 2064 6570 656e 6469 6e67 206f 6e20 7369   depending on si
-0000d1c0: 7a65 2076 616c 7565 2e20 4974 206d 6179  ze value. It may
-0000d1d0: 2068 656c 7020 6465 636f 6d70 7265 7373   help decompress
-0000d1e0: 696f 6e20 636f 6465 2074 6f20 616c 6c6f  ion code to allo
-0000d1f0: 6361 7465 206f 7574 7075 7420 6275 6666  cate output buff
-0000d200: 6572 2066 6173 7465 722e 0a0a 2020 2020  er faster...    
-0000d210: 2020 2020 5c2a 203a 7079 3a63 6c61 7373      \* :py:class
-0000d220: 3a60 5a73 7464 436f 6d70 7265 7373 6f72  :`ZstdCompressor
-0000d230: 6020 6861 7320 616e 2075 6e64 6f63 756d  ` has an undocum
-0000d240: 656e 7465 6420 6d65 7468 6f64 2074 6f20  ented method to 
-0000d250: 7365 7420 7468 6520 7369 7a65 2c20 6060  set the size, ``
-0000d260: 6865 6c70 285a 7374 6443 6f6d 7072 6573  help(ZstdCompres
-0000d270: 736f 722e 5f73 6574 5f70 6c65 6467 6564  sor._set_pledged
-0000d280: 5f69 6e70 7574 5f73 697a 6529 6060 2074  _input_size)`` t
-0000d290: 6f20 7365 6520 7468 6520 7573 6167 652e  o see the usage.
-0000d2a0: 0a0a 2020 2020 2e2e 2070 793a 6174 7472  ..    .. py:attr
-0000d2b0: 6962 7574 653a 3a20 6368 6563 6b73 756d  ibute:: checksum
-0000d2c0: 466c 6167 0a0a 2020 2020 2020 2020 4120  Flag..        A 
-0000d2d0: 342d 6279 7465 2063 6865 636b 7375 6d20  4-byte checksum 
-0000d2e0: 6f66 2075 6e63 6f6d 7072 6573 7365 6420  of uncompressed 
-0000d2f0: 636f 6e74 656e 7420 6973 2077 7269 7474  content is writt
-0000d300: 656e 2061 7420 7468 6520 656e 6420 6f66  en at the end of
-0000d310: 2066 7261 6d65 2e0a 0a20 2020 2020 2020   frame...       
-0000d320: 2044 6566 6175 6c74 2076 616c 7565 2069   Default value i
-0000d330: 7320 6060 3060 602c 2063 616e 2062 6520  s ``0``, can be 
-0000d340: 6060 3160 602e 0a0a 2020 2020 2020 2020  ``1``...        
-0000d350: 5a73 7464 2773 2064 6563 6f6d 7072 6573  Zstd's decompres
-0000d360: 7369 6f6e 2063 6f64 6520 7665 7269 6669  sion code verifi
-0000d370: 6573 2069 742e 2049 6620 6368 6563 6b73  es it. If checks
-0000d380: 756d 206d 6973 6d61 7463 682c 2072 6169  um mismatch, rai
-0000d390: 7365 7320 6120 3a70 793a 636c 6173 733a  ses a :py:class:
-0000d3a0: 605a 7374 6445 7272 6f72 6020 6578 6365  `ZstdError` exce
-0000d3b0: 7074 696f 6e2c 2077 6974 6820 6120 6d65  ption, with a me
-0000d3c0: 7373 6167 6520 6c69 6b65 2022 5265 7374  ssage like "Rest
-0000d3d0: 6f72 6564 2064 6174 6120 646f 6573 6e27  ored data doesn'
-0000d3e0: 7420 6d61 7463 6820 6368 6563 6b73 756d  t match checksum
-0000d3f0: 222e 0a0a 2020 2020 2e2e 2070 793a 6174  "...    .. py:at
-0000d400: 7472 6962 7574 653a 3a20 6469 6374 4944  tribute:: dictID
-0000d410: 466c 6167 0a0a 2020 2020 2020 2020 5768  Flag..        Wh
-0000d420: 656e 2061 7070 6c69 6361 626c 652c 2064  en applicable, d
-0000d430: 6963 7469 6f6e 6172 7927 7320 4944 2069  ictionary's ID i
-0000d440: 7320 7772 6974 7465 6e20 696e 746f 2066  s written into f
-0000d450: 7261 6d65 2068 6561 6465 722e 2053 6565  rame header. See
-0000d460: 203a 7265 663a 6074 6869 7320 6e6f 7465   :ref:`this note
-0000d470: 3c64 6963 745f 6964 3e60 2066 6f72 2064  <dict_id>` for d
-0000d480: 6574 6169 6c73 2e0a 0a20 2020 2020 2020  etails...       
-0000d490: 2044 6566 6175 6c74 2076 616c 7565 2069   Default value i
-0000d4a0: 7320 6060 3160 602c 2063 616e 2062 6520  s ``1``, can be 
-0000d4b0: 6060 3060 602e 0a0a 2020 2020 2e2e 2070  ``0``...    .. p
-0000d4c0: 793a 6174 7472 6962 7574 653a 3a20 6e62  y:attribute:: nb
-0000d4d0: 576f 726b 6572 730a 0a20 2020 2020 2020  Workers..       
-0000d4e0: 2053 656c 6563 7420 686f 7720 6d61 6e79   Select how many
-0000d4f0: 2074 6872 6561 6473 2077 696c 6c20 6265   threads will be
-0000d500: 2073 7061 776e 6564 2074 6f20 636f 6d70   spawned to comp
-0000d510: 7265 7373 2069 6e20 7061 7261 6c6c 656c  ress in parallel
-0000d520: 2e0a 0a20 2020 2020 2020 2057 6865 6e20  ...        When 
-0000d530: 6e62 576f 726b 6572 7320 3e3d 2060 6031  nbWorkers >= ``1
-0000d540: 6060 2c20 656e 6162 6c65 7320 6d75 6c74  ``, enables mult
-0000d550: 692d 7468 7265 6164 6564 2063 6f6d 7072  i-threaded compr
-0000d560: 6573 7369 6f6e 2c20 6060 3160 6020 6d65  ession, ``1`` me
-0000d570: 616e 7320 2231 2d74 6872 6561 6420 6d75  ans "1-thread mu
-0000d580: 6c74 692d 7468 7265 6164 6564 206d 6f64  lti-threaded mod
-0000d590: 6522 2e20 5365 6520 3a72 6566 3a60 7a73  e". See :ref:`zs
-0000d5a0: 7464 206d 756c 7469 2d74 6872 6561 6465  td multi-threade
-0000d5b0: 6420 636f 6d70 7265 7373 696f 6e3c 6d74  d compression<mt
-0000d5c0: 5f63 6f6d 7072 6573 7369 6f6e 3e60 2066  _compression>` f
-0000d5d0: 6f72 2064 6574 6169 6c73 2e0a 0a20 2020  or details...   
-0000d5e0: 2020 2020 204d 6f72 6520 776f 726b 6572       More worker
-0000d5f0: 7320 696d 7072 6f76 6520 7370 6565 642c  s improve speed,
-0000d600: 2062 7574 2061 6c73 6f20 696e 6372 6561   but also increa
-0000d610: 7365 206d 656d 6f72 7920 7573 6167 652e  se memory usage.
-0000d620: 0a0a 2020 2020 2020 2020 6060 3060 6020  ..        ``0`` 
-0000d630: 2864 6566 6175 6c74 2920 6d65 616e 7320  (default) means 
-0000d640: 2273 696e 676c 652d 7468 7265 6164 6564  "single-threaded
-0000d650: 206d 6f64 6522 2c20 6e6f 2077 6f72 6b65   mode", no worke
-0000d660: 7220 6973 2073 7061 776e 6564 2c20 636f  r is spawned, co
-0000d670: 6d70 7265 7373 696f 6e20 6973 2070 6572  mpression is per
-0000d680: 666f 726d 6564 2069 6e73 6964 6520 6361  formed inside ca
-0000d690: 6c6c 6572 2773 2074 6872 6561 642e 0a0a  ller's thread...
-0000d6a0: 2020 2020 2e2e 2076 6572 7369 6f6e 6368      .. versionch
-0000d6b0: 616e 6765 643a 3a20 302e 3135 2e31 0a20  anged:: 0.15.1. 
-0000d6c0: 2020 2020 2020 2053 6574 7469 6e67 2074         Setting t
-0000d6d0: 6f20 6060 3160 6020 6d65 616e 7320 2231  o ``1`` means "1
-0000d6e0: 2d74 6872 6561 6420 6d75 6c74 692d 7468  -thread multi-th
-0000d6f0: 7265 6164 6564 206d 6f64 6522 2c20 696e  readed mode", in
-0000d700: 7374 6561 6420 6f66 2022 7369 6e67 6c65  stead of "single
-0000d710: 2d74 6872 6561 6465 6420 6d6f 6465 222e  -threaded mode".
-0000d720: 0a0a 2020 2020 2e2e 2070 793a 6174 7472  ..    .. py:attr
-0000d730: 6962 7574 653a 3a20 6a6f 6253 697a 650a  ibute:: jobSize.
-0000d740: 0a20 2020 2020 2020 2053 697a 6520 6f66  .        Size of
-0000d750: 2061 2063 6f6d 7072 6573 7369 6f6e 206a   a compression j
-0000d760: 6f62 2c20 696e 2062 7974 6573 2e0a 0a20  ob, in bytes... 
-0000d770: 2020 2020 2020 2054 6869 7320 7661 6c75         This valu
-0000d780: 6520 6973 2065 6e66 6f72 6365 6420 6f6e  e is enforced on
-0000d790: 6c79 2077 6865 6e20 3a70 793a 6174 7472  ly when :py:attr
-0000d7a0: 3a60 7e43 5061 7261 6d65 7465 722e 6e62  :`~CParameter.nb
-0000d7b0: 576f 726b 6572 7360 203e 3d20 312e 0a0a  Workers` >= 1...
-0000d7c0: 2020 2020 2020 2020 4561 6368 2063 6f6d          Each com
-0000d7d0: 7072 6573 7369 6f6e 206a 6f62 2069 7320  pression job is 
-0000d7e0: 636f 6d70 6c65 7465 6420 696e 2070 6172  completed in par
-0000d7f0: 616c 6c65 6c2c 2073 6f20 7468 6973 2076  allel, so this v
-0000d800: 616c 7565 2063 616e 2069 6e64 6972 6563  alue can indirec
-0000d810: 746c 7920 696d 7061 6374 2074 6865 206e  tly impact the n
-0000d820: 756d 6265 7220 6f66 2061 6374 6976 6520  umber of active 
-0000d830: 7468 7265 6164 732e 0a0a 2020 2020 2020  threads...      
-0000d840: 2020 6060 3060 6020 6d65 616e 7320 6465    ``0`` means de
-0000d850: 6661 756c 742c 2077 6869 6368 2069 7320  fault, which is 
-0000d860: 6479 6e61 6d69 6361 6c6c 7920 6465 7465  dynamically dete
-0000d870: 726d 696e 6564 2062 6173 6564 206f 6e20  rmined based on 
-0000d880: 636f 6d70 7265 7373 696f 6e20 7061 7261  compression para
-0000d890: 6d65 7465 7273 2e0a 0a20 2020 2020 2020  meters...       
-0000d8a0: 204e 6f6e 2d7a 6572 6f20 7661 6c75 6520   Non-zero value 
-0000d8b0: 7769 6c6c 2062 6520 7369 6c65 6e74 6c79  will be silently
-0000d8c0: 2063 6c61 6d70 6564 2074 6f3a 0a0a 2020   clamped to:..  
-0000d8d0: 2020 2020 2020 2a20 6d69 6e69 6d75 6d20        * minimum 
-0000d8e0: 7661 6c75 653a 2060 606d 6178 286f 7665  value: ``max(ove
-0000d8f0: 726c 6170 5f73 697a 652c 2035 3132 5f4b  rlap_size, 512_K
-0000d900: 6942 2960 602e 206f 7665 726c 6170 5f73  iB)``. overlap_s
-0000d910: 697a 6520 6973 2073 7065 6369 6669 6564  ize is specified
-0000d920: 2062 7920 3a70 793a 6174 7472 3a60 7e43   by :py:attr:`~C
-0000d930: 5061 7261 6d65 7465 722e 6f76 6572 6c61  Parameter.overla
-0000d940: 704c 6f67 6020 7061 7261 6d65 7465 722e  pLog` parameter.
-0000d950: 0a20 2020 2020 2020 202a 206d 6178 696d  .        * maxim
-0000d960: 756d 2076 616c 7565 3a20 6060 3531 325f  um value: ``512_
-0000d970: 4d69 4220 6966 2033 325f 6269 745f 6275  MiB if 32_bit_bu
-0000d980: 696c 6420 656c 7365 2031 3032 345f 4d69  ild else 1024_Mi
-0000d990: 4260 602e 0a0a 2020 2020 2e2e 2070 793a  B``...    .. py:
-0000d9a0: 6174 7472 6962 7574 653a 3a20 6f76 6572  attribute:: over
-0000d9b0: 6c61 704c 6f67 0a0a 2020 2020 2020 2020  lapLog..        
-0000d9c0: 436f 6e74 726f 6c20 7468 6520 6f76 6572  Control the over
-0000d9d0: 6c61 7020 7369 7a65 2c20 6173 2061 2066  lap size, as a f
-0000d9e0: 7261 6374 696f 6e20 6f66 2077 696e 646f  raction of windo
-0000d9f0: 7720 7369 7a65 2e20 2854 6865 2022 7769  w size. (The "wi
-0000da00: 6e64 6f77 2073 697a 6522 2068 6572 6520  ndow size" here 
-0000da10: 6973 206e 6f74 2073 7472 6963 7420 3a70  is not strict :p
-0000da20: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
-0000da30: 7465 722e 7769 6e64 6f77 4c6f 6760 2c20  ter.windowLog`, 
-0000da40: 7365 6520 7a73 7464 2073 6f75 7263 6520  see zstd source 
-0000da50: 636f 6465 2e29 0a0a 2020 2020 2020 2020  code.)..        
-0000da60: 5468 6973 2076 616c 7565 2069 7320 656e  This value is en
-0000da70: 666f 7263 6564 206f 6e6c 7920 7768 656e  forced only when
-0000da80: 203a 7079 3a61 7474 723a 607e 4350 6172   :py:attr:`~CPar
-0000da90: 616d 6574 6572 2e6e 6257 6f72 6b65 7273  ameter.nbWorkers
-0000daa0: 6020 3e3d 2031 2e0a 0a20 2020 2020 2020  ` >= 1...       
-0000dab0: 2054 6865 206f 7665 726c 6170 2073 697a   The overlap siz
-0000dac0: 6520 6973 2061 6e20 616d 6f75 6e74 206f  e is an amount o
-0000dad0: 6620 6461 7461 2072 656c 6f61 6465 6420  f data reloaded 
-0000dae0: 6672 6f6d 2070 7265 7669 6f75 7320 6a6f  from previous jo
-0000daf0: 6220 6174 2074 6865 2062 6567 696e 6e69  b at the beginni
-0000db00: 6e67 206f 6620 6120 6e65 7720 6a6f 622e  ng of a new job.
-0000db10: 2049 7420 6865 6c70 7320 7072 6573 6572   It helps preser
-0000db20: 7665 2063 6f6d 7072 6573 7369 6f6e 2072  ve compression r
-0000db30: 6174 696f 2c20 7768 696c 6520 6561 6368  atio, while each
-0000db40: 206a 6f62 2069 7320 636f 6d70 7265 7373   job is compress
-0000db50: 6564 2069 6e20 7061 7261 6c6c 656c 2e20  ed in parallel. 
-0000db60: 4c61 7267 6572 2076 616c 7565 7320 696e  Larger values in
-0000db70: 6372 6561 7365 2063 6f6d 7072 6573 7369  crease compressi
-0000db80: 6f6e 2072 6174 696f 2c20 6275 7420 6465  on ratio, but de
-0000db90: 6372 6561 7365 2073 7065 6564 2e0a 0a20  crease speed... 
-0000dba0: 2020 2020 2020 2050 6f73 7369 626c 6520         Possible 
-0000dbb0: 7661 6c75 6573 2072 616e 6765 2066 726f  values range fro
-0000dbc0: 6d20 3020 746f 2039 3a0a 0a20 2020 2020  m 0 to 9:..     
-0000dbd0: 2020 202d 2030 206d 6561 6e73 2022 6465     - 0 means "de
-0000dbe0: 6661 756c 7422 203a 2054 6865 2076 616c  fault" : The val
-0000dbf0: 7565 2077 696c 6c20 6265 2064 6574 6572  ue will be deter
-0000dc00: 6d69 6e65 6420 6279 2074 6865 206c 6962  mined by the lib
-0000dc10: 7261 7279 2e20 5468 6520 7661 6c75 6520  rary. The value 
-0000dc20: 7661 7269 6573 2062 6574 7765 656e 2036  varies between 6
-0000dc30: 2061 6e64 2039 2c20 6465 7065 6e64 696e   and 9, dependin
-0000dc40: 6720 6f6e 203a 7079 3a61 7474 723a 607e  g on :py:attr:`~
-0000dc50: 4350 6172 616d 6574 6572 2e73 7472 6174  CParameter.strat
-0000dc60: 6567 7960 2e0a 2020 2020 2020 2020 2d20  egy`..        - 
-0000dc70: 3120 6d65 616e 7320 226e 6f20 6f76 6572  1 means "no over
-0000dc80: 6c61 7022 0a20 2020 2020 2020 202d 2039  lap".        - 9
-0000dc90: 206d 6561 6e73 2022 6675 6c6c 206f 7665   means "full ove
-0000dca0: 726c 6170 222c 2075 7369 6e67 2061 2066  rlap", using a f
-0000dcb0: 756c 6c20 7769 6e64 6f77 2073 697a 652e  ull window size.
-0000dcc0: 0a0a 2020 2020 2020 2020 4561 6368 2069  ..        Each i
-0000dcd0: 6e74 6572 6d65 6469 6174 6520 7261 6e6b  ntermediate rank
-0000dce0: 2069 6e63 7265 6173 6573 2f64 6563 7265   increases/decre
-0000dcf0: 6173 6573 206c 6f61 6420 7369 7a65 2062  ases load size b
-0000dd00: 7920 6120 6661 6374 6f72 2032 3a0a 0a20  y a factor 2:.. 
-0000dd10: 2020 2020 2020 2039 3a20 6675 6c6c 2077         9: full w
-0000dd20: 696e 646f 773b 2020 383a 2077 2f32 3b20  indow;  8: w/2; 
-0000dd30: 2037 3a20 772f 343b 2020 363a 2077 2f38   7: w/4;  6: w/8
-0000dd40: 3b20 2035 3a20 772f 3136 3b20 2034 3a20  ;  5: w/16;  4: 
-0000dd50: 772f 3332 3b20 2033 3a20 772f 3634 3b20  w/32;  3: w/64; 
-0000dd60: 2032 3a20 772f 3132 383b 2020 313a 206e   2: w/128;  1: n
-0000dd70: 6f20 6f76 6572 6c61 703b 2020 303a 2064  o overlap;  0: d
-0000dd80: 6566 6175 6c74 2e0a 0a0a 2e2e 205f 4450  efault...... _DP
-0000dd90: 6172 616d 6574 6572 3a0a 0a2e 2e20 7079  arameter:.... py
-0000dda0: 3a63 6c61 7373 3a3a 2044 5061 7261 6d65  :class:: DParame
-0000ddb0: 7465 7228 496e 7445 6e75 6d29 0a0a 2020  ter(IntEnum)..  
-0000ddc0: 2020 4164 7661 6e63 6564 2064 6563 6f6d    Advanced decom
-0000ddd0: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
-0000dde0: 6572 732e 0a0a 2020 2020 5768 656e 2075  ers...    When u
-0000ddf0: 7369 6e67 2c20 7075 7420 7468 6520 7061  sing, put the pa
-0000de00: 7261 6d65 7465 7273 2069 6e20 6120 6060  rameters in a ``
-0000de10: 6469 6374 6060 206f 626a 6563 742c 2074  dict`` object, t
-0000de20: 6865 206b 6579 2069 7320 6120 3a70 793a  he key is a :py:
-0000de30: 636c 6173 733a 6044 5061 7261 6d65 7465  class:`DParamete
-0000de40: 7260 206e 616d 652c 2074 6865 2076 616c  r` name, the val
-0000de50: 7565 2069 7320 6120 3332 2d62 6974 2073  ue is a 32-bit s
-0000de60: 6967 6e65 6420 696e 7465 6765 7220 7661  igned integer va
-0000de70: 6c75 652e 0a0a 2020 2020 2e2e 2073 6f75  lue...    .. sou
-0000de80: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
-0000de90: 0a0a 2020 2020 2020 2020 2320 7365 7420  ..        # set 
-0000dea0: 6d65 6d6f 7279 2061 6c6c 6f63 6174 696f  memory allocatio
-0000deb0: 6e20 6c69 6d69 7420 746f 2031 3620 4d69  n limit to 16 Mi
-0000dec0: 4220 2831 203c 3c20 3234 290a 2020 2020  B (1 << 24).    
-0000ded0: 2020 2020 6f70 7469 6f6e 203d 207b 4450      option = {DP
-0000dee0: 6172 616d 6574 6572 2e77 696e 646f 774c  arameter.windowL
-0000def0: 6f67 4d61 7820 3a20 3234 7d0a 0a20 2020  ogMax : 24}..   
-0000df00: 2020 2020 2023 2075 7365 6420 7769 7468       # used with
-0000df10: 2064 6563 6f6d 7072 6573 7328 2920 6675   decompress() fu
-0000df20: 6e63 7469 6f6e 0a20 2020 2020 2020 2064  nction.        d
-0000df30: 6563 6f6d 7072 6573 7365 645f 6461 7420  ecompressed_dat 
-0000df40: 3d20 6465 636f 6d70 7265 7373 2864 6174  = decompress(dat
-0000df50: 2c20 6f70 7469 6f6e 3d6f 7074 696f 6e29  , option=option)
-0000df60: 0a0a 2020 2020 2020 2020 2320 7573 6564  ..        # used
-0000df70: 2077 6974 6820 5a73 7464 4465 636f 6d70   with ZstdDecomp
-0000df80: 7265 7373 6f72 206f 626a 6563 740a 2020  ressor object.  
-0000df90: 2020 2020 2020 6420 3d20 5a73 7464 4465        d = ZstdDe
-0000dfa0: 636f 6d70 7265 7373 6f72 286f 7074 696f  compressor(optio
-0000dfb0: 6e3d 6f70 7469 6f6e 290a 2020 2020 2020  n=option).      
-0000dfc0: 2020 6465 636f 6d70 7265 7373 6564 5f64    decompressed_d
-0000dfd0: 6174 203d 2064 2e64 6563 6f6d 7072 6573  at = d.decompres
-0000dfe0: 7328 6461 7429 0a0a 2020 2020 5061 7261  s(dat)..    Para
-0000dff0: 6d65 7465 7220 7661 6c75 6520 7368 6f75  meter value shou
-0000e000: 6c64 2062 656c 6f6e 6720 746f 2061 6e20  ld belong to an 
-0000e010: 696e 7465 7276 616c 2077 6974 6820 6c6f  interval with lo
-0000e020: 7765 7220 616e 6420 7570 7065 7220 626f  wer and upper bo
-0000e030: 756e 6473 2c20 6f74 6865 7277 6973 6520  unds, otherwise 
-0000e040: 7468 6579 2077 696c 6c20 6569 7468 6572  they will either
-0000e050: 2074 7269 6767 6572 2061 6e20 6572 726f   trigger an erro
-0000e060: 7220 6f72 2062 6520 636c 616d 7065 6420  r or be clamped 
-0000e070: 7369 6c65 6e74 6c79 2e0a 0a20 2020 2054  silently...    T
-0000e080: 6865 2063 6f6e 7374 616e 7420 7661 6c75  he constant valu
-0000e090: 6573 206d 656e 7469 6f6e 6564 2062 656c  es mentioned bel
-0000e0a0: 6f77 2061 7265 2064 6566 696e 6564 2069  ow are defined i
-0000e0b0: 6e20 607a 7374 642e 6820 3c68 7474 7073  n `zstd.h <https
-0000e0c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
-0000e0d0: 6365 626f 6f6b 2f7a 7374 642f 626c 6f62  cebook/zstd/blob
-0000e0e0: 2f72 656c 6561 7365 2f6c 6962 2f7a 7374  /release/lib/zst
-0000e0f0: 642e 683e 605f 2c20 6e6f 7465 2074 6861  d.h>`_, note tha
-0000e100: 7420 7468 6573 6520 7661 6c75 6573 206d  t these values m
-0000e110: 6179 2062 6520 6469 6666 6572 656e 7420  ay be different 
-0000e120: 696e 2064 6966 6665 7265 6e74 207a 7374  in different zst
-0000e130: 6420 7665 7273 696f 6e73 2e0a 0a20 2020  d versions...   
-0000e140: 202e 2e20 7079 3a6d 6574 686f 643a 3a20   .. py:method:: 
-0000e150: 626f 756e 6473 2873 656c 6629 0a0a 2020  bounds(self)..  
-0000e160: 2020 2020 2020 5265 7475 726e 206c 6f77        Return low
-0000e170: 6572 2061 6e64 2075 7070 6572 2062 6f75  er and upper bou
-0000e180: 6e64 7320 6f66 2061 2070 6172 616d 6574  nds of a paramet
-0000e190: 6572 2c20 626f 7468 2069 6e63 6c75 7369  er, both inclusi
-0000e1a0: 7665 2e0a 0a20 2020 2020 2020 202e 2e20  ve...        .. 
-0000e1b0: 736f 7572 6365 636f 6465 3a3a 2070 7974  sourcecode:: pyt
-0000e1c0: 686f 6e0a 0a20 2020 2020 2020 2020 2020  hon..           
-0000e1d0: 203e 3e3e 2044 5061 7261 6d65 7465 722e   >>> DParameter.
-0000e1e0: 7769 6e64 6f77 4c6f 674d 6178 2e62 6f75  windowLogMax.bou
-0000e1f0: 6e64 7328 290a 2020 2020 2020 2020 2020  nds().          
-0000e200: 2020 2831 302c 2033 3129 0a0a 2020 2020    (10, 31)..    
-0000e210: 2e2e 2070 793a 6174 7472 6962 7574 653a  .. py:attribute:
-0000e220: 3a20 7769 6e64 6f77 4c6f 674d 6178 0a0a  : windowLogMax..
-0000e230: 2020 2020 2020 2020 5365 6c65 6374 2061          Select a
-0000e240: 2073 697a 6520 6c69 6d69 7420 2869 6e20   size limit (in 
-0000e250: 706f 7765 7220 6f66 2032 2920 6265 796f  power of 2) beyo
-0000e260: 6e64 2077 6869 6368 2074 6865 2073 7472  nd which the str
-0000e270: 6561 6d69 6e67 2041 5049 2077 696c 6c20  eaming API will 
-0000e280: 7265 6675 7365 2074 6f20 616c 6c6f 6361  refuse to alloca
-0000e290: 7465 206d 656d 6f72 7920 6275 6666 6572  te memory buffer
-0000e2a0: 2069 6e20 6f72 6465 7220 746f 2070 726f   in order to pro
-0000e2b0: 7465 6374 2074 6865 2068 6f73 7420 6672  tect the host fr
-0000e2c0: 6f6d 2075 6e72 6561 736f 6e61 626c 6520  om unreasonable 
-0000e2d0: 6d65 6d6f 7279 2072 6571 7569 7265 6d65  memory requireme
-0000e2e0: 6e74 732e 0a0a 2020 2020 2020 2020 4966  nts...        If
-0000e2f0: 2061 203a 7265 663a 6066 7261 6d65 3c66   a :ref:`frame<f
-0000e300: 7261 6d65 5f62 6c6f 636b 3e60 2072 6571  rame_block>` req
-0000e310: 7569 7265 7320 6d6f 7265 206d 656d 6f72  uires more memor
-0000e320: 7920 7468 616e 2074 6865 2073 6574 2076  y than the set v
-0000e330: 616c 7565 2c20 7261 6973 6573 2061 203a  alue, raises a :
-0000e340: 7079 3a63 6c61 7373 3a60 5a73 7464 4572  py:class:`ZstdEr
-0000e350: 726f 7260 2065 7863 6570 7469 6f6e 2c20  ror` exception, 
-0000e360: 7769 7468 2061 206d 6573 7361 6765 206c  with a message l
-0000e370: 696b 6520 2246 7261 6d65 2072 6571 7569  ike "Frame requi
-0000e380: 7265 7320 746f 6f20 6d75 6368 206d 656d  res too much mem
-0000e390: 6f72 7920 666f 7220 6465 636f 6469 6e67  ory for decoding
-0000e3a0: 222e 0a0a 2020 2020 2020 2020 5468 6973  "...        This
-0000e3b0: 2070 6172 616d 6574 6572 2069 7320 6f6e   parameter is on
-0000e3c0: 6c79 2075 7365 6675 6c20 696e 2073 7472  ly useful in str
-0000e3d0: 6561 6d69 6e67 206d 6f64 652c 2073 696e  eaming mode, sin
-0000e3e0: 6365 206e 6f20 696e 7465 726e 616c 2062  ce no internal b
-0000e3f0: 7566 6665 7220 6973 2061 6c6c 6f63 6174  uffer is allocat
-0000e400: 6564 2069 6e20 7369 6e67 6c65 2d70 6173  ed in single-pas
-0000e410: 7320 6d6f 6465 2e20 3a70 793a 6675 6e63  s mode. :py:func
-0000e420: 3a60 6465 636f 6d70 7265 7373 6020 6675  :`decompress` fu
-0000e430: 6e63 7469 6f6e 206d 6179 2075 7365 2073  nction may use s
-0000e440: 7472 6561 6d69 6e67 206d 6f64 6520 6f72  treaming mode or
-0000e450: 2073 696e 676c 652d 7061 7373 206d 6f64   single-pass mod
-0000e460: 652e 0a0a 2020 2020 2020 2020 4279 2064  e...        By d
-0000e470: 6566 6175 6c74 2c20 6120 6465 636f 6d70  efault, a decomp
-0000e480: 7265 7373 696f 6e20 636f 6e74 6578 7420  ression context 
-0000e490: 6163 6365 7074 7320 7769 6e64 6f77 2073  accepts window s
-0000e4a0: 697a 6573 203c 3d20 6060 2831 203c 3c20  izes <= ``(1 << 
-0000e4b0: 5a53 5444 5f57 494e 444f 574c 4f47 5f4c  ZSTD_WINDOWLOG_L
-0000e4c0: 494d 4954 5f44 4546 4155 4c54 2960 602c  IMIT_DEFAULT)``,
-0000e4d0: 2074 6865 2063 6f6e 7374 616e 7420 6973   the constant is
-0000e4e0: 2060 6032 3760 6020 696e 207a 7374 6420   ``27`` in zstd 
-0000e4f0: 7631 2e32 2b2c 206d 6561 6e73 2031 3238  v1.2+, means 128
-0000e500: 204d 6942 2028 3120 3c3c 2032 3729 2e20   MiB (1 << 27). 
-0000e510: 4966 2066 7261 6d65 2072 6571 7565 7374  If frame request
-0000e520: 6564 2077 696e 646f 7720 7369 7a65 2069  ed window size i
-0000e530: 7320 6772 6561 7465 7220 7468 616e 2074  s greater than t
-0000e540: 6869 7320 7661 6c75 652c 206e 6565 6420  his value, need 
-0000e550: 746f 2065 7870 6c69 6369 746c 7920 7365  to explicitly se
-0000e560: 7420 7468 6973 2070 6172 616d 6574 6572  t this parameter
-0000e570: 2e0a 0a20 2020 2020 2020 2053 7065 6369  ...        Speci
-0000e580: 616c 3a20 7661 6c75 6520 6060 3060 6020  al: value ``0`` 
-0000e590: 6d65 616e 7320 2275 7365 2064 6566 6175  means "use defau
-0000e5a0: 6c74 206d 6178 696d 756d 2077 696e 646f  lt maximum windo
-0000e5b0: 774c 6f67 222e 0a0a 0a2e 2e20 7079 3a63  wLog"...... py:c
-0000e5c0: 6c61 7373 3a3a 2053 7472 6174 6567 7928  lass:: Strategy(
-0000e5d0: 496e 7445 6e75 6d29 0a0a 2020 2020 5573  IntEnum)..    Us
-0000e5e0: 6564 2066 6f72 203a 7079 3a61 7474 723a  ed for :py:attr:
-0000e5f0: 6043 5061 7261 6d65 7465 722e 7374 7261  `CParameter.stra
-0000e600: 7465 6779 602e 0a0a 2020 2020 436f 6d70  tegy`...    Comp
-0000e610: 7265 7373 696f 6e20 7374 7261 7465 6769  ression strategi
-0000e620: 6573 2c20 6c69 7374 6564 2066 726f 6d20  es, listed from 
-0000e630: 6661 7374 6573 7420 746f 2073 7472 6f6e  fastest to stron
-0000e640: 6765 7374 2e0a 0a20 2020 204e 6f74 6520  gest...    Note 
-0000e650: 3a20 6e65 7720 7374 7261 7465 6769 6573  : new strategies
-0000e660: 202a 2a6d 6967 6874 2a2a 2062 6520 6164   **might** be ad
-0000e670: 6465 6420 696e 2074 6865 2066 7574 7572  ded in the futur
-0000e680: 652c 206f 6e6c 7920 7468 6520 6f72 6465  e, only the orde
-0000e690: 7220 2866 726f 6d20 6661 7374 2074 6f20  r (from fast to 
-0000e6a0: 7374 726f 6e67 2920 6973 2067 7561 7261  strong) is guara
-0000e6b0: 6e74 6565 642e 0a0a 2020 2020 2e2e 2070  nteed...    .. p
-0000e6c0: 793a 6174 7472 6962 7574 653a 3a20 6661  y:attribute:: fa
-0000e6d0: 7374 0a20 2020 202e 2e20 7079 3a61 7474  st.    .. py:att
-0000e6e0: 7269 6275 7465 3a3a 2064 6661 7374 0a20  ribute:: dfast. 
-0000e6f0: 2020 202e 2e20 7079 3a61 7474 7269 6275     .. py:attribu
-0000e700: 7465 3a3a 2067 7265 6564 790a 2020 2020  te:: greedy.    
-0000e710: 2e2e 2070 793a 6174 7472 6962 7574 653a  .. py:attribute:
-0000e720: 3a20 6c61 7a79 0a20 2020 202e 2e20 7079  : lazy.    .. py
-0000e730: 3a61 7474 7269 6275 7465 3a3a 206c 617a  :attribute:: laz
-0000e740: 7932 0a20 2020 202e 2e20 7079 3a61 7474  y2.    .. py:att
-0000e750: 7269 6275 7465 3a3a 2062 746c 617a 7932  ribute:: btlazy2
-0000e760: 0a20 2020 202e 2e20 7079 3a61 7474 7269  .    .. py:attri
-0000e770: 6275 7465 3a3a 2062 746f 7074 0a20 2020  bute:: btopt.   
-0000e780: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
-0000e790: 3a3a 2062 7475 6c74 7261 0a20 2020 202e  :: btultra.    .
-0000e7a0: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
-0000e7b0: 2062 7475 6c74 7261 320a 0a20 2020 202e   btultra2..    .
-0000e7c0: 2e20 736f 7572 6365 636f 6465 3a3a 2070  . sourcecode:: p
-0000e7d0: 7974 686f 6e0a 0a20 2020 2020 2020 206f  ython..        o
-0000e7e0: 7074 696f 6e20 3d20 7b43 5061 7261 6d65  ption = {CParame
-0000e7f0: 7465 722e 7374 7261 7465 6779 203a 2053  ter.strategy : S
-0000e800: 7472 6174 6567 792e 6c61 7a79 322c 0a20  trategy.lazy2,. 
-0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e820: 2043 5061 7261 6d65 7465 722e 6368 6563   CParameter.chec
-0000e830: 6b73 756d 466c 6167 203a 2031 7d0a 2020  ksumFlag : 1}.  
-0000e840: 2020 2020 2020 636f 6d70 7265 7373 6564        compressed
-0000e850: 5f64 6174 203d 2063 6f6d 7072 6573 7328  _dat = compress(
-0000e860: 7261 775f 6461 742c 206f 7074 696f 6e29  raw_dat, option)
-0000e870: 0a0a 0a49 6e66 6f72 6d61 7469 7665 206e  ...Informative n
-0000e880: 6f74 6573 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  otes.-----------
-0000e890: 2d2d 2d2d 2d2d 0a0a 436f 6d70 7265 7373  ------..Compress
-0000e8a0: 696f 6e20 6c65 7665 6c0a 3e3e 3e3e 3e3e  ion level.>>>>>>
-0000e8b0: 3e3e 3e3e 3e3e 3e3e 3e3e 3e0a 0a2e 2e20  >>>>>>>>>>>.... 
-0000e8c0: 5f63 6f6d 7072 6573 7369 6f6e 5f6c 6576  _compression_lev
-0000e8d0: 656c 3a0a 0a2e 2e20 6e6f 7465 3a3a 2043  el:.... note:: C
-0000e8e0: 6f6d 7072 6573 7369 6f6e 206c 6576 656c  ompression level
-0000e8f0: 0a0a 2020 2020 436f 6d70 7265 7373 696f  ..    Compressio
-0000e900: 6e20 6c65 7665 6c20 6973 2061 6e20 696e  n level is an in
-0000e910: 7465 6765 723a 0a0a 2020 2020 2a20 6060  teger:..    * ``
-0000e920: 3160 6020 746f 2060 6032 3260 6020 2863  1`` to ``22`` (c
-0000e930: 7572 7265 6e74 6c79 292c 2072 6567 756c  urrently), regul
-0000e940: 6172 206c 6576 656c 732e 204c 6576 656c  ar levels. Level
-0000e950: 7320 3e3d 2032 302c 206c 6162 656c 6564  s >= 20, labeled
-0000e960: 202a 756c 7472 612a 2c20 7368 6f75 6c64   *ultra*, should
-0000e970: 2062 6520 7573 6564 2077 6974 6820 6361   be used with ca
-0000e980: 7574 696f 6e2c 2061 7320 7468 6579 2072  ution, as they r
-0000e990: 6571 7569 7265 206d 6f72 6520 6d65 6d6f  equire more memo
-0000e9a0: 7279 2e0a 2020 2020 2a20 6060 3060 6020  ry..    * ``0`` 
-0000e9b0: 6d65 616e 7320 7573 6520 7468 6520 6465  means use the de
-0000e9c0: 6661 756c 7420 6c65 7665 6c2c 2077 6869  fault level, whi
-0000e9d0: 6368 2069 7320 6375 7272 656e 746c 7920  ch is currently 
-0000e9e0: 6060 3360 6020 6465 6669 6e65 6420 6279  ``3`` defined by
-0000e9f0: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-0000ea00: 7a73 7464 206c 6962 7261 7279 2e0a 2020  zstd library..  
-0000ea10: 2020 2a20 6060 2d31 3331 3037 3260 6020    * ``-131072`` 
-0000ea20: 746f 2060 602d 3160 602c 206e 6567 6174  to ``-1``, negat
-0000ea30: 6976 6520 6c65 7665 6c73 2065 7874 656e  ive levels exten
-0000ea40: 6420 7468 6520 7261 6e67 6520 6f66 2073  d the range of s
-0000ea50: 7065 6564 2076 7320 7261 7469 6f20 7072  peed vs ratio pr
-0000ea60: 6566 6572 656e 6365 732e 2054 6865 206c  eferences. The l
-0000ea70: 6f77 6572 2074 6865 206c 6576 656c 2c20  ower the level, 
-0000ea80: 7468 6520 6661 7374 6572 2074 6865 2073  the faster the s
-0000ea90: 7065 6564 2c20 6275 7420 6174 2074 6865  peed, but at the
-0000eaa0: 2063 6f73 7420 6f66 2063 6f6d 7072 6573   cost of compres
-0000eab0: 7369 6f6e 2072 6174 696f 2e20 3133 3130  sion ratio. 1310
-0000eac0: 3732 203d 2031 3238 2a31 3032 342e 0a0a  72 = 128*1024...
-0000ead0: 2020 2020 3a70 793a 6461 7461 3a60 636f      :py:data:`co
-0000eae0: 6d70 7265 7373 696f 6e4c 6576 656c 5f76  mpressionLevel_v
-0000eaf0: 616c 7565 7360 2061 7265 2073 6f6d 6520  alues` are some 
-0000eb00: 7661 6c75 6573 2064 6566 696e 6564 2062  values defined b
-0000eb10: 7920 7468 6520 756e 6465 726c 7969 6e67  y the underlying
-0000eb20: 207a 7374 6420 6c69 6272 6172 792e 0a0a   zstd library...
-0000eb30: 2020 2020 2a2a 466f 7220 6164 7661 6e63      **For advanc
-0000eb40: 6564 2075 7365 722a 2a0a 0a20 2020 2043  ed user**..    C
-0000eb50: 6f6d 7072 6573 7369 6f6e 206c 6576 656c  ompression level
-0000eb60: 7320 6172 6520 6a75 7374 206e 756d 6265  s are just numbe
-0000eb70: 7273 2074 6861 7420 6d61 7020 746f 2061  rs that map to a
-0000eb80: 2073 6574 206f 6620 636f 6d70 7265 7373   set of compress
-0000eb90: 696f 6e20 7061 7261 6d65 7465 7273 2c20  ion parameters, 
-0000eba0: 7365 6520 6074 6869 7320 7461 626c 6520  see `this table 
-0000ebb0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-0000ebc0: 636f 6d2f 6661 6365 626f 6f6b 2f7a 7374  com/facebook/zst
-0000ebd0: 642f 626c 6f62 2f72 656c 6561 7365 2f6c  d/blob/release/l
-0000ebe0: 6962 2f63 6f6d 7072 6573 732f 636c 6576  ib/compress/clev
-0000ebf0: 656c 732e 683e 605f 2066 6f72 206f 7665  els.h>`_ for ove
-0000ec00: 7276 6965 772e 2054 6865 2070 6172 616d  rview. The param
-0000ec10: 6574 6572 7320 6d61 7920 6265 2061 646a  eters may be adj
-0000ec20: 7573 7465 6420 6279 2074 6865 2075 6e64  usted by the und
-0000ec30: 6572 6c79 696e 6720 7a73 7464 206c 6962  erlying zstd lib
-0000ec40: 7261 7279 2061 6674 6572 2067 6174 6865  rary after gathe
-0000ec50: 7269 6e67 2073 6f6d 6520 696e 666f 726d  ring some inform
-0000ec60: 6174 696f 6e2c 2073 7563 6820 6173 2064  ation, such as d
-0000ec70: 6174 6120 7369 7a65 2c20 7573 696e 6720  ata size, using 
-0000ec80: 6469 6374 696f 6e61 7279 206f 7220 6e6f  dictionary or no
-0000ec90: 742e 0a0a 2020 2020 5365 7474 696e 6720  t...    Setting 
-0000eca0: 6120 636f 6d70 7265 7373 696f 6e20 6c65  a compression le
-0000ecb0: 7665 6c20 646f 6573 206e 6f74 2073 6574  vel does not set
-0000ecc0: 2061 6c6c 206f 7468 6572 203a 7265 663a   all other :ref:
-0000ecd0: 6063 6f6d 7072 6573 7369 6f6e 2070 6172  `compression par
-0000ece0: 616d 6574 6572 733c 4350 6172 616d 6574  ameters<CParamet
-0000ecf0: 6572 3e60 2074 6f20 6465 6661 756c 742e  er>` to default.
-0000ed00: 2053 6574 7469 6e67 2074 6869 7320 7769   Setting this wi
-0000ed10: 6c6c 2064 796e 616d 6963 616c 6c79 2069  ll dynamically i
-0000ed20: 6d70 6163 7420 7468 6520 636f 6d70 7265  mpact the compre
-0000ed30: 7373 696f 6e20 7061 7261 6d65 7465 7273  ssion parameters
-0000ed40: 2077 6869 6368 2068 6176 6520 6e6f 7420   which have not 
-0000ed50: 6265 656e 206d 616e 7561 6c6c 7920 7365  been manually se
-0000ed60: 742c 2074 6865 206d 616e 7561 6c6c 7920  t, the manually 
-0000ed70: 7365 7420 6f6e 6573 2077 696c 6c20 2273  set ones will "s
-0000ed80: 7469 636b 222e 0a0a 0a46 7261 6d65 2061  tick"....Frame a
-0000ed90: 6e64 2062 6c6f 636b 0a3e 3e3e 3e3e 3e3e  nd block.>>>>>>>
-0000eda0: 3e3e 3e3e 3e3e 3e3e 0a0a 2e2e 205f 6672  >>>>>>>>.... _fr
-0000edb0: 616d 655f 626c 6f63 6b3a 0a0a 2e2e 206e  ame_block:.... n
-0000edc0: 6f74 653a 3a20 4672 616d 6520 616e 6420  ote:: Frame and 
-0000edd0: 626c 6f63 6b0a 0a20 2020 202a 2a46 7261  block..    **Fra
-0000ede0: 6d65 2a2a 0a0a 2020 2020 5a73 7464 2064  me**..    Zstd d
-0000edf0: 6174 6120 636f 6e73 6973 7473 206f 6620  ata consists of 
-0000ee00: 6f6e 6520 6f72 206d 6f72 6520 696e 6465  one or more inde
-0000ee10: 7065 6e64 656e 7420 2266 7261 6d65 7322  pendent "frames"
-0000ee20: 2e20 5468 6520 6465 636f 6d70 7265 7373  . The decompress
-0000ee30: 6564 2063 6f6e 7465 6e74 206f 6620 6d75  ed content of mu
-0000ee40: 6c74 6970 6c65 2063 6f6e 6361 7465 6e61  ltiple concatena
-0000ee50: 7465 6420 6672 616d 6573 2069 7320 7468  ted frames is th
-0000ee60: 6520 636f 6e63 6174 656e 6174 696f 6e20  e concatenation 
-0000ee70: 6f66 2065 6163 6820 6672 616d 6520 6465  of each frame de
-0000ee80: 636f 6d70 7265 7373 6564 2063 6f6e 7465  compressed conte
-0000ee90: 6e74 2e0a 0a20 2020 2041 2066 7261 6d65  nt...    A frame
-0000eea0: 2069 7320 636f 6d70 6c65 7465 6c79 2069   is completely i
-0000eeb0: 6e64 6570 656e 6465 6e74 2c20 6861 7320  ndependent, has 
-0000eec0: 6120 6672 616d 6520 6865 6164 6572 2c20  a frame header, 
-0000eed0: 616e 6420 6120 7365 7420 6f66 2070 6172  and a set of par
-0000eee0: 616d 6574 6572 7320 7768 6963 6820 7465  ameters which te
-0000eef0: 6c6c 7320 7468 6520 6465 636f 6465 7220  lls the decoder 
-0000ef00: 686f 7720 746f 2064 6563 6f6d 7072 6573  how to decompres
-0000ef10: 7320 6974 2e0a 0a20 2020 2049 6e20 6164  s it...    In ad
-0000ef20: 6469 7469 6f6e 2074 6f20 6e6f 726d 616c  dition to normal
-0000ef30: 2066 7261 6d65 2c20 7468 6572 6520 6973   frame, there is
-0000ef40: 2060 736b 6970 7061 626c 6520 6672 616d   `skippable fram
-0000ef50: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
-0000ef60: 622e 636f 6d2f 6661 6365 626f 6f6b 2f7a  b.com/facebook/z
-0000ef70: 7374 642f 626c 6f62 2f72 656c 6561 7365  std/blob/release
-0000ef80: 2f64 6f63 2f7a 7374 645f 636f 6d70 7265  /doc/zstd_compre
-0000ef90: 7373 696f 6e5f 666f 726d 6174 2e6d 6423  ssion_format.md#
-0000efa0: 736b 6970 7061 626c 652d 6672 616d 6573  skippable-frames
-0000efb0: 3e60 5f20 7468 6174 2063 616e 2063 6f6e  >`_ that can con
-0000efc0: 7461 696e 2061 6e79 2075 7365 722d 6465  tain any user-de
-0000efd0: 6669 6e65 6420 6461 7461 2c20 736b 6970  fined data, skip
-0000efe0: 7061 626c 6520 6672 616d 6520 7769 6c6c  pable frame will
-0000eff0: 2062 6520 6465 636f 6d70 7265 7373 6564   be decompressed
-0000f000: 2074 6f20 6060 6227 2760 602e 0a0a 2020   to ``b''``...  
-0000f010: 2020 2a2a 426c 6f63 6b2a 2a0a 0a20 2020    **Block**..   
-0000f020: 2041 2066 7261 6d65 2065 6e63 6170 7375   A frame encapsu
-0000f030: 6c61 7465 7320 6f6e 6520 6f72 206d 756c  lates one or mul
-0000f040: 7469 706c 6520 2262 6c6f 636b 7322 2e20  tiple "blocks". 
-0000f050: 426c 6f63 6b20 6861 7320 6120 6775 6172  Block has a guar
-0000f060: 616e 7465 6564 206d 6178 696d 756d 2073  anteed maximum s
-0000f070: 697a 6520 2833 2062 7974 6573 2062 6c6f  ize (3 bytes blo
-0000f080: 636b 2068 6561 6465 7220 2b20 3132 3820  ck header + 128 
-0000f090: 4b69 4229 2c20 7468 6520 6163 7475 616c  KiB), the actual
-0000f0a0: 206d 6178 696d 756d 2073 697a 6520 6465   maximum size de
-0000f0b0: 7065 6e64 7320 6f6e 2066 7261 6d65 2070  pends on frame p
-0000f0c0: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
-0000f0d0: 556e 6c69 6b65 2069 6e64 6570 656e 6465  Unlike independe
-0000f0e0: 6e74 2066 7261 6d65 732c 2065 6163 6820  nt frames, each 
-0000f0f0: 626c 6f63 6b20 6465 7065 6e64 7320 6f6e  block depends on
-0000f100: 2070 7265 7669 6f75 7320 626c 6f63 6b73   previous blocks
-0000f110: 2066 6f72 2070 726f 7065 7220 6465 636f   for proper deco
-0000f120: 6469 6e67 2c20 6275 7420 646f 6573 6e27  ding, but doesn'
-0000f130: 7420 6e65 6564 2074 6865 2066 6f6c 6c6f  t need the follo
-0000f140: 7769 6e67 2062 6c6f 636b 732c 2061 2063  wing blocks, a c
-0000f150: 6f6d 706c 6574 6520 626c 6f63 6b20 6361  omplete block ca
-0000f160: 6e20 6265 2066 756c 6c79 2064 6563 6f6d  n be fully decom
-0000f170: 7072 6573 7365 642e 2053 6f20 666c 7573  pressed. So flus
-0000f180: 6869 6e67 2062 6c6f 636b 206d 6179 2062  hing block may b
-0000f190: 6520 7573 6564 2069 6e20 636f 6d6d 756e  e used in commun
-0000f1a0: 6963 6174 696f 6e20 7363 656e 6172 696f  ication scenario
-0000f1b0: 732c 2073 6565 203a 7079 3a61 7474 723a  s, see :py:attr:
-0000f1c0: 605a 7374 6443 6f6d 7072 6573 736f 722e  `ZstdCompressor.
-0000f1d0: 464c 5553 485f 424c 4f43 4b60 2e0a 0a20  FLUSH_BLOCK`... 
-0000f1e0: 2020 202e 2e20 6174 7465 6e74 696f 6e3a     .. attention:
-0000f1f0: 3a0a 0a20 2020 2020 2020 2049 6e20 736f  :..        In so
-0000f200: 6d65 2060 6c61 6e67 7561 6765 2062 696e  me `language bin
-0000f210: 6469 6e67 7320 3c68 7474 7073 3a2f 2f66  dings <https://f
-0000f220: 6163 6562 6f6f 6b2e 6769 7468 7562 2e69  acebook.github.i
-0000f230: 6f2f 7a73 7464 2f23 6f74 6865 722d 6c61  o/zstd/#other-la
-0000f240: 6e67 7561 6765 733e 605f 2c20 6465 636f  nguages>`_, deco
-0000f250: 6d70 7265 7373 2829 2066 756e 6374 696f  mpress() functio
-0000f260: 6e20 646f 6573 6e27 7420 7375 7070 6f72  n doesn't suppor
-0000f270: 7420 6d75 6c74 6970 6c65 2066 7261 6d65  t multiple frame
-0000f280: 732c 206f 722f 616e 6420 646f 6573 6e27  s, or/and doesn'
-0000f290: 7420 7375 7070 6f72 7420 6120 6672 616d  t support a fram
-0000f2a0: 6520 7769 7468 2075 6e6b 6e6f 776e 203a  e with unknown :
-0000f2b0: 7265 663a 6063 6f6e 7465 6e74 2073 697a  ref:`content siz
-0000f2c0: 653c 636f 6e74 656e 745f 7369 7a65 3e60  e<content_size>`
-0000f2d0: 2c20 7061 7920 6174 7465 6e74 696f 6e20  , pay attention 
-0000f2e0: 7768 656e 2063 6f6d 7072 6573 7369 6e67  when compressing
-0000f2f0: 2064 6174 6120 666f 7220 6f74 6865 7220   data for other 
-0000f300: 6c61 6e67 7561 6765 2062 696e 6469 6e67  language binding
-0000f310: 732e 0a0a 0a4d 756c 7469 2d74 6872 6561  s....Multi-threa
-0000f320: 6465 6420 636f 6d70 7265 7373 696f 6e0a  ded compression.
-0000f330: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
-0000f340: 3e3e 3e3e 3e3e 3e3e 3e3e 0a0a 2e2e 205f  >>>>>>>>>>.... _
-0000f350: 6d74 5f63 6f6d 7072 6573 7369 6f6e 3a0a  mt_compression:.
-0000f360: 0a2e 2e20 6e6f 7465 3a3a 204d 756c 7469  ... note:: Multi
-0000f370: 2d74 6872 6561 6465 6420 636f 6d70 7265  -threaded compre
-0000f380: 7373 696f 6e0a 0a20 2020 205a 7374 6420  ssion..    Zstd 
-0000f390: 6c69 6272 6172 7920 7375 7070 6f72 7473  library supports
-0000f3a0: 206d 756c 7469 2d74 6872 6561 6465 6420   multi-threaded 
-0000f3b0: 636f 6d70 7265 7373 696f 6e2e 2053 6574  compression. Set
-0000f3c0: 203a 7079 3a61 7474 723a 6043 5061 7261   :py:attr:`CPara
-0000f3d0: 6d65 7465 722e 6e62 576f 726b 6572 7360  meter.nbWorkers`
-0000f3e0: 2070 6172 616d 6574 6572 203e 3d20 6060   parameter >= ``
-0000f3f0: 3160 6020 746f 2065 6e61 626c 6520 6d75  1`` to enable mu
-0000f400: 6c74 692d 7468 7265 6164 6564 2063 6f6d  lti-threaded com
-0000f410: 7072 6573 7369 6f6e 2c20 6060 3160 6020  pression, ``1`` 
-0000f420: 6d65 616e 7320 2231 2d74 6872 6561 6420  means "1-thread 
-0000f430: 6d75 6c74 692d 7468 7265 6164 6564 206d  multi-threaded m
-0000f440: 6f64 6522 2e0a 0a20 2020 2054 6865 2074  ode"...    The t
-0000f450: 6872 6561 6473 2061 7265 2073 7061 776e  hreads are spawn
-0000f460: 6564 2062 7920 7468 6520 756e 6465 726c  ed by the underl
-0000f470: 7969 6e67 207a 7374 6420 6c69 6272 6172  ying zstd librar
-0000f480: 792c 206e 6f74 2062 7920 7079 7a73 7464  y, not by pyzstd
-0000f490: 206d 6f64 756c 652e 0a0a 2020 2020 2e2e   module...    ..
-0000f4a0: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
-0000f4b0: 7468 6f6e 0a0a 2020 2020 2020 2020 2320  thon..        # 
-0000f4c0: 7573 6520 3420 7468 7265 6164 7320 746f  use 4 threads to
-0000f4d0: 2063 6f6d 7072 6573 730a 2020 2020 2020   compress.      
-0000f4e0: 2020 6f70 7469 6f6e 203d 207b 4350 6172    option = {CPar
-0000f4f0: 616d 6574 6572 2e6e 6257 6f72 6b65 7273  ameter.nbWorkers
-0000f500: 203a 2034 7d0a 2020 2020 2020 2020 636f   : 4}.        co
-0000f510: 6d70 7265 7373 6564 5f64 6174 203d 2063  mpressed_dat = c
-0000f520: 6f6d 7072 6573 7328 7261 775f 6461 742c  ompress(raw_dat,
-0000f530: 206f 7074 696f 6e29 0a0a 2020 2020 5468   option)..    Th
-0000f540: 6520 6461 7461 2077 696c 6c20 6265 2073  e data will be s
-0000f550: 706c 6974 2069 6e74 6f20 706f 7274 696f  plit into portio
-0000f560: 6e73 2061 6e64 2063 6f6d 7072 6573 7365  ns and compresse
-0000f570: 6420 696e 2070 6172 616c 6c65 6c2e 2054  d in parallel. T
-0000f580: 6865 2070 6f72 7469 6f6e 2073 697a 6520  he portion size 
-0000f590: 6361 6e20 6265 2073 7065 6369 6669 6564  can be specified
-0000f5a0: 2062 7920 3a70 793a 6174 7472 3a60 4350   by :py:attr:`CP
-0000f5b0: 6172 616d 6574 6572 2e6a 6f62 5369 7a65  arameter.jobSize
-0000f5c0: 6020 7061 7261 6d65 7465 722c 2074 6865  ` parameter, the
-0000f5d0: 206f 7665 726c 6170 2073 697a 6520 6361   overlap size ca
-0000f5e0: 6e20 6265 2073 7065 6369 6669 6564 2062  n be specified b
-0000f5f0: 7920 3a70 793a 6174 7472 3a60 4350 6172  y :py:attr:`CPar
-0000f600: 616d 6574 6572 2e6f 7665 726c 6170 4c6f  ameter.overlapLo
-0000f610: 6760 2070 6172 616d 6574 6572 2c20 7573  g` parameter, us
-0000f620: 7561 6c6c 7920 646f 6e27 7420 6e65 6564  ually don't need
-0000f630: 2074 6f20 7365 7420 7468 6573 652e 0a0a   to set these...
-0000f640: 2020 2020 5468 6520 6d75 6c74 692d 7468      The multi-th
-0000f650: 7265 6164 6564 206f 7574 7075 7420 7769  readed output wi
-0000f660: 6c6c 2062 6520 6469 6666 6572 656e 7420  ll be different 
-0000f670: 7468 616e 2074 6865 2073 696e 676c 652d  than the single-
-0000f680: 7468 7265 6164 6564 206f 7574 7075 742e  threaded output.
-0000f690: 2048 6f77 6576 6572 2c20 626f 7468 2061   However, both a
-0000f6a0: 7265 2064 6574 6572 6d69 6e69 7374 6963  re deterministic
-0000f6b0: 2c20 616e 6420 7468 6520 6d75 6c74 692d  , and the multi-
-0000f6c0: 7468 7265 6164 6564 206f 7574 7075 7420  threaded output 
-0000f6d0: 7072 6f64 7563 6573 2074 6865 2073 616d  produces the sam
-0000f6e0: 6520 636f 6d70 7265 7373 6564 2064 6174  e compressed dat
-0000f6f0: 6120 6e6f 206d 6174 7465 7220 686f 7720  a no matter how 
-0000f700: 6d61 6e79 2074 6872 6561 6473 2075 7365  many threads use
-0000f710: 642e 0a0a 2020 2020 5468 6520 6d75 6c74  d...    The mult
-0000f720: 692d 7468 7265 6164 6564 206f 7574 7075  i-threaded outpu
-0000f730: 7420 6973 2061 2073 696e 676c 6520 3a72  t is a single :r
-0000f740: 6566 3a60 6672 616d 653c 6672 616d 655f  ef:`frame<frame_
-0000f750: 626c 6f63 6b3e 602c 2069 7427 7320 6c61  block>`, it's la
-0000f760: 7267 6572 2061 206c 6974 746c 652e 2043  rger a little. C
-0000f770: 6f6d 7072 6573 7369 6e67 2061 2035 3230  ompressing a 520
-0000f780: 2e35 3820 4d69 4220 6461 7461 2c20 7369  .58 MiB data, si
-0000f790: 6e67 6c65 2d74 6872 6561 6465 6420 6f75  ngle-threaded ou
-0000f7a0: 7470 7574 2069 7320 3237 332e 3535 204d  tput is 273.55 M
-0000f7b0: 6942 2c20 6d75 6c74 692d 7468 7265 6164  iB, multi-thread
-0000f7c0: 6564 206f 7574 7075 7420 6973 2032 3734  ed output is 274
-0000f7d0: 2e33 3320 4d69 422e 0a0a 2020 2020 2e2e  .33 MiB...    ..
-0000f7e0: 2068 696e 743a 3a0a 2020 2020 2020 2020   hint::.        
-0000f7f0: 5573 696e 6720 2243 5055 2070 6879 7369  Using "CPU physi
-0000f800: 6361 6c20 636f 7265 7320 6e75 6d62 6572  cal cores number
-0000f810: 2220 6173 2074 6872 6561 6473 206e 756d  " as threads num
-0000f820: 6265 7220 6d61 7920 6265 2074 6865 2066  ber may be the f
-0000f830: 6173 7465 7374 2c20 746f 2067 6574 2074  astest, to get t
-0000f840: 6865 206e 756d 6265 7220 6e65 6564 2074  he number need t
-0000f850: 6f20 696e 7374 616c 6c20 7468 6972 642d  o install third-
-0000f860: 7061 7274 7920 6d6f 6475 6c65 2e20 606f  party module. `o
-0000f870: 732e 6370 755f 636f 756e 7428 2920 3c68  s.cpu_count() <h
-0000f880: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
-0000f890: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
-0000f8a0: 2f6f 732e 6874 6d6c 236f 732e 6370 755f  /os.html#os.cpu_
-0000f8b0: 636f 756e 743e 605f 2063 616e 206f 6e6c  count>`_ can onl
-0000f8c0: 7920 6765 7420 2243 5055 206c 6f67 6963  y get "CPU logic
-0000f8d0: 616c 2063 6f72 6573 206e 756d 6265 7222  al cores number"
-0000f8e0: 2028 6879 7065 722d 7468 7265 6164 696e   (hyper-threadin
-0000f8f0: 6720 6361 7061 6269 6c69 7479 292e 0a0a  g capability)...
-0000f900: 0a52 6963 6820 6d65 6d6f 7279 206d 6f64  .Rich memory mod
-0000f910: 650a 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  e.>>>>>>>>>>>>>>
-0000f920: 3e3e 0a0a 2e2e 205f 7269 6368 5f6d 656d  >>.... _rich_mem
-0000f930: 3a0a 0a2e 2e20 6e6f 7465 3a3a 2052 6963  :.... note:: Ric
-0000f940: 6820 6d65 6d6f 7279 206d 6f64 650a 0a20  h memory mode.. 
-0000f950: 2020 2070 797a 7374 6420 6d6f 6475 6c65     pyzstd module
-0000f960: 2068 6173 2061 2022 7269 6368 206d 656d   has a "rich mem
-0000f970: 6f72 7920 6d6f 6465 2220 666f 7220 636f  ory mode" for co
-0000f980: 6d70 7265 7373 696f 6e2e 2049 7420 616c  mpression. It al
-0000f990: 6c6f 6361 7465 7320 6d6f 7265 206d 656d  locates more mem
-0000f9a0: 6f72 7920 666f 7220 6f75 7470 7574 2062  ory for output b
-0000f9b0: 7566 6665 722c 2061 6e64 2066 6173 7465  uffer, and faste
-0000f9c0: 7220 696e 2073 6f6d 6520 6361 7365 732e  r in some cases.
-0000f9d0: 2053 7569 7461 626c 6520 666f 7220 6578   Suitable for ex
-0000f9e0: 7472 656d 656c 7920 6661 7374 2063 6f6d  tremely fast com
-0000f9f0: 7072 6573 7369 6f6e 2073 6365 6e61 7269  pression scenari
-0000fa00: 6f73 2e0a 0a20 2020 2054 6865 7265 2069  os...    There i
-0000fa10: 7320 6120 3a70 793a 6675 6e63 3a60 7269  s a :py:func:`ri
-0000fa20: 6368 6d65 6d5f 636f 6d70 7265 7373 6020  chmem_compress` 
-0000fa30: 6675 6e63 7469 6f6e 2c20 6120 3a70 793a  function, a :py:
-0000fa40: 636c 6173 733a 6052 6963 684d 656d 5a73  class:`RichMemZs
-0000fa50: 7464 436f 6d70 7265 7373 6f72 6020 636c  tdCompressor` cl
-0000fa60: 6173 732e 0a0a 2020 2020 4375 7272 656e  ass...    Curren
-0000fa70: 746c 7920 6974 2077 6f6e 2774 2062 6520  tly it won't be 
-0000fa80: 6661 7374 6572 2077 6865 6e20 7573 696e  faster when usin
-0000fa90: 6720 3a72 6566 3a60 7a73 7464 206d 756c  g :ref:`zstd mul
-0000faa0: 7469 2d74 6872 6561 6465 6420 636f 6d70  ti-threaded comp
-0000fab0: 7265 7373 696f 6e20 3c6d 745f 636f 6d70  ression <mt_comp
-0000fac0: 7265 7373 696f 6e3e 602c 2069 7420 7769  ression>`, it wi
-0000fad0: 6c6c 2069 7373 7565 2061 2060 6052 6573  ll issue a ``Res
-0000fae0: 6f75 7263 6557 6172 6e69 6e67 7360 6020  ourceWarnings`` 
-0000faf0: 696e 2074 6869 7320 6361 7365 2e0a 0a20  in this case... 
-0000fb00: 2020 2045 6666 6563 7473 3a0a 0a20 2020     Effects:..   
-0000fb10: 202a 2054 6865 206f 7574 7075 7420 6275   * The output bu
-0000fb20: 6666 6572 2069 7320 6c61 7267 6572 2074  ffer is larger t
-0000fb30: 6861 6e20 696e 7075 7420 6461 7461 2061  han input data a
-0000fb40: 206c 6974 746c 652e 0a20 2020 202a 2049   little..    * I
-0000fb50: 6620 696e 7075 7420 6461 7461 2069 7320  f input data is 
-0000fb60: 6c61 7267 6572 2074 6861 6e20 7e33 312e  larger than ~31.
-0000fb70: 384b 422c 2075 7020 746f 2032 3225 2066  8KB, up to 22% f
-0000fb80: 6173 7465 722e 2054 6865 206c 6f77 6572  aster. The lower
-0000fb90: 2074 6865 2063 6f6d 7072 6573 7369 6f6e   the compression
-0000fba0: 206c 6576 656c 2c20 7468 6520 6d75 6368   level, the much
-0000fbb0: 2066 6173 7465 7220 6974 2069 7320 7573   faster it is us
-0000fbc0: 7561 6c6c 792e 0a0a 2020 2020 5768 656e  ually...    When
-0000fbd0: 206e 6f74 2075 7369 6e67 2074 6869 7320   not using this 
-0000fbe0: 6d6f 6465 2c20 7468 6520 6f75 7470 7574  mode, the output
-0000fbf0: 2062 7566 6665 7220 6772 6f77 7320 6067   buffer grows `g
-0000fc00: 7261 6475 616c 6c79 203c 6874 7470 733a  radually <https:
-0000fc10: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6e69  //github.com/ani
-0000fc20: 6d61 6c69 7a65 2f70 797a 7374 642f 626c  malize/pyzstd/bl
-0000fc30: 6f62 2f30 2e31 352e 372f 7372 632f 6269  ob/0.15.7/src/bi
-0000fc40: 6e5f 6578 742f 5f7a 7374 646d 6f64 756c  n_ext/_zstdmodul
-0000fc50: 652e 6323 4c32 3138 2d4c 3234 333e 605f  e.c#L218-L243>`_
-0000fc60: 2c20 696e 206f 7264 6572 206e 6f74 2074  , in order not t
-0000fc70: 6f20 616c 6c6f 6361 7465 2074 6f6f 206d  o allocate too m
-0000fc80: 7563 6820 6d65 6d6f 7279 2e20 5468 6520  uch memory. The 
-0000fc90: 6e65 6761 7469 7665 2065 6666 6563 7420  negative effect 
-0000fca0: 6973 2074 6861 7420 7079 7a73 7464 206d  is that pyzstd m
-0000fcb0: 6f64 756c 6520 7573 7561 6c6c 7920 6e65  odule usually ne
-0000fcc0: 6564 2074 6f20 6361 6c6c 2074 6865 2075  ed to call the u
-0000fcd0: 6e64 6572 6c79 696e 6720 7a73 7464 206c  nderlying zstd l
-0000fce0: 6962 7261 7279 2773 2063 6f6d 7072 6573  ibrary's compres
-0000fcf0: 7320 6675 6e63 7469 6f6e 206d 756c 7469  s function multi
-0000fd00: 706c 6520 7469 6d65 732e 0a0a 2020 2020  ple times...    
-0000fd10: 5768 656e 2075 7369 6e67 2074 6869 7320  When using this 
-0000fd20: 6d6f 6465 2c20 7468 6520 7369 7a65 206f  mode, the size o
-0000fd30: 6620 6f75 7470 7574 2062 7566 6665 7220  f output buffer 
-0000fd40: 6973 2070 726f 7669 6465 6420 6279 205a  is provided by Z
-0000fd50: 5354 445f 636f 6d70 7265 7373 426f 756e  STD_compressBoun
-0000fd60: 6428 2920 6675 6e63 7469 6f6e 2c20 7768  d() function, wh
-0000fd70: 6963 6820 6973 206c 6172 6765 7220 7468  ich is larger th
-0000fd80: 616e 2069 6e70 7574 2064 6174 6120 6120  an input data a 
-0000fd90: 6c69 7474 6c65 2028 6d61 7869 6d75 6d20  little (maximum 
-0000fda0: 636f 6d70 7265 7373 6564 2073 697a 6520  compressed size 
-0000fdb0: 696e 2077 6f72 7374 2063 6173 6520 7369  in worst case si
-0000fdc0: 6e67 6c65 2d70 6173 7320 7363 656e 6172  ngle-pass scenar
-0000fdd0: 696f 292e 2046 6f72 2061 2031 3030 204d  io). For a 100 M
-0000fde0: 6942 2069 6e70 7574 2064 6174 612c 2074  iB input data, t
-0000fdf0: 6865 2061 6c6c 6f63 6174 6564 206f 7574  he allocated out
-0000fe00: 7075 7420 6275 6666 6572 2069 7320 2831  put buffer is (1
-0000fe10: 3030 204d 6942 202b 2034 3030 204b 6942  00 MiB + 400 KiB
-0000fe20: 292e 2054 6865 2075 6e64 6572 6c79 696e  ). The underlyin
-0000fe30: 6720 7a73 7464 206c 6962 7261 7279 2061  g zstd library a
-0000fe40: 766f 6964 7320 6578 7472 6120 6d65 6d6f  voids extra memo
-0000fe50: 7279 2063 6f70 7920 666f 7220 7468 6973  ry copy for this
-0000fe60: 206f 7574 7075 7420 6275 6666 6572 2073   output buffer s
-0000fe70: 697a 652e 0a0a 2020 2020 2e2e 2073 6f75  ize...    .. sou
-0000fe80: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
-0000fe90: 0a0a 2020 2020 2020 2020 2320 7573 6520  ..        # use 
-0000fea0: 7269 6368 6d65 6d5f 636f 6d70 7265 7373  richmem_compress
-0000feb0: 2829 2066 756e 6374 696f 6e0a 2020 2020  () function.    
-0000fec0: 2020 2020 636f 6d70 7265 7373 6564 5f64      compressed_d
-0000fed0: 6174 203d 2072 6963 686d 656d 5f63 6f6d  at = richmem_com
-0000fee0: 7072 6573 7328 7261 775f 6461 7429 0a0a  press(raw_dat)..
-0000fef0: 2020 2020 2020 2020 2320 7265 7573 6520          # reuse 
-0000ff00: 5269 6368 4d65 6d5a 7374 6443 6f6d 7072  RichMemZstdCompr
-0000ff10: 6573 736f 7220 6f62 6a65 6374 0a20 2020  essor object.   
-0000ff20: 2020 2020 2063 203d 2052 6963 684d 656d       c = RichMem
-0000ff30: 5a73 7464 436f 6d70 7265 7373 6f72 2829  ZstdCompressor()
-0000ff40: 0a20 2020 2020 2020 2066 7261 6d65 3120  .        frame1 
-0000ff50: 3d20 632e 636f 6d70 7265 7373 2872 6177  = c.compress(raw
-0000ff60: 5f64 6174 3129 0a20 2020 2020 2020 2066  _dat1).        f
-0000ff70: 7261 6d65 3220 3d20 632e 636f 6d70 7265  rame2 = c.compre
-0000ff80: 7373 2872 6177 5f64 6174 3229 0a0a 2020  ss(raw_dat2)..  
-0000ff90: 2020 436f 6d70 7265 7373 696e 6720 6120    Compressing a 
-0000ffa0: 3532 302e 3538 204d 6942 2064 6174 612c  520.58 MiB data,
-0000ffb0: 2069 7420 6163 6365 6c65 7261 7465 7320   it accelerates 
-0000ffc0: 6672 6f6d 2035 2e34 3020 7365 636f 6e64  from 5.40 second
-0000ffd0: 7320 746f 2034 2e36 3220 7365 636f 6e64  s to 4.62 second
-0000ffe0: 732e 0a0a 0a55 7365 2077 6974 6820 7461  s....Use with ta
-0000fff0: 7266 696c 6520 6d6f 6475 6c65 0a3e 3e3e  rfile module.>>>
-00010000: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
-00010010: 3e3e 3e3e 0a0a 2e2e 205f 7769 7468 5f74  >>>>.... _with_t
-00010020: 6172 6669 6c65 3a0a 0a2e 2e20 6e6f 7465  arfile:.... note
-00010030: 3a3a 2055 7365 2077 6974 6820 7461 7266  :: Use with tarf
-00010040: 696c 6520 6d6f 6475 6c65 0a0a 2020 2020  ile module..    
-00010050: 5079 7468 6f6e 2773 2060 7461 7266 696c  Python's `tarfil
-00010060: 6520 3c68 7474 7073 3a2f 2f64 6f63 732e  e <https://docs.
-00010070: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
-00010080: 7261 7279 2f74 6172 6669 6c65 2e68 746d  rary/tarfile.htm
-00010090: 6c3e 605f 206d 6f64 756c 6520 7375 7070  l>`_ module supp
-000100a0: 6f72 7473 2061 7262 6974 7261 7279 2063  orts arbitrary c
-000100b0: 6f6d 7072 6573 7369 6f6e 2061 6c67 6f72  ompression algor
-000100c0: 6974 686d 7320 6279 2070 726f 7669 6469  ithms by providi
-000100d0: 6e67 2061 2066 696c 6520 6f62 6a65 6374  ng a file object
-000100e0: 2e0a 0a20 2020 2054 6869 7320 636f 6465  ...    This code
-000100f0: 2065 6e63 6170 7375 6c61 7465 7320 6120   encapsulates a 
-00010100: 6060 5a73 7464 5461 7246 696c 6560 6020  ``ZstdTarFile`` 
-00010110: 636c 6173 7320 7573 696e 6720 3a70 793a  class using :py:
-00010120: 636c 6173 733a 605a 7374 6446 696c 6560  class:`ZstdFile`
-00010130: 2c20 6974 2063 616e 2062 6520 7573 6564  , it can be used
-00010140: 206c 696b 6520 6074 6172 6669 6c65 2e54   like `tarfile.T
-00010150: 6172 4669 6c65 203c 6874 7470 733a 2f2f  arFile <https://
-00010160: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-00010170: 332f 6c69 6272 6172 792f 7461 7266 696c  3/library/tarfil
-00010180: 652e 6874 6d6c 2374 6172 6669 6c65 2e54  e.html#tarfile.T
-00010190: 6172 4669 6c65 3e60 5f20 636c 6173 733a  arFile>`_ class:
-000101a0: 0a0a 2020 2020 2e2e 2073 6f75 7263 6563  ..    .. sourcec
-000101b0: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
-000101c0: 2020 2020 2020 696d 706f 7274 2074 6172        import tar
-000101d0: 6669 6c65 0a0a 2020 2020 2020 2020 2320  file..        # 
-000101e0: 7768 656e 2075 7369 6e67 2072 6561 6420  when using read 
-000101f0: 6d6f 6465 2028 6465 636f 6d70 7265 7373  mode (decompress
-00010200: 696f 6e29 2c20 7468 6520 6c65 7665 6c5f  ion), the level_
-00010210: 6f72 5f6f 7074 696f 6e20 7061 7261 6d65  or_option parame
-00010220: 7465 720a 2020 2020 2020 2020 2320 6361  ter.        # ca
-00010230: 6e20 6f6e 6c79 2062 6520 6120 6469 6374  n only be a dict
-00010240: 206f 626a 6563 742c 2074 6861 7420 7265   object, that re
-00010250: 7072 6573 656e 7473 2064 6563 6f6d 7072  presents decompr
-00010260: 6573 7369 6f6e 206f 7074 696f 6e2e 2049  ession option. I
-00010270: 740a 2020 2020 2020 2020 2320 646f 6573  t.        # does
-00010280: 6e27 7420 7375 7070 6f72 7420 696e 7420  n't support int 
-00010290: 7479 7065 2063 6f6d 7072 6573 7369 6f6e  type compression
-000102a0: 206c 6576 656c 2069 6e20 7468 6973 2063   level in this c
-000102b0: 6173 652e 0a0a 2020 2020 2020 2020 636c  ase...        cl
-000102c0: 6173 7320 5a73 7464 5461 7246 696c 6528  ass ZstdTarFile(
-000102d0: 7461 7266 696c 652e 5461 7246 696c 6529  tarfile.TarFile)
-000102e0: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-000102f0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00010300: 206e 616d 652c 206d 6f64 653d 2772 272c   name, mode='r',
-00010310: 202a 2c20 6c65 7665 6c5f 6f72 5f6f 7074   *, level_or_opt
-00010320: 696f 6e3d 4e6f 6e65 2c20 7a73 7464 5f64  ion=None, zstd_d
-00010330: 6963 743d 4e6f 6e65 2c20 2a2a 6b77 6172  ict=None, **kwar
-00010340: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
-00010350: 2020 2020 2073 656c 662e 7a73 7464 5f66       self.zstd_f
-00010360: 696c 6520 3d20 5a73 7464 4669 6c65 286e  ile = ZstdFile(n
-00010370: 616d 652c 206d 6f64 652c 0a20 2020 2020  ame, mode,.     
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103a0: 2020 2020 206c 6576 656c 5f6f 725f 6f70       level_or_op
-000103b0: 7469 6f6e 3d6c 6576 656c 5f6f 725f 6f70  tion=level_or_op
-000103c0: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103f0: 7a73 7464 5f64 6963 743d 7a73 7464 5f64  zstd_dict=zstd_d
-00010400: 6963 7429 0a20 2020 2020 2020 2020 2020  ict).           
-00010410: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00010420: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00010430: 7065 7228 292e 5f5f 696e 6974 5f5f 2866  per().__init__(f
-00010440: 696c 656f 626a 3d73 656c 662e 7a73 7464  ileobj=self.zstd
-00010450: 5f66 696c 652c 206d 6f64 653d 6d6f 6465  _file, mode=mode
-00010460: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
-00010470: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00010480: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-00010490: 2020 2020 2020 2020 7365 6c66 2e7a 7374          self.zst
-000104a0: 645f 6669 6c65 2e63 6c6f 7365 2829 0a20  d_file.close(). 
-000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104c0: 2020 2072 6169 7365 0a0a 2020 2020 2020     raise..      
-000104d0: 2020 2020 2020 6465 6620 636c 6f73 6528        def close(
-000104e0: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
-000104f0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010510: 7375 7065 7228 292e 636c 6f73 6528 290a  super().close().
-00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010530: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
-00010540: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010550: 662e 7a73 7464 5f66 696c 652e 636c 6f73  f.zstd_file.clos
-00010560: 6528 290a 0a20 2020 2020 2020 2023 2077  e()..        # w
-00010570: 7269 7465 202e 7461 722e 7a73 7420 6669  rite .tar.zst fi
-00010580: 6c65 2028 636f 6d70 7265 7373 696f 6e29  le (compression)
-00010590: 0a20 2020 2020 2020 2077 6974 6820 5a73  .        with Zs
-000105a0: 7464 5461 7246 696c 6528 2761 7263 6869  tdTarFile('archi
-000105b0: 7665 2e74 6172 2e7a 7374 272c 206d 6f64  ve.tar.zst', mod
-000105c0: 653d 2777 272c 206c 6576 656c 5f6f 725f  e='w', level_or_
-000105d0: 6f70 7469 6f6e 3d35 2920 6173 2074 6172  option=5) as tar
-000105e0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000105f0: 646f 2073 6f6d 6574 6869 6e67 0a0a 2020  do something..  
-00010600: 2020 2020 2020 2320 7265 6164 202e 7461        # read .ta
-00010610: 722e 7a73 7420 6669 6c65 2028 6465 636f  r.zst file (deco
-00010620: 6d70 7265 7373 696f 6e29 0a20 2020 2020  mpression).     
-00010630: 2020 2077 6974 6820 5a73 7464 5461 7246     with ZstdTarF
-00010640: 696c 6528 2761 7263 6869 7665 2e74 6172  ile('archive.tar
-00010650: 2e7a 7374 272c 206d 6f64 653d 2772 2729  .zst', mode='r')
-00010660: 2061 7320 7461 723a 0a20 2020 2020 2020   as tar:.       
-00010670: 2020 2020 2023 2064 6f20 736f 6d65 7468       # do someth
-00010680: 696e 670a 0a20 2020 2057 6865 6e20 7468  ing..    When th
-00010690: 6520 6162 6f76 6520 636f 6465 2069 7320  e above code is 
-000106a0: 696e 2072 6561 6420 6d6f 6465 2028 6465  in read mode (de
-000106b0: 636f 6d70 7265 7373 696f 6e29 2c20 616e  compression), an
-000106c0: 6420 7365 6c65 6374 6976 656c 7920 7265  d selectively re
-000106d0: 6164 2066 696c 6573 206d 756c 7469 706c  ad files multipl
-000106e0: 6520 7469 6d65 732c 2069 7420 6d61 7920  e times, it may 
-000106f0: 7365 656b 2074 6f20 7072 6576 696f 7573  seek to previous
-00010700: 2070 6f73 6974 696f 6e73 2c20 7468 656e   positions, then
-00010710: 2074 6865 2064 6563 6f6d 7072 6573 7369   the decompressi
-00010720: 6f6e 2068 6173 2074 6f20 6265 2072 6573  on has to be res
-00010730: 7461 7274 6564 2066 726f 6d20 7a65 726f  tarted from zero
-00010740: 2e20 4966 2074 6869 7320 736c 6f77 7320  . If this slows 
-00010750: 646f 776e 2074 6865 206f 7065 7261 7469  down the operati
-00010760: 6f6e 732c 2074 6865 2061 7263 6869 7665  ons, the archive
-00010770: 2063 616e 2062 6520 6465 636f 6d70 7265   can be decompre
-00010780: 7373 6564 2074 6f20 6120 7465 6d70 6f72  ssed to a tempor
-00010790: 6172 7920 6669 6c65 2c20 616e 6420 7265  ary file, and re
-000107a0: 6164 2066 726f 6d20 6974 2e20 5468 6973  ad from it. This
-000107b0: 2063 6f64 6520 656e 6361 7073 756c 6174   code encapsulat
-000107c0: 6573 2074 6865 2070 726f 6365 7373 3a0a  es the process:.
-000107d0: 0a20 2020 202e 2e20 736f 7572 6365 636f  .    .. sourceco
-000107e0: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
-000107f0: 2020 2020 2069 6d70 6f72 7420 636f 6e74       import cont
-00010800: 6578 746c 6962 0a20 2020 2020 2020 2069  extlib.        i
-00010810: 6d70 6f72 7420 696f 0a20 2020 2020 2020  mport io.       
-00010820: 2069 6d70 6f72 7420 7461 7266 696c 650a   import tarfile.
-00010830: 2020 2020 2020 2020 696d 706f 7274 2074          import t
-00010840: 656d 7066 696c 650a 2020 2020 2020 2020  empfile.        
-00010850: 6672 6f6d 2070 797a 7374 6420 696d 706f  from pyzstd impo
-00010860: 7274 2064 6563 6f6d 7072 6573 735f 7374  rt decompress_st
-00010870: 7265 616d 0a0a 2020 2020 2020 2020 4063  ream..        @c
-00010880: 6f6e 7465 7874 6c69 622e 636f 6e74 6578  ontextlib.contex
-00010890: 746d 616e 6167 6572 0a20 2020 2020 2020  tmanager.       
-000108a0: 2064 6566 205a 7374 6454 6172 5265 6164   def ZstdTarRead
-000108b0: 6572 286e 616d 652c 202a 2c20 7a73 7464  er(name, *, zstd
-000108c0: 5f64 6963 743d 4e6f 6e65 2c20 6f70 7469  _dict=None, opti
-000108d0: 6f6e 3d4e 6f6e 652c 202a 2a6b 7761 7267  on=None, **kwarg
-000108e0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-000108f0: 7769 7468 2069 6f2e 6f70 656e 286e 616d  with io.open(nam
-00010900: 652c 2027 7262 2729 2061 7320 6966 683a  e, 'rb') as ifh:
-00010910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010920: 2077 6974 6820 7465 6d70 6669 6c65 2e54   with tempfile.T
-00010930: 656d 706f 7261 7279 4669 6c65 2829 2061  emporaryFile() a
-00010940: 7320 746d 705f 6669 6c65 3a0a 2020 2020  s tmp_file:.    
-00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010960: 6465 636f 6d70 7265 7373 5f73 7472 6561  decompress_strea
-00010970: 6d28 6966 682c 2074 6d70 5f66 696c 652c  m(ifh, tmp_file,
-00010980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109a0: 2020 2020 2020 207a 7374 645f 6469 6374         zstd_dict
-000109b0: 3d7a 7374 645f 6469 6374 2c20 6f70 7469  =zstd_dict, opti
-000109c0: 6f6e 3d6f 7074 696f 6e29 0a20 2020 2020  on=option).     
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000109e0: 6d70 5f66 696c 652e 7365 656b 2830 290a  mp_file.seek(0).
-000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a00: 2020 2020 7769 7468 2074 6172 6669 6c65      with tarfile
-00010a10: 2e54 6172 4669 6c65 2866 696c 656f 626a  .TarFile(fileobj
-00010a20: 3d74 6d70 5f66 696c 652c 202a 2a6b 7761  =tmp_file, **kwa
-00010a30: 7267 7329 2061 7320 7461 723a 0a20 2020  rgs) as tar:.   
-00010a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a50: 2020 2020 2079 6965 6c64 2074 6172 0a0a       yield tar..
-00010a60: 2020 2020 2020 2020 7769 7468 205a 7374          with Zst
-00010a70: 6454 6172 5265 6164 6572 2827 6172 6368  dTarReader('arch
-00010a80: 6976 652e 7461 722e 7a73 7427 2920 6173  ive.tar.zst') as
-00010a90: 2074 6172 3a0a 2020 2020 2020 2020 2020   tar:.          
-00010aa0: 2020 2320 646f 2073 6f6d 6574 6869 6e67    # do something
-00010ab0: 0a0a 0a5a 7374 6420 6469 6374 696f 6e61  ...Zstd dictiona
-00010ac0: 7279 2049 440a 3e3e 3e3e 3e3e 3e3e 3e3e  ry ID.>>>>>>>>>>
-00010ad0: 3e3e 3e3e 3e3e 3e3e 0a0a 2e2e 205f 6469  >>>>>>>>.... _di
-00010ae0: 6374 5f69 643a 0a0a 2e2e 206e 6f74 653a  ct_id:.... note:
-00010af0: 3a20 5a73 7464 2064 6963 7469 6f6e 6172  : Zstd dictionar
-00010b00: 7920 4944 0a0a 2020 2020 4469 6374 696f  y ID..    Dictio
-00010b10: 6e61 7279 2049 4420 6973 2061 2033 322d  nary ID is a 32-
-00010b20: 6269 7420 756e 7369 676e 6564 2069 6e74  bit unsigned int
-00010b30: 6567 6572 2076 616c 7565 2e20 4465 636f  eger value. Deco
-00010b40: 6465 7220 7573 6573 2069 7420 746f 2063  der uses it to c
-00010b50: 6865 636b 2069 6620 7468 6520 636f 7272  heck if the corr
-00010b60: 6563 7420 6469 6374 696f 6e61 7279 2069  ect dictionary i
-00010b70: 7320 7573 6564 2e0a 0a20 2020 2041 6363  s used...    Acc
-00010b80: 6f72 6469 6e67 2074 6f20 7a73 7464 2064  ording to zstd d
-00010b90: 6963 7469 6f6e 6172 7920 666f 726d 6174  ictionary format
-00010ba0: 2060 7370 6563 6966 6963 6174 696f 6e20   `specification 
-00010bb0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00010bc0: 636f 6d2f 6661 6365 626f 6f6b 2f7a 7374  com/facebook/zst
-00010bd0: 642f 626c 6f62 2f72 656c 6561 7365 2f64  d/blob/release/d
-00010be0: 6f63 2f7a 7374 645f 636f 6d70 7265 7373  oc/zstd_compress
-00010bf0: 696f 6e5f 666f 726d 6174 2e6d 6423 6469  ion_format.md#di
-00010c00: 6374 696f 6e61 7279 2d66 6f72 6d61 743e  ctionary-format>
-00010c10: 605f 2c20 6966 2061 2064 6963 7469 6f6e  `_, if a diction
-00010c20: 6172 7920 6973 2067 6f69 6e67 2074 6f20  ary is going to 
-00010c30: 6265 2064 6973 7472 6962 7574 6564 2069  be distributed i
-00010c40: 6e20 7075 626c 6963 2c20 7468 6520 666f  n public, the fo
-00010c50: 6c6c 6f77 696e 6720 7261 6e67 6573 2061  llowing ranges a
-00010c60: 7265 2072 6573 6572 7665 6420 666f 7220  re reserved for 
-00010c70: 6675 7475 7265 2072 6567 6973 7472 6172  future registrar
-00010c80: 2061 6e64 2073 6861 6c6c 206e 6f74 2062   and shall not b
-00010c90: 6520 7573 6564 3a0a 0a20 2020 2020 2020  e used:..       
-00010ca0: 202d 206c 6f77 2072 616e 6765 3a20 3c3d   - low range: <=
-00010cb0: 2033 3237 3637 0a20 2020 2020 2020 202d   32767.        -
-00010cc0: 2068 6967 6820 7261 6e67 653a 203e 3d20   high range: >= 
-00010cd0: 325e 3331 0a0a 2020 2020 4f75 7473 6964  2^31..    Outsid
-00010ce0: 6520 6f66 2074 6865 7365 2072 616e 6765  e of these range
-00010cf0: 732c 2061 6e79 2076 616c 7565 2069 6e20  s, any value in 
-00010d00: 2833 3237 3637 203c 2076 203c 2032 5e33  (32767 < v < 2^3
-00010d10: 3129 2063 616e 2062 6520 7573 6564 2066  1) can be used f
-00010d20: 7265 656c 792c 2065 7665 6e20 696e 2070  reely, even in p
-00010d30: 7562 6c69 6320 656e 7669 726f 6e6d 656e  ublic environmen
-00010d40: 742e 0a0a 2020 2020 496e 207a 7374 6420  t...    In zstd 
-00010d50: 6672 616d 6520 6865 6164 6572 2c20 7468  frame header, th
-00010d60: 6520 6044 6963 7469 6f6e 6172 795f 4944  e `Dictionary_ID
-00010d70: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00010d80: 2e63 6f6d 2f66 6163 6562 6f6f 6b2f 7a73  .com/facebook/zs
-00010d90: 7464 2f62 6c6f 622f 7265 6c65 6173 652f  td/blob/release/
-00010da0: 646f 632f 7a73 7464 5f63 6f6d 7072 6573  doc/zstd_compres
-00010db0: 7369 6f6e 5f66 6f72 6d61 742e 6d64 2364  sion_format.md#d
-00010dc0: 6963 7469 6f6e 6172 795f 6964 3e60 5f20  ictionary_id>`_ 
-00010dd0: 6669 656c 6420 6361 6e20 6265 2030 2f31  field can be 0/1
-00010de0: 2f32 2f34 2062 7974 6573 2e20 4966 2074  /2/4 bytes. If t
-00010df0: 6865 2076 616c 7565 2069 7320 736d 616c  he value is smal
-00010e00: 6c2c 2074 6869 7320 6361 6e20 7361 7665  l, this can save
-00010e10: 2032 7e33 2062 7974 6573 2e20 4f72 2064   2~3 bytes. Or d
-00010e20: 6f6e 2774 2077 7269 7465 2074 6865 2049  on't write the I
-00010e30: 4420 6279 2073 6574 7469 6e67 203a 7079  D by setting :py
-00010e40: 3a61 7474 723a 6043 5061 7261 6d65 7465  :attr:`CParamete
-00010e50: 722e 6469 6374 4944 466c 6167 6020 7061  r.dictIDFlag` pa
-00010e60: 7261 6d65 7465 722e 0a0a 2020 2020 7079  rameter...    py
-00010e70: 7a73 7464 206d 6f64 756c 6520 646f 6573  zstd module does
-00010e80: 6e27 7420 7375 7070 6f72 7420 7370 6563  n't support spec
-00010e90: 6966 7969 6e67 2049 4420 7768 656e 2074  ifying ID when t
-00010ea0: 7261 696e 696e 6720 6469 6374 696f 6e61  raining dictiona
-00010eb0: 7279 2063 7572 7265 6e74 6c79 2e20 4966  ry currently. If
-00010ec0: 2077 616e 7420 746f 2073 7065 6369 6679   want to specify
-00010ed0: 2074 6865 2049 442c 206d 6f64 6966 7920   the ID, modify 
-00010ee0: 7468 6520 6469 6374 696f 6e61 7279 2063  the dictionary c
-00010ef0: 6f6e 7465 6e74 2061 6363 6f72 6469 6e67  ontent according
-00010f00: 2074 6f20 666f 726d 6174 2073 7065 6369   to format speci
-00010f10: 6669 6361 7469 6f6e 2c20 616e 6420 7461  fication, and ta
-00010f20: 6b65 2074 6865 2063 6f72 7265 7370 6f6e  ke the correspon
-00010f30: 6469 6e67 2072 6973 6b73 2e0a 0a20 2020  ding risks...   
-00010f40: 202a 2a41 7474 656e 7469 6f6e 2a2a 0a0a   **Attention**..
-00010f50: 2020 2020 496e 203a 7079 3a63 6c61 7373      In :py:class
-00010f60: 3a60 5a73 7464 4469 6374 6020 636c 6173  :`ZstdDict` clas
-00010f70: 732c 203a 7079 3a61 7474 723a 605a 7374  s, :py:attr:`Zst
-00010f80: 6444 6963 742e 6469 6374 5f69 6460 2061  dDict.dict_id` a
-00010f90: 7474 7269 6275 7465 203d 3d20 3020 6d65  ttribute == 0 me
-00010fa0: 616e 7320 7468 6520 6469 6374 696f 6e61  ans the dictiona
-00010fb0: 7279 2069 7320 6120 2272 6177 2063 6f6e  ry is a "raw con
-00010fc0: 7465 6e74 2220 6469 6374 696f 6e61 7279  tent" dictionary
-00010fd0: 2c20 6672 6565 206f 6620 616e 7920 666f  , free of any fo
-00010fe0: 726d 6174 2072 6573 7472 6963 7469 6f6e  rmat restriction
-00010ff0: 2c20 7573 6564 2066 6f72 2061 6476 616e  , used for advan
-00011000: 6365 6420 7573 6572 2e20 4e6f 6e2d 7a65  ced user. Non-ze
-00011010: 726f 206d 6561 6e73 2069 7427 7320 616e  ro means it's an
-00011020: 206f 7264 696e 6172 7920 6469 6374 696f   ordinary dictio
-00011030: 6e61 7279 2c20 7761 7320 6372 6561 7465  nary, was create
-00011040: 6420 6279 207a 7374 6420 6675 6e63 7469  d by zstd functi
-00011050: 6f6e 732c 2066 6f6c 6c6f 7720 7468 6520  ons, follow the 
-00011060: 666f 726d 6174 2073 7065 6369 6669 6361  format specifica
-00011070: 7469 6f6e 2e0a 0a20 2020 2049 6e20 3a70  tion...    In :p
-00011080: 793a 6675 6e63 3a60 6765 745f 6672 616d  y:func:`get_fram
-00011090: 655f 696e 666f 6020 6675 6e63 7469 6f6e  e_info` function
-000110a0: 2c20 6060 6469 6374 696f 6e61 7279 5f69  , ``dictionary_i
-000110b0: 6460 6020 3d3d 2030 206d 6561 6e73 2064  d`` == 0 means d
-000110c0: 6963 7469 6f6e 6172 7920 4944 2077 6173  ictionary ID was
-000110d0: 206e 6f74 2072 6563 6f72 6465 6420 696e   not recorded in
-000110e0: 2074 6865 2066 7261 6d65 2068 6561 6465   the frame heade
-000110f0: 722c 2074 6865 2066 7261 6d65 206d 6179  r, the frame may
-00011100: 206f 7220 6d61 7920 6e6f 7420 6e65 6564   or may not need
-00011110: 2061 2064 6963 7469 6f6e 6172 7920 746f   a dictionary to
-00011120: 2062 6520 6465 636f 6465 642c 2061 6e64   be decoded, and
-00011130: 2074 6865 2049 4420 6f66 2073 7563 6820   the ID of such 
-00011140: 6120 6469 6374 696f 6e61 7279 2069 7320  a dictionary is 
-00011150: 6e6f 7420 7370 6563 6966 6965 642e 0a0a  not specified...
-00011160: 0a55 7365 207a 7374 6420 6173 2061 2070  .Use zstd as a p
-00011170: 6174 6368 696e 6720 656e 6769 6e65 0a3e  atching engine.>
-00011180: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
-00011190: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 0a0a 2e2e  >>>>>>>>>>>>....
-000111a0: 205f 7061 7463 6869 6e67 5f65 6e67 696e   _patching_engin
-000111b0: 653a 0a0a 2e2e 206e 6f74 653a 3a20 5573  e:.... note:: Us
-000111c0: 6520 7a73 7464 2061 7320 6120 7061 7463  e zstd as a patc
-000111d0: 6869 6e67 2065 6e67 696e 650a 0a20 2020  hing engine..   
-000111e0: 205a 7374 6420 6361 6e20 6265 2075 7365   Zstd can be use
-000111f0: 6420 6173 2061 2067 7265 6174 2060 7061  d as a great `pa
-00011200: 7463 6869 6e67 2065 6e67 696e 6520 3c68  tching engine <h
-00011210: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00011220: 6d2f 6661 6365 626f 6f6b 2f7a 7374 642f  m/facebook/zstd/
-00011230: 7769 6b69 2f5a 7374 616e 6461 7264 2d61  wiki/Zstandard-a
-00011240: 732d 612d 7061 7463 6869 6e67 2d65 6e67  s-a-patching-eng
-00011250: 696e 653e 605f 2c20 616c 7468 6f75 6768  ine>`_, although
-00011260: 2069 7420 6861 7320 736f 6d65 206c 696d   it has some lim
-00011270: 6974 6174 696f 6e73 2e0a 0a20 2020 2049  itations...    I
-00011280: 6e20 7468 6973 2070 6172 7469 6375 6c61  n this particula
-00011290: 7220 7363 656e 6172 696f 2c20 7061 7373  r scenario, pass
-000112a0: 203a 7079 3a61 7474 723a 605a 7374 6444   :py:attr:`ZstdD
-000112b0: 6963 742e 6173 5f70 7265 6669 7860 2061  ict.as_prefix` a
-000112c0: 7320 607a 7374 645f 6469 6374 6020 6172  s `zstd_dict` ar
-000112d0: 6775 6d65 6e74 2e20 2250 7265 6669 7822  gument. "Prefix"
-000112e0: 2069 7320 7369 6d69 6c61 7220 746f 2022   is similar to "
-000112f0: 7261 7720 636f 6e74 656e 7422 2064 6963  raw content" dic
-00011300: 7469 6f6e 6172 792c 2062 7574 207a 7374  tionary, but zst
-00011310: 6420 696e 7465 726e 616c 6c79 2068 616e  d internally han
-00011320: 646c 6573 2074 6865 6d20 6469 6666 6572  dles them differ
-00011330: 656e 746c 792c 2073 6565 2060 7468 6973  ently, see `this
-00011340: 2069 7373 7565 203c 6874 7470 733a 2f2f   issue <https://
-00011350: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
-00011360: 6f6f 6b2f 7a73 7464 2f69 7373 7565 732f  ook/zstd/issues/
-00011370: 3238 3335 3e60 5f2e 0a0a 2020 2020 4573  2835>`_...    Es
-00011380: 7365 6e74 6961 6c6c 792c 2070 7265 6669  sentially, prefi
-00011390: 7820 6973 206c 696b 6520 6265 696e 6720  x is like being 
-000113a0: 706c 6163 6564 2062 6566 6f72 6520 7468  placed before th
-000113b0: 6520 6461 7461 2074 6f20 6265 2063 6f6d  e data to be com
-000113c0: 7072 6573 7365 642e 2053 6565 2022 5a53  pressed. See "ZS
-000113d0: 5444 5f63 5f64 6574 6572 6d69 6e69 7374  TD_c_determinist
-000113e0: 6963 5265 6650 7265 6669 7822 2069 6e20  icRefPrefix" in 
-000113f0: 6074 6869 7320 6669 6c65 203c 6874 7470  `this file <http
-00011400: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-00011410: 6163 6562 6f6f 6b2f 7a73 7464 2f62 6c6f  acebook/zstd/blo
-00011420: 622f 7265 6c65 6173 652f 6c69 622f 7a73  b/release/lib/zs
-00011430: 7464 2e68 3e60 5f2e 0a0a 2020 2020 312c  td.h>`_...    1,
-00011440: 2047 656e 6572 6174 696e 6720 6120 7061   Generating a pa
-00011450: 7463 6820 2863 6f6d 7072 6573 7329 0a0a  tch (compress)..
-00011460: 2020 2020 4173 7375 6d69 6e67 2056 4552      Assuming VER
-00011470: 5f31 2061 6e64 2056 4552 5f32 2061 7265  _1 and VER_2 are
-00011480: 2074 776f 2076 6572 7369 6f6e 732e 0a0a   two versions...
-00011490: 2020 2020 4c65 7420 7468 6520 2277 696e      Let the "win
-000114a0: 646f 7722 2063 6f76 6572 2074 6865 206c  dow" cover the l
-000114b0: 6f6e 6765 7374 2076 6572 7369 6f6e 2c20  ongest version, 
-000114c0: 6279 2073 6574 7469 6e67 203a 7079 3a61  by setting :py:a
-000114d0: 7474 723a 6043 5061 7261 6d65 7465 722e  ttr:`CParameter.
-000114e0: 7769 6e64 6f77 4c6f 6760 2e20 416e 6420  windowLog`. And 
-000114f0: 656e 6162 6c65 2022 6c6f 6e67 2064 6973  enable "long dis
-00011500: 7461 6e63 6520 6d61 7463 6869 6e67 2220  tance matching" 
-00011510: 6279 2073 6574 7469 6e67 203a 7079 3a61  by setting :py:a
-00011520: 7474 723a 6043 5061 7261 6d65 7465 722e  ttr:`CParameter.
-00011530: 656e 6162 6c65 4c6f 6e67 4469 7374 616e  enableLongDistan
-00011540: 6365 4d61 7463 6869 6e67 6020 746f 2031  ceMatching` to 1
-00011550: 2e20 5468 6520 6060 2d2d 7061 7463 682d  . The ``--patch-
-00011560: 6672 6f6d 6060 206f 7074 696f 6e20 6f66  from`` option of
-00011570: 207a 7374 6420 434c 4920 616c 736f 2075   zstd CLI also u
-00011580: 7365 7320 6f74 6865 7220 7061 7261 6d65  ses other parame
-00011590: 7465 7273 2c20 6275 7420 7468 6573 6520  ters, but these 
-000115a0: 7477 6f20 6d61 7474 6572 2074 6865 206d  two matter the m
-000115b0: 6f73 742e 0a0a 2020 2020 5468 6520 7661  ost...    The va
-000115c0: 6c69 6420 7661 6c75 6520 6f66 2060 7769  lid value of `wi
-000115d0: 6e64 6f77 4c6f 6760 2069 7320 5b31 302c  ndowLog` is [10,
-000115e0: 3330 5d20 696e 2033 322d 6269 7420 6275  30] in 32-bit bu
-000115f0: 696c 642c 205b 3130 2c33 315d 2069 6e20  ild, [10,31] in 
-00011600: 3634 2d62 6974 2062 7569 6c64 2e20 536f  64-bit build. So
-00011610: 2069 6e20 3634 2d62 6974 2062 7569 6c64   in 64-bit build
-00011620: 2c20 6974 2068 6173 2061 2060 3247 6942  , it has a `2GiB
-00011630: 206c 656e 6774 6820 6c69 6d69 7420 3c68   length limit <h
-00011640: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00011650: 6d2f 6661 6365 626f 6f6b 2f7a 7374 642f  m/facebook/zstd/
-00011660: 6973 7375 6573 2f32 3137 333e 605f 2e20  issues/2173>`_. 
-00011670: 5374 7269 6374 6c79 2073 7065 616b 696e  Strictly speakin
-00011680: 672c 2074 6865 206c 696d 6974 2069 7320  g, the limit is 
-00011690: 2832 4769 4220 2d20 7e31 3030 4b69 4229  (2GiB - ~100KiB)
-000116a0: 2e20 5768 656e 2074 6869 7320 6c69 6d69  . When this limi
-000116b0: 7420 6973 2065 7863 6565 6465 642c 2074  t is exceeded, t
-000116c0: 6865 2070 6174 6368 2062 6563 6f6d 6573  he patch becomes
-000116d0: 2076 6572 7920 6c61 7267 6520 616e 6420   very large and 
-000116e0: 6c6f 7365 7320 7468 6520 6d65 616e 696e  loses the meanin
-000116f0: 6720 6f66 2061 2070 6174 6368 2e0a 0a20  g of a patch... 
-00011700: 2020 202e 2e20 736f 7572 6365 636f 6465     .. sourcecode
-00011710: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-00011720: 2020 2023 2075 7365 2056 4552 5f31 2061     # use VER_1 a
-00011730: 7320 7072 6566 6978 2e0a 2020 2020 2020  s prefix..      
-00011740: 2020 7631 203d 205a 7374 6444 6963 7428    v1 = ZstdDict(
-00011750: 5645 525f 312c 2069 735f 7261 773d 5472  VER_1, is_raw=Tr
-00011760: 7565 290a 0a20 2020 2020 2020 2023 206c  ue)..        # l
-00011770: 6574 2074 6865 2077 696e 646f 7720 636f  et the window co
-00011780: 7665 7220 7468 6520 6c6f 6e67 6573 7420  ver the longest 
-00011790: 7665 7273 696f 6e2e 0a20 2020 2020 2020  version..       
-000117a0: 2023 2064 6f6e 2774 2066 6f72 6765 7420   # don't forget 
-000117b0: 746f 2063 6c61 6d70 2077 696e 646f 774c  to clamp windowL
-000117c0: 6f67 2074 6f20 7661 6c69 6420 7261 6e67  og to valid rang
-000117d0: 652e 0a20 2020 2020 2020 2023 2065 6e61  e..        # ena
-000117e0: 626c 6520 226c 6f6e 6720 6469 7374 616e  ble "long distan
-000117f0: 6365 206d 6174 6368 696e 6722 2e0a 2020  ce matching"..  
-00011800: 2020 2020 2020 7769 6e64 6f77 4c6f 6720        windowLog 
-00011810: 3d20 6d61 7828 6c65 6e28 5645 525f 3129  = max(len(VER_1)
-00011820: 2c20 6c65 6e28 5645 525f 3229 292e 6269  , len(VER_2)).bi
-00011830: 745f 6c65 6e67 7468 2829 0a20 2020 2020  t_length().     
-00011840: 2020 206f 7074 696f 6e20 3d20 7b43 5061     option = {CPa
-00011850: 7261 6d65 7465 722e 7769 6e64 6f77 4c6f  rameter.windowLo
-00011860: 673a 2077 696e 646f 774c 6f67 2c0a 2020  g: windowLog,.  
-00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011880: 4350 6172 616d 6574 6572 2e65 6e61 626c  CParameter.enabl
-00011890: 654c 6f6e 6744 6973 7461 6e63 654d 6174  eLongDistanceMat
-000118a0: 6368 696e 673a 2031 7d0a 0a20 2020 2020  ching: 1}..     
-000118b0: 2020 2023 2067 6574 2061 2073 6d61 6c6c     # get a small
-000118c0: 2050 4154 4348 0a20 2020 2020 2020 2050   PATCH.        P
-000118d0: 4154 4348 203d 2063 6f6d 7072 6573 7328  ATCH = compress(
-000118e0: 5645 525f 322c 206c 6576 656c 5f6f 725f  VER_2, level_or_
-000118f0: 6f70 7469 6f6e 3d6f 7074 696f 6e2c 207a  option=option, z
-00011900: 7374 645f 6469 6374 3d76 312e 6173 5f70  std_dict=v1.as_p
-00011910: 7265 6669 7829 0a0a 2020 2020 322c 2041  refix)..    2, A
-00011920: 7070 6c79 696e 6720 7468 6520 7061 7463  pplying the patc
-00011930: 6820 2864 6563 6f6d 7072 6573 7329 0a0a  h (decompress)..
-00011940: 2020 2020 5072 6566 6978 2069 7320 6e6f      Prefix is no
-00011950: 7420 6469 6374 696f 6e61 7279 2c20 736f  t dictionary, so
-00011960: 2074 6865 2066 7261 6d65 2068 6561 6465   the frame heade
-00011970: 7220 646f 6573 6e27 7420 7265 636f 7264  r doesn't record
-00011980: 2061 203a 7265 663a 6064 6963 7469 6f6e   a :ref:`diction
-00011990: 6172 7920 6964 3c64 6963 745f 6964 3e60  ary id<dict_id>`
-000119a0: 2e20 5768 656e 2064 6563 6f6d 7072 6573  . When decompres
-000119b0: 7369 6e67 2c20 6d75 7374 2075 7365 2074  sing, must use t
-000119c0: 6865 2073 616d 6520 7072 6566 6978 2061  he same prefix a
-000119d0: 7320 7768 656e 2063 6f6d 7072 6573 7369  s when compressi
-000119e0: 6e67 2e20 4f74 6865 7277 6973 6520 5a73  ng. Otherwise Zs
-000119f0: 7464 4572 726f 7220 6578 6365 7074 696f  tdError exceptio
-00011a00: 6e20 6d61 7920 6265 2072 6169 7365 6420  n may be raised 
-00011a10: 7769 7468 2061 206d 6573 7361 6765 206c  with a message l
-00011a20: 696b 6520 2244 6174 6120 636f 7272 7570  ike "Data corrup
-00011a30: 7469 6f6e 2064 6574 6563 7465 6422 2e0a  tion detected"..
-00011a40: 0a20 2020 2044 6563 6f6d 7072 6573 7369  .    Decompressi
-00011a50: 6e67 2072 6571 7569 7265 7320 6120 7769  ng requires a wi
-00011a60: 6e64 6f77 206f 6620 7468 6520 7361 6d65  ndow of the same
-00011a70: 2073 697a 6520 6173 2077 6865 6e20 636f   size as when co
-00011a80: 6d70 7265 7373 696e 672c 2074 6869 7320  mpressing, this 
-00011a90: 6d61 7920 6265 2061 2070 726f 626c 656d  may be a problem
-00011aa0: 2066 6f72 2073 6d61 6c6c 2052 414d 2064   for small RAM d
-00011ab0: 6576 6963 652e 2049 6620 7468 6520 7769  evice. If the wi
-00011ac0: 6e64 6f77 2069 7320 6c61 7267 6572 2074  ndow is larger t
-00011ad0: 6861 6e20 3132 384d 6942 2c20 6e65 6564  han 128MiB, need
-00011ae0: 2074 6f20 6578 706c 6963 6974 6c79 2073   to explicitly s
-00011af0: 6574 203a 7079 3a61 7474 723a 6044 5061  et :py:attr:`DPa
-00011b00: 7261 6d65 7465 722e 7769 6e64 6f77 4c6f  rameter.windowLo
-00011b10: 674d 6178 6020 746f 2061 6c6c 6f77 206c  gMax` to allow l
-00011b20: 6172 6765 7220 7769 6e64 6f77 2e0a 0a20  arger window... 
-00011b30: 2020 202e 2e20 736f 7572 6365 636f 6465     .. sourcecode
-00011b40: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-00011b50: 2020 2023 2075 7365 2056 4552 5f31 2061     # use VER_1 a
-00011b60: 7320 7072 6566 6978 0a20 2020 2020 2020  s prefix.       
-00011b70: 2076 3120 3d20 5a73 7464 4469 6374 2856   v1 = ZstdDict(V
-00011b80: 4552 5f31 2c20 6973 5f72 6177 3d54 7275  ER_1, is_raw=Tru
-00011b90: 6529 0a0a 2020 2020 2020 2020 2320 616c  e)..        # al
-00011ba0: 6c6f 7720 6c61 7267 6520 7769 6e64 6f77  low large window
-00011bb0: 2c20 7468 6520 6163 7475 616c 2077 696e  , the actual win
-00011bc0: 646f 774c 6f67 2069 7320 6672 6f6d 2066  dowLog is from f
-00011bd0: 7261 6d65 2068 6561 6465 722e 0a20 2020  rame header..   
-00011be0: 2020 2020 206f 7074 696f 6e20 3d20 7b44       option = {D
-00011bf0: 5061 7261 6d65 7465 722e 7769 6e64 6f77  Parameter.window
-00011c00: 4c6f 674d 6178 3a20 3331 7d0a 0a20 2020  LogMax: 31}..   
-00011c10: 2020 2020 2023 2067 6574 2056 4552 5f32       # get VER_2
-00011c20: 2066 726f 6d20 2856 4552 5f31 202b 2050   from (VER_1 + P
-00011c30: 4154 4348 290a 2020 2020 2020 2020 5645  ATCH).        VE
-00011c40: 525f 3220 3d20 6465 636f 6d70 7265 7373  R_2 = decompress
-00011c50: 2850 4154 4348 2c20 7a73 7464 5f64 6963  (PATCH, zstd_dic
-00011c60: 743d 7631 2e61 735f 7072 6566 6978 2c20  t=v1.as_prefix, 
-00011c70: 6f70 7469 6f6e 3d6f 7074 696f 6e29 0a0a  option=option)..
-00011c80: 0a42 7569 6c64 2070 797a 7374 6420 6d6f  .Build pyzstd mo
-00011c90: 6475 6c65 2077 6974 6820 6f70 7469 6f6e  dule with option
-00011ca0: 730a 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  s.>>>>>>>>>>>>>>
-00011cb0: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
-00011cc0: 3e3e 0a0a 2e2e 205f 6275 696c 645f 7079  >>.... _build_py
-00011cd0: 7a73 7464 3a0a 0a2e 2e20 6e6f 7465 3a3a  zstd:.... note::
-00011ce0: 2042 7569 6c64 2070 797a 7374 6420 6d6f   Build pyzstd mo
-00011cf0: 6475 6c65 2077 6974 6820 6f70 7469 6f6e  dule with option
-00011d00: 730a 0a20 2020 2031 efb8 8fe2 83a3 2049  s..    1...... I
-00011d10: 6620 7072 6f76 6964 6520 6060 2d2d 6176  f provide ``--av
-00011d20: 7832 6060 2062 7569 6c64 206f 7074 696f  x2`` build optio
-00011d30: 6e2c 2069 7420 7769 6c6c 2062 7569 6c64  n, it will build
-00011d40: 2077 6974 6820 4156 5832 2f42 4d49 3220   with AVX2/BMI2 
-00011d50: 696e 7374 7275 6374 696f 6e73 2e20 496e  instructions. In
-00011d60: 204d 5356 4320 6275 696c 6420 2873 7461   MSVC build (sta
-00011d70: 7469 6320 6c69 6e6b 292c 2074 6869 7320  tic link), this 
-00011d80: 6272 696e 6773 2073 6f6d 6520 7065 7266  brings some perf
-00011d90: 6f72 6d61 6e63 6520 696d 7072 6f76 656d  ormance improvem
-00011da0: 656e 7473 2e20 4743 432f 434c 414e 4720  ents. GCC/CLANG 
-00011db0: 6275 696c 6473 2061 6c72 6561 6479 2064  builds already d
-00011dc0: 796e 616d 6963 616c 6c79 2064 6973 7061  ynamically dispa
-00011dd0: 7463 6820 736f 6d65 2066 756e 6374 696f  tch some functio
-00011de0: 6e73 2066 6f72 2042 4d49 3220 696e 7374  ns for BMI2 inst
-00011df0: 7275 6374 696f 6e73 2c20 736f 206e 6f20  ructions, so no 
-00011e00: 7369 676e 6966 6963 616e 7420 696d 7072  significant impr
-00011e10: 6f76 656d 656e 742e 0a0a 2020 2020 2e2e  ovement...    ..
-00011e20: 2073 6f75 7263 6563 6f64 653a 3a20 7368   sourcecode:: sh
-00011e30: 656c 6c0a 0a20 2020 2020 2020 2023 20f0  ell..        # .
-00011e40: 9f9f a020 7079 7a73 7464 2030 2e31 352e  ... pyzstd 0.15.
-00011e50: 342b 2061 6e64 2070 6970 2032 322e 312b  4+ and pip 22.1+
-00011e60: 2073 7570 706f 7274 2050 4550 2d35 3137   support PEP-517
-00011e70: 3a0a 2020 2020 2020 2020 2320 6275 696c  :.        # buil
-00011e80: 6420 616e 6420 696e 7374 616c 6c0a 2020  d and install.  
-00011e90: 2020 2020 2020 7069 7020 696e 7374 616c        pip instal
-00011ea0: 6c20 2d2d 636f 6e66 6967 2d73 6574 7469  l --config-setti
-00011eb0: 6e67 733d 222d 2d62 7569 6c64 2d6f 7074  ngs="--build-opt
-00011ec0: 696f 6e3d 2d2d 6176 7832 2220 2d76 2070  ion=--avx2" -v p
-00011ed0: 797a 7374 642d 302e 3135 2e34 2e74 6172  yzstd-0.15.4.tar
-00011ee0: 2e67 7a0a 2020 2020 2020 2020 2320 6275  .gz.        # bu
-00011ef0: 696c 6420 6120 7265 6469 7374 7269 6275  ild a redistribu
-00011f00: 7461 626c 6520 7768 6565 6c0a 2020 2020  table wheel.    
-00011f10: 2020 2020 7069 7020 7768 6565 6c20 2d2d      pip wheel --
-00011f20: 636f 6e66 6967 2d73 6574 7469 6e67 733d  config-settings=
-00011f30: 222d 2d62 7569 6c64 2d6f 7074 696f 6e3d  "--build-option=
-00011f40: 2d2d 6176 7832 2220 2d76 2070 797a 7374  --avx2" -v pyzst
-00011f50: 642d 302e 3135 2e34 2e74 6172 2e67 7a0a  d-0.15.4.tar.gz.
-00011f60: 2020 2020 2020 2020 2320 f09f 9fa0 206c          # .... l
-00011f70: 6567 6163 7920 636f 6d6d 616e 6473 3a0a  egacy commands:.
-00011f80: 2020 2020 2020 2020 2320 6275 696c 6420          # build 
-00011f90: 616e 6420 696e 7374 616c 6c0a 2020 2020  and install.    
-00011fa0: 2020 2020 7079 7468 6f6e 2073 6574 7570      python setup
-00011fb0: 2e70 7920 696e 7374 616c 6c20 2d2d 6176  .py install --av
-00011fc0: 7832 0a20 2020 2020 2020 2023 2062 7569  x2.        # bui
-00011fd0: 6c64 2061 2072 6564 6973 7472 6962 7574  ld a redistribut
-00011fe0: 6162 6c65 2077 6865 656c 0a20 2020 2020  able wheel.     
-00011ff0: 2020 2070 7974 686f 6e20 7365 7475 702e     python setup.
-00012000: 7079 2062 6469 7374 5f77 6865 656c 202d  py bdist_wheel -
-00012010: 2d61 7678 320a 0a20 2020 2032 efb8 8fe2  -avx2..    2....
-00012020: 83a3 2050 797a 7374 6420 6d6f 6475 6c65  .. Pyzstd module
-00012030: 2073 7570 706f 7274 733a 0a0a 2020 2020   supports:..    
-00012040: 2020 2020 2a20 4479 6e61 6d69 6361 6c6c      * Dynamicall
-00012050: 7920 6c69 6e6b 2074 6f20 7a73 7464 206c  y link to zstd l
-00012060: 6962 7261 7279 2028 7072 6f76 6964 6564  ibrary (provided
-00012070: 2062 7920 7379 7374 656d 206f 7220 6120   by system or a 
-00012080: 444c 4c20 6c69 6272 6172 7929 2c20 7468  DLL library), th
-00012090: 656e 2074 6865 207a 7374 6420 736f 7572  en the zstd sour
-000120a0: 6365 2063 6f64 6520 696e 2060 607a 7374  ce code in ``zst
-000120b0: 6460 6020 666f 6c64 6572 2077 696c 6c20  d`` folder will 
-000120c0: 6265 2069 676e 6f72 6564 2e0a 2020 2020  be ignored..    
-000120d0: 2020 2020 2a20 5072 6f76 6964 6520 6120      * Provide a 
-000120e0: 6043 4646 4920 3c68 7474 7073 3a2f 2f64  `CFFI <https://d
-000120f0: 6f63 2e70 7970 792e 6f72 672f 656e 2f6c  oc.pypy.org/en/l
-00012100: 6174 6573 742f 6578 7465 6e64 696e 672e  atest/extending.
-00012110: 6874 6d6c 2363 6666 693e 605f 2069 6d70  html#cffi>`_ imp
-00012120: 6c65 6d65 6e74 6174 696f 6e20 7468 6174  lementation that
-00012130: 2063 616e 2077 6f72 6b20 7769 7468 2050   can work with P
-00012140: 7950 792e 0a0a 2020 2020 4f6e 2043 5079  yPy...    On CPy
-00012150: 7468 6f6e 2c20 7072 6f76 6964 6520 7468  thon, provide th
-00012160: 6573 6520 6275 696c 6420 6f70 7469 6f6e  ese build option
-00012170: 733a 0a0a 2020 2020 2020 2020 232e 206e  s:..        #. n
-00012180: 6f20 6f70 7469 6f6e 3a20 4320 696d 706c  o option: C impl
-00012190: 656d 656e 7461 7469 6f6e 2c20 7374 6174  ementation, stat
-000121a0: 6963 616c 6c79 206c 696e 6b20 746f 207a  ically link to z
-000121b0: 7374 6420 6c69 6272 6172 792e 0a20 2020  std library..   
-000121c0: 2020 2020 2023 2e20 6060 2d2d 6479 6e61       #. ``--dyna
-000121d0: 6d69 632d 6c69 6e6b 2d7a 7374 6460 603a  mic-link-zstd``:
-000121e0: 2043 2069 6d70 6c65 6d65 6e74 6174 696f   C implementatio
-000121f0: 6e2c 2064 796e 616d 6963 616c 6c79 206c  n, dynamically l
-00012200: 696e 6b20 746f 207a 7374 6420 6c69 6272  ink to zstd libr
-00012210: 6172 792e 0a20 2020 2020 2020 2023 2e20  ary..        #. 
-00012220: 6060 2d2d 6366 6669 6060 3a20 4346 4649  ``--cffi``: CFFI
-00012230: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-00012240: 2873 6c6f 7765 7229 2c20 7374 6174 6963  (slower), static
-00012250: 616c 6c79 206c 696e 6b20 746f 207a 7374  ally link to zst
-00012260: 6420 6c69 6272 6172 792e 0a20 2020 2020  d library..     
-00012270: 2020 2023 2e20 6060 2d2d 6366 6669 202d     #. ``--cffi -
-00012280: 2d64 796e 616d 6963 2d6c 696e 6b2d 7a73  -dynamic-link-zs
-00012290: 7464 6060 3a20 4346 4649 2069 6d70 6c65  td``: CFFI imple
-000122a0: 6d65 6e74 6174 696f 6e20 2873 6c6f 7765  mentation (slowe
-000122b0: 7229 2c20 6479 6e61 6d69 6361 6c6c 7920  r), dynamically 
-000122c0: 6c69 6e6b 2074 6f20 7a73 7464 206c 6962  link to zstd lib
-000122d0: 7261 7279 2e0a 0a20 2020 204f 6e20 5079  rary...    On Py
-000122e0: 5079 2c20 6f6e 6c79 2043 4646 4920 696d  Py, only CFFI im
-000122f0: 706c 656d 656e 7461 7469 6f6e 2063 616e  plementation can
-00012300: 2062 6520 7573 6564 2c20 736f 2060 602d   be used, so ``-
-00012310: 2d63 6666 6960 6020 6973 2061 6464 6564  -cffi`` is added
-00012320: 2069 6d70 6c69 6369 746c 792e 2060 602d   implicitly. ``-
-00012330: 2d64 796e 616d 6963 2d6c 696e 6b2d 7a73  -dynamic-link-zs
-00012340: 7464 6060 2069 7320 6f70 7469 6f6e 616c  td`` is optional
-00012350: 2e0a 0a20 2020 202e 2e20 736f 7572 6365  ...    .. source
-00012360: 636f 6465 3a3a 2073 6865 6c6c 0a0a 2020  code:: shell..  
-00012370: 2020 2020 2020 2320 f09f 9fa0 2070 797a        # .... pyz
-00012380: 7374 6420 302e 3135 2e34 2b20 616e 6420  std 0.15.4+ and 
-00012390: 7069 7020 3232 2e31 2b20 7375 7070 6f72  pip 22.1+ suppor
-000123a0: 7420 5045 502d 3531 373a 0a20 2020 2020  t PEP-517:.     
-000123b0: 2020 2023 2062 7569 6c64 2061 6e64 2069     # build and i
-000123c0: 6e73 7461 6c6c 0a20 2020 2020 2020 2070  nstall.        p
-000123d0: 6970 3320 696e 7374 616c 6c20 2d2d 636f  ip3 install --co
-000123e0: 6e66 6967 2d73 6574 7469 6e67 733d 222d  nfig-settings="-
-000123f0: 2d62 7569 6c64 2d6f 7074 696f 6e3d 2d2d  -build-option=--
-00012400: 6479 6e61 6d69 632d 6c69 6e6b 2d7a 7374  dynamic-link-zst
-00012410: 6422 202d 7620 7079 7a73 7464 2d30 2e31  d" -v pyzstd-0.1
-00012420: 352e 342e 7461 722e 677a 0a20 2020 2020  5.4.tar.gz.     
-00012430: 2020 2023 2062 7569 6c64 2061 2072 6564     # build a red
-00012440: 6973 7472 6962 7574 6162 6c65 2077 6865  istributable whe
-00012450: 656c 0a20 2020 2020 2020 2070 6970 3320  el.        pip3 
-00012460: 7768 6565 6c20 2d2d 636f 6e66 6967 2d73  wheel --config-s
-00012470: 6574 7469 6e67 733d 222d 2d62 7569 6c64  ettings="--build
-00012480: 2d6f 7074 696f 6e3d 2d2d 6479 6e61 6d69  -option=--dynami
-00012490: 632d 6c69 6e6b 2d7a 7374 6422 202d 7620  c-link-zstd" -v 
-000124a0: 7079 7a73 7464 2d30 2e31 352e 342e 7461  pyzstd-0.15.4.ta
-000124b0: 722e 677a 0a20 2020 2020 2020 2023 2073  r.gz.        # s
-000124c0: 7065 6369 6679 206d 6f72 6520 7468 616e  pecify more than
-000124d0: 206f 6e65 206f 7074 696f 6e0a 2020 2020   one option.    
-000124e0: 2020 2020 7069 7033 2077 6865 656c 202d      pip3 wheel -
-000124f0: 2d63 6f6e 6669 672d 7365 7474 696e 6773  -config-settings
-00012500: 3d22 2d2d 6275 696c 642d 6f70 7469 6f6e  ="--build-option
-00012510: 3d2d 2d64 796e 616d 6963 2d6c 696e 6b2d  =--dynamic-link-
-00012520: 7a73 7464 202d 2d63 6666 6922 202d 7620  zstd --cffi" -v 
-00012530: 7079 7a73 7464 2d30 2e31 352e 342e 7461  pyzstd-0.15.4.ta
-00012540: 722e 677a 0a20 2020 2020 2020 2023 20f0  r.gz.        # .
-00012550: 9f9f a020 6c65 6761 6379 2063 6f6d 6d61  ... legacy comma
-00012560: 6e64 733a 0a20 2020 2020 2020 2023 2062  nds:.        # b
-00012570: 7569 6c64 2061 6e64 2069 6e73 7461 6c6c  uild and install
-00012580: 0a20 2020 2020 2020 2070 7974 686f 6e33  .        python3
-00012590: 2073 6574 7570 2e70 7920 696e 7374 616c   setup.py instal
-000125a0: 6c20 2d2d 6479 6e61 6d69 632d 6c69 6e6b  l --dynamic-link
-000125b0: 2d7a 7374 640a 2020 2020 2020 2020 2320  -zstd.        # 
-000125c0: 6275 696c 6420 6120 7265 6469 7374 7269  build a redistri
-000125d0: 6275 7461 626c 6520 7768 6565 6c0a 2020  butable wheel.  
-000125e0: 2020 2020 2020 7079 7468 6f6e 3320 7365        python3 se
-000125f0: 7475 702e 7079 2062 6469 7374 5f77 6865  tup.py bdist_whe
-00012600: 656c 202d 2d64 796e 616d 6963 2d6c 696e  el --dynamic-lin
-00012610: 6b2d 7a73 7464 0a0a 2020 2020 536f 6d65  k-zstd..    Some
-00012620: 206e 6f74 6573 3a0a 0a20 2020 2020 2020   notes:..       
-00012630: 202a 2054 6865 2077 6865 656c 7320 6f6e   * The wheels on
-00012640: 2060 5079 5049 203c 6874 7470 733a 2f2f   `PyPI <https://
-00012650: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00012660: 2f70 797a 7374 643e 605f 2075 7365 2073  /pyzstd>`_ use s
-00012670: 7461 7469 6320 6c69 6e6b 696e 672c 2074  tatic linking, t
-00012680: 6865 2070 6163 6b61 6765 7320 6f6e 2060  he packages on `
-00012690: 416e 6163 6f6e 6461 203c 6874 7470 733a  Anaconda <https:
-000126a0: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f63  //anaconda.org/c
-000126b0: 6f6e 6461 2d66 6f72 6765 2f70 797a 7374  onda-forge/pyzst
-000126c0: 643e 605f 2075 7365 2064 796e 616d 6963  d>`_ use dynamic
-000126d0: 206c 696e 6b69 6e67 2e0a 2020 2020 2020   linking..      
-000126e0: 2020 2a20 4e6f 206d 6174 7465 7220 7374    * No matter st
-000126f0: 6174 6963 206f 7220 6479 6e61 6d69 6320  atic or dynamic 
-00012700: 6c69 6e6b 696e 672c 2070 797a 7374 6420  linking, pyzstd 
-00012710: 6d6f 6475 6c65 2072 6571 7569 7265 7320  module requires 
-00012720: 7a73 7464 2076 312e 342e 302b 2e0a 2020  zstd v1.4.0+..  
-00012730: 2020 2020 2020 2a20 5374 6174 6963 206c        * Static l
-00012740: 696e 6b69 6e67 3a20 5573 6520 7a73 7464  inking: Use zstd
-00012750: 2773 206f 6666 6963 6961 6c20 7265 6c65  's official rele
-00012760: 6173 6520 7769 7468 6f75 7420 616e 7920  ase without any 
-00012770: 6368 616e 6765 2e20 4966 2077 616e 7420  change. If want 
-00012780: 746f 2075 7067 7261 6465 206f 7220 646f  to upgrade or do
-00012790: 776e 6772 6164 6520 7468 6520 7a73 7464  wngrade the zstd
-000127a0: 206c 6962 7261 7279 2c20 6a75 7374 2072   library, just r
-000127b0: 6570 6c61 6365 2060 607a 7374 6460 6020  eplace ``zstd`` 
-000127c0: 666f 6c64 6572 2e0a 2020 2020 2020 2020  folder..        
-000127d0: 2a20 4479 6e61 6d69 6320 6c69 6e6b 696e  * Dynamic linkin
-000127e0: 673a 2049 6620 6e65 7720 7a73 7464 2041  g: If new zstd A
-000127f0: 5049 2069 7320 7573 6564 2061 7420 636f  PI is used at co
-00012800: 6d70 696c 652d 7469 6d65 2c20 6c69 6e6b  mpile-time, link
-00012810: 696e 6720 746f 206c 6f77 6572 2076 6572  ing to lower ver
-00012820: 7369 6f6e 2072 756e 2d74 696d 6520 7a73  sion run-time zs
-00012830: 7464 206c 6962 7261 7279 2077 696c 6c20  td library will 
-00012840: 6661 696c 2e20 5573 6520 7631 2e35 2e30  fail. Use v1.5.0
-00012850: 206e 6577 2041 5049 2069 6620 706f 7373   new API if poss
-00012860: 6962 6c65 2e0a 0a20 2020 204f 6e20 5769  ible...    On Wi
-00012870: 6e64 6f77 732c 2074 6865 7265 2069 7320  ndows, there is 
-00012880: 6e6f 2073 7973 7465 6d2d 7769 6465 207a  no system-wide z
-00012890: 7374 6420 6c69 6272 6172 792e 2050 797a  std library. Pyz
-000128a0: 7374 6420 6d6f 6475 6c65 2063 616e 2064  std module can d
-000128b0: 796e 616d 6963 616c 6c79 206c 696e 6b20  ynamically link 
-000128c0: 746f 2061 2044 4c4c 206c 6962 7261 7279  to a DLL library
-000128d0: 2c20 6d6f 6469 6679 2060 6073 6574 7570  , modify ``setup
-000128e0: 2e70 7960 603a 0a0a 2020 2020 2e2e 2073  .py``:..    .. s
-000128f0: 6f75 7263 6563 6f64 653a 3a20 7079 7468  ourcecode:: pyth
-00012900: 6f6e 0a0a 2020 2020 2020 2020 2320 453a  on..        # E:
-00012910: 5c7a 7374 645f 646c 6c20 666f 6c64 6572  \zstd_dll folder
-00012920: 2068 6173 207a 7374 642e 6820 2f20 7a64   has zstd.h / zd
-00012930: 6963 742e 6820 2f20 6c69 627a 7374 642e  ict.h / libzstd.
-00012940: 6c69 6220 7468 6174 0a20 2020 2020 2020  lib that.       
-00012950: 2023 2061 6c6f 6e67 2077 6974 6820 6c69   # along with li
-00012960: 627a 7374 642e 646c 6c0a 2020 2020 2020  bzstd.dll.      
-00012970: 2020 6966 2044 594e 414d 4943 5f4c 494e    if DYNAMIC_LIN
-00012980: 4b3a 0a20 2020 2020 2020 2020 2020 206b  K:.            k
-00012990: 7761 7267 7320 3d20 7b0a 2020 2020 2020  wargs = {.      
-000129a0: 2020 2020 2020 2769 6e63 6c75 6465 5f64        'include_d
-000129b0: 6972 7327 3a20 5b27 453a 5c7a 7374 645f  irs': ['E:\zstd_
-000129c0: 646c 6c27 5d2c 2023 202e 6820 6469 7265  dll'], # .h dire
-000129d0: 6374 6f72 790a 2020 2020 2020 2020 2020  ctory.          
-000129e0: 2020 276c 6962 7261 7279 5f64 6972 7327    'library_dirs'
-000129f0: 3a20 5b27 453a 5c7a 7374 645f 646c 6c27  : ['E:\zstd_dll'
-00012a00: 5d2c 2023 202e 6c69 6220 6469 7265 6374  ], # .lib direct
-00012a10: 6f72 790a 2020 2020 2020 2020 2020 2020  ory.            
-00012a20: 276c 6962 7261 7269 6573 273a 205b 276c  'libraries': ['l
-00012a30: 6962 7a73 7464 275d 2c20 2020 2020 2020  ibzstd'],       
-00012a40: 2023 206c 6962 206e 616d 652c 206e 6f74   # lib name, not
-00012a50: 2066 696c 656e 616d 652c 2066 6f72 2074   filename, for t
-00012a60: 6865 206c 696e 6b65 722e 0a20 2020 2020  he linker..     
-00012a70: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
-00012a80: 416e 6420 7075 7420 6060 6c69 627a 7374  And put ``libzst
-00012a90: 642e 646c 6c60 6020 696e 746f 206f 6e65  d.dll`` into one
-00012aa0: 206f 6620 7468 6573 6520 6469 7265 6374   of these direct
-00012ab0: 6f72 6965 733a 0a0a 2020 2020 2020 2020  ories:..        
-00012ac0: 2a20 4469 7265 6374 6f72 7920 6164 6465  * Directory adde
-00012ad0: 6420 6279 2060 6f73 2e61 6464 5f64 6c6c  d by `os.add_dll
-00012ae0: 5f64 6972 6563 746f 7279 2829 203c 6874  _directory() <ht
-00012af0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00012b00: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-00012b10: 6f73 2e68 746d 6c23 6f73 2e61 6464 5f64  os.html#os.add_d
-00012b20: 6c6c 5f64 6972 6563 746f 7279 3e60 5f20  ll_directory>`_ 
-00012b30: 6675 6e63 7469 6f6e 2e20 2854 6865 2075  function. (The u
-00012b40: 6e69 742d 7465 7374 7320 616e 6420 7468  nit-tests and th
-00012b50: 6520 434c 4920 6361 6e27 7420 7574 696c  e CLI can't util
-00012b60: 697a 6520 7468 6973 290a 2020 2020 2020  ize this).      
-00012b70: 2020 2a20 5079 7468 6f6e 2773 2072 6f6f    * Python's roo
-00012b80: 7420 6469 7265 6374 6f72 7920 7468 6174  t directory that
-00012b90: 2068 6173 2070 7974 686f 6e2e 6578 652e   has python.exe.
-00012ba0: 0a20 2020 2020 2020 202a 2025 5379 7374  .        * %Syst
-00012bb0: 656d 526f 6f74 255c 5379 7374 656d 3332  emRoot%\System32
-00012bc0: 0a0a 2020 2020 4e6f 7465 2074 6861 7420  ..    Note that 
-00012bd0: 7468 6520 6162 6f76 6520 6c69 7374 2064  the above list d
-00012be0: 6f65 736e 2774 2069 6e63 6c75 6465 2074  oesn't include t
-00012bf0: 6865 2063 7572 7265 6e74 2077 6f72 6b69  he current worki
-00012c00: 6e67 2064 6972 6563 746f 7279 2061 6e64  ng directory and
-00012c10: 2025 5041 5448 2520 6469 7265 6374 6f72   %PATH% director
-00012c20: 6965 732e 0a0a 2020 2020 33ef b88f e283  ies...    3.....
-00012c30: a320 5573 6520 226d 756c 7469 2d70 6861  . Use "multi-pha
-00012c40: 7365 2069 6e69 7469 616c 697a 6174 696f  se initializatio
-00012c50: 6e22 206f 6e20 4350 7974 686f 6e2e 0a0a  n" on CPython...
-00012c60: 2020 2020 4966 2070 726f 7669 6465 2060      If provide `
-00012c70: 602d 2d6d 756c 7469 2d70 6861 7365 2d69  `--multi-phase-i
-00012c80: 6e69 7460 6020 6275 696c 6420 6f70 7469  nit`` build opti
-00012c90: 6f6e 2c20 6974 2077 696c 6c20 6275 696c  on, it will buil
-00012ca0: 6420 7769 7468 2022 6d75 6c74 692d 7068  d with "multi-ph
-00012cb0: 6173 6520 696e 6974 6961 6c69 7a61 7469  ase initializati
-00012cc0: 6f6e 2220 2860 5045 502d 3438 3920 3c68  on" (`PEP-489 <h
-00012cd0: 7474 7073 3a2f 2f70 6570 732e 7079 7468  ttps://peps.pyth
-00012ce0: 6f6e 2e6f 7267 2f70 6570 2d30 3438 392f  on.org/pep-0489/
-00012cf0: 3e60 5f29 206f 6e20 4350 7974 686f 6e20  >`_) on CPython 
-00012d00: 332e 3131 2b2e 0a0a 2020 2020 5369 6e63  3.11+...    Sinc
-00012d10: 6520 6974 2061 6464 7320 6120 7469 6e79  e it adds a tiny
-00012d20: 206f 7665 7268 6561 642c 2069 7427 7320   overhead, it's 
-00012d30: 6469 7361 626c 6564 2062 7920 6465 6661  disabled by defa
-00012d40: 756c 742e 2049 7420 6361 6e20 6265 2065  ult. It can be e
-00012d50: 6e61 626c 6564 2061 6674 6572 2043 5079  nabled after CPy
-00012d60: 7468 6f6e 2773 2060 7375 622d 696e 7465  thon's `sub-inte
-00012d70: 7270 7265 7465 7273 203c 6874 7470 733a  rpreters <https:
-00012d80: 2f2f 7065 7073 2e70 7974 686f 6e2e 6f72  //peps.python.or
-00012d90: 672f 7065 702d 3035 3534 2f3e 605f 2069  g/pep-0554/>`_ i
-00012da0: 7320 6d61 7475 7265 2e0a                 s mature..
+00009ff0: 4275 6666 6572 6564 494f 4261 7365 2e77  BufferedIOBase.w
+0000a000: 7269 7465 3e60 5f0a 2020 2020 2020 2020  rite>`_.        
+0000a010: 2a20 602e 666c 7573 6828 6d6f 6465 3d5a  * `.flush(mode=Z
+0000a020: 7374 6446 696c 652e 464c 5553 485f 424c  stdFile.FLUSH_BL
+0000a030: 4f43 4b29 203c 6874 7470 733a 2f2f 646f  OCK) <https://do
+0000a040: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+0000a050: 6c69 6272 6172 792f 696f 2e68 746d 6c23  library/io.html#
+0000a060: 696f 2e49 4f42 6173 652e 666c 7573 683e  io.IOBase.flush>
+0000a070: 605f 2c20 666c 7573 6820 746f 2074 6865  `_, flush to the
+0000a080: 2075 6e64 6572 6c79 696e 6720 7374 7265   underlying stre
+0000a090: 616d 2e20 5468 6520 2a6d 6f64 652a 2061  am. The *mode* a
+0000a0a0: 7267 756d 656e 7420 6361 6e20 6265 2060  rgument can be `
+0000a0b0: 605a 7374 6446 696c 652e 464c 5553 485f  `ZstdFile.FLUSH_
+0000a0c0: 424c 4f43 4b60 602c 2060 605a 7374 6446  BLOCK``, ``ZstdF
+0000a0d0: 696c 652e 464c 5553 485f 4652 414d 4560  ile.FLUSH_FRAME`
+0000a0e0: 602e 2041 6275 7365 206f 6620 7468 6973  `. Abuse of this
+0000a0f0: 206d 6574 686f 6420 7769 6c6c 2072 6564   method will red
+0000a100: 7563 6520 636f 6d70 7265 7373 696f 6e20  uce compression 
+0000a110: 7261 7469 6f2c 2075 7365 2069 7420 6f6e  ratio, use it on
+0000a120: 6c79 2077 6865 6e20 6e65 6365 7373 6172  ly when necessar
+0000a130: 792e 2049 6620 7468 6520 7072 6f67 7261  y. If the progra
+0000a140: 6d20 6973 2069 6e74 6572 7275 7074 6564  m is interrupted
+0000a150: 2061 6674 6572 7761 7264 732c 2061 6c6c   afterwards, all
+0000a160: 2064 6174 6120 6361 6e20 6265 2072 6563   data can be rec
+0000a170: 6f76 6572 6564 2e20 546f 2065 6e73 7572  overed. To ensur
+0000a180: 6520 7361 7669 6e67 2074 6f20 6469 736b  e saving to disk
+0000a190: 2c20 616c 736f 206e 6565 6420 606f 732e  , also need `os.
+0000a1a0: 6673 796e 6328 6664 2920 3c68 7474 7073  fsync(fd) <https
+0000a1b0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+0000a1c0: 7267 2f33 2f6c 6962 7261 7279 2f6f 732e  rg/3/library/os.
+0000a1d0: 6874 6d6c 236f 732e 6673 796e 633e 605f  html#os.fsync>`_
+0000a1e0: 2e20 2028 2a41 6464 6564 2069 6e20 7665  .  (*Added in ve
+0000a1f0: 7273 696f 6e20 302e 3135 2e31 2c20 6164  rsion 0.15.1, ad
+0000a200: 6465 6420 6d6f 6465 2061 7267 756d 656e  ded mode argumen
+0000a210: 7420 696e 2076 6572 7369 6f6e 2030 2e31  t in version 0.1
+0000a220: 352e 382e 2a29 0a0a 2020 2020 496e 2062  5.8.*)..    In b
+0000a230: 6f74 6820 7265 6164 696e 6720 616e 6420  oth reading and 
+0000a240: 7772 6974 696e 6720 6d6f 6465 732c 2074  writing modes, t
+0000a250: 6865 7365 206d 6574 686f 6473 2061 6e64  hese methods and
+0000a260: 2070 726f 7065 7274 7920 6172 6520 6176   property are av
+0000a270: 6169 6c61 626c 653a 0a0a 2020 2020 2020  ailable:..      
+0000a280: 2020 2a20 602e 636c 6f73 6528 2920 3c68    * `.close() <h
+0000a290: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
+0000a2a0: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
+0000a2b0: 2f69 6f2e 6874 6d6c 2369 6f2e 494f 4261  /io.html#io.IOBa
+0000a2c0: 7365 2e63 6c6f 7365 3e60 5f0a 2020 2020  se.close>`_.    
+0000a2d0: 2020 2020 2a20 602e 7465 6c6c 2829 203c      * `.tell() <
+0000a2e0: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
+0000a2f0: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
+0000a300: 792f 696f 2e68 746d 6c23 696f 2e49 4f42  y/io.html#io.IOB
+0000a310: 6173 652e 7465 6c6c 3e60 5f2c 2072 6574  ase.tell>`_, ret
+0000a320: 7572 6e20 7468 6520 6375 7272 656e 7420  urn the current 
+0000a330: 706f 7369 7469 6f6e 206f 6620 756e 636f  position of unco
+0000a340: 6d70 7265 7373 6564 2063 6f6e 7465 6e74  mpressed content
+0000a350: 2e20 496e 2061 7070 656e 6420 6d6f 6465  . In append mode
+0000a360: 2c20 7468 6520 696e 6974 6961 6c20 706f  , the initial po
+0000a370: 7369 7469 6f6e 2069 7320 302e 0a20 2020  sition is 0..   
+0000a380: 2020 2020 202a 2060 2e66 696c 656e 6f28       * `.fileno(
+0000a390: 2920 3c68 7474 7073 3a2f 2f64 6f63 732e  ) <https://docs.
+0000a3a0: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+0000a3b0: 7261 7279 2f69 6f2e 6874 6d6c 2369 6f2e  rary/io.html#io.
+0000a3c0: 494f 4261 7365 2e66 696c 656e 6f3e 605f  IOBase.fileno>`_
+0000a3d0: 0a20 2020 2020 2020 202a 2060 2e63 6c6f  .        * `.clo
+0000a3e0: 7365 6420 3c68 7474 7073 3a2f 2f64 6f63  sed <https://doc
+0000a3f0: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+0000a400: 6962 7261 7279 2f69 6f2e 6874 6d6c 2369  ibrary/io.html#i
+0000a410: 6f2e 494f 4261 7365 2e63 6c6f 7365 643e  o.IOBase.closed>
+0000a420: 605f 2028 6120 7072 6f70 6572 7479 2061  `_ (a property a
+0000a430: 7474 7269 6275 7465 290a 2020 2020 2020  ttribute).      
+0000a440: 2020 2a20 602e 7772 6974 6162 6c65 2829    * `.writable()
+0000a450: 203c 6874 7470 733a 2f2f 646f 6373 2e70   <https://docs.p
+0000a460: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
+0000a470: 6172 792f 696f 2e68 746d 6c23 696f 2e49  ary/io.html#io.I
+0000a480: 4f42 6173 652e 7772 6974 6162 6c65 3e60  OBase.writable>`
+0000a490: 5f0a 2020 2020 2020 2020 2a20 602e 7265  _.        * `.re
+0000a4a0: 6164 6162 6c65 2829 203c 6874 7470 733a  adable() <https:
+0000a4b0: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
+0000a4c0: 672f 332f 6c69 6272 6172 792f 696f 2e68  g/3/library/io.h
+0000a4d0: 746d 6c23 696f 2e49 4f42 6173 652e 7265  tml#io.IOBase.re
+0000a4e0: 6164 6162 6c65 3e60 5f0a 2020 2020 2020  adable>`_.      
+0000a4f0: 2020 2a20 602e 7365 656b 6162 6c65 2829    * `.seekable()
+0000a500: 203c 6874 7470 733a 2f2f 646f 6373 2e70   <https://docs.p
+0000a510: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
+0000a520: 6172 792f 696f 2e68 746d 6c23 696f 2e49  ary/io.html#io.I
+0000a530: 4f42 6173 652e 7365 656b 6162 6c65 3e60  OBase.seekable>`
+0000a540: 5f0a 0a2e 2e20 7079 3a66 756e 6374 696f  _.... py:functio
+0000a550: 6e3a 3a20 6f70 656e 2866 696c 656e 616d  n:: open(filenam
+0000a560: 652c 206d 6f64 653d 2272 6222 2c20 2a2c  e, mode="rb", *,
+0000a570: 206c 6576 656c 5f6f 725f 6f70 7469 6f6e   level_or_option
+0000a580: 3d4e 6f6e 652c 207a 7374 645f 6469 6374  =None, zstd_dict
+0000a590: 3d4e 6f6e 652c 2065 6e63 6f64 696e 673d  =None, encoding=
+0000a5a0: 4e6f 6e65 2c20 6572 726f 7273 3d4e 6f6e  None, errors=Non
+0000a5b0: 652c 206e 6577 6c69 6e65 3d4e 6f6e 6529  e, newline=None)
+0000a5c0: 0a0a 2020 2020 4f70 656e 2061 207a 7374  ..    Open a zst
+0000a5d0: 642d 636f 6d70 7265 7373 6564 2066 696c  d-compressed fil
+0000a5e0: 6520 696e 2062 696e 6172 7920 6f72 2074  e in binary or t
+0000a5f0: 6578 7420 6d6f 6465 2c20 7265 7475 726e  ext mode, return
+0000a600: 696e 6720 6120 6669 6c65 206f 626a 6563  ing a file objec
+0000a610: 742e 0a0a 2020 2020 5468 6973 2066 756e  t...    This fun
+0000a620: 6374 696f 6e20 6973 2076 6572 7920 7369  ction is very si
+0000a630: 6d69 6c61 7220 746f 2060 627a 322e 6f70  milar to `bz2.op
+0000a640: 656e 2829 203c 6874 7470 733a 2f2f 646f  en() <https://do
+0000a650: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+0000a660: 6c69 6272 6172 792f 627a 322e 6874 6d6c  library/bz2.html
+0000a670: 2362 7a32 2e6f 7065 6e3e 605f 202f 2060  #bz2.open>`_ / `
+0000a680: 677a 6970 2e6f 7065 6e28 2920 3c68 7474  gzip.open() <htt
+0000a690: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+0000a6a0: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f67  .org/3/library/g
+0000a6b0: 7a69 702e 6874 6d6c 2367 7a69 702e 6f70  zip.html#gzip.op
+0000a6c0: 656e 3e60 5f20 2f20 606c 7a6d 612e 6f70  en>`_ / `lzma.op
+0000a6d0: 656e 2829 203c 6874 7470 733a 2f2f 646f  en() <https://do
+0000a6e0: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+0000a6f0: 6c69 6272 6172 792f 6c7a 6d61 2e68 746d  library/lzma.htm
+0000a700: 6c23 6c7a 6d61 2e6f 7065 6e3e 605f 2066  l#lzma.open>`_ f
+0000a710: 756e 6374 696f 6e73 2069 6e20 5079 7468  unctions in Pyth
+0000a720: 6f6e 2073 7461 6e64 6172 6420 6c69 6272  on standard libr
+0000a730: 6172 792e 0a0a 2020 2020 5468 6520 2a66  ary...    The *f
+0000a740: 696c 656e 616d 652a 2070 6172 616d 6574  ilename* paramet
+0000a750: 6572 2063 616e 2062 6520 616e 2065 7869  er can be an exi
+0000a760: 7374 696e 6720 6066 696c 6520 6f62 6a65  sting `file obje
+0000a770: 6374 203c 6874 7470 733a 2f2f 646f 6373  ct <https://docs
+0000a780: 2e70 7974 686f 6e2e 6f72 672f 332f 676c  .python.org/3/gl
+0000a790: 6f73 7361 7279 2e68 746d 6c23 7465 726d  ossary.html#term
+0000a7a0: 2d66 696c 652d 6f62 6a65 6374 3e60 5f20  -file-object>`_ 
+0000a7b0: 746f 2077 7261 702c 206f 7220 7468 6520  to wrap, or the 
+0000a7c0: 6e61 6d65 206f 6620 7468 6520 6669 6c65  name of the file
+0000a7d0: 2074 6f20 6f70 656e 2028 6173 2061 2060   to open (as a `
+0000a7e0: 6073 7472 6060 2c20 6060 6279 7465 7360  `str``, ``bytes`
+0000a7f0: 6020 6f72 2060 7061 7468 2d6c 696b 6520  ` or `path-like 
+0000a800: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
+0000a810: 7468 6f6e 2e6f 7267 2f33 2f67 6c6f 7373  thon.org/3/gloss
+0000a820: 6172 792e 6874 6d6c 2374 6572 6d2d 7061  ary.html#term-pa
+0000a830: 7468 2d6c 696b 652d 6f62 6a65 6374 3e60  th-like-object>`
+0000a840: 5f20 6f62 6a65 6374 292e 2057 6865 6e20  _ object). When 
+0000a850: 7772 6170 7069 6e67 2061 6e20 6578 6973  wrapping an exis
+0000a860: 7469 6e67 2066 696c 6520 6f62 6a65 6374  ting file object
+0000a870: 2c20 7468 6520 7772 6170 7065 6420 6669  , the wrapped fi
+0000a880: 6c65 2077 696c 6c20 6e6f 7420 6265 2063  le will not be c
+0000a890: 6c6f 7365 6420 7768 656e 2074 6865 2072  losed when the r
+0000a8a0: 6574 7572 6e65 6420 6669 6c65 206f 626a  eturned file obj
+0000a8b0: 6563 7420 6973 2063 6c6f 7365 642e 0a0a  ect is closed...
+0000a8c0: 2020 2020 5468 6520 2a6d 6f64 652a 2070      The *mode* p
+0000a8d0: 6172 616d 6574 6572 2063 616e 2062 6520  arameter can be 
+0000a8e0: 616e 7920 6f66 2022 7222 2c20 2272 6222  any of "r", "rb"
+0000a8f0: 2c20 2277 222c 2022 7762 222c 2022 7822  , "w", "wb", "x"
+0000a900: 2c20 2278 6222 2c20 2261 2220 6f72 2022  , "xb", "a" or "
+0000a910: 6162 2220 666f 7220 6269 6e61 7279 206d  ab" for binary m
+0000a920: 6f64 652c 206f 7220 2272 7422 2c20 2277  ode, or "rt", "w
+0000a930: 7422 2c20 2278 7422 2c20 6f72 2022 6174  t", "xt", or "at
+0000a940: 2220 666f 7220 7465 7874 206d 6f64 652e  " for text mode.
+0000a950: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
+0000a960: 2272 6222 2e0a 0a20 2020 2049 6620 696e  "rb"...    If in
+0000a970: 2072 6561 6469 6e67 206d 6f64 6520 2864   reading mode (d
+0000a980: 6563 6f6d 7072 6573 7369 6f6e 292c 2074  ecompression), t
+0000a990: 6865 202a 6c65 7665 6c5f 6f72 5f6f 7074  he *level_or_opt
+0000a9a0: 696f 6e2a 2070 6172 616d 6574 6572 2063  ion* parameter c
+0000a9b0: 616e 206f 6e6c 7920 6265 2061 2060 6064  an only be a ``d
+0000a9c0: 6963 7460 6020 6f62 6a65 6374 2c20 7468  ict`` object, th
+0000a9d0: 6174 2072 6570 7265 7365 6e74 7320 6465  at represents de
+0000a9e0: 636f 6d70 7265 7373 696f 6e20 6f70 7469  compression opti
+0000a9f0: 6f6e 2e20 4974 2064 6f65 736e 2774 2073  on. It doesn't s
+0000aa00: 7570 706f 7274 2060 6069 6e74 6060 2074  upport ``int`` t
+0000aa10: 7970 6520 636f 6d70 7265 7373 696f 6e20  ype compression 
+0000aa20: 6c65 7665 6c20 696e 2074 6869 7320 6361  level in this ca
+0000aa30: 7365 2e0a 0a20 2020 2049 6e20 6269 6e61  se...    In bina
+0000aa40: 7279 206d 6f64 652c 2061 203a 7079 3a63  ry mode, a :py:c
+0000aa50: 6c61 7373 3a60 5a73 7464 4669 6c65 6020  lass:`ZstdFile` 
+0000aa60: 6f62 6a65 6374 2069 7320 7265 7475 726e  object is return
+0000aa70: 6564 2e0a 0a20 2020 2049 6e20 7465 7874  ed...    In text
+0000aa80: 206d 6f64 652c 2061 203a 7079 3a63 6c61   mode, a :py:cla
+0000aa90: 7373 3a60 5a73 7464 4669 6c65 6020 6f62  ss:`ZstdFile` ob
+0000aaa0: 6a65 6374 2069 7320 6372 6561 7465 642c  ject is created,
+0000aab0: 2061 6e64 2077 7261 7070 6564 2069 6e20   and wrapped in 
+0000aac0: 616e 2060 696f 2e54 6578 7449 4f57 7261  an `io.TextIOWra
+0000aad0: 7070 6572 203c 6874 7470 733a 2f2f 646f  pper <https://do
+0000aae0: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+0000aaf0: 6c69 6272 6172 792f 696f 2e68 746d 6c23  library/io.html#
+0000ab00: 696f 2e54 6578 7449 4f57 7261 7070 6572  io.TextIOWrapper
+0000ab10: 3e60 5f20 6f62 6a65 6374 2077 6974 6820  >`_ object with 
+0000ab20: 7468 6520 7370 6563 6966 6965 6420 656e  the specified en
+0000ab30: 636f 6469 6e67 2c20 6572 726f 7220 6861  coding, error ha
+0000ab40: 6e64 6c69 6e67 2062 6568 6176 696f 722c  ndling behavior,
+0000ab50: 2061 6e64 206c 696e 6520 656e 6469 6e67   and line ending
+0000ab60: 2873 292e 0a0a 5365 656b 6162 6c65 5a73  (s)...SeekableZs
+0000ab70: 7464 4669 6c65 2063 6c61 7373 0a2d 2d2d  tdFile class.---
+0000ab80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ab90: 2d2d 2d0a 0a20 2020 2054 6869 7320 7365  ---..    This se
+0000aba0: 6374 696f 6e20 636f 6e74 6169 6e73 2066  ction contains f
+0000abb0: 6163 696c 6974 6965 7320 7468 6174 2073  acilities that s
+0000abc0: 7570 706f 7274 696e 6720 605a 7374 616e  upporting `Zstan
+0000abd0: 6461 7264 2053 6565 6b61 626c 6520 466f  dard Seekable Fo
+0000abe0: 726d 6174 203c 6874 7470 733a 2f2f 6769  rmat <https://gi
+0000abf0: 7468 7562 2e63 6f6d 2f66 6163 6562 6f6f  thub.com/faceboo
+0000ac00: 6b2f 7a73 7464 2f62 6c6f 622f 6465 762f  k/zstd/blob/dev/
+0000ac10: 636f 6e74 7269 622f 7365 656b 6162 6c65  contrib/seekable
+0000ac20: 5f66 6f72 6d61 742f 7a73 7464 5f73 6565  _format/zstd_see
+0000ac30: 6b61 626c 655f 636f 6d70 7265 7373 696f  kable_compressio
+0000ac40: 6e5f 666f 726d 6174 2e6d 643e 605f 3a0a  n_format.md>`_:.
+0000ac50: 0a20 2020 2020 2020 202a 2065 7863 6570  .        * excep
+0000ac60: 7469 6f6e 203a 7079 3a63 6c61 7373 3a60  tion :py:class:`
+0000ac70: 5365 656b 6162 6c65 466f 726d 6174 4572  SeekableFormatEr
+0000ac80: 726f 7260 0a20 2020 2020 2020 202a 2063  ror`.        * c
+0000ac90: 6c61 7373 203a 7079 3a63 6c61 7373 3a60  lass :py:class:`
+0000aca0: 5365 656b 6162 6c65 5a73 7464 4669 6c65  SeekableZstdFile
+0000acb0: 600a 0a2e 2e20 7079 3a65 7863 6570 7469  `.... py:excepti
+0000acc0: 6f6e 3a3a 2053 6565 6b61 626c 6546 6f72  on:: SeekableFor
+0000acd0: 6d61 7445 7272 6f72 0a0a 2020 2020 416e  matError..    An
+0000ace0: 2065 7272 6f72 2072 656c 6174 6564 2074   error related t
+0000acf0: 6f20 225a 7374 616e 6461 7264 2053 6565  o "Zstandard See
+0000ad00: 6b61 626c 6520 466f 726d 6174 222e 2053  kable Format". S
+0000ad10: 7562 636c 6173 7320 6f66 2060 6045 7863  ubclass of ``Exc
+0000ad20: 6570 7469 6f6e 6060 2e0a 0a20 2020 202e  eption``...    .
+0000ad30: 2e20 7665 7273 696f 6e61 6464 6564 3a3a  . versionadded::
+0000ad40: 2030 2e31 352e 380a 0a2e 2e20 7079 3a63   0.15.8.... py:c
+0000ad50: 6c61 7373 3a3a 2053 6565 6b61 626c 655a  lass:: SeekableZ
+0000ad60: 7374 6446 696c 650a 0a20 2020 2053 7562  stdFile..    Sub
+0000ad70: 636c 6173 7320 6f66 203a 7079 3a63 6c61  class of :py:cla
+0000ad80: 7373 3a60 5a73 7464 4669 6c65 602e 2054  ss:`ZstdFile`. T
+0000ad90: 6869 7320 636c 6173 7320 6361 6e20 2a2a  his class can **
+0000ada0: 6f6e 6c79 2a2a 2063 7265 6174 652f 7772  only** create/wr
+0000adb0: 6974 652f 7265 6164 2060 5a73 7461 6e64  ite/read `Zstand
+0000adc0: 6172 6420 5365 656b 6162 6c65 2046 6f72  ard Seekable For
+0000add0: 6d61 7420 3c68 7474 7073 3a2f 2f67 6974  mat <https://git
+0000ade0: 6875 622e 636f 6d2f 6661 6365 626f 6f6b  hub.com/facebook
+0000adf0: 2f7a 7374 642f 626c 6f62 2f64 6576 2f63  /zstd/blob/dev/c
+0000ae00: 6f6e 7472 6962 2f73 6565 6b61 626c 655f  ontrib/seekable_
+0000ae10: 666f 726d 6174 2f7a 7374 645f 7365 656b  format/zstd_seek
+0000ae20: 6162 6c65 5f63 6f6d 7072 6573 7369 6f6e  able_compression
+0000ae30: 5f66 6f72 6d61 742e 6d64 3e60 5f20 6669  _format.md>`_ fi
+0000ae40: 6c65 2c20 6f72 2072 6561 6420 302d 7369  le, or read 0-si
+0000ae50: 7a65 2066 696c 652e 2049 7420 7072 6f76  ze file. It prov
+0000ae60: 6964 6573 2072 656c 6174 6976 656c 7920  ides relatively 
+0000ae70: 6661 7374 2073 6565 6b69 6e67 2061 6269  fast seeking abi
+0000ae80: 6c69 7479 2069 6e20 7265 6164 206d 6f64  lity in read mod
+0000ae90: 652e 0a0a 2020 2020 4e6f 7465 2074 6861  e...    Note tha
+0000aea0: 7420 6974 2064 6f65 736e 2774 2076 6572  t it doesn't ver
+0000aeb0: 6966 792f 7772 6974 6520 7468 6520 5858  ify/write the XX
+0000aec0: 4836 3420 6368 6563 6b73 756d 2066 6965  H64 checksum fie
+0000aed0: 6c64 732c 2075 7369 6e67 203a 7079 3a61  lds, using :py:a
+0000aee0: 7474 723a 607e 4350 6172 616d 6574 6572  ttr:`~CParameter
+0000aef0: 2e63 6865 636b 7375 6d46 6c61 6760 2069  .checksumFlag` i
+0000af00: 7320 6661 7374 6572 2061 6e64 206d 6f72  s faster and mor
+0000af10: 6520 666c 6578 6962 6c65 2e0a 0a20 2020  e flexible...   
+0000af20: 203a 7079 3a63 6c61 7373 3a60 5a73 7464   :py:class:`Zstd
+0000af30: 4669 6c65 6020 636c 6173 7320 6361 6e20  File` class can 
+0000af40: 616c 736f 2072 6561 6420 225a 7374 616e  also read "Zstan
+0000af50: 6461 7264 2053 6565 6b61 626c 6520 466f  dard Seekable Fo
+0000af60: 726d 6174 2220 6669 6c65 2c20 6275 7420  rmat" file, but 
+0000af70: 6e6f 2066 6173 7420 7365 656b 696e 6720  no fast seeking 
+0000af80: 6162 696c 6974 792e 0a0a 2020 2020 2e2e  ability...    ..
+0000af90: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
+0000afa0: 302e 3135 2e38 0a0a 2020 2020 2e2e 2070  0.15.8..    .. p
+0000afb0: 793a 6d65 7468 6f64 3a3a 205f 5f69 6e69  y:method:: __ini
+0000afc0: 745f 5f28 7365 6c66 2c20 6669 6c65 6e61  t__(self, filena
+0000afd0: 6d65 2c20 6d6f 6465 3d22 7222 2c20 2a2c  me, mode="r", *,
+0000afe0: 206c 6576 656c 5f6f 725f 6f70 7469 6f6e   level_or_option
+0000aff0: 3d4e 6f6e 652c 207a 7374 645f 6469 6374  =None, zstd_dict
+0000b000: 3d4e 6f6e 652c 2072 6561 645f 7369 7a65  =None, read_size
+0000b010: 3d31 3331 5f30 3735 2c20 7772 6974 655f  =131_075, write_
+0000b020: 6275 6666 6572 5f73 697a 653d 3133 315f  buffer_size=131_
+0000b030: 3539 312c 206d 6178 5f66 7261 6d65 5f63  591, max_frame_c
+0000b040: 6f6e 7465 6e74 5f73 697a 653d 3130 3234  ontent_size=1024
+0000b050: 2a31 3032 342a 3130 3234 290a 0a20 2020  *1024*1024)..   
+0000b060: 2020 2020 2053 616d 6520 6173 203a 7079       Same as :py
+0000b070: 3a6d 6574 683a 605a 7374 6446 696c 652e  :meth:`ZstdFile.
+0000b080: 5f5f 696e 6974 5f5f 602e 2045 7863 6570  __init__`. Excep
+0000b090: 7420 696e 2061 7070 656e 6420 6d6f 6465  t in append mode
+0000b0a0: 2028 612c 2061 6229 2c20 2a66 696c 656e   (a, ab), *filen
+0000b0b0: 616d 652a 2061 7267 756d 656e 7420 6361  ame* argument ca
+0000b0c0: 6e27 7420 6265 2061 2066 696c 6520 6f62  n't be a file ob
+0000b0d0: 6a65 6374 2c20 706c 6561 7365 2075 7365  ject, please use
+0000b0e0: 2066 696c 6520 7061 7468 2028 7374 722f   file path (str/
+0000b0f0: 6279 7465 732f 5061 7468 4c69 6b65 2066  bytes/PathLike f
+0000b100: 6f72 6d29 2069 6e20 7468 6973 206d 6f64  orm) in this mod
+0000b110: 652e 0a0a 2020 2020 2020 2020 2e2e 2061  e...        .. a
+0000b120: 7474 656e 7469 6f6e 3a3a 0a0a 2020 2020  ttention::..    
+0000b130: 2020 2020 2020 2020 2a6d 6178 5f66 7261          *max_fra
+0000b140: 6d65 5f63 6f6e 7465 6e74 5f73 697a 652a  me_content_size*
+0000b150: 2061 7267 756d 656e 7420 6973 2075 7365   argument is use
+0000b160: 6420 666f 7220 636f 6d70 7265 7373 696f  d for compressio
+0000b170: 6e20 6d6f 6465 7320 2877 2c20 7762 2c20  n modes (w, wb, 
+0000b180: 612c 2061 622c 2078 2c20 7862 292e 0a0a  a, ab, x, xb)...
+0000b190: 2020 2020 2020 2020 2020 2020 5768 656e              When
+0000b1a0: 2074 6865 2075 6e63 6f6d 7072 6573 7365   the uncompresse
+0000b1b0: 6420 6461 7461 2073 697a 6520 7265 6163  d data size reac
+0000b1c0: 6865 7320 2a6d 6178 5f66 7261 6d65 5f63  hes *max_frame_c
+0000b1d0: 6f6e 7465 6e74 5f73 697a 652a 2c20 6120  ontent_size*, a 
+0000b1e0: 3a72 6566 3a60 6672 616d 653c 6672 616d  :ref:`frame<fram
+0000b1f0: 655f 626c 6f63 6b3e 6020 6973 2067 656e  e_block>` is gen
+0000b200: 6572 6174 6564 2061 7574 6f6d 6174 6963  erated automatic
+0000b210: 616c 6c79 2e0a 0a20 2020 2020 2020 2020  ally...         
+0000b220: 2020 2054 6865 2064 6566 6175 6c74 2076     The default v
+0000b230: 616c 7565 2028 3120 4769 4229 2069 7320  alue (1 GiB) is 
+0000b240: 616c 6d6f 7374 2075 7365 6c65 7373 2e20  almost useless. 
+0000b250: 5573 6572 2073 686f 756c 6420 7365 7420  User should set 
+0000b260: 7468 6973 2076 616c 7565 2062 6173 6564  this value based
+0000b270: 206f 6e20 7468 6520 6461 7461 2061 6e64   on the data and
+0000b280: 2073 6565 6b69 6e67 2072 6571 7569 7265   seeking require
+0000b290: 6d65 6e74 2e0a 0a20 2020 2020 2020 2020  ment...         
+0000b2a0: 2020 2054 6f20 7265 7472 6965 7665 2061     To retrieve a
+0000b2b0: 2062 7974 652c 206e 6565 6420 746f 2064   byte, need to d
+0000b2c0: 6563 6f6d 7072 6573 7320 616c 6c20 6461  ecompress all da
+0000b2d0: 7461 2062 6566 6f72 6520 7468 6973 2062  ta before this b
+0000b2e0: 7974 6520 696e 2074 6861 7420 6672 616d  yte in that fram
+0000b2f0: 652e 2053 6f20 6966 2074 6865 2073 697a  e. So if the siz
+0000b300: 6520 6973 2073 6d61 6c6c 2c20 6974 2077  e is small, it w
+0000b310: 696c 6c20 696e 6372 6561 7365 2073 6565  ill increase see
+0000b320: 6b69 6e67 2073 7065 6564 2c20 6275 7420  king speed, but 
+0000b330: 7265 6475 6365 2063 6f6d 7072 6573 7369  reduce compressi
+0000b340: 6f6e 2072 6174 696f 2e20 4966 2074 6865  on ratio. If the
+0000b350: 2073 697a 6520 6973 206c 6172 6765 2c20   size is large, 
+0000b360: 6974 2077 696c 6c20 7265 6475 6365 2073  it will reduce s
+0000b370: 6565 6b69 6e67 2073 7065 6564 2c20 6275  eeking speed, bu
+0000b380: 7420 696e 6372 6561 7365 2063 6f6d 7072  t increase compr
+0000b390: 6573 7369 6f6e 2072 6174 696f 2e0a 0a20  ession ratio... 
+0000b3a0: 2020 2020 2020 2020 2020 2041 766f 6964             Avoid
+0000b3b0: 2072 6561 6c6c 7920 7469 6e79 2066 7261   really tiny fra
+0000b3c0: 6d65 2073 697a 6573 2028 3c31 204b 6942  me sizes (<1 KiB
+0000b3d0: 292c 2074 6861 7420 776f 756c 6420 6875  ), that would hu
+0000b3e0: 7274 2063 6f6d 7072 6573 7369 6f6e 2072  rt compression r
+0000b3f0: 6174 696f 2063 6f6e 7369 6465 7261 626c  atio considerabl
+0000b400: 792e 0a0a 2020 2020 2020 2020 2020 2020  y...            
+0000b410: 596f 7520 6361 6e20 616c 736f 206d 616e  You can also man
+0000b420: 7561 6c6c 7920 6765 6e65 7261 7465 2061  ually generate a
+0000b430: 2066 7261 6d65 2075 7369 6e67 2060 6066   frame using ``f
+0000b440: 2e66 6c75 7368 286d 6f64 653d 662e 464c  .flush(mode=f.FL
+0000b450: 5553 485f 4652 414d 4529 6060 2e0a 0a20  USH_FRAME)``... 
+0000b460: 2020 202e 2e20 7079 3a73 7461 7469 636d     .. py:staticm
+0000b470: 6574 686f 643a 3a20 6973 5f73 6565 6b61  ethod:: is_seeka
+0000b480: 626c 655f 666f 726d 6174 5f66 696c 6528  ble_format_file(
+0000b490: 6669 6c65 6e61 6d65 290a 0a20 2020 2020  filename)..     
+0000b4a0: 2020 2054 6869 7320 7374 6174 6963 206d     This static m
+0000b4b0: 6574 686f 6420 6368 6563 6b73 2069 6620  ethod checks if 
+0000b4c0: 6120 6669 6c65 2069 7320 225a 7374 616e  a file is "Zstan
+0000b4d0: 6461 7264 2053 6565 6b61 626c 6520 466f  dard Seekable Fo
+0000b4e0: 726d 6174 2220 6669 6c65 206f 7220 302d  rmat" file or 0-
+0000b4f0: 7369 7a65 2066 696c 652e 0a0a 2020 2020  size file...    
+0000b500: 2020 2020 4974 2070 6172 7365 7320 7468      It parses th
+0000b510: 6520 7365 656b 2074 6162 6c65 2061 7420  e seek table at 
+0000b520: 7468 6520 656e 6420 6f66 2074 6865 2066  the end of the f
+0000b530: 696c 652c 2072 6574 7572 6e73 2060 6054  ile, returns ``T
+0000b540: 7275 6560 6020 6966 206e 6f20 666f 726d  rue`` if no form
+0000b550: 6174 2065 7272 6f72 2e0a 0a20 2020 2020  at error...     
+0000b560: 2020 203a 7061 7261 6d20 6669 6c65 6e61     :param filena
+0000b570: 6d65 3a20 4120 6669 6c65 2074 6f20 6265  me: A file to be
+0000b580: 2063 6865 636b 6564 0a20 2020 2020 2020   checked.       
+0000b590: 203a 7479 7065 2066 696c 656e 616d 653a   :type filename:
+0000b5a0: 2046 696c 6520 7061 7468 2028 7374 722f   File path (str/
+0000b5b0: 6279 7465 732f 5061 7468 4c69 6b65 292c  bytes/PathLike),
+0000b5c0: 206f 7220 6669 6c65 206f 626a 6563 7420   or file object 
+0000b5d0: 696e 2072 6561 6469 6e67 206d 6f64 652e  in reading mode.
+0000b5e0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000b5f0: 3a20 5265 7375 6c74 0a20 2020 2020 2020  : Result.       
+0000b600: 203a 7274 7970 653a 2062 6f6f 6c0a 0a20   :rtype: bool.. 
+0000b610: 2020 202e 2e20 736f 7572 6365 636f 6465     .. sourcecode
+0000b620: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+0000b630: 2020 2023 2043 6f6e 7665 7274 2061 6e20     # Convert an 
+0000b640: 6578 6973 7469 6e67 207a 7374 6420 6669  existing zstd fi
+0000b650: 6c65 2074 6f20 5a73 7461 6e64 6172 6420  le to Zstandard 
+0000b660: 5365 656b 6162 6c65 2046 6f72 6d61 7420  Seekable Format 
+0000b670: 6669 6c65 2e0a 2020 2020 2020 2020 2320  file..        # 
+0000b680: 3130 204d 6942 2070 6572 2066 7261 6d65  10 MiB per frame
+0000b690: 2e0a 2020 2020 2020 2020 7769 7468 205a  ..        with Z
+0000b6a0: 7374 6446 696c 6528 494e 5f46 494c 452c  stdFile(IN_FILE,
+0000b6b0: 2027 7227 2920 6173 2069 6668 3a0a 2020   'r') as ifh:.  
+0000b6c0: 2020 2020 2020 2020 2020 7769 7468 2053            with S
+0000b6d0: 6565 6b61 626c 655a 7374 6446 696c 6528  eekableZstdFile(
+0000b6e0: 4f55 545f 4649 4c45 2c20 2777 272c 0a20  OUT_FILE, 'w',. 
+0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b710: 206d 6178 5f66 7261 6d65 5f63 6f6e 7465   max_frame_conte
+0000b720: 6e74 5f73 697a 653d 3130 2a31 3032 342a  nt_size=10*1024*
+0000b730: 3130 3234 2920 6173 206f 6668 3a0a 2020  1024) as ofh:.  
+0000b740: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+0000b750: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
+0000b760: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000b770: 7420 3d20 6966 682e 7265 6164 2833 302a  t = ifh.read(30*
+0000b780: 3130 3234 2a31 3032 3429 0a20 2020 2020  1024*1024).     
+0000b790: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000b7a0: 6620 6e6f 7420 6461 743a 0a20 2020 2020  f not dat:.     
+0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7c0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+0000b7d0: 2020 2020 2020 2020 2020 2020 206f 6668               ofh
+0000b7e0: 2e77 7269 7465 2864 6174 290a 0a20 2020  .write(dat)..   
+0000b7f0: 2020 2020 2023 2072 6574 7572 6e20 5472       # return Tr
+0000b800: 7565 0a20 2020 2020 2020 2053 6565 6b61  ue.        Seeka
+0000b810: 626c 655a 7374 6446 696c 652e 6973 5f73  bleZstdFile.is_s
+0000b820: 6565 6b61 626c 655f 666f 726d 6174 5f66  eekable_format_f
+0000b830: 696c 6528 4f55 545f 4649 4c45 290a 0a41  ile(OUT_FILE)..A
+0000b840: 6476 616e 6365 6420 7061 7261 6d65 7465  dvanced paramete
+0000b850: 7273 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  rs.-------------
+0000b860: 2d2d 2d2d 2d2d 0a0a 2020 2020 5468 6973  ------..    This
+0000b870: 2073 6563 7469 6f6e 2063 6f6e 7461 696e   section contain
+0000b880: 7320 636c 6173 7320 3a70 793a 636c 6173  s class :py:clas
+0000b890: 733a 6043 5061 7261 6d65 7465 7260 2c20  s:`CParameter`, 
+0000b8a0: 3a70 793a 636c 6173 733a 6044 5061 7261  :py:class:`DPara
+0000b8b0: 6d65 7465 7260 2c20 3a70 793a 636c 6173  meter`, :py:clas
+0000b8c0: 733a 6053 7472 6174 6567 7960 2c20 7468  s:`Strategy`, th
+0000b8d0: 6579 2061 7265 2073 7562 636c 6173 7365  ey are subclasse
+0000b8e0: 7320 6f66 2060 6049 6e74 456e 756d 6060  s of ``IntEnum``
+0000b8f0: 2c20 7573 6564 2066 6f72 2073 6574 7469  , used for setti
+0000b900: 6e67 2061 6476 616e 6365 6420 7061 7261  ng advanced para
+0000b910: 6d65 7465 7273 2e0a 0a20 2020 2041 7474  meters...    Att
+0000b920: 7269 6275 7465 7320 6f66 203a 7079 3a63  ributes of :py:c
+0000b930: 6c61 7373 3a60 4350 6172 616d 6574 6572  lass:`CParameter
+0000b940: 6020 636c 6173 733a 0a0a 2020 2020 2020  ` class:..      
+0000b950: 2020 2d20 436f 6d70 7265 7373 696f 6e20    - Compression 
+0000b960: 6c65 7665 6c20 283a 7079 3a61 7474 723a  level (:py:attr:
+0000b970: 607e 4350 6172 616d 6574 6572 2e63 6f6d  `~CParameter.com
+0000b980: 7072 6573 7369 6f6e 4c65 7665 6c60 290a  pressionLevel`).
+0000b990: 2020 2020 2020 2020 2d20 436f 6d70 7265          - Compre
+0000b9a0: 7373 2061 6c67 6f72 6974 686d 2070 6172  ss algorithm par
+0000b9b0: 616d 6574 6572 7320 283a 7079 3a61 7474  ameters (:py:att
+0000b9c0: 723a 607e 4350 6172 616d 6574 6572 2e77  r:`~CParameter.w
+0000b9d0: 696e 646f 774c 6f67 602c 203a 7079 3a61  indowLog`, :py:a
+0000b9e0: 7474 723a 607e 4350 6172 616d 6574 6572  ttr:`~CParameter
+0000b9f0: 2e68 6173 684c 6f67 602c 203a 7079 3a61  .hashLog`, :py:a
+0000ba00: 7474 723a 607e 4350 6172 616d 6574 6572  ttr:`~CParameter
+0000ba10: 2e63 6861 696e 4c6f 6760 2c20 3a70 793a  .chainLog`, :py:
+0000ba20: 6174 7472 3a60 7e43 5061 7261 6d65 7465  attr:`~CParamete
+0000ba30: 722e 7365 6172 6368 4c6f 6760 2c20 3a70  r.searchLog`, :p
+0000ba40: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
+0000ba50: 7465 722e 6d69 6e4d 6174 6368 602c 203a  ter.minMatch`, :
+0000ba60: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
+0000ba70: 6574 6572 2e74 6172 6765 744c 656e 6774  eter.targetLengt
+0000ba80: 6860 2c20 3a70 793a 6174 7472 3a60 7e43  h`, :py:attr:`~C
+0000ba90: 5061 7261 6d65 7465 722e 7374 7261 7465  Parameter.strate
+0000baa0: 6779 6029 0a20 2020 2020 2020 202d 204c  gy`).        - L
+0000bab0: 6f6e 6720 6469 7374 616e 6365 206d 6174  ong distance mat
+0000bac0: 6368 696e 6720 283a 7079 3a61 7474 723a  ching (:py:attr:
+0000bad0: 607e 4350 6172 616d 6574 6572 2e65 6e61  `~CParameter.ena
+0000bae0: 626c 654c 6f6e 6744 6973 7461 6e63 654d  bleLongDistanceM
+0000baf0: 6174 6368 696e 6760 2c20 3a70 793a 6174  atching`, :py:at
+0000bb00: 7472 3a60 7e43 5061 7261 6d65 7465 722e  tr:`~CParameter.
+0000bb10: 6c64 6d48 6173 684c 6f67 602c 203a 7079  ldmHashLog`, :py
+0000bb20: 3a61 7474 723a 607e 4350 6172 616d 6574  :attr:`~CParamet
+0000bb30: 6572 2e6c 646d 4d69 6e4d 6174 6368 602c  er.ldmMinMatch`,
+0000bb40: 203a 7079 3a61 7474 723a 607e 4350 6172   :py:attr:`~CPar
+0000bb50: 616d 6574 6572 2e6c 646d 4275 636b 6574  ameter.ldmBucket
+0000bb60: 5369 7a65 4c6f 6760 2c20 3a70 793a 6174  SizeLog`, :py:at
+0000bb70: 7472 3a60 7e43 5061 7261 6d65 7465 722e  tr:`~CParameter.
+0000bb80: 6c64 6d48 6173 6852 6174 654c 6f67 6029  ldmHashRateLog`)
+0000bb90: 0a20 2020 2020 2020 202d 204d 6973 6320  .        - Misc 
+0000bba0: 283a 7079 3a61 7474 723a 607e 4350 6172  (:py:attr:`~CPar
+0000bbb0: 616d 6574 6572 2e63 6f6e 7465 6e74 5369  ameter.contentSi
+0000bbc0: 7a65 466c 6167 602c 203a 7079 3a61 7474  zeFlag`, :py:att
+0000bbd0: 723a 607e 4350 6172 616d 6574 6572 2e63  r:`~CParameter.c
+0000bbe0: 6865 636b 7375 6d46 6c61 6760 2c20 3a70  hecksumFlag`, :p
+0000bbf0: 793a 6174 7472 3a60 7e43 5061 7261 6d65  y:attr:`~CParame
+0000bc00: 7465 722e 6469 6374 4944 466c 6167 6029  ter.dictIDFlag`)
+0000bc10: 0a20 2020 2020 2020 202d 204d 756c 7469  .        - Multi
+0000bc20: 2d74 6872 6561 6465 6420 636f 6d70 7265  -threaded compre
+0000bc30: 7373 696f 6e20 283a 7079 3a61 7474 723a  ssion (:py:attr:
+0000bc40: 607e 4350 6172 616d 6574 6572 2e6e 6257  `~CParameter.nbW
+0000bc50: 6f72 6b65 7273 602c 203a 7079 3a61 7474  orkers`, :py:att
+0000bc60: 723a 607e 4350 6172 616d 6574 6572 2e6a  r:`~CParameter.j
+0000bc70: 6f62 5369 7a65 602c 203a 7079 3a61 7474  obSize`, :py:att
+0000bc80: 723a 607e 4350 6172 616d 6574 6572 2e6f  r:`~CParameter.o
+0000bc90: 7665 726c 6170 4c6f 6760 290a 0a20 2020  verlapLog`)..   
+0000bca0: 2041 7474 7269 6275 7465 206f 6620 3a70   Attribute of :p
+0000bcb0: 793a 636c 6173 733a 6044 5061 7261 6d65  y:class:`DParame
+0000bcc0: 7465 7260 2063 6c61 7373 3a0a 0a20 2020  ter` class:..   
+0000bcd0: 2020 2020 202d 2044 6563 6f6d 7072 6573       - Decompres
+0000bce0: 7369 6f6e 2070 6172 616d 6574 6572 2028  sion parameter (
+0000bcf0: 3a70 793a 6174 7472 3a60 7e44 5061 7261  :py:attr:`~DPara
+0000bd00: 6d65 7465 722e 7769 6e64 6f77 4c6f 674d  meter.windowLogM
+0000bd10: 6178 6029 0a0a 2020 2020 4174 7472 6962  ax`)..    Attrib
+0000bd20: 7574 6573 206f 6620 3a70 793a 636c 6173  utes of :py:clas
+0000bd30: 733a 6053 7472 6174 6567 7960 2063 6c61  s:`Strategy` cla
+0000bd40: 7373 3a0a 0a20 2020 2020 2020 203a 7079  ss:..        :py
+0000bd50: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
+0000bd60: 2e66 6173 7460 2c20 3a70 793a 6174 7472  .fast`, :py:attr
+0000bd70: 3a60 7e53 7472 6174 6567 792e 6466 6173  :`~Strategy.dfas
+0000bd80: 7460 2c20 3a70 793a 6174 7472 3a60 7e53  t`, :py:attr:`~S
+0000bd90: 7472 6174 6567 792e 6772 6565 6479 602c  trategy.greedy`,
+0000bda0: 203a 7079 3a61 7474 723a 607e 5374 7261   :py:attr:`~Stra
+0000bdb0: 7465 6779 2e6c 617a 7960 2c20 3a70 793a  tegy.lazy`, :py:
+0000bdc0: 6174 7472 3a60 7e53 7472 6174 6567 792e  attr:`~Strategy.
+0000bdd0: 6c61 7a79 3260 2c20 3a70 793a 6174 7472  lazy2`, :py:attr
+0000bde0: 3a60 7e53 7472 6174 6567 792e 6274 6c61  :`~Strategy.btla
+0000bdf0: 7a79 3260 2c20 3a70 793a 6174 7472 3a60  zy2`, :py:attr:`
+0000be00: 7e53 7472 6174 6567 792e 6274 6f70 7460  ~Strategy.btopt`
+0000be10: 2c20 3a70 793a 6174 7472 3a60 7e53 7472  , :py:attr:`~Str
+0000be20: 6174 6567 792e 6274 756c 7472 6160 2c20  ategy.btultra`, 
+0000be30: 3a70 793a 6174 7472 3a60 7e53 7472 6174  :py:attr:`~Strat
+0000be40: 6567 792e 6274 756c 7472 6132 602e 0a0a  egy.btultra2`...
+0000be50: 2e2e 205f 4350 6172 616d 6574 6572 3a0a  .. _CParameter:.
+0000be60: 0a2e 2e20 7079 3a63 6c61 7373 3a3a 2043  ... py:class:: C
+0000be70: 5061 7261 6d65 7465 7228 496e 7445 6e75  Parameter(IntEnu
+0000be80: 6d29 0a0a 2020 2020 4164 7661 6e63 6564  m)..    Advanced
+0000be90: 2063 6f6d 7072 6573 7369 6f6e 2070 6172   compression par
+0000bea0: 616d 6574 6572 732e 0a0a 2020 2020 5768  ameters...    Wh
+0000beb0: 656e 2075 7369 6e67 2c20 7075 7420 7468  en using, put th
+0000bec0: 6520 7061 7261 6d65 7465 7273 2069 6e20  e parameters in 
+0000bed0: 6120 6060 6469 6374 6060 206f 626a 6563  a ``dict`` objec
+0000bee0: 742c 2074 6865 206b 6579 2069 7320 6120  t, the key is a 
+0000bef0: 3a70 793a 636c 6173 733a 6043 5061 7261  :py:class:`CPara
+0000bf00: 6d65 7465 7260 206e 616d 652c 2074 6865  meter` name, the
+0000bf10: 2076 616c 7565 2069 7320 6120 3332 2d62   value is a 32-b
+0000bf20: 6974 2073 6967 6e65 6420 696e 7465 6765  it signed intege
+0000bf30: 7220 7661 6c75 652e 0a0a 2020 2020 2e2e  r value...    ..
+0000bf40: 2073 6f75 7263 6563 6f64 653a 3a20 7079   sourcecode:: py
+0000bf50: 7468 6f6e 0a0a 2020 2020 2020 2020 6f70  thon..        op
+0000bf60: 7469 6f6e 203d 207b 4350 6172 616d 6574  tion = {CParamet
+0000bf70: 6572 2e63 6f6d 7072 6573 7369 6f6e 4c65  er.compressionLe
+0000bf80: 7665 6c20 3a20 3130 2c0a 2020 2020 2020  vel : 10,.      
+0000bf90: 2020 2020 2020 2020 2020 2020 4350 6172              CPar
+0000bfa0: 616d 6574 6572 2e63 6865 636b 7375 6d46  ameter.checksumF
+0000bfb0: 6c61 6720 3a20 317d 0a0a 2020 2020 2020  lag : 1}..      
+0000bfc0: 2020 2320 7573 6564 2077 6974 6820 636f    # used with co
+0000bfd0: 6d70 7265 7373 2829 2066 756e 6374 696f  mpress() functio
+0000bfe0: 6e0a 2020 2020 2020 2020 636f 6d70 7265  n.        compre
+0000bff0: 7373 6564 5f64 6174 203d 2063 6f6d 7072  ssed_dat = compr
+0000c000: 6573 7328 7261 775f 6461 742c 206f 7074  ess(raw_dat, opt
+0000c010: 696f 6e29 0a0a 2020 2020 2020 2020 2320  ion)..        # 
+0000c020: 7573 6564 2077 6974 6820 5a73 7464 436f  used with ZstdCo
+0000c030: 6d70 7265 7373 6f72 206f 626a 6563 740a  mpressor object.
+0000c040: 2020 2020 2020 2020 6320 3d20 5a73 7464          c = Zstd
+0000c050: 436f 6d70 7265 7373 6f72 286c 6576 656c  Compressor(level
+0000c060: 5f6f 725f 6f70 7469 6f6e 3d6f 7074 696f  _or_option=optio
+0000c070: 6e29 0a20 2020 2020 2020 2063 6f6d 7072  n).        compr
+0000c080: 6573 7365 645f 6461 7431 203d 2063 2e63  essed_dat1 = c.c
+0000c090: 6f6d 7072 6573 7328 7261 775f 6461 7429  ompress(raw_dat)
+0000c0a0: 0a20 2020 2020 2020 2063 6f6d 7072 6573  .        compres
+0000c0b0: 7365 645f 6461 7432 203d 2063 2e66 6c75  sed_dat2 = c.flu
+0000c0c0: 7368 2829 0a0a 2020 2020 5061 7261 6d65  sh()..    Parame
+0000c0d0: 7465 7220 7661 6c75 6520 7368 6f75 6c64  ter value should
+0000c0e0: 2062 656c 6f6e 6720 746f 2061 6e20 696e   belong to an in
+0000c0f0: 7465 7276 616c 2077 6974 6820 6c6f 7765  terval with lowe
+0000c100: 7220 616e 6420 7570 7065 7220 626f 756e  r and upper boun
+0000c110: 6473 2c20 6f74 6865 7277 6973 6520 7468  ds, otherwise th
+0000c120: 6579 2077 696c 6c20 6569 7468 6572 2074  ey will either t
+0000c130: 7269 6767 6572 2061 6e20 6572 726f 7220  rigger an error 
+0000c140: 6f72 2062 6520 636c 616d 7065 6420 7369  or be clamped si
+0000c150: 6c65 6e74 6c79 2e0a 0a20 2020 2054 6865  lently...    The
+0000c160: 2063 6f6e 7374 616e 7420 7661 6c75 6573   constant values
+0000c170: 206d 656e 7469 6f6e 6564 2062 656c 6f77   mentioned below
+0000c180: 2061 7265 2064 6566 696e 6564 2069 6e20   are defined in 
+0000c190: 607a 7374 642e 6820 3c68 7474 7073 3a2f  `zstd.h <https:/
+0000c1a0: 2f67 6974 6875 622e 636f 6d2f 6661 6365  /github.com/face
+0000c1b0: 626f 6f6b 2f7a 7374 642f 626c 6f62 2f72  book/zstd/blob/r
+0000c1c0: 656c 6561 7365 2f6c 6962 2f7a 7374 642e  elease/lib/zstd.
+0000c1d0: 683e 605f 2c20 6e6f 7465 2074 6861 7420  h>`_, note that 
+0000c1e0: 7468 6573 6520 7661 6c75 6573 206d 6179  these values may
+0000c1f0: 2062 6520 6469 6666 6572 656e 7420 696e   be different in
+0000c200: 2064 6966 6665 7265 6e74 207a 7374 6420   different zstd 
+0000c210: 7665 7273 696f 6e73 2e0a 0a20 2020 202e  versions...    .
+0000c220: 2e20 7079 3a6d 6574 686f 643a 3a20 626f  . py:method:: bo
+0000c230: 756e 6473 2873 656c 6629 0a0a 2020 2020  unds(self)..    
+0000c240: 2020 2020 5265 7475 726e 206c 6f77 6572      Return lower
+0000c250: 2061 6e64 2075 7070 6572 2062 6f75 6e64   and upper bound
+0000c260: 7320 6f66 2061 2070 6172 616d 6574 6572  s of a parameter
+0000c270: 2c20 626f 7468 2069 6e63 6c75 7369 7665  , both inclusive
+0000c280: 2e0a 0a20 2020 2020 2020 202e 2e20 736f  ...        .. so
+0000c290: 7572 6365 636f 6465 3a3a 2070 7974 686f  urcecode:: pytho
+0000c2a0: 6e0a 0a20 2020 2020 2020 2020 2020 203e  n..            >
+0000c2b0: 3e3e 2043 5061 7261 6d65 7465 722e 636f  >> CParameter.co
+0000c2c0: 6d70 7265 7373 696f 6e4c 6576 656c 2e62  mpressionLevel.b
+0000c2d0: 6f75 6e64 7328 290a 2020 2020 2020 2020  ounds().        
+0000c2e0: 2020 2020 282d 3133 3130 3732 2c20 3232      (-131072, 22
+0000c2f0: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+0000c300: 3e20 4350 6172 616d 6574 6572 2e77 696e  > CParameter.win
+0000c310: 646f 774c 6f67 2e62 6f75 6e64 7328 290a  dowLog.bounds().
+0000c320: 2020 2020 2020 2020 2020 2020 2831 302c              (10,
+0000c330: 2033 3129 0a20 2020 2020 2020 2020 2020   31).           
+0000c340: 203e 3e3e 2043 5061 7261 6d65 7465 722e   >>> CParameter.
+0000c350: 656e 6162 6c65 4c6f 6e67 4469 7374 616e  enableLongDistan
+0000c360: 6365 4d61 7463 6869 6e67 2e62 6f75 6e64  ceMatching.bound
+0000c370: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+0000c380: 2830 2c20 3129 0a0a 2020 2020 2e2e 2070  (0, 1)..    .. p
+0000c390: 793a 6174 7472 6962 7574 653a 3a20 636f  y:attribute:: co
+0000c3a0: 6d70 7265 7373 696f 6e4c 6576 656c 0a0a  mpressionLevel..
+0000c3b0: 2020 2020 2020 2020 5365 7420 636f 6d70          Set comp
+0000c3c0: 7265 7373 696f 6e20 7061 7261 6d65 7465  ression paramete
+0000c3d0: 7273 2061 6363 6f72 6469 6e67 2074 6f20  rs according to 
+0000c3e0: 7072 652d 6465 6669 6e65 6420 636f 6d70  pre-defined comp
+0000c3f0: 7265 7373 696f 6e4c 6576 656c 2074 6162  ressionLevel tab
+0000c400: 6c65 2c20 7365 6520 3a72 6566 3a60 636f  le, see :ref:`co
+0000c410: 6d70 7265 7373 696f 6e20 6c65 7665 6c3c  mpression level<
+0000c420: 636f 6d70 7265 7373 696f 6e5f 6c65 7665  compression_leve
+0000c430: 6c3e 6020 666f 7220 6465 7461 696c 732e  l>` for details.
+0000c440: 0a0a 2020 2020 2020 2020 5365 7474 696e  ..        Settin
+0000c450: 6720 6120 636f 6d70 7265 7373 696f 6e20  g a compression 
+0000c460: 6c65 7665 6c20 646f 6573 206e 6f74 2073  level does not s
+0000c470: 6574 2061 6c6c 206f 7468 6572 2063 6f6d  et all other com
+0000c480: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
+0000c490: 6572 7320 746f 2064 6566 6175 6c74 2e20  ers to default. 
+0000c4a0: 5365 7474 696e 6720 7468 6973 2077 696c  Setting this wil
+0000c4b0: 6c20 6479 6e61 6d69 6361 6c6c 7920 696d  l dynamically im
+0000c4c0: 7061 6374 2074 6865 2063 6f6d 7072 6573  pact the compres
+0000c4d0: 7369 6f6e 2070 6172 616d 6574 6572 7320  sion parameters 
+0000c4e0: 7768 6963 6820 6861 7665 206e 6f74 2062  which have not b
+0000c4f0: 6565 6e20 6d61 6e75 616c 6c79 2073 6574  een manually set
+0000c500: 2c20 7468 6520 6d61 6e75 616c 6c79 2073  , the manually s
+0000c510: 6574 206f 6e65 7320 7769 6c6c 2022 7374  et ones will "st
+0000c520: 6963 6b22 2e0a 0a20 2020 202e 2e20 7079  ick"...    .. py
+0000c530: 3a61 7474 7269 6275 7465 3a3a 2077 696e  :attribute:: win
+0000c540: 646f 774c 6f67 0a0a 2020 2020 2020 2020  dowLog..        
+0000c550: 4d61 7869 6d75 6d20 616c 6c6f 7765 6420  Maximum allowed 
+0000c560: 6261 636b 2d72 6566 6572 656e 6365 2064  back-reference d
+0000c570: 6973 7461 6e63 652c 2065 7870 7265 7373  istance, express
+0000c580: 6564 2061 7320 706f 7765 7220 6f66 2032  ed as power of 2
+0000c590: 2c20 6060 3120 3c3c 2077 696e 646f 774c  , ``1 << windowL
+0000c5a0: 6f67 6060 2062 7974 6573 2e0a 0a20 2020  og`` bytes...   
+0000c5b0: 2020 2020 204c 6172 6765 7220 7661 6c75       Larger valu
+0000c5c0: 6573 2072 6571 7569 7269 6e67 206d 6f72  es requiring mor
+0000c5d0: 6520 6d65 6d6f 7279 2061 6e64 2074 7970  e memory and typ
+0000c5e0: 6963 616c 6c79 2063 6f6d 7072 6573 7369  ically compressi
+0000c5f0: 6e67 206d 6f72 652e 0a0a 2020 2020 2020  ng more...      
+0000c600: 2020 5468 6973 2077 696c 6c20 7365 7420    This will set 
+0000c610: 6120 6d65 6d6f 7279 2062 7564 6765 7420  a memory budget 
+0000c620: 666f 7220 7374 7265 616d 696e 6720 6465  for streaming de
+0000c630: 636f 6d70 7265 7373 696f 6e2e 2055 7369  compression. Usi
+0000c640: 6e67 2061 2076 616c 7565 2067 7265 6174  ng a value great
+0000c650: 6572 2074 6861 6e20 6060 5a53 5444 5f57  er than ``ZSTD_W
+0000c660: 494e 444f 574c 4f47 5f4c 494d 4954 5f44  INDOWLOG_LIMIT_D
+0000c670: 4546 4155 4c54 6060 2072 6571 7569 7265  EFAULT`` require
+0000c680: 7320 6578 706c 6963 6974 6c79 2061 6c6c  s explicitly all
+0000c690: 6f77 696e 6720 7375 6368 2073 697a 6520  owing such size 
+0000c6a0: 6174 2073 7472 6561 6d69 6e67 2064 6563  at streaming dec
+0000c6b0: 6f6d 7072 6573 7369 6f6e 2073 7461 6765  ompression stage
+0000c6c0: 2c20 7365 6520 3a70 793a 6174 7472 3a60  , see :py:attr:`
+0000c6d0: 4450 6172 616d 6574 6572 2e77 696e 646f  DParameter.windo
+0000c6e0: 774c 6f67 4d61 7860 2e20 6060 5a53 5444  wLogMax`. ``ZSTD
+0000c6f0: 5f57 494e 444f 574c 4f47 5f4c 494d 4954  _WINDOWLOG_LIMIT
+0000c700: 5f44 4546 4155 4c54 6060 2069 7320 3237  _DEFAULT`` is 27
+0000c710: 2069 6e20 7a73 7464 2076 312e 322b 2c20   in zstd v1.2+, 
+0000c720: 6d65 616e 7320 3132 3820 4d69 4220 2831  means 128 MiB (1
+0000c730: 203c 3c20 3237 292e 0a0a 2020 2020 2020   << 27)...      
+0000c740: 2020 4d75 7374 2062 6520 636c 616d 7065    Must be clampe
+0000c750: 6420 6265 7477 6565 6e20 6060 5a53 5444  d between ``ZSTD
+0000c760: 5f57 494e 444f 574c 4f47 5f4d 494e 6060  _WINDOWLOG_MIN``
+0000c770: 2061 6e64 2060 605a 5354 445f 5749 4e44   and ``ZSTD_WIND
+0000c780: 4f57 4c4f 475f 4d41 5860 602e 0a0a 2020  OWLOG_MAX``...  
+0000c790: 2020 2020 2020 5370 6563 6961 6c3a 2076        Special: v
+0000c7a0: 616c 7565 2060 6030 6060 206d 6561 6e73  alue ``0`` means
+0000c7b0: 2022 7573 6520 6465 6661 756c 7420 7769   "use default wi
+0000c7c0: 6e64 6f77 4c6f 6722 2c20 7468 656e 2074  ndowLog", then t
+0000c7d0: 6865 2076 616c 7565 2069 7320 6479 6e61  he value is dyna
+0000c7e0: 6d69 6361 6c6c 7920 7365 742c 2073 6565  mically set, see
+0000c7f0: 2022 5722 2063 6f6c 756d 6e20 696e 2060   "W" column in `
+0000c800: 7468 6973 2074 6162 6c65 203c 6874 7470  this table <http
+0000c810: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
+0000c820: 6163 6562 6f6f 6b2f 7a73 7464 2f62 6c6f  acebook/zstd/blo
+0000c830: 622f 7265 6c65 6173 652f 6c69 622f 636f  b/release/lib/co
+0000c840: 6d70 7265 7373 2f63 6c65 7665 6c73 2e68  mpress/clevels.h
+0000c850: 3e60 5f2e 0a0a 2020 2020 2e2e 2070 793a  >`_...    .. py:
+0000c860: 6174 7472 6962 7574 653a 3a20 6861 7368  attribute:: hash
+0000c870: 4c6f 670a 0a20 2020 2020 2020 2053 697a  Log..        Siz
+0000c880: 6520 6f66 2074 6865 2069 6e69 7469 616c  e of the initial
+0000c890: 2070 726f 6265 2074 6162 6c65 2c20 6173   probe table, as
+0000c8a0: 2061 2070 6f77 6572 206f 6620 322c 2072   a power of 2, r
+0000c8b0: 6573 756c 7469 6e67 206d 656d 6f72 7920  esulting memory 
+0000c8c0: 7573 6167 6520 6973 2060 6031 203c 3c20  usage is ``1 << 
+0000c8d0: 2868 6173 684c 6f67 2b32 2960 6020 6279  (hashLog+2)`` by
+0000c8e0: 7465 732e 0a0a 2020 2020 2020 2020 4d75  tes...        Mu
+0000c8f0: 7374 2062 6520 636c 616d 7065 6420 6265  st be clamped be
+0000c900: 7477 6565 6e20 6060 5a53 5444 5f48 4153  tween ``ZSTD_HAS
+0000c910: 484c 4f47 5f4d 494e 6060 2061 6e64 2060  HLOG_MIN`` and `
+0000c920: 605a 5354 445f 4841 5348 4c4f 475f 4d41  `ZSTD_HASHLOG_MA
+0000c930: 5860 602e 0a0a 2020 2020 2020 2020 4c61  X``...        La
+0000c940: 7267 6572 2074 6162 6c65 7320 696d 7072  rger tables impr
+0000c950: 6f76 6520 636f 6d70 7265 7373 696f 6e20  ove compression 
+0000c960: 7261 7469 6f20 6f66 2073 7472 6174 6567  ratio of strateg
+0000c970: 6965 7320 3c3d 203a 7079 3a61 7474 723a  ies <= :py:attr:
+0000c980: 607e 5374 7261 7465 6779 2e64 6661 7374  `~Strategy.dfast
+0000c990: 602c 2061 6e64 2069 6d70 726f 7665 2073  `, and improve s
+0000c9a0: 7065 6564 206f 6620 7374 7261 7465 6769  peed of strategi
+0000c9b0: 6573 203e 203a 7079 3a61 7474 723a 607e  es > :py:attr:`~
+0000c9c0: 5374 7261 7465 6779 2e64 6661 7374 602e  Strategy.dfast`.
+0000c9d0: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
+0000c9e0: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
+0000c9f0: 6561 6e73 2022 7573 6520 6465 6661 756c  eans "use defaul
+0000ca00: 7420 6861 7368 4c6f 6722 2c20 7468 656e  t hashLog", then
+0000ca10: 2074 6865 2076 616c 7565 2069 7320 6479   the value is dy
+0000ca20: 6e61 6d69 6361 6c6c 7920 7365 742c 2073  namically set, s
+0000ca30: 6565 2022 4822 2063 6f6c 756d 6e20 696e  ee "H" column in
+0000ca40: 2060 7468 6973 2074 6162 6c65 203c 6874   `this table <ht
+0000ca50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000ca60: 2f66 6163 6562 6f6f 6b2f 7a73 7464 2f62  /facebook/zstd/b
+0000ca70: 6c6f 622f 7265 6c65 6173 652f 6c69 622f  lob/release/lib/
+0000ca80: 636f 6d70 7265 7373 2f63 6c65 7665 6c73  compress/clevels
+0000ca90: 2e68 3e60 5f2e 0a0a 2020 2020 2e2e 2070  .h>`_...    .. p
+0000caa0: 793a 6174 7472 6962 7574 653a 3a20 6368  y:attribute:: ch
+0000cab0: 6169 6e4c 6f67 0a0a 2020 2020 2020 2020  ainLog..        
+0000cac0: 5369 7a65 206f 6620 7468 6520 6d75 6c74  Size of the mult
+0000cad0: 692d 7072 6f62 6520 7365 6172 6368 2074  i-probe search t
+0000cae0: 6162 6c65 2c20 6173 2061 2070 6f77 6572  able, as a power
+0000caf0: 206f 6620 322c 2072 6573 756c 7469 6e67   of 2, resulting
+0000cb00: 206d 656d 6f72 7920 7573 6167 6520 6973   memory usage is
+0000cb10: 2060 6031 203c 3c20 2863 6861 696e 4c6f   ``1 << (chainLo
+0000cb20: 672b 3229 6060 2062 7974 6573 2e0a 0a20  g+2)`` bytes... 
+0000cb30: 2020 2020 2020 204d 7573 7420 6265 2063         Must be c
+0000cb40: 6c61 6d70 6564 2062 6574 7765 656e 2060  lamped between `
+0000cb50: 605a 5354 445f 4348 4149 4e4c 4f47 5f4d  `ZSTD_CHAINLOG_M
+0000cb60: 494e 6060 2061 6e64 2060 605a 5354 445f  IN`` and ``ZSTD_
+0000cb70: 4348 4149 4e4c 4f47 5f4d 4158 6060 2e0a  CHAINLOG_MAX``..
+0000cb80: 0a20 2020 2020 2020 204c 6172 6765 7220  .        Larger 
+0000cb90: 7461 626c 6573 2072 6573 756c 7420 696e  tables result in
+0000cba0: 2062 6574 7465 7220 616e 6420 736c 6f77   better and slow
+0000cbb0: 6572 2063 6f6d 7072 6573 7369 6f6e 2e0a  er compression..
+0000cbc0: 0a20 2020 2020 2020 2054 6869 7320 7061  .        This pa
+0000cbd0: 7261 6d65 7465 7220 6973 2075 7365 6c65  rameter is usele
+0000cbe0: 7373 2066 6f72 203a 7079 3a61 7474 723a  ss for :py:attr:
+0000cbf0: 607e 5374 7261 7465 6779 2e66 6173 7460  `~Strategy.fast`
+0000cc00: 2073 7472 6174 6567 792e 0a0a 2020 2020   strategy...    
+0000cc10: 2020 2020 4974 2773 2073 7469 6c6c 2075      It's still u
+0000cc20: 7365 6675 6c20 7768 656e 2075 7369 6e67  seful when using
+0000cc30: 203a 7079 3a61 7474 723a 607e 5374 7261   :py:attr:`~Stra
+0000cc40: 7465 6779 2e64 6661 7374 6020 7374 7261  tegy.dfast` stra
+0000cc50: 7465 6779 2c20 696e 2077 6869 6368 2063  tegy, in which c
+0000cc60: 6173 6520 6974 2064 6566 696e 6573 2061  ase it defines a
+0000cc70: 2073 6563 6f6e 6461 7279 2070 726f 6265   secondary probe
+0000cc80: 2074 6162 6c65 2e0a 0a20 2020 2020 2020   table...       
+0000cc90: 2053 7065 6369 616c 3a20 7661 6c75 6520   Special: value 
+0000cca0: 6060 3060 6020 6d65 616e 7320 2275 7365  ``0`` means "use
+0000ccb0: 2064 6566 6175 6c74 2063 6861 696e 4c6f   default chainLo
+0000ccc0: 6722 2c20 7468 656e 2074 6865 2076 616c  g", then the val
+0000ccd0: 7565 2069 7320 6479 6e61 6d69 6361 6c6c  ue is dynamicall
+0000cce0: 7920 7365 742c 2073 6565 2022 4322 2063  y set, see "C" c
+0000ccf0: 6f6c 756d 6e20 696e 2060 7468 6973 2074  olumn in `this t
+0000cd00: 6162 6c65 203c 6874 7470 733a 2f2f 6769  able <https://gi
+0000cd10: 7468 7562 2e63 6f6d 2f66 6163 6562 6f6f  thub.com/faceboo
+0000cd20: 6b2f 7a73 7464 2f62 6c6f 622f 7265 6c65  k/zstd/blob/rele
+0000cd30: 6173 652f 6c69 622f 636f 6d70 7265 7373  ase/lib/compress
+0000cd40: 2f63 6c65 7665 6c73 2e68 3e60 5f2e 0a0a  /clevels.h>`_...
+0000cd50: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
+0000cd60: 7574 653a 3a20 7365 6172 6368 4c6f 670a  ute:: searchLog.
+0000cd70: 0a20 2020 2020 2020 204e 756d 6265 7220  .        Number 
+0000cd80: 6f66 2073 6561 7263 6820 6174 7465 6d70  of search attemp
+0000cd90: 7473 2c20 6173 2061 2070 6f77 6572 206f  ts, as a power o
+0000cda0: 6620 322e 0a0a 2020 2020 2020 2020 4d6f  f 2...        Mo
+0000cdb0: 7265 2061 7474 656d 7074 7320 7265 7375  re attempts resu
+0000cdc0: 6c74 2069 6e20 6265 7474 6572 2061 6e64  lt in better and
+0000cdd0: 2073 6c6f 7765 7220 636f 6d70 7265 7373   slower compress
+0000cde0: 696f 6e2e 0a0a 2020 2020 2020 2020 5468  ion...        Th
+0000cdf0: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
+0000ce00: 7573 656c 6573 7320 666f 7220 3a70 793a  useless for :py:
+0000ce10: 6174 7472 3a60 7e53 7472 6174 6567 792e  attr:`~Strategy.
+0000ce20: 6661 7374 6020 616e 6420 3a70 793a 6174  fast` and :py:at
+0000ce30: 7472 3a60 7e53 7472 6174 6567 792e 6466  tr:`~Strategy.df
+0000ce40: 6173 7460 2073 7472 6174 6567 6965 732e  ast` strategies.
+0000ce50: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
+0000ce60: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
+0000ce70: 6561 6e73 2022 7573 6520 6465 6661 756c  eans "use defaul
+0000ce80: 7420 7365 6172 6368 4c6f 6722 2c20 7468  t searchLog", th
+0000ce90: 656e 2074 6865 2076 616c 7565 2069 7320  en the value is 
+0000cea0: 6479 6e61 6d69 6361 6c6c 7920 7365 742c  dynamically set,
+0000ceb0: 2073 6565 2022 5322 2063 6f6c 756d 6e20   see "S" column 
+0000cec0: 696e 2060 7468 6973 2074 6162 6c65 203c  in `this table <
+0000ced0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000cee0: 6f6d 2f66 6163 6562 6f6f 6b2f 7a73 7464  om/facebook/zstd
+0000cef0: 2f62 6c6f 622f 7265 6c65 6173 652f 6c69  /blob/release/li
+0000cf00: 622f 636f 6d70 7265 7373 2f63 6c65 7665  b/compress/cleve
+0000cf10: 6c73 2e68 3e60 5f2e 0a0a 2020 2020 2e2e  ls.h>`_...    ..
+0000cf20: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
+0000cf30: 6d69 6e4d 6174 6368 0a0a 2020 2020 2020  minMatch..      
+0000cf40: 2020 4d69 6e69 6d75 6d20 7369 7a65 206f    Minimum size o
+0000cf50: 6620 7365 6172 6368 6564 206d 6174 6368  f searched match
+0000cf60: 6573 2e0a 0a20 2020 2020 2020 204e 6f74  es...        Not
+0000cf70: 6520 7468 6174 205a 7374 616e 6461 7264  e that Zstandard
+0000cf80: 2063 616e 2073 7469 6c6c 2066 696e 6420   can still find 
+0000cf90: 6d61 7463 6865 7320 6f66 2073 6d61 6c6c  matches of small
+0000cfa0: 6572 2073 697a 652c 2069 7420 6a75 7374  er size, it just
+0000cfb0: 2074 7765 616b 7320 6974 7320 7365 6172   tweaks its sear
+0000cfc0: 6368 2061 6c67 6f72 6974 686d 2074 6f20  ch algorithm to 
+0000cfd0: 6c6f 6f6b 2066 6f72 2074 6869 7320 7369  look for this si
+0000cfe0: 7a65 2061 6e64 206c 6172 6765 722e 0a0a  ze and larger...
+0000cff0: 2020 2020 2020 2020 4c61 7267 6572 2076          Larger v
+0000d000: 616c 7565 7320 696e 6372 6561 7365 2063  alues increase c
+0000d010: 6f6d 7072 6573 7369 6f6e 2061 6e64 2064  ompression and d
+0000d020: 6563 6f6d 7072 6573 7369 6f6e 2073 7065  ecompression spe
+0000d030: 6564 2c20 6275 7420 6465 6372 6561 7365  ed, but decrease
+0000d040: 2072 6174 696f 2e0a 0a20 2020 2020 2020   ratio...       
+0000d050: 204d 7573 7420 6265 2063 6c61 6d70 6564   Must be clamped
+0000d060: 2062 6574 7765 656e 2060 605a 5354 445f   between ``ZSTD_
+0000d070: 4d49 4e4d 4154 4348 5f4d 494e 6060 2061  MINMATCH_MIN`` a
+0000d080: 6e64 2060 605a 5354 445f 4d49 4e4d 4154  nd ``ZSTD_MINMAT
+0000d090: 4348 5f4d 4158 6060 2e0a 0a20 2020 2020  CH_MAX``...     
+0000d0a0: 2020 204e 6f74 6520 7468 6174 2063 7572     Note that cur
+0000d0b0: 7265 6e74 6c79 2c20 666f 7220 616c 6c20  rently, for all 
+0000d0c0: 7374 7261 7465 6769 6573 203c 203a 7079  strategies < :py
+0000d0d0: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
+0000d0e0: 2e62 746f 7074 602c 2065 6666 6563 7469  .btopt`, effecti
+0000d0f0: 7665 206d 696e 696d 756d 2069 7320 6060  ve minimum is ``
+0000d100: 3460 602c 2066 6f72 2061 6c6c 2073 7472  4``, for all str
+0000d110: 6174 6567 6965 7320 3e20 3a70 793a 6174  ategies > :py:at
+0000d120: 7472 3a60 7e53 7472 6174 6567 792e 6661  tr:`~Strategy.fa
+0000d130: 7374 602c 2065 6666 6563 7469 7665 206d  st`, effective m
+0000d140: 6178 696d 756d 2069 7320 6060 3660 602e  aximum is ``6``.
+0000d150: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
+0000d160: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
+0000d170: 6561 6e73 2022 7573 6520 6465 6661 756c  eans "use defaul
+0000d180: 7420 6d69 6e4d 6174 6368 4c65 6e67 7468  t minMatchLength
+0000d190: 222c 2074 6865 6e20 7468 6520 7661 6c75  ", then the valu
+0000d1a0: 6520 6973 2064 796e 616d 6963 616c 6c79  e is dynamically
+0000d1b0: 2073 6574 2c20 7365 6520 224c 2220 636f   set, see "L" co
+0000d1c0: 6c75 6d6e 2069 6e20 6074 6869 7320 7461  lumn in `this ta
+0000d1d0: 626c 6520 3c68 7474 7073 3a2f 2f67 6974  ble <https://git
+0000d1e0: 6875 622e 636f 6d2f 6661 6365 626f 6f6b  hub.com/facebook
+0000d1f0: 2f7a 7374 642f 626c 6f62 2f72 656c 6561  /zstd/blob/relea
+0000d200: 7365 2f6c 6962 2f63 6f6d 7072 6573 732f  se/lib/compress/
+0000d210: 636c 6576 656c 732e 683e 605f 2e0a 0a20  clevels.h>`_... 
+0000d220: 2020 202e 2e20 7079 3a61 7474 7269 6275     .. py:attribu
+0000d230: 7465 3a3a 2074 6172 6765 744c 656e 6774  te:: targetLengt
+0000d240: 680a 0a20 2020 2020 2020 2049 6d70 6163  h..        Impac
+0000d250: 7420 6f66 2074 6869 7320 6669 656c 6420  t of this field 
+0000d260: 6465 7065 6e64 7320 6f6e 2073 7472 6174  depends on strat
+0000d270: 6567 792e 0a0a 2020 2020 2020 2020 466f  egy...        Fo
+0000d280: 7220 7374 7261 7465 6769 6573 203a 7079  r strategies :py
+0000d290: 3a61 7474 723a 607e 5374 7261 7465 6779  :attr:`~Strategy
+0000d2a0: 2e62 746f 7074 602c 203a 7079 3a61 7474  .btopt`, :py:att
+0000d2b0: 723a 607e 5374 7261 7465 6779 2e62 7475  r:`~Strategy.btu
+0000d2c0: 6c74 7261 6020 2620 3a70 793a 6174 7472  ltra` & :py:attr
+0000d2d0: 3a60 7e53 7472 6174 6567 792e 6274 756c  :`~Strategy.btul
+0000d2e0: 7472 6132 603a 0a0a 2020 2020 2020 2020  tra2`:..        
+0000d2f0: 2020 2020 4c65 6e67 7468 206f 6620 4d61      Length of Ma
+0000d300: 7463 6820 636f 6e73 6964 6572 6564 2022  tch considered "
+0000d310: 676f 6f64 2065 6e6f 7567 6822 2074 6f20  good enough" to 
+0000d320: 7374 6f70 2073 6561 7263 682e 0a0a 2020  stop search...  
+0000d330: 2020 2020 2020 2020 2020 4c61 7267 6572            Larger
+0000d340: 2076 616c 7565 7320 6d61 6b65 2063 6f6d   values make com
+0000d350: 7072 6573 7369 6f6e 2073 7472 6f6e 6765  pression stronge
+0000d360: 722c 2061 6e64 2073 6c6f 7765 722e 0a0a  r, and slower...
+0000d370: 2020 2020 2020 2020 466f 7220 7374 7261          For stra
+0000d380: 7465 6779 203a 7079 3a61 7474 723a 607e  tegy :py:attr:`~
+0000d390: 5374 7261 7465 6779 2e66 6173 7460 3a0a  Strategy.fast`:.
+0000d3a0: 0a20 2020 2020 2020 2020 2020 2044 6973  .            Dis
+0000d3b0: 7461 6e63 6520 6265 7477 6565 6e20 6d61  tance between ma
+0000d3c0: 7463 6820 7361 6d70 6c69 6e67 2e0a 0a20  tch sampling... 
+0000d3d0: 2020 2020 2020 2020 2020 204c 6172 6765             Large
+0000d3e0: 7220 7661 6c75 6573 206d 616b 6520 636f  r values make co
+0000d3f0: 6d70 7265 7373 696f 6e20 6661 7374 6572  mpression faster
+0000d400: 2c20 616e 6420 7765 616b 6572 2e0a 0a20  , and weaker... 
+0000d410: 2020 2020 2020 2053 7065 6369 616c 3a20         Special: 
+0000d420: 7661 6c75 6520 6060 3060 6020 6d65 616e  value ``0`` mean
+0000d430: 7320 2275 7365 2064 6566 6175 6c74 2074  s "use default t
+0000d440: 6172 6765 744c 656e 6774 6822 2c20 7468  argetLength", th
+0000d450: 656e 2074 6865 2076 616c 7565 2069 7320  en the value is 
+0000d460: 6479 6e61 6d69 6361 6c6c 7920 7365 742c  dynamically set,
+0000d470: 2073 6565 2022 544c 2220 636f 6c75 6d6e   see "TL" column
+0000d480: 2069 6e20 6074 6869 7320 7461 626c 6520   in `this table 
+0000d490: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+0000d4a0: 636f 6d2f 6661 6365 626f 6f6b 2f7a 7374  com/facebook/zst
+0000d4b0: 642f 626c 6f62 2f72 656c 6561 7365 2f6c  d/blob/release/l
+0000d4c0: 6962 2f63 6f6d 7072 6573 732f 636c 6576  ib/compress/clev
+0000d4d0: 656c 732e 683e 605f 2e0a 0a20 2020 202e  els.h>`_...    .
+0000d4e0: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
+0000d4f0: 2073 7472 6174 6567 790a 0a20 2020 2020   strategy..     
+0000d500: 2020 2053 6565 203a 7079 3a61 7474 723a     See :py:attr:
+0000d510: 6053 7472 6174 6567 7960 2063 6c61 7373  `Strategy` class
+0000d520: 2064 6566 696e 6974 696f 6e2e 0a0a 2020   definition...  
+0000d530: 2020 2020 2020 5468 6520 6869 6768 6572        The higher
+0000d540: 2074 6865 2076 616c 7565 206f 6620 7365   the value of se
+0000d550: 6c65 6374 6564 2073 7472 6174 6567 792c  lected strategy,
+0000d560: 2074 6865 206d 6f72 6520 636f 6d70 6c65   the more comple
+0000d570: 7820 6974 2069 732c 2072 6573 756c 7469  x it is, resulti
+0000d580: 6e67 2069 6e20 7374 726f 6e67 6572 2061  ng in stronger a
+0000d590: 6e64 2073 6c6f 7765 7220 636f 6d70 7265  nd slower compre
+0000d5a0: 7373 696f 6e2e 0a0a 2020 2020 2020 2020  ssion...        
+0000d5b0: 5370 6563 6961 6c3a 2076 616c 7565 2060  Special: value `
+0000d5c0: 6030 6060 206d 6561 6e73 2022 7573 6520  `0`` means "use 
+0000d5d0: 6465 6661 756c 7420 7374 7261 7465 6779  default strategy
+0000d5e0: 222c 2074 6865 6e20 7468 6520 7661 6c75  ", then the valu
+0000d5f0: 6520 6973 2064 796e 616d 6963 616c 6c79  e is dynamically
+0000d600: 2073 6574 2c20 7365 6520 2273 7472 6174   set, see "strat
+0000d610: 2220 636f 6c75 6d6e 2069 6e20 6074 6869  " column in `thi
+0000d620: 7320 7461 626c 6520 3c68 7474 7073 3a2f  s table <https:/
+0000d630: 2f67 6974 6875 622e 636f 6d2f 6661 6365  /github.com/face
+0000d640: 626f 6f6b 2f7a 7374 642f 626c 6f62 2f72  book/zstd/blob/r
+0000d650: 656c 6561 7365 2f6c 6962 2f63 6f6d 7072  elease/lib/compr
+0000d660: 6573 732f 636c 6576 656c 732e 683e 605f  ess/clevels.h>`_
+0000d670: 2e0a 0a20 2020 202e 2e20 7079 3a61 7474  ...    .. py:att
+0000d680: 7269 6275 7465 3a3a 2065 6e61 626c 654c  ribute:: enableL
+0000d690: 6f6e 6744 6973 7461 6e63 654d 6174 6368  ongDistanceMatch
+0000d6a0: 696e 670a 0a20 2020 2020 2020 2045 6e61  ing..        Ena
+0000d6b0: 626c 6520 6c6f 6e67 2064 6973 7461 6e63  ble long distanc
+0000d6c0: 6520 6d61 7463 6869 6e67 2e0a 0a20 2020  e matching...   
+0000d6d0: 2020 2020 2044 6566 6175 6c74 2076 616c       Default val
+0000d6e0: 7565 2069 7320 6060 3060 602c 2063 616e  ue is ``0``, can
+0000d6f0: 2062 6520 6060 3160 602e 0a0a 2020 2020   be ``1``...    
+0000d700: 2020 2020 5468 6973 2070 6172 616d 6574      This paramet
+0000d710: 6572 2069 7320 6465 7369 676e 6564 2074  er is designed t
+0000d720: 6f20 696d 7072 6f76 6520 636f 6d70 7265  o improve compre
+0000d730: 7373 696f 6e20 7261 7469 6f2c 2066 6f72  ssion ratio, for
+0000d740: 206c 6172 6765 2069 6e70 7574 732c 2062   large inputs, b
+0000d750: 7920 6669 6e64 696e 6720 6c61 7267 6520  y finding large 
+0000d760: 6d61 7463 6865 7320 6174 206c 6f6e 6720  matches at long 
+0000d770: 6469 7374 616e 6365 2e20 4974 2069 6e63  distance. It inc
+0000d780: 7265 6173 6573 206d 656d 6f72 7920 7573  reases memory us
+0000d790: 6167 6520 616e 6420 7769 6e64 6f77 2073  age and window s
+0000d7a0: 697a 652e 0a0a 2020 2020 2020 2020 4e6f  ize...        No
+0000d7b0: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
+0000d7c0: 2a20 456e 6162 6c69 6e67 2074 6869 7320  * Enabling this 
+0000d7d0: 7061 7261 6d65 7465 7220 696e 6372 6561  parameter increa
+0000d7e0: 7365 7320 6465 6661 756c 7420 3a70 793a  ses default :py:
+0000d7f0: 6174 7472 3a60 7e43 5061 7261 6d65 7465  attr:`~CParamete
+0000d800: 722e 7769 6e64 6f77 4c6f 6760 2074 6f20  r.windowLog` to 
+0000d810: 3132 3820 4d69 4220 6578 6365 7074 2077  128 MiB except w
+0000d820: 6865 6e20 6578 7072 6573 736c 7920 7365  hen expressly se
+0000d830: 7420 746f 2061 2064 6966 6665 7265 6e74  t to a different
+0000d840: 2076 616c 7565 2e0a 2020 2020 2020 2020   value..        
+0000d850: 2020 2020 2a20 5468 6973 2077 696c 6c20      * This will 
+0000d860: 6265 2065 6e61 626c 6564 2062 7920 6465  be enabled by de
+0000d870: 6661 756c 7420 6966 203a 7079 3a61 7474  fault if :py:att
+0000d880: 723a 607e 4350 6172 616d 6574 6572 2e77  r:`~CParameter.w
+0000d890: 696e 646f 774c 6f67 6020 3e3d 2031 3238  indowLog` >= 128
+0000d8a0: 204d 6942 2061 6e64 2063 6f6d 7072 6573   MiB and compres
+0000d8b0: 7369 6f6e 2073 7472 6174 6567 7920 3e3d  sion strategy >=
+0000d8c0: 203a 7079 3a61 7474 723a 607e 5374 7261   :py:attr:`~Stra
+0000d8d0: 7465 6779 2e62 746f 7074 6020 2863 6f6d  tegy.btopt` (com
+0000d8e0: 7072 6573 7369 6f6e 206c 6576 656c 2031  pression level 1
+0000d8f0: 362b 292e 0a0a 2020 2020 2e2e 2070 793a  6+)...    .. py:
+0000d900: 6174 7472 6962 7574 653a 3a20 6c64 6d48  attribute:: ldmH
+0000d910: 6173 684c 6f67 0a0a 2020 2020 2020 2020  ashLog..        
+0000d920: 5369 7a65 206f 6620 7468 6520 7461 626c  Size of the tabl
+0000d930: 6520 666f 7220 6c6f 6e67 2064 6973 7461  e for long dista
+0000d940: 6e63 6520 6d61 7463 6869 6e67 2c20 6173  nce matching, as
+0000d950: 2061 2070 6f77 6572 206f 6620 322e 0a0a   a power of 2...
+0000d960: 2020 2020 2020 2020 4c61 7267 6572 2076          Larger v
+0000d970: 616c 7565 7320 696e 6372 6561 7365 206d  alues increase m
+0000d980: 656d 6f72 7920 7573 6167 6520 616e 6420  emory usage and 
+0000d990: 636f 6d70 7265 7373 696f 6e20 7261 7469  compression rati
+0000d9a0: 6f2c 2062 7574 2064 6563 7265 6173 6520  o, but decrease 
+0000d9b0: 636f 6d70 7265 7373 696f 6e20 7370 6565  compression spee
+0000d9c0: 642e 0a0a 2020 2020 2020 2020 4d75 7374  d...        Must
+0000d9d0: 2062 6520 636c 616d 7065 6420 6265 7477   be clamped betw
+0000d9e0: 6565 6e20 6060 5a53 5444 5f48 4153 484c  een ``ZSTD_HASHL
+0000d9f0: 4f47 5f4d 494e 6060 2061 6e64 2060 605a  OG_MIN`` and ``Z
+0000da00: 5354 445f 4841 5348 4c4f 475f 4d41 5860  STD_HASHLOG_MAX`
+0000da10: 602c 2064 6566 6175 6c74 3a20 3a70 793a  `, default: :py:
+0000da20: 6174 7472 3a60 7e43 5061 7261 6d65 7465  attr:`~CParamete
+0000da30: 722e 7769 6e64 6f77 4c6f 6760 202d 2037  r.windowLog` - 7
+0000da40: 2e0a 0a20 2020 2020 2020 2053 7065 6369  ...        Speci
+0000da50: 616c 3a20 7661 6c75 6520 6060 3060 6020  al: value ``0`` 
+0000da60: 6d65 616e 7320 2261 7574 6f6d 6174 6963  means "automatic
+0000da70: 616c 6c79 2064 6574 6572 6d69 6e65 2068  ally determine h
+0000da80: 6173 686c 6f67 222e 0a0a 2020 2020 2e2e  ashlog"...    ..
+0000da90: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
+0000daa0: 6c64 6d4d 696e 4d61 7463 680a 0a20 2020  ldmMinMatch..   
+0000dab0: 2020 2020 204d 696e 696d 756d 206d 6174       Minimum mat
+0000dac0: 6368 2073 697a 6520 666f 7220 6c6f 6e67  ch size for long
+0000dad0: 2064 6973 7461 6e63 6520 6d61 7463 6865   distance matche
+0000dae0: 722e 0a0a 2020 2020 2020 2020 4c61 7267  r...        Larg
+0000daf0: 6572 2f74 6f6f 2073 6d61 6c6c 2076 616c  er/too small val
+0000db00: 7565 7320 7573 7561 6c6c 7920 6465 6372  ues usually decr
+0000db10: 6561 7365 2063 6f6d 7072 6573 7369 6f6e  ease compression
+0000db20: 2072 6174 696f 2e0a 0a20 2020 2020 2020   ratio...       
+0000db30: 204d 7573 7420 6265 2063 6c61 6d70 6564   Must be clamped
+0000db40: 2062 6574 7765 656e 2060 605a 5354 445f   between ``ZSTD_
+0000db50: 4c44 4d5f 4d49 4e4d 4154 4348 5f4d 494e  LDM_MINMATCH_MIN
+0000db60: 6060 2061 6e64 2060 605a 5354 445f 4c44  `` and ``ZSTD_LD
+0000db70: 4d5f 4d49 4e4d 4154 4348 5f4d 4158 6060  M_MINMATCH_MAX``
+0000db80: 2e0a 0a20 2020 2020 2020 2053 7065 6369  ...        Speci
+0000db90: 616c 3a20 7661 6c75 6520 6060 3060 6020  al: value ``0`` 
+0000dba0: 6d65 616e 7320 2275 7365 2064 6566 6175  means "use defau
+0000dbb0: 6c74 2076 616c 7565 2220 2864 6566 6175  lt value" (defau
+0000dbc0: 6c74 3a20 3634 292e 0a0a 2020 2020 2e2e  lt: 64)...    ..
+0000dbd0: 2070 793a 6174 7472 6962 7574 653a 3a20   py:attribute:: 
+0000dbe0: 6c64 6d42 7563 6b65 7453 697a 654c 6f67  ldmBucketSizeLog
+0000dbf0: 0a0a 2020 2020 2020 2020 4c6f 6720 7369  ..        Log si
+0000dc00: 7a65 206f 6620 6561 6368 2062 7563 6b65  ze of each bucke
+0000dc10: 7420 696e 2074 6865 204c 444d 2068 6173  t in the LDM has
+0000dc20: 6820 7461 626c 6520 666f 7220 636f 6c6c  h table for coll
+0000dc30: 6973 696f 6e20 7265 736f 6c75 7469 6f6e  ision resolution
+0000dc40: 2e0a 0a20 2020 2020 2020 204c 6172 6765  ...        Large
+0000dc50: 7220 7661 6c75 6573 2069 6d70 726f 7665  r values improve
+0000dc60: 2063 6f6c 6c69 7369 6f6e 2072 6573 6f6c   collision resol
+0000dc70: 7574 696f 6e20 6275 7420 6465 6372 6561  ution but decrea
+0000dc80: 7365 2063 6f6d 7072 6573 7369 6f6e 2073  se compression s
+0000dc90: 7065 6564 2e0a 0a20 2020 2020 2020 2054  peed...        T
+0000dca0: 6865 206d 6178 696d 756d 2076 616c 7565  he maximum value
+0000dcb0: 2069 7320 6060 5a53 5444 5f4c 444d 5f42   is ``ZSTD_LDM_B
+0000dcc0: 5543 4b45 5453 495a 454c 4f47 5f4d 4158  UCKETSIZELOG_MAX
+0000dcd0: 6060 2e0a 0a20 2020 2020 2020 2053 7065  ``...        Spe
+0000dce0: 6369 616c 3a20 7661 6c75 6520 6060 3060  cial: value ``0`
+0000dcf0: 6020 6d65 616e 7320 2275 7365 2064 6566  ` means "use def
+0000dd00: 6175 6c74 2076 616c 7565 2220 2864 6566  ault value" (def
+0000dd10: 6175 6c74 3a20 3329 2e0a 0a20 2020 202e  ault: 3)...    .
+0000dd20: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
+0000dd30: 206c 646d 4861 7368 5261 7465 4c6f 670a   ldmHashRateLog.
+0000dd40: 0a20 2020 2020 2020 2046 7265 7175 656e  .        Frequen
+0000dd50: 6379 206f 6620 696e 7365 7274 696e 672f  cy of inserting/
+0000dd60: 6c6f 6f6b 696e 6720 7570 2065 6e74 7269  looking up entri
+0000dd70: 6573 2069 6e74 6f20 7468 6520 4c44 4d20  es into the LDM 
+0000dd80: 6861 7368 2074 6162 6c65 2e0a 0a20 2020  hash table...   
+0000dd90: 2020 2020 204d 7573 7420 6265 2063 6c61       Must be cla
+0000dda0: 6d70 6564 2062 6574 7765 656e 2030 2061  mped between 0 a
+0000ddb0: 6e64 2060 6028 5a53 5444 5f57 494e 444f  nd ``(ZSTD_WINDO
+0000ddc0: 574c 4f47 5f4d 4158 202d 205a 5354 445f  WLOG_MAX - ZSTD_
+0000ddd0: 4841 5348 4c4f 475f 4d49 4e29 6060 2e0a  HASHLOG_MIN)``..
+0000dde0: 0a20 2020 2020 2020 2044 6566 6175 6c74  .        Default
+0000ddf0: 2069 7320 4d41 5828 302c 2028 3a70 793a   is MAX(0, (:py:
+0000de00: 6174 7472 3a60 7e43 5061 7261 6d65 7465  attr:`~CParamete
+0000de10: 722e 7769 6e64 6f77 4c6f 6760 202d 203a  r.windowLog` - :
+0000de20: 7079 3a61 7474 723a 607e 4350 6172 616d  py:attr:`~CParam
+0000de30: 6574 6572 2e6c 646d 4861 7368 4c6f 6760  eter.ldmHashLog`
+0000de40: 2929 2c20 6f70 7469 6d69 7a69 6e67 2068  )), optimizing h
+0000de50: 6173 6820 7461 626c 6520 7573 6167 652e  ash table usage.
+0000de60: 0a0a 2020 2020 2020 2020 4c61 7267 6572  ..        Larger
+0000de70: 2076 616c 7565 7320 696d 7072 6f76 6520   values improve 
+0000de80: 636f 6d70 7265 7373 696f 6e20 7370 6565  compression spee
+0000de90: 642e 0a0a 2020 2020 2020 2020 4465 7669  d...        Devi
+0000dea0: 6174 696e 6720 6661 7220 6672 6f6d 2064  ating far from d
+0000deb0: 6566 6175 6c74 2076 616c 7565 2077 696c  efault value wil
+0000dec0: 6c20 6c69 6b65 6c79 2072 6573 756c 7420  l likely result 
+0000ded0: 696e 2061 2063 6f6d 7072 6573 7369 6f6e  in a compression
+0000dee0: 2072 6174 696f 2064 6563 7265 6173 652e   ratio decrease.
+0000def0: 0a0a 2020 2020 2020 2020 5370 6563 6961  ..        Specia
+0000df00: 6c3a 2076 616c 7565 2060 6030 6060 206d  l: value ``0`` m
+0000df10: 6561 6e73 2022 6175 746f 6d61 7469 6361  eans "automatica
+0000df20: 6c6c 7920 6465 7465 726d 696e 6520 6861  lly determine ha
+0000df30: 7368 5261 7465 4c6f 6722 2e0a 0a20 2020  shRateLog"...   
+0000df40: 202e 2e20 5f63 6f6e 7465 6e74 5f73 697a   .. _content_siz
+0000df50: 653a 0a0a 2020 2020 2e2e 2070 793a 6174  e:..    .. py:at
+0000df60: 7472 6962 7574 653a 3a20 636f 6e74 656e  tribute:: conten
+0000df70: 7453 697a 6546 6c61 670a 0a20 2020 2020  tSizeFlag..     
+0000df80: 2020 2055 6e63 6f6d 7072 6573 7365 6420     Uncompressed 
+0000df90: 636f 6e74 656e 7420 7369 7a65 2077 696c  content size wil
+0000dfa0: 6c20 6265 2077 7269 7474 656e 2069 6e74  l be written int
+0000dfb0: 6f20 6672 616d 6520 6865 6164 6572 2077  o frame header w
+0000dfc0: 6865 6e65 7665 7220 6b6e 6f77 6e2e 0a0a  henever known...
+0000dfd0: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
+0000dfe0: 7661 6c75 6520 6973 2060 6031 6060 2c20  value is ``1``, 
+0000dff0: 6361 6e20 6265 2060 6030 6060 2e0a 0a20  can be ``0``... 
+0000e000: 2020 2020 2020 2049 6e20 7472 6164 6974         In tradit
+0000e010: 696f 6e61 6c20 7374 7265 616d 696e 6720  ional streaming 
+0000e020: 636f 6d70 7265 7373 696f 6e2c 2063 6f6e  compression, con
+0000e030: 7465 6e74 2073 697a 6520 6973 2075 6e6b  tent size is unk
+0000e040: 6e6f 776e 2e0a 0a20 2020 2020 2020 2049  nown...        I
+0000e050: 6e20 7468 6573 6520 636f 6d70 7265 7373  n these compress
+0000e060: 696f 6e73 2c20 7468 6520 636f 6e74 656e  ions, the conten
+0000e070: 7420 7369 7a65 2069 7320 6b6e 6f77 6e3a  t size is known:
+0000e080: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
+0000e090: 3a70 793a 6675 6e63 3a60 636f 6d70 7265  :py:func:`compre
+0000e0a0: 7373 6020 6675 6e63 7469 6f6e 0a20 2020  ss` function.   
+0000e0b0: 2020 2020 2020 2020 202a 203a 7079 3a66           * :py:f
+0000e0c0: 756e 633a 6072 6963 686d 656d 5f63 6f6d  unc:`richmem_com
+0000e0d0: 7072 6573 7360 2066 756e 6374 696f 6e0a  press` function.
+0000e0e0: 2020 2020 2020 2020 2020 2020 2a20 3a70              * :p
+0000e0f0: 793a 636c 6173 733a 605a 7374 6443 6f6d  y:class:`ZstdCom
+0000e100: 7072 6573 736f 7260 2063 6c61 7373 2075  pressor` class u
+0000e110: 7369 6e67 2061 2073 696e 676c 6520 3a70  sing a single :p
+0000e120: 793a 6174 7472 3a60 7e5a 7374 6443 6f6d  y:attr:`~ZstdCom
+0000e130: 7072 6573 736f 722e 464c 5553 485f 4652  pressor.FLUSH_FR
+0000e140: 414d 4560 206d 6f64 650a 2020 2020 2020  AME` mode.      
+0000e150: 2020 2020 2020 2a20 3a70 793a 636c 6173        * :py:clas
+0000e160: 733a 6052 6963 684d 656d 5a73 7464 436f  s:`RichMemZstdCo
+0000e170: 6d70 7265 7373 6f72 6020 636c 6173 730a  mpressor` class.
+0000e180: 2020 2020 2020 2020 2020 2020 2a20 3a70              * :p
+0000e190: 793a 6675 6e63 3a60 636f 6d70 7265 7373  y:func:`compress
+0000e1a0: 5f73 7472 6561 6d60 2066 756e 6374 696f  _stream` functio
+0000e1b0: 6e20 7365 7474 696e 6720 2a70 6c65 6467  n setting *pledg
+0000e1c0: 6564 5f69 6e70 7574 5f73 697a 652a 2070  ed_input_size* p
+0000e1d0: 6172 616d 6574 6572 0a0a 2020 2020 2020  arameter..      
+0000e1e0: 2020 5468 6520 6669 656c 6420 696e 2066    The field in f
+0000e1f0: 7261 6d65 2068 6561 6465 7220 6973 2031  rame header is 1
+0000e200: 2f32 2f34 2f38 2062 7974 6573 2c20 6465  /2/4/8 bytes, de
+0000e210: 7065 6e64 696e 6720 6f6e 2073 697a 6520  pending on size 
+0000e220: 7661 6c75 652e 2049 7420 6d61 7920 6865  value. It may he
+0000e230: 6c70 2064 6563 6f6d 7072 6573 7369 6f6e  lp decompression
+0000e240: 2063 6f64 6520 746f 2061 6c6c 6f63 6174   code to allocat
+0000e250: 6520 6f75 7470 7574 2062 7566 6665 7220  e output buffer 
+0000e260: 6661 7374 6572 2e0a 0a20 2020 2020 2020  faster...       
+0000e270: 205c 2a20 3a70 793a 636c 6173 733a 605a   \* :py:class:`Z
+0000e280: 7374 6443 6f6d 7072 6573 736f 7260 2068  stdCompressor` h
+0000e290: 6173 2061 6e20 756e 646f 6375 6d65 6e74  as an undocument
+0000e2a0: 6564 206d 6574 686f 6420 746f 2073 6574  ed method to set
+0000e2b0: 2074 6865 2073 697a 652c 2060 6068 656c   the size, ``hel
+0000e2c0: 7028 5a73 7464 436f 6d70 7265 7373 6f72  p(ZstdCompressor
+0000e2d0: 2e5f 7365 745f 706c 6564 6765 645f 696e  ._set_pledged_in
+0000e2e0: 7075 745f 7369 7a65 2960 6020 746f 2073  put_size)`` to s
+0000e2f0: 6565 2074 6865 2075 7361 6765 2e0a 0a20  ee the usage... 
+0000e300: 2020 202e 2e20 7079 3a61 7474 7269 6275     .. py:attribu
+0000e310: 7465 3a3a 2063 6865 636b 7375 6d46 6c61  te:: checksumFla
+0000e320: 670a 0a20 2020 2020 2020 2041 2034 2d62  g..        A 4-b
+0000e330: 7974 6520 6368 6563 6b73 756d 2028 5858  yte checksum (XX
+0000e340: 4836 3429 206f 6620 756e 636f 6d70 7265  H64) of uncompre
+0000e350: 7373 6564 2063 6f6e 7465 6e74 2069 7320  ssed content is 
+0000e360: 7772 6974 7465 6e20 6174 2074 6865 2065  written at the e
+0000e370: 6e64 206f 6620 6672 616d 652e 0a0a 2020  nd of frame...  
+0000e380: 2020 2020 2020 4465 6661 756c 7420 7661        Default va
+0000e390: 6c75 6520 6973 2060 6030 6060 2c20 6361  lue is ``0``, ca
+0000e3a0: 6e20 6265 2060 6031 6060 2e0a 0a20 2020  n be ``1``...   
+0000e3b0: 2020 2020 205a 7374 6427 7320 6465 636f       Zstd's deco
+0000e3c0: 6d70 7265 7373 696f 6e20 636f 6465 2076  mpression code v
+0000e3d0: 6572 6966 6965 7320 6974 2e20 4966 2063  erifies it. If c
+0000e3e0: 6865 636b 7375 6d20 6d69 736d 6174 6368  hecksum mismatch
+0000e3f0: 2c20 7261 6973 6573 2061 203a 7079 3a63  , raises a :py:c
+0000e400: 6c61 7373 3a60 5a73 7464 4572 726f 7260  lass:`ZstdError`
+0000e410: 2065 7863 6570 7469 6f6e 2c20 7769 7468   exception, with
+0000e420: 2061 206d 6573 7361 6765 206c 696b 6520   a message like 
+0000e430: 2252 6573 746f 7265 6420 6461 7461 2064  "Restored data d
+0000e440: 6f65 736e 2774 206d 6174 6368 2063 6865  oesn't match che
+0000e450: 636b 7375 6d22 2e0a 0a20 2020 202e 2e20  cksum"...    .. 
+0000e460: 7079 3a61 7474 7269 6275 7465 3a3a 2064  py:attribute:: d
+0000e470: 6963 7449 4446 6c61 670a 0a20 2020 2020  ictIDFlag..     
+0000e480: 2020 2057 6865 6e20 6170 706c 6963 6162     When applicab
+0000e490: 6c65 2c20 6469 6374 696f 6e61 7279 2773  le, dictionary's
+0000e4a0: 2049 4420 6973 2077 7269 7474 656e 2069   ID is written i
+0000e4b0: 6e74 6f20 6672 616d 6520 6865 6164 6572  nto frame header
+0000e4c0: 2e20 5365 6520 3a72 6566 3a60 7468 6973  . See :ref:`this
+0000e4d0: 206e 6f74 653c 6469 6374 5f69 643e 6020   note<dict_id>` 
+0000e4e0: 666f 7220 6465 7461 696c 732e 0a0a 2020  for details...  
+0000e4f0: 2020 2020 2020 4465 6661 756c 7420 7661        Default va
+0000e500: 6c75 6520 6973 2060 6031 6060 2c20 6361  lue is ``1``, ca
+0000e510: 6e20 6265 2060 6030 6060 2e0a 0a20 2020  n be ``0``...   
+0000e520: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+0000e530: 3a3a 206e 6257 6f72 6b65 7273 0a0a 2020  :: nbWorkers..  
+0000e540: 2020 2020 2020 5365 6c65 6374 2068 6f77        Select how
+0000e550: 206d 616e 7920 7468 7265 6164 7320 7769   many threads wi
+0000e560: 6c6c 2062 6520 7370 6177 6e65 6420 746f  ll be spawned to
+0000e570: 2063 6f6d 7072 6573 7320 696e 2070 6172   compress in par
+0000e580: 616c 6c65 6c2e 0a0a 2020 2020 2020 2020  allel...        
+0000e590: 5768 656e 206e 6257 6f72 6b65 7273 203e  When nbWorkers >
+0000e5a0: 3d20 6060 3160 602c 2065 6e61 626c 6573  = ``1``, enables
+0000e5b0: 206d 756c 7469 2d74 6872 6561 6465 6420   multi-threaded 
+0000e5c0: 636f 6d70 7265 7373 696f 6e2c 2060 6031  compression, ``1
+0000e5d0: 6060 206d 6561 6e73 2022 312d 7468 7265  `` means "1-thre
+0000e5e0: 6164 206d 756c 7469 2d74 6872 6561 6465  ad multi-threade
+0000e5f0: 6420 6d6f 6465 222e 2053 6565 203a 7265  d mode". See :re
+0000e600: 663a 607a 7374 6420 6d75 6c74 692d 7468  f:`zstd multi-th
+0000e610: 7265 6164 6564 2063 6f6d 7072 6573 7369  readed compressi
+0000e620: 6f6e 3c6d 745f 636f 6d70 7265 7373 696f  on<mt_compressio
+0000e630: 6e3e 6020 666f 7220 6465 7461 696c 732e  n>` for details.
+0000e640: 0a0a 2020 2020 2020 2020 4d6f 7265 2077  ..        More w
+0000e650: 6f72 6b65 7273 2069 6d70 726f 7665 2073  orkers improve s
+0000e660: 7065 6564 2c20 6275 7420 616c 736f 2069  peed, but also i
+0000e670: 6e63 7265 6173 6520 6d65 6d6f 7279 2075  ncrease memory u
+0000e680: 7361 6765 2e0a 0a20 2020 2020 2020 2060  sage...        `
+0000e690: 6030 6060 2028 6465 6661 756c 7429 206d  `0`` (default) m
+0000e6a0: 6561 6e73 2022 7369 6e67 6c65 2d74 6872  eans "single-thr
+0000e6b0: 6561 6465 6420 6d6f 6465 222c 206e 6f20  eaded mode", no 
+0000e6c0: 776f 726b 6572 2069 7320 7370 6177 6e65  worker is spawne
+0000e6d0: 642c 2063 6f6d 7072 6573 7369 6f6e 2069  d, compression i
+0000e6e0: 7320 7065 7266 6f72 6d65 6420 696e 7369  s performed insi
+0000e6f0: 6465 2063 616c 6c65 7227 7320 7468 7265  de caller's thre
+0000e700: 6164 2e0a 0a20 2020 202e 2e20 7665 7273  ad...    .. vers
+0000e710: 696f 6e63 6861 6e67 6564 3a3a 2030 2e31  ionchanged:: 0.1
+0000e720: 352e 310a 2020 2020 2020 2020 5365 7474  5.1.        Sett
+0000e730: 696e 6720 746f 2060 6031 6060 206d 6561  ing to ``1`` mea
+0000e740: 6e73 2022 312d 7468 7265 6164 206d 756c  ns "1-thread mul
+0000e750: 7469 2d74 6872 6561 6465 6420 6d6f 6465  ti-threaded mode
+0000e760: 222c 2069 6e73 7465 6164 206f 6620 2273  ", instead of "s
+0000e770: 696e 676c 652d 7468 7265 6164 6564 206d  ingle-threaded m
+0000e780: 6f64 6522 2e0a 0a20 2020 202e 2e20 7079  ode"...    .. py
+0000e790: 3a61 7474 7269 6275 7465 3a3a 206a 6f62  :attribute:: job
+0000e7a0: 5369 7a65 0a0a 2020 2020 2020 2020 5369  Size..        Si
+0000e7b0: 7a65 206f 6620 6120 636f 6d70 7265 7373  ze of a compress
+0000e7c0: 696f 6e20 6a6f 622c 2069 6e20 6279 7465  ion job, in byte
+0000e7d0: 732e 0a0a 2020 2020 2020 2020 5468 6973  s...        This
+0000e7e0: 2076 616c 7565 2069 7320 656e 666f 7263   value is enforc
+0000e7f0: 6564 206f 6e6c 7920 7768 656e 203a 7079  ed only when :py
+0000e800: 3a61 7474 723a 607e 4350 6172 616d 6574  :attr:`~CParamet
+0000e810: 6572 2e6e 6257 6f72 6b65 7273 6020 3e3d  er.nbWorkers` >=
+0000e820: 2031 2e0a 0a20 2020 2020 2020 2045 6163   1...        Eac
+0000e830: 6820 636f 6d70 7265 7373 696f 6e20 6a6f  h compression jo
+0000e840: 6220 6973 2063 6f6d 706c 6574 6564 2069  b is completed i
+0000e850: 6e20 7061 7261 6c6c 656c 2c20 736f 2074  n parallel, so t
+0000e860: 6869 7320 7661 6c75 6520 6361 6e20 696e  his value can in
+0000e870: 6469 7265 6374 6c79 2069 6d70 6163 7420  directly impact 
+0000e880: 7468 6520 6e75 6d62 6572 206f 6620 6163  the number of ac
+0000e890: 7469 7665 2074 6872 6561 6473 2e0a 0a20  tive threads... 
+0000e8a0: 2020 2020 2020 2060 6030 6060 206d 6561         ``0`` mea
+0000e8b0: 6e73 2064 6566 6175 6c74 2c20 7768 6963  ns default, whic
+0000e8c0: 6820 6973 2064 796e 616d 6963 616c 6c79  h is dynamically
+0000e8d0: 2064 6574 6572 6d69 6e65 6420 6261 7365   determined base
+0000e8e0: 6420 6f6e 2063 6f6d 7072 6573 7369 6f6e  d on compression
+0000e8f0: 2070 6172 616d 6574 6572 732e 0a0a 2020   parameters...  
+0000e900: 2020 2020 2020 4e6f 6e2d 7a65 726f 2076        Non-zero v
+0000e910: 616c 7565 2077 696c 6c20 6265 2073 696c  alue will be sil
+0000e920: 656e 746c 7920 636c 616d 7065 6420 746f  ently clamped to
+0000e930: 3a0a 0a20 2020 2020 2020 202a 206d 696e  :..        * min
+0000e940: 696d 756d 2076 616c 7565 3a20 6060 6d61  imum value: ``ma
+0000e950: 7828 6f76 6572 6c61 705f 7369 7a65 2c20  x(overlap_size, 
+0000e960: 3531 325f 4b69 4229 6060 2e20 6f76 6572  512_KiB)``. over
+0000e970: 6c61 705f 7369 7a65 2069 7320 7370 6563  lap_size is spec
+0000e980: 6966 6965 6420 6279 203a 7079 3a61 7474  ified by :py:att
+0000e990: 723a 607e 4350 6172 616d 6574 6572 2e6f  r:`~CParameter.o
+0000e9a0: 7665 726c 6170 4c6f 6760 2070 6172 616d  verlapLog` param
+0000e9b0: 6574 6572 2e0a 2020 2020 2020 2020 2a20  eter..        * 
+0000e9c0: 6d61 7869 6d75 6d20 7661 6c75 653a 2060  maximum value: `
+0000e9d0: 6035 3132 5f4d 6942 2069 6620 3332 5f62  `512_MiB if 32_b
+0000e9e0: 6974 5f62 7569 6c64 2065 6c73 6520 3130  it_build else 10
+0000e9f0: 3234 5f4d 6942 6060 2e0a 0a20 2020 202e  24_MiB``...    .
+0000ea00: 2e20 7079 3a61 7474 7269 6275 7465 3a3a  . py:attribute::
+0000ea10: 206f 7665 726c 6170 4c6f 670a 0a20 2020   overlapLog..   
+0000ea20: 2020 2020 2043 6f6e 7472 6f6c 2074 6865       Control the
+0000ea30: 206f 7665 726c 6170 2073 697a 652c 2061   overlap size, a
+0000ea40: 7320 6120 6672 6163 7469 6f6e 206f 6620  s a fraction of 
+0000ea50: 7769 6e64 6f77 2073 697a 652e 2028 5468  window size. (Th
+0000ea60: 6520 2277 696e 646f 7720 7369 7a65 2220  e "window size" 
+0000ea70: 6865 7265 2069 7320 6e6f 7420 7374 7269  here is not stri
+0000ea80: 6374 203a 7079 3a61 7474 723a 607e 4350  ct :py:attr:`~CP
+0000ea90: 6172 616d 6574 6572 2e77 696e 646f 774c  arameter.windowL
+0000eaa0: 6f67 602c 2073 6565 207a 7374 6420 736f  og`, see zstd so
+0000eab0: 7572 6365 2063 6f64 652e 290a 0a20 2020  urce code.)..   
+0000eac0: 2020 2020 2054 6869 7320 7661 6c75 6520       This value 
+0000ead0: 6973 2065 6e66 6f72 6365 6420 6f6e 6c79  is enforced only
+0000eae0: 2077 6865 6e20 3a70 793a 6174 7472 3a60   when :py:attr:`
+0000eaf0: 7e43 5061 7261 6d65 7465 722e 6e62 576f  ~CParameter.nbWo
+0000eb00: 726b 6572 7360 203e 3d20 312e 0a0a 2020  rkers` >= 1...  
+0000eb10: 2020 2020 2020 5468 6520 6f76 6572 6c61        The overla
+0000eb20: 7020 7369 7a65 2069 7320 616e 2061 6d6f  p size is an amo
+0000eb30: 756e 7420 6f66 2064 6174 6120 7265 6c6f  unt of data relo
+0000eb40: 6164 6564 2066 726f 6d20 7072 6576 696f  aded from previo
+0000eb50: 7573 206a 6f62 2061 7420 7468 6520 6265  us job at the be
+0000eb60: 6769 6e6e 696e 6720 6f66 2061 206e 6577  ginning of a new
+0000eb70: 206a 6f62 2e20 4974 2068 656c 7073 2070   job. It helps p
+0000eb80: 7265 7365 7276 6520 636f 6d70 7265 7373  reserve compress
+0000eb90: 696f 6e20 7261 7469 6f2c 2077 6869 6c65  ion ratio, while
+0000eba0: 2065 6163 6820 6a6f 6220 6973 2063 6f6d   each job is com
+0000ebb0: 7072 6573 7365 6420 696e 2070 6172 616c  pressed in paral
+0000ebc0: 6c65 6c2e 204c 6172 6765 7220 7661 6c75  lel. Larger valu
+0000ebd0: 6573 2069 6e63 7265 6173 6520 636f 6d70  es increase comp
+0000ebe0: 7265 7373 696f 6e20 7261 7469 6f2c 2062  ression ratio, b
+0000ebf0: 7574 2064 6563 7265 6173 6520 7370 6565  ut decrease spee
+0000ec00: 642e 0a0a 2020 2020 2020 2020 506f 7373  d...        Poss
+0000ec10: 6962 6c65 2076 616c 7565 7320 7261 6e67  ible values rang
+0000ec20: 6520 6672 6f6d 2030 2074 6f20 393a 0a0a  e from 0 to 9:..
+0000ec30: 2020 2020 2020 2020 2d20 3020 6d65 616e          - 0 mean
+0000ec40: 7320 2264 6566 6175 6c74 2220 3a20 5468  s "default" : Th
+0000ec50: 6520 7661 6c75 6520 7769 6c6c 2062 6520  e value will be 
+0000ec60: 6465 7465 726d 696e 6564 2062 7920 7468  determined by th
+0000ec70: 6520 6c69 6272 6172 792e 2054 6865 2076  e library. The v
+0000ec80: 616c 7565 2076 6172 6965 7320 6265 7477  alue varies betw
+0000ec90: 6565 6e20 3620 616e 6420 392c 2064 6570  een 6 and 9, dep
+0000eca0: 656e 6469 6e67 206f 6e20 3a70 793a 6174  ending on :py:at
+0000ecb0: 7472 3a60 7e43 5061 7261 6d65 7465 722e  tr:`~CParameter.
+0000ecc0: 7374 7261 7465 6779 602e 0a20 2020 2020  strategy`..     
+0000ecd0: 2020 202d 2031 206d 6561 6e73 2022 6e6f     - 1 means "no
+0000ece0: 206f 7665 726c 6170 220a 2020 2020 2020   overlap".      
+0000ecf0: 2020 2d20 3920 6d65 616e 7320 2266 756c    - 9 means "ful
+0000ed00: 6c20 6f76 6572 6c61 7022 2c20 7573 696e  l overlap", usin
+0000ed10: 6720 6120 6675 6c6c 2077 696e 646f 7720  g a full window 
+0000ed20: 7369 7a65 2e0a 0a20 2020 2020 2020 2045  size...        E
+0000ed30: 6163 6820 696e 7465 726d 6564 6961 7465  ach intermediate
+0000ed40: 2072 616e 6b20 696e 6372 6561 7365 732f   rank increases/
+0000ed50: 6465 6372 6561 7365 7320 6c6f 6164 2073  decreases load s
+0000ed60: 697a 6520 6279 2061 2066 6163 746f 7220  ize by a factor 
+0000ed70: 323a 0a0a 2020 2020 2020 2020 393a 2066  2:..        9: f
+0000ed80: 756c 6c20 7769 6e64 6f77 3b20 2038 3a20  ull window;  8: 
+0000ed90: 772f 323b 2020 373a 2077 2f34 3b20 2036  w/2;  7: w/4;  6
+0000eda0: 3a20 772f 383b 2020 353a 2077 2f31 363b  : w/8;  5: w/16;
+0000edb0: 2020 343a 2077 2f33 323b 2020 333a 2077    4: w/32;  3: w
+0000edc0: 2f36 343b 2020 323a 2077 2f31 3238 3b20  /64;  2: w/128; 
+0000edd0: 2031 3a20 6e6f 206f 7665 726c 6170 3b20   1: no overlap; 
+0000ede0: 2030 3a20 6465 6661 756c 742e 0a0a 0a2e   0: default.....
+0000edf0: 2e20 5f44 5061 7261 6d65 7465 723a 0a0a  . _DParameter:..
+0000ee00: 2e2e 2070 793a 636c 6173 733a 3a20 4450  .. py:class:: DP
+0000ee10: 6172 616d 6574 6572 2849 6e74 456e 756d  arameter(IntEnum
+0000ee20: 290a 0a20 2020 2041 6476 616e 6365 6420  )..    Advanced 
+0000ee30: 6465 636f 6d70 7265 7373 696f 6e20 7061  decompression pa
+0000ee40: 7261 6d65 7465 7273 2e0a 0a20 2020 2057  rameters...    W
+0000ee50: 6865 6e20 7573 696e 672c 2070 7574 2074  hen using, put t
+0000ee60: 6865 2070 6172 616d 6574 6572 7320 696e  he parameters in
+0000ee70: 2061 2060 6064 6963 7460 6020 6f62 6a65   a ``dict`` obje
+0000ee80: 6374 2c20 7468 6520 6b65 7920 6973 2061  ct, the key is a
+0000ee90: 203a 7079 3a63 6c61 7373 3a60 4450 6172   :py:class:`DPar
+0000eea0: 616d 6574 6572 6020 6e61 6d65 2c20 7468  ameter` name, th
+0000eeb0: 6520 7661 6c75 6520 6973 2061 2033 322d  e value is a 32-
+0000eec0: 6269 7420 7369 676e 6564 2069 6e74 6567  bit signed integ
+0000eed0: 6572 2076 616c 7565 2e0a 0a20 2020 202e  er value...    .
+0000eee0: 2e20 736f 7572 6365 636f 6465 3a3a 2070  . sourcecode:: p
+0000eef0: 7974 686f 6e0a 0a20 2020 2020 2020 2023  ython..        #
+0000ef00: 2073 6574 206d 656d 6f72 7920 616c 6c6f   set memory allo
+0000ef10: 6361 7469 6f6e 206c 696d 6974 2074 6f20  cation limit to 
+0000ef20: 3136 204d 6942 2028 3120 3c3c 2032 3429  16 MiB (1 << 24)
+0000ef30: 0a20 2020 2020 2020 206f 7074 696f 6e20  .        option 
+0000ef40: 3d20 7b44 5061 7261 6d65 7465 722e 7769  = {DParameter.wi
+0000ef50: 6e64 6f77 4c6f 674d 6178 203a 2032 347d  ndowLogMax : 24}
+0000ef60: 0a0a 2020 2020 2020 2020 2320 7573 6564  ..        # used
+0000ef70: 2077 6974 6820 6465 636f 6d70 7265 7373   with decompress
+0000ef80: 2829 2066 756e 6374 696f 6e0a 2020 2020  () function.    
+0000ef90: 2020 2020 6465 636f 6d70 7265 7373 6564      decompressed
+0000efa0: 5f64 6174 203d 2064 6563 6f6d 7072 6573  _dat = decompres
+0000efb0: 7328 6461 742c 206f 7074 696f 6e3d 6f70  s(dat, option=op
+0000efc0: 7469 6f6e 290a 0a20 2020 2020 2020 2023  tion)..        #
+0000efd0: 2075 7365 6420 7769 7468 205a 7374 6444   used with ZstdD
+0000efe0: 6563 6f6d 7072 6573 736f 7220 6f62 6a65  ecompressor obje
+0000eff0: 6374 0a20 2020 2020 2020 2064 203d 205a  ct.        d = Z
+0000f000: 7374 6444 6563 6f6d 7072 6573 736f 7228  stdDecompressor(
+0000f010: 6f70 7469 6f6e 3d6f 7074 696f 6e29 0a20  option=option). 
+0000f020: 2020 2020 2020 2064 6563 6f6d 7072 6573         decompres
+0000f030: 7365 645f 6461 7420 3d20 642e 6465 636f  sed_dat = d.deco
+0000f040: 6d70 7265 7373 2864 6174 290a 0a20 2020  mpress(dat)..   
+0000f050: 2050 6172 616d 6574 6572 2076 616c 7565   Parameter value
+0000f060: 2073 686f 756c 6420 6265 6c6f 6e67 2074   should belong t
+0000f070: 6f20 616e 2069 6e74 6572 7661 6c20 7769  o an interval wi
+0000f080: 7468 206c 6f77 6572 2061 6e64 2075 7070  th lower and upp
+0000f090: 6572 2062 6f75 6e64 732c 206f 7468 6572  er bounds, other
+0000f0a0: 7769 7365 2074 6865 7920 7769 6c6c 2065  wise they will e
+0000f0b0: 6974 6865 7220 7472 6967 6765 7220 616e  ither trigger an
+0000f0c0: 2065 7272 6f72 206f 7220 6265 2063 6c61   error or be cla
+0000f0d0: 6d70 6564 2073 696c 656e 746c 792e 0a0a  mped silently...
+0000f0e0: 2020 2020 5468 6520 636f 6e73 7461 6e74      The constant
+0000f0f0: 2076 616c 7565 7320 6d65 6e74 696f 6e65   values mentione
+0000f100: 6420 6265 6c6f 7720 6172 6520 6465 6669  d below are defi
+0000f110: 6e65 6420 696e 2060 7a73 7464 2e68 203c  ned in `zstd.h <
+0000f120: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000f130: 6f6d 2f66 6163 6562 6f6f 6b2f 7a73 7464  om/facebook/zstd
+0000f140: 2f62 6c6f 622f 7265 6c65 6173 652f 6c69  /blob/release/li
+0000f150: 622f 7a73 7464 2e68 3e60 5f2c 206e 6f74  b/zstd.h>`_, not
+0000f160: 6520 7468 6174 2074 6865 7365 2076 616c  e that these val
+0000f170: 7565 7320 6d61 7920 6265 2064 6966 6665  ues may be diffe
+0000f180: 7265 6e74 2069 6e20 6469 6666 6572 656e  rent in differen
+0000f190: 7420 7a73 7464 2076 6572 7369 6f6e 732e  t zstd versions.
+0000f1a0: 0a0a 2020 2020 2e2e 2070 793a 6d65 7468  ..    .. py:meth
+0000f1b0: 6f64 3a3a 2062 6f75 6e64 7328 7365 6c66  od:: bounds(self
+0000f1c0: 290a 0a20 2020 2020 2020 2052 6574 7572  )..        Retur
+0000f1d0: 6e20 6c6f 7765 7220 616e 6420 7570 7065  n lower and uppe
+0000f1e0: 7220 626f 756e 6473 206f 6620 6120 7061  r bounds of a pa
+0000f1f0: 7261 6d65 7465 722c 2062 6f74 6820 696e  rameter, both in
+0000f200: 636c 7573 6976 652e 0a0a 2020 2020 2020  clusive...      
+0000f210: 2020 2e2e 2073 6f75 7263 6563 6f64 653a    .. sourcecode:
+0000f220: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+0000f230: 2020 2020 2020 3e3e 3e20 4450 6172 616d        >>> DParam
+0000f240: 6574 6572 2e77 696e 646f 774c 6f67 4d61  eter.windowLogMa
+0000f250: 782e 626f 756e 6473 2829 0a20 2020 2020  x.bounds().     
+0000f260: 2020 2020 2020 2028 3130 2c20 3331 290a         (10, 31).
+0000f270: 0a20 2020 202e 2e20 7079 3a61 7474 7269  .    .. py:attri
+0000f280: 6275 7465 3a3a 2077 696e 646f 774c 6f67  bute:: windowLog
+0000f290: 4d61 780a 0a20 2020 2020 2020 2053 656c  Max..        Sel
+0000f2a0: 6563 7420 6120 7369 7a65 206c 696d 6974  ect a size limit
+0000f2b0: 2028 696e 2070 6f77 6572 206f 6620 3229   (in power of 2)
+0000f2c0: 2062 6579 6f6e 6420 7768 6963 6820 7468   beyond which th
+0000f2d0: 6520 7374 7265 616d 696e 6720 4150 4920  e streaming API 
+0000f2e0: 7769 6c6c 2072 6566 7573 6520 746f 2061  will refuse to a
+0000f2f0: 6c6c 6f63 6174 6520 6d65 6d6f 7279 2062  llocate memory b
+0000f300: 7566 6665 7220 696e 206f 7264 6572 2074  uffer in order t
+0000f310: 6f20 7072 6f74 6563 7420 7468 6520 686f  o protect the ho
+0000f320: 7374 2066 726f 6d20 756e 7265 6173 6f6e  st from unreason
+0000f330: 6162 6c65 206d 656d 6f72 7920 7265 7175  able memory requ
+0000f340: 6972 656d 656e 7473 2e0a 0a20 2020 2020  irements...     
+0000f350: 2020 2049 6620 6120 3a72 6566 3a60 6672     If a :ref:`fr
+0000f360: 616d 653c 6672 616d 655f 626c 6f63 6b3e  ame<frame_block>
+0000f370: 6020 7265 7175 6972 6573 206d 6f72 6520  ` requires more 
+0000f380: 6d65 6d6f 7279 2074 6861 6e20 7468 6520  memory than the 
+0000f390: 7365 7420 7661 6c75 652c 2072 6169 7365  set value, raise
+0000f3a0: 7320 6120 3a70 793a 636c 6173 733a 605a  s a :py:class:`Z
+0000f3b0: 7374 6445 7272 6f72 6020 6578 6365 7074  stdError` except
+0000f3c0: 696f 6e2c 2077 6974 6820 6120 6d65 7373  ion, with a mess
+0000f3d0: 6167 6520 6c69 6b65 2022 4672 616d 6520  age like "Frame 
+0000f3e0: 7265 7175 6972 6573 2074 6f6f 206d 7563  requires too muc
+0000f3f0: 6820 6d65 6d6f 7279 2066 6f72 2064 6563  h memory for dec
+0000f400: 6f64 696e 6722 2e0a 0a20 2020 2020 2020  oding"...       
+0000f410: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
+0000f420: 6973 206f 6e6c 7920 7573 6566 756c 2069  is only useful i
+0000f430: 6e20 7374 7265 616d 696e 6720 6d6f 6465  n streaming mode
+0000f440: 2c20 7369 6e63 6520 6e6f 2069 6e74 6572  , since no inter
+0000f450: 6e61 6c20 6275 6666 6572 2069 7320 616c  nal buffer is al
+0000f460: 6c6f 6361 7465 6420 696e 2073 696e 676c  located in singl
+0000f470: 652d 7061 7373 206d 6f64 652e 203a 7079  e-pass mode. :py
+0000f480: 3a66 756e 633a 6064 6563 6f6d 7072 6573  :func:`decompres
+0000f490: 7360 2066 756e 6374 696f 6e20 6d61 7920  s` function may 
+0000f4a0: 7573 6520 7374 7265 616d 696e 6720 6d6f  use streaming mo
+0000f4b0: 6465 206f 7220 7369 6e67 6c65 2d70 6173  de or single-pas
+0000f4c0: 7320 6d6f 6465 2e0a 0a20 2020 2020 2020  s mode...       
+0000f4d0: 2042 7920 6465 6661 756c 742c 2061 2064   By default, a d
+0000f4e0: 6563 6f6d 7072 6573 7369 6f6e 2063 6f6e  ecompression con
+0000f4f0: 7465 7874 2061 6363 6570 7473 2077 696e  text accepts win
+0000f500: 646f 7720 7369 7a65 7320 3c3d 2060 6028  dow sizes <= ``(
+0000f510: 3120 3c3c 205a 5354 445f 5749 4e44 4f57  1 << ZSTD_WINDOW
+0000f520: 4c4f 475f 4c49 4d49 545f 4445 4641 554c  LOG_LIMIT_DEFAUL
+0000f530: 5429 6060 2c20 7468 6520 636f 6e73 7461  T)``, the consta
+0000f540: 6e74 2069 7320 6060 3237 6060 2069 6e20  nt is ``27`` in 
+0000f550: 7a73 7464 2076 312e 322b 2c20 6d65 616e  zstd v1.2+, mean
+0000f560: 7320 3132 3820 4d69 4220 2831 203c 3c20  s 128 MiB (1 << 
+0000f570: 3237 292e 2049 6620 6672 616d 6520 7265  27). If frame re
+0000f580: 7175 6573 7465 6420 7769 6e64 6f77 2073  quested window s
+0000f590: 697a 6520 6973 2067 7265 6174 6572 2074  ize is greater t
+0000f5a0: 6861 6e20 7468 6973 2076 616c 7565 2c20  han this value, 
+0000f5b0: 6e65 6564 2074 6f20 6578 706c 6963 6974  need to explicit
+0000f5c0: 6c79 2073 6574 2074 6869 7320 7061 7261  ly set this para
+0000f5d0: 6d65 7465 722e 0a0a 2020 2020 2020 2020  meter...        
+0000f5e0: 5370 6563 6961 6c3a 2076 616c 7565 2060  Special: value `
+0000f5f0: 6030 6060 206d 6561 6e73 2022 7573 6520  `0`` means "use 
+0000f600: 6465 6661 756c 7420 6d61 7869 6d75 6d20  default maximum 
+0000f610: 7769 6e64 6f77 4c6f 6722 2e0a 0a0a 2e2e  windowLog"......
+0000f620: 2070 793a 636c 6173 733a 3a20 5374 7261   py:class:: Stra
+0000f630: 7465 6779 2849 6e74 456e 756d 290a 0a20  tegy(IntEnum).. 
+0000f640: 2020 2055 7365 6420 666f 7220 3a70 793a     Used for :py:
+0000f650: 6174 7472 3a60 4350 6172 616d 6574 6572  attr:`CParameter
+0000f660: 2e73 7472 6174 6567 7960 2e0a 0a20 2020  .strategy`...   
+0000f670: 2043 6f6d 7072 6573 7369 6f6e 2073 7472   Compression str
+0000f680: 6174 6567 6965 732c 206c 6973 7465 6420  ategies, listed 
+0000f690: 6672 6f6d 2066 6173 7465 7374 2074 6f20  from fastest to 
+0000f6a0: 7374 726f 6e67 6573 742e 0a0a 2020 2020  strongest...    
+0000f6b0: 4e6f 7465 203a 206e 6577 2073 7472 6174  Note : new strat
+0000f6c0: 6567 6965 7320 2a2a 6d69 6768 742a 2a20  egies **might** 
+0000f6d0: 6265 2061 6464 6564 2069 6e20 7468 6520  be added in the 
+0000f6e0: 6675 7475 7265 2c20 6f6e 6c79 2074 6865  future, only the
+0000f6f0: 206f 7264 6572 2028 6672 6f6d 2066 6173   order (from fas
+0000f700: 7420 746f 2073 7472 6f6e 6729 2069 7320  t to strong) is 
+0000f710: 6775 6172 616e 7465 6564 2e0a 0a20 2020  guaranteed...   
+0000f720: 202e 2e20 7079 3a61 7474 7269 6275 7465   .. py:attribute
+0000f730: 3a3a 2066 6173 740a 2020 2020 2e2e 2070  :: fast.    .. p
+0000f740: 793a 6174 7472 6962 7574 653a 3a20 6466  y:attribute:: df
+0000f750: 6173 740a 2020 2020 2e2e 2070 793a 6174  ast.    .. py:at
+0000f760: 7472 6962 7574 653a 3a20 6772 6565 6479  tribute:: greedy
+0000f770: 0a20 2020 202e 2e20 7079 3a61 7474 7269  .    .. py:attri
+0000f780: 6275 7465 3a3a 206c 617a 790a 2020 2020  bute:: lazy.    
+0000f790: 2e2e 2070 793a 6174 7472 6962 7574 653a  .. py:attribute:
+0000f7a0: 3a20 6c61 7a79 320a 2020 2020 2e2e 2070  : lazy2.    .. p
+0000f7b0: 793a 6174 7472 6962 7574 653a 3a20 6274  y:attribute:: bt
+0000f7c0: 6c61 7a79 320a 2020 2020 2e2e 2070 793a  lazy2.    .. py:
+0000f7d0: 6174 7472 6962 7574 653a 3a20 6274 6f70  attribute:: btop
+0000f7e0: 740a 2020 2020 2e2e 2070 793a 6174 7472  t.    .. py:attr
+0000f7f0: 6962 7574 653a 3a20 6274 756c 7472 610a  ibute:: btultra.
+0000f800: 2020 2020 2e2e 2070 793a 6174 7472 6962      .. py:attrib
+0000f810: 7574 653a 3a20 6274 756c 7472 6132 0a0a  ute:: btultra2..
+0000f820: 2020 2020 2e2e 2073 6f75 7263 6563 6f64      .. sourcecod
+0000f830: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+0000f840: 2020 2020 6f70 7469 6f6e 203d 207b 4350      option = {CP
+0000f850: 6172 616d 6574 6572 2e73 7472 6174 6567  arameter.strateg
+0000f860: 7920 3a20 5374 7261 7465 6779 2e6c 617a  y : Strategy.laz
+0000f870: 7932 2c0a 2020 2020 2020 2020 2020 2020  y2,.            
+0000f880: 2020 2020 2020 4350 6172 616d 6574 6572        CParameter
+0000f890: 2e63 6865 636b 7375 6d46 6c61 6720 3a20  .checksumFlag : 
+0000f8a0: 317d 0a20 2020 2020 2020 2063 6f6d 7072  1}.        compr
+0000f8b0: 6573 7365 645f 6461 7420 3d20 636f 6d70  essed_dat = comp
+0000f8c0: 7265 7373 2872 6177 5f64 6174 2c20 6f70  ress(raw_dat, op
+0000f8d0: 7469 6f6e 290a 0a0a 496e 666f 726d 6174  tion)...Informat
+0000f8e0: 6976 6520 6e6f 7465 730a 2d2d 2d2d 2d2d  ive notes.------
+0000f8f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a43 6f6d  -----------..Com
+0000f900: 7072 6573 7369 6f6e 206c 6576 656c 0a3e  pression level.>
+0000f910: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
+0000f920: 0a0a 2e2e 205f 636f 6d70 7265 7373 696f  .... _compressio
+0000f930: 6e5f 6c65 7665 6c3a 0a0a 2e2e 206e 6f74  n_level:.... not
+0000f940: 653a 3a20 436f 6d70 7265 7373 696f 6e20  e:: Compression 
+0000f950: 6c65 7665 6c0a 0a20 2020 2043 6f6d 7072  level..    Compr
+0000f960: 6573 7369 6f6e 206c 6576 656c 2069 7320  ession level is 
+0000f970: 616e 2069 6e74 6567 6572 3a0a 0a20 2020  an integer:..   
+0000f980: 202a 2060 6031 6060 2074 6f20 6060 3232   * ``1`` to ``22
+0000f990: 6060 2028 6375 7272 656e 746c 7929 2c20  `` (currently), 
+0000f9a0: 7265 6775 6c61 7220 6c65 7665 6c73 2e20  regular levels. 
+0000f9b0: 4c65 7665 6c73 203e 3d20 3230 2c20 6c61  Levels >= 20, la
+0000f9c0: 6265 6c65 6420 2a75 6c74 7261 2a2c 2073  beled *ultra*, s
+0000f9d0: 686f 756c 6420 6265 2075 7365 6420 7769  hould be used wi
+0000f9e0: 7468 2063 6175 7469 6f6e 2c20 6173 2074  th caution, as t
+0000f9f0: 6865 7920 7265 7175 6972 6520 6d6f 7265  hey require more
+0000fa00: 206d 656d 6f72 792e 0a20 2020 202a 2060   memory..    * `
+0000fa10: 6030 6060 206d 6561 6e73 2075 7365 2074  `0`` means use t
+0000fa20: 6865 2064 6566 6175 6c74 206c 6576 656c  he default level
+0000fa30: 2c20 7768 6963 6820 6973 2063 7572 7265  , which is curre
+0000fa40: 6e74 6c79 2060 6033 6060 2064 6566 696e  ntly ``3`` defin
+0000fa50: 6564 2062 7920 7468 6520 756e 6465 726c  ed by the underl
+0000fa60: 7969 6e67 207a 7374 6420 6c69 6272 6172  ying zstd librar
+0000fa70: 792e 0a20 2020 202a 2060 602d 3133 3130  y..    * ``-1310
+0000fa80: 3732 6060 2074 6f20 6060 2d31 6060 2c20  72`` to ``-1``, 
+0000fa90: 6e65 6761 7469 7665 206c 6576 656c 7320  negative levels 
+0000faa0: 6578 7465 6e64 2074 6865 2072 616e 6765  extend the range
+0000fab0: 206f 6620 7370 6565 6420 7673 2072 6174   of speed vs rat
+0000fac0: 696f 2070 7265 6665 7265 6e63 6573 2e20  io preferences. 
+0000fad0: 5468 6520 6c6f 7765 7220 7468 6520 6c65  The lower the le
+0000fae0: 7665 6c2c 2074 6865 2066 6173 7465 7220  vel, the faster 
+0000faf0: 7468 6520 7370 6565 642c 2062 7574 2061  the speed, but a
+0000fb00: 7420 7468 6520 636f 7374 206f 6620 636f  t the cost of co
+0000fb10: 6d70 7265 7373 696f 6e20 7261 7469 6f2e  mpression ratio.
+0000fb20: 2031 3331 3037 3220 3d20 3132 382a 3130   131072 = 128*10
+0000fb30: 3234 2e0a 0a20 2020 203a 7079 3a64 6174  24...    :py:dat
+0000fb40: 613a 6063 6f6d 7072 6573 7369 6f6e 4c65  a:`compressionLe
+0000fb50: 7665 6c5f 7661 6c75 6573 6020 6172 6520  vel_values` are 
+0000fb60: 736f 6d65 2076 616c 7565 7320 6465 6669  some values defi
+0000fb70: 6e65 6420 6279 2074 6865 2075 6e64 6572  ned by the under
+0000fb80: 6c79 696e 6720 7a73 7464 206c 6962 7261  lying zstd libra
+0000fb90: 7279 2e0a 0a20 2020 202a 2a46 6f72 2061  ry...    **For a
+0000fba0: 6476 616e 6365 6420 7573 6572 2a2a 0a0a  dvanced user**..
+0000fbb0: 2020 2020 436f 6d70 7265 7373 696f 6e20      Compression 
+0000fbc0: 6c65 7665 6c73 2061 7265 206a 7573 7420  levels are just 
+0000fbd0: 6e75 6d62 6572 7320 7468 6174 206d 6170  numbers that map
+0000fbe0: 2074 6f20 6120 7365 7420 6f66 2063 6f6d   to a set of com
+0000fbf0: 7072 6573 7369 6f6e 2070 6172 616d 6574  pression paramet
+0000fc00: 6572 732c 2073 6565 2060 7468 6973 2074  ers, see `this t
+0000fc10: 6162 6c65 203c 6874 7470 733a 2f2f 6769  able <https://gi
+0000fc20: 7468 7562 2e63 6f6d 2f66 6163 6562 6f6f  thub.com/faceboo
+0000fc30: 6b2f 7a73 7464 2f62 6c6f 622f 7265 6c65  k/zstd/blob/rele
+0000fc40: 6173 652f 6c69 622f 636f 6d70 7265 7373  ase/lib/compress
+0000fc50: 2f63 6c65 7665 6c73 2e68 3e60 5f20 666f  /clevels.h>`_ fo
+0000fc60: 7220 6f76 6572 7669 6577 2e20 5468 6520  r overview. The 
+0000fc70: 7061 7261 6d65 7465 7273 206d 6179 2062  parameters may b
+0000fc80: 6520 6164 6a75 7374 6564 2062 7920 7468  e adjusted by th
+0000fc90: 6520 756e 6465 726c 7969 6e67 207a 7374  e underlying zst
+0000fca0: 6420 6c69 6272 6172 7920 6166 7465 7220  d library after 
+0000fcb0: 6761 7468 6572 696e 6720 736f 6d65 2069  gathering some i
+0000fcc0: 6e66 6f72 6d61 7469 6f6e 2c20 7375 6368  nformation, such
+0000fcd0: 2061 7320 6461 7461 2073 697a 652c 2075   as data size, u
+0000fce0: 7369 6e67 2064 6963 7469 6f6e 6172 7920  sing dictionary 
+0000fcf0: 6f72 206e 6f74 2e0a 0a20 2020 2053 6574  or not...    Set
+0000fd00: 7469 6e67 2061 2063 6f6d 7072 6573 7369  ting a compressi
+0000fd10: 6f6e 206c 6576 656c 2064 6f65 7320 6e6f  on level does no
+0000fd20: 7420 7365 7420 616c 6c20 6f74 6865 7220  t set all other 
+0000fd30: 3a72 6566 3a60 636f 6d70 7265 7373 696f  :ref:`compressio
+0000fd40: 6e20 7061 7261 6d65 7465 7273 3c43 5061  n parameters<CPa
+0000fd50: 7261 6d65 7465 723e 6020 746f 2064 6566  rameter>` to def
+0000fd60: 6175 6c74 2e20 5365 7474 696e 6720 7468  ault. Setting th
+0000fd70: 6973 2077 696c 6c20 6479 6e61 6d69 6361  is will dynamica
+0000fd80: 6c6c 7920 696d 7061 6374 2074 6865 2063  lly impact the c
+0000fd90: 6f6d 7072 6573 7369 6f6e 2070 6172 616d  ompression param
+0000fda0: 6574 6572 7320 7768 6963 6820 6861 7665  eters which have
+0000fdb0: 206e 6f74 2062 6565 6e20 6d61 6e75 616c   not been manual
+0000fdc0: 6c79 2073 6574 2c20 7468 6520 6d61 6e75  ly set, the manu
+0000fdd0: 616c 6c79 2073 6574 206f 6e65 7320 7769  ally set ones wi
+0000fde0: 6c6c 2022 7374 6963 6b22 2e0a 0a0a 4672  ll "stick"....Fr
+0000fdf0: 616d 6520 616e 6420 626c 6f63 6b0a 3e3e  ame and block.>>
+0000fe00: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e0a 0a2e  >>>>>>>>>>>>>...
+0000fe10: 2e20 5f66 7261 6d65 5f62 6c6f 636b 3a0a  . _frame_block:.
+0000fe20: 0a2e 2e20 6e6f 7465 3a3a 2046 7261 6d65  ... note:: Frame
+0000fe30: 2061 6e64 2062 6c6f 636b 0a0a 2020 2020   and block..    
+0000fe40: 2a2a 4672 616d 652a 2a0a 0a20 2020 205a  **Frame**..    Z
+0000fe50: 7374 6420 6461 7461 2063 6f6e 7369 7374  std data consist
+0000fe60: 7320 6f66 206f 6e65 206f 7220 6d6f 7265  s of one or more
+0000fe70: 2069 6e64 6570 656e 6465 6e74 2022 6672   independent "fr
+0000fe80: 616d 6573 222e 2054 6865 2064 6563 6f6d  ames". The decom
+0000fe90: 7072 6573 7365 6420 636f 6e74 656e 7420  pressed content 
+0000fea0: 6f66 206d 756c 7469 706c 6520 636f 6e63  of multiple conc
+0000feb0: 6174 656e 6174 6564 2066 7261 6d65 7320  atenated frames 
+0000fec0: 6973 2074 6865 2063 6f6e 6361 7465 6e61  is the concatena
+0000fed0: 7469 6f6e 206f 6620 6561 6368 2066 7261  tion of each fra
+0000fee0: 6d65 2064 6563 6f6d 7072 6573 7365 6420  me decompressed 
+0000fef0: 636f 6e74 656e 742e 0a0a 2020 2020 4120  content...    A 
+0000ff00: 6672 616d 6520 6973 2063 6f6d 706c 6574  frame is complet
+0000ff10: 656c 7920 696e 6465 7065 6e64 656e 742c  ely independent,
+0000ff20: 2068 6173 2061 2066 7261 6d65 2068 6561   has a frame hea
+0000ff30: 6465 722c 2061 6e64 2061 2073 6574 206f  der, and a set o
+0000ff40: 6620 7061 7261 6d65 7465 7273 2077 6869  f parameters whi
+0000ff50: 6368 2074 656c 6c73 2074 6865 2064 6563  ch tells the dec
+0000ff60: 6f64 6572 2068 6f77 2074 6f20 6465 636f  oder how to deco
+0000ff70: 6d70 7265 7373 2069 742e 0a0a 2020 2020  mpress it...    
+0000ff80: 496e 2061 6464 6974 696f 6e20 746f 206e  In addition to n
+0000ff90: 6f72 6d61 6c20 6672 616d 652c 2074 6865  ormal frame, the
+0000ffa0: 7265 2069 7320 6073 6b69 7070 6162 6c65  re is `skippable
+0000ffb0: 2066 7261 6d65 203c 6874 7470 733a 2f2f   frame <https://
+0000ffc0: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
+0000ffd0: 6f6f 6b2f 7a73 7464 2f62 6c6f 622f 7265  ook/zstd/blob/re
+0000ffe0: 6c65 6173 652f 646f 632f 7a73 7464 5f63  lease/doc/zstd_c
+0000fff0: 6f6d 7072 6573 7369 6f6e 5f66 6f72 6d61  ompression_forma
+00010000: 742e 6d64 2373 6b69 7070 6162 6c65 2d66  t.md#skippable-f
+00010010: 7261 6d65 733e 605f 2074 6861 7420 6361  rames>`_ that ca
+00010020: 6e20 636f 6e74 6169 6e20 616e 7920 7573  n contain any us
+00010030: 6572 2d64 6566 696e 6564 2064 6174 612c  er-defined data,
+00010040: 2073 6b69 7070 6162 6c65 2066 7261 6d65   skippable frame
+00010050: 2077 696c 6c20 6265 2064 6563 6f6d 7072   will be decompr
+00010060: 6573 7365 6420 746f 2060 6062 2727 6060  essed to ``b''``
+00010070: 2e0a 0a20 2020 202a 2a42 6c6f 636b 2a2a  ...    **Block**
+00010080: 0a0a 2020 2020 4120 6672 616d 6520 656e  ..    A frame en
+00010090: 6361 7073 756c 6174 6573 206f 6e65 206f  capsulates one o
+000100a0: 7220 6d75 6c74 6970 6c65 2022 626c 6f63  r multiple "bloc
+000100b0: 6b73 222e 2042 6c6f 636b 2068 6173 2061  ks". Block has a
+000100c0: 2067 7561 7261 6e74 6565 6420 6d61 7869   guaranteed maxi
+000100d0: 6d75 6d20 7369 7a65 2028 3320 6279 7465  mum size (3 byte
+000100e0: 7320 626c 6f63 6b20 6865 6164 6572 202b  s block header +
+000100f0: 2031 3238 204b 6942 292c 2074 6865 2061   128 KiB), the a
+00010100: 6374 7561 6c20 6d61 7869 6d75 6d20 7369  ctual maximum si
+00010110: 7a65 2064 6570 656e 6473 206f 6e20 6672  ze depends on fr
+00010120: 616d 6520 7061 7261 6d65 7465 7273 2e0a  ame parameters..
+00010130: 0a20 2020 2055 6e6c 696b 6520 696e 6465  .    Unlike inde
+00010140: 7065 6e64 656e 7420 6672 616d 6573 2c20  pendent frames, 
+00010150: 6561 6368 2062 6c6f 636b 2064 6570 656e  each block depen
+00010160: 6473 206f 6e20 7072 6576 696f 7573 2062  ds on previous b
+00010170: 6c6f 636b 7320 666f 7220 7072 6f70 6572  locks for proper
+00010180: 2064 6563 6f64 696e 672c 2062 7574 2064   decoding, but d
+00010190: 6f65 736e 2774 206e 6565 6420 7468 6520  oesn't need the 
+000101a0: 666f 6c6c 6f77 696e 6720 626c 6f63 6b73  following blocks
+000101b0: 2c20 6120 636f 6d70 6c65 7465 2062 6c6f  , a complete blo
+000101c0: 636b 2063 616e 2062 6520 6675 6c6c 7920  ck can be fully 
+000101d0: 6465 636f 6d70 7265 7373 6564 2e20 536f  decompressed. So
+000101e0: 2066 6c75 7368 696e 6720 626c 6f63 6b20   flushing block 
+000101f0: 6d61 7920 6265 2075 7365 6420 696e 2063  may be used in c
+00010200: 6f6d 6d75 6e69 6361 7469 6f6e 2073 6365  ommunication sce
+00010210: 6e61 7269 6f73 2c20 7365 6520 3a70 793a  narios, see :py:
+00010220: 6174 7472 3a60 5a73 7464 436f 6d70 7265  attr:`ZstdCompre
+00010230: 7373 6f72 2e46 4c55 5348 5f42 4c4f 434b  ssor.FLUSH_BLOCK
+00010240: 602e 0a0a 2020 2020 2e2e 2061 7474 656e  `...    .. atten
+00010250: 7469 6f6e 3a3a 0a0a 2020 2020 2020 2020  tion::..        
+00010260: 496e 2073 6f6d 6520 606c 616e 6775 6167  In some `languag
+00010270: 6520 6269 6e64 696e 6773 203c 6874 7470  e bindings <http
+00010280: 733a 2f2f 6661 6365 626f 6f6b 2e67 6974  s://facebook.git
+00010290: 6875 622e 696f 2f7a 7374 642f 236f 7468  hub.io/zstd/#oth
+000102a0: 6572 2d6c 616e 6775 6167 6573 3e60 5f2c  er-languages>`_,
+000102b0: 2064 6563 6f6d 7072 6573 7328 2920 6675   decompress() fu
+000102c0: 6e63 7469 6f6e 2064 6f65 736e 2774 2073  nction doesn't s
+000102d0: 7570 706f 7274 206d 756c 7469 706c 6520  upport multiple 
+000102e0: 6672 616d 6573 2c20 6f72 2f61 6e64 2064  frames, or/and d
+000102f0: 6f65 736e 2774 2073 7570 706f 7274 2061  oesn't support a
+00010300: 2066 7261 6d65 2077 6974 6820 756e 6b6e   frame with unkn
+00010310: 6f77 6e20 3a72 6566 3a60 636f 6e74 656e  own :ref:`conten
+00010320: 7420 7369 7a65 3c63 6f6e 7465 6e74 5f73  t size<content_s
+00010330: 697a 653e 602c 2070 6179 2061 7474 656e  ize>`, pay atten
+00010340: 7469 6f6e 2077 6865 6e20 636f 6d70 7265  tion when compre
+00010350: 7373 696e 6720 6461 7461 2066 6f72 206f  ssing data for o
+00010360: 7468 6572 206c 616e 6775 6167 6520 6269  ther language bi
+00010370: 6e64 696e 6773 2e0a 0a0a 4d75 6c74 692d  ndings....Multi-
+00010380: 7468 7265 6164 6564 2063 6f6d 7072 6573  threaded compres
+00010390: 7369 6f6e 0a3e 3e3e 3e3e 3e3e 3e3e 3e3e  sion.>>>>>>>>>>>
+000103a0: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e0a  >>>>>>>>>>>>>>>.
+000103b0: 0a2e 2e20 5f6d 745f 636f 6d70 7265 7373  ... _mt_compress
+000103c0: 696f 6e3a 0a0a 2e2e 206e 6f74 653a 3a20  ion:.... note:: 
+000103d0: 4d75 6c74 692d 7468 7265 6164 6564 2063  Multi-threaded c
+000103e0: 6f6d 7072 6573 7369 6f6e 0a0a 2020 2020  ompression..    
+000103f0: 5a73 7464 206c 6962 7261 7279 2073 7570  Zstd library sup
+00010400: 706f 7274 7320 6d75 6c74 692d 7468 7265  ports multi-thre
+00010410: 6164 6564 2063 6f6d 7072 6573 7369 6f6e  aded compression
+00010420: 2e20 5365 7420 3a70 793a 6174 7472 3a60  . Set :py:attr:`
+00010430: 4350 6172 616d 6574 6572 2e6e 6257 6f72  CParameter.nbWor
+00010440: 6b65 7273 6020 7061 7261 6d65 7465 7220  kers` parameter 
+00010450: 3e3d 2060 6031 6060 2074 6f20 656e 6162  >= ``1`` to enab
+00010460: 6c65 206d 756c 7469 2d74 6872 6561 6465  le multi-threade
+00010470: 6420 636f 6d70 7265 7373 696f 6e2c 2060  d compression, `
+00010480: 6031 6060 206d 6561 6e73 2022 312d 7468  `1`` means "1-th
+00010490: 7265 6164 206d 756c 7469 2d74 6872 6561  read multi-threa
+000104a0: 6465 6420 6d6f 6465 222e 0a0a 2020 2020  ded mode"...    
+000104b0: 5468 6520 7468 7265 6164 7320 6172 6520  The threads are 
+000104c0: 7370 6177 6e65 6420 6279 2074 6865 2075  spawned by the u
+000104d0: 6e64 6572 6c79 696e 6720 7a73 7464 206c  nderlying zstd l
+000104e0: 6962 7261 7279 2c20 6e6f 7420 6279 2070  ibrary, not by p
+000104f0: 797a 7374 6420 6d6f 6475 6c65 2e0a 0a20  yzstd module... 
+00010500: 2020 202e 2e20 736f 7572 6365 636f 6465     .. sourcecode
+00010510: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+00010520: 2020 2023 2075 7365 2034 2074 6872 6561     # use 4 threa
+00010530: 6473 2074 6f20 636f 6d70 7265 7373 0a20  ds to compress. 
+00010540: 2020 2020 2020 206f 7074 696f 6e20 3d20         option = 
+00010550: 7b43 5061 7261 6d65 7465 722e 6e62 576f  {CParameter.nbWo
+00010560: 726b 6572 7320 3a20 347d 0a20 2020 2020  rkers : 4}.     
+00010570: 2020 2063 6f6d 7072 6573 7365 645f 6461     compressed_da
+00010580: 7420 3d20 636f 6d70 7265 7373 2872 6177  t = compress(raw
+00010590: 5f64 6174 2c20 6f70 7469 6f6e 290a 0a20  _dat, option).. 
+000105a0: 2020 2054 6865 2064 6174 6120 7769 6c6c     The data will
+000105b0: 2062 6520 7370 6c69 7420 696e 746f 2070   be split into p
+000105c0: 6f72 7469 6f6e 7320 616e 6420 636f 6d70  ortions and comp
+000105d0: 7265 7373 6564 2069 6e20 7061 7261 6c6c  ressed in parall
+000105e0: 656c 2e20 5468 6520 706f 7274 696f 6e20  el. The portion 
+000105f0: 7369 7a65 2063 616e 2062 6520 7370 6563  size can be spec
+00010600: 6966 6965 6420 6279 203a 7079 3a61 7474  ified by :py:att
+00010610: 723a 6043 5061 7261 6d65 7465 722e 6a6f  r:`CParameter.jo
+00010620: 6253 697a 6560 2070 6172 616d 6574 6572  bSize` parameter
+00010630: 2c20 7468 6520 6f76 6572 6c61 7020 7369  , the overlap si
+00010640: 7a65 2063 616e 2062 6520 7370 6563 6966  ze can be specif
+00010650: 6965 6420 6279 203a 7079 3a61 7474 723a  ied by :py:attr:
+00010660: 6043 5061 7261 6d65 7465 722e 6f76 6572  `CParameter.over
+00010670: 6c61 704c 6f67 6020 7061 7261 6d65 7465  lapLog` paramete
+00010680: 722c 2075 7375 616c 6c79 2064 6f6e 2774  r, usually don't
+00010690: 206e 6565 6420 746f 2073 6574 2074 6865   need to set the
+000106a0: 7365 2e0a 0a20 2020 2054 6865 206d 756c  se...    The mul
+000106b0: 7469 2d74 6872 6561 6465 6420 6f75 7470  ti-threaded outp
+000106c0: 7574 2077 696c 6c20 6265 2064 6966 6665  ut will be diffe
+000106d0: 7265 6e74 2074 6861 6e20 7468 6520 7369  rent than the si
+000106e0: 6e67 6c65 2d74 6872 6561 6465 6420 6f75  ngle-threaded ou
+000106f0: 7470 7574 2e20 486f 7765 7665 722c 2062  tput. However, b
+00010700: 6f74 6820 6172 6520 6465 7465 726d 696e  oth are determin
+00010710: 6973 7469 632c 2061 6e64 2074 6865 206d  istic, and the m
+00010720: 756c 7469 2d74 6872 6561 6465 6420 6f75  ulti-threaded ou
+00010730: 7470 7574 2070 726f 6475 6365 7320 7468  tput produces th
+00010740: 6520 7361 6d65 2063 6f6d 7072 6573 7365  e same compresse
+00010750: 6420 6461 7461 206e 6f20 6d61 7474 6572  d data no matter
+00010760: 2068 6f77 206d 616e 7920 7468 7265 6164   how many thread
+00010770: 7320 7573 6564 2e0a 0a20 2020 2054 6865  s used...    The
+00010780: 206d 756c 7469 2d74 6872 6561 6465 6420   multi-threaded 
+00010790: 6f75 7470 7574 2069 7320 6120 7369 6e67  output is a sing
+000107a0: 6c65 203a 7265 663a 6066 7261 6d65 3c66  le :ref:`frame<f
+000107b0: 7261 6d65 5f62 6c6f 636b 3e60 2c20 6974  rame_block>`, it
+000107c0: 2773 206c 6172 6765 7220 6120 6c69 7474  's larger a litt
+000107d0: 6c65 2e20 436f 6d70 7265 7373 696e 6720  le. Compressing 
+000107e0: 6120 3532 302e 3538 204d 6942 2064 6174  a 520.58 MiB dat
+000107f0: 612c 2073 696e 676c 652d 7468 7265 6164  a, single-thread
+00010800: 6564 206f 7574 7075 7420 6973 2032 3733  ed output is 273
+00010810: 2e35 3520 4d69 422c 206d 756c 7469 2d74  .55 MiB, multi-t
+00010820: 6872 6561 6465 6420 6f75 7470 7574 2069  hreaded output i
+00010830: 7320 3237 342e 3333 204d 6942 2e0a 0a20  s 274.33 MiB... 
+00010840: 2020 202e 2e20 6869 6e74 3a3a 0a20 2020     .. hint::.   
+00010850: 2020 2020 2055 7369 6e67 2022 4350 5520       Using "CPU 
+00010860: 7068 7973 6963 616c 2063 6f72 6573 206e  physical cores n
+00010870: 756d 6265 7222 2061 7320 7468 7265 6164  umber" as thread
+00010880: 7320 6e75 6d62 6572 206d 6179 2062 6520  s number may be 
+00010890: 7468 6520 6661 7374 6573 742c 2074 6f20  the fastest, to 
+000108a0: 6765 7420 7468 6520 6e75 6d62 6572 206e  get the number n
+000108b0: 6565 6420 746f 2069 6e73 7461 6c6c 2074  eed to install t
+000108c0: 6869 7264 2d70 6172 7479 206d 6f64 756c  hird-party modul
+000108d0: 652e 2060 6f73 2e63 7075 5f63 6f75 6e74  e. `os.cpu_count
+000108e0: 2829 203c 6874 7470 733a 2f2f 646f 6373  () <https://docs
+000108f0: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+00010900: 6272 6172 792f 6f73 2e68 746d 6c23 6f73  brary/os.html#os
+00010910: 2e63 7075 5f63 6f75 6e74 3e60 5f20 6361  .cpu_count>`_ ca
+00010920: 6e20 6f6e 6c79 2067 6574 2022 4350 5520  n only get "CPU 
+00010930: 6c6f 6769 6361 6c20 636f 7265 7320 6e75  logical cores nu
+00010940: 6d62 6572 2220 2868 7970 6572 2d74 6872  mber" (hyper-thr
+00010950: 6561 6469 6e67 2063 6170 6162 696c 6974  eading capabilit
+00010960: 7929 2e0a 0a0a 5269 6368 206d 656d 6f72  y)....Rich memor
+00010970: 7920 6d6f 6465 0a3e 3e3e 3e3e 3e3e 3e3e  y mode.>>>>>>>>>
+00010980: 3e3e 3e3e 3e3e 3e0a 0a2e 2e20 5f72 6963  >>>>>>>.... _ric
+00010990: 685f 6d65 6d3a 0a0a 2e2e 206e 6f74 653a  h_mem:.... note:
+000109a0: 3a20 5269 6368 206d 656d 6f72 7920 6d6f  : Rich memory mo
+000109b0: 6465 0a0a 2020 2020 7079 7a73 7464 206d  de..    pyzstd m
+000109c0: 6f64 756c 6520 6861 7320 6120 2272 6963  odule has a "ric
+000109d0: 6820 6d65 6d6f 7279 206d 6f64 6522 2066  h memory mode" f
+000109e0: 6f72 2063 6f6d 7072 6573 7369 6f6e 2e20  or compression. 
+000109f0: 4974 2061 6c6c 6f63 6174 6573 206d 6f72  It allocates mor
+00010a00: 6520 6d65 6d6f 7279 2066 6f72 206f 7574  e memory for out
+00010a10: 7075 7420 6275 6666 6572 2c20 616e 6420  put buffer, and 
+00010a20: 6661 7374 6572 2069 6e20 736f 6d65 2063  faster in some c
+00010a30: 6173 6573 2e20 5375 6974 6162 6c65 2066  ases. Suitable f
+00010a40: 6f72 2065 7874 7265 6d65 6c79 2066 6173  or extremely fas
+00010a50: 7420 636f 6d70 7265 7373 696f 6e20 7363  t compression sc
+00010a60: 656e 6172 696f 732e 0a0a 2020 2020 5468  enarios...    Th
+00010a70: 6572 6520 6973 2061 203a 7079 3a66 756e  ere is a :py:fun
+00010a80: 633a 6072 6963 686d 656d 5f63 6f6d 7072  c:`richmem_compr
+00010a90: 6573 7360 2066 756e 6374 696f 6e2c 2061  ess` function, a
+00010aa0: 203a 7079 3a63 6c61 7373 3a60 5269 6368   :py:class:`Rich
+00010ab0: 4d65 6d5a 7374 6443 6f6d 7072 6573 736f  MemZstdCompresso
+00010ac0: 7260 2063 6c61 7373 2e0a 0a20 2020 2043  r` class...    C
+00010ad0: 7572 7265 6e74 6c79 2069 7420 776f 6e27  urrently it won'
+00010ae0: 7420 6265 2066 6173 7465 7220 7768 656e  t be faster when
+00010af0: 2075 7369 6e67 203a 7265 663a 607a 7374   using :ref:`zst
+00010b00: 6420 6d75 6c74 692d 7468 7265 6164 6564  d multi-threaded
+00010b10: 2063 6f6d 7072 6573 7369 6f6e 203c 6d74   compression <mt
+00010b20: 5f63 6f6d 7072 6573 7369 6f6e 3e60 2c20  _compression>`, 
+00010b30: 6974 2077 696c 6c20 6973 7375 6520 6120  it will issue a 
+00010b40: 6060 5265 736f 7572 6365 5761 726e 696e  ``ResourceWarnin
+00010b50: 6773 6060 2069 6e20 7468 6973 2063 6173  gs`` in this cas
+00010b60: 652e 0a0a 2020 2020 4566 6665 6374 733a  e...    Effects:
+00010b70: 0a0a 2020 2020 2a20 5468 6520 6f75 7470  ..    * The outp
+00010b80: 7574 2062 7566 6665 7220 6973 206c 6172  ut buffer is lar
+00010b90: 6765 7220 7468 616e 2069 6e70 7574 2064  ger than input d
+00010ba0: 6174 6120 6120 6c69 7474 6c65 2e0a 2020  ata a little..  
+00010bb0: 2020 2a20 4966 2069 6e70 7574 2064 6174    * If input dat
+00010bc0: 6120 6973 206c 6172 6765 7220 7468 616e  a is larger than
+00010bd0: 207e 3331 2e38 4b42 2c20 7570 2074 6f20   ~31.8KB, up to 
+00010be0: 3232 2520 6661 7374 6572 2e20 5468 6520  22% faster. The 
+00010bf0: 6c6f 7765 7220 7468 6520 636f 6d70 7265  lower the compre
+00010c00: 7373 696f 6e20 6c65 7665 6c2c 2074 6865  ssion level, the
+00010c10: 206d 7563 6820 6661 7374 6572 2069 7420   much faster it 
+00010c20: 6973 2075 7375 616c 6c79 2e0a 0a20 2020  is usually...   
+00010c30: 2057 6865 6e20 6e6f 7420 7573 696e 6720   When not using 
+00010c40: 7468 6973 206d 6f64 652c 2074 6865 206f  this mode, the o
+00010c50: 7574 7075 7420 6275 6666 6572 2067 726f  utput buffer gro
+00010c60: 7773 2060 6772 6164 7561 6c6c 7920 3c68  ws `gradually <h
+00010c70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00010c80: 6d2f 616e 696d 616c 697a 652f 7079 7a73  m/animalize/pyzs
+00010c90: 7464 2f62 6c6f 622f 302e 3135 2e37 2f73  td/blob/0.15.7/s
+00010ca0: 7263 2f62 696e 5f65 7874 2f5f 7a73 7464  rc/bin_ext/_zstd
+00010cb0: 6d6f 6475 6c65 2e63 234c 3231 382d 4c32  module.c#L218-L2
+00010cc0: 3433 3e60 5f2c 2069 6e20 6f72 6465 7220  43>`_, in order 
+00010cd0: 6e6f 7420 746f 2061 6c6c 6f63 6174 6520  not to allocate 
+00010ce0: 746f 6f20 6d75 6368 206d 656d 6f72 792e  too much memory.
+00010cf0: 2054 6865 206e 6567 6174 6976 6520 6566   The negative ef
+00010d00: 6665 6374 2069 7320 7468 6174 2070 797a  fect is that pyz
+00010d10: 7374 6420 6d6f 6475 6c65 2075 7375 616c  std module usual
+00010d20: 6c79 206e 6565 6420 746f 2063 616c 6c20  ly need to call 
+00010d30: 7468 6520 756e 6465 726c 7969 6e67 207a  the underlying z
+00010d40: 7374 6420 6c69 6272 6172 7927 7320 636f  std library's co
+00010d50: 6d70 7265 7373 2066 756e 6374 696f 6e20  mpress function 
+00010d60: 6d75 6c74 6970 6c65 2074 696d 6573 2e0a  multiple times..
+00010d70: 0a20 2020 2057 6865 6e20 7573 696e 6720  .    When using 
+00010d80: 7468 6973 206d 6f64 652c 2074 6865 2073  this mode, the s
+00010d90: 697a 6520 6f66 206f 7574 7075 7420 6275  ize of output bu
+00010da0: 6666 6572 2069 7320 7072 6f76 6964 6564  ffer is provided
+00010db0: 2062 7920 5a53 5444 5f63 6f6d 7072 6573   by ZSTD_compres
+00010dc0: 7342 6f75 6e64 2829 2066 756e 6374 696f  sBound() functio
+00010dd0: 6e2c 2077 6869 6368 2069 7320 6c61 7267  n, which is larg
+00010de0: 6572 2074 6861 6e20 696e 7075 7420 6461  er than input da
+00010df0: 7461 2061 206c 6974 746c 6520 286d 6178  ta a little (max
+00010e00: 696d 756d 2063 6f6d 7072 6573 7365 6420  imum compressed 
+00010e10: 7369 7a65 2069 6e20 776f 7273 7420 6361  size in worst ca
+00010e20: 7365 2073 696e 676c 652d 7061 7373 2073  se single-pass s
+00010e30: 6365 6e61 7269 6f29 2e20 466f 7220 6120  cenario). For a 
+00010e40: 3130 3020 4d69 4220 696e 7075 7420 6461  100 MiB input da
+00010e50: 7461 2c20 7468 6520 616c 6c6f 6361 7465  ta, the allocate
+00010e60: 6420 6f75 7470 7574 2062 7566 6665 7220  d output buffer 
+00010e70: 6973 2028 3130 3020 4d69 4220 2b20 3430  is (100 MiB + 40
+00010e80: 3020 4b69 4229 2e20 5468 6520 756e 6465  0 KiB). The unde
+00010e90: 726c 7969 6e67 207a 7374 6420 6c69 6272  rlying zstd libr
+00010ea0: 6172 7920 6176 6f69 6473 2065 7874 7261  ary avoids extra
+00010eb0: 206d 656d 6f72 7920 636f 7079 2066 6f72   memory copy for
+00010ec0: 2074 6869 7320 6f75 7470 7574 2062 7566   this output buf
+00010ed0: 6665 7220 7369 7a65 2e0a 0a20 2020 202e  fer size...    .
+00010ee0: 2e20 736f 7572 6365 636f 6465 3a3a 2070  . sourcecode:: p
+00010ef0: 7974 686f 6e0a 0a20 2020 2020 2020 2023  ython..        #
+00010f00: 2075 7365 2072 6963 686d 656d 5f63 6f6d   use richmem_com
+00010f10: 7072 6573 7328 2920 6675 6e63 7469 6f6e  press() function
+00010f20: 0a20 2020 2020 2020 2063 6f6d 7072 6573  .        compres
+00010f30: 7365 645f 6461 7420 3d20 7269 6368 6d65  sed_dat = richme
+00010f40: 6d5f 636f 6d70 7265 7373 2872 6177 5f64  m_compress(raw_d
+00010f50: 6174 290a 0a20 2020 2020 2020 2023 2072  at)..        # r
+00010f60: 6575 7365 2052 6963 684d 656d 5a73 7464  euse RichMemZstd
+00010f70: 436f 6d70 7265 7373 6f72 206f 626a 6563  Compressor objec
+00010f80: 740a 2020 2020 2020 2020 6320 3d20 5269  t.        c = Ri
+00010f90: 6368 4d65 6d5a 7374 6443 6f6d 7072 6573  chMemZstdCompres
+00010fa0: 736f 7228 290a 2020 2020 2020 2020 6672  sor().        fr
+00010fb0: 616d 6531 203d 2063 2e63 6f6d 7072 6573  ame1 = c.compres
+00010fc0: 7328 7261 775f 6461 7431 290a 2020 2020  s(raw_dat1).    
+00010fd0: 2020 2020 6672 616d 6532 203d 2063 2e63      frame2 = c.c
+00010fe0: 6f6d 7072 6573 7328 7261 775f 6461 7432  ompress(raw_dat2
+00010ff0: 290a 0a20 2020 2043 6f6d 7072 6573 7369  )..    Compressi
+00011000: 6e67 2061 2035 3230 2e35 3820 4d69 4220  ng a 520.58 MiB 
+00011010: 6461 7461 2c20 6974 2061 6363 656c 6572  data, it acceler
+00011020: 6174 6573 2066 726f 6d20 352e 3430 2073  ates from 5.40 s
+00011030: 6563 6f6e 6473 2074 6f20 342e 3632 2073  econds to 4.62 s
+00011040: 6563 6f6e 6473 2e0a 0a0a 5573 6520 7769  econds....Use wi
+00011050: 7468 2074 6172 6669 6c65 206d 6f64 756c  th tarfile modul
+00011060: 650a 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  e.>>>>>>>>>>>>>>
+00011070: 3e3e 3e3e 3e3e 3e3e 3e0a 0a2e 2e20 5f77  >>>>>>>>>.... _w
+00011080: 6974 685f 7461 7266 696c 653a 0a0a 2e2e  ith_tarfile:....
+00011090: 206e 6f74 653a 3a20 5573 6520 7769 7468   note:: Use with
+000110a0: 2074 6172 6669 6c65 206d 6f64 756c 650a   tarfile module.
+000110b0: 0a20 2020 2050 7974 686f 6e27 7320 6074  .    Python's `t
+000110c0: 6172 6669 6c65 203c 6874 7470 733a 2f2f  arfile <https://
+000110d0: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+000110e0: 332f 6c69 6272 6172 792f 7461 7266 696c  3/library/tarfil
+000110f0: 652e 6874 6d6c 3e60 5f20 6d6f 6475 6c65  e.html>`_ module
+00011100: 2073 7570 706f 7274 7320 6172 6269 7472   supports arbitr
+00011110: 6172 7920 636f 6d70 7265 7373 696f 6e20  ary compression 
+00011120: 616c 676f 7269 7468 6d73 2062 7920 7072  algorithms by pr
+00011130: 6f76 6964 696e 6720 6120 6669 6c65 206f  oviding a file o
+00011140: 626a 6563 742e 0a0a 2020 2020 5468 6973  bject...    This
+00011150: 2063 6f64 6520 656e 6361 7073 756c 6174   code encapsulat
+00011160: 6573 2061 2060 605a 7374 6454 6172 4669  es a ``ZstdTarFi
+00011170: 6c65 6060 2063 6c61 7373 2075 7369 6e67  le`` class using
+00011180: 203a 7079 3a63 6c61 7373 3a60 5a73 7464   :py:class:`Zstd
+00011190: 4669 6c65 602c 2069 7420 6361 6e20 6265  File`, it can be
+000111a0: 2075 7365 6420 6c69 6b65 2060 7461 7266   used like `tarf
+000111b0: 696c 652e 5461 7246 696c 6520 3c68 7474  ile.TarFile <htt
+000111c0: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+000111d0: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f74  .org/3/library/t
+000111e0: 6172 6669 6c65 2e68 746d 6c23 7461 7266  arfile.html#tarf
+000111f0: 696c 652e 5461 7246 696c 653e 605f 2063  ile.TarFile>`_ c
+00011200: 6c61 7373 3a0a 0a20 2020 202e 2e20 736f  lass:..    .. so
+00011210: 7572 6365 636f 6465 3a3a 2070 7974 686f  urcecode:: pytho
+00011220: 6e0a 0a20 2020 2020 2020 2069 6d70 6f72  n..        impor
+00011230: 7420 7461 7266 696c 650a 0a20 2020 2020  t tarfile..     
+00011240: 2020 2023 2077 6865 6e20 7573 696e 6720     # when using 
+00011250: 7265 6164 206d 6f64 6520 2864 6563 6f6d  read mode (decom
+00011260: 7072 6573 7369 6f6e 292c 2074 6865 206c  pression), the l
+00011270: 6576 656c 5f6f 725f 6f70 7469 6f6e 2070  evel_or_option p
+00011280: 6172 616d 6574 6572 0a20 2020 2020 2020  arameter.       
+00011290: 2023 2063 616e 206f 6e6c 7920 6265 2061   # can only be a
+000112a0: 2064 6963 7420 6f62 6a65 6374 2c20 7468   dict object, th
+000112b0: 6174 2072 6570 7265 7365 6e74 7320 6465  at represents de
+000112c0: 636f 6d70 7265 7373 696f 6e20 6f70 7469  compression opti
+000112d0: 6f6e 2e20 4974 0a20 2020 2020 2020 2023  on. It.        #
+000112e0: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
+000112f0: 2069 6e74 2074 7970 6520 636f 6d70 7265   int type compre
+00011300: 7373 696f 6e20 6c65 7665 6c20 696e 2074  ssion level in t
+00011310: 6869 7320 6361 7365 2e0a 0a20 2020 2020  his case...     
+00011320: 2020 2063 6c61 7373 205a 7374 6454 6172     class ZstdTar
+00011330: 4669 6c65 2874 6172 6669 6c65 2e54 6172  File(tarfile.Tar
+00011340: 4669 6c65 293a 0a20 2020 2020 2020 2020  File):.         
+00011350: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00011360: 7365 6c66 2c20 6e61 6d65 2c20 6d6f 6465  self, name, mode
+00011370: 3d27 7227 2c20 2a2c 206c 6576 656c 5f6f  ='r', *, level_o
+00011380: 725f 6f70 7469 6f6e 3d4e 6f6e 652c 207a  r_option=None, z
+00011390: 7374 645f 6469 6374 3d4e 6f6e 652c 202a  std_dict=None, *
+000113a0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+000113b0: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
+000113c0: 7374 645f 6669 6c65 203d 205a 7374 6446  std_file = ZstdF
+000113d0: 696c 6528 6e61 6d65 2c20 6d6f 6465 2c0a  ile(name, mode,.
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 2020 2020 2020 2020 2020 6c65 7665 6c5f            level_
+00011410: 6f72 5f6f 7074 696f 6e3d 6c65 7665 6c5f  or_option=level_
+00011420: 6f72 5f6f 7074 696f 6e2c 0a20 2020 2020  or_option,.     
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011450: 2020 2020 207a 7374 645f 6469 6374 3d7a       zstd_dict=z
+00011460: 7374 645f 6469 6374 290a 2020 2020 2020  std_dict).      
+00011470: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+000114a0: 745f 5f28 6669 6c65 6f62 6a3d 7365 6c66  t__(fileobj=self
+000114b0: 2e7a 7374 645f 6669 6c65 2c20 6d6f 6465  .zstd_file, mode
+000114c0: 3d6d 6f64 652c 202a 2a6b 7761 7267 7329  =mode, **kwargs)
+000114d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000114e0: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+000114f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011500: 662e 7a73 7464 5f66 696c 652e 636c 6f73  f.zstd_file.clos
+00011510: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00011520: 2020 2020 2020 2020 7261 6973 650a 0a20          raise.. 
+00011530: 2020 2020 2020 2020 2020 2064 6566 2063             def c
+00011540: 6c6f 7365 2873 656c 6629 3a0a 2020 2020  lose(self):.    
+00011550: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00011560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011570: 2020 2020 2073 7570 6572 2829 2e63 6c6f       super().clo
+00011580: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
+00011590: 2020 2020 2066 696e 616c 6c79 3a0a 2020       finally:.  
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115b0: 2020 7365 6c66 2e7a 7374 645f 6669 6c65    self.zstd_file
+000115c0: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
+000115d0: 2020 2320 7772 6974 6520 2e74 6172 2e7a    # write .tar.z
+000115e0: 7374 2066 696c 6520 2863 6f6d 7072 6573  st file (compres
+000115f0: 7369 6f6e 290a 2020 2020 2020 2020 7769  sion).        wi
+00011600: 7468 205a 7374 6454 6172 4669 6c65 2827  th ZstdTarFile('
+00011610: 6172 6368 6976 652e 7461 722e 7a73 7427  archive.tar.zst'
+00011620: 2c20 6d6f 6465 3d27 7727 2c20 6c65 7665  , mode='w', leve
+00011630: 6c5f 6f72 5f6f 7074 696f 6e3d 3529 2061  l_or_option=5) a
+00011640: 7320 7461 723a 0a20 2020 2020 2020 2020  s tar:.         
+00011650: 2020 2023 2064 6f20 736f 6d65 7468 696e     # do somethin
+00011660: 670a 0a20 2020 2020 2020 2023 2072 6561  g..        # rea
+00011670: 6420 2e74 6172 2e7a 7374 2066 696c 6520  d .tar.zst file 
+00011680: 2864 6563 6f6d 7072 6573 7369 6f6e 290a  (decompression).
+00011690: 2020 2020 2020 2020 7769 7468 205a 7374          with Zst
+000116a0: 6454 6172 4669 6c65 2827 6172 6368 6976  dTarFile('archiv
+000116b0: 652e 7461 722e 7a73 7427 2c20 6d6f 6465  e.tar.zst', mode
+000116c0: 3d27 7227 2920 6173 2074 6172 3a0a 2020  ='r') as tar:.  
+000116d0: 2020 2020 2020 2020 2020 2320 646f 2073            # do s
+000116e0: 6f6d 6574 6869 6e67 0a0a 2020 2020 5768  omething..    Wh
+000116f0: 656e 2074 6865 2061 626f 7665 2063 6f64  en the above cod
+00011700: 6520 6973 2069 6e20 7265 6164 206d 6f64  e is in read mod
+00011710: 6520 2864 6563 6f6d 7072 6573 7369 6f6e  e (decompression
+00011720: 292c 2061 6e64 2073 656c 6563 7469 7665  ), and selective
+00011730: 6c79 2072 6561 6420 6669 6c65 7320 6d75  ly read files mu
+00011740: 6c74 6970 6c65 2074 696d 6573 2c20 6974  ltiple times, it
+00011750: 206d 6179 2073 6565 6b20 746f 2061 2070   may seek to a p
+00011760: 6f73 6974 696f 6e20 6265 666f 7265 2074  osition before t
+00011770: 6865 2063 7572 7265 6e74 2070 6f73 6974  he current posit
+00011780: 696f 6e2c 2074 6865 6e20 7468 6520 6465  ion, then the de
+00011790: 636f 6d70 7265 7373 696f 6e20 6861 7320  compression has 
+000117a0: 746f 2062 6520 7265 7374 6172 7465 6420  to be restarted 
+000117b0: 6672 6f6d 207a 6572 6f2e 2049 6620 7468  from zero. If th
+000117c0: 6973 2073 6c6f 7773 2064 6f77 6e20 7468  is slows down th
+000117d0: 6520 6f70 6572 6174 696f 6e73 2c20 796f  e operations, yo
+000117e0: 7520 6361 6e3a 0a0a 2020 2020 2020 2020  u can:..        
+000117f0: 232e 2055 7365 203a 7079 3a63 6c61 7373  #. Use :py:class
+00011800: 3a60 5365 656b 6162 6c65 5a73 7464 4669  :`SeekableZstdFi
+00011810: 6c65 6020 636c 6173 7320 746f 2063 7265  le` class to cre
+00011820: 6174 652f 7265 6164 202e 7461 722e 7a73  ate/read .tar.zs
+00011830: 7420 6669 6c65 2e0a 2020 2020 2020 2020  t file..        
+00011840: 232e 2044 6563 6f6d 7072 6573 7320 7468  #. Decompress th
+00011850: 6520 6172 6368 6976 6520 746f 2061 2074  e archive to a t
+00011860: 656d 706f 7261 7279 2066 696c 652c 2061  emporary file, a
+00011870: 6e64 2072 6561 6420 6672 6f6d 2069 742e  nd read from it.
+00011880: 2054 6869 7320 636f 6465 2065 6e63 6170   This code encap
+00011890: 7375 6c61 7465 7320 7468 6520 7072 6f63  sulates the proc
+000118a0: 6573 733a 0a0a 2020 2020 2e2e 2073 6f75  ess:..    .. sou
+000118b0: 7263 6563 6f64 653a 3a20 7079 7468 6f6e  rcecode:: python
+000118c0: 0a0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+000118d0: 2063 6f6e 7465 7874 6c69 620a 2020 2020   contextlib.    
+000118e0: 2020 2020 696d 706f 7274 2069 6f0a 2020      import io.  
+000118f0: 2020 2020 2020 696d 706f 7274 2074 6172        import tar
+00011900: 6669 6c65 0a20 2020 2020 2020 2069 6d70  file.        imp
+00011910: 6f72 7420 7465 6d70 6669 6c65 0a20 2020  ort tempfile.   
+00011920: 2020 2020 2066 726f 6d20 7079 7a73 7464       from pyzstd
+00011930: 2069 6d70 6f72 7420 6465 636f 6d70 7265   import decompre
+00011940: 7373 5f73 7472 6561 6d0a 0a20 2020 2020  ss_stream..     
+00011950: 2020 2040 636f 6e74 6578 746c 6962 2e63     @contextlib.c
+00011960: 6f6e 7465 7874 6d61 6e61 6765 720a 2020  ontextmanager.  
+00011970: 2020 2020 2020 6465 6620 5a73 7464 5461        def ZstdTa
+00011980: 7252 6561 6465 7228 6e61 6d65 2c20 2a2c  rReader(name, *,
+00011990: 207a 7374 645f 6469 6374 3d4e 6f6e 652c   zstd_dict=None,
+000119a0: 206f 7074 696f 6e3d 4e6f 6e65 2c20 2a2a   option=None, **
+000119b0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+000119c0: 2020 2020 2077 6974 6820 696f 2e6f 7065       with io.ope
+000119d0: 6e28 6e61 6d65 2c20 2772 6227 2920 6173  n(name, 'rb') as
+000119e0: 2069 6668 3a0a 2020 2020 2020 2020 2020   ifh:.          
+000119f0: 2020 2020 2020 7769 7468 2074 656d 7066        with tempf
+00011a00: 696c 652e 5465 6d70 6f72 6172 7946 696c  ile.TemporaryFil
+00011a10: 6528 2920 6173 2074 6d70 5f66 696c 653a  e() as tmp_file:
+00011a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011a30: 2020 2020 2064 6563 6f6d 7072 6573 735f       decompress_
+00011a40: 7374 7265 616d 2869 6668 2c20 746d 705f  stream(ifh, tmp_
+00011a50: 6669 6c65 2c0a 2020 2020 2020 2020 2020  file,.          
+00011a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a70: 2020 2020 2020 2020 2020 2020 7a73 7464              zstd
+00011a80: 5f64 6963 743d 7a73 7464 5f64 6963 742c  _dict=zstd_dict,
+00011a90: 206f 7074 696f 6e3d 6f70 7469 6f6e 290a   option=option).
+00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ab0: 2020 2020 746d 705f 6669 6c65 2e73 6565      tmp_file.see
+00011ac0: 6b28 3029 0a20 2020 2020 2020 2020 2020  k(0).           
+00011ad0: 2020 2020 2020 2020 2077 6974 6820 7461           with ta
+00011ae0: 7266 696c 652e 5461 7246 696c 6528 6669  rfile.TarFile(fi
+00011af0: 6c65 6f62 6a3d 746d 705f 6669 6c65 2c20  leobj=tmp_file, 
+00011b00: 2a2a 6b77 6172 6773 2920 6173 2074 6172  **kwargs) as tar
+00011b10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011b20: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
+00011b30: 7461 720a 0a20 2020 2020 2020 2077 6974  tar..        wit
+00011b40: 6820 5a73 7464 5461 7252 6561 6465 7228  h ZstdTarReader(
+00011b50: 2761 7263 6869 7665 2e74 6172 2e7a 7374  'archive.tar.zst
+00011b60: 2729 2061 7320 7461 723a 0a20 2020 2020  ') as tar:.     
+00011b70: 2020 2020 2020 2023 2064 6f20 736f 6d65         # do some
+00011b80: 7468 696e 670a 0a0a 5a73 7464 2064 6963  thing...Zstd dic
+00011b90: 7469 6f6e 6172 7920 4944 0a3e 3e3e 3e3e  tionary ID.>>>>>
+00011ba0: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e0a 0a2e  >>>>>>>>>>>>>...
+00011bb0: 2e20 5f64 6963 745f 6964 3a0a 0a2e 2e20  . _dict_id:.... 
+00011bc0: 6e6f 7465 3a3a 205a 7374 6420 6469 6374  note:: Zstd dict
+00011bd0: 696f 6e61 7279 2049 440a 0a20 2020 2044  ionary ID..    D
+00011be0: 6963 7469 6f6e 6172 7920 4944 2069 7320  ictionary ID is 
+00011bf0: 6120 3332 2d62 6974 2075 6e73 6967 6e65  a 32-bit unsigne
+00011c00: 6420 696e 7465 6765 7220 7661 6c75 652e  d integer value.
+00011c10: 2044 6563 6f64 6572 2075 7365 7320 6974   Decoder uses it
+00011c20: 2074 6f20 6368 6563 6b20 6966 2074 6865   to check if the
+00011c30: 2063 6f72 7265 6374 2064 6963 7469 6f6e   correct diction
+00011c40: 6172 7920 6973 2075 7365 642e 0a0a 2020  ary is used...  
+00011c50: 2020 4163 636f 7264 696e 6720 746f 207a    According to z
+00011c60: 7374 6420 6469 6374 696f 6e61 7279 2066  std dictionary f
+00011c70: 6f72 6d61 7420 6073 7065 6369 6669 6361  ormat `specifica
+00011c80: 7469 6f6e 203c 6874 7470 733a 2f2f 6769  tion <https://gi
+00011c90: 7468 7562 2e63 6f6d 2f66 6163 6562 6f6f  thub.com/faceboo
+00011ca0: 6b2f 7a73 7464 2f62 6c6f 622f 7265 6c65  k/zstd/blob/rele
+00011cb0: 6173 652f 646f 632f 7a73 7464 5f63 6f6d  ase/doc/zstd_com
+00011cc0: 7072 6573 7369 6f6e 5f66 6f72 6d61 742e  pression_format.
+00011cd0: 6d64 2364 6963 7469 6f6e 6172 792d 666f  md#dictionary-fo
+00011ce0: 726d 6174 3e60 5f2c 2069 6620 6120 6469  rmat>`_, if a di
+00011cf0: 6374 696f 6e61 7279 2069 7320 676f 696e  ctionary is goin
+00011d00: 6720 746f 2062 6520 6469 7374 7269 6275  g to be distribu
+00011d10: 7465 6420 696e 2070 7562 6c69 632c 2074  ted in public, t
+00011d20: 6865 2066 6f6c 6c6f 7769 6e67 2072 616e  he following ran
+00011d30: 6765 7320 6172 6520 7265 7365 7276 6564  ges are reserved
+00011d40: 2066 6f72 2066 7574 7572 6520 7265 6769   for future regi
+00011d50: 7374 7261 7220 616e 6420 7368 616c 6c20  strar and shall 
+00011d60: 6e6f 7420 6265 2075 7365 643a 0a0a 2020  not be used:..  
+00011d70: 2020 2020 2020 2d20 6c6f 7720 7261 6e67        - low rang
+00011d80: 653a 203c 3d20 3332 3736 370a 2020 2020  e: <= 32767.    
+00011d90: 2020 2020 2d20 6869 6768 2072 616e 6765      - high range
+00011da0: 3a20 3e3d 2032 5e33 310a 0a20 2020 204f  : >= 2^31..    O
+00011db0: 7574 7369 6465 206f 6620 7468 6573 6520  utside of these 
+00011dc0: 7261 6e67 6573 2c20 616e 7920 7661 6c75  ranges, any valu
+00011dd0: 6520 696e 2028 3332 3736 3720 3c20 7620  e in (32767 < v 
+00011de0: 3c20 325e 3331 2920 6361 6e20 6265 2075  < 2^31) can be u
+00011df0: 7365 6420 6672 6565 6c79 2c20 6576 656e  sed freely, even
+00011e00: 2069 6e20 7075 626c 6963 2065 6e76 6972   in public envir
+00011e10: 6f6e 6d65 6e74 2e0a 0a20 2020 2049 6e20  onment...    In 
+00011e20: 7a73 7464 2066 7261 6d65 2068 6561 6465  zstd frame heade
+00011e30: 722c 2074 6865 2060 4469 6374 696f 6e61  r, the `Dictiona
+00011e40: 7279 5f49 4420 3c68 7474 7073 3a2f 2f67  ry_ID <https://g
+00011e50: 6974 6875 622e 636f 6d2f 6661 6365 626f  ithub.com/facebo
+00011e60: 6f6b 2f7a 7374 642f 626c 6f62 2f72 656c  ok/zstd/blob/rel
+00011e70: 6561 7365 2f64 6f63 2f7a 7374 645f 636f  ease/doc/zstd_co
+00011e80: 6d70 7265 7373 696f 6e5f 666f 726d 6174  mpression_format
+00011e90: 2e6d 6423 6469 6374 696f 6e61 7279 5f69  .md#dictionary_i
+00011ea0: 643e 605f 2066 6965 6c64 2063 616e 2062  d>`_ field can b
+00011eb0: 6520 302f 312f 322f 3420 6279 7465 732e  e 0/1/2/4 bytes.
+00011ec0: 2049 6620 7468 6520 7661 6c75 6520 6973   If the value is
+00011ed0: 2073 6d61 6c6c 2c20 7468 6973 2063 616e   small, this can
+00011ee0: 2073 6176 6520 327e 3320 6279 7465 732e   save 2~3 bytes.
+00011ef0: 204f 7220 646f 6e27 7420 7772 6974 6520   Or don't write 
+00011f00: 7468 6520 4944 2062 7920 7365 7474 696e  the ID by settin
+00011f10: 6720 3a70 793a 6174 7472 3a60 4350 6172  g :py:attr:`CPar
+00011f20: 616d 6574 6572 2e64 6963 7449 4446 6c61  ameter.dictIDFla
+00011f30: 6760 2070 6172 616d 6574 6572 2e0a 0a20  g` parameter... 
+00011f40: 2020 2070 797a 7374 6420 6d6f 6475 6c65     pyzstd module
+00011f50: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
+00011f60: 2073 7065 6369 6679 696e 6720 4944 2077   specifying ID w
+00011f70: 6865 6e20 7472 6169 6e69 6e67 2064 6963  hen training dic
+00011f80: 7469 6f6e 6172 7920 6375 7272 656e 746c  tionary currentl
+00011f90: 792e 2049 6620 7761 6e74 2074 6f20 7370  y. If want to sp
+00011fa0: 6563 6966 7920 7468 6520 4944 2c20 6d6f  ecify the ID, mo
+00011fb0: 6469 6679 2074 6865 2064 6963 7469 6f6e  dify the diction
+00011fc0: 6172 7920 636f 6e74 656e 7420 6163 636f  ary content acco
+00011fd0: 7264 696e 6720 746f 2066 6f72 6d61 7420  rding to format 
+00011fe0: 7370 6563 6966 6963 6174 696f 6e2c 2061  specification, a
+00011ff0: 6e64 2074 616b 6520 7468 6520 636f 7272  nd take the corr
+00012000: 6573 706f 6e64 696e 6720 7269 736b 732e  esponding risks.
+00012010: 0a0a 2020 2020 2a2a 4174 7465 6e74 696f  ..    **Attentio
+00012020: 6e2a 2a0a 0a20 2020 2049 6e20 3a70 793a  n**..    In :py:
+00012030: 636c 6173 733a 605a 7374 6444 6963 7460  class:`ZstdDict`
+00012040: 2063 6c61 7373 2c20 3a70 793a 6174 7472   class, :py:attr
+00012050: 3a60 5a73 7464 4469 6374 2e64 6963 745f  :`ZstdDict.dict_
+00012060: 6964 6020 6174 7472 6962 7574 6520 3d3d  id` attribute ==
+00012070: 2030 206d 6561 6e73 2074 6865 2064 6963   0 means the dic
+00012080: 7469 6f6e 6172 7920 6973 2061 2022 7261  tionary is a "ra
+00012090: 7720 636f 6e74 656e 7422 2064 6963 7469  w content" dicti
+000120a0: 6f6e 6172 792c 2066 7265 6520 6f66 2061  onary, free of a
+000120b0: 6e79 2066 6f72 6d61 7420 7265 7374 7269  ny format restri
+000120c0: 6374 696f 6e2c 2075 7365 6420 666f 7220  ction, used for 
+000120d0: 6164 7661 6e63 6564 2075 7365 722e 204e  advanced user. N
+000120e0: 6f6e 2d7a 6572 6f20 6d65 616e 7320 6974  on-zero means it
+000120f0: 2773 2061 6e20 6f72 6469 6e61 7279 2064  's an ordinary d
+00012100: 6963 7469 6f6e 6172 792c 2077 6173 2063  ictionary, was c
+00012110: 7265 6174 6564 2062 7920 7a73 7464 2066  reated by zstd f
+00012120: 756e 6374 696f 6e73 2c20 666f 6c6c 6f77  unctions, follow
+00012130: 2074 6865 2066 6f72 6d61 7420 7370 6563   the format spec
+00012140: 6966 6963 6174 696f 6e2e 0a0a 2020 2020  ification...    
+00012150: 496e 203a 7079 3a66 756e 633a 6067 6574  In :py:func:`get
+00012160: 5f66 7261 6d65 5f69 6e66 6f60 2066 756e  _frame_info` fun
+00012170: 6374 696f 6e2c 2060 6064 6963 7469 6f6e  ction, ``diction
+00012180: 6172 795f 6964 6060 203d 3d20 3020 6d65  ary_id`` == 0 me
+00012190: 616e 7320 6469 6374 696f 6e61 7279 2049  ans dictionary I
+000121a0: 4420 7761 7320 6e6f 7420 7265 636f 7264  D was not record
+000121b0: 6564 2069 6e20 7468 6520 6672 616d 6520  ed in the frame 
+000121c0: 6865 6164 6572 2c20 7468 6520 6672 616d  header, the fram
+000121d0: 6520 6d61 7920 6f72 206d 6179 206e 6f74  e may or may not
+000121e0: 206e 6565 6420 6120 6469 6374 696f 6e61   need a dictiona
+000121f0: 7279 2074 6f20 6265 2064 6563 6f64 6564  ry to be decoded
+00012200: 2c20 616e 6420 7468 6520 4944 206f 6620  , and the ID of 
+00012210: 7375 6368 2061 2064 6963 7469 6f6e 6172  such a dictionar
+00012220: 7920 6973 206e 6f74 2073 7065 6369 6669  y is not specifi
+00012230: 6564 2e0a 0a0a 5573 6520 7a73 7464 2061  ed....Use zstd a
+00012240: 7320 6120 7061 7463 6869 6e67 2065 6e67  s a patching eng
+00012250: 696e 650a 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  ine.>>>>>>>>>>>>
+00012260: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
+00012270: 3e0a 0a2e 2e20 5f70 6174 6368 696e 675f  >.... _patching_
+00012280: 656e 6769 6e65 3a0a 0a2e 2e20 6e6f 7465  engine:.... note
+00012290: 3a3a 2055 7365 207a 7374 6420 6173 2061  :: Use zstd as a
+000122a0: 2070 6174 6368 696e 6720 656e 6769 6e65   patching engine
+000122b0: 0a0a 2020 2020 5a73 7464 2063 616e 2062  ..    Zstd can b
+000122c0: 6520 7573 6564 2061 7320 6120 6772 6561  e used as a grea
+000122d0: 7420 6070 6174 6368 696e 6720 656e 6769  t `patching engi
+000122e0: 6e65 203c 6874 7470 733a 2f2f 6769 7468  ne <https://gith
+000122f0: 7562 2e63 6f6d 2f66 6163 6562 6f6f 6b2f  ub.com/facebook/
+00012300: 7a73 7464 2f77 696b 692f 5a73 7461 6e64  zstd/wiki/Zstand
+00012310: 6172 642d 6173 2d61 2d70 6174 6368 696e  ard-as-a-patchin
+00012320: 672d 656e 6769 6e65 3e60 5f2c 2061 6c74  g-engine>`_, alt
+00012330: 686f 7567 6820 6974 2068 6173 2073 6f6d  hough it has som
+00012340: 6520 6c69 6d69 7461 7469 6f6e 732e 0a0a  e limitations...
+00012350: 2020 2020 496e 2074 6869 7320 7061 7274      In this part
+00012360: 6963 756c 6172 2073 6365 6e61 7269 6f2c  icular scenario,
+00012370: 2070 6173 7320 3a70 793a 6174 7472 3a60   pass :py:attr:`
+00012380: 5a73 7464 4469 6374 2e61 735f 7072 6566  ZstdDict.as_pref
+00012390: 6978 6020 6174 7472 6962 7574 6520 6173  ix` attribute as
+000123a0: 2060 7a73 7464 5f64 6963 7460 2061 7267   `zstd_dict` arg
+000123b0: 756d 656e 742e 2022 5072 6566 6978 2220  ument. "Prefix" 
+000123c0: 6973 2073 696d 696c 6172 2074 6f20 2272  is similar to "r
+000123d0: 6177 2063 6f6e 7465 6e74 2220 6469 6374  aw content" dict
+000123e0: 696f 6e61 7279 2c20 6275 7420 7a73 7464  ionary, but zstd
+000123f0: 2069 6e74 6572 6e61 6c6c 7920 6861 6e64   internally hand
+00012400: 6c65 7320 7468 656d 2064 6966 6665 7265  les them differe
+00012410: 6e74 6c79 2c20 7365 6520 6074 6869 7320  ntly, see `this 
+00012420: 6973 7375 6520 3c68 7474 7073 3a2f 2f67  issue <https://g
+00012430: 6974 6875 622e 636f 6d2f 6661 6365 626f  ithub.com/facebo
+00012440: 6f6b 2f7a 7374 642f 6973 7375 6573 2f32  ok/zstd/issues/2
+00012450: 3833 353e 605f 2e0a 0a20 2020 2045 7373  835>`_...    Ess
+00012460: 656e 7469 616c 6c79 2c20 7072 6566 6978  entially, prefix
+00012470: 2069 7320 6c69 6b65 2062 6569 6e67 2070   is like being p
+00012480: 6c61 6365 6420 6265 666f 7265 2074 6865  laced before the
+00012490: 2064 6174 6120 746f 2062 6520 636f 6d70   data to be comp
+000124a0: 7265 7373 6564 2e20 5365 6520 225a 5354  ressed. See "ZST
+000124b0: 445f 635f 6465 7465 726d 696e 6973 7469  D_c_deterministi
+000124c0: 6352 6566 5072 6566 6978 2220 696e 2060  cRefPrefix" in `
+000124d0: 7468 6973 2066 696c 6520 3c68 7474 7073  this file <https
+000124e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
+000124f0: 6365 626f 6f6b 2f7a 7374 642f 626c 6f62  cebook/zstd/blob
+00012500: 2f72 656c 6561 7365 2f6c 6962 2f7a 7374  /release/lib/zst
+00012510: 642e 683e 605f 2e0a 0a20 2020 2031 2c20  d.h>`_...    1, 
+00012520: 4765 6e65 7261 7469 6e67 2061 2070 6174  Generating a pat
+00012530: 6368 2028 636f 6d70 7265 7373 290a 0a20  ch (compress).. 
+00012540: 2020 2041 7373 756d 696e 6720 5645 525f     Assuming VER_
+00012550: 3120 616e 6420 5645 525f 3220 6172 6520  1 and VER_2 are 
+00012560: 7477 6f20 7665 7273 696f 6e73 2e0a 0a20  two versions... 
+00012570: 2020 204c 6574 2074 6865 2022 7769 6e64     Let the "wind
+00012580: 6f77 2220 636f 7665 7220 7468 6520 6c6f  ow" cover the lo
+00012590: 6e67 6573 7420 7665 7273 696f 6e2c 2062  ngest version, b
+000125a0: 7920 7365 7474 696e 6720 3a70 793a 6174  y setting :py:at
+000125b0: 7472 3a60 4350 6172 616d 6574 6572 2e77  tr:`CParameter.w
+000125c0: 696e 646f 774c 6f67 602e 2041 6e64 2065  indowLog`. And e
+000125d0: 6e61 626c 6520 226c 6f6e 6720 6469 7374  nable "long dist
+000125e0: 616e 6365 206d 6174 6368 696e 6722 2062  ance matching" b
+000125f0: 7920 7365 7474 696e 6720 3a70 793a 6174  y setting :py:at
+00012600: 7472 3a60 4350 6172 616d 6574 6572 2e65  tr:`CParameter.e
+00012610: 6e61 626c 654c 6f6e 6744 6973 7461 6e63  nableLongDistanc
+00012620: 654d 6174 6368 696e 6760 2074 6f20 312e  eMatching` to 1.
+00012630: 2054 6865 2060 602d 2d70 6174 6368 2d66   The ``--patch-f
+00012640: 726f 6d60 6020 6f70 7469 6f6e 206f 6620  rom`` option of 
+00012650: 7a73 7464 2043 4c49 2061 6c73 6f20 7573  zstd CLI also us
+00012660: 6573 206f 7468 6572 2070 6172 616d 6574  es other paramet
+00012670: 6572 732c 2062 7574 2074 6865 7365 2074  ers, but these t
+00012680: 776f 206d 6174 7465 7220 7468 6520 6d6f  wo matter the mo
+00012690: 7374 2e0a 0a20 2020 2054 6865 2076 616c  st...    The val
+000126a0: 6964 2076 616c 7565 206f 6620 6077 696e  id value of `win
+000126b0: 646f 774c 6f67 6020 6973 205b 3130 2c33  dowLog` is [10,3
+000126c0: 305d 2069 6e20 3332 2d62 6974 2062 7569  0] in 32-bit bui
+000126d0: 6c64 2c20 5b31 302c 3331 5d20 696e 2036  ld, [10,31] in 6
+000126e0: 342d 6269 7420 6275 696c 642e 2053 6f20  4-bit build. So 
+000126f0: 696e 2036 342d 6269 7420 6275 696c 642c  in 64-bit build,
+00012700: 2069 7420 6861 7320 6120 6032 4769 4220   it has a `2GiB 
+00012710: 6c65 6e67 7468 206c 696d 6974 203c 6874  length limit <ht
+00012720: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00012730: 2f66 6163 6562 6f6f 6b2f 7a73 7464 2f69  /facebook/zstd/i
+00012740: 7373 7565 732f 3231 3733 3e60 5f2e 2053  ssues/2173>`_. S
+00012750: 7472 6963 746c 7920 7370 6561 6b69 6e67  trictly speaking
+00012760: 2c20 7468 6520 6c69 6d69 7420 6973 2028  , the limit is (
+00012770: 3247 6942 202d 207e 3130 304b 6942 292e  2GiB - ~100KiB).
+00012780: 2057 6865 6e20 7468 6973 206c 696d 6974   When this limit
+00012790: 2069 7320 6578 6365 6564 6564 2c20 7468   is exceeded, th
+000127a0: 6520 7061 7463 6820 6265 636f 6d65 7320  e patch becomes 
+000127b0: 7665 7279 206c 6172 6765 2061 6e64 206c  very large and l
+000127c0: 6f73 6573 2074 6865 206d 6561 6e69 6e67  oses the meaning
+000127d0: 206f 6620 6120 7061 7463 682e 0a0a 2020   of a patch...  
+000127e0: 2020 2e2e 2073 6f75 7263 6563 6f64 653a    .. sourcecode:
+000127f0: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+00012800: 2020 2320 7573 6520 5645 525f 3120 6173    # use VER_1 as
+00012810: 2070 7265 6669 780a 2020 2020 2020 2020   prefix.        
+00012820: 7631 203d 205a 7374 6444 6963 7428 5645  v1 = ZstdDict(VE
+00012830: 525f 312c 2069 735f 7261 773d 5472 7565  R_1, is_raw=True
+00012840: 290a 0a20 2020 2020 2020 2023 206c 6574  )..        # let
+00012850: 2074 6865 2077 696e 646f 7720 636f 7665   the window cove
+00012860: 7220 7468 6520 6c6f 6e67 6573 7420 7665  r the longest ve
+00012870: 7273 696f 6e2e 0a20 2020 2020 2020 2023  rsion..        #
+00012880: 2064 6f6e 2774 2066 6f72 6765 7420 746f   don't forget to
+00012890: 2063 6c61 6d70 2077 696e 646f 774c 6f67   clamp windowLog
+000128a0: 2074 6f20 7661 6c69 6420 7261 6e67 652e   to valid range.
+000128b0: 0a20 2020 2020 2020 2023 2065 6e61 626c  .        # enabl
+000128c0: 6520 226c 6f6e 6720 6469 7374 616e 6365  e "long distance
+000128d0: 206d 6174 6368 696e 6722 2e0a 2020 2020   matching"..    
+000128e0: 2020 2020 7769 6e64 6f77 4c6f 6720 3d20      windowLog = 
+000128f0: 6d61 7828 6c65 6e28 5645 525f 3129 2c20  max(len(VER_1), 
+00012900: 6c65 6e28 5645 525f 3229 292e 6269 745f  len(VER_2)).bit_
+00012910: 6c65 6e67 7468 2829 0a20 2020 2020 2020  length().       
+00012920: 206f 7074 696f 6e20 3d20 7b43 5061 7261   option = {CPara
+00012930: 6d65 7465 722e 7769 6e64 6f77 4c6f 673a  meter.windowLog:
+00012940: 2077 696e 646f 774c 6f67 2c0a 2020 2020   windowLog,.    
+00012950: 2020 2020 2020 2020 2020 2020 2020 4350                CP
+00012960: 6172 616d 6574 6572 2e65 6e61 626c 654c  arameter.enableL
+00012970: 6f6e 6744 6973 7461 6e63 654d 6174 6368  ongDistanceMatch
+00012980: 696e 673a 2031 7d0a 0a20 2020 2020 2020  ing: 1}..       
+00012990: 2023 2067 6574 2061 2073 6d61 6c6c 2050   # get a small P
+000129a0: 4154 4348 0a20 2020 2020 2020 2050 4154  ATCH.        PAT
+000129b0: 4348 203d 2063 6f6d 7072 6573 7328 5645  CH = compress(VE
+000129c0: 525f 322c 206c 6576 656c 5f6f 725f 6f70  R_2, level_or_op
+000129d0: 7469 6f6e 3d6f 7074 696f 6e2c 207a 7374  tion=option, zst
+000129e0: 645f 6469 6374 3d76 312e 6173 5f70 7265  d_dict=v1.as_pre
+000129f0: 6669 7829 0a0a 2020 2020 322c 2041 7070  fix)..    2, App
+00012a00: 6c79 696e 6720 7468 6520 7061 7463 6820  lying the patch 
+00012a10: 2864 6563 6f6d 7072 6573 7329 0a0a 2020  (decompress)..  
+00012a20: 2020 5072 6566 6978 2069 7320 6e6f 7420    Prefix is not 
+00012a30: 6469 6374 696f 6e61 7279 2c20 736f 2074  dictionary, so t
+00012a40: 6865 2066 7261 6d65 2068 6561 6465 7220  he frame header 
+00012a50: 646f 6573 6e27 7420 7265 636f 7264 2061  doesn't record a
+00012a60: 203a 7265 663a 6064 6963 7469 6f6e 6172   :ref:`dictionar
+00012a70: 7920 6964 3c64 6963 745f 6964 3e60 2e20  y id<dict_id>`. 
+00012a80: 5768 656e 2064 6563 6f6d 7072 6573 7369  When decompressi
+00012a90: 6e67 2c20 6d75 7374 2075 7365 2074 6865  ng, must use the
+00012aa0: 2073 616d 6520 7072 6566 6978 2061 7320   same prefix as 
+00012ab0: 7768 656e 2063 6f6d 7072 6573 7369 6e67  when compressing
+00012ac0: 2e20 4f74 6865 7277 6973 6520 5a73 7464  . Otherwise Zstd
+00012ad0: 4572 726f 7220 6578 6365 7074 696f 6e20  Error exception 
+00012ae0: 6d61 7920 6265 2072 6169 7365 6420 7769  may be raised wi
+00012af0: 7468 2061 206d 6573 7361 6765 206c 696b  th a message lik
+00012b00: 6520 2244 6174 6120 636f 7272 7570 7469  e "Data corrupti
+00012b10: 6f6e 2064 6574 6563 7465 6422 2e0a 0a20  on detected"... 
+00012b20: 2020 2044 6563 6f6d 7072 6573 7369 6e67     Decompressing
+00012b30: 2072 6571 7569 7265 7320 6120 7769 6e64   requires a wind
+00012b40: 6f77 206f 6620 7468 6520 7361 6d65 2073  ow of the same s
+00012b50: 697a 6520 6173 2077 6865 6e20 636f 6d70  ize as when comp
+00012b60: 7265 7373 696e 672c 2074 6869 7320 6d61  ressing, this ma
+00012b70: 7920 6265 2061 2070 726f 626c 656d 2066  y be a problem f
+00012b80: 6f72 2073 6d61 6c6c 2052 414d 2064 6576  or small RAM dev
+00012b90: 6963 652e 2049 6620 7468 6520 7769 6e64  ice. If the wind
+00012ba0: 6f77 2069 7320 6c61 7267 6572 2074 6861  ow is larger tha
+00012bb0: 6e20 3132 384d 6942 2c20 6e65 6564 2074  n 128MiB, need t
+00012bc0: 6f20 6578 706c 6963 6974 6c79 2073 6574  o explicitly set
+00012bd0: 203a 7079 3a61 7474 723a 6044 5061 7261   :py:attr:`DPara
+00012be0: 6d65 7465 722e 7769 6e64 6f77 4c6f 674d  meter.windowLogM
+00012bf0: 6178 6020 746f 2061 6c6c 6f77 206c 6172  ax` to allow lar
+00012c00: 6765 7220 7769 6e64 6f77 2e0a 0a20 2020  ger window...   
+00012c10: 202e 2e20 736f 7572 6365 636f 6465 3a3a   .. sourcecode::
+00012c20: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+00012c30: 2023 2075 7365 2056 4552 5f31 2061 7320   # use VER_1 as 
+00012c40: 7072 6566 6978 0a20 2020 2020 2020 2076  prefix.        v
+00012c50: 3120 3d20 5a73 7464 4469 6374 2856 4552  1 = ZstdDict(VER
+00012c60: 5f31 2c20 6973 5f72 6177 3d54 7275 6529  _1, is_raw=True)
+00012c70: 0a0a 2020 2020 2020 2020 2320 616c 6c6f  ..        # allo
+00012c80: 7720 6c61 7267 6520 7769 6e64 6f77 2c20  w large window, 
+00012c90: 7468 6520 6163 7475 616c 2077 696e 646f  the actual windo
+00012ca0: 774c 6f67 2069 7320 6672 6f6d 2066 7261  wLog is from fra
+00012cb0: 6d65 2068 6561 6465 722e 0a20 2020 2020  me header..     
+00012cc0: 2020 206f 7074 696f 6e20 3d20 7b44 5061     option = {DPa
+00012cd0: 7261 6d65 7465 722e 7769 6e64 6f77 4c6f  rameter.windowLo
+00012ce0: 674d 6178 3a20 3331 7d0a 0a20 2020 2020  gMax: 31}..     
+00012cf0: 2020 2023 2067 6574 2056 4552 5f32 2066     # get VER_2 f
+00012d00: 726f 6d20 2856 4552 5f31 202b 2050 4154  rom (VER_1 + PAT
+00012d10: 4348 290a 2020 2020 2020 2020 5645 525f  CH).        VER_
+00012d20: 3220 3d20 6465 636f 6d70 7265 7373 2850  2 = decompress(P
+00012d30: 4154 4348 2c20 7a73 7464 5f64 6963 743d  ATCH, zstd_dict=
+00012d40: 7631 2e61 735f 7072 6566 6978 2c20 6f70  v1.as_prefix, op
+00012d50: 7469 6f6e 3d6f 7074 696f 6e29 0a0a 0a42  tion=option)...B
+00012d60: 7569 6c64 2070 797a 7374 6420 6d6f 6475  uild pyzstd modu
+00012d70: 6c65 2077 6974 6820 6f70 7469 6f6e 730a  le with options.
+00012d80: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
+00012d90: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
+00012da0: 0a0a 2e2e 205f 6275 696c 645f 7079 7a73  .... _build_pyzs
+00012db0: 7464 3a0a 0a2e 2e20 6e6f 7465 3a3a 2042  td:.... note:: B
+00012dc0: 7569 6c64 2070 797a 7374 6420 6d6f 6475  uild pyzstd modu
+00012dd0: 6c65 2077 6974 6820 6f70 7469 6f6e 730a  le with options.
+00012de0: 0a20 2020 2031 efb8 8fe2 83a3 2049 6620  .    1...... If 
+00012df0: 7072 6f76 6964 6520 6060 2d2d 6176 7832  provide ``--avx2
+00012e00: 6060 2062 7569 6c64 206f 7074 696f 6e2c  `` build option,
+00012e10: 2069 7420 7769 6c6c 2062 7569 6c64 2077   it will build w
+00012e20: 6974 6820 4156 5832 2f42 4d49 3220 696e  ith AVX2/BMI2 in
+00012e30: 7374 7275 6374 696f 6e73 2e20 496e 204d  structions. In M
+00012e40: 5356 4320 6275 696c 6420 2873 7461 7469  SVC build (stati
+00012e50: 6320 6c69 6e6b 292c 2074 6869 7320 6272  c link), this br
+00012e60: 696e 6773 2073 6f6d 6520 7065 7266 6f72  ings some perfor
+00012e70: 6d61 6e63 6520 696d 7072 6f76 656d 656e  mance improvemen
+00012e80: 7473 2e20 4743 432f 434c 414e 4720 6275  ts. GCC/CLANG bu
+00012e90: 696c 6473 2061 6c72 6561 6479 2064 796e  ilds already dyn
+00012ea0: 616d 6963 616c 6c79 2064 6973 7061 7463  amically dispatc
+00012eb0: 6820 736f 6d65 2066 756e 6374 696f 6e73  h some functions
+00012ec0: 2066 6f72 2042 4d49 3220 696e 7374 7275   for BMI2 instru
+00012ed0: 6374 696f 6e73 2c20 736f 206e 6f20 7369  ctions, so no si
+00012ee0: 676e 6966 6963 616e 7420 696d 7072 6f76  gnificant improv
+00012ef0: 656d 656e 742c 206f 7220 776f 7273 652e  ement, or worse.
+00012f00: 0a0a 2020 2020 2e2e 2073 6f75 7263 6563  ..    .. sourcec
+00012f10: 6f64 653a 3a20 7368 656c 6c0a 0a20 2020  ode:: shell..   
+00012f20: 2020 2020 2023 20f0 9f9f a020 7079 7a73       # .... pyzs
+00012f30: 7464 2030 2e31 352e 342b 2061 6e64 2070  td 0.15.4+ and p
+00012f40: 6970 2032 322e 312b 2073 7570 706f 7274  ip 22.1+ support
+00012f50: 2050 4550 2d35 3137 3a0a 2020 2020 2020   PEP-517:.      
+00012f60: 2020 2320 6275 696c 6420 616e 6420 696e    # build and in
+00012f70: 7374 616c 6c0a 2020 2020 2020 2020 7069  stall.        pi
+00012f80: 7020 696e 7374 616c 6c20 2d2d 636f 6e66  p install --conf
+00012f90: 6967 2d73 6574 7469 6e67 733d 222d 2d62  ig-settings="--b
+00012fa0: 7569 6c64 2d6f 7074 696f 6e3d 2d2d 6176  uild-option=--av
+00012fb0: 7832 2220 2d76 2070 797a 7374 642d 302e  x2" -v pyzstd-0.
+00012fc0: 3135 2e34 2e74 6172 2e67 7a0a 2020 2020  15.4.tar.gz.    
+00012fd0: 2020 2020 2320 6275 696c 6420 6120 7265      # build a re
+00012fe0: 6469 7374 7269 6275 7461 626c 6520 7768  distributable wh
+00012ff0: 6565 6c0a 2020 2020 2020 2020 7069 7020  eel.        pip 
+00013000: 7768 6565 6c20 2d2d 636f 6e66 6967 2d73  wheel --config-s
+00013010: 6574 7469 6e67 733d 222d 2d62 7569 6c64  ettings="--build
+00013020: 2d6f 7074 696f 6e3d 2d2d 6176 7832 2220  -option=--avx2" 
+00013030: 2d76 2070 797a 7374 642d 302e 3135 2e34  -v pyzstd-0.15.4
+00013040: 2e74 6172 2e67 7a0a 2020 2020 2020 2020  .tar.gz.        
+00013050: 2320 f09f 9fa0 206c 6567 6163 7920 636f  # .... legacy co
+00013060: 6d6d 616e 6473 3a0a 2020 2020 2020 2020  mmands:.        
+00013070: 2320 6275 696c 6420 616e 6420 696e 7374  # build and inst
+00013080: 616c 6c0a 2020 2020 2020 2020 7079 7468  all.        pyth
+00013090: 6f6e 2073 6574 7570 2e70 7920 696e 7374  on setup.py inst
+000130a0: 616c 6c20 2d2d 6176 7832 0a20 2020 2020  all --avx2.     
+000130b0: 2020 2023 2062 7569 6c64 2061 2072 6564     # build a red
+000130c0: 6973 7472 6962 7574 6162 6c65 2077 6865  istributable whe
+000130d0: 656c 0a20 2020 2020 2020 2070 7974 686f  el.        pytho
+000130e0: 6e20 7365 7475 702e 7079 2062 6469 7374  n setup.py bdist
+000130f0: 5f77 6865 656c 202d 2d61 7678 320a 0a20  _wheel --avx2.. 
+00013100: 2020 2032 efb8 8fe2 83a3 2050 797a 7374     2...... Pyzst
+00013110: 6420 6d6f 6475 6c65 2073 7570 706f 7274  d module support
+00013120: 733a 0a0a 2020 2020 2020 2020 2a20 4479  s:..        * Dy
+00013130: 6e61 6d69 6361 6c6c 7920 6c69 6e6b 2074  namically link t
+00013140: 6f20 7a73 7464 206c 6962 7261 7279 2028  o zstd library (
+00013150: 7072 6f76 6964 6564 2062 7920 7379 7374  provided by syst
+00013160: 656d 206f 7220 6120 444c 4c20 6c69 6272  em or a DLL libr
+00013170: 6172 7929 2c20 7468 656e 2074 6865 207a  ary), then the z
+00013180: 7374 6420 736f 7572 6365 2063 6f64 6520  std source code 
+00013190: 696e 2060 607a 7374 6460 6020 666f 6c64  in ``zstd`` fold
+000131a0: 6572 2077 696c 6c20 6265 2069 676e 6f72  er will be ignor
+000131b0: 6564 2e0a 2020 2020 2020 2020 2a20 5072  ed..        * Pr
+000131c0: 6f76 6964 6520 6120 6043 4646 4920 3c68  ovide a `CFFI <h
+000131d0: 7474 7073 3a2f 2f64 6f63 2e70 7970 792e  ttps://doc.pypy.
+000131e0: 6f72 672f 656e 2f6c 6174 6573 742f 6578  org/en/latest/ex
+000131f0: 7465 6e64 696e 672e 6874 6d6c 2363 6666  tending.html#cff
+00013200: 693e 605f 2069 6d70 6c65 6d65 6e74 6174  i>`_ implementat
+00013210: 696f 6e20 7468 6174 2063 616e 2077 6f72  ion that can wor
+00013220: 6b20 7769 7468 2050 7950 792e 0a0a 2020  k with PyPy...  
+00013230: 2020 4f6e 2043 5079 7468 6f6e 2c20 7072    On CPython, pr
+00013240: 6f76 6964 6520 7468 6573 6520 6275 696c  ovide these buil
+00013250: 6420 6f70 7469 6f6e 733a 0a0a 2020 2020  d options:..    
+00013260: 2020 2020 232e 206e 6f20 6f70 7469 6f6e      #. no option
+00013270: 3a20 4320 696d 706c 656d 656e 7461 7469  : C implementati
+00013280: 6f6e 2c20 7374 6174 6963 616c 6c79 206c  on, statically l
+00013290: 696e 6b20 746f 207a 7374 6420 6c69 6272  ink to zstd libr
+000132a0: 6172 792e 0a20 2020 2020 2020 2023 2e20  ary..        #. 
+000132b0: 6060 2d2d 6479 6e61 6d69 632d 6c69 6e6b  ``--dynamic-link
+000132c0: 2d7a 7374 6460 603a 2043 2069 6d70 6c65  -zstd``: C imple
+000132d0: 6d65 6e74 6174 696f 6e2c 2064 796e 616d  mentation, dynam
+000132e0: 6963 616c 6c79 206c 696e 6b20 746f 207a  ically link to z
+000132f0: 7374 6420 6c69 6272 6172 792e 0a20 2020  std library..   
+00013300: 2020 2020 2023 2e20 6060 2d2d 6366 6669       #. ``--cffi
+00013310: 6060 3a20 4346 4649 2069 6d70 6c65 6d65  ``: CFFI impleme
+00013320: 6e74 6174 696f 6e20 2873 6c6f 7765 7229  ntation (slower)
+00013330: 2c20 7374 6174 6963 616c 6c79 206c 696e  , statically lin
+00013340: 6b20 746f 207a 7374 6420 6c69 6272 6172  k to zstd librar
+00013350: 792e 0a20 2020 2020 2020 2023 2e20 6060  y..        #. ``
+00013360: 2d2d 6366 6669 202d 2d64 796e 616d 6963  --cffi --dynamic
+00013370: 2d6c 696e 6b2d 7a73 7464 6060 3a20 4346  -link-zstd``: CF
+00013380: 4649 2069 6d70 6c65 6d65 6e74 6174 696f  FI implementatio
+00013390: 6e20 2873 6c6f 7765 7229 2c20 6479 6e61  n (slower), dyna
+000133a0: 6d69 6361 6c6c 7920 6c69 6e6b 2074 6f20  mically link to 
+000133b0: 7a73 7464 206c 6962 7261 7279 2e0a 0a20  zstd library... 
+000133c0: 2020 204f 6e20 5079 5079 2c20 6f6e 6c79     On PyPy, only
+000133d0: 2043 4646 4920 696d 706c 656d 656e 7461   CFFI implementa
+000133e0: 7469 6f6e 2063 616e 2062 6520 7573 6564  tion can be used
+000133f0: 2c20 736f 2060 602d 2d63 6666 6960 6020  , so ``--cffi`` 
+00013400: 6973 2061 6464 6564 2069 6d70 6c69 6369  is added implici
+00013410: 746c 792e 2060 602d 2d64 796e 616d 6963  tly. ``--dynamic
+00013420: 2d6c 696e 6b2d 7a73 7464 6060 2069 7320  -link-zstd`` is 
+00013430: 6f70 7469 6f6e 616c 2e0a 0a20 2020 202e  optional...    .
+00013440: 2e20 736f 7572 6365 636f 6465 3a3a 2073  . sourcecode:: s
+00013450: 6865 6c6c 0a0a 2020 2020 2020 2020 2320  hell..        # 
+00013460: f09f 9fa0 2070 797a 7374 6420 302e 3135  .... pyzstd 0.15
+00013470: 2e34 2b20 616e 6420 7069 7020 3232 2e31  .4+ and pip 22.1
+00013480: 2b20 7375 7070 6f72 7420 5045 502d 3531  + support PEP-51
+00013490: 373a 0a20 2020 2020 2020 2023 2062 7569  7:.        # bui
+000134a0: 6c64 2061 6e64 2069 6e73 7461 6c6c 0a20  ld and install. 
+000134b0: 2020 2020 2020 2070 6970 3320 696e 7374         pip3 inst
+000134c0: 616c 6c20 2d2d 636f 6e66 6967 2d73 6574  all --config-set
+000134d0: 7469 6e67 733d 222d 2d62 7569 6c64 2d6f  tings="--build-o
+000134e0: 7074 696f 6e3d 2d2d 6479 6e61 6d69 632d  ption=--dynamic-
+000134f0: 6c69 6e6b 2d7a 7374 6422 202d 7620 7079  link-zstd" -v py
+00013500: 7a73 7464 2d30 2e31 352e 342e 7461 722e  zstd-0.15.4.tar.
+00013510: 677a 0a20 2020 2020 2020 2023 2062 7569  gz.        # bui
+00013520: 6c64 2061 2072 6564 6973 7472 6962 7574  ld a redistribut
+00013530: 6162 6c65 2077 6865 656c 0a20 2020 2020  able wheel.     
+00013540: 2020 2070 6970 3320 7768 6565 6c20 2d2d     pip3 wheel --
+00013550: 636f 6e66 6967 2d73 6574 7469 6e67 733d  config-settings=
+00013560: 222d 2d62 7569 6c64 2d6f 7074 696f 6e3d  "--build-option=
+00013570: 2d2d 6479 6e61 6d69 632d 6c69 6e6b 2d7a  --dynamic-link-z
+00013580: 7374 6422 202d 7620 7079 7a73 7464 2d30  std" -v pyzstd-0
+00013590: 2e31 352e 342e 7461 722e 677a 0a20 2020  .15.4.tar.gz.   
+000135a0: 2020 2020 2023 2073 7065 6369 6679 206d       # specify m
+000135b0: 6f72 6520 7468 616e 206f 6e65 206f 7074  ore than one opt
+000135c0: 696f 6e0a 2020 2020 2020 2020 7069 7033  ion.        pip3
+000135d0: 2077 6865 656c 202d 2d63 6f6e 6669 672d   wheel --config-
+000135e0: 7365 7474 696e 6773 3d22 2d2d 6275 696c  settings="--buil
+000135f0: 642d 6f70 7469 6f6e 3d2d 2d64 796e 616d  d-option=--dynam
+00013600: 6963 2d6c 696e 6b2d 7a73 7464 202d 2d63  ic-link-zstd --c
+00013610: 6666 6922 202d 7620 7079 7a73 7464 2d30  ffi" -v pyzstd-0
+00013620: 2e31 352e 342e 7461 722e 677a 0a20 2020  .15.4.tar.gz.   
+00013630: 2020 2020 2023 20f0 9f9f a020 6c65 6761       # .... lega
+00013640: 6379 2063 6f6d 6d61 6e64 733a 0a20 2020  cy commands:.   
+00013650: 2020 2020 2023 2062 7569 6c64 2061 6e64       # build and
+00013660: 2069 6e73 7461 6c6c 0a20 2020 2020 2020   install.       
+00013670: 2070 7974 686f 6e33 2073 6574 7570 2e70   python3 setup.p
+00013680: 7920 696e 7374 616c 6c20 2d2d 6479 6e61  y install --dyna
+00013690: 6d69 632d 6c69 6e6b 2d7a 7374 640a 2020  mic-link-zstd.  
+000136a0: 2020 2020 2020 2320 6275 696c 6420 6120        # build a 
+000136b0: 7265 6469 7374 7269 6275 7461 626c 6520  redistributable 
+000136c0: 7768 6565 6c0a 2020 2020 2020 2020 7079  wheel.        py
+000136d0: 7468 6f6e 3320 7365 7475 702e 7079 2062  thon3 setup.py b
+000136e0: 6469 7374 5f77 6865 656c 202d 2d64 796e  dist_wheel --dyn
+000136f0: 616d 6963 2d6c 696e 6b2d 7a73 7464 0a0a  amic-link-zstd..
+00013700: 2020 2020 536f 6d65 206e 6f74 6573 3a0a      Some notes:.
+00013710: 0a20 2020 2020 2020 202a 2054 6865 2077  .        * The w
+00013720: 6865 656c 7320 6f6e 2060 5079 5049 203c  heels on `PyPI <
+00013730: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00013740: 2f70 726f 6a65 6374 2f70 797a 7374 643e  /project/pyzstd>
+00013750: 605f 2075 7365 2073 7461 7469 6320 6c69  `_ use static li
+00013760: 6e6b 696e 672c 2074 6865 2070 6163 6b61  nking, the packa
+00013770: 6765 7320 6f6e 2060 416e 6163 6f6e 6461  ges on `Anaconda
+00013780: 203c 6874 7470 733a 2f2f 616e 6163 6f6e   <https://anacon
+00013790: 6461 2e6f 7267 2f63 6f6e 6461 2d66 6f72  da.org/conda-for
+000137a0: 6765 2f70 797a 7374 643e 605f 2075 7365  ge/pyzstd>`_ use
+000137b0: 2064 796e 616d 6963 206c 696e 6b69 6e67   dynamic linking
+000137c0: 2e0a 2020 2020 2020 2020 2a20 4e6f 206d  ..        * No m
+000137d0: 6174 7465 7220 7374 6174 6963 206f 7220  atter static or 
+000137e0: 6479 6e61 6d69 6320 6c69 6e6b 696e 672c  dynamic linking,
+000137f0: 2070 797a 7374 6420 6d6f 6475 6c65 2072   pyzstd module r
+00013800: 6571 7569 7265 7320 7a73 7464 2076 312e  equires zstd v1.
+00013810: 342e 302b 2e0a 2020 2020 2020 2020 2a20  4.0+..        * 
+00013820: 5374 6174 6963 206c 696e 6b69 6e67 3a20  Static linking: 
+00013830: 5573 6520 7a73 7464 2773 206f 6666 6963  Use zstd's offic
+00013840: 6961 6c20 7265 6c65 6173 6520 7769 7468  ial release with
+00013850: 6f75 7420 616e 7920 6368 616e 6765 2e20  out any change. 
+00013860: 4966 2077 616e 7420 746f 2075 7067 7261  If want to upgra
+00013870: 6465 206f 7220 646f 776e 6772 6164 6520  de or downgrade 
+00013880: 7468 6520 7a73 7464 206c 6962 7261 7279  the zstd library
+00013890: 2c20 6a75 7374 2072 6570 6c61 6365 2060  , just replace `
+000138a0: 607a 7374 6460 6020 666f 6c64 6572 2e0a  `zstd`` folder..
+000138b0: 2020 2020 2020 2020 2a20 4479 6e61 6d69          * Dynami
+000138c0: 6320 6c69 6e6b 696e 673a 2049 6620 6e65  c linking: If ne
+000138d0: 7720 7a73 7464 2041 5049 2069 7320 7573  w zstd API is us
+000138e0: 6564 2061 7420 636f 6d70 696c 652d 7469  ed at compile-ti
+000138f0: 6d65 2c20 6c69 6e6b 696e 6720 746f 206c  me, linking to l
+00013900: 6f77 6572 2076 6572 7369 6f6e 2072 756e  ower version run
+00013910: 2d74 696d 6520 7a73 7464 206c 6962 7261  -time zstd libra
+00013920: 7279 2077 696c 6c20 6661 696c 2e20 5573  ry will fail. Us
+00013930: 6520 7631 2e35 2e30 206e 6577 2041 5049  e v1.5.0 new API
+00013940: 2069 6620 706f 7373 6962 6c65 2e0a 0a20   if possible... 
+00013950: 2020 204f 6e20 5769 6e64 6f77 732c 2074     On Windows, t
+00013960: 6865 7265 2069 7320 6e6f 2073 7973 7465  here is no syste
+00013970: 6d2d 7769 6465 207a 7374 6420 6c69 6272  m-wide zstd libr
+00013980: 6172 792e 2050 797a 7374 6420 6d6f 6475  ary. Pyzstd modu
+00013990: 6c65 2063 616e 2064 796e 616d 6963 616c  le can dynamical
+000139a0: 6c79 206c 696e 6b20 746f 2061 2044 4c4c  ly link to a DLL
+000139b0: 206c 6962 7261 7279 2c20 6d6f 6469 6679   library, modify
+000139c0: 2060 6073 6574 7570 2e70 7960 603a 0a0a   ``setup.py``:..
+000139d0: 2020 2020 2e2e 2073 6f75 7263 6563 6f64      .. sourcecod
+000139e0: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+000139f0: 2020 2020 2320 453a 5c7a 7374 645f 646c      # E:\zstd_dl
+00013a00: 6c20 666f 6c64 6572 2068 6173 207a 7374  l folder has zst
+00013a10: 642e 6820 2f20 7a64 6963 742e 6820 2f20  d.h / zdict.h / 
+00013a20: 6c69 627a 7374 642e 6c69 6220 7468 6174  libzstd.lib that
+00013a30: 0a20 2020 2020 2020 2023 2061 6c6f 6e67  .        # along
+00013a40: 2077 6974 6820 6c69 627a 7374 642e 646c   with libzstd.dl
+00013a50: 6c0a 2020 2020 2020 2020 6966 2044 594e  l.        if DYN
+00013a60: 414d 4943 5f4c 494e 4b3a 0a20 2020 2020  AMIC_LINK:.     
+00013a70: 2020 2020 2020 206b 7761 7267 7320 3d20         kwargs = 
+00013a80: 7b0a 2020 2020 2020 2020 2020 2020 2769  {.            'i
+00013a90: 6e63 6c75 6465 5f64 6972 7327 3a20 5b27  nclude_dirs': ['
+00013aa0: 453a 5c7a 7374 645f 646c 6c27 5d2c 2023  E:\zstd_dll'], #
+00013ab0: 202e 6820 6469 7265 6374 6f72 790a 2020   .h directory.  
+00013ac0: 2020 2020 2020 2020 2020 276c 6962 7261            'libra
+00013ad0: 7279 5f64 6972 7327 3a20 5b27 453a 5c7a  ry_dirs': ['E:\z
+00013ae0: 7374 645f 646c 6c27 5d2c 2023 202e 6c69  std_dll'], # .li
+00013af0: 6220 6469 7265 6374 6f72 790a 2020 2020  b directory.    
+00013b00: 2020 2020 2020 2020 276c 6962 7261 7269          'librari
+00013b10: 6573 273a 205b 276c 6962 7a73 7464 275d  es': ['libzstd']
+00013b20: 2c20 2020 2020 2020 2023 206c 6962 206e  ,        # lib n
+00013b30: 616d 652c 206e 6f74 2066 696c 656e 616d  ame, not filenam
+00013b40: 652c 2066 6f72 2074 6865 206c 696e 6b65  e, for the linke
+00013b50: 722e 0a20 2020 2020 2020 2020 2020 202e  r..            .
+00013b60: 2e2e 0a0a 2020 2020 416e 6420 7075 7420  ....    And put 
+00013b70: 6060 6c69 627a 7374 642e 646c 6c60 6020  ``libzstd.dll`` 
+00013b80: 696e 746f 206f 6e65 206f 6620 7468 6573  into one of thes
+00013b90: 6520 6469 7265 6374 6f72 6965 733a 0a0a  e directories:..
+00013ba0: 2020 2020 2020 2020 2a20 4469 7265 6374          * Direct
+00013bb0: 6f72 7920 6164 6465 6420 6279 2060 6f73  ory added by `os
+00013bc0: 2e61 6464 5f64 6c6c 5f64 6972 6563 746f  .add_dll_directo
+00013bd0: 7279 2829 203c 6874 7470 733a 2f2f 646f  ry() <https://do
+00013be0: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+00013bf0: 6c69 6272 6172 792f 6f73 2e68 746d 6c23  library/os.html#
+00013c00: 6f73 2e61 6464 5f64 6c6c 5f64 6972 6563  os.add_dll_direc
+00013c10: 746f 7279 3e60 5f20 6675 6e63 7469 6f6e  tory>`_ function
+00013c20: 2e20 2854 6865 2075 6e69 742d 7465 7374  . (The unit-test
+00013c30: 7320 616e 6420 7468 6520 434c 4920 6361  s and the CLI ca
+00013c40: 6e27 7420 7574 696c 697a 6520 7468 6973  n't utilize this
+00013c50: 290a 2020 2020 2020 2020 2a20 5079 7468  ).        * Pyth
+00013c60: 6f6e 2773 2072 6f6f 7420 6469 7265 6374  on's root direct
+00013c70: 6f72 7920 7468 6174 2068 6173 2070 7974  ory that has pyt
+00013c80: 686f 6e2e 6578 652e 0a20 2020 2020 2020  hon.exe..       
+00013c90: 202a 2025 5379 7374 656d 526f 6f74 255c   * %SystemRoot%\
+00013ca0: 5379 7374 656d 3332 0a0a 2020 2020 4e6f  System32..    No
+00013cb0: 7465 2074 6861 7420 7468 6520 6162 6f76  te that the abov
+00013cc0: 6520 6c69 7374 2064 6f65 736e 2774 2069  e list doesn't i
+00013cd0: 6e63 6c75 6465 2074 6865 2063 7572 7265  nclude the curre
+00013ce0: 6e74 2077 6f72 6b69 6e67 2064 6972 6563  nt working direc
+00013cf0: 746f 7279 2061 6e64 2025 5041 5448 2520  tory and %PATH% 
+00013d00: 6469 7265 6374 6f72 6965 732e 0a0a 2020  directories...  
+00013d10: 2020 33ef b88f e283 a320 5573 6520 226d    3...... Use "m
+00013d20: 756c 7469 2d70 6861 7365 2069 6e69 7469  ulti-phase initi
+00013d30: 616c 697a 6174 696f 6e22 206f 6e20 4350  alization" on CP
+00013d40: 7974 686f 6e2e 0a0a 2020 2020 4966 2070  ython...    If p
+00013d50: 726f 7669 6465 2060 602d 2d6d 756c 7469  rovide ``--multi
+00013d60: 2d70 6861 7365 2d69 6e69 7460 6020 6275  -phase-init`` bu
+00013d70: 696c 6420 6f70 7469 6f6e 2c20 6974 2077  ild option, it w
+00013d80: 696c 6c20 6275 696c 6420 7769 7468 2022  ill build with "
+00013d90: 6d75 6c74 692d 7068 6173 6520 696e 6974  multi-phase init
+00013da0: 6961 6c69 7a61 7469 6f6e 2220 2860 5045  ialization" (`PE
+00013db0: 502d 3438 3920 3c68 7474 7073 3a2f 2f70  P-489 <https://p
+00013dc0: 6570 732e 7079 7468 6f6e 2e6f 7267 2f70  eps.python.org/p
+00013dd0: 6570 2d30 3438 392f 3e60 5f29 206f 6e20  ep-0489/>`_) on 
+00013de0: 4350 7974 686f 6e20 332e 3131 2b2e 0a0a  CPython 3.11+...
+00013df0: 2020 2020 5369 6e63 6520 6974 2061 6464      Since it add
+00013e00: 7320 6120 7469 6e79 206f 7665 7268 6561  s a tiny overhea
+00013e10: 642c 2069 7427 7320 6469 7361 626c 6564  d, it's disabled
+00013e20: 2062 7920 6465 6661 756c 742e 2049 7420   by default. It 
+00013e30: 6361 6e20 6265 2065 6e61 626c 6564 2061  can be enabled a
+00013e40: 6674 6572 2043 5079 7468 6f6e 2773 2060  fter CPython's `
+00013e50: 7375 622d 696e 7465 7270 7265 7465 7273  sub-interpreters
+00013e60: 203c 6874 7470 733a 2f2f 7065 7073 2e70   <https://peps.p
+00013e70: 7974 686f 6e2e 6f72 672f 7065 702d 3035  ython.org/pep-05
+00013e80: 3534 2f3e 605f 2069 7320 6d61 7475 7265  54/>`_ is mature
+00013e90: 2e0a                                     ..
```

### Comparing `pyzstd-0.15.7/pyzstd.egg-info/PKG-INFO` & `pyzstd-0.15.8/pyzstd.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyzstd
-Version: 0.15.7
+Version: 0.15.8
 Summary: Python bindings to Zstandard (zstd) compression library, the API style is similar to Python's bz2/lzma/zlib modules.
 Home-page: https://github.com/animalize/pyzstd
 Author: Ma Lin
 Author-email: malincns@163.com
 License: The 3-Clause BSD License
-Keywords: zstandard zstd compression decompression compress decompress
+Keywords: zstandard zstd zst tar file seekable format
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Archiving :: Compression
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3.5
@@ -30,27 +30,38 @@
 Pyzstd module provides classes and functions for compressing and decompressing data, using Facebook's `Zstandard <http://www.zstd.net>`_ (or zstd as short name) algorithm.
 
 The API style is similar to Python's bz2/lzma/zlib modules.
 
 * Includes zstd v1.5.5 source code
 * Can also dynamically link to zstd library provided by system, see `this note <https://pyzstd.readthedocs.io/en/latest/#build-pyzstd>`_.
 * Has a CFFI implementation that can work with PyPy
+* ``ZstdFile`` class has C language level performance
+* Supports `Zstandard Seekable Format <https://github.com/facebook/zstd/blob/dev/contrib/seekable_format/zstd_seekable_compression_format.md>`__
 * Has a command line interface: ``python -m pyzstd --help``
 
-
 Links
 -----------
 
 Documentation: https://pyzstd.readthedocs.io/en/latest
 
 GitHub: https://github.com/animalize/pyzstd
 
 
 Release note
 ------------
+**0.15.8  (Jun 13, 2023)**
+
+#. Add `SeekableZstdFile <https://pyzstd.readthedocs.io/en/latest/#SeekableZstdFile>`_ class, it's a subclass of ``ZstdFile``, supports `Zstandard Seekable Format <https://github.com/facebook/zstd/blob/dev/contrib/seekable_format/zstd_seekable_compression_format.md>`__.
+
+#. Add *mode* argument to ``ZstdFile.flush()`` method, now it can flush a zstd frame.
+
+#. Add *read_size* and *write_buffer_size* arguments to ``ZstdFile.__init__()`` method, can work with Network File Systems better.
+
+#. Optimize ``ZstdFile`` performance to C language level.
+
 **0.15.7  (Apr 21, 2023)**
 
 ZstdDict class changes:
 
 #. Fix these advanced compression parameters may be ignored when loading a dictionary: ``windowLog``, ``hashLog``, ``chainLog``, ``searchLog``, ``minMatch``, ``targetLength``, ``strategy``, ``enableLongDistanceMatching``, ``ldmHashLog``, ``ldmMinMatch``, ``ldmBucketSizeLog``, ``ldmHashRateLog``, and some non-public parameters.
 
 #. When compressing, load undigested dictionary instead of digested dictionary by default. Loading again an undigested is slower, see `differences <https://pyzstd.readthedocs.io/en/latest/#ZstdDict.as_digested_dict>`_.
```

### Comparing `pyzstd-0.15.7/pyzstd.egg-info/SOURCES.txt` & `pyzstd-0.15.8/pyzstd.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,29 @@
 pyzstd.egg-info/SOURCES.txt
 pyzstd.egg-info/dependency_links.txt
 pyzstd.egg-info/top_level.txt
 src/__init__.py
 src/__init__.pyi
 src/__main__.py
 src/py.typed
-src/bin_ext/_zstdmodule.c
-src/bin_ext/build_cffi.py
+src/seekable_zstdfile.py
+src/zstdfile.py
+src/bin_ext/compressor.c
+src/bin_ext/decompressor.c
+src/bin_ext/dict.c
+src/bin_ext/file.c
+src/bin_ext/macro_functions.h
+src/bin_ext/pyzstd.c
+src/bin_ext/pyzstd.h
+src/bin_ext/pyzstd_build_cffi.py
+src/bin_ext/stream.c
 src/c/c_pyzstd.py
 src/cffi/cffi_pyzstd.py
 tests/__init__.py
+tests/test_seekable.py
 tests/test_zstd.py
 zstd/lib/.gitignore
 zstd/lib/BUCK
 zstd/lib/Makefile
 zstd/lib/README.md
 zstd/lib/libzstd.mk
 zstd/lib/libzstd.pc.in
```

### Comparing `pyzstd-0.15.7/setup.py` & `pyzstd-0.15.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     PYZSTD_AVX2 = False
     PYZSTD_DEBUG = False
     PYZSTD_WARNING_AS_ERROR = False
     PYZSTD_CONFIG_MSG = ''
 
     def build_extensions(self):
         # Print build config message in actual build
-        print(self.PYZSTD_CONFIG_MSG, flush=True)
+        print(self.PYZSTD_CONFIG_MSG)
 
         # Accept assembly files
         self.compiler.src_extensions.extend(['.s', '.S'])
         # Build debug build
         self.debug = self.PYZSTD_DEBUG
 
         for extension in self.extensions:
@@ -68,15 +68,15 @@
                 #   C stack trace, so -g0 and -g2 are same for most users.
                 # -flto:
                 #   This option runs the standard link-time optimizer. To use the
                 #   link-time optimizer, -flto and optimization options should be
                 #   specified at compile time and during the final link.
                 more_options = ['-g0', '-flto']
                 if self.PYZSTD_AVX2:
-                    instrs = ['-mavx2', '-mbmi', '-mbmi2', '-mlzcnt']
+                    instrs = ['-mavx2', '-mlzcnt', '-mbmi', '-mbmi2']
                     more_options.extend(instrs)
                 if self.PYZSTD_WARNING_AS_ERROR:
                     more_options.append('-Werror')
                 extension.extra_compile_args.extend(more_options)
                 extension.extra_link_args.extend(['-g0', '-flto'])
             elif self.compiler.compiler_type == 'msvc':
                 # Remove .S source files, they use gcc/clang syntax.
@@ -163,23 +163,23 @@
         # packages
         packages = ['pyzstd', 'pyzstd.cffi']
 
         # binary extension
         kwargs['module_name'] = 'pyzstd.cffi._cffi_zstd'
 
         sys.path.append('src/bin_ext')
-        import build_cffi
-        binary_extension = build_cffi.get_extension(**kwargs)
+        import pyzstd_build_cffi
+        binary_extension = pyzstd_build_cffi.get_extension(**kwargs)
     else:  # C implementation
         # packages
         packages = ['pyzstd', 'pyzstd.c']
 
         # binary extension
         kwargs['name'] = 'pyzstd.c._zstd'
-        kwargs['sources'].append('src/bin_ext/_zstdmodule.c')
+        kwargs['sources'].append('src/bin_ext/pyzstd.c')
         if MULTI_PHASE_INIT:
             # use multi-phase initialization (PEP-489) on CPython 3.11+
             kwargs['define_macros'].append(('USE_MULTI_PHASE_INIT', None))
 
         binary_extension = Extension(**kwargs)
 
     setup(
@@ -207,15 +207,15 @@
             "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
         ],
-        keywords='zstandard zstd compression decompression compress decompress',
+        keywords='zstandard zstd zst tar file seekable format',
 
         package_dir={'pyzstd': 'src'},
         packages=packages,
         package_data={'pyzstd': ['__init__.pyi', 'py.typed']},
 
         ext_modules=[binary_extension],
         cmdclass={'build_ext': pyzstd_build_ext},
```

### Comparing `pyzstd-0.15.7/src/__init__.pyi` & `pyzstd-0.15.8/src/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -71,30 +71,30 @@
     def __init__(self,
                  dict_content,
                  is_raw: bool = False) -> None: ...
 
     def __len__(self) -> int: ...
 
 class ZstdCompressor:
-    CONTINUE: ClassVar[int]
-    FLUSH_BLOCK: ClassVar[int]
-    FLUSH_FRAME: ClassVar[int]
+    CONTINUE:    ClassVar[Literal[0]]
+    FLUSH_BLOCK: ClassVar[Literal[1]]
+    FLUSH_FRAME: ClassVar[Literal[2]]
 
-    last_mode: Union[ZstdCompressor.CONTINUE, ZstdCompressor.FLUSH_BLOCK, ZstdCompressor.FLUSH_FRAME]
+    last_mode: Literal[0, 1, 2]
 
     def __init__(self,
                  level_or_option: Union[None, int, Dict[CParameter, int]] = None,
                  zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None) -> None: ...
 
     def compress(self,
                  data,
-                 mode: Union[ZstdCompressor.CONTINUE, ZstdCompressor.FLUSH_BLOCK, ZstdCompressor.FLUSH_FRAME] = ZstdCompressor.CONTINUE) -> bytes: ...
+                 mode: Literal[0, 1, 2] = ZstdCompressor.CONTINUE) -> bytes: ...
 
     def flush(self,
-              mode: Union[ZstdCompressor.FLUSH_BLOCK, ZstdCompressor.FLUSH_FRAME] = ZstdCompressor.FLUSH_FRAME) -> bytes: ...
+              mode: Literal[1, 2] = ZstdCompressor.FLUSH_FRAME) -> bytes: ...
 
     def _set_pledged_input_size(self, size: Union[int, None]) -> None: ...
 
 class RichMemZstdCompressor:
     def __init__(self,
                  level_or_option: Union[None, int, Dict[CParameter, int]] = None,
                  zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None) -> None: ...
@@ -110,26 +110,30 @@
                  zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
                  option: Optional[Dict[DParameter, int]] = None) -> None: ...
 
     def decompress(self,
                    data: ByteString,
                    max_length: int = -1) -> bytes: ...
 
+    def _reset_session(self) -> None: ...
+
 class EndlessZstdDecompressor:
     needs_input: bool
     at_frame_edge: bool
 
     def __init__(self,
                  zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
                  option: Optional[Dict[DParameter, int]] = None) -> None: ...
 
     def decompress(self,
                    data: ByteString,
                    max_length: int = -1) -> bytes: ...
 
+    def _reset_session(self) -> None: ...
+
 class ZstdError(Exception):
     ...
 
 def compress(data,
              level_or_option: Union[None, int, Dict[CParameter, int]] = None,
              zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None) -> bytes: ...
 
@@ -167,24 +171,30 @@
     dictionary_id: int
 
 def get_frame_info(frame_buffer: ByteString) -> frame_info: ...
 
 def get_frame_size(frame_buffer: ByteString) -> int: ...
 
 class ZstdFile(io.BufferedIOBase):
+    FLUSH_BLOCK: ClassVar[Literal[1]]
+    FLUSH_FRAME: ClassVar[Literal[2]]
+
     def __init__(self,
                  filename: Union[str, bytes, PathLike, BinaryIO],
                  mode: str = "r",
                  *,
                  level_or_option: Union[None, int, Dict[CParameter, int], Dict[DParameter, int]] = None,
-                 zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None) -> None: ...
+                 zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
+                 read_size: int = 131075,
+                 write_buffer_size: int = 131591) -> None: ...
     def close(self) -> None: ...
 
     def write(self, data) -> int: ...
-    def flush(self) -> None: ...
+    def flush(self,
+              mode: Literal[1, 2] = ZstdFile.FLUSH_BLOCK) -> None: ...
 
     def read(self, size: int = -1) -> bytes: ...
     def read1(self, size: int = -1) -> bytes: ...
     def readinto(self, b) -> int: ...
     def readinto1(self, b) -> int: ...
     def readline(self, size: int = -1) -> bytes: ...
     def seek(self,
@@ -196,14 +206,31 @@
     def fileno(self) -> int: ...
     @property
     def closed(self) -> bool: ...
     def writable(self) -> bool: ...
     def readable(self) -> bool: ...
     def seekable(self) -> bool: ...
 
+class SeekableZstdFile(ZstdFile):
+    def __init__(self,
+                 filename: Union[str, bytes, PathLike, BinaryIO],
+                 mode: str = "r",
+                 *,
+                 level_or_option: Union[None, int, Dict[CParameter, int], Dict[DParameter, int]] = None,
+                 zstd_dict: Union[None, ZstdDict, ZstdDictInfo] = None,
+                 read_size: int = 131075,
+                 write_buffer_size: int = 131591,
+                 max_frame_content_size: int = 1024*1024*1024) -> None: ...
+
+    @property
+    def seek_table_info(self) -> Tuple[int, int, int]: ...
+
+    @staticmethod
+    def is_seekable_format_file(filename: Union[str, bytes, PathLike, BinaryIO]) -> bool: ...
+
 _BinaryMode = Literal["r", "rb", # read
                       "w", "wb", "a", "ab", "x", "xb"] # write
 _TextMode = Literal["rt", # read
                     "wt", "at", "xt"] # write
 
 @overload
 def open(filename: Union[str, bytes, PathLike, BinaryIO],
```

### Comparing `pyzstd-0.15.7/src/__main__.py` & `pyzstd-0.15.8/src/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,17 @@
             setattr(args, self.dest, v)
     return RangeAction
 
 def parse_arg():
     p = argparse.ArgumentParser(
                     prog = 'CLI of pyzstd module',
                     description = ("The command style is similar to zstd's "
-                                   "CLI, but there are some differences."),
+                                   "CLI, but there are some differences.\n"
+                                   "Zstd's CLI should be faster, it has "
+                                   "some I/O optimizations."),
                     epilog=('Examples of use:\n'
                             '  compress a file:\n'
                             '    python -m pyzstd -c IN_FILE -o OUT_FILE\n'
                             '  decompress a file:\n'
                             '    python -m pyzstd -d IN_FILE -o OUT_FILE\n'
                             '  create a tar archive:\n'
                             '    python -m pyzstd --tar-input-dir DIR -o OUT_FILE\n'
```

### Comparing `pyzstd-0.15.7/src/bin_ext/build_cffi.py` & `pyzstd-0.15.8/src/bin_ext/pyzstd_build_cffi.py`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/src/c/c_pyzstd.py` & `pyzstd-0.15.8/src/c/c_pyzstd.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,21 @@
            'CParameter', 'DParameter', 'Strategy',
            # From _zstd
            'ZstdCompressor', 'RichMemZstdCompressor',
            'ZstdDecompressor', 'EndlessZstdDecompressor',
            'ZstdDict', 'ZstdError', 'decompress', 'get_frame_size',
            'compress_stream', 'decompress_stream',
            'zstd_version', 'zstd_version_info',
+           '_train_dict', '_finalize_dict',
+           'ZstdFileReader', 'ZstdFileWriter',
+           '_ZSTD_CStreamSizes', '_ZSTD_DStreamSizes',
            'PYZSTD_CONFIG')
 
-
-# Used in __init__.py
-_ZSTD_DStreamInSize = _zstd._ZSTD_DStreamInSize
+_ZSTD_CStreamSizes = _zstd._ZSTD_CStreamSizes
+_ZSTD_DStreamSizes = _zstd._ZSTD_DStreamSizes
 _train_dict = _zstd._train_dict
 _finalize_dict = _zstd._finalize_dict
 
 
 # compressionLevel_values
 _nt_values = namedtuple('values', ['default', 'min', 'max'])
 compressionLevel_values = _nt_values(*_zstd._compressionLevel_values)
```

### Comparing `pyzstd-0.15.7/src/cffi/cffi_pyzstd.py` & `pyzstd-0.15.8/src/cffi/cffi_pyzstd.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,36 +10,42 @@
 __all__ = ('ZstdCompressor', 'RichMemZstdCompressor',
            'ZstdDecompressor', 'EndlessZstdDecompressor',
            'ZstdDict', 'ZstdError',
            'CParameter', 'DParameter', 'Strategy',
            'decompress', 'get_frame_info', 'get_frame_size',
            'compress_stream', 'decompress_stream',
            'zstd_version', 'zstd_version_info',
-           'compressionLevel_values', 'PYZSTD_CONFIG')
+           'compressionLevel_values',
+           '_train_dict', '_finalize_dict',
+           'ZstdFileReader', 'ZstdFileWriter',
+           '_ZSTD_CStreamSizes', '_ZSTD_DStreamSizes',
+           'PYZSTD_CONFIG')
 
 PYZSTD_CONFIG = (64 if maxsize > 2**32 else 32,
                  'cffi', bool(m.pyzstd_static_link), False)
 
-# Used in __init__.py
-_ZSTD_DStreamInSize = m.ZSTD_DStreamInSize()
+_ZSTD_CStreamSizes = (m.ZSTD_CStreamInSize(), m.ZSTD_CStreamOutSize())
+_ZSTD_DStreamSizes = (m.ZSTD_DStreamInSize(), m.ZSTD_DStreamOutSize())
+_ZSTD_DStreamOutSize = m.ZSTD_DStreamOutSize()
 
 zstd_version = ffi.string(m.ZSTD_versionString()).decode('ascii')
 zstd_version_info = tuple(int(i) for i in zstd_version.split('.'))
 
 _nt_values = namedtuple('values', ['default', 'min', 'max'])
 compressionLevel_values = _nt_values(m.ZSTD_defaultCLevel(),
                                      m.ZSTD_minCLevel(),
                                      m.ZSTD_maxCLevel())
 
 _new_nonzero = ffi.new_allocator(should_clear_after_alloc=False)
 
 def _nbytes(dat):
     if isinstance(dat, (bytes, bytearray)):
         return len(dat)
-    return memoryview(dat).nbytes
+    with memoryview(dat) as mv:
+        return mv.nbytes
 
 class ZstdError(Exception):
     "Call to the underlying zstd library failed."
     pass
 
 def _get_param_bounds(is_compress, key):
     # Get parameter bounds
@@ -432,16 +438,14 @@
         "Unable to finalize zstd dictionary: %s")
 
     @staticmethod
     def get_type_msg(type):
         return _ErrorType._TYPE_MSG[type]
 
 def _set_zstd_error(type, zstd_ret):
-    assert m.ZSTD_isError(zstd_ret)
-
     msg = _ErrorType.get_type_msg(type) % \
           ffi.string(m.ZSTD_getErrorName(zstd_ret)).decode('utf-8')
     raise ZstdError(msg)
 
 def _set_parameter_error(is_compress, key, value):
     COMPRESS_PARAMETERS = \
     {m.ZSTD_c_compressionLevel: "compressionLevel",
@@ -740,21 +744,20 @@
                       or m.ZSTD_isError(zstd_ret)):
                     break
 
             # Check error
             if m.ZSTD_isError(zstd_ret):
                 _set_zstd_error(_ErrorType.ERR_COMPRESS, zstd_ret)
 
-            # Finished
-            if in_buf.pos == in_buf.size:
-                return out.finish(out_buf)
-
-            # Output buffer should be exhausted, grow the buffer.
+            # Like ._compress_impl(), output as much as possible.
             if out_buf.pos == out_buf.size:
                 out.grow(out_buf)
+            elif in_buf.pos == in_buf.size:
+                # Finished
+                return out.finish(out_buf)
 
     def __reduce__(self):
         msg = "Cannot pickle %s object." % type(self)
         raise TypeError(msg)
 
 class ZstdCompressor(_Compressor):
     """A streaming compressor. Thread-safe at method level."""
@@ -1080,15 +1083,14 @@
                 use_input_buffer = False
 
                 in_buf.src = ffi.from_buffer(data)
                 in_buf.size = len(data)
                 in_buf.pos = 0
             elif len(data) == 0:
                 # Has unconsumed data, fast path for b"".
-                assert self._in_begin < self._in_end
                 use_input_buffer = True
 
                 in_buf.src = self._input_buffer + self._in_begin
                 in_buf.size = self._in_end - self._in_begin
                 in_buf.pos = 0
             else:
                 # Has unconsumed data
@@ -1098,18 +1100,14 @@
                 used_now = self._in_end - self._in_begin
                 # Number of bytes we can append to input buffer
                 avail_now = self._input_buffer_size - self._in_end
                 # Number of bytes we can append if we move existing
                 # contents to beginning of buffer
                 avail_total = self._input_buffer_size - used_now
 
-                assert (used_now > 0
-                        and avail_now >= 0
-                        and avail_total >= 0)
-
                 if avail_total < len(data):
                     new_size = used_now + len(data)
                     # Allocate with new size
                     tmp = _new_nonzero("char[]", new_size)
                     if tmp == ffi.NULL:
                         raise MemoryError
 
@@ -1189,30 +1187,42 @@
                     self._in_end = data_size
                 else:
                     # Use input buffer
                     self._in_begin += in_buf.pos
 
             return ret
         except:
-            # Reset variables
-            self._in_begin = 0
-            self._in_end = 0
-
-            self._needs_input = True
-            if self._type == _TYPE_DEC:
-                self._eof = False
-            else:
-                self._at_frame_edge = True
-
-            # Resetting session never fail
-            m.ZSTD_DCtx_reset(self._dctx, m.ZSTD_reset_session_only)
+            # Reset decompressor's states/session
+            self.__reset_session()
             raise
         finally:
             self._lock.release()
 
+    def __reset_session(self):
+        # Reset variables
+        self._in_begin = 0
+        self._in_end = 0
+
+        self._needs_input = True
+        if self._type == _TYPE_DEC:
+            self._eof = False
+            self._unused_data = ffi.NULL
+        else:
+            self._at_frame_edge = True
+
+        # Resetting session never fail
+        m.ZSTD_DCtx_reset(self._dctx, m.ZSTD_reset_session_only)
+
+    def _reset_session(self):
+        """This is an undocumented method. Reset decompressor's states/session, don't
+        reset parameters and dictionary.
+        """
+        with self._lock:
+            self.__reset_session()
+
     def __reduce__(self):
         msg = "Cannot pickle %s object." % type(self)
         raise TypeError(msg)
 
 class ZstdDecompressor(_Decompressor):
     """A streaming decompressor, it stops after a frame is decompressed.
     Thread-safe at method level."""
@@ -1342,41 +1352,375 @@
         msg = ("Decompression failed: zstd data ends in an incomplete "
                "frame, maybe the input data was truncated. Decompressed "
                "data is %d bytes%s") % (len(ret), extra_msg)
         raise ZstdError(msg)
 
     return ret
 
-def _write_to_output(output_stream, out_mv, out_buf):
-    write_pos = 0
+class ZstdFileReader:
+    def __init__(self, fp, zstd_dict, option, read_size):
+        if read_size <= 0:
+            raise ValueError("read_size argument should > 0")
+        self._read_size = read_size
+
+        # File states, the last three are public attributes.
+        self._fp = fp
+        self.eof = False
+        self.pos = 0     # Decompressed position
+        self.size = -1   # File size, -1 means unknown.
 
-    while write_pos < out_buf.pos:
-        left_bytes = out_buf.pos - write_pos
+        # Decompression states
+        self._needs_input = True
+        self._at_frame_edge = True
 
-        write_bytes = output_stream.write(out_mv[write_pos:out_buf.pos])
-        if write_bytes is None:
-            # The raw stream is set not to block and no single
-            # byte could be readily written to it
-            continue
+        # Input state, need to be initialized with 0.
+        self._in_buf = ffi.new("ZSTD_inBuffer *")
+        if self._in_buf == ffi.NULL:
+            raise MemoryError
+        # Output state
+        self._out_buf = _new_nonzero("ZSTD_outBuffer *")
+        if self._out_buf == ffi.NULL:
+            raise MemoryError
+        # Lazy create forward output buffer
+        self._tmp_output = ffi.NULL
+
+        # Decompression context
+        self._dctx = m.ZSTD_createDCtx()
+        if self._dctx == ffi.NULL:
+            raise ZstdError("Unable to create ZSTD_DCtx instance.")
+
+        # Load dictionary to decompression context
+        if zstd_dict is not None:
+            _load_d_dict(self._dctx, zstd_dict)
+            self.__dict = zstd_dict
+
+        # Set option to decompression context
+        if option is not None:
+            _set_d_parameters(self._dctx, option)
+
+    def __del__(self):
+        try:
+            m.ZSTD_freeDCtx(self._dctx)
+            self._dctx = ffi.NULL
+        except AttributeError:
+            pass
+
+    def _decompress_into(self, out_b, fill_full):
+        # Return
+        if self.eof or out_b.size == out_b.pos:
+            return
+
+        in_b = self._in_buf
+        orig_pos = out_b.pos
+        while True:
+            if in_b.size == in_b.pos and self._needs_input:
+                # Read
+                self._in_dat = self._fp.read(self._read_size)
+                # EOF
+                if not self._in_dat:
+                    if self._at_frame_edge:
+                        self.eof = True
+                        self.pos += out_b.pos - orig_pos
+                        self.size = self.pos
+                        return
+                    else:
+                        raise EOFError("Compressed file ended before the "
+                                       "end-of-stream marker was reached")
+                in_b.src = ffi.from_buffer(self._in_dat)
+                in_b.size = _nbytes(self._in_dat)
+                in_b.pos = 0
+
+            # Decompress
+            zstd_ret = m.ZSTD_decompressStream(self._dctx, out_b, in_b)
+            if m.ZSTD_isError(zstd_ret):
+                _set_zstd_error(_ErrorType.ERR_DECOMPRESS, zstd_ret)
+
+            # Set flags
+            if zstd_ret == 0:
+                self._needs_input = True
+                self._at_frame_edge = True
+            else:
+                self._needs_input = (out_b.size != out_b.pos)
+                self._at_frame_edge = False
+
+            if fill_full:
+                if out_b.size != out_b.pos:
+                    continue
+                else:
+                    self.pos += out_b.pos - orig_pos
+                    return
+            else:
+                if out_b.pos != orig_pos:
+                    self.pos += out_b.pos - orig_pos
+                    return
+
+    def readinto(self, b):
+        out_b = self._out_buf
+        out_b.dst = ffi.from_buffer(b)
+        out_b.size = _nbytes(b)
+        out_b.pos = 0
+
+        self._decompress_into(out_b, False)
+        return out_b.pos
+
+    def readall(self):
+        out_b = self._out_buf
+        out = _BlocksOutputBuffer()
+        if self.size >= 0:
+            # Known file size
+            out.initWithSize(out_b, -1, self.size - self.pos)
         else:
-            if write_bytes < 0 or write_bytes > left_bytes:
-                msg = ("output_stream.write() returned invalid length %d "
-+                      "(should be 0 <= value <= %d)")
-                raise ValueError(msg % (write_bytes, left_bytes))
-            write_pos += write_bytes
+            # Unknown file size
+            out.initAndGrow(out_b, -1)
+
+        while True:
+            self._decompress_into(out_b, True)
+            if self.eof:
+                # Finished
+                return out.finish(out_b)
+            if out_b.size == out_b.pos:
+                # Grow output buffer
+                out.grow(out_b)
+
+    # If obj is None, forward to EOF.
+    # If obj <= 0, do nothing.
+    def forward(self, offset):
+        # Lazy create forward output buffer
+        if self._tmp_output == ffi.NULL:
+            # ZSTD_outBuffer struct
+            self._out_tmp = _new_nonzero("ZSTD_outBuffer *")
+            if self._out_tmp == ffi.NULL:
+                raise MemoryError
+            # Forward output buffer
+            self._tmp_output = _new_nonzero("char[]", _ZSTD_DStreamOutSize)
+            if self._tmp_output == ffi.NULL:
+                raise MemoryError
+            # ZSTD_outBuffer.dst
+            self._out_tmp.dst = self._tmp_output
+        out_b = self._out_tmp
+
+        # Forward to EOF
+        if offset is None:
+            out_b.size = _ZSTD_DStreamOutSize
+            while True:
+                out_b.pos = 0
+                self._decompress_into(out_b, True)
+                if self.eof:
+                    return
+
+        # Forward to offset
+        while offset > 0:
+            out_b.size = min(_ZSTD_DStreamOutSize, offset)
+            out_b.pos = 0
+            self._decompress_into(out_b, True)
+
+            if self.eof:
+                return
+            offset -= out_b.pos
+
+    def reset_session(self):
+        # Reset decompression states
+        self._needs_input = True
+        self._at_frame_edge = True
+        self._in_buf.size = 0
+        self._in_buf.pos = 0
+
+        # Resetting session never fail
+        m.ZSTD_DCtx_reset(self._dctx, m.ZSTD_reset_session_only)
+
+class ZstdFileWriter:
+    def __init__(self, fp, level_or_option, zstd_dict, write_buffer_size):
+        # File object
+        self._fp = fp
+        self._fp_has_flush = hasattr(fp, "flush")
+
+        # States
+        self._last_mode = m.ZSTD_e_end
+        self._use_multithread = False
+        level = 0  # 0 means use zstd's default compression level
+
+        # Write buffer
+        if write_buffer_size <= 0:
+            raise ValueError("write_buffer_size argument should > 0")
+        self._write_buffer_size = write_buffer_size
+
+        self._write_buffer = _new_nonzero("char[]", write_buffer_size)
+        if self._write_buffer == ffi.NULL:
+            raise MemoryError
+
+        # Singleton buffer objects
+        self._in_buf = _new_nonzero("ZSTD_inBuffer *")
+        if self._in_buf == ffi.NULL:
+            raise MemoryError
+
+        self._out_buf = _new_nonzero("ZSTD_outBuffer *")
+        if self._out_buf == ffi.NULL:
+            raise MemoryError
+
+        self._out_mv = memoryview(ffi.buffer(self._write_buffer))
+
+        # Compression context
+        self._cctx = m.ZSTD_createCCtx()
+        if self._cctx == ffi.NULL:
+            raise ZstdError("Unable to create ZSTD_CCtx instance.")
+
+        # Set compressLevel/option to compression context
+        if level_or_option is not None:
+            level, self._use_multithread = \
+                  _set_c_parameters(self._cctx, level_or_option)
+
+        # Load dictionary to compression context
+        if zstd_dict is not None:
+            _load_c_dict(self._cctx, zstd_dict, level)
+            self.__dict = zstd_dict
+
+    def __del__(self):
+        try:
+            m.ZSTD_freeCCtx(self._cctx)
+            self._cctx = ffi.NULL
+        except AttributeError:
+            pass
+
+    def write(self, data):
+        # Output size
+        output_size = 0
+
+        # Input buffer
+        in_b = self._in_buf
+        in_b.src = ffi.from_buffer(data)
+        in_b.size = _nbytes(data)
+        in_b.pos = 0
+
+        # Output buffer, out.pos will be set later.
+        out_b = self._out_buf
+        out_b.dst = self._write_buffer
+        out_b.size = self._write_buffer_size
+
+        # State
+        self._last_mode = m.ZSTD_e_continue
+
+        while True:
+            # Output position
+            out_b.pos = 0
+
+            # Compress
+            if not self._use_multithread:
+                zstd_ret = m.ZSTD_compressStream2(self._cctx, out_b, in_b,
+                                                  m.ZSTD_e_continue)
+            else:
+                while True:
+                    zstd_ret = m.ZSTD_compressStream2(self._cctx, out_b, in_b,
+                                                      m.ZSTD_e_continue)
+                    if (out_b.pos == out_b.size
+                           or in_b.pos == in_b.size
+                           or m.ZSTD_isError(zstd_ret)):
+                        break
+
+            if m.ZSTD_isError(zstd_ret):
+                _set_zstd_error(_ErrorType.ERR_COMPRESS, zstd_ret)
+
+            # Accumulate output bytes
+            output_size += out_b.pos
+
+            # Write output to fp
+            _write_to_fp("self._fp.write()", self._fp,
+                         self._out_mv, out_b)
+
+            # Finished
+            if not self._use_multithread:
+                # Single-thread compression + .CONTINUE mode
+                if zstd_ret == 0:
+                    break
+            else:
+                # Multi-thread compression + .CONTINUE mode
+                if in_b.size == in_b.pos and \
+                   out_b.size != out_b.pos:
+                    break
+
+        return (in_b.size, output_size)
+
+    def flush(self, mode):
+        # Mode argument
+        if mode not in (m.ZSTD_e_flush, m.ZSTD_e_end):
+            msg = ("mode argument wrong value, it should be "
+                   "ZstdFile.FLUSH_BLOCK or ZstdFile.FLUSH_FRAME.")
+            raise ValueError(msg)
+
+        # Don't generate empty content frame
+        if mode == self._last_mode:
+            return (0, 0)
+
+        # Output size
+        output_size = 0
+
+        # Input buffer
+        in_b = self._in_buf
+        in_b.src = self._write_buffer
+        in_b.size = 0
+        in_b.pos = 0
+
+        # Output buffer, out.pos will be set later.
+        out_b = self._out_buf
+        out_b.dst = self._write_buffer
+        out_b.size = self._write_buffer_size
+
+        # State
+        self._last_mode = mode
+
+        while True:
+            # Output position
+            out_b.pos = 0
+
+            # Compress
+            zstd_ret = m.ZSTD_compressStream2(self._cctx, out_b, in_b, mode)
+            if m.ZSTD_isError(zstd_ret):
+                _set_zstd_error(_ErrorType.ERR_COMPRESS, zstd_ret)
+
+            # Accumulate output bytes
+            output_size += out_b.pos
+
+            # Write output to fp
+            _write_to_fp("self._fp.write()", self._fp,
+                         self._out_mv, out_b)
+
+            # Finished
+            if zstd_ret == 0:
+                break
+
+        # Flush
+        if self._fp_has_flush:
+            self._fp.flush()
+
+        return (0, output_size)
+
+# Write output data to fp.
+# If (out_b.pos == 0), do nothing.
+def _write_to_fp(func_name, fp, out_mv, out_b):
+    if out_b.pos == 0:
+        return
+
+    write_ret = fp.write(out_mv[:out_b.pos])
+    if write_ret != out_b.pos:
+        msg = ("%s returned invalid length %d "
+               "(should be %d <= value <= %d)") % \
+               (func_name, write_ret, out_b.pos, out_b.pos)
+        raise ValueError(msg)
 
 def _invoke_callback(callback, in_mv, in_buf, callback_read_pos,
                      out_mv, out_buf, total_input_size, total_output_size):
-    # Input memoryview
+    # Only yield input data once
     in_size = in_buf.size - callback_read_pos
-    # Only yield read data once
     callback_read_pos = in_buf.size
-    in_memoryview = in_mv[:in_size]
 
-    # Output memoryview
+    # Don't yield empty data
+    if in_size == 0 and out_buf.pos == 0:
+        return callback_read_pos
+
+    # memoryview
+    in_memoryview = in_mv[:in_size]
     out_memoryview = out_mv[:out_buf.pos]
 
     # Callback
     callback(total_input_size, total_output_size,
              in_memoryview, out_memoryview)
 
     return callback_read_pos
@@ -1481,27 +1825,24 @@
         out_buf.dst = ffi.from_buffer(_output_block)
         out_buf.size = write_size
 
         # Read
         while True:
             # Invoke .readinto() method
             read_bytes = input_stream.readinto(_input_block)
-            if read_bytes is None:
-                # Non-blocking mode and no bytes are available
-                continue
-            else:
-                if read_bytes < 0 or read_bytes > read_size:
-                    msg = ("input_stream.readinto() returned invalid length "
-                           "%d (should be 0 <= value <= %d)")
-                    raise ValueError(msg % (read_bytes, read_size))
+            if read_bytes < 0 or read_bytes > read_size:
+                msg = ("input_stream.readinto() returned invalid length "
+                       "%d (should be 0 <= value <= %d)") % \
+                       (read_bytes, read_size)
+                raise ValueError(msg)
 
-                # Don't generate empty frame
-                if read_bytes == 0 and total_input_size == 0:
-                    break
-                total_input_size += read_bytes
+            # Don't generate empty frame
+            if read_bytes == 0 and total_input_size == 0:
+                break
+            total_input_size += read_bytes
 
             in_buf.size = read_bytes
             in_buf.pos = 0
             callback_read_pos = 0
             end_directive = m.ZSTD_e_end \
                             if (read_bytes == 0) \
                             else m.ZSTD_e_continue
@@ -1526,25 +1867,27 @@
                     _set_zstd_error(_ErrorType.ERR_COMPRESS, zstd_ret)
 
                 # Accumulate output bytes
                 total_output_size += out_buf.pos
 
                 # Write all output to output_stream
                 if output_stream is not None:
-                    _write_to_output(output_stream, out_mv, out_buf)
+                    _write_to_fp("output_stream.write()", output_stream,
+                                 out_mv, out_buf)
 
                 # Invoke callback
                 if callback is not None:
                     callback_read_pos = _invoke_callback(
                                      callback, in_mv, in_buf, callback_read_pos,
                                      out_mv, out_buf, total_input_size, total_output_size)
 
                 # Finished
-                if end_directive == m.ZSTD_e_continue:
-                    if in_buf.pos == in_buf.size:
+                if use_multithread and end_directive == m.ZSTD_e_continue:
+                    if in_buf.pos == in_buf.size and \
+                       out_buf.pos != out_buf.size:
                         break
                 else:
                     if zstd_ret == 0:
                         break
 
             # Input stream ended
             if read_bytes == 0:
@@ -1632,24 +1975,21 @@
         out_buf.dst = ffi.from_buffer(_output_block)
         out_buf.size = write_size
 
         # Read
         while True:
             # Invoke .readinto() method
             read_bytes = input_stream.readinto(_input_block)
-            if read_bytes is None:
-                # Non-blocking mode and no bytes are available
-                continue
-            else:
-                if read_bytes < 0 or read_bytes > read_size:
-                    msg = ("input_stream.readinto() returned invalid length "
-                           "%d (should be 0 <= value <= %d)")
-                    raise ValueError(msg % (read_bytes, read_size))
+            if read_bytes < 0 or read_bytes > read_size:
+                msg = ("input_stream.readinto() returned invalid length "
+                       "%d (should be 0 <= value <= %d)") % \
+                       (read_bytes, read_size)
+                raise ValueError(msg)
 
-                total_input_size += read_bytes
+            total_input_size += read_bytes
 
             in_buf.size = read_bytes
             in_buf.pos = 0
             callback_read_pos = 0
 
             # Decompress & write
             while True:
@@ -1670,15 +2010,16 @@
                 at_frame_edge = (zstd_ret == 0)
 
                 # Accumulate output bytes
                 total_output_size += out_buf.pos
 
                 # Write all output to output_stream
                 if output_stream is not None:
-                    _write_to_output(output_stream, out_mv, out_buf)
+                    _write_to_fp("output_stream.write()", output_stream,
+                                 out_mv, out_buf)
 
                 # Invoke callback
                 if callback is not None:
                     callback_read_pos = _invoke_callback(
                                      callback, in_mv, in_buf, callback_read_pos,
                                      out_mv, out_buf, total_input_size, total_output_size)
```

### Comparing `pyzstd-0.15.7/zstd/lib/BUCK` & `pyzstd-0.15.8/zstd/lib/BUCK`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/Makefile` & `pyzstd-0.15.8/zstd/lib/Makefile`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/README.md` & `pyzstd-0.15.8/zstd/lib/README.md`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/allocations.h` & `pyzstd-0.15.8/zstd/lib/common/allocations.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/bits.h` & `pyzstd-0.15.8/zstd/lib/common/bits.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/bitstream.h` & `pyzstd-0.15.8/zstd/lib/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/compiler.h` & `pyzstd-0.15.8/zstd/lib/common/compiler.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/cpu.h` & `pyzstd-0.15.8/zstd/lib/common/cpu.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/debug.c` & `pyzstd-0.15.8/zstd/lib/common/debug.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/debug.h` & `pyzstd-0.15.8/zstd/lib/common/debug.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/entropy_common.c` & `pyzstd-0.15.8/zstd/lib/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/error_private.c` & `pyzstd-0.15.8/zstd/lib/common/error_private.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/error_private.h` & `pyzstd-0.15.8/zstd/lib/common/error_private.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/fse.h` & `pyzstd-0.15.8/zstd/lib/common/fse.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/fse_decompress.c` & `pyzstd-0.15.8/zstd/lib/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/huf.h` & `pyzstd-0.15.8/zstd/lib/common/huf.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/mem.h` & `pyzstd-0.15.8/zstd/lib/common/mem.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/pool.c` & `pyzstd-0.15.8/zstd/lib/common/pool.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/pool.h` & `pyzstd-0.15.8/zstd/lib/common/pool.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/portability_macros.h` & `pyzstd-0.15.8/zstd/lib/common/portability_macros.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/threading.c` & `pyzstd-0.15.8/zstd/lib/common/threading.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/threading.h` & `pyzstd-0.15.8/zstd/lib/common/threading.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/xxhash.c` & `pyzstd-0.15.8/zstd/lib/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/xxhash.h` & `pyzstd-0.15.8/zstd/lib/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/zstd_common.c` & `pyzstd-0.15.8/zstd/lib/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/zstd_deps.h` & `pyzstd-0.15.8/zstd/lib/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/zstd_internal.h` & `pyzstd-0.15.8/zstd/lib/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/common/zstd_trace.h` & `pyzstd-0.15.8/zstd/lib/common/zstd_trace.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/clevels.h` & `pyzstd-0.15.8/zstd/lib/compress/clevels.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/fse_compress.c` & `pyzstd-0.15.8/zstd/lib/compress/fse_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/hist.c` & `pyzstd-0.15.8/zstd/lib/compress/hist.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/hist.h` & `pyzstd-0.15.8/zstd/lib/compress/hist.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/huf_compress.c` & `pyzstd-0.15.8/zstd/lib/compress/huf_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_compress.c` & `pyzstd-0.15.8/zstd/lib/compress/zstd_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_internal.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_compress_internal.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_literals.c` & `pyzstd-0.15.8/zstd/lib/compress/zstd_compress_literals.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_literals.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_compress_literals.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_sequences.c` & `pyzstd-0.15.8/zstd/lib/compress/zstd_compress_sequences.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_sequences.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_compress_sequences.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_superblock.c` & `pyzstd-0.15.8/zstd/lib/compress/zstd_compress_superblock.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_compress_superblock.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_compress_superblock.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_cwksp.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_cwksp.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_double_fast.c` & `pyzstd-0.15.8/zstd/lib/compress/zstd_double_fast.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_double_fast.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_double_fast.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_fast.c` & `pyzstd-0.15.8/zstd/lib/compress/zstd_fast.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_fast.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_fast.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_lazy.c` & `pyzstd-0.15.8/zstd/lib/compress/zstd_lazy.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_lazy.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_lazy.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_ldm.c` & `pyzstd-0.15.8/zstd/lib/compress/zstd_ldm.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_ldm.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_ldm.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_ldm_geartab.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_ldm_geartab.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_opt.c` & `pyzstd-0.15.8/zstd/lib/compress/zstd_opt.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstd_opt.h` & `pyzstd-0.15.8/zstd/lib/compress/zstd_opt.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstdmt_compress.c` & `pyzstd-0.15.8/zstd/lib/compress/zstdmt_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/compress/zstdmt_compress.h` & `pyzstd-0.15.8/zstd/lib/compress/zstdmt_compress.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/decompress/huf_decompress.c` & `pyzstd-0.15.8/zstd/lib/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/decompress/huf_decompress_amd64.S` & `pyzstd-0.15.8/zstd/lib/decompress/huf_decompress_amd64.S`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/decompress/zstd_ddict.c` & `pyzstd-0.15.8/zstd/lib/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/decompress/zstd_ddict.h` & `pyzstd-0.15.8/zstd/lib/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress.c` & `pyzstd-0.15.8/zstd/lib/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_block.c` & `pyzstd-0.15.8/zstd/lib/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_block.h` & `pyzstd-0.15.8/zstd/lib/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/decompress/zstd_decompress_internal.h` & `pyzstd-0.15.8/zstd/lib/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/deprecated/zbuff.h` & `pyzstd-0.15.8/zstd/lib/deprecated/zbuff.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/deprecated/zbuff_common.c` & `pyzstd-0.15.8/zstd/lib/deprecated/zbuff_common.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/deprecated/zbuff_compress.c` & `pyzstd-0.15.8/zstd/lib/deprecated/zbuff_compress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/deprecated/zbuff_decompress.c` & `pyzstd-0.15.8/zstd/lib/deprecated/zbuff_decompress.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dictBuilder/cover.c` & `pyzstd-0.15.8/zstd/lib/dictBuilder/cover.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dictBuilder/cover.h` & `pyzstd-0.15.8/zstd/lib/dictBuilder/cover.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dictBuilder/divsufsort.c` & `pyzstd-0.15.8/zstd/lib/dictBuilder/divsufsort.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dictBuilder/divsufsort.h` & `pyzstd-0.15.8/zstd/lib/dictBuilder/divsufsort.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dictBuilder/fastcover.c` & `pyzstd-0.15.8/zstd/lib/dictBuilder/fastcover.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dictBuilder/zdict.c` & `pyzstd-0.15.8/zstd/lib/dictBuilder/zdict.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dll/example/Makefile` & `pyzstd-0.15.8/zstd/lib/dll/example/Makefile`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dll/example/README.md` & `pyzstd-0.15.8/zstd/lib/dll/example/README.md`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dll/example/build_package.bat` & `pyzstd-0.15.8/zstd/lib/dll/example/build_package.bat`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dll/example/fullbench-dll.sln` & `pyzstd-0.15.8/zstd/lib/dll/example/fullbench-dll.sln`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/dll/example/fullbench-dll.vcxproj` & `pyzstd-0.15.8/zstd/lib/dll/example/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_legacy.h` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_legacy.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v01.c` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v01.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v01.h` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v01.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v02.c` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v02.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v02.h` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v02.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v03.c` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v03.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v03.h` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v03.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v04.c` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v04.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v04.h` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v04.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v05.c` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v05.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v05.h` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v05.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v06.c` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v06.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v06.h` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v06.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v07.c` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v07.c`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/legacy/zstd_v07.h` & `pyzstd-0.15.8/zstd/lib/legacy/zstd_v07.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/libzstd.mk` & `pyzstd-0.15.8/zstd/lib/libzstd.mk`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/module.modulemap` & `pyzstd-0.15.8/zstd/lib/module.modulemap`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/zdict.h` & `pyzstd-0.15.8/zstd/lib/zdict.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/zstd.h` & `pyzstd-0.15.8/zstd/lib/zstd.h`

 * *Files identical despite different names*

### Comparing `pyzstd-0.15.7/zstd/lib/zstd_errors.h` & `pyzstd-0.15.8/zstd/lib/zstd_errors.h`

 * *Files identical despite different names*

