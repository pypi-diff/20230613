# Comparing `tmp/pxblat-0.1.6.tar.gz` & `tmp/pxblat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxblat-0.1.6.tar", max compression
+gzip compressed data, was "pxblat-0.2.0.tar", max compression
```

## Comparing `pxblat-0.1.6.tar` & `pxblat-0.2.0.tar`

### file list

```diff
@@ -1,187 +1,199 @@
--rw-r--r--   0        0        0     1067 2023-05-27 06:02:16.177192 pxblat-0.1.6/LICENSE
--rw-r--r--   0        0        0     5596 2023-05-27 06:03:03.530489 pxblat-0.1.6/README.md
--rw-r--r--   0        0        0     8696 2023-05-27 06:02:16.609204 pxblat-0.1.6/build.py
--rw-r--r--   0        0        0     2582 2023-05-27 06:03:03.530489 pxblat-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1092 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/__init__.py
--rw-r--r--   0        0        0       40 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/__init__.py
--rw-r--r--   0        0        0      559 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/cli.py
--rw-r--r--   0        0        0     5944 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/client.py
--rw-r--r--   0        0        0     2325 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/fa2twobit.py
--rw-r--r--   0        0        0      214 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/log.py
--rw-r--r--   0        0        0     7914 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/cli/server.py
--rw-r--r--   0        0        0       54 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/__init__.py
--rw-r--r--   0        0        0    22786 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/__init__.pyi
--rw-r--r--   0        0        0       40 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/.clang-format
--rw-r--r--   0        0        0     1966 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/_extc.cpp
--rw-r--r--   0        0        0       11 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/_extc.modules
--rw-r--r--   0        0        0       81 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/_extc.sources
--rw-r--r--   0        0        0     2163 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
--rw-r--r--   0        0        0    10994 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfClient.cpp
--rw-r--r--   0        0        0    20542 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfServer.cpp
--rw-r--r--   0        0        0     2721 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfServer_1.cpp
--rw-r--r--   0        0        0     3431 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/binder/pygfServer.cpp
--rw-r--r--   0        0        0    33509 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/bs_thread_pool.hpp
--rw-r--r--   0        0        0    28417 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/dbg.h
--rw-r--r--   0        0        0     1986 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/faToTwoBit.cpp
--rw-r--r--   0        0        0     1243 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/faToTwoBit.hpp
--rw-r--r--   0        0        0    13734 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfClient.cpp
--rw-r--r--   0        0        0     4866 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfClient.hpp
--rw-r--r--   0        0        0     6429 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfClient2.cpp
--rw-r--r--   0        0        0      506 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfClient2.hpp
--rw-r--r--   0        0        0    60953 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfServer.cpp
--rw-r--r--   0        0        0    11648 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/gfServer.hpp
--rw-r--r--   0        0        0    11360 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/pygfServer.cpp
--rw-r--r--   0        0        0      979 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/bindings/pygfServer.hpp
--rw-r--r--   0        0        0    24597 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/blat.c
--rw-r--r--   0        0        0     3485 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/faToTwoBit.c
--rw-r--r--   0        0        0     9944 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/gfClient.c
--rw-r--r--   0        0        0    53782 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/gfServer.c
--rw-r--r--   0        0        0       40 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/.clang-format
--rw-r--r--   0        0        0     2088 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/bandExt.h
--rw-r--r--   0        0        0     1073 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/base64.h
--rw-r--r--   0        0        0    27036 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/cheapcgi.h
--rw-r--r--   0        0        0     2097 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/filePath.h
--rw-r--r--   0        0        0      871 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/gfxPoly.h
--rw-r--r--   0        0        0     1034 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/hex.h
--rw-r--r--   0        0        0    10111 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/htmlPage.h
--rw-r--r--   0        0        0     9985 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/htmshell.h
--rw-r--r--   0        0        0      332 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/https.h
--rw-r--r--   0        0        0     4404 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/internet.h
--rw-r--r--   0        0        0     1990 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/kxTok.h
--rw-r--r--   0        0        0    16767 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/memgfx.h
--rw-r--r--   0        0        0     2997 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/mime.h
--rw-r--r--   0        0        0     1166 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/portimpl.h
--rw-r--r--   0        0        0     4401 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/rbTree.h
--rw-r--r--   0        0        0      164 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/aux/srcVersion.h
--rw-r--r--   0        0        0      916 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/aliType.h
--rw-r--r--   0        0        0    10193 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/axt.h
--rw-r--r--   0        0        0     6449 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/bPlusTree.h
--rw-r--r--   0        0        0     4355 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/binRange.h
--rw-r--r--   0        0        0     3456 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/bits.h
--rw-r--r--   0        0        0     5877 2023-05-27 06:02:16.629205 pxblat-0.1.6/src/pxblat/extc/include/core/chain.h
--rw-r--r--   0        0        0     1839 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/chainBlock.h
--rw-r--r--   0        0        0    56916 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/common.h
--rw-r--r--   0        0        0     4198 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/dlist.h
--rw-r--r--   0        0        0     2681 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/dnaseq.h
--rw-r--r--   0        0        0    10058 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/dnautil.h
--rw-r--r--   0        0        0     3658 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/dystring.h
--rw-r--r--   0        0        0     2795 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/errAbort.h
--rw-r--r--   0        0        0     2128 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/errCatch.h
--rw-r--r--   0        0        0     5228 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/fa.h
--rw-r--r--   0        0        0    10590 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/fuzzyFind.h
--rw-r--r--   0        0        0    19945 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/genoFind.h
--rw-r--r--   0        0        0     1115 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/gfClientLib.h
--rw-r--r--   0        0        0     2884 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/gfInternal.h
--rw-r--r--   0        0        0    12187 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/hash.h
--rw-r--r--   0        0        0    14055 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/linefile.h
--rw-r--r--   0        0        0     3618 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/localmem.h
--rw-r--r--   0        0        0    10130 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/maf.h
--rw-r--r--   0        0        0     1786 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/memalloc.h
--rw-r--r--   0        0        0    12155 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/net.h
--rw-r--r--   0        0        0    12162 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/netlib.h
--rw-r--r--   0        0        0     4114 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/nib.h
--rw-r--r--   0        0        0     8773 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/obscure.h
--rw-r--r--   0        0        0      605 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/ooc.h
--rw-r--r--   0        0        0     3981 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/options.h
--rw-r--r--   0        0        0     1910 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/patSpace.h
--rw-r--r--   0        0        0     7300 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/pipeline.h
--rw-r--r--   0        0        0     6256 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/portable.h
--rw-r--r--   0        0        0    14633 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/psl.h
--rw-r--r--   0        0        0     4818 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/rangeTree.h
--rw-r--r--   0        0        0     2459 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/repMask.h
--rw-r--r--   0        0        0     3070 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/sig.h
--rw-r--r--   0        0        0     6814 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/sqlList.h
--rw-r--r--   0        0        0     3444 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/sqlNum.h
--rw-r--r--   0        0        0     2492 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/supStitch.h
--rw-r--r--   0        0        0     2086 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/trans3.h
--rw-r--r--   0        0        0     8657 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/twoBit.h
--rw-r--r--   0        0        0     9058 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/udc.h
--rw-r--r--   0        0        0     1821 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/core/verbose.h
--rw-r--r--   0        0        0        0 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/net/gfNet.h
--rw-r--r--   0        0        0     2278 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/include/net/log.h
--rw-r--r--   0        0        0       40 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/.clang-format
--rw-r--r--   0        0        0    31426 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/axt.c
--rw-r--r--   0        0        0    14386 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/bandExt.c
--rw-r--r--   0        0        0     2996 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/base64.c
--rw-r--r--   0        0        0    11289 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/binRange.c
--rw-r--r--   0        0        0    25709 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/blastOut.c
--rw-r--r--   0        0        0    80472 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/cheapcgi.c
--rw-r--r--   0        0        0    32618 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/ffSeedExtend.c
--rw-r--r--   0        0        0     6436 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/filePath.c
--rw-r--r--   0        0        0     2363 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/hex.c
--rw-r--r--   0        0        0    53011 2023-05-27 06:02:16.633205 pxblat-0.1.6/src/pxblat/extc/src/aux/htmlPage.c
--rw-r--r--   0        0        0    46630 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/htmshell.c
--rw-r--r--   0        0        0    27672 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/https.c
--rw-r--r--   0        0        0     2489 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/intExp.c
--rw-r--r--   0        0        0    16703 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/internet.c
--rw-r--r--   0        0        0    24031 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/maf.c
--rw-r--r--   0        0        0     2306 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/mafFromAxt.c
--rw-r--r--   0        0        0    16690 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/mime.c
--rw-r--r--   0        0        0    62706 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/net.c
--rw-r--r--   0        0        0    62778 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/netlib.c
--rw-r--r--   0        0        0     1742 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/ooc.c
--rw-r--r--   0        0        0    11962 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/patSpace.c
--rw-r--r--   0        0        0     3896 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/portimpl.c
--rw-r--r--   0        0        0    13003 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/rangeTree.c
--rw-r--r--   0        0        0    18572 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/rbTree.c
--rw-r--r--   0        0        0     5678 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/repMask.c
--rw-r--r--   0        0        0      848 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servBrcMcw.c
--rw-r--r--   0        0        0     1033 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servCrunx.c
--rw-r--r--   0        0        0      864 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servcis.c
--rw-r--r--   0        0        0      906 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servmsII.c
--rw-r--r--   0        0        0      921 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/servpws.c
--rw-r--r--   0        0        0    27041 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/sqlList.c
--rw-r--r--   0        0        0     7239 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/sqlNum.c
--rw-r--r--   0        0        0     3898 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/aux/wildcmp.c
--rw-r--r--   0        0        0      930 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/aliType.c
--rw-r--r--   0        0        0    19732 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/bPlusTree.c
--rw-r--r--   0        0        0     9051 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/bits.c
--rw-r--r--   0        0        0    17259 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/chain.c
--rw-r--r--   0        0        0    17077 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/chainBlock.c
--rw-r--r--   0        0        0    90522 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/common.c
--rw-r--r--   0        0        0     9450 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/dlist.c
--rw-r--r--   0        0        0     4604 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/dnaseq.c
--rw-r--r--   0        0        0    29952 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/dnautil.c
--rw-r--r--   0        0        0     7156 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/dystring.c
--rw-r--r--   0        0        0    12046 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/errAbort.c
--rw-r--r--   0        0        0     3932 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/errCatch.c
--rw-r--r--   0        0        0    15611 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/fa.c
--rw-r--r--   0        0        0     3714 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/ffAli.c
--rw-r--r--   0        0        0    10802 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/ffAliHelp.c
--rw-r--r--   0        0        0     4868 2023-05-27 06:02:16.637205 pxblat-0.1.6/src/pxblat/extc/src/core/ffScore.c
--rw-r--r--   0        0        0    40189 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/fuzzyFind.c
--rw-r--r--   0        0        0    70461 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/genoFind.c
--rw-r--r--   0        0        0    52425 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/gfBlatLib.c
--rw-r--r--   0        0        0     6363 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/gfClientLib.c
--rw-r--r--   0        0        0     3845 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/gfInternal.c
--rw-r--r--   0        0        0    18190 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/gfOut.c
--rw-r--r--   0        0        0    22265 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/hash.c
--rw-r--r--   0        0        0     5273 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/kxTok.c
--rw-r--r--   0        0        0    40326 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/linefile.c
--rw-r--r--   0        0        0     7256 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/localmem.c
--rw-r--r--   0        0        0    15074 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/memalloc.c
--rw-r--r--   0        0        0    12778 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/nib.c
--rw-r--r--   0        0        0    24969 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/obscure.c
--rw-r--r--   0        0        0    13012 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/options.c
--rw-r--r--   0        0        0    20522 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/osunix.c
--rw-r--r--   0        0        0    23419 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/pipeline.c
--rw-r--r--   0        0        0    63467 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/psl.c
--rw-r--r--   0        0        0     1203 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/servcl.c
--rw-r--r--   0        0        0    26961 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/supStitch.c
--rw-r--r--   0        0        0     3216 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/trans3.c
--rw-r--r--   0        0        0    33527 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/twoBit.c
--rw-r--r--   0        0        0    71967 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/udc.c
--rw-r--r--   0        0        0     4255 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/core/verbose.c
--rw-r--r--   0        0        0     2571 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/net/gfNet.c
--rw-r--r--   0        0        0     8795 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/extc/src/net/log.c
--rw-r--r--   0        0        0     3052 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/parser.py
--rw-r--r--   0        0        0        0 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/py.typed
--rw-r--r--   0        0        0     1042 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/__init__.py
--rw-r--r--   0        0        0    16982 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/basic.py
--rw-r--r--   0        0        0     4680 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/client.py
--rw-r--r--   0        0        0    10076 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/server.py
--rw-r--r--   0        0        0     1041 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/status.py
--rw-r--r--   0        0        0      115 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/server/utils.py
--rw-r--r--   0        0        0     3431 2023-05-27 06:02:16.641205 pxblat-0.1.6/src/pxblat/utils.py
--rw-r--r--   0        0        0     7213 1970-01-01 00:00:00.000000 pxblat-0.1.6/setup.py
--rw-r--r--   0        0        0     6497 1970-01-01 00:00:00.000000 pxblat-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-13 04:56:47.859163 pxblat-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7841 2023-06-13 04:56:47.859163 pxblat-0.2.0/README.md
+-rw-r--r--   0        0        0     8835 2023-06-13 04:56:48.311165 pxblat-0.2.0/build.py
+-rw-r--r--   0        0        0     2671 2023-06-13 04:57:21.947353 pxblat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1356 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/__init__.py
+-rw-r--r--   0        0        0       40 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/cli.py
+-rw-r--r--   0        0        0     5944 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/client.py
+-rw-r--r--   0        0        0     2316 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/fa2twobit.py
+-rw-r--r--   0        0        0      214 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/log.py
+-rw-r--r--   0        0        0     7914 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/server.py
+-rw-r--r--   0        0        0     3587 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/twobit2fa.py
+-rw-r--r--   0        0        0      560 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/__init__.py
+-rw-r--r--   0        0        0    27659 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/.clang-format
+-rw-r--r--   0        0        0     2083 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/_extc.cpp
+-rw-r--r--   0        0        0       11 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/_extc.modules
+-rw-r--r--   0        0        0       81 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/_extc.sources
+-rw-r--r--   0        0        0     2163 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
+-rw-r--r--   0        0        0    10670 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfClient.cpp
+-rw-r--r--   0        0        0    20188 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfServer.cpp
+-rw-r--r--   0        0        0     2715 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfServer_1.cpp
+-rw-r--r--   0        0        0     4632 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/pygfServer.cpp
+-rw-r--r--   0        0        0     5912 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/twoBitToFa.cpp
+-rw-r--r--   0        0        0    33509 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/bs_thread_pool.hpp
+-rw-r--r--   0        0        0    28417 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/dbg.h
+-rw-r--r--   0        0        0     2116 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/faToTwoBit.cpp
+-rw-r--r--   0        0        0     1243 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/faToTwoBit.hpp
+-rw-r--r--   0        0        0    13652 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/gfClient.cpp
+-rw-r--r--   0        0        0     4820 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/gfClient.hpp
+-rw-r--r--   0        0        0    60809 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/gfServer.cpp
+-rw-r--r--   0        0        0    11554 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/gfServer.hpp
+-rw-r--r--   0        0        0    11325 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/pygfServer.cpp
+-rw-r--r--   0        0        0      973 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/pygfServer.hpp
+-rw-r--r--   0        0        0     8728 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/twoBitToFa.cpp
+-rw-r--r--   0        0        0     3521 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/twoBitToFa.hpp
+-rw-r--r--   0        0        0    24597 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/blat.c
+-rw-r--r--   0        0        0     3485 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/faToTwoBit.c
+-rw-r--r--   0        0        0     9944 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/gfClient.c
+-rw-r--r--   0        0        0    53782 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/gfServer.c
+-rw-r--r--   0        0        0       40 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/.clang-format
+-rw-r--r--   0        0        0     2088 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/bandExt.h
+-rw-r--r--   0        0        0     1073 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/base64.h
+-rw-r--r--   0        0        0    27036 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/cheapcgi.h
+-rw-r--r--   0        0        0     2097 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/filePath.h
+-rw-r--r--   0        0        0      871 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/gfxPoly.h
+-rw-r--r--   0        0        0     1034 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/hex.h
+-rw-r--r--   0        0        0    10111 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/htmlPage.h
+-rw-r--r--   0        0        0     9985 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/htmshell.h
+-rw-r--r--   0        0        0      332 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/https.h
+-rw-r--r--   0        0        0     4404 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/internet.h
+-rw-r--r--   0        0        0     1990 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/kxTok.h
+-rw-r--r--   0        0        0    16767 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/memgfx.h
+-rw-r--r--   0        0        0     2997 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/mime.h
+-rw-r--r--   0        0        0     1166 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/portimpl.h
+-rw-r--r--   0        0        0     4401 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/rbTree.h
+-rw-r--r--   0        0        0      164 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/srcVersion.h
+-rw-r--r--   0        0        0      916 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/core/aliType.h
+-rw-r--r--   0        0        0     6547 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/core/asParse.h
+-rw-r--r--   0        0        0    10193 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/axt.h
+-rw-r--r--   0        0        0     6470 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/bPlusTree.h
+-rw-r--r--   0        0        0    14293 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/basicBed.h
+-rw-r--r--   0        0        0     4355 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/binRange.h
+-rw-r--r--   0        0        0     3456 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/bits.h
+-rw-r--r--   0        0        0     5877 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/chain.h
+-rw-r--r--   0        0        0     1839 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/chainBlock.h
+-rw-r--r--   0        0        0    56916 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/common.h
+-rw-r--r--   0        0        0     4198 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/dlist.h
+-rw-r--r--   0        0        0     2681 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/dnaseq.h
+-rw-r--r--   0        0        0    10058 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/dnautil.h
+-rw-r--r--   0        0        0     3658 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/dystring.h
+-rw-r--r--   0        0        0     2795 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/errAbort.h
+-rw-r--r--   0        0        0     2128 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/errCatch.h
+-rw-r--r--   0        0        0     5228 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/fa.h
+-rw-r--r--   0        0        0    10590 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/fuzzyFind.h
+-rw-r--r--   0        0        0    19945 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/genoFind.h
+-rw-r--r--   0        0        0     1115 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/gfClientLib.h
+-rw-r--r--   0        0        0     2884 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/gfInternal.h
+-rw-r--r--   0        0        0    12187 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/hash.h
+-rw-r--r--   0        0        0     1111 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/htmlColor.h
+-rw-r--r--   0        0        0    14055 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/linefile.h
+-rw-r--r--   0        0        0     3618 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/localmem.h
+-rw-r--r--   0        0        0    10130 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/maf.h
+-rw-r--r--   0        0        0     1786 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/memalloc.h
+-rw-r--r--   0        0        0    12155 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/net.h
+-rw-r--r--   0        0        0    12162 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/netlib.h
+-rw-r--r--   0        0        0     4114 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/nib.h
+-rw-r--r--   0        0        0     8773 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/obscure.h
+-rw-r--r--   0        0        0      605 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/ooc.h
+-rw-r--r--   0        0        0     3981 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/options.h
+-rw-r--r--   0        0        0     1910 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/patSpace.h
+-rw-r--r--   0        0        0     7300 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/pipeline.h
+-rw-r--r--   0        0        0     6256 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/portable.h
+-rw-r--r--   0        0        0    14633 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/psl.h
+-rw-r--r--   0        0        0     4818 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/rangeTree.h
+-rw-r--r--   0        0        0     2459 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/repMask.h
+-rw-r--r--   0        0        0     3070 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/sig.h
+-rw-r--r--   0        0        0     6814 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/sqlList.h
+-rw-r--r--   0        0        0     3444 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/sqlNum.h
+-rw-r--r--   0        0        0     2492 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/supStitch.h
+-rw-r--r--   0        0        0     2499 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/tokenizer.h
+-rw-r--r--   0        0        0     2086 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/trans3.h
+-rw-r--r--   0        0        0     8657 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/twoBit.h
+-rw-r--r--   0        0        0     9058 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/udc.h
+-rw-r--r--   0        0        0     1821 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/verbose.h
+-rw-r--r--   0        0        0        0 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/net/gfNet.h
+-rw-r--r--   0        0        0     2278 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/net/log.h
+-rw-r--r--   0        0        0       40 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/.clang-format
+-rw-r--r--   0        0        0    31426 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/axt.c
+-rw-r--r--   0        0        0    14386 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/bandExt.c
+-rw-r--r--   0        0        0     2996 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/base64.c
+-rw-r--r--   0        0        0    11289 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/binRange.c
+-rw-r--r--   0        0        0    25709 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/blastOut.c
+-rw-r--r--   0        0        0    80472 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/cheapcgi.c
+-rw-r--r--   0        0        0    32618 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/ffSeedExtend.c
+-rw-r--r--   0        0        0     6436 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/filePath.c
+-rw-r--r--   0        0        0     2363 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/hex.c
+-rw-r--r--   0        0        0    53011 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/htmlPage.c
+-rw-r--r--   0        0        0    46630 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/htmshell.c
+-rw-r--r--   0        0        0    27672 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/https.c
+-rw-r--r--   0        0        0     2489 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/intExp.c
+-rw-r--r--   0        0        0    16703 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/internet.c
+-rw-r--r--   0        0        0    24031 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/maf.c
+-rw-r--r--   0        0        0     2306 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/mafFromAxt.c
+-rw-r--r--   0        0        0    16690 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/mime.c
+-rw-r--r--   0        0        0    62706 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/net.c
+-rw-r--r--   0        0        0    62778 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/netlib.c
+-rw-r--r--   0        0        0     1742 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/ooc.c
+-rw-r--r--   0        0        0    11962 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/patSpace.c
+-rw-r--r--   0        0        0     3896 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/portimpl.c
+-rw-r--r--   0        0        0    13003 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/rangeTree.c
+-rw-r--r--   0        0        0    18572 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/rbTree.c
+-rw-r--r--   0        0        0     5678 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/repMask.c
+-rw-r--r--   0        0        0      848 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servBrcMcw.c
+-rw-r--r--   0        0        0     1033 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servCrunx.c
+-rw-r--r--   0        0        0      864 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servcis.c
+-rw-r--r--   0        0        0      906 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servmsII.c
+-rw-r--r--   0        0        0      921 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servpws.c
+-rw-r--r--   0        0        0    27041 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/sqlList.c
+-rw-r--r--   0        0        0     7239 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/sqlNum.c
+-rw-r--r--   0        0        0     3898 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/wildcmp.c
+-rw-r--r--   0        0        0      930 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/aliType.c
+-rw-r--r--   0        0        0    21737 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/asParse.c
+-rw-r--r--   0        0        0    19732 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/bPlusTree.c
+-rw-r--r--   0        0        0    54752 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/basicBed.c
+-rw-r--r--   0        0        0     9051 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/bits.c
+-rw-r--r--   0        0        0    17259 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/chain.c
+-rw-r--r--   0        0        0    17077 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/chainBlock.c
+-rw-r--r--   0        0        0    90522 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/common.c
+-rw-r--r--   0        0        0     9450 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/dlist.c
+-rw-r--r--   0        0        0     4604 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/dnaseq.c
+-rw-r--r--   0        0        0    29952 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/dnautil.c
+-rw-r--r--   0        0        0     7156 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/dystring.c
+-rw-r--r--   0        0        0    12046 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/errAbort.c
+-rw-r--r--   0        0        0     3932 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/errCatch.c
+-rw-r--r--   0        0        0    15611 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/fa.c
+-rw-r--r--   0        0        0     3714 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/ffAli.c
+-rw-r--r--   0        0        0    10802 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/ffAliHelp.c
+-rw-r--r--   0        0        0     4868 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/ffScore.c
+-rw-r--r--   0        0        0    40189 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/fuzzyFind.c
+-rw-r--r--   0        0        0    70461 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/genoFind.c
+-rw-r--r--   0        0        0    52425 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/gfBlatLib.c
+-rw-r--r--   0        0        0     6363 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/gfClientLib.c
+-rw-r--r--   0        0        0     3845 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/gfInternal.c
+-rw-r--r--   0        0        0    18190 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/gfOut.c
+-rw-r--r--   0        0        0    22265 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/hash.c
+-rw-r--r--   0        0        0     2919 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/htmlColor.c
+-rw-r--r--   0        0        0     5273 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/kxTok.c
+-rw-r--r--   0        0        0    40326 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/linefile.c
+-rw-r--r--   0        0        0     7256 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/localmem.c
+-rw-r--r--   0        0        0    15074 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/memalloc.c
+-rw-r--r--   0        0        0    12778 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/nib.c
+-rw-r--r--   0        0        0    24969 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/obscure.c
+-rw-r--r--   0        0        0    13012 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/options.c
+-rw-r--r--   0        0        0    20522 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/osunix.c
+-rw-r--r--   0        0        0    23419 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/pipeline.c
+-rw-r--r--   0        0        0    63467 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/psl.c
+-rw-r--r--   0        0        0     1203 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/servcl.c
+-rw-r--r--   0        0        0    26961 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/supStitch.c
+-rw-r--r--   0        0        0     5025 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/tokenizer.c
+-rw-r--r--   0        0        0     3216 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/trans3.c
+-rw-r--r--   0        0        0    33527 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/twoBit.c
+-rw-r--r--   0        0        0    71967 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/udc.c
+-rw-r--r--   0        0        0     4255 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/verbose.c
+-rw-r--r--   0        0        0     2571 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/net/gfNet.c
+-rw-r--r--   0        0        0     8795 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/net/log.c
+-rw-r--r--   0        0        0     7666 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/extc/twoBitToFa.c
+-rw-r--r--   0        0        0     3052 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/parser.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/py.typed
+-rw-r--r--   0        0        0      988 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/__init__.py
+-rw-r--r--   0        0        0    15567 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/basic.py
+-rw-r--r--   0        0        0     4665 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/client.py
+-rw-r--r--   0        0        0    10366 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/server.py
+-rw-r--r--   0        0        0     1041 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/status.py
+-rw-r--r--   0        0        0      115 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/utils.py
+-rw-r--r--   0        0        0     1796 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/toolkit/__init__.py
+-rw-r--r--   0        0        0     3431 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/utils.py
+-rw-r--r--   0        0        0     9495 1970-01-01 00:00:00.000000 pxblat-0.2.0/setup.py
+-rw-r--r--   0        0        0     8742 1970-01-01 00:00:00.000000 pxblat-0.2.0/PKG-INFO
```

### Comparing `pxblat-0.1.6/LICENSE` & `pxblat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/build.py` & `pxblat-0.2.0/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 from pybind11.setup_helpers import ParallelCompile
 from pybind11.setup_helpers import Pybind11Extension
 from setuptools import Distribution
 from setuptools import Extension
 from setuptools.command.build_ext import build_ext as _build_ext
 
 
