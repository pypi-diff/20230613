# Comparing `tmp/naluconfigs-11.1.0.tar.gz` & `tmp/naluconfigs-11.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-11.1.0.tar", last modified: Mon Jun 12 00:27:09 2023, max compression
+gzip compressed data, was "naluconfigs-11.1.1.tar", last modified: Mon Jun 12 23:28:59 2023, max compression
```

## Comparing `naluconfigs-11.1.0.tar` & `naluconfigs-11.1.1.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:27:09.824990 naluconfigs-11.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-12 00:27:09.824990 naluconfigs-11.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 00:27:09.824990 naluconfigs-11.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:27:09.812990 naluconfigs-11.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:27:09.812990 naluconfigs-11.1.0/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:27:09.812990 naluconfigs-11.1.0/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:27:09.816990 naluconfigs-11.1.0/src/naluconfigs/data/chips/
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/chips/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/chips/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/chips/aodsv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/chips/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/chips/hdsocv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/chips/udc16.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:27:09.820990 naluconfigs-11.1.0/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:27:09.820990 naluconfigs-11.1.0/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32645 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:27:09.812990 naluconfigs-11.1.0/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-12 00:27:09.000000 naluconfigs-11.1.0/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-12 00:27:09.000000 naluconfigs-11.1.0/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 00:27:09.000000 naluconfigs-11.1.0/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-12 00:27:09.000000 naluconfigs-11.1.0/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 00:27:09.000000 naluconfigs-11.1.0/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:27:09.824990 naluconfigs-11.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/tests/test_multichip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-12 00:26:51.000000 naluconfigs-11.1.0/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.554154 naluconfigs-11.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.558154 naluconfigs-11.1.1/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.554154 naluconfigs-11.1.1/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.558154 naluconfigs-11.1.1/src/naluconfigs/data/chips/
+-rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/aodsv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/hdsocv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/udc16.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.562154 naluconfigs-11.1.1/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv3_gbe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.558154 naluconfigs-11.1.1/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_range_keys.py
```

### Comparing `naluconfigs-11.1.0/PKG-INFO` & `naluconfigs-11.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.1.0
+Version: 11.1.1
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.1.0/README.md` & `naluconfigs-11.1.1/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/pyproject.toml` & `naluconfigs-11.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/setup.py` & `naluconfigs-11.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/__init__.py` & `naluconfigs-11.1.1/src/naluconfigs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from . import _constructors
 from ._version import __version__
 from .helpers import CLOCKS_DIR, REGISTERS_DIR
 
 _VALID_BOARDS = [
     "aardvarcv2",
     "aardvarcv3",
+    "aardvarcv3_gbe",
     "aardvarcv4",
     "aodsv1",
     "aodsv2_eval",
     "asoc",
     "asocv2",
     "asocv3",
     "trbhm",
```

### Comparing `naluconfigs-11.1.0/src/naluconfigs/_constructors.py` & `naluconfigs-11.1.1/src/naluconfigs/_constructors.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/chips/aardvarcv3.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/chips/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/chips/aodsv1.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/chips/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/chips/aodsv2.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/chips/aodsv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/chips/asocv3.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/chips/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/chips/hdsocv1.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/chips/hdsocv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/chips/udc16.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/chips/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/chips/aardvarcv4.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,104 +1,14 @@
-model: aardvarcv4
-features:
-  adc2mv: true
-  dac_sweep: true
-  ext_dac: true
-  pedestals: true
-  threshold_scan: true
-  tia_dac: false
-  timing_calibration: true
-  naludaq_rs: true
 params:
-  chanmask: 0xE00
   channels: 8
-  chanshift: 9
-  clock_file: Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
-  connections:
-    - serial
-    - d2xx
-    - udp
-  si5341_address: 0xE8
-  default_baud:
-    115200: 53
-  default_baudrate: 115200
-  default_clock: 100000000.0
-  default_divider: 53
-  default_trigger_value: 1500
-  threshold_scan:
-    min_vref: 0
-    max_vref: 2500
-    start: 500
-    stop: 3500
-    stepsize: 5
-    units: counts
-  expected_scalmon: 2500
-  ext_dac:
-    chip: dac7578
-    max_mv: 1200
-    max_counts: 4095
-    channels:
-      0..7: 2048
-    address_mapping:
-      0..7: 0x4E
-    channel_mapping:
-      0: 4
-      1: 3
-      2: 5
-      3: 2
-      4: 6
-      5: 1
-      6: 7
-      7: 0
-  headers: 3
-  new_firmware: True
-  numregs: 64
-  pedestals_blocks: 16
-  peripherals:
-    current:
-      chan: 0
-      addr: 0xD0
-      bits: 16
-      gain: 8
-    vadjn:
-      chan: 0
-      addr: 0xD8
-      bits: 16
-      gain: 1
-    vadjp:
-      chan: 1
-      addr: 0xD8
-      bits: 16
-      gain: 1
-  possible_bauds:
-    115200: 53
-    230400: 26
-    691200: 8
-    1041667: 5
+  name: aardvarcv4
+  readable_name: AARDVARCv4
   resolution: 12
   samples: 64
-  samplingrate: 10.0
-  stop_word: !!binary |
-    +s4=
-  strobe_values_correction: True  # Shift the strobe values on certain boards with swapped internal routing.
-  strobe_correction_keys:
-    - calstrb_le
-    - calstrb_te
-    - wrstrb1_le
-    - wrstrb1_te
-    - wrstrb2_le
-    - wrstrb2_te
-    - wrsync1_le
-    - wrsync1_te
-    - wrsync2_le
-    - wrsync2_te
-  wait: AE000001
-  wbias: 2000
-  windmask: 0x1FE
-  windows: 255
+  windows: 510
 registers:
   analog_registers:
     mont2_select:
       address: 0x00
       bitposition: 0
       bitwidth: 3
       description: ''
@@ -856,414 +766,14 @@
     # vtune:
     #   address: 0x16
     #   bitposition: 0
     #   bitwidth: 12
     #   description: ''
     #   readwrite: w
     #   value: 1365
-  control_registers:
-    1v2_en:
-      address: 0x17
-      bitposition: 1
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    2v5_en:
-      address: 0x17
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    3v3_i2c_en:
-      address: 0x17
-      bitposition: 2
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    8b10b_en:
-      address: 0x19
-      bitposition: 12
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    addr:
-      address: 0x16
-      bitposition: 0
-      bitwidth: 9
-      description: ''
-      readwrite: rw
-      value: 0
-    addr_user:
-      address: 0x16
-      bitposition: 15
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    chansel:
-      address: 0x06
-      bitposition: 12
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 15
-    clk1v8_en:
-      address: 0x17
-      bitposition: 4
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk2v5_en:
-      address: 0x17
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk_fdec:
-      address: 0x17
-      bitposition: 9
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_finc:
-      address: 0x17
-      bitposition: 8
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_i2c_sel:
-      address: 0x17
-      bitposition: 5
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk_oeb:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_reset:
-      address: 0x17
-      bitposition: 7
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_sync:
-      address: 0x17
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    data:
-      address: 0x14
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    data_user:
-      address: 0x14
-      bitposition: 15
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    debug_data:
-      address: 0x15
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    debug_data_user:
-      address: 0x15
-      bitposition: 15
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    digrst:
-      address: 0x16
-      bitposition: 9
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    digser_rst:
-      address: 0x19
-      bitposition: 13
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    exttrig:
-      address: 0x04
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    gccclr:
-      address: 0x04
-      bitposition: 4
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    identifier:
-      address: 0x00
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 43716
-    iomode0:
-      address: 0x04
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    iomode1:
-      address: 0x04
-      bitposition: 6
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    leds:
-      address: 0x18
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    loadwait:
-      address: 0x07
-      bitposition: 8
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 15
-    nramp:
-      address: 0x04
-      bitposition: 5
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    nrw:
-      address: 0x04
-      bitposition: 11
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    numwinds:
-      address: 0x08
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 1
-    pclk:
-      address: 0x04
-      bitposition: 2
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    pclkwidth:
-      address: 0x07
-      bitposition: 12
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 15
-    ramplen:
-      address: 0x06
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 2000
-    regclr:
-      address: 0x04
-      bitposition: 1
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    runevs:
-      address: 0x05
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 1
-    rx_data0:
-      address: 0x1A
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data1:
-      address: 0x1B
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data2:
-      address: 0x1C
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data3:
-      address: 0x1D
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data4:
-      address: 0x1E
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data5:
-      address: 0x1F
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_data6:
-      address: 0x20
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_en:
-      address: 0x19
-      bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_num_words:
-      address: 0x19
-      bitposition: 2
-      bitwidth: 6
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_oneshot:
-      address: 0x19
-      bitposition: 1
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_speed:
-      address: 0x19
-      bitposition: 8
-      bitwidth: 2
-      description: ''
-      readwrite: rw
-      value: 0
-    sel:
-      address: 0x04
-      bitposition: 12
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    selany:
-      address: 0x04
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    slow_sysclk:
-      address: 0x19
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    stopacq:
-      address: 0x04
-      bitposition: 13
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    syncloc:
-      address: 0x09
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    sysclk:
-      address: 0x04
-      bitposition: 8
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    sysrst:
-      address: 0x04
-      bitposition: 9
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    tx_en:
-      address: 0x19
-      bitposition: 11
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    windsel:
-      address: 0x07
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    wrstrboff:
-      address: 0x04
-      bitposition: 7
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
   digital_registers:
     scal0:
       address: 0x00
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
@@ -1628,92 +1138,7 @@
     roilength76:
       address: 0xBC
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
-  i2c_registers:
-    i2c_en:
-      address: 0x0F
-      bitposition: 14
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    i2c_send:
-      address: 0x0F
-      bitposition: 15
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    i2c_words:
-      address: 0x0F
-      bitposition: 8
-      bitwidth: 3
-      description: ''
-      readwrite: rw
-      value: 0
-    i2c_addr:
-      address: 0x0F
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    i2c_data0:
-      address: 0x10
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    i2c_data1:
-      address: 0x11
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    i2c_data2:
-      address: 0x12
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    i2c_data3:
-      address: 0x13
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 0
-    response0:
-      address: 0x48
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: r
-      value: 0
-    response1:
-      address: 0x49
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: r
-      value: 0
-    response2:
-      address: 0x4A
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: r
-      value: 0
-    response3:
-      address: 0x4B
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: r
-      value: 0
```

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsoc_asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsv2_eval.yml`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
       0..3: 0xC
     channel_mapping:
       0: 1
       1: 0
       2: 5
       3: 4
   headers: 3
-  numregs: 36
+  numregs: 64
   pedestals_blocks: 32
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
@@ -247,15 +247,15 @@
       value: 0
     ext_en:
       address: 0x0B
       bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: false
     exttrig:
       address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
@@ -572,34 +572,34 @@
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
     response0:
-      address: 0x2C
+      address: 0x48
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x2D
+      address: 0x49
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x2E
+      address: 0x4A
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x2F
+      address: 0x4B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/asocv2.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/asocv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/asocv3.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/asocv3.yml`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
       0..3: 0xC
     channel_mapping:
       0: 1
       1: 0
       2: 5
       3: 4
   headers: 3
-  numregs: 36
+  numregs: 64
   pedestals_blocks: 32
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
@@ -287,15 +287,15 @@
       value: false
     ext_en:
       address: 0x0B
       bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: false
     exttrig:
       address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
@@ -565,15 +565,15 @@
       description: ''
       readwrite: rw
       value: false
     trigger_mux:
       address: 0x22
       bitposition: 5
       bitwidth: 4
-      description: 'Change which trigger type is used to trigger the chip, there are 8 diffeerent modes.'
+      description: 'Change which trigger type is used to trigger the chip, there are 9 different modes.'
       readwrite: rw
       value: 8
     windsel:
       address: 0x07
       bitposition: 0
       bitwidth: 8
       description: ''
@@ -717,34 +717,34 @@
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
     response0:
-      address: 0x2C
+      address: 0x48
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x2D
+      address: 0x49
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x2E
+      address: 0x4A
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x2F
+      address: 0x4B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
   possible_bauds:
     115200: 868
     2000000: 50
     # 691200: 8
     # 1041667: 5
   resolution: 12
   samples: 32
-  samplingrate: 1000000000
+  samplingrate: 1.0
   stop_word: FA5A
   register_stop_word: CAFE
   tia_dac:
     max_vref: 2500
     min_vref: 0
     ref_bits: 4
     val_bits: 8
```

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/hiper.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/hiper.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/hiper_fmc.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/oleas_box2.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/siread.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/trbhm.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/upac32.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/upac96.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/upaci.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/data/registers/zdigitizer.yml` & `naluconfigs-11.1.1/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/exceptions.py` & `naluconfigs-11.1.1/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/helpers.py` & `naluconfigs-11.1.1/src/naluconfigs/helpers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs/postprocess.py` & `naluconfigs-11.1.1/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-11.1.1/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.1.0
+Version: 11.1.1
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.1.0/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-11.1.1/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/naluconfigs/postprocess.py
 src/naluconfigs.egg-info/PKG-INFO
 src/naluconfigs.egg-info/SOURCES.txt
 src/naluconfigs.egg-info/dependency_links.txt
 src/naluconfigs.egg-info/requires.txt
 src/naluconfigs.egg-info/top_level.txt
 src/naluconfigs/data/chips/aardvarcv3.yml
+src/naluconfigs/data/chips/aardvarcv4.yml
 src/naluconfigs/data/chips/aodsv1.yml
 src/naluconfigs/data/chips/aodsv2.yml
 src/naluconfigs/data/chips/asocv3.yml
 src/naluconfigs/data/chips/hdsocv1.yml
 src/naluconfigs/data/chips/udc16.yml
 src/naluconfigs/data/clocks/AODS_300GCC.txt
 src/naluconfigs/data/clocks/AODS_8M.txt
@@ -39,14 +40,15 @@
 src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
 src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
 src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
 src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
 src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
 src/naluconfigs/data/registers/aardvarcv2.yml
 src/naluconfigs/data/registers/aardvarcv3.yml
+src/naluconfigs/data/registers/aardvarcv3_gbe.yml
 src/naluconfigs/data/registers/aardvarcv4.yml
 src/naluconfigs/data/registers/aodsoc_aods.yml
 src/naluconfigs/data/registers/aodsoc_asoc.yml
 src/naluconfigs/data/registers/aodsv1.yml
 src/naluconfigs/data/registers/aodsv2_eval.yml
 src/naluconfigs/data/registers/asoc.yml
 src/naluconfigs/data/registers/asocv2.yml
```

### Comparing `naluconfigs-11.1.0/tests/test_hex_addr_converter.py` & `naluconfigs-11.1.1/tests/test_hex_addr_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 import os
+import subprocess
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-import subprocess
 
 import naluconfigs
-from naluconfigs import get_configuration_from_file, get_available_models, get_register_file
+from naluconfigs import (
+    get_available_models,
+    get_configuration_from_file,
+    get_register_file,
+)
+
 
 def test_hex_addr_converter():
     """Tests conversion of converting register addresses to
     hex literals
     """
-    SCRIPT_PATH = Path(naluconfigs.__file__).parent.parent / "scripts" / "hex_addr_converter.py"
+    SCRIPT_PATH = (
+        Path(naluconfigs.__file__).parent.parent.parent
+        / "scripts"
+        / "hex_addr_converter.py"
+    )
     assert os.path.exists(SCRIPT_PATH)
     for model in get_available_models():
         file_name = get_register_file(model)
         tf = NamedTemporaryFile(delete=False)
-        
-        with open(tf.name, 'w') as temp_file:
-            cmd = f'python {SCRIPT_PATH} -i {file_name} -o {tf.name}'
+
+        with open(tf.name, "w") as temp_file:
+            cmd = f"python {SCRIPT_PATH} -i {file_name} -o {tf.name}"
             subprocess.run(cmd)
             temp_file.seek(0)
 
         config = get_configuration_from_file(file_name)
         new_config = get_configuration_from_file(tf.name)
         tf.close()
         os.unlink(tf.name)
         _convert_register_addresses_to_hex(config)
         _convert_register_addresses_to_hex(new_config)
         assert config == new_config
-        
+
+
 def _convert_register_addresses_to_hex(config: dict):
-    """Convert all register addresses to hex strings
-    """
-    for register_group in config.get('registers', {}).values():
+    """Convert all register addresses to hex strings"""
+    for register_group in config.get("registers", {}).values():
         for reg in register_group.values():
-            addr = reg['address']
+            addr = reg["address"]
             if isinstance(addr, str):
                 addr = int(addr, 16)
-            reg['address'] = addr
+            reg["address"] = addr
```

### Comparing `naluconfigs-11.1.0/tests/test_i2c_registers.py` & `naluconfigs-11.1.1/tests/test_i2c_registers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from ast import Assert
 import pytest
 
-from naluconfigs import get_configuration, get_available_models
+from naluconfigs import get_available_models, get_configuration
 
-
-EXCLUDE_MODELS = [
-    'asoc'
-]
+EXCLUDE_MODELS = ["asoc"]
 
 
 @pytest.fixture
 def all_configs() -> dict:
-    """Dict of {model: config} for all boards supporting I2C
-    """
+    """Dict of {model: config} for all boards supporting I2C"""
     configs = {}
     models = get_available_models()
     for model in models:
         config = get_configuration(model)
         if model in EXCLUDE_MODELS:
             continue
-        if 'i2c_registers' in config['registers']:
+        if "i2c_registers" in config["registers"]:
             configs[model] = config
     return configs
 
 
 def test_i2c_response_addrs(all_configs: dict):
     """Make sure all the response registers have the correct
     addresses. Addresses should be NGPR+8 to NGPR+11.
     """
     for model, config in all_configs.items():
-        i2c_regs = config['registers']['i2c_registers']
-        ngpr = config['params']['numregs'] # numregs is NGPR
+        i2c_regs = config["registers"]["i2c_registers"]
+        ngpr = config["params"]["numregs"]  # numregs is NGPR
 
-        for i, offset in enumerate(range(8, 12)): # NGPR+8 to NGPR+11
-            reg_addr = i2c_regs[f'response{i}']['address']
+        offset = 8
+        if model in ["upac96"]:  # defined differently in the UPAC96 firmware
+            offset = 0
+
+        for i, offset in enumerate(range(offset, offset + 4)):
+            reg_addr = i2c_regs[f"response{i}"]["address"]
             expected = ngpr + offset
 
             try:
                 assert reg_addr == expected
             except AssertionError as e:
-                raise AssertionError(f'Wrong response address for {model}') from e
+                raise AssertionError(f"Wrong response address for {model}") from e
 
 
 def test_reg_existence(all_configs):
     """Tests for the existence of expected in registers in all
     boards that support I2C.
     """
     needed_regs = [
-        'i2c_en',
-        'i2c_addr',
-        'i2c_words',
-        *[f'i2c_data{i}' for i in range(4)],
-        *[f'response{i}' for i in range(4)],
+        "i2c_en",
+        "i2c_addr",
+        "i2c_words",
+        *[f"i2c_data{i}" for i in range(4)],
+        *[f"response{i}" for i in range(4)],
     ]
     for model, config in all_configs.items():
-        i2c_regs = config['registers']['i2c_registers']
+        i2c_regs = config["registers"]["i2c_registers"]
 
         for regname in needed_regs:
             try:
                 assert regname in i2c_regs
             except AssertionError as e:
-                raise AssertionError(f'Missing register for {model}') from e
+                raise AssertionError(f"Missing register for {model}") from e
 
 
 def test_for_segmented_registers(all_configs):
     """Tests for the existence of register addresses on the FPGA that are split
     between control and i2c registers (BAD!). This is important because writing to i2c
     registers on such addresses will set all control registers on the same address
     to zero.
     """
     for model, config in all_configs.items():
-        control_reg_addresses = set([
-            _get_register_addr(reg)
-            for reg in config['registers']['control_registers'].values()
-        ])
-        for name, i2c_reg in config['registers']['i2c_registers'].items():
+        control_reg_addresses = set(
+            [
+                _get_register_addr(reg)
+                for reg in config["registers"]["control_registers"].values()
+            ]
+        )
+        for name, i2c_reg in config["registers"]["i2c_registers"].items():
             i2c_reg_addr = _get_register_addr(i2c_reg)
             try:
                 assert i2c_reg_addr not in control_reg_addresses
             except AssertionError:
                 raise AssertionError(
-                    f'I2C register {name} for {model} shares address 0x{i2c_reg_addr:02x} with one or more control registers'
+                    f"I2C register {name} for {model} shares address 0x{i2c_reg_addr:02x} with one or more control registers"
                 )
 
 
 def _get_register_addr(reg: dict) -> int:
-    """Get the address from for a register as an int.
-    """
-    addr = reg['address']
+    """Get the address from for a register as an int."""
+    addr = reg["address"]
     if isinstance(addr, str):
-        addr = int(reg['address'], 16)
+        addr = int(reg["address"], 16)
     return addr
```

### Comparing `naluconfigs-11.1.0/tests/test_multichip.py` & `naluconfigs-11.1.1/tests/test_multichip.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/tests/test_post_processing.py` & `naluconfigs-11.1.1/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.0/tests/test_range_keys.py` & `naluconfigs-11.1.1/tests/test_range_keys.py`

 * *Files identical despite different names*

