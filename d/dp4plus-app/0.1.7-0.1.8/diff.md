# Comparing `tmp/dp4plus_app-0.1.7.tar.gz` & `tmp/dp4plus_app-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp4plus_app-0.1.7.tar", last modified: Thu Jun  1 18:31:46 2023, max compression
+gzip compressed data, was "dp4plus_app-0.1.8.tar", last modified: Tue Jun 13 14:01:12 2023, max compression
```

## Comparing `dp4plus_app-0.1.7.tar` & `dp4plus_app-0.1.8.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:46.958386 dp4plus_app-0.1.7/
--rw-rw-rw-   0        0        0     1092 2023-03-10 18:45:01.000000 dp4plus_app-0.1.7/LICENCE
--rw-rw-rw-   0        0        0     4578 2023-06-01 18:31:46.958386 dp4plus_app-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4008 2023-06-01 16:21:20.000000 dp4plus_app-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 18:31:46.958386 dp4plus_app-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1990 2023-06-01 18:31:27.000000 dp4plus_app-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:44.942704 dp4plus_app-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:45.067708 dp4plus_app-0.1.7/src/dp4plus_app/
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:45.177087 dp4plus_app-0.1.7/src/dp4plus_app/UserGuide/
--rw-rw-rw-   0        0        0  2019530 2023-05-24 16:22:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/UserGuide/UserGuide.docx
--rw-rw-rw-   0        0        0  1000915 2023-05-24 16:22:39.000000 dp4plus_app-0.1.7/src/dp4plus_app/UserGuide/UserGuide.pdf
--rw-rw-rw-   0        0        0   765044 2023-05-31 15:25:45.000000 dp4plus_app-0.1.7/src/dp4plus_app/UserGuide/UserGuideFigures.pptx
--rw-rw-rw-   0        0        0        0 2023-03-23 20:21:29.000000 dp4plus_app-0.1.7/src/dp4plus_app/__init__.py
--rw-rw-rw-   0        0        0     9324 2023-06-01 17:42:33.000000 dp4plus_app-0.1.7/src/dp4plus_app/bugs_a_warning_module.py
--rw-rw-rw-   0        0        0     9506 2023-05-24 18:48:39.000000 dp4plus_app-0.1.7/src/dp4plus_app/correlation_module.py
--rw-rw-rw-   0        0        0    18555 2023-05-31 17:43:48.000000 dp4plus_app-0.1.7/src/dp4plus_app/custom_gui_module.py
--rw-rw-rw-   0        0        0     8550 2023-06-01 16:53:35.000000 dp4plus_app-0.1.7/src/dp4plus_app/custom_module.py
--rw-rw-rw-   0        0        0    13608 2023-06-01 17:06:25.000000 dp4plus_app-0.1.7/src/dp4plus_app/data_base_Custom.xlsx
--rw-rw-rw-   0        0        0    61121 2023-05-16 14:51:37.000000 dp4plus_app-0.1.7/src/dp4plus_app/data_base_MM.xlsx
--rw-rw-rw-   0        0        0    42509 2023-02-28 18:07:42.000000 dp4plus_app-0.1.7/src/dp4plus_app/data_base_QM.xlsx
--rw-rw-rw-   0        0        0     7269 2023-05-30 17:36:59.000000 dp4plus_app-0.1.7/src/dp4plus_app/dp4_module.py
--rw-rw-rw-   0        0        0    73188 2023-03-07 17:33:34.000000 dp4plus_app-0.1.7/src/dp4plus_app/logo_CONICET.png
--rw-rw-rw-   0        0        0    21045 2023-03-07 17:09:01.000000 dp4plus_app-0.1.7/src/dp4plus_app/logo_INGEBIO.png
--rw-rw-rw-   0        0        0     3710 2023-05-31 18:15:06.000000 dp4plus_app-0.1.7/src/dp4plus_app/main.py
--rw-rw-rw-   0        0        0    18960 2023-05-31 17:04:28.000000 dp4plus_app-0.1.7/src/dp4plus_app/main_gui_module.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:45.286463 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/
--rw-rw-rw-   0        0        0    36815 2023-05-31 14:49:36.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx
--rw-rw-rw-   0        0        0    67105 2023-03-14 13:31:40.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/custom_molecules_set.docx
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:45.536471 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/
--rw-rw-rw-   0        0        0      588 2023-03-09 17:59:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc
--rw-rw-rw-   0        0        0      529 2023-03-09 17:59:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1057 2023-03-09 17:59:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1539 2023-03-09 17:59:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1537 2023-03-15 13:03:00.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc
--rw-rw-rw-   0        0        0     1531 2023-03-09 17:59:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1530 2023-03-15 13:03:00.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc
--rw-rw-rw-   0        0        0      750 2023-03-09 17:59:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1032 2023-03-09 17:59:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1368 2023-03-09 17:59:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1372 2023-03-15 13:03:00.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc
--rw-rw-rw-   0        0        0     1374 2023-03-15 13:03:00.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc
--rw-rw-rw-   0        0        0     1384 2023-03-15 13:03:00.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc
--rw-rw-rw-   0        0        0     1716 2023-03-09 17:59:12.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1725 2023-03-15 13:03:00.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:45.864607 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/
--rw-rw-rw-   0        0        0      588 2022-10-04 14:19:04.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc
--rw-rw-rw-   0        0        0      529 2022-10-04 14:19:04.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1057 2022-10-04 14:19:04.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1539 2022-10-04 14:19:04.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1536 2022-10-04 14:19:04.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc
--rw-rw-rw-   0        0        0     1534 2022-10-04 14:19:06.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1529 2022-10-04 14:19:06.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc
--rw-rw-rw-   0        0        0      749 2022-10-04 14:19:04.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1030 2022-10-04 14:19:16.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1369 2022-10-04 14:19:08.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1372 2022-10-04 14:19:08.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc
--rw-rw-rw-   0        0        0     1376 2022-10-04 14:19:08.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc
--rw-rw-rw-   0        0        0     1382 2022-10-04 14:19:08.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc
--rw-rw-rw-   0        0        0     1712 2022-10-04 14:19:10.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1724 2022-10-04 14:19:10.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:46.942761 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/
--rw-rw-rw-   0        0        0    16107 2023-03-13 19:26:08.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a - copia.xlsx
--rw-rw-rw-   0        0        0    62190 2022-05-17 17:47:26.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62202 2022-05-17 17:59:17.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62133 2022-05-17 18:10:35.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62150 2022-05-17 18:21:10.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62411 2022-05-17 18:31:50.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62149 2022-05-17 18:42:51.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62608 2022-05-17 18:54:27.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62119 2022-05-17 19:06:23.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62121 2022-05-17 19:17:42.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-17 19:29:29.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62393 2022-05-17 19:40:13.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62174 2022-05-17 19:51:50.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62373 2022-05-17 20:02:41.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62105 2022-05-17 20:14:06.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62116 2022-05-17 20:24:59.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62115 2022-05-17 20:35:55.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62446 2022-05-17 20:46:44.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62187 2022-05-17 20:57:46.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62154 2022-05-17 21:08:39.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62493 2022-05-17 18:10:10.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62148 2022-05-17 18:40:52.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62142 2022-05-17 19:11:10.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62196 2022-05-17 19:40:30.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62042 2022-05-17 20:09:33.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62182 2022-05-17 20:38:31.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62183 2022-05-17 21:08:56.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 21:39:48.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62186 2022-05-17 22:10:41.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62172 2022-05-17 22:41:37.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62078 2022-05-17 23:14:34.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62352 2022-05-17 23:49:30.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62156 2022-05-18 00:18:50.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62159 2022-05-18 00:52:59.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-18 01:23:09.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62635 2022-05-18 01:55:00.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62125 2022-05-18 02:27:45.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62530 2022-05-18 02:58:42.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62375 2022-05-18 03:34:04.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62140 2022-05-17 18:21:07.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62059 2022-05-17 18:56:41.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    61990 2022-05-17 19:26:23.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62108 2022-05-17 19:53:58.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62035 2022-05-17 20:19:33.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62125 2022-05-17 20:47:31.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62189 2022-05-17 21:16:05.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62289 2022-05-17 21:40:37.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62204 2022-05-17 22:05:51.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62168 2022-05-17 22:33:21.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62204 2022-05-17 23:01:32.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62373 2022-05-17 23:36:01.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62132 2022-05-18 00:05:25.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62094 2022-05-18 00:41:01.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62003 2022-05-18 01:14:58.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-18 01:51:51.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62174 2022-05-18 02:25:20.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62111 2022-05-18 03:04:33.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62153 2022-05-18 03:34:21.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62159 2022-05-17 18:26:26.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62110 2022-05-17 18:32:41.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62223 2022-05-17 18:39:11.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62314 2022-05-17 18:46:00.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62290 2022-05-17 18:52:29.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 18:59:07.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62387 2022-05-17 19:05:40.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62437 2022-05-17 19:12:26.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62096 2022-05-17 19:18:31.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    66884 2022-05-17 19:25:09.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62111 2022-05-17 19:31:38.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62040 2022-05-17 19:37:41.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62317 2022-05-17 19:44:23.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 19:51:02.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62010 2022-05-17 19:57:03.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62101 2022-05-17 20:03:32.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62045 2022-05-17 20:10:05.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    63152 2022-05-17 20:16:50.000000 dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    10836 2023-06-01 16:54:02.000000 dp4plus_app-0.1.7/src/dp4plus_app/output_module.py
--rw-rw-rw-   0        0        0     5113 2023-05-24 18:48:16.000000 dp4plus_app-0.1.7/src/dp4plus_app/validation_module.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:45.130210 dp4plus_app-0.1.7/src/dp4plus_app.egg-info/
--rw-rw-rw-   0        0        0     4578 2023-06-01 18:31:44.000000 dp4plus_app-0.1.7/src/dp4plus_app.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7047 2023-06-01 18:31:44.000000 dp4plus_app-0.1.7/src/dp4plus_app.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:31:44.000000 dp4plus_app-0.1.7/src/dp4plus_app.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-06-01 18:31:44.000000 dp4plus_app-0.1.7/src/dp4plus_app.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-06-01 18:31:44.000000 dp4plus_app-0.1.7/src/dp4plus_app.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-01 18:31:44.000000 dp4plus_app-0.1.7/src/dp4plus_app.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 14:01:12.228048 dp4plus_app-0.1.8/
+-rw-rw-rw-   0        0        0     1092 2023-03-10 18:45:01.000000 dp4plus_app-0.1.8/LICENCE
+-rw-rw-rw-   0        0        0     7497 2023-06-13 14:01:12.228048 dp4plus_app-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6903 2023-06-13 13:58:55.000000 dp4plus_app-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 14:01:12.228048 dp4plus_app-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1990 2023-06-13 13:59:20.000000 dp4plus_app-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.009713 dp4plus_app-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.447221 dp4plus_app-0.1.8/src/dp4plus_app/
+drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.650350 dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/
+-rw-rw-rw-   0        0        0  1983578 2023-06-05 16:41:59.000000 dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuide.docx
+-rw-rw-rw-   0        0        0  2040794 2023-06-05 16:42:18.000000 dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuide.pdf
+-rw-rw-rw-   0        0        0   765044 2023-05-31 15:25:45.000000 dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuideFigures.pptx
+-rw-rw-rw-   0        0        0        0 2023-03-23 20:21:29.000000 dp4plus_app-0.1.8/src/dp4plus_app/__init__.py
+-rw-rw-rw-   0        0        0     9508 2023-06-02 17:21:15.000000 dp4plus_app-0.1.8/src/dp4plus_app/bugs_a_warning_module.py
+-rw-rw-rw-   0        0        0     9896 2023-06-07 19:08:21.000000 dp4plus_app-0.1.8/src/dp4plus_app/correlation_module.py
+-rw-rw-rw-   0        0        0    19040 2023-06-02 19:18:30.000000 dp4plus_app-0.1.8/src/dp4plus_app/custom_gui_module.py
+-rw-rw-rw-   0        0        0     8702 2023-06-02 17:39:19.000000 dp4plus_app-0.1.8/src/dp4plus_app/custom_module.py
+-rw-rw-rw-   0        0        0    13608 2023-06-01 17:06:25.000000 dp4plus_app-0.1.8/src/dp4plus_app/data_base_Custom.xlsx
+-rw-rw-rw-   0        0        0    61121 2023-05-16 14:51:37.000000 dp4plus_app-0.1.8/src/dp4plus_app/data_base_MM.xlsx
+-rw-rw-rw-   0        0        0    42509 2023-02-28 18:07:42.000000 dp4plus_app-0.1.8/src/dp4plus_app/data_base_QM.xlsx
+-rw-rw-rw-   0        0        0     7269 2023-05-30 17:36:59.000000 dp4plus_app-0.1.8/src/dp4plus_app/dp4_module.py
+-rw-rw-rw-   0        0        0    73188 2023-03-07 17:33:34.000000 dp4plus_app-0.1.8/src/dp4plus_app/logo_CONICET.png
+-rw-rw-rw-   0        0        0    21045 2023-03-07 17:09:01.000000 dp4plus_app-0.1.8/src/dp4plus_app/logo_INGEBIO.png
+-rw-rw-rw-   0        0        0     3710 2023-05-31 18:15:06.000000 dp4plus_app-0.1.8/src/dp4plus_app/main.py
+-rw-rw-rw-   0        0        0    19424 2023-06-02 19:17:37.000000 dp4plus_app-0.1.8/src/dp4plus_app/main_gui_module.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.712852 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/
+-rw-rw-rw-   0        0        0    36815 2023-05-31 14:49:36.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx
+-rw-rw-rw-   0        0        0    67105 2023-03-14 13:31:40.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/custom_molecules_set.docx
+drwxrwxrwx   0        0        0        0 2023-06-13 14:01:10.009734 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/
+-rw-rw-rw-   0        0        0      588 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc
+-rw-rw-rw-   0        0        0      529 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1057 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1539 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1537 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0     1531 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1530 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0      750 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1032 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1368 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1372 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0     1374 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc
+-rw-rw-rw-   0        0        0     1384 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc
+-rw-rw-rw-   0        0        0     1716 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1725 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc
+drwxrwxrwx   0        0        0        0 2023-06-13 14:01:10.400369 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/
+-rw-rw-rw-   0        0        0      588 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc
+-rw-rw-rw-   0        0        0      529 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1057 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1539 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1536 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0     1534 2022-10-04 14:19:06.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1529 2022-10-04 14:19:06.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0      749 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1030 2022-10-04 14:19:16.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1369 2022-10-04 14:19:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1372 2022-10-04 14:19:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0     1376 2022-10-04 14:19:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc
+-rw-rw-rw-   0        0        0     1382 2022-10-04 14:19:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc
+-rw-rw-rw-   0        0        0     1712 2022-10-04 14:19:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1724 2022-10-04 14:19:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc
+drwxrwxrwx   0        0        0        0 2023-06-13 14:01:12.212422 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/
+-rw-rw-rw-   0        0        0    16107 2023-03-13 19:26:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a - copia.xlsx
+-rw-rw-rw-   0        0        0    62190 2022-05-17 17:47:26.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62202 2022-05-17 17:59:17.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62133 2022-05-17 18:10:35.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62150 2022-05-17 18:21:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62411 2022-05-17 18:31:50.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62149 2022-05-17 18:42:51.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62608 2022-05-17 18:54:27.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62119 2022-05-17 19:06:23.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62121 2022-05-17 19:17:42.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-17 19:29:29.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62393 2022-05-17 19:40:13.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62174 2022-05-17 19:51:50.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62373 2022-05-17 20:02:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62105 2022-05-17 20:14:06.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62116 2022-05-17 20:24:59.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62115 2022-05-17 20:35:55.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62446 2022-05-17 20:46:44.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62187 2022-05-17 20:57:46.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62154 2022-05-17 21:08:39.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62493 2022-05-17 18:10:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62148 2022-05-17 18:40:52.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62142 2022-05-17 19:11:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62196 2022-05-17 19:40:30.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62042 2022-05-17 20:09:33.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62182 2022-05-17 20:38:31.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62183 2022-05-17 21:08:56.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 21:39:48.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62186 2022-05-17 22:10:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62172 2022-05-17 22:41:37.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62078 2022-05-17 23:14:34.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62352 2022-05-17 23:49:30.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62156 2022-05-18 00:18:50.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62159 2022-05-18 00:52:59.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-18 01:23:09.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62635 2022-05-18 01:55:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62125 2022-05-18 02:27:45.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62530 2022-05-18 02:58:42.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62375 2022-05-18 03:34:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62140 2022-05-17 18:21:07.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62059 2022-05-17 18:56:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    61990 2022-05-17 19:26:23.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62108 2022-05-17 19:53:58.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62035 2022-05-17 20:19:33.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62125 2022-05-17 20:47:31.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62189 2022-05-17 21:16:05.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62289 2022-05-17 21:40:37.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62204 2022-05-17 22:05:51.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62168 2022-05-17 22:33:21.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62204 2022-05-17 23:01:32.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62373 2022-05-17 23:36:01.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62132 2022-05-18 00:05:25.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62094 2022-05-18 00:41:01.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62003 2022-05-18 01:14:58.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-18 01:51:51.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62174 2022-05-18 02:25:20.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62111 2022-05-18 03:04:33.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62153 2022-05-18 03:34:21.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62159 2022-05-17 18:26:26.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62110 2022-05-17 18:32:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62223 2022-05-17 18:39:11.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62314 2022-05-17 18:46:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62290 2022-05-17 18:52:29.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 18:59:07.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62387 2022-05-17 19:05:40.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62437 2022-05-17 19:12:26.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62096 2022-05-17 19:18:31.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    66884 2022-05-17 19:25:09.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62111 2022-05-17 19:31:38.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62040 2022-05-17 19:37:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62317 2022-05-17 19:44:23.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 19:51:02.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62010 2022-05-17 19:57:03.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62101 2022-05-17 20:03:32.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62045 2022-05-17 20:10:05.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    63152 2022-05-17 20:16:50.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    10836 2023-06-01 16:54:02.000000 dp4plus_app-0.1.8/src/dp4plus_app/output_module.py
+-rw-rw-rw-   0        0        0     5375 2023-06-02 17:47:02.000000 dp4plus_app-0.1.8/src/dp4plus_app/validation_module.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.494098 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/
+-rw-rw-rw-   0        0        0     7497 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7047 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/top_level.txt
```

### Comparing `dp4plus_app-0.1.7/LICENCE` & `dp4plus_app-0.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/setup.py` & `dp4plus_app-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md') as file:         #sirve para incluir el REEDME
     long_description = file.read()
 
 short_description = 'A tool to simplify your DP4+ calculations'
 
 setup(
     name='dp4plus_app',
-    version='0.1.7',
+    version='0.1.8',
     
     author='Bruno A. Franco',
     author_email='bruno.agustin.franco@gmail.com',
     url='https://github.com/RosarioCCLab/DP4plus-App',
     description =short_description	,
     long_description = long_description,
     long_description_content_type ="text/markdown",
```

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/UserGuide/UserGuide.docx` & `dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuide.docx`

 * *Files 11% similar despite different names*

#### docx2txt

```diff
@@ -1,48 +1,54 @@
                                    DP4+ App
                      https://github.com/Sarotti-Lab/ . . .
                          sarotti@iquir-conicet.gov.ar
               Instructive, general recommendations and case study
 Content
 Overview and usage recommendations	1
-Probability calculations: DP4+, MM-DP4+ and Custom-DP4+	2
+Probability calculations: DP4+, MM-DP4+ and Custom-DP4+	1
 Prepare your files	2
-Perform a calculation	3
+Perform a calculation	4
 Results output	4
-Reparametrization: Custom-DP4+	5
-Create a new level	5
+Reparametrization: Custom-DP4+	6
+Create a new level	6
 Update a level	7
-Warnings and Input Control	7
-Questionable values	7
-Gaussian calculation files	8
-Data spreadsheet	8
-Malfunctions report	9
+Warnings and Input control	8
+Questionable values	8
+Gaussian calculation files	9
+Data spreadsheet	9
+Malfunctions report	10
 
 Overview and usage recommendations
-DP4+ App is an integrated software capable of performing already parameterized DP4+ and MM-DP4+ calculations. Furthermore, Custom-DP4+ calculations can be performed, where any level of theory required can be parameterized. Its friendly graphical interface allows easy manipulation of multiple Gaussian calculations and automatic information processing to perform the probabilistic calculus.  
-To use the application, it is only necessary to create a folder that contains the following files:
- Well-labeled Gaussian output files, from NMR calculations, of all conformers for all isomeric candidates.
- An Excel file with the experimental information and the correlation labels of each nucleus with the Gaussian calculations.
-The recommendations below should be followed for the optimal use of the program:
- Despite DP4+ App can handle any amount of isomers, keeping the number of candidates to a minimum has several advantages, as it reduces both the overall computational cost and the probability that the calculated data for an incorrect isomer ends up having a better fit with the experimental values than the correct candidate.
- The conformational search should provide a good description of the conformational landscape of the system under study. Improper computational work might lead to potentially negative consequences in the overall results. Systematic sampling is always recommended, but impractical in highly flexible molecules. In those cases, stochastic searches using a reasonably large number of steps should be carried out. All conformations within a safe energy window from the corresponding global minimum should be kept to avoid missing potentially relevant conformations. We recommend a 10 kcal/mol cutoff value for this application using the MMFF force field.
- It is important to respect the suggested theory levels since DP4+ and MM-DP4+ were optimized for those levels. If the desired theory level is not parameterized, you can generate your own level following the instructions of the Custom-DP4+ method.
- Using unassigned or misassigned NMR data can lead to erroneous results. The chemical shifts of equivalent nuclei that show fast interconversion should be averaged (such as the case of methyl groups, or some methylene groups). Treating the signal of each proton independently is wrong (for example, computing three different chemical shifts for the same methyl group). Another problem arises when dealing with diastereotopic methylene protons, which are often arbitrarily correlated. Unless the discrimination of both signals as pro-R and pro-S is made using additional NMR information (such as NOE or J coupling), the most convenient way to tackle this issue is to treat them as interchangeable signals. Follow the instructions to learn how to deal with these issues. 
+The DP4+ App is a comprehensive software designed to perform parameterized DP4+ and MM-DP4+ calculations seamlessly. Additionally, it offers the capability to conduct Custom-DP4+ calculations, allowing users to parameterize any required level of theory. With its friendly graphical interface, users can easily manage multiple Gaussian calculations and automate information processing for probabilistic calculations.
+To get started with the application, simply create a folder and ensure that it contains the following files:
+        Well-labeled Gaussian output files: These files should include NMR calculations for all conformers of each isomeric candidate. Make sure to label them appropriately for easy identification.
+        Excel file with experimental information: This file should contain the necessary experimental data along with the correlation labels for each nucleus corresponding to the Gaussian calculations.
+By providing these files, the DP4+ App can efficiently process the information and perform the desired calculations.
+
+To ensure optimal use of the program, it is recommended to follow the guidelines below:
+ Minimize the number of candidates: While the DP4+ App can handle any number of isomers, keeping the candidate count to a minimum offers several advantages. It reduces both the overall computational cost and the risk of calculated data for an incorrect isomer yielding a better fit with experimental values compared to the correct candidate.
+ Conduct a thorough conformational search: It is essential to obtain an accurate depiction of the conformational landscape of the system under study. Care should be taken to avoid improper computational work that could potentially affect the overall results. Systematic sampling is always recommended, but in the case of highly flexible molecules, stochastic searches with a reasonably large number of steps should be carried out. All conformations within a safe energy window from the corresponding global minimum should be retained to avoid missing potentially significant conformations. For this application, it is advised to use a 10 kcal/mol cutoff value, employing the MMFF force field.
+ Adhere to the suggested theory levels: It is important to use the recommended theory levels since DP4+ and MM-DP4+ were optimized for these levels. If the desired theory level is not parameterized, you have the option to generate your own level by following the instructions provided in the Custom-DP4+ method.
+ Ensure correct assignment of NMR data: The use of unassigned or misassigned NMR data can lead to erroneous results. When dealing with equivalent nuclei that undergo fast interconversion (e.g., methyl or methylene groups), it is necessary to average the chemical shifts. Treating each proton signal independently, such as computing different chemical shifts for the same methyl group, is incorrect. Additionally, diastereotopic methylene protons often pose challenges with arbitrary correlation. Unless additional NMR information, such as NOE or J coupling, is available to discriminate between the pro-R and pro-S signals, the most suitable approach is to treat them as interchangeable signals. Detailed instructions are provided to assist you in addressing these issues effectively.
 Probability calculations: DP4+, MM-DP4+ and Custom-DP4+
 Prepare your files 
-To run a correlation calculus, DP4+ App needs the selection of a working directory and an Excel file. The program has a series of controls to ensure correct data entry. 
-The Excel file (.xlsx) must contain the information in the "shifts" sheet. This will be the only sheet read by the program and must have the structure defined in Figure 1 (see Warnings and Input control). The column headers must be the same. For isomers with the same labels, only three columns need to be used. If isomers use different labels, each candidate should have three labeling columns (label 1|label 2|label 3). The name of this document does not have any requirement, since it will be selected individually.
+To perform correlation calculations using the DP4+ App, it is essential to prepare the necessary files. The program provides a set of controls to ensure accurate data entry. Follow the guidelines below to set up your files correctly: 
+The Excel file (.xlsx) should include the information on the "shifts" sheet. This sheet will be the only one read by the program and must adhere to the structure defined in Figure 1 (refer to Warnings and Input Control). Ensure that the column headers match accordingly. For isomers with the same labels, only three columns are required. However, if isomers use different labels, each candidate should have three labeling columns (label 1 | label 2 | label 3). The name of this document does not have any specific requirements as it will be selected individually during the process.
                                        
 Figure 1. Excel sheet (experimental information and correlation labels)
-The Gaussian files must be "nmr" calculations results from Gaussian software (.log or .out). The labeling must be as follows: n_m_*_nmr.log, where n is the isomer id, m is the conformer number, and * is a user annotation. 
-The selection will be made by pressing the "Select . . ." buttons via popup windows. We strongly recommend using the given example ("Create Example" button) as a template to build your working directory.
+The Gaussian files should be the results of "nmr" calculations obtained from the Gaussian software (.log or .out files). Follow the labeling convention as follows: n_m_*_nmr.log, where:
+ "n" represents the isomer ID,
+ "m" denotes the conformer number, and
+ "*" indicates a user annotation.
+To select these files, use the "Select..." buttons, which will prompt popup windows for file selection. It is highly recommended to utilize the provided example ("Create Example" button) as a template to build your working directory effectively.
+By following these guidelines and organizing your files accordingly, you can ensure a smooth and accurate execution of the probability calculations using the DP4+ App..
                                        
 Figure 2. Entry buttons and example button
 Perform a calculation
-With DP4+ App it is possible to determine the probability of correlation at 60 already parameterized theory levels. They arise from the combination of various functionals, basis sets, and solvation modes. Of the total, 24 levels were parameterized from geometries optimized with quantum mechanics at the B3LYP/6-31G* (QM mode) and the remaining 36, through molecular mechanics with the MMFF force field (MM mode).
+With the DP4+ App, you can determine the correlation probability using 60 pre-parameterized theory levels. These levels encompass a combination of different functionals, basis sets, and solvation modes. Out of the total, 24 levels were derived from geometries optimized using quantum mechanics at the B3LYP/6-31G* level (QM mode), while the remaining 36 levels were obtained through molecular mechanics using the MMFF force field (MM mode).
 QM mode theory levels combinations 
 Functional
 B3L
 mPW1PW91
 Basis Set
 6-31G(d)
 6-31+G(d,p)
@@ -64,85 +70,88 @@
 6-31G(d,p)
 6-31+G(d,p)
 6-311+G(d,p)
 Solvatation
 GAS
 PCM (CH3Cl)
 SMD (CH3Cl)
-Although it is allowed to carry out calculations at any selected level, for a better use of DP4+ App, the program controls the coincidence between the command lines of the Gaussian files with the selected theory level. In case the levels are not matched a warning will pop up, but it will not prevent the calculus execution (figure 3).
+While it is possible to perform calculations at any selected level, for optimal utilization of the DP4+ App, the program ensures the alignment between the command lines of the Gaussian files and the selected theory level. In the event of a mismatch, a warning will appear, but it will not impede the execution of the calculation (refer to Figure 3).
                                        
 Figure 3. Modes selection and example of miss matching theory level and command lines  
-To perform calculations with a different theory level than those mentioned you must first parameterize it following the instructions of the Custom mode (next section). For this mode, the matching of the command lines is not checked automatically, but it is possible to do it yourself on the final results sheet.
+If you wish to perform calculations at a different theory level not mentioned, you must first parameterize it by following the instructions in the Custom mode (covered in the next section). In the Custom mode, the automatic validation of command line matching is not performed, but you have the ability to verify it manually on the final results sheet.
+By adhering to these guidelines, you can effectively perform calculations using the DP4+ App, ensuring compatibility between theory levels and leveraging the Custom mode for parameterizing new levels if necessary.
 Results output
-A pop-up will indicate the calculation has finished correctly and the results will be presented in an Excel file inside the selected working folder. The name of the output will correspond with the calculation mode used. 
-There will be five sheets, one with the probability results, two with the chemical shifts and two with the correlation errors. In the main sheet ("results"), you will find the probabilities of the candidates classified by their nuclei, scaling and the full version. In addition, the selected theory level, the command line of the Gaussian calculations and the automatic coincidence check are printed.
+After the completion of the calculation, a pop-up notification will confirm the successful execution, and the results will be presented in an Excel file located within the selected working folder. The name of the output file will correspond to the calculation mode utilized.
+The Excel file will consist of five sheets, each serving a specific purpose. These sheets include:
+ Probability Results: This sheet, labeled as "results," provides the probabilities of the candidates categorized by their nuclei, scaling, and the full version. It also displays the selected theory level, the command line used for the Gaussian calculations, and the automatic coincidence check.
+ Chemical Shifts: Two sheets are dedicated to displaying the chemical shifts obtained from the calculations ("d_sca" and "d_uns").
+ Correlation Errors: Similarly, two sheets are allocated for presenting the correlation errors. ("e_sca" and "e_uns").
 
 Figure 4. Output Excel file 
-In cases where the selected theory level does not coincide with the Gaussian calculation command line, it will warn about the misuse of the tool and the inconsistencies found (figure 5). 
-In Custom mode, it will be indicated that the theory level cannot be verified, and it becomes the user's responsibility to perform this verification. Additionally, below the results, the database of the Custom level used will be provided, including the standard tensors, distribution parameters, date, and parametrization method.
+In cases where the selected theory level does not align with the Gaussian calculation command line, a warning will be displayed, indicating any inconsistencies encountered (refer to Figure 5).
+In the Custom mode, it will be explicitly stated that the theory level cannot be verified automatically, and the responsibility falls upon the user to perform the necessary verification. Additionally, below the results, the database of the Custom level used will be provided, including standard tensors, distribution parameters, date, and parametrization method.
+By reviewing the comprehensive results output in the provided Excel file, users can analyze the probability results, chemical shifts, correlation errors, and ensure the appropriate utilization of the selected theory level and Custom mode if applicable.
                                        
 Figure 5. Examples of Custom mode traceability and theory level miss selection
 Reparametrization: Custom-DP4+ 
 Create a new level
-Within the Custom mode of the main window, there is the "+ new" option that will redirect you to the reparameterization module. There you have to select the parameterization mode and assign a name to your custom level. The name can only have numbers and lowercase letters (do not use special characters either).
+In the Custom mode of the main window, you have the option "+ new" which will redirect you to the reparameterization module. In this module, you need to select the parameterization mode and assign a name to your custom level. The name should only consist of numbers and lowercase letters, avoiding the use of special characters.
                                        
 Figure 6. Selection to create a new custom level and redirecting window. 
-In the case you have already parameterized a theory level, you can enter the distribution parameters and tensors of the TMS by keyboard (Figure 7.a).
-However, if you need to calculate distribution statistics, you will need to load a working directory and the corresponding Excel file in the main window. The working folder should contain the NMR calculations for all labeled conformations in the format 'n_m_nmr.log', and TMS specified as 'TMS_nmr.log'. The Excel spreadsheet should have the same number of sheets as the parametrization molecules, with each sheet named after the ID of the respective compounds. The application will automatically determine the parameters, and you can view them when using the custom level in a calculation. 
-Based on the findings presented in J. Org. Chem. 2021, 86, 12, 8544 - 8548, it is recommended to use a set of 8 molecules in Table 1 for parametrizing your theory level, as they have been tested and proven to estimate the distribution parameters accurately. To facilitate their preparation, you can download the input files for Gaussian calculations in both MM (force field MMFF) and QM (theory level B3LYP) optimization. (Figure 7.b). In the window, you can type the command line that should specify the theory level as specified by Gaussian, along with the 'nmr' calculation instruction.
+If you have already parameterized a theory level, you can manually enter the distribution parameters and tensors of the TMS (Figure 7.a) using the keyboard.
+However, if you need to calculate distribution statistics, you will need to load a working directory and the corresponding Excel file in the main window. The working folder should contain the NMR calculations for all labeled conformations in the format 'n_m_nmr.log', and the TMS calculation specified as 'TMS_nmr.log'. The Excel spreadsheet should have the same number of sheets as the parametrization molecules, with each sheet named after the ID of the respective compounds. The application will automatically determine the parameters, and you can view them when using the custom level in a calculation.
                                        
 Figure 7. a) Input parameters mode: allow to entry the values of an already parametrized level. b) Load mode: capable of automatically determine the distribution parameters using the training set calculus. Also, offers templates of the training set in QM y MM optimization.  
-The Excel file with the experimental data and the correlation labels already assigned will be provided with the Gaussian inputs. In it, the data set of each molecule is placed in a sheet with the associated ID as mentioned before. The information follows the same structure as the correlation "shifts" sheet in figure 1. 
-                                       
-                                       
-                                       
-                                       
-                                       
-                                       
-                                       
+Based on the findings presented in the article J. Org. Chem. 2021, 86, 12, 8544 - 8548, it is recommended to use the set of 8 molecules listed in Table 1 for parametrizing your theory level. These molecules have been thoroughly tested and proven to accurately estimate the distribution parameters. To facilitate their preparation, you can download the input files for Gaussian calculations in both MM (using the MMFF force field) and QM (using the B3LYP theory level) optimization (Figure 7.b). In the input window, you can specify the command line as required by Gaussian, along with the 'nmr' calculation instruction.
+The Excel file containing the experimental data and the assigned correlation labels will be provided along with the Gaussian inputs. Each molecule's data set will be placed in a sheet named after the associated ID, following the same structure as the correlation "shifts" sheet shown in Figure 1.
                                        
 Table 1. Training set molecules with experimental labels. 
-As mentioned by Sarotti (2021), it is important to consider the number of sampling points used for parameterization analysis to avoid potential inaccuracies in estimating the degrees of freedom. If a data set consists of fewer than 150 elements, a pop-up window will notify about the potential inaccuracies in fitting a t-Student distribution. This notification specifically applies to the recommended set mentioned in Table 1.
-You have two options: you can either utilize the average values from the original publication, which have been proven to yield accurate results for DP4+ type calculations or retain the actual values. If you choose to use the estimated values, it is strongly recommended to verify that the degrees of freedom (ν) in your calculations are less than 30.
+As mentioned by Sarotti (2021), it is crucial to consider the number of sampling points used for parameterization analysis to avoid potential inaccuracies in estimating the degrees of freedom. If a data set consists of fewer than 150 elements, a pop-up window will notify you about the potential inaccuracies in fitting a t-Student distribution. This notification specifically applies to the recommended set mentioned in Table 1.
+You have two options: either utilize the average values from the original publication, which have been proven to yield accurate results for DP4+ type calculations, or retain the actual values. If you choose to use the estimated values, it is strongly recommended to verify that the degrees of freedom (ν) in your calculations are less than 30.
+By following these guidelines for reparametrization in the Custom-DP4+ mode, you can create a new level and effectively determine the distribution parameters for accurate correlation calculations.
                                        
 Figure 8. Warning popup for insufficient parametrization set
 
 Update a level
-To update a level simply follow the steps in the previous section and overwrite the name of the desire custom level. A popup will warn you about the existence of that level before updating the data. You can go back and change the name if you want to keep both parametrizations (figure 8). The update can be generated in any mode, it is not necessary to use the same as the one before. 
+To update a custom level, you can follow the steps outlined in the previous section and overwrite the name of the desired custom level. When you attempt to update the data, a popup will notify you if a level with the same name already exists, allowing you to make a decision. If you wish to keep both parametrizations, you can go back and modify the name accordingly (refer to Figure 8). It is important to note that the update can be generated in any mode, and it is not necessary to use the same mode as before.
                                        
 Figure 8. Example of update/overwriting a custom level 
 Warnings and Input control
-To enhance the user's understanding of anomalous results in DP4+ type calculations, a warning system has been implemented. This system assists in interpreting and identifying any unusual outcomes. Additionally, DP4+ App includes multiple checkpoints to validate the accuracy of data entry. If any discrepancies or inconsistencies are detected that do not meet the program's requirements, it will promptly notify the user.
+To enhance the user's understanding of anomalous results in DP4+ type calculations, DP4+ App has implemented a comprehensive warning system. This system assists users in interpreting and identifying any unusual outcomes that may arise during the calculation process. Additionally, the application includes multiple checkpoints to validate the accuracy of data entry, ensuring reliable and consistent results.
 Questionable values
-Although DP4+ App can perform calculations with any given input (which follows the requested format), there are some chemical criteria that must be taken into account for a result to be valid. 
-Those calculations that do not meet the following requirements will be warned about said deviations: 
- σH > 6ppm and σC > 120ppm, not marked as sp2
+DP4+ App applies specific chemical criteria to validate the results of calculations. Any values that deviate from these criteria will trigger warnings to alert the user. The following conditions are considered questionable: 
+ σH > 6ppm and σC > 120 ppm, not marked as sp2
  σH > 14ppm, identified as 13C
  esca-H > 0.7 and esca-C > 10, related to possible miscorrelation/missed assignment
-The calculations can proceed as usual, and any warnings will be easily identifiable as highlighted cells. In the case of DP4+ type calculations, the warnings will be printed on the e_sca sheet within the results. During the parameterization process, a popup will prompt you to confirm whether you wish to proceed, and the highlights will be displayed in the input spreadsheet. 
+While these warnings indicate potential issues, the calculations can still proceed. The highlighted cells will draw attention to the questionable values, allowing the user to evaluate their significance. If possible, it is recommended to experiment with different paths and interpret the results to make informed decisions.
+For DP4+ type calculations, the warnings will be displayed on the e_sca sheet of the results. During the parameterization process, a popup will appear to confirm whether to proceed, and the input spreadsheet will show the highlighted values.
                                        
 Figure 9. Example of deviant values for parametrization method
 Gaussian calculation files
-In order to ensure the completeness of information provided by the Gaussian outputs, it is important to verify that the last line of each file indicates 'Normal Termination'. Any files where this string cannot be found will be automatically separated into a folder labeled 'Removed Files'. A popup will then allow you to choose whether you want to proceed with the calculation without those files or cancel to initiate a recalculation. 
+DP4+ App ensures the completeness of information from Gaussian calculation files by verifying the presence of the "Normal Termination" indicator in each file. If any file lacks this indicator, it will be automatically moved to a folder labeled "Removed Files." A popup will then offer the option to proceed with the calculation without those files or initiate a recalculation. 
                                        
                                        
 Figure 10. Examples of warning and input error 
 Data spreadsheet 
-The provided spreadsheet must adhere to the format shown in Figure 1, as mentioned earlier. The following checkpoints are in place for this file:
+The Excel spreadsheet provided for DP4+ App must follow a specific format, as illustrated in Figure 1. To ensure the accuracy of data entry, the program performs several checks on the spreadsheet:
 
- Column not found: If a header is missing or not found.
- Data not found: If there is missing data in the 'nuclei', 'exp_data', or 'labels' columns.
- Incorrect data:
+ Column not found: Detects missing or incorrect column headers.
+ Data not found: Identifies missing data in the 'nuclei', 'exp_data', or 'labels' columns.
+ Incorrect data: Checks for valid data types in specific columns
  For the 'nuclei' column, the data must be either 'C' or 'H'.
  For the 'exp_data' column, the data must be a numerical value.
  For the 'labels' column, the data must be an integer number.
- For the 'fos sp2' column, the data must be 'X', 'x', or '1'.
- Label index out of range: In cases where the label does not match any nuclei in the Gaussian calculation matrix.
- A different number of candidate isomers and set of labels: If there is a mismatch between the number of candidate isomers and the set of labels used.
- Mismatched diastereotopic labels: When the diastereotopic labels are not paired correctly.
+ For the 'sp2' column, the data must be 'X', 'x', or '1'.
+ Label index out of range: Alerts if a label does not match any nuclei in the Gaussian calculation matrix.
+ Mismatched diastereotopic labels: Notifies when diastereotopic labels are not paired correctly.
+ Different number of candidate isomers and set of labels: Detects inconsistencies between the number of candidate isomers and the set of labels used.
 
-If any of these situations occur, the program will be unable to perform the calculation. In such cases, you will need to correct the inconsistency before proceeding.
+If any of these situations occur, the program will be unable to proceed with the calculation. Therefore, it is essential for the user to rectify any inconsistencies before proceeding further.
 Malfunctions report
-If you find a faulty operation of DP4+ App, please report your situation in detail to the following emails:
+We strive to provide a reliable and efficient user experience with DP4+ App. However, if you encounter any malfunctions or issues while using the software, we appreciate your assistance in reporting them. By providing detailed information about the problem you encountered, you can contribute to the continuous improvement of DP4+ App.
+Please report any faulty operations or unexpected behavior to the following email addresses:
+
  brunoafranco@uca.edu.ar 
  zanardi@inv.rosario-conicet.gov.ar 
  sarotti@iquir-conicet.gov.ar 
+
+Your feedback is valuable to us, and we will make every effort to address and resolve any reported malfunctions promptly. Thank you for your cooperation in helping us enhance the functionality and performance of DP4+ App.
```

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/UserGuide/UserGuideFigures.pptx` & `dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuideFigures.pptx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/bugs_a_warning_module.py` & `dp4plus_app-0.1.8/src/dp4plus_app/bugs_a_warning_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,16 +214,21 @@
     
 def check_NormalTermination():
     '''Checks that the Gaussian calculations have finished correctly
     Those cases that "Normal Termination" is not found are removed to a 
     subfolder to continue with the calculation of DP4+.
     '''
     removed_files = False
+        
+    listing = []
+    for file in glob.glob('*'): 
+        if ('nmr' in file.casefold() and 
+            any(extention in file[-4:] for extention in ['.out','.log'])): 
+            listing.append(file)
     
-    listing=glob.glob("*.log")
     for file in listing:
         with open(file) as f:
             rline = f.readlines()
         if not " Normal termination" in rline[-1]:
             if not os.path.exists("Removed files"):
                 os.makedirs("Removed files")
```

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/correlation_module.py` & `dp4plus_app-0.1.8/src/dp4plus_app/correlation_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,19 +89,28 @@
     nucleus in the G09 order (there isn't any correlation process yet) 
     It uses an iterator to ponderate the confomers of each isomer in a 
     np.array().'''
     
     first_isom = True 
     
     for j, isom in enumerate(isomer_list):
-        files = glob.glob(f'{isom}_*.log') + glob.glob(f'{isom}_*.out')
         #generate matrix for each isomeric candidate (conf in columns)
+        files = []
+        for file in glob.glob('*'): 
+            if ('nmr' in file.casefold() and 
+                str(isom).casefold() == file.casefold().split('_')[0] and 
+                any(extention in file[-4:] for extention in ['.out','.log'])): 
+                files.append(file)
         
         if TMS: 
-            files = files = glob.glob('*tms*.log') + glob.glob('*tms*.out')
+            files = []
+            for file in glob.glob('*'): 
+                if ('tms' in file.casefold() and 
+                    any(extention in file[-4:] for extention in ['.out','.log'])): 
+                    files.append(file)
         
         energies = list()
         conf_tens, energy = get_scf_tensors(files.pop(0), energies) #1st conf for template
         isom_matrix = np.empty((conf_tens.shape[0],len(files)+1))
         isom_matrix [:,0] = conf_tens
         energies.append(energy)
```

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/custom_gui_module.py` & `dp4plus_app-0.1.8/src/dp4plus_app/custom_gui_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,24 +292,32 @@
     dir_label = tk.Label(files_frame, width=60, anchor='w')
     dir_label.grid(row=1,column=1,sticky='W', columnspan=2)
     
     molec_label = tk.Label(files_frame, text='_',
              width=60, anchor='w')
     molec_label.grid(row=2,column=1, columnspan=2, sticky="nsew")
     
-    if custom_app.direc == '':
+    if not custom_app.direc:
         dir_label['text'] = custom_app.direc = '<- Select a folder '
         return
     
     os.chdir(custom_app.direc)
     
-    if not glob.glob('*nmr*.log') + glob.glob('*nmr*.out'):
+    files = []
+    for file in glob.glob('*'): 
+        if (any(extention in file[-4:] for extention in ['.out','.log'])): 
+            files.append(file)
+    
+    if not files: 
+        dir_label['text'] = custom_app.direc ='<- G09 files not found (.log or .out). Try again'
+        return
+    elif not any('nmr' in file.casefold() for file in files):
         dir_label['text'] = custom_app.direc ='<- "_nmr" G09 files not found. Try again'
         return
-    elif not glob.glob('*TMS*.log') or not glob.glob('*tms*.log'):
+    elif not any('tms' in file.casefold() for file in files):
         dir_label['text'] = custom_app.direc ='<- TMS file not found. Try again'
         return
 
     
     dir_label['text'] = custom_app.direc[:9]+'  . . .  '+custom_app.direc[-50:]
     
     global molecule_set
@@ -317,23 +325,26 @@
     molec_label['text'] = f'Parametrization set of {cant_comp} molecules'
     return    
 
 def molecules_count():
     '''Determine the amount of molecules used for parametrization
     The files must be named by: name_ * _nmr.log 
     '''
-    files= glob.glob('*nmr*.log') + glob.glob('*nmr*.out')
-    
-    if glob.glob('*TMS*.log') or glob.glob('*tms*.log'): 
-        pop = glob.glob('*tms*.out') + glob.glob('*tms*.log')
-        try: 
-            for i in pop: 
-                files.remove(i)
-        except: pass 
-            
+    files = []
+    for file in glob.glob('*'): 
+        if ('nmr' in file.casefold() and 
+            any(extention in file[-4:] for extention in ['.out','.log'])): 
+            files.append(file)
+    
+    #takes out the TMS if its identify with "nmr" too
+    for file in glob.glob('*'): 
+        if ('nmr' in file.casefold() and 
+            'tms' in file.casefold() and 
+            any(extention in file[-4:] for extention in ['.out','.log'])): 
+            files.remove(file)
     
     molecule_set =[]
     for file in files:
         if file.split('_',1)[0] not in molecule_set:
             molecule_set.append(file.split('_',1)[0])
         else:
             continue
```

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/custom_module.py` & `dp4plus_app-0.1.8/src/dp4plus_app/custom_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,21 @@
     param.loc['Hsp3'] = st.t.fit(e_vectors['Hsp3']) 
     
     return param
 
 def get_command():
     '''saves the command line of 10% of the files used in the 
     parameterization
-    '''
-    files= glob.glob('*nmr*.log') + glob.glob('*nmr*.out')
+    '''    
+    files = []
+    for file in glob.glob('*'): 
+        if ('nmr' in file.casefold() and 
+            any(extention in file[-4:] for extention in ['.out','.log'])): 
+            files.append(file)
+    
     choose = sample(files, (len(files)//10)+1 )
     g09command =[]
     
     for file in choose: 
         with open(file,'r') as to_read: 
                 for row in to_read.readlines(): 
                     if '#' in row:
```

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/data_base_Custom.xlsx` & `dp4plus_app-0.1.8/src/dp4plus_app/data_base_Custom.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/data_base_MM.xlsx` & `dp4plus_app-0.1.8/src/dp4plus_app/data_base_MM.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/data_base_QM.xlsx` & `dp4plus_app-0.1.8/src/dp4plus_app/data_base_QM.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/dp4_module.py` & `dp4plus_app-0.1.8/src/dp4plus_app/dp4_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/logo_CONICET.png` & `dp4plus_app-0.1.8/src/dp4plus_app/logo_CONICET.png`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/logo_INGEBIO.png` & `dp4plus_app-0.1.8/src/dp4plus_app/logo_INGEBIO.png`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/main.py` & `dp4plus_app-0.1.8/src/dp4plus_app/main.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/main_gui_module.py` & `dp4plus_app-0.1.8/src/dp4plus_app/main_gui_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,22 +168,28 @@
     root.direc = filedialog.askdirectory(title='Select directory')
     
     tk.Label(root,text='\n   \n', width=60, height=15 ).place(x=145,y=120)
     
     singboard = tk.Label(root, text='')
     singboard.place(x=148,y=115)
     
-    if root.direc == '':
+    if not root.direc:
         singboard.config( text='<- Select a folder                                     ')
         button_run['state'] = 'disable'
         return
     
     os.chdir(root.direc)
     
-    if not glob.glob('*nmr*.log') + glob.glob('*nmr*.out'):
+    files = []
+    for file in glob.glob('*'): 
+        if ('nmr' in file.casefold() and 
+            any(extention in file[-4:] for extention in ['.out','.log'])): 
+            files.append(file)
+    
+    if not files:
         singboard.config( text='"_nmr" G09 files not found. Try again')
         button_run['state'] = 'disable'
         return
     
     sing = root.direc[:9]+'  . . .  '+root.direc[-50:]
     singboard.config( text=sing)
     
@@ -353,16 +359,22 @@
                    mode_ddl, func_ddl, base_ddl, solv_ddl]:
         button['state']='disabled'
         
     return 
 
 def isomer_count():
     '''Determine the amount of isomeric candidates to be evaluated
-    The files must be named by: isomerID_ * .log '''
-    files= glob.glob('*nmr*.log') + glob.glob('*nmr*.out')
+    The files must be named by: isomerID_ * .log 
+    '''    
+    files = []
+    for file in glob.glob('*'): 
+        if ('nmr' in file.casefold() and 
+            any(extention in file[-4:] for extention in ['.out','.log'])): 
+            files.append(file)
+    
     isomer_list =[]
     for file in files:
         if file.split('_',1)[0] not in isomer_list:
             isomer_list.append(file.split('_',1)[0])
         else:
             continue
     isomer_list.sort() ##RG
@@ -371,15 +383,19 @@
 
 def thlev_id():
     '''It chooses 10% random files and check if the user theory level input
     match the G09 calcs command lines. 
     First assumption is there are no mistakes (wanr is empty). If 
     inconsistencies are found the appropiate warning is added to the list.
     '''
-    files= glob.glob('*nmr*.log') + glob.glob('*nmr*.out')
+    files = []
+    for file in glob.glob('*'): 
+        if ('nmr' in file.casefold() and 
+            any(extention in file[-4:] for extention in ['.out','.log'])): 
+            files.append(file)
     
     choose = sample(files, (len(files)//10)+1 )
     
     singboard = tk.Label(root, text='')
     singboard.place(x=160,y=160)    
     
     global warn, G09command
```

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/custom_molecules_set.docx` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/custom_molecules_set.docx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a - copia.xlsx` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a - copia.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/output_module.py` & `dp4plus_app-0.1.8/src/dp4plus_app/output_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app/validation_module.py` & `dp4plus_app-0.1.8/src/dp4plus_app/validation_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,16 +90,22 @@
         
         parameters = pd.read_excel(data_base,sheet_name=inputs['the_lev'],index_col=0)
         
         
         ### ACÁ SE MODIFICA CON UN ITERADOR PARA CADA XLSX --------------------
         def isomer_count(number):
             '''Determine the amount of isomeric candidates to be evaluated