+DEBUG = False
+
+
 class PxblatExtensionBuilder(_build_ext):
     def build_extension(self, extension: setuptools.extension.Extension) -> None:  # type: ignore
         extension.library_dirs.append(self.build_lib)  # type: ignore
         super().build_extension(extension)
 
     def build_extensions(self) -> None:
         """
@@ -156,14 +159,15 @@
 
 def _extra_compile_args_for_libpxblat():
     return [
         "-D_FILE_OFFSET_BITS=64",
         "-D_LARGEFILE_SOURCE",
         "-D_GNU_SOURCE",
         "-DMACHTYPE_$(MACHTYPE)",
+        "-DPXBLATLIB",
     ]
 
 
 def _include_dirs_for_libpxblat():
     return [
         "src/pxblat/extc/include/core",
         "src/pxblat/extc/include/aux",
@@ -174,17 +178,18 @@
 def _include_dirs_for_pxblat():
     return [
         "src/pxblat/extc/bindings",
     ]
 
 
 def _extra_compile_args_for_pxblat():
-    return [
-        "-DDBG_MACRO_DISABLE",
-    ]
+    flag = []
+    if not DEBUG:
+        flag.append("-DDBG_MACRO_DISABLE")
+    return flag
 
 
 ParallelCompile(f"{get_thread_count()}").install()
 
 extra_compile_args = ["-pthread"]
 hidden_visibility_args = []
 include_dirs: list[str] = []
@@ -205,14 +210,15 @@
     include_dirs.append(lib_include_dir.as_posix())
 
 if sys.platform == "win32":
     raise RuntimeError("Windows is not supported.")
 elif sys.platform == "darwin":
     # See https://conda-forge.org/docs/maintainer/knowledge_base.html#newer-c-features-with-old-sdk
     extra_compile_args.append("-D_LIBCPP_DISABLE_AVAILABILITY")
+    extra_compile_args.append("-undefined dynamic_lookup")
     hidden_visibility_args.append("-fvisibility=hidden")
     config_vars = distutils.sysconfig.get_config_vars()  # type: ignore
     config_vars["LDSHARED"] = config_vars["LDSHARED"].replace("-bundle", "")  # type: ignore
     python_module_link_args.append("-bundle")
     builder = setuptools.command.build_ext.build_ext(Distribution())  # type: ignore
     full_name = builder.get_ext_filename("libpxblat")
     print(f"full_name: {full_name}")
@@ -253,22 +259,22 @@
         library_dirs=library_dirs,
     )
 
     pxblat_libs = [_get_pxblat_libname()]
     extension_modules.append(pxblat_library)
 
     """
