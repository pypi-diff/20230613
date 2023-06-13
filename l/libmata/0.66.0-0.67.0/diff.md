# Comparing `tmp/libmata-0.66.0.tar.gz` & `tmp/libmata-0.67.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmata-0.66.0.tar", last modified: Mon Jun 12 12:08:06 2023, max compression
+gzip compressed data, was "libmata-0.67.0.tar", last modified: Tue Jun 13 15:19:01 2023, max compression
```

## Comparing `libmata-0.66.0.tar` & `libmata-0.67.0.tar`

### file list

```diff
@@ -1,423 +1,422 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-06-12 12:08:06.034110 libmata-0.66.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)  1876374 2023-06-12 12:05:00.166062 libmata-0.66.0/libmata.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-06-12 12:04:00.194025 libmata-0.66.0/libmata.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    69663 2023-06-12 12:04:00.194025 libmata-0.66.0/libmata.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.006110 libmata-0.66.0/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.006110 libmata-0.66.0/mata/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    79534 2023-06-12 12:04:00.130025 libmata-0.66.0/mata/3rdparty/args.hxx
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/catch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-06-12 12:04:00.134025 libmata-0.66.0/mata/3rdparty/catch.hpp.1.9.3
--rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-06-12 12:04:00.138025 libmata-0.66.0/mata/3rdparty/catch.hpp.2.0.1
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/catch.hpp.2.13.9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.006110 libmata-0.66.0/mata/3rdparty/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd/README
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd/RELEASE.NOTES
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.014110 libmata-0.66.0/mata/3rdparty/cudd/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)   118373 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cplusplus/testobj.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.022110 libmata-0.66.0/mata/3rdparty/cudd/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-12 12:04:00.166025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-12 12:04:00.170025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-12 12:04:00.174025 libmata-0.66.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/cudd/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/cudd/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/cudd_config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.022110 libmata-0.66.0/mata/3rdparty/cudd/dddmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/README.dddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/README.testdddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.026110 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/commands.html
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/credit.html
--rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
--rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
--rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-12 12:04:00.178025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
--rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.026110 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/0.add
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/1.add
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.max1
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.max2
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/dddmp/testdddmp.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.026110 libmata-0.66.0/mata/3rdparty/cudd/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/doc/cudd.tex.in
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-06-12 12:04:00.182025 libmata-0.66.0/mata/3rdparty/cudd/doc/phase.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.026110 libmata-0.66.0/mata/3rdparty/cudd/epd/
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/epd/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/epd/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/epd/epdInt.h
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/groups.dox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:05.998110 libmata-0.66.0/mata/3rdparty/cudd/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:05.998110 libmata-0.66.0/mata/3rdparty/cudd/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.030110 libmata-0.66.0/mata/3rdparty/cudd/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29061 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.030110 libmata-0.66.0/mata/3rdparty/cudd/mtr/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/mtr/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/mtr/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/mtr/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/mtr/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/mtr/test.groups
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/mtr/testmtr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.030110 libmata-0.66.0/mata/3rdparty/cudd/st/
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/st/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/st/st.h
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/st/test_st.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/st/testst.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.030110 libmata-0.66.0/mata/3rdparty/cudd/util/
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/cudd/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.014110 libmata-0.66.0/mata/3rdparty/cudd-min/
--rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/bnet.c
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/bnet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/chkMterm.c
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/config.h
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-12 12:04:00.142025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-12 12:04:00.146025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-12 12:04:00.150025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-12 12:04:00.154025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/dddmpUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/epdInt.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:05.998110 libmata-0.66.0/mata/3rdparty/cudd-min/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:05.998110 libmata-0.66.0/mata/3rdparty/cudd-min/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.014110 libmata-0.66.0/mata/3rdparty/cudd-min/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/ntr.c
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-06-12 12:04:00.158025 libmata-0.66.0/mata/3rdparty/cudd-min/ntr.h
--rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/ntrBddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/ntrHeap.c
--rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/ntrMflow.c
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/ntrShort.c
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/ntrZddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/st.h
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/testdddmp.c
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/testmtr.c
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/testobj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/testst.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-12 12:04:00.162025 libmata-0.66.0/mata/3rdparty/cudd-min/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.030110 libmata-0.66.0/mata/3rdparty/re2/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.030110 libmata-0.66.0/mata/3rdparty/re2/re2/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/re2/bitmap256.h
--rw-r--r--   0 runner    (1001) docker     (123)    36693 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/re2/compile.cc
--rw-r--r--   0 runner    (1001) docker     (123)    76014 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/re2/parse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/re2/perl_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/re2/pod_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    31484 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/re2/prog.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/re2/prog.h
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-12 12:04:00.186025 libmata-0.66.0/mata/3rdparty/re2/re2/re2.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/re2.h
--rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/regexp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/regexp.h
--rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/simplify.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/sparse_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/sparse_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/stringpiece.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/stringpiece.h
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/tostring.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/unicode_casefold.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/unicode_casefold.h
--rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/unicode_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/unicode_groups.h
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/re2/walker-inl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/mata/3rdparty/re2/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/util/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/util/mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/util/rune.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/util/strutil.cc
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/util/strutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/util/utf.h
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/re2/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.002110 libmata-0.66.0/mata/3rdparty/simlib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.002110 libmata-0.66.0/mata/3rdparty/simlib/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.002110 libmata-0.66.0/mata/3rdparty/simlib/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-12 12:04:00.190025 libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/mata/3rdparty/simlib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-06-12 12:04:00.194025 libmata-0.66.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-12 12:08:05.834110 libmata-0.66.0/mata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-12 12:08:05.834110 libmata-0.66.0/mata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 12:08:05.834110 libmata-0.66.0/mata/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.002110 libmata-0.66.0/mata/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/mata/include/mata/
--rw-r--r--   0 runner    (1001) docker     (123)    17278 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/afa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    21177 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/alphabet.hh
--rw-r--r--   0 runner    (1001) docker     (123)    18751 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/closed-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/inter-aut.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/mintermization.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/nfa-algorithms.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/nfa-plumbing.hh
--rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/nfa-strings.hh
--rw-r--r--   0 runner    (1001) docker     (123)    50446 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/nfa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/number-predicate.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/ord-vector.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/re2parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/rrt.hh
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/synchronized-iterator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/include/mata/util.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/mata/src/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/mata/src/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    37233 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/config.cc.in
--rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/inter-aut.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/mata/src/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/nfa/nfa-complement.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/nfa/nfa-concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/nfa/nfa-inclusion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/nfa/nfa-intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-12 12:04:00.202025 libmata-0.66.0/mata/src/nfa/nfa-universal.cc
--rw-r--r--   0 runner    (1001) docker     (123)    68257 2023-06-12 12:04:00.206025 libmata-0.66.0/mata/src/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-12 12:04:00.206025 libmata-0.66.0/mata/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-06-12 12:04:00.206025 libmata-0.66.0/mata/src/re2parser.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:08:06.034110 libmata-0.66.0/mata/src/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-06-12 12:04:00.206025 libmata-0.66.0/mata/src/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-12 12:04:00.206025 libmata-0.66.0/mata/src/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-12 12:04:00.206025 libmata-0.66.0/mata/src/strings/nfa-strings.cc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 12:04:00.194025 libmata-0.66.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-06-12 12:04:00.194025 libmata-0.66.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.454522 libmata-0.67.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-06-13 15:19:01.454522 libmata-0.67.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)  1876374 2023-06-13 15:16:38.444378 libmata-0.67.0/libmata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-06-13 15:15:54.308125 libmata-0.67.0/libmata.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    69663 2023-06-13 15:15:54.308125 libmata-0.67.0/libmata.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.438521 libmata-0.67.0/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.438521 libmata-0.67.0/mata/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    79534 2023-06-13 15:15:54.260121 libmata-0.67.0/mata/3rdparty/args.hxx
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/catch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-06-13 15:15:54.264121 libmata-0.67.0/mata/3rdparty/catch.hpp.1.9.3
+-rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-06-13 15:15:54.264121 libmata-0.67.0/mata/3rdparty/catch.hpp.2.0.1
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/catch.hpp.2.13.9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.438521 libmata-0.67.0/mata/3rdparty/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/README
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/RELEASE.NOTES
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.442521 libmata-0.67.0/mata/3rdparty/cudd/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)   118373 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cplusplus/testobj.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.446521 libmata-0.67.0/mata/3rdparty/cudd/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-13 15:15:54.288123 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/cudd_config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.446521 libmata-0.67.0/mata/3rdparty/cudd/dddmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/README.dddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/README.testdddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
+-rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-13 15:15:54.292124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.446521 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/commands.html
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/credit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
+-rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/0.add
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/1.add
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.max1
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.max2
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-13 15:15:54.296124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/dddmp/testdddmp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/cudd/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/doc/cudd.tex.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/doc/phase.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/cudd/epd/
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/epd/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/epd/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/epd/epdInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/groups.dox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.434521 libmata-0.67.0/mata/3rdparty/cudd/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.434521 libmata-0.67.0/mata/3rdparty/cudd/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/cudd/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29061 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/cudd/mtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/mtr/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/mtr/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/mtr/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/mtr/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/mtr/test.groups
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/mtr/testmtr.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/cudd/st/
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/st/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/st/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/st/test_st.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/st/testst.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/cudd/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/cudd/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.442521 libmata-0.67.0/mata/3rdparty/cudd-min/
+-rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/bnet.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/bnet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/chkMterm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-13 15:15:54.268122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-13 15:15:54.272122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-13 15:15:54.276122 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/dddmpUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/epdInt.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.430521 libmata-0.67.0/mata/3rdparty/cudd-min/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.430521 libmata-0.67.0/mata/3rdparty/cudd-min/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.442521 libmata-0.67.0/mata/3rdparty/cudd-min/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/ntr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/ntr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/ntrBddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/ntrHeap.c
+-rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/ntrMflow.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/ntrShort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/ntrZddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-13 15:15:54.280123 libmata-0.67.0/mata/3rdparty/cudd-min/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/testdddmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/testmtr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/testobj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/testst.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-13 15:15:54.284123 libmata-0.67.0/mata/3rdparty/cudd-min/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/re2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/re2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/re2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/re2/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/re2/re2/bitmap256.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36693 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/re2/re2/compile.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    76014 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/re2/re2/parse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/re2/re2/perl_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/re2/re2/pod_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31484 2023-06-13 15:15:54.300124 libmata-0.67.0/mata/3rdparty/re2/re2/prog.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/prog.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/re2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/re2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/regexp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/regexp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/simplify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/sparse_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/sparse_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/stringpiece.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/stringpiece.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/tostring.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/unicode_casefold.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/unicode_casefold.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/unicode_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/unicode_groups.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/re2/walker-inl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/re2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/util/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/util/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/util/rune.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/util/strutil.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/util/strutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/util/utf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/re2/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.434521 libmata-0.67.0/mata/3rdparty/simlib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.434521 libmata-0.67.0/mata/3rdparty/simlib/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.434521 libmata-0.67.0/mata/3rdparty/simlib/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.450522 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.454522 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.454522 libmata-0.67.0/mata/3rdparty/simlib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-06-13 15:15:54.304125 libmata-0.67.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-13 15:19:01.326520 libmata-0.67.0/mata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-13 15:19:01.326520 libmata-0.67.0/mata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 15:19:01.326520 libmata-0.67.0/mata/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.434521 libmata-0.67.0/mata/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.454522 libmata-0.67.0/mata/include/mata/
+-rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/afa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/alphabet.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/closed-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/inter-aut.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/mintermization.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/nfa-algorithms.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/nfa-plumbing.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/nfa-strings.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    43482 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/nfa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/number-predicate.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/ord-vector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/re2parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/synchronized-iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/include/mata/util.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.454522 libmata-0.67.0/mata/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/src/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.454522 libmata-0.67.0/mata/src/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    37976 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/src/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/src/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/src/config.cc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26404 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/src/inter-aut.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/src/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.454522 libmata-0.67.0/mata/src/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/src/nfa/nfa-complement.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/src/nfa/nfa-concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-13 15:15:54.312125 libmata-0.67.0/mata/src/nfa/nfa-inclusion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-13 15:15:54.316125 libmata-0.67.0/mata/src/nfa/nfa-intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-13 15:15:54.316125 libmata-0.67.0/mata/src/nfa/nfa-universal.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    75093 2023-06-13 15:15:54.316125 libmata-0.67.0/mata/src/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-06-13 15:15:54.316125 libmata-0.67.0/mata/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-06-13 15:15:54.316125 libmata-0.67.0/mata/src/re2parser.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:19:01.454522 libmata-0.67.0/mata/src/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-06-13 15:15:54.316125 libmata-0.67.0/mata/src/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-13 15:15:54.316125 libmata-0.67.0/mata/src/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-13 15:15:54.316125 libmata-0.67.0/mata/src/strings/nfa-strings.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 15:15:54.308125 libmata-0.67.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-06-13 15:15:54.308125 libmata-0.67.0/setup.py
```

### Comparing `libmata-0.66.0/PKG-INFO` & `libmata-0.67.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmata
-Version: 0.66.0
+Version: 0.67.0
 Summary: The automata library
 Home-page: https://github.com/verifit/mata
 Author: Lukáš Holík <holik@fit.vutbr.cz>, Ondřej Lengál <lengal@fit.vutbr.cz>, Martin Hruška <ihruskam@fit.vutbr.cz>, Tomáš Fiedor <ifiedortom@fit.vutbr.cz>, David Chocholatý <chocholaty.david@protonmail.com>, Juraj Síč <sicjuraj@fit.vutbr.cz>, Tomáš Vojnar <vojnar@fit.vutbr.cz>
 Author-email: lengal@fit.vutbr.cz
 License: UNKNOWN
 Keywords: automata,finite automata,alternating automata
 Platform: UNKNOWN
```

### Comparing `libmata-0.66.0/libmata.cpp` & `libmata-0.67.0/libmata.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/libmata.pxd` & `libmata-0.67.0/libmata.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/libmata.pyx` & `libmata-0.67.0/libmata.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/args.hxx` & `libmata-0.67.0/mata/3rdparty/args.hxx`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/catch.hpp` & `libmata-0.67.0/mata/3rdparty/catch.hpp`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/catch.hpp.1.9.3` & `libmata-0.67.0/mata/3rdparty/catch.hpp.1.9.3`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/catch.hpp.2.0.1` & `libmata-0.67.0/mata/3rdparty/catch.hpp.2.0.1`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/catch.hpp.2.13.9` & `libmata-0.67.0/mata/3rdparty/catch.hpp.2.13.9`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/Doxyfile.in` & `libmata-0.67.0/mata/3rdparty/cudd/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/LICENSE` & `libmata-0.67.0/mata/3rdparty/cudd/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/README` & `libmata-0.67.0/mata/3rdparty/cudd/README`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/RELEASE.NOTES` & `libmata-0.67.0/mata/3rdparty/cudd/RELEASE.NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc` & `libmata-0.67.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in` & `libmata-0.67.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cplusplus/testmulti.cc` & `libmata-0.67.0/mata/3rdparty/cudd/cplusplus/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cplusplus/testobj.cc` & `libmata-0.67.0/mata/3rdparty/cudd/cplusplus/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAPI.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddApply.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddFind.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddInv.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddIte.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddAnneal.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddApa.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddApprox.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddBddIte.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddBridge.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddCache.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddCheck.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddClip.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddCof.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddCompose.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddDecomp.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddEssent.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddExact.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddExport.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddGenCof.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddGenetic.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddGroup.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddHarwell.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddInit.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddInt.h` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddInteract.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddLCache.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddLinear.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddLiteral.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddMatMult.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddPriority.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddRead.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddRef.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddReorder.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSat.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSign.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSolve.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSplit.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddTable.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddUtil.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddWindow.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddCount.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddLin.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddPort.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddReord.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/test_cudd.test.in` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/test_cudd.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/testcudd.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd/testextra.c` & `libmata-0.67.0/mata/3rdparty/cudd/cudd/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/cudd_config.h.in` & `libmata-0.67.0/mata/3rdparty/cudd/cudd_config.h.in`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/README.dddmp` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/README.dddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/README.testdddmp` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/README.testdddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmp.h` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpInt.h` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/1.add` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/1.add`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/1.bdd` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/2.bdd` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/2.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/3.bdd` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.cnf` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.cnf`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.max1` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.max1`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4.max2` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4.max2`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/dddmp/testdddmp.c` & `libmata-0.67.0/mata/3rdparty/cudd/dddmp/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/doc/cudd.tex.in` & `libmata-0.67.0/mata/3rdparty/cudd/doc/cudd.tex.in`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/doc/phase.pdf` & `libmata-0.67.0/mata/3rdparty/cudd/doc/phase.pdf`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/epd/epd.c` & `libmata-0.67.0/mata/3rdparty/cudd/epd/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/epd/epd.h` & `libmata-0.67.0/mata/3rdparty/cudd/epd/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/epd/epdInt.h` & `libmata-0.67.0/mata/3rdparty/cudd/epd/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/groups.dox` & `libmata-0.67.0/mata/3rdparty/cudd/groups.dox`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h` & `libmata-0.67.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh` & `libmata-0.67.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/mtr/mtr.h` & `libmata-0.67.0/mata/3rdparty/cudd/mtr/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/mtr/mtrBasic.c` & `libmata-0.67.0/mata/3rdparty/cudd/mtr/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/mtr/mtrGroup.c` & `libmata-0.67.0/mata/3rdparty/cudd/mtr/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/mtr/mtrInt.h` & `libmata-0.67.0/mata/3rdparty/cudd/mtr/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/mtr/test_mtr.test.in` & `libmata-0.67.0/mata/3rdparty/cudd/mtr/test_mtr.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/mtr/testmtr.c` & `libmata-0.67.0/mata/3rdparty/cudd/mtr/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/st/st.c` & `libmata-0.67.0/mata/3rdparty/cudd/st/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/st/st.h` & `libmata-0.67.0/mata/3rdparty/cudd/st/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/st/testst.c` & `libmata-0.67.0/mata/3rdparty/cudd/st/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/cpu_stats.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/cpu_time.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/cstringstream.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/cstringstream.h` & `libmata-0.67.0/mata/3rdparty/cudd/util/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/datalimit.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/pathsearch.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/pipefork.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/prtime.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/safe_mem.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/strsav.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/texpand.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/ucbqsort.c` & `libmata-0.67.0/mata/3rdparty/cudd/util/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd/util/util.h` & `libmata-0.67.0/mata/3rdparty/cudd/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/bnet.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/bnet.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/bnet.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/bnet.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/chkMterm.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/chkMterm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/config.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/config.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cpu_stats.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cpu_time.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cstringstream.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cstringstream.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cudd.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAPI.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddAbs.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddApply.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddFind.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddInv.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddIte.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddNeg.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAddWalsh.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAndAbs.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddAnneal.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddApa.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddApprox.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddBddAbs.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddBddCorr.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddBddIte.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddBridge.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddCache.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddCheck.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddClip.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddCof.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddCompose.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddDecomp.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddEssent.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddExact.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddExport.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddGenCof.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddGenetic.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddGroup.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddHarwell.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddInit.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddInt.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddInteract.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddLCache.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddLevelQ.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddLinear.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddLiteral.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddMatMult.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddObj.cc` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddObj.hh` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddPriority.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddRead.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddRef.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddReorder.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddSat.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddSign.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddSolve.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddSplit.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddSubsetHB.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddSubsetSP.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddSymmetry.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddTable.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddUtil.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddWindow.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddCount.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddFuncs.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddGroup.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddIsop.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddLin.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddMisc.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddPort.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddReord.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddSetop.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddSymm.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/cuddZddUtil.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/datalimit.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmp.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpBinary.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpConvert.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpDbg.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpInt.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpLoad.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/dddmpUtil.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/epd.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/epd.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/epdInt.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh` & `libmata-0.67.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/main.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/main.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/mtr.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/mtrBasic.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/mtrGroup.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/mtrInt.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/ntr.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/ntr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/ntr.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/ntr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/ntrBddTest.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/ntrBddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/ntrHeap.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/ntrHeap.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/ntrMflow.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/ntrMflow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/ntrShort.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/ntrShort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/ntrZddTest.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/ntrZddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/pathsearch.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/pipefork.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/prtime.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/safe_mem.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/st.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/st.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/strsav.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/testcudd.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/testdddmp.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/testextra.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/testmtr.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/testmulti.cc` & `libmata-0.67.0/mata/3rdparty/cudd-min/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/testobj.cc` & `libmata-0.67.0/mata/3rdparty/cudd-min/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/testst.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/texpand.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/ucbqsort.c` & `libmata-0.67.0/mata/3rdparty/cudd-min/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/cudd-min/util.h` & `libmata-0.67.0/mata/3rdparty/cudd-min/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/CONTRIBUTORS` & `libmata-0.67.0/mata/3rdparty/re2/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/LICENSE` & `libmata-0.67.0/mata/3rdparty/re2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/bitmap256.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/bitmap256.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/compile.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/compile.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/parse.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/parse.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/perl_groups.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/perl_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/pod_array.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/pod_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/prog.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/prog.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/prog.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/prog.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/re2.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/re2.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/re2.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/re2.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/regexp.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/regexp.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/regexp.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/regexp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/simplify.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/simplify.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/sparse_array.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/sparse_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/sparse_set.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/sparse_set.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/stringpiece.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/stringpiece.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/stringpiece.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/tostring.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/tostring.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/unicode_casefold.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/unicode_casefold.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/unicode_casefold.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/unicode_casefold.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/unicode_groups.cc` & `libmata-0.67.0/mata/3rdparty/re2/re2/unicode_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/unicode_groups.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/unicode_groups.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/re2/walker-inl.h` & `libmata-0.67.0/mata/3rdparty/re2/re2/walker-inl.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/util/logging.h` & `libmata-0.67.0/mata/3rdparty/re2/util/logging.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/util/mutex.h` & `libmata-0.67.0/mata/3rdparty/re2/util/mutex.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/util/rune.cc` & `libmata-0.67.0/mata/3rdparty/re2/util/rune.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/util/strutil.cc` & `libmata-0.67.0/mata/3rdparty/re2/util/strutil.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/util/utf.h` & `libmata-0.67.0/mata/3rdparty/re2/util/utf.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/re2/util/util.h` & `libmata-0.67.0/mata/3rdparty/re2/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh` & `libmata-0.67.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc` & `libmata-0.67.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/LICENSE` & `libmata-0.67.0/mata/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/README.md` & `libmata-0.67.0/mata/README.md`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/include/mata/afa.hh` & `libmata-0.67.0/mata/include/mata/afa.hh`

 * *Files 18% similar despite different names*

```diff
@@ -11,50 +11,44 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#ifndef _MATA_AFA_HH_
-#define _MATA_AFA_HH_
+#ifndef MATA_AFA_HH_
+#define MATA_AFA_HH_
 
 #include <algorithm>
 #include <cassert>
 #include <cstdint>
 #include <set>
 #include <unordered_map>
 #include <unordered_set>
 #include <vector>
 #include <memory>
 
-// MATA headers
-#include <mata/alphabet.hh>
-#include <mata/nfa.hh>
-#include <mata/parser.hh>
-#include <mata/util.hh>
-#include <mata/ord-vector.hh>
-#include <mata/closed-set.hh>
+#include "mata/alphabet.hh"
+#include "mata/nfa.hh"
+#include "mata/parser.hh"
+#include "mata/util.hh"
+#include "mata/ord-vector.hh"
+#include "mata/closed-set.hh"
 
-namespace Mata
-{
 /**
  * Alternating Finite Automata including structures, transitions and algorithms.
  *
  * In particular, this includes:
  *   1. Structures (Automaton, Transitions, Results),
  *   2. Algorithms (operations, checks, tests),
  *   3. Constructions.
  */
-namespace Afa
-{
+namespace Mata::Afa {
 extern const std::string TYPE_AFA;
 
-// START OF THE DECLARATIONS
-
 using State = Mata::Nfa::State;
 
 template<typename T> using OrdVec = Mata::Util::OrdVector<T>;
 
 using Node = OrdVec<State>;
 using Nodes = OrdVec<Node>;
 
@@ -81,397 +75,371 @@
 * a formula can be converted to the DNF, we can represent it as an ordered vector
 * of nodes. The ordered vector represents a set of disjuncts. Each node corresponds
 * to a single disjunct of a formula in DNF (states connected by conjunctions).
 *
 */
 struct Trans
 {
-	State src; // source state
-	Symbol symb; // transition symbol
-	Nodes dst; // a vector of vectors of states
-
-	Trans() : src(), symb(), dst() { }
-	Trans(State src, Symbol symb, Node dst) : src(src), symb(symb), dst(Nodes(dst)) { }
-	Trans(State src, Symbol symb, Nodes dst) : src(src), symb(symb), dst(dst) { }
-
-	bool operator==(const Trans& rhs) const
-	{ // {{{
-		return src == rhs.src && symb == rhs.symb && dst == rhs.dst ;
-	} // operator== }}}
-	bool operator!=(const Trans& rhs) const { return !this->operator==(rhs); }
+    State src; // source state
+    Symbol symb; // transition symbol
+    Nodes dst; // a vector of vectors of states
+
+    Trans() : src(), symb(), dst() { }
+    Trans(State src, Symbol symb, Node dst) : src(src), symb(symb), dst(Nodes(dst)) { }
+    Trans(State src, Symbol symb, Nodes dst) : src(src), symb(symb), dst(dst) { }
+
+    bool operator==(const Trans& rhs) const
+    { // {{{
+        return src == rhs.src && symb == rhs.symb && dst == rhs.dst ;
+    } // operator== }}}
+    bool operator!=(const Trans& rhs) const { return !this->operator==(rhs); }
 
 }; // struct Trans
 
 using TransList = std::vector<Trans>;
 using TransRelation = std::vector<TransList>;
 
 /* A tuple (result_node, precondition). The node result_node is a predecessor
 * of a given node 'N' if the node 'precondition' is its subset. */
 struct InverseResults{
 
-	Node result_node{};
-	Node precondition{};
+    Node result_node{};
+    Node precondition{};
 
-	InverseResults() : result_node(), precondition() { }
-	InverseResults(State state, Node precondition) : result_node(Node(state)),
-	precondition(precondition) { }
-	InverseResults(Node result_node, Node precondition) : result_node(result_node),
-	precondition(precondition) { }
-
-	bool operator==(InverseResults rhs) const
-	{ // {{{
-		return precondition == rhs.precondition && result_node == rhs.result_node;
-	} // operator== }}}
-
-	bool operator!=(InverseResults rhs) const
-	{ // {{{
-		return !this->operator==(rhs);
-	} // operator!= }}}
-
-	bool operator<(InverseResults rhs) const
-	{ // {{{
-		return precondition < rhs.precondition ||
-		(precondition == rhs.precondition && result_node < rhs.result_node);
-	} // operator< }}}
+    InverseResults() : result_node(), precondition() { }
+    InverseResults(State state, Node precondition) : result_node(Node(state)),
+    precondition(precondition) { }
+    InverseResults(Node result_node, Node precondition) : result_node(result_node),
+    precondition(precondition) { }
+
+    bool operator==(const InverseResults& rhs) const
+    { // {{{
+        return precondition == rhs.precondition && result_node == rhs.result_node;
+    } // operator== }}}
+
+    bool operator!=(const InverseResults& rhs) const
+    { // {{{
+        return !this->operator==(rhs);
+    } // operator!= }}}
+
+    bool operator<(const InverseResults& rhs) const
+    { // {{{
+        return precondition < rhs.precondition ||
+        (precondition == rhs.precondition && result_node < rhs.result_node);
+    } // operator< }}}
 
 }; // struct InverseResults
 
-/*
-* A tuple (state, symb, inverseResults). The structure inverseResults contains tuples (inverseResult,
-* precondition). If a node is a subset of 'precondition', the 'inverseResult' is a predecessor
-* of the given node which is accessible through the symbol 'symb'.
-* The state 'state' is always part of all 'preconditions' and it is a minimal element of them.
-*/
-struct InverseTrans{
-
-	State state;
-	Symbol symb;
-	std::vector<InverseResults> inverseResults{};
-
-	InverseTrans() : symb(), inverseResults() { }
-	InverseTrans(Symbol symb) : symb(symb), inverseResults(std::vector<InverseResults>()) { }
-	InverseTrans(Symbol symb, InverseResults inverseResults_) : symb(symb)
-	{ inverseResults.push_back(inverseResults_); }
-	InverseTrans(State state, Symbol symb, InverseResults inverseResults_) : state(state), symb(symb)
-	{ inverseResults.push_back(inverseResults_); }
-
+/**
+ * A tuple (state, symb, inverseResults). The structure inverseResults contains tuples (inverseResult,
+ * precondition). If a node is a subset of 'precondition', the 'inverseResult' is a predecessor
+ * of the given node which is accessible through the symbol 'symb'.
+ * The state 'state' is always part of all 'preconditions' and it is a minimal element of them.
+ */
+struct InverseTrans {
+    State state;
+    Symbol symb;
+    std::vector<InverseResults> inverseResults{};
+
+    InverseTrans() : symb(), inverseResults() { }
+    InverseTrans(Symbol symb) : symb(symb), inverseResults(std::vector<InverseResults>()) { }
+    InverseTrans(Symbol symb, InverseResults inverseResults_) : symb(symb) { inverseResults.push_back(inverseResults_); }
+    InverseTrans(State state, Symbol symb, InverseResults inverseResults_)
+        : state(state), symb(symb) { inverseResults.push_back(inverseResults_); }
 }; // struct InverseTrans
 
 using InverseTransRelation = std::vector<std::vector<InverseTrans>>;
 
 struct Afa;
 
 /// serializes Afa into a ParsedSection
 Mata::Parser::ParsedSection serialize(
-	const Afa&                aut,
-	const SymbolToStringMap*  symbol_map = nullptr,
-	const StateToStringMap*   state_map = nullptr);
+    const Afa&                aut,
+    const SymbolToStringMap*  symbol_map = nullptr,
+    const StateToStringMap*   state_map = nullptr);
 
 
 ///  An AFA
 struct Afa
 { // {{{
 private:
     TransRelation transitionrelation{};
     InverseTransRelation inverseTransRelation{};
 
 public:
 
-	Afa() : transitionrelation(), inverseTransRelation() {}
+    Afa() : transitionrelation(), inverseTransRelation() {}
 
-	explicit Afa(const unsigned long num_of_states, const Nodes& initial_states = Nodes{},
-		         const StateSet& final_states = StateSet{})
-		: transitionrelation(num_of_states), inverseTransRelation(num_of_states),
-		initialstates(initial_states), finalstates(final_states) {}
+    explicit Afa(const unsigned long num_of_states, const Nodes& initial_states = Nodes{},
+                 const StateSet& final_states = StateSet{})
+        : transitionrelation(num_of_states), inverseTransRelation(num_of_states),
+        initialstates(initial_states), finalstates(final_states) {}
 
 public:
 
-	Nodes initialstates = {};
-	StateSet finalstates = {};
+    Nodes initialstates = {};
+    StateSet finalstates = {};
 
-	State add_new_state(void);
+    State add_new_state();
 
-	auto get_num_of_states() const { return transitionrelation.size(); }
+    auto get_num_of_states() const { return transitionrelation.size(); }
 
-	void add_initial(State state) { this->initialstates.insert(Node({state})); }
-	void add_initial(Node node) { this->initialstates.insert(node); }
-	void add_initial(const std::vector<State> vec)
-	{ // {{{
-		Node node{};
-		for (const State& st : vec) { node.insert(st); }
-		this->initialstates.insert(node);
-	} // }}}
-	bool has_initial(State state) const
-	{ // {{{
-		return has_initial(Node({state}));
-	} // }}}
-	bool has_initial(Node node) const
-	{ // {{{
-		return StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1,
-		initialstates).contains(node);
-	} // }}}
-	void add_final(State state) { this->finalstates.insert(state); }
-	void add_final(const std::vector<State> vec)
-	{ // {{{
-		for (const State& st : vec) { this->add_final(st); }
-	} // }}}
-	bool has_final(State state) const
-	{ // {{{
-		return Mata::Util::haskey(this->finalstates, state);
-	} // }}}
-
-	void add_trans(const Trans& trans);
-	void add_trans(State src, Symbol symb, State dst)
-	{ // {{{
-		this->add_trans({src, symb, Nodes(Node(dst))});
-	} // }}}
-	void add_trans(State src, Symbol symb, Node dst)
-	{ // {{{
-		this->add_trans({src, symb, Nodes(dst)});
-	} // }}}
-	void add_trans(State src, Symbol symb, Nodes dst)
-	{ // {{{
-		this->add_trans({src, symb, dst});
-	} // }}}
-
-	void add_inverse_trans(const Trans& trans);
-	void add_inverse_trans(State src, Symbol symb, Node dst)
-	{ // {{{
-		this->add_inverse_trans({src, symb, Nodes(dst)});
-	} // }}}
-	void add_inverse_trans(State src, Symbol symb, Nodes dst)
-	{ // {{{
-		this->add_inverse_trans({src, symb, dst});
-	} // }}}
-
-	std::vector<InverseResults> perform_inverse_trans(State src, Symbol symb) const;
-	std::vector<InverseResults> perform_inverse_trans(Node src, Symbol symb) const;
-
-	bool has_trans(const Trans& trans) const;
-	bool has_trans(State src, Symbol symb, Node dst) const
-	{ // {{{
-		return this->has_trans({src, symb, Nodes(dst)});
-	} // }}}
-	bool has_trans(State src, Symbol symb, Nodes dst) const
-	{ // {{{
-		return this->has_trans({src, symb, dst});
-	} // }}}
-
-	std::vector<Trans> get_trans_from_state(State state) const;
-	Trans get_trans_from_state(State state, Symbol symbol) const;
-
-	bool trans_empty() const {!transitionrelation.size();};// no transitions
-	size_t trans_size() const;/// number of transitions; has linear time complexity
-
-
-	StateClosedSet post(State state, Symbol symb) const;
-	StateClosedSet post(Node node, Symbol symb) const;
-	StateClosedSet post(Nodes nodes, Symbol symb) const;
-	StateClosedSet post(StateClosedSet closed_set, Symbol symb) const;
-
-	StateClosedSet post(Node node) const;
-	StateClosedSet post(Nodes nodes) const;
-
-	StateClosedSet post(StateClosedSet closed_set) const;
-
-	StateClosedSet pre(Node node, Symbol symb) const;
-	StateClosedSet pre(State state, Symbol symb) const {return pre(Node(state), symb);};
-	StateClosedSet pre(Nodes nodes, Symbol symb) const;
-	StateClosedSet pre(StateClosedSet closed_set, Symbol symb) const;
-
-	StateClosedSet pre(Node node) const;
-	StateClosedSet pre(Nodes nodes) const;
-
-	StateClosedSet pre(StateClosedSet closed_set) const {return pre(closed_set.antichain());};
-
-	StateClosedSet get_initial_nodes(void) const
-	{
-		StateClosedSet result = StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1);
-		for(const auto& node : initialstates)
-		{
-			result.insert(node);
-		}
-		return result;
-	}
-
-	StateClosedSet get_non_initial_nodes(void) const {return StateClosedSet(upward_closed_set,
-	0, transitionrelation.size()-1, initialstates).complement();};
-	StateClosedSet get_final_nodes(void) const {return StateClosedSet(downward_closed_set,
-	0, transitionrelation.size()-1, finalstates);};
-	StateClosedSet get_non_final_nodes(void) const;
+    void add_initial(State state) { this->initialstates.insert(Node({state})); }
+    void add_initial(Node node) { this->initialstates.insert(node); }
+    void add_initial(const std::vector<State>& vec)
+    { // {{{
+        Node node{};
+        for (const State& st : vec) { node.insert(st); }
+        this->initialstates.insert(node);
+    } // }}}
+    bool has_initial(State state) const
+    { // {{{
+        return has_initial(Node({state}));
+    } // }}}
+    bool has_initial(Node node) const
+    { // {{{
+        return StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1, initialstates).contains(node);
+    } // }}}
+    void add_final(State state) { this->finalstates.insert(state); }
+    void add_final(const std::vector<State> vec)
+    { // {{{
+        for (const State& st : vec) { this->add_final(st); }
+    } // }}}
+    bool has_final(State state) const
+    { // {{{
+        return Mata::Util::haskey(this->finalstates, state);
+    } // }}}
+
+    void add_trans(const Trans& trans);
+    void add_trans(State src, Symbol symb, State dst)
+    { // {{{
+        this->add_trans({src, symb, Nodes(Node(dst))});
+    } // }}}
+    void add_trans(State src, Symbol symb, Node dst)
+    { // {{{
+        this->add_trans({src, symb, Nodes(dst)});
+    } // }}}
+    void add_trans(State src, Symbol symb, Nodes dst)
+    { // {{{
+        this->add_trans({src, symb, dst});
+    } // }}}
+
+    void add_inverse_trans(const Trans& trans);
+    void add_inverse_trans(State src, Symbol symb, Node dst)
+    { // {{{
+        this->add_inverse_trans({src, symb, Nodes(dst)});
+    } // }}}
+    void add_inverse_trans(State src, Symbol symb, Nodes dst)
+    { // {{{
+        this->add_inverse_trans({src, symb, dst});
+    } // }}}
+
+    std::vector<InverseResults> perform_inverse_trans(State src, Symbol symb) const;
+    std::vector<InverseResults> perform_inverse_trans(Node src, Symbol symb) const;
+
+    bool has_trans(const Trans& trans) const;
+    bool has_trans(State src, Symbol symb, Node dst) const
+    { // {{{
+        return this->has_trans({src, symb, Nodes(dst)});
+    } // }}}
+    bool has_trans(State src, Symbol symb, Nodes dst) const
+    { // {{{
+        return this->has_trans({src, symb, dst});
+    } // }}}
+
+    std::vector<Trans> get_trans_from_state(State state) const;
+    Trans get_trans_from_state(State state, Symbol symbol) const;
+
+    bool trans_empty() const {!transitionrelation.size();};// no transitions
+    size_t trans_size() const;/// number of transitions; has linear time complexity
+
+
+    StateClosedSet post(State state, Symbol symb) const;
+    StateClosedSet post(Node node, Symbol symb) const;
+    StateClosedSet post(Nodes nodes, Symbol symb) const;
+    StateClosedSet post(StateClosedSet closed_set, Symbol symb) const;
+
+    StateClosedSet post(Node node) const;
+    StateClosedSet post(Nodes nodes) const;
+
+    StateClosedSet post(StateClosedSet closed_set) const;
+
+    StateClosedSet pre(Node node, Symbol symb) const;
+    StateClosedSet pre(State state, Symbol symb) const { return pre(Node(state), symb); };
+    StateClosedSet pre(Nodes nodes, Symbol symb) const;
+    StateClosedSet pre(StateClosedSet closed_set, Symbol symb) const;
+
+    StateClosedSet pre(Node node) const;
+    StateClosedSet pre(Nodes nodes) const;
+
+    StateClosedSet pre(StateClosedSet closed_set) const { return pre(closed_set.antichain()); };
+
+    StateClosedSet get_initial_nodes() const;
+
+    StateClosedSet get_non_initial_nodes() const {
+        return StateClosedSet{ upward_closed_set, 0, transitionrelation.size()-1, initialstates }.complement();
+    };
+    StateClosedSet get_final_nodes() const {
+        return { downward_closed_set, 0, transitionrelation.size()-1, finalstates };
+    };
+
+    /**
+     * @brief This function returns an upward-closed set of all the nodes which are non-final.
+     * @return Closed set of non-final nodes.
+     */
+    StateClosedSet get_non_final_nodes() const;
 
 }; // Afa }}}
 
