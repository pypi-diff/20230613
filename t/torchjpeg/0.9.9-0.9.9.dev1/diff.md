# Comparing `tmp/torchjpeg-0.9.9.tar.gz` & `tmp/torchjpeg-0.9.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchjpeg-0.9.9.tar", last modified: Tue Sep 22 00:27:50 2020, max compression
+gzip compressed data, was "torchjpeg-0.9.9.dev1.tar", last modified: Tue Sep 22 00:22:16 2020, max compression
```

## Comparing `torchjpeg-0.9.9.tar` & `torchjpeg-0.9.9.dev1.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0     1068 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/LICENSE
--rw-r--r--   0        0        0     2944 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/README.md
--rw-r--r--   0        0        0      660 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/build.py
--rw-r--r--   0        0        0     2541 2020-09-22 00:27:50.000000 torchjpeg-0.9.9/pyproject.toml
--rw-r--r--   0        0        0     5188 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/Makefile.am
--rw-r--r--   0        0        0    45774 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/Makefile.in
--rw-r--r--   0        0        0    18584 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/README
--rw-r--r--   0        0        0   375769 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/aclocal.m4
--rwxr-xr-x   0        0        0     5827 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/ar-lib
--rw-r--r--   0        0        0     5442 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/cderror.h
--rw-r--r--   0        0        0     4682 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/cdjpeg.c
--rw-r--r--   0        0        0     6319 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/cdjpeg.h
--rw-r--r--   0        0        0    19631 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/change.log
--rw-r--r--   0        0        0    13814 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/cjpeg.1
--rw-r--r--   0        0        0    21818 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/cjpeg.c
--rw-r--r--   0        0        0    12166 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/ckconfig.c
--rw-r--r--   0        0        0     5364 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/coderules.txt
--rwxr-xr-x   0        0        0     7383 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/compile
--rwxr-xr-x   0        0        0    44166 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/config.guess
--rwxr-xr-x   0        0        0    36141 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/config.sub
--rwxr-xr-x   0        0        0   473932 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/configure
--rw-r--r--   0        0        0    11963 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/configure.ac
--rwxr-xr-x   0        0        0    23568 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/depcomp
--rw-r--r--   0        0        0     7937 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/djpeg.1
--rw-r--r--   0        0        0    19990 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/djpeg.c
--rw-r--r--   0        0        0    17091 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/example.c
--rw-r--r--   0        0        0     8483 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/filelist.txt
--rwxr-xr-x   0        0        0    15368 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/install-sh
--rw-r--r--   0        0        0    54647 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/install.txt
--rw-r--r--   0        0        0     5082 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jaricom.c
--rw-r--r--   0        0        0     9384 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcapimin.c
--rw-r--r--   0        0        0     5940 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcapistd.c
--rw-r--r--   0        0        0    28255 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcarith.c
--rw-r--r--   0        0        0    16650 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jccoefct.c
--rw-r--r--   0        0        0    19458 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jccolor.c
--rw-r--r--   0        0        0    15550 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcdctmgr.c
--rw-r--r--   0        0        0    50282 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jchuff.c
--rw-r--r--   0        0        0    10663 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcinit.c
--rw-r--r--   0        0        0     9656 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcmainct.c
--rw-r--r--   0        0        0    18914 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcmarker.c
--rw-r--r--   0        0        0    23150 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcmaster.c
--rw-r--r--   0        0        0     8114 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcomapi.c
--rw-r--r--   0        0        0     1416 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.bcc
--rw-r--r--   0        0        0     1605 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.cfg
--rw-r--r--   0        0        0     1143 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.dj
--rw-r--r--   0        0        0     1199 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.mac
--rw-r--r--   0        0        0     1197 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.manx
--rw-r--r--   0        0        0     1668 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.mc6
--rw-r--r--   0        0        0     1170 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.sas
--rw-r--r--   0        0        0     1308 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.st
--rw-r--r--   0        0        0     5821 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.txt
--rw-r--r--   0        0        0     1553 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.vc
--rw-r--r--   0        0        0      979 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.vms
--rw-r--r--   0        0        0     1139 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jconfig.wat
--rw-r--r--   0        0        0    19835 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcparam.c
--rw-r--r--   0        0        0    12216 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcprepct.c
--rw-r--r--   0        0        0    19923 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jcsample.c
--rw-r--r--   0        0        0    14627 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jctrans.c
--rw-r--r--   0        0        0    12842 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdapimin.c
--rw-r--r--   0        0        0     9393 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdapistd.c
--rw-r--r--   0        0        0    24272 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdarith.c
--rw-r--r--   0        0        0     8680 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdatadst.c
--rw-r--r--   0        0        0     9345 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdatasrc.c
--rw-r--r--   0        0        0    25428 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdcoefct.c
--rw-r--r--   0        0        0    23085 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdcolor.c
--rw-r--r--   0        0        0    17619 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdct.h
--rw-r--r--   0        0        0    12380 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jddctmgr.c
--rw-r--r--   0        0        0    48761 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdhuff.c
--rw-r--r--   0        0        0    25087 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdinput.c
--rw-r--r--   0        0        0    20370 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdmainct.c
--rw-r--r--   0        0        0    45824 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdmarker.c
--rw-r--r--   0        0        0    19092 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdmaster.c
--rw-r--r--   0        0        0    15632 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdmerge.c
--rw-r--r--   0        0        0     9723 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdpostct.c
--rw-r--r--   0        0        0    11932 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdsample.c
--rw-r--r--   0        0        0     5053 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jdtrans.c
--rw-r--r--   0        0        0     7850 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jerror.c
--rw-r--r--   0        0        0    14588 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jerror.h
--rw-r--r--   0        0        0     6049 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jfdctflt.c
--rw-r--r--   0        0        0     8021 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jfdctfst.c
--rw-r--r--   0        0        0   159013 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jfdctint.c
--rw-r--r--   0        0        0     8362 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jidctflt.c
--rw-r--r--   0        0        0    12718 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jidctfst.c
--rw-r--r--   0        0        0   184800 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jidctint.c
--rw-r--r--   0        0        0     3499 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jinclude.h
--rw-r--r--   0        0        0     4610 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jmemansi.c
--rw-r--r--   0        0        0    18977 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jmemdos.c
--rw-r--r--   0        0        0     8314 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jmemdosa.asm
--rw-r--r--   0        0        0     9507 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jmemmac.c
--rw-r--r--   0        0        0    41029 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jmemmgr.c
--rw-r--r--   0        0        0     8314 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jmemname.c
--rw-r--r--   0        0        0     2910 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jmemnobs.c
--rw-r--r--   0        0        0     8230 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jmemsys.h
--rw-r--r--   0        0        0    14925 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jmorecfg.h
--rw-r--r--   0        0        0    18025 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jpegint.h
--rw-r--r--   0        0        0    49408 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jpeglib.h
--rw-r--r--   0        0        0    11173 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jpegtran.1
--rw-r--r--   0        0        0    21390 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jpegtran.c
--rw-r--r--   0        0        0    31327 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jquant1.c
--rw-r--r--   0        0        0    48471 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jquant2.c
--rw-r--r--   0        0        0     6742 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jutils.c
--rw-r--r--   0        0        0      396 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/jversion.h
--rw-r--r--   0        0        0       34 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/libjpeg.map
--rw-r--r--   0        0        0      248 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/libjpeg.pc.in
--rw-r--r--   0        0        0   163729 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/libjpeg.txt
--rw-r--r--   0        0        0   324089 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/ltmain.sh
--rw-r--r--   0        0        0     1674 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makcjpeg.st
--rw-r--r--   0        0        0     1674 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makdjpeg.st
--rw-r--r--   0        0        0     1252 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makeadsw.vc6
--rw-r--r--   0        0        0     2845 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makeasln.v16
--rw-r--r--   0        0        0     1139 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makecdep.vc6
--rw-r--r--   0        0        0     3343 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makecdsp.vc6
--rw-r--r--   0        0        0     2288 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makecfil.v16
--rw-r--r--   0        0        0     3277 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makecmak.vc6
--rw-r--r--   0        0        0     5974 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makecvcx.v16
--rw-r--r--   0        0        0     1139 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makeddep.vc6
--rw-r--r--   0        0        0     3343 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makeddsp.vc6
--rw-r--r--   0        0        0     2288 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makedfil.v16
--rw-r--r--   0        0        0     3277 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makedmak.vc6
--rw-r--r--   0        0        0     5974 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makedvcx.v16
--rw-r--r--   0        0        0    12358 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.ansi
--rw-r--r--   0        0        0    13978 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.b32
--rw-r--r--   0        0        0    15033 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.bcc
--rw-r--r--   0        0        0    12494 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.dj
--rw-r--r--   0        0        0    12282 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.manx
--rw-r--r--   0        0        0    14478 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.mc6
--rw-r--r--   0        0        0    13844 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.mms
--rw-r--r--   0        0        0    13145 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.sas
--rw-r--r--   0        0        0    12732 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.unix
--rw-r--r--   0        0        0    17942 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.vc
--rw-r--r--   0        0        0     4421 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.vms
--rw-r--r--   0        0        0    17943 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.vs
--rw-r--r--   0        0        0    13020 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makefile.wat
--rw-r--r--   0        0        0     5546 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makejdep.vc6
--rw-r--r--   0        0        0     5177 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makejdsp.vc6
--rw-r--r--   0        0        0      532 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makejdsw.vc6
--rw-r--r--   0        0        0     5789 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makejfil.v16
--rw-r--r--   0        0        0     8082 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makejmak.vc6
--rw-r--r--   0        0        0     1057 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makejsln.v16
--rw-r--r--   0        0        0     6769 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makejvcx.v16
--rw-r--r--   0        0        0    10373 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makeproj.mac
--rw-r--r--   0        0        0      140 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makerdep.vc6
--rw-r--r--   0        0        0     2636 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makerdsp.vc6
--rw-r--r--   0        0        0     1142 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makerfil.v16
--rw-r--r--   0        0        0     2474 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makermak.vc6
--rw-r--r--   0        0        0     4974 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makervcx.v16
--rw-r--r--   0        0        0      649 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/maketdep.vc6
--rw-r--r--   0        0        0     3276 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/maketdsp.vc6
--rw-r--r--   0        0        0     2123 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/maketfil.v16
--rw-r--r--   0        0        0     2868 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/maketmak.vc6
--rw-r--r--   0        0        0     5914 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/maketvcx.v16
--rw-r--r--   0        0        0      140 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makewdep.vc6
--rw-r--r--   0        0        0     2636 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makewdsp.vc6
--rw-r--r--   0        0        0     1142 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makewfil.v16
--rw-r--r--   0        0        0     2474 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makewmak.vc6
--rw-r--r--   0        0        0     4974 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makewvcx.v16
--rw-r--r--   0        0        0     4184 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makljpeg.st
--rw-r--r--   0        0        0     1252 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/maktjpeg.st
--rw-r--r--   0        0        0      210 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/makvms.opt
--rwxr-xr-x   0        0        0     6878 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/missing
--rw-r--r--   0        0        0    15075 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/rdbmp.c
--rw-r--r--   0        0        0     6849 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/rdcolmap.c
--rw-r--r--   0        0        0    22701 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/rdgif.c
--rw-r--r--   0        0        0     1703 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/rdjpgcom.1
--rw-r--r--   0        0        0    14466 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/rdjpgcom.c
--rw-r--r--   0        0        0    15762 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/rdppm.c
--rw-r--r--   0        0        0    11462 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/rdrle.c
--rw-r--r--   0        0        0    10799 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/rdswitch.c
--rw-r--r--   0        0        0    15099 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/rdtarga.c
--rw-r--r--   0        0        0    51565 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/structure.txt
--rw-r--r--   0        0        0    35050 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/testimg.bmp
--rw-r--r--   0        0        0    21718 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/testimg.gif
--rw-r--r--   0        0        0     5764 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/testimg.jpg
--rw-r--r--   0        0        0   101484 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/testimg.ppm
--rw-r--r--   0        0        0     5645 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/testimgp.jpg
--rw-r--r--   0        0        0     5770 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/testorig.jpg
--rw-r--r--   0        0        0     5655 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/testprog.jpg
--rw-r--r--   0        0        0    88214 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/transupp.c
--rw-r--r--   0        0        0    10083 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/transupp.h
--rw-r--r--   0        0        0    34609 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/usage.txt
--rw-r--r--   0        0        0     9759 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/wizard.txt
--rw-r--r--   0        0        0    13801 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/wrbmp.c
--rw-r--r--   0        0        0    17942 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/wrgif.c
--rw-r--r--   0        0        0     2627 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/wrjpgcom.1
--rw-r--r--   0        0        0    17181 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/wrjpgcom.c
--rw-r--r--   0        0        0     8307 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/wrppm.c
--rw-r--r--   0        0        0     9189 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/wrrle.c
--rw-r--r--   0        0        0     7481 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/libjpeg/wrtarga.c
--rw-r--r--   0        0        0      152 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/__init__.py
--rw-r--r--   0        0        0     4060 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/codec/__init__.py
--rw-r--r--   0        0        0    17844 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/codec/codec_ops.cpp
--rw-r--r--   0        0        0    14111 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/dct/__init__.py
--rw-r--r--   0        0        0     2298 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/dct/_block.py
--rw-r--r--   0        0        0     2803 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/dct/_color.py
--rw-r--r--   0        0        0     5053 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/dct/_nn.py
--rw-r--r--   0        0        0     3652 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/dct/_stats.py
--rw-r--r--   0        0        0      487 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/metrics/__init__.py
--rw-r--r--   0        0        0      822 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/metrics/_psnr.py
--rw-r--r--   0        0        0     4112 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/metrics/_psnrb.py
--rw-r--r--   0        0        0     1144 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/metrics/_size.py
--rw-r--r--   0        0        0     1822 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/metrics/_ssim.py
--rw-r--r--   0        0        0     3381 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/quantization/__init__.py
--rw-r--r--   0        0        0     1732 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/quantization/_quantize.py
--rw-r--r--   0        0        0     5658 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/quantization/ijg.py
--rw-r--r--   0        0        0     2266 2020-09-22 00:25:53.000000 torchjpeg-0.9.9/src/torchjpeg/transforms/__init__.py
--rw-r--r--   0        0        0     3896 2020-09-22 00:27:51.240117 torchjpeg-0.9.9/setup.py
--rw-r--r--   0        0        0     3934 2020-09-22 00:27:51.240551 torchjpeg-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/LICENSE
+-rw-r--r--   0        0        0     2944 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/README.md
+-rw-r--r--   0        0        0      660 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/build.py
+-rw-r--r--   0        0        0     2546 2020-09-22 00:22:15.000000 torchjpeg-0.9.9.dev1/pyproject.toml
+-rw-r--r--   0        0        0     5188 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/Makefile.am
+-rw-r--r--   0        0        0    45774 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/Makefile.in
+-rw-r--r--   0        0        0    18584 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/README
+-rw-r--r--   0        0        0   375769 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/aclocal.m4
+-rwxr-xr-x   0        0        0     5827 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/ar-lib
+-rw-r--r--   0        0        0     5442 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/cderror.h
+-rw-r--r--   0        0        0     4682 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/cdjpeg.c
+-rw-r--r--   0        0        0     6319 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/cdjpeg.h
+-rw-r--r--   0        0        0    19631 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/change.log
+-rw-r--r--   0        0        0    13814 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/cjpeg.1
+-rw-r--r--   0        0        0    21818 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/cjpeg.c
+-rw-r--r--   0        0        0    12166 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/ckconfig.c
+-rw-r--r--   0        0        0     5364 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/coderules.txt
+-rwxr-xr-x   0        0        0     7383 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/compile
+-rwxr-xr-x   0        0        0    44166 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/config.guess
+-rwxr-xr-x   0        0        0    36141 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/config.sub
+-rwxr-xr-x   0        0        0   473932 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/configure
+-rw-r--r--   0        0        0    11963 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/configure.ac
+-rwxr-xr-x   0        0        0    23568 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/depcomp
+-rw-r--r--   0        0        0     7937 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/djpeg.1
+-rw-r--r--   0        0        0    19990 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/djpeg.c
+-rw-r--r--   0        0        0    17091 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/example.c
+-rw-r--r--   0        0        0     8483 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/filelist.txt
+-rwxr-xr-x   0        0        0    15368 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/install-sh
+-rw-r--r--   0        0        0    54647 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/install.txt
+-rw-r--r--   0        0        0     5082 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jaricom.c
+-rw-r--r--   0        0        0     9384 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcapimin.c
+-rw-r--r--   0        0        0     5940 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcapistd.c
+-rw-r--r--   0        0        0    28255 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcarith.c
+-rw-r--r--   0        0        0    16650 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jccoefct.c
+-rw-r--r--   0        0        0    19458 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jccolor.c
+-rw-r--r--   0        0        0    15550 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcdctmgr.c
+-rw-r--r--   0        0        0    50282 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jchuff.c
+-rw-r--r--   0        0        0    10663 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcinit.c
+-rw-r--r--   0        0        0     9656 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcmainct.c
+-rw-r--r--   0        0        0    18914 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcmarker.c
+-rw-r--r--   0        0        0    23150 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcmaster.c
+-rw-r--r--   0        0        0     8114 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcomapi.c
+-rw-r--r--   0        0        0     1416 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.bcc
+-rw-r--r--   0        0        0     1605 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.cfg
+-rw-r--r--   0        0        0     1143 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.dj
+-rw-r--r--   0        0        0     1199 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.mac
+-rw-r--r--   0        0        0     1197 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.manx
+-rw-r--r--   0        0        0     1668 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.mc6
+-rw-r--r--   0        0        0     1170 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.sas
+-rw-r--r--   0        0        0     1308 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.st
+-rw-r--r--   0        0        0     5821 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.txt
+-rw-r--r--   0        0        0     1553 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.vc
+-rw-r--r--   0        0        0      979 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.vms
+-rw-r--r--   0        0        0     1139 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.wat
+-rw-r--r--   0        0        0    19835 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcparam.c
+-rw-r--r--   0        0        0    12216 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcprepct.c
+-rw-r--r--   0        0        0    19923 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jcsample.c
+-rw-r--r--   0        0        0    14627 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jctrans.c
+-rw-r--r--   0        0        0    12842 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdapimin.c
+-rw-r--r--   0        0        0     9393 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdapistd.c
+-rw-r--r--   0        0        0    24272 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdarith.c
+-rw-r--r--   0        0        0     8680 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdatadst.c
+-rw-r--r--   0        0        0     9345 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdatasrc.c
+-rw-r--r--   0        0        0    25428 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdcoefct.c
+-rw-r--r--   0        0        0    23085 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdcolor.c
+-rw-r--r--   0        0        0    17619 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdct.h
+-rw-r--r--   0        0        0    12380 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jddctmgr.c
+-rw-r--r--   0        0        0    48761 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdhuff.c
+-rw-r--r--   0        0        0    25087 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdinput.c
+-rw-r--r--   0        0        0    20370 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdmainct.c
+-rw-r--r--   0        0        0    45824 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdmarker.c
+-rw-r--r--   0        0        0    19092 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdmaster.c
+-rw-r--r--   0        0        0    15632 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdmerge.c
+-rw-r--r--   0        0        0     9723 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdpostct.c
+-rw-r--r--   0        0        0    11932 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdsample.c
+-rw-r--r--   0        0        0     5053 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jdtrans.c
+-rw-r--r--   0        0        0     7850 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jerror.c
+-rw-r--r--   0        0        0    14588 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jerror.h
+-rw-r--r--   0        0        0     6049 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jfdctflt.c
+-rw-r--r--   0        0        0     8021 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jfdctfst.c
+-rw-r--r--   0        0        0   159013 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jfdctint.c
+-rw-r--r--   0        0        0     8362 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jidctflt.c
+-rw-r--r--   0        0        0    12718 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jidctfst.c
+-rw-r--r--   0        0        0   184800 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jidctint.c
+-rw-r--r--   0        0        0     3499 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jinclude.h
+-rw-r--r--   0        0        0     4610 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jmemansi.c
+-rw-r--r--   0        0        0    18977 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jmemdos.c
+-rw-r--r--   0        0        0     8314 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jmemdosa.asm
+-rw-r--r--   0        0        0     9507 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jmemmac.c
+-rw-r--r--   0        0        0    41029 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jmemmgr.c
+-rw-r--r--   0        0        0     8314 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jmemname.c
+-rw-r--r--   0        0        0     2910 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jmemnobs.c
+-rw-r--r--   0        0        0     8230 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jmemsys.h
+-rw-r--r--   0        0        0    14925 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jmorecfg.h
+-rw-r--r--   0        0        0    18025 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jpegint.h
+-rw-r--r--   0        0        0    49408 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jpeglib.h
+-rw-r--r--   0        0        0    11173 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jpegtran.1
+-rw-r--r--   0        0        0    21390 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jpegtran.c
+-rw-r--r--   0        0        0    31327 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jquant1.c
+-rw-r--r--   0        0        0    48471 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jquant2.c
+-rw-r--r--   0        0        0     6742 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jutils.c
+-rw-r--r--   0        0        0      396 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/jversion.h
+-rw-r--r--   0        0        0       34 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/libjpeg.map
+-rw-r--r--   0        0        0      248 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/libjpeg.pc.in
+-rw-r--r--   0        0        0   163729 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/libjpeg.txt
+-rw-r--r--   0        0        0   324089 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/ltmain.sh
+-rw-r--r--   0        0        0     1674 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makcjpeg.st
+-rw-r--r--   0        0        0     1674 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makdjpeg.st
+-rw-r--r--   0        0        0     1252 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makeadsw.vc6
+-rw-r--r--   0        0        0     2845 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makeasln.v16
+-rw-r--r--   0        0        0     1139 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makecdep.vc6
+-rw-r--r--   0        0        0     3343 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makecdsp.vc6
+-rw-r--r--   0        0        0     2288 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makecfil.v16
+-rw-r--r--   0        0        0     3277 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makecmak.vc6
+-rw-r--r--   0        0        0     5974 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makecvcx.v16
+-rw-r--r--   0        0        0     1139 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makeddep.vc6
+-rw-r--r--   0        0        0     3343 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makeddsp.vc6
+-rw-r--r--   0        0        0     2288 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makedfil.v16
+-rw-r--r--   0        0        0     3277 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makedmak.vc6
+-rw-r--r--   0        0        0     5974 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makedvcx.v16
+-rw-r--r--   0        0        0    12358 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.ansi
+-rw-r--r--   0        0        0    13978 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.b32
+-rw-r--r--   0        0        0    15033 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.bcc
+-rw-r--r--   0        0        0    12494 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.dj
+-rw-r--r--   0        0        0    12282 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.manx
+-rw-r--r--   0        0        0    14478 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.mc6
+-rw-r--r--   0        0        0    13844 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.mms
+-rw-r--r--   0        0        0    13145 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.sas
+-rw-r--r--   0        0        0    12732 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.unix
+-rw-r--r--   0        0        0    17942 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.vc
+-rw-r--r--   0        0        0     4421 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.vms
+-rw-r--r--   0        0        0    17943 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.vs
+-rw-r--r--   0        0        0    13020 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makefile.wat
+-rw-r--r--   0        0        0     5546 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makejdep.vc6
+-rw-r--r--   0        0        0     5177 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makejdsp.vc6
+-rw-r--r--   0        0        0      532 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makejdsw.vc6
+-rw-r--r--   0        0        0     5789 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makejfil.v16
+-rw-r--r--   0        0        0     8082 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makejmak.vc6
+-rw-r--r--   0        0        0     1057 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makejsln.v16
+-rw-r--r--   0        0        0     6769 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makejvcx.v16
+-rw-r--r--   0        0        0    10373 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makeproj.mac
+-rw-r--r--   0        0        0      140 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makerdep.vc6
+-rw-r--r--   0        0        0     2636 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makerdsp.vc6
+-rw-r--r--   0        0        0     1142 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makerfil.v16
+-rw-r--r--   0        0        0     2474 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makermak.vc6
+-rw-r--r--   0        0        0     4974 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makervcx.v16
+-rw-r--r--   0        0        0      649 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/maketdep.vc6
+-rw-r--r--   0        0        0     3276 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/maketdsp.vc6
+-rw-r--r--   0        0        0     2123 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/maketfil.v16
+-rw-r--r--   0        0        0     2868 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/maketmak.vc6
+-rw-r--r--   0        0        0     5914 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/maketvcx.v16
+-rw-r--r--   0        0        0      140 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makewdep.vc6
+-rw-r--r--   0        0        0     2636 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makewdsp.vc6
+-rw-r--r--   0        0        0     1142 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makewfil.v16
+-rw-r--r--   0        0        0     2474 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makewmak.vc6
+-rw-r--r--   0        0        0     4974 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makewvcx.v16
+-rw-r--r--   0        0        0     4184 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makljpeg.st
+-rw-r--r--   0        0        0     1252 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/maktjpeg.st
+-rw-r--r--   0        0        0      210 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/makvms.opt
+-rwxr-xr-x   0        0        0     6878 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/missing
+-rw-r--r--   0        0        0    15075 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/rdbmp.c
+-rw-r--r--   0        0        0     6849 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/rdcolmap.c
+-rw-r--r--   0        0        0    22701 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/rdgif.c
+-rw-r--r--   0        0        0     1703 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/rdjpgcom.1
+-rw-r--r--   0        0        0    14466 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/rdjpgcom.c
+-rw-r--r--   0        0        0    15762 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/rdppm.c
+-rw-r--r--   0        0        0    11462 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/rdrle.c
+-rw-r--r--   0        0        0    10799 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/rdswitch.c
+-rw-r--r--   0        0        0    15099 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/rdtarga.c
+-rw-r--r--   0        0        0    51565 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/structure.txt
+-rw-r--r--   0        0        0    35050 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/testimg.bmp
+-rw-r--r--   0        0        0    21718 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/testimg.gif
+-rw-r--r--   0        0        0     5764 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/testimg.jpg
+-rw-r--r--   0        0        0   101484 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/testimg.ppm
+-rw-r--r--   0        0        0     5645 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/testimgp.jpg
+-rw-r--r--   0        0        0     5770 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/testorig.jpg
+-rw-r--r--   0        0        0     5655 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/testprog.jpg
+-rw-r--r--   0        0        0    88214 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/transupp.c
+-rw-r--r--   0        0        0    10083 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/transupp.h
+-rw-r--r--   0        0        0    34609 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/usage.txt
+-rw-r--r--   0        0        0     9759 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/wizard.txt
+-rw-r--r--   0        0        0    13801 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/wrbmp.c
+-rw-r--r--   0        0        0    17942 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/wrgif.c
+-rw-r--r--   0        0        0     2627 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/wrjpgcom.1
+-rw-r--r--   0        0        0    17181 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/wrjpgcom.c
+-rw-r--r--   0        0        0     8307 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/wrppm.c
+-rw-r--r--   0        0        0     9189 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/wrrle.c
+-rw-r--r--   0        0        0     7481 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/libjpeg/wrtarga.c
+-rw-r--r--   0        0        0      152 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/__init__.py
+-rw-r--r--   0        0        0     4060 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/codec/__init__.py
+-rw-r--r--   0        0        0    17844 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/codec/codec_ops.cpp
+-rw-r--r--   0        0        0    14111 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/dct/__init__.py
+-rw-r--r--   0        0        0     2298 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/dct/_block.py
+-rw-r--r--   0        0        0     2803 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/dct/_color.py
+-rw-r--r--   0        0        0     5053 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/dct/_nn.py
+-rw-r--r--   0        0        0     3652 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/dct/_stats.py
+-rw-r--r--   0        0        0      487 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/metrics/__init__.py
+-rw-r--r--   0        0        0      822 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/metrics/_psnr.py
+-rw-r--r--   0        0        0     4112 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/metrics/_psnrb.py
+-rw-r--r--   0        0        0     1144 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/metrics/_size.py
+-rw-r--r--   0        0        0     1822 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/metrics/_ssim.py
+-rw-r--r--   0        0        0     3381 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/quantization/__init__.py
+-rw-r--r--   0        0        0     1732 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/quantization/_quantize.py
+-rw-r--r--   0        0        0     5658 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/quantization/ijg.py
+-rw-r--r--   0        0        0     2266 2020-09-22 00:20:18.000000 torchjpeg-0.9.9.dev1/src/torchjpeg/transforms/__init__.py
+-rw-r--r--   0        0        0     3901 2020-09-22 00:22:16.852604 torchjpeg-0.9.9.dev1/setup.py
+-rw-r--r--   0        0        0     3939 2020-09-22 00:22:16.853117 torchjpeg-0.9.9.dev1/PKG-INFO
```

### Comparing `torchjpeg-0.9.9/LICENSE` & `torchjpeg-0.9.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/README.md` & `torchjpeg-0.9.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/build.py` & `torchjpeg-0.9.9.dev1/build.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/pyproject.toml` & `torchjpeg-0.9.9.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "torchjpeg"
-version = "0.9.9" # This is a placeholder, version is set by the CI during build
+version = "0.9.9.dev1" # This is a placeholder, version is set by the CI during build
 description = "Utilities for JPEG data access and manipulation in pytorch"
 authors = [
     "Max Ehrlich"
 ]
 
 license = "MIT"
 readme = "README.md"