-    An extension module which contains the main Python bindings for turbodbc
+    An extension module which contains the main Python bindings for libblat
     """
     pxblat_python_sources = [
         "src/pxblat/extc/bindings/faToTwoBit.cpp",
+        "src/pxblat/extc/bindings/twoBitToFa.cpp",
         "src/pxblat/extc/bindings/gfServer.cpp",
         "src/pxblat/extc/bindings/pygfServer.cpp",
         "src/pxblat/extc/bindings/gfClient.cpp",
-        "src/pxblat/extc/bindings/gfClient2.cpp",
     ] + list(
         filter_files(get_files_by_suffix("src/pxblat/extc/bindings/binder", [".cpp"]))
     )
 
     pxblat_python = Pybind11Extension(
         "pxblat._extc",
         language="c++",
```

### Comparing `pxblat-0.1.6/pyproject.toml` & `pxblat-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxblat"
-version = "0.1.6"
+version = "0.2.0"
 description = "A native python binding for blat suit"
 authors = ["Yangyang Li <yangyang.li@northwestern.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -66,34 +66,34 @@
 "src/pxblat/extc/__init__.py" = ["F405", "F403"]
 "src/pxblat/server/basic.py" = ["PLR0913"]
 "src/pxblat/server/server.py" = ["PLR0913"]
 "src/pxblat/server/client.py" = ["PLR0913"]
 "src/pxblat/cli/server.py" = ["PLR0913"]
 "src/pxblat/cli/client.py" = ["B008", "PLR0913"]
 "src/pxblat/cli/fa2twobit.py" = ["B008", "PLR0913"]
-
+"src/pxblat/cli/twobit2fa.py" = ["B008", "PLR0913"]
+"src/pxblat/toolkit/__init__.py" = ["PLR0913"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-sugar = "^0.9.7"
 black = "^23.3.0"
-ruff = "^0.0.270"
+ruff = ">=0.0.270,<0.0.273"
 ipython = "^8.13.1"
-pybind11-stubgen = ">=0.13,<0.15"
+pybind11-stubgen = ">=0.13,<0.16"
 invoke = "^2.1.2"
 ipdb = "^0.13.13"
 pysam = "^0.21.0"
 pytest-ordering = "^0.6"
 pytest-xdist = "^3.3.1"
 scienceplots = "^2.0.1"
 tikzplotlib = "^0.10.1"
 nox = "^2023.4.22"
 nox-poetry = "^1.0.2"
 codecov = "^2.1.13"
-urllib3 = "1.26.9"
 myst-parser = "^1.0.0"
 sphinx-immaterial = "^0.11.3"
 linkify-it-py = "^2.0.2"
 sphinx-copybutton = "^0.5.2"
 sphinx-togglebutton = "^0.3.2"
 sphinxcontrib-bibtex = "^2.5.0"
 sphinx-autoapi = "^2.1.0"
```

### Comparing `pxblat-0.1.6/src/pxblat/__init__.py` & `pxblat-0.2.0/src/pxblat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,53 @@
+from .extc import ClientOption
+from .extc import ServerOption
+from .extc import TwoBitToFaOption
+from .extc import UsageStats
 from .parser import read
 from .server import check_port_in_use
 from .server import check_port_open
 from .server import Client
 from .server import create_client_option
 from .server import create_server_option
 from .server import DEFAULT_PORT
-from .server import fa_to_two_bit
 from .server import files
 from .server import find_free_port
 from .server import query_server
 from .server import Server
 from .server import server_query
 from .server import start_server
 from .server import start_server_mt
 from .server import start_server_mt_nb
 from .server import Status
 from .server import status_server
 from .server import stop_server
 from .server import wait_server_ready
-
+from .toolkit import fa_to_two_bit
+from .toolkit import two_bit_to_fa
 
 __all__ = [
     "Server",
     "Client",
     "files",
     "server_query",
     "start_server_mt",
     "start_server",
     "status_server",
     "stop_server",
     "create_client_option",
     "query_server",
     "fa_to_two_bit",
+    "two_bit_to_fa",
     "create_server_option",
     "check_port_open",
     "start_server_mt_nb",
     "wait_server_ready",
     "find_free_port",
     "check_port_in_use",
     "DEFAULT_PORT",
     "Status",
     "read",
+    "TwoBitToFaOption",
+    "ClientOption",
+    "ServerOption",
+    "UsageStats",
 ]
```

### Comparing `pxblat-0.1.6/src/pxblat/cli/cli.py` & `pxblat-0.2.0/src/pxblat/cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import sys
 
 import typer
 
 from .client import client
 from .fa2twobit import faToTwoBit
 from .server import server_app
+from .twobit2fa import twoBitToFa
 
 app = typer.Typer(
-    epilog="YangyangLi 2023 please cite me",
+    epilog="YangyangLi 2023 yangyang.li@northwstern.edu",
     context_settings={"help_option_names": ["-h", "--help"]},
 )
 
 app.command()(faToTwoBit)
 app.command()(client)
+app.command()(twoBitToFa)
 
 
 app.add_typer(server_app, name="server")
 
 
 if "sphinx" in sys.modules and __name__ != "__main__":
     # Create the typer click object to generate docs with sphinx-click
```

### Comparing `pxblat-0.1.6/src/pxblat/cli/client.py` & `pxblat-0.2.0/src/pxblat/cli/client.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/cli/fa2twobit.py` & `pxblat-0.2.0/src/pxblat/cli/fa2twobit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from pathlib import Path
 
 import typer
-from pxblat.server import fa_to_two_bit
+from pxblat import fa_to_two_bit
 
 from .log import logger
 
 # faToTwoBit - Convert DNA from fasta to 2bit format
 # usage:
 #    faToTwoBit in.fa [in2.fa in3.fa ...] out.2bit
 # options:
 #    -long          use 64-bit offsets for index.   Allow for twoBit to contain more than 4Gb of sequence.
 #                   NOT COMPATIBLE WITH OLDER CODE.
 #    -noMask        Ignore lower-case masking in fa file.
 #    -stripVersion  Strip off version number after '.' for GenBank accessions.
 #    -ignoreDups    Convert first sequence only if there are duplicate sequence
 #                   names.  Use 'twoBitDup' to find duplicate sequences.
-#
 
 
 def faToTwoBit(
     infa: list[Path] = typer.Argument(
         ...,
         exists=True,
         dir_okay=False,
```

### Comparing `pxblat-0.1.6/src/pxblat/cli/server.py` & `pxblat-0.2.0/src/pxblat/cli/server.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/binder/_extc.cpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/binder/_extc.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #include <stdexcept>
 #include <string>
 
 #include <pybind11/pybind11.h>
 
 typedef std::function< pybind11::module & (std::string const &) > ModuleGetter;
 
+void bind_twoBitToFa(std::function< pybind11::module &(std::string const &namespace_) > &M);
 void bind_faToTwoBit(std::function< pybind11::module &(std::string const &namespace_) > &M);
 void bind_gfClient(std::function< pybind11::module &(std::string const &namespace_) > &M);
 void bind_gfServer(std::function< pybind11::module &(std::string const &namespace_) > &M);
 void bind_gfServer_1(std::function< pybind11::module &(std::string const &namespace_) > &M);
 void bind_pygfServer(std::function< pybind11::module &(std::string const &namespace_) > &M);
 
 
@@ -40,14 +41,15 @@
 	std::vector< std::pair<std::string, std::string> > sub_modules {
 		{"", "cppbinding"},
 	};
 	for(auto &p : sub_modules ) modules[p.first.size() ? p.first+"::"+p.second : p.second] = modules[p.first].def_submodule( mangle_namespace_name(p.second).c_str(), ("Bindings for " + p.first + "::" + p.second + " namespace").c_str() );
 
 	//pybind11::class_<std::shared_ptr<void>>(M(""), "_encapsulated_data_");
 
+    bind_twoBitToFa(M);
 	bind_faToTwoBit(M);
 	bind_gfClient(M);
 	bind_gfServer(M);
 	bind_gfServer_1(M);
 	bind_pygfServer(M);
 
 }
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/binder/faToTwoBit.cpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/binder/faToTwoBit.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfClient.cpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfClient.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #include <gfClient.hpp>
-#include <gfClient2.hpp>
 #include <ios>
 #include <iterator>
 #include <locale>
 #include <memory>
 #include <ostream>
 #include <sstream> // __str__
 #include <streambuf>
@@ -20,68 +19,69 @@
 	PYBIND11_DECLARE_HOLDER_TYPE(T, std::shared_ptr<T>)
 	PYBIND11_DECLARE_HOLDER_TYPE(T, T*)
 	PYBIND11_MAKE_OPAQUE(std::shared_ptr<void>)
 #endif
 
 void bind_gfClient(std::function< pybind11::module &(std::string const &namespace_) > &M)
 {
-	{ // cppbinding::gfClientOption file:gfClient.hpp line:69
-		pybind11::class_<cppbinding::gfClientOption, std::shared_ptr<cppbinding::gfClientOption>> cl(M("cppbinding"), "gfClientOption", "");
-		cl.def( pybind11::init( [](){ return new cppbinding::gfClientOption(); } ) );
-		cl.def( pybind11::init( [](cppbinding::gfClientOption const &o){ return new cppbinding::gfClientOption(o); } ) );
-		cl.def_readwrite("hostName", &cppbinding::gfClientOption::hostName);
-		cl.def_readwrite("portName", &cppbinding::gfClientOption::portName);
-		cl.def_readwrite("tType", &cppbinding::gfClientOption::tType);
-		cl.def_readwrite("qType", &cppbinding::gfClientOption::qType);
-		cl.def_readwrite("dots", &cppbinding::gfClientOption::dots);
-		cl.def_readwrite("nohead", &cppbinding::gfClientOption::nohead);
-		cl.def_readwrite("minScore", &cppbinding::gfClientOption::minScore);
-		cl.def_readwrite("minIdentity", &cppbinding::gfClientOption::minIdentity);
-		cl.def_readwrite("outputFormat", &cppbinding::gfClientOption::outputFormat);
-		cl.def_readwrite("maxIntron", &cppbinding::gfClientOption::maxIntron);
-		cl.def_readwrite("genome", &cppbinding::gfClientOption::genome);
-		cl.def_readwrite("genomeDataDir", &cppbinding::gfClientOption::genomeDataDir);
-		cl.def_readwrite("isDynamic", &cppbinding::gfClientOption::isDynamic);
-		cl.def_readwrite("SeqDir", &cppbinding::gfClientOption::SeqDir);
-		cl.def_readwrite("inName", &cppbinding::gfClientOption::inName);
-		cl.def_readwrite("outName", &cppbinding::gfClientOption::outName);
-		cl.def_readwrite("inSeq", &cppbinding::gfClientOption::inSeq);
-		cl.def("build", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)()) &cppbinding::gfClientOption::build, "C++: cppbinding::gfClientOption::build() --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic);
-		cl.def("withHost", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withHost, "C++: cppbinding::gfClientOption::withHost(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("hostName_"));
-		cl.def("withPort", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withPort, "C++: cppbinding::gfClientOption::withPort(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("portName_"));
-		cl.def("withTType", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withTType, "C++: cppbinding::gfClientOption::withTType(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("tType_"));
-		cl.def("withQType", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withQType, "C++: cppbinding::gfClientOption::withQType(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("qType_"));
-		cl.def("withDots", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(int)) &cppbinding::gfClientOption::withDots, "C++: cppbinding::gfClientOption::withDots(int) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("dots_"));
-		cl.def("withNohead", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(bool)) &cppbinding::gfClientOption::withNohead, "C++: cppbinding::gfClientOption::withNohead(bool) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("nohead_"));
-		cl.def("withMinScore", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(int)) &cppbinding::gfClientOption::withMinScore, "C++: cppbinding::gfClientOption::withMinScore(int) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("minScore_"));
-		cl.def("withMinIdentity", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(double)) &cppbinding::gfClientOption::withMinIdentity, "C++: cppbinding::gfClientOption::withMinIdentity(double) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("minIdentity_"));
-		cl.def("withOutputFormat", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withOutputFormat, "C++: cppbinding::gfClientOption::withOutputFormat(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("outputFormat_"));
-		cl.def("withMaxIntron", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(long)) &cppbinding::gfClientOption::withMaxIntron, "C++: cppbinding::gfClientOption::withMaxIntron(long) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxIntron_"));
-		cl.def("withGenome", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withGenome, "C++: cppbinding::gfClientOption::withGenome(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("genome_"));
-		cl.def("withGenomeDataDir", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withGenomeDataDir, "C++: cppbinding::gfClientOption::withGenomeDataDir(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("genomeDataDir_"));
-		cl.def("withIsDynamic", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(bool)) &cppbinding::gfClientOption::withIsDynamic, "C++: cppbinding::gfClientOption::withIsDynamic(bool) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("isDynamic_"));
-		cl.def("withSeqDir", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withSeqDir, "C++: cppbinding::gfClientOption::withSeqDir(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("SeqDir_"));
-		cl.def("withInName", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withInName, "C++: cppbinding::gfClientOption::withInName(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("inName_"));
-		cl.def("withOutName", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withOutName, "C++: cppbinding::gfClientOption::withOutName(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("outName_"));
-		cl.def("withInSeq", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withInSeq, "C++: cppbinding::gfClientOption::withInSeq(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("inseq_"));
-		cl.def("to_string", (std::string (cppbinding::gfClientOption::*)() const) &cppbinding::gfClientOption::to_string, "C++: cppbinding::gfClientOption::to_string() const --> std::string");
+	{ // cppbinding::ClientOption file:gfClient.hpp line:69
+		pybind11::class_<cppbinding::ClientOption, std::shared_ptr<cppbinding::ClientOption>> cl(M("cppbinding"), "ClientOption", "");
 
-		cl.def("__str__", [](cppbinding::gfClientOption const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
+		cl.def( pybind11::init( [](){ return new cppbinding::ClientOption(); } ) );
+		cl.def( pybind11::init( [](cppbinding::ClientOption const &o){ return new cppbinding::ClientOption(o); } ) );
+		cl.def_readwrite("hostName", &cppbinding::ClientOption::hostName);
+		cl.def_readwrite("portName", &cppbinding::ClientOption::portName);
+		cl.def_readwrite("tType", &cppbinding::ClientOption::tType);
+		cl.def_readwrite("qType", &cppbinding::ClientOption::qType);
+		cl.def_readwrite("dots", &cppbinding::ClientOption::dots);
+		cl.def_readwrite("nohead", &cppbinding::ClientOption::nohead);
+		cl.def_readwrite("minScore", &cppbinding::ClientOption::minScore);
+		cl.def_readwrite("minIdentity", &cppbinding::ClientOption::minIdentity);
+		cl.def_readwrite("outputFormat", &cppbinding::ClientOption::outputFormat);
+		cl.def_readwrite("maxIntron", &cppbinding::ClientOption::maxIntron);
+		cl.def_readwrite("genome", &cppbinding::ClientOption::genome);
+		cl.def_readwrite("genomeDataDir", &cppbinding::ClientOption::genomeDataDir);
+		cl.def_readwrite("isDynamic", &cppbinding::ClientOption::isDynamic);
+		cl.def_readwrite("SeqDir", &cppbinding::ClientOption::SeqDir);
+		cl.def_readwrite("inName", &cppbinding::ClientOption::inName);
+		cl.def_readwrite("outName", &cppbinding::ClientOption::outName);
+		cl.def_readwrite("inSeq", &cppbinding::ClientOption::inSeq);
+		cl.def("build", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)()) &cppbinding::ClientOption::build, "C++: cppbinding::ClientOption::build() --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic);
+		cl.def("withHost", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withHost, "C++: cppbinding::ClientOption::withHost(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("hostName_"));
+		cl.def("withPort", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withPort, "C++: cppbinding::ClientOption::withPort(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("portName_"));
+		cl.def("withTType", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withTType, "C++: cppbinding::ClientOption::withTType(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("tType_"));
+		cl.def("withQType", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withQType, "C++: cppbinding::ClientOption::withQType(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("qType_"));
+		cl.def("withDots", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(int)) &cppbinding::ClientOption::withDots, "C++: cppbinding::ClientOption::withDots(int) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("dots_"));
+		cl.def("withNohead", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(bool)) &cppbinding::ClientOption::withNohead, "C++: cppbinding::ClientOption::withNohead(bool) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("nohead_"));
+		cl.def("withMinScore", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(int)) &cppbinding::ClientOption::withMinScore, "C++: cppbinding::ClientOption::withMinScore(int) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("minScore_"));
+		cl.def("withMinIdentity", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(double)) &cppbinding::ClientOption::withMinIdentity, "C++: cppbinding::ClientOption::withMinIdentity(double) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("minIdentity_"));
+		cl.def("withOutputFormat", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withOutputFormat, "C++: cppbinding::ClientOption::withOutputFormat(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("outputFormat_"));
+		cl.def("withMaxIntron", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(long)) &cppbinding::ClientOption::withMaxIntron, "C++: cppbinding::ClientOption::withMaxIntron(long) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxIntron_"));
+		cl.def("withGenome", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withGenome, "C++: cppbinding::ClientOption::withGenome(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("genome_"));
+		cl.def("withGenomeDataDir", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withGenomeDataDir, "C++: cppbinding::ClientOption::withGenomeDataDir(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("genomeDataDir_"));
+		cl.def("withIsDynamic", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(bool)) &cppbinding::ClientOption::withIsDynamic, "C++: cppbinding::ClientOption::withIsDynamic(bool) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("isDynamic_"));
+		cl.def("withSeqDir", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withSeqDir, "C++: cppbinding::ClientOption::withSeqDir(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("SeqDir_"));
+		cl.def("withInName", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withInName, "C++: cppbinding::ClientOption::withInName(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("inName_"));
+		cl.def("withOutName", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withOutName, "C++: cppbinding::ClientOption::withOutName(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("outName_"));
+		cl.def("withInSeq", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withInSeq, "C++: cppbinding::ClientOption::withInSeq(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("inseq_"));
+		cl.def("to_string", (std::string (cppbinding::ClientOption::*)() const) &cppbinding::ClientOption::to_string, "C++: cppbinding::ClientOption::to_string() const --> std::string");
 
-        cl.def(pybind11::pickle([](const cppbinding::gfClientOption& p){
+		cl.def("__str__", [](cppbinding::ClientOption const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
+
+        cl.def(pybind11::pickle([](const cppbinding::ClientOption& p){
                return pybind11::make_tuple(p.hostName, p.portName,p.tType, p.qType, p.dots,
                                            p.nohead, p.minScore, p.minIdentity,
                                            p.outputFormat, p.maxIntron, p.genome,
                                            p.genomeDataDir, p.isDynamic, p.SeqDir,
                                            p.inName, p.outName, p.inSeq); },
+
                                 [](pybind11::tuple t){
                                 if (t.size() != 17)
                                     throw std::runtime_error("Invalid state!");
-
-                                cppbinding::gfClientOption p{};
+                                cppbinding::ClientOption p{};
                                 p.hostName = t[0].cast<std::string>();
                                 p.portName = t[1].cast<std::string>();
                                 p.tType = t[2].cast<std::string>();
                                 p.qType = t[3].cast<std::string>();
                                 p.dots = t[4].cast<bool>();
                                 p.nohead = t[5].cast<bool>();
                                 p.minScore = t[6].cast<long>();
@@ -91,25 +91,24 @@
                                 p.genome = t[10].cast<std::string>();
                                 p.genomeDataDir = t[11].cast<std::string>();
                                 p.isDynamic = t[12].cast<bool>();
                                 p.SeqDir = t[13].cast<std::string>();
                                 p.inName = t[14].cast<std::string>();
                                 p.outName = t[15].cast<std::string>();
                                 p.inSeq = t[16].cast<std::string>();
-                                return p;}));
-
+                                return p;})
+               );
 
 	}
-	// cppbinding::pygfClient(struct cppbinding::gfClientOption &) file:gfClient.hpp line:118
-  M("cppbinding").def("pygfClient", [](cppbinding::gfClientOption&o) {
+
+	// cppbinding::pygfClient(struct cppbinding::ClientOption &) file:gfClient.hpp line:118
+  M("cppbinding").def("pygfClient", [](cppbinding::ClientOption&o) {
     auto ret = cppbinding::pygfClient(o);
     return pybind11::bytes(ret);
-  }, "C++: cppbinding::pygfClient(struct cppbinding::gfClientOption &) --> std::string", pybind11::arg("option"));
+  }, "C++: cppbinding::pygfClient(struct cppbinding::ClientOption &) --> std::string", pybind11::arg("option"));
 
-   M("cppbinding").def("pygfClient_no_gil", [](cppbinding::gfClientOption o) {
+   M("cppbinding").def("pygfClient_no_gil", [](cppbinding::ClientOption o) {
     auto ret = cppbinding::pygfClient_no_gil(o);
     // return pybind11::bytes(ret);
-  }, "C++: cppbinding::pygfClient(struct cppbinding::gfClientOption &) --> std::string", pybind11::arg("option"));
-
+  }, "C++: cppbinding::pygfClient(struct cppbinding::ClientOption &) --> std::string", pybind11::arg("option"));
 
-  M("cppbinding").def("pygfClient2", &cppbinding2::pygfClient2);
 }
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfServer.cpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfServer.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -62,86 +62,86 @@
                     p.warnCount = t[4].cast<int>();
                     p.noSigCount = t[5].cast<int>();
                     p.missCount = t[6].cast<int>();
                     p.trimCount = t[7].cast<int>();
                     return p;
                 }));
 	}
-	{ // cppbinding::gfServerOption file:gfServer.hpp line:74
-		pybind11::class_<cppbinding::gfServerOption, std::shared_ptr<cppbinding::gfServerOption>> cl(M("cppbinding"), "gfServerOption", "");
-		cl.def( pybind11::init( [](){ return new cppbinding::gfServerOption(); } ) );
-		cl.def( pybind11::init( [](cppbinding::gfServerOption const &o){ return new cppbinding::gfServerOption(o); } ) );
-		cl.def_readwrite("canStop", &cppbinding::gfServerOption::canStop);
-		cl.def_readwrite("log", &cppbinding::gfServerOption::log);
-		cl.def_readwrite("logFacility", &cppbinding::gfServerOption::logFacility);
-		cl.def_readwrite("mask", &cppbinding::gfServerOption::mask);
-		cl.def_readwrite("maxAaSize", &cppbinding::gfServerOption::maxAaSize);
-		cl.def_readwrite("maxDnaHits", &cppbinding::gfServerOption::maxDnaHits);
-		cl.def_readwrite("maxGap", &cppbinding::gfServerOption::maxGap);
-		cl.def_readwrite("maxNtSize", &cppbinding::gfServerOption::maxNtSize);
-		cl.def_readwrite("maxTransHits", &cppbinding::gfServerOption::maxTransHits);
-		cl.def_readwrite("minMatch", &cppbinding::gfServerOption::minMatch);
-		cl.def_readwrite("repMatch", &cppbinding::gfServerOption::repMatch);
-		cl.def_readwrite("seqLog", &cppbinding::gfServerOption::seqLog);
-		cl.def_readwrite("ipLog", &cppbinding::gfServerOption::ipLog);
-		cl.def_readwrite("debugLog", &cppbinding::gfServerOption::debugLog);
-		cl.def_readwrite("tileSize", &cppbinding::gfServerOption::tileSize);
-		cl.def_readwrite("stepSize", &cppbinding::gfServerOption::stepSize);
-		cl.def_readwrite("trans", &cppbinding::gfServerOption::trans);
-		cl.def_readwrite("syslog", &cppbinding::gfServerOption::syslog);
-		cl.def_readwrite("perSeqMax", &cppbinding::gfServerOption::perSeqMax);
-		cl.def_readwrite("noSimpRepMask", &cppbinding::gfServerOption::noSimpRepMask);
-		cl.def_readwrite("indexFile", &cppbinding::gfServerOption::indexFile);
-		cl.def_readwrite("timeout", &cppbinding::gfServerOption::timeout);
-		cl.def_readwrite("genome", &cppbinding::gfServerOption::genome);
-		cl.def_readwrite("genomeDataDir", &cppbinding::gfServerOption::genomeDataDir);
-		cl.def_readwrite("threads", &cppbinding::gfServerOption::threads);
-		cl.def_readwrite("allowOneMismatch", &cppbinding::gfServerOption::allowOneMismatch);
-		cl.def("build", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)()) &cppbinding::gfServerOption::build, "C++: cppbinding::gfServerOption::build() --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic);
-		cl.def("to_string", (std::string (cppbinding::gfServerOption::*)() const) &cppbinding::gfServerOption::to_string, "C++: cppbinding::gfServerOption::to_string() const --> std::string");
-		cl.def("withCanStop", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(bool)) &cppbinding::gfServerOption::withCanStop, "C++: cppbinding::gfServerOption::withCanStop(bool) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("canStop_"));
-		cl.def("withLogFacility", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(std::string)) &cppbinding::gfServerOption::withLogFacility, "C++: cppbinding::gfServerOption::withLogFacility(std::string) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("logFacility_"));
-		cl.def("withLog", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(std::string)) &cppbinding::gfServerOption::withLog, "C++: cppbinding::gfServerOption::withLog(std::string) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("log_"));
-		cl.def("withMask", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(bool)) &cppbinding::gfServerOption::withMask, "C++: cppbinding::gfServerOption::withMask(bool) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("mask_"));
-		cl.def("withMaxAaSize", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withMaxAaSize, "C++: cppbinding::gfServerOption::withMaxAaSize(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxAaSize_"));
-		cl.def("withMaxDnaHits", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withMaxDnaHits, "C++: cppbinding::gfServerOption::withMaxDnaHits(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxDnaHits_"));
-		cl.def("withMaxGap", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withMaxGap, "C++: cppbinding::gfServerOption::withMaxGap(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxGap_"));
-		cl.def("withMaxNtSize", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withMaxNtSize, "C++: cppbinding::gfServerOption::withMaxNtSize(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxNtSize_"));
-		cl.def("withMaxTransHits", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withMaxTransHits, "C++: cppbinding::gfServerOption::withMaxTransHits(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxTransHits_"));
-		cl.def("withMinMatch", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withMinMatch, "C++: cppbinding::gfServerOption::withMinMatch(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("minMatch_"));
-		cl.def("withRepMatch", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withRepMatch, "C++: cppbinding::gfServerOption::withRepMatch(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("repMatch_"));
-		cl.def("withSeqLog", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(bool)) &cppbinding::gfServerOption::withSeqLog, "C++: cppbinding::gfServerOption::withSeqLog(bool) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("seqLog_"));
-		cl.def("withIpLog", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(bool)) &cppbinding::gfServerOption::withIpLog, "C++: cppbinding::gfServerOption::withIpLog(bool) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("ipLog_"));
-		cl.def("withDebugLog", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(bool)) &cppbinding::gfServerOption::withDebugLog, "C++: cppbinding::gfServerOption::withDebugLog(bool) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("debugLog_"));
-		cl.def("withTileSize", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withTileSize, "C++: cppbinding::gfServerOption::withTileSize(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("tileSize_"));
-		cl.def("withStepSize", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withStepSize, "C++: cppbinding::gfServerOption::withStepSize(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("stepSize_"));
-		cl.def("withTrans", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(bool)) &cppbinding::gfServerOption::withTrans, "C++: cppbinding::gfServerOption::withTrans(bool) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("trans_"));
-		cl.def("withSyslog", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(bool)) &cppbinding::gfServerOption::withSyslog, "C++: cppbinding::gfServerOption::withSyslog(bool) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("syslog_"));
-		cl.def("withPerSeqMax", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(std::string)) &cppbinding::gfServerOption::withPerSeqMax, "C++: cppbinding::gfServerOption::withPerSeqMax(std::string) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("perSeqMax_"));
-		cl.def("withNoSimpRepMask", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(bool)) &cppbinding::gfServerOption::withNoSimpRepMask, "C++: cppbinding::gfServerOption::withNoSimpRepMask(bool) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("noSimpRepMask_"));
-		cl.def("withIndexFile", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(std::string)) &cppbinding::gfServerOption::withIndexFile, "C++: cppbinding::gfServerOption::withIndexFile(std::string) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("indexFile_"));
-		cl.def("withTimeout", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withTimeout, "C++: cppbinding::gfServerOption::withTimeout(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("timeout_"));
-		cl.def("withThreads", (struct cppbinding::gfServerOption & (cppbinding::gfServerOption::*)(int)) &cppbinding::gfServerOption::withThreads, "C++: cppbinding::gfServerOption::withThreads(int) --> struct cppbinding::gfServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("threads_"));
+	{ // cppbinding::ServerOption file:gfServer.hpp line:74
+		pybind11::class_<cppbinding::ServerOption, std::shared_ptr<cppbinding::ServerOption>> cl(M("cppbinding"), "ServerOption", "");
+		cl.def( pybind11::init( [](){ return new cppbinding::ServerOption(); } ) );
+		cl.def( pybind11::init( [](cppbinding::ServerOption const &o){ return new cppbinding::ServerOption(o); } ) );
+		cl.def_readwrite("canStop", &cppbinding::ServerOption::canStop);
+		cl.def_readwrite("log", &cppbinding::ServerOption::log);
+		cl.def_readwrite("logFacility", &cppbinding::ServerOption::logFacility);
+		cl.def_readwrite("mask", &cppbinding::ServerOption::mask);
+		cl.def_readwrite("maxAaSize", &cppbinding::ServerOption::maxAaSize);
+		cl.def_readwrite("maxDnaHits", &cppbinding::ServerOption::maxDnaHits);
+		cl.def_readwrite("maxGap", &cppbinding::ServerOption::maxGap);
+		cl.def_readwrite("maxNtSize", &cppbinding::ServerOption::maxNtSize);
+		cl.def_readwrite("maxTransHits", &cppbinding::ServerOption::maxTransHits);
+		cl.def_readwrite("minMatch", &cppbinding::ServerOption::minMatch);
+		cl.def_readwrite("repMatch", &cppbinding::ServerOption::repMatch);
+		cl.def_readwrite("seqLog", &cppbinding::ServerOption::seqLog);
+		cl.def_readwrite("ipLog", &cppbinding::ServerOption::ipLog);
+		cl.def_readwrite("debugLog", &cppbinding::ServerOption::debugLog);
+		cl.def_readwrite("tileSize", &cppbinding::ServerOption::tileSize);
+		cl.def_readwrite("stepSize", &cppbinding::ServerOption::stepSize);
+		cl.def_readwrite("trans", &cppbinding::ServerOption::trans);
+		cl.def_readwrite("syslog", &cppbinding::ServerOption::syslog);
+		cl.def_readwrite("perSeqMax", &cppbinding::ServerOption::perSeqMax);
+		cl.def_readwrite("noSimpRepMask", &cppbinding::ServerOption::noSimpRepMask);
+		cl.def_readwrite("indexFile", &cppbinding::ServerOption::indexFile);
+		cl.def_readwrite("timeout", &cppbinding::ServerOption::timeout);
+		cl.def_readwrite("genome", &cppbinding::ServerOption::genome);
+		cl.def_readwrite("genomeDataDir", &cppbinding::ServerOption::genomeDataDir);
+		cl.def_readwrite("threads", &cppbinding::ServerOption::threads);
+		cl.def_readwrite("allowOneMismatch", &cppbinding::ServerOption::allowOneMismatch);
+		cl.def("build", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)()) &cppbinding::ServerOption::build, "C++: cppbinding::ServerOption::build() --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic);
+		cl.def("to_string", (std::string (cppbinding::ServerOption::*)() const) &cppbinding::ServerOption::to_string, "C++: cppbinding::ServerOption::to_string() const --> std::string");
+		cl.def("withCanStop", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(bool)) &cppbinding::ServerOption::withCanStop, "C++: cppbinding::ServerOption::withCanStop(bool) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("canStop_"));
+		cl.def("withLogFacility", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(std::string)) &cppbinding::ServerOption::withLogFacility, "C++: cppbinding::ServerOption::withLogFacility(std::string) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("logFacility_"));
+		cl.def("withLog", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(std::string)) &cppbinding::ServerOption::withLog, "C++: cppbinding::ServerOption::withLog(std::string) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("log_"));
+		cl.def("withMask", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(bool)) &cppbinding::ServerOption::withMask, "C++: cppbinding::ServerOption::withMask(bool) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("mask_"));
+		cl.def("withMaxAaSize", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withMaxAaSize, "C++: cppbinding::ServerOption::withMaxAaSize(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxAaSize_"));
+		cl.def("withMaxDnaHits", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withMaxDnaHits, "C++: cppbinding::ServerOption::withMaxDnaHits(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxDnaHits_"));
+		cl.def("withMaxGap", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withMaxGap, "C++: cppbinding::ServerOption::withMaxGap(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxGap_"));
+		cl.def("withMaxNtSize", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withMaxNtSize, "C++: cppbinding::ServerOption::withMaxNtSize(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxNtSize_"));
+		cl.def("withMaxTransHits", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withMaxTransHits, "C++: cppbinding::ServerOption::withMaxTransHits(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("maxTransHits_"));
+		cl.def("withMinMatch", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withMinMatch, "C++: cppbinding::ServerOption::withMinMatch(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("minMatch_"));
+		cl.def("withRepMatch", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withRepMatch, "C++: cppbinding::ServerOption::withRepMatch(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("repMatch_"));
+		cl.def("withSeqLog", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(bool)) &cppbinding::ServerOption::withSeqLog, "C++: cppbinding::ServerOption::withSeqLog(bool) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("seqLog_"));
+		cl.def("withIpLog", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(bool)) &cppbinding::ServerOption::withIpLog, "C++: cppbinding::ServerOption::withIpLog(bool) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("ipLog_"));
+		cl.def("withDebugLog", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(bool)) &cppbinding::ServerOption::withDebugLog, "C++: cppbinding::ServerOption::withDebugLog(bool) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("debugLog_"));
+		cl.def("withTileSize", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withTileSize, "C++: cppbinding::ServerOption::withTileSize(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("tileSize_"));
+		cl.def("withStepSize", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withStepSize, "C++: cppbinding::ServerOption::withStepSize(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("stepSize_"));
+		cl.def("withTrans", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(bool)) &cppbinding::ServerOption::withTrans, "C++: cppbinding::ServerOption::withTrans(bool) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("trans_"));
+		cl.def("withSyslog", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(bool)) &cppbinding::ServerOption::withSyslog, "C++: cppbinding::ServerOption::withSyslog(bool) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("syslog_"));
+		cl.def("withPerSeqMax", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(std::string)) &cppbinding::ServerOption::withPerSeqMax, "C++: cppbinding::ServerOption::withPerSeqMax(std::string) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("perSeqMax_"));
+		cl.def("withNoSimpRepMask", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(bool)) &cppbinding::ServerOption::withNoSimpRepMask, "C++: cppbinding::ServerOption::withNoSimpRepMask(bool) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("noSimpRepMask_"));
+		cl.def("withIndexFile", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(std::string)) &cppbinding::ServerOption::withIndexFile, "C++: cppbinding::ServerOption::withIndexFile(std::string) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("indexFile_"));
+		cl.def("withTimeout", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withTimeout, "C++: cppbinding::ServerOption::withTimeout(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("timeout_"));
+		cl.def("withThreads", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withThreads, "C++: cppbinding::ServerOption::withThreads(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("threads_"));
 
-		cl.def("__str__", [](cppbinding::gfServerOption const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
+		cl.def("__str__", [](cppbinding::ServerOption const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
 
         cl.def(pybind11::pickle(
-            [](const cppbinding::gfServerOption &p) { // __getstate__
+            [](const cppbinding::ServerOption &p) { // __getstate__
 
                 return pybind11::make_tuple(p.canStop,p.log,p.logFacility, p.mask, p.maxAaSize, p.maxDnaHits,
                                             p.maxGap, p.maxNtSize, p.maxTransHits, p.minMatch, p.repMatch,
                                             p.seqLog, p.ipLog, p.debugLog, p.tileSize, p.stepSize,p.trans,
                                             p.syslog, p.perSeqMax, p.noSimpRepMask, p.indexFile, p.timeout,
                                             p.genome, p.genomeDataDir,p.threads,p.allowOneMismatch);
 
                  },
                 [](pybind11::tuple t) { // __setstate__
                   if (t.size() != 26)
                       throw std::runtime_error("Invalid state!");
-                    cppbinding::gfServerOption p{};
+                    cppbinding::ServerOption p{};
                     p.withCanStop(t[0].cast<bool>());
                     p.withLog(t[1].cast<std::string>());
                     p.withLogFacility(t[2].cast<std::string>());
                     p.withMask(t[3].cast<bool>());
                     p.withMaxAaSize(t[4].cast<int>());
                     p.withMaxDnaHits(t[5].cast<int>());
                     p.withMaxGap(t[6].cast<int>());
@@ -164,41 +164,41 @@
                     p.genome = t[22].cast<std::string>();
                     p.genomeDataDir = t[23].cast<std::string>();
                     p.withThreads(t[24].cast<int>());
                     p.allowOneMismatch = t[25].cast<bool>();
                     return p;
             }));
 	}
-	// cppbinding::gfServer(struct cppbinding::gfServerOption &) file:gfServer.hpp line:146
-	M("cppbinding").def("gfServer", (void (*)(struct cppbinding::gfServerOption &)) &cppbinding::gfServer, "C++: cppbinding::gfServer(struct cppbinding::gfServerOption &) --> void", pybind11::arg("options"));
+	// cppbinding::gfServer(struct cppbinding::ServerOption &) file:gfServer.hpp line:146
+	M("cppbinding").def("gfServer", (void (*)(struct cppbinding::ServerOption &)) &cppbinding::gfServer, "C++: cppbinding::gfServer(struct cppbinding::ServerOption &) --> void", pybind11::arg("options"));
 
-	// cppbinding::genoFindDirect(std::string &, int, class std::vector<std::string > &, const struct cppbinding::gfServerOption &) file:gfServer.hpp line:158
-	M("cppbinding").def("genoFindDirect", (void (*)(std::string &, int, class std::vector<std::string > &, const struct cppbinding::gfServerOption &)) &cppbinding::genoFindDirect, "C++: cppbinding::genoFindDirect(std::string &, int, class std::vector<std::string > &, const struct cppbinding::gfServerOption &) --> void", pybind11::arg("probeName"), pybind11::arg("fileCount"), pybind11::arg("seqFiles"), pybind11::arg("options"));
+	// cppbinding::genoFindDirect(std::string &, int, class std::vector<std::string > &, const struct cppbinding::ServerOption &) file:gfServer.hpp line:158
+	M("cppbinding").def("genoFindDirect", (void (*)(std::string &, int, class std::vector<std::string > &, const struct cppbinding::ServerOption &)) &cppbinding::genoFindDirect, "C++: cppbinding::genoFindDirect(std::string &, int, class std::vector<std::string > &, const struct cppbinding::ServerOption &) --> void", pybind11::arg("probeName"), pybind11::arg("fileCount"), pybind11::arg("seqFiles"), pybind11::arg("options"));
 
-	// cppbinding::genoPcrDirect(std::string &, std::string &, int, class std::vector<std::string > &, const struct cppbinding::gfServerOption &) file:gfServer.hpp line:162
-	M("cppbinding").def("genoPcrDirect", (void (*)(std::string &, std::string &, int, class std::vector<std::string > &, const struct cppbinding::gfServerOption &)) &cppbinding::genoPcrDirect, "C++: cppbinding::genoPcrDirect(std::string &, std::string &, int, class std::vector<std::string > &, const struct cppbinding::gfServerOption &) --> void", pybind11::arg("fPrimer"), pybind11::arg("rPrimer"), pybind11::arg("fileCount"), pybind11::arg("seqFiles"), pybind11::arg("options"));
+	// cppbinding::genoPcrDirect(std::string &, std::string &, int, class std::vector<std::string > &, const struct cppbinding::ServerOption &) file:gfServer.hpp line:162
+	M("cppbinding").def("genoPcrDirect", (void (*)(std::string &, std::string &, int, class std::vector<std::string > &, const struct cppbinding::ServerOption &)) &cppbinding::genoPcrDirect, "C++: cppbinding::genoPcrDirect(std::string &, std::string &, int, class std::vector<std::string > &, const struct cppbinding::ServerOption &) --> void", pybind11::arg("fPrimer"), pybind11::arg("rPrimer"), pybind11::arg("fileCount"), pybind11::arg("seqFiles"), pybind11::arg("options"));
 
-	// cppbinding::startServer(std::string &, std::string &, int, class std::vector<std::string > &, struct cppbinding::gfServerOption &, struct cppbinding::UsageStats &) file:gfServer.hpp line:167
-	M("cppbinding").def("startServer", (void (*)(std::string &, std::string &, int, class std::vector<std::string > &, struct cppbinding::gfServerOption &, struct cppbinding::UsageStats &)) &cppbinding::startServer, "C++: cppbinding::startServer(std::string &, std::string &, int, class std::vector<std::string > &, struct cppbinding::gfServerOption &, struct cppbinding::UsageStats &) --> void", pybind11::arg("hostName"), pybind11::arg("portName"), pybind11::arg("fileCount"), pybind11::arg("seqFiles"), pybind11::arg("options"), pybind11::arg("stats"));
+	// cppbinding::startServer(std::string &, std::string &, int, class std::vector<std::string > &, struct cppbinding::ServerOption &, struct cppbinding::UsageStats &) file:gfServer.hpp line:167
+	M("cppbinding").def("startServer", (void (*)(std::string &, std::string &, int, class std::vector<std::string > &, struct cppbinding::ServerOption &, struct cppbinding::UsageStats &)) &cppbinding::startServer, "C++: cppbinding::startServer(std::string &, std::string &, int, class std::vector<std::string > &, struct cppbinding::ServerOption &, struct cppbinding::UsageStats &) --> void", pybind11::arg("hostName"), pybind11::arg("portName"), pybind11::arg("fileCount"), pybind11::arg("seqFiles"), pybind11::arg("options"), pybind11::arg("stats"));
 
 	// cppbinding::stopServer(std::string &, std::string &) file:gfServer.hpp line:171
 	M("cppbinding").def("stopServer", (void (*)(std::string &, std::string &)) &cppbinding::stopServer, "C++: cppbinding::stopServer(std::string &, std::string &) --> void", pybind11::arg("hostName"), pybind11::arg("portName"));
 
 	// cppbinding::queryServer(std::string &, std::string &, std::string &, std::string &, bool, bool) file:gfServer.hpp line:174
 	M("cppbinding").def("queryServer", (void (*)(std::string &, std::string &, std::string &, std::string &, bool, bool)) &cppbinding::queryServer, "C++: cppbinding::queryServer(std::string &, std::string &, std::string &, std::string &, bool, bool) --> void", pybind11::arg("type"), pybind11::arg("hostName"), pybind11::arg("portName"), pybind11::arg("faName"), pybind11::arg("complex"), pybind11::arg("isProt"));
 
 	// cppbinding::pcrServer(std::string &, std::string &, std::string &, std::string &, int) file:gfServer.hpp line:179
 	M("cppbinding").def("pcrServer", (void (*)(std::string &, std::string &, std::string &, std::string &, int)) &cppbinding::pcrServer, "C++: cppbinding::pcrServer(std::string &, std::string &, std::string &, std::string &, int) --> void", pybind11::arg("hostName"), pybind11::arg("portName"), pybind11::arg("fPrimer"), pybind11::arg("rPrimer"), pybind11::arg("maxSize"));
 
-	// cppbinding::statusServer(std::string &, std::string &, struct cppbinding::gfServerOption &) file:gfServer.hpp line:182
-	M("cppbinding").def("statusServer", (int (*)(std::string &, std::string &, struct cppbinding::gfServerOption &)) &cppbinding::statusServer, "C++: cppbinding::statusServer(std::string &, std::string &, struct cppbinding::gfServerOption &) --> int", pybind11::arg("hostName"), pybind11::arg("portName"), pybind11::arg("options"));
+	// cppbinding::statusServer(std::string &, std::string &, struct cppbinding::ServerOption &) file:gfServer.hpp line:182
+	M("cppbinding").def("statusServer", (int (*)(std::string &, std::string &, struct cppbinding::ServerOption &)) &cppbinding::statusServer, "C++: cppbinding::statusServer(std::string &, std::string &, struct cppbinding::ServerOption &) --> int", pybind11::arg("hostName"), pybind11::arg("portName"), pybind11::arg("options"));
 
 	// cppbinding::getFileList(std::string &, std::string &) file:gfServer.hpp line:185
 	M("cppbinding").def("getFileList", (void (*)(std::string &, std::string &)) &cppbinding::getFileList, "C++: cppbinding::getFileList(std::string &, std::string &) --> void", pybind11::arg("hostName"), pybind11::arg("portName"));
 
-	// cppbinding::buildIndex(std::string &, int, class std::vector<std::string >, const struct cppbinding::gfServerOption &) file:gfServer.hpp line:189
-	M("cppbinding").def("buildIndex", (void (*)(std::string &, int, class std::vector<std::string >, const struct cppbinding::gfServerOption &)) &cppbinding::buildIndex, "C++: cppbinding::buildIndex(std::string &, int, class std::vector<std::string >, const struct cppbinding::gfServerOption &) --> void", pybind11::arg("gfxFile"), pybind11::arg("fileCount"), pybind11::arg("seqFiles"), pybind11::arg("options"));
+	// cppbinding::buildIndex(std::string &, int, class std::vector<std::string >, const struct cppbinding::ServerOption &) file:gfServer.hpp line:189
+	M("cppbinding").def("buildIndex", (void (*)(std::string &, int, class std::vector<std::string >, const struct cppbinding::ServerOption &)) &cppbinding::buildIndex, "C++: cppbinding::buildIndex(std::string &, int, class std::vector<std::string >, const struct cppbinding::ServerOption &) --> void", pybind11::arg("gfxFile"), pybind11::arg("fileCount"), pybind11::arg("seqFiles"), pybind11::arg("options"));
 
 	// cppbinding::getPortIx(char *) file:gfServer.hpp line:191
 	M("cppbinding").def("getPortIx", (int (*)(char *)) &cppbinding::getPortIx, "C++: cppbinding::getPortIx(char *) --> int", pybind11::arg("portName"));
 
 }
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/binder/gfServer_1.cpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfServer_1.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 	PYBIND11_DECLARE_HOLDER_TYPE(T, std::shared_ptr<T>)
 	PYBIND11_DECLARE_HOLDER_TYPE(T, T*)
 	PYBIND11_MAKE_OPAQUE(std::shared_ptr<void>)
 #endif
 
 void bind_gfServer_1(std::function< pybind11::module &(std::string const &namespace_) > &M)
 {
-	// cppbinding::pystatusServer(std::string &, std::string &, struct cppbinding::gfServerOption &) file:gfServer.hpp line:238
-	M("cppbinding").def("pystatusServer", (std::string (*)(std::string &, std::string &, struct cppbinding::gfServerOption &)) &cppbinding::pystatusServer, "C++: cppbinding::pystatusServer(std::string &, std::string &, struct cppbinding::gfServerOption &) --> std::string", pybind11::arg("hostName"), pybind11::arg("portName"), pybind11::arg("options"));
+	// cppbinding::pystatusServer(std::string &, std::string &, struct cppbinding::ServerOption &) file:gfServer.hpp line:238
+	M("cppbinding").def("pystatusServer", (std::string (*)(std::string &, std::string &, struct cppbinding::ServerOption &)) &cppbinding::pystatusServer, "C++: cppbinding::pystatusServer(std::string &, std::string &, struct cppbinding::ServerOption &) --> std::string", pybind11::arg("hostName"), pybind11::arg("portName"), pybind11::arg("options"));
 
 	// cppbinding::pygetFileList(std::string &, std::string &) file:gfServer.hpp line:239
 	M("cppbinding").def("pygetFileList", (std::string (*)(std::string &, std::string &)) &cppbinding::pygetFileList, "C++: cppbinding::pygetFileList(std::string &, std::string &) --> std::string", pybind11::arg("hostName"), pybind11::arg("portName"));
 
 	// cppbinding::pyqueryServer(std::string &, std::string &, std::string &, std::string &, bool, bool) file:gfServer.hpp line:240
 	M("cppbinding").def("pyqueryServer", (std::string (*)(std::string &, std::string &, std::string &, std::string &, bool, bool)) &cppbinding::pyqueryServer, "C++: cppbinding::pyqueryServer(std::string &, std::string &, std::string &, std::string &, bool, bool) --> std::string", pybind11::arg("type"), pybind11::arg("hostName"), pybind11::arg("portName"), pybind11::arg("faName"), pybind11::arg("complex"), pybind11::arg("isProt"));
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/bs_thread_pool.hpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/bs_thread_pool.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/dbg.h` & `pxblat-0.2.0/src/pxblat/extc/bindings/dbg.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/faToTwoBit.cpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/faToTwoBit.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #pragma GCC diagnostic ignored "-Wwrite-strings"
 
 #include "faToTwoBit.hpp"
 
+#include <stdexcept>
+
 namespace cppbinding {
 
 void unknownToN(char *s, int size)
 /* Convert non ACGT characters to N. */
 {
   char c;
   int i;
@@ -23,14 +25,16 @@
 //-1 errAbort("Duplicate sequence name %s", seq.name);
 int faToTwoBit(std::vector<std::string> &inFiles, std::string &outFile, bool noMask, bool stripVersion, bool ignoreDups,
                bool useLong)
 
 /* Convert inFiles in fasta format to outfile in 2 bit
  * format. */
 {
+  dnaUtilOpen();
+
   struct twoBit *twoBitList = NULL, *twoBit;
   // int i;
   struct hash *uniqHash = newHash(18);
   FILE *f;
 
   for (auto &fileName : inFiles) {
     struct lineFile *lf = lineFileOpen(fileName.data(), TRUE);
@@ -48,15 +52,17 @@
         sp = strchr(seq.name, '.');
         if (sp != NULL) *sp = '\0';
       }
 
       if (hashLookup(uniqHash, seq.name)) {
         if (!ignoreDups)
           // errAbort("Duplicate sequence name %s", seq.name);
-          return -1;
+          throw std::runtime_error("Duplicate sequence name " + std::string(seq.name));
+        // return -1;
+
         else
           continue;
       }
       hashAdd(uniqHash, seq.name, NULL);
       if (noMask)
         faToDna(seq.dna, seq.size);
       else
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/faToTwoBit.hpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/faToTwoBit.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/gfClient.cpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/gfClient.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
   while (fgets(line, buffsize, file) != NULL) {
     ret_str << line;
   }
   return ret_str.str();
 }
 
-std::string pygfClient_no_gil(gfClientOption option) {
+std::string pygfClient_no_gil(ClientOption option) {
   // setFfIntronMax(option.maxIntron);
   pybind11::gil_scoped_release release;
 
   long enterMainTime = clock1000();
 
   auto hostName = option.hostName.data();
   auto portName = option.portName.data();
@@ -160,15 +160,15 @@
     return read_inmem_file(out);
   }
   pybind11::gil_scoped_acquire acquire;
   return "";
 }
 
 /* gfClient - A client for the genomic finding program that produces a .psl file. */
-std::string pygfClient(gfClientOption &option) {
+std::string pygfClient(ClientOption &option) {
   setFfIntronMax(option.maxIntron);
   long enterMainTime = clock1000();
 
   auto hostName = option.hostName.data();
   auto portName = option.portName.data();
 
   auto minIdentity = option.minIdentity;
@@ -295,117 +295,117 @@
 
   if (option.outName.empty()) {
     return read_inmem_file(out);
   }
   return "";
 }
 
-gfClientOption &gfClientOption::build() {
+ClientOption &ClientOption::build() {
   // char *hostName, char *portName, char *tSeqDir, char *inName, char *outName, char *tTypeName, char *qTypeName
   if (tType == "prot" || tType == "dnax" || tType == "rnax") minIdentity = 25;
 
   if (!genomeDataDir.empty() && genome.empty())
     // errAbort("-genomeDataDir requires the -genome option");
     throw std::runtime_error("-genomeDataDir requires the -genome option");
 
   if (!genome.empty() && genomeDataDir.empty()) genomeDataDir = ".";
   if (!genomeDataDir.empty()) isDynamic = true;
 
   return *this;
 }
 
-gfClientOption &gfClientOption::withHost(const std::string &hostName_) {
+ClientOption &ClientOption::withHost(const std::string &hostName_) {
   hostName = hostName_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withPort(const std::string &portName_) {
+ClientOption &ClientOption::withPort(const std::string &portName_) {
   portName = portName_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withTType(const std::string &tType_) {
+ClientOption &ClientOption::withTType(const std::string &tType_) {
   tType = tType_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withQType(const std::string &qType_) {
+ClientOption &ClientOption::withQType(const std::string &qType_) {
   qType = qType_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withDots(int dots_) {
+ClientOption &ClientOption::withDots(int dots_) {
   dots = dots_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withNohead(bool nohead_) {
+ClientOption &ClientOption::withNohead(bool nohead_) {
   nohead = nohead_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withMinScore(int minScore_) {
+ClientOption &ClientOption::withMinScore(int minScore_) {
   minScore = minScore_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withMinIdentity(double minIdentity_) {
+ClientOption &ClientOption::withMinIdentity(double minIdentity_) {
   minIdentity = minIdentity_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withOutputFormat(const std::string &outputFormat_) {
+ClientOption &ClientOption::withOutputFormat(const std::string &outputFormat_) {
   outputFormat = outputFormat_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withMaxIntron(long maxIntron_) {
+ClientOption &ClientOption::withMaxIntron(long maxIntron_) {
   maxIntron = maxIntron_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withGenome(const std::string &genome_) {
+ClientOption &ClientOption::withGenome(const std::string &genome_) {
   genome = genome_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withGenomeDataDir(const std::string &genomeDataDir_) {
+ClientOption &ClientOption::withGenomeDataDir(const std::string &genomeDataDir_) {
   genomeDataDir = genomeDataDir_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withIsDynamic(bool isDynamic_) {
+ClientOption &ClientOption::withIsDynamic(bool isDynamic_) {
   isDynamic = isDynamic_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withSeqDir(const std::string &SeqDir_) {
+ClientOption &ClientOption::withSeqDir(const std::string &SeqDir_) {
   SeqDir = SeqDir_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withInName(const std::string &inName_) {
+ClientOption &ClientOption::withInName(const std::string &inName_) {
   inName = inName_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withOutName(const std::string &outName_) {
+ClientOption &ClientOption::withOutName(const std::string &outName_) {
   outName = outName_;
   return *this;
 }
 
-gfClientOption &gfClientOption::withInSeq(const std::string &inseq_) {
+ClientOption &ClientOption::withInSeq(const std::string &inseq_) {
   inSeq = inseq_;
   return *this;
 }
 
-std::string gfClientOption::to_string() const {
+std::string ClientOption::to_string() const {
   std::ostringstream ret{};
 
-  ret << "gfClientOption(";
+  ret << "ClientOption(";
   ret << "hostName=" << hostName;
   ret << ", portName=" << portName;
   ret << ", tType=" << tType;
   ret << ", qType=" << qType;
   ret << ", dots=" << dots;
   ret << ", nohead=" << std::boolalpha << nohead;
   ret << ", minScore=" << minScore;
@@ -419,13 +419,13 @@
   ret << ", inName=" << inName;
   ret << ", outName=" << outName;
   ret << ")";
 
   return ret.str();
 }
 
-std::ostream &operator<<(std::ostream &os, const gfClientOption &option) {
+std::ostream &operator<<(std::ostream &os, const ClientOption &option) {
   os << option.to_string();
   return os;
 }
 
 }  // namespace cppbinding
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/gfClient.hpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/gfClient.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 // char *qType = "dna";
 // char *tType = "dna";
 // char *genome = NULL;
 // char *genomeDataDir = NULL;
 // boolean isDynamic = FALSE;
 // long enterMainTime = 0;
 
-struct gfClientOption {
+struct ClientOption {
   std::string hostName{};
   std::string portName{};
 
   std::string tType{"dna"};
   std::string qType{"dna"};
   int dots{0};
   bool nohead{false};
@@ -86,40 +86,40 @@
 
   std::string SeqDir{};
   std::string inName{};
   std::string outName{};
 
   std::string inSeq{};
 
-  gfClientOption() = default;
+  ClientOption() = default;
 
-  gfClientOption &build();
+  ClientOption &build();
 
-  gfClientOption &withHost(const std::string &hostName_);
-  gfClientOption &withPort(const std::string &portName_);
+  ClientOption &withHost(const std::string &hostName_);
+  ClientOption &withPort(const std::string &portName_);
 
-  gfClientOption &withTType(const std::string &tType_);
-  gfClientOption &withQType(const std::string &qType_);
-  gfClientOption &withDots(int dots_);
-  gfClientOption &withNohead(bool nohead_);
-  gfClientOption &withMinScore(int minScore_);
-  gfClientOption &withMinIdentity(double minIdentity_);
-  gfClientOption &withOutputFormat(const std::string &outputFormat_);
-  gfClientOption &withMaxIntron(long maxIntron_);
-  gfClientOption &withGenome(const std::string &genome_);
-  gfClientOption &withGenomeDataDir(const std::string &genomeDataDir_);
-  gfClientOption &withIsDynamic(bool isDynamic_);
-  gfClientOption &withSeqDir(const std::string &SeqDir_);
-  gfClientOption &withInName(const std::string &inName_);
-  gfClientOption &withOutName(const std::string &outName_);
-  gfClientOption &withInSeq(const std::string &inseq_);
+  ClientOption &withTType(const std::string &tType_);
+  ClientOption &withQType(const std::string &qType_);
+  ClientOption &withDots(int dots_);
+  ClientOption &withNohead(bool nohead_);
+  ClientOption &withMinScore(int minScore_);
+  ClientOption &withMinIdentity(double minIdentity_);
+  ClientOption &withOutputFormat(const std::string &outputFormat_);
+  ClientOption &withMaxIntron(long maxIntron_);
+  ClientOption &withGenome(const std::string &genome_);
+  ClientOption &withGenomeDataDir(const std::string &genomeDataDir_);
+  ClientOption &withIsDynamic(bool isDynamic_);
+  ClientOption &withSeqDir(const std::string &SeqDir_);
+  ClientOption &withInName(const std::string &inName_);
+  ClientOption &withOutName(const std::string &outName_);
+  ClientOption &withInSeq(const std::string &inseq_);
 
   std::string to_string() const;
-  friend std::ostream &operator<<(std::ostream &os, const gfClientOption &option);
+  friend std::ostream &operator<<(std::ostream &os, const ClientOption &option);
 };
 
-std::string pygfClient_no_gil(gfClientOption option);
-std::string pygfClient(gfClientOption &option);
+std::string pygfClient_no_gil(ClientOption option);
+std::string pygfClient(ClientOption &option);
 std::string read_inmem_file(FILE *file);
 }  // namespace cppbinding
 
 #endif
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/gfServer.cpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/gfServer.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 // long baseCount = 0, blatCount = 0, aaCount = 0, pcrCount = 0;
 // int warnCount = 0;
 // int noSigCount = 0;
 // int missCount = 0;
 // int trimCount = 0;
 
 void dnaQuery(struct genoFind *gf, struct dnaSeq *seq, int connectionHandle, struct hash *perSeqMaxHash,
-              gfServerOption const &options, UsageStats &stats, boolean &sendOk)
+              ServerOption const &options, UsageStats &stats, boolean &sendOk)
 /* Handle a query for DNA/DNA match. */
 {
   auto maxDnaHits = options.maxDnaHits;
 
   char buf[256];
   struct gfClump *clumpList = NULL, *clump;
   int limit = 1000;
@@ -134,15 +134,15 @@
   lmCleanup(&lm);
   logDebug("%lu %d clumps, %d hits", clock1000(), clumpCount, hitCount);
 
   dbg(clumpCount);
   dbg(hitCount);
 }
 
-void transQuery(struct genoFind *transGf[2][3], aaSeq *seq, int connectionHandle, gfServerOption const &options,
+void transQuery(struct genoFind *transGf[2][3], aaSeq *seq, int connectionHandle, ServerOption const &options,
                 UsageStats &stats, boolean &sendOk)
 /* Handle a query for protein/translated DNA match. */
 {
   auto tileSize = options.tileSize;
   auto maxTransHits = options.maxTransHits;
 
   char buf[256];
@@ -181,15 +181,15 @@
   if (clumpCount == 0) ++stats.missCount;
   dyStringFree(&dy);
   lmCleanup(&lm);
   logDebug("%lu %d clumps, %d hits", clock1000(), clumpCount, hitCount);
 }
 
 void transTransQuery(struct genoFind *transGf[2][3], struct dnaSeq *seq, int connectionHandle,
-                     gfServerOption const &options, UsageStats &stats, boolean &sendOk)
+                     ServerOption const &options, UsageStats &stats, boolean &sendOk)
 /* Handle a query for protein/translated DNA match. */
 {
   auto tileSize = options.tileSize;
   auto maxTransHits = options.maxTransHits;
 
   char buf[256];
   struct gfClump *clumps[3][3], *clump;
@@ -297,15 +297,15 @@
 {
   errorSafeCleanup();
   logError("Recovering from error via longjmp");
   errSendString(connectionHandle, message, sendOk);
 }
 
 void errorSafeQuery(boolean doTrans, boolean queryIsProt, struct dnaSeq *seq, struct genoFindIndex *gfIdx,
-                    int connectionHandle, char *buf, struct hash *perSeqMaxHash, gfServerOption const &options,
+                    int connectionHandle, char *buf, struct hash *perSeqMaxHash, ServerOption const &options,
                     UsageStats &stats, boolean &sendOk)
 /* Wrap error handling code around index query. */
 {
   int status;
   errorSafeSetup();
   status = setjmp(gfRecover);
   if (status == 0) /* Always true except after long jump. */
@@ -381,15 +381,15 @@
                     copy);
     hashAddInt(perSeqMaxHash, seqFile, 0);
   }
   lineFileClose(&lf);
   return perSeqMaxHash;
 }
 
-struct hash *maybePerSeqMax(int fileCount, char *seqFiles[], gfServerOption &options)
+struct hash *maybePerSeqMax(int fileCount, char *seqFiles[], ServerOption &options)
 /* If options include -perSeqMax=file, then read the sequences named in the file
  * into a hash for testing membership in the set of sequences to exclude from
  * -maxDnaHits accounting. */
 {
   // char *fileName = optionVal("perSeqMax", NULL);
   char *fileName = options.perSeqMax.empty() ? NULL : options.perSeqMax.data();
 
@@ -403,15 +403,15 @@
 /* Set the value of every element of hash to NULL (0 for ints). */
 {
   struct hashEl *hel;
   struct hashCookie cookie = hashFirst(hash);
   while ((hel = hashNext(&cookie)) != NULL) hel->val = 0;
 }
 
-void checkIndexFileName(char *gfxFile, char *seqFile, gfServerOption const &options)
+void checkIndexFileName(char *gfxFile, char *seqFile, ServerOption const &options)
 /* validate that index matches conventions, as base name is stored in index */
 {
   boolean doTrans = bool2boolean(options.trans);
 
   char seqBaseName[FILENAME_LEN], seqExt[FILEEXT_LEN];
   splitPath(seqFile, NULL, seqBaseName, seqExt);
   if ((strlen(seqBaseName) == 0) || !sameString(seqExt, ".2bit"))
@@ -448,15 +448,15 @@
 {
   boolean isTrans;              // translated
   char genome[256];             // genome name
   struct hash *perSeqMaxHash;   // max hits per sequence
   struct genoFindIndex *gfIdx;  // index
 };
 
-struct genoFindIndex *loadGfIndex(char *gfIdxFile, boolean isTrans, gfServerOption &options)
+struct genoFindIndex *loadGfIndex(char *gfIdxFile, boolean isTrans, ServerOption &options)
 /* load index and set globals from it */
 {
   struct genoFindIndex *gfIdx = genoFindIndexLoad(gfIdxFile, isTrans);
   struct genoFind *gf = isTrans ? gfIdx->transGf[0][0] : gfIdx->untransGf;
 
   // minMatch = gf->minMatch;
   // maxGap = gf->maxGap;
@@ -481,15 +481,15 @@
 {
   logErrorVa(format, args);
   vfprintf(stderr, format, args);
   fputc('\n', stderr);
 }
 
 void dynSessionInit(struct dynSession *dynSession, char *rootDir, char *genome, char *genomeDataDir, boolean isTrans,
-                    gfServerOption &options)
+                    ServerOption &options)
 /* Initialize or reinitialize a dynSession object */
 {
   if ((!isSafeRelativePath(genome)) || (strchr(genome, '/') != NULL))
     errAbort("genome argument can't contain '/' or '..': %s", genome);
   if (!isSafeRelativePath(genomeDataDir))
     errAbort(
         "genomeDataDir argument must be a relative path without '..' "
@@ -540,15 +540,15 @@
   char *cmd = cloneString(buf + strlen(gfSignature()));
   logInfo("dynserver: %s", cmd);
   return cmd;
 }
 
 // static const int DYN_CMD_MAX_ARGS = 8;  // more than needed to check for junk
 
-int dynNextCommand(char *rootDir, struct dynSession *dynSession, char **args, gfServerOption &options)
+int dynNextCommand(char *rootDir, struct dynSession *dynSession, char **args, ServerOption &options)
 /* Read query request from stdin and (re)initialize session to match
  * parameters.  Return number of arguments or zero on EOF
  *
  * Commands are in the format:
  *  signature+command genome genomeDataDir [arg ...]
  *  signature+status
  */
@@ -567,15 +567,15 @@
 
   // initialize session if new or changed
   if ((dynSession->isTrans != isTrans) || (!sameString(dynSession->genome, args[1])))
     dynSessionInit(dynSession, rootDir, args[1], args[2], isTrans, options);
   return numArgs;
 }
 
-struct dnaSeq *dynReadQuerySeq(int qSize, boolean isTrans, boolean queryIsProt, gfServerOption const &options)
+struct dnaSeq *dynReadQuerySeq(int qSize, boolean isTrans, boolean queryIsProt, ServerOption const &options)
 /* read the DNA sequence from the query, filtering junk  */
 {
   auto maxAaSize = options.maxAaSize;
   auto maxNtSize = options.maxNtSize;
 
   struct dnaSeq *seq;
   // AllocVar(seq);
@@ -597,15 +597,15 @@
     seq->size = maxSize;
     seq->dna[maxSize] = 0;
   }
 
   return seq;
 }
 
-void dynamicServerQuery(struct dynSession *dynSession, int numArgs, char **args, gfServerOption const &options,
+void dynamicServerQuery(struct dynSession *dynSession, int numArgs, char **args, ServerOption const &options,
                         UsageStats &stats, boolean &sendOk)
 /* handle search queries
  *
  *  signature+command genome genomeDataDir qsize
  */
 {
   struct genoFindIndex *gfIdx = dynSession->gfIdx;
@@ -678,15 +678,15 @@
   char *fPrimer = args[3];
   char *rPrimer = args[4];
   int maxDistance = atoi(args[5]);
   if (badPcrPrimerSeq(fPrimer) || badPcrPrimerSeq(rPrimer)) errAbort("Can only handle ACGT in primer sequences.");
   pcrQuery(gfIdx->untransGf, fPrimer, rPrimer, maxDistance, STDOUT_FILENO, sendOk);
 }
 
-bool dynamicServerCommand(char *rootDir, struct dynSession *dynSession, gfServerOption &options, UsageStats &stats,
+bool dynamicServerCommand(char *rootDir, struct dynSession *dynSession, ServerOption &options, UsageStats &stats,
                           boolean &sendOk)
 /* Execute one command from stdin, (re)initializing session as needed */
 {
   const int DYN_CMD_MAX_ARGS = 8;  // more than needed to check for junk
 
   time_t startTime = clock1000();
   char *args[DYN_CMD_MAX_ARGS];
@@ -704,15 +704,15 @@
     errAbort("invalid command '%s'", args[0]);
 
   logInfo("dynserver: %s completed in %4.3f seconds", args[0], 0.001 * (clock1000() - startTime));
   freeMem(args[0]);
   return TRUE;
 }
 
-void gfServer(gfServerOption &options)
+void gfServer(ServerOption &options)
 /* Process command line. */
 {
   char *command;
 
   gfCatchPipes();
   dnaUtilOpen();
 
@@ -806,15 +806,15 @@
     // usage(options);
     printf("usage\n");
   }
 }
 
 // cpp implementation
 void genoFindDirect(std::string &probeName, int fileCount, std::vector<std::string> &seqFiles,
-                    gfServerOption const &options)
+                    ServerOption const &options)
 /* Don't set up server - just directly look for matches. */
 {
   auto minMatch = options.minMatch;
   auto maxGap = options.maxGap;
   auto tileSize = options.tileSize;
   auto repMatch = options.repMatch;
   auto stepSize = options.stepSize;
@@ -853,15 +853,15 @@
     lmCleanup(&lm);
   }
   lineFileClose(&lf);
   genoFindFree(&gf);
 }
 
 void genoPcrDirect(std::string &fPrimer, std::string &rPrimer, int fileCount, std::vector<std::string> &seqFiles,
-                   gfServerOption const &options) {
+                   ServerOption const &options) {
   auto minMatch = options.minMatch;
   auto maxGap = options.maxGap;
   auto tileSize = options.tileSize;
   auto repMatch = options.repMatch;
   auto stepSize = options.stepSize;
 
   boolean allowOneMismatch = bool2boolean(options.allowOneMismatch);
@@ -910,15 +910,15 @@
     gfClumpDump(gf, clump, stdout);
   }
 
   genoFindFree(&gf);
 }
 
 genoFindIndex *pybuildIndex4Server(std::string &hostName, std::string &portName, int fileCount, char *seqFiles[],
-                                   hash *perSeqMaxHash, gfServerOption &option) {
+                                   hash *perSeqMaxHash, ServerOption &option) {
   auto indexFile = option.indexFile.empty() ? NULL : option.indexFile.data();
 
   // auto ipLog = option.ipLog;
   auto minMatch = option.minMatch;
   auto maxGap = option.maxGap;
   auto tileSize = option.tileSize;
   auto repMatch = option.repMatch;
@@ -962,15 +962,15 @@
     logInfo("index loading completed in %4.3f seconds", 0.001 * (clock1000() - startIndexTime));
   }
   logGenoFindIndex(gfIdx);
   return gfIdx;
 }
 // void startServer(char *hostName, char *portName, int fileCount, char *seqFiles[])
 void startServer(std::string &hostName, std::string &portName, int fileCount, std::vector<std::string> &seqFiles,
-                 gfServerOption &options, UsageStats &stats)
+                 ServerOption &options, UsageStats &stats)
 /* Load up index and hang out in RAM. */
 {
   auto indexFile = options.indexFile.empty() ? NULL : options.indexFile.data();
 
   auto ipLog = options.ipLog;
   auto minMatch = options.minMatch;
   auto maxGap = options.maxGap;
@@ -1373,15 +1373,15 @@
     } else {
       printf("%s\n", buf);
     }
   }
   close(sd);
 }
 
-std::string pystatusServer(std::string &hostName, std::string &portName, gfServerOption &options)
+std::string pystatusServer(std::string &hostName, std::string &portName, ServerOption &options)
 /* Send status message to server arnd report result. */
 {
   auto ret_str = std::ostringstream{};
   auto genome = options.genome.empty() ? NULL : options.genome.data();
   auto genomeDataDir = options.genomeDataDir.empty() ? NULL : options.genomeDataDir.data();
   boolean doTrans = bool2boolean(options.trans);
 
@@ -1409,15 +1409,15 @@
     else
       ret_str << buf << "\n";
   }
   close(sd);
   return ret_str.str();
 }
 
-int statusServer(std::string &hostName, std::string &portName, gfServerOption &options)
+int statusServer(std::string &hostName, std::string &portName, ServerOption &options)
 /* Send status message to server arnd report result. */
 {
   auto genome = options.genome.empty() ? NULL : options.genome.data();
   auto genomeDataDir = options.genomeDataDir.empty() ? NULL : options.genomeDataDir.data();
   boolean doTrans = bool2boolean(options.trans);
 
   char buf[256];
@@ -1494,15 +1494,15 @@
     for (i = 0; i < fileCount; ++i) {
       printf("%s\n", netRecieveString(sd, buf));
     }
   }
   close(sd);
 }
 
-void buildIndex(std::string &gfxFile, int fileCount, std::vector<std::string> seqFiles, gfServerOption const &options)
+void buildIndex(std::string &gfxFile, int fileCount, std::vector<std::string> seqFiles, ServerOption const &options)
 /* build pre-computed index for seqFiles and write to gfxFile */
 {
   auto minMatch = options.minMatch;
   auto maxGap = options.maxGap;
   auto tileSize = options.tileSize;
   auto repMatch = options.repMatch;
   auto stepSize = options.stepSize;
@@ -1522,15 +1522,15 @@
   checkIndexFileName(gfxFile.data(), cseqFiles.front(), options);
 
   struct genoFindIndex *gfIdx = genoFindIndexBuild(fileCount, cseqFiles.data(), minMatch, maxGap, tileSize, repMatch,
                                                    doTrans, NULL, allowOneMismatch, doMask, stepSize, noSimpRepMask);
   genoFindIndexWrite(gfIdx, gfxFile.data());
 }
 
-void dynamicServer(std::string &rootDir, gfServerOption &options, UsageStats &stats, boolean &sendOk)
+void dynamicServer(std::string &rootDir, ServerOption &options, UsageStats &stats, boolean &sendOk)
 /* dynamic server for inetd. Read query from stdin, open index, query, respond,
  * exit. only one query at a time */
 {
   pushWarnHandler(dynWarnHandler);
   logDebug("dynamicServer connect");
   struct runTimes startTimes = getTimesInSeconds();
 
@@ -1545,15 +1545,15 @@
   logInfo("dynserver: exit: clock: %0.4f user: %0.4f system: %0.4f (seconds)",
           endTimes.clockSecs - startTimes.clockSecs, endTimes.userSecs - startTimes.userSecs,
           endTimes.sysSecs - startTimes.sysSecs);
 
   logDebug("dynamicServer disconnect");
 }
 
-gfServerOption &gfServerOption::build() {
+ServerOption &ServerOption::build() {
   if (trans) {
     tileSize = 4;
     stepSize = tileSize;
     minMatch = 3;
     maxGap = 0;
     repMatch = gfPepMaxTileUse;
   }
@@ -1562,132 +1562,132 @@
     repMatch = gfDefaultRepMatch(tileSize, stepSize, bool2boolean(trans));
   else
     repMatch = 0;
 
   return *this;
 }
 
-gfServerOption &gfServerOption::withCanStop(bool canStop_) {
+ServerOption &ServerOption::withCanStop(bool canStop_) {
   canStop = canStop_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withLog(std::string log_) {
+ServerOption &ServerOption::withLog(std::string log_) {
   log = std::move(log_);
   return *this;
 }
 
-gfServerOption &gfServerOption::withLogFacility(std::string logFacility_) {
+ServerOption &ServerOption::withLogFacility(std::string logFacility_) {
   logFacility = std::move(logFacility_);
   return *this;
 }
 
-gfServerOption &gfServerOption::withMask(bool mask_) {
+ServerOption &ServerOption::withMask(bool mask_) {
   mask = mask_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withMaxAaSize(int maxAaSize_) {
+ServerOption &ServerOption::withMaxAaSize(int maxAaSize_) {
   maxAaSize = maxAaSize_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withMaxDnaHits(int maxDnaHits_) {
+ServerOption &ServerOption::withMaxDnaHits(int maxDnaHits_) {
   maxDnaHits = maxDnaHits_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withMaxGap(int maxGap_) {
+ServerOption &ServerOption::withMaxGap(int maxGap_) {
   maxGap = maxGap_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withMaxNtSize(int maxNtSize_) {
+ServerOption &ServerOption::withMaxNtSize(int maxNtSize_) {
   maxNtSize = maxNtSize_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withMaxTransHits(int maxTransHits_) {
+ServerOption &ServerOption::withMaxTransHits(int maxTransHits_) {
   maxTransHits = maxTransHits_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withMinMatch(int minMatch_) {
+ServerOption &ServerOption::withMinMatch(int minMatch_) {
   minMatch = minMatch_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withRepMatch(int repMatch_) {
+ServerOption &ServerOption::withRepMatch(int repMatch_) {
   repMatch = repMatch_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withSeqLog(bool seqLog_) {
+ServerOption &ServerOption::withSeqLog(bool seqLog_) {
   seqLog = seqLog_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withIpLog(bool ipLog_) {
+ServerOption &ServerOption::withIpLog(bool ipLog_) {
   ipLog = ipLog_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withDebugLog(bool debugLog_) {
+ServerOption &ServerOption::withDebugLog(bool debugLog_) {
   debugLog = debugLog_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withTileSize(int tileSize_) {
+ServerOption &ServerOption::withTileSize(int tileSize_) {
   tileSize = tileSize_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withStepSize(int stepSize_) {
+ServerOption &ServerOption::withStepSize(int stepSize_) {
   stepSize = stepSize_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withTrans(bool trans_) {
+ServerOption &ServerOption::withTrans(bool trans_) {
   trans = trans_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withSyslog(bool syslog_) {
+ServerOption &ServerOption::withSyslog(bool syslog_) {
   syslog = syslog_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withPerSeqMax(std::string perSeqMax_) {
+ServerOption &ServerOption::withPerSeqMax(std::string perSeqMax_) {
   perSeqMax = std::move(perSeqMax_);
   return *this;
 }
 
-gfServerOption &gfServerOption::withNoSimpRepMask(bool noSimpRepMask_) {
+ServerOption &ServerOption::withNoSimpRepMask(bool noSimpRepMask_) {
   noSimpRepMask = noSimpRepMask_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withIndexFile(std::string indexFile_) {
+ServerOption &ServerOption::withIndexFile(std::string indexFile_) {
   indexFile = std::move(indexFile_);
   return *this;
 }
 
-gfServerOption &gfServerOption::withTimeout(int timeout_) {
+ServerOption &ServerOption::withTimeout(int timeout_) {
   timeout = timeout_;
   return *this;
 }
 
-gfServerOption &gfServerOption::withThreads(int threads_) {
+ServerOption &ServerOption::withThreads(int threads_) {
   threads = threads_;
   return *this;
 }
 
-std::string gfServerOption::to_string() const {
+std::string ServerOption::to_string() const {
   std::stringstream s{};
-  s << "gfServerOption(";
+  s << "ServerOption(";
   s << "canStop: " << std::boolalpha << canStop;
   s << ", log: " << log;
   s << ", logFacility: " << logFacility;
   s << ", mask: " << mask;
   s << ", maxAaSize: " << maxAaSize;
   s << ", maxDnaHits: " << maxDnaHits;
   s << ", maxGap: " << maxGap;
@@ -1710,15 +1710,15 @@
   s << ", genomeDataDir: " << genomeDataDir;
   s << ", threads: " << threads;
   s << ", allowOneMismatch: " << std::boolalpha << allowOneMismatch << ")";
 
   return s.str();
 }
 
-std::ostream &operator<<(std::ostream &os, const gfServerOption &option) {
+std::ostream &operator<<(std::ostream &os, const ServerOption &option) {
   os << option.to_string();
   return os;
 }
 
 std::ostream &operator<<(std::ostream &os, const UsageStats &stats) {
   os << "UsageStats(";
   os << "baseCount: " << stats.baseCount;
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/gfServer.hpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/gfServer.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -70,16 +70,16 @@
 // char *genomeDataDir = NULL;
 
 // constexpr int timeout = 90;  // default timeout in seconds
 
 // {self.gfserver} -canStop -log={self.log_file_path} -stepSize=5 start "
 //             f"localhost {self.port} {os.path.basename(self.ref_2bit)}"
 
-struct gfServerOption {
-  using self = gfServerOption;
+struct ServerOption {
+  using self = ServerOption;
   bool canStop{false};        //-canStop      If set, a quit message will actually take down the server.
   std::string log{};          //-log=logFile  Keep a log file that records server requests.
   std::string logFacility{};  //-logFacility=facility  Log to the specified syslog facility default local0
   bool mask{};                //-mask   Use masking from .2bit file.
   int maxAaSize{8000};        //-maxAaSize=N  Maximum size of protein or translated DNA queries."
   int maxDnaHits{100};        //-maxDnaHits=N   Maximum number of hits for a DNA query that are sent from the server"
   int maxGap{gfMaxGap};       //-maxGap=N    Number of insertions or deletions allowed between n-mers. Default is 2 for
@@ -110,139 +110,139 @@
   int timeout{90};              //-timeout=N  Timeout in seconds
   std::string genome{};         // no need to get
   std::string genomeDataDir{};  // no need to get
 
   int threads{1};
   bool allowOneMismatch{false};
 
-  gfServerOption() = default;
+  ServerOption() = default;
   self &build();
 
   std::string to_string() const;
 
-  gfServerOption &withCanStop(bool canStop_);
-  gfServerOption &withLogFacility(std::string logFacility_);
-  gfServerOption &withLog(std::string log_);
-  gfServerOption &withMask(bool mask_);
-  gfServerOption &withMaxAaSize(int maxAaSize_);
-  gfServerOption &withMaxDnaHits(int maxDnaHits_);
-  gfServerOption &withMaxGap(int maxGap_);
-  gfServerOption &withMaxNtSize(int maxNtSize_);
-  gfServerOption &withMaxTransHits(int maxTransHits_);
-  gfServerOption &withMinMatch(int minMatch_);
-  gfServerOption &withRepMatch(int repMatch_);
-  gfServerOption &withSeqLog(bool seqLog_);
-  gfServerOption &withIpLog(bool ipLog_);
-  gfServerOption &withDebugLog(bool debugLog_);
-  gfServerOption &withTileSize(int tileSize_);
-  gfServerOption &withStepSize(int stepSize_);
-  gfServerOption &withTrans(bool trans_);
-  gfServerOption &withSyslog(bool syslog_);
-  gfServerOption &withPerSeqMax(std::string perSeqMax_);
-  gfServerOption &withNoSimpRepMask(bool noSimpRepMask_);
-  gfServerOption &withIndexFile(std::string indexFile_);
-  gfServerOption &withTimeout(int timeout_);
-  gfServerOption &withThreads(int threads_);
+  ServerOption &withCanStop(bool canStop_);
+  ServerOption &withLogFacility(std::string logFacility_);
+  ServerOption &withLog(std::string log_);
+  ServerOption &withMask(bool mask_);
+  ServerOption &withMaxAaSize(int maxAaSize_);
+  ServerOption &withMaxDnaHits(int maxDnaHits_);
+  ServerOption &withMaxGap(int maxGap_);
+  ServerOption &withMaxNtSize(int maxNtSize_);
+  ServerOption &withMaxTransHits(int maxTransHits_);
+  ServerOption &withMinMatch(int minMatch_);
+  ServerOption &withRepMatch(int repMatch_);
+  ServerOption &withSeqLog(bool seqLog_);
+  ServerOption &withIpLog(bool ipLog_);
+  ServerOption &withDebugLog(bool debugLog_);
+  ServerOption &withTileSize(int tileSize_);
+  ServerOption &withStepSize(int stepSize_);
+  ServerOption &withTrans(bool trans_);
+  ServerOption &withSyslog(bool syslog_);
+  ServerOption &withPerSeqMax(std::string perSeqMax_);
+  ServerOption &withNoSimpRepMask(bool noSimpRepMask_);
+  ServerOption &withIndexFile(std::string indexFile_);
+  ServerOption &withTimeout(int timeout_);
+  ServerOption &withThreads(int threads_);
 
   friend std::ostream &operator<<(std::ostream &os, const self &option);
 };
 
-void gfServer(gfServerOption &options);
+void gfServer(ServerOption &options);
 bool boolean2bool(boolean b);
 
 boolean bool2boolean(bool b);
 
 void setSendOk(boolean &sendOk);
 void errSendString(int sd, char *s, boolean &sendOk);
 void errSendLongString(int sd, char *s, boolean &sendOk);
 void logGenoFind(struct genoFind *gf);
 void logGenoFindIndex(struct genoFindIndex *gfIdx);
 
 // void genoFindDirect(char *probeName, int fileCount, char *seqFiles[]);
 void genoFindDirect(std::string &probeName, int fileCount, std::vector<std::string> &seqFiles,
-                    gfServerOption const &options);
+                    ServerOption const &options);
 
 // void genoPcrDirect(char *fPrimer, char *rPrimer, int fileCount, char *seqFiles[]);
 void genoPcrDirect(std::string &fPrimer, std::string &rPrimer, int fileCount, std::vector<std::string> &seqFiles,
-                   gfServerOption const &options);
+                   ServerOption const &options);
 
 /* Load up index and hang out in RAM. */
 // void startServer(char *hostName, char *portName, int fileCount, char *seqFiles[]);
 void startServer(std::string &hostName, std::string &portName, int fileCount, std::vector<std::string> &seqFiles,
-                 gfServerOption &options, UsageStats &stats);
+                 ServerOption &options, UsageStats &stats);
 
 // void stopServer(char *hostName, char *portName);
 void stopServer(std::string &hostName, std::string &portName);
 
 // void queryServer(char *type, char *hostName, char *portName, char *faName, boolean complex, boolean isProt);
 void queryServer(std::string &type, std::string &hostName, std::string &portName, std::string &faName, bool complex,
                  bool isProt);
 
 /* Do a PCR query to server daemon. */
 // void pcrServer(char *hostName, char *portName, char *fPrimer, char *rPrimer, int maxSize);
 void pcrServer(std::string &hostName, std::string &portName, std::string &fPrimer, std::string &rPrimer, int maxSize);
 
 // int statusServer(char *hostName, char *portName);
-int statusServer(std::string &hostName, std::string &portName, gfServerOption &options);
+int statusServer(std::string &hostName, std::string &portName, ServerOption &options);
 
 // void getFileList(char *hostName, char *portName);
 void getFileList(std::string &hostName, std::string &portName);
 
 // build pre-computed index for seqFiles and write to
 // void buildIndex(char *gfxFile, int fileCount, char *seqFiles[]);
-void buildIndex(std::string &gfxFile, int fileCount, std::vector<std::string> seqFiles, gfServerOption const &options);
+void buildIndex(std::string &gfxFile, int fileCount, std::vector<std::string> seqFiles, ServerOption const &options);
 
 int getPortIx(char *portName);
 
 /* Handle a query for DNA/DNA match. */
 // void dnaQuery(struct genoFind *gf, struct dnaSeq *seq, int connectionHandle, struct hash *perSeqMaxHash);
 void dnaQuery(struct genoFind *gf, struct dnaSeq *seq, int connectionHandle, struct hash *perSeqMaxHash,
-              gfServerOption const &options, UsageStats &stats, boolean &sendOk);
+              ServerOption const &options, UsageStats &stats, boolean &sendOk);
 
 // void transQuery(struct genoFind *transGf[2][3], aaSeq *seq, int connectionHandle);
-void transQuery(struct genoFind *transGf[2][3], aaSeq *seq, int connectionHandle, gfServerOption const &options,
+void transQuery(struct genoFind *transGf[2][3], aaSeq *seq, int connectionHandle, ServerOption const &options,
                 UsageStats &stats, boolean &sendOk);
 
 // void transTransQuery(struct genoFind *transGf[2][3], struct dnaSeq *seq, int connectionHandle);
 void transTransQuery(struct genoFind *transGf[2][3], struct dnaSeq *seq, int connectionHandle,
-                     gfServerOption const &options, UsageStats &stats, boolean &sendOk);
+                     ServerOption const &options, UsageStats &stats, boolean &sendOk);
 
 void errorSafeQuery(boolean doTrans, boolean queryIsProt, struct dnaSeq *seq, struct genoFindIndex *gfIdx,
-                    int connectionHandle, char *buf, struct hash *perSeqMaxHash, gfServerOption const &options,
+                    int connectionHandle, char *buf, struct hash *perSeqMaxHash, ServerOption const &options,
                     UsageStats &stats, boolean &sendOk);
 
-void checkIndexFileName(char *gfxFile, char *seqFile, gfServerOption const &options);
+void checkIndexFileName(char *gfxFile, char *seqFile, ServerOption const &options);
 
-struct genoFindIndex *loadGfIndex(char *gfIdxFile, boolean isTrans, gfServerOption &options);
+struct genoFindIndex *loadGfIndex(char *gfIdxFile, boolean isTrans, ServerOption &options);
 void dynSessionInit(struct dynSession *dynSession, char *rootDir, char *genome, char *genomeDataDir, boolean isTrans,
-                    gfServerOption &options);
-int dynNextCommand(char *rootDir, struct dynSession *dynSession, char **args, gfServerOption &options);
+                    ServerOption &options);
+int dynNextCommand(char *rootDir, struct dynSession *dynSession, char **args, ServerOption &options);
 
 /* NOTE: will change options' value <05-03-23, Yangyang Li yangyang.li@northwestern.edu> */
-bool dynamicServerCommand(char *rootDir, struct dynSession *dynSession, gfServerOption &options, UsageStats &stats,
+bool dynamicServerCommand(char *rootDir, struct dynSession *dynSession, ServerOption &options, UsageStats &stats,
                           boolean &sendOk);
-void dynamicServer(std::string &rootDir, gfServerOption &options, UsageStats &stats, boolean &sendOk);
+void dynamicServer(std::string &rootDir, ServerOption &options, UsageStats &stats, boolean &sendOk);
 
-struct dnaSeq *dynReadQuerySeq(int qSize, boolean isTrans, boolean queryIsProt, gfServerOption const &options);
+struct dnaSeq *dynReadQuerySeq(int qSize, boolean isTrans, boolean queryIsProt, ServerOption const &options);
 
-void dynamicServerQuery(struct dynSession *dynSession, int numArgs, char **args, gfServerOption const &options,
+void dynamicServerQuery(struct dynSession *dynSession, int numArgs, char **args, ServerOption const &options,
                         UsageStats &stats, boolean &sendOk);
 
-struct hash *maybePerSeqMax(int fileCount, char *seqFiles[], gfServerOption &options);
+struct hash *maybePerSeqMax(int fileCount, char *seqFiles[], ServerOption &options);
 boolean badPcrPrimerSeq(char *s);
 
 void setSocketTimeout(int sockfd, int delayInSeconds);
 void hashZeroVals(struct hash *hash);
 void errorSafePcr(struct genoFind *gf, char *fPrimer, char *rPrimer, int maxDistance, int connectionHandle,
                   boolean &sendOk);
 
 genoFindIndex *pybuildIndex4Server(std::string &hostName, std::string &portName, int fileCount, char *seqFiles[],
-                                   hash *perSeqMaxHash, gfServerOption &option);
+                                   hash *perSeqMaxHash, ServerOption &option);
 
-std::string pystatusServer(std::string &hostName, std::string &portName, gfServerOption &options);
+std::string pystatusServer(std::string &hostName, std::string &portName, ServerOption &options);
 std::string pygetFileList(std::string &hostName, std::string &portName);
 std::string pyqueryServer(std::string &type, std::string &hostName, std::string &portName, std::string &faName,
                           bool complex, bool isProt);
 
 void test_stdout();
 void test_add(int &a);
 void test_stat(UsageStats &stats);
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/pygfServer.cpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/pygfServer.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #include "dbg.h"
 #include "gfServer.hpp"
 #include "pygfServer.hpp"
 
 namespace cppbinding {
 
 void pyerrorSafeQuery(boolean doTrans, boolean queryIsProt, struct dnaSeq *seq, struct genoFindIndex *gfIdx,
-                      int connectionHandle, char *buf, struct hash *perSeqMaxHash, gfServerOption const &options,
+                      int connectionHandle, char *buf, struct hash *perSeqMaxHash, ServerOption const &options,
                       UsageStats &stats, boolean &sendOk)
 /* Wrap error handling code around index query. */
 {
   // status = setjmp(gfRecover);
   // if (status == 0) /* Always true except after long jump. */
   // {
   if (doTrans) {
@@ -56,15 +56,15 @@
 // anything more on this connection.
 {
   if (sendOk) sendOk = pynetSendString(sd, s);
 }
 
 void handle_client(int connectionHandle, std::string hostName, std::string portName, int fileCount,
                    std::vector<std::string> const &seqFiles, hash *perSeqMaxHash, genoFindIndex *gfIdx,
-                   gfServerOption const &option) {
+                   ServerOption const &option) {
   // dbg("begin func ", connectionHandle, hostName, portName, fileCount, seqFiles, perSeqMaxHash, gfIdx, option);
 
   // print current thread id
 
   dbg("thread id: ", std::this_thread::get_id());
 
   // auto ipLog = option.ipLog;
@@ -260,15 +260,15 @@
     ++stats.warnCount;
   }
   close(connectionHandle);
   // connectionHandle = 0;
 }
 
 int pystartServer(std::string &hostName, std::string &portName, int fileCount, std::vector<std::string> &seqFiles,
-                  gfServerOption &option, UsageStats &stats) {
+                  ServerOption &option, UsageStats &stats) {
   BS::thread_pool pool(option.threads);
 
   std::vector<char *> cseqFiles{};
   cseqFiles.reserve(seqFiles.size());
   for (auto &string : seqFiles) {
     cseqFiles.push_back(string.data());
   }
@@ -284,16 +284,14 @@
 
   /* Set up socket.  Get ready to listen to it. */
   socketHandle = netAcceptingSocket(port, 100);
   if (socketHandle < 0)
     throw std::runtime_error("Fatal Error: Unable to open listening socket on port " + portName + ".");
   // errAbort("Fatal Error: Unable to open listening socket on port %d.", port);
 
-  // signal.isReady = true;
-
   int connectFailCount = 0;
   for (;;) {
     ZeroVar(&fromAddr);
     fromLen = sizeof(fromAddr);
     int connectionHandle = accept(socketHandle, (struct sockaddr *)&fromAddr, &fromLen);
 
     // setSendOk(sendOk);
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/bindings/pygfServer.hpp` & `pxblat-0.2.0/src/pxblat/extc/bindings/pygfServer.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 #define PYGF_SERVER_HPP
 
 #include "gfServer.hpp"
 
 namespace cppbinding {
 
 void pyerrorSafeQuery(boolean doTrans, boolean queryIsProt, struct dnaSeq *seq, struct genoFindIndex *gfIdx,
-                      int connectionHandle, char *buf, struct hash *perSeqMaxHash, gfServerOption const &options,
+                      int connectionHandle, char *buf, struct hash *perSeqMaxHash, ServerOption const &options,
                       UsageStats &stats, boolean &sendOk);
 
 boolean pynetSendString(int sd, char *s);
 
 void pyerrSendString(int sd, char *s, boolean &sendOk);
 
 void handle_client(int connectionHandle, std::string hostName, std::string portName, int fileCount,
                    std::vector<std::string> const &seqFiles, hash *perSeqMaxHash, genoFindIndex *gfIdx,
-                   gfServerOption const &option);
+                   ServerOption const &option);
 
 int pystartServer(std::string &hostName, std::string &portName, int fileCount, std::vector<std::string> &seqFiles,
-                  gfServerOption &options, UsageStats &stats);
+                  ServerOption &options, UsageStats &stats);
 
 }  // namespace cppbinding
 
 #endif  // !#ifndef PYGF_SERVER_HPP
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/blat.c` & `pxblat-0.2.0/src/pxblat/extc/blat.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/faToTwoBit.c` & `pxblat-0.2.0/src/pxblat/extc/faToTwoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/gfClient.c` & `pxblat-0.2.0/src/pxblat/extc/gfClient.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/gfServer.c` & `pxblat-0.2.0/src/pxblat/extc/gfServer.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/bandExt.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/bandExt.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/base64.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/base64.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/cheapcgi.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/cheapcgi.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/filePath.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/filePath.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/gfxPoly.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/gfxPoly.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/hex.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/hex.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/htmlPage.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/htmlPage.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/htmshell.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/htmshell.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/internet.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/internet.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/kxTok.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/kxTok.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/memgfx.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/memgfx.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/mime.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/mime.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/portimpl.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/portimpl.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/aux/rbTree.h` & `pxblat-0.2.0/src/pxblat/extc/include/aux/rbTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/aliType.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/aliType.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/axt.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/axt.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/bPlusTree.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/bPlusTree.h`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 #ifndef BPLUSTREE_H
 #define BPLUSTREE_H
 
 #ifdef __cplusplus
 extern "C" {
 #endif  // __cplusplus
 
+#include "common.h"
+
 struct bptFile
 /* B+ tree index file handle. */
     {
     struct bptFile *next;	/* Next in list of index files if any. */
     char *fileName;		/* Name of file - for error reporting. */
     struct udcFile *udc;			/* Open file pointer. */
     bits32 blockSize;		/* Size of block. */
```

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/binRange.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/binRange.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/bits.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/bits.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/chain.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/chain.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/chainBlock.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/chainBlock.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/common.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/common.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/dlist.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/dlist.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/dnaseq.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/dnaseq.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/dnautil.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/dnautil.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/dystring.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/dystring.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/errAbort.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/errAbort.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/errCatch.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/errCatch.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/fa.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/fa.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/fuzzyFind.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/fuzzyFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/genoFind.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/genoFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/gfClientLib.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/gfClientLib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/gfInternal.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/gfInternal.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/hash.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/hash.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/linefile.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/linefile.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/localmem.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/localmem.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/maf.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/maf.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/memalloc.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/memalloc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/net.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/net.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/netlib.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/netlib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/nib.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/nib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/obscure.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/obscure.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/ooc.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/ooc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/options.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/options.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/patSpace.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/patSpace.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/pipeline.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/portable.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/portable.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/psl.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/psl.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/rangeTree.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/rangeTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/repMask.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/repMask.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/sig.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/sig.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/sqlList.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/sqlList.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/sqlNum.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/sqlNum.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/supStitch.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/supStitch.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/trans3.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/trans3.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/twoBit.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/twoBit.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/udc.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/udc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/core/verbose.h` & `pxblat-0.2.0/src/pxblat/extc/include/core/verbose.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/include/net/log.h` & `pxblat-0.2.0/src/pxblat/extc/include/net/log.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/axt.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/axt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/bandExt.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/bandExt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/base64.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/base64.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/binRange.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/binRange.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/blastOut.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/blastOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/cheapcgi.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/cheapcgi.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/ffSeedExtend.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/ffSeedExtend.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/filePath.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/filePath.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/hex.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/hex.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/htmlPage.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/htmlPage.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/htmshell.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/htmshell.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/https.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/https.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/intExp.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/intExp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/internet.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/internet.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/maf.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/maf.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/mafFromAxt.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/mafFromAxt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/mime.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/mime.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/net.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/net.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/netlib.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/netlib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/ooc.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/ooc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/patSpace.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/patSpace.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/portimpl.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/portimpl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/rangeTree.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/rangeTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/rbTree.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/rbTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/repMask.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/repMask.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/servBrcMcw.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/servBrcMcw.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/servCrunx.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/servCrunx.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/servcis.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/servcis.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/servmsII.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/servmsII.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/servpws.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/servpws.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/sqlList.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/sqlList.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/sqlNum.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/sqlNum.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/aux/wildcmp.c` & `pxblat-0.2.0/src/pxblat/extc/src/aux/wildcmp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/aliType.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/aliType.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/bPlusTree.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/bPlusTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/bits.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/bits.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/chain.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/chain.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/chainBlock.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/chainBlock.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/common.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/common.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/dlist.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/dlist.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/dnaseq.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/dnaseq.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/dnautil.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/dnautil.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/dystring.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/dystring.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/errAbort.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/errAbort.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/errCatch.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/errCatch.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/fa.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/fa.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/ffAli.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/ffAli.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/ffAliHelp.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/ffAliHelp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/ffScore.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/ffScore.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/fuzzyFind.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/fuzzyFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/genoFind.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/genoFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/gfBlatLib.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/gfBlatLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/gfClientLib.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/gfClientLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/gfInternal.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/gfInternal.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/gfOut.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/gfOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/hash.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/hash.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/kxTok.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/kxTok.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/linefile.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/linefile.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/localmem.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/localmem.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/memalloc.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/memalloc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/nib.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/nib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/obscure.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/obscure.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/options.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/options.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/osunix.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/osunix.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/pipeline.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/pipeline.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/psl.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/psl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/servcl.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/servcl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/supStitch.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/supStitch.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/trans3.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/trans3.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/twoBit.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/twoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/udc.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/udc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/core/verbose.c` & `pxblat-0.2.0/src/pxblat/extc/src/core/verbose.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/net/gfNet.c` & `pxblat-0.2.0/src/pxblat/extc/src/net/gfNet.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/extc/src/net/log.c` & `pxblat-0.2.0/src/pxblat/extc/src/net/log.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/parser.py` & `pxblat-0.2.0/src/pxblat/parser.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/server/__init__.py` & `pxblat-0.2.0/src/pxblat/server/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from .basic import check_port_in_use
 from .basic import check_port_open
 from .basic import DEFAULT_PORT
-from .basic import fa_to_two_bit
 from .basic import files
 from .basic import find_free_port
 from .basic import server_query
 from .basic import start_server
 from .basic import start_server_mt
 from .basic import start_server_mt_nb
 from .basic import status_server
@@ -26,15 +25,14 @@
     "server_query",
     "start_server_mt",
     "start_server",
     "status_server",
     "stop_server",
     "create_client_option",
     "query_server",
-    "fa_to_two_bit",
     "create_server_option",
     "check_port_open",
     "start_server_mt_nb",
     "wait_server_ready",
     "find_free_port",
     "check_port_in_use",
     "DEFAULT_PORT",
```

### Comparing `pxblat-0.1.6/src/pxblat/server/basic.py` & `pxblat-0.2.0/src/pxblat/server/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 import time
 import typing as t
 import warnings
 from collections import Counter
 from multiprocessing import Process
 
 from deprecated import deprecated  # type: ignore
-from pxblat.extc import faToTwoBit
-from pxblat.extc import gfServerOption
 from pxblat.extc import pygetFileList
 from pxblat.extc import pyqueryServer
 from pxblat.extc import pystartServer
+from pxblat.extc import ServerOption
 from pxblat.extc import startServer
 from pxblat.extc import UsageStats
 
 from .status import Status
 from .utils import logger
 
 DEFAULT_PORT = 65000
@@ -77,15 +76,15 @@
     res = [_check_port_in_use_by_connect(host, port) for _ in range(tries)]
     counter = Counter(res)
     logger.debug(f"{res}")
     return counter[True] > counter[False]
 
 
 def _check_port_in_use_by_status(
-    host: str, port: int, gfserver_option: gfServerOption
+    host: str, port: int, gfserver_option: ServerOption
 ) -> bool:
     """Check the port is in use by status_server
 
     Args:
         host: host name
         port: port number
         gfserver_option: server option for the opening server