-
 /// a wrapper encapsulating @p Afa for higher-level use
 struct AfaWrapper
 { // {{{
-	/// the AFA
-	Afa afa;
+    /// the AFA
+    Afa afa;
 
-	/// the alphabet
-	Alphabet* alphabet;
+    /// the alphabet
+    Alphabet* alphabet;
 
-	/// mapping of state names (as strings) to their numerical values
-	StringToStateMap state_dict;
+    /// mapping of state names (as strings) to their numerical values
+    StringToStateMap state_dict;
 }; // AfaWrapper }}}
 
-
 /// Do the automata have disjoint sets of states?
 bool are_state_disjoint(const Afa& lhs, const Afa& rhs);
 /// Is the language of the automaton empty?
 bool is_lang_empty(const Afa& aut, Path* cex = nullptr);
 bool is_lang_empty_cex(const Afa& aut, Word* cex);
 
 bool antichain_concrete_forward_emptiness_test_old(const Afa& aut);
 bool antichain_concrete_backward_emptiness_test_old(const Afa& aut);
 
 bool antichain_concrete_forward_emptiness_test_new(const Afa& aut);
 bool antichain_concrete_backward_emptiness_test_new(const Afa& aut);
 
-
 /// Retrieves the states reachable from initial states
 std::unordered_set<State> get_fwd_reach_states(const Afa& aut);
 
 /// Is the language of the automaton universal?
 bool is_universal(
-	const Afa&         aut,
-	const Alphabet&    alphabet,
-	Word*              cex = nullptr,
-	const StringDict&  params = {{"algorithm", "antichains"}});
+    const Afa&         aut,
+    const Alphabet&    alphabet,
+    Word*              cex = nullptr,
+    const StringDict&  params = {{"algorithm", "antichains"}});
 
 inline bool is_universal(
-	const Afa&         aut,
-	const Alphabet&    alphabet,
-	const StringDict&  params)
+    const Afa&         aut,
+    const Alphabet&    alphabet,
+    const StringDict&  params)
 { // {{{
-	return is_universal(aut, alphabet, nullptr, params);
+    return is_universal(aut, alphabet, nullptr, params);
 } // }}}
 
 /// Does the language of the automaton contain epsilon?
 bool accepts_epsilon(const Afa& aut);
 
 /// Checks inclusion of languages of two automata (smaller <= bigger)?
 bool is_incl(
-	const Afa&         smaller,
-	const Afa&         bigger,
-	const Alphabet&    alphabet,
-	Word*              cex = nullptr,
-	const StringDict&  params = {{"algorithm", "antichains"}});
+    const Afa&         smaller,
+    const Afa&         bigger,
+    const Alphabet&    alphabet,
+    Word*              cex = nullptr,
+    const StringDict&  params = {{"algorithm", "antichains"}});
 
 inline bool is_incl(
-	const Afa&         smaller,
-	const Afa&         bigger,
-	const Alphabet&    alphabet,
-	const StringDict&  params)
+    const Afa&         smaller,
+    const Afa&         bigger,
+    const Alphabet&    alphabet,
+    const StringDict&  params)
 { // {{{
-	return is_incl(smaller, bigger, alphabet, nullptr, params);
+    return is_incl(smaller, bigger, alphabet, nullptr, params);
 } // }}}
 
 /// Compute union of a pair of automata
 /// Assumes that sets of states of lhs, rhs, and result are disjoint
 void union_norename(
-	Afa*        result,
-	const Afa&  lhs,
-	const Afa&  rhs);
+    Afa*        result,
+    const Afa&  lhs,
+    const Afa&  rhs);
 
 /// Compute union of a pair of automata
 inline Afa union_norename(
-	const Afa&  lhs,
-	const Afa&  rhs)
+    const Afa&  lhs,
+    const Afa&  rhs)
 { // {{{
-	Afa result;
-	union_norename(&result, lhs, rhs);
-	return result;
+    Afa result;
+    union_norename(&result, lhs, rhs);
+    return result;
 } // union_norename }}}
 
 /// Compute union of a pair of automata
 /// The states of the automata do not need to be disjoint; renaming will be done
 Afa union_rename(
-	const Afa&  lhs,
-	const Afa&  rhs);
+    const Afa&  lhs,
+    const Afa&  rhs);
 
 
 /// makes the transition relation complete
 void make_complete(
-	Afa*             aut,
-	const Alphabet&  alphabet,
-	State            sink_state);
+    Afa*             aut,
+    const Alphabet&  alphabet,
+    State            sink_state);
 
 /// Reverting the automaton
 void revert(Afa* result, const Afa& aut);
 
-inline Afa revert(const Afa& aut)
-{ // {{{
-	Afa result;
-	revert(&result, aut);
-	return result;
-} // revert }}}
+inline Afa revert(const Afa& aut) {
+    Afa result;
+    revert(&result, aut);
+    return result;
+}
 
 /// Removing epsilon transitions
 void remove_epsilon(Afa* result, const Afa& aut, Symbol epsilon);
 
-inline Afa remove_epsilon(const Afa& aut, Symbol epsilon)
-{ // {{{
-	Afa result;
-	remove_epsilon(&result, aut, epsilon);
-	return result;
-} // }}}
-
+inline Afa remove_epsilon(const Afa& aut, Symbol epsilon) { return remove_epsilon(aut, epsilon); }
 
 /// Minimizes an AFA.  The method can be set using @p params
 void minimize(
-	Afa*               result,
-	const Afa&         aut,
-	const StringDict&  params = {});
+    Afa*               result,
+    const Afa&         aut,
+    const StringDict&  params = {});
 
 
 inline Afa minimize(
-	const Afa&         aut,
-	const StringDict&  params = {})
+    const Afa&         aut,
+    const StringDict&  params = {})
 { // {{{
-	Afa result;
-	minimize(&result, aut, params);
-	return result;
+    Afa result;
+    minimize(&result, aut, params);
+    return result;
 } // minimize }}}
 
 
 /// Test whether an automaton is deterministic, i.e., whether it has exactly
 /// one initial state and every state has at most one outgoing transition over
 /// every symbol.  Checks the whole automaton, not only the reachable part
 bool is_deterministic(const Afa& aut);
 
 /// Test for automaton completeness wrt an alphabet.  An automaton is complete
 /// if every reachable state has at least one outgoing transition over every
 /// symbol.
 bool is_complete(const Afa& aut, const Alphabet& alphabet);
 
 /** Loads an automaton from Parsed object */
-Afa construct(
-	    const Mata::Parser::ParsedSection&   parsec,
-	    Alphabet*                            alphabet,
-	    StringToStateMap*                    state_map = nullptr);
-/**
- * Loads automaton from intermediate automaton
- */
-Afa construct(
-        const Mata::IntermediateAut&         inter_aut,
-        Alphabet*                            alphabet,
-        StringToStateMap*                    state_map = nullptr);
+Afa construct(const Mata::Parser::ParsedSection& parsec, Alphabet* alphabet, StringToStateMap* state_map = nullptr);
+/** Loads automaton from intermediate automaton */
+Afa construct(const Mata::IntermediateAut& inter_aut, Alphabet* alphabet, StringToStateMap* state_map = nullptr);
 
 /**
- * Loads automaton from parsed object (either ParsedSection or Intermediate automaton.
+ * @brief Loads automaton from parsed object (either ParsedSection or Intermediate automaton.
+ *
  * If user does not provide symbol map or state map, it allocates its own ones.
  */
 template <class ParsedObject>
-Afa construct(
-        const ParsedObject&                  parsed,
-        StringToSymbolMap*                   symbol_map = nullptr,
-        StringToStateMap*                    state_map = nullptr)
-{ // {{{
+Afa construct(const ParsedObject& parsed, StringToSymbolMap* symbol_map = nullptr, StringToStateMap* state_map = nullptr) {
     StringToSymbolMap tmp_symbol_map;
     if (symbol_map) {
         tmp_symbol_map = *symbol_map;
     }
     Mata::OnTheFlyAlphabet alphabet(tmp_symbol_map);
 
     Afa aut = construct(parsed, &alphabet, state_map);
@@ -479,23 +447,18 @@
     if (symbol_map) {
         *symbol_map = alphabet.get_symbol_map();
     }
     return aut;
 }
 
 /** Loads an automaton from Parsed object */
-template <class ParsedObject>
-void construct(
-        Afa*                                 result,
-        const ParsedObject&                  parsed,
-        StringToSymbolMap*                   symbol_map = nullptr,
-        StringToStateMap*                    state_map = nullptr)
-{ // {{{
+template <class ParsedObject> void construct(Afa* result, const ParsedObject& parsed,
+    StringToSymbolMap* symbol_map = nullptr, StringToStateMap* state_map = nullptr) {
     *result = construct(parsed, symbol_map, state_map);
-} // construct }}}
+}
 
 /**
  * @brief  Obtains a word corresponding to a path in an automaton (or sets a flag)
  *
  * Returns a word that is consistent with @p path of states in automaton @p
  * aut, or sets a flag to @p false if such a word does not exist.  Note that
  * there may be several words with the same path (in case some pair of states
@@ -506,56 +469,35 @@
  *
  * @returns  A pair (word, bool) where if @p bool is @p true, then @p word is a
  *           word consistent with @p path, and if @p bool is @p false, this
  *           denotes that the path is invalid in @p aut
  */
 std::pair<Word, bool> get_word_for_path(const Afa& aut, const Path& path);
 
-
 /// Checks whether a string is in the language of an automaton
 bool is_in_lang(const Afa& aut, const Word& word);
 
 /// Checks whether the prefix of a string is in the language of an automaton
 bool is_prfx_in_lang(const Afa& aut, const Word& word);
 
-/** Encodes a vector of strings (each corresponding to one symbol) into a
- *  @c Word instance
- */
-inline Word encode_word(
-	const StringToSymbolMap&         symbol_map,
-	const std::vector<std::string>&  input)
-{ // {{{
-	Word result;
-	for (auto str : input) { result.insert(symbol_map.at(str)); }
-	return result;
-} // encode_word }}}
+/** Encodes a vector of strings (each corresponding to one symbol) into a @c Word instance. */
+inline Word encode_word(const StringToSymbolMap& symbol_map, const std::vector<std::string>& input);
 
-/// operator<<
 std::ostream& operator<<(std::ostream& os, const Afa& afa);
 
 /// global constructor to be called at program startup (from vm-dispatch)
 void init();
 
-// CLOSING NAMESPACES AND GUARDS
-} /* Afa */
-} /* Mata */
+} // namespace Mata::Afa.
 