-            The files must be named by: isomerID_ * .log '''
-            files= glob.glob(f'{number}*.log') + glob.glob(f'{number}*.out')
+            The files must be named by: isomerID_ * .log '''         
+            files = []
+            for file in glob.glob('*'): 
+                if ('nmr' in file.casefold() and 
+                    str(number).casefold() in file.casefold() and
+                    any(extention in file[-4:] for extention in ['.out','.log'])): 
+                    files.append(file)
+            
             isomer_list =[]
             for file in files:
                 if file.split('_',1)[0] not in isomer_list:
                     isomer_list.append(file.split('_',1)[0])
                 else:
                     continue
             isomer_list.sort() ##RG
@@ -110,15 +116,15 @@
         
         
         di = os.path.split(inputs['xlsx'])[0]
         
         level = os.getcwd()
         level = os.path.split(level)[-1]
         
-        files = glob.glob(di+'\\*.xlsx')
+        files = glob.glob('*.xlsx', root_dir=di)
         files = [file for file in files if not '~$' in file]
 
         for file in files:             
             inputs['xlsx'] = file
             correct = os.path.split(file)[-1]
             correct = correct.split('_')[0]
             inputs['isom'] = isomer_count(correct[:-1])
```

### Comparing `dp4plus_app-0.1.7/src/dp4plus_app.egg-info/SOURCES.txt` & `dp4plus_app-0.1.8/src/dp4plus_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