@@ -185,31 +184,31 @@
             if time.perf_counter() - start > timeout:
                 raise RuntimeError("wait for server ready timeout")
 
 
 def check_server_status(
     host: str,
     port: int,
-    gfserver_option: gfServerOption,
+    gfserver_option: ServerOption,
 ) -> bool:
     """Check the status of a server by attempting to connect to it using the specified host, port, and gfserver_option.
 
     Args:
         host (str): The hostname or IP address of the server to check.
         port (int): The port number to use when attempting to connect to the server.
-        gfserver_option (gfServerOption): The gfserver option to use when attempting to connect to the server.
+        gfserver_option (ServerOption): The gfserver option to use when attempting to connect to the server.
 
     Returns:
         bool: True if the server is running and accepting connections, False otherwise.
 
     Raises:
         ConnectionRefusedError: If the server is not running or is not accepting connections.
 
     Example:
-        >>> check_server_status('localhost', 8080, gfServerOption)
+        >>> check_server_status('localhost', 8080, ServerOption)
         True
     """
     try:
         status_server(host, port, gfserver_option)
     except ConnectionRefusedError:
         return False
     else:
@@ -230,61 +229,30 @@
         return s.connect_ex((host, port)) == 0
 
 
 def gfSignature() -> str:
     return "0ddf270562684f29"
 
 