-namespace std
-{ // {{{
-template <>
-struct hash<Mata::Afa::Trans>
-{
-	inline size_t operator()(const Mata::Afa::Trans& trans) const
-	{
-		size_t accum = std::hash<Mata::Afa::State>{}(trans.src);
-		accum = Mata::Util::hash_combine(accum, trans.symb);
-		accum = Mata::Util::hash_combine(accum, trans.dst);
-		return accum;
-	}
+namespace std {
+
+template <> struct hash<Mata::Afa::Trans> {
+    inline size_t operator()(const Mata::Afa::Trans& trans) const;
 };
 
 std::ostream& operator<<(std::ostream& os, const Mata::Afa::Trans& trans);
 std::ostream& operator<<(std::ostream& os, const Mata::Afa::AfaWrapper& afa_wrap);
-} // std }}}
 
+} // namespace std.
 
-#endif /* _MATA_AFA_HH_ */
+#endif /* MATA_AFA_HH_ */
```

### Comparing `libmata-0.66.0/mata/include/mata/alphabet.hh` & `libmata-0.67.0/mata/include/mata/alphabet.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,519 +1,389 @@
-/* alphabet.hh -- File containing alphabets for automata
+/* alphabet.hh -- File containing alphabets for automata.
  *
  * This file is a part of libmata.
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#ifndef _MATA_ALPHABET_HH
-#define _MATA_ALPHABET_HH
+#ifndef MATA_ALPHABET_HH
+#define MATA_ALPHABET_HH
 
 #include <forward_list>
 #include <string>
+#include <utility>
 
-#include <mata/util.hh>
-#include <mata/ord-vector.hh>
+#include "mata/util.hh"
+#include "mata/ord-vector.hh"
 
 namespace Mata {
-        using Symbol = unsigned;
-        using StringToSymbolMap = std::unordered_map<std::string, Symbol>;
 
-         /**
-          * The abstract interface for NFA alphabets.
-          */
-        class Alphabet {
-        public:
-            /// translates a string into a symbol
-            virtual Symbol translate_symb(const std::string &symb) = 0;
-
-            /**
-             * Translate sequence of symbol names to sequence of their respective values.
-             */
-            virtual std::vector<Symbol> translate_word(const std::vector<std::string>& word) const {
-                (void)word;
-                throw std::runtime_error("Unimplemented");
-            }
-
-            /**
-             * @brief Translate internal @p symbol representation back to its original string name.
-             *
-             * Throws an exception when the @p symbol is missing in the alphabet.
-             * @param[in] symbol Symbol to translate.
-             * @return @p symbol original name.
-             */
-            virtual std::string reverse_translate_symbol(Symbol symbol) const = 0;
-
-            /// also translates strings to symbols
-            Symbol operator[](const std::string &symb) { return this->translate_symb(symb); }
-
-            /**
-             * @brief Get a set of all symbols in the alphabet.
-             *
-             * The result does not have to equal the list of symbols in the automaton using this alphabet.
-             */
-            virtual Util::OrdVector<Symbol> get_alphabet_symbols() const { // {{{
-                throw std::runtime_error("Unimplemented");
-            } // }}}
-
-            /// complement of a set of symbols wrt the alphabet
-            virtual Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const { // {{{
-                (void) symbols;
-                throw std::runtime_error("Unimplemented");
-            } // }}}
-
-            virtual ~Alphabet() = default;
-
-            /**
-             * @brief Check whether two alphabets are equal.
-             *
-             * In general, two alphabets are equal if and only if they are of the same class instance.
-             * @param other_alphabet The other alphabet to compare with for equality.
-             * @return True if equal, false otherwise.
-             */
-            virtual bool is_equal(const Alphabet &other_alphabet) const {
-                return address() == other_alphabet.address();
-            }
-
-            /**
-             * @brief Check whether two alphabets are equal.
-             *
-             * In general, two alphabets are equal if and only if they are of the same class instance.
-             * @param other_alphabet The other alphabet to compare with for equality.
-             * @return True if equal, false otherwise.
-             */
-            virtual bool is_equal(const Alphabet *const other_alphabet) const {
-                return address() == other_alphabet->address();
-            }
-
-            bool operator==(const Alphabet &) const = delete;
-
-        protected:
-            virtual const void *address() const { return this; }
-        }; // class Alphabet.
-
-        /**
-        * Direct alphabet (also identity alphabet or integer alphabet) using integers as symbols.
-        *
-        * This alphabet presumes that all integers are valid symbols.
-        * Therefore, calling member functions get_complement() and get_alphabet_symbols() makes no sense in this context and the methods
-        *  will throw exceptions warning about the inappropriate use of IntAlphabet. If one needs these functions, they should
-        *  use OnTheFlyAlphabet instead of IntAlphabet.
-        */
-        class IntAlphabet : public Alphabet {
-        public:
-            IntAlphabet() : alphabet_instance(IntAlphabetSingleton::get()) {}
-
-            Symbol translate_symb(const std::string &symb) override {
-                Symbol symbol;
-                std::istringstream stream{ symb };
-                stream >> symbol;
-                if (stream.fail() || !stream.eof()) {
-                    throw std::runtime_error("Cannot translate string '" + symb + "' to symbol.");
-                }
-                return symbol;
-            }
-
-            std::string reverse_translate_symbol(Symbol symbol) const override {
-                return std::to_string(symbol);
-            }
-
-            Util::OrdVector<Symbol> get_alphabet_symbols() const override {
-                throw std::runtime_error("Nonsensical use of get_alphabet_symbols() on IntAlphabet.");
-            }
-
-            Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const override {
-                (void) symbols;
-                throw std::runtime_error("Nonsensical use of get_complement() on IntAlphabet.");
-            }
-
-            IntAlphabet(const IntAlphabet &) = default;
-
-            IntAlphabet &operator=(const IntAlphabet &int_alphabet) = delete;
-
-        protected:
-            const void *address() const override { return &alphabet_instance; }
-
-        private:
-            /**
-             * Singleton class implementing integer alphabet_instance for class IntAlphabet.
-             *
-             * Users have to use IntAlphabet instead which provides interface identical to other alphabets and can be used in
-             *  places where an instance of the abstract class Alphabet is required.
-             */
-            class IntAlphabetSingleton {
-            public:
-                static IntAlphabetSingleton &get() {
-                    static IntAlphabetSingleton alphabet;
-                    return alphabet;
-                }
-
-                IntAlphabetSingleton(IntAlphabetSingleton &) = delete;
-
-                IntAlphabetSingleton(IntAlphabetSingleton &&) = delete;
-
-                IntAlphabetSingleton &operator=(const IntAlphabetSingleton &) = delete;
-
-                IntAlphabetSingleton &operator=(IntAlphabetSingleton &&) = delete;
-
-                ~IntAlphabetSingleton() = default;
-
-            protected:
-                IntAlphabetSingleton() = default;
-            }; // class IntAlphabetSingleton.
-
-            IntAlphabetSingleton &alphabet_instance;
-        }; // class IntAlphabet.
-
-    /**
-     * Enumerated alphabet using a set of integers as symbols maintaining a set of specified symbols.
-     *
-     * @c EnumAlphabet is a version of direct (identity) alphabet (does not give names to symbols, their name is their
-     *  integer value directly). However, unlike @c IntAlphabet, @c EnumAlphabet maintains an ordered set of symbols in
-     *  the alphabet.
-     *
-     * Therefore, calling member functions @c get_complement() and @c get_alphabet_symbols() makes sense in the context
-     *  of @c EnumAlphabet and the functions give the expected results.
-     *
-     *  Example:
-     *  ```cpp
-     *  Alphabet alph{ EnumAlphabet{ 0, 4, 6, 8, 9 } };
-     *  CHECK(alph.translate_symb("6") == 6);
-     *  CHECK_THROWS(alph.translate_symb("5")); // Throws an exception about an unknown symbol.
-     *  CHECK(alph.get_complement({ Util::OrdVector<Symbol>{ 0, 6, 9 } }) == Util::OrdVector<Symbol>{ 4, 8 });
-     *  ```
+using Symbol = unsigned;
+using StringToSymbolMap = std::unordered_map<std::string, Symbol>;
+
+ /**
+  * The abstract interface for NFA alphabets.
+  */
+class Alphabet {
+public:
+    /// translates a string into a symbol
+    virtual Symbol translate_symb(const std::string &symb) = 0;
+
+    /**
+     * Translate sequence of symbol names to sequence of their respective values.
      */
-    class EnumAlphabet : public Alphabet {
-    public:
-        explicit EnumAlphabet() = default;
-        EnumAlphabet(const EnumAlphabet& rhs) = default;
-        EnumAlphabet(EnumAlphabet&& rhs) = default;
-
-        Util::OrdVector<Symbol> get_alphabet_symbols() const override { return m_symbols; }
-        Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const override {
-            return m_symbols.difference(symbols);
-        }
+    virtual std::vector<Symbol> translate_word(const std::vector<std::string>& word) const {
+        (void)word;
+        throw std::runtime_error("Unimplemented");
+    }
 
-        std::string reverse_translate_symbol(const Symbol symbol) const override {
-            if (m_symbols.find(symbol) == m_symbols.end()) {
-                throw std::runtime_error("Symbol '" + std::to_string(symbol) + "' is out of range of enumeration.");
-            }
-            return std::to_string(symbol);
-        }
+    /**
+     * @brief Translate internal @p symbol representation back to its original string name.
+     *
+     * Throws an exception when the @p symbol is missing in the alphabet.
+     * @param[in] symbol Symbol to translate.
+     * @return @p symbol original name.
+     */
+    virtual std::string reverse_translate_symbol(Symbol symbol) const = 0;
 
-    private:
-        EnumAlphabet& operator=(const EnumAlphabet& rhs);
+    /// also translates strings to symbols
+    Symbol operator[](const std::string &symb) { return this->translate_symb(symb); }
 
-    public:
-        /**
-         * @brief Expand alphabet by symbols from the passed @p symbols.
-         *
-         * Adding a symbol name which already exists will throw an exception.
-         * @param[in] symbols Vector of symbols to add.
-         */
-        void add_symbols_from(const Mata::Util::OrdVector<Symbol>& symbols) { m_symbols.insert(symbols); }
-
-        /**
-         * @brief Expand alphabet by symbols from the passed @p alphabet.
-         *
-         * @param[in] symbols_to_add Vector of symbols to add.
-         */
-        void add_symbols_from(const EnumAlphabet& alphabet) { m_symbols.insert(alphabet.get_alphabet_symbols()); }
-
-        EnumAlphabet(std::initializer_list<Symbol> symbols) : EnumAlphabet(symbols.begin(), symbols.end()) {}
-
-        template <class InputIt>
-        EnumAlphabet(InputIt first, InputIt last) : EnumAlphabet() {
-            for (; first != last; ++first) {
-                add_new_symbol(*first);
-            }
-        }
+    /**
+     * @brief Get a set of all symbols in the alphabet.
+     *
+     * The result does not have to equal the list of symbols in the automaton using this alphabet.
+     */
+    virtual Util::OrdVector<Symbol> get_alphabet_symbols() const { throw std::runtime_error("Unimplemented"); }
 
-        EnumAlphabet(std::initializer_list<std::string> l) : EnumAlphabet(l.begin(), l.end()) {}
+    /// complement of a set of symbols wrt the alphabet
+    virtual Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const { // {{{
+        (void) symbols;
+        throw std::runtime_error("Unimplemented");
+    } // }}}
 
-        Symbol translate_symb(const std::string& str) override {
-            Symbol symbol;
-            std::istringstream stream{ str };
-            stream >> symbol;
-            if (stream.fail() || !stream.eof()) {
-                throw std::runtime_error("Cannot translate string '" + str + "' to symbol.");
-            }
-            if (m_symbols.find(symbol) == m_symbols.end()) {
-                throw std::runtime_error("Unknown symbol'" + str + "' to be translated to Symbol.");
-            }
+    virtual ~Alphabet() = default;
 
-            return symbol;
-        }
+    /**
+     * @brief Check whether two alphabets are equal.
+     *
+     * In general, two alphabets are equal if and only if they are of the same class instance.
+     * @param other_alphabet The other alphabet to compare with for equality.
+     * @return True if equal, false otherwise.
+     */
+    virtual bool is_equal(const Alphabet &other_alphabet) const { return address() == other_alphabet.address(); }
 
-        std::vector<Symbol> translate_word(const std::vector<std::string>& word) const override {
-            const size_t word_size{ word.size() };
-            std::vector<Symbol> translated_symbols;
-            Symbol symbol;
-            std::stringstream stream;
-            translated_symbols.reserve(word_size);
-            for (const auto& str_symbol: word) {
-                stream << str_symbol;
-                stream >> symbol;
-                if (m_symbols.find(symbol) == m_symbols.end()) {
-                    throw std::runtime_error("Unknown symbol \'" + str_symbol + "\'");
-                }
-                translated_symbols.push_back(symbol);
-            }
-            return translated_symbols;
-        }
+    /**
+     * @brief Check whether two alphabets are equal.
+     *
+     * In general, two alphabets are equal if and only if they are of the same class instance.
+     * @param other_alphabet The other alphabet to compare with for equality.
+     * @return True if equal, false otherwise.
+     */
+    virtual bool is_equal(const Alphabet *const other_alphabet) const {
+        return address() == other_alphabet->address();
+    }
 
-        /**
-         * @brief Add new symbol to the alphabet with the value identical to its string representation.
-         *
-         * @param[in] symbol User-space representation of the symbol.
-         * @return Result of the insertion as @c InsertionResult.
-         */
-        void add_new_symbol(const std::string& symbol) {
-            std::istringstream str_stream{ symbol };
-            Symbol converted_symbol;
-            str_stream >> converted_symbol;
-            add_new_symbol(converted_symbol);
-        }
+    bool operator==(const Alphabet &) const = delete;
 
-        /**
-         * @brief Add new symbol to the alphabet.
-         *
-         * @param[in] key User-space representation of the symbol.
-         * @param[in] symbol Number of the symbol to be used on transitions.
-         * @return Result of the insertion as @c InsertionResult.
-         */
-        void add_new_symbol(Symbol symbol) {
-            m_symbols.insert(symbol);
-            update_next_symbol_value(symbol);
-        }
+protected:
+    virtual const void *address() const { return this; }
+}; // class Alphabet.
+
+/**
+* Direct alphabet (also identity alphabet or integer alphabet) using integers as symbols.
+*
+* This alphabet presumes that all integers are valid symbols.
+* Therefore, calling member functions get_complement() and get_alphabet_symbols() makes no sense in this context and the methods
+*  will throw exceptions warning about the inappropriate use of IntAlphabet. If one needs these functions, they should
+*  use OnTheFlyAlphabet instead of IntAlphabet.
+*/
+class IntAlphabet : public Alphabet {
+public:
+    IntAlphabet() : alphabet_instance(IntAlphabetSingleton::get()) {}
+
+    Symbol translate_symb(const std::string &symb) override;
+
+    std::string reverse_translate_symbol(Symbol symbol) const override { return std::to_string(symbol); }
+
+    Util::OrdVector<Symbol> get_alphabet_symbols() const override {
+        throw std::runtime_error("Nonsensical use of get_alphabet_symbols() on IntAlphabet.");
+    }
+
+    Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const override {
+        (void) symbols;
+        throw std::runtime_error("Nonsensical use of get_complement() on IntAlphabet.");
+    }
 
-        /**
-         * Get the next value for a potential new symbol.
-         * @return Next Symbol value.
-         */
-        Symbol get_next_value() const { return next_symbol_value; }
-
-        /**
-         * Get the number of existing symbols, epsilon symbols excluded.
-         * @return The number of symbols.
-         */
-        size_t get_number_of_symbols() const { return m_symbols.size(); }
-
-    private:
-        Mata::Util::OrdVector<Symbol> m_symbols{}; ///< Map of string transition symbols to symbol values.
-        Symbol next_symbol_value{ 0 }; ///< Next value to be used for a newly added symbol.
+    IntAlphabet(const IntAlphabet&) = default;
 
+    IntAlphabet& operator=(const IntAlphabet& int_alphabet) = delete;
+
+protected:
+    const void* address() const override { return &alphabet_instance; }
+
+private:
+    /**
+     * Singleton class implementing integer alphabet_instance for class IntAlphabet.
+     *
+     * Users have to use IntAlphabet instead which provides interface identical to other alphabets and can be used in
+     *  places where an instance of the abstract class Alphabet is required.
+     */
+    class IntAlphabetSingleton {
     public:
-        /**
-         * @brief Update next symbol value when appropriate.
-         *
-         * When the newly inserted value is larger or equal to the current next symbol value, update the next symbol
-         *  value to a value one larger than the new value.
-         * @param value The value of the newly added symbol.
-         */
-        void update_next_symbol_value(Symbol value) {
-            if (next_symbol_value <= value) {
-                next_symbol_value = value + 1;
-            }
+        static IntAlphabetSingleton& get() {
+            static IntAlphabetSingleton alphabet;
+            return alphabet;
         }
-    }; // class EnumAlphabet.
 
+        IntAlphabetSingleton(IntAlphabetSingleton&) = delete;
+        IntAlphabetSingleton(IntAlphabetSingleton&&) = delete;
+        IntAlphabetSingleton& operator=(const IntAlphabetSingleton&) = delete;
+        IntAlphabetSingleton& operator=(IntAlphabetSingleton&&) = delete;
+
+        ~IntAlphabetSingleton() = default;
+
+    protected:
+        IntAlphabetSingleton() = default;
+    }; // class IntAlphabetSingleton.
+
+    IntAlphabetSingleton& alphabet_instance;
+}; // class IntAlphabet.
+
+/**
+ * Enumerated alphabet using a set of integers as symbols maintaining a set of specified symbols.
+ *
+ * @c EnumAlphabet is a version of direct (identity) alphabet (does not give names to symbols, their name is their
+ *  integer value directly). However, unlike @c IntAlphabet, @c EnumAlphabet maintains an ordered set of symbols in
+ *  the alphabet.
+ *
+ * Therefore, calling member functions @c get_complement() and @c get_alphabet_symbols() makes sense in the context
+ *  of @c EnumAlphabet and the functions give the expected results.
+ *
+ *  Example:
+ *  ```cpp
+ *  Alphabet alph{ EnumAlphabet{ 0, 4, 6, 8, 9 } };
+ *  CHECK(alph.translate_symb("6") == 6);
+ *  CHECK_THROWS(alph.translate_symb("5")); // Throws an exception about an unknown symbol.
+ *  CHECK(alph.get_complement({ Util::OrdVector<Symbol>{ 0, 6, 9 } }) == Util::OrdVector<Symbol>{ 4, 8 });
+ *  ```
+ */
+class EnumAlphabet : public Alphabet {
+public:
+    explicit EnumAlphabet() = default;
+    EnumAlphabet(const EnumAlphabet& rhs) = default;
+    EnumAlphabet(EnumAlphabet&& rhs) = default;
+
+    Util::OrdVector<Symbol> get_alphabet_symbols() const override { return m_symbols; }
+    Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const override {
+        return m_symbols.difference(symbols);
+    }
+
+    std::string reverse_translate_symbol(const Symbol symbol) const override;
+
+private:
+    EnumAlphabet& operator=(const EnumAlphabet& rhs);
+
+public:
     /**
-     * An alphabet constructed 'on the fly'.
-     * Should be use anytime the automata have a specific names for the symbols.
+     * @brief Expand alphabet by symbols from the passed @p symbols.
+     *
+     * Adding a symbol name which already exists will throw an exception.
+     * @param[in] symbols Vector of symbols to add.
      */
-    class OnTheFlyAlphabet : public Alphabet {
-    public:
-        using InsertionResult = std::pair<StringToSymbolMap::const_iterator, bool>; ///< Result of the insertion of a new symbol.
+    void add_symbols_from(const Mata::Util::OrdVector<Symbol>& symbols) { m_symbols.insert(symbols); }
 
-        explicit OnTheFlyAlphabet(Symbol init_symbol = 0) : next_symbol_value(init_symbol) {};
-        OnTheFlyAlphabet(const OnTheFlyAlphabet& rhs) : symbol_map(rhs.symbol_map), next_symbol_value(rhs.next_symbol_value) {}
+    /**
+     * @brief Expand alphabet by symbols from the passed @p alphabet.
+     *
+     * @param[in] symbols_to_add Vector of symbols to add.
+     */
+    void add_symbols_from(const EnumAlphabet& alphabet) { m_symbols.insert(alphabet.get_alphabet_symbols()); }
 
-        explicit OnTheFlyAlphabet(const StringToSymbolMap& str_sym_map)
-                : symbol_map(str_sym_map) {}
+    EnumAlphabet(std::initializer_list<Symbol> symbols) : EnumAlphabet(symbols.begin(), symbols.end()) {}
+    template <class InputIt> EnumAlphabet(InputIt first, InputIt last) : EnumAlphabet() {
+        for (; first != last; ++first) { add_new_symbol(*first); }
+    }
+    EnumAlphabet(std::initializer_list<std::string> l) : EnumAlphabet(l.begin(), l.end()) {}
 
-        /**
-         * Create alphabet from a list of symbol names.
-         * @param symbol_names Names for symbols on transitions.
-         * @param init_symbol Start of a sequence of values to use for new symbols.
-         */
-        explicit OnTheFlyAlphabet(const std::vector<std::string>& symbol_names, Symbol init_symbol = 0)
-                : symbol_map(), next_symbol_value(init_symbol) { add_symbols_from(symbol_names); }
-
-        Util::OrdVector<Symbol> get_alphabet_symbols() const override;
-        Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const override;
-
-        std::string reverse_translate_symbol(const Symbol symbol) const override {
-            for (const auto& symbol_mapping: symbol_map) {
-                if (symbol_mapping.second == symbol) {
-                    return symbol_mapping.first;
-                }
-            }
-            throw std::runtime_error("symbol '" + std::to_string(symbol) + "' is out of range of enumeration");
-        }
+    Symbol translate_symb(const std::string& str) override;
+    std::vector<Symbol> translate_word(const std::vector<std::string>& word) const override;
 
-    private:
-        OnTheFlyAlphabet& operator=(const OnTheFlyAlphabet& rhs);
+    /**
+     * @brief Add new symbol to the alphabet with the value identical to its string representation.
+     *
+     * @param[in] symbol User-space representation of the symbol.
+     * @return Result of the insertion as @c InsertionResult.
+     */
+    void add_new_symbol(const std::string& symbol);
 
-    public:
-        /**
-         * @brief Expand alphabet by symbols from the passed @p symbol_names.
-         *
-         * Adding a symbol name which already exists will throw an exception.
-         * @param[in] symbol_names Vector of symbol names.
-         */
-        void add_symbols_from(const std::vector<std::string>& symbol_names) {
-            for (const std::string& symbol_name: symbol_names) {
-                add_new_symbol(symbol_name);
-            }
-        }
+    /**
+     * @brief Add new symbol to the alphabet.
+     *
+     * @param[in] key User-space representation of the symbol.
+     * @param[in] symbol Number of the symbol to be used on transitions.
+     * @return Result of the insertion as @c InsertionResult.
+     */
+    void add_new_symbol(Symbol symbol);
 
-        /**
-         * @brief Expand alphabet by symbols from the passed @p symbol_map.
-         *
-         * The value of the already existing symbols will NOT be overwritten.
-         * @param[in] new_symbol_map Map of strings to symbols.
-         */
-        void add_symbols_from(const StringToSymbolMap& new_symbol_map);
-
-        template <class InputIt>
-        OnTheFlyAlphabet(InputIt first, InputIt last) : OnTheFlyAlphabet() {
-            for (; first != last; ++first) {
-                add_new_symbol(*first, next_symbol_value);
-            }
-        }
+    /**
+     * Get the next value for a potential new symbol.
+     * @return Next Symbol value.
+     */
+    Symbol get_next_value() const { return next_symbol_value; }
 
-        OnTheFlyAlphabet(std::initializer_list<std::string> l) : OnTheFlyAlphabet(l.begin(), l.end()) {}
+    /**
+     * Get the number of existing symbols, epsilon symbols excluded.
+     * @return The number of symbols.
+     */
+    size_t get_number_of_symbols() const { return m_symbols.size(); }
 
-        Symbol translate_symb(const std::string& str) override
-        {
-            const auto it_insert_pair = symbol_map.insert({str, next_symbol_value});
-            if (it_insert_pair.second) {
-                return next_symbol_value++;
-            } else {
-                return it_insert_pair.first->second;
-            }
-
-            // TODO: How can the user specify to throw exceptions when we encounter an unknown symbol? How to specify that
-            //  the alphabet should have only the previously fixed symbols?
-            //auto it = symbol_map.find(str);
-            //if (symbol_map.end() == it)
-            //{
-            //    throw std::runtime_error("unknown symbol \'" + str + "\'");
-            //}
+private:
+    Mata::Util::OrdVector<Symbol> m_symbols{}; ///< Map of string transition symbols to symbol values.
+    Symbol next_symbol_value{ 0 }; ///< Next value to be used for a newly added symbol.
 
-            //return it->second;
-        }
+public:
+    /**
+     * @brief Update next symbol value when appropriate.
+     *
+     * When the newly inserted value is larger or equal to the current next symbol value, update the next symbol
+     *  value to a value one larger than the new value.
+     * @param value The value of the newly added symbol.
+     */
+    void update_next_symbol_value(Symbol value);
+}; // class EnumAlphabet.
 
-        virtual std::vector<Symbol> translate_word(const std::vector<std::string>& word) const {
-            const size_t word_size{ word.size() };
-            std::vector<Symbol> symbols;
-            symbols.reserve(word_size);
-            for (size_t i{ 0 }; i < word_size; ++i) {
-                const auto symbol_mapping_it = symbol_map.find(word[i]);
-                if (symbol_mapping_it == symbol_map.end()) {
-                    throw std::runtime_error("Unknown symbol \'" + word[i] + "\'");
-                }
-                symbols.push_back(symbol_mapping_it->second);
-            }
-            return symbols;
-        }
+/**
+ * An alphabet constructed 'on the fly'.
+ * Should be use anytime the automata have a specific names for the symbols.
+ */
+class OnTheFlyAlphabet : public Alphabet {
+public:
+    /// Result of the insertion of a new symbol.
+    using InsertionResult = std::pair<StringToSymbolMap::const_iterator, bool>;
+
+    explicit OnTheFlyAlphabet(Symbol init_symbol = 0) : next_symbol_value(init_symbol) {};
+    OnTheFlyAlphabet(const OnTheFlyAlphabet& rhs) : symbol_map(rhs.symbol_map), next_symbol_value(rhs.next_symbol_value) {}
+    explicit OnTheFlyAlphabet(StringToSymbolMap str_sym_map) : symbol_map(std::move(str_sym_map)) {}
+    /**
+     * Create alphabet from a list of symbol names.
+     * @param symbol_names Names for symbols on transitions.
+     * @param init_symbol Start of a sequence of values to use for new symbols.
+     */
+    explicit OnTheFlyAlphabet(const std::vector<std::string>& symbol_names, Symbol init_symbol = 0)
+            : symbol_map(), next_symbol_value(init_symbol) { add_symbols_from(symbol_names); }
 
-        /**
-         * @brief Add new symbol to the alphabet with the value of @c next_symbol_value.
-         *
-         * Throws an exception when the adding fails.
-         *
-         * @param[in] key User-space representation of the symbol.
-         * @return Result of the insertion as @c InsertionResult.
-         */
-        InsertionResult add_new_symbol(const std::string& key) {
-            InsertionResult insertion_result{ try_add_new_symbol(key, next_symbol_value) };
-            if (!insertion_result.second) { // If the insertion of key-value pair failed.
-                throw std::runtime_error("multiple occurrences of the same symbol");
-            }
-            ++next_symbol_value;
-            return insertion_result;
-        }
+    Util::OrdVector<Symbol> get_alphabet_symbols() const override;
+    Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const override;
 
-        /**
-         * @brief Add new symbol to the alphabet.
-         *
-         * Throws an exception when the adding fails.
-         *
-         * @param[in] key User-space representation of the symbol.
-         * @param[in] value Number of the symbol to be used on transitions.
-         * @return Result of the insertion as @c InsertionResult.
-         */
-        InsertionResult add_new_symbol(const std::string& key, Symbol value) {
-            InsertionResult insertion_result{ try_add_new_symbol(key, value) };
-            if (!insertion_result.second) { // If the insertion of key-value pair failed.
-                throw std::runtime_error("multiple occurrences of the same symbol");
-            }
-            update_next_symbol_value(value);
-            return insertion_result;
-        }
+    std::string reverse_translate_symbol(const Symbol symbol) const override;
 
-        /**
-         * @brief Try to add symbol to the alphabet map.
-         *
-         * Does not throw an exception when the adding fails.
-         *
-         * @param[in] key User-space representation of the symbol.
-         * @param[in] value Number of the symbol to be used on transitions.
-         * @return Result of the insertion as @c InsertionResult.
-         */
-        InsertionResult try_add_new_symbol(const std::string& key, Symbol value) {
-            return symbol_map.insert({ key, value});
-        }
+private:
+    OnTheFlyAlphabet& operator=(const OnTheFlyAlphabet& rhs);
 
-        /**
-         * Get the next value for a potential new symbol.
-         * @return Next Symbol value.
-         */
-        Symbol get_next_value() const { return next_symbol_value; }
-
-        /**
-         * Get the number of existing symbols, epsilon symbols excluded.
-         * @return The number of symbols.
-         */
-        size_t get_number_of_symbols() const { return next_symbol_value; }
-
-        /**
-         * Get the symbol map used in the alphabet.
-         * @return Map mapping strings to symbols used internally in Mata.
-         */
-        const StringToSymbolMap& get_symbol_map() const { return symbol_map; }
-
-    private:
-        StringToSymbolMap symbol_map{}; ///< Map of string transition symbols to symbol values.
-        Symbol next_symbol_value{}; ///< Next value to be used for a newly added symbol.
+public:
+    /**
+     * @brief Expand alphabet by symbols from the passed @p symbol_names.
+     *
+     * Adding a symbol name which already exists will throw an exception.
+     * @param[in] symbol_names Vector of symbol names.
+     */
+    void add_symbols_from(const std::vector<std::string>& symbol_names);
 
-    public:
-        /**
-         * @brief Update next symbol value when appropriate.
-         *
-         * When the newly inserted value is larger or equal to the current next symbol value, update the next symbol
-         *  value to a value one larger than the new value.
-         * @param value The value of the newly added symbol.
-         */
-        void update_next_symbol_value(Symbol value) {
-            if (next_symbol_value <= value) {
-                next_symbol_value = value + 1;
-            }
+    /**
+     * @brief Expand alphabet by symbols from the passed @p symbol_map.
+     *
+     * The value of the already existing symbols will NOT be overwritten.
+     * @param[in] new_symbol_map Map of strings to symbols.
+     */
+    void add_symbols_from(const StringToSymbolMap& new_symbol_map);
+
+    template <class InputIt> OnTheFlyAlphabet(InputIt first, InputIt last) {
+        for (; first != last; ++first) {
+            add_new_symbol(*first, next_symbol_value);
         }
-    }; // class OnTheFlyAlphabet.
+    }
+    OnTheFlyAlphabet(std::initializer_list<std::string> l) : OnTheFlyAlphabet(l.begin(), l.end()) {}
+
+    Symbol translate_symb(const std::string& str) override;
+
+    virtual std::vector<Symbol> translate_word(const std::vector<std::string>& word) const;
+
+    /**
+     * @brief Add new symbol to the alphabet with the value of @c next_symbol_value.
+     *
+     * Throws an exception when the adding fails.
+     *
+     * @param[in] key User-space representation of the symbol.
+     * @return Result of the insertion as @c InsertionResult.
+     */
+    InsertionResult add_new_symbol(const std::string& key);
+
+    /**
+     * @brief Add new symbol to the alphabet.
+     *
+     * Throws an exception when the adding fails.
+     *
+     * @param[in] key User-space representation of the symbol.
+     * @param[in] value Number of the symbol to be used on transitions.
+     * @return Result of the insertion as @c InsertionResult.
+     */
+    InsertionResult add_new_symbol(const std::string& key, Symbol value);
+
+    /**
+     * @brief Try to add symbol to the alphabet map.
+     *
+     * Does not throw an exception when the adding fails.
+     *
+     * @param[in] key User-space representation of the symbol.
+     * @param[in] value Number of the symbol to be used on transitions.
+     * @return Result of the insertion as @c InsertionResult.
+     */
+    InsertionResult try_add_new_symbol(const std::string& key, Symbol value) { return symbol_map.insert({ key, value}); }
+
+    /**
+     * Get the next value for a potential new symbol.
+     * @return Next Symbol value.
+     */
+    Symbol get_next_value() const { return next_symbol_value; }
+
+    /**
+     * Get the number of existing symbols, epsilon symbols excluded.
+     * @return The number of symbols.
+     */
+    size_t get_number_of_symbols() const { return next_symbol_value; }
+
+    /**
+     * Get the symbol map used in the alphabet.
+     * @return Map mapping strings to symbols used internally in Mata.
+     */
+    const StringToSymbolMap& get_symbol_map() const { return symbol_map; }
+
+private:
+    StringToSymbolMap symbol_map{}; ///< Map of string transition symbols to symbol values.
+    Symbol next_symbol_value{}; ///< Next value to be used for a newly added symbol.
+
+public:
+    /**
+     * @brief Update next symbol value when appropriate.
+     *
+     * When the newly inserted value is larger or equal to the current next symbol value, update the next symbol
+     *  value to a value one larger than the new value.
+     * @param value The value of the newly added symbol.
+     */
+    void update_next_symbol_value(Symbol value);
+}; // class OnTheFlyAlphabet.
 } // namespace Mata
 
 namespace std
 { // {{{
     std::ostream& operator<<(std::ostream& os, const Mata::Alphabet& alphabet);
 }
-#endif //_MATA_ALPHABET_HH
+#endif //MATA_ALPHABET_HH
```

### Comparing `libmata-0.66.0/mata/include/mata/closed-set.hh` & `libmata-0.67.0/mata/include/mata/closed-set.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-/* closed_set.hh --- downward and upward closed sets
- *
- * Copyright (c) TODO
+/* closed-set.hh --- Downward and upward closed sets.
  *
  * This file is a part of libmata.
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-/** @file closed_set.hh
- *  @brief Definition of a closed set
+/**
+ * @file closed_set.hh
+ * @brief Definition of a downward and upward closed set.
  *
- *  This file contains definition of a closed set and function which
+ * This file contains definition of a closed set and function which
  *  allow us to work with them (membership, inclusion, union, intersection)
  *
- *
  * Description:
  * In this context, an upward-closed set is a set of sets of elements of type T,
  * (set of nodes of type T, where a node is a set of elements of type T)
  * where the elements come from the discrete range <min_val; max_val>. If the upward
  * closed set contains a subset A of the range <min_val; max_val>, it also contains
  * all the supersets of A (in context of the discrete range <min_val; max_val>).
  * Thus, the upward closed set could be easily represented by its 1) type (upward closed),
@@ -45,478 +43,418 @@
  *
  * It is not possible to:
  *
  * -> choose a custom carrier which is not a discrete range <min_val; max_val>
  * -> <=- and >=-compare two closed sets of the different types (nonsense)
  * -> remove a node/more nodes from the closed set (nonsense)
  * -> perform an union over two closed sets of different types or different carriers (nonsense)
- * -> perform an intersection over two closed sets of different types or different carriers (nonsense) 
+ * -> perform an intersection over two closed sets of different types or different carriers (nonsense)
  *
  * Examples:
  *
- * Let us have the carrier {0, 1, 2, 3} and the upward-closed set with the antichain 
+ * Let us have the carrier {0, 1, 2, 3} and the upward-closed set with the antichain
  * {{0}, {1, 2}}. We can write↑{{0}, {1, 2}} = {{0}, {0, 1}, {0, 2}, {0, 3}, {0, 1, 2},
  * {0, 1, 3}, {0, 2, 3}, {1, 2}, {1, 2, 3}, {0, 1, 2, 3}}.
  *
- * Let us have the carrier {0, 1, 2, 3} and the downward-closed set with the antichain 
+ * Let us have the carrier {0, 1, 2, 3} and the downward-closed set with the antichain
  * {{0}, {1, 2}}. We can write ↓{{0}, {1, 2}} = {{0}, {1, 2}, {1}, {2}, {}}.
  *
  *  @author Tomáš Kocourek
  */
 
-#ifndef _MATA_CLOSED_SET_HH_
-#define _MATA_CLOSED_SET_HH_
+#ifndef MATA_CLOSED_SET_HH_
+#define MATA_CLOSED_SET_HH_
 
 #include <cassert>
 
-#include <mata/util.hh>
-#include <mata/ord-vector.hh>
+#include "mata/util.hh"
+#include "mata/ord-vector.hh"
 
-namespace Mata
-{
+namespace Mata {
 
-// Ordered vector
+// Ordered vector.
 template<typename T> using OrdVec = Mata::Util::OrdVector<T>;
 
-// A closed set could be upward-closed or downward-closed
+// A closed set could be upward-closed or downward-closed.
 enum ClosedSetType {upward_closed_set, downward_closed_set};
 
-// Closed set
-// contains discrete range borders, its type
-// and the corresponding antichain
-// It is neccessary to be able to evaluate relation operators
-// <, <=, >, >=, ==, != over instances of this datatype T
-template <typename T> 
-struct ClosedSet
-{
+/**
+ * @brief Closed set.
+ *
+ * Contains discrete range borders, its type and the corresponding anti-chain. It is necessary to be able to evaluate
+ *  relation operators <, <=, >, >=, ==, != over instances of this datatype T.
+ * @tparam T Datatype the closed set contains.
+ */
+template <typename T>
+struct ClosedSet {
     using Node = OrdVec<T>;
     using Nodes = OrdVec<Node>;
 
     private:
 
        ClosedSetType type_{upward_closed_set}; // upward_closed or downward_closed sets
        T min_val_;
        T max_val_;
-       Nodes antichain_{}; 
+       Nodes antichain_{};
 
     public:
-    
-       // constructors
-       /////////////////////////////////////////////
 
+       // constructors
        ClosedSet() : type_(), min_val_(), max_val_(), antichain_() { }
 
-       // inserting a single value of the datatype T           
-       ClosedSet(ClosedSetType type, T min_val, T max_val, T value) : 
-       type_(type), min_val_(min_val), max_val_(max_val), antichain_(Nodes(value)) 
-       { 
-            assert(min_val <= max_val); 
-            assert(min_val <= value && value <= max_val);
+       // inserting a single value of the datatype T
+       ClosedSet(ClosedSetType type, T min_val, T max_val, T value)
+           : type_(type), min_val_(min_val), max_val_(max_val), antichain_(Nodes(value)) {
+           assert(min_val <= max_val);
+           assert(min_val <= value && value <= max_val);
        }
 
        // inserting a single vector of the datatype T
-       ClosedSet(ClosedSetType type, T min_val, T max_val, Node node) : 
-       type_(type), min_val_(min_val), max_val_(max_val), antichain_(Node(node)) 
-       { 
-            assert(min_val <= max_val);
-            assert(in_interval(node));
+       ClosedSet(ClosedSetType type, T min_val, T max_val, Node node)
+           : type_(type), min_val_(min_val), max_val_(max_val), antichain_(Node(node)) {
+           assert(min_val <= max_val);
+           assert(in_interval(node));
        }
 
        // inserting a whole antichain
-       ClosedSet(ClosedSetType type, T min_val, T max_val, Nodes antichain = Nodes()) : 
-       type_(type), min_val_(min_val), max_val_(max_val)
-       { 
-            assert(min_val <= max_val);
-            insert(antichain);
+       ClosedSet(ClosedSetType type, T min_val, T max_val, Nodes antichain = Nodes())
+           : type_(type), min_val_(min_val), max_val_(max_val) {
+           assert(min_val <= max_val);
+           insert(antichain);
        }
 
-       /////////////////////////////////////////////
-
        // operators
-       /////////////////////////////////////////////
 
-       // Two closed sets are equivalent iff their type, borders 
-	   // and corresponding antichains are the same
+       // Two closed sets are equivalent iff their type, borders
+       // and corresponding antichains are the same
        bool operator==(ClosedSet<T> rhs) const
-	    { // {{{
-		    return type_ == rhs.type && min_val_ == rhs.min_val && 
-			max_val_ == rhs.max_val && antichain_ == rhs.antichain;
-	    } // operator== }}}
+        { // {{{
+            return type_ == rhs.type && min_val_ == rhs.min_val &&
+            max_val_ == rhs.max_val && antichain_ == rhs.antichain;
+        } // operator== }}}
 
-       // Two closed sets are not equivalent iff their type, 
-	   // borders or corresponding antichains differ
+       // Two closed sets are not equivalent iff their type,
+       // borders or corresponding antichains differ
        bool operator!=(ClosedSet<T> rhs) const
-	    { // {{{
-		    return type_ != rhs.type_ || min_val_ != rhs.min_val_ ||
-			max_val_ != rhs.max_val_ || antichain_ != rhs.antichain_;
-	    } // operator!= }}}
+        { // {{{
+            return type_ != rhs.type_ || min_val_ != rhs.min_val_ ||
+            max_val_ != rhs.max_val_ || antichain_ != rhs.antichain_;
+        } // operator!= }}}
 
         // A closed set is considered to be smaller than the other one iff
-		// it is a subset of the other one
-		// It is not possible to perform <=-comparisons accros upward- and downward-closed
-		// sets, each argument has to be upward- or downward-closed set
+        // it is a subset of the other one
+        // It is not possible to perform <=-comparisons accros upward- and downward-closed
+        // sets, each argument has to be upward- or downward-closed set
         bool operator<=(ClosedSet<T> rhs) const
-	    { // {{{
+        { // {{{
             assert(type_ == rhs.type_ && min_val_ == rhs.min_val_ && max_val_ == rhs.max_val_ &&
-			"Types and borders of given closed sets must be the same to perform their <=-comparison.");
+            "Types and borders of given closed sets must be the same to perform their <=-comparison.");
             return rhs.contains(antichain_);
-	    } // operator<= }}}
+        } // operator<= }}}
 
-        // A closed set is considered to be bigger than the other one iff 
-		// it is a superset of the other one
-        // It is not possible to perform <=-comparisons of accros upward- 
-		// and downward-closed sets, each argument
+        // A closed set is considered to be bigger than the other one iff
+        // it is a superset of the other one
+        // It is not possible to perform <=-comparisons of accros upward-
+        // and downward-closed sets, each argument
         // has to be upward- or downward-closed set
         bool operator>=(ClosedSet<T> rhs) const
-	    { // {{{
+        { // {{{
             assert(type_ == rhs.type_ && min_val_ == rhs.min_val_ && max_val_ == rhs.max_val_ &&
-			"Types and borders of given closed sets must be the same to perform their <=-comparison.");
+            "Types and borders of given closed sets must be the same to perform their <=-comparison.");
             return contains(rhs.antichain);
-	    } // operator<= }}}
+        } // operator<= }}}
 
         // Text representation of a closed set
-        friend std::ostream& operator<<(std::ostream& os, const ClosedSet<T> cs)
-        {
-            std::string strType = "TYPE: ";
-            strType += cs.type() == upward_closed_set ? "UPWARD CLOSED" : "DOWNWARD CLOSED";
-            strType += "\n";
-            std::string strInterval = "INTERVAL: " + std::to_string(cs.get_min()) + 
-			" - " + std::to_string(cs.get_max()) + "\n";
-            std::string strValues = "ANTICHAIN: {";
-            for(auto node : cs.antichain())
-            {
-                strValues += "{";
-                for(auto state : node)
-                {
-                    strValues += " " + std::to_string(state);
-                }
-                strValues += "}";
-            }
-            strValues += "}";
-            return os << strType + strInterval + strValues + "\n";
-        }
-
-       bool is_upward_closed(void) const {return type_ == upward_closed_set;};
-       bool is_downward_closed(void) const {return type_ == downward_closed_set;};
-
-       ClosedSetType type() {return type_;}
-       const ClosedSetType type() const {return type_;}
-
-       Nodes antichain() {return antichain_;}
-       const Nodes antichain() const {return antichain_;}
-
-       T get_min() {return min_val_;}
-       const T get_min() const {return min_val_;}
-
-       T get_max() {return max_val_;}
-       const T get_max() const {return max_val_;}
-
-       bool contains (Node node) const;
-       bool contains (Nodes nodes) const;
+        friend std::ostream& operator<<(std::ostream& os, const ClosedSet<T> cs);
 
-       bool in_interval (Node node) const;      
+        bool is_upward_closed() const {return type_ == upward_closed_set;};
+        bool is_downward_closed() const {return type_ == downward_closed_set;};
 
-       void insert(T el) {insert(Node(el));};
-       void insert(Node node);
-       void insert(Nodes nodes) {for(auto node : nodes) insert(node);};
+        ClosedSetType type() {return type_;}
+        const ClosedSetType type() const {return type_;}
 
-       ClosedSet Union (const ClosedSet rhs) const;
-       ClosedSet intersection (const ClosedSet rhs) const;
-       ClosedSet complement () const;
-
-       /////////////////////////////////////////////
-}; // ClosedSet }}}
+        Nodes antichain() {return antichain_;}
+        const Nodes antichain() const {return antichain_;}
+
+        T get_min() {return min_val_;}
+        const T get_min() const {return min_val_;}
+
+        T get_max() {return max_val_;}
+        const T get_max() const {return max_val_;}
+
+        bool contains (Node node) const;
+        bool contains (Nodes nodes) const;
+
+        bool in_interval (Node node) const;
+
+        void insert(T el) {insert(Node(el));};
+        void insert(Node node);
+        void insert(Nodes nodes) {for(auto node : nodes) insert(node);};
+
+        ClosedSet Union (const ClosedSet rhs) const;
+        ClosedSet intersection (const ClosedSet rhs) const;
+        ClosedSet complement () const;
+}; // class ClosedSet.
+
+template<typename T>
+std::ostream& operator<<(std::ostream& os, const ClosedSet<T> cs) {
+    std::string strType = "TYPE: ";
+    strType += cs.type() == upward_closed_set ? "UPWARD CLOSED" : "DOWNWARD CLOSED";
+    strType += "\n";
+    std::string strInterval = "INTERVAL: " + std::to_string(cs.get_min()) + " - " + std::to_string(cs.get_max()) + "\n";
+    std::string strValues = "ANTICHAIN: {";
+    for(auto node : cs.antichain()) {
+        strValues += "{";
+        for(auto state : node) {
+            strValues += " " + std::to_string(state);
+        }
+        strValues += "}";
+    }
+    strValues += "}";
+    return os << strType + strInterval + strValues + "\n";
+}
 
 /** This function decides whether a set of elements is part of the closed set
-* by subset-compraring the input with all elements of the antichain 
+* by subset-compraring the input with all elements of the antichain
 * @brief decides whether the closed set contains a given element
 * @param node a given ordered vector of elements of the type T
 * @return true iff the given ordered vector belongs to the current closed set
 */
 template <typename T>
-bool ClosedSet<T>::contains(Node node) const
-{
-    if(type_ == upward_closed_set)
-    {         
-        for(auto element : antichain_)
-        {
-            if(element.IsSubsetOf(node))
-            {
+bool ClosedSet<T>::contains(Node node) const {
+    if(type_ == upward_closed_set) {
+        for(auto element : antichain_) {
+            if(element.IsSubsetOf(node)) {
                 return true;
             }
         }
     }
-    else if(type_ == downward_closed_set)
-    {         
-        for(auto element : antichain_)
-        {
-            if(node.IsSubsetOf(element))
-            {
+    else if(type_ == downward_closed_set) {
+        for(auto element : antichain_) {
+            if(node.IsSubsetOf(element)) {
                 return true;
             }
         }
     }
     return false;
-} // contains }}}
+}
 
 /** This function decides whether a set of sets of elements is a part of the closed set
-* by subset-compraring the input with all elements of the antichain 
+* by subset-compraring the input with all elements of the antichain
 * @brief decides whether the closed set contains a given set of sets of elements
 * @param nodes a given ordered vector of ordered vectors of elements of the type T
 * @return true iff the given ordered vector of ordered vectors belongs to the current closed set
 */
 template <typename T>
-bool ClosedSet<T>::contains(Nodes nodes) const
-{
-    for(auto node : nodes)
-    {
-        if(!contains(node))
-        {
+bool ClosedSet<T>::contains(Nodes nodes) const {
+    for(auto node : nodes) {
+        if(!contains(node)) {
             return false;
         }
     }
     return true;
-} // contains }}}
+}
 
 /** This function decides whether a given ordered vector of elements of the datatype T
 * belongs to the discrete interval of the current closed set
 * @brief decides whether the given vector respects the borders
 * @param node a given ordered vector of elements of the type T which will be inspected
 * @return true iff the given ordered vector respects the borders
 */
 template <typename T>
-bool ClosedSet<T>::in_interval(Node node) const
-{
-    for(auto value : node)
-    {
-        if(value < min_val_ || value > max_val_)
-        {
+bool ClosedSet<T>::in_interval(Node node) const {
+    for(auto value : node) {
+        if(value < min_val_ || value > max_val_) {
             return false;
         }
     }
     return true;
-} // in_interval }}}
+}
 
 /** Adds a new element to the closed set. If the element is already contained in the closed
 * set, the closed set remains unchanged. Otherwise, the antichain will be recomputed.
 * @brief inserts a new element to the closed set
 * @param node a given node which will be added to the closed set
 */
 template <typename T>
-void ClosedSet<T>::insert(Node node)
-{
+void ClosedSet<T>::insert(Node node) {
     assert(in_interval(node) && "Each element of the given node has to respect " &&
-	"the carrier of the closed set.");
+    "the carrier of the closed set.");
     // If the closed set is empty, the antichain could be simply changed
-	// by adding the given node as the only node to the antichain
-    if(antichain_.empty())
-    {
+    // by adding the given node as the only node to the antichain
+    if(antichain_.empty()) {
         antichain_.insert(node);
         return;
     }
     // If the closed set already contains the given node, there is no
     // need to change the closed set
-    if(contains(node))
-    {
+    if(contains(node)) {
         return;
     }
     // We need to collect all the elements off the antichain which could be removed
     // as soon as the new element is added to keep the antichain <=-uncomparable
     OrdVec<OrdVec<T>> to_erase{};
 
     // If the closed set is upward-closed, we have to erase all the elements of
     // the antichain which are supersets of the inserted node
-    // Example: Let us have an upward-closed set ↑{{0, 1}, {2}} with a corresponding 
+    // Example: Let us have an upward-closed set ↑{{0, 1}, {2}} with a corresponding
     // antichain {{0, 1}, {2}}. If we add {0} to the closed set, the element {0, 1}
     // needs to be erased from the antichain since the set {{0}, {0, 1}, {2}} contains
     // <=-comparable elements and the result should be upward-closed.
-    if(type_ == upward_closed_set)
-    {
-        for(auto element : antichain_)
-        {
-            if(node.IsSubsetOf(element))
-            {
+    if(type_ == upward_closed_set) {
+        for(auto element : antichain_) {
+            if(node.IsSubsetOf(element)) {
                 to_erase.insert(element);
             }
         }
     }
 
     // If the closed set is downward-closed, we have to erase all the elements of
     // the antichain which are subsets of the inserted node
-    // Example: Let us have an upward-closed set ↓{{0, 1}, {2}} with a corresponding 
+    // Example: Let us have an upward-closed set ↓{{0, 1}, {2}} with a corresponding
     // antichain {{0, 1}, {2}}. If we add {1, 2} to the closed set, the element {2}
     // needs to be erased from the antichain since the set {{0}, {1, 2}, {2}} contains
     // <=-comparable elements and the result should be downward-closed.
-    else if(type_ == downward_closed_set)
-    {
-        for(auto element : antichain_)
-        {
-            if(element.IsSubsetOf(node))
-            {
+    else if(type_ == downward_closed_set) {
+        for(auto element : antichain_) {
+            if(element.IsSubsetOf(node)) {
                 to_erase.insert(element);
             }
         }
     }
 
-    for(auto element : to_erase)
-    {
+    for(auto element : to_erase) {
         antichain_.remove(element);
     }
     antichain_.insert(node);
 } // insert }}}
 
-/** Performs an union over two closed sets with the same type and carrier. 
+/** Performs an union over two closed sets with the same type and carrier.
 * This function simply adds all the
 * elements of the antichain of the first closed set to the second closed set
 * @brief performs an union over closed sets
 * @param rhs a given closed set which will be unioned with the current one
 * @return an union of the given closed sets
 */
 template <typename T>
-ClosedSet<T> ClosedSet<T>::Union(const ClosedSet<T> rhs) const
-{
+ClosedSet<T> ClosedSet<T>::Union(const ClosedSet<T> rhs) const {
     assert(type_ == rhs.type_ && min_val_ == rhs.min_val_ && max_val_ == rhs.max_val_ &&
-	"Types and borders of given closed sets must be the same to compute their union.");
+    "Types and borders of given closed sets must be the same to compute their union.");
     ClosedSet<T> result(type_, min_val_, max_val_, antichain_);
     result.insert(rhs.antichain());
     return result;
-} // Union }}}
+}
 
 /** Performs an intersection over two closed sets with the same type and carrier.
 * @brief performs an intersection over closed sets
 * @param rhs a given closed set which will be intersectioned with the current one
 * @return an intersection of the given closed sets
 */
 template <typename T>
-ClosedSet<T> ClosedSet<T>::intersection(const ClosedSet<T> rhs) const
-{
+ClosedSet<T> ClosedSet<T>::intersection(const ClosedSet<T> rhs) const {
     assert(type_ == rhs.type_ && min_val_ == rhs.min_val_ && max_val_ == rhs.max_val_ &&
-	"Types and borders of given closed sets must be the same to compute their union.");
+    "Types and borders of given closed sets must be the same to compute their union.");
     ClosedSet<T> result(type_, min_val_, max_val_);
 
-    // Iterates through all the tuples from Antichan1 X Antichan2 
-	// and creates an union of them
-    if(type_ == upward_closed_set)
-    {
-        for(auto element1 : antichain_)
-        {
-            for(auto element2 : rhs.antichain())
-            {
-               result.insert(element1.Union(element2));    
+    // Iterates through all the tuples from Antichan1 X Antichan2
+    // and creates an union of them
+    if(type_ == upward_closed_set) {
+        for(auto element1 : antichain_) {
+            for(auto element2 : rhs.antichain()) {
+               result.insert(element1.Union(element2));
             }
         }
     }
 
-    // Iterates through all the tuples from Antichan1 X Antichan2 
-	// and creates an intersection of them
-    if(type_ == downward_closed_set)
-    {
-        for(auto element1 : antichain_)
-        {
-            for(auto element2 : rhs.antichain())
-            {
-               result.insert(element1.intersection(element2));    
+    // Iterates through all the tuples from Antichan1 X Antichan2
+    // and creates an intersection of them
+    if(type_ == downward_closed_set) {
+        for(auto element1 : antichain_) {
+            for(auto element2 : rhs.antichain()) {
+               result.insert(element1.intersection(element2));
             }
         }
-    }    
+    }
     return result;
 } // intersection }}}
 
 /** Performs a complementation over a closed set. The result will
 * contain nodes which are not elements of the former closed set.
 * The complement of an upward-closed set is always downward-closed and vice versa.
 * @brief performs a complementation over a closed set
 * @return a complement of a closed set
 */
 template <typename T>
-ClosedSet<T> ClosedSet<T>::complement() const
-{
-	// The complement of an upward-closed set is
-	// always downward-closed and vice versa.
-	ClosedSetType new_type = upward_closed_set;
-	if(type_ == upward_closed_set)
-	{
-		new_type = downward_closed_set;
-	}
-	ClosedSet<T> result = ClosedSet(new_type, get_min(), get_max(), antichain());
-	
-	if(type_ == upward_closed_set)
-	{
-		// Initially, a complement contains all possible elements
-		// which will be then (possibly) removed.
-		Node initialValues{};
-		for(long unsigned i = 0; i <= max_val_; ++i)
-		{
-			initialValues.insert(i);
-		}
-		result.insert(initialValues);       
-		
-		// For each element of the closed set {xa, xb, xc, ...}, we
-		// create a set of all sets Xa, Xb, Xc,... such that Xn contains
-		// all elements of the carrier except of xn
-		// For example, for a node {0, 2, 3} (the maximal element is 4),
-		// we create a set {{1, 2, 3, 4}, {0, 1, 3, 4}, {0, 1, 2, 4}}.
-		// This set corresponds to an antichain of a new downward-closed set.
-		// The result will be an intersection of all downward-closed sets
-		// created using this procedure.
-		for(const auto& element : antichain())
-		{
-			ClosedSet preparingAntichain(downward_closed_set, get_min(), get_max());
-			for(int i = 0; i <= max_val_; ++i)
-			{
-				if(!element.count(i))
-				{
-					continue;
-				}		
-	            Node candidates{};
-	            for(int j = 0; j <= max_val_; ++j)
-	            {
-	                if(i!=j)
-	                {
-	                    candidates.insert(j);
-	                }
-	            }
-	            preparingAntichain.insert(candidates);
-			}
-			result = result.intersection(preparingAntichain);
-	    }
-    }
-
-    else if(type_ == downward_closed_set)
-    {
-		// Initially, a complement contains all possible elements
-		// which will be then (possibly) removed.
-		result.insert(Node());   
-
-		// For each element of the closed set {xa, xb, xc, ...}, we
-		// create a set of all sets Xa, Xb, Xc,... such that Xn contains
-		// only xn. For example, for a node {0, 2, 3}, we create a set 
-		// {{0}, {2}, {3}}.
-		// This set corresponds to an antichain of a new upward-closed set.
-		// The result will be an intersection of all upward-closed sets
-		// created using this procedure. 
-        for(Node element : antichain())
-        {
+ClosedSet<T> ClosedSet<T>::complement() const {
+    // The complement of an upward-closed set is
+    // always downward-closed and vice versa.
+    ClosedSetType new_type = upward_closed_set;
+    if(type_ == upward_closed_set) {
+        new_type = downward_closed_set;
+    }
+    ClosedSet<T> result = ClosedSet(new_type, get_min(), get_max(), antichain());
+
+    if(type_ == upward_closed_set) {
+        // Initially, a complement contains all possible elements
+        // which will be then (possibly) removed.
+        Node initialValues{};
+        for(long unsigned i = 0; i <= max_val_; ++i) {
+            initialValues.insert(i);
+        }
+        result.insert(initialValues);
+
+        // For each element of the closed set {xa, xb, xc, ...}, we
+        // create a set of all sets Xa, Xb, Xc,... such that Xn contains
+        // all elements of the carrier except of xn
+        // For example, for a node {0, 2, 3} (the maximal element is 4),
+        // we create a set {{1, 2, 3, 4}, {0, 1, 3, 4}, {0, 1, 2, 4}}.
+        // This set corresponds to an antichain of a new downward-closed set.
+        // The result will be an intersection of all downward-closed sets
+        // created using this procedure.
+        for(const auto& element : antichain()) {
+            ClosedSet preparingAntichain(downward_closed_set, get_min(), get_max());
+            for(int i = 0; i <= max_val_; ++i) {
+                if(!element.count(i)) {
+                    continue;
+                }
+                Node candidates{};
+                for(int j = 0; j <= max_val_; ++j) {
+                    if(i!=j) {
+                        candidates.insert(j);
+                    }
+                }
+                preparingAntichain.insert(candidates);
+            }
+            result = result.intersection(preparingAntichain);
+        }
+    }
+
+    else if(type_ == downward_closed_set) {
+        // Initially, a complement contains all possible elements
+        // which will be then (possibly) removed.
+        result.insert(Node());
+
+        // For each element of the closed set {xa, xb, xc, ...}, we
+        // create a set of all sets Xa, Xb, Xc,... such that Xn contains
+        // only xn. For example, for a node {0, 2, 3}, we create a set
+        // {{0}, {2}, {3}}.
+        // This set corresponds to an antichain of a new upward-closed set.
+        // The result will be an intersection of all upward-closed sets
+        // created using this procedure.
+        for(Node element : antichain()) {
             ClosedSet preparingAntichain(upward_closed_set, min_val_, max_val_);
-            for(T i = min_val_; i <= max_val_; ++i)
-            {
+            for(T i = min_val_; i <= max_val_; ++i) {
                 Node candidates{i};
-                if(!element.count(i))
-                {
+                if(!element.count(i)) {
                     preparingAntichain.insert({i});
                 }
             }
-                result = result.intersection(preparingAntichain);   
+            result = result.intersection(preparingAntichain);
         }
     }
 
     return result;
-
-///////////////////////////////////////////////////////////////
-
 } // complement }}}
 
+} // namespace Mata.
 
-} // std }}}
-
-
-#endif /* _MATA_CLOSED_SET_HH_ */
+#endif /* MATA_CLOSED_SET_HH_ */
```

### Comparing `libmata-0.66.0/mata/include/mata/inter-aut.hh` & `libmata-0.67.0/mata/include/mata/inter-aut.hh`

 * *Files 7% similar despite different names*

```diff
@@ -14,65 +14,62 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-
-#ifndef _MATA_INTER_AUT_HH
-#define _MATA_INTER_AUT_HH
+#ifndef MATA_INTER_AUT_HH
+#define MATA_INTER_AUT_HH
 
 #include <unordered_map>
 #include <unordered_set>
-
-#include <mata/parser.hh>
-
 #include <string>
+#include <utility>
 #include <vector>
 
-namespace Mata
-{
+#include "mata/parser.hh"
+
+namespace Mata {
 
 /**
  * A node of graph representing transition formula. A node could be operator (!,&,|) or operand (symbol, state, node).
  * Each node has a name (in case of marking naming, an initial character defining type of node is removed and stored in
  * name), raw (name including potential type marker), and information about its type.
  */
-struct FormulaNode
-{
+struct FormulaNode {
 public:
-    enum OperandType {
+    enum class OperandType {
         SYMBOL,
         STATE,
         NODE,
         NOT_OPERAND
     };
 
-    enum OperatorType {
+    enum class OperatorType {
         NEG,
         AND,
         OR,
         NOT_OPERATOR
     };
 
-    enum Type {
+    enum class Type {
         OPERAND,
         OPERATOR,
         LEFT_PARENTHESIS,
         RIGHT_PARENTHESIS,
         UNKNOWN
     };
 
     /// Define whether a node is operand or operator
     Type type;
     /// Raw name of node as it was specified in input text, i.e., including type marker.
     std::string raw;
     /// Parsed name, i.e., a potential type marker (first character) is removed.
-    std::string name; // parsed name. When type marking is used, markers are removed.
+    std::string name; // Parsed name. When type marking is used, markers are removed.
     /// if a node is operator, it defines which one
     OperatorType operator_type;
     /// if a node is operand, it defines which one
     OperandType operand_type;
 
     bool is_operand() const { return type == Type::OPERAND; }
 
@@ -82,112 +79,107 @@
 
     bool is_leftpar() const { return type == Type::LEFT_PARENTHESIS; }
 
     bool is_state() const { return operand_type == OperandType::STATE; }
 
     bool is_symbol() const { return operand_type == OperandType::SYMBOL; }
 
-    bool is_and() const { return type == OPERATOR && operator_type == AND; }
+    bool is_and() const { return type == Type::OPERATOR && operator_type == OperatorType::AND; }
 
-    bool is_neg() const { return type == OPERATOR && operator_type == NEG; }
+    bool is_neg() const { return type == Type::OPERATOR && operator_type == OperatorType::NEG; }
 
     // TODO: should constant be its own operand type?
-    bool is_constant() const { return type == OPERAND && (name == "true" || name == "false"); }
-    bool is_true() const { return type == OPERAND && name == "true"; }
-    bool is_false() const { return type == OPERAND && name == "false"; }
+    bool is_constant() const { return type == Type::OPERAND && (name == "true" || name == "false"); }
+    bool is_true() const { return type == Type::OPERAND && name == "true"; }
+    bool is_false() const { return type == Type::OPERAND && name == "false"; }
 
-    FormulaNode() : type(UNKNOWN), raw(""), name(""), operator_type(NOT_OPERATOR), operand_type(NOT_OPERAND) {}
+    FormulaNode()
+        : type(Type::UNKNOWN), raw(), name(), operator_type(OperatorType::NOT_OPERATOR),
+          operand_type(OperandType::NOT_OPERAND) {}
 
-    FormulaNode(Type t, std::string raw, std::string name,
-                OperatorType operator_t) : type(t), raw(raw), name(name), operator_type(operator_t),
-                                           operand_type(NOT_OPERAND) {}
+    FormulaNode(Type t, std::string raw, std::string name, OperatorType operator_t)
+        : type(t), raw(std::move(raw)), name(std::move(name)), operator_type(operator_t), operand_type(OperandType::NOT_OPERAND) {}
 
-    FormulaNode(Type t, std::string raw, std::string name,
-                OperandType operand) : type(t), raw(raw), name(name), operator_type(NOT_OPERATOR),
-                                       operand_type(operand) {}
+    FormulaNode(Type t, std::string raw, std::string name, OperandType operand)
+        : type(t), raw(std::move(raw)), name(std::move(name)), operator_type(OperatorType::NOT_OPERATOR), operand_type(operand) {}
 
-    FormulaNode(Type t, std::string raw) : type(t), raw(raw), name(raw), operator_type(NOT_OPERATOR),
-                                        operand_type(NOT_OPERAND) {}
+    FormulaNode(Type t, const std::string& raw)
+        : type(t), raw(raw), name(raw), operator_type(OperatorType::NOT_OPERATOR), operand_type(OperandType::NOT_OPERAND) {}
 
-    FormulaNode(const FormulaNode& n) : type(n.type), raw(n.raw), name(n.name), operator_type(n.operator_type),
-                                        operand_type(n.operand_type) {}
+    FormulaNode(const FormulaNode& n)
+        : type(n.type), raw(n.raw), name(n.name), operator_type(n.operator_type), operand_type(n.operand_type) {}
 };
 
 /**
  * Structure representing a transition formula using a graph.
  * A node of graph consists of node itself and set of children nodes.
  * Nodes are operators and operands of the formula.
  * E.g., a formula q1 & s1 will be transformed to a tree with & as a root node
  * and q1 and s2 being children nodes of the root.
  */
-struct FormulaGraph
-{
+struct FormulaGraph {
     FormulaNode node;
     std::vector<FormulaGraph> children;
 
     FormulaGraph() : node(), children() {}
-    FormulaGraph(FormulaNode n) : node(n), children() {}
+    FormulaGraph(const FormulaNode& n) : node(n), children() {}
     FormulaGraph(const FormulaGraph& g) : node(g.node), children(g.children) {}
 
     std::unordered_set<std::string> collect_node_names() const;
     void print_tree(std::ostream& os) const;
 };
 
 /**
  * Structure for a general intermediate representation of parsed automaton.
  * It contains information about type of automata, type of naming of nodes, symbols and states
  * and type of alphabet. It contains also the transitions formula and formula for initial and final
  * states. The formulas are represented as tree where nodes are either operands or operators.
  */
-struct IntermediateAut
-{
+struct IntermediateAut {
     /**
      * Type of automaton. So far we support nondeterministic finite automata (NFA) and
      * alternating finite automata (AFA)
      */
-    enum AutomatonType
-    {
+    enum class AutomatonType {
         NFA,
         AFA
     };
 
     /**
      * The possible kinds of naming of items in sets of states, nodes, or symbols.
      * It implies how the given set is defined.
      * Naming could be automatic (all things in formula not belonging to other sets will be assigned to a
      * set with automatic naming), marker based (everything beginning with `q` is a state, with `s` is a symbol,
      * with `n` is a node), or enumerated (the given set is defined by enumeration).
      * There are two special cases used for alphabet - symbols could be any character (CHARS) or anything from utf (UTF).
      */
-    enum Naming
-    {
+     enum class Naming {
         AUTO,
         MARKED,
         ENUM,
         CHARS,
         UTF
     };
 
     /**
      * Type of alphabet. We can have explicit alphabet (containing explicit symbols), or bitvector, or class of symbols
      * (e.g., alphabet is everything in utf), or intervals.
      * So far, only explicit representation is supported.
      */
-    enum AlphabetType
-    {
+    enum class AlphabetType {
         EXPLICIT,
         BITVECTOR,
         CLASS,
         INTERVALS
     };
 
 public:
-    Naming state_naming = MARKED;
-    Naming symbol_naming = MARKED;
-    Naming node_naming = MARKED;
+    Naming state_naming = Naming::MARKED;
+    Naming symbol_naming = Naming::MARKED;
+    Naming node_naming = Naming::MARKED;
     AlphabetType alphabet_type;
     AutomatonType automaton_type;
 
     // The vectors represent the given sets when enumeration is used.
     std::vector<std::string> states_names;
     std::vector<std::string> symbols_names;
     std::vector<std::string> nodes_names;
@@ -232,16 +224,15 @@
 
     bool is_nfa() const {return automaton_type == AutomatonType::NFA;}
     bool is_afa() const {return automaton_type == AutomatonType::AFA;}
 
     std::unordered_set<std::string> get_enumerated_initials() const {return initial_formula.collect_node_names();}
     std::unordered_set<std::string> get_enumerated_finals() const {return final_formula.collect_node_names();}
 
-    bool are_final_states_conjunction_of_negation() const
-    {
+    bool are_final_states_conjunction_of_negation() const {
         return is_graph_conjunction_of_negations(final_formula);
     }
 
     static bool is_graph_conjunction_of_negations(const FormulaGraph& graph);
 
     /**
      * Method returns a set of final states in the case that they were entered as a conjunction
@@ -251,17 +242,16 @@
 
     size_t get_number_of_disjuncts() const;
 
     static void parse_transition(Mata::IntermediateAut &aut, const std::vector<std::string> &tokens);
     void add_transition(const FormulaNode& lhs, const FormulaNode& symbol, const FormulaGraph& rhs);
     void add_transition(const FormulaNode& lhs, const FormulaNode& rhs);
     void print_transitions_trees(std::ostream&) const;
-};
+}; // class IntermediateAut.
 
-} /* Mata */
+} // namespace Mata.
 
-namespace std
-{
+namespace std {
     std::ostream& operator<<(std::ostream& os, const Mata::IntermediateAut& inter_aut);
 }
 
-#endif //_MATA_INTER_AUT_HH
+#endif //MATA_INTER_AUT_HH
```

### Comparing `libmata-0.66.0/mata/include/mata/mintermization.hh` & `libmata-0.67.0/mata/include/mata/mintermization.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,47 @@
-/*
- * mintermization.hh -- Mintermization of automaton
+/* mintermization.hh -- Mintermization of automaton.
  * It transforms an automaton with a bitvector formula used as a symbol to minterminized version of the automaton.
  *
- * Copyright (c) 2022 Martin Hruska <hruskamartin25@gmail.com>
- *
  * This file is a part of libmata.
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#ifndef _MATA_MINTERM_HH
-#define _MATA_MINTERM_HH
+#ifndef MATA_MINTERM_HH
+#define MATA_MINTERM_HH
 
 #include <mata/cudd/cuddObj.hh>
 
-#include <mata/inter-aut.hh>
+#include "mata/inter-aut.hh"
 
-namespace Mata
-{
+namespace Mata {
 
-class Mintermization
-{
+class Mintermization {
 private: // data types
-    struct OptionalBdd
-    {
-        enum TYPE {NOTHING_E, BDD_E};
+    struct OptionalBdd {
+        enum class TYPE {NOTHING_E, BDD_E};
 
         TYPE type;
         BDD val;
 
         explicit OptionalBdd(TYPE t) : type(t) {}
-        explicit OptionalBdd(const BDD& bdd) : type(BDD_E), val(bdd) {}
+        explicit OptionalBdd(const BDD& bdd) : type(TYPE::BDD_E), val(bdd) {}
         OptionalBdd(TYPE t, const BDD& bdd) : type(t), val(bdd) {}
 
-        OptionalBdd operator*(const OptionalBdd& b) const
-        {
-            if (this->type == NOTHING_E)
-                return b;
-            else if (b.type == NOTHING_E)
-                return *this;
-            else
-                return OptionalBdd{BDD_E, this->val * b.val};
-        }
-
-        OptionalBdd operator+(const OptionalBdd& b) const
-        {
-            if (this->type == NOTHING_E)
-                return b;
-            else if (b.type == NOTHING_E)
-                return *this;
-            else
-                return OptionalBdd{BDD_E, this->val + b.val};
-        }
-
-        OptionalBdd operator!() const
-        {
-            if (this->type == NOTHING_E)
-                return OptionalBdd(NOTHING_E);
-            else
-                return OptionalBdd{BDD_E, !this->val};
-        }
+        OptionalBdd operator*(const OptionalBdd& b) const;
+        OptionalBdd operator+(const OptionalBdd& b) const;
+        OptionalBdd operator!() const;
     };
 
     using DisjunctStatesPair = std::pair<const FormulaGraph *, const FormulaGraph *>;
 
 private: // private data members
     Cudd bdd_mng; // Manager of BDDs from lib cubdd, it allocates and manages BDDs.
     std::unordered_map<std::string, BDD> symbol_to_bddvar;
@@ -130,25 +100,25 @@
     /**
      * The method performs the mintermization over @aut with given @minterms.
      * It is method specialized for NFA.
      * @param res The resulting mintermized automaton
      * @param aut Automaton to be mintermized
      * @param minterms Set of minterms for mintermization
      */
-    void minterms_to_aut_nfa(Mata::IntermediateAut& res, const Mata::IntermediateAut& aut, const std::unordered_set<BDD>& minterms);
+    void minterms_to_aut_nfa(Mata::IntermediateAut& res, const Mata::IntermediateAut& aut,
+                             const std::unordered_set<BDD>& minterms);
 
     /**
      * The method for mintermization of alternating finite automaton using
      * a given set of minterms
      * @param res The resulting mintermized automaton
      * @param aut Automaton to be mintermized
      * @param minterms Set of minterms for mintermization
      */
-    void minterms_to_aut_afa(Mata::IntermediateAut& res,
-                             const Mata::IntermediateAut& aut, const std::unordered_set<BDD>& minterms);
+    void minterms_to_aut_afa(Mata::IntermediateAut& res, const Mata::IntermediateAut& aut,
+                             const std::unordered_set<BDD>& minterms);
 
-    Mintermization() : bdd_mng(0), symbol_to_bddvar{}, trans_to_bddvar()
-    {}
-};
+    Mintermization() : bdd_mng(0), symbol_to_bddvar{}, trans_to_bddvar() {}
+}; // class Mintermization.
 
-}  // namespace Mata
-#endif //_MATA_MINTERM_HH
+} // namespace Mata
+#endif //MATA_MINTERM_HH
```

### Comparing `libmata-0.66.0/mata/include/mata/nfa-algorithms.hh` & `libmata-0.67.0/mata/include/mata/nfa-algorithms.hh`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-/* nfa-internals.hh -- Wrapping up algorithms for Nfa manipulation which would be otherwise in anonymous namespaces
- *
- * Copyright (c) 2022
+/* nfa-internals.hh -- Wrapping up algorithms for Nfa manipulation which would be otherwise in anonymous namespaces.
  *
  * This file is a part of libmata.
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 3 of the License, or
  * (at your option) any later version.
@@ -34,106 +32,104 @@
  *   1. Complementation,
  *   2. Inclusion,
  *   3. Universality checking,
  *   4. Intersection/concatenation with epsilon transitions, or,
  *   5. Computing relation.
  */
 namespace Mata::Nfa::Algorithms {
-    /**
-     * Brzozowski minimization of automata (revert -> determinize -> revert -> determinize).
-     * @param[in] aut Automaton to be minimized.
-     * @return Minimized automaton.
-     */
-    Nfa minimize_brzozowski(const Nfa& aut);
-
-    /**
-     * Complement implemented by determization, adding sink state and making automaton complete. Then it adds
-     * final states which were non final in the original automaton.
-     * @param[in] aut Automaton to be complemented.
-     * @param[in] symbols Symbols needed to make the automaton complete.
-     * @param[in] minimize_during_determinization Whether the determinized automaton is computed by (brzozowski) minimization
-     * @return Complemented automaton.
-     */
-    Nfa complement_classical(const Nfa& aut, const Mata::Util::OrdVector<Symbol>& symbols,
-                             bool minimize_during_determinization = false);
-
-    /**
-     * Inclusion implemented by complementation of bigger automaton, intersecting it with smaller and then
-     * it checks emptiness of intersection
-     * @param[in] smaller Automaton which language should be included in the bigger one
-     * @param[in] bigger Automaton which language should include the smaller one
-     * @param[in] alphabet Alphabet of both automata (it is computed automatically, but it is more efficient to set it if you have it)
-     * @param[out] cex A potential counterexample word which breaks inclusion
-     * @return True if smaller language is included,
-     * i.e., if the final intersection of smaller complement of bigger is empty.
-     */
-    bool is_included_naive(const Nfa& smaller, const Nfa& bigger, const Alphabet* alphabet = nullptr, Run* cex = nullptr);
-
-    /**
-     * Inclusion implemented by antichain algorithms.
-     * @param[in] smaller Automaton which language should be included in the bigger one
-     * @param[in] bigger Automaton which language should include the smaller one
-     * @param[in] alphabet Alphabet of both automata (not needed for antichain algorithm)
-     * @param[out] cex A potential counterexample word which breaks inclusion
-     * @return True if smaller language is included,
-     * i.e., if the final intersection of smaller complement of bigger is empty.
-     */
-    bool is_included_antichains(const Nfa& smaller, const Nfa& bigger, const Alphabet*  alphabet = nullptr, Run* cex = nullptr);
-
-    /**
-     * Universality check implemented by checking emptiness of complemented automaton
-     * @param[in] aut Automaton which universality is checked
-     * @param[in] alphabet Alphabet of the automaton
-     * @param[out] cex Counterexample word which eventually breaks the universality
-     * @return True if the complemented automaton has non empty language, i.e., the original one is not universal
-     */
-    bool is_universal_naive(
-            const Nfa&         aut,
-            const Alphabet&    alphabet,
-            Run*               cex);
-
-    /**
-     * Universality checking based on subset construction with antichain.
-     * @param[in] aut Automaton which universality is checked
-     * @param[in] alphabet Alphabet of the automaton
-     * @param[out] cex Counterexample word which eventually breaks the universality
-     * @return True if the automaton is universal, otherwise false.
-     */
-    bool is_universal_antichains(
-            const Nfa&         aut,
-            const Alphabet&    alphabet,
-            Run*              cex);
-
-    Simlib::Util::BinaryRelation compute_relation(
-            const Nfa& aut,
-            const StringMap&  params = {{"relation", "simulation"}, {"direction", "forward"}});
-
-        /**
-         * @brief Compute intersection of two NFAs with a possibility of using multiple epsilons.
-         *
-         * @param[in] lhs First NFA to compute intersection for.
-         * @param[in] rhs Second NFA to compute intersection for.
-         * @param[in] preserve_epsilon Whether to compute intersection preserving epsilon transitions.
-         * @param[in] epsilons Set of symbols to be considered as epsilons
-         * @param[out] prod_map Mapping of pairs of the original states (lhs_state, rhs_state) to new product states.
-         * @return NFA as a product of NFAs @p lhs and @p rhs with ε-transitions preserved.
-         */
-        Nfa intersection_eps(const Nfa& lhs, const Nfa& rhs, bool preserve_epsilon, const std::set<Symbol>& epsilons,
-            std::unordered_map<std::pair<State,State>, State> *prod_map = nullptr);
-
-        /**
-         * @brief Concatenate two NFAs.
-         *
-         * Supports epsilon symbols when @p use_epsilon is set to true.
-         * @param[in] lhs First automaton to concatenate.
-         * @param[in] rhs Second automaton to concatenate.
-         * @param[in] epsilon Epsilon to be used co concatenation (provided @p use_epsilon is true)
-         * @param[in] use_epsilon Whether to concatenate over epsilon symbol.
-         * @param[out] lhs_result_states_map Map mapping lhs states to result states.
-         * @param[out] rhs_result_states_map Map mapping rhs states to result states.
-         * @return Concatenated automaton.
-         */
-        Nfa concatenate_eps(const Nfa& lhs, const Nfa& rhs, const Symbol& epsilon, bool use_epsilon = false,
-            StateToStateMap* lhs_result_states_map = nullptr, StateToStateMap* rhs_result_states_map = nullptr);
+
+/**
+ * Brzozowski minimization of automata (revert -> determinize -> revert -> determinize).
+ * @param[in] aut Automaton to be minimized.
+ * @return Minimized automaton.
+ */
+Nfa minimize_brzozowski(const Nfa& aut);
+
+/**
+ * Complement implemented by determization, adding sink state and making automaton complete. Then it adds final states
+ *  which were non final in the original automaton.
+ * @param[in] aut Automaton to be complemented.
+ * @param[in] symbols Symbols needed to make the automaton complete.
+ * @param[in] minimize_during_determinization Whether the determinized automaton is computed by (brzozowski)
+ *  minimization.
+ * @return Complemented automaton.
+ */
+Nfa complement_classical(const Nfa& aut, const Mata::Util::OrdVector<Symbol>& symbols,
+                         bool minimize_during_determinization = false);
+
+/**
+ * Inclusion implemented by complementation of bigger automaton, intersecting it with smaller and then it checks
+ *  emptiness of intersection.
+ * @param[in] smaller Automaton which language should be included in the bigger one.
+ * @param[in] bigger Automaton which language should include the smaller one.
+ * @param[in] alphabet Alphabet of both automata (it is computed automatically, but it is more efficient to set it if
+ *  you have it).
+ * @param[out] cex A potential counterexample word which breaks inclusion
+ * @return True if smaller language is included,
+ * i.e., if the final intersection of smaller complement of bigger is empty.
+ */
+bool is_included_naive(const Nfa& smaller, const Nfa& bigger, const Alphabet* alphabet = nullptr, Run* cex = nullptr);
+
+/**
+ * Inclusion implemented by antichain algorithms.
+ * @param[in] smaller Automaton which language should be included in the bigger one
+ * @param[in] bigger Automaton which language should include the smaller one
+ * @param[in] alphabet Alphabet of both automata (not needed for antichain algorithm)
+ * @param[out] cex A potential counterexample word which breaks inclusion
+ * @return True if smaller language is included,
+ * i.e., if the final intersection of smaller complement of bigger is empty.
+ */
+bool is_included_antichains(const Nfa& smaller, const Nfa& bigger, const Alphabet*  alphabet = nullptr, Run* cex = nullptr);
+
+/**
+ * Universality check implemented by checking emptiness of complemented automaton
+ * @param[in] aut Automaton which universality is checked
+ * @param[in] alphabet Alphabet of the automaton
+ * @param[out] cex Counterexample word which eventually breaks the universality
+ * @return True if the complemented automaton has non empty language, i.e., the original one is not universal
+ */
+bool is_universal_naive(const Nfa& aut, const Alphabet& alphabet, Run* cex);
+
+/**
+ * Universality checking based on subset construction with antichain.
+ * @param[in] aut Automaton which universality is checked
+ * @param[in] alphabet Alphabet of the automaton
+ * @param[out] cex Counterexample word which eventually breaks the universality
+ * @return True if the automaton is universal, otherwise false.
+ */
+bool is_universal_antichains(const Nfa& aut, const Alphabet& alphabet, Run* cex);
+
+Simlib::Util::BinaryRelation compute_relation(
+        const Nfa& aut,
+        const StringMap&  params = {{"relation", "simulation"}, {"direction", "forward"}});
+
+/**
+ * @brief Compute intersection of two NFAs with a possibility of using multiple epsilons.
+ *
+ * @param[in] lhs First NFA to compute intersection for.
+ * @param[in] rhs Second NFA to compute intersection for.
+ * @param[in] preserve_epsilon Whether to compute intersection preserving epsilon transitions.
+ * @param[in] epsilons Set of symbols to be considered as epsilons
+ * @param[out] prod_map Mapping of pairs of the original states (lhs_state, rhs_state) to new product states.
+ * @return NFA as a product of NFAs @p lhs and @p rhs with ε-transitions preserved.
+ */
+Nfa intersection_eps(const Nfa& lhs, const Nfa& rhs, bool preserve_epsilon, const std::set<Symbol>& epsilons,
+    std::unordered_map<std::pair<State,State>, State> *prod_map = nullptr);
+
+/**
+ * @brief Concatenate two NFAs.
+ *
+ * Supports epsilon symbols when @p use_epsilon is set to true.
+ * @param[in] lhs First automaton to concatenate.
+ * @param[in] rhs Second automaton to concatenate.
+ * @param[in] epsilon Epsilon to be used co concatenation (provided @p use_epsilon is true)
+ * @param[in] use_epsilon Whether to concatenate over epsilon symbol.
+ * @param[out] lhs_result_states_map Map mapping lhs states to result states.
+ * @param[out] rhs_result_states_map Map mapping rhs states to result states.
+ * @return Concatenated automaton.
+ */
+Nfa concatenate_eps(const Nfa& lhs, const Nfa& rhs, const Symbol& epsilon, bool use_epsilon = false,
+    StateToStateMap* lhs_result_states_map = nullptr, StateToStateMap* rhs_result_states_map = nullptr);
+
 } // Namespace Mata::Nfa::Algorithms.
 
 #endif // MATA_NFA_INTERNALS_HH_
```

### Comparing `libmata-0.66.0/mata/include/mata/nfa-strings.hh` & `libmata-0.67.0/mata/include/mata/nfa-strings.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 /* nfa-strings.hh -- Operations on NFAs for string solving.
  *
- * Copyright (c) 2022 David Chocholatý <chocholaty.david@protonmail.com>
- *
  * This file is a part of libmata.
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 3 of the License, or
  * (at your option) any later version.
  *
@@ -17,410 +15,410 @@
 
 #ifndef MATA_NFA_STRING_SOLVING_HH_
 #define MATA_NFA_STRING_SOLVING_HH_
 
 #include <memory>
 #include <optional>
 
-#include <mata/nfa.hh>
+#include "mata/nfa.hh"
 
 namespace {
     using namespace Mata::Nfa;
 }
 
-namespace Mata {
 /**
  * NFA Algorithms usable for solving string constraints.
  */
-namespace Strings {
+namespace Mata::Strings {
+
+/**
+ * Class mapping states to the shortest words accepted by languages of the states.
+ */
+class ShortestWordsMap {
+public:
     /**
-     * Class mapping states to the shortest words accepted by languages of the states.
+     * Maps states in the automaton @p aut to shortest words accepted by languages of the states.
+     * @param aut Automaton to compute shortest words for.
      */
-    class ShortestWordsMap {
-    public:
-        /**
-         * Maps states in the automaton @p aut to shortest words accepted by languages of the states.
-         * @param aut Automaton to compute shortest words for.
-         */
-        explicit ShortestWordsMap(const Nfa::Nfa& aut) : reversed_automaton(revert(aut)) {
-            insert_initial_lengths();
-            compute();
-        }
-
-        /**
-         * Gets shortest words for the given @p states.
-         * @param[in] states States to map shortest words for.
-         * @return Set of shortest words.
-         */
-        WordSet get_shortest_words_for(const StateSet& states) const;
-
-        /**
-         * Gets shortest words for the given @p state.
-         * @param[in] state State to map shortest words for.
-         * @return Set of shortest words.
-         */
-        WordSet get_shortest_words_for(State state) const;
-
-    private:
-        using WordLength = int; ///< A length of a word.
-        /// Pair binding the length of all words in the word set and word set with words of the given length.
-        using LengthWordsPair = std::pair<WordLength, WordSet>;
-        /// Map mapping states to the shortest words accepted by the automaton from the mapped state.
-        std::unordered_map<State, LengthWordsPair> shortest_words_map{};
-        std::set<State> processed{}; ///< Set of already processed states.
-        std::deque<State> fifo_queue{}; ///< FIFO queue for states to process.
-        const Nfa::Nfa reversed_automaton; ///< Reversed input automaton.
-
-        /**
-         * @brief Inserts initial lengths into the shortest words map.
-         *
-         * Inserts initial length of length 0 for final state in the automaton (initial states in the reversed automaton).
-         */
-        void insert_initial_lengths();
-
-        /**
-         * Computes shortest words for all states in the automaton.
-         */
-        void compute();
-
-        /**
-         * Computes shortest words for the given @p state.
-         * @param[in] state State to compute shortest words for.
-         */
-        void compute_for_state(State state);
-
-        /**
-         * Creates default shortest words mapping for yet unprocessed @p state.
-         * @param[in] state State to map default shortest words.
-         * @return Created default shortest words map element for the given @p state.
-         */
-        LengthWordsPair map_default_shortest_words(const State state) {
-            return shortest_words_map.emplace(state, std::make_pair(-1, WordSet{})).first->second;
-        }
-
-        /**
-         * Update words for the current state.
-         * @param[out] act Current state shortest words and length.
-         * @param[in] dst Transition target state shortest words and length.
-         * @param[in] symbol Symbol to update with.
-         */
-        static void update_current_words(LengthWordsPair& act, const LengthWordsPair& dst, Symbol symbol);
-    }; // Class ShortestWordsMap.
+    explicit ShortestWordsMap(const Nfa::Nfa& aut) : reversed_automaton(revert(aut)) {
+        insert_initial_lengths();
+        compute();
+    }
 
     /**
-     * Get shortest words (regarding their length) of the automaton using BFS.
+     * Gets shortest words for the given @p states.
+     * @param[in] states States to map shortest words for.
      * @return Set of shortest words.
      */
-    WordSet get_shortest_words(const Nfa::Nfa& nfa);
+    WordSet get_shortest_words_for(const StateSet& states) const;
 
     /**
-     * @brief Get the lengths of all words in the automaton @p aut. The function returns a set of pairs <u,v> where for each
-     * such a pair there is a word with length u+k*v for all ks. The disjunction of such formulae of all pairs hence precisely
-     * describe lengths of all words in the automaton.
-     *
-     * @param aut Input automaton
-     * @return Set of pairs describing lengths
+     * Gets shortest words for the given @p state.
+     * @param[in] state State to map shortest words for.
+     * @return Set of shortest words.
      */
-    std::set<std::pair<int, int>> get_word_lengths(const Nfa::Nfa& aut);
+    WordSet get_shortest_words_for(State state) const;
+
+private:
+    using WordLength = int; ///< A length of a word.
+    /// Pair binding the length of all words in the word set and word set with words of the given length.
+    using LengthWordsPair = std::pair<WordLength, WordSet>;
+    /// Map mapping states to the shortest words accepted by the automaton from the mapped state.
+    std::unordered_map<State, LengthWordsPair> shortest_words_map{};
+    std::set<State> processed{}; ///< Set of already processed states.
+    std::deque<State> fifo_queue{}; ///< FIFO queue for states to process.
+    const Nfa::Nfa reversed_automaton; ///< Reversed input automaton.
 
     /**
-     * @brief Checks if the automaton @p nfa accepts only a single word \eps.
+     * @brief Inserts initial lengths into the shortest words map.
      *
-     * @param nfa Input automaton
-     * @return true iff L(nfa) = {\eps}
+     * Inserts initial length of length 0 for final state in the automaton (initial states in the reversed automaton).
      */
-    bool is_lang_eps(const Nfa::Nfa& nfa);
+    void insert_initial_lengths();
 
     /**
-     * Create an automaton accepting only a single @p word.
+     * Computes shortest words for all states in the automaton.
      */
-    Nfa::Nfa create_single_word_nfa(const std::vector<Symbol>& word);
+    void compute();
 
     /**
-     * Create an automaton accepting only a single @p word.
-     *
-     * @param word Word to accept.
-     * @param alphabet Alphabet to use in NFA for translating word into symbols. If specified, the alphabet has to contain
-     *  translations for all of the word symbols. If left empty, a new alphabet with only the symbols of the word will be
-     *  created.
+     * Computes shortest words for the given @p state.
+     * @param[in] state State to compute shortest words for.
+     */
+    void compute_for_state(State state);
+
+    /**
+     * Creates default shortest words mapping for yet unprocessed @p state.
+     * @param[in] state State to map default shortest words.
+     * @return Created default shortest words map element for the given @p state.
+     */
+    LengthWordsPair map_default_shortest_words(const State state) {
+        return shortest_words_map.emplace(state, std::make_pair(-1, WordSet{})).first->second;
+    }
+
+    /**
+     * Update words for the current state.
+     * @param[out] act Current state shortest words and length.
+     * @param[in] dst Transition target state shortest words and length.
+     * @param[in] symbol Symbol to update with.
      */
-    Nfa::Nfa create_single_word_nfa(const std::vector<std::string>& word, Alphabet* alphabet = nullptr);
+    static void update_current_words(LengthWordsPair& act, const LengthWordsPair& dst, Symbol symbol);
+}; // Class ShortestWordsMap.
+
+/**
+ * Get shortest words (regarding their length) of the automaton using BFS.
+ * @return Set of shortest words.
+ */
+WordSet get_shortest_words(const Nfa::Nfa& nfa);
+
+/**
+ * @brief Get the lengths of all words in the automaton @p aut. The function returns a set of pairs <u,v> where for each
+ * such a pair there is a word with length u+k*v for all ks. The disjunction of such formulae of all pairs hence precisely
+ * describe lengths of all words in the automaton.
+ *
+ * @param aut Input automaton
+ * @return Set of pairs describing lengths
+ */
+std::set<std::pair<int, int>> get_word_lengths(const Nfa::Nfa& aut);
+
+/**
+ * @brief Checks if the automaton @p nfa accepts only a single word \eps.
+ *
+ * @param nfa Input automaton
+ * @return true iff L(nfa) = {\eps}
+ */
+bool is_lang_eps(const Nfa::Nfa& nfa);
+
+/**
+ * Create an automaton accepting only a single @p word.
+ */
+Nfa::Nfa create_single_word_nfa(const std::vector<Symbol>& word);
+
+/**
+ * Create an automaton accepting only a single @p word.
+ *
+ * @param word Word to accept.
+ * @param alphabet Alphabet to use in NFA for translating word into symbols. If specified, the alphabet has to contain
+ *  translations for all of the word symbols. If left empty, a new alphabet with only the symbols of the word will be
+ *  created.
+ */
+Nfa::Nfa create_single_word_nfa(const std::vector<std::string>& word, Alphabet* alphabet = nullptr);
 
 /**
  * Segment Automata including structs and algorithms.
  *
  * These are automata whose state space can be split into several segments connected by ε-transitions in a chain.
  * No other ε-transitions are allowed. As a consequence, no ε-transitions can appear in a cycle.
  * Segment automaton can have initial states only in the first segment and final states only in the last segment.
  */
 namespace SegNfa {
-    using SegNfa = Nfa::Nfa;
-    using VisitedEpsMap = std::map<State, std::map<Symbol, unsigned>>;
 
-    /// Number of visited epsilons
-    using EpsCntMap = std::map<Symbol, unsigned>;
-    /// Projection of EpsCntMap to sorted keys (desc)
-    using EpsCntVector = std::vector<unsigned>;
-
-    /**
-    * Class executing segmentation operations for a given segment automaton. Works only with segment automata.
-    */
-    class Segmentation {
-    public:
-        using EpsilonDepth = unsigned; ///< Depth of ε-transitions.
-        /// Dictionary of lists of ε-transitions grouped by their depth.
-        /// For each depth 'i' we have 'depths[i]' which contains a list of ε-transitions of depth 'i'.
-        using EpsilonDepthTransitions = std::unordered_map<EpsilonDepth, TransSequence>;
-        using EpsilonDepthTransitionMap = std::unordered_map<EpsilonDepth, std::unordered_map<State,TransSequence>>;
-
-        /**
-         * Prepare automaton @p aut for segmentation.
-         * @param[in] aut Segment automaton to make segments for.
-         * @param[in] epsilon Symbol to execute segmentation for.
-         */
-        explicit Segmentation(const SegNfa& aut, const std::set<Symbol> epsilons) : epsilons(epsilons), automaton(aut) {
-            compute_epsilon_depths(); // Map depths to epsilon transitions.
-        }
-
-        /**
-         * Get segmentation depths for ε-transitions.
-         * @return Map of depths to lists of ε-transitions.
-         */
-        const EpsilonDepthTransitions& get_epsilon_depths() const { return epsilon_depth_transitions; }
-
-        /**
-         * Get the epsilon depth trans map object (mapping of depths and states to eps-successors)
-         *
-         * @return Map of depths to a map of states to transitions
-         */
-        const EpsilonDepthTransitionMap& get_epsilon_depth_trans_map() const { return this->eps_depth_trans_map; }
-
-        /**
-         * Get segment automata.
-         * @return A vector of segments for the segment automaton in the order from the left (initial state in segment automaton)
-         * to the right (final states of segment automaton).
-         */
-        const AutSequence& get_segments();
-
-        /**
-         * Get raw segment automata.
-         * @return A vector of segments for the segment automaton in the order from the left (initial state in segment automaton)
-         * to the right (final states of segment automaton) without trimming (the states are same as in the original automaton).
-         */
-        const AutSequence& get_untrimmed_segments();
-
-        const VisitedEpsMap& get_visited_eps() const { return this->visited_eps; }
-
-    private:
-        const std::set<Symbol> epsilons; ///< Symbol for which to execute segmentation.
-        /// Automaton to execute segmentation for. Must be a segment automaton (can be split into @p segments).
-        const SegNfa& automaton;
-        EpsilonDepthTransitions epsilon_depth_transitions{}; ///< Epsilon depths.
-        EpsilonDepthTransitionMap eps_depth_trans_map{}; /// Epsilon depths with mapping of states to epsilon transitions
-        AutSequence segments{}; ///< Segments for @p automaton.
-        AutSequence segments_raw{}; ///< Raw segments for @p automaton.
-        VisitedEpsMap visited_eps{}; /// number of visited eps for each state
-
-        /**
-         * Pair of state and its depth.
-         */
-        struct StateDepthTuple {
-            State state; ///< State with a depth.
-            EpsilonDepth depth; ///< Depth of a state.
-            EpsCntMap eps; /// visited epsilons and their numbers
-        };
-
-        /**
-         * Compute epsilon depths with their transitions.
-         */
-        void compute_epsilon_depths();
-
-        /**
-         * Split segment @c automaton into @c segments.
-         */
-        void split_aut_into_segments();
-
-        /**
-         * Propagate changes to the current segment automaton to the next segment automaton.
-         * @param[in] current_depth Current depth.
-         * @param[in] transition Current epsilon transition.
-         */
-        void update_next_segment(size_t current_depth, const Trans& transition);
-
-        /**
-         * Update current segment automaton.
-         * @param[in] current_depth Current depth.
-         * @param[in] transition Current epsilon transition.
-         */
-        void update_current_segment(size_t current_depth, const Trans& transition);
-
-        /**
-         * Initialize map of visited states.
-         * @return Map of visited states.
-         */
-        std::unordered_map<State, bool> initialize_visited_map() const;
-
-        /**
-         * Initialize worklist of states with depths to process.
-         * @return Queue of state and its depth pairs.
-         */
-        std::deque<StateDepthTuple> initialize_worklist() const;
-
-        /**
-         * Process pair of state and its depth.
-         * @param[in] state_depth_pair Current state depth pair.
-         * @param[out] worklist Worklist of state and depth pairs to process.
-         */
-        void process_state_depth_pair(const StateDepthTuple& state_depth_pair, std::deque<StateDepthTuple>& worklist);
-
-        /**
-         * Add states with non-epsilon transitions to the @p worklist.
-         * @param state_transitions[in] Transitions from current state.
-         * @param depth[in] Current depth.
-         * @param worklist[out] Worklist of state and depth pairs to process.
-         */
-        void add_transitions_to_worklist(const StateDepthTuple& state_depth_pair, const Move& state_transitions,
-                                                std::deque<StateDepthTuple>& worklist);
-
-        /**
-         * Process epsilon transitions for the current state.
-         * @param[in] state_depth_pair Current state depth pair.
-         * @param[in] state_transitions Transitions from current state.
-         * @param[out] worklist Worklist of state and depth pairs to process.
-         */
-        void handle_epsilon_transitions(const StateDepthTuple& state_depth_pair, const Move& state_transitions,
-                                        std::deque<StateDepthTuple>& worklist);
-
-        /**
-         * @brief Remove inner initial and final states.
-         *
-         * Remove all initial states for all segments but the first one and all final states for all segments but the
-         *  last one.
-         */
-        void remove_inner_initial_and_final_states();
-    }; // Class Segmentation.
-
-    /// A noodle is represented as a sequence of segments (a copy of the segment automata) created as if there was exactly
-    ///  one ε-transition between each two consecutive segments.
-    using Noodle = std::vector<SharedPtrAut>;
-    using NoodleSequence = std::vector<Noodle>; ///< A sequence of noodles.
-
-    /// Noodles as segments enriched with EpsCntMap
-    using NoodleSubst = std::vector<std::pair<SharedPtrAut, EpsCntVector>>;
-    using NoodleSubstSequence = std::vector<NoodleSubst>;
+using SegNfa = Nfa::Nfa;
+using VisitedEpsMap = std::map<State, std::map<Symbol, unsigned>>;
+
+/// Number of visited epsilons
+using EpsCntMap = std::map<Symbol, unsigned>;
+/// Projection of EpsCntMap to sorted keys (desc)
+using EpsCntVector = std::vector<unsigned>;
+
+/**
+* Class executing segmentation operations for a given segment automaton. Works only with segment automata.
+*/
+class Segmentation {
+public:
+    using EpsilonDepth = unsigned; ///< Depth of ε-transitions.
+    /// Dictionary of lists of ε-transitions grouped by their depth.
+    /// For each depth 'i' we have 'depths[i]' which contains a list of ε-transitions of depth 'i'.
+    using EpsilonDepthTransitions = std::unordered_map<EpsilonDepth, TransSequence>;
+    using EpsilonDepthTransitionMap = std::unordered_map<EpsilonDepth, std::unordered_map<State,TransSequence>>;
 
     /**
-     * @brief segs_one_initial_final
-     *
-     * segments_one_initial_final[init, final] is the pointer to automaton created from one of
-     * the segments such that init and final are one of the initial and final states of the segment
-     * and the created automaton takes this segment, sets initial={init}, final={final}
-     * and trims it; also segments_one_initial_final[unused_state, final] is used for the first
-     * segment (where we always want all initial states, only final state changes) and
-     * segments_one_initial_final[init, unused_state] is similarly for the last segment
-     * TODO: should we use unordered_map? then we need hash
+     * Prepare automaton @p aut for segmentation.
+     * @param[in] aut Segment automaton to make segments for.
+     * @param[in] epsilon Symbol to execute segmentation for.
      */
-    void segs_one_initial_final(const Mata::Nfa::AutSequence& segments, bool include_empty,
-        const State& unused_state, std::map<std::pair<State, State>, std::shared_ptr<Nfa::Nfa>>& out);
+    explicit Segmentation(const SegNfa& aut, const std::set<Symbol>& epsilons) : epsilons(epsilons), automaton(aut) {
+        compute_epsilon_depths(); // Map depths to epsilon transitions.
+    }
 
     /**
-     * @brief Create noodles from segment automaton @p aut.
-     *
-     * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
-     * A noodle is a vector of pointers to copy of the segments automata created as if there was exactly one ε-transition
-     *  between each two consecutive segments.
-     *
-     * @param[in] automaton Segment automaton to noodlify.
-     * @param[in] epsilon Epsilon symbol to noodlify for.
-     * @param[in] include_empty Whether to also include empty noodles.
-     * @return A list of all (non-empty) noodles.
+     * Get segmentation depths for ε-transitions.
+     * @return Map of depths to lists of ε-transitions.
      */
-    NoodleSequence noodlify(const SegNfa& aut, Symbol epsilon, bool include_empty = false);
+    const EpsilonDepthTransitions& get_epsilon_depths() const { return epsilon_depth_transitions; }
 
     /**
-     * @brief Create noodles from segment automaton @p aut.
-     *
-     * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
-     * A noodle is a vector of pointers to copy of the segments automata created as if there was exactly one ε-transition
-     *  between each two consecutive segments.
+     * Get the epsilon depth trans map object (mapping of depths and states to eps-successors)
      *
-     * @param[in] automaton Segment automaton to noodlify.
-     * @param[in] epsilons Epsilon symbols to noodlify for.
-     * @param[in] include_empty Whether to also include empty noodles.
-     * @return A list of all (non-empty) noodles.
+     * @return Map of depths to a map of states to transitions
      */
-    NoodleSubstSequence noodlify_mult_eps(const SegNfa& aut, const std::set<Symbol>& epsilons, bool include_empty = false);
+    const EpsilonDepthTransitionMap& get_epsilon_depth_trans_map() const { return this->eps_depth_trans_map; }
 
     /**
-     * @brief Create noodles for left and right side of equation.
-     *
-     * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
-     * A noodle is a copy of the segment automaton with exactly one ε-transition between each two consecutive segments.
-     *
-     * Mata cannot work with equations, queries etc. Hence, we compute the noodles for the equation, but represent
-     *  the equation in a way that libMata understands. The left side automata represent the left side of the equation
-     *  and the right automaton represents the right side of the equation. To create noodles, we need a segment automaton
-     *  representing the intersection. That can be achieved by computing a product of both sides. First, the left side
-     *  has to be concatenated over an epsilon transitions into a single automaton to compute the intersection on, though.
-     *
-     * @param[in] left_automata Sequence of segment automata for left side of an equation to noodlify.
-     * @param[in] right_automaton Segment automaton for right side of an equation to noodlify.
-     * @param[in] include_empty Whether to also include empty noodles.
-     * @param[in] params Additional parameters for the noodlification:
-     *     - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
-     *                 minimization before noodlification.
-     * @return A list of all (non-empty) noodles.
+     * Get segment automata.
+     * @return A vector of segments for the segment automaton in the order from the left (initial state in segment automaton)
+     * to the right (final states of segment automaton).
      */
-    NoodleSequence noodlify_for_equation(const AutRefSequence& left_automata, const Nfa::Nfa& right_automaton,
-                                         bool include_empty = false, const StringMap& params = {{"reduce", "false"}});
+    const AutSequence& get_segments();
 
     /**
-     * @brief Create noodles for left and right side of equation.
-     *
-     * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
-     * A noodle is a copy of the segment automaton with exactly one ε-transition between each two consecutive segments.
-     *
-     * Mata cannot work with equations, queries etc. Hence, we compute the noodles for the equation, but represent
-     *  the equation in a way that libMata understands. The left side automata represent the left side of the equation
-     *  and the right automaton represents the right side of the equation. To create noodles, we need a segment automaton
-     *  representing the intersection. That can be achieved by computing a product of both sides. First, the left side
-     *  has to be concatenated over an epsilon transitions into a single automaton to compute the intersection on, though.
-     *
-     * @param[in] left_automata Sequence of pointers to segment automata for left side of an equation to noodlify.
-     * @param[in] right_automaton Segment automaton for right side of an equation to noodlify.
-     * @param[in] include_empty Whether to also include empty noodles.
-     * @param[in] params Additional parameters for the noodlification:
-     *     - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
-     *                 minimization before noodlification.
-     * @return A list of all (non-empty) noodles.
+     * Get raw segment automata.
+     * @return A vector of segments for the segment automaton in the order from the left (initial state in segment automaton)
+     * to the right (final states of segment automaton) without trimming (the states are same as in the original automaton).
      */
-    NoodleSequence noodlify_for_equation(const AutPtrSequence& left_automata, const Nfa::Nfa& right_automaton,
-                                         bool include_empty = false, const StringMap& params = {{"reduce", "false"}});
+    const AutSequence& get_untrimmed_segments();
+
+    const VisitedEpsMap& get_visited_eps() const { return this->visited_eps; }
+
+private:
+    const std::set<Symbol> epsilons; ///< Symbol for which to execute segmentation.
+    /// Automaton to execute segmentation for. Must be a segment automaton (can be split into @p segments).
+    const SegNfa& automaton;
+    EpsilonDepthTransitions epsilon_depth_transitions{}; ///< Epsilon depths.
+    EpsilonDepthTransitionMap eps_depth_trans_map{}; /// Epsilon depths with mapping of states to epsilon transitions
+    AutSequence segments{}; ///< Segments for @p automaton.
+    AutSequence segments_raw{}; ///< Raw segments for @p automaton.
+    VisitedEpsMap visited_eps{}; /// number of visited eps for each state
 
     /**
-     * @brief Create noodles for left and right side of equation (both sides are given as a sequence of automata).
-     *
-     * @param[in] left_automata Sequence of pointers to segment automata for left side of an equation to noodlify.
-     * @param[in] right_automaton Sequence of pointers to segment automata for right side of an equation to noodlify.
-     * @param[in] include_empty Whether to also include empty noodles.
-     * @param[in] params Additional parameters for the noodlification:
-     *     - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
-     *                 minimization before noodlification.
-     * @return A list of all (non-empty) noodles together with the positions reached from the beginning of left/right side.
+     * Pair of state and its depth.
+     */
+    struct StateDepthTuple {
+        State state; ///< State with a depth.
+        EpsilonDepth depth; ///< Depth of a state.
+        EpsCntMap eps; /// visited epsilons and their numbers
+    };
+
+    /**
+     * Compute epsilon depths with their transitions.
      */
-    NoodleSubstSequence noodlify_for_equation(const std::vector<std::shared_ptr<Nfa::Nfa>>& left_automata, const std::vector<std::shared_ptr<Nfa::Nfa>>& right_automata,
-                                                     bool include_empty = false, const StringMap& params = {{"reduce", "false"}});
+    void compute_epsilon_depths();
 
     /**
-     * @brief Process epsilon map to a sequence of values (sorted according to key desc)
+     * Split segment @c automaton into @c segments.
+     */
+    void split_aut_into_segments();
+
+    /**
+     * Propagate changes to the current segment automaton to the next segment automaton.
+     * @param[in] current_depth Current depth.
+     * @param[in] transition Current epsilon transition.
+     */
+    void update_next_segment(size_t current_depth, const Trans& transition);
+
+    /**
+     * Update current segment automaton.
+     * @param[in] current_depth Current depth.
+     * @param[in] transition Current epsilon transition.
+     */
+    void update_current_segment(size_t current_depth, const Trans& transition);
+
+    /**
+     * Initialize map of visited states.
+     * @return Map of visited states.
+     */
+    std::unordered_map<State, bool> initialize_visited_map() const;
+
+    /**
+     * Initialize worklist of states with depths to process.
+     * @return Queue of state and its depth pairs.
+     */
+    std::deque<StateDepthTuple> initialize_worklist() const;
+
+    /**
+     * Process pair of state and its depth.
+     * @param[in] state_depth_pair Current state depth pair.
+     * @param[out] worklist Worklist of state and depth pairs to process.
+     */
+    void process_state_depth_pair(const StateDepthTuple& state_depth_pair, std::deque<StateDepthTuple>& worklist);
+
+    /**
+     * Add states with non-epsilon transitions to the @p worklist.
+     * @param state_transitions[in] Transitions from current state.
+     * @param depth[in] Current depth.
+     * @param worklist[out] Worklist of state and depth pairs to process.
+     */
+    void add_transitions_to_worklist(const StateDepthTuple& state_depth_pair, const Move& state_transitions,
+                                     std::deque<StateDepthTuple>& worklist);
+
+    /**
+     * Process epsilon transitions for the current state.
+     * @param[in] state_depth_pair Current state depth pair.
+     * @param[in] state_transitions Transitions from current state.
+     * @param[out] worklist Worklist of state and depth pairs to process.
+     */
+    void handle_epsilon_transitions(const StateDepthTuple& state_depth_pair, const Move& state_transitions,
+                                    std::deque<StateDepthTuple>& worklist);
+
+    /**
+     * @brief Remove inner initial and final states.
      *
-     * @param eps_cnt Epsilon count
-     * @return Vector of keys (count of epsilons)
+     * Remove all initial states for all segments but the first one and all final states for all segments but the
+     *  last one.
      */
-    EpsCntVector process_eps_map(const EpsCntMap& eps_cnt);
+    void remove_inner_initial_and_final_states();
+}; // Class Segmentation.
+
+/// A noodle is represented as a sequence of segments (a copy of the segment automata) created as if there was exactly
+///  one ε-transition between each two consecutive segments.
+using Noodle = std::vector<SharedPtrAut>;
+using NoodleSequence = std::vector<Noodle>; ///< A sequence of noodles.
+
+/// Noodles as segments enriched with EpsCntMap
+using NoodleSubst = std::vector<std::pair<SharedPtrAut, EpsCntVector>>;
+using NoodleSubstSequence = std::vector<NoodleSubst>;
+
+/**
+ * @brief segs_one_initial_final
+ *
+ * segments_one_initial_final[init, final] is the pointer to automaton created from one of
+ * the segments such that init and final are one of the initial and final states of the segment
+ * and the created automaton takes this segment, sets initial={init}, final={final}
+ * and trims it; also segments_one_initial_final[unused_state, final] is used for the first
+ * segment (where we always want all initial states, only final state changes) and
+ * segments_one_initial_final[init, unused_state] is similarly for the last segment
+ * TODO: should we use unordered_map? then we need hash
+ */
+void segs_one_initial_final(const Mata::Nfa::AutSequence& segments, bool include_empty,
+    const State& unused_state, std::map<std::pair<State, State>, std::shared_ptr<Nfa::Nfa>>& out);
+
+/**
+ * @brief Create noodles from segment automaton @p aut.
+ *
+ * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
+ * A noodle is a vector of pointers to copy of the segments automata created as if there was exactly one ε-transition
+ *  between each two consecutive segments.
+ *
+ * @param[in] automaton Segment automaton to noodlify.
+ * @param[in] epsilon Epsilon symbol to noodlify for.
+ * @param[in] include_empty Whether to also include empty noodles.
+ * @return A list of all (non-empty) noodles.
+ */
+NoodleSequence noodlify(const SegNfa& aut, Symbol epsilon, bool include_empty = false);
+
+/**
+ * @brief Create noodles from segment automaton @p aut.
+ *
+ * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
+ * A noodle is a vector of pointers to copy of the segments automata created as if there was exactly one ε-transition
+ *  between each two consecutive segments.
+ *
+ * @param[in] automaton Segment automaton to noodlify.
+ * @param[in] epsilons Epsilon symbols to noodlify for.
+ * @param[in] include_empty Whether to also include empty noodles.
+ * @return A list of all (non-empty) noodles.
+ */
+NoodleSubstSequence noodlify_mult_eps(const SegNfa& aut, const std::set<Symbol>& epsilons, bool include_empty = false);
+
+/**
+ * @brief Create noodles for left and right side of equation.
+ *
+ * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
+ * A noodle is a copy of the segment automaton with exactly one ε-transition between each two consecutive segments.
+ *
+ * Mata cannot work with equations, queries etc. Hence, we compute the noodles for the equation, but represent
+ *  the equation in a way that libMata understands. The left side automata represent the left side of the equation
+ *  and the right automaton represents the right side of the equation. To create noodles, we need a segment automaton
+ *  representing the intersection. That can be achieved by computing a product of both sides. First, the left side
+ *  has to be concatenated over an epsilon transitions into a single automaton to compute the intersection on, though.
+ *
+ * @param[in] left_automata Sequence of segment automata for left side of an equation to noodlify.
+ * @param[in] right_automaton Segment automaton for right side of an equation to noodlify.
+ * @param[in] include_empty Whether to also include empty noodles.
+ * @param[in] params Additional parameters for the noodlification:
+ *     - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
+ *                 minimization before noodlification.
+ * @return A list of all (non-empty) noodles.
+ */
+NoodleSequence noodlify_for_equation(const AutRefSequence& left_automata, const Nfa::Nfa& right_automaton,
+                                     bool include_empty = false, const StringMap& params = {{"reduce", "false"}});
+
+/**
+ * @brief Create noodles for left and right side of equation.
+ *
+ * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
+ * A noodle is a copy of the segment automaton with exactly one ε-transition between each two consecutive segments.
+ *
+ * Mata cannot work with equations, queries etc. Hence, we compute the noodles for the equation, but represent
+ *  the equation in a way that libMata understands. The left side automata represent the left side of the equation
+ *  and the right automaton represents the right side of the equation. To create noodles, we need a segment automaton
+ *  representing the intersection. That can be achieved by computing a product of both sides. First, the left side
+ *  has to be concatenated over an epsilon transitions into a single automaton to compute the intersection on, though.
+ *
+ * @param[in] left_automata Sequence of pointers to segment automata for left side of an equation to noodlify.
+ * @param[in] right_automaton Segment automaton for right side of an equation to noodlify.
+ * @param[in] include_empty Whether to also include empty noodles.
+ * @param[in] params Additional parameters for the noodlification:
+ *     - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
+ *                 minimization before noodlification.
+ * @return A list of all (non-empty) noodles.
+ */
+NoodleSequence noodlify_for_equation(const AutPtrSequence& left_automata, const Nfa::Nfa& right_automaton,
+                                     bool include_empty = false, const StringMap& params = {{"reduce", "false"}});
+
+/**
+ * @brief Create noodles for left and right side of equation (both sides are given as a sequence of automata).
+ *
+ * @param[in] left_automata Sequence of pointers to segment automata for left side of an equation to noodlify.
+ * @param[in] right_automaton Sequence of pointers to segment automata for right side of an equation to noodlify.
+ * @param[in] include_empty Whether to also include empty noodles.
+ * @param[in] params Additional parameters for the noodlification:
+ *     - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
+ *                 minimization before noodlification.
+ * @return A list of all (non-empty) noodles together with the positions reached from the beginning of left/right side.
+ */
+NoodleSubstSequence noodlify_for_equation(const std::vector<std::shared_ptr<Nfa::Nfa>>& left_automata, const std::vector<std::shared_ptr<Nfa::Nfa>>& right_automata,
+                                                 bool include_empty = false, const StringMap& params = {{"reduce", "false"}});
+
+/**
+ * @brief Process epsilon map to a sequence of values (sorted according to key desc)
+ *
+ * @param eps_cnt Epsilon count
+ * @return Vector of keys (count of epsilons)
+ */
+EpsCntVector process_eps_map(const EpsCntMap& eps_cnt);
 
-} // Namespace SegNfa.
+} // namespace SegNfa.
 
-} // Namespace Strings.
-} // Namespace Mata.
+} // namespace Mata::Strings.
 
 #endif // MATA_NFA_STRING_SOLVING_HH_.
```

### Comparing `libmata-0.66.0/mata/include/mata/nfa.hh` & `libmata-0.67.0/mata/include/mata/nfa.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-/* nfa.hh -- nondeterministic finite automaton (over finite words)
- *
- * Copyright (c) 2018 Ondrej Lengal <ondra.lengal@gmail.com>
+/* nfa.hh -- Nondeterministic finite automaton (over finite words).
  *
  * This file is a part of libmata.
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#ifndef _MATA_NFA_HH_
-#define _MATA_NFA_HH_
+#ifndef MATA_NFA_HH_
+#define MATA_NFA_HH_
 
-//#define _STATIC_STRUCTURES_ //static data structures, such as search stack, in algorithms. Might have some effect on some algorithms (like fragile_revert)
+// Static data structures, such as search stack, in algorithms. Might have some effect on some algorithms (like
+//  fragile_revert).
+//#define _STATIC_STRUCTURES_
 
 #include <algorithm>
 #include <cassert>
 #include <cstdint>
 #include <memory>
 #include <limits>
 #include <set>
 #include <unordered_map>
 #include <unordered_set>
 #include <utility>
 #include <vector>
 
-// MATA headers
-#include <mata/alphabet.hh>
-#include <mata/parser.hh>
-#include <mata/util.hh>
-#include <mata/ord-vector.hh>
-#include <mata/inter-aut.hh>
-#include <mata/synchronized-iterator.hh>
+#include "mata/alphabet.hh"
+#include "mata/parser.hh"
+#include "mata/util.hh"
+#include "mata/ord-vector.hh"
+#include "mata/inter-aut.hh"
+#include "mata/synchronized-iterator.hh"
 
 /**
  * Nondeterministic Finite Automata including structures, transitions and algorithms.
  *
  * In particular, this includes:
  *   1. Structures (Automaton, Transitions, Results, Delta),
  *   2. Algorithms (operations, checks, tests),
@@ -75,31 +74,30 @@
 /*TODO: this should become a part of the automaton somehow.
  * It should be a vector indexed by states.
  * */
 
 using StringMap = std::unordered_map<std::string, std::string>;
 
 /*TODO: What about to
- * have names Set, UMap/OMap, State, Symbol, Sequence... and name by Set<State>, State<UMap>, ...
+ * have names Set, UMap/OMap, State, Symbol, Sequence... and name by Set<State>, UMap<State>, ...
  * maybe something else is needed for the more complex maps*/
 
-static constexpr struct Limits {
-    State maxState = std::numeric_limits<State>::max();
-    State minState = std::numeric_limits<State>::min();
-    Symbol maxSymbol = std::numeric_limits<Symbol>::max();
-    Symbol minSymbol = std::numeric_limits<Symbol>::min();
-} limits;
+struct Limits {
+    static const State maxState = std::numeric_limits<State>::max();
+    static const State minState = std::numeric_limits<State>::min();
+    static const Symbol maxSymbol = std::numeric_limits<Symbol>::max();
+    static const Symbol minSymbol = std::numeric_limits<Symbol>::min();
+};
 
 /*TODO: Ideally remove functions using this struct as a parameter.
  * unpack the trans. relation to transitions is inefficient, goes against the hairs of the library.
  * Do we want to support it?
  */
-/// A transition.
-struct Trans
-{
+/// A single transition.
+struct Trans {
 	State src;
 	Symbol symb;
 	State tgt;
 
 	Trans() : src(), symb(), tgt() { }
 	Trans(State src, Symbol symb, State tgt) : src(src), symb(symb), tgt(tgt) { }
 
@@ -136,36 +134,29 @@
 /// serializes Nfa into a ParsedSection
 Mata::Parser::ParsedSection serialize(
 	const Nfa&                aut,
 	const SymbolToStringMap*  symbol_map = nullptr,
 	const StateToStringMap*   state_map = nullptr);
 
 /**
- * Structure represents a move which is symbol and set of right-handed states of transitions.
+ * Structure represents a move which is a symbol and a set of target states of transitions.
  */
 struct Move {
+public:
     Symbol symbol{};
-    StateSet targets;
+    StateSet targets{};
 
     Move() = default;
-    explicit Move(Symbol symbolOnTransition) : symbol(symbolOnTransition), targets() {}
-    Move(Symbol symbolOnTransition, State states_to) :
-            symbol(symbolOnTransition), targets{states_to} {}
-    Move(Symbol symbolOnTransition, const StateSet& states_to) :
-            symbol(symbolOnTransition), targets(states_to) {}
+    explicit Move(Symbol symbol) : symbol{ symbol }, targets{} {}
+    Move(Symbol symbol, State state_to) : symbol{ symbol }, targets{ state_to } {}
+    Move(Symbol symbol, StateSet states_to) : symbol{ symbol }, targets{ std::move(states_to) } {}
 
     Move(Move&& rhs) noexcept : symbol{ rhs.symbol }, targets{ std::move(rhs.targets) } {}
     Move(const Move& rhs) = default;
-    Move& operator=(Move&& rhs) noexcept {
-        if (*this != rhs) {
-            symbol = rhs.symbol;
-            targets = std::move(rhs.targets);
-        }
-        return *this;
-    }
+    Move& operator=(Move&& rhs) noexcept;
     Move& operator=(const Move& rhs) = default;
 
     inline bool operator<(const Move& rhs) const { return symbol < rhs.symbol; }
     inline bool operator<=(const Move& rhs) const { return symbol <= rhs.symbol; }
     inline bool operator==(const Move& rhs) const { return symbol == rhs.symbol; }
     inline bool operator!=(const Move& rhs) const { return symbol != rhs.symbol; }
     inline bool operator>(const Move& rhs) const { return symbol > rhs.symbol; }
@@ -177,40 +168,25 @@
     StateSet::const_iterator cbegin() const  { return targets.cbegin(); }
     StateSet::const_iterator cend() const { return targets.cend(); }
 
     size_t count(State s) const { return targets.count(s); }
     bool empty() const { return targets.empty(); }
     size_t size() const { return targets.size(); }
 
-    void insert(State s)
-    {
-        if (targets.find(s) == targets.end()) {
-            targets.insert(s);
-        }
-    }
-
-    void insert(StateSet states)
-    {
-        for (State s : states) {
-            insert(s);
-        }
-    }
+    void insert(State s);
+    void insert(StateSet states);
 
     // THIS BREAKS THE SORTEDNESS INVARIANT,
     // dangerous,
     // but useful for adding states in a random order to sort later (supposedly more efficient than inserting in a random order)
-    void inline push_back(const State s)
-    {
-        targets.push_back(s);
-    }
+    void inline push_back(const State s) { targets.push_back(s); }
 
     void remove(State s) { targets.remove(s); }
 
     const std::vector<State>::iterator find(State s) const { targets.find(s); }
-
     std::vector<State>::iterator find(State s) { return targets.find(s); }
 };
 
 /**
  * Post is a data structure representing possible transitions over different symbols.
  * It is an ordered vector containing possible Moves (i.e., pair of symbol and target states.
  * Vector is ordered by symbols which are numbers.
@@ -231,28 +207,28 @@
     using super::ToVector;
     using super::erase;
     // dangerous, breaks the sortedness invariant
     using super::push_back;
     // is adding non-const version as well ok?
     using super::back;
     using super::filter;
-};
+}; // struct Post.
 
 /**
  * Delta is a data structure for representing transition relation.
  * Its underlying data structure is vector of Post structures.
  * Each index of vector corresponds to one state, that is a number of
  * state is an index to the vector of Posts.
  */
 struct Delta {
 private:
     std::vector<Post> posts;
 
 public:
-    inline static const Post empty_post; //when posts[q] is not allocated, then delta[q] returns this.
+    inline static const Post empty_post; // When posts[q] is not allocated, then delta[q] returns this.
 
     Delta() : posts() {}
     explicit Delta(size_t n) : posts(n) {}
 
     void reserve(size_t n) {
         posts.reserve(n);
     };
@@ -268,81 +244,22 @@
     //
     // Namely, it allocates the post of the state if it was not allocated yet. This in turn may cause that
     // the entire post data structure is re-allocated, iterators to it get invalidated ...
     // Use the constant [] operator below if possible.
     // Or, to prevent the side effect form happening, one might want to make sure that posts of all states in the automaton
     // are allocated, e.g., write an NFA method that allocate delta for all states of the NFA.
     // But it feels fragile, before doing something like that, better think and talk to people.
-    Post& get_mutable_post(State q) {
-        if (q >= posts.size()) {
-            Util::reserve_on_insert(posts, q);
-            const size_t new_size{ q + 1 };
-            posts.resize(new_size);
-        }
-
-        return posts[q];
-    };
+    Post& get_mutable_post(State q);
 
     // TODO: why do we have the code of all these methods in the header file? Should we move it out?
     // TODO: Explain what is returned from this method.
-    std::vector<State> defragment(Util::NumberPredicate<State> & is_staying) {
-        //first, indexes of post are filtered (places of to be removed states are taken by states on their right)
-        size_t move_index{ 0 };
-        posts.erase(
-            std::remove_if(posts.begin(), posts.end(), [&](Post& _post) -> bool {
-                size_t prev{ move_index };
-                ++move_index;
-                return !is_staying[prev];
-            }),
-            posts.end()
-        );
-
-        //get renaming of current states to new numbers:
-        std::vector<State> renaming(this->find_max_state()+1);
-        size_t i = 0;
-        for (State q:is_staying.get_elements()) {
-            if (q >= renaming.size())
-                break;
-            renaming[q] = i;
-            i++;
-        }
-
-        //this iterates through every post and ever, filters and renames states,
-        //and finally removes moves that became empty from the post.
-        for (State q=0,size=posts.size(); q < size; ++q) {
-            //should we have a function Post::transform(Lambda) for this?
-            Post & p = get_mutable_post(q);
-            for (auto move = p.begin(); move < p.end(); ++move) {
-                move->targets.erase(
-                    std::remove_if(move->targets.begin(), move->targets.end(), [&](State q) -> bool {
-                        return !is_staying[q];
-                    }),
-                    move->targets.end()
-                );
-                move->targets.rename(renaming);
-            }
-            p.erase(
-                std::remove_if(p.begin(), p.end(), [&](Move& move) -> bool {
-                    return move.targets.empty();
-                }),
-                p.end()
-            );
-        }
-
-        //the renaming can be useful somewhere, computed anyway, we can as well return it.
-        return renaming;
-    };
+    std::vector<State> defragment(Util::NumberPredicate<State> & is_staying);
 
     // Get a constant reference to the post of a state. No side effects.
-    const Post & operator[] (State q) const {
-        if (q >= posts.size())
-            return empty_post;
-        else
-            return posts[q];
-    };
+    const Post & operator[] (State q) const;
 
     void emplace_back() { posts.emplace_back(); }
 
     void clear() { posts.clear(); }
 
     void increase_size(size_t n) {
         assert(n >= posts.size());
@@ -383,70 +300,44 @@
 
         const_iterator(const std::vector<Post>& post_p, size_t as,
                        Post::const_iterator pi, StateSet::const_iterator ti, bool ise = false) :
                 post(post_p), current_state(as), post_iterator(pi), targets_position(ti), is_end(ise) {};
 
         const_iterator(const const_iterator& other) = default;
 
-        Trans operator*() const
-        {
-            return Trans{current_state, (*post_iterator).symbol, *targets_position};
-        }
+        Trans operator*() const { return Trans{current_state, (*post_iterator).symbol, *targets_position}; }
 
         // Prefix increment
         const_iterator& operator++();
-
         // Postfix increment
-        const const_iterator operator++(int)
-        {
-            const const_iterator tmp = *this;
-            ++(*this);
-            return tmp;
-        }
-
-        const_iterator& operator=(const const_iterator& x)
-        {
-            this->post_iterator = x.post_iterator;
-            this->targets_position = x.targets_position;
-            this->current_state = x.current_state;
-            this->is_end = x.is_end;
-
-            return *this;
-        }
-
-        friend bool operator==(const const_iterator& a, const const_iterator& b)
-        {
-            if (a.is_end && b.is_end)
-                return true;
-            else if ((a.is_end && !b.is_end) || (!a.is_end && b.is_end))
-                return false;
-            else
-                return a.current_state == b.current_state && a.post_iterator == b.post_iterator
-                       && a.targets_position == b.targets_position;
-        }
+        const const_iterator operator++(int);
+
+        const_iterator& operator=(const const_iterator& x);
 
-        friend bool operator!= (const const_iterator& a, const const_iterator& b) { return !(a == b); };
+        friend bool operator==(const const_iterator& a, const const_iterator& b);
+        friend bool operator!=(const const_iterator& a, const const_iterator& b) { return !(a == b); };
     };
 
-    struct const_iterator cbegin() const { return const_iterator(posts); }
-    struct const_iterator cend() const { return const_iterator(posts, true); }
-    struct const_iterator begin() const { return cbegin(); }
-    struct const_iterator end() const { return cend(); }
+    const_iterator cbegin() const { return const_iterator(posts); }
+    const_iterator cend() const { return const_iterator(posts, true); }
+    const_iterator begin() const { return cbegin(); }
+    const_iterator end() const { return cend(); }
 
 private:
     State find_max_state();
-};
+}; // struct Delta.
 
 /// An epsilon symbol which is now defined as the maximal value of data type used for symbols.
-constexpr Symbol EPSILON = limits.maxSymbol;
+constexpr Symbol EPSILON = Limits::maxSymbol;
 
 /**
  * A struct representing an NFA.
  */
 struct Nfa {
+public:
     /**
      * @brief For state q, delta[q] keeps the list of transitions ordered by symbols.
      *
      * The set of states of this automaton are the numbers from 0 to the number of states minus one.
      */
     Delta delta;
     Util::NumberPredicate<State> initial{};
@@ -458,91 +349,63 @@
     ///  respective names, or "transition_dict" for transition dictionary adding a human-readable meaning to each
     ///  transition.
     // TODO: When there is a need for state dictionary, consider creating default library implementation of state
     //  dictionary in the attributes.
     std::unordered_map<std::string, void*> attributes{};
 
 public:
-    Nfa() : delta(), initial(), final() {}
-
+    explicit Nfa(Delta delta = {}, Util::NumberPredicate<State> initial_states = {},
+                 Util::NumberPredicate<State> final_states = {}, Alphabet* alphabet = nullptr)
+        : delta(std::move(delta)), initial(std::move(initial_states)), final(std::move(final_states)), alphabet(alphabet) {}
+        
     /**
      * @brief Construct a new explicit NFA with num_of_states states and optionally set initial and final states.
      *
      * @param[in] num_of_states Number of states for which to preallocate Delta.
      */
-    explicit Nfa(const unsigned long num_of_states, const StateSet& initial_states = StateSet{},
-                 const StateSet& final_states = StateSet{}, Alphabet* alphabet = nullptr)
-        : delta(num_of_states), initial(initial_states), final(final_states), alphabet(alphabet) {}
+    explicit Nfa(const unsigned long num_of_states, StateSet initial_states = {},
+                 StateSet final_states = {}, Alphabet* alphabet = nullptr)
+        : delta(num_of_states), initial(std::move(initial_states)), final(std::move(final_states)), alphabet(alphabet) {}
 
     /**
      * @brief Construct a new explicit NFA from other NFA.
      */
     Nfa(const Mata::Nfa::Nfa& other) = default;
 
     Nfa(Mata::Nfa::Nfa&& other) noexcept
         : delta{ std::move(other.delta) }, initial{ std::move(other.initial) }, final{ std::move(other.final) },
-          alphabet{ other.alphabet }, attributes{ std::move(other.attributes) } {
-        other.alphabet = nullptr;
-    }
+          alphabet{ other.alphabet }, attributes{ std::move(other.attributes) } { other.alphabet = nullptr; }
 
     Nfa& operator=(const Mata::Nfa::Nfa& other) = default;
-    Nfa& operator=(Mata::Nfa::Nfa&& other) noexcept {
-        if (this != &other) {
-            delta = std::move(other.delta);
-            initial = std::move(other.initial);
-            final = std::move(other.final);
-            alphabet = other.alphabet;
-            attributes = std::move(other.attributes);
-            other.alphabet = nullptr;
-        }
-        return *this;
-    }
+    Nfa& operator=(Mata::Nfa::Nfa&& other) noexcept;
 
     /**
      * Clear transitions but keep the automata states.
      */
-    void clear_transitions() {
-        const size_t delta_size = delta.num_of_states();
-        for (size_t i = 0; i < delta_size; ++i) {
-            delta.get_mutable_post(i) = Post();
-        }
-    }
+    void clear_transitions();
 
     /**
      * Add a new (fresh) state to the automaton.
      * @return The newly created state.
      */
-    State add_state() {
-        const size_t num_of_states{ size() };
-        delta.increase_size(num_of_states + 1 );
-        return num_of_states;
-    }
+    State add_state();
 
     /**
      * Add state @p state to @c delta if @p state is not in @c delta yet.
      * @return The requested @p state.
      */
-    State add_state(State state) {
-        if (state >= delta.num_of_states()) {
-            delta.increase_size(state + 1);
-        }
-        return state;
-    }
+    State add_state(State state);
 
     /**
      * @brief Get the current number of states in the whole automaton.
      *
      * This includes the initial and final states as well as states in the transition relation.
      * @return The number of states.
      */
-     size_t size() const {
-        return std::max({ static_cast<unsigned long>(initial.domain_size()),
-                          static_cast<unsigned long>(final.domain_size()),
-                          static_cast<unsigned long>(delta.num_of_states()) });
-    }
+     size_t size() const;
 
     /**
      * Unify initial states into a single new initial state.
      */
     void unify_initial();
 
     /**
@@ -553,91 +416,33 @@
     bool is_state(const State &state_to_check) const { return state_to_check < size(); }
 
     /**
      * @brief Clear the underlying NFA to a blank NFA.
      *
      * The whole NFA is cleared, each member is set to its zero value.
      */
-    void clear() {
-        delta.clear();
-        initial.clear();
-        final.clear();
-    }
+    void clear();
 
     /**
      * @brief Check if @c this is exactly identical to @p aut.
      *
      * This is exact equality of automata, including state numbering (so even stronger than isomorphism),
      *  essentially only useful for testing purposes.
      * @return True if automata are exactly identical, false otherwise.
      */
-    bool is_identical(const Nfa & aut) {
-        if (Util::OrdVector<State>(initial.get_elements()) != Util::OrdVector<State>(aut.initial.get_elements())) {
-            return false;
-        }
-        if (Util::OrdVector<State>(final.get_elements()) != Util::OrdVector<State>(aut.final.get_elements())) {
-            return false;
-        }
-
-        std::vector<Trans> this_trans;
-        for (auto trans: *this) { this_trans.push_back(trans); }
-        std::vector<Trans> aut_trans;
-        for (auto trans: aut) { aut_trans.push_back(trans); }
-        return this_trans == aut_trans;
-    };
+    bool is_identical(const Nfa & aut);
 
     /**
      * @brief Get the set of symbols used on the transitions in the automaton.
      *
      * Does not necessarily have to equal the set of symbols in the alphabet used by the automaton.
      * @return Set of symbols used on the transitions.
      * TODO: this should be a method of Delta?
      */
-    Util::OrdVector<Symbol> get_used_symbols() const {
-        //TODO: look at the variants in profiling (there are tests in tests-nfa-profiling.cc),
-        // for instance figure out why NumberPredicate and OrdVedctor are slow,
-        // try also with _STATIC_DATA_STRUCTURES_, it changes things.
-
-        //below are different variant, with different data structures for accumulating symbols,
-        //that then must be converted to an OrdVector
-        //measured are times with "Mata::Nfa::get_used_symbols speed, harder", "[.profiling]" now on line 104 of nfa-profiling.cc
-
-        //WITH VECTOR (4.434 s)
-        //return get_used_symbols_vec();
-
-        //WITH SET (26.5 s)
-        //auto from_set = get_used_symbols_set();
-        //return Util::OrdVector<Symbol> (from_set .begin(),from_set.end());
-
-        //WITH NUMBER PREDICATE (4.857s)
-        //return Util::OrdVector(get_used_symbols_np().get_elements());
-
-        //WITH BOOL VECTOR (error !!!!!!!):
-        //return Util::OrdVector<Symbol>(Util::NumberPredicate<Symbol>(get_used_symbols_bv()));
-
-        //WITH BOOL VECTOR (1.9s):
-        std::vector<bool> bv = get_used_symbols_bv();
-        Util::OrdVector<Symbol> ov;
-        //int count = 0;
-        //for(Symbol i = 0;i<bv.size();i++)
-        //    if (bv[i]) {
-        //        count++;
-        //    }
-        //ov.reserve(count);
-        for(Symbol i = 0;i<bv.size();i++)
-            if (bv[i]) {
-                ov.push_back(i);
-            }
-        return ov;
-
-        ///WITH BOOL VECTOR, DIFFERENT VARIANT? (1.9s):
-        //std::vector<bool> bv = get_used_symbols_bv();
-        //std::vector<Symbol> v(std::count(bv.begin(), bv.end(), true));
-        //return Util::OrdVector<Symbol>(v);
-    };
+    Util::OrdVector<Symbol> get_used_symbols() const;
 
     Mata::Util::OrdVector<Symbol> get_used_symbols_vec() const;
     std::set<Symbol> get_used_symbols_set() const;
     Mata::Util::NumberPredicate<Symbol> get_used_symbols_np() const;
     std::vector<bool> get_used_symbols_bv() const;
 
     /**
@@ -668,15 +473,14 @@
      *
      * Useful states are reachable and terminating states.
      * @return Set of useful states.
      * TODO: with the new get_useful_states, we can delete this probably.
      */
     StateSet get_useful_states_old() const;
 
-
     //I just want to return something as constant reference to the thing, without copying anything, how?
     const Util::NumberPredicate<State> get_useful_states() const;
 
     /**
      * @brief Remove inaccessible (unreachable) and not co-accessible (non-terminating) states.
      *
      * Remove states which are not accessible (unreachable; state is accessible when the state is the endpoint of a path
@@ -684,17 +488,15 @@
      * the starting point of a path ending in a final state).
      *
      * @param[out] state_map Mapping of trimmed states to new states.
      * TODO: we can probably keep just trim_reverting, much faster. But the speed difference and how it is achieved is interesting. Keeping as a demonstration for now.
      */
     void trim_inplace(StateToStateMap* state_map = nullptr);
     void trim_reverting(StateToStateMap* state_map = nullptr);
-    void trim(StateToStateMap* state_map = nullptr) {
-        trim_reverting(state_map);
-    }
+    void trim(StateToStateMap* state_map = nullptr) { trim_reverting(state_map); }
 
     /**
      * @brief Remove inaccessible (unreachable) and not co-accessible (non-terminating) states.
      *
      * Remove states which are not accessible (unreachable; state is accessible when the state is the endpoint of a path
      * starting from an initial state) or not co-accessible (non-terminating; state is co-accessible when the state is
      * the starting point of a path ending in a final state).
@@ -728,16 +530,15 @@
      * Get transitions leading from @p state_from.
      *
      * If we try to access a state which is present in the delta as a target state, yet does not have allocated space
      *  for itself in @c post, @c post is resized to include @p state_from.
      * @param state_from[in] Source state for transitions to get.
      * @return List of transitions leading from @p state_from.
      */
-    const Post& get_moves_from(const State state_from) const
-    {
+    const Post& get_moves_from(const State state_from) const {
         assert(state_from < size());
         return delta[state_from];
     }
 
     /**
      * Get transitions leading to @p state_to.
      * @param state_to[in] Target state for transitions to get.
@@ -774,42 +575,34 @@
     void get_one_letter_aut(Nfa& result) const;
 
     void print_to_DOT(std::ostream &outputStream) const;
 
     // TODO: Relict from VATA. What to do with inclusion/ universality/ this post function? Revise all of them.
     StateSet post(const StateSet& states, const Symbol& symbol) const;
 
-    struct const_iterator
-    { // {{{
+    struct const_iterator {
         const Nfa* nfa;
         size_t trIt;
         Post::const_iterator tlIt;
         StateSet::const_iterator ssIt;
         Trans trans;
         bool is_end = { false };
 
         const_iterator() : nfa(), trIt(0), tlIt(), ssIt(), trans() { };
         static const_iterator for_begin(const Nfa* nfa);
         static const_iterator for_end(const Nfa* nfa);
 
-        //he, what is this? Some comment would help.
-        // I am thinking about that removing everything having to do with Transition might be a good thing. Transition adds clutter and makes people write inefficient code.
-        void refresh_trans()
-        { // {{{
-            this->trans = {trIt, this->tlIt->symbol, *(this->ssIt)};
-        } // }}}
+        // FIXME: He, what is this? Some comment would help.
+        // I am thinking about that removing everything having to do with Transition might be a good thing. Transition
+        //  adds clutter and makes people write inefficient code.
+        void refresh_trans() { this->trans = {trIt, this->tlIt->symbol, *(this->ssIt)}; }
 
         const Trans& operator*() const { return this->trans; }
 
-        bool operator==(const const_iterator& rhs) const
-        { // {{{
-            if (this->is_end && rhs.is_end) { return true; }
-            if ((this->is_end && !rhs.is_end) || (!this->is_end && rhs.is_end)) { return false; }
-            return ssIt == rhs.ssIt && tlIt == rhs.tlIt && trIt == rhs.trIt;
-        } // }}}
+        bool operator==(const const_iterator& rhs) const;
         bool operator!=(const const_iterator& rhs) const { return !(*this == rhs);}
         const_iterator& operator++();
     }; // }}}
 
     const_iterator begin() const { return const_iterator::for_begin(this); }
     const_iterator end() const { return const_iterator::for_end(this); }
 
@@ -998,33 +791,28 @@
  * on transitions from given state) to new sink state (if no new transitions are added, this sink state is not created).
  * In the case that @p aut does not contain any states, this function does nothing.
  *
  * @param[in] aut Automaton to make complete.
  * @param[in] alphabet Alphabet to use for computing "missing" symbols.
  * @return True if some new transition (and sink state) was added to the automaton.
  */
-inline bool make_complete(
-        Nfa&             aut,
-        const Alphabet&  alphabet)
-{
-    return make_complete(aut, alphabet, aut.size());
-}
+inline bool make_complete(Nfa& aut, const Alphabet& alphabet) { return make_complete(aut, alphabet, aut.size()); }
 
 /**
  * @brief Compute automaton accepting complement of @p aut.
  *
  * @param[in] aut Automaton whose complement to compute.
  * @param[in] alphabet Alphabet used for complementation.
  * @param[in] params Optional parameters to control the complementation algorithm:
  * - "algorithm": "classical" (classical algorithm determinizes the automaton, makes it complete and swaps final and non-final states);
  * - "minimize": "true"/"false" (whether to compute minimal deterministic automaton for classical algorithm);
  * @return Complemented automaton.
  */
 Nfa complement(const Nfa& aut, const Alphabet& alphabet,
-    const StringMap& params = {{"algorithm", "classical"}, {"minimize", "false"}});
+   const StringMap& params = {{"algorithm", "classical"}, {"minimize", "false"}});
 
 /**
  * @brief Compute automaton accepting complement of @p aut.
  *
  * This overloaded version complements over an already created ordered set of @p symbols instead of an alphabet.
  * This is a more efficient solution in case you already have @p symbols precomputed or want to complement multiple
  *  automata over the same set of @c symbols: the function does not need to compute the ordered set of symbols from
@@ -1044,59 +832,51 @@
  * @brief Compute minimal deterministic automaton.
  *
  * @param[in] aut Automaton whose minimal version to compute.
  * @param[in] params Optional parameters to control the minimization algorithm:
  * - "algorithm": "brzozowski"
  * @return Minimal deterministic automaton.
  */
-Nfa minimize(
-        const Nfa &aut,
-        const StringMap& params = {{"algorithm", "brzozowski"}});
+Nfa minimize(const Nfa &aut, const StringMap& params = {{"algorithm", "brzozowski"}});
 
 /**
  * @brief Determinize automaton.
  *
  * @param[in] aut Automaton to determinize.
  * @param[out] subset_map Map that maps sets of states of input automaton to states of determinized automaton.
  * @return Determinized automaton.
  */
-Nfa determinize(
-        const Nfa&  aut,
-        std::unordered_map<StateSet, State> *subset_map = nullptr);
+Nfa determinize(const Nfa&  aut, std::unordered_map<StateSet, State> *subset_map = nullptr);
 
 /**
  * Reduce the size of the automaton.
  *
  * @param[in] aut Automaton to reduce.
  * @param[in] trim_input Whether to trim the input automaton first or not.
  * @param[out] state_map Mapping of trimmed states to new states.
  * @param[in] params Optional parameters to control the reduction algorithm:
  * - "algorithm": "simulation".
  * @return Reduced automaton.
  */
-Nfa reduce(
-        const Nfa &aut,
-        bool trim_input = true,
-        StateToStateMap *state_map = nullptr,
-        const StringMap&  params = {{"algorithm", "simulation"}});
+Nfa reduce(const Nfa &aut, bool trim_input = true, StateToStateMap *state_map = nullptr,
+    const StringMap&  params = {{"algorithm", "simulation"}});
 
 /// Is the language of the automaton universal?
 bool is_universal(
         const Nfa&         aut,
         const Alphabet&    alphabet,
         Run*              cex = nullptr,
         const StringMap&  params = {{"algorithm", "antichains"}});
 
 inline bool is_universal(
         const Nfa&         aut,
         const Alphabet&    alphabet,
-        const StringMap&  params)
-{ // {{{
+        const StringMap&  params) {
     return is_universal(aut, alphabet, nullptr, params);
-} // }}}
+}
 
 /**
  * @brief Checks inclusion of languages of two NFAs: @p smaller and @p bigger (smaller <= bigger).
  *
  * @param[in] smaller First automaton to concatenate.
  * @param[in] bigger Second automaton to concatenate.
  * @param[out] cex Counterexample for the inclusion.
@@ -1122,18 +902,17 @@
  * - "algorithm": "naive", "antichains" (Default: "antichains")
  * @return True if @p smaller is included in @p bigger, false otherwise.
  */
 inline bool is_included(
         const Nfa&             smaller,
         const Nfa&             bigger,
         const Alphabet* const  alphabet = nullptr,
-        const StringMap&      params = {{"algorithm", "antichains"}})
-{ // {{{
+        const StringMap&      params = {{"algorithm", "antichains"}}) {
     return is_included(smaller, bigger, nullptr, alphabet, params);
-} // }}}
+}
 
 /**
  * @brief Perform equivalence check of two NFAs: @p lhs and @p rhs.
  *
  * @param[in] lhs First automaton to concatenate.
  * @param[in] rhs Second automaton to concatenate.
  * @param[in] alphabet Alphabet of both NFAs to compute with.
@@ -1205,22 +984,15 @@
 
 /** Encodes a vector of strings (each corresponding to one symbol) into a
  *  @c Word instance
  */
  // TODO: rename to something, but no idea to what.
  // Maybe we need some terminology - Symbols and Words are made of numbers.
  // What are the symbol names and their sequences?
-inline Run encode_word(
-	const StringToSymbolMap&         symbol_map,
-	const std::vector<std::string>&  input)
-{ // {{{
-	Run result;
-	for (const auto& str : input) { result.word.push_back(symbol_map.at(str)); }
-	return result;
-} // encode_word }}}
+Run encode_word(const StringToSymbolMap& symbol_map, const std::vector<std::string>& input);
 
 /** Loads an automaton from Parsed object */
 Nfa construct(
         const Mata::Parser::ParsedSection&   parsec,
         Alphabet*                            alphabet,
         StringToStateMap*                    state_map = nullptr);
 
@@ -1230,45 +1002,40 @@
         Alphabet*                            alphabet,
         StringToStateMap*                    state_map = nullptr);
 
 template <class ParsedObject>
 Nfa construct(
         const ParsedObject&                  parsed,
         StringToSymbolMap*                   symbol_map = nullptr,
-        StringToStateMap*                    state_map = nullptr)
-{ // {{{
+        StringToStateMap*                    state_map = nullptr) {
     StringToSymbolMap tmp_symbol_map;
     if (symbol_map) {
         tmp_symbol_map = *symbol_map;
     }
     Mata::OnTheFlyAlphabet alphabet(tmp_symbol_map);
 
     Nfa aut = construct(parsed, &alphabet, state_map);
 
     if (symbol_map) {
         *symbol_map = alphabet.get_symbol_map();
     }
     return aut;
-}
+} // construct().
 
 } // namespace Mata::Nfa.
 
-namespace std
-{ // {{{
+namespace std {
 template <>
-struct hash<Mata::Nfa::Trans>
-{
-	inline size_t operator()(const Mata::Nfa::Trans& trans) const
-	{
+struct hash<Mata::Nfa::Trans> {
+	inline size_t operator()(const Mata::Nfa::Trans& trans) const {
 		size_t accum = std::hash<Mata::Nfa::State>{}(trans.src);
 		accum = Mata::Util::hash_combine(accum, trans.symb);
 		accum = Mata::Util::hash_combine(accum, trans.tgt);
 		return accum;
 	}
 };
 
 std::ostream& operator<<(std::ostream& os, const Mata::Nfa::Trans& trans);
 std::ostream& operator<<(std::ostream& os, const Mata::Nfa::Nfa& nfa);
-} // std }}}
-
+} // namespace std.
 
-#endif /* _MATA_NFA_HH_ */
+#endif /* MATA_NFA_HH_ */
```

### Comparing `libmata-0.66.0/mata/include/mata/number-predicate.hh` & `libmata-0.67.0/mata/include/mata/number-predicate.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/include/mata/ord-vector.hh` & `libmata-0.67.0/mata/include/mata/ord-vector.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-/*****************************************************************************
- *  Mata Tree Automata Library
+/* ord-vector.hh -- Implementation of a set (ordered vector) using std::vector.
  *
- *  Copyright (c) 2011  Ondra Lengal <ilengal@fit.vutbr.cz>
+ * This file is a part of libmata.
  *
- *  Description:
- *    File with the OrdVector class.
+ * This program is free software; you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation; either version 3 of the License, or
+ * (at your option) any later version.
  *
- *****************************************************************************/
+ * This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ * GNU General Public License for more details.
+ */
 
 #ifndef MATA_ORD_VECTOR_HH_
 #define MATA_ORD_VECTOR_HH_
 
 #include <vector>
 #include <algorithm>
 #include <cassert>
 
-#include <mata/number-predicate.hh>
-#include <mata/util.hh>
+#include "mata/number-predicate.hh"
+#include "mata/util.hh"
 
 namespace {
 /**
  * @brief  Converts an object to string
  *
  * Static method for conversion of an object of any class with the << output
  * operator into a string
  *
  * @param[in]  n  The object for the conversion
  *
  * @returns  The string representation of the object
  */
 template <typename T>
-static std::string ToString(const T& n)
-{
+std::string ToString(const T& n) {
     // the output stream for the string
     std::ostringstream oss;
     // insert the object into the stream
     oss << n;
     // return the string
     return oss.str();
 }
@@ -52,37 +56,33 @@
     for (auto q: lhs)
         if (rhs[q])
             return false;
     return true;
 }
 
 template <class T>
-bool are_disjoint(const Util::OrdVector<T>& lhs, const Util::OrdVector<T>& rhs)
-{
+bool are_disjoint(const Util::OrdVector<T>& lhs, const Util::OrdVector<T>& rhs) {
     auto itLhs = lhs.begin();
     auto itRhs = rhs.begin();
-    while (itLhs != lhs.end() && itRhs != rhs.end())
-    {
+    while (itLhs != lhs.end() && itRhs != rhs.end()) {
         if (*itLhs == *itRhs) { return false; }
         else if (*itLhs < *itRhs) { ++itLhs; }
         else {++itRhs; }
     }
-
     return true;
 }
 
-template <class Key> bool is_sorted(std::vector<Key> vec) {
-    for (auto itVec = vec.cbegin() + 1; itVec < vec.cend(); ++itVec)
-    {	// check that the vector is sorted
-        if (!(*(itVec - 1) < *itVec))
-        {	// in case there is an unordered pair (or there is one element twice)
+template <class Key>
+bool is_sorted(const std::vector<Key>& vec) {
+    for (auto itVec = vec.cbegin() + 1; itVec < vec.cend(); ++itVec) {
+        if (!(*(itVec - 1) < *itVec)) {
+            // In case there is an unordered pair (or there is one element twice).
             return false;
         }
     }
-
     return true;
 }
 
 /**
  * @brief  Implementation of a set using ordered vector
  *
  * This class implements the interface of a set (the same interface as
@@ -105,97 +105,69 @@
     VectorType vec_;
 
 private:  // Private methods
     bool vectorIsSorted() const { return(Mata::Util::is_sorted(vec_)); }
 
 public:
     OrdVector() : vec_() {}
-
-    explicit OrdVector(const VectorType& vec) :
-        vec_(vec)
-    {
-        Util::sort_and_rmdupl(vec_);
-    }
-
+    explicit OrdVector(const VectorType& vec) : vec_(vec) { Util::sort_and_rmdupl(vec_); }
     explicit OrdVector(const std::set<Key>& set): vec_{ set.begin(), set.end() } { Util::sort_and_rmdupl(vec_); }
-
-    OrdVector(std::initializer_list<Key> list) :
-        vec_(list)
-    {
-        Util::sort_and_rmdupl(vec_);
-    }
-
+    OrdVector(std::initializer_list<Key> list) : vec_(list) { Util::sort_and_rmdupl(vec_); }
     OrdVector(const OrdVector& rhs) = default;
     OrdVector(OrdVector&& other) noexcept : vec_{ std::move(other.vec_) } {}
+    explicit OrdVector(const Key& key) : vec_(1, key) { assert(vectorIsSorted()); }
+    explicit OrdVector(const NumberPredicate<Key>& p) : OrdVector(p.get_elements()) {};
+    template <class InputIterator>
+    OrdVector(InputIterator first, InputIterator last) : vec_(first, last) { Util::sort_and_rmdupl(vec_); }
 
     OrdVector& operator=(const OrdVector& other) {
         if (&other != this) { vec_ = other.vec_; }
         return *this;
     }
 
     OrdVector& operator=(OrdVector&& other) noexcept {
         if (&other != this) { vec_ = std::move(other.vec_); }
         return *this;
     }
 
-    explicit OrdVector(const Key& key) : vec_(1, key) {
-        // Assertions
-        assert(vectorIsSorted());
-    }
-
-    OrdVector(const NumberPredicate<Key>& p) : OrdVector(p.get_elements()) {};
-
-    template <class InputIterator>
-    OrdVector(InputIterator first, InputIterator last) :
-        vec_(first, last)
-    {
-        Util::sort_and_rmdupl(vec_);
-    }
-
     virtual ~OrdVector() = default;
 
     /**
      * Create OrdVector with reserved @p capacity.
      * @param[in] capacity Capacity of OrdVector to reserve.
      * @return Newly create OrdVector.
      */
     static OrdVector with_reserved(const size_t capacity) {
         OrdVector ord_vector{};
         ord_vector.vec_.reserve(capacity);
         return ord_vector;
     }
 
-    void insert(iterator itr, const Key& x)
-    {
+    void insert(iterator itr, const Key& x) {
         assert(itr == this->end() || x <= *itr);
         vec_.insert(itr,x);
     }
 
     // PUSH_BACK WHICH BREAKS SORTEDNESS,
     // dangerous,
     // but useful in NFA where temporarily breaking the sortedness invariant allows for a faster algorithm (e.g. revert)
     virtual inline void push_back(const Key& x) {
         reserve_on_insert(vec_);
         vec_.emplace_back(x);
     }
 
-    virtual inline void reserve(size_t  size) {
-        vec_.reserve(size);
-    }
+    virtual inline void reserve(size_t  size) { vec_.reserve(size); }
 
-    virtual inline void erase(const_iterator first, const_iterator last) {
-        vec_.erase(first, last);
-    }
+    virtual inline void erase(const_iterator first, const_iterator last) { vec_.erase(first, last); }
 
-    virtual void insert(const Key& x)
-    {
-        reserve_on_insert(vec_);
-        // Assertions
+    virtual void insert(const Key& x) {
         assert(vectorIsSorted());
 
+        reserve_on_insert(vec_);
+
         // perform binary search (cannot use std::binary_search because it is
         // ineffective due to not returning the iterator to the position of the
         // desirable insertion in case the searched element is not present in the
         // range)
         size_t first = 0;
         size_t last = vec_.size();
 
@@ -225,48 +197,36 @@
 
         vec_.resize(vec_.size() + 1);
         std::copy_backward(vec_.begin() + first, vec_.end() - 1, vec_.end());
 
         // insert the new element
         vec_[first] = x;
 
-        // Assertions
         assert(vectorIsSorted());
     }
 
-    virtual void insert(const OrdVector& vec)
-    {
-        // Assertions
+    virtual void insert(const OrdVector& vec) {
         assert(vectorIsSorted());
         assert(vec.vectorIsSorted());
-
         vec_ = OrdVector::Union(*this, vec).vec_;
-
-        // Assertions
         assert(vectorIsSorted());
     }
 
     inline void clear() { vec_.clear(); }
 
     virtual inline size_t size() const { return vec_.size(); }
 
-
-    inline size_t count(const Key& key) const
-    {
-        // Assertions
+    inline size_t count(const Key& key) const {
         assert(vectorIsSorted());
-
-        for (auto v : this->vec_)
-        {
+        for (auto v : this->vec_) {
             if (v == key)
                 return 1;
             else if (v > key)
                 return 0;
         }
-
         return 0;
     }
 
     /**
      * Compute set difference as @c this minus @p rhs.
      * @param rhs Other vector with symbols to be excluded.
      * @return @c this minus @p rhs.
@@ -275,30 +235,26 @@
 
     OrdVector intersection(const OrdVector& rhs) const { return intersection(*this, rhs); }
 
     OrdVector Union(const OrdVector& rhs) const { return Union(*this, rhs); }
 
     //TODO: this code of find was duplicated, not nice.
     // Replacing the original code by std function, but keeping the original here commented, it was nice, might be even better.
-    virtual const_iterator find(const Key& key) const
-    {
-        // Assertions
+    virtual const_iterator find(const Key& key) const {
         assert(vectorIsSorted());
 
         auto it = std::lower_bound(vec_.begin(), vec_.end(),key);
         if (it == vec_.end() || *it != key)
             return vec_.end();
         else
             return it;
     }
 
     //TODO: the original code was duplicated, see comments above.
-    virtual iterator find(const Key& key)
-    {
-        // Assertions
+    virtual iterator find(const Key& key) {
         assert(vectorIsSorted());
 
         auto it = std::lower_bound(vec_.begin(), vec_.end(),key);
         if (it == vec_.end() || *it != key)
             return vec_.end();
         else
             return it;
@@ -365,65 +321,44 @@
 	 * @see  to_string()
 	 *
 	 * @param[in]  os    The output stream
 	 * @param[in]  vec   Assignment to the variables
 	 *
 	 * @returns  Modified output stream
 	 */
-	friend std::ostream& operator<<(std::ostream& os, const OrdVector& vec)
-	{
+	friend std::ostream& operator<<(std::ostream& os, const OrdVector& vec) {
 		std::string result = "{";
 
-		for (auto it = vec.cbegin(); it != vec.cend(); ++it)
-		{
+		for (auto it = vec.cbegin(); it != vec.cend(); ++it) {
 			result += ((it != vec.begin())? ", " : " ") + ToString(*it);
 		}
 
 		return os << (result + "}");
 	}
 
-	bool operator==(const OrdVector& rhs) const
-	{
-		// Assertions
+	bool operator==(const OrdVector& rhs) const {
 		assert(vectorIsSorted());
 		assert(rhs.vectorIsSorted());
-
 		return (vec_ == rhs.vec_);
 	}
+    bool operator!=(const OrdVector& rhs) const { return !(*this == rhs); }
 
-    bool operator!=(const OrdVector& rhs) const
-    {
-        // Assertions
+    bool operator<(const OrdVector& rhs) const {
         assert(vectorIsSorted());
         assert(rhs.vectorIsSorted());
-
-        return (vec_ != rhs.vec_);
-    }
-
-    bool operator<(const OrdVector& rhs) const
-    {
-        // Assertions
-        assert(vectorIsSorted());
-        assert(rhs.vectorIsSorted());
-
-        return std::lexicographical_compare(vec_.begin(), vec_.end(),
-            rhs.vec_.begin(), rhs.vec_.end());
+        return std::lexicographical_compare(vec_.begin(), vec_.end(), rhs.vec_.begin(), rhs.vec_.end());
     }
 
     const std::vector<Key>& ToVector() const { return vec_; }
 
-    bool IsSubsetOf(const OrdVector& bigger) const
-    {
-        return std::includes(bigger.cbegin(), bigger.cend(),
-            this->cbegin(), this->cend());
+    bool IsSubsetOf(const OrdVector& bigger) const {
+        return std::includes(bigger.cbegin(), bigger.cend(), this->cbegin(), this->cend());
     }
 
-    bool HaveEmptyIntersection(const OrdVector& rhs) const
-    {
-        // Assertions
+    bool HaveEmptyIntersection(const OrdVector& rhs) const {
         assert(vectorIsSorted());
         assert(rhs.vectorIsSorted());
 
         const_iterator itLhs = begin();
         const_iterator itRhs = rhs.begin();
 
         while ((itLhs != end()) && (itRhs != rhs.end()))
@@ -438,21 +373,19 @@
             }
             else
             {	// in case the element in rhs is smaller
                 assert(*itLhs > *itRhs);
                 ++itRhs;
             }
         }
-
         return true;
     }
 
     // Renames numbers in the vector according to the renaming, q becomes renaming[q].
-   void rename(const std::vector<Key> & renaming) { Util::rename(vec_,renaming); }
-
+    void rename(const std::vector<Key> & renaming) { Util::rename(vec_,renaming); }
 
     static OrdVector difference(const OrdVector& lhs, const OrdVector& rhs) {
         assert(lhs.vectorIsSorted());
         assert(rhs.vectorIsSorted());
 
         OrdVector result{};
         auto lhs_it{ lhs.begin() };
@@ -538,17 +471,15 @@
     }
 }; // Class OrdVector.
 
 } // Namespace Mata::Util.
 
 namespace std {
     template <class Key>
-    struct hash<Mata::Util::OrdVector<Key>>
-    {
-        std::size_t operator()(const Mata::Util::OrdVector<Key>& vec) const
-        {
+    struct hash<Mata::Util::OrdVector<Key>> {
+        std::size_t operator()(const Mata::Util::OrdVector<Key>& vec) const {
             return std::hash<std::vector<Key>>{}(vec.ToVector());
         }
     };
 }
 
 #endif // MATA_ORD_VECTOR_HH_.
```

### Comparing `libmata-0.66.0/mata/include/mata/re2parser.hh` & `libmata-0.67.0/mata/include/mata/re2parser.hh`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-/* re2parser.hh -- parser transforming re2 regular expressions to our Nfa
- *
- * Copyright (c) 2022 Michal Horky
+/* re2parser.hh -- Parser transforming re2 regular expressions to their corresponding automata representations.
  *
  * This file is a part of libmata.
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 3 of the License, or
  * (at your option) any later version.
@@ -15,20 +13,21 @@
  * GNU General Public License for more details.
  */
 
 #ifndef MATA_RE2PARSER_HH
 #define MATA_RE2PARSER_HH
 
 #include <string>
-#include <mata/nfa.hh>
 
-namespace Mata {
+#include "mata/nfa.hh"
 
-    /**
-     * Parser from regular expression to automata (currently `Nfa` and `Afa` are supported).
-     */
-    namespace Parser {
-        void create_nfa(Nfa::Nfa* nfa, const std::string &pattern, bool use_epsilon = false, int epsilon_value = 306, bool use_reduction = true);
-    }
+/**
+ * @brief Parser from regular expression to automata.
+ *
+ * Currently supported automata types are NFA and AFA.
+ */
+namespace Mata::Parser {
+    void create_nfa(Nfa::Nfa* nfa, const std::string &pattern, bool use_epsilon = false, int epsilon_value = 306,
+                    bool use_reduction = true);
 }
 
 #endif // MATA_RE2PARSER_HH
```

### Comparing `libmata-0.66.0/mata/include/mata/synchronized-iterator.hh` & `libmata-0.67.0/mata/include/mata/synchronized-iterator.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,300 +1,300 @@
-//
-// Created by Lukáš Holík on 29.10.2022.
-//
-
-#ifndef LIBMATA_SYNCHRONIZED_ITERATOR_HH
-#define LIBMATA_SYNCHRONIZED_ITERATOR_HH
-
-#include <mata/ord-vector.hh>
-
-namespace Mata {
-    namespace Util {
-       /* Two classes that provide "synchronized" iterators through a vector of ordered vectors,
-        *  (or of some ordered OrdContainer that have a similar iterator),
-        *  needed in computation of post
-        *  in subset construction, product, and non-determinization.
-        *  The Type stored in OrdContainers must be comparable with <,>,==,!=,<=,>=,
-        *  and it must be a total (linear) ordering.
-        *  The intended usage in, for instance, determinisation is for Type to be TransSymbolStates.
-        *  TransSymbolStates is ordered by the symbol.
-        *
-        *  SyncrhonisedIterator is the parent virtual class.
-        *  It stores a vector of end-iterators for the OrdContainer v and a vector of current positions.
-        *  They are filled in using the function push_back(begin,end), that adds begin and end iterators of v to positions and ends, respectively
-        *  Method advance advances all positions forward so that they are synchronized on the next smallest equiv class
-        *  (next smallest symbol in the case of TransSymbolStates).
-        *
-        *  There are two versions of the class.
-        *  i) In product, ALL positions must point to currently the smallest equiv. class (Moves with the same symbol).
-        *  Method get_current then returns the vector of all position iterators, synchronized.
-        *  ii) In determinization, it is enough that there EXISTS a position that points to the smallest class.
-        *  Method get_current then returns the vector of only those positions that point to the smallest equiv. class.
-        *
-        *  Usage: 0) construct, 1) fill in using push_back, iterate using advance and get_current, 2) reset, goto 1)
-        *
-        *  The memory allocated internally for positions and ends is kept after reset, so it is advisable to use the same iterator for many iterations, as
-        *  opposed to creating a new one for each iteration.
-        */
-        template<typename Iterator> class SynchronizedIterator {
-        public:
-
-            std::vector<Iterator> positions;
-            std::vector<Iterator> ends;
-
-            //@param size Number of elements to reserve up-front for positions and ends.
-            explicit SynchronizedIterator(const int size = 0)
-            {
-                positions.reserve(size);
-                ends.reserve(size);
-            };
-
-           /* This is supposed to be called only before an iteration,
-            * after constructor of reset.
-            * Calling after advance breaks the iterator.
-            * Specifies begin and end of one vector, to initialise before the iteration starts.
-            */
-            virtual void push_back (const Iterator &begin, const Iterator &end) {
-                // Btw, I don't know what I am doing with the const & parameter passing,
-                // begin is actually incremented in advance ...? But tests do pass ...
-                this->positions.emplace_back(begin);
-                this->ends.emplace_back(end);
-            };
-
-
-           /* Empties positions and ends.
-            * Though they should keep the allocated space.
-            * @param size Number of elements to reserve up-front for positions and ends.
-            */
-            void reset(const int size = 0) {
-                positions.clear();
-                ends.clear();
-                if (size > 0) {
-                    positions.reserve(size);
-                    ends.reserve(size);
+/* parser.hh -- Classes for synchronized iteration.
+ *
+ * This file is a part of libmata.
+ *
+ * This program is free software; you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation; either version 3 of the License, or
+ * (at your option) any later version.
+ *
+ * This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ * GNU General Public License for more details.
+ */
+
+#ifndef MATA_SYNCHRONIZED_ITERATOR_HH
+#define MATA_SYNCHRONIZED_ITERATOR_HH
+
+#include "mata/ord-vector.hh"
+
+namespace Mata::Util {
+
+/**
+ * Two classes that provide "synchronized" iterators through a vector of ordered vectors,
+ * (or of some ordered OrdContainer that have a similar iterator),
+ * needed in computation of post
+ * in subset construction, product, and non-determinization.
+ *
+ * The Type stored in OrdContainers must be comparable with <,>,==,!=,<=,>=,
+ * and it must be a total (linear) ordering.
+ * The intended usage in, for instance, determinisation is for Type to be TransSymbolStates.
+ * TransSymbolStates is ordered by the symbol.
+ *
+ * SynchronisedIterator is the parent virtual class.
+ * It stores a vector of end-iterators for the OrdContainer v and a vector of current positions.
+ * They are filled in using the function push_back(begin,end), that adds begin and end iterators of v to positions and
+ *  ends, respectively
+ * Method advance advances all positions forward so that they are synchronized on the next smallest equiv class
+ * (next smallest symbol in the case of TransSymbolStates).
+ *
+ * There are two versions of the class.
+ * i) In product, ALL positions must point to currently the smallest equiv. class (Moves with the same symbol).
+ * Method get_current then returns the vector of all position iterators, synchronized.
+ * ii) In determinization, it is enough that there EXISTS a position that points to the smallest class.
+ * Method get_current then returns the vector of only those positions that point to the smallest equiv. class.
+ *
+ * Usage: 0) construct, 1) fill in using push_back, iterate using advance and get_current, 2) reset, goto 1)
+ *
+ * The memory allocated internally for positions and ends is kept after reset, so it is advisable to use the same iterator for many iterations, as
+ * opposed to creating a new one for each iteration.
+ */
+
+/// Class implementing synchronized iteration.
+template<typename Iterator> class SynchronizedIterator {
+public:
+
+    std::vector<Iterator> positions;
+    std::vector<Iterator> ends;
+
+    /// @param size Number of elements to reserve up-front for positions and ends.
+    explicit SynchronizedIterator(const int size = 0) {
+        positions.reserve(size);
+        ends.reserve(size);
+    };
+
+    /** This is supposed to be called only before an iteration,
+     * after constructor of reset.
+     * Calling after advance breaks the iterator.
+     * Specifies begin and end of one vector, to initialise before the iteration starts.
+     */
+    virtual void push_back (const Iterator &begin, const Iterator &end) {
+        // Btw, I don't know what I am doing with the const & parameter passing,
+        // begin is actually incremented in advance ...? But tests do pass ...
+        this->positions.emplace_back(begin);
+        this->ends.emplace_back(end);
+    };
+
+
+    /** Empties positions and ends.
+     * Though they should keep the allocated space.
+     * @param size Number of elements to reserve up-front for positions and ends.
+     */
+    void reset(const int size = 0) {
+        positions.clear();
+        ends.clear();
+        if (size > 0) {
+            positions.reserve(size);
+            ends.reserve(size);
+        }
+    };
+
+    virtual bool advance() = 0;
+    virtual const std::vector<Iterator> get_current() = 0;
+};
+
+
+
+template<typename Iterator>
+class SynchronizedUniversalIterator: public SynchronizedIterator<Iterator> {
+public:
+
+    /** "minimum" would be the smallest class bounded from below by all positions that appears in all OrdContainers.
+     * Are we sure that all positions at this class?
+     * Invariant: it can be true only if all positions are indeed synchronized.
+     */
+    bool synchronized_at_current_minimum = false;
+
+    /**
+     * Advances all positions to the NEXT minimum and returns true (though the next minimum might be the current state
+     *  if synchronized_at_current_minimum is false), or returns false if positions cannot be synchronized.
+     *
+     * If positions are synchronized to start with, then synchronized_at_current_minimum decides whether to stay or
+     *  advance further.
+     * The general of the algorithm is to synchronize everybody with position[0].
+     */
+    bool advance() {
+        //Nothing to synchronize.
+        if (this->positions.empty()) { return false;  } // TODO: ?? or not?
+
+        // If already synchronized, start moving forward by advancing position[0] (and so break synchronization).
+        if (this->synchronized_at_current_minimum) {
+            ++this->positions[0];
+            synchronized_at_current_minimum = false;
+        }
+
+        // If positions[0] has nowhere to go, then sync is not possible.
+        if (this->positions[0] == this->ends[0]) { return false; }
+
+        // Synchronise all positions with position[0].
+        for (size_t i = 1, positions_size = this->positions.size(); i < positions_size; ++i) {
+            // If some positions has nowhere to go, then sync is not possible.
+            if (this->positions[i] == this->ends[i]) { return false; }
+
+            //  Advance position[i] and position[0] to the closest equal values.
+            while (*this->positions[i] != *this->positions[0]) {
+
+                // Advance position[i] to or beyond position[0].
+                while (*this->positions[i] < *this->positions[0]) {
+                    ++this->positions[i];
+                    if (this->positions[i] == this->ends[i]) { return false; }
                 }
-            };
 
-            virtual bool advance() = 0;
-            virtual const std::vector<Iterator> get_current() = 0;
-        };
-
-
-
-        template<typename Iterator>
-        class SynchronizedUniversalIterator: public SynchronizedIterator<Iterator> {
-        public:
-
-           /* "minimum" would be the smallest class bounded from below by all positions that appears in all OrdContainers.
-            * Are we sure that all positions at this class?
-            * Invariant: it can be true only if all positions are indeed synchronized.
-            */
-            bool synchronized_at_current_minimum = false;
-
-           /* advance() advances all positions to the NEXT minimum and returns true.
-            * (though the next minimum might be the current state if synchronized_at_current_minimum is false).
-            * or returns false if positions cannot be synchronized.
-            * If positions are synchronized to start with,
-            * then synchronized_at_current_minimum decides whether to stay or advance further.
-            * The general of the algorithm is to synchronize everybody with position[0].
-            */
-            bool advance()
-            {
-                //Nothing to synchronize.
-                if (this->positions.empty())
-                    return false; //?? or not?
-
-                // If already synchronized, start moving forward by advancing position[0] (and so break synchronization).
-                if (this->synchronized_at_current_minimum) {
+                // Advance position[0] to or beyond position[i].
+                while (*this->positions[i] > *this->positions[0]) {
                     ++this->positions[0];
-                    synchronized_at_current_minimum = false;
+                    if (this->positions[0] == this->ends[0]) { return false; }
                 }
 
-                // If positions[0] has nowhere to go, then sync is not possible.
-                if (this->positions[0] == this->ends[0])
-                    return false;
-
-                // Synchronise all positions with position[0].
-                for (size_t i = 1, positions_size = this->positions.size(); i < positions_size; ++i)
-                {
-                    // If some positions has nowhere to go, then sync is not possible.
-                    if (this->positions[i] == this->ends[i])
-                        return false;
-
-                    //  Advance position[i] and position[0] to the closest equal values.
-                    while (*this->positions[i] != *this->positions[0]) {
-
-                        // Advance position[i] to or beyond position[0].
-                        while (*this->positions[i] < *this->positions[0]) {
-                            ++this->positions[i];
-                            if (this->positions[i] == this->ends[i])
-                                return false;
-                        }
-
-                        // Advance position[0] to or beyond position[i].
-                        while (*this->positions[i] > *this->positions[0]) {
-                            ++this->positions[0];
-                            if (this->positions[0] == this->ends[0])
-                                return false;
-                        }
-
-                        // If position[0] changed, start from position 1 again.
-                        // (note that
-                        // i gets incremented at the end of the for-loop body,
-                        // and that,
-                        // since we are inside the for, there are at least two positions
-                        // as the for starts with i=1.)
-                        if (this->positions[0] > this->positions[1])
-                            i=0;
-                    }
-                }
-                this->synchronized_at_current_minimum = true;
-                return true;
+                // If position[0] changed, start from position 1 again.
+                // (note that
+                // i gets incremented at the end of the for-loop body,
+                // and that,
+                // since we are inside the for, there are at least two positions
+                // as the for starts with i=1.)
+                if (this->positions[0] > this->positions[1]) { i=0; }
             }
+        }
+        this->synchronized_at_current_minimum = true;
+        return true;
+    }
 
-            // Returns the vector of current positions.
-            const std::vector<Iterator> get_current()
-            {
-                // How to return so that things don't get copied?
-                // Or maybe we should return a copy of positions anyway, to prevent a side effect of advance?
-                // Instead of returning a vector, we could also provide iterators through the result.
-                return this->positions;
-            };
-
-            explicit SynchronizedUniversalIterator(const int size=0) : SynchronizedIterator<Iterator>(size) {};
-
-            void reset(const int size = 0) {
-                SynchronizedIterator < Iterator > ::reset(size);
-                this->synchronized_at_current_minimum = false;
-            };
-        };
-
-        template<typename Iterator>
-        class SynchronizedExistentialIterator : public SynchronizedIterator<Iterator> {
-        public:
-
-            std::vector<Iterator> currently_synchronized; // Positions that are currently synchronized.
+    /// Returns the vector of current positions.
+    const std::vector<Iterator> get_current() {
+        // How to return so that things don't get copied?
+        // Or maybe we should return a copy of positions anyway, to prevent a side effect of advance?
+        // Instead of returning a vector, we could also provide iterators through the result.
+        return this->positions;
+    };
+
+    explicit SynchronizedUniversalIterator(const int size=0) : SynchronizedIterator<Iterator>(size) {};
+
+    void reset(const int size = 0) {
+        SynchronizedIterator < Iterator > ::reset(size);
+        this->synchronized_at_current_minimum = false;
+    };
+};
+
+template<typename Iterator>
+class SynchronizedExistentialIterator : public SynchronizedIterator<Iterator> {
+public:
+
+    std::vector<Iterator> currently_synchronized; // Positions that are currently synchronized.
+
+    Iterator next_minimum; // the value we should synchronise on after the first next call of advance().
+
+    bool is_synchronized() { return !currently_synchronized.empty(); }
+
+    Iterator get_current_minimum() {
+        if (currently_synchronized.empty()) {
+            throw std::runtime_error("Trying to get minimum from sync. ex. iterator which has no minimum. Don't do "
+                                     "that ever again or your nose falls off!");
+        }
+        return currently_synchronized[0];
+    }
 
-            Iterator next_minimum; // the value we should synchronise on after the first next call of advance().
 
-            bool is_synchronized() {
-                return !currently_synchronized.empty();
+    /**
+     * Advances all positions just above current_minimum,
+     * that is, to or above next_minimum.
+     * Those at next_minimum are added to currently_synchronized.
+     * Since next_minimum becomes the current minimum,
+     * new next_minimum must be updated too.
+     */
+    bool advance() {
+        // The next_minimum becomes the current current_minimum.
+        auto current_minimum = this->next_minimum;
+
+        // Here we collect the result.
+        currently_synchronized.clear();
+
+        for (size_t i = 0, positions_size = this->positions.size();i < positions_size;) {
+            if (this->positions[i] == this->ends[i]) {
+                // If there is nothing left at the position, it is removed, that is,
+                // swapped with a position form the end of the vector,
+                // and shorten the vector.
+                // The same is done with ends.
+                while (this->positions[i] == this->ends[i] && i < positions_size) {
+                    this->positions[i] = this->positions[positions_size - 1];
+                    this->ends[i] =      this->ends     [positions_size - 1];
+                    this->positions.pop_back();
+                    this->ends     .pop_back();
+                    positions_size--;
+                }
             }
-
-            const Iterator get_current_minimum()
-            {
-                if (currently_synchronized.empty())
-                    throw std::runtime_error("Trying to get minimum from sync. ex. iterator which has no minimum. Don't do that ever again or your nose falls off!");
-                return currently_synchronized[0];
+            // If the i-th position, i.e., where we are now, was erased,
+            // then we reached the end of active positions.
+            if (i == positions_size) { return !currently_synchronized.empty(); }
+
+            // If we are at the current_minimum, then save it and advance the position.
+            if (*this->positions[i] == *current_minimum) {
+                this->currently_synchronized.emplace_back(this->positions[i]);
+                ++this->positions[i];
+                continue;
             }
 
+            // If the position (now larger than current_minimum) is smaller than next_minimum,
+            // or next_minimum has not yet been updated, then update the next_minimum.
+            if (*this->next_minimum > *this->positions[i] || *this->next_minimum == *current_minimum) {
+                this->next_minimum = this->positions[i];
+            }
 
-            /* Advances all positions just above current_minimum,
-             * that is, to or above next_minimum.
-             * Those at next_minimum are added to currently_synchronized.
-             * Since next_minimum becomes the current minimum,
-             * new next_minimum must be updated too.
-             */
-            bool advance() {
-                // The next_minimum becomes the current current_minimum.
-                auto current_minimum = this->next_minimum;
-
-                // Here we collect the result.
-                currently_synchronized.clear();
-
-                for (size_t i = 0, positions_size = this->positions.size();i < positions_size;)
-                {
-                    if (this->positions[i] == this->ends[i])
-                        // If there is nothing left at the position, it is removed, that is,
-                        // swapped with a position form the end of the vector,
-                        // and shorten the vector.
-                        // The same is done with ends.
-                        while (this->positions[i] == this->ends[i] && i < positions_size)
-                        {
-                            this->positions[i] = this->positions[positions_size - 1];
-                            this->ends[i] =      this->ends     [positions_size - 1];
-                            this->positions.pop_back();
-                            this->ends     .pop_back();
-                            positions_size--;
-                        }
-                    // If the i-th position, i.e., where we are now, was erased,
-                    // then we reached the end of active positions.
-                    if (i == positions_size)
-                        return !currently_synchronized.empty();
-
-                    // If we are at the current_minimum, then save it and advance the position.
-                    if (*this->positions[i] == *current_minimum)
-                    {
-                        this->currently_synchronized.emplace_back(this->positions[i]);
-                        ++this->positions[i];
-                        continue;
-                    }
-
-                    // If the position (now larger than current_minimum) is smaller than next_minimum,
-                    // or next_minimum has not yet been updated, then update the next_minimum.
-                    if (*this->next_minimum > *this->positions[i] || *this->next_minimum == *current_minimum)
-                        this->next_minimum = this->positions[i];
-
-                    ++i;
-                }
-                return !currently_synchronized.empty();
-            };
-
-           /* Returns the vector of current still active positions.
-            * Beware, thy will be ordered differently from how there were input into the iterator.
-            * This is due to swapping of the emptied positions with positions at the end.
-            */
-            const std::vector<Iterator> get_current()
-            {
-                return this->currently_synchronized;
-            };
-
-            void push_back (const Iterator &begin, const Iterator &end) {
-
-                // Empty vector would not have any effect (unlike in the case of the universal iterator).
-                if (begin == end) return;
-
-                // Initialise next_minimum as the first position at the first vector.
-                if (this->positions.empty())
-                    this->next_minimum = begin;
-
-
-                // If the first position is of the new vector is smaller than minimum,
-                // update minimum.
-                else if (*this->next_minimum > *begin)
-                    this->next_minimum = begin;
-
-                // Let position point to the beginning the vector,
-                // save the end of the vector.
-                this->positions.emplace_back(begin);
-                this->ends.emplace_back(end);
-            };
-
-            explicit SynchronizedExistentialIterator(const int size=0) : SynchronizedIterator<Iterator>(size)
-            {
-                this->currently_synchronized.reserve(size);
-            };
-
-            void reset(const int size = 0) {
-                SynchronizedIterator < Iterator > ::reset(size);
-                if (size > 0) {
-                    this->currently_synchronized.reserve(size);
-                }
-
-                this->currently_synchronized.clear();
+            ++i;
+        }
+        return !currently_synchronized.empty();
+    };
+
+    /**
+     * @brief Returns the vector of current still active positions.
+     *
+     * Beware, thy will be ordered differently from how there were input into the iterator.
+     * This is due to swapping of the emptied positions with positions at the end.
+     */
+    const std::vector<Iterator> get_current() { return this->currently_synchronized; };
+
+    void push_back (const Iterator &begin, const Iterator &end) {
+
+        // Empty vector would not have any effect (unlike in the case of the universal iterator).
+        if (begin == end) return;
+
+        // Initialise next_minimum as the first position at the first vector.
+        if (this->positions.empty()) {
+            this->next_minimum = begin;
+        } else if (*this->next_minimum > *begin) {
+            // If the first position is of the new vector is smaller than minimum, update minimum.
+            this->next_minimum = begin;
+        }
+
+        // Let position point to the beginning the vector,
+        // save the end of the vector.
+        this->positions.emplace_back(begin);
+        this->ends.emplace_back(end);
+    }
 
-            };
-        };
+    explicit SynchronizedExistentialIterator(const int size=0) : SynchronizedIterator<Iterator>(size) {
+        this->currently_synchronized.reserve(size);
+    }
 
-       /* In order to make initialisation of the sync. iterator nicer than inputting v.begin() and v.end()
-        * as the two parameters of the method push_back,
-        * this function wraps the method push_back,
-        * takes the iterator and v and extracts the v.begin() and v.end() from v.
-        */
-        template<class Container>
-        void push_back (SynchronizedIterator<typename Container::const_iterator> &i,const Container &container) {
-            i.push_back(container.begin(),container.end());
-        };
+    void reset(const int size = 0) {
+        SynchronizedIterator < Iterator > ::reset(size);
+        if (size > 0) {
+            this->currently_synchronized.reserve(size);
+        }
+        this->currently_synchronized.clear();
     }
+};
+
+/**
+ * In order to make initialisation of the sync. iterator nicer than inputting v.begin() and v.end()
+ * as the two parameters of the method push_back,
+ * this function wraps the method push_back,
+ * takes the iterator and v and extracts the v.begin() and v.end() from v.
+ */
+template<class Container>
+void push_back (SynchronizedIterator<typename Container::const_iterator> &i,const Container &container) {
+    i.push_back(container.begin(),container.end());
 }
 
-#endif //LIBMATA_SYNCHRONIZED_ITERATOR_HH
+} // namespace Mata::Util.
+
+#endif // MATA_SYNCHRONIZED_ITERATOR_HH.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `libmata-0.66.0/mata/include/mata/util.hh` & `libmata-0.67.0/mata/include/mata/util.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/src/afa/afa.cc` & `libmata-0.67.0/mata/src/afa/afa.cc`

 * *Files 1% similar despite different names*

```diff
@@ -539,31 +539,35 @@
 	for(auto state : transitionrelation)
 	{
 		result += state.size();
 	}
 	return result;
 } // trans_size() }}}
 
-/** This function returns an upward-closed set of all
-* the nodes which are non-final
-* @return closed set of non-final nodes
-*/
-StateClosedSet Afa::get_non_final_nodes(void) const
-{
+StateClosedSet Afa::get_non_final_nodes() const {
 	StateClosedSet result(upward_closed_set, 0, transitionrelation.size()-1);
 	auto transSize = transitionrelation.size();
 	for(State state = 0; state < transSize; ++state)
 	{
 		if(!has_final(state))
 		{
 			result.insert(state);
-		}    
+		}
 	}
 	return result;
-} // get_non_final_nodes() }}}
+}
+
+StateClosedSet Afa::get_initial_nodes() const {
+    StateClosedSet result = StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1);
+    for(const auto& node : initialstates)
+    {
+        result.insert(node);
+    }
+    return result;
+}
 
 
 std::ostream& Mata::Afa::operator<<(std::ostream& os, const Afa& afa)
 { // {{{
 	return os << std::to_string(serialize(afa));
 } // Nfa::operator<<(ostream) }}}
 
@@ -1023,50 +1027,50 @@
         }
 
         return tgt_node;
     };
 
 
     const FormulaGraph* init_graph = &inter_aut.initial_formula;
-    if (is_node_operator(init_graph->node, FormulaNode::AND)) { // initial formula is just conjunction
+    if (is_node_operator(init_graph->node, FormulaNode::OperatorType::AND)) { // initial formula is just conjunction
     	Node initial_node;
         for (const auto& str : init_graph->collect_node_names())
         {
             State state = get_state_name(str);
             initial_node.insert(state);
         }
         aut.add_initial(initial_node);
     } else { // initial formula is dnf
-        while (is_node_operator(init_graph->node, FormulaNode::OR))
+        while (is_node_operator(init_graph->node, FormulaNode::OperatorType::OR))
         {  // Processes each clause separately
             assert(init_graph->children[1].node.is_operand() ||
-                   is_node_operator(init_graph->children[1].node, FormulaNode::AND) ||
+                   is_node_operator(init_graph->children[1].node, FormulaNode::OperatorType::AND) ||
                    "Clause should be conjunction or single state");
             // Conjunction is the right son of initent node
             Node initial_node;
             for (const auto s : init_graph->children[1].collect_node_names())
                 initial_node.insert(get_state_name(s));
             aut.add_initial(initial_node);
 
             // jump to another clause which is the left son of initent node
             init_graph = &init_graph->children.front();
         }
         assert(init_graph->node.is_operand() ||
-               is_node_operator(init_graph->node, FormulaNode::AND) ||
+               is_node_operator(init_graph->node, FormulaNode::OperatorType::AND) ||
                        "Remaining clause should be conjunction or single element");
         Node initial_node;
         for (const auto s : init_graph->collect_node_names())
             initial_node.insert(get_state_name(s));
         aut.add_initial(initial_node);
     }
 
     for (const auto& trans : inter_aut.transitions)
     {
         State src_state = get_state_name(trans.first.name);
-        if (trans.second.node.is_operand() && trans.second.node.operand_type == FormulaNode::SYMBOL)
+        if (trans.second.node.is_operand() && trans.second.node.operand_type == FormulaNode::OperandType::SYMBOL)
         {
             Symbol symbol = alphabet->translate_symb(trans.second.node.name);
             aut.add_trans(src_state, symbol, Node());
             continue;
         }
         else if (trans.second.children.size() != 2)
         {
@@ -1076,37 +1080,37 @@
             }
             else
             {
                 throw std::runtime_error("Invalid transition");
             }
         }
 
-        assert(is_node_operator(trans.second.node, FormulaNode::AND) ||
+        assert(is_node_operator(trans.second.node, FormulaNode::OperatorType::AND) ||
             "Clause of DNF should be conjunction");
         assert(trans.second.children.front().node.is_operand() || "Node in conjunction should be operand");
         Symbol symbol = alphabet->translate_symb(trans.second.children.front().node.name);
 
         const FormulaGraph* curr_graph = &trans.second.children[1];
 
-        while (is_node_operator(curr_graph->node, FormulaNode::OR))
+        while (is_node_operator(curr_graph->node, FormulaNode::OperatorType::OR))
         {  // Processes each clause separately
             assert(curr_graph->children[1].node.is_operand() ||
-                   is_node_operator(curr_graph->children[1].node, FormulaNode::AND) ||
+                   is_node_operator(curr_graph->children[1].node, FormulaNode::OperatorType::AND) ||
                    "Clause should be conjunction");
             // Conjunction is the right son of current node
             aut.add_trans(src_state, symbol,
                           create_node(curr_graph->children[1].collect_node_names()));
 
             // jump to another clause which is the left son of current node
             curr_graph = &curr_graph->children.front();
         }
 
         // process remaining conjunction
         assert(curr_graph->node.is_operand() ||
-               is_node_operator(curr_graph->node, FormulaNode::AND) ||
+               is_node_operator(curr_graph->node, FormulaNode::OperatorType::AND) ||
                "Remaining clause should be conjunction");
         aut.add_trans(src_state, symbol,
                       create_node(curr_graph->collect_node_names()));
     }
 
 	// TODO final states can be also given as true/false
 	if (inter_aut.are_final_states_conjunction_of_negation()) {
@@ -1162,26 +1166,33 @@
   assert(&aut);
   assert(&alphabet);
 
   // TODO
   assert(false);
 } // is_complete }}}
 
-bool Mata::Afa::accepts_epsilon(const Afa& aut)
-{ // {{{
-	for (const Node &node : aut.initialstates) {
-		if(node.IsSubsetOf(aut.finalstates))
-		{
-			return true;
-		}
-	}
+bool Mata::Afa::accepts_epsilon(const Afa& aut) {
+    return std::any_of(aut.initialstates.cbegin(), aut.initialstates.cend(),
+        [&aut](const Node& node) { return node.IsSubsetOf(aut.finalstates); });
+}
 
-	return false;
-} // accepts_epsilon }}}
+Word encode_word(const Mata::StringToSymbolMap &symbol_map, const std::vector<std::string> &input) {
+    Word result;
+    for (const auto& str : input) { result.insert(symbol_map.at(str)); }
+    return result;
+}
 
 std::ostream& std::operator<<(std::ostream& os, const Mata::Afa::AfaWrapper& afa_wrap)
 { // {{{
 	os << "{AFA wrapper|AFA: " << afa_wrap.afa << "|alphabet: " << afa_wrap.alphabet <<
 		"|state_dict: " << std::to_string(afa_wrap.state_dict) << "}";
 	return os;
 } // operator<<(AfaWrapper) }}}
 
+namespace std {
+    inline size_t hash<Mata::Afa::Trans>::operator()(const Mata::Afa::Trans& trans) const {
+        size_t accum = std::hash<Mata::Afa::State>{}(trans.src);
+        accum = Mata::Util::hash_combine(accum, trans.symb);
+        accum = Mata::Util::hash_combine(accum, trans.dst);
+        return accum;
+    }
+}
```

### Comparing `libmata-0.66.0/mata/src/inter-aut.cc` & `libmata-0.67.0/mata/src/inter-aut.cc`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,22 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#include <mata/inter-aut.hh>
-#include <mata/util.hh>
+#include "mata/inter-aut.hh"
 
-namespace
-{
+namespace {
     bool has_atmost_one_auto_naming(const Mata::IntermediateAut& aut)
     {
         return !(!(aut.node_naming == Mata::IntermediateAut::Naming::AUTO &&
               aut.symbol_naming == Mata::IntermediateAut::Naming::AUTO) &&
-                 (aut.state_naming == Mata::IntermediateAut::AUTO));
+                 (aut.state_naming == Mata::IntermediateAut::Naming::AUTO));
     }
 
     bool is_logical_operator(char ch)
     {
         return (Mata::Util::haskey(std::set<char>{'&', '|', '!'}, ch));
     }
 
@@ -187,17 +185,17 @@
         assert(false);
     }
 
     /**
      * Checks if @p op1 has lower precedence than @p op2. Precedence from the lowest to highest is: | < & < !
      */
     bool lower_precedence(Mata::FormulaNode::OperatorType op1, Mata::FormulaNode::OperatorType op2) {
-        if (op1 == Mata::FormulaNode::NEG) {
+        if (op1 == Mata::FormulaNode::OperatorType::NEG) {
             return false;
-        } else if (op1 == Mata::FormulaNode::AND && op2 != Mata::FormulaNode::NEG) {
+        } else if (op1 == Mata::FormulaNode::OperatorType::AND && op2 != Mata::FormulaNode::OperatorType::NEG) {
             return false;
         }
 
         return true;
     }
 
     /**
@@ -210,28 +208,28 @@
             const Mata::IntermediateAut &aut, const std::vector<std::string> &tokens) {
         std::vector<Mata::FormulaNode> opstack;
         std::vector<Mata::FormulaNode> output;
 
         for (const auto& token : tokens) {
             Mata::FormulaNode node = create_node(aut, token);
             switch (node.type) {
-                case Mata::FormulaNode::OPERAND:
+                case Mata::FormulaNode::Type::OPERAND:
                     output.push_back(node);
                     break;
-                case Mata::FormulaNode::LEFT_PARENTHESIS:
+                case Mata::FormulaNode::Type::LEFT_PARENTHESIS:
                     opstack.push_back(node);
                     break;
-                case Mata::FormulaNode::RIGHT_PARENTHESIS:
+                case Mata::FormulaNode::Type::RIGHT_PARENTHESIS:
                     while (!opstack.back().is_leftpar()) {
                         output.push_back(opstack.back());
                         opstack.pop_back();
                     }
                     opstack.pop_back();
                     break;
-                case Mata::FormulaNode::OPERATOR:
+                case Mata::FormulaNode::Type::OPERATOR:
                     for (int j = opstack.size()-1; j >= 0; --j) {
                         assert(!opstack[j].is_operand());
                         if (opstack[j].is_leftpar())
                             break;
                         if (lower_precedence(node.operator_type, opstack[j].operator_type)) {
                             output.push_back(opstack[j]);
                             opstack.erase(opstack.begin()+j);
@@ -265,20 +263,20 @@
     Mata::FormulaGraph postfix_to_graph(const std::vector<Mata::FormulaNode> &postfix)
     {
         std::vector<Mata::FormulaGraph> opstack;
 
         for (const auto& node : postfix) {
             Mata::FormulaGraph gr(node);
             switch (node.type) {
-                case Mata::FormulaNode::OPERAND:
+                case Mata::FormulaNode::Type::OPERAND:
                     opstack.push_back(gr);
                     break;
-                case Mata::FormulaNode::OPERATOR:
+                case Mata::FormulaNode::Type::OPERATOR:
                     switch (node.operator_type) {
-                        case Mata::FormulaNode::NEG:
+                        case Mata::FormulaNode::OperatorType::NEG:
                             assert(!opstack.empty());
                             gr.children.push_back(opstack.back());
                             opstack.pop_back();
                             opstack.push_back(gr);
                             break;
                         default:
                             assert(opstack.size() > 1);
@@ -316,21 +314,21 @@
         }
 
         std::vector<Mata::FormulaNode> res;
         if (postfix.size() >= 2) {
             res.push_back(postfix[0]);
             res.push_back(postfix[1]);
             res.push_back(Mata::FormulaNode(
-                    Mata::FormulaNode::OPERATOR, "|", "|", Mata::FormulaNode::OR));
+                    Mata::FormulaNode::Type::OPERATOR, "|", "|", Mata::FormulaNode::OperatorType::OR));
         }
 
         for (size_t i = 2; i < postfix.size(); ++i) {
             res.push_back(postfix[i]);
             res.push_back(Mata::FormulaNode(
-                    Mata::FormulaNode::OPERATOR, "|", "|", Mata::FormulaNode::OR));
+                    Mata::FormulaNode::Type::OPERATOR, "|", "|", Mata::FormulaNode::OperatorType::OR));
         }
 
         return res;
     }
 
     /**
      * The wrapping function for parsing one section of input to IntermediateAut.
@@ -411,15 +409,15 @@
         size_t trans_disjuncts = 0;
         std::vector<const FormulaGraph *> stack;
         stack.push_back(&trans.second);
 
         while (!stack.empty()) {
             const FormulaGraph *gr = stack.back();
             stack.pop_back();
-            if (gr->node.is_operator() && gr->node.operator_type == FormulaNode::OR)
+            if (gr->node.is_operator() && gr->node.operator_type == FormulaNode::OperatorType::OR)
                 trans_disjuncts++;
             for (const auto &ch: gr->children)
                 stack.push_back(&ch);
         }
         res += std::max(trans_disjuncts, (size_t) 1);
     }
 
@@ -437,31 +435,31 @@
     assert(tokens.size() > 1); // transition formula has at least two items
     const Mata::FormulaNode lhs = create_node(aut, tokens[0]);
     const std::vector<std::string> rhs(tokens.begin()+1, tokens.end());
 
     std::vector<Mata::FormulaNode> postfix;
 
     // add implicit conjunction to NFA explicit states, i.e. p a q -> p a & q
-    if (aut.automaton_type == Mata::IntermediateAut::NFA && tokens[tokens.size()-2] != "&") {
+    if (aut.automaton_type == Mata::IntermediateAut::AutomatonType::NFA && tokens[tokens.size()-2] != "&") {
         // we need to take care about this case manually since user does not need to determine
         // symbol and state naming and put conjunction to transition
-        if (aut.alphabet_type != Mata::IntermediateAut::BITVECTOR) {
+        if (aut.alphabet_type != Mata::IntermediateAut::AlphabetType::BITVECTOR) {
             assert(rhs.size() == 2);
             postfix.push_back(Mata::FormulaNode{Mata::FormulaNode::Type::OPERAND, rhs[0], rhs[0],
                                                 Mata::FormulaNode::OperandType::SYMBOL});
             postfix.push_back(create_node(aut,rhs[1]));
-        } else if (aut.alphabet_type == Mata::IntermediateAut::BITVECTOR) {
+        } else if (aut.alphabet_type == Mata::IntermediateAut::AlphabetType::BITVECTOR) {
             // this is a case where rhs state not separated by conjunction from rest of trans
             postfix = infix_to_postfix(aut, std::vector<std::string>(rhs.begin(), rhs.end()-1));
             postfix.push_back(create_node(aut,rhs.back()));
         } else
             assert(false && "Unknown NFA type");
 
         postfix.push_back(Mata::FormulaNode(
-                Mata::FormulaNode::OPERATOR, "&", "&", Mata::FormulaNode::AND));
+                Mata::FormulaNode::Type::OPERATOR, "&", "&", Mata::FormulaNode::OperatorType::AND));
     } else
         postfix = infix_to_postfix(aut, rhs);
 
     for (const auto& node : postfix) {
         assert(node.is_operator() || (node.name != "!" && node.name != "&" && node.name != "|"));
         assert(node.is_leftpar() || node.name != "(");
         assert(node.is_rightpar() || node.name != ")");
@@ -478,15 +476,15 @@
 
     stack.push_back(reinterpret_cast<const FormulaGraph *const>(&(this->node)));
     while (!stack.empty()) {
         const FormulaGraph* g = stack.back();
         assert(g != nullptr);
         stack.pop_back();
 
-        if (g->node.type == FormulaNode::UNKNOWN)
+        if (g->node.type == FormulaNode::Type::UNKNOWN)
            continue; // skip undefined nodes
 
         if (g->node.is_operand()) {
             res.insert(g->node.name);
         }
 
         for (const auto& child : g->children) {
@@ -534,23 +532,23 @@
 
 const Mata::FormulaGraph& Mata::IntermediateAut::get_symbol_part_of_transition(
         const std::pair<FormulaNode, FormulaGraph>& trans) const
 {
     if (!this->is_nfa()) {
         throw std::runtime_error("We currently support symbol extraction only for NFA");
     }
-    assert(trans.first.is_operand() && trans.first.operand_type == FormulaNode::STATE);
+    assert(trans.first.is_operand() && trans.first.operand_type == FormulaNode::OperandType::STATE);
     assert(trans.second.node.is_operator()); // conjunction with rhs state
     assert(trans.second.children[1].node.is_operand()); // rhs state
     return trans.second.children[0];
 }
 
 void Mata::IntermediateAut::add_transition(const FormulaNode& lhs, const FormulaNode& symbol, const FormulaGraph& rhs)
 {
-    FormulaNode conjunction(FormulaNode::OPERATOR, "&", "&", FormulaNode::AND);
+    FormulaNode conjunction(FormulaNode::Type::OPERATOR, "&", "&", FormulaNode::OperatorType::AND);
     FormulaGraph graph(conjunction);
     graph.children.push_back(FormulaGraph(symbol));
     graph.children.push_back(rhs);
     this->transitions.push_back(std::pair<FormulaNode, FormulaGraph>(lhs, graph));
 }
 
 void Mata::IntermediateAut::add_transition(const FormulaNode& lhs, const FormulaNode& rhs)
@@ -603,17 +601,17 @@
     return (act_graph->node.is_operator() && act_graph->node.is_neg());
 }
 
 std::ostream& std::operator<<(std::ostream& os, const Mata::IntermediateAut& inter_aut)
 {
     std::string type = inter_aut.is_nfa() ? "NFA" : (inter_aut.is_afa() ? "AFA" : "Unknown");
     os << "Intermediate automaton type " << type << '\n';
-    os << "Naming - state: " << inter_aut.state_naming << " symbol: " << inter_aut.symbol_naming << " node: "
-        << inter_aut.node_naming << '\n';
-    os << "Alphabet " << inter_aut.alphabet_type << '\n';
+    os << "Naming - state: " << static_cast<size_t>(inter_aut.state_naming) << " symbol: "
+       << static_cast<size_t>(inter_aut.symbol_naming) << " node: " << static_cast<size_t>(inter_aut.node_naming) << '\n';
+    os << "Alphabet " << static_cast<size_t>(inter_aut.alphabet_type) << '\n';
 
     os << "Initial states: ";
     for (const auto& state : inter_aut.initial_formula.collect_node_names()) {
         os << state << ' ';
     }
     os << '\n';
```

### Comparing `libmata-0.66.0/mata/src/mintermization.cc` & `libmata-0.67.0/mata/src/mintermization.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 /*
- * mintermization.hh -- Mintermization of automaton
+ * mintermization.hh -- Mintermization of automaton.
  * It transforms an automaton with a bitvector formula used a symbol to mintermized version of the automaton.
  *
- * Copyright (c) 2022 Martin Hruska <hruskamartin25@gmail.com>
- *
  * This file is a part of libmata.
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#include <mata/mintermization.hh>
+#include "mata/mintermization.hh"
 
-namespace
-{
+namespace {
     const Mata::FormulaGraph* detect_state_part(const Mata::FormulaGraph* node)
     {
         if (node->node.is_state())
             return node;
 
         std::vector<const Mata::FormulaGraph *> worklist{node};
         while (!worklist.empty()) {
@@ -82,19 +79,19 @@
         lhs_to_disjuncts_and_states[&trans.first] = std::vector<DisjunctStatesPair>();
         if (trans.second.node.is_state()) { // node from state to state
             lhs_to_disjuncts_and_states[&trans.first].push_back(DisjunctStatesPair(&trans.second, &trans.second));
         }
         // split transition to disjuncts
         const FormulaGraph *act_graph = &trans.second;
 
-        if (!trans.second.node.is_state() && act_graph->node.is_operator() && act_graph->node.operator_type != FormulaNode::OR) // there are no disjuncts
+        if (!trans.second.node.is_state() && act_graph->node.is_operator() && act_graph->node.operator_type != FormulaNode::OperatorType::OR) // there are no disjuncts
             lhs_to_disjuncts_and_states[&trans.first].push_back(DisjunctStatesPair(act_graph, detect_state_part(
                     act_graph)));
         else if (!trans.second.node.is_state()) {
-            while (act_graph->node.is_operator() && act_graph->node.operator_type == FormulaNode::OR) {
+            while (act_graph->node.is_operator() && act_graph->node.operator_type == FormulaNode::OperatorType::OR) {
                 // map lhs to disjunct and its state formula. The content of disjunct is right son of actual graph
                 // since the left one is a rest of formula
                 lhs_to_disjuncts_and_states[&trans.first].push_back(DisjunctStatesPair(&act_graph->children[1],
                                                                                        detect_state_part(
                                                                                            &act_graph->children[1])));
                 act_graph = &(act_graph->children.front());
             }
@@ -107,15 +104,15 @@
 
         // Foreach disjunct create a BDD
         for (const DisjunctStatesPair& ds_pair : lhs_to_disjuncts_and_states[&trans.first]) {
             // create bdd for the whole disjunct
             const auto bdd = (ds_pair.first == ds_pair.second) ? // disjunct contains only states
                     OptionalBdd(bdd_mng.bddOne()) : // transition from state to states -> add true as symbol
                     graph_to_bdd_afa(*ds_pair.first);
-            assert(bdd.type == OptionalBdd::BDD_E);
+            assert(bdd.type == OptionalBdd::TYPE::BDD_E);
             if (bdd.val.IsZero())
                 continue;
             trans_to_bddvar[ds_pair.first] = bdd.val;
             bdds.insert(bdd.val);
         }
     }
 }
@@ -148,35 +145,35 @@
 
 const Mata::Mintermization::OptionalBdd Mata::Mintermization::graph_to_bdd_afa(const FormulaGraph &graph)
 {
     const FormulaNode& node = graph.node;
 
     if (node.is_operand()) {
         if (node.is_state())
-            return OptionalBdd(OptionalBdd::NOTHING_E);
+            return OptionalBdd(OptionalBdd::TYPE::NOTHING_E);
         if (symbol_to_bddvar.count(node.name)) {
             return OptionalBdd(symbol_to_bddvar.at(node.name));
         } else {
             BDD res = (node.name == "true") ? bdd_mng.bddOne() :
                     (node.name == "false" ? bdd_mng.bddZero() : bdd_mng.bddVar());
             symbol_to_bddvar[node.name] = res;
             return OptionalBdd(res);
         }
     } else if (node.is_operator()) {
-        if (node.operator_type == FormulaNode::AND) {
+        if (node.operator_type == FormulaNode::OperatorType::AND) {
             assert(graph.children.size() == 2);
             const OptionalBdd op1 = graph_to_bdd_afa(graph.children[0]);
             const OptionalBdd op2 = graph_to_bdd_afa(graph.children[1]);
             return op1 * op2;
-        } else if (node.operator_type == FormulaNode::OR) {
+        } else if (node.operator_type == FormulaNode::OperatorType::OR) {
             assert(graph.children.size() == 2);
             const OptionalBdd op1 = graph_to_bdd_afa(graph.children[0]);
             const OptionalBdd op2 = graph_to_bdd_afa(graph.children[1]);
             return op1 + op2;
-        } else if (node.operator_type == FormulaNode::NEG) {
+        } else if (node.operator_type == FormulaNode::OperatorType::NEG) {
             assert(graph.children.size() == 1);
             const OptionalBdd op1 = graph_to_bdd_afa(graph.children[0]);
             return !op1;
         } else
             assert(false && "Unknown type of operation. It should conjunction, disjunction, or negation.");
     }
 
@@ -193,25 +190,25 @@
         } else {
             BDD res = (node.name == "true") ? bdd_mng.bddOne() :
                       (node.name == "false" ? bdd_mng.bddZero() : bdd_mng.bddVar());
             symbol_to_bddvar[node.name] = res;
             return res;
         }
     } else if (node.is_operator()) {
-        if (node.operator_type == FormulaNode::AND) {
+        if (node.operator_type == FormulaNode::OperatorType::AND) {
             assert(graph.children.size() == 2);
             const BDD op1 = graph_to_bdd_nfa(graph.children[0]);
             const BDD op2 = graph_to_bdd_nfa(graph.children[1]);
             return op1 * op2;
-        } else if (node.operator_type == FormulaNode::OR) {
+        } else if (node.operator_type == FormulaNode::OperatorType::OR) {
             assert(graph.children.size() == 2);
             const BDD op1 = graph_to_bdd_nfa(graph.children[0]);
             const BDD op2 = graph_to_bdd_nfa(graph.children[1]);
             return op1 + op2;
-        } else if (node.operator_type == FormulaNode::NEG) {
+        } else if (node.operator_type == FormulaNode::OperatorType::NEG) {
             assert(graph.children.size() == 1);
             const BDD op1 = graph_to_bdd_nfa(graph.children[0]);
             return !op1;
         } else
             assert(false);
     }
 
@@ -258,15 +255,15 @@
             size_t symbol = 0;
             for (const auto &minterm: minterms) {
                 // for each minterm x:
                 if (!((bdd * minterm).IsZero())) {
                     // if for symbol s of t is BDD_s < x
                     // add q1,x,q2 to transitions
                     const auto str_symbol = std::to_string(symbol);
-                    FormulaNode node_symbol(FormulaNode::OPERAND, str_symbol, str_symbol,
+                    FormulaNode node_symbol(FormulaNode::Type::OPERAND, str_symbol, str_symbol,
                                             Mata::FormulaNode::OperandType::SYMBOL);
                     if (ds_pair.second != nullptr)
                         res.add_transition(trans.first, node_symbol, *ds_pair.second);
                     else // transition without state on the right handed side
                         res.add_transition(trans.first, node_symbol);
                 }
                 ++symbol;
@@ -278,28 +275,28 @@
 Mata::IntermediateAut Mata::Mintermization::mintermize(const Mata::IntermediateAut& aut) {
     return mintermize(std::vector<const Mata::IntermediateAut *> {&aut})[0];
 }
 
 std::vector<Mata::IntermediateAut> Mata::Mintermization::mintermize(const std::vector<const Mata::IntermediateAut *> &auts)
 {
     for (const Mata::IntermediateAut *aut : auts) {
-        if ((!aut->is_nfa() && !aut->is_afa()) || aut->alphabet_type != IntermediateAut::BITVECTOR) {
+        if ((!aut->is_nfa() && !aut->is_afa()) || aut->alphabet_type != IntermediateAut::AlphabetType::BITVECTOR) {
             throw std::runtime_error("We currently support mintermization only for NFA and AFA with bitvectors");
         }
 
         aut->is_nfa() ? trans_to_bdd_nfa(*aut) : trans_to_bdd_afa(*aut);
     }
 
     // Build minterm tree over BDDs
     auto minterms = compute_minterms(bdds);
 
     std::vector<Mata::IntermediateAut> res;
     for (const Mata::IntermediateAut *aut : auts) {
         IntermediateAut mintermized_aut = *aut;
-        mintermized_aut.alphabet_type = IntermediateAut::EXPLICIT;
+        mintermized_aut.alphabet_type = IntermediateAut::AlphabetType::EXPLICIT;
         mintermized_aut.transitions.clear();
 
         if (aut->is_nfa())
             minterms_to_aut_nfa(mintermized_aut, *aut, minterms);
         else if (aut->is_afa())
             minterms_to_aut_afa(mintermized_aut, *aut, minterms);
 
@@ -312,7 +309,37 @@
 std::vector<Mata::IntermediateAut> Mata::Mintermization::mintermize(const std::vector<Mata::IntermediateAut> &auts) {
     std::vector<const Mata::IntermediateAut *> auts_pointers;
     for (const Mata::IntermediateAut &aut : auts) {
         auts_pointers.push_back(&aut);
     }
     return mintermize(auts_pointers);
 }
+
+Mata::Mintermization::OptionalBdd Mata::Mintermization::OptionalBdd::operator*(
+    const Mata::Mintermization::OptionalBdd& b) const {
+    if (this->type == TYPE::NOTHING_E) {
+        return b;
+    } else if (b.type == TYPE::NOTHING_E) {
+        return *this;
+    } else {
+        return OptionalBdd{ TYPE::BDD_E, this->val * b.val };
+    }
+}
+
+Mata::Mintermization::OptionalBdd Mata::Mintermization::OptionalBdd::operator+(
+    const Mata::Mintermization::OptionalBdd& b) const {
+    if (this->type == TYPE::NOTHING_E) {
+        return b;
+    } else if (b.type == TYPE::NOTHING_E) {
+        return *this;
+    } else {
+        return OptionalBdd{ TYPE::BDD_E, this->val + b.val };
+    }
+}
+
+Mata::Mintermization::OptionalBdd Mata::Mintermization::OptionalBdd::operator!() const {
+    if (this->type == TYPE::NOTHING_E) {
+        return OptionalBdd(TYPE::NOTHING_E);
+    } else {
+        return OptionalBdd{ TYPE::BDD_E, !this->val };
+    }
+}
```

### Comparing `libmata-0.66.0/mata/src/nfa/nfa-complement.cc` & `libmata-0.67.0/mata/src/nfa/nfa-complement.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/src/nfa/nfa-concatenation.cc` & `libmata-0.67.0/mata/src/nfa/nfa-concatenation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/src/nfa/nfa-inclusion.cc` & `libmata-0.67.0/mata/src/nfa/nfa-inclusion.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/src/nfa/nfa-intersection.cc` & `libmata-0.67.0/mata/src/nfa/nfa-intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/src/nfa/nfa-universal.cc` & `libmata-0.67.0/mata/src/nfa/nfa-universal.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/src/nfa/nfa.cc` & `libmata-0.67.0/mata/src/nfa/nfa.cc`

 * *Files 3% similar despite different names*

```diff
@@ -418,14 +418,39 @@
         post_iterator = post[current_state].begin();
         targets_position = post_iterator->targets.begin();
     }
 
     return *this;
 }
 
+const Delta::const_iterator Delta::const_iterator::operator++(int) {
+    const const_iterator tmp = *this;
+    ++(*this);
+    return tmp;
+}
+
+Delta::const_iterator& Delta::const_iterator::operator=(const Delta::const_iterator& x) {
+    this->post_iterator = x.post_iterator;
+    this->targets_position = x.targets_position;
+    this->current_state = x.current_state;
+    this->is_end = x.is_end;
+
+    return *this;
+}
+
+bool Mata::Nfa::operator==(const Delta::const_iterator& a, const Delta::const_iterator& b) {
+    if (a.is_end && b.is_end)
+        return true;
+    else if ((a.is_end && !b.is_end) || (!a.is_end && b.is_end))
+        return false;
+    else
+        return a.current_state == b.current_state && a.post_iterator == b.post_iterator
+               && a.targets_position == b.targets_position;
+}
+
 State Delta::find_max_state() {
     size_t max = 0;
     State src = 0;
     for (Post & p: posts) {
         if (src > max)
             max = src;
         for (Move & m: p) {
@@ -434,15 +459,80 @@
                     max = m.targets.back();
         }
         src++;
     }
     return max;
 }
 
-///// Nfa structure related methods
+Post& Delta::get_mutable_post(State q) {
+    if (q >= posts.size()) {
+        Util::reserve_on_insert(posts, q);
+        const size_t new_size{ q + 1 };
+        posts.resize(new_size);
+    }
+
+    return posts[q];
+}
+
+std::vector<State> Delta::defragment(NumberPredicate<State>& is_staying) {
+    //first, indexes of post are filtered (places of to be removed states are taken by states on their right)
+    size_t move_index{ 0 };
+    posts.erase(
+            std::remove_if(posts.begin(), posts.end(), [&](Post& _post) -> bool {
+                size_t prev{ move_index };
+                ++move_index;
+                return !is_staying[prev];
+            }),
+            posts.end()
+    );
+
+    //get renaming of current states to new numbers:
+    std::vector<State> renaming(this->find_max_state()+1);
+    size_t i = 0;
+    for (State q:is_staying.get_elements()) {
+        if (q >= renaming.size())
+            break;
+        renaming[q] = i;
+        i++;
+    }
+
+    //this iterates through every post and ever, filters and renames states,
+    //and finally removes moves that became empty from the post.
+    for (State q=0,size=posts.size(); q < size; ++q) {
+        //should we have a function Post::transform(Lambda) for this?
+        Post & p = get_mutable_post(q);
+        for (auto move = p.begin(); move < p.end(); ++move) {
+            move->targets.erase(
+                    std::remove_if(move->targets.begin(), move->targets.end(), [&](State q) -> bool {
+                        return !is_staying[q];
+                    }),
+                    move->targets.end()
+            );
+            move->targets.rename(renaming);
+        }
+        p.erase(
+                std::remove_if(p.begin(), p.end(), [&](Move& move) -> bool {
+                    return move.targets.empty();
+                }),
+                p.end()
+        );
+    }
+
+    //the renaming can be useful somewhere, computed anyway, we can as well return it.
+    return renaming;
+}
+
+const Post& Delta::operator[](State q) const {
+    if (q >= posts.size()) {
+        return empty_post;
+    }
+    return posts[q];
+}
+
+///// Nfa structure related methods.
 
 void Nfa::remove_epsilon(const Symbol epsilon)
 {
     *this = Mata::Nfa::remove_epsilon(*this, epsilon);
 }
 
 StateSet Nfa::get_reachable_states() const
@@ -710,16 +800,14 @@
     }
 
     return was_something_added;
 }
 
 //TODO: based on the comments inside, this function needs to be rewritten in a more optimal way.
 Nfa Mata::Nfa::remove_epsilon(const Nfa& aut, Symbol epsilon) {
-    Nfa result{ aut.delta.num_of_states() };
-
     // cannot use multimap, because it can contain multiple occurrences of (a -> a), (a -> a)
     std::unordered_map<State, StateSet> eps_closure;
 
     // TODO: grossly inefficient
     // first we compute the epsilon closure
     const size_t num_of_states{aut.size() };
     for (size_t i{ 0 }; i < num_of_states; ++i)
@@ -733,56 +821,50 @@
                 // TODO: Fix possibly insert to OrdVector. Create list already ordered, then merge (do not need to resize each time);
                 closure.insert(trans.targets);
             }
         }
     }
 
     bool changed = true;
-    while (changed) { // compute the fixpoint
+    while (changed) { // Compute the fixpoint.
         changed = false;
-        for (size_t i=0; i < num_of_states; ++i) {
-            const auto& state_transitions{ aut.delta[i] };
-            const auto state_symbol_transitions{
-                state_transitions.find(Move{epsilon}) };
-            if (state_symbol_transitions != state_transitions.end()) {
-                StateSet &src_eps_cl = eps_closure[i];
-                for (const State tgt: state_symbol_transitions->targets) {
-                    const StateSet &tgt_eps_cl = eps_closure[tgt];
+        for (size_t i = 0; i < num_of_states; ++i) {
+            const Post& post{ aut.delta[i] };
+            const auto eps_move_it { post.find(Move{ epsilon}) };//TODO: make faster if default epsilon
+            if (eps_move_it != post.end()) {
+                StateSet& src_eps_cl = eps_closure[i];
+                for (const State tgt: eps_move_it->targets) {
+                    const StateSet& tgt_eps_cl = eps_closure[tgt];
                     for (const State st: tgt_eps_cl) {
                         if (src_eps_cl.count(st) == 0) {
                             changed = true;
                             break;
                         }
                     }
                     src_eps_cl.insert(tgt_eps_cl);
                 }
             }
         }
     }
 
-    // now we construct the automaton without epsilon transitions
-    //TODO: this is a stupid way of initialising it ...
-    result.initial.add(aut.initial.get_elements());
-    result.final.add(aut.final.get_elements());
-    State max_state{};
-    for (const auto& state_closure_pair : eps_closure) { // for every state
+    // Construct the automaton without epsilon transitions.
+    Nfa result{ Delta{}, aut.initial, aut.final, aut.alphabet };
+    for (const auto& state_closure_pair : eps_closure) { // For every state.
         State src_state = state_closure_pair.first;
-        for (State eps_cl_state : state_closure_pair.second) { // for every state in its eps cl
+        for (State eps_cl_state : state_closure_pair.second) { // For every state in its epsilon closure.
             if (aut.final[eps_cl_state]) result.final.add(src_state);
-            for (const auto& symb_set : aut.delta[eps_cl_state]) {
-                if (symb_set.symbol == epsilon) continue;
-
+            for (const Move& move : aut.delta[eps_cl_state]) {
+                if (move.symbol == epsilon) continue;
                 // TODO: this could be done more efficiently if we had a better add method
-                for (State tgt_state : symb_set.targets) {
-                    result.delta.add(src_state, symb_set.symbol, tgt_state);
+                for (State tgt_state : move.targets) {
+                    result.delta.add(src_state, move.symbol, tgt_state);
                 }
             }
         }
     }
-
     return result;
 }
 
 Nfa Mata::Nfa::fragile_revert(const Nfa& aut) {
     const size_t num_of_states{ aut.size() };
 
     Nfa result(num_of_states);
@@ -1772,15 +1854,22 @@
         return *this;
     }
 
     // out of transitions
     this->is_end = true;
 
     return *this;
-} // operator++ }}}
+}
+
+bool Nfa::const_iterator::operator==(const Nfa::const_iterator& rhs) const {
+    if (this->is_end && rhs.is_end) { return true; }
+    if ((this->is_end && !rhs.is_end) || (!this->is_end && rhs.is_end)) { return false; }
+    return ssIt == rhs.ssIt && tlIt == rhs.tlIt && trIt == rhs.trIt;
+}
+// operator++ }}}
 
 std::ostream& std::operator<<(std::ostream& os, const Mata::Nfa::Nfa& nfa) {
     os << "{ NFA: " << std::to_string(serialize(nfa));
     if (nfa.alphabet != nullptr) {
         os << "|alphabet: " << *(nfa.alphabet);
     }
     // TODO: If the default implementation for state_dict is implemented, consider printing the state dictionary with
@@ -1931,14 +2020,118 @@
         for (const auto& state_transitions: delta[state]) {
             alphabet.update_next_symbol_value(state_transitions.symbol);
             alphabet.try_add_new_symbol(std::to_string(state_transitions.symbol), state_transitions.symbol);
         }
     }
 }
 
+Nfa& Nfa::operator=(Nfa&& other) noexcept {
+    if (this != &other) {
+        delta = std::move(other.delta);
+        initial = std::move(other.initial);
+        final = std::move(other.final);
+        alphabet = other.alphabet;
+        attributes = std::move(other.attributes);
+        other.alphabet = nullptr;
+    }
+    return *this;
+}
+
+void Nfa::clear_transitions() {
+    const size_t delta_size = delta.num_of_states();
+    for (size_t i = 0; i < delta_size; ++i) {
+        delta.get_mutable_post(i) = Post();
+    }
+}
+
+State Nfa::add_state() {
+    const size_t num_of_states{ size() };
+    delta.increase_size(num_of_states + 1 );
+    return num_of_states;
+}
+
+State Nfa::add_state(State state) {
+    if (state >= delta.num_of_states()) {
+        delta.increase_size(state + 1);
+    }
+    return state;
+}
+
+size_t Nfa::size() const {
+    return std::max({
+        static_cast<unsigned long>(initial.domain_size()),
+        static_cast<unsigned long>(final.domain_size()),
+        static_cast<unsigned long>(delta.num_of_states())
+    });
+}
+
+void Nfa::clear() {
+    delta.clear();
+    initial.clear();
+    final.clear();
+}
+
+bool Nfa::is_identical(const Nfa& aut) {
+    if (Util::OrdVector<State>(initial.get_elements()) != Util::OrdVector<State>(aut.initial.get_elements())) {
+        return false;
+    }
+    if (Util::OrdVector<State>(final.get_elements()) != Util::OrdVector<State>(aut.final.get_elements())) {
+        return false;
+    }
+
+    std::vector<Trans> this_trans;
+    for (auto trans: *this) { this_trans.push_back(trans); }
+    std::vector<Trans> aut_trans;
+    for (auto trans: aut) { aut_trans.push_back(trans); }
+    return this_trans == aut_trans;
+}
+
+OrdVector<Symbol> Nfa::get_used_symbols() const {
+    //TODO: look at the variants in profiling (there are tests in tests-nfa-profiling.cc),
+    // for instance figure out why NumberPredicate and OrdVedctor are slow,
+    // try also with _STATIC_DATA_STRUCTURES_, it changes things.
+
+    //below are different variant, with different data structures for accumulating symbols,
+    //that then must be converted to an OrdVector
+    //measured are times with "Mata::Nfa::get_used_symbols speed, harder", "[.profiling]" now on line 104 of nfa-profiling.cc
+
+    //WITH VECTOR (4.434 s)
+    //return get_used_symbols_vec();
+
+    //WITH SET (26.5 s)
+    //auto from_set = get_used_symbols_set();
+    //return Util::OrdVector<Symbol> (from_set .begin(),from_set.end());
+
+    //WITH NUMBER PREDICATE (4.857s)
+    //return Util::OrdVector(get_used_symbols_np().get_elements());
+
+    //WITH BOOL VECTOR (error !!!!!!!):
+    //return Util::OrdVector<Symbol>(Util::NumberPredicate<Symbol>(get_used_symbols_bv()));
+
+    //WITH BOOL VECTOR (1.9s):
+    std::vector<bool> bv = get_used_symbols_bv();
+    Util::OrdVector<Symbol> ov;
+    //int count = 0;
+    //for(Symbol i = 0;i<bv.size();i++)
+    //    if (bv[i]) {
+    //        count++;
+    //    }
+    //ov.reserve(count);
+    for(Symbol i = 0;i<bv.size();i++)
+        if (bv[i]) {
+            ov.push_back(i);
+        }
+    return ov;
+
+    ///WITH BOOL VECTOR, DIFFERENT VARIANT? (1.9s):
+    //std::vector<bool> bv = get_used_symbols_bv();
+    //std::vector<Symbol> v(std::count(bv.begin(), bv.end(), true));
+    //return Util::OrdVector<Symbol>(v);
+}
+
 Mata::OnTheFlyAlphabet Mata::Nfa::create_alphabet(const ConstAutRefSequence& nfas) {
     Mata::OnTheFlyAlphabet alphabet{};
     for (const auto& nfa: nfas) {
         fill_alphabet(nfa, alphabet);
     }
     return alphabet;
 }
@@ -1974,7 +2167,33 @@
 Nfa Mata::Nfa::create_sigma_star_nfa(Mata::Alphabet* alphabet) {
     Nfa nfa{ 1, StateSet{ 0 }, StateSet{ 0 }, alphabet };
     for (const Mata::Symbol& symbol : alphabet->get_alphabet_symbols()) {
         nfa.delta.add(0, symbol, 0);
     }
     return nfa;
 }
+
+Run Mata::Nfa::encode_word(const Mata::StringToSymbolMap& symbol_map, const std::vector<std::string>& input) {
+    Run result;
+    for (const auto& str : input) { result.word.push_back(symbol_map.at(str)); }
+    return result;
+}
+
+Move& Move::operator=(Move&& rhs) noexcept {
+    if (*this != rhs) {
+        symbol = rhs.symbol;
+        targets = std::move(rhs.targets);
+    }
+    return *this;
+}
+
+void Move::insert(State s) {
+    if (targets.find(s) == targets.end()) {
+        targets.insert(s);
+    }
+}
+
+void Move::insert(StateSet states) {
+    for (State s : states) {
+        insert(s);
+    }
+}
```

### Comparing `libmata-0.66.0/mata/src/parser.cc` & `libmata-0.67.0/mata/src/parser.cc`

 * *Files 6% similar despite different names*

```diff
@@ -397,7 +397,47 @@
 	const std::string&  input,
 	bool                keepQuotes)
 { // {{{
 	std::istringstream stream(input);
 	ParsedSection result = parse_mf_section(stream, keepQuotes);
 	return result;
 } // parse_mf_section(std::string) }}}
+
+const std::vector<std::string>& Mata::Parser::ParsedSection::operator[](const std::string& key) const {
+    auto it = this->dict.find(key);
+    if (this->dict.end() == it) {
+        assert(false);
+        // return this->dict.at("");
+    }
+
+    return it->second;
+}
+
+bool Mata::Parser::ParsedSection::operator==(const ParsedSection& rhs) const {
+    return
+        this->type == rhs.type &&
+        this->dict == rhs.dict &&
+        this->body == rhs.body;
+}
+
+std::ostream& Mata::Parser::operator<<(std::ostream& os, const ParsedSection& parsec) {
+    os << "@" << parsec.type << "\n";
+    for (const auto& string_list_pair : parsec.dict) {
+        os << "%" << string_list_pair.first;
+        for (const std::string& str : string_list_pair.second) {
+            os << " " << str;
+        }
+        os << "\n";
+    }
+
+    os << "# Body:\n";
+    for (const auto& body_line : parsec.body) {
+        bool first = true;
+        for (const std::string& str : body_line) {
+            if (!first) { os << " ";}
+            first = false;
+            os << str;
+        }
+        os << "\n";
+    }
+    return os;
+}
```

### Comparing `libmata-0.66.0/mata/src/re2parser.cc` & `libmata-0.67.0/mata/src/re2parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/src/strings/nfa-noodlification.cc` & `libmata-0.67.0/mata/src/strings/nfa-noodlification.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/src/strings/nfa-segmentation.cc` & `libmata-0.67.0/mata/src/strings/nfa-segmentation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.66.0/mata/src/strings/nfa-strings.cc` & `libmata-0.67.0/mata/src/strings/nfa-strings.cc`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 using namespace Mata::Nfa;
 using namespace Mata::Strings;
 
 WordSet Mata::Strings::get_shortest_words(const Nfa::Nfa& nfa) {
     // Map mapping states to a set of the shortest words accepted by the automaton from the mapped state.
     // Get the shortest words for all initial states accepted by the whole automaton (not just a part of the automaton).
-    return Strings::ShortestWordsMap{ nfa }.get_shortest_words_for(nfa.initial);
+    return ShortestWordsMap{ nfa }.get_shortest_words_for(StateSet{ nfa.initial });
 }
 
 WordSet ShortestWordsMap::get_shortest_words_for(const StateSet& states) const
 {
     WordSet result{};
 
     if (!shortest_words_map.empty())
```

### Comparing `libmata-0.66.0/setup.py` & `libmata-0.67.0/setup.py`

 * *Files identical despite different names*