```

### Comparing `torchjpeg-0.9.9/src/libjpeg/Makefile.am` & `torchjpeg-0.9.9.dev1/src/libjpeg/Makefile.am`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/Makefile.in` & `torchjpeg-0.9.9.dev1/src/libjpeg/Makefile.in`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/README` & `torchjpeg-0.9.9.dev1/src/libjpeg/README`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/aclocal.m4` & `torchjpeg-0.9.9.dev1/src/libjpeg/aclocal.m4`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/ar-lib` & `torchjpeg-0.9.9.dev1/src/libjpeg/ar-lib`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/cderror.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/cderror.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/cdjpeg.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/cdjpeg.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/cdjpeg.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/cdjpeg.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/change.log` & `torchjpeg-0.9.9.dev1/src/libjpeg/change.log`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/cjpeg.1` & `torchjpeg-0.9.9.dev1/src/libjpeg/cjpeg.1`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/cjpeg.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/cjpeg.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/ckconfig.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/ckconfig.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/coderules.txt` & `torchjpeg-0.9.9.dev1/src/libjpeg/coderules.txt`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/compile` & `torchjpeg-0.9.9.dev1/src/libjpeg/compile`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/config.guess` & `torchjpeg-0.9.9.dev1/src/libjpeg/config.guess`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/config.sub` & `torchjpeg-0.9.9.dev1/src/libjpeg/config.sub`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/configure` & `torchjpeg-0.9.9.dev1/src/libjpeg/configure`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/configure.ac` & `torchjpeg-0.9.9.dev1/src/libjpeg/configure.ac`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/depcomp` & `torchjpeg-0.9.9.dev1/src/libjpeg/depcomp`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/djpeg.1` & `torchjpeg-0.9.9.dev1/src/libjpeg/djpeg.1`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/djpeg.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/djpeg.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/example.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/example.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/filelist.txt` & `torchjpeg-0.9.9.dev1/src/libjpeg/filelist.txt`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/install-sh` & `torchjpeg-0.9.9.dev1/src/libjpeg/install-sh`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/install.txt` & `torchjpeg-0.9.9.dev1/src/libjpeg/install.txt`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jaricom.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jaricom.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcapimin.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcapimin.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcapistd.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcapistd.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcarith.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcarith.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jccoefct.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jccoefct.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jccolor.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jccolor.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcdctmgr.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcdctmgr.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jchuff.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jchuff.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcinit.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcinit.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcmainct.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcmainct.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcmarker.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcmarker.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcmaster.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcmaster.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcomapi.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcomapi.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.bcc` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.bcc`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.cfg` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.cfg`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.dj` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.dj`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.mac` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.mac`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.manx` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.manx`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.mc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.mc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.sas` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.sas`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.st` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.st`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.txt` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.txt`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.vc` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.vc`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.vms` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.vms`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jconfig.wat` & `torchjpeg-0.9.9.dev1/src/libjpeg/jconfig.wat`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcparam.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcparam.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcprepct.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcprepct.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jcsample.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jcsample.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jctrans.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jctrans.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdapimin.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdapimin.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdapistd.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdapistd.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdarith.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdarith.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdatadst.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdatadst.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdatasrc.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdatasrc.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdcoefct.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdcoefct.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdcolor.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdcolor.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdct.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdct.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jddctmgr.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jddctmgr.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdhuff.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdhuff.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdinput.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdinput.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdmainct.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdmainct.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdmarker.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdmarker.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdmaster.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdmaster.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdmerge.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdmerge.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdpostct.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdpostct.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdsample.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdsample.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jdtrans.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jdtrans.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jerror.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jerror.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jerror.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/jerror.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jfdctflt.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jfdctflt.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jfdctfst.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jfdctfst.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jfdctint.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jfdctint.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jidctflt.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jidctflt.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jidctfst.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jidctfst.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jidctint.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jidctint.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jinclude.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/jinclude.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jmemansi.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jmemansi.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jmemdos.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jmemdos.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jmemdosa.asm` & `torchjpeg-0.9.9.dev1/src/libjpeg/jmemdosa.asm`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jmemmac.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jmemmac.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jmemmgr.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jmemmgr.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jmemname.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jmemname.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jmemnobs.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jmemnobs.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jmemsys.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/jmemsys.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jmorecfg.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/jmorecfg.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jpegint.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/jpegint.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jpeglib.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/jpeglib.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jpegtran.1` & `torchjpeg-0.9.9.dev1/src/libjpeg/jpegtran.1`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jpegtran.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jpegtran.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jquant1.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jquant1.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jquant2.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jquant2.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/jutils.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/jutils.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/libjpeg.txt` & `torchjpeg-0.9.9.dev1/src/libjpeg/libjpeg.txt`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/ltmain.sh` & `torchjpeg-0.9.9.dev1/src/libjpeg/ltmain.sh`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makcjpeg.st` & `torchjpeg-0.9.9.dev1/src/libjpeg/makcjpeg.st`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makdjpeg.st` & `torchjpeg-0.9.9.dev1/src/libjpeg/makdjpeg.st`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makeadsw.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makeadsw.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makeasln.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makeasln.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makecdep.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makecdep.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makecdsp.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makecdsp.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makecfil.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makecfil.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makecmak.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makecmak.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makecvcx.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makecvcx.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makeddep.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makeddep.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makeddsp.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makeddsp.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makedfil.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makedfil.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makedmak.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makedmak.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makedvcx.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makedvcx.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.ansi` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.ansi`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.b32` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.b32`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.bcc` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.bcc`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.dj` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.dj`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.manx` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.manx`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.mc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.mc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.mms` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.mms`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.sas` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.sas`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.unix` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.unix`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.vc` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.vc`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.vms` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.vms`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.vs` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.vs`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makefile.wat` & `torchjpeg-0.9.9.dev1/src/libjpeg/makefile.wat`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makejdep.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makejdep.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makejdsp.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makejdsp.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makejdsw.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makejdsw.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makejfil.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makejfil.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makejmak.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makejmak.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makejsln.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makejsln.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makejvcx.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makejvcx.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makeproj.mac` & `torchjpeg-0.9.9.dev1/src/libjpeg/makeproj.mac`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makerdsp.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makerdsp.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makerfil.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makerfil.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makermak.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makermak.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makervcx.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makervcx.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/maketdep.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/maketdep.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/maketdsp.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/maketdsp.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/maketfil.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/maketfil.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/maketmak.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/maketmak.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/maketvcx.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/maketvcx.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makewdsp.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makewdsp.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makewfil.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makewfil.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makewmak.vc6` & `torchjpeg-0.9.9.dev1/src/libjpeg/makewmak.vc6`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makewvcx.v16` & `torchjpeg-0.9.9.dev1/src/libjpeg/makewvcx.v16`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/makljpeg.st` & `torchjpeg-0.9.9.dev1/src/libjpeg/makljpeg.st`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/maktjpeg.st` & `torchjpeg-0.9.9.dev1/src/libjpeg/maktjpeg.st`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/missing` & `torchjpeg-0.9.9.dev1/src/libjpeg/missing`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/rdbmp.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/rdbmp.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/rdcolmap.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/rdcolmap.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/rdgif.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/rdgif.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/rdjpgcom.1` & `torchjpeg-0.9.9.dev1/src/libjpeg/rdjpgcom.1`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/rdjpgcom.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/rdjpgcom.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/rdppm.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/rdppm.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/rdrle.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/rdrle.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/rdswitch.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/rdswitch.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/rdtarga.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/rdtarga.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/structure.txt` & `torchjpeg-0.9.9.dev1/src/libjpeg/structure.txt`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/testimg.bmp` & `torchjpeg-0.9.9.dev1/src/libjpeg/testimg.bmp`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/testimg.gif` & `torchjpeg-0.9.9.dev1/src/libjpeg/testimg.gif`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/testimg.jpg` & `torchjpeg-0.9.9.dev1/src/libjpeg/testimg.jpg`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/testimg.ppm` & `torchjpeg-0.9.9.dev1/src/libjpeg/testimg.ppm`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/testimgp.jpg` & `torchjpeg-0.9.9.dev1/src/libjpeg/testimgp.jpg`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/testorig.jpg` & `torchjpeg-0.9.9.dev1/src/libjpeg/testorig.jpg`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/testprog.jpg` & `torchjpeg-0.9.9.dev1/src/libjpeg/testprog.jpg`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/transupp.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/transupp.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/transupp.h` & `torchjpeg-0.9.9.dev1/src/libjpeg/transupp.h`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/usage.txt` & `torchjpeg-0.9.9.dev1/src/libjpeg/usage.txt`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/wizard.txt` & `torchjpeg-0.9.9.dev1/src/libjpeg/wizard.txt`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/wrbmp.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/wrbmp.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/wrgif.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/wrgif.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/wrjpgcom.1` & `torchjpeg-0.9.9.dev1/src/libjpeg/wrjpgcom.1`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/wrjpgcom.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/wrjpgcom.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/wrppm.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/wrppm.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/wrrle.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/wrrle.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/libjpeg/wrtarga.c` & `torchjpeg-0.9.9.dev1/src/libjpeg/wrtarga.c`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/codec/__init__.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/codec/__init__.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/codec/codec_ops.cpp` & `torchjpeg-0.9.9.dev1/src/torchjpeg/codec/codec_ops.cpp`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/dct/__init__.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/dct/__init__.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/dct/_block.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/dct/_block.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/dct/_color.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/dct/_color.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/dct/_nn.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/dct/_nn.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/dct/_stats.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/dct/_stats.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/metrics/_psnr.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/metrics/_psnr.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/metrics/_psnrb.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/metrics/_psnrb.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/metrics/_size.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/metrics/_size.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/metrics/_ssim.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/metrics/_ssim.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/quantization/__init__.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/quantization/_quantize.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/quantization/_quantize.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/quantization/ijg.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/quantization/ijg.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/src/torchjpeg/transforms/__init__.py` & `torchjpeg-0.9.9.dev1/src/torchjpeg/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `torchjpeg-0.9.9/setup.py` & `torchjpeg-0.9.9.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=7.2.0', 'torch==1.6.0', 'torchvision==0.7.0']
 
 setup_kwargs = {
     'name': 'torchjpeg',
-    'version': '0.9.9',
+    'version': '0.9.9.dev1',
     'description': 'Utilities for JPEG data access and manipulation in pytorch',
     'long_description': '# TorchJPEG\n\n[![pipeline status](https://gitlab.com/Queuecumber/torchjpeg/badges/master/pipeline.svg)](https://gitlab.com/Queuecumber/torchjpeg/-/pipelines/latest)\n[![coverage report](https://gitlab.com/Queuecumber/torchjpeg/badges/master/coverage.svg)](https://gitlab.com/Queuecumber/torchjpeg/-/pipelines/latest)\n[![PyPI](https://img.shields.io/pypi/v/torchjpeg)](https://pypi.org/project/torchjpeg/)\n[![License](https://img.shields.io/badge/license-MIT-blue)](https://gitlab.com/Queuecumber/torchjpeg/-/blob/master/LICENSE)\n\nThis package contains a C++ extension for pytorch that interfaces with libjpeg to allow for manipulation of low-level JPEG data.\nBy using libjpeg, quantization results are guaranteed to be consistent with other applications, like image viewers or MATLAB,\nwhich use libjpeg to compress and decompress images. This is useful because JPEG images can be effected by round-off\nerrors or slight differences in the decompression procedure. Besides this, this library can be used to read and write\nDCT coefficients, functionality which is not available from other python interfaces.\n\nBesides this, the library includes many utilities related to JPEG compression, many of which are written using native pytorch code meaning\nthey can be differentiated or GPU accelerated. The library currently includes packages related to the DCT, quantization, metrics, and dataset\ntransformations.\n\n## LIBJPEG\n\nCurrently builds against: `libjpeg-9d`. libjpeg is statically linked during the build process. See [http://www.ijg.org/files/](http://www.ijg.org/files/) for libjpeg source. \nThe full libjpeg source is included with the torchjpeg source code and will be built during the install process (for a source or sdist install).\n\n## Install\n\nPackages are hosted on [pypi](https://pypi.org/project/torchjpeg/). Install using pip, note that only Linux builds are supported at the moment. \n\n```\npip install torchjpeg\n```\n\nIf there is demand for builds on other platforms it may happen in the future. Also note that the wheel is intended to be compatible with manylinux2014\nwhich means it should work on modern Linux systems, however, because of they way pytorch works, we can\'t actually build it using all of the manylinux2014\ntools. So compliance is not guaranteed and YMMV.\n\n```{warning}\ntorchjpeg is currently in pre-beta development and consists mostly of converted research code. The public facing API, including any and all names of\nparameters and functions, is subject to change at any time. We follow semver for versioning and will adhere to that before making and breaking\nchanges.\n```\n\n## Citation\n\nIf you use our code in a publication, we ask that you cite the following paper ([bibtex](http://maxehr.umiacs.io/bibtex/ehrlich2020quantization.txt)):\n\n> Max Ehrlich, Larry Davis, Ser-Nam Lim, and Abhinav Shrivastava. "Quantization Guided JPEG Artifact Correction." In Proceedings of the European Conference on Computer Vision, 2020',
     'author': 'Max Ehrlich',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://queuecumber.gitlab.io/torchjpeg',
```

### Comparing `torchjpeg-0.9.9/PKG-INFO` & `torchjpeg-0.9.9.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchjpeg
-Version: 0.9.9
+Version: 0.9.9.dev1
 Summary: Utilities for JPEG data access and manipulation in pytorch
 Home-page: https://queuecumber.gitlab.io/torchjpeg
 License: MIT
 Author: Max Ehrlich
 Requires-Python: >=3.6.1,<3.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