-def fa_to_two_bit(
-    inFiles: t.List[str],
-    outFile: str,
-    noMask: bool = False,
-    stripVersion: bool = False,
-    ignoreDups: bool = False,
-    useLong: bool = False,
-):
-    """Convert one or more FASTA files to two-bit format.
-
-    Args:
-        inFiles (List[str]): A list of paths to the input FASTA files.
-        outFile (str): The path to the output two-bit file.
-        noMask (bool, optional): If True, do not mask the output sequence. Defaults to False.
-        stripVersion (bool, optional): If True, strip the version number from the sequence IDs. Defaults to False.
-        ignoreDups (bool, optional): If True, ignore duplicate sequences in the input files. Defaults to False.
-        useLong (bool, optional): If True, use the long format for the two-bit file. Defaults to False.
-
-    Returns:
-        None
-
-    This function converts one or more input FASTA files to two-bit format and saves the result to the specified output file.
-    The function takes several optional arguments that control the behavior of the conversion process, such as whether to mask
-    the output sequence or strip the version number from the sequence IDs. The function returns None.
-
-    Example:
-        >>> fa_to_two_bit(['input.fasta'], 'output.2bit')
-    """
-    return faToTwoBit(inFiles, outFile, noMask, stripVersion, ignoreDups, useLong)
-
-
 def status_server(
-    host: str, port: int, options: gfServerOption, instance=False
+    host: str, port: int, options: ServerOption, instance=False
 ) -> t.Union[Status, t.Dict[str, str]]:
     """Get the status of a running server.
 
     Args:
         host (str): The hostname or IP address of the server to check.
         port (int): The port number to use when attempting to connect to the server.
-        options (gfServerOption): The gfserver option to use when attempting to connect to the server.
+        options (ServerOption): The gfserver option to use when attempting to connect to the server.
         instance (bool, optional): If True, return a Status object instead of a dictionary. Defaults to False.
 
     Returns:
         Union[Status, Dict[str, str]]: A dictionary or Status object containing the status information for the server.
 
     Example:
-        >>> status_server('localhost', 8080, gfServerOption, instance=True)
+        >>> status_server('localhost', 8080, ServerOption, instance=True)
         Status(uptime='0', queries='0', sequences='0', bytes='0', memory='0', threads='0', connections='0')
     """
     if not options.genome:
         message = f"{gfSignature()}status".encode()
     else:
         temp = "transInfo" if options.trans else "untransInfo"
         message = (
@@ -404,43 +372,43 @@
     return re_str
 
 
 def start_server(
     host: str,
     port: int,
     two_bit_file: str,
-    option: gfServerOption,
+    option: ServerOption,
     stat: UsageStats,
 ):
     """Start a server in blocking mode.
 
     Args:
         host (str): The hostname or IP address to bind the server to.
         port (int): The port number to bind the server to.
         two_bit_file (str): The path to the 2bit file to use for the server.
-        option (gfServerOption): The options to use for the server.
+        option (ServerOption): The options to use for the server.
         stat (UsageStats): The usage statistics for the server.
 
     Returns:
         None
 
     This function starts a server in blocking mode by calling the pystartServer function with the given arguments. The function
     takes the hostname, port number, 2bit file path, server options, and usage statistics as arguments. The function returns None.
 
     Example:
-        >>> start_server('localhost', 8080, '/path/to/2bit/file', gfServerOption, UsageStats())
+        >>> start_server('localhost', 8080, '/path/to/2bit/file', ServerOption, UsageStats())
     """
     return startServer(host, str(port), 1, [two_bit_file], option, stat)
 
 
 def start_server_mt(
     host: str,
     port: int,
     two_bit_file: str,
-    option: gfServerOption,
+    option: ServerOption,
     stat: UsageStats,
     use_others: bool = False,
     timeout: int = 60,
     try_new_port: bool = True,
 ):
     """Start server in blocking mode.
 
@@ -468,15 +436,15 @@
         raise e
 
 
 def start_server_mt_nb(
     host: str,
     port: int,
     two_bit_file: str,
-    option: gfServerOption,
+    option: ServerOption,
     stat: UsageStats,
     use_others: bool = False,
     timeout: int = 60,
     try_new_port: bool = True,
 ) -> Process:
     """Start server in non-blocking mode.
```

### Comparing `pxblat-0.1.6/src/pxblat/server/client.py` & `pxblat-0.2.0/src/pxblat/server/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 import tempfile
 from pathlib import Path
 from threading import Thread
 from typing import Optional
 
-from pxblat.extc import gfClientOption
+from pxblat.extc import ClientOption
 from pxblat.extc import pygfClient
 from pxblat.parser import read
 
 from .basic import wait_server_ready
-from .server import gfServerOption
+from .server import ServerOption
 
 
 def create_client_option():
     """
-    Creates a new gfClientOption object with default values.
+    Creates a new ClientOption object with default values.
 
     Return:
-        gfClientOption object
+        ClientOption object
 
     """
-    return gfClientOption()
+    return ClientOption()
 
 
 def _resolve_host_port(
-    client_option: gfClientOption, host: Optional[str], port: Optional[int]
+    client_option: ClientOption, host: Optional[str], port: Optional[int]
 ):
     """Resolves the host and port for the client option.
 
     Args:
-        client_option: gfClientOption object
+        client_option: ClientOption object
         host: Optional[str]
         port: Optional[int]
     """
     if host is not None:
         client_option.hostName = host
 
     if port is not None:
         client_option.portName = str(port)
 
     if not client_option.hostName and not client_option.portName:
         raise ValueError("host and port are both empty")
 
 
 def query_server(
-    option: gfClientOption,
+    option: ClientOption,
     host: Optional[str] = None,
     port: Optional[int] = None,
     seqname: Optional[str] = None,
     parse: bool = True,
 ):
     """
     Sends a query to the server and returns the result.
 
     Args:
-        option: gfClientOption object
+        option: ClientOption object
         host: Optional[str]
         port: Optional[int]
         seqname: Optional[str]
         parse: bool
 
     Returns:
         str or bytes: The result of the query.
@@ -86,42 +86,42 @@
         ret_decode = ret.decode().rsplit(",\n", 1)[0]  # type: ignore
     except UnicodeDecodeError:
         ret_decode = ret.decode("latin-1").rsplit(",\n", 1)[0]  # type: ignore
 
     if fafile is not None:
         Path(fafile.name).unlink()
 
-    if parse:
+    if parse and ret_decode:
         return read(ret_decode, "psl")
 
     return ret_decode
 
 
 class Client(Thread):
     def __init__(
         self,
-        option: gfClientOption,
+        option: ClientOption,
         host: Optional[str] = None,
         port: Optional[int] = None,
         wait_ready: bool = False,
         wait_timeout: int = 60,
-        server_option: Optional[gfServerOption] = None,
+        server_option: Optional[ServerOption] = None,
         seqname: Optional[str] = None,
         parse: bool = True,
         daemon: bool = True,
     ):
         """A class for querying a gfServer using a separate thread.
 
         Args:
-            option: gfClientOption object
+            option: ClientOption object
             host: Optional[str]
             port: Optional[int]
             wait_ready: bool
             wait_timeout: int
-            server_option: Optional[gfServerOption]
+            server_option: Optional[ServerOption]
             seqname: Optional[str]
             parse: bool
             daemon: bool
 
         Attributes:
             result: The result of the query.
 
@@ -178,17 +178,17 @@
     @port.setter
     def port(self, value: int):
         self._port = value
 
     @classmethod
     def create_option(cls):
         """
-        Creates a new gfClientOption object with default values.
+        Creates a new ClientOption object with default values.
 
         Return:
-            gfClientOption object
+            ClientOption object
 
         """
         return create_client_option()
 
     def _resolve_host_port(self):
         _resolve_host_port(self.option, self._host, self._port)
```

### Comparing `pxblat-0.1.6/src/pxblat/server/server.py` & `pxblat-0.2.0/src/pxblat/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,57 +1,67 @@
 import typing as t
 from contextlib import ContextDecorator
 from multiprocessing import Process
 from pathlib import Path
 from typing import Union
 
-from pxblat.extc import gfServerOption
 from pxblat.extc import pystartServer
+from pxblat.extc import ServerOption
 from pxblat.extc import UsageStats
 
 from .basic import check_port_in_use
 from .basic import files
 from .basic import find_free_port
 from .basic import logger
 from .basic import server_query
 from .basic import status_server
 from .basic import stop_server
 from .basic import wait_server_ready
 from .status import Status
 
 
-def create_server_option() -> gfServerOption:
+def _pystartServer(
+    hostName: str,
+    portName: str,
+    seqFiles: t.List[str],
+    options: ServerOption,
+    stats: UsageStats,
+):
+    pystartServer(hostName, portName, len(seqFiles), seqFiles, options, stats)
+
+
+def create_server_option() -> ServerOption:
     """
-    Creates a new gfServerOption object with default values.
+    Creates a new ServerOption object with default values.
 
     Returns:
-        gfServerOption: A new gfServerOption object with default values.
+        ServerOption: A new ServerOption object with default values.
     """
-    return gfServerOption()
+    return ServerOption()
 
 
 class Server(ContextDecorator):
     def __init__(
         self,
         host: str,
         port: int,
         two_bit: Union[Path, str],
-        option: gfServerOption,
+        option: ServerOption,
         daemon=True,
         use_others: bool = False,
         timeout: int = 60,
         block: bool = False,
     ):
         """Initializes a gfServer object with the given parameters.
 
         Args:
             host (str): The hostname or IP address to bind the server to.
             port (int): The port number to bind the server to.
             two_bit (Union[Path, str]): The path to the 2bit file or the URL of the 2bit file.
-            option (gfServerOption): The options to use when starting the server.
+            option (ServerOption): The options to use when starting the server.
             daemon (bool, optional): Whether to run the server as a daemon process. Defaults to True.
             use_others (bool, optional): Whether to allow other users to access the server. Defaults to False.
             timeout (int, optional): The number of seconds to wait for the server to start. Defaults to 60.
             block (bool, optional): Whether to block until the server is ready. Defaults to False.
 
         Raises:
             ValueError: If the given two_bit file or URL is invalid.
@@ -135,35 +145,37 @@
                 if self.use_others:
                     self._is_open = False
                     # wait_server_ready(host, port, timeout)
                 else:
                     self._is_open = True
                     new_port = find_free_port(self._host, start=self.port + 1)
                     self.port = new_port
+                    host = self.host
+                    port = self.port
+
                     self._process = Process(
-                        target=pystartServer,
+                        target=_pystartServer,
                         args=(
-                            self.host,
-                            str(self.port),
-                            1,
+                            host,
+                            str(port),
                             [two_bit_file],
                             self.option,
                             self.stat,
                         ),
                         daemon=self.daemon,
                     )
+
             else:
                 self._is_open = True
                 logger.debug(f"{self.port} port not in use")
                 self._process = Process(
-                    target=pystartServer,
+                    target=_pystartServer,
                     args=(
                         self.host,
                         str(self.port),
-                        1,
                         [two_bit_file],
                         self.option,
                         self.stat,
                     ),
                     daemon=self.daemon,
                 )
         except Exception as e:
@@ -190,14 +202,17 @@
         Stops the gfServer instance if it is running.
 
         This method sends a stop signal to the server process, causing it to terminate gracefully.
         """
         if self._is_open:
             stop_server(self.host, self.port)
 
+        if self._process is not None:
+            self._process.terminate()
+
     def status(self, instance=False) -> t.Union[t.Dict[str, str], Status]:
         """
         Retrieves the status of the gfServer instance.
 
         Args:
             instance (bool, optional): If True, returns a Status object. If False, returns a dictionary with status information. Defaults to False.
```

### Comparing `pxblat-0.1.6/src/pxblat/server/status.py` & `pxblat-0.2.0/src/pxblat/server/status.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/src/pxblat/utils.py` & `pxblat-0.2.0/src/pxblat/utils.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.6/setup.py` & `pxblat-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['pxblat', 'pxblat.cli', 'pxblat.extc', 'pxblat.server']
+['pxblat', 'pxblat.cli', 'pxblat.extc', 'pxblat.server', 'pxblat.toolkit']
 
 package_data = \
 {'': ['*'],
  'pxblat.extc': ['bindings/*',
                  'bindings/binder/*',
                  'include/*',
                  'include/aux/*',
@@ -33,17 +33,17 @@
  'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['pxblat = pxblat.cli.cli:app']}
 
 setup_kwargs = {
     'name': 'pxblat',
-    'version': '0.1.6',
+    'version': '0.2.0',
     'description': 'A native python binding for blat suit',
-    'long_description': "# PxBLAT: An Efficient and Ergonomics Python Binding Library for BLAT\n\n[![python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)](https://www.python.org/)\n[![c++](https://img.shields.io/badge/C++-00599C.svg?style=for-the-badge&logo=C++&logoColor=white)](https://en.cppreference.com/w/)\n[![c](https://img.shields.io/badge/C-A8B9CC.svg?style=for-the-badge&logo=C&logoColor=black)](https://www.gnu.org/software/gnu-c-manual/)\n[![pypi](https://img.shields.io/pypi/v/pxblat.svg?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![pyversion](https://img.shields.io/pypi/pyversions/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![license](https://img.shields.io/pypi/l/pxblat?style=for-the-badge)](https://opensource.org/licenses/mit)\n[![precommit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&style=for-the-badge)](https://github.com/charliermarsh/ruff)\n[![download](https://img.shields.io/pypi/dm/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge)](https://app.codecov.io/gh/cauliyang/pxblat)\n[![lastcommit](https://img.shields.io/github/last-commit/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/)\n[![docs](https://img.shields.io/readthedocs/pxblat?style=for-the-badge)](https://pxblat.readthedocs.io/en/latest/)\n[![release](https://img.shields.io/github/release-date/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/releases)\n[![issue](https://img.shields.io/github/issues-raw/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc)\n[![tests](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml/badge.svg?style=for-the-badge)](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml)\n[![All Contributors](https://img.shields.io/github/all-contributors/cauliyang/pxblat?color=ee8449&style=flat-the-badge)](#contributors)\n\n---\n\n## 📚 Table of Contents\n\n- [📚 Table of Contents](#-table-of-contents)\n- [🔮 Features](#-features)\n- [🏎💨 Getting Started](#-getting-started)\n- [🤝 Contributing](#-contributing)\n- [\U0001faaa License](#-license)\n- [🙏 Acknowledgments](#-acknowledgments)\n\n---\n\n## 🔮 Features\n\n- no intermidiate files, all in memory\n- no system call\n- no need to bother with log files to get status of tool\n- no need to worry about file format\n- no other dependency\n- higher proformance and Ergonomics (compare with current blat endpoint)\n\n## To-do\n\n- [x] parser gfclient result\n- [x] parse gfserver query result\n- [x] benchmarking multi connection and original version\n- [x] test result with original version\n- [x] fix build.py to build ssl, hts, maybe libuv when install with pip\n- [ ] add tool to conda channel\n- [x] add tool to pip\n- [ ] change abort to throw exceptions\n- [ ] implement psl2sam\n- [ ] implement twobit2fa\n\n---\n\n## 🚀 Getting Started\n\n```sh\npip install pxblat\n```\n\n```sh\nconda install pxblat\n```\n\n### ✅ Prerequisites\n\nBefore you begin, ensure that you have the following prerequisites installed:\n\n> `[📌  INSERT-PROJECT-PREREQUISITES]`\n\n### 💻 Installation\n\n1. Clone the pxblat repository:\n\n```sh\ngit clone https://github.com/cauliyang/pxblat.git\n```\n\n2. Change to the project directory:\n\n```sh\ncd pxblat\n```\n\n3. Install the dependencies:\n\n```sh\npoetry install\n```\n\n### 🤖 Using pxblat\n\n```sh\npxblat\n```\n\n### 🧪 Running Tests\n\n```sh\npytest\n```\n\n---\n\n## 🤝 Contributing\n\nContributions are always welcome! Please follow these steps:\n\n1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.\n2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.\n3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).\n\n```sh\ngit checkout -b new-feature-branch\n```\n\n4. Make changes to the project's codebase.\n5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.\n\n```sh\ngit commit -m 'Implemented new feature.'\n```\n\n6. Push your changes to your forked repository on GitHub using the following command\n\n```sh\ngit push origin new-feature-branch\n```\n\n7. Create a pull request to the original repository.\n   Open a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.\n   The project maintainers will review your changes and provide feedback or merge them into the main branch.\n\n---\n\n## \U0001faaa License\n\nThis project is licensed under the `[📌  INSERT-LICENSE-TYPE]` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.\n\n## Contributors\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\n---\n\n## 🙏 Acknowledgments\n\n[📌 INSERT-DESCRIPTION]\n\n---\n\n<!-- github-only -->\n",
+    'long_description': '# <img src="https://raw.githubusercontent.com/cauliyang/pxblat/main/docs/_static/logo.png" alt="logo" height=100> **PxBLAT** [![social](https://img.shields.io/github/stars/cauliyang/pxblat?style=social)](https://github.com/cauliyang/pxblat/stargazers)\n\n_An Efficient and Ergonomics Python Binding Library for BLAT_\n\n[![python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)](https://www.python.org/)\n[![c++](https://img.shields.io/badge/C++-00599C.svg?style=for-the-badge&logo=C++&logoColor=white)](https://en.cppreference.com/w/)\n[![c](https://img.shields.io/badge/C-A8B9CC.svg?style=for-the-badge&logo=C&logoColor=black)](https://www.gnu.org/software/gnu-c-manual/)\n[![pypi](https://img.shields.io/pypi/v/pxblat.svg?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![pyversion](https://img.shields.io/pypi/pyversions/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![license](https://img.shields.io/pypi/l/pxblat?style=for-the-badge)](https://opensource.org/licenses/mit)\n[![precommit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&style=for-the-badge)](https://github.com/charliermarsh/ruff)\n[![download](https://img.shields.io/pypi/dm/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge)](https://app.codecov.io/gh/cauliyang/pxblat)\n[![docs](https://img.shields.io/readthedocs/pxblat?style=for-the-badge)](https://pxblat.readthedocs.io/en/latest/)\n[![release](https://img.shields.io/github/release-date/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/releases)\n[![open-issue](https://img.shields.io/github/issues-raw/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc)\n[![close-issue](https://img.shields.io/github/issues-closed-raw/cauliyang/pxblat?style=for-the-badge)][close-issue]\n[![activity](https://img.shields.io/github/commit-activity/m/cauliyang/pxblat?style=for-the-badge)][repo]\n[![lastcommit](https://img.shields.io/github/last-commit/cauliyang/pxblat?style=for-the-badge)][repo]\n[![opull](https://img.shields.io/github/issues-pr-raw/cauliyang/pxblat?style=for-the-badge)][opull]\n[![tests](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml/badge.svg?style=for-the-badge)](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml)\n[![all contributors](https://img.shields.io/github/all-contributors/cauliyang/pxblat?style=for-the-badge)](#contributors)\n\n[repo]: https://github.com/cauliyang/pxblat\n[close-issue]: https://github.com/cauliyang/pxblat/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aclosed\n[opull]: https://github.com/cauliyang/pxblat/pulls?q=is%3Apr+is%3Aopen+sort%3Aupdated-desc\n\n## 📚 **Table of Contents**\n\n- [📚 Table of Contents](#-table-of-contents)\n- [🔮 Features](#-features)\n- [📎 Citation](#-citation)\n- [📆 To-do](#-to-do)\n- [🏎💨 Getting Started](#-getting-started)\n- [🤝 Contributing](#-contributing)\n- [\U0001faaa License](#-license)\n- [🙏 Acknowledgments](#-acknowledgments)\n\n## 🔮 **Features**\n\n**Zero System Calls**: Avoids system calls, leading to a smoother, quicker operation.<br>\n**Ergonomics**: With an ergonomic design, `PxBLAT` aims for a seamless user experience.<br>\n**No External Dependencies**: `PxBLAT` operates independently without any external dependencies.<br>\n**Self-Monitoring**: No need to trawl through log files; `PxBLAT` monitors its status internally.<br>\n**Robust Validation**: Extensively tested to ensure reliable performance and superior stability as BLAT.<br>\n**Format-Agnostic:** `PxBLAT` doesn\'t require you to worry about file formats.<br>\n**In-Memory Processing**: `PxBLAT` discards the need for intermediate files by doing all its operations in memory, ensuring speed and efficiency.<br>\n\n## 📎 **Citation**\n\nPxBLAT is scientific software, with a published paper in the [Journal].\nCheck the [published] to read the paper.\n\n## 📆 **To-do**\n\n- [x] parser gfclient result\n- [x] parse gfserver query result\n- [x] benchmarking multi connection and original version\n- [x] test result with original version\n- [x] fix build.py to build ssl, hts, maybe libuv when install with pip\n- [ ] add tool to conda channel\n- [x] add tool to pip\n- [x] change abort to throw exceptions\n- [x] implement twobit2fa\n- [ ] implement psl2sam\n\n## 🚀 **Getting Started**\n\nThe very first step in starting your journey with `PxBLAT` is to install the tool.\nTo do this, there are two options shown as below:\n\n- PyPI\n\n```bash\npip install pxblat\n```\n\n- CONDA\n\n```bash\nconda install pxblat\n```\n\nCongratulations! You\'ve successfully installed `PxBLAT` on your local machine.\nIf you have some issues, please check the [document](https://pxblat.readthedocs.io/en/latest/) first before opening a issue.\n\n### 🤖 **Using pxblat**\n\n```bash\npxblat -h\n```\n\nPlease see the [document](https://pxblat.readthedocs.io/en/latest/) for details.\n\n## 🤝 **Contributing**\n\nContributions are always welcome! Please follow these steps:\n\n1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.\n2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.\n3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).\n\n```bash\ngit checkout -b new-feature-branch\n```\n\n4. Take changes to the project\'s codebase.\n5. Install the latest package\n\n```bash\npoetry install\n```\n\n6. Test your changes\n\n```bash\npytest -vlsx test\n```\n\n7. Commit your changes to your local branch with a clear commit message that explains the changes you\'ve made.\n\n```bash\ngit commit -m \'Implemented new feature.\'\n```\n\n8. Push your changes to your forked repository on GitHub using the following command\n\n```bash\ngit push origin new-feature-branch\n```\n\nCreate a pull request to the original repository.\nOpen a new pull request to the original project repository. In the pull request, describe the changes you\'ve made and why they\'re necessary.\nThe project maintainers will review your changes and provide feedback or merge them into the main branch.\n\n## \U0001faaa **License**\n\nThis project is licensed under the [MIT](https://opensource.org/licenses/mit) License. See the [LICENSE](https://github.com/cauliyang/pxblat/blob/main/LICENSE) file for additional info.\nThe license of [BLAT](http://genome.ucsc.edu/goldenPath/help/blatSpec.html) is [here](https://genome.ucsc.edu/license/).\n\n## **Contributors**\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://yangyangli.top"><img src="https://avatars.githubusercontent.com/u/38903141?v=4?s=100" width="100px;" alt="yangliz5"/><br /><sub><b>yangliz5</b></sub></a><br /><a href="#maintenance-cauliyang" title="Maintenance">🚧</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\n## 🙏 **Acknowledgments**\n\n- [UCSC](https://github.com/ucscGenomeBrowser/kent)\n- [pybind11](https://github.com/pybind/pybind11/tree/stable)\n\n<!-- github-only -->\n',
     'author': 'Yangyang Li',
     'author_email': 'yangyang.li@northwestern.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

