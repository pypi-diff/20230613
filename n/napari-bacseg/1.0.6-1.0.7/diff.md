# Comparing `tmp/napari-bacseg-1.0.6.tar.gz` & `tmp/napari-bacseg-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-bacseg-1.0.6.tar", last modified: Sat May  6 06:44:33 2023, max compression
+gzip compressed data, was "napari-bacseg-1.0.7.tar", last modified: Tue Jun 13 16:26:18 2023, max compression
```

## Comparing `napari-bacseg-1.0.6.tar` & `napari-bacseg-1.0.7.tar`

### file list

```diff
@@ -1,118 +1,120 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.572559 napari-bacseg-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.211103 napari-bacseg-1.0.6/.github/
-drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.234044 napari-bacseg-1.0.6/.github/workflows/
--rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.6/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.240028 napari-bacseg-1.0.6/.napari-hub/
--rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/.napari-hub/DESCRIPTION.md
--rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/.napari-hub/config.yml
--rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.6/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4732 2023-05-06 06:44:33.573557 napari-bacseg-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/README.md
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/bacseg_ui.py
--rw-rw-rw-   0        0        0      988 2023-05-06 06:42:46.000000 napari-bacseg-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     2035 2023-05-06 06:44:33.576549 napari-bacseg-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.213098 napari-bacseg-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.478899 napari-bacseg-1.0.6/src/_dev/
--rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.6/src/_dev/Export Masks to AKSEG v5 dev.py
--rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.6/src/_dev/ScanR dev.py
--rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.6/src/_dev/Troodos dev.py
--rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.6/src/_dev/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.6/src/_dev/akseg_db_stats.py
--rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/akseg_dev.py
--rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/akseg_dev2.py
--rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.6/src/_dev/akseg_txt_metadata.py
--rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/align_alex_datadump.py
--rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/alison_datadump.py
--rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.6/src/_dev/autocontast_dev.py
--rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/cellposedev.py
--rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.6/src/_dev/cellposeshapely.py
--rw-rw-rw-   0        0        0     1279 2023-03-27 16:45:42.000000 napari-bacseg-1.0.6/src/_dev/chatGPT_midlines.py
--rw-rw-rw-   0        0        0     6105 2023-05-05 10:49:23.000000 napari-bacseg-1.0.6/src/_dev/check_AluGasketv12_DFP.py
--rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/check_metadata.py
--rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.6/src/_dev/colicoords_cellldist_dev.py
--rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.6/src/_dev/colicoords_ldist_dev.py
--rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.6/src/_dev/database_dev.py
--rw-rw-rw-   0        0        0     1023 2023-03-23 14:05:20.000000 napari-bacseg-1.0.6/src/_dev/deepsegmattest.py
--rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.6/src/_dev/edit_database_columns.py
--rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.6/src/_dev/fits_dev.py
--rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/fix_alison_missing_file_list.py
--rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/generate_scanr_movie.py
--rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/get_akseg_stats.py
--rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.6/src/_dev/get_species_info.py
--rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/luke__script.py
--rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.6/src/_dev/matplotlib_Events.py
--rw-rw-rw-   0        0        0    40825 2023-03-22 17:47:52.000000 napari-bacseg-1.0.6/src/_dev/move_AluGasketDFP.py
--rw-rw-rw-   0        0        0    44028 2023-04-04 10:28:53.000000 napari-bacseg-1.0.6/src/_dev/move_AluGasketDFP_poster.py
--rw-rw-rw-   0        0        0    48241 2023-04-26 15:22:38.000000 napari-bacseg-1.0.6/src/_dev/move_AluGasketv12_DFP.py
--rw-rw-rw-   0        0        0    46551 2023-05-05 08:15:07.000000 napari-bacseg-1.0.6/src/_dev/move_AluGasketv12_DFP_Titration.py
--rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.6/src/_dev/move_conor_nim_dfp_data.py
--rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.6/src/_dev/move_pillar_data.py
--rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/move_pillar_zstack_data.py
--rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.6/src/_dev/move_unlearning_files.py
--rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.6/src/_dev/new_metadata2.pickle.py
--rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.6/src/_dev/new_read_akseg_directory.py
--rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/nim_dev.py
--rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/omnipose_dev.py
--rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.6/src/_dev/omnipose_midlines.py
--rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.6/src/_dev/omnipose_train.py
--rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.6/src/_dev/oufti_dilate.py
--rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.6/src/_dev/oufti_dilate_with_midlines.py
--rw-rw-rw-   0        0        0     4449 2023-05-04 09:42:23.000000 napari-bacseg-1.0.6/src/_dev/pandas_speed.py
--rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/process_alex_datadump.py
--rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/process_alex_datadump_clinical.py
--rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/process_conor_datadump.py
--rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/process_gramstain_datadump.py
--rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.6/src/_dev/read_non_tif.py
--rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/rebuild_usermeta.py
--rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/rebuild_usermeta_2.py
--rw-rw-rw-   0        0        0     3034 2023-03-23 13:58:59.000000 napari-bacseg-1.0.6/src/_dev/recreate_user_metadata.py
--rw-rw-rw-   0        0        0     2117 2023-04-20 14:14:30.000000 napari-bacseg-1.0.6/src/_dev/scalebar_dev.py
--rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/sort_midlines.py
--rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/stelios_stats.py
--rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/tile_meta_check.py
--rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.6/src/_dev/tiler_dev.py
--rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.6/src/_dev/updade_akseg_metadata.py
--rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.6/src/_dev/update_img_metadata.py
--rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/video_iamges.py
--rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.6/src/_dev/zooniverse.py
--rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_move.py
--rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_move_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_titration_upload.py
--rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_upload.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.544724 napari-bacseg-1.0.6/src/napari_bacseg/
--rw-rw-rw-   0        0        0      155 2023-05-06 06:42:46.000000 napari-bacseg-1.0.6/src/napari_bacseg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.571563 napari-bacseg-1.0.6/src/napari_bacseg/_tests/
--rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/src/napari_bacseg/_tests/__init__.py
--rw-rw-rw-   0        0        0    26398 2023-05-03 08:53:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_tests/test_bacseg.py
--rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_tests/test_widget.py
--rw-rw-rw-   0        0        0    88965 2023-05-06 06:32:34.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils.py
--rw-rw-rw-   0        0        0    13550 2023-04-21 11:56:56.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_cellpose.py
--rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_colicoords.py
--rw-rw-rw-   0        0        0    20495 2023-05-03 08:53:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_database.py
--rw-rw-rw-   0        0        0    46793 2023-05-06 06:37:46.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_database_IO.py
--rw-rw-rw-   0        0        0     1645 2023-03-09 18:16:07.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_imagej.py
--rw-rw-rw-   0        0        0    37022 2023-05-06 06:32:34.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_interface_events.py
--rw-rw-rw-   0        0        0     4279 2023-05-03 08:53:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_json.py
--rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_oufti.py
--rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_refine.py
--rw-rw-rw-   0        0        0    21190 2023-03-27 09:54:48.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_statistics.py
--rw-rw-rw-   0        0        0     7055 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_tiler.py
--rw-rw-rw-   0        0        0      164 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg/_version.py
--rw-rw-rw-   0        0        0    79705 2023-05-06 06:34:35.000000 napari-bacseg-1.0.6/src/napari_bacseg/_widget.py
--rw-rw-rw-   0        0        0   162470 2023-05-05 08:42:27.000000 napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.py
--rw-rw-rw-   0        0        0   160468 2023-05-05 08:42:22.000000 napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.ui
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/gapseq_ui.py
--rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.6/src/napari_bacseg/napari.yaml
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/napari_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.561589 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/
--rw-rw-rw-   0        0        0     4732 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3271 2023-05-06 06:44:33.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      352 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.249218 napari-bacseg-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:26:17.997889 napari-bacseg-1.0.7/.github/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.033792 napari-bacseg-1.0.7/.github/workflows/
+-rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/.github/workflows/test_and_deploy.yml
+-rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.7/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.037782 napari-bacseg-1.0.7/.napari-hub/
+-rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/.napari-hub/DESCRIPTION.md
+-rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/.napari-hub/config.yml
+-rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.7/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4732 2023-06-13 16:26:18.249218 napari-bacseg-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/README.md
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/bacseg_ui.py
+-rw-rw-rw-   0        0        0      988 2023-06-13 16:26:05.000000 napari-bacseg-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     2035 2023-06-13 16:26:18.252210 napari-bacseg-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 16:26:17.998886 napari-bacseg-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.181398 napari-bacseg-1.0.7/src/_dev/
+-rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.7/src/_dev/Export Masks to AKSEG v5 dev.py
+-rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7/src/_dev/ScanR dev.py
+-rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.7/src/_dev/Troodos dev.py
+-rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.7/src/_dev/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.7/src/_dev/akseg_db_stats.py
+-rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/akseg_dev.py
+-rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/akseg_dev2.py
+-rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.7/src/_dev/akseg_txt_metadata.py
+-rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/align_alex_datadump.py
+-rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/alison_datadump.py
+-rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.7/src/_dev/autocontast_dev.py
+-rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/cellposedev.py
+-rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.7/src/_dev/cellposeshapely.py
+-rw-rw-rw-   0        0        0     1279 2023-03-27 16:45:42.000000 napari-bacseg-1.0.7/src/_dev/chatGPT_midlines.py
+-rw-rw-rw-   0        0        0     6105 2023-05-05 10:49:23.000000 napari-bacseg-1.0.7/src/_dev/check_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/check_metadata.py
+-rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.7/src/_dev/colicoords_cellldist_dev.py
+-rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.7/src/_dev/colicoords_ldist_dev.py
+-rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.7/src/_dev/database_dev.py
+-rw-rw-rw-   0        0        0     1023 2023-03-23 14:05:20.000000 napari-bacseg-1.0.7/src/_dev/deepsegmattest.py
+-rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.7/src/_dev/edit_database_columns.py
+-rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.7/src/_dev/fits_dev.py
+-rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/fix_alison_missing_file_list.py
+-rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/generate_scanr_movie.py
+-rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/get_akseg_stats.py
+-rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.7/src/_dev/get_species_info.py
+-rw-rw-rw-   0        0        0     1991 2023-06-13 13:41:08.000000 napari-bacseg-1.0.7/src/_dev/imagej_dev.py
+-rw-rw-rw-   0        0        0     5034 2023-06-13 08:40:50.000000 napari-bacseg-1.0.7/src/_dev/json_nuclei_dev.py
+-rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/luke__script.py
+-rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.7/src/_dev/matplotlib_Events.py
+-rw-rw-rw-   0        0        0    40825 2023-03-22 17:47:52.000000 napari-bacseg-1.0.7/src/_dev/move_AluGasketDFP.py
+-rw-rw-rw-   0        0        0    44028 2023-04-04 10:28:53.000000 napari-bacseg-1.0.7/src/_dev/move_AluGasketDFP_poster.py
+-rw-rw-rw-   0        0        0    48241 2023-04-26 15:22:38.000000 napari-bacseg-1.0.7/src/_dev/move_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0    46551 2023-05-05 08:15:07.000000 napari-bacseg-1.0.7/src/_dev/move_AluGasketv12_DFP_Titration.py
+-rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.7/src/_dev/move_conor_nim_dfp_data.py
+-rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.7/src/_dev/move_pillar_data.py
+-rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/move_pillar_zstack_data.py
+-rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.7/src/_dev/move_unlearning_files.py
+-rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.7/src/_dev/new_metadata2.pickle.py
+-rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.7/src/_dev/new_read_akseg_directory.py
+-rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/nim_dev.py
+-rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/omnipose_dev.py
+-rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7/src/_dev/omnipose_midlines.py
+-rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7/src/_dev/omnipose_train.py
+-rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.7/src/_dev/oufti_dilate.py
+-rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.7/src/_dev/oufti_dilate_with_midlines.py
+-rw-rw-rw-   0        0        0     4449 2023-05-04 09:42:23.000000 napari-bacseg-1.0.7/src/_dev/pandas_speed.py
+-rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/process_alex_datadump.py
+-rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/process_alex_datadump_clinical.py
+-rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/process_conor_datadump.py
+-rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/process_gramstain_datadump.py
+-rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.7/src/_dev/read_non_tif.py
+-rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/rebuild_usermeta.py
+-rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/rebuild_usermeta_2.py
+-rw-rw-rw-   0        0        0     3034 2023-03-23 13:58:59.000000 napari-bacseg-1.0.7/src/_dev/recreate_user_metadata.py
+-rw-rw-rw-   0        0        0     2117 2023-04-20 14:14:30.000000 napari-bacseg-1.0.7/src/_dev/scalebar_dev.py
+-rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/sort_midlines.py
+-rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/stelios_stats.py
+-rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/tile_meta_check.py
+-rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.7/src/_dev/tiler_dev.py
+-rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7/src/_dev/updade_akseg_metadata.py
+-rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.7/src/_dev/update_img_metadata.py
+-rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/video_iamges.py
+-rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.7/src/_dev/zooniverse.py
+-rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_move.py
+-rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_move_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_titration_upload.py
+-rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_upload.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.221292 napari-bacseg-1.0.7/src/napari_bacseg/
+-rw-rw-rw-   0        0        0      155 2023-06-13 16:18:00.000000 napari-bacseg-1.0.7/src/napari_bacseg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.247223 napari-bacseg-1.0.7/src/napari_bacseg/_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/src/napari_bacseg/_tests/__init__.py
+-rw-rw-rw-   0        0        0    26817 2023-06-13 13:36:57.000000 napari-bacseg-1.0.7/src/napari_bacseg/_tests/test_bacseg.py
+-rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    90731 2023-06-13 16:07:22.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils.py
+-rw-rw-rw-   0        0        0    14723 2023-06-13 08:44:12.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_cellpose.py
+-rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_colicoords.py
+-rw-rw-rw-   0        0        0    20495 2023-05-03 08:53:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_database.py
+-rw-rw-rw-   0        0        0    47487 2023-06-13 09:49:45.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_database_IO.py
+-rw-rw-rw-   0        0        0     1670 2023-06-13 13:50:19.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_imagej.py
+-rw-rw-rw-   0        0        0    40215 2023-06-13 08:44:13.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_interface_events.py
+-rw-rw-rw-   0        0        0     6485 2023-06-13 08:44:12.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_json.py
+-rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_oufti.py
+-rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_refine.py
+-rw-rw-rw-   0        0        0    22517 2023-06-09 14:18:42.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_statistics.py
+-rw-rw-rw-   0        0        0     7837 2023-06-09 14:18:42.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_tiler.py
+-rw-rw-rw-   0        0        0      218 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg/_version.py
+-rw-rw-rw-   0        0        0    83296 2023-06-13 15:33:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_widget.py
+-rw-rw-rw-   0        0        0   172700 2023-06-13 16:10:14.000000 napari-bacseg-1.0.7/src/napari_bacseg/bacseg_ui.py
+-rw-rw-rw-   0        0        0   172251 2023-06-13 16:10:08.000000 napari-bacseg-1.0.7/src/napari_bacseg/bacseg_ui.ui
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/gapseq_ui.py
+-rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.7/src/napari_bacseg/napari.yaml
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/napari_ui.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.242236 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/
+-rw-rw-rw-   0        0        0     4732 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      352 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/tox.ini
```

### Comparing `napari-bacseg-1.0.6/.github/workflows/test_and_deploy.yml` & `napari-bacseg-1.0.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/.gitignore` & `napari-bacseg-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/.napari-hub/config.yml` & `napari-bacseg-1.0.7/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/.pre-commit-config.yaml` & `napari-bacseg-1.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/LICENSE` & `napari-bacseg-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/PKG-INFO` & `napari-bacseg-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.6
+Version: 1.0.7
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.6/README.md` & `napari-bacseg-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/pyproject.toml` & `napari-bacseg-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [project]
 name = "napari-bacseg"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Piers Turner", email="piers.turner@physics.ox.ac.uk"},
 ]
 description = "Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `napari-bacseg-1.0.6/setup.cfg` & `napari-bacseg-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/Export Masks to AKSEG v5 dev.py` & `napari-bacseg-1.0.7/src/_dev/Export Masks to AKSEG v5 dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/ScanR dev.py` & `napari-bacseg-1.0.7/src/_dev/ScanR dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/akseg_db_stats.py` & `napari-bacseg-1.0.7/src/_dev/akseg_db_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/akseg_dev.py` & `napari-bacseg-1.0.7/src/_dev/akseg_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/akseg_dev2.py` & `napari-bacseg-1.0.7/src/_dev/akseg_dev2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/akseg_txt_metadata.py` & `napari-bacseg-1.0.7/src/_dev/akseg_txt_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/align_alex_datadump.py` & `napari-bacseg-1.0.7/src/_dev/align_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/alison_datadump.py` & `napari-bacseg-1.0.7/src/_dev/alison_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/autocontast_dev.py` & `napari-bacseg-1.0.7/src/_dev/autocontast_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/chatGPT_midlines.py` & `napari-bacseg-1.0.7/src/_dev/chatGPT_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/check_AluGasketv12_DFP.py` & `napari-bacseg-1.0.7/src/_dev/check_AluGasketv12_DFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/check_metadata.py` & `napari-bacseg-1.0.7/src/_dev/check_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/colicoords_cellldist_dev.py` & `napari-bacseg-1.0.7/src/_dev/colicoords_cellldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/colicoords_ldist_dev.py` & `napari-bacseg-1.0.7/src/_dev/colicoords_ldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/database_dev.py` & `napari-bacseg-1.0.7/src/_dev/database_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/deepsegmattest.py` & `napari-bacseg-1.0.7/src/_dev/deepsegmattest.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/edit_database_columns.py` & `napari-bacseg-1.0.7/src/_dev/edit_database_columns.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/fits_dev.py` & `napari-bacseg-1.0.7/src/_dev/fits_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/fix_alison_missing_file_list.py` & `napari-bacseg-1.0.7/src/_dev/fix_alison_missing_file_list.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/generate_scanr_movie.py` & `napari-bacseg-1.0.7/src/_dev/generate_scanr_movie.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/get_akseg_stats.py` & `napari-bacseg-1.0.7/src/_dev/get_akseg_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/get_species_info.py` & `napari-bacseg-1.0.7/src/_dev/get_species_info.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/luke__script.py` & `napari-bacseg-1.0.7/src/_dev/luke__script.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/matplotlib_Events.py` & `napari-bacseg-1.0.7/src/_dev/matplotlib_Events.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/move_AluGasketDFP.py` & `napari-bacseg-1.0.7/src/_dev/move_AluGasketDFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/move_AluGasketDFP_poster.py` & `napari-bacseg-1.0.7/src/_dev/move_AluGasketDFP_poster.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/move_AluGasketv12_DFP.py` & `napari-bacseg-1.0.7/src/_dev/move_AluGasketv12_DFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/move_AluGasketv12_DFP_Titration.py` & `napari-bacseg-1.0.7/src/_dev/move_AluGasketv12_DFP_Titration.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/move_conor_nim_dfp_data.py` & `napari-bacseg-1.0.7/src/_dev/move_conor_nim_dfp_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/move_pillar_data.py` & `napari-bacseg-1.0.7/src/_dev/move_pillar_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/move_pillar_zstack_data.py` & `napari-bacseg-1.0.7/src/_dev/move_pillar_zstack_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/move_unlearning_files.py` & `napari-bacseg-1.0.7/src/_dev/move_unlearning_files.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/new_metadata2.pickle.py` & `napari-bacseg-1.0.7/src/_dev/new_metadata2.pickle.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/new_read_akseg_directory.py` & `napari-bacseg-1.0.7/src/_dev/new_read_akseg_directory.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/nim_dev.py` & `napari-bacseg-1.0.7/src/_dev/nim_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/omnipose_dev.py` & `napari-bacseg-1.0.7/src/_dev/omnipose_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/omnipose_midlines.py` & `napari-bacseg-1.0.7/src/_dev/omnipose_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/omnipose_train.py` & `napari-bacseg-1.0.7/src/_dev/omnipose_train.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/oufti_dilate.py` & `napari-bacseg-1.0.7/src/_dev/oufti_dilate.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/oufti_dilate_with_midlines.py` & `napari-bacseg-1.0.7/src/_dev/oufti_dilate_with_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/pandas_speed.py` & `napari-bacseg-1.0.7/src/_dev/pandas_speed.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/process_alex_datadump.py` & `napari-bacseg-1.0.7/src/_dev/process_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/process_alex_datadump_clinical.py` & `napari-bacseg-1.0.7/src/_dev/process_alex_datadump_clinical.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/process_conor_datadump.py` & `napari-bacseg-1.0.7/src/_dev/process_conor_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/process_gramstain_datadump.py` & `napari-bacseg-1.0.7/src/_dev/process_gramstain_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/read_non_tif.py` & `napari-bacseg-1.0.7/src/_dev/read_non_tif.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/rebuild_usermeta.py` & `napari-bacseg-1.0.7/src/_dev/rebuild_usermeta.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/rebuild_usermeta_2.py` & `napari-bacseg-1.0.7/src/_dev/rebuild_usermeta_2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/recreate_user_metadata.py` & `napari-bacseg-1.0.7/src/_dev/recreate_user_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/scalebar_dev.py` & `napari-bacseg-1.0.7/src/_dev/scalebar_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/sort_midlines.py` & `napari-bacseg-1.0.7/src/_dev/sort_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/stelios_stats.py` & `napari-bacseg-1.0.7/src/_dev/stelios_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/tile_meta_check.py` & `napari-bacseg-1.0.7/src/_dev/tile_meta_check.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/tiler_dev.py` & `napari-bacseg-1.0.7/src/_dev/tiler_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/updade_akseg_metadata.py` & `napari-bacseg-1.0.7/src/_dev/updade_akseg_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/update_img_metadata.py` & `napari-bacseg-1.0.7/src/_dev/update_img_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/video_iamges.py` & `napari-bacseg-1.0.7/src/_dev/video_iamges.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/zooniverse.py` & `napari-bacseg-1.0.7/src/_dev/zooniverse.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/zooniverse_move.py` & `napari-bacseg-1.0.7/src/_dev/zooniverse_move.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/zooniverse_move_titrations.py` & `napari-bacseg-1.0.7/src/_dev/zooniverse_move_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/zooniverse_titration_upload.py` & `napari-bacseg-1.0.7/src/_dev/zooniverse_titration_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/zooniverse_titrations.py` & `napari-bacseg-1.0.7/src/_dev/zooniverse_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/_dev/zooniverse_upload.py` & `napari-bacseg-1.0.7/src/_dev/zooniverse_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_tests/test_bacseg.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_tests/test_bacseg.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,61 +9,76 @@
 import numpy as np
 import pandas as pd
 import tifffile
 from glob2 import glob
 
 
 class test_bacseg(unittest.TestCase):
+    
     @classmethod
     def setUpClass(cls):
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=DeprecationWarning)
 
             from napari import Viewer
 
             from napari_bacseg._widget import BacSeg
 
             viewer = Viewer()
 
             cls.BacSeg = BacSeg(viewer)
             cls.BacSeg.widget_notifications = False
 
-            cls.export_setting_dict = {"mode": ["masks", "images", "images + masks", "oufti", "cellpose", "imagej", "json", "csv", ], "overwrite": [True, False], "export_images": [True,
-                                                                                                                                                                                    False], "normalise": [
-                True, False], "invert": [True, False], "autocontrast": [True, False], }
-
-            cls.import_images_setting_dict = {"mode": ["images", "scanr", "nim"], "filemode": ["directory", "file"], "import_limit": ["None", "1", "5", "100"], "import_precision": [
-                "int16"], "multiframe_mode_index": [0, 1, 2, 3], "crop_mode_index": [0, 1, 2, 3], }
-
-            cls.import_masks_setting_dict = {"mode": ["masks", "imagej", "json", "csv"], "filemode": ["directory", "file"], "import_limit": ["None", "100", "1000"], "import_precision": ["int8",
-                                                                                                                                                                                          "int16",
-                                                                                                                                                                                          "int32",
-                                                                                                                                                                                          "native"], "multiframe_mode_index": [
-                0, 1, 2, 3], "crop_mode_index": [0, 1, 2, 3], }
+            cls.export_setting_dict = {"mode": ["masks", "images", "images + masks", "oufti", "cellpose", "imagej", "json", "csv", ], 
+                                       "overwrite": [True, False],
+                                       "export_images": [True,False],
+                                       "normalise": [True, False],
+                                       "invert": [True, False],
+                                       "autocontrast": [True, False], }
+
+            cls.import_images_setting_dict = {"mode": ["images", "scanr", "nim"],
+                                              "filemode": ["directory", "file"],
+                                              "import_limit": ["None", "1", "5", "100"], 
+                                              "import_precision": ["int16"],
+                                              "multiframe_mode_index": [0, 1, 2, 3],
+                                              "crop_mode_index": [0, 1, 2, 3], }
+
+            cls.import_masks_setting_dict = {"mode": ["masks", "imagej", "json", "csv"],
+                                             "filemode": ["directory", "file"],
+                                             "import_limit": ["None", "100", "1000"],
+                                             "import_precision": ["int8","int16","int32","native"],
+                                             "multiframe_mode_index": [0, 1, 2, 3], 
+                                             "crop_mode_index": [0, 1, 2, 3], }
 
+
+    
     def perumuation_test(self, function, setting_dict={}, limit=10, shuffle=True):
+        
         modes = setting_dict.pop("mode")
 
         for mode in modes:
             settings = setting_dict.values()
 
             possible_settings_values = list(itertools.product(*settings))
 
             if shuffle == True:
                 random.shuffle(possible_settings_values)
 
             possible_settings_values = possible_settings_values[:limit]
 
             for setting in possible_settings_values:
+                
                 active_settings = dict(zip(setting_dict.keys(), setting))
 
                 with self.subTest(msg="getAll"):
                     function(mode=mode, **active_settings)
 
+
     def import_images(self, mode="images", filemode="directory", import_limit="None", import_precision="int16", multiframe_mode_index=0, crop_mode_index=0, ):
+        
         if filemode == "directory":
             self.BacSeg.import_filemode.setCurrentText("Import Directory")
         elif filemode == "file":
             self.BacSeg.import_filemode.setCurrentText("Import File")
 
         self.BacSeg.import_limit.setCurrentText(import_limit)
 
@@ -123,15 +138,15 @@
             target_num_images = len(measurements)
             target_channels = channels
 
             data = self.BacSeg.read_nim_images(measurements=measurements, channels=channels, progress_callback=None, )
 
         self.BacSeg._process_import(data)
 
-        layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
         loaded_images = self.BacSeg.viewer.layers[layer_names[0]].data
 
         if import_limit != "None":
             if target_num_images > int(import_limit):
                 target_num_images = int(import_limit)
 
@@ -224,15 +239,15 @@
 
             data = self.BacSeg.import_imagej(mask_paths)
 
             self.BacSeg._process_import(data)
 
         mask_dict = self.read_mask_files(mask_paths)
 
-        layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
         for layer in layer_names:
             metadata = self.BacSeg.viewer.layers[layer].metadata
 
             for index, meta in metadata.items():
                 image_name = meta["image_name"].strip()
                 mask = self.BacSeg.segLayer.data[index]
 
@@ -244,15 +259,15 @@
 
     def export_data(self, mode="masks", overwrite=False, export_images=False, normalise=False, invert=False, autocontrast=False, export_modifier="_BacSeg", ):
         if self.BacSeg.segLayer.data.shape == (1, 100, 100):
             self.import_masks(mode="masks")
 
         self.BacSeg.export_directory = "test_data/exported_data"
 
-        layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
         if os.path.isdir(self.BacSeg.export_directory) != True:
             os.mkdir(self.BacSeg.export_directory)
         else:
             shutil.rmtree(self.BacSeg.export_directory)
             os.mkdir(self.BacSeg.export_directory)
 
@@ -287,15 +302,15 @@
 
         self.BacSeg.export_files = self.BacSeg.wrapper(export_files)
 
         self.BacSeg.export_files(mode="All", progress_callback=None)
 
         num_exported_files = len(glob(self.BacSeg.export_directory + "/*"))
 
-        layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
         num_images = self.BacSeg.viewer.layers[layer_names[0]].data.shape[0]
 
         if export_images == True and mode in ["oufti", "cellpose", "json", "csv", ]:
             targeted_image_num = num_images * 2
         elif mode == "images + masks":
             num_exported_files = len(glob(self.BacSeg.export_directory + "/*/*"))
@@ -388,15 +403,14 @@
         database_directory = self.BacSeg._create_bacseg_database(path=path)
 
         self.BacSeg.database_path = database_directory
 
         return database_directory
 
     def get_database_metadata(self, user_initial="all"):
-
         database_directory = self.BacSeg.database_path
 
         if user_initial != "all":
             meta_path = os.path.join(self.BacSeg.database_path, "images", user_initial, f"{user_initial}_file_metadata.txt", )
 
             if os.path.exists(meta_path) == True:
                 metadata = pd.read_csv(meta_path, sep=",", low_memory=False)
@@ -446,49 +460,48 @@
 
         self.BacSeg.update_database_metadata(control=None)
 
         for control_name, control_text in upload_control_dict.items():
             combo_box = getattr(self.BacSeg, control_name)
             combo_box.setCurrentText(control_text)
 
-    def upload_database(self, path=None, mode="active", user_initial="AK", content="BacSeg", microscope="Nikon", modalilty="Fluorescence", source="LED", stain="None", stain_target="None", overwrite_images=False, overwrite_masks=False, overwrite_all_metadata=False, overwrite_selected_metadata=False, ):
-
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", category=ResourceWarning)
+    # def upload_database(self, path=None, mode="active", user_initial="AK", content="BacSeg", microscope="Nikon", modalilty="Fluorescence", source="LED", stain="None", stain_target="None", overwrite_images=False, overwrite_masks=False, overwrite_all_metadata=False, overwrite_selected_metadata=False, ):
+    #     with warnings.catch_warnings():
+    #         warnings.filterwarnings("ignore", category=ResourceWarning)
 
-            if type(path) == str:
-                self.create_database(path=path)
+    #         if type(path) == str:
+    #             self.create_database(path=path)
 
-            pre_upload_metadata = len(self.get_database_metadata(user_initial=user_initial))
+    #         pre_upload_metadata = len(self.get_database_metadata(user_initial=user_initial))
 
-            self.BacSeg.upload_initial.setCurrentText(user_initial)
-            self.BacSeg.upload_content.setCurrentText(content)
-            self.BacSeg.upload_microscope.setCurrentText(microscope)
-            self.BacSeg.label_modality.setCurrentText(modalilty)
-            self.BacSeg.label_light_source.setCurrentText(source)
-            self.BacSeg.label_stain.setCurrentText(stain)
-            self.BacSeg.label_stain_target.setCurrentText(stain_target)
-            self.BacSeg.upload_overwrite_images.setChecked(overwrite_images)
-            self.BacSeg.upload_overwrite_masks.setChecked(overwrite_masks)
-            self.BacSeg.overwrite_all_metadata.setChecked(overwrite_all_metadata)
-            self.BacSeg.overwrite_selected_metadata.setChecked(overwrite_selected_metadata)
+    #         self.BacSeg.upload_initial.setCurrentText(user_initial)
+    #         self.BacSeg.upload_content.setCurrentText(content)
+    #         self.BacSeg.upload_microscope.setCurrentText(microscope)
+    #         self.BacSeg.label_modality.setCurrentText(modalilty)
+    #         self.BacSeg.label_light_source.setCurrentText(source)
+    #         self.BacSeg.label_stain.setCurrentText(stain)
+    #         self.BacSeg.label_stain_target.setCurrentText(stain_target)
+    #         self.BacSeg.upload_overwrite_images.setChecked(overwrite_images)
+    #         self.BacSeg.upload_overwrite_masks.setChecked(overwrite_masks)
+    #         self.BacSeg.overwrite_all_metadata.setChecked(overwrite_all_metadata)
+    #         self.BacSeg.overwrite_selected_metadata.setChecked(overwrite_selected_metadata)
 
-            from napari_bacseg._utils_database_IO import (_upload_bacseg_database, )
+    #         from napari_bacseg._utils_database_IO import (_upload_bacseg_database, )
 
-            self.BacSeg._upload_bacseg_database = self.BacSeg.wrapper(_upload_bacseg_database)
+    #         self.BacSeg._upload_bacseg_database = self.BacSeg.wrapper(_upload_bacseg_database)
 
-            self.BacSeg._upload_bacseg_database(mode=mode, progress_callback=None)
+    #         self.BacSeg._upload_bacseg_database(mode=mode, progress_callback=None)
 
-            post_upload_metadata = len(self.get_database_metadata(user_initial=user_initial))
+    #         post_upload_metadata = len(self.get_database_metadata(user_initial=user_initial))
 
-            database_length_increase = (post_upload_metadata - pre_upload_metadata)
+    #         database_length_increase = (post_upload_metadata - pre_upload_metadata)
 
-            self.update_database_metadata(user_initial)
+    #         self.update_database_metadata(user_initial)
 
-        return database_length_increase
+    #     return database_length_increase
 
     # def test_database_upload(self, mode = "all"):
     #
     #     self.create_database()
     #     self.import_masks(mode="imagej")
     #
     #     database_length_increase = self.upload_database(mode = mode)
@@ -505,96 +518,102 @@
     #         active_layer = self.BacSeg.viewer.layers.selection.active.name
     #         target_num_uploads = self.BacSeg.viewer.layers[active_layer].data.shape[0]
     #
     #     assert target_num_uploads == num_uploads
     #     assert target_num_uploads == database_length_increase
     #
 
-    def test_database_download(self, import_limit=1):
-
-        meta_keys = ["user_initial", "content", "microscope", "antibiotic", "treatment time (mins)", "source", "modality", "stain", "antibiotic concentration", "mounting method", "protocol",
-            "segmented", "segmentation_curated", "labelled", "label_curated", "user_meta1", "user_meta2", "user_meta3", ]
-
-        self.load_database()
-
-        metadata = self.get_database_metadata()
-
-        metadata = metadata[meta_keys]
-
-        metadata = metadata.sample(n=import_limit, random_state=0).dropna(axis=1, how="all")
-
-        meta_options = {}
-        for column in metadata.columns.values:
-            value = metadata[column].values[0]
-
-            if value != "None":
-                meta_options[column] = value
-
-        user_initial = meta_options.pop("user_initial")
-
-        keys = random.sample(list(meta_options), 3)
-        meta_options = {key: meta_options[key] for key in keys}
-
-        self.BacSeg.upload_initial.setCurrentText(user_initial)
-
-        # if "content" in meta_options:
-        #     self.BacSeg.upload_content.setCurrentText(meta_options["content"])
-        # if "microscope" in meta_options:
-        #     self.BacSeg.upload_microscope.setCurrentText(meta_options["microscope"])
-        # if "antibiotic" in meta_options:
-        #     self.BacSeg.upload_antibiotic.setCurrentText(meta_options["antibiotic"])
-        # if "treatment time (mins)" in meta_options:
-        #     self.BacSeg.upload_treatment_time.setCurrentText(meta_options["treatment time (mins)"])
-        # if "antibiotic concentration" in meta_options:
-        #     self.BacSeg.upload_abxconcentration.setCurrentText(meta_options["antibiotic concentration"])
-        # if "mounting method" in meta_options:
-        #     self.BacSeg.upload_mount.setCurrentText(meta_options["mounting method"])
-        # if "protocol" in meta_options:
-        #     self.BacSeg.upload_protocol.setCurrentText(meta_options["protocol"])
-        #
-        # if "segmentation_curated" in meta_options:
-        #     if meta_options["segmentation_curated"] == True:
-        #         self.BacSeg.upload_segmentation_combo.setCurrentIndex(3)
-        #     else:
-        #         self.BacSeg.upload_segmentation_combo.setCurrentIndex(2)
-        # elif "segmented" in meta_options:
-        #     if meta_options["segmented"] == True:
-        #         self.BacSeg.upload_segmentation_combo.setCurrentIndex(2)
-        #     else:
-        #         self.BacSeg.upload_segmentation_combo.setCurrentIndex(1)
-        # else:
-        #     self.BacSeg.upload_segmentation_combo.setCurrentIndex(0)
-        #
-        # if "label_curated" in meta_options:
-        #     if meta_options["label_curated"] == True:
-        #         self.BacSeg.upload_label_combo.setCurrentIndex(3)
-        #     else:
-        #         self.BacSeg.upload_label_combo.setCurrentIndex(2)
-        # elif "labelled" in meta_options:
-        #     if meta_options["labelled"] == True:
-        #         self.BacSeg.upload_label_combo.setCurrentIndex(2)
-        #     else:
-        #         self.BacSeg.upload_label_combo.setCurrentIndex(1)
-        # else:
-        #     self.BacSeg.upload_label_combo.setCurrentIndex(0)
-
-        from napari_bacseg._utils_database_IO import (get_filtered_database_metadata, read_bacseg_images, )
-
-        self.BacSeg.get_filtered_database_metadata = self.BacSeg.wrapper(get_filtered_database_metadata)
-        self.BacSeg.read_bacseg_images = self.BacSeg.wrapper(read_bacseg_images)
-
-        self.BacSeg.active_import_mode = "BacSeg"
-
-        (measurements, file_paths, channels,) = self.BacSeg.get_filtered_database_metadata()
-
-        data = self.BacSeg.read_bacseg_images(measurements=measurements, channels=channels, progress_callback=None, )
-        self.BacSeg._process_import(data)
-
-        layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
-
-        loaded_images = len(self.BacSeg.viewer.layers[layer_names[0]].data)
-
-        assert loaded_images == import_limit
+    # def test_database_download(self, import_limit=1):
+    #     meta_keys = ["user_initial", "content", "microscope", "antibiotic", "treatment time (mins)", "source", "modality", "stain", "antibiotic concentration", "mounting method", "protocol",
+    #         "segmented", "segmentation_curated", "labelled", "label_curated", "user_meta1", "user_meta2", "user_meta3", ]
+
+    #     self.load_database()
+
+    #     metadata = self.get_database_metadata()
+
+    #     metadata = metadata[meta_keys]
+
+    #     metadata = metadata.sample(n=import_limit, random_state=0).dropna(axis=1, how="all")
+
+    #     meta_options = {}
+    #     for column in metadata.columns.values:
+    #         value = metadata[column].values[0]
+
+    #         if value != "None":
+    #             meta_options[column] = value
+
+    #     user_initial = meta_options.pop("user_initial")
+
+    #     keys = random.sample(list(meta_options), 3)
+    #     meta_options = {key: meta_options[key] for key in keys}
+
+    #     self.BacSeg.upload_initial.setCurrentText(user_initial)
+
+    #     # if "content" in meta_options:
+    #     #     self.BacSeg.upload_content.setCurrentText(meta_options["content"])
+    #     # if "microscope" in meta_options:
+    #     #     self.BacSeg.upload_microscope.setCurrentText(meta_options["microscope"])
+    #     # if "antibiotic" in meta_options:
+    #     #     self.BacSeg.upload_antibiotic.setCurrentText(meta_options["antibiotic"])
+    #     # if "treatment time (mins)" in meta_options:
+    #     #     self.BacSeg.upload_treatment_time.setCurrentText(meta_options["treatment time (mins)"])
+    #     # if "antibiotic concentration" in meta_options:
+    #     #     self.BacSeg.upload_abxconcentration.setCurrentText(meta_options["antibiotic concentration"])
+    #     # if "mounting method" in meta_options:
+    #     #     self.BacSeg.upload_mount.setCurrentText(meta_options["mounting method"])
+    #     # if "protocol" in meta_options:
+    #     #     self.BacSeg.upload_protocol.setCurrentText(meta_options["protocol"])
+    #     #
+    #     # if "segmentation_curated" in meta_options:
+    #     #     if meta_options["segmentation_curated"] == True:
+    #     #         self.BacSeg.upload_segmentation_combo.setCurrentIndex(3)
+    #     #     else:
+    #     #         self.BacSeg.upload_segmentation_combo.setCurrentIndex(2)
+    #     # elif "segmented" in meta_options:
+    #     #     if meta_options["segmented"] == True:
+    #     #         self.BacSeg.upload_segmentation_combo.setCurrentIndex(2)
+    #     #     else:
+    #     #         self.BacSeg.upload_segmentation_combo.setCurrentIndex(1)
+    #     # else:
+    #     #     self.BacSeg.upload_segmentation_combo.setCurrentIndex(0)
+    #     #
+    #     # if "label_curated" in meta_options:
+    #     #     if meta_options["label_curated"] == True:
+    #     #         self.BacSeg.upload_label_combo.setCurrentIndex(3)
+    #     #     else:
+    #     #         self.BacSeg.upload_label_combo.setCurrentIndex(2)
+    #     # elif "labelled" in meta_options:
+    #     #     if meta_options["labelled"] == True:
+    #     #         self.BacSeg.upload_label_combo.setCurrentIndex(2)
+    #     #     else:
+    #     #         self.BacSeg.upload_label_combo.setCurrentIndex(1)
+    #     # else:
+    #     #     self.BacSeg.upload_label_combo.setCurrentIndex(0)
+
+    #     from napari_bacseg._utils_database_IO import (get_filtered_database_metadata, read_bacseg_images, )
+
+    #     self.BacSeg.get_filtered_database_metadata = self.BacSeg.wrapper(get_filtered_database_metadata)
+    #     self.BacSeg.read_bacseg_images = self.BacSeg.wrapper(read_bacseg_images)
+
+    #     self.BacSeg.active_import_mode = "BacSeg"
+
+    #     (measurements, file_paths, channels,) = self.BacSeg.get_filtered_database_metadata()
+
+    #     data = self.BacSeg.read_bacseg_images(measurements=measurements, channels=channels, progress_callback=None, )
+    #     self.BacSeg._process_import(data)
+
+    #     layer_names = [layer.name for layer in self.BacSeg.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+
+    #     loaded_images = len(self.BacSeg.viewer.layers[layer_names[0]].data)
+
+    #     assert loaded_images == import_limit
+
+
+    # def test_import(self):
+    #     self.perumuation_test(self.import_images, setting_dict=self.import_images_setting_dict)
+    # def test_export(self):
+    #     self.perumuation_test(self.export_data, setting_dict=self.export_setting_dict)
+        
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_tests/test_widget.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from astropy.io import fits
 from glob2 import glob
 from napari.utils.notifications import show_info
 
 # from napari_bacseg._utils_imagej import read_imagej_file
 from skimage import exposure
 from skimage.registration import phase_cross_correlation
-
+import copy
 
 def normalize99(X):
     """normalize image so 0.0 is 0.01st percentile and 1.0 is 99.99th percentile"""
 
     if np.max(X) > 0:
         X = X.copy()
         v_min, v_max = np.percentile(X[X != 0], (0.1, 99.9))
@@ -58,57 +58,43 @@
 
                 if type(image_list) == dict:
                     image_list = [image_list]
 
                 for i in range(len(image_list)):
                     img = image_list[i]
 
-                    objective_id = int(
-                        img["ObjectiveSettings"]["@ID"].split(":")[-1]
-                    )
-                    objective_dat = dat["Instrument"]["Objective"][
-                        objective_id
-                    ]
-                    objective_mag = float(
-                        objective_dat["@NominalMagnification"]
-                    )
+                    objective_id = int(img["ObjectiveSettings"]["@ID"].split(":")[-1])
+                    objective_dat = dat["Instrument"]["Objective"][objective_id]
+                    objective_mag = float(objective_dat["@NominalMagnification"])
                     objective_na = float(objective_dat["@LensNA"])
 
                     pixel_size = float(img["Pixels"]["@PhysicalSizeX"])
 
                     position_index = i
                     microscope = "ScanR"
                     light_source = "LED"
 
                     channel_dict = {}
 
                     for j in range(len(img["Pixels"]["Channel"])):
                         channel_data = img["Pixels"]["Channel"][j]
 
-                        channel_dict[j] = dict(
-                            modality=channel_data["@IlluminationType"],
-                            channel=channel_data["@Name"],
-                            mode=channel_data["@AcquisitionMode"],
-                            well=channel_data["@ID"]
-                            .split("W")[1]
-                            .split("P")[0],
-                        )
+                        channel_dict[j] = dict(modality=channel_data["@IlluminationType"], channel=channel_data["@Name"], mode=channel_data["@AcquisitionMode"], well=
+                        channel_data["@ID"].split("W")[1].split("P")[0], )
 
                     primary_channel = ""
 
                     for j in range(len(img["Pixels"]["TiffData"])):
                         num_channels = img["Pixels"]["@SizeC"]
                         num_zstack = img["Pixels"]["@SizeZ"]
 
                         tiff_data = img["Pixels"]["TiffData"][j]
 
                         file_name = tiff_data["UUID"]["@FileName"]
-                        file_path = os.path.abspath(
-                            path.replace(os.path.basename(path), file_name)
-                        )
+                        file_path = os.path.abspath(path.replace(os.path.basename(path), file_name))
 
                         try:
                             plane_data = img["Pixels"]["Plane"][j]
                             exposure_time = plane_data["@ExposureTime"]
                             posX = float(plane_data["@PositionX"])
                             posY = float(plane_data["@PositionY"])
                             posZ = float(plane_data["@PositionZ"])
@@ -131,33 +117,16 @@
                             time_index = None
                             z_index = None
                             channel_dat = None
                             modality = None
                             channel = None
                             well_index = None
 
-                        files[file_path] = dict(
-                            file_name=file_name,
-                            well_index=well_index,
-                            position_index=position_index,
-                            channel_index=channel_index,
-                            time_index=time_index,
-                            z_index=z_index,
-                            microscope=microscope,
-                            light_source=light_source,
-                            channel=channel,
-                            modality=modality,
-                            pixel_size=pixel_size,
-                            objective_magnification=objective_mag,
-                            objective_na=objective_na,
-                            exposure_time=exposure_time,
-                            posX=posX,
-                            posY=posY,
-                            posZ=posZ,
-                        )
+                        files[
+                            file_path] = dict(file_name=file_name, well_index=well_index, position_index=position_index, channel_index=channel_index, time_index=time_index, z_index=z_index, microscope=microscope, light_source=light_source, channel=channel, modality=modality, pixel_size=pixel_size, objective_magnification=objective_mag, objective_na=objective_na, exposure_time=exposure_time, posX=posX, posY=posY, posZ=posZ, )
     except:
         print(traceback.format_exc())
 
     return files
 
 
 def read_scanr_directory(self, path):
@@ -169,39 +138,29 @@
 
         if len(path) == 1:
             path = os.path.abspath(path[0])
 
             if os.path.isfile(path) == True:
                 selected_paths = [path]
                 image_path = os.path.abspath(path)
-                file_directory = os.path.abspath(
-                    image_path.split(image_path.split("\\")[-1])[0]
-                )
+                file_directory = os.path.abspath(image_path.split(image_path.split("\\")[-1])[0])
                 file_paths = glob(file_directory + r"*\*.tif")
 
             else:
                 file_paths = glob(path + r"*\**\*.tif", recursive=True)
                 selected_paths = []
         else:
             selected_paths = [os.path.abspath(path) for path in path]
             image_path = os.path.abspath(path[0])
-            file_directory = os.path.abspath(
-                image_path.split(image_path.split("\\")[-1])[0]
-            )
+            file_directory = os.path.abspath(image_path.split(image_path.split("\\")[-1])[0])
             file_paths = glob(file_directory + r"*\*.tif")
 
-        scanR_meta_files = [
-            path.replace(os.path.basename(path), "") for path in file_paths
-        ]
+        scanR_meta_files = [path.replace(os.path.basename(path), "") for path in file_paths]
         scanR_meta_files = np.unique(scanR_meta_files).tolist()
-        scanR_meta_files = [
-            glob(path + "*.ome.xml")[0]
-            for path in scanR_meta_files
-            if len(glob(path + "*.ome.xml")) > 0
-        ]
+        scanR_meta_files = [glob(path + "*.ome.xml")[0] for path in scanR_meta_files if len(glob(path + "*.ome.xml")) > 0]
 
         file_info = read_xml(scanR_meta_files)
 
         files = []
 
         for path in file_paths:
             try:
@@ -240,55 +199,39 @@
             if int(import_limit) > num_measurements:
                 import_limit = num_measurements
 
         acquisitions = files.position_index.unique()[: int(import_limit)]
 
         files = files[files["position_index"] <= acquisitions[-1]]
 
-        measurements = files.groupby(
-            by=["parent_folder", "position_index", "time_index", "z_index"]
-        )
+        measurements = files.groupby(by=["parent_folder", "position_index", "time_index", "z_index"])
 
         if selected_paths != []:
             filtered_measurements = []
 
             for i in range(len(measurements)):
-                measurement = measurements.get_group(
-                    list(measurements.groups)[i]
-                )
+                measurement = measurements.get_group(list(measurements.groups)[i])
                 measurement_paths = measurement["path"].tolist()
 
-                selected_paths = [
-                    os.path.abspath(path) for path in selected_paths
-                ]
-                measurement_paths = [
-                    os.path.abspath(path) for path in measurement_paths
-                ]
+                selected_paths = [os.path.abspath(path) for path in selected_paths]
+                measurement_paths = [os.path.abspath(path) for path in measurement_paths]
 
                 if not set(selected_paths).isdisjoint(measurement_paths):
                     filtered_measurements.append(measurement)
 
             filtered_measurements = pd.concat(filtered_measurements)
 
-            measurements = filtered_measurements.groupby(
-                by=["folder", "position_index", "time_index", "z_index"]
-            )
+            measurements = filtered_measurements.groupby(by=["folder", "position_index", "time_index", "z_index"])
 
         channels = files["channel"].drop_duplicates().to_list()
 
         channel_num = str(len(files["channel"].unique()))
 
         if self.widget_notifications:
-            show_info(
-                "Found "
-                + str(len(measurements))
-                + " measurments in ScanR Folder(s) with "
-                + channel_num
-                + " channels."
-            )
+            show_info("Found " + str(len(measurements)) + " measurments in ScanR Folder(s) with " + channel_num + " channels.")
 
     except:
         measurements, file_paths, channels = None, None, None
         print(traceback.format_exc())
 
     return measurements, file_paths, channels
 
@@ -320,39 +263,30 @@
 
             try:
                 progress_callback.emit(progress)
             except:
                 pass
 
             if self.widget_notifications:
-                show_info(
-                    "loading image["
-                    + channel
-                    + "] "
-                    + str(i + 1)
-                    + " of "
-                    + str(len(measurements))
-                )
+                show_info("loading image[" + channel + "] " + str(i + 1) + " of " + str(len(measurements)))
 
             if channel in measurement_channels:
                 dat = measurement[measurement["channel"] == channel]
 
                 path = dat["path"].item()
                 laser = "LED"
                 folder = dat["folder"].item()
                 parent_folder = dat["parent_folder"].item()
                 modality = dat["modality"].item()
 
                 import_precision = self.import_precision.currentText()
                 multiframe_mode = self.import_multiframe_mode.currentIndex()
                 crop_mode = self.import_crop_mode.currentIndex()
 
-                img, meta = read_image_file(
-                    path, import_precision, multiframe_mode, crop_mode
-                )
+                img, meta = read_image_file(path, import_precision, multiframe_mode, crop_mode)
 
                 contrast_limit, alpha, beta, gamma = autocontrast_values(img)
 
                 self.active_import_mode = "ScanR"
 
                 meta["image_name"] = os.path.basename(path)
                 meta["image_path"] = path
@@ -399,27 +333,26 @@
                 meta["contrast_beta"] = None
                 meta["contrast_gamma"] = None
                 meta["dims"] = [img.shape[-1], img.shape[-2]]
                 meta["crop"] = [0, img.shape[-2], 0, img.shape[-1]]
                 meta["light_source"] = channel
 
             if channel not in scanr_images:
-                scanr_images[channel] = dict(
-                    images=[img], masks=[], classes=[], metadata={i: meta}
-                )
+                scanr_images[channel] = dict(images=[img], masks=[], nmasks=[], classes=[], metadata={i: meta}, )
             else:
                 scanr_images[channel]["images"].append(img)
                 scanr_images[channel]["metadata"][i] = meta
 
     imported_data = dict(imported_images=scanr_images)
 
     return imported_data
 
 
 def import_imagej(self, progress_callback, paths):
+
     if isinstance(paths, list) == False:
         paths = [paths]
 
     if len(paths) == 1:
         paths = os.path.abspath(paths[0])
 
         if os.path.isfile(paths) == True:
@@ -430,79 +363,99 @@
     else:
         file_paths = paths
 
     file_paths = [file for file in file_paths if file.split(".")[-1] == "tif"]
 
     images = []
     masks = []
+    nmasks = []
     metadata = {}
     imported_images = {}
 
+    img_index = 0
+
     for i in range(len(file_paths)):
         progress = int(((i + 1) / len(file_paths)) * 100)
         try:
             progress_callback.emit(progress)
         except:
             pass
 
         if self.widget_notifications:
-            show_info(
-                "loading image " + str(i + 1) + " of " + str(len(file_paths))
-            )
+            show_info("loading image " + str(i + 1) + " of " + str(len(file_paths)))
 
         paths = file_paths[i]
         paths = os.path.abspath(paths)
 
         import_precision = self.import_precision.currentText()
         multiframe_mode = self.import_multiframe_mode.currentIndex()
         crop_mode = self.import_crop_mode.currentIndex()
-        image, meta = read_image_file(paths, import_precision, multiframe_mode)
+
+        image_list, meta = read_image_file(paths, import_precision, multiframe_mode, crop_mode)
+
+        akseg_hash = get_hash(img_path=paths)
 
         from napari_bacseg._utils_imagej import read_imagej_file
 
-        mask = read_imagej_file(paths, image)
+        file_name = os.path.basename(paths)
 
-        contrast_limit, alpha, beta, gamma = autocontrast_values(image)
+        for index, frame in enumerate(image_list):
 
-        self.active_import_mode = "Dataset"
+            contrast_limit = np.percentile(frame, (1, 99))
+            contrast_limit = [int(contrast_limit[0] * 0.5), int(contrast_limit[1] * 2), ]
 
-        meta["akseg_hash"] = get_hash(img_path=paths)
-        meta["image_name"] = os.path.basename(paths)
-        meta["image_path"] = paths
-        meta["mask_name"] = os.path.basename(paths)
-        meta["mask_path"] = paths
-        meta["label_name"] = None
-        meta["label_path"] = None
-        meta["import_mode"] = "Dataset"
-        meta["contrast_limit"] = contrast_limit
-        meta["contrast_alpha"] = alpha
-        meta["contrast_beta"] = beta
-        meta["contrast_gamma"] = gamma
-        meta["dims"] = [image.shape[-1], image.shape[-2]]
-        meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
-
-        images.append(image)
-        masks.append(mask)
-        metadata[i] = meta
+            mask = read_imagej_file(paths, frame)
 
-        if imported_images == {}:
-            imported_images["Image"] = dict(
-                images=[image], masks=[mask], classes=[], metadata={i: meta}
-            )
-        else:
-            imported_images["Image"]["images"].append(image)
-            imported_images["Image"]["masks"].append(mask)
-            imported_images["Image"]["metadata"][i] = meta
+            self.active_import_mode = "imagej"
+
+            if len(image_list) > 1:
+                frame_name = file_name.replace(".", "_") + "_" + str(index) + ".tif"
+            else:
+                frame_name = copy.deepcopy(file_name)
+
+            frame_meta = copy.deepcopy(meta)
+
+            frame_meta["akseg_hash"] = akseg_hash
+            frame_meta["image_name"] = frame_name
+            frame_meta["image_path"] = paths
+            frame_meta["mask_name"] = frame_name
+            frame_meta["mask_path"] = paths
+            frame_meta["label_name"] = None
+            frame_meta["label_path"] = None
+            frame_meta["import_mode"] = "Dataset"
+            frame_meta["contrast_limit"] = contrast_limit
+            frame_meta["contrast_alpha"] = 0
+            frame_meta["contrast_beta"] = 0
+            frame_meta["contrast_gamma"] = 0
+            frame_meta["dims"] = [frame.shape[-1], frame.shape[-2]]
+            frame_meta["crop"] = [0, frame.shape[-2], 0, frame.shape[-1]]
+
+            images.append(frame)
+            masks.append(mask)
+            metadata[img_index] = frame_meta
+
+            if imported_images == {}:
+                imported_images["Image"] = dict(images=[frame], masks=[mask], nmasks=[], classes=[], metadata={img_index: frame_meta}, )
+            else:
+                imported_images["Image"]["images"].append(frame)
+                imported_images["Image"]["masks"].append(mask)
+                imported_images["Image"]["metadata"][img_index] = frame_meta
+
+            img_index += 1
 
     imported_data = dict(imported_images=imported_images)
 
+    for i in range(len(imported_images["Image"]["images"])):
+        print(i, imported_images["Image"]["metadata"][i]["image_name"], i)
+
     return imported_data
 
 
 def read_nim_directory(self, path):
+
     if isinstance(path, list) == False:
         path = [path]
 
     if len(path) == 1:
         path = os.path.abspath(path[0])
 
         if os.path.isfile(path) == True:
@@ -513,27 +466,15 @@
     else:
         file_paths = path
 
     file_paths = [file for file in file_paths if file.split(".")[-1] == "tif"]
 
     file_names = [path.split("\\")[-1] for path in file_paths]
 
-    files = pd.DataFrame(
-        columns=[
-            "path",
-            "file_name",
-            "folder",
-            "parent_folder",
-            "posX",
-            "posY",
-            "posZ",
-            "laser",
-            "timestamp",
-        ]
-    )
+    files = pd.DataFrame(columns=["path", "file_name", "folder", "parent_folder", "posX", "posY", "posZ", "laser", "timestamp", ])
 
     for i in range(len(file_paths)):
         try:
             path = file_paths[i]
             path = os.path.abspath(path)
 
             file_name = path.split("\\")[-1]
@@ -556,53 +497,37 @@
                 timestamp = metadata["timestamp_us"]
 
                 posX, posY, posZ = metadata["StagePos_um"]
 
                 if True in laseractive:
                     laseractive = np.array(laseractive, dtype=bool)
                     laserpowers = np.array(laserpowers, dtype=float)
-                    laserwavelength_nm = np.array(
-                        laserwavelength_nm, dtype=str
-                    )
+                    laserwavelength_nm = np.array(laserwavelength_nm, dtype=str)
 
                     # finds maximum active power
                     power = laserpowers[laseractive == True].max()
 
                     laser_index = np.where(laserpowers == power)
 
                     laser = laserwavelength_nm[laser_index][0]
                 else:
                     laser = "White Light"
 
                 file_name = path.split("\\")[-1]
 
                 data = [path, file_name, posX, posY, posZ, laser, timestamp]
 
-                files.loc[len(files)] = [
-                    path,
-                    file_name,
-                    folder,
-                    parent_folder,
-                    posX,
-                    posY,
-                    posZ,
-                    laser,
-                    timestamp,
-                ]
+                files.loc[len(files)] = [path, file_name, folder, parent_folder, posX, posY, posZ, laser, timestamp, ]
 
         except:
             pass
 
-    files[["posX", "posY", "posZ"]] = files[["posX", "posY", "posZ"]].round(
-        decimals=0
-    )
-
-    files = files.sort_values(
-        by=["timestamp", "posX", "posY", "laser"], ascending=True
-    )
+    files[["posX", "posY", "posZ"]] = files[["posX", "posY", "posZ"]].round(decimals=0)
+
+    files = files.sort_values(by=["timestamp", "posX", "posY", "laser"], ascending=True)
     files = files.reset_index(drop=True)
     files["aquisition"] = 0
 
     positions = files[["posX", "posY"]].drop_duplicates()
     channels = files["laser"].drop_duplicates().to_list()
 
     acquisition = 0
@@ -649,21 +574,15 @@
 
     measurements = files.groupby(by=["aquisition"])
     channels = files["laser"].drop_duplicates().to_list()
 
     channel_num = str(len(files["laser"].unique()))
 
     if self.widget_notifications:
-        show_info(
-            "Found "
-            + str(len(measurements))
-            + " measurments in NIM Folder with "
-            + channel_num
-            + " channels."
-        )
+        show_info("Found " + str(len(measurements)) + " measurments in NIM Folder with " + channel_num + " channels.")
 
     return measurements, file_paths, channels
 
 
 def get_folder(files):
     folder = ""
     parent_folder = ""
@@ -684,27 +603,24 @@
         folder = paths[0].split("\\")[-2]
         parent_folder = paths[0].split("\\")[-3]
 
     return folder, parent_folder
 
 
 def read_image_file(path, precision="native", multiframe_mode=0, crop_mode=0):
+
     image_name = os.path.basename(path)
 
     if os.path.splitext(image_name)[1] == ".fits":
         with fits.open(path, ignore_missing_simple=True) as hdul:
             image = hdul[0].data
             try:
                 metadata = dict(hdul[0].header)
 
-                unserializable_keys = [
-                    key
-                    for key, value in metadata.items()
-                    if type(value) not in [bool, int, float, str]
-                ]
+                unserializable_keys = [key for key, value in metadata.items() if type(value) not in [bool, int, float, str]]
 
                 for key in unserializable_keys:
                     metadata.pop(key)
 
             except:
                 metadata = {}
     else:
@@ -739,45 +655,53 @@
         metadata["mask_path"] = None
         metadata["label_name"] = None
         metadata["label_path"] = None
         metadata["crop_mode"] = crop_mode
         metadata["multiframe_mode"] = multiframe_mode
         metadata["folder"] = folder
         metadata["parent_folder"] = parent_folder
-        metadata["dims"] = [image.shape[-1], image.shape[-2]]
-        metadata["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
+        metadata["dims"] = [image[0].shape[-1], image[0].shape[-2]]
+        metadata["crop"] = [0, image[0].shape[-2], 0, image[0].shape[-1]]
 
     return image, metadata
 
 
 def get_frame(img, multiframe_mode):
+
     if len(img.shape) > 2:
         if multiframe_mode == 0:
             img = img[0, :, :]
 
         elif multiframe_mode == 1:
             img = np.max(img, axis=0)
 
         elif multiframe_mode == 2:
             img = np.mean(img, axis=0).astype(np.uint16)
 
         elif multiframe_mode == 3:
             img = np.sum(img, axis=0)
 
+        elif multiframe_mode == 4:
+            img = [im for im in img]
+
+    if type(img) != list:
+        img = [img]
+
     return img
 
 
 def crop_image(img, crop_mode=0):
+
     if crop_mode != 0:
         if len(img.shape) > 2:
             imgL = img[:, :, : img.shape[-1] // 2]
-            imgR = img[:, :, img.shape[-1] // 2 :]
+            imgR = img[:, :, img.shape[-1] // 2:]
         else:
             imgL = img[:, : img.shape[-1] // 2]
-            imgR = img[:, img.shape[-1] // 2 :]
+            imgR = img[:, img.shape[-1] // 2:]
 
         if crop_mode == 1:
             img = imgL
         if crop_mode == 2:
             img = imgR
 
         if crop_mode == 3:
@@ -786,163 +710,191 @@
             else:
                 img = imgR
 
     return img
 
 
 def rescale_image(image, precision="int16"):
-    precision_dict = {
-        "int8": np.uint8,
-        "int16": np.uint16,
-        "int32": np.uint32,
-        "native": image.dtype,
-    }
+
+    precision_dict = {"int8": np.uint8, "int16": np.uint16, "int32": np.uint32, "native": image[0].dtype, }
 
     dtype = precision_dict[precision]
 
     if "int" in str(dtype):
         max_value = np.iinfo(dtype).max - 1
     else:
         max_value = np.finfo(dtype).max - 1
 
     if precision != "native":
-        image = ((image - np.min(image)) / np.max(image)) * max_value
-        image = image.astype(dtype)
+
+        for i, img in enumerate(image):
+            img = ((img - np.min(img)) / np.max(img)) * max_value
+            img = img.astype(dtype)
+            image[i] = img
 
     return image
 
 
 def read_nim_images(self, progress_callback, measurements, channels):
+
     nim_images = {}
     img_shape = (100, 100)
+    num_frames = 1
     img_type = np.uint16
     iter = 0
 
+    img_index = {}
+
     for i in range(len(measurements)):
+
         measurement = measurements.get_group(list(measurements.groups)[i])
         measurement_channels = measurement["laser"].tolist()
 
         for j in range(len(channels)):
+
             channel = channels[j]
 
+            if channel not in img_index.keys():
+                img_index[channel] = 0
+
             iter += 1
             progress = int((iter / (len(measurements) * len(channels))) * 100)
 
             try:
                 progress_callback.emit(progress)
             except:
                 pass
 
             if self.widget_notifications:
-                show_info(
-                    "loading image["
-                    + channel
-                    + "] "
-                    + str(i + 1)
-                    + " of "
-                    + str(len(measurements))
-                )
+                show_info("loading image[" + channel + "] " + str(i + 1) + " of " + str(len(measurements)))
 
             if channel in measurement_channels:
+
                 dat = measurement[measurement["laser"] == channel]
 
                 path = dat["path"].item()
                 laser = dat["laser"].item()
                 folder = dat["folder"].item()
                 parent_folder = dat["parent_folder"].item()
 
                 import_precision = self.import_precision.currentText()
                 multiframe_mode = self.import_multiframe_mode.currentIndex()
                 crop_mode = self.import_crop_mode.currentIndex()
-                img, meta = read_image_file(
-                    path, import_precision, multiframe_mode, crop_mode
-                )
 
-                contrast_limit, alpha, beta, gamma = autocontrast_values(img)
+                image_list, meta = read_image_file(path, import_precision, multiframe_mode, crop_mode)
 
-                self.active_import_mode = "NIM"
+                num_frames = len(image_list)
 
-                meta["image_name"] = os.path.basename(path)
-                meta["image_path"] = path
-                meta["folder"] = folder
-                meta["parent_folder"] = parent_folder
-                meta["akseg_hash"] = get_hash(img_path=path)
-                meta["import_mode"] = "NIM"
-                meta["contrast_limit"] = contrast_limit
-                meta["contrast_alpha"] = alpha
-                meta["contrast_beta"] = beta
-                meta["contrast_gamma"] = gamma
-                meta["dims"] = [img.shape[-1], img.shape[-2]]
-                meta["crop"] = [0, img.shape[-2], 0, img.shape[-1]]
+                akseg_hash = get_hash(img_path=path)
 
-                if meta["InstrumentSerial"] == "6D699GN6":
-                    meta["microscope"] = "BIO-NIM"
-                elif meta["InstrumentSerial"] == "2EC5XTUC":
-                    meta["microscope"] = "JR-NIM"
-                else:
-                    meta["microscope"] = None
+                file_name = os.path.basename(path)
 
-                if meta["IlluminationAngle_deg"] < 1:
-                    meta["modality"] = "Epifluorescence"
-                elif 1 < meta["IlluminationAngle_deg"] < 53:
-                    meta["modality"] = "HILO"
-                elif 53 < meta["IlluminationAngle_deg"]:
-                    meta["modality"] = "TIRF"
+                for index, frame in enumerate(image_list):
 
-                meta["light_source"] = channel
+                    frame_name = copy.deepcopy(file_name)
+                    frame_meta = copy.deepcopy(meta)
 
-                if meta["light_source"] == "White Light":
-                    meta["modality"] = "Bright Field"
+                    contrast_limit = np.percentile(frame, (1, 99))
+                    contrast_limit = [int(contrast_limit[0] * 0.5), int(contrast_limit[1] * 2), ]
 
-                img_shape = img.shape
-                img_type = np.array(img).dtype
+                    self.active_import_mode = "nim"
 
-                image_path = meta["image_path"]
+                    if len(image_list) > 1:
+                        frame_name = frame_name.replace(".", "_") + "_" + str(index) + ".tif"
 
-                if "pos_" in image_path:
-                    meta["folder"] = image_path.split("\\")[-4]
-                    meta["parent_folder"] = image_path.split("\\")[-5]
+                    self.active_import_mode = "NIM"
 
-            else:
-                img = np.zeros(img_shape, dtype=img_type)
-                meta = {}
+                    frame_meta["image_name"] = frame_name
+                    frame_meta["image_path"] = path
+                    frame_meta["folder"] = folder
+                    frame_meta["parent_folder"] = parent_folder
+                    frame_meta["akseg_hash"] = akseg_hash
+                    frame_meta["import_mode"] = "NIM"
+                    frame_meta["contrast_limit"] = contrast_limit
+                    frame_meta["contrast_alpha"] = 0
+                    frame_meta["contrast_beta"] = 0
+                    frame_meta["contrast_gamma"] = 0
+                    frame_meta["dims"] = [frame.shape[-1], frame.shape[-2]]
+                    frame_meta["crop"] = [0, frame.shape[-2], 0, frame.shape[-1]]
 
-                self.active_import_mode = "NIM"
+                    if frame_meta["InstrumentSerial"] == "6D699GN6":
+                        frame_meta["microscope"] = "BIO-NIM"
+                    elif frame_meta["InstrumentSerial"] == "2EC5XTUC":
+                        frame_meta["microscope"] = "JR-NIM"
+                    else:
+                        frame_meta["microscope"] = None
 
-                meta["image_name"] = "missing image channel"
-                meta["image_path"] = "missing image channel"
-                meta["folder"] = (None,)
-                meta["parent_folder"] = (None,)
-                meta["akseg_hash"] = None
-                meta["fov_mode"] = None
-                meta["import_mode"] = "NIM"
-                meta["contrast_limit"] = None
-                meta["contrast_alpha"] = None
-                meta["contrast_beta"] = None
-                meta["contrast_gamma"] = None
-                meta["dims"] = [img.shape[-1], img.shape[-2]]
-                meta["crop"] = [0, img.shape[-2], 0, img.shape[-1]]
-                meta["light_source"] = channel
+                    if frame_meta["IlluminationAngle_deg"] < 1:
+                        frame_meta["modality"] = "Epifluorescence"
+                    elif 1 < frame_meta["IlluminationAngle_deg"] < 53:
+                        frame_meta["modality"] = "HILO"
+                    elif 53 < frame_meta["IlluminationAngle_deg"]:
+                        frame_meta["modality"] = "TIRF"
 
-            if channel not in nim_images:
-                nim_images[channel] = dict(
-                    images=[img], masks=[], classes=[], metadata={i: meta}
-                )
+                    frame_meta["light_source"] = channel
+
+                    if frame_meta["light_source"] == "White Light":
+                        frame_meta["modality"] = "Bright Field"
+
+                    img_shape = frame.shape
+                    img_type = np.array(frame).dtype
+
+                    image_path = frame_meta["image_path"]
+
+                    if "pos_" in image_path:
+                        frame_meta["folder"] = image_path.split("\\")[-4]
+                        frame_meta["parent_folder"] = image_path.split("\\")[-5]
+
+                    if channel not in nim_images:
+                        nim_images[channel] = dict(images=[frame], masks=[], nmasks=[], classes=[], metadata={img_index[channel]: frame_meta}, )
+                    else:
+                        nim_images[channel]["images"].append(frame)
+                        nim_images[channel]["metadata"][img_index[channel]] = frame_meta
+
+                    img_index[channel] += 1
             else:
-                nim_images[channel]["images"].append(img)
-                nim_images[channel]["metadata"][i] = meta
+
+                for index in range(num_frames):
+
+                    frame = np.zeros(img_shape, dtype=img_type)
+                    frame_meta = {}
+
+                    self.active_import_mode = "NIM"
+
+                    frame_meta["image_name"] = "missing image channel"
+                    frame_meta["image_path"] = "missing image channel"
+                    frame_meta["folder"] = (None,)
+                    frame_meta["parent_folder"] = (None,)
+                    frame_meta["akseg_hash"] = None
+                    frame_meta["fov_mode"] = None
+                    frame_meta["import_mode"] = "NIM"
+                    frame_meta["contrast_limit"] = None
+                    frame_meta["contrast_alpha"] = None
+                    frame_meta["contrast_beta"] = None
+                    frame_meta["contrast_gamma"] = None
+                    frame_meta["dims"] = [frame.shape[-1], frame.shape[-2]]
+                    frame_meta["crop"] = [0, frame.shape[-2], 0, frame.shape[-1]]
+                    frame_meta["light_source"] = channel
+
+                    if channel not in nim_images:
+                        nim_images[channel] = dict(images=[frame], masks=[], nmasks=[], classes=[], metadata={img_index[channel]: frame_meta}, )
+                    else:
+                        nim_images[channel]["images"].append(frame)
+                        nim_images[channel]["metadata"][img_index[channel]] = frame_meta
+
+                    img_index[channel] += 1
 
     imported_data = dict(imported_images=nim_images)
 
     return imported_data
 
 
 def get_brightest_fov(image):
     imageL = image[0, :, : image.shape[2] // 2]
-    imageR = image[0, :, image.shape[2] // 2 :]
+    imageR = image[0, :, image.shape[2] // 2:]
 
     if np.mean(imageL) > np.mean(imageR):
         image = image[:, :, : image.shape[2] // 2]
     else:
         image = image[:, :, : image.shape[2] // 2]
 
     return image
@@ -967,15 +919,15 @@
             img = np.mean(img, axis=0).astype(np.uint16)
 
     return img
 
 
 def get_fov(img, channel_mode):
     imgL = img[:, : img.shape[1] // 2]
-    imgR = img[:, img.shape[1] // 2 :]
+    imgR = img[:, img.shape[1] // 2:]
 
     if channel_mode == 0:
         if np.mean(imgL) > np.mean(imgR):
             img = imgL
         else:
             img = imgR
     if channel_mode == 1:
@@ -1079,43 +1031,35 @@
             image_paths = image_paths[: int(import_limit)]
 
         for i in range(len(image_paths)):
             progress = int(((i + 1) / len(image_paths)) * 100)
             progress_callback.emit(progress)
 
             if self.widget_notifications:
-                show_info(
-                    "loading image "
-                    + str(i + 1)
-                    + " of "
-                    + str(len(image_paths))
-                )
+                show_info("loading image " + str(i + 1) + " of " + str(len(image_paths)))
 
             image_path = os.path.abspath(image_paths[i])
             mask_path = image_path.replace("\\images\\", "\\masks\\")
 
             image_name = image_path.split("\\")[-1]
             mask_name = mask_path.split("\\")[-1]
 
             import_precision = self.import_precision.currentText()
             multiframe_mode = self.import_multiframe_mode.currentIndex()
             crop_mode = self.import_crop_mode.currentIndex()
-            image, meta = read_image_file(
-                path, import_precision, multiframe_mode
-            )
+
+            image, meta = read_image_file(path, import_precision, multiframe_mode)
 
             crop_mode = self.import_crop_mode.currentIndex()
             image = crop_image(image, crop_mode)
 
             if os.path.exists(mask_path):
                 mask = tifffile.imread(mask_path)
                 mask = crop_image(mask, crop_mode)
-                assert (
-                    len(mask.shape) < 3
-                ), "Can only import single channel masks"
+                assert (len(mask.shape) < 3), "Can only import single channel masks"
 
             else:
                 mask_name = None
                 mask_path = None
                 mask = np.zeros(image.shape, dtype=np.uint16)
 
             contrast_limit, alpha, beta, gamma = autocontrast_values(image)
@@ -1137,20 +1081,15 @@
             meta["dims"] = [image.shape[-1], image.shape[-2]]
             meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
 
             images.append(image)
             metadata[i] = meta
 
             if imported_images == {}:
-                imported_images["Image"] = dict(
-                    images=[image],
-                    masks=[mask],
-                    classes=[],
-                    metadata={i: meta},
-                )
+                imported_images["Image"] = dict(images=[image], masks=[mask], nmasks=[], classes=[], metadata={i: meta}, )
             else:
                 imported_images["Image"]["images"].append(image)
                 imported_images["Image"]["masks"].append(mask)
                 imported_images["Image"]["metadata"][i] = meta
 
     imported_data = dict(imported_images=imported_images)
 
@@ -1182,48 +1121,36 @@
             image_paths = image_paths[: int(import_limit)]
 
         for i in range(len(image_paths)):
             progress = int(((i + 1) / len(image_paths)) * 100)
             progress_callback.emit(progress)
 
             if self.widget_notifications:
-                show_info(
-                    "loading image "
-                    + str(i + 1)
-                    + " of "
-                    + str(len(image_paths))
-                )
+                show_info("loading image " + str(i + 1) + " of " + str(len(image_paths)))
 
             image_path = os.path.abspath(image_paths[i])
-            json_path = image_path.replace("\\images\\", "\\json\\").replace(
-                ".tif", ".txt"
-            )
+            json_path = image_path.replace("\\images\\", "\\json\\").replace(".tif", ".txt")
 
             import_precision = self.import_precision.currentText()
-            image, meta_stack = read_image_file(
-                path, import_precision, multiframe_mode=0
-            )
+            image, meta_stack = read_image_file(path, import_precision, multiframe_mode=0)
 
             crop_mode = self.import_crop_mode.currentIndex()
             image = crop_image(image, crop_mode)
 
             if os.path.exists(json_path):
                 from napari_bacseg._utils_json import import_coco_json
 
-                mask, label = import_coco_json(json_path)
+                mask, nmask, label = import_coco_json(json_path)
                 mask = crop_image(mask, crop_mode)
                 label = crop_image(label, crop_mode)
 
             else:
-                label = np.zeros(
-                    (image.shape[0], image.shape[1]), dtype=np.uint16
-                )
-                mask = np.zeros(
-                    (image.shape[0], image.shape[1]), dtype=np.uint16
-                )
+                label = np.zeros((image.shape[0], image.shape[1]), dtype=np.uint16)
+                mask = np.zeros((image.shape[0], image.shape[1]), dtype=np.uint16)
+                nmask = np.zeros((image.shape[0], image.shape[1]), dtype=np.uint16)
 
             for j, channel in enumerate(meta_stack["channels"]):
                 img = image[j, :, :]
 
                 contrast_limit, alpha, beta, gamma = autocontrast_values(img)
 
                 self.active_import_mode = "BacSeg"
@@ -1234,136 +1161,141 @@
                 meta["contrast_alpha"] = alpha
                 meta["contrast_beta"] = beta
                 meta["contrast_gamma"] = gamma
                 meta["dims"] = [img.shape[0], img.shape[1]]
                 meta["crop"] = [0, img.shape[1], 0, img.shape[0]]
 
                 if channel not in imported_images.keys():
-                    imported_images[channel] = dict(
-                        images=[img],
-                        masks=[mask],
-                        classes=[label],
-                        metadata={i: meta},
-                    )
+                    imported_images[channel] = dict(images=[img], masks=[mask], nmasks=[], classes=[label], metadata={i: meta}, )
                 else:
                     imported_images[channel]["images"].append(img)
                     imported_images[channel]["masks"].append(mask)
+                    imported_images[channel]["nmasks"].append(nmask)
                     imported_images[channel]["classes"].append(label)
                     imported_images[channel]["metadata"][i] = meta
 
     akmeta = meta_stack
     akmeta.pop("layer_meta")
 
     imported_data = dict(imported_images=imported_images, akmeta=akmeta)
 
     return imported_data
 
 
 def import_images(self, progress_callback, file_paths):
+
     if os.path.isdir(file_paths[0]):
         file_paths = glob(file_paths[0] + r"**\*", recursive=True)
 
     image_formats = ["tif", "png", "jpeg", "fits"]
 
-    file_paths = [
-        path for path in file_paths if path.split(".")[-1] in image_formats
-    ]
+    file_paths = [path for path in file_paths if path.split(".")[-1] in image_formats]
 
     import_limit = self.import_limit.currentText()
 
     if import_limit != "None" and len(file_paths) > int(import_limit):
         file_paths = file_paths[: int(import_limit)]
 
     images = []
     metadata = {}
     imported_images = {}
 
+    img_index = 0
+
     for i in range(len(file_paths)):
+
         progress = int(((i + 1) / len(file_paths)) * 100)
 
         try:
             progress_callback.emit(progress)
         except:
             pass
+
         if self.widget_notifications:
-            show_info(
-                "loading image " + str(i + 1) + " of " + str(len(file_paths))
-            )
+            show_info("loading image " + str(i + 1) + " of " + str(len(file_paths)))
 
         file_path = os.path.abspath(file_paths[i])
         file_name = os.path.basename(file_path)
 
         import_precision = self.import_precision.currentText()
         multiframe_mode = self.import_multiframe_mode.currentIndex()
         crop_mode = self.import_crop_mode.currentIndex()
 
-        image, meta = read_image_file(
-            file_path, import_precision, multiframe_mode, crop_mode
-        )
-
-        contrast_limit, alpha, beta, gamma = autocontrast_values(image)
-
-        self.active_import_mode = "image"
-
-        meta["akseg_hash"] = get_hash(img_path=file_path)
-        meta["image_name"] = file_name
-        meta["image_path"] = file_path
-        meta["mask_name"] = None
-        meta["mask_path"] = None
-        meta["label_name"] = None
-        meta["label_path"] = None
-        meta["import_mode"] = "image"
-        meta["contrast_limit"] = contrast_limit
-        meta["contrast_alpha"] = alpha
-        meta["contrast_beta"] = beta
-        meta["contrast_gamma"] = gamma
-        meta["dims"] = [image.shape[-1], image.shape[-2]]
-        meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
+        image_list, meta = read_image_file(file_path, import_precision, multiframe_mode, crop_mode)
 
-        images.append(image)
-        metadata[i] = meta
+        akseg_hash = get_hash(img_path=file_path)
 
-        if imported_images == {}:
-            imported_images["Image"] = dict(
-                images=[image], masks=[], classes=[], metadata={i: meta}
-            )
-        else:
-            imported_images["Image"]["images"].append(image)
-            imported_images["Image"]["metadata"][i] = meta
+        file_name = os.path.basename(file_path)
+
+        for index, frame in enumerate(image_list):
+
+            contrast_limit = np.percentile(frame, (1, 99))
+            contrast_limit = [int(contrast_limit[0] * 0.5), int(contrast_limit[1] * 2), ]
+
+            self.active_import_mode = "image"
+
+            if len(image_list) > 1:
+                frame_name = file_name.replace(".", "_") + "_" + str(index) + ".tif"
+            else:
+                frame_name = copy.deepcopy(file_name)
+
+            frame_meta = copy.deepcopy(meta)
+
+            frame_meta["akseg_hash"] = akseg_hash
+            frame_meta["image_name"] = frame_name
+            frame_meta["image_path"] = file_path
+            frame_meta["mask_name"] = None
+            frame_meta["mask_path"] = None
+            frame_meta["label_name"] = None
+            frame_meta["label_path"] = None
+            frame_meta["import_mode"] = "image"
+            frame_meta["contrast_limit"] = contrast_limit
+            frame_meta["contrast_alpha"] = 0
+            frame_meta["contrast_beta"] = 0
+            frame_meta["contrast_gamma"] = 0
+            frame_meta["dims"] = [frame.shape[-1], frame.shape[-2]]
+            frame_meta["crop"] = [0, frame.shape[-2], 0, frame.shape[-1]]
+
+            images.append(frame)
+            metadata[i] = frame_meta
+
+            if imported_images == {}:
+                imported_images["Image"] = dict(images=[frame], masks=[], nmasks=[], classes=[], metadata={img_index: frame_meta}, )
+            else:
+                imported_images["Image"]["images"].append(frame)
+                imported_images["Image"]["metadata"][img_index] = frame_meta
+
+            img_index += 1
 
     imported_data = dict(imported_images=imported_images)
 
     return imported_data
 
 
 def import_cellpose(self, progress_callback, file_paths):
     if os.path.isdir(file_paths[0]):
         file_paths = glob(file_paths[0] + r"**\*", recursive=True)
 
     image_formats = ["npy"]
 
-    file_paths = [
-        path for path in file_paths if path.split(".")[-1] in image_formats
-    ]
+    file_paths = [path for path in file_paths if path.split(".")[-1] in image_formats]
 
     import_limit = self.import_limit.currentText()
 
     if import_limit != "None" and len(file_paths) > int(import_limit):
         file_paths = file_paths[: int(import_limit)]
 
     imported_images = {}
 
     for i in range(len(file_paths)):
         progress = int(((i + 1) / len(file_paths)) * 100)
         progress_callback.emit(progress)
 
         if self.widget_notifications:
-            show_info(
-                "loading image " + str(i + 1) + " of " + str(len(file_paths))
-            )
+            show_info("loading image " + str(i + 1) + " of " + str(len(file_paths)))
 
         file_path = os.path.abspath(file_paths[i])
         file_name = file_path.split("\\")[-1]
 
         dat = np.load(file_path, allow_pickle=True).item()
 
         mask = dat["masks"]
@@ -1372,17 +1304,15 @@
         image_path = file_path.replace("_seg.npy", ".tif")
 
         if os.path.exists(image_path):
             image_name = image_path.split("\\")[-1]
 
             import_precision = self.import_precision.currentText()
             multiframe_mode = self.import_multiframe_mode.currentIndex()
-            img, meta = read_image_file(
-                image_path, import_precision, multiframe_mode
-            )
+            img, meta = read_image_file(image_path, import_precision, multiframe_mode)
 
             crop_mode = self.import_crop_mode.currentIndex()
             img = crop_image(img, crop_mode)
             mask = crop_image(mask, crop_mode)
 
             contrast_limit, alpha, beta, gamma = autocontrast_values(img)
 
@@ -1409,37 +1339,19 @@
             contrast_limit, alpha, beta, gamma = autocontrast_values(image)
 
             self.active_import_mode = "cellpose"
 
             folder = os.path.abspath(file_path).split("\\")[-2]
             parent_folder = os.path.abspath(file_path).split("\\")[-3]
 
-            meta = dict(
-                image_name=file_name,
-                image_path=file_path,
-                mask_name=file_name,
-                mask_path=file_path,
-                label_name=None,
-                label_path=None,
-                folder=folder,
-                parent_folder=parent_folder,
-                contrast_limit=contrast_limit,
-                contrast_alpha=alpha,
-                contrast_beta=beta,
-                contrast_gamma=gamma,
-                akseg_hash=get_hash(img_path=file_path),
-                import_mode="cellpose",
-                dims=[image.shape[0], image.shape[1]],
-                crop=[0, image.shape[1], 0, image.shape[0]],
-            )
+            meta = dict(image_name=file_name, image_path=file_path, mask_name=file_name, mask_path=file_path, label_name=None, label_path=None, folder=folder, parent_folder=parent_folder, contrast_limit=contrast_limit, contrast_alpha=alpha, contrast_beta=beta, contrast_gamma=gamma, akseg_hash=get_hash(img_path=file_path), import_mode="cellpose", dims=[
+                image.shape[0], image.shape[1]], crop=[0, image.shape[1], 0, image.shape[0]], )
 
         if imported_images == {}:
-            imported_images["Image"] = dict(
-                images=[img], masks=[mask], classes=[], metadata={i: meta}
-            )
+            imported_images["Image"] = dict(images=[img], masks=[mask], nmasks=[], classes=[], metadata={i: meta}, )
         else:
             imported_images["Image"]["images"].append(img)
             imported_images["Image"]["masks"].append(mask)
             imported_images["Image"]["metadata"][i] = meta
 
     imported_data = dict(imported_images=imported_images)
 
@@ -1448,28 +1360,24 @@
 
 def import_oufti(self, progress_callback, file_paths):
     if os.path.isdir(file_paths[0]):
         file_paths = glob(file_paths[0] + r"**\*", recursive=True)
 
     image_formats = ["mat"]
 
-    file_paths = [
-        path for path in file_paths if path.split(".")[-1] in image_formats
-    ]
+    file_paths = [path for path in file_paths if path.split(".")[-1] in image_formats]
 
     file_path = os.path.abspath(file_paths[0])
     parent_dir = file_path.replace(file_path.split("\\")[-1], "")
 
     mat_paths = file_paths
     image_paths = glob(parent_dir + r"**\*", recursive=True)
 
     image_formats = ["tif"]
-    image_paths = [
-        path for path in image_paths if path.split(".")[-1] in image_formats
-    ]
+    image_paths = [path for path in image_paths if path.split(".")[-1] in image_formats]
 
     mat_files = [path.split("\\")[-1] for path in mat_paths]
     image_files = [path.split("\\")[-1] for path in image_paths]
 
     matching_image_paths = []
     matching_mat_paths = []
 
@@ -1496,17 +1404,15 @@
             image_files = [matching_image_paths[index]]
             mat_files = [matching_mat_paths[index]]
 
         else:
             if self.widget_notifications:
                 show_info("Matching image/mesh files could not be found")
             self.viewer.text_overlay.visible = True
-            self.viewer.text_overlay.text = (
-                "Matching image/mesh files could not be found"
-            )
+            self.viewer.text_overlay.text = ("Matching image/mesh files could not be found")
 
     else:
         image_files = matching_image_paths
         mat_files = matching_mat_paths
 
     import_limit = self.import_limit.currentText()
 
@@ -1517,20 +1423,15 @@
 
     for i in range(len(mat_files)):
         try:
             progress = int(((i + 1) / len(mat_files)) * 100)
             progress_callback.emit(progress)
 
             if self.widget_notifications:
-                show_info(
-                    "loading image "
-                    + str(i + 1)
-                    + " of "
-                    + str(len(mat_files))
-                )
+                show_info("loading image " + str(i + 1) + " of " + str(len(mat_files)))
 
             mat_path = mat_files[i]
             image_path = image_files[i]
 
             image_name = image_path.split("\\")[-1]
             mat_name = mat_path.split("\\")[-1]
 
@@ -1556,20 +1457,15 @@
             meta["contrast_alpha"] = alpha
             meta["contrast_beta"] = beta
             meta["contrast_gamma"] = gamma
             meta["dims"] = [image.shape[-1], image.shape[-2]]
             meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
 
             if imported_images == {}:
-                imported_images["Image"] = dict(
-                    images=[image],
-                    masks=[mask],
-                    classes=[],
-                    metadata={i: meta},
-                )
+                imported_images["Image"] = dict(images=[image], masks=[mask], nmasks=[], classes=[], metadata={i: meta}, )
             else:
                 imported_images["Image"]["images"].append(image)
                 imported_images["Image"]["masks"].append(mask)
                 imported_images["Image"]["metadata"][i] = meta
 
         except:
             pass
@@ -1579,17 +1475,15 @@
     return imported_data
 
 
 def import_mat_data(self, image_path, mat_path):
     import_precision = self.import_precision.currentText()
     multiframe_mode = self.import_multiframe_mode.currentIndex()
     crop_mode = self.import_crop_mode.currentIndex()
-    image, meta = read_image_file(
-        image_path, import_precision, multiframe_mode
-    )
+    image, meta = read_image_file(image_path, import_precision, multiframe_mode)
 
     mat_data = mat4py.loadmat(mat_path)
 
     mat_data = mat_data["cellList"]
 
     contours = []
 
@@ -1606,41 +1500,34 @@
 
         cv2.drawContours(mask, [cnt], -1, i + 1, -1)
 
     return image, mask, meta
 
 
 def unstack_images(stack, axis=0):
-    images = [
-        np.squeeze(e, axis)
-        for e in np.split(stack, stack.shape[axis], axis=axis)
-    ]
+    images = [np.squeeze(e, axis) for e in np.split(stack, stack.shape[axis], axis=axis)]
 
     return images
 
 
-def append_image_stacks(
-    current_metadata, new_metadata, current_image_stack, new_image_stack
-):
+def append_image_stacks(current_metadata, new_metadata, current_image_stack, new_image_stack):
     current_image_stack = unstack_images(current_image_stack)
 
     new_image_stack = unstack_images(new_image_stack)
 
     appended_image_stack = current_image_stack + new_image_stack
 
     appended_metadata = current_metadata
 
     for key, value in new_metadata.items():
         new_key = max(appended_metadata.keys()) + 1
 
         appended_metadata[new_key] = value
 
-    appended_image_stack, appended_metadata = stack_images(
-        appended_image_stack, appended_metadata
-    )
+    appended_image_stack, appended_metadata = stack_images(appended_image_stack, appended_metadata)
 
     return appended_image_stack, appended_metadata
 
 
 def append_metadata(current_metadata, new_metadata):
     appended_metadata = current_metadata
 
@@ -1649,27 +1536,23 @@
 
         appended_metadata[new_key] = value
 
         return appended_metadata
 
 
 def read_ak_metadata(self):
-    meta_path = os.path.join(
-        self.database_path, "Metadata", "AKSEG Metadata.xlsx"
-    )
+    meta_path = os.path.join(self.database_path, "Metadata", "AKSEG Metadata.xlsx")
 
     ak_meta = pd.read_excel(meta_path)
 
     user_initials = list(ak_meta["User Initials"].dropna())
     microscope = list(ak_meta["Microscope"].dropna())
     modality = list(ak_meta["Image Modality"].dropna())
 
-    ak_meta = dict(
-        user_initials=user_initials, microscope=microscope, modality=modality
-    )
+    ak_meta = dict(user_initials=user_initials, microscope=microscope, modality=modality)
 
     return ak_meta
 
 
 def get_hash(img_path=None, img=None):
     if img is not None:
         img_path = tempfile.TemporaryFile(suffix=".tif").name
@@ -1680,19 +1563,15 @@
 
         hash_code = hashlib.sha256(bytes).hexdigest()
 
         return hash_code
 
 
 def align_image_channels(self):
-    layer_names = [
-        layer.name
-        for layer in self.viewer.layers
-        if layer.name not in ["Segmentations", "Classes", "center_lines"]
-    ]
+    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
     if self.import_align.isChecked() and len(layer_names) > 1:
         primary_image = layer_names[-1]
 
         layer_names.remove(primary_image)
 
         dim_range = int(self.viewer.dims.range[0][1])
@@ -1700,17 +1579,15 @@
         for i in range(dim_range):
             img = self.viewer.layers[primary_image].data[i, :, :]
 
             for layer in layer_names:
                 shifted_img = self.viewer.layers[layer].data[i, :, :]
 
                 try:
-                    shift, error, diffphase = phase_cross_correlation(
-                        img, shifted_img, upsample_factor=100
-                    )
+                    shift, error, diffphase = phase_cross_correlation(img, shifted_img, upsample_factor=100)
                     shifted_img = scipy.ndimage.shift(shifted_img, shift)
 
                 except:
                     pass
 
                 self.viewer.layers[layer].data[i, :, :] = shifted_img
 
@@ -1756,19 +1633,15 @@
                 label_id = np.unique(label[cnt_mask == 255])[0]
 
                 if label_id in export_labels:
                     new_mask_id = np.max(np.unique(export_mask)) + 1
                     export_mask[cnt_mask == 255] = new_mask_id
                     export_label[cnt_mask == 255] = label_id
 
-                    cnt, _ = cv2.findContours(
-                        cnt_mask.astype(np.uint8),
-                        cv2.RETR_EXTERNAL,
-                        cv2.CHAIN_APPROX_NONE,
-                    )
+                    cnt, _ = cv2.findContours(cnt_mask.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE, )
 
                     contours.append(cnt[0])
 
         export_mask_stack[i, :, :][y1:y2, x1:x2] = export_mask
         export_label_stack[i, :, :][y1:y2, x1:x2] = export_label
         export_contours[i] = contours
 
@@ -1777,17 +1650,15 @@
 
 def import_JSON(self, progress_callback, file_paths):
     if os.path.isdir(file_paths[0]):
         file_paths = glob(file_paths[0] + r"**\*", recursive=True)
 
     image_formats = ["txt"]
 
-    json_paths = [
-        path for path in file_paths if path.split(".")[-1] in image_formats
-    ]
+    json_paths = [path for path in file_paths if path.split(".")[-1] in image_formats]
 
     file_path = os.path.abspath(file_paths[0])
     parent_dir = file_path.replace(file_path.split("\\")[-1], "")
 
     image_paths = glob(parent_dir + "*.tif", recursive=True)
 
     json_files = [path.split("\\")[-1] for path in json_paths]
@@ -1826,17 +1697,15 @@
             json_files = [matching_json_paths[index]]
 
         else:
             if self.widget_notifications:
                 show_info("Matching image/mesh files could not be found")
 
             self.viewer.text_overlay.visible = True
-            self.viewer.text_overlay.text = (
-                "Matching image/mesh files could not be found"
-            )
+            self.viewer.text_overlay.text = ("Matching image/mesh files could not be found")
 
     else:
         image_files = matching_image_paths
         json_files = matching_json_paths
 
     imported_images = {}
 
@@ -1845,41 +1714,35 @@
 
     for i in range(len(json_files)):
         try:
             progress = int(((i + 1) / len(json_files)) * 100)
             progress_callback.emit(progress)
 
             if self.widget_notifications:
-                show_info(
-                    "loading image "
-                    + str(i + 1)
-                    + " of "
-                    + str(len(json_files))
-                )
+                show_info("loading image " + str(i + 1) + " of " + str(len(json_files)))
 
             json_path = json_files[i]
             image_path = image_files[i]
 
             image_name = image_path.split("\\")[-1]
             json_name = json_path.split("\\")[-1]
 
             import_precision = self.import_precision.currentText()
             multiframe_mode = self.import_multiframe_mode.currentIndex()
             crop_mode = self.import_crop_mode.currentIndex()
-            image, meta = read_image_file(
-                image_path, import_precision, multiframe_mode
-            )
+            image, meta = read_image_file(image_path, import_precision, multiframe_mode)
 
             from napari_bacseg._utils_json import import_coco_json
 
-            mask, labels = import_coco_json(json_path)
+            mask, nmask, labels = import_coco_json(json_path)
 
             crop_mode = self.import_crop_mode.currentIndex()
             image = crop_image(image, crop_mode)
             mask = crop_image(mask, crop_mode)
+            nmask = crop_image(nmask, crop_mode)
             labels = crop_image(labels, crop_mode)
 
             contrast_limit, alpha, beta, gamma = autocontrast_values(image)
 
             self.active_import_mode = "JSON"
 
             meta["akseg_hash"] = get_hash(img_path=image_path)
@@ -1894,23 +1757,19 @@
             meta["contrast_alpha"] = alpha
             meta["contrast_beta"] = beta
             meta["contrast_gamma"] = gamma
             meta["dims"] = [image.shape[-1], image.shape[-2]]
             meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
 
             if imported_images == {}:
-                imported_images["Image"] = dict(
-                    images=[image],
-                    masks=[mask],
-                    classes=[labels],
-                    metadata={i: meta},
-                )
+                imported_images["Image"] = dict(images=[image], masks=[mask], nmasks=[nmask], classes=[labels], metadata={i: meta}, )
             else:
                 imported_images["Image"]["images"].append(image)
                 imported_images["Image"]["masks"].append(mask)
+                imported_images["Image"]["nmasks"].append(nmask)
                 imported_images["Image"]["classes"].append(labels)
                 imported_images["Image"]["metadata"][i] = meta
 
         except:
             pass
 
     imported_data = dict(imported_images=imported_images)
@@ -1943,15 +1802,15 @@
     for i in a:
         b.append(b[-1] + i)
     return np.array(b)
 
 
 def autocontrast_values(image, clip_hist_percent=0.001):
     # calculate histogram
-    hist, bin_edges = np.histogram(image, bins=(2**16) - 1)
+    hist, bin_edges = np.histogram(image, bins=(2 ** 16) - 1)
     hist_size = len(hist)
 
     # calculate cumulative distribution from the histogram
     accumulator = cumsum(hist)
 
     # Locate points to clip
     maximum = accumulator[-1]
@@ -1995,39 +1854,32 @@
         contrast_limit = [np.min(image), np.max(image)]
 
     return contrast_limit, alpha, beta, gamma
 
 
 def import_masks(self, file_paths, file_extension=""):
     mask_stack = self.segLayer.data.copy()
+    nmask_stack = self.nucLayer.data.copy()
     class_stack = self.classLayer.data.copy()
 
     if os.path.isdir(file_paths[0]):
         file_paths = os.path.abspath(file_paths[0])
         import_folder = file_paths
 
     if os.path.isfile(file_paths[0]):
         file_paths = os.path.abspath(file_paths[0])
         import_folder = file_paths.replace(file_paths.split("\\")[-1], "")
 
     import_folder = os.path.abspath(import_folder)
-    mask_paths = glob(
-        import_folder + r"**\**\*" + file_extension, recursive=True
-    )
+    mask_paths = glob(import_folder + r"**\**\*" + file_extension, recursive=True)
 
     mask_files = [path.split("\\")[-1] for path in mask_paths]
-    mask_search = [
-        file.split(file.split(".")[-1])[0][:-1] for file in mask_files
-    ]
-
-    layer_names = [
-        layer.name
-        for layer in self.viewer.layers
-        if layer.name not in ["Segmentations", "Classes", "center_lines"]
-    ]
+    mask_search = [file.split(file.split(".")[-1])[0][:-1] for file in mask_files]
+
+    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
     matching_masks = []
 
     for layer in layer_names:
         image_stack = self.viewer.layers[layer].data
         meta_stack = self.viewer.layers[layer].metadata
 
@@ -2057,19 +1909,21 @@
             mask = tifffile.imread(mask_path)
             mask_stack[i, :, :][y1:y2, x1:x2] = mask
             self.segLayer.data = mask_stack.astype(np.uint16)
 
         if file_format == "txt":
             from napari_bacseg._utils_json import import_coco_json
 
-            mask, label = import_coco_json(mask_path)
+            mask, nmask, label = import_coco_json(mask_path)
             mask_stack[i, :, :][y1:y2, x1:x2] = mask
+            nmask_stack[i, :, :][y1:y2, x1:x2] = nmask
             class_stack[i, :, :][y1:y2, x1:x2] = label
 
             self.segLayer.data = mask_stack.astype(np.uint16)
+            self.nucLayer.data = nmask_stack.astype(np.uint16)
             self.classLayer.data = class_stack.astype(np.uint16)
 
         if file_format == "npy":
             dat = np.load(mask_path, allow_pickle=True).item()
 
             mask = dat["masks"]
             mask = mask.astype(np.uint16)
@@ -2118,32 +1972,28 @@
                 label_id = np.unique(label[cnt_mask == 255])[0]
 
                 if label_id in export_labels:
                     new_mask_id = np.max(np.unique(export_mask)) + 1
                     export_mask[cnt_mask == 255] = new_mask_id
                     export_label[cnt_mask == 255] = label_id
 
-                    cnt, _ = cv2.findContours(
-                        cnt_mask.astype(np.uint8),
-                        cv2.RETR_EXTERNAL,
-                        cv2.CHAIN_APPROX_NONE,
-                    )
+                    cnt, _ = cv2.findContours(cnt_mask.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE, )
 
                     contours.append(cnt[0])
 
         except:
             pass
 
     return contours
 
 
 def automatic_brightness_and_contrast(image, clip_hist_percent=0.1):
     if np.max(image) > 0:
         # Calculate grayscale histogram
-        hist = cv2.calcHist([image], [0], None, [2**16], [0, 2**16])
+        hist = cv2.calcHist([image], [0], None, [2 ** 16], [0, 2 ** 16])
         hist_size = len(hist)
 
         # Calculate cumulative distribution from the histogram
         accumulator = []
         accumulator.append(float(hist[0]))
         for index in range(1, hist_size):
             accumulator.append(accumulator[index - 1] + float(hist[index]))
@@ -2168,24 +2018,15 @@
         beta = -minimum_gray * alpha
 
         image = cv2.convertScaleAbs(image, alpha=alpha, beta=beta)
 
     return image
 
 
-def add_scale_bar(
-    image,
-    pixel_resolution=100,
-    pixel_resolution_units="nm",
-    scalebar_size=20,
-    scalebar_size_units="um",
-    scalebar_colour="white",
-    scalebar_thickness=10,
-    scalebar_margin=10,
-):
+def add_scale_bar(image, pixel_resolution=100, pixel_resolution_units="nm", scalebar_size=20, scalebar_size_units="um", scalebar_colour="white", scalebar_thickness=10, scalebar_margin=10, ):
     try:
         if float(pixel_resolution) > 0 and float(scalebar_size) > 0:
             h, w = image.shape
 
             pixel_resolution = float(pixel_resolution)
             scalebar_size = float(scalebar_size)
 
@@ -2197,69 +2038,39 @@
                 rescaled_pixel_resolution = pixel_resolution
 
             if scalebar_size_units != "nm":
                 rescaled_scalebar_size = scalebar_size * 1000
             else:
                 rescaled_scalebar_size = scalebar_size
 
-            scalebar_len = int(
-                rescaled_scalebar_size / rescaled_pixel_resolution
-            )
+            scalebar_len = int(rescaled_scalebar_size / rescaled_pixel_resolution)
 
             if scalebar_len > 0 and scalebar_len < w:
                 if scalebar_colour == "White":
                     bit_depth = str(image.dtype)
                     bit_depth = int(bit_depth.replace("uint", ""))
-                    colour = (2**bit_depth) - 1
+                    colour = (2 ** bit_depth) - 1
                 else:
                     colour = 0
 
-                scalebar_pos = (
-                    w - scalebar_margin - scalebar_len,
-                    h - scalebar_margin - int(scalebar_thickness),
-                )  # Position of the scale bar in the image (in pixels)
-
-                image = cv2.rectangle(
-                    image,
-                    scalebar_pos,
-                    (
-                        scalebar_pos[0] + scalebar_len,
-                        scalebar_pos[1] + int(scalebar_thickness),
-                    ),
-                    colour,
-                    -1,
-                )
+                scalebar_pos = (w - scalebar_margin - scalebar_len, h - scalebar_margin - int(scalebar_thickness),)  # Position of the scale bar in the image (in pixels)
+
+                image = cv2.rectangle(image, scalebar_pos, (scalebar_pos[0] + scalebar_len, scalebar_pos[1] + int(scalebar_thickness),), colour, -1, )
 
             else:
-                show_info(
-                    f"{int(scalebar_size)} ({scalebar_size_units}) Scale bar is too large for the {(rescaled_pixel_resolution/1000)*w}x{(rescaled_pixel_resolution/1000)*h} (um) image"
-                )
+                show_info(f"{int(scalebar_size)} ({scalebar_size_units}) Scale bar is too large for the {(rescaled_pixel_resolution / 1000) * w}x{(rescaled_pixel_resolution / 1000) * h} (um) image")
 
     except:
         print(traceback.format_exc())
 
     return image
 
 
-def generate_export_image(
-    self,
-    export_channel,
-    dim,
-    normalize=False,
-    invert=False,
-    autocontrast=False,
-    scalebar=False,
-    cropzoom=False,
-    mask_background=False,
-):
-    layer_names = [
-        layer.name
-        for layer in self.viewer.layers
-        if layer.name not in ["Segmentations", "Classes", "center_lines"]
-    ]
+def generate_export_image(self, export_channel, dim, normalize=False, invert=False, autocontrast=False, scalebar=False, cropzoom=False, mask_background=False, ):
+    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
     layer_names.reverse()
 
     if export_channel == "All Channels (Stack)":
         mode = "stack"
     elif export_channel == "First Three Channels (RGB)":
         mode = "rgb"
@@ -2267,38 +2078,41 @@
         mode = "single"
         layer_names = [export_channel]
 
     if mode == "rgb":
         layer_names = layer_names[:3]
 
     mask = self.segLayer.data
+    nmask = self.nucLayer.data
     label = self.classLayer.data
     metadata = self.viewer.layers[layer_names[0]].metadata
 
     mask = mask[dim]
+    nmask = nmask[dim]
     label = label[dim]
     metadata = metadata[dim[0]]
 
     if cropzoom:
         layer = self.viewer.layers[layer_names[0]]
         crop = layer.corner_pixels.T
         y_range = crop[-2]
         x_range = crop[-1]
-        mask = mask[y_range[0] : y_range[1], x_range[0] : x_range[1]]
-        label = label[y_range[0] : y_range[1], x_range[0] : x_range[1]]
+        mask = mask[y_range[0]: y_range[1], x_range[0]: x_range[1]]
+        nmask = nmask[y_range[0]: y_range[1], x_range[0]: x_range[1]]
+        label = label[y_range[0]: y_range[1], x_range[0]: x_range[1]]
 
     image = []
 
     for layer in layer_names:
         img = self.viewer.layers[layer].data.copy()
 
         img = img[dim]
 
         if cropzoom:
-            img = img[y_range[0] : y_range[1], x_range[0] : x_range[1]]
+            img = img[y_range[0]: y_range[1], x_range[0]: x_range[1]]
 
         if mask_background:
             img[mask == 0] = 0
 
         if invert:
             img = cv2.bitwise_not(img)
 
@@ -2306,71 +2120,165 @@
             img = normalize99(img)
 
         if autocontrast:
             img = automatic_brightness_and_contrast(img)
 
         if scalebar:
             pixel_resolution = self.export_scalebar_resolution.text()
-            pixel_resolution_units = (
-                self.export_scalebar_resolution_units.currentText()
-            )
+            pixel_resolution_units = (self.export_scalebar_resolution_units.currentText())
             scalebar_size = self.export_scalebar_size.text()
             scalebar_size_units = self.export_scalebar_size_units.currentText()
             scalebar_colour = self.export_scalebar_colour.currentText()
             scalebar_thickness = self.export_scalebar_thickness.currentText()
 
-            img = add_scale_bar(
-                img,
-                pixel_resolution=pixel_resolution,
-                pixel_resolution_units=pixel_resolution_units,
-                scalebar_size=scalebar_size,
-                scalebar_size_units=scalebar_size_units,
-                scalebar_colour=scalebar_colour,
-                scalebar_thickness=scalebar_thickness,
-            )
+            img = add_scale_bar(img, pixel_resolution=pixel_resolution, pixel_resolution_units=pixel_resolution_units, scalebar_size=scalebar_size, scalebar_size_units=scalebar_size_units, scalebar_colour=scalebar_colour, scalebar_thickness=scalebar_thickness, )
 
         image.append(img)
 
     if mode == "rgb":
         while len(image) < 3:
             blank = np.zeros(img.shape, dtype=img.dtype)
 
             if scalebar:
-                blank = add_scale_bar(
-                    blank,
-                    pixel_resolution=pixel_resolution,
-                    pixel_resolution_units=pixel_resolution_units,
-                    scalebar_size=scalebar_size,
-                    scalebar_size_units=scalebar_size_units,
-                    scalebar_colour=scalebar_colour,
-                    scalebar_thickness=scalebar_thickness,
-                )
+                blank = add_scale_bar(blank, pixel_resolution=pixel_resolution, pixel_resolution_units=pixel_resolution_units, scalebar_size=scalebar_size, scalebar_size_units=scalebar_size_units, scalebar_colour=scalebar_colour, scalebar_thickness=scalebar_thickness, )
 
             image.append(blank)
 
     if mode == "rgb":
         image = np.stack(image, axis=-1)
 
         image = rescale01(image)
-        image = image * (2**16 - 1)
+        image = image * (2 ** 16 - 1)
         image = image.astype(np.uint16)
 
     elif mode == "stack":
         image = np.stack(image, axis=0)
     else:
         image = image[0]
 
-    return image, mask, label, metadata, mode
+    return image, mask, nmask, label, metadata, mode
+
+
+def export_stacks(self, progress_callback, mode):
+
+    try:
+
+        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+
+        export_stack_channel = self.export_stack_channel.currentText()
+        export_stack_mode = self.export_stack_mode.currentText()
+        export_stack_modifier = self.export_stack_modifier.text()
+
+        if mode == "active":
+            export_channels = [self.export_stack_channel.currentText()]
+        else:
+            export_channels = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+
+        overwrite = self.export_stack_overwrite_setting.isChecked()
+        export_images = self.export_stack_image_setting.isChecked()
+
+        normalise = self.export_normalise.isChecked()
+        invert = self.export_invert.isChecked()
+        autocontrast = self.export_autocontrast.isChecked()
+        scalebar = self.export_scalebar.isChecked()
+        cropzoom = self.export_cropzoom.isChecked()
+        mask_background = self.export_mask_background.isChecked()
+
+        for channel in export_channels:
+
+            image_stack = []
+            mask_stack = []
+
+            dims = self.viewer.layers[channel].data.shape[0]
+
+            for dim in range(dims):
+
+                progress_callback.emit(int((dim / (dims-1)) * 100))
+
+                image, mask, nmask, label, meta, mode = generate_export_image(
+                    self, channel, (dim,),
+                    normalise, invert, autocontrast,
+                    scalebar,
+                    cropzoom, mask_background,
+                )
+
+                if len(image.shape) > 2:
+                    image = image[0]
+                    mask = mask[0]
+
+                image_stack.append(image)
+                mask_stack.append(mask)
+
+            image_stack = np.stack(image_stack, axis=0)
+            mask_stack = np.stack(mask_stack, axis=0)
+
+            file_name = meta["image_name"]
+
+            if "image_path" in meta.keys():
+                image_path = meta["image_path"]
+            if "path" in meta.keys():
+                image_path = meta["path"]
+
+            file_name, file_extension = os.path.splitext(file_name)
+
+            file_name = file_name + export_stack_modifier + ".tif"
+            image_path = image_path.replace(image_path.split("\\")[-1], file_name)
+
+            if (self.export_stack_location.currentText() == "Import Directory" and file_name != None and image_path != None):
+                export_path = os.path.abspath(image_path.replace(file_name, ""))
+
+            elif self.export_stack_location.currentText() == "Select Directory":
+                export_path = os.path.abspath(self.export_directory)
+
+            else:
+                export_path = None
+
+            if os.path.isdir(export_path) != True:
+                if self.widget_notifications:
+                    show_info("Directory does not exist, try selecting a directory instead!")
+
+            else:
+                y1, y2, x1, x2 = meta["crop"]
+
+                if len(image.shape) > 2:
+                    image = image[:, y1:y2, x1:x2]
+                    mask = mask[:, y1:y2, x1:x2]
+                else:
+                    image = image[y1:y2, x1:x2]
+                    mask = mask[y1:y2, x1:x2]
+
+                if os.path.isdir(export_path) == False:
+                    os.makedirs(file_path)
+
+                file_path = export_path + "\\" + file_name
+
+                if os.path.isfile(file_path) == True and overwrite == False:
+                    if self.widget_notifications:
+                        show_info(file_name + " already exists, BacSeg will not overwrite files!")
+
+                else:
+
+                    if export_stack_mode == "Export .tif Images":
+                        tifffile.imwrite(file_path, image_stack, metadata=meta)
+
+                    if export_stack_mode == "Export .tif Masks":
+                        tifffile.imwrite(file_path, mask_stack, metadata=meta)
+
+    except:
+        print(traceback.format_exc())
+        pass
+
 
 
 def export_files(self, progress_callback, mode):
     desktop = os.path.expanduser("~/Desktop")
 
     overwrite = self.export_overwrite_setting.isChecked()
     export_images = self.export_image_setting.isChecked()
+
     normalise = self.export_normalise.isChecked()
     invert = self.export_invert.isChecked()
     autocontrast = self.export_autocontrast.isChecked()
     scalebar = self.export_scalebar.isChecked()
     cropzoom = self.export_cropzoom.isChecked()
     mask_background = self.export_mask_background.isChecked()
 
@@ -2395,25 +2303,15 @@
             if len(viewer_dims) == 2:
                 for tile_index in range(*viewer_dims[1]):
                     dim_list.append((image_index, tile_index))
             else:
                 dim_list.append((image_index,))
 
     for i, dim in enumerate(dim_list):
-        image, mask, label, meta, mode = generate_export_image(
-            self,
-            export_channel,
-            dim,
-            normalise,
-            invert,
-            autocontrast,
-            scalebar,
-            cropzoom,
-            mask_background,
-        )
+        image, mask, nmask, label, meta, mode = generate_export_image(self, export_channel, dim, normalise, invert, autocontrast, scalebar, cropzoom, mask_background, )
         contours = get_contours_from_mask(mask, label, export_labels)
 
         if "midlines" in meta.keys():
             midlines = meta["midlines"].copy()
         else:
             midlines = None
 
@@ -2431,32 +2329,26 @@
 
         if len(dim) == 2:
             file_name = file_name + f"_{dim}"
 
         file_name = file_name + export_modifier + ".tif"
         image_path = image_path.replace(image_path.split("\\")[-1], file_name)
 
-        if (
-            self.export_location.currentText() == "Import Directory"
-            and file_name != None
-            and image_path != None
-        ):
+        if (self.export_location.currentText() == "Import Directory" and file_name != None and image_path != None):
             export_path = os.path.abspath(image_path.replace(file_name, ""))
 
         elif self.export_location.currentText() == "Select Directory":
             export_path = os.path.abspath(self.export_directory)
 
         else:
             export_path = None
 
         if os.path.isdir(export_path) != True:
             if self.widget_notifications:
-                show_info(
-                    "Directory does not exist, try selecting a directory instead!"
-                )
+                show_info("Directory does not exist, try selecting a directory instead!")
 
         else:
             y1, y2, x1, x2 = meta["crop"]
 
             if len(image.shape) > 2:
                 image = image[:, y1:y2, x1:x2]
             else:
@@ -2468,30 +2360,24 @@
             if os.path.isdir(export_path) == False:
                 os.makedirs(file_path)
 
             file_path = export_path + "\\" + file_name
 
             if os.path.isfile(file_path) == True and overwrite == False:
                 if self.widget_notifications:
-                    show_info(
-                        file_name
-                        + " already exists, BacSeg will not overwrite files!"
-                    )
+                    show_info(file_name + " already exists, BacSeg will not overwrite files!")
 
             else:
                 if self.export_mode.currentText() == "Export .tif Images":
                     tifffile.imwrite(file_path, image, metadata=meta)
 
                 if self.export_mode.currentText() == "Export .tif Masks":
                     tifffile.imwrite(file_path, mask, metadata=meta)
 
-                if (
-                    self.export_mode.currentText()
-                    == "Export .tif Images and Masks"
-                ):
+                if (self.export_mode.currentText() == "Export .tif Images and Masks"):
                     image_path = os.path.abspath(export_path + "\\images")
                     mask_path = os.path.abspath(export_path + "\\masks")
 
                     if not os.path.exists(image_path):
                         os.makedirs(image_path)
 
                     if not os.path.exists(mask_path):
@@ -2512,53 +2398,42 @@
                         tifffile.imwrite(file_path, image, metadata=meta)
 
                 if self.export_mode.currentText() == "Export Oufti":
                     try:
                         with warnings.catch_warnings():
                             warnings.filterwarnings("ignore")
 
-                            from napari_bacseg._utils_oufti import (
-                                export_oufti,
-                                get_oufti_data,
-                            )
-
-                            oufti_data = get_oufti_data(
-                                self, image, mask, midlines
-                            )
+                            from napari_bacseg._utils_oufti import (export_oufti, get_oufti_data, )
+
+                            oufti_data = get_oufti_data(self, image, mask, midlines)
 
                             if "midlines" in meta.keys():
                                 meta.pop("midlines")
 
                             export_oufti(image, oufti_data, file_path)
 
                             if export_images:
-                                tifffile.imwrite(
-                                    file_path, image, metadata=meta
-                                )
+                                tifffile.imwrite(file_path, image, metadata=meta)
 
                     except:
-                        raise Exception(
-                            "BacSeg can't load Cellpose and OUFTI dependencies simultaneously. Restart BacSeg, reload images/masks, then export Oufti"
-                        )
+                        raise Exception("BacSeg can't load Cellpose and OUFTI dependencies simultaneously. Restart BacSeg, reload images/masks, then export Oufti")
 
                 if self.export_mode.currentText() == "Export ImageJ":
                     from napari_bacseg._utils_imagej import export_imagej
 
                     if mode == "rgb":
                         if self.widget_notifications:
-                            show_info(
-                                "ImageJ can't handle RGB images with annotations, export as image stack instead..."
-                            )
+                            show_info("ImageJ can't handle RGB images with annotations, export as image stack instead...")
 
                     export_imagej(image, contours, meta, file_path)
 
                 if self.export_mode.currentText() == "Export JSON":
                     from napari_bacseg._utils_json import export_coco_json
 
-                    export_coco_json(file_name, image, mask, label, file_path)
+                    export_coco_json(file_name, image, mask, nmask, label, file_path)
 
                     if export_images:
                         tifffile.imwrite(file_path, image, metadata=meta)
 
                 if self.export_mode.currentText() == "Export CSV":
                     export_csv(image, contours, meta, file_path)
 
@@ -2587,102 +2462,63 @@
 
         for i in range(len(contours)):
             try:
                 cnt = contours[i]
                 cnt = np.vstack(cnt).squeeze().astype(str)
 
                 if len(cnt.shape) < max_length:
-                    cnt = np.pad(
-                        cnt,
-                        ((0, max_length - cnt.shape[0]), (0, 0)),
-                        "constant",
-                        constant_values="",
-                    )
+                    cnt = np.pad(cnt, ((0, max_length - cnt.shape[0]), (0, 0)), "constant", constant_values="", )
 
                 processed_contours.append(cnt)
 
             except:
                 pass
 
         try:
             file_extension = file_path.split(".")[-1]
             file_path = file_path.replace(file_extension, "csv")
 
             processed_contours = np.hstack(processed_contours)
-            headers = np.array(
-                [
-                    [f"x[{str(x)}]", f"y[{str((x))}]"]
-                    for x in range(processed_contours.shape[-1] // 2)
-                ]
-            ).flatten()
-
-            pd.DataFrame(processed_contours, columns=headers).to_csv(
-                file_path, index=False, header=True
-            )
+            headers = np.array([[f"x[{str(x)}]", f"y[{str((x))}]"] for x in range(processed_contours.shape[-1] // 2)]).flatten()
+
+            pd.DataFrame(processed_contours, columns=headers).to_csv(file_path, index=False, header=True)
 
         except:
             print(traceback.format_exc())
 
 
 def _manualImport(self):
     try:
-        if (
-            self.viewer.layers.index("Segmentations")
-            != len(self.viewer.layers) - 1
-        ):
+        if (self.viewer.layers.index("Segmentations") != len(self.viewer.layers) - 1):
             # reshapes masks to be same shape as active image
             self.active_layer = self.viewer.layers[-1]
 
             if self.active_layer.metadata == {}:
                 active_image = self.active_layer.data
 
                 if len(active_image.shape) < 3:
                     active_image = np.expand_dims(active_image, axis=0)
                     self.active_layer.data = active_image
 
                 if self.classLayer.data.shape != self.active_layer.data.shape:
-                    self.classLayer.data = np.zeros(
-                        active_image.shape, np.uint16
-                    )
+                    self.classLayer.data = np.zeros(active_image.shape, np.uint16)
 
                 if self.segLayer.data.shape != self.active_layer.data.shape:
-                    self.segLayer.data = np.zeros(
-                        active_image.shape, np.uint16
-                    )
+                    self.segLayer.data = np.zeros(active_image.shape, np.uint16)
 
                 image_name = str(self.viewer.layers[-1]) + ".tif"
 
                 meta = {}
                 for i in range(active_image.shape[0]):
                     img = active_image[i, :, :]
 
-                    contrast_limit, alpha, beta, gamma = autocontrast_values(
-                        img, clip_hist_percent=1
-                    )
-
-                    img_meta = dict(
-                        image_name=image_name,
-                        image_path="Unknown",
-                        mask_name=None,
-                        mask_path=None,
-                        label_name=None,
-                        label_path=None,
-                        folder=None,
-                        parent_folder=None,
-                        contrast_limit=contrast_limit,
-                        contrast_alpha=alpha,
-                        contrast_beta=beta,
-                        contrast_gamma=gamma,
-                        akseg_hash=None,
-                        import_mode="manual",
-                        dims=[img.shape[1], img.shape[0]],
-                        crop=[0, img.shape[0], 0, img.shape[1]],
-                        frame=i,
-                        frames=active_image.shape[0],
-                    )
+                    contrast_limit, alpha, beta, gamma = autocontrast_values(img, clip_hist_percent=1)
+
+                    img_meta = dict(image_name=image_name, image_path="Unknown", mask_name=None, mask_path=None, label_name=None, label_path=None, folder=None, parent_folder=None, contrast_limit=contrast_limit, contrast_alpha=alpha, contrast_beta=beta, contrast_gamma=gamma, akseg_hash=None, import_mode="manual", dims=[
+                        img.shape[1], img.shape[0]], crop=[0, img.shape[0], 0, img.shape[1]], frame=i, frames=active_image.shape[0], )
 
                     meta[i] = img_meta
 
                 self.active_layer.metadata = meta
                 self.segLayer.metadata = meta
                 self.classLayer.metadata = meta
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_cellpose.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_cellpose.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,44 @@
             "filename": file_path,
             "flows": flow,
             "est_diam": 15,
         },
     )
 
 
+def _postpocess_cellpose(self, mask):
+    try:
+        min_seg_size = int(self.cellpose_min_seg_size.currentText())
+
+        print(min_seg_size)
+
+        post_processed_mask = np.zeros(mask.shape, dtype=np.uint16)
+
+        mask_ids = sorted(np.unique(mask))
+
+        for i in range(1, len(mask_ids)):
+            cell_mask = np.zeros(mask.shape, dtype=np.uint8)
+            cell_mask[mask == i] = 255
+
+            contours, _ = cv2.findContours(
+                cell_mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE
+            )
+
+            cnt = contours[0]
+
+            area = cv2.contourArea(cnt)
+
+            if area > min_seg_size:
+                post_processed_mask[mask == i] = i
+    except:
+        post_processed_mask = mask
+
+    return post_processed_mask
+
+
 def _run_cellpose(self, progress_callback, images):
     mask_stack = []
 
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", category=DeprecationWarning)
 
         flow_threshold = float(self.cellpose_flowthresh_label.text())
@@ -94,14 +124,16 @@
                     channels=[0, 0],
                     flow_threshold=flow_threshold,
                     cellprob_threshold=mask_threshold,
                     min_size=min_size,
                     batch_size=3,
                 )
 
+                mask = _postpocess_cellpose(self, mask)
+
                 masks.append(mask)
 
             mask_stack = np.stack(masks, axis=0)
 
         if gpu:
             import torch
 
@@ -110,48 +142,46 @@
         return mask_stack
 
 
 def _process_cellpose(self, segmentation_data):
     if len(segmentation_data) > 0:
         masks = segmentation_data
 
-        if self.segLayer.data.shape != masks.shape:
+        if self.cellpose_seg_mode.currentIndex() == 0:
+            output_layer = self.segLayer
+        else:
+            output_layer = self.nucLayer
+
+        if output_layer.data.shape != masks.shape:
             current_fov = self.viewer.dims.current_step[0]
-            self.segLayer.data[current_fov, :, :] = masks
+            output_layer.data[current_fov, :, :] = masks
 
         else:
-            self.segLayer.data = masks
+            output_layer.data = masks
 
-        self.segLayer.contour = 1
-        self.segLayer.opacity = 1
+        output_layer.contour = 1
+        output_layer.opacity = 1
 
         self.cellpose_segmentation = True
         self.cellpose_progressbar.setValue(0)
-        self._autoClassify(reset=True)
+
+        if self.cellpose_seg_mode.currentIndex() == 0:
+            self._autoClassify(reset=True)
+
         self._autoContrast()
 
         if self.cellpose_resetimage.isChecked() == True:
             self.viewer.reset_view()
 
         self._reorderLayers()
 
-        # layer_names = [
-        #     layer.name
-        #     for layer in self.viewer.layers
-        #     if layer.name not in ["Segmentations", "Classes", "center_lines"]
-        # ]
-        #
-        # # ensures segmentation and classes is in correct order in the viewer
-        # for layer in layer_names:
-        #     layer_index = self.viewer.layers.index(layer)
-        #     self.viewer.layers.move(layer_index, 0)
+        # layer_names = [  #     layer.name  #     for layer in self.viewer.layers  #     if layer.name not in ["Segmentations", "Classes", "center_lines"]  # ]  #  # # ensures segmentation and classes is in correct order in the viewer  # for layer in layer_names:  #     layer_index = self.viewer.layers.index(layer)  #     self.viewer.layers.move(layer_index, 0)
 
 
 def load_cellpose_dependencies(self, omni=False):
-
     if self.widget_notifications:
         show_info("Loading Cellpose dependencies")
 
     if omni == True:
         from omnipose.core import labels_to_flows
     else:
         from cellpose.dynamics import labels_to_flows
@@ -191,15 +221,15 @@
                         f"Loading Cellpose Model: {os.path.basename(model_path)}"
                     )
             elif "cellpose_" in model_name:
                 load_model = True
                 omnipose_model = False
                 if self.widget_notifications:
                     show_info(
-                        f"Loading Omnipose Model: {os.path.basename(model_path)}"
+                        f"Loading Cellpose Model: {os.path.basename(model_path)}"
                     )
             else:
                 if self.widget_notifications:
                     show_info(f"BacSeg Cannot train Omnipose models")
                 load_model = False
 
             if load_model == True:
@@ -279,18 +309,22 @@
 
 
 def train_cellpose_model(self, progress_callback=0):
     try:
         channel = self.cellpose_trainchannel.currentText()
 
         images = self.viewer.layers[channel].data
-        masks = self.segLayer.data
-
         images = unstack_images(images, axis=0)
-        masks = unstack_images(masks, axis=0)
+
+        if self.cellpose_seg_mode.currentIndex() == 0:
+            masks = self.segLayer.data
+            masks = unstack_images(masks, axis=0)
+        else:
+            masks = self.nucleiLayer.data
+            masks = unstack_images(masks, axis=0)
 
         nepochs = int(self.cellpose_nepochs.currentText())
         batchsize = int(self.cellpose_batchsize.currentText())
         model_type = self.cellpose_trainmodel.currentText()
         model_load_path = self.cellpose_custom_model_path
         model_save_path = self.cellpose_train_model_path
         diameter = int(self.cellpose_diameter_label.text())
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_colicoords.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_colicoords.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_database.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_database.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_database_IO.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_database_IO.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,24 +109,26 @@
     try:
         imported_images = {}
 
         for dat in imported_data:
             for channel, channel_data in dat.items():
                 image = channel_data["images"]
                 mask = channel_data["masks"]
+                nmask = channel_data["nmasks"]
                 label = channel_data["classes"]
                 meta = channel_data["metadata"]
 
                 if channel not in imported_images.keys():
-                    imported_images[channel] = dict(images=[image], masks=[mask], classes=[label], metadata={0: meta}, )
+                    imported_images[channel] = dict(images=[image], masks=[mask], nmasks=[nmask], classes=[label], metadata={0: meta}, )
                 else:
                     image_index = len(imported_images[channel]["images"])
 
                     imported_images[channel]["images"].append(image)
                     imported_images[channel]["masks"].append(mask)
+                    imported_images[channel]["nmasks"].append(nmask)
                     imported_images[channel]["classes"].append(label)
                     imported_images[channel]["metadata"][image_index] = meta
 
     except:
         print(traceback.format_exc())
 
     imported_data = dict(imported_images=imported_images)
@@ -174,15 +176,15 @@
 
     for key in range(1, num_user_keys + 1):
         control_name = f"upload_usermeta{key}"
         combo_box = getattr(self, control_name)
         combo_box_value = combo_box.currentText()
         metadata[f"usermeta{key}"] = combo_box_value
 
-    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
     layer_names.reverse()
 
     # put segmentation channel as first channel in stack
     segChannel = self.cellpose_segchannel.currentText()
     layer_names.remove(segChannel)
     layer_names.insert(0, segChannel)
@@ -286,15 +288,15 @@
 
         segmentation_file = measurement[measurement["channel"] == segmentation_channel]["file_name"].item()
         user_initial = measurement[measurement["channel"] == segmentation_channel]["user_initial"].item()
         folder = measurement[measurement["channel"] == segmentation_channel]["folder"].item()
 
         json_path = os.path.join(database_path, "Images", user_initial, "json", folder, segmentation_file, )
 
-        mask, label = import_coco_json(json_path)
+        mask, nmask, label = import_coco_json(json_path)
 
         for j in range(len(channels)):
             channel = channels[j]
 
             measurement_channels = measurement["channel"].unique()
 
             if channel in measurement_channels:
@@ -325,14 +327,15 @@
                     if meta["segmentation_file"] in [None, "None"]:
                         meta["segmentation_file"] = list_from_string(measurement["file_list"].iloc[0])[0]
                         meta["segmentation_channel"] = list_from_string(measurement["channel_list"].iloc[0])[0]
 
             else:
                 image = np.zeros((100, 100), dtype=np.uint16)
                 mask = np.zeros((100, 100), dtype=np.uint16)
+                nmask = np.zeros((100, 100), dtype=np.uint16)
                 label = np.zeros((100, 100), dtype=np.uint16)
 
                 meta = {}
 
                 meta["image_name"] = "missing image channel"
                 meta["image_path"] = "missing image channel"
                 meta["folder"] = (None,)
@@ -344,15 +347,15 @@
                 meta["contrast_alpha"] = None
                 meta["contrast_beta"] = None
                 meta["contrast_gamma"] = None
                 meta["dims"] = [image.shape[-1], image.shape[-2]]
                 meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
                 meta["light_source"] = channel
 
-            imported_images[channel] = dict(images=image, masks=mask, classes=label, metadata=meta)
+            imported_images[channel] = dict(images=image, masks=mask, nmasks=nmask, classes=label, metadata=meta, )
 
     except:
         pass
 
     return imported_images
 
 
@@ -362,14 +365,15 @@
     try:
         dat = np.load(path, allow_pickle=True).item()
 
         user_metadata = dat["user_metadata"]
         image = dat["image"]
         image_meta = dat["image_meta"]
         mask = dat["mask"]
+        nmask = dat["nmask"]
         class_mask = dat["class_mask"]
         save_dir = dat["save_dir"]
         overwrite_images = dat["overwrite_images"]
         overwrite_masks = dat["overwrite_masks"]
         overwrite_metadata = dat["overwrite_metadata"]
         overwrite_selected_metadata = dat["overwrite_selected_metadata"]
         overwrite_all_metadata = dat["overwrite_all_metadata"]
@@ -470,14 +474,15 @@
 
                 if len(img.shape) > 2:
                     img = img[:, y1:y2, x1:x2]
                 else:
                     img = img[y1:y2, x1:x2]
 
                 mask = mask[y1:y2, x1:x2]
+                nmask = nmask[y1:y2, x1:x2]
                 class_mask = class_mask[y1:y2, x1:x2]
 
                 unique_segmentations = np.unique(mask)
                 unique_segmentations = np.delete(unique_segmentations, np.where(unique_segmentations == 0))
 
                 num_segmentations = len(unique_segmentations)
                 image_laplacian = cv2.Laplacian(img, cv2.CV_64F).var()
@@ -502,15 +507,15 @@
                 if upload_images is True:
                     if (os.path.isfile(image_path) is False or import_mode == "BacSeg" or overwrite_images is True or overwrite_metadata is True):
                         tifffile.imwrite(os.path.abspath(image_path), img, metadata=meta)
 
                 if upload_segmentations is True:
                     if (os.path.isfile(mask_path) is False or import_mode == "BacSeg" or overwrite_masks is True or overwrite_metadata is True):
                         if file_name == segmentation_file:
-                            export_coco_json(file_name, img, mask, class_mask, json_path)
+                            export_coco_json(file_name, img, mask, nmask, class_mask, json_path, )
 
                 if "mask_path" not in meta.keys():
                     meta["mask_path"] = None
                 if "label_path" not in meta.keys():
                     meta["label_path"] = None
 
                 file_metadata = {"date_uploaded": date_uploaded, "date_created": date_created, "date_modified": date_modified, "file_name": file_name, "channel": get_meta_value(meta, "channel"), "file_list": get_meta_value(meta, "file_list"), "channel_list": get_meta_value(meta, "channel_list"), "segmentation_file": get_meta_value(meta, "segmentation_file"), "segmentation_channel": get_meta_value(meta, "segmentation_channel"), "strain": get_meta_value(meta, "strain"), "phenotype": get_meta_value(meta, "phenotype"), "akseg_hash": get_meta_value(meta, "akseg_hash"), "user_initial": get_meta_value(meta, "user_initial"), "content": get_meta_value(meta, "image_content"), "microscope": get_meta_value(meta, "microscope"), "modality": get_meta_value(meta, "modality"), "source": get_meta_value(meta, "light_source"), "stain": get_meta_value(meta, "stain"), "stain_target": get_meta_value(meta, "stain_target"), "antibiotic": get_meta_value(meta, "antibiotic"), "treatment time (mins)": get_meta_value(meta, "treatmenttime"), "antibiotic concentration": get_meta_value(meta, "abxconcentration"), "mounting method": get_meta_value(meta, "mount"), "protocol": get_meta_value(meta, "protocol"), "folder": get_meta_value(meta, "folder"), "parent_folder": get_meta_value(meta, "parent_folder"), "num_segmentations": num_segmentations, "image_laplacian": image_laplacian, "image_focus": get_meta_value(meta, "image_focus"), "image_debris": get_meta_value(meta, "image_debris"), "segmented": get_meta_value(meta, "segmented"), "labelled": get_meta_value(meta, "labelled"), "segmentation_curated": get_meta_value(meta, "segmentations_curated"), "label_curated": get_meta_value(meta, "labels_curated"), "posX": posX, "posY": posY, "posZ": posZ, "image_load_path": get_meta_value(meta, "image_path"), "image_save_path": image_path, "mask_load_path": get_meta_value(meta, "mask_path"), "mask_save_path": mask_path, "label_load_path": get_meta_value(meta, "label_path"), "label_save_path": class_path, }
@@ -523,15 +528,15 @@
     except:
         file_metadata_list = []
         print(traceback.format_exc())
 
     return file_metadata_list
 
 
-def generate_upload_tempfiles(user_metadata, image_stack, meta_stack, mask_stack, class_stack, save_dir, overwrite_images, overwrite_masks, overwrite_metadata, overwrite_selected_metadata, overwrite_all_metadata, upload_images, upload_segmentations, upload_metadata, ):
+def generate_upload_tempfiles(user_metadata, image_stack, meta_stack, mask_stack, nmask_stack, class_stack, save_dir, overwrite_images, overwrite_masks, overwrite_metadata, overwrite_selected_metadata, overwrite_all_metadata, upload_images, upload_segmentations, upload_metadata, ):
     upload_tempfiles = []
 
     upload_dir = os.path.join(tempfile.gettempdir(), "BacSeg")
 
     if os.path.isdir(upload_dir) != True:
         os.mkdir(upload_dir)
     else:
@@ -539,14 +544,15 @@
         os.mkdir(upload_dir)
 
     for i in range(len(image_stack)):
         try:
             image = image_stack[i]
             image_meta = meta_stack[i]
             mask = mask_stack[i]
+            nmask = nmask_stack[i]
             class_mask = class_stack[i]
 
             meta = image_meta[image_meta["channel_list"][0]]
 
             folder = meta["folder"]
 
             image_dir = os.path.join(save_dir, "images", folder)
@@ -562,15 +568,15 @@
 
             if os.path.exists(json_dir) == False:
                 os.makedirs(json_dir)
 
             if os.path.exists(class_dir) == False:
                 os.makedirs(class_dir)
 
-            upload_data = dict(user_metadata=user_metadata, image=image, image_meta=image_meta, mask=mask, class_mask=class_mask, save_dir=save_dir, overwrite_images=overwrite_images, overwrite_masks=overwrite_masks, overwrite_metadata=overwrite_metadata, overwrite_selected_metadata=overwrite_selected_metadata, overwrite_all_metadata=overwrite_all_metadata, image_dir=image_dir, mask_dir=mask_dir, json_dir=json_dir, class_dir=class_dir, upload_images=upload_images, upload_segmentations=upload_segmentations, upload_metadata=upload_metadata, )
+            upload_data = dict(user_metadata=user_metadata, image=image, image_meta=image_meta, mask=mask, nmask=nmask, class_mask=class_mask, save_dir=save_dir, overwrite_images=overwrite_images, overwrite_masks=overwrite_masks, overwrite_metadata=overwrite_metadata, overwrite_selected_metadata=overwrite_selected_metadata, overwrite_all_metadata=overwrite_all_metadata, image_dir=image_dir, mask_dir=mask_dir, json_dir=json_dir, class_dir=class_dir, upload_images=upload_images, upload_segmentations=upload_segmentations, upload_metadata=upload_metadata, )
 
             # if "segmentation_file" in user_metadata:
             #     print("segmentation_file in user_metadata")
             # elif "segmentation_channel" in image_meta:
             #     print("segmentation_channel in image_meta")
             # else:
             #     print("segmentation_file not in user_metadata and segmentation_channel not in image_meta")
@@ -638,15 +644,15 @@
 
                 metadata_file_names = []
                 metadata_akseg_hash = []
 
                 user_metadata = pd.DataFrame(columns=self.metadata_columns)
 
             channel_labels = ["modality", "light_source", "stain", "stain_target", ]
-            channel_metadata = [layer.metadata[0] for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+            channel_metadata = [layer.metadata[0] for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
             metalabels = []
 
             for label in channel_labels:
                 for channel_meta in channel_metadata:
                     if label in channel_meta.keys():
                         metalabels.append(channel_meta[label])
@@ -657,39 +663,41 @@
 
             if ("Required for upload" in metalabels and self.active_import_mode != "BacSeg"):
                 if self.widget_notifications:
                     show_info("Please fill out channel (all channels) and image metadata before uploading files")
 
             else:
                 segChannel = self.cellpose_segchannel.currentText()
-                channel_list = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+                channel_list = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines", ]]
 
                 if segChannel == "":
                     if self.widget_notifications:
                         show_info("Please pick an image channel to upload")
 
                 else:
                     backup_user_metadata(self, user_metadata)
 
                     image_layer = self.viewer.layers[segChannel]
 
                     (image_stack, meta_stack, channel_list,) = generate_multichannel_stack(self)
                     mask_stack = self.segLayer.data
+                    nmask_stack = self.nucLayer.data
                     class_stack = self.classLayer.data
 
                     if len(image_stack) >= 1:
                         if mode == "active":
                             current_step = self.viewer.dims.current_step[0]
 
                             image_stack = np.expand_dims(image_stack[current_step], axis=0)
                             mask_stack = np.expand_dims(mask_stack[current_step], axis=0)
+                            nmask_stack = np.expand_dims(nmask_stack[current_step], axis=0)
                             class_stack = np.expand_dims(class_stack[current_step], axis=0)
                             meta_stack = np.expand_dims(meta_stack[current_step], axis=0)
 
-                    upload_tempfiles = generate_upload_tempfiles(user_metadata, image_stack, meta_stack, mask_stack, class_stack, save_dir, overwrite_images, overwrite_masks, overwrite_metadata, overwrite_selected_metadata, overwrite_all_metadata, upload_images, upload_segmentations, upload_metadata, )
+                    upload_tempfiles = generate_upload_tempfiles(user_metadata, image_stack, meta_stack, mask_stack, nmask_stack, class_stack, save_dir, overwrite_images, overwrite_masks, overwrite_metadata, overwrite_selected_metadata, overwrite_all_metadata, upload_images, upload_segmentations, upload_metadata, )
 
                     if mode == "active":
                         results = upload_bacseg_files(upload_tempfiles[0], num_user_keys)
 
                     else:
                         with Pool(4) as pool:
                             iter = []
@@ -791,25 +799,27 @@
             with open(user_metadata_path) as f:
                 for row in range(10):
                     line = next(f).strip()
                     delim = sniffer.sniff(line)
 
             user_metadata = pd.read_csv(user_metadata_path, sep=delim.delimiter, low_memory=False)
 
-            user_metadata[["treatment time (mins)"]] = user_metadata[["treatment time (mins)"]].apply(pd.to_numeric, downcast="float")
+            user_metadata[["treatment time (mins)"]] = user_metadata[["treatment time (mins)"]].apply(pd.to_numeric, downcast="float", errors="coerce")
 
             user_metadata, expected_columns = check_metadata_format(user_metadata, self.metadata_columns)
 
             user_metadata["segmentation_channel"] = user_metadata["segmentation_channel"].astype(str)
 
             self.user_metadata = user_metadata
             self.expected_columns = expected_columns
 
     except:
+        print(traceback.format_exc())
         user_metadata = None
+        expected_columns = None
 
     return user_metadata, expected_columns
 
 
 def backup_user_metadata(self, user_metadata=""):
     try:
         if type(user_metadata) is str:
@@ -950,14 +960,16 @@
                 user_metadata = user_metadata.sort_values(sort_names, ascending=sort_directions).reset_index(drop=True)
 
             import_limit = self.database_download_limit.currentText()
 
             segmentation_files = user_metadata["segmentation_file"].unique()
             num_measurements = len(segmentation_files)
 
+            print(num_measurements)
+
             if import_limit == "All":
                 import_limit = num_measurements
             else:
                 if int(import_limit) > num_measurements:
                     import_limit = num_measurements
 
             user_metadata = user_metadata[user_metadata["segmentation_file"].isin(segmentation_files[: int(import_limit)])]
@@ -993,14 +1005,14 @@
                 user_metadata.loc[user_metadata["posY"].isna(), "posY"] = 0
             if "posZ" in user_metadata.columns:
                 sort_columns.append("posZ")
                 user_metadata.loc[user_metadata["posZ"].isna(), "posZ"] = 0
 
             measurements = user_metadata.groupby(sort_columns)
 
-            show_info(f"Found {len(file_paths)//len(channels)} matching database files.")
+            show_info(f"Found {len(file_paths) // len(channels)} matching database files.")
 
     except:
         print(traceback.format_exc())
         measurements, file_paths, channels = None, None, None
 
     return measurements, file_paths, channels
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_imagej.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_imagej.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import numpy as np
 import tifffile
 from napari.utils.notifications import show_info
 from roifile import ImagejRoi, roiread
 
 
 def read_imagej_file(path, image, widget_notifications=True):
+
     contours = []
-    mask = np.zeros_like(image)
+    mask = np.zeros(image.shape[-2:], dtype=np.uint16)
 
     # reads overlays sequentially and then converts them to openCV contours
     try:
         for roi in roiread(path):
             coordinates = roi.integer_coordinates
 
             top = roi.top
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_interface_events.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_interface_events.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import cv2
 import numpy as np
 from napari.utils.notifications import show_info
 
 
 def find_contours(img):
     # finds contours of shapes, only returns the external contours of the shapes
-    contours, hierarchy = cv2.findContours(img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE)
+    contours, hierarchy = cv2.findContours(
+        img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE
+    )
     contours = sorted(contours, key=cv2.contourArea, reverse=True)
     return contours
 
 
 def fill_holes(mask, colour):
     try:
         fill_mask = mask.copy()
@@ -28,41 +30,57 @@
 
     except:
         pass
 
     return mask
 
 
+def _modify_channel_changed(self, event):
+    if self.modify_channel.currentIndex() == 0:
+        self.viewer.layers.selection.active = self.segLayer
+    else:
+        self.viewer.layers.selection.active = self.nucLayer
+
+
 def _segmentationEvents(self, viewer, event):
     try:
         if "Control" in event.modifiers:
             self._modifyMode(mode="delete")
 
         if "Shift" in event.modifiers:
             self._modifyMode(mode="add")
 
+        if self.modify_channel.currentIndex() == 0:
+            modify_channel = self.segLayer
+            self.viewer.layers.selection.active = self.segLayer
+        else:
+            modify_channel = self.nucLayer
+            self.viewer.layers.selection.active = self.nucLayer
+
         if self.interface_mode == "segment":
             # add segmentation
             if self.segmentation_mode in ["add", "extend"]:
-                self.segLayer.mode = "paint"
-                self.segLayer.brush_size = 1
+                modify_channel.mode = "paint"
+                modify_channel.brush_size = 1
 
-                stored_mask = self.segLayer.data.copy()
+                stored_mask = modify_channel.data.copy()
                 stored_class = self.classLayer.data.copy()
-                meta = self.segLayer.metadata.copy()
+                meta = modify_channel.metadata.copy()
 
                 if self.segmentation_mode == "add":
                     new_colour = _newSegColour(self)
                 else:
-                    data_coordinates = self.segLayer.world_to_data(event.position)
+                    data_coordinates = modify_channel.world_to_data(
+                        event.position
+                    )
                     coord = np.round(data_coordinates).astype(int)
-                    new_colour = self.segLayer.get_value(coord)
+                    new_colour = modify_channel.get_value(coord)
 
-                    self.segLayer.selected_label = new_colour
-                    new_colour = self.segLayer.get_value(coord)
+                    modify_channel.selected_label = new_colour
+                    new_colour = modify_channel.get_value(coord)
 
                     new_class = self.classLayer.get_value(coord)
 
                     if new_class != None:
                         self.class_colour = new_class
 
                 dragged = False
@@ -74,274 +92,306 @@
                 while event.type == "mouse_move":
                     coordinates.append(event.position)
                     dragged = True
                     yield
 
                 # on release
                 if dragged:
-                    if (new_colour != 0 and new_colour != None and self.class_colour != None):
-                        coordinates = np.round(np.array(coordinates)).astype(np.int32)
+                    if (
+                        new_colour != 0
+                        and new_colour != None
+                        and self.class_colour != None
+                    ):
+                        coordinates = np.round(np.array(coordinates)).astype(
+                            np.int32
+                        )
 
                         mask_dim = tuple(list(coordinates[0][:-2]) + [...])
 
                         cnt = coordinates[:, -2:]
 
                         cnt = np.fliplr(cnt)
                         cnt = cnt.reshape((-1, 1, 2))
 
-                        seg_stack = self.segLayer.data
+                        seg_stack = modify_channel.data
 
                         seg_mask = seg_stack[mask_dim]
 
-                        cv2.drawContours(seg_mask, [cnt], -1, int(new_colour), -1)
+                        cv2.drawContours(
+                            seg_mask, [cnt], -1, int(new_colour), -1
+                        )
 
                         seg_mask = fill_holes(seg_mask, new_colour)
 
                         seg_stack[mask_dim] = seg_mask
 
-                        self.segLayer.data = seg_stack
+                        modify_channel.data = seg_stack
 
                         # update class
 
                         class_stack = self.classLayer.data
                         class_colour = self.class_colour
-                        seg_stack = self.segLayer.data
+                        seg_stack = modify_channel.data
 
                         seg_mask = seg_stack[mask_dim]
                         class_mask = class_stack[mask_dim]
 
                         class_mask[seg_mask == int(new_colour)] = class_colour
                         class_stack[mask_dim] = class_mask
 
                         self.classLayer.data = class_stack
 
                         # update metadata
 
                         meta["manual_segmentation"] = True
-                        self.segLayer.metadata = meta
-                        self.segLayer.mode = "pan_zoom"
+                        modify_channel.metadata = meta
+                        modify_channel.mode = "pan_zoom"
                         self.update_image_folds()
 
                     else:
-                        self.segLayer.data = stored_mask
+                        modify_channel.data = stored_mask
                         self.classLayer.data = stored_class
-                        self.segLayer.mode = "pan_zoom"
+                        modify_channel.mode = "pan_zoom"
 
             # join segmentations
             if self.segmentation_mode == "join":
-                self.segLayer.mode = "paint"
-                self.segLayer.brush_size = 1
+                modify_channel.mode = "paint"
+                modify_channel.brush_size = 1
 
-                stored_mask = self.segLayer.data.copy()
+                stored_mask = modify_channel.data.copy()
                 stored_class = self.classLayer.data.copy()
-                meta = self.segLayer.metadata.copy()
+                meta = modify_channel.metadata.copy()
 
-                data_coordinates = self.segLayer.world_to_data(event.position)
+                data_coordinates = modify_channel.world_to_data(event.position)
                 coord = np.round(data_coordinates).astype(int)
-                new_colour = self.segLayer.get_value(coord)
+                new_colour = modify_channel.get_value(coord)
 
-                self.segLayer.selected_label = new_colour
-                new_colour = self.segLayer.get_value(coord)
+                modify_channel.selected_label = new_colour
+                new_colour = modify_channel.get_value(coord)
 
                 new_class = self.classLayer.get_value(coord)
 
                 if new_class != None:
                     self.class_colour = new_class
 
                 dragged = False
                 colours = []
                 classes = []
                 coords = []
                 yield
 
                 # on move
                 while event.type == "mouse_move":
-                    data_coordinates = self.segLayer.world_to_data(event.position)
+                    data_coordinates = modify_channel.world_to_data(
+                        event.position
+                    )
                     coord = np.round(data_coordinates).astype(int)
-                    mask_val = self.segLayer.get_value(coord)
+                    mask_val = modify_channel.get_value(coord)
                     class_val = self.classLayer.get_value(coord)
                     colours.append(mask_val)
                     classes.append(class_val)
                     coords.append(coord)
                     dragged = True
                     yield
 
                 # on release
                 if dragged:
                     colours = np.array(colours)
                     colours = np.unique(colours)
                     colours = np.delete(colours, np.where(colours == 0))
 
                     if new_colour in colours:
-                        colours = np.delete(colours, np.where(colours == new_colour))
-
-                    if (len(colours) == 1 and new_colour not in colours and new_colour != None):
-                        mask_stack = self.segLayer.data
+                        colours = np.delete(
+                            colours, np.where(colours == new_colour)
+                        )
+
+                    if (
+                        len(colours) == 1
+                        and new_colour not in colours
+                        and new_colour != None
+                    ):
+                        mask_stack = modify_channel.data
 
                         mask_dim = tuple(list(coords[0][:-2]) + [...])
 
                         mask = mask_stack[mask_dim]
 
                         mask[mask == colours[0]] = new_colour
 
                         mask = fill_holes(mask, new_colour)
 
                         mask_stack[mask_dim] = mask
 
-                        self.segLayer.data = mask_stack
+                        modify_channel.data = mask_stack
 
                         # update class
 
                         class_stack = self.classLayer.data
-                        seg_stack = self.segLayer.data
+                        seg_stack = modify_channel.data
 
                         seg_mask = seg_stack[mask_dim]
                         class_mask = class_stack[mask_dim]
 
                         class_mask[seg_mask == new_colour] = 2
                         class_stack[mask_dim] = class_mask
 
                         self.classLayer.data = class_stack
 
                         # update metadata
 
                         meta["manual_segmentation"] = True
-                        self.segLayer.metadata = meta
-                        self.segLayer.mode = "pan_zoom"
+                        modify_channel.metadata = meta
+                        modify_channel.mode = "pan_zoom"
                         self.update_image_folds()
 
                     else:
-                        self.segLayer.data = stored_mask
+                        modify_channel.data = stored_mask
                         self.classLayer.data = stored_class
-                        self.segLayer.mode = "pan_zoom"
+                        modify_channel.mode = "pan_zoom"
 
             # split segmentations
             if self.segmentation_mode == "split":
-                self.segLayer.mode = "paint"
-                self.segLayer.brush_size = 1
+                modify_channel.mode = "paint"
+                modify_channel.brush_size = 1
 
                 new_colour = _newSegColour(self)
-                stored_mask = self.segLayer.data.copy()
+                stored_mask = modify_channel.data.copy()
                 stored_class = self.classLayer.data
-                meta = self.segLayer.metadata.copy()
+                meta = modify_channel.metadata.copy()
 
                 dragged = False
                 colours = []
                 yield
 
                 # on move
                 while event.type == "mouse_move":
-                    data_coordinates = self.segLayer.world_to_data(event.position)
+                    data_coordinates = modify_channel.world_to_data(
+                        event.position
+                    )
                     coords = np.round(data_coordinates).astype(int)
-                    mask_val = self.segLayer.get_value(coords)
+                    mask_val = modify_channel.get_value(coords)
                     colours.append(mask_val)
                     dragged = True
                     yield
 
                 # on release
                 if dragged:
                     colours = np.array(colours)
-                    colours = np.delete(colours, np.where(colours == new_colour))
+                    colours = np.delete(
+                        colours, np.where(colours == new_colour)
+                    )
 
                     colours[colours == None] = 0
 
                     num_colours = len(np.unique(colours))
 
                     if num_colours == 2 or num_colours == 3:
                         if num_colours == 2:
                             maskref = colours[colours != 0][0]
                         else:
-                            maskref = sorted(set(colours.tolist()), key=lambda x: colours.tolist().index(x), )[1]
-
-                        bisection = (colours[0] != maskref and colours[-1] != maskref)
+                            maskref = sorted(
+                                set(colours.tolist()),
+                                key=lambda x: colours.tolist().index(x),
+                            )[1]
+
+                        bisection = (
+                            colours[0] != maskref and colours[-1] != maskref
+                        )
 
                         if bisection and new_colour != None:
                             mask_dim = tuple(list(coords[:-2]) + [...])
                             shape_mask = stored_mask[mask_dim].copy()
 
                             class_mask = stored_class[mask_dim].copy()
                             class_mask[shape_mask == maskref] = 3
                             stored_class[mask_dim] = class_mask
                             self.classLayer.data = stored_class
 
                             shape_mask[shape_mask != maskref] = 0
                             shape_mask[shape_mask == maskref] = 255
                             shape_mask = shape_mask.astype(np.uint8)
 
-                            line_mask = self.segLayer.data.copy()
+                            line_mask = modify_channel.data.copy()
                             line_mask = line_mask[mask_dim]
                             line_mask[line_mask != new_colour] = 0
                             line_mask[line_mask == new_colour] = 255
                             line_mask = line_mask.astype(np.uint8)
 
                             overlap = cv2.bitwise_and(shape_mask, line_mask)
 
-                            shape_mask_split = cv2.bitwise_xor(shape_mask, overlap).astype(np.uint8)
+                            shape_mask_split = cv2.bitwise_xor(
+                                shape_mask, overlap
+                            ).astype(np.uint8)
 
                             # update labels layers with split shape
                             split_mask = stored_mask[mask_dim]
                             split_mask[overlap == 255] = new_colour
                             stored_mask[mask_dim] = split_mask
-                            self.segLayer.data = stored_mask
+                            modify_channel.data = stored_mask
 
                             # fill one have of the split shape with the new colour
                             indices = np.where(shape_mask_split == 255)
-                            split_dim = list(list(mask_dim[:-1]) + [indices[0][0], indices[1][0]])
+                            split_dim = list(
+                                list(mask_dim[:-1])
+                                + [indices[0][0], indices[1][0]]
+                            )
                             split_dim = np.array(split_dim).flatten().tolist()
 
-                            self.segLayer.fill(split_dim, new_colour)
+                            modify_channel.fill(split_dim, new_colour)
 
                             meta["manual_segmentation"] = True
-                            self.segLayer.metadata = meta
-                            self.segLayer.mode = "pan_zoom"
+                            modify_channel.metadata = meta
+                            modify_channel.mode = "pan_zoom"
                             self.update_image_folds()
 
                         else:
-                            self.segLayer.data = stored_mask
-                            self.segLayer.mode = "pan_zoom"
+                            modify_channel.data = stored_mask
+                            modify_channel.mode = "pan_zoom"
                     else:
-                        self.segLayer.data = stored_mask
-                        self.segLayer.mode = "pan_zoom"
+                        modify_channel.data = stored_mask
+                        modify_channel.mode = "pan_zoom"
                 else:
-                    self.segLayer.data = stored_mask
-                    self.segLayer.mode = "pan_zoom"
+                    modify_channel.data = stored_mask
+                    modify_channel.mode = "pan_zoom"
 
             # delete segmentations
             if self.segmentation_mode == "delete":
-                self.segLayer.mode = "paint"
-                self.segLayer.brush_size = 1
+                modify_channel.mode = "paint"
+                modify_channel.brush_size = 1
 
                 new_colour = _newSegColour(self)
-                stored_mask = self.segLayer.data.copy()
+                stored_mask = modify_channel.data.copy()
                 stored_class = self.classLayer.data
-                meta = self.segLayer.metadata.copy()
+                meta = modify_channel.metadata.copy()
 
                 dragged = False
                 coordinates = []
                 yield
 
                 # on move
                 while event.type == "mouse_move":
                     coordinates.append(event.position)
                     dragged = True
                     yield
 
                 # on release
                 if dragged:
-                    self.segLayer.data = stored_mask
+                    modify_channel.data = stored_mask
 
-                    coordinates = np.round(np.array(coordinates)).astype(np.int32)
+                    coordinates = np.round(np.array(coordinates)).astype(
+                        np.int32
+                    )
                     cnt = coordinates[:, -2:]
 
                     cnt = np.fliplr(cnt)
                     cnt = cnt.reshape((-1, 1, 2))
 
                     mask_dim = tuple(list(coordinates[0][:-2]) + [...])
 
-                    seg_stack = self.segLayer.data.copy()
+                    seg_stack = modify_channel.data.copy()
                     class_stack = self.classLayer.data.copy()
 
                     seg_mask = seg_stack[mask_dim]
                     class_mask = class_stack[mask_dim]
 
                     delete_mask = np.zeros_like(seg_mask)
                     cv2.drawContours(delete_mask, [cnt], -1, 255, -1)
@@ -352,342 +402,385 @@
                         seg_mask[seg_mask == colour] = 0
 
                     class_mask[seg_mask == 0] = 0
 
                     seg_stack[mask_dim] = seg_mask
                     class_stack[mask_dim] = class_mask
 
-                    self.segLayer.data = seg_stack
+                    modify_channel.data = seg_stack
                     self.classLayer.data = class_stack
 
                 else:
-                    self.segLayer.data = stored_mask
-                    self.segLayer.mode = "pan_zoom"
+                    modify_channel.data = stored_mask
+                    modify_channel.mode = "pan_zoom"
                     self.update_image_folds()
 
-                    meta = self.segLayer.metadata.copy()
+                    meta = modify_channel.metadata.copy()
 
-                    data_coordinates = self.segLayer.world_to_data(event.position)
+                    data_coordinates = modify_channel.world_to_data(
+                        event.position
+                    )
                     coord = np.round(data_coordinates).astype(int)
-                    mask_val = self.segLayer.get_value(coord)
+                    mask_val = modify_channel.get_value(coord)
 
                     if mask_val != 0:
                         mask_dim = tuple(list(coord[:-2]) + [...])[0]
 
-                        mask_stack = self.segLayer.data
+                        mask_stack = modify_channel.data
                         class_stack = self.classLayer.data
 
                         mask = mask_stack[mask_dim]
                         class_mask = class_stack[mask_dim]
 
                         class_mask[mask == mask_val] = 0
                         mask[mask == mask_val] = 0
 
                         class_stack[mask_dim] = class_mask
                         mask_stack[mask_dim] = mask
 
                         self.classLayer.data = class_stack
-                        self.segLayer.data = mask_stack
+                        modify_channel.data = mask_stack
 
                         # update metadata
 
                         meta["manual_segmentation"] = True
-                        self.segLayer.metadata = meta
-                        self.segLayer.mode = "pan_zoom"
+                        modify_channel.metadata = meta
+                        modify_channel.mode = "pan_zoom"
                         self.update_image_folds()
 
             if self.segmentation_mode == "refine":
-                layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+                layer_names = [
+                    layer.name
+                    for layer in self.viewer.layers
+                    if layer.name
+                    not in [
+                        "Segmentations",
+                        "Nucleoid",
+                        "Classes",
+                        "center_lines",
+                    ]
+                ]
 
-                self.segLayer.mode == "pan_zoom"
-                self.segLayer.brush_size = 1
+                modify_channel.mode == "pan_zoom"
+                modify_channel.brush_size = 1
 
-                data_coordinates = self.segLayer.world_to_data(event.position)
+                data_coordinates = modify_channel.world_to_data(event.position)
                 coord = np.round(data_coordinates).astype(int)
-                mask_id = self.segLayer.get_value(coord)
+                mask_id = modify_channel.get_value(coord)
 
-                self.segLayer.selected_label = mask_id
+                modify_channel.selected_label = mask_id
 
                 if mask_id != 0:
                     current_fov = self.viewer.dims.current_step[0]
 
                     channel = self.refine_channel.currentText()
                     channel = channel.replace("Mask + ", "")
 
                     label_stack = self.classLayer.data
-                    mask_stack = self.segLayer.data
+                    mask_stack = modify_channel.data
 
                     mask = mask_stack[current_fov, :, :].copy()
                     label = label_stack[current_fov, :, :].copy()
 
                     image = []
                     for layer in layer_names:
-                        image.append(self.viewer.layers[layer].data[current_fov])
+                        image.append(
+                            self.viewer.layers[layer].data[current_fov]
+                        )
                     image = np.stack(image, axis=0)
 
                     cell_mask = np.zeros(mask.shape, dtype=np.uint8)
 
                     mask[mask != mask_id] = 0
                     cell_mask[mask != mask_id] = 0
                     cell_mask[mask == mask_id] = 1
 
-                    from napari_bacseg._utils_colicoords import (process_colicoords, run_colicoords, )
+                    from napari_bacseg._utils_colicoords import (
+                        process_colicoords,
+                        run_colicoords,
+                    )
                     from napari_bacseg._utils_statistics import get_cell_images
 
-                    colicoords_dir = os.path.join(tempfile.gettempdir(), "colicoords")
-
-                    cell_images_path = get_cell_images(self, image, mask, cell_mask, mask_id, layer_names, colicoords_dir, )
+                    colicoords_dir = os.path.join(
+                        tempfile.gettempdir(), "colicoords"
+                    )
+
+                    cell_images_path = get_cell_images(
+                        self,
+                        image,
+                        mask,
+                        cell_mask,
+                        mask_id,
+                        layer_names,
+                        colicoords_dir,
+                    )
 
                     cell_data = {"cell_images_path": cell_images_path}
 
-                    colicoords_data = run_colicoords(self, cell_data=[cell_data], colicoords_channel=channel, multithreaded=True, )
+                    colicoords_data = run_colicoords(
+                        self,
+                        cell_data=[cell_data],
+                        colicoords_channel=channel,
+                        multithreaded=True,
+                    )
 
                     process_colicoords(self, colicoords_data)
 
         if self.interface_mode == "classify":
-            self.segLayer.mode == "pan_zoom"
-            self.segLayer.brush_size = 1
+            modify_channel.mode == "pan_zoom"
+            modify_channel.brush_size = 1
 
-            data_coordinates = self.segLayer.world_to_data(event.position)
+            data_coordinates = modify_channel.world_to_data(event.position)
             coord = np.round(data_coordinates).astype(int)
-            mask_val = self.segLayer.get_value(coord).copy()
+            mask_val = modify_channel.get_value(coord).copy()
 
-            self.segLayer.selected_label = mask_val
+            modify_channel.selected_label = mask_val
 
             if mask_val != 0:
-                stored_mask = self.segLayer.data.copy()
+                stored_mask = modify_channel.data.copy()
                 stored_class = self.classLayer.data.copy()
 
                 if len(stored_mask.shape) > 2:
                     current_fov = self.viewer.dims.current_step[0]
 
                     seg_mask = stored_mask[current_fov, :, :]
                     class_mask = stored_class[current_fov, :, :]
 
                     class_mask[seg_mask == mask_val] = self.class_colour
 
                     stored_class[current_fov, :, :] = class_mask
 
                     self.classLayer.data = stored_class
-                    self.segLayer.mode = "pan_zoom"
+                    modify_channel.mode = "pan_zoom"
 
                 else:
                     stored_class[stored_mask == mask_val] = self.class_colour
 
                     self.classLayer.data = stored_class
-                    self.segLayer.mode = "pan_zoom"
+                    modify_channel.mode = "pan_zoom"
 
         if self.interface_mode == "panzoom":
             mouse_button = event.button
 
-            data_coordinates = self.segLayer.world_to_data(event.position)
+            data_coordinates = modify_channel.world_to_data(event.position)
             coord = np.round(data_coordinates).astype(int)
 
         if self.modify_auto_panzoom.isChecked() == True:
             self.interface_mode = "panzoom"
             self.modify_panzoom.setEnabled(False)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(True)
 
     except:
         print(traceback.format_exc())
 
 
 def _newSegColour(self):
-    mask_stack = self.segLayer.data
+    if self.modify_channel.currentIndex() == 0:
+        modify_channel = self.segLayer
+    else:
+        modify_channel = self.nucLayer
 
+    mask_stack = modify_channel.data
     current_fov = self.viewer.dims.current_step[0]
 
     if len(mask_stack.shape) > 2:
         mask = mask_stack[current_fov, :, :]
     else:
         mask = mask_stack
 
     colours = np.unique(mask)
     new_colour = max(colours) + 1
 
-    self.segLayer.selected_label = new_colour
+    modify_channel.selected_label = new_colour
 
     return new_colour
 
 
 def _modifyMode(self, mode, viewer=None):
     def _event(viewer):
+        if self.modify_channel.currentIndex() == 0:
+            modify_channel = self.segLayer
+            self.viewer.layers.selection.active = self.segLayer
+        else:
+            modify_channel = self.nucLayer
+            self.viewer.layers.selection.active = self.nucLayer
+
         if mode == "panzoom":
-            self.segLayer.mode = "pan_zoom"
+            modify_channel.mode = "pan_zoom"
 
             self.interface_mode = "panzoom"
             self.modify_panzoom.setEnabled(False)
             self.modify_panzoom.setEnabled(False)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(True)
 
         if mode == "segment":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "add"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
             self.modify_classify.setEnabled(True)
 
         if mode == "classify":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "classify"
             self.segmentation_mode = "add"
             self.class_mode = 1
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
 
         if mode == "clicktozoom":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "clicktozoom"  # self.modify_panzoom.setEnabled(True)  # self.modify_segment.setEnabled(True)  # self.modify_classify.setEnabled(True)
 
         if mode == "add":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "add"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
             show_info("Add (click/drag to add)")
 
         if mode == "extend":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "extend"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
             show_info("Extend (click/drag to extend)")
 
         if mode == "join":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "join"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
             show_info("Join (click/drag to join)")
 
         if mode == "split":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "split"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
             show_info("Split (click/drag to split)")
 
         if mode == "delete":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "delete"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
             show_info("Delete (click/drag to delete)")
 
         if mode == "edit_vertex":
-            self.viewer.layers.selection.select_only(self.shapeLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "shapes"
             self.segmentation_mode = "edit_vertex"
 
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
 
         if mode == "refine":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "refine"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
             show_info("Refine (click to refine)")
 
         if self.interface_mode == "segment":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
         if mode == "single":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.class_mode = mode
             self.class_colour = 1
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
             show_info("Single (click to classify)")
 
         if mode == "dividing":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.class_mode = mode
             self.class_colour = 2
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
             show_info("Dividing (click to classify)")
 
         if mode == "divided":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.class_mode = mode
             self.class_colour = 3
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
             show_info("Divided (click to classify)")
 
         if mode == "vertical":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.class_mode = mode
             self.class_colour = 4
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
             show_info("Vertical (click to classify)")
 
         if mode == "broken":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.class_mode = mode
             self.class_colour = 5
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
             show_info("Broken (click to classify)")
 
         if mode == "edge":
-            self.viewer.layers.selection.select_only(self.segLayer)
+            self.viewer.layers.selection.select_only(modify_channel)
 
             self.class_mode = mode
             self.class_colour = 6
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
             show_info("Edge (click to classify)")
 
     return _event
 
 
 def autocontrast_values(image, clip_hist_percent=0.001):
     # calculate histogram
-    hist, bin_edges = np.histogram(image, bins=(2 ** 16) - 1)
+    hist, bin_edges = np.histogram(image, bins=(2**16) - 1)
     hist_size = len(hist)
 
     # calculate cumulative distribution from the histogram
     accumulator = cumsum(hist)
 
     # Locate points to clip
     maximum = accumulator[-1]
@@ -795,40 +888,54 @@
         if key == "viewlabels":
             self.classLayer.visible = self.modify_viewlabels.isChecked()
 
         if key == "viewmasks":
             self.segLayer.visible = self.modify_viewmasks.isChecked()
 
         if key == "c":
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+            ]
 
             if len(layer_names) != 0:
                 active_layer = layer_names[-1]
 
-                image_dims = tuple(list(self.viewer.dims.current_step[:-2]) + [...])
-
-                image = (self.viewer.layers[str(active_layer)].data[image_dims].copy())
-
-                crop = self.viewer.layers[str(active_layer)].corner_pixels[:, -2:]
+                image_dims = tuple(
+                    list(self.viewer.dims.current_step[:-2]) + [...]
+                )
+
+                image = (
+                    self.viewer.layers[str(active_layer)]
+                    .data[image_dims]
+                    .copy()
+                )
+
+                crop = self.viewer.layers[str(active_layer)].corner_pixels[
+                    :, -2:
+                ]
 
                 [[y1, x1], [y2, x2]] = crop
 
                 image_crop = image[y1:y2, x1:x2]
 
                 contrast_limit = [np.min(image_crop), np.max(image_crop)]
 
                 if contrast_limit[1] > contrast_limit[0]:
-                    self.viewer.layers[str(active_layer)].contrast_limits = contrast_limit
+                    self.viewer.layers[
+                        str(active_layer)
+                    ].contrast_limits = contrast_limit
 
     return _event
 
 
 def _imageControls(self, key, viewer=None):
     def _event(viewer):
-
         if key == "Upload":
             self._uploadDatabase("active")
 
         if len(self.viewer.dims.current_step) == 3:
             current_frame = self.viewer.dims.current_step[0]
             frame_range = int(self.viewer.dims.range[0][1]) - 1
 
@@ -880,15 +987,20 @@
 
 def _clear_images(self):
     self.segLayer.data = np.zeros((1, 100, 100), dtype=np.uint16)
 
     layer_names = [layer.name for layer in self.viewer.layers]
 
     for layer_name in layer_names:
-        if layer_name not in ["Segmentations", "Classes", "center_lines"]:
+        if layer_name not in [
+            "Segmentations",
+            "Nucleoid",
+            "Classes",
+            "center_lines",
+        ]:
             self.viewer.layers.remove(self.viewer.layers[layer_name])
 
 
 def _copymasktoall(self):
     current_fov = self.viewer.dims.current_step[0]
 
     mask = self.segLayer.data[current_fov]
@@ -924,15 +1036,17 @@
 
             else:
                 for image_index in range(*viewer_dims[0]):
                     mask = self.segLayer.data[image_index].copy()
                     mask_ids = np.unique(mask)
 
                     if len(viewer_dims) == 2:
-                        self.update_image_folds(mask_ids=mask_ids, image_index=image_index)
+                        self.update_image_folds(
+                            mask_ids=mask_ids, image_index=image_index
+                        )
 
                     else:
                         for mask_id in mask_ids:
                             mask[mask == mask_id] = 0
 
                         self.segLayer.data[image_index] = mask
                         self.segLayer.refresh()
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_json.py` & `napari-bacseg-1.0.7/src/_dev/json_nuclei_dev.py`

 * *Files 22% similar despite different names*

```diff
@@ -110,29 +110,69 @@
     with open(json_path, 'r') as f:
         dat = json.load(f)
 
     h = dat["images"][0]["height"]
     w = dat["images"][0]["width"]
 
     mask = np.zeros((h, w), dtype=np.uint16)
+    nmask = np.zeros((h, w), dtype=np.uint16)
     labels = np.zeros((h, w), dtype=np.uint16)
 
     categories = {}
 
     for i, cat in enumerate(dat["categories"]):
         cat_id = cat["id"]
         cat_name = cat["name"]
 
         categories[cat_id] = cat_name
 
     annotations = dat["annotations"]
 
     for i in range(len(annotations)):
         annot = annotations[i]["segmentation"][0]
+        
+        if "nucleoid_segmentation" in annotations[i].keys():
+            nucleoid_annot = annotations[i]["nucleoid_segmentation"][0]
+            cnt = np.array(nucleoid_annot).reshape(-1, 1, 2).astype(np.int32)
+            cv2.drawContours(nmask, [cnt], contourIdx=-1, color=i + 1, thickness=-1)
+            
         category_id = annotations[i]["category_id"]
 
         cnt = np.array(annot).reshape(-1, 1, 2).astype(np.int32)
 
         cv2.drawContours(mask, [cnt], contourIdx=-1, color=i + 1, thickness=-1)
         cv2.drawContours(labels, [cnt], contourIdx=-1, color=category_id, thickness=-1)
 
-    return mask, labels
+    return mask, labels
+
+
+
+
+
+
+
+
+
+json_dir = r"\\physics\dfs\DAQ\CondensedMatterGroups\AKGroup\Piers\AKSEG\Images\CF\json\110423_ConorDFP_L484840_AluGasketv12"
+
+from glob2 import glob
+
+json_files = glob(json_dir + "/*.txt")
+
+json_path = json_files[1]
+
+# json_path = os.path.splitext(json_path)[0] + ".txt"
+
+with open(json_path, 'r') as f:
+    dat = json.load(f)
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_oufti.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_oufti.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_refine.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_refine.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_statistics.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,67 @@
-# -*- coding: utf-8 -*-
 """
 Created on Wed Apr 27 10:32:45 2022
 
 @author: turnerp
 """
 
-import numpy as np
-import cv2
 import math
-from skimage import exposure
-import pandas as pd
 import os
 import tempfile
-from qtpy.QtWidgets import QFileDialog
-import shutil
-from functools import partial
-from napari.utils.notifications import show_info
+
+import cv2
+import numpy as np
+import pandas as pd
+from skimage import exposure
+
 
 def normalize99(X):
-    """ normalize image so 0.0 is 0.01st percentile and 1.0 is 99.99th percentile """
+    """normalize image so 0.0 is 0.01st percentile and 1.0 is 99.99th percentile"""
 
     if np.max(X) > 0:
         X = X.copy()
         v_min, v_max = np.percentile(X[X != 0], (1, 99))
         X = exposure.rescale_intensity(X, in_range=(v_min, v_max))
 
     return X
 
 
 def find_contours(img):
     # finds contours of shapes, only returns the external contours of the shapes
 
-    contours, hierarchy = cv2.findContours(img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE)
+    contours, hierarchy = cv2.findContours(
+        img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE
+    )
     contours = sorted(contours, key=cv2.contourArea, reverse=True)
     return contours
 
 
 def determine_overlap(cnt_num, contours, image):
-
     try:
-
         # gets current contour of interest
         cnt = contours[cnt_num]
 
         # number of pixels in contour
         cnt_pixels = len(cnt)
 
         # gets all other contours
         cnts = contours.copy()
         del cnts[cnt_num]
 
         # create mask of all contours, without contour of interest. Contours are filled
         cnts_mask = np.zeros(image.shape, dtype=np.uint8)
-        cv2.drawContours(cnts_mask, cnts, contourIdx=-1, color=(1, 1, 1), thickness=-1)
+        cv2.drawContours(
+            cnts_mask, cnts, contourIdx=-1, color=(1, 1, 1), thickness=-1
+        )
 
         # create mask of contour of interest. Only the contour outline is drawn.
         cnt_mask = np.zeros(image.shape, dtype=np.uint8)
-        cv2.drawContours(cnt_mask, [cnt], contourIdx=-1, color=(1, 1, 1), thickness=1)
+        cv2.drawContours(
+            cnt_mask, [cnt], contourIdx=-1, color=(1, 1, 1), thickness=1
+        )
 
         # dilate the contours mask. Neighbouring contours will now overlap.
         kernel = np.ones((3, 3), np.uint8)
         cnts_mask = cv2.dilate(cnts_mask, kernel, iterations=1)
 
         # get overlapping pixels
         overlap = cv2.bitwise_and(cnt_mask, cnts_mask)
@@ -74,15 +75,14 @@
     except:
         overlap_percentage = None
 
     return overlap_percentage
 
 
 def get_contour_statistics(cnt, image, pixel_size):
-
     # cell area
     try:
         area = cv2.contourArea(cnt) * pixel_size**2
     except:
         area = None
 
     # convex hull
@@ -113,27 +113,29 @@
         y1, y2, x1, x2 = y, (y + h), x, (x + w)
     except:
         y1, y2, x1, x2 = None, None, None, None
 
     # calculates moments, and centre of flake coordinates
     try:
         M = cv2.moments(cnt)
-        cx = int(M['m10'] / M['m00'])
-        cy = int(M['m01'] / M['m00'])
+        cx = int(M["m10"] / M["m00"])
+        cy = int(M["m01"] / M["m00"])
         cell_centre = [int(cx), int(cy)]
     except:
         cx = None
         cy = None
         cell_centre = [None, None]
 
     # cell length and width from PCA analysis
     try:
         cx, cy, lx, ly, wx, wy, data_pts = pca(cnt)
-        length, width, angle = get_pca_points(image, cnt, cx, cy, lx, ly, wx, wy)
-        radius = width/2
+        length, width, angle = get_pca_points(
+            image, cnt, cx, cy, lx, ly, wx, wy
+        )
+        radius = width / 2
         length = length * pixel_size
         width = width * pixel_size
         radius = radius * pixel_size
 
     except:
         length = None
         width = None
@@ -141,26 +143,28 @@
 
     # asepct ratio
     try:
         aspect_ratio = length / width
     except:
         aspect_ratio = None
 
-    contour_statistics = dict(numpy_BBOX=[x1, x2, y1, y2],
-                              coco_BBOX=[x1, y1, h, w],
-                              pascal_BBOX=[x1, y1, x2, y2],
-                              cell_centre=cell_centre,
-                              cell_area=area,
-                              cell_length=length,
-                              cell_width=width,
-                              cell_radius=radius,
-                              aspect_ratio=aspect_ratio,
-                              circumference=perimeter,
-                              solidity=solidity,
-                              aOp=aOp)
+    contour_statistics = dict(
+        numpy_BBOX=[x1, x2, y1, y2],
+        coco_BBOX=[x1, y1, h, w],
+        pascal_BBOX=[x1, y1, x2, y2],
+        cell_centre=cell_centre,
+        cell_area=area,
+        cell_length=length,
+        cell_width=width,
+        cell_radius=radius,
+        aspect_ratio=aspect_ratio,
+        circumference=perimeter,
+        solidity=solidity,
+        aOp=aOp,
+    )
 
     return contour_statistics
 
 
 def angle_of_line(x1, y1, x2, y2):
     try:
         angle = math.degrees(math.atan2(y2 - y1, x2 - x1))
@@ -185,36 +189,47 @@
         data_pts[i, 1] = pts[i, 0, 1]
 
     # #removes duplicate contour points
     arr, uniq_cnt = np.unique(data_pts, axis=0, return_counts=True)
     data_pts = arr[uniq_cnt == 1]
 
     # Perform PCA analysis
-    mean = np.empty((0))
+    mean = np.empty(0)
     mean, eigenvectors, eigenvalues = cv2.PCACompute2(data_pts, mean)
 
     # Store the center of the object
     cx, cy = (mean[0, 0], mean[0, 1])
-    lx, ly = (cx + 0.02 * eigenvectors[0, 0] * eigenvalues[0, 0], cy + 0.02 * eigenvectors[0, 1] * eigenvalues[0, 0])
-    wx, wy = (cx - 0.02 * eigenvectors[1, 0] * eigenvalues[1, 0], cy - 0.02 * eigenvectors[1, 1] * eigenvalues[1, 0])
+    lx, ly = (
+        cx + 0.02 * eigenvectors[0, 0] * eigenvalues[0, 0],
+        cy + 0.02 * eigenvectors[0, 1] * eigenvalues[0, 0],
+    )
+    wx, wy = (
+        cx - 0.02 * eigenvectors[1, 0] * eigenvalues[1, 0],
+        cy - 0.02 * eigenvectors[1, 1] * eigenvalues[1, 0],
+    )
 
     return cx, cy, lx, ly, wx, wy, data_pts
 
 
 def get_pca_points(img, cnt, cx, cy, lx, ly, wx, wy):
-
     if (lx - cx) == 0 or (wx - cx) == 0:
-
         pca_error = True
         length = 0
         width = 0
-        pca_points = {"lx1": 0, "ly1": 0, "lx2": 0, "ly2": 0,
-                      "wx1": 0, "wy1": 0, "wx2": 0, "wy2": 0, }
+        pca_points = {
+            "lx1": 0,
+            "ly1": 0,
+            "lx2": 0,
+            "ly2": 0,
+            "wx1": 0,
+            "wy1": 0,
+            "wx2": 0,
+            "wy2": 0,
+        }
     else:
-
         pca_error = False
 
         # get line slope and intercept
         length_slope = (ly - cy) / (lx - cx)
         length_intercept = cy - length_slope * cx
         width_slope = (wy - cy) / (wx - cx)
         width_intercept = cy - width_slope * cx
@@ -228,39 +243,68 @@
         wx2 = max(img.shape)
         wy1 = width_slope * wx1 + width_intercept
         wy2 = width_slope * wx2 + width_intercept
 
         contour_mask = np.zeros(img.shape, dtype=np.uint8)
         length_line_mask = np.zeros(img.shape, dtype=np.uint8)
         width_line_mask = np.zeros(img.shape, dtype=np.uint8)
-        cv2.drawContours(contour_mask, [cnt], contourIdx=-1, color=(255, 255, 255), thickness=-1)
-        cv2.line(length_line_mask, (int(lx1), int(ly1)), (int(lx2), int(ly2)), (255, 255, 255), 2)
-        cv2.line(width_line_mask, (int(wx1), int(wy1)), (int(wx2), int(wy2)), (255, 255, 255), 2)
+        cv2.drawContours(
+            contour_mask,
+            [cnt],
+            contourIdx=-1,
+            color=(255, 255, 255),
+            thickness=-1,
+        )
+        cv2.line(
+            length_line_mask,
+            (int(lx1), int(ly1)),
+            (int(lx2), int(ly2)),
+            (255, 255, 255),
+            2,
+        )
+        cv2.line(
+            width_line_mask,
+            (int(wx1), int(wy1)),
+            (int(wx2), int(wy2)),
+            (255, 255, 255),
+            2,
+        )
 
         Intersection = cv2.bitwise_and(contour_mask, length_line_mask)
         Intersection = np.array(np.where(Intersection.T == 255)).T
-        [[lx1, ly1], [lx2, ly2]] = np.array([Intersection[0], Intersection[-1]])
+        [[lx1, ly1], [lx2, ly2]] = np.array(
+            [Intersection[0], Intersection[-1]]
+        )
 
         Intersection = cv2.bitwise_and(contour_mask, width_line_mask)
         Intersection = np.array(np.where(Intersection.T == 255)).T
-        [[wx1, wy1], [wx2, wy2]] = np.array([Intersection[0], Intersection[-1]])
-
-        pca_points = {"lx1": lx1, "ly1": ly1, "lx2": lx2, "ly2": ly2,
-                      "wx1": wx1, "wy1": wy1, "wx2": wx2, "wy2": wy2, }
+        [[wx1, wy1], [wx2, wy2]] = np.array(
+            [Intersection[0], Intersection[-1]]
+        )
+
+        pca_points = {
+            "lx1": lx1,
+            "ly1": ly1,
+            "lx2": lx2,
+            "ly2": ly2,
+            "wx1": wx1,
+            "wy1": wy1,
+            "wx2": wx2,
+            "wy2": wy2,
+        }
 
         length = euclidian_distance(lx1, ly1, lx2, ly2)
         width = euclidian_distance(wx1, wy1, wx2, wy2)
 
         angle = angle_of_line(lx1, ly1, lx2, ly2)
 
     return length, width, angle
 
 
 def rotate_contour(cnt, angle=90, units="DEGREES"):
-
     x = cnt[:, :, 1].copy()
     y = cnt[:, :, 0].copy()
 
     x_shift, y_shift = sum(x) / len(x), sum(y) / len(y)
 
     # Shift to origin (0,0)
     x = x - int(x_shift)
@@ -279,28 +323,28 @@
 
     shift_xy = [x_shift[0], y_shift[0]]
 
     return cnt, shift_xy
 
 
 def rotate_image(image, shift_xy, angle=90):
-
     x_shift, y_shift = shift_xy
 
     (h, w) = image.shape[:2]
 
     # Perform image rotation
     M = cv2.getRotationMatrix2D((y_shift, x_shift), angle, 1.0)
     image = cv2.warpAffine(image, M, (w, h))
 
     return image, shift_xy
 
 
-def get_cell_images(self, image, mask, cell_mask, mask_id, layer_names, colicoords_dir):
-
+def get_cell_images(
+    self, image, mask, cell_mask, mask_id, layer_names, colicoords_dir
+):
     cell_image = image.copy()
 
     inverted_cell_mask = np.zeros(mask.shape, dtype=np.uint8)
     inverted_cell_mask[mask != 0] = 1
     inverted_cell_mask[mask == mask_id] = 0
 
     cnt = find_contours(cell_mask)[0]
@@ -308,15 +352,17 @@
     x, y, w, h = cv2.boundingRect(cnt)
 
     if h > w:
         vertical = True
         cell_mask = np.zeros(mask.shape, dtype=np.uint8)
         cnt, shift_xy = rotate_contour(cnt, angle=90)
         cell_image, shift_xy = rotate_image(cell_image, shift_xy, angle=90)
-        inverted_cell_mask, shift_xy = rotate_image(inverted_cell_mask, shift_xy, angle=90)
+        inverted_cell_mask, shift_xy = rotate_image(
+            inverted_cell_mask, shift_xy, angle=90
+        )
         cv2.drawContours(cell_mask, [cnt], -1, 1, -1)
     else:
         vertical = False
         shift_xy = None
 
     x, y, w, h = cv2.boundingRect(cnt)
     y1, y2, x1, x2 = y, (y + h), x, (x + w)
@@ -349,254 +395,331 @@
         x2 = cell_mask.shape[1]
         edge = True
 
     h, w = y2 - y1, x2 - x1
 
     inverted_cell_mask = inverted_cell_mask[y1:y2, x1:x2]
     cell_mask = cell_mask[y1:y2, x1:x2]
-    cell_image = cell_image[:,y1:y2, x1:x2]
+    cell_image = cell_image[:, y1:y2, x1:x2]
 
     for i in range(len(cell_image)):
-
         cell_img = cell_image[i].copy()
         cell_img[inverted_cell_mask == 1] = 0
         cell_img = normalize99(cell_img)
         cell_image[i] = cell_img
 
     offset = [y1, x1]
     box = [y1, y2, x1, x2]
 
-    cell_images = dict(cell_image=cell_image,
-                       cell_mask=cell_mask,
-                       channels=layer_names,
-                       offset=offset,
-                       shift_xy=shift_xy,
-                       box=box,
-                       edge=edge,
-                       vertical=vertical,
-                       mask_id=mask_id,
-                       contour=cnt)
+    cell_images = dict(
+        cell_image=cell_image,
+        cell_mask=cell_mask,
+        channels=layer_names,
+        offset=offset,
+        shift_xy=shift_xy,
+        box=box,
+        edge=edge,
+        vertical=vertical,
+        mask_id=mask_id,
+        contour=cnt,
+    )
 
     if os.path.isdir(colicoords_dir) is False:
         os.mkdir(colicoords_dir)
 
-    temp_path = tempfile.TemporaryFile(prefix="colicoords", suffix=".npy", dir=colicoords_dir).name
+    temp_path = tempfile.TemporaryFile(
+        prefix="colicoords", suffix=".npy", dir=colicoords_dir
+    ).name
 
-    np.save(temp_path,cell_images)
+    np.save(temp_path, cell_images)
 
     return temp_path
 
 
 def get_layer_statistics(image, cell_mask, box, layer_names):
-
     layer_statistics = {}
 
     for i in range(len(image)):
-
         layer = layer_names[i]
 
         x1, x2, y1, y2 = box
 
         cell_image_crop = image[i][y1:y2, x1:x2].copy()
         cell_mask_crop = cell_mask[y1:y2, x1:x2].copy()
 
         try:
-            cell_brightness = int(np.mean(cell_image_crop[cell_mask_crop != 0]))
-            cell_background_brightness = int(np.mean(cell_image_crop[cell_mask_crop == 0]))
+            cell_brightness = int(
+                np.mean(cell_image_crop[cell_mask_crop != 0])
+            )
+            cell_background_brightness = int(
+                np.mean(cell_image_crop[cell_mask_crop == 0])
+            )
             cell_contrast = cell_brightness / cell_background_brightness
-            cell_laplacian = int(cv2.Laplacian(cell_image_crop, cv2.CV_64F).var())
+            cell_laplacian = int(
+                cv2.Laplacian(cell_image_crop, cv2.CV_64F).var()
+            )
         except:
             cell_brightness = None
             cell_contrast = None
             cell_laplacian = None
 
-        stats = {"cell_brightness[" + layer + "]": cell_brightness,
-                 "cell_contrast[" + layer + "]": cell_contrast,
-                 "cell_laplacian[" + layer + "]": cell_laplacian}
+        stats = {
+            "cell_brightness[" + layer + "]": cell_brightness,
+            "cell_contrast[" + layer + "]": cell_contrast,
+            "cell_laplacian[" + layer + "]": cell_laplacian,
+        }
 
         layer_statistics = {**layer_statistics, **stats}
 
-    layer_statistics = {key: value for key, value in sorted(layer_statistics.items())}
+    layer_statistics = {
+        key: value for key, value in sorted(layer_statistics.items())
+    }
 
     return layer_statistics
 
 
-
-def get_cell_statistics(self, mode, pixel_size, colicoords_dir, progress_callback=None):
-
-    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes","center_lines"]]
+def get_cell_statistics(
+    self, mode, pixel_size, colicoords_dir, progress_callback=None
+):
+    layer_names = [
+        layer.name
+        for layer in self.viewer.layers
+        if layer.name
+        not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+    ]
 
     if mode == "active":
         dims = [self.viewer.dims.current_step[0]]
     else:
         dim_range = int(self.viewer.dims.range[0][1])
         dims = np.arange(0, dim_range)
 
     image_stack = []
     file_name_stack = []
 
     for i in dims:
-
         image = []
         file_names = []
 
         for layer in layer_names:
-
             image.append(self.viewer.layers[layer].data[i])
-            file_names.append(self.viewer.layers[layer].metadata[i]["image_name"])
+            file_names.append(
+                self.viewer.layers[layer].metadata[i]["image_name"]
+            )
 
         image = np.stack(image, axis=0)
         image_stack.append(image)
         file_name_stack.append(file_names)
 
     image_stack = np.stack(image_stack, axis=0)
 
     mask_stack = self.segLayer.data.copy()
     meta_stack = self.segLayer.metadata.copy()
     label_stack = self.classLayer.data.copy()
 
     if mode == "active":
-
         current_step = self.viewer.dims.current_step[0]
 
         mask_stack = np.expand_dims(mask_stack[current_step], axis=0)
         label_stack = np.expand_dims(label_stack[current_step], axis=0)
         meta_stack = np.expand_dims(meta_stack[current_step], axis=0)
 
     cell_statistics = []
 
-    cell_dict = {1: "Single", 2: "Dividing", 3: "Divided", 4: "Broken", 5: "Vertical", 6: "Edge"}
+    cell_dict = {
+        1: "Single",
+        2: "Dividing",
+        3: "Divided",
+        4: "Broken",
+        5: "Vertical",
+        6: "Edge",
+    }
 
     for i in range(len(image_stack)):
-
         progress = int(((i + 1) / len(image_stack)) * 100)
         progress_callback.emit(progress)
 
         image = image_stack[i]
         mask = mask_stack[i]
         meta = meta_stack[i]
         label = label_stack[i]
         file_names = file_name_stack[i]
 
         image_stats = {}
         for j in range(len(image)):
             layer = layer_names[j]
             img = image[j]
-            dat = {"image_brightness[" + layer + "]" : int(np.mean(img)),
-                   "image_laplacian[" + layer + "]": int(cv2.Laplacian(img, cv2.CV_64F).var())}
+            dat = {
+                "image_brightness[" + layer + "]": int(np.mean(img)),
+                "image_laplacian["
+                + layer
+                + "]": int(cv2.Laplacian(img, cv2.CV_64F).var()),
+            }
             image_stats = {**image_stats, **dat}
 
         contours = []
         contour_mask_ids = []
         cell_types = []
         mask_ids = np.unique(mask)
 
         for j in range(len(mask_ids)):
-
             mask_id = mask_ids[j]
 
             if mask_id != 0:
-
                 cell_mask = np.zeros(mask.shape, dtype=np.uint8)
                 cell_mask[mask == mask_id] = 1
 
                 cnt = find_contours(cell_mask)[0]
                 contours.append(cnt)
                 contour_mask_ids.append(mask_id)
 
                 cell_label = np.unique(label[mask == mask_id])[0]
 
                 if cell_label in cell_dict.keys():
                     cell_types.append(cell_dict[cell_label])
 
                     try:
                         background = np.zeros(mask.shape, dtype=np.uint8)
-                        cv2.drawContours(background, contours, contourIdx=-1, color=(1, 1, 1), thickness=-1)
+                        cv2.drawContours(
+                            background,
+                            contours,
+                            contourIdx=-1,
+                            color=(1, 1, 1),
+                            thickness=-1,
+                        )
                     except:
                         background = None
 
         for j in range(len(contours)):
-
             try:
-
                 cnt = contours[j]
                 mask_id = contour_mask_ids[j]
                 cell_type = cell_types[j]
 
                 cell_mask = np.zeros(mask.shape, dtype=np.uint8)
-                cv2.drawContours(cell_mask, [cnt], contourIdx=-1, color=(1, 1, 1), thickness=-1)
+                cv2.drawContours(
+                    cell_mask,
+                    [cnt],
+                    contourIdx=-1,
+                    color=(1, 1, 1),
+                    thickness=-1,
+                )
 
                 overlap_percentage = determine_overlap(j, contours, mask)
 
-                contour_statistics = get_contour_statistics(cnt, mask, pixel_size)
+                contour_statistics = get_contour_statistics(
+                    cnt, mask, pixel_size
+                )
 
                 box = contour_statistics["numpy_BBOX"]
 
-                cell_images_path = get_cell_images(self, image, mask, cell_mask, mask_id, layer_names, colicoords_dir)
-
-                layer_stats = get_layer_statistics(image, cell_mask, box, layer_names)
-
-                morphology_stats = dict(file_names=file_names,
-                                        colicoords=False,
-                                        cell_type=cell_type,
-                                        pixel_size_um=pixel_size,
-                                        length=contour_statistics["cell_length"],
-                                        radius=(contour_statistics["cell_radius"]),
-                                        area=contour_statistics["cell_area"],
-                                        circumference=contour_statistics["circumference"],
-                                        aspect_ratio=contour_statistics["aspect_ratio"],
-                                        solidity=contour_statistics["solidity"],
-                                        overlap_percentage=overlap_percentage,
-                                        box=box,
-                                        cell_images_path = cell_images_path)
+                cell_images_path = get_cell_images(
+                    self,
+                    image,
+                    mask,
+                    cell_mask,
+                    mask_id,
+                    layer_names,
+                    colicoords_dir,
+                )
+
+                layer_stats = get_layer_statistics(
+                    image, cell_mask, box, layer_names
+                )
+
+                morphology_stats = dict(
+                    file_names=file_names,
+                    colicoords=False,
+                    cell_type=cell_type,
+                    pixel_size_um=pixel_size,
+                    length=contour_statistics["cell_length"],
+                    radius=(contour_statistics["cell_radius"]),
+                    area=contour_statistics["cell_area"],
+                    circumference=contour_statistics["circumference"],
+                    aspect_ratio=contour_statistics["aspect_ratio"],
+                    solidity=contour_statistics["solidity"],
+                    overlap_percentage=overlap_percentage,
+                    box=box,
+                    cell_images_path=cell_images_path,
+                )
 
                 stats = {**morphology_stats, **image_stats, **layer_stats}
 
                 cell_statistics.append(stats)
 
             except:
                 pass
 
     return cell_statistics
 
 
-def process_cell_statistics(self,cell_statistics,path):
-
+def process_cell_statistics(self, cell_statistics, path):
     def _event(viewer, cell_statistics=None):
-
         if type(cell_statistics) == dict:
             ldist_data = cell_statistics["ldist_data"]
-            ldist_data = pd.DataFrame.from_dict(ldist_data).dropna(how='all')
+            ldist_data = pd.DataFrame.from_dict(ldist_data).dropna(how="all")
             cell_statistics = cell_statistics["cell_statistics"]
         else:
             ldist_data = None
 
-        export_path = os.path.join(path,'statistics.xlsx')
+        export_path = os.path.join(path, "statistics.xlsx")
 
-        drop_columns = ['cell_image', 'cell_mask','offset', 'shift_xy','edge',
-                        'vertical','mask_id','contour','edge','vertical','mask_id','cell','refined_cnt',
-                        'oufti','statistics','colicoords_channel','channels','cell_images_path', 'ldist']
+        drop_columns = [
+            "cell_image",
+            "cell_mask",
+            "offset",
+            "shift_xy",
+            "edge",
+            "vertical",
+            "mask_id",
+            "contour",
+            "edge",
+            "vertical",
+            "mask_id",
+            "cell",
+            "refined_cnt",
+            "oufti",
+            "statistics",
+            "colicoords_channel",
+            "channels",
+            "cell_images_path",
+            "ldist",
+        ]
 
         cell_statistics = pd.DataFrame(cell_statistics)
 
-        cell_statistics = cell_statistics.drop(columns=[col for col in cell_statistics if col in drop_columns])
+        cell_statistics = cell_statistics.drop(
+            columns=[col for col in cell_statistics if col in drop_columns]
+        )
 
-        cell_statistics = cell_statistics.dropna(how='all')
+        cell_statistics = cell_statistics.dropna(how="all")
 
         with pd.ExcelWriter(export_path) as writer:
-            cell_statistics.to_excel(writer, sheet_name='Cell Statistics', index=False, startrow=1, startcol=1,)
+            cell_statistics.to_excel(
+                writer,
+                sheet_name="Cell Statistics",
+                index=False,
+                startrow=1,
+                startcol=1,
+            )
             if isinstance(ldist_data, pd.DataFrame):
-                ldist_data.to_excel(writer, sheet_name='Length Distribution Data', index=False, startrow=1, startcol=1)
+                ldist_data.to_excel(
+                    writer,
+                    sheet_name="Length Distribution Data",
+                    index=False,
+                    startrow=1,
+                    startcol=1,
+                )
 
         return
 
     return _event
 
-def _compute_simple_cell_stats(self):
 
+def _compute_simple_cell_stats(self):
     if self.unfolded == True:
         self.fold_images()
 
     current_fov = self.viewer.dims.current_step[0]
 
     mask = self.segLayer.data[current_fov]
 
@@ -606,21 +729,21 @@
     cell_solidity = []
     cell_aspect_ratio = []
     cell_centre = []
     cell_zoom = []
     cell_id = []
 
     for mask_id in mask_ids:
-
         if mask_id != 0:
-
             cnt_mask = np.zeros(mask.shape, dtype=np.uint8)
-            cnt_mask[mask==mask_id] = 255
+            cnt_mask[mask == mask_id] = 255
 
-            cnt, _ = cv2.findContours(cnt_mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE)
+            cnt, _ = cv2.findContours(
+                cnt_mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE
+            )
 
             x, y, w, h = cv2.boundingRect(cnt[0])
             y1, y2, x1, x2 = y, (y + h), x, (x + w)
 
             try:
                 area = cv2.contourArea(cnt[0])
                 hull = cv2.convexHull(cnt[0])
@@ -632,30 +755,34 @@
             except:
                 area = 0
                 solidity = 0
                 aspect_ratio = 0
 
             centre = (0, y1 + (y2 - y1) // 2, x1 + (x2 - x1) // 2)
 
-            zoom = min((mask.shape[0]/(y2-y1)), (mask.shape[1]/(x2-x1)))/2
+            zoom = (
+                min((mask.shape[0] / (y2 - y1)), (mask.shape[1] / (x2 - x1)))
+                / 2
+            )
 
             cell_area.append(area)
             cell_solidity.append(solidity)
             cell_aspect_ratio.append(aspect_ratio)
             cell_centre.append(centre)
             cell_zoom.append(zoom)
             cell_id.append(mask_id)
 
-    cell_stats = {'cell_area': cell_area,
-                  'cell_solidity':cell_solidity,
-                  'cell_aspect_ratio':cell_aspect_ratio,
-                  'cell_centre': cell_centre,
-                  'cell_zoom': cell_zoom,
-                  'mask_id': cell_id}
+    cell_stats = {
+        "cell_area": cell_area,
+        "cell_solidity": cell_solidity,
+        "cell_aspect_ratio": cell_aspect_ratio,
+        "cell_centre": cell_centre,
+        "cell_zoom": cell_zoom,
+        "mask_id": cell_id,
+    }
 
     layer_names = [layer.name for layer in self.viewer.layers if layer.name]
 
     for layer in layer_names:
-
         meta = self.viewer.layers[layer].metadata[current_fov]
-        meta['simple_cell_stats'] = cell_stats
-        self.viewer.layers[layer].metadata[current_fov] = meta
+        meta["simple_cell_stats"] = cell_stats
+        self.viewer.layers[layer].metadata[current_fov] = meta
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_utils_tiler.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_utils_tiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-
-
 import numpy as np
-from tiler import Tiler, Merger
+from tiler import Merger
 
 
 def unfold_images(self):
-
     if self.unfolded == False:
-
         current_step = list(self.viewer.dims.current_step)
         current_step = [0] * len(current_step)
         self.viewer.dims.current_step = tuple(current_step)
 
-        from tiler import Tiler, Merger
+        from tiler import Tiler
 
         layer_names = [layer.name for layer in self.viewer.layers]
 
         tile_size = int(self.unfold_tile_size.currentText())
         tile_shape = (tile_size, tile_size)
         overlap = int(self.unfold_tile_overlap.currentText())
 
         for layer in layer_names:
-
             image = self.viewer.layers[layer].data.copy()
             metadata_stack = self.viewer.layers[layer].metadata.copy()
 
-            self.tiler_object = Tiler(data_shape=image[0].shape,
-                                      tile_shape=tile_shape,
-                                      overlap=overlap)
+            self.tiler_object = Tiler(
+                data_shape=image[0].shape,
+                tile_shape=tile_shape,
+                overlap=overlap,
+            )
 
             if self.unfold_mode.currentIndex() == 0:
-
                 tiled_image = []
 
                 for i in range(image.shape[0]):
-
                     tiles = []
 
                     for tile_id, tile in self.tiler_object.iterate(image[i]):
                         tiles.append(tile)
 
                     tiles = np.stack(tiles)
                     tiled_image.append(tiles)
@@ -49,95 +44,105 @@
                 self.viewer.layers[layer].ndisplay = 3
                 self.viewer.reset_view()
 
                 self.unfolded = True
                 self._autoContrast()
 
             if self.unfold_mode.currentIndex() == 1:
-
                 from napari_bacseg._utils import get_hash
 
                 tiled_images = []
                 tiled_metadata = {}
 
                 for i in range(image.shape[0]):
-
                     num_image_tiles = 0
 
                     for tile_id, tile in self.tiler_object.iterate(image[i]):
-
-                        bbox = np.array(self.tiler_object.get_tile_bbox(tile_id=tile_id))
+                        bbox = np.array(
+                            self.tiler_object.get_tile_bbox(tile_id=tile_id)
+                        )
                         bbox = bbox[..., [-2, -1]]
-                        y1, x1, y2, x2 = bbox[0][0], bbox[0][1], bbox[1][0], bbox[1][1]
+                        y1, x1, y2, x2 = (
+                            bbox[0][0],
+                            bbox[0][1],
+                            bbox[1][0],
+                            bbox[1][1],
+                        )
 
                         if y2 > image.shape[-2]:
                             y2 = image.shape[-2]
                         if x2 > image.shape[-1]:
                             x2 = image.shape[-1]
 
                         x2 = x2 - x1
                         x1 = 0
                         y2 = y2 - y1
                         y1 = 0
 
                         if (y2 - y1, x2 - x1) == tile_shape:
-
                             num_image_tiles += 1
                             tiled_images.append(tile)
 
                             if layer != "Classes":
                                 meta = dict(metadata_stack[i])
                                 image_name = meta["image_name"]
 
                                 tile_meta = dict(meta)
-                                tile_name = str(image_name).split(".")[0] + "_tile" + str(num_image_tiles) + ".tif"
+                                tile_name = (
+                                    str(image_name).split(".")[0]
+                                    + "_tile"
+                                    + str(num_image_tiles)
+                                    + ".tif"
+                                )
                                 tile_meta["akseg_hash"] = get_hash(img=tile)
                                 tile_meta["image_name"] = tile_name
-                                tile_meta["dims"] = [tile.shape[-1], tile.shape[-2]]
-                                tile_meta["crop"] = [int(y1), int(y2), int(x1), int(x2)]
-
-                                tiled_metadata[len(tiled_images) - 1] = tile_meta
+                                tile_meta["dims"] = [
+                                    tile.shape[-1],
+                                    tile.shape[-2],
+                                ]
+                                tile_meta["crop"] = [
+                                    int(y1),
+                                    int(y2),
+                                    int(x1),
+                                    int(x2),
+                                ]
+
+                                tiled_metadata[
+                                    len(tiled_images) - 1
+                                ] = tile_meta
 
                 image = np.stack(tiled_images)
                 self.viewer.layers[layer].data = image
                 self.viewer.layers[layer].ndisplay = 2
                 self.viewer.reset_view()
                 self.unfolded = False
                 self._autoContrast()
 
                 if layer != "Classes":
                     self.viewer.layers[layer].metadata = tiled_metadata
 
     self._updateFileName()
 
 
-
-
-
-
 def fold_images(self):
-
     if self.unfolded == True:
-
         current_step = list(self.viewer.dims.current_step)
         current_step = [0] * len(current_step)
         self.viewer.dims.current_step = tuple(current_step)
 
         layer_names = [layer.name for layer in self.viewer.layers]
 
         for layer in layer_names:
-
             image = self.viewer.layers[layer].data.copy()
 
             merger = Merger(self.tiler_object)
 
             merged_image = []
 
             for i in range(image.shape[0]):
-
                 merger.reset()
 
                 for j in range(image.shape[1]):
                     img = image[i, j].copy()
 
                     merger.add(j, img.data)
 
@@ -149,78 +154,77 @@
             self.viewer.layers[layer].data = image
             self.viewer.layers[layer].ndisplay = 2
             self.viewer.reset_view()
             self.unfolded = False
             self._autoContrast()
 
 
-def update_image_folds(self, mask_ids = None, image_index = None):
-
+def update_image_folds(self, mask_ids=None, image_index=None):
     if self.unfolded == True:
+        from tiler import Merger
 
-        from tiler import Tiler, Merger
-
-        layer_names = ["Segmentations", "Classes"]
+        layer_names = ["Segmentations", "Nucleoid", "Classes"]
 
         if image_index is not None:
             target_img_id = image_index
         else:
             target_img_id = self.viewer.dims.current_step[0]
 
         target_tile_id = self.viewer.dims.current_step[1]
 
         for layer in layer_names:
-
             image = self.viewer.layers[layer].data.copy()
 
             frame = image[target_img_id]
 
             merger = Merger(self.tiler_object)
 
             merger.reset()
 
             overwrite_tile_box = []
             overwrite_tile_img = []
 
             for j in range(frame.shape[0]):
-
                 img = frame[j].copy()
 
                 if j == target_tile_id:
-                    overwrite_tile_box = np.array(self.tiler_object.get_tile_bbox(target_tile_id))
+                    overwrite_tile_box = np.array(
+                        self.tiler_object.get_tile_bbox(target_tile_id)
+                    )
                     overwrite_tile_box = overwrite_tile_box[..., [-2, -1]]
                     overwrite_tile_img = img
 
                 merger.add(j, img.data)
 
-            y1, x1, y2, x2 = overwrite_tile_box[0][0], overwrite_tile_box[0][1], \
-                             overwrite_tile_box[1][0], overwrite_tile_box[1][1]
+            y1, x1, y2, x2 = (
+                overwrite_tile_box[0][0],
+                overwrite_tile_box[0][1],
+                overwrite_tile_box[1][0],
+                overwrite_tile_box[1][1],
+            )
 
             frame = merger.merge(dtype=img.dtype)
 
             if y1 < 0:
                 y1 = 0
             if y2 > frame.shape[0]:
                 y2 = frame.shape[0]
             if x1 < 0:
                 x1 = 0
             if x2 > frame.shape[1]:
                 x2 = frame.shape[1]
 
-            frame[y1:y2, x1:x2] = overwrite_tile_img[:y2 - y1, :x2 - x1]
+            frame[y1:y2, x1:x2] = overwrite_tile_img[: y2 - y1, : x2 - x1]
 
             if mask_ids is not None:
-
                 for mask_id in mask_ids:
-                    frame[frame==mask_id] = 0
+                    frame[frame == mask_id] = 0
 
             tiles = []
 
             for tile_id, tile in self.tiler_object.iterate(frame):
                 tiles.append(tile)
 
             tiles = np.stack(tiles)
 
             image[target_img_id] = tiles
             self.viewer.layers[layer].data = image
-
-
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/_widget.py` & `napari-bacseg-1.0.7/src/napari_bacseg/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
         super().__init__()
 
         # import functions
         from napari_bacseg._utils import _manualImport, stack_images
         from napari_bacseg._utils_cellpose import (_initialise_cellpose_model, _select_cellpose_save_directory, _select_cellpose_save_path, _select_custom_cellpose_model, train_cellpose_model, )
         from napari_bacseg._utils_database import (_create_bacseg_database, _load_bacseg_database, _populateUSERMETA, _show_database_controls, populate_upload_combos, update_database_metadata, )
-        from napari_bacseg._utils_interface_events import (_copymasktoall, _delete_active_image, _deleteallmasks, _doubeClickEvents, _imageControls, _modifyMode, _segmentationEvents, _viewerControls, )
+        from napari_bacseg._utils_interface_events import (_copymasktoall, _delete_active_image, _deleteallmasks, _doubeClickEvents, _imageControls, _modify_channel_changed, _modifyMode, _segmentationEvents, _viewerControls, )
         from napari_bacseg._utils_oufti import (_update_active_midlines, centre_oufti_midlines, generate_midlines, midline_edit_toggle, update_midlines, )
         from napari_bacseg._utils_statistics import _compute_simple_cell_stats
         from napari_bacseg._utils_tiler import (fold_images, unfold_images, update_image_folds, )
         from napari_bacseg.bacseg_ui import Ui_tab_widget
 
         self.populate_upload_combos = self.wrapper(populate_upload_combos)
         self.update_database_metadata = self.wrapper(update_database_metadata)
@@ -159,14 +159,15 @@
         self._viewerControls = self.wrapper(_viewerControls)
         self._copymasktoall = self.wrapper(_copymasktoall)
         self._deleteallmasks = self.wrapper(_deleteallmasks)
         self._delete_active_image = self.wrapper(_delete_active_image)
         self._populateUSERMETA = self.wrapper(_populateUSERMETA)
         self._imageControls = self.wrapper(_imageControls)
         self._segmentationEvents = self.wrapper(_segmentationEvents)
+        self._modify_channel_changed = self.wrapper(_modify_channel_changed)
         self._manualImport = self.wrapper(_manualImport)
         self.train_cellpose_model = self.wrapper(train_cellpose_model)
         self._initialise_cellpose_model = self.wrapper(_initialise_cellpose_model)
         self._select_custom_cellpose_model = self.wrapper(_select_custom_cellpose_model)
         self._select_cellpose_save_directory = self.wrapper(_select_cellpose_save_directory)
         self._select_cellpose_save_path = self.wrapper(_select_cellpose_save_path)
         self.unfold_images = self.wrapper(unfold_images)
@@ -279,14 +280,16 @@
         self.cellpose_resetimage = self.findChild(QCheckBox, "cellpose_resetimage")
         self.cellpose_progressbar = self.findChild(QProgressBar, "cellpose_progressbar")
         self.cellpose_train_model = self.findChild(QPushButton, "cellpose_train_model")
         self.cellpose_save_dir = self.findChild(QPushButton, "cellpose_save_dir")
         self.cellpose_trainchannel = self.findChild(QComboBox, "cellpose_trainchannel")
         self.cellpose_nepochs = self.findChild(QComboBox, "cellpose_nepochs")
         self.cellpose_batchsize = self.findChild(QComboBox, "cellpose_batchsize")
+        self.cellpose_min_seg_size = self.findChild(QComboBox, "cellpose_min_seg_size")
+        self.cellpose_seg_mode = self.findChild(QComboBox, "cellpose_seg_mode")
 
         # modify tab controls + variables from Qt Desinger References
         self.interface_mode = "panzoom"
         self.segmentation_mode = "add"
         self.class_mode = "single"
         self.class_colour = 1
         self.modify_panzoom = self.findChild(QPushButton, "modify_panzoom")
@@ -297,14 +300,15 @@
         self.refine_all = self.findChild(QPushButton, "refine_all")
         self.modify_copymasktoall = self.findChild(QPushButton, "modify_copymasktoall")
         self.modify_deleteallmasks = self.findChild(QPushButton, "modify_deleteallmasks")
         self.modify_deleteactivemasks = self.findChild(QPushButton, "modify_deleteactivemasks")
         self.modify_deleteactiveimage = self.findChild(QPushButton, "modify_deleteactiveimage")
         self.modify_deleteotherimages = self.findChild(QPushButton, "modify_deleteotherimages")
         self.modify_progressbar = self.findChild(QProgressBar, "modify_progressbar")
+        self.modify_channel = self.findChild(QComboBox, "modify_channel")
 
         self.modify_auto_panzoom = self.findChild(QCheckBox, "modify_auto_panzoom")
         self.modify_add = self.findChild(QPushButton, "modify_add")
         self.modify_extend = self.findChild(QPushButton, "modify_extend")
         self.modify_split = self.findChild(QPushButton, "modify_split")
         self.modify_join = self.findChild(QPushButton, "modify_join")
         self.modify_delete = self.findChild(QPushButton, "modify_delete")
@@ -426,14 +430,23 @@
         self.export_scalebar_size = self.findChild(QLineEdit, "export_scalebar_size")
         self.export_scalebar_size_units = self.findChild(QComboBox, "export_scalebar_size_units")
         self.export_scalebar_colour = self.findChild(QComboBox, "export_scalebar_colour")
         self.export_scalebar_thickness = self.findChild(QComboBox, "export_scalebar_thickness")
         self.export_cropzoom = self.findChild(QCheckBox, "export_crop_zoom")
         self.export_mask_background = self.findChild(QCheckBox, "export_mask_background")
 
+        self.export_stack_channel = self.findChild(QComboBox, "export_stack_channel")
+        self.export_stack_mode = self.findChild(QComboBox, "export_stack_mode")
+        self.export_stack_location = self.findChild(QComboBox, "export_stack_location")
+        self.export_stack_modifier = self.findChild(QLineEdit, "export_stack_modifier")
+        self.export_stack_image_setting = self.findChild(QCheckBox, "export_stack_image_setting")
+        self.export_stack_overwrite_setting = self.findChild(QCheckBox, "export_stack_overwrite_setting")
+        self.export_stack_active = self.findChild(QPushButton, "export_stack_active")
+        self.export_stack_all = self.findChild(QPushButton, "export_stack_all")
+
         self.export_autocontrast = self.findChild(QCheckBox, "export_autocontrast")
         self.export_statistics_pixelsize = self.findChild(QLineEdit, "export_statistics_pixelsize")
         self.export_statistics_active = self.findChild(QPushButton, "export_statistics_active")
         self.export_statistics_all = self.findChild(QPushButton, "export_statistics_all")
         self.export_colicoords_mode = self.findChild(QComboBox, "export_colicoords_mode")
         self.export_progressbar = self.findChild(QProgressBar, "export_progressbar")
         self.export_image_setting = self.findChild(QCheckBox, "export_image_setting")
@@ -445,15 +458,15 @@
         self.import_import.clicked.connect(self._importDialog)
         self.label_overwrite.clicked.connect(self.overwrite_channel_info)
 
         # view events
         self.fold.clicked.connect(self.fold_images)
         self.unfold.clicked.connect(self.unfold_images)
         self.tiler_object = None
-        self.tile_dict = {"Segmentations": [], "Classes": []}
+        self.tile_dict = {"Segmentations": [], "Classes": [], "Nucleoid": []}
         self.unfolded = False
         self.align_active_image.clicked.connect(partial(self._align_images, mode="active"))
         self.align_all_images.clicked.connect(partial(self._align_images, mode="all"))
         self.scalebar_show.stateChanged.connect(self._updateScaleBar)
         self.scalebar_resolution.textChanged.connect(self._updateScaleBar)
         self.scalebar_units.currentTextChanged.connect(self._updateScaleBar)
         self.overlay_filename.stateChanged.connect(self._updateFileName)
@@ -524,18 +537,21 @@
         self.modify_copymasktoall.clicked.connect(self._copymasktoall)
         self.modify_deleteallmasks.clicked.connect(self._deleteallmasks(mode="all"))
         self.modify_deleteactivemasks.clicked.connect(self._deleteallmasks(mode="active"))
         self.modify_deleteactiveimage.clicked.connect(self._delete_active_image(mode="active"))
         self.modify_deleteotherimages.clicked.connect(self._delete_active_image(mode="other"))
         self.find_next.clicked.connect(self._sort_cells("next"))
         self.find_previous.clicked.connect(self._sort_cells("previous"))
+        self.modify_channel.currentTextChanged.connect(self._modify_channel_changed)
 
         # export events
         self.export_active.clicked.connect(self._export("active"))
         self.export_all.clicked.connect(self._export("all"))
+        self.export_stack_active.clicked.connect(self._export_stack("active"))
+        self.export_stack_all.clicked.connect(self._export_stack("all"))
         self.export_statistics_active.clicked.connect(self._export_statistics("active"))
         self.export_statistics_all.clicked.connect(self._export_statistics("all"))
 
         # oufti events
         self.oufti_generate_all_midlines.clicked.connect(self.generate_midlines(mode="all"))
         self.oufti_generate_active_midlines.clicked.connect(self.generate_midlines(mode="active"))
         self.viewer.bind_key(key="m", func=self.midline_edit_toggle, overwrite=True)
@@ -559,14 +575,15 @@
         self.viewer.dims.events.current_step.connect(self._sliderEvent)
 
         # self.segImage = self.viewer.add_image(np.zeros((1,100,100),dtype=np.uint16),name="Image")
         self.class_colours = {1: (255 / 255, 255 / 255, 255 / 255, 1), 2: (0 / 255, 255 / 255, 0 / 255, 1), 3: (0 / 255, 170 / 255, 255 / 255, 1), 4: (170 / 255, 0 / 255, 255 / 255, 1), 5: (
         255 / 255, 170 / 255, 0 / 255, 1), 6: (255 / 255, 0 / 255, 0 / 255, 1), }
 
         self.classLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=0.25, name="Classes", color=self.class_colours, metadata={0: {"image_name": ""}}, visible=False, )
+        self.nucLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=1, name="Nucleoid", metadata={0: {"image_name": ""}}, )
         self.segLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=1, name="Segmentations", metadata={0: {"image_name": ""}}, )
 
         self.segLayer.contour = 1
 
         # keyboard events, only triggered when viewer is not empty (an image is loaded/active)
         self.viewer.bind_key(key="a", func=self._modifyMode(mode="add"), overwrite=True)
         self.viewer.bind_key(key="e", func=self._modifyMode(mode="extend"), overwrite=True)
@@ -613,61 +630,57 @@
         self.viewer.bind_key(key="Alt-Down", func=self._manual_align_channels("down", mode="all"), overwrite=True, )
 
         self.import_filemode.currentIndexChanged.connect(self.update_import_limit)
         self.update_import_limit()
 
         # mouse events
         self.segLayer.mouse_drag_callbacks.append(self._segmentationEvents)
+        self.nucLayer.mouse_drag_callbacks.append(self._segmentationEvents)
+
         # self.segLayer.mouse_move_callbac1ks.append(self._zoomEvents)
         self.segLayer.mouse_double_click_callbacks.append(self._doubeClickEvents)
 
         # viewer events
         self.viewer.layers.events.inserted.connect(self._manualImport)
         self.viewer.layers.events.removed.connect(self._updateSegmentationCombo)
         self.viewer.layers.selection.events.changed.connect(self._updateFileName)
 
         self.threadpool = QThreadPool()  # self.load_dev_data()
 
         self.widget_notifications = True
 
-
     def _applyZoom(self):
-
         try:
-
             import re
 
             magnification = self.zoom_magnification.currentText()
             pixel_resolution = float(self.scalebar_resolution.text())
-            magnification = magnification.lower().replace("x","").replace("%","")
+            magnification = (magnification.lower().replace("x", "").replace("%", ""))
 
-            magnification = re.findall(r'\b\d+\b',magnification)[0]
+            magnification = re.findall(r"\b\d+\b", magnification)[0]
 
             if magnification.isdigit():
                 magnification = int(magnification)
 
                 if magnification == 0:
                     self.viewer.reset_view()
                 elif magnification > 0:
+                    magnification = 1 + magnification / 100
 
-                    magnification = (1 + magnification/100)
-
-                    self.viewer.camera.zoom = magnification * (1/pixel_resolution)
+                    self.viewer.camera.zoom = magnification * (1 / pixel_resolution)
 
         except:
             print(traceback.format_exc())
-            pass
-
 
     def _align_images(self, viewer=None, mode="active"):
         import scipy
         from skimage.registration import phase_cross_correlation
 
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
             if len(layer_names) > 2:
                 num_images = self.viewer.layers[layer_names[0]].data.shape[0]
 
                 if mode == "active":
                     fov_list = [self.viewer.dims.current_step[0]]
                 else:
@@ -703,15 +716,15 @@
         self.set_image_quality(mode="focus", value=1)
 
     def set_focused(self, viewer=None):
         self.set_image_quality(mode="focus", value=5)
 
     def set_image_quality(self, mode="", value=""):
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
             update_mode = self.set_quality_mode.currentIndex()
 
             if len(layer_names) > 0:
                 current_fov = self.viewer.dims.current_step[0]
                 n_frames = self.viewer.dims.nsteps[0]
                 active_layer = self.viewer.layers.selection.active.name
@@ -760,15 +773,15 @@
         all_layers = [layer.name for layer in self.viewer.layers]
         selected_layers = [layer.name for layer in self.viewer.layers.selection]
 
         if len(selected_layers) == 1:
             selected_layer = selected_layers[0]
             all_layers.pop(all_layers.index(selected_layer))
 
-            if selected_layer not in ["Segmentations", "Classes", "center_lines", ]:
+            if selected_layer not in ["Segmentations", "Nucleoid", "Classes", "center_lines", ]:
                 metadata = self.viewer.layers[selected_layer].metadata.copy()
 
                 label_modality = self.label_modality.currentText()
                 label_light_source = self.label_light_source.currentText()
                 label_stain = self.label_stain.currentText()
                 label_stain_target = self.label_stain_target.currentText()
 
@@ -1057,25 +1070,24 @@
                     (measurements, file_paths, channels,) = self.get_filtered_database_metadata()
 
                     if len(file_paths) == 0:
                         if self.widget_notifications:
                             show_info("no matching database files found")
 
                     else:
-
                         worker = Worker(self.read_bacseg_images, measurements=measurements, channels=channels, )
                         worker.signals.result.connect(self._process_import)
                         worker.signals.progress.connect(partial(self._Progresbar, progressbar="database"))
                         self.threadpool.start(worker)
 
         except:
             print(traceback.format_exc())
 
     def _updateSegChannels(self):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
         segChannel = self.cellpose_segchannel.currentText()
 
         self.export_channel.setCurrentText(segChannel)
 
     def _Progresbar(self, progress, progressbar):
         if progressbar == "import":
@@ -1186,14 +1198,37 @@
                 measurements, file_paths, channels = read_scanr_directory(self, paths)
 
                 worker = Worker(self.read_scanr_images, measurements=measurements, channels=channels, )
                 worker.signals.result.connect(self._process_import)
                 worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
                 self.threadpool.start(worker)
 
+    def _export_stack(self, mode, viewer=None):
+
+        def _event(viewer):
+
+            execute_export = True
+
+            if self.export_location.currentIndex() == 1:
+                desktop = os.path.expanduser("~/Desktop")
+                self.export_directory = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+
+                if self.export_directory == "":
+                    execute_export = False
+
+            if execute_export == True:
+                self.export_stacks = self.wrapper(napari_bacseg._utils.export_stacks)
+
+                worker = Worker(self.export_stacks, mode=mode)
+                worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
+                self.threadpool.start(worker)
+
+        return _event
+
+
     def _export(self, mode, viewer=None):
         def _event(viewer):
             # if self.unfolded == True:
             #     self.fold_images()
 
             execute_export = True
 
@@ -1274,15 +1309,15 @@
 
         if (slider_name == "cellpose_flowthresh" or slider_name == "cellpose_maskthresh"):
             self.label.setText(str(slider_value / 100))
         else:
             self.label.setText(str(slider_value))
 
     def _updateSegmentationCombo(self):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
         self.cellpose_segchannel.clear()
         self.cellpose_segchannel.addItems(layer_names)
 
         self.cellpose_trainchannel.clear()
         self.cellpose_trainchannel.addItems(layer_names)
 
@@ -1293,14 +1328,17 @@
         self.alignment_channel.addItems(layer_names)
 
         self.export_channel.clear()
         export_layers = layer_names
         export_layers.extend(["All Channels (Stack)", "First Three Channels (RGB)"])
         self.export_channel.addItems(export_layers)
 
+        self.export_stack_channel.clear()
+        self.export_stack_channel.addItems(layer_names)
+
         self.refine_channel.clear()
         refine_layers = ["Mask + " + layer for layer in layer_names]
         self.refine_channel.addItems(["Mask"] + refine_layers)
 
         self.export_colicoords_mode.clear()
         refine_layers = ["Mask + " + layer for layer in layer_names]
         self.export_colicoords_mode.addItems(["None (OpenCV Stats)", "Mask"] + refine_layers)
@@ -1342,15 +1380,15 @@
 
         except:
             self.viewer.scale_bar.visible = False
 
     def _autoContrast(self):
         try:
             if self.autocontrast.isChecked():
-                layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+                layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines", ]]
 
                 if len(layer_names) != 0:
                     active_layer = layer_names[-1]
 
                     image_dims = tuple(list(self.viewer.dims.current_step[:-2]) + [...])
 
                     image = (self.viewer.layers[str(active_layer)].data[image_dims].copy())
@@ -1376,14 +1414,16 @@
             active_layer = self.viewer.layers.selection.active
 
             image = self.viewer.layers[str(active_layer)].data[current_fov]
             metadata = self.viewer.layers[str(active_layer)].metadata[current_fov]
 
             viewer_text = ""
 
+            # print(metadata['image_name'])
+
             if (self.overlay_filename.isChecked() and "image_name" in metadata.keys()):
                 viewer_text = f"File Name: {metadata['image_name']}"
             if self.overlay_folder.isChecked() and "folder" in metadata.keys():
                 viewer_text = viewer_text + f"\nFolder: {metadata['folder']}"
             if (self.overlay_microscope.isChecked() and "microscope" in metadata.keys()):
                 viewer_text = (viewer_text + f"\nMicroscope: {metadata['microscope']}")
             if (self.overlay_datemodified.isChecked() and "date_modified" in metadata.keys()):
@@ -1421,43 +1461,56 @@
             else:
                 self.viewer.text_overlay.visible = False
 
         except:
             pass
 
     def _process_import(self, imported_data, rearrange=True):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
         if self.clear_previous.isChecked() == True:
             # removes all layers (except segmentation layer)
             for layer_name in layer_names:
                 self.viewer.layers.remove(self.viewer.layers[layer_name])
             # reset segmentation and class layers
             self.segLayer.data = np.zeros((1, 100, 100), dtype=np.uint16)
+            self.nucLayer.data = np.zeros((1, 100, 100), dtype=np.uint16)
             self.classLayer.data = np.zeros((1, 100, 100), dtype=np.uint16)
 
         imported_images = imported_data["imported_images"]
 
         self.viewer.dims.set_current_step(0, 0)
 
         for layer_name, layer_data in imported_images.items():
             images = layer_data["images"]
             masks = layer_data["masks"]
             classes = layer_data["classes"]
             metadata = layer_data["metadata"]
 
+            # for i in range(len(images)):
+            #     print(metadata[i]["image_name"])
+
+            if "nmasks" in layer_data.keys():
+                nmasks = layer_data["nmasks"]
+            else:
+                nmasks = []
+
             from napari_bacseg._utils import stack_images
 
             new_image_stack, new_metadata = stack_images(images, metadata)
             new_mask_stack, new_metadata = stack_images(masks, metadata)
+            new_nmask_stack, new_metadata = stack_images(nmasks, metadata)
             new_class_stack, new_metadata = stack_images(classes, metadata)
 
             if len(new_mask_stack) == 0:
                 new_mask_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
 
+            if len(new_nmask_stack) == 0:
+                new_nmask_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
+
             if len(new_class_stack) == 0:
                 new_class_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
 
             colormap = "gray"
 
             if layer_name == "405":
                 colormap = "green"
@@ -1468,79 +1521,87 @@
             if layer_name == "DAPI":
                 colormap = "green"
 
             if (self.clear_previous.isChecked() == False and layer_name in layer_names):
                 current_image_stack = self.viewer.layers[layer_name].data
                 current_metadata = self.viewer.layers[layer_name].metadata
                 current_mask_stack = self.segLayer.data
+                current_nmask_stack = self.nucLayer.data
                 current_class_stack = self.classLayer.data
 
                 if len(current_image_stack) == 0:
                     setattr(self, layer_name, self.viewer.add_image(new_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=new_metadata, ), )
 
                     image_layer = getattr(self, layer_name)
                     image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
                     image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
 
                     self.segLayer.data = new_mask_stack
+                    self.nucLayer.data = new_nmask_stack
                     self.classLayer.data = new_class_stack
                     self.segLayer.metadata = new_metadata
 
                 else:
                     from napari_bacseg._utils import append_image_stacks
 
                     (appended_image_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_image_stack, new_image_stack, )
 
                     (appended_mask_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_mask_stack, new_mask_stack, )
 
+                    (appended_nmask_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_nmask_stack, new_nmask_stack, )
+
                     (appended_class_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_class_stack, new_class_stack, )
 
                     self.viewer.layers.remove(self.viewer.layers[layer_name])
 
                     setattr(self, layer_name, self.viewer.add_image(appended_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=appended_metadata, ), )
 
                     image_layer = getattr(self, layer_name)
                     image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
                     image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
 
                     self.segLayer.data = appended_mask_stack
+                    self.nucLayer.data = appended_nmask_stack
                     self.classLayer.data = appended_class_stack
                     self.segLayer.metadata = appended_metadata
 
             else:
                 setattr(self, layer_name, self.viewer.add_image(new_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=new_metadata, ), )
 
                 image_layer = getattr(self, layer_name)
                 image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
                 image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
 
                 self.segLayer.data = new_mask_stack
+                self.nucLayer.data = new_nmask_stack
                 self.classLayer.data = new_class_stack
                 self.segLayer.metadata = new_metadata
 
         # sets labels such that only label contours are shown
         self.segLayer.contour = 1
         self.segLayer.opacity = 1
+        self.nucLayer.contour = 1
+        self.nucLayer.opacity = 1
 
         self._reorderLayers()
         self._updateFileName()
         self._updateSegmentationCombo()
         self._updateSegChannels()
         self.import_progressbar.reset()
         self.viewer.reset_view()
         self._autoClassify()
         align_image_channels(self)
         self._autoContrast()
         self._updateScaleBar()
 
     def _reorderLayers(self):
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name in ["Segmentations", "Classes", "center_lines"]]
+            layer_names = [layer.name for layer in self.viewer.layers if layer.name in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
 
-            for layer in ["center_lines", "Classes", "Segmentations"]:
+            for layer in ["center_lines", "Classes", "Nucleoid", "Segmentations", ]:
                 if layer in layer_names:
                     layer_index = self.viewer.layers.index(layer)
                     self.viewer.layers.move(layer_index, -1)
 
         except:
             pass
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.py` & `napari-bacseg-1.0.7/src/napari_bacseg/bacseg_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         self.formLayout_8.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.label_30)
         self.import_multiframe_mode = QtWidgets.QComboBox(self.import_tab)
         self.import_multiframe_mode.setObjectName("import_multiframe_mode")
         self.import_multiframe_mode.addItem("")
         self.import_multiframe_mode.addItem("")
         self.import_multiframe_mode.addItem("")
         self.import_multiframe_mode.addItem("")
+        self.import_multiframe_mode.addItem("")
         self.formLayout_8.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.import_multiframe_mode)
         self.label_22 = QtWidgets.QLabel(self.import_tab)
         self.label_22.setObjectName("label_22")
         self.formLayout_8.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.label_22)
         self.import_crop_mode = QtWidgets.QComboBox(self.import_tab)
         self.import_crop_mode.setObjectName("import_crop_mode")
         self.import_crop_mode.addItem("")
@@ -112,15 +113,15 @@
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.import_mode.addItem("")
         self.formLayout_8.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.import_mode)
         self.label_27 = QtWidgets.QLabel(self.import_tab)
         self.label_27.setObjectName("label_27")
-        self.formLayout_8.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_27)
+        self.formLayout_8.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_27)
         self.verticalLayout.addLayout(self.formLayout_8)
         spacerItem2 = QtWidgets.QSpacerItem(334, 5, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
         self.verticalLayout.addItem(spacerItem2)
         self.gridLayout_9 = QtWidgets.QGridLayout()
         self.gridLayout_9.setObjectName("gridLayout_9")
         self.import_clear_previous = QtWidgets.QCheckBox(self.import_tab)
         self.import_clear_previous.setChecked(True)
@@ -455,33 +456,41 @@
         self.tabWidget_3.setObjectName("tabWidget_3")
         self.tab_6 = QtWidgets.QWidget()
         self.tab_6.setObjectName("tab_6")
         self.verticalLayout_10 = QtWidgets.QVBoxLayout(self.tab_6)
         self.verticalLayout_10.setObjectName("verticalLayout_10")
         self.formLayout_12 = QtWidgets.QFormLayout()
         self.formLayout_12.setObjectName("formLayout_12")
+        self.label_97 = QtWidgets.QLabel(self.tab_6)
+        self.label_97.setObjectName("label_97")
+        self.formLayout_12.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_97)
         self.label_2 = QtWidgets.QLabel(self.tab_6)
         self.label_2.setObjectName("label_2")
-        self.formLayout_12.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_2)
+        self.formLayout_12.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_2)
         self.cellpose_segchannel = QtWidgets.QComboBox(self.tab_6)
         self.cellpose_segchannel.setObjectName("cellpose_segchannel")
-        self.formLayout_12.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_segchannel)
+        self.formLayout_12.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_segchannel)
         self.label = QtWidgets.QLabel(self.tab_6)
         self.label.setObjectName("label")
-        self.formLayout_12.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label)
+        self.formLayout_12.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label)
         self.cellpose_segmodel = QtWidgets.QComboBox(self.tab_6)
         self.cellpose_segmodel.setObjectName("cellpose_segmodel")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
-        self.formLayout_12.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_segmodel)
+        self.formLayout_12.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.cellpose_segmodel)
+        self.cellpose_seg_mode = QtWidgets.QComboBox(self.tab_6)
+        self.cellpose_seg_mode.setObjectName("cellpose_seg_mode")
+        self.cellpose_seg_mode.addItem("")
+        self.cellpose_seg_mode.addItem("")
+        self.formLayout_12.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_seg_mode)
         self.verticalLayout_10.addLayout(self.formLayout_12)
         spacerItem13 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
         self.verticalLayout_10.addItem(spacerItem13)
         self.cellpose_segment_active = QtWidgets.QPushButton(self.tab_6)
         self.cellpose_segment_active.setObjectName("cellpose_segment_active")
         self.verticalLayout_10.addWidget(self.cellpose_segment_active)
         self.cellpose_segment_all = QtWidgets.QPushButton(self.tab_6)
@@ -563,14 +572,22 @@
         self.cellpose_train_model.setObjectName("cellpose_train_model")
         self.verticalLayout_13.addWidget(self.cellpose_train_model)
         self.tabWidget_3.addTab(self.tab_11, "")
         self.tab_12 = QtWidgets.QWidget()
         self.tab_12.setObjectName("tab_12")
         self.verticalLayout_14 = QtWidgets.QVBoxLayout(self.tab_12)
         self.verticalLayout_14.setObjectName("verticalLayout_14")
+        self.label_94 = QtWidgets.QLabel(self.tab_12)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_94.setFont(font)
+        self.label_94.setObjectName("label_94")
+        self.verticalLayout_14.addWidget(self.label_94)
         self.gridLayout_2 = QtWidgets.QGridLayout()
         self.gridLayout_2.setObjectName("gridLayout_2")
         self.cellpose_flowthresh_label = QtWidgets.QLabel(self.tab_12)
         self.cellpose_flowthresh_label.setMinimumSize(QtCore.QSize(28, 22))
         self.cellpose_flowthresh_label.setObjectName("cellpose_flowthresh_label")
         self.gridLayout_2.addWidget(self.cellpose_flowthresh_label, 0, 2, 1, 1, QtCore.Qt.AlignLeft)
         self.cellpose_flowthresh = QtWidgets.QSlider(self.tab_12)
@@ -627,14 +644,38 @@
         self.gridLayout_2.addWidget(self.label_4, 3, 0, 1, 1)
         self.cellpose_diameter_label = QtWidgets.QLabel(self.tab_12)
         self.cellpose_diameter_label.setObjectName("cellpose_diameter_label")
         self.gridLayout_2.addWidget(self.cellpose_diameter_label, 3, 2, 1, 1)
         self.verticalLayout_14.addLayout(self.gridLayout_2)
         spacerItem16 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_14.addItem(spacerItem16)
+        self.label_95 = QtWidgets.QLabel(self.tab_12)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_95.setFont(font)
+        self.label_95.setObjectName("label_95")
+        self.verticalLayout_14.addWidget(self.label_95)
+        self.formLayout_21 = QtWidgets.QFormLayout()
+        self.formLayout_21.setObjectName("formLayout_21")
+        self.label_96 = QtWidgets.QLabel(self.tab_12)
+        self.label_96.setObjectName("label_96")
+        self.formLayout_21.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_96)
+        self.cellpose_min_seg_size = QtWidgets.QComboBox(self.tab_12)
+        self.cellpose_min_seg_size.setEditable(True)
+        self.cellpose_min_seg_size.setObjectName("cellpose_min_seg_size")
+        self.cellpose_min_seg_size.addItem("")
+        self.cellpose_min_seg_size.addItem("")
+        self.cellpose_min_seg_size.addItem("")
+        self.cellpose_min_seg_size.addItem("")
+        self.formLayout_21.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_min_seg_size)
+        self.verticalLayout_14.addLayout(self.formLayout_21)
+        spacerItem17 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_14.addItem(spacerItem17)
         self.cellpose_clear_previous = QtWidgets.QCheckBox(self.tab_12)
         self.cellpose_clear_previous.setChecked(True)
         self.cellpose_clear_previous.setObjectName("cellpose_clear_previous")
         self.verticalLayout_14.addWidget(self.cellpose_clear_previous)
         self.cellpose_usegpu = QtWidgets.QCheckBox(self.tab_12)
         self.cellpose_usegpu.setChecked(True)
         self.cellpose_usegpu.setObjectName("cellpose_usegpu")
@@ -646,16 +687,16 @@
         self.tabWidget_3.addTab(self.tab_12, "")
         self.verticalLayout_2.addWidget(self.tabWidget_3)
         self.line_6 = QtWidgets.QFrame(self.segement_tab)
         self.line_6.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_6.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_6.setObjectName("line_6")
         self.verticalLayout_2.addWidget(self.line_6)
-        spacerItem17 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_2.addItem(spacerItem17)
+        spacerItem18 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_2.addItem(spacerItem18)
         tab_widget.addTab(self.segement_tab, "")
         self.tab_3 = QtWidgets.QWidget()
         self.tab_3.setEnabled(True)
         self.tab_3.setObjectName("tab_3")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.tab_3)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.line_4 = QtWidgets.QFrame(self.tab_3)
@@ -679,20 +720,33 @@
         self.modify_classify = QtWidgets.QPushButton(self.tab_3)
         self.modify_classify.setObjectName("modify_classify")
         self.gridLayout_3.addWidget(self.modify_classify, 0, 3, 1, 1)
         self.modify_segment = QtWidgets.QPushButton(self.tab_3)
         self.modify_segment.setObjectName("modify_segment")
         self.gridLayout_3.addWidget(self.modify_segment, 0, 1, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_3)
+        spacerItem19 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem19)
+        self.formLayout_22 = QtWidgets.QFormLayout()
+        self.formLayout_22.setObjectName("formLayout_22")
+        self.label_98 = QtWidgets.QLabel(self.tab_3)
+        self.label_98.setObjectName("label_98")
+        self.formLayout_22.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_98)
+        self.modify_channel = QtWidgets.QComboBox(self.tab_3)
+        self.modify_channel.setObjectName("modify_channel")
+        self.modify_channel.addItem("")
+        self.modify_channel.addItem("")
+        self.formLayout_22.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.modify_channel)
+        self.verticalLayout_3.addLayout(self.formLayout_22)
         self.modify_auto_panzoom = QtWidgets.QCheckBox(self.tab_3)
         self.modify_auto_panzoom.setChecked(True)
         self.modify_auto_panzoom.setObjectName("modify_auto_panzoom")
         self.verticalLayout_3.addWidget(self.modify_auto_panzoom)
-        spacerItem18 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_3.addItem(spacerItem18)
+        spacerItem20 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem20)
         self.line_18 = QtWidgets.QFrame(self.tab_3)
         self.line_18.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_18.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_18.setObjectName("line_18")
         self.verticalLayout_3.addWidget(self.line_18)
         self.label_16 = QtWidgets.QLabel(self.tab_3)
         font = QtGui.QFont()
@@ -719,16 +773,16 @@
         self.modify_split = QtWidgets.QPushButton(self.tab_3)
         self.modify_split.setObjectName("modify_split")
         self.gridLayout_4.addWidget(self.modify_split, 1, 0, 1, 1)
         self.modify_extend = QtWidgets.QPushButton(self.tab_3)
         self.modify_extend.setObjectName("modify_extend")
         self.gridLayout_4.addWidget(self.modify_extend, 0, 1, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_4)
-        spacerItem19 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_3.addItem(spacerItem19)
+        spacerItem21 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem21)
         self.line_19 = QtWidgets.QFrame(self.tab_3)
         self.line_19.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_19.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_19.setObjectName("line_19")
         self.verticalLayout_3.addWidget(self.line_19)
         self.label_28 = QtWidgets.QLabel(self.tab_3)
         font = QtGui.QFont()
@@ -762,16 +816,16 @@
         self.classify_broken.setObjectName("classify_broken")
         self.gridLayout_5.addWidget(self.classify_broken, 1, 1, 1, 1)
         self.classify_single = QtWidgets.QPushButton(self.tab_3)
         self.classify_single.setStyleSheet("color: rgb(255, 255, 255);")
         self.classify_single.setObjectName("classify_single")
         self.gridLayout_5.addWidget(self.classify_single, 0, 0, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_5)
-        spacerItem20 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_3.addItem(spacerItem20)
+        spacerItem22 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem22)
         self.line_21 = QtWidgets.QFrame(self.tab_3)
         self.line_21.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_21.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_21.setObjectName("line_21")
         self.verticalLayout_3.addWidget(self.line_21)
         self.label_14 = QtWidgets.QLabel(self.tab_3)
         font = QtGui.QFont()
@@ -854,16 +908,16 @@
         self.set_debris_4 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_4.setObjectName("set_debris_4")
         self.gridLayout_22.addWidget(self.set_debris_4, 0, 4, 1, 1)
         self.set_debris_5 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_5.setObjectName("set_debris_5")
         self.gridLayout_22.addWidget(self.set_debris_5, 0, 5, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_22)
-        spacerItem21 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_3.addItem(spacerItem21)
+        spacerItem23 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_3.addItem(spacerItem23)
         tab_widget.addTab(self.tab_3, "")
         self.tab_2 = QtWidgets.QWidget()
         self.tab_2.setObjectName("tab_2")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.tab_2)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.label_29 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
@@ -878,16 +932,16 @@
         self.oufti_panzoom_mode = QtWidgets.QRadioButton(self.tab_2)
         self.oufti_panzoom_mode.setObjectName("oufti_panzoom_mode")
         self.gridLayout_10.addWidget(self.oufti_panzoom_mode, 0, 0, 1, 1)
         self.oufti_edit_mode = QtWidgets.QRadioButton(self.tab_2)
         self.oufti_edit_mode.setObjectName("oufti_edit_mode")
         self.gridLayout_10.addWidget(self.oufti_edit_mode, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_10)
-        spacerItem22 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_7.addItem(spacerItem22)
+        spacerItem24 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem24)
         self.label_20 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_20.setFont(font)
         self.label_20.setObjectName("label_20")
@@ -915,16 +969,16 @@
         self.gridLayout_17 = QtWidgets.QGridLayout()
         self.gridLayout_17.setObjectName("gridLayout_17")
         self.oufti_generate_all_midlines = QtWidgets.QPushButton(self.tab_2)
         self.oufti_generate_all_midlines.setObjectName("oufti_generate_all_midlines")
         self.gridLayout_17.addWidget(self.oufti_generate_all_midlines, 0, 0, 1, 1)
         self.gridLayout_16.addLayout(self.gridLayout_17, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_16)
-        spacerItem23 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_7.addItem(spacerItem23)
+        spacerItem25 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem25)
         self.label_63 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_63.setFont(font)
         self.label_63.setObjectName("label_63")
@@ -934,16 +988,16 @@
         self.oufti_centre_active_midlines = QtWidgets.QPushButton(self.tab_2)
         self.oufti_centre_active_midlines.setObjectName("oufti_centre_active_midlines")
         self.gridLayout_15.addWidget(self.oufti_centre_active_midlines, 0, 0, 1, 1)
         self.oufti_centre_all_midlines = QtWidgets.QPushButton(self.tab_2)
         self.oufti_centre_all_midlines.setObjectName("oufti_centre_all_midlines")
         self.gridLayout_15.addWidget(self.oufti_centre_all_midlines, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_15)
-        spacerItem24 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_7.addItem(spacerItem24)
+        spacerItem26 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem26)
         self.label_61 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_61.setFont(font)
         self.label_61.setObjectName("label_61")
@@ -979,16 +1033,16 @@
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.formLayout_7.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.oufti_mesh_dilation)
         self.verticalLayout_7.addLayout(self.formLayout_7)
-        spacerItem25 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_7.addItem(spacerItem25)
+        spacerItem27 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_7.addItem(spacerItem27)
         tab_widget.addTab(self.tab_2, "")
         self.upload_tab = QtWidgets.QWidget()
         self.upload_tab.setEnabled(True)
         self.upload_tab.setObjectName("upload_tab")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.upload_tab)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
         self.line_24 = QtWidgets.QFrame(self.upload_tab)
@@ -1021,16 +1075,16 @@
         self.display_database_path = QtWidgets.QLineEdit(self.upload_tab)
         self.display_database_path.setAlignment(QtCore.Qt.AlignCenter)
         self.display_database_path.setReadOnly(True)
         self.display_database_path.setClearButtonEnabled(False)
         self.display_database_path.setObjectName("display_database_path")
         self.formLayout_9.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.display_database_path)
         self.verticalLayout_4.addLayout(self.formLayout_9)
-        spacerItem26 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem26)
+        spacerItem28 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_4.addItem(spacerItem28)
         self.metadata_controls = QtWidgets.QTabWidget(self.upload_tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.metadata_controls.sizePolicy().hasHeightForWidth())
         self.metadata_controls.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
@@ -1366,16 +1420,16 @@
         self.label_stain_target.addItem("")
         self.label_stain_target.addItem("")
         self.formLayout_10.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.label_stain_target)
         self.verticalLayout_8.addLayout(self.formLayout_10)
         self.label_overwrite = QtWidgets.QPushButton(self.image_metadata)
         self.label_overwrite.setObjectName("label_overwrite")
         self.verticalLayout_8.addWidget(self.label_overwrite)
-        spacerItem27 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_8.addItem(spacerItem27)
+        spacerItem29 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_8.addItem(spacerItem29)
         self.metadata_controls.addTab(self.image_metadata, "")
         self.user_metadata = QtWidgets.QWidget()
         self.user_metadata.setObjectName("user_metadata")
         self.verticalLayout_19 = QtWidgets.QVBoxLayout(self.user_metadata)
         self.verticalLayout_19.setObjectName("verticalLayout_19")
         self.formLayout_2 = QtWidgets.QFormLayout()
         self.formLayout_2.setObjectName("formLayout_2")
@@ -1424,23 +1478,23 @@
         self.formLayout_2.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_92)
         self.upload_usermeta6 = QtWidgets.QComboBox(self.user_metadata)
         self.upload_usermeta6.setEnabled(True)
         self.upload_usermeta6.setEditable(True)
         self.upload_usermeta6.setObjectName("upload_usermeta6")
         self.formLayout_2.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta6)
         self.verticalLayout_19.addLayout(self.formLayout_2)
-        spacerItem28 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_19.addItem(spacerItem28)
+        spacerItem30 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_19.addItem(spacerItem30)
         self.metadata_controls.addTab(self.user_metadata, "")
         self.verticalLayout_4.addWidget(self.metadata_controls)
         self.update_metadata = QtWidgets.QPushButton(self.upload_tab)
         self.update_metadata.setObjectName("update_metadata")
         self.verticalLayout_4.addWidget(self.update_metadata)
-        spacerItem29 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem29)
+        spacerItem31 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_4.addItem(spacerItem31)
         self.label_87 = QtWidgets.QLabel(self.upload_tab)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_87.setFont(font)
         self.label_87.setObjectName("label_87")
@@ -1466,16 +1520,16 @@
         self.upload_label_combo.addItem("")
         self.upload_label_combo.setItemText(0, "")
         self.upload_label_combo.addItem("")
         self.upload_label_combo.addItem("")
         self.upload_label_combo.addItem("")
         self.formLayout_16.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.upload_label_combo)
         self.verticalLayout_4.addLayout(self.formLayout_16)
-        spacerItem30 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem30)
+        spacerItem32 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_4.addItem(spacerItem32)
         self.tabWidget_2 = QtWidgets.QTabWidget(self.upload_tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.tabWidget_2.sizePolicy().hasHeightForWidth())
         self.tabWidget_2.setSizePolicy(sizePolicy)
         self.tabWidget_2.setMaximumSize(QtCore.QSize(16777215, 500))
@@ -1605,16 +1659,16 @@
         self.overwrite_all_metadata.setObjectName("overwrite_all_metadata")
         self.gridLayout_25.addWidget(self.overwrite_all_metadata, 1, 0, 1, 1)
         self.overwrite_selected_metadata = QtWidgets.QCheckBox(self.tab_4)
         self.overwrite_selected_metadata.setEnabled(True)
         self.overwrite_selected_metadata.setObjectName("overwrite_selected_metadata")
         self.gridLayout_25.addWidget(self.overwrite_selected_metadata, 1, 1, 1, 1)
         self.verticalLayout_11.addLayout(self.gridLayout_25)
-        spacerItem31 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_11.addItem(spacerItem31)
+        spacerItem33 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_11.addItem(spacerItem33)
         self.database_upload_buttons_2 = QtWidgets.QGridLayout()
         self.database_upload_buttons_2.setObjectName("database_upload_buttons_2")
         self.upload_all = QtWidgets.QPushButton(self.tab_4)
         self.upload_all.setEnabled(True)
         self.upload_all.setObjectName("upload_all")
         self.database_upload_buttons_2.addWidget(self.upload_all, 0, 1, 1, 1)
         self.upload_active = QtWidgets.QPushButton(self.tab_4)
@@ -1631,16 +1685,16 @@
         self.gridLayout_18.addWidget(self.label_89, 0, 0, 1, 1)
         self.upload_progressbar = QtWidgets.QProgressBar(self.upload_tab)
         self.upload_progressbar.setEnabled(True)
         self.upload_progressbar.setProperty("value", 0)
         self.upload_progressbar.setObjectName("upload_progressbar")
         self.gridLayout_18.addWidget(self.upload_progressbar, 0, 1, 1, 1)
         self.verticalLayout_4.addLayout(self.gridLayout_18)
-        spacerItem32 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_4.addItem(spacerItem32)
+        spacerItem34 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_4.addItem(spacerItem34)
         tab_widget.addTab(self.upload_tab, "")
         self.export_tab = QtWidgets.QWidget()
         self.export_tab.setEnabled(True)
         self.export_tab.setObjectName("export_tab")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.export_tab)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.tabWidget_4 = QtWidgets.QTabWidget(self.export_tab)
@@ -1650,270 +1704,335 @@
         sizePolicy.setHeightForWidth(self.tabWidget_4.sizePolicy().hasHeightForWidth())
         self.tabWidget_4.setSizePolicy(sizePolicy)
         self.tabWidget_4.setObjectName("tabWidget_4")
         self.tab_8 = QtWidgets.QWidget()
         self.tab_8.setObjectName("tab_8")
         self.verticalLayout_15 = QtWidgets.QVBoxLayout(self.tab_8)
         self.verticalLayout_15.setObjectName("verticalLayout_15")
+        self.tabWidget = QtWidgets.QTabWidget(self.tab_8)
+        self.tabWidget.setObjectName("tabWidget")
+        self.tab_18 = QtWidgets.QWidget()
+        self.tab_18.setObjectName("tab_18")
+        self.verticalLayout_26 = QtWidgets.QVBoxLayout(self.tab_18)
+        self.verticalLayout_26.setObjectName("verticalLayout_26")
         self.formLayout_6 = QtWidgets.QFormLayout()
         self.formLayout_6.setObjectName("formLayout_6")
-        self.export_mode = QtWidgets.QComboBox(self.tab_8)
+        self.export_mode = QtWidgets.QComboBox(self.tab_18)
         self.export_mode.setObjectName("export_mode")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.export_mode.addItem("")
         self.formLayout_6.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.export_mode)
-        self.label_19 = QtWidgets.QLabel(self.tab_8)
+        self.label_19 = QtWidgets.QLabel(self.tab_18)
         self.label_19.setObjectName("label_19")
         self.formLayout_6.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_19)
-        self.export_location = QtWidgets.QComboBox(self.tab_8)
+        self.export_location = QtWidgets.QComboBox(self.tab_18)
         self.export_location.setObjectName("export_location")
         self.export_location.addItem("")
         self.export_location.addItem("")
         self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.export_location)
-        self.label_44 = QtWidgets.QLabel(self.tab_8)
+        self.label_44 = QtWidgets.QLabel(self.tab_18)
         self.label_44.setObjectName("label_44")
         self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_44)
-        self.export_channel = QtWidgets.QComboBox(self.tab_8)
+        self.export_channel = QtWidgets.QComboBox(self.tab_18)
         self.export_channel.setObjectName("export_channel")
         self.export_channel.addItem("")
         self.export_channel.addItem("")
         self.formLayout_6.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_channel)
-        self.label_45 = QtWidgets.QLabel(self.tab_8)
+        self.label_45 = QtWidgets.QLabel(self.tab_18)
         self.label_45.setObjectName("label_45")
         self.formLayout_6.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_45)
-        self.verticalLayout_15.addLayout(self.formLayout_6)
+        self.verticalLayout_26.addLayout(self.formLayout_6)
         self.formLayout_5 = QtWidgets.QFormLayout()
         self.formLayout_5.setObjectName("formLayout_5")
-        self.label_26 = QtWidgets.QLabel(self.tab_8)
+        self.label_26 = QtWidgets.QLabel(self.tab_18)
         self.label_26.setObjectName("label_26")
         self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_26)
-        self.export_modifier = QtWidgets.QLineEdit(self.tab_8)
+        self.export_modifier = QtWidgets.QLineEdit(self.tab_18)
         self.export_modifier.setObjectName("export_modifier")
         self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_modifier)
-        self.verticalLayout_15.addLayout(self.formLayout_5)
-        self.gridLayout_14 = QtWidgets.QGridLayout()
-        self.gridLayout_14.setObjectName("gridLayout_14")
-        self.export_overwrite_setting = QtWidgets.QCheckBox(self.tab_8)
-        self.export_overwrite_setting.setObjectName("export_overwrite_setting")
-        self.gridLayout_14.addWidget(self.export_overwrite_setting, 1, 1, 1, 1)
-        self.export_image_setting = QtWidgets.QCheckBox(self.tab_8)
+        self.verticalLayout_26.addLayout(self.formLayout_5)
+        self.gridLayout_32 = QtWidgets.QGridLayout()
+        self.gridLayout_32.setObjectName("gridLayout_32")
+        self.export_image_setting = QtWidgets.QCheckBox(self.tab_18)
         self.export_image_setting.setChecked(True)
         self.export_image_setting.setObjectName("export_image_setting")
-        self.gridLayout_14.addWidget(self.export_image_setting, 1, 0, 1, 1)
-        self.verticalLayout_15.addLayout(self.gridLayout_14)
-        spacerItem33 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_15.addItem(spacerItem33)
-        self.label_12 = QtWidgets.QLabel(self.tab_8)
-        font = QtGui.QFont()
-        font.setPointSize(10)
-        font.setBold(True)
-        font.setWeight(75)
-        self.label_12.setFont(font)
-        self.label_12.setObjectName("label_12")
-        self.verticalLayout_15.addWidget(self.label_12)
-        self.gridLayout_19 = QtWidgets.QGridLayout()
-        self.gridLayout_19.setObjectName("gridLayout_19")
-        self.export_autocontrast = QtWidgets.QCheckBox(self.tab_8)
-        self.export_autocontrast.setObjectName("export_autocontrast")
-        self.gridLayout_19.addWidget(self.export_autocontrast, 1, 0, 1, 1)
-        self.export_normalise = QtWidgets.QCheckBox(self.tab_8)
-        self.export_normalise.setObjectName("export_normalise")
-        self.gridLayout_19.addWidget(self.export_normalise, 1, 1, 1, 1)
-        self.export_scalebar = QtWidgets.QCheckBox(self.tab_8)
-        self.export_scalebar.setObjectName("export_scalebar")
-        self.gridLayout_19.addWidget(self.export_scalebar, 2, 0, 1, 1)
-        self.export_invert = QtWidgets.QCheckBox(self.tab_8)
-        self.export_invert.setObjectName("export_invert")
-        self.gridLayout_19.addWidget(self.export_invert, 1, 2, 1, 1)
-        self.export_mask_background = QtWidgets.QCheckBox(self.tab_8)
-        self.export_mask_background.setObjectName("export_mask_background")
-        self.gridLayout_19.addWidget(self.export_mask_background, 2, 1, 1, 1)
-        self.export_crop_zoom = QtWidgets.QCheckBox(self.tab_8)
-        self.export_crop_zoom.setObjectName("export_crop_zoom")
-        self.gridLayout_19.addWidget(self.export_crop_zoom, 2, 2, 1, 1)
-        self.verticalLayout_15.addLayout(self.gridLayout_19)
-        spacerItem34 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_15.addItem(spacerItem34)
-        self.export_active = QtWidgets.QPushButton(self.tab_8)
+        self.gridLayout_32.addWidget(self.export_image_setting, 0, 0, 1, 1)
+        self.export_overwrite_setting = QtWidgets.QCheckBox(self.tab_18)
+        self.export_overwrite_setting.setObjectName("export_overwrite_setting")
+        self.gridLayout_32.addWidget(self.export_overwrite_setting, 0, 1, 1, 1)
+        self.verticalLayout_26.addLayout(self.gridLayout_32)
+        spacerItem35 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_26.addItem(spacerItem35)
+        self.export_active = QtWidgets.QPushButton(self.tab_18)
         self.export_active.setObjectName("export_active")
-        self.verticalLayout_15.addWidget(self.export_active)
-        self.export_all = QtWidgets.QPushButton(self.tab_8)
+        self.verticalLayout_26.addWidget(self.export_active)
+        self.export_all = QtWidgets.QPushButton(self.tab_18)
         self.export_all.setObjectName("export_all")
-        self.verticalLayout_15.addWidget(self.export_all)
-        self.tabWidget_4.addTab(self.tab_8, "")
-        self.tab_9 = QtWidgets.QWidget()
-        self.tab_9.setObjectName("tab_9")
-        self.verticalLayout_17 = QtWidgets.QVBoxLayout(self.tab_9)
-        self.verticalLayout_17.setObjectName("verticalLayout_17")
-        self.label_46 = QtWidgets.QLabel(self.tab_9)
-        font = QtGui.QFont()
-        font.setPointSize(10)
-        font.setBold(True)
-        font.setWeight(75)
-        self.label_46.setFont(font)
-        self.label_46.setObjectName("label_46")
-        self.verticalLayout_17.addWidget(self.label_46)
-        self.gridLayout_11 = QtWidgets.QGridLayout()
-        self.gridLayout_11.setObjectName("gridLayout_11")
-        self.label_54 = QtWidgets.QLabel(self.tab_9)
-        self.label_54.setObjectName("label_54")
-        self.gridLayout_11.addWidget(self.label_54, 1, 0, 1, 1)
-        self.export_statistics_pixelsize = QtWidgets.QLineEdit(self.tab_9)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.export_statistics_pixelsize.sizePolicy().hasHeightForWidth())
-        self.export_statistics_pixelsize.setSizePolicy(sizePolicy)
-        self.export_statistics_pixelsize.setObjectName("export_statistics_pixelsize")
-        self.gridLayout_11.addWidget(self.export_statistics_pixelsize, 0, 1, 1, 1)
-        self.export_colicoords_mode = QtWidgets.QComboBox(self.tab_9)
-        self.export_colicoords_mode.setObjectName("export_colicoords_mode")
-        self.export_colicoords_mode.addItem("")
-        self.export_colicoords_mode.addItem("")
-        self.gridLayout_11.addWidget(self.export_colicoords_mode, 1, 1, 1, 1)
-        self.label_52 = QtWidgets.QLabel(self.tab_9)
-        self.label_52.setObjectName("label_52")
-        self.gridLayout_11.addWidget(self.label_52, 0, 0, 1, 1)
-        self.verticalLayout_17.addLayout(self.gridLayout_11)
-        spacerItem35 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_17.addItem(spacerItem35)
-        self.export_statistics_multithreaded = QtWidgets.QCheckBox(self.tab_9)
-        self.export_statistics_multithreaded.setChecked(True)
-        self.export_statistics_multithreaded.setObjectName("export_statistics_multithreaded")
-        self.verticalLayout_17.addWidget(self.export_statistics_multithreaded)
-        self.export_statistics_active = QtWidgets.QPushButton(self.tab_9)
-        self.export_statistics_active.setObjectName("export_statistics_active")
-        self.verticalLayout_17.addWidget(self.export_statistics_active)
-        self.export_statistics_all = QtWidgets.QPushButton(self.tab_9)
-        self.export_statistics_all.setObjectName("export_statistics_all")
-        self.verticalLayout_17.addWidget(self.export_statistics_all)
-        self.tabWidget_4.addTab(self.tab_9, "")
-        self.tab_13 = QtWidgets.QWidget()
-        self.tab_13.setObjectName("tab_13")
-        self.verticalLayout_16 = QtWidgets.QVBoxLayout(self.tab_13)
-        self.verticalLayout_16.setObjectName("verticalLayout_16")
-        self.label_43 = QtWidgets.QLabel(self.tab_13)
+        self.verticalLayout_26.addWidget(self.export_all)
+        self.tabWidget.addTab(self.tab_18, "")
+        self.tab_19 = QtWidgets.QWidget()
+        self.tab_19.setObjectName("tab_19")
+        self.verticalLayout_25 = QtWidgets.QVBoxLayout(self.tab_19)
+        self.verticalLayout_25.setObjectName("verticalLayout_25")
+        self.formLayout_23 = QtWidgets.QFormLayout()
+        self.formLayout_23.setObjectName("formLayout_23")
+        self.label_101 = QtWidgets.QLabel(self.tab_19)
+        self.label_101.setObjectName("label_101")
+        self.formLayout_23.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_101)
+        self.export_stack_channel = QtWidgets.QComboBox(self.tab_19)
+        self.export_stack_channel.setObjectName("export_stack_channel")
+        self.formLayout_23.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_stack_channel)
+        self.label_99 = QtWidgets.QLabel(self.tab_19)
+        self.label_99.setObjectName("label_99")
+        self.formLayout_23.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_99)
+        self.export_stack_mode = QtWidgets.QComboBox(self.tab_19)
+        self.export_stack_mode.setObjectName("export_stack_mode")
+        self.export_stack_mode.addItem("")
+        self.export_stack_mode.addItem("")
+        self.formLayout_23.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.export_stack_mode)
+        self.label_100 = QtWidgets.QLabel(self.tab_19)
+        self.label_100.setObjectName("label_100")
+        self.formLayout_23.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_100)
+        self.export_stack_location = QtWidgets.QComboBox(self.tab_19)
+        self.export_stack_location.setObjectName("export_stack_location")
+        self.export_stack_location.addItem("")
+        self.export_stack_location.addItem("")
+        self.formLayout_23.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.export_stack_location)
+        self.verticalLayout_25.addLayout(self.formLayout_23)
+        self.formLayout_25 = QtWidgets.QFormLayout()
+        self.formLayout_25.setObjectName("formLayout_25")
+        self.label_103 = QtWidgets.QLabel(self.tab_19)
+        self.label_103.setObjectName("label_103")
+        self.formLayout_25.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_103)
+        self.export_stack_modifier = QtWidgets.QLineEdit(self.tab_19)
+        self.export_stack_modifier.setObjectName("export_stack_modifier")
+        self.formLayout_25.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_stack_modifier)
+        self.verticalLayout_25.addLayout(self.formLayout_25)
+        self.gridLayout_33 = QtWidgets.QGridLayout()
+        self.gridLayout_33.setObjectName("gridLayout_33")
+        self.export_stack_image_setting = QtWidgets.QCheckBox(self.tab_19)
+        self.export_stack_image_setting.setChecked(True)
+        self.export_stack_image_setting.setObjectName("export_stack_image_setting")
+        self.gridLayout_33.addWidget(self.export_stack_image_setting, 0, 0, 1, 1)
+        self.export_stack_overwrite_setting = QtWidgets.QCheckBox(self.tab_19)
+        self.export_stack_overwrite_setting.setObjectName("export_stack_overwrite_setting")
+        self.gridLayout_33.addWidget(self.export_stack_overwrite_setting, 0, 1, 1, 1)
+        self.verticalLayout_25.addLayout(self.gridLayout_33)
+        spacerItem36 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_25.addItem(spacerItem36)
+        self.export_stack_active = QtWidgets.QPushButton(self.tab_19)
+        self.export_stack_active.setObjectName("export_stack_active")
+        self.verticalLayout_25.addWidget(self.export_stack_active)
+        self.export_stack_all = QtWidgets.QPushButton(self.tab_19)
+        self.export_stack_all.setObjectName("export_stack_all")
+        self.verticalLayout_25.addWidget(self.export_stack_all)
+        self.tabWidget.addTab(self.tab_19, "")
+        self.tab_20 = QtWidgets.QWidget()
+        self.tab_20.setObjectName("tab_20")
+        self.verticalLayout_27 = QtWidgets.QVBoxLayout(self.tab_20)
+        self.verticalLayout_27.setObjectName("verticalLayout_27")
+        self.label_43 = QtWidgets.QLabel(self.tab_20)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_43.setFont(font)
         self.label_43.setObjectName("label_43")
-        self.verticalLayout_16.addWidget(self.label_43)
+        self.verticalLayout_27.addWidget(self.label_43)
         self.gridLayout = QtWidgets.QGridLayout()
         self.gridLayout.setObjectName("gridLayout")
-        self.export_single = QtWidgets.QCheckBox(self.tab_13)
+        self.export_single = QtWidgets.QCheckBox(self.tab_20)
         self.export_single.setChecked(True)
         self.export_single.setObjectName("export_single")
         self.gridLayout.addWidget(self.export_single, 0, 0, 1, 1)
-        self.export_vertical = QtWidgets.QCheckBox(self.tab_13)
+        self.export_vertical = QtWidgets.QCheckBox(self.tab_20)
         self.export_vertical.setChecked(True)
         self.export_vertical.setObjectName("export_vertical")
         self.gridLayout.addWidget(self.export_vertical, 1, 0, 1, 1)
-        self.export_divided = QtWidgets.QCheckBox(self.tab_13)
+        self.export_divided = QtWidgets.QCheckBox(self.tab_20)
         self.export_divided.setChecked(True)
         self.export_divided.setObjectName("export_divided")
         self.gridLayout.addWidget(self.export_divided, 0, 2, 1, 1)
-        self.export_dividing = QtWidgets.QCheckBox(self.tab_13)
+        self.export_dividing = QtWidgets.QCheckBox(self.tab_20)
         self.export_dividing.setChecked(True)
         self.export_dividing.setObjectName("export_dividing")
         self.gridLayout.addWidget(self.export_dividing, 0, 1, 1, 1)
-        self.export_edge = QtWidgets.QCheckBox(self.tab_13)
+        self.export_edge = QtWidgets.QCheckBox(self.tab_20)
         self.export_edge.setChecked(True)
         self.export_edge.setObjectName("export_edge")
         self.gridLayout.addWidget(self.export_edge, 1, 2, 1, 1)
-        self.export_broken = QtWidgets.QCheckBox(self.tab_13)
+        self.export_broken = QtWidgets.QCheckBox(self.tab_20)
         self.export_broken.setChecked(True)
         self.export_broken.setObjectName("export_broken")
         self.gridLayout.addWidget(self.export_broken, 1, 1, 1, 1)
-        self.verticalLayout_16.addLayout(self.gridLayout)
-        spacerItem36 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_16.addItem(spacerItem36)
-        self.label_49 = QtWidgets.QLabel(self.tab_13)
+        self.verticalLayout_27.addLayout(self.gridLayout)
+        spacerItem37 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_27.addItem(spacerItem37)
+        self.label_49 = QtWidgets.QLabel(self.tab_20)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_49.setFont(font)
         self.label_49.setObjectName("label_49")
-        self.verticalLayout_16.addWidget(self.label_49)
+        self.verticalLayout_27.addWidget(self.label_49)
         self.gridLayout_27 = QtWidgets.QGridLayout()
         self.gridLayout_27.setObjectName("gridLayout_27")
-        self.export_scalebar_resolution_units = QtWidgets.QComboBox(self.tab_13)
+        self.export_scalebar_resolution_units = QtWidgets.QComboBox(self.tab_20)
         self.export_scalebar_resolution_units.setMaximumSize(QtCore.QSize(200, 100))
         self.export_scalebar_resolution_units.setObjectName("export_scalebar_resolution_units")
         self.export_scalebar_resolution_units.addItem("")
         self.export_scalebar_resolution_units.addItem("")
         self.gridLayout_27.addWidget(self.export_scalebar_resolution_units, 0, 2, 1, 1)
-        self.label_50 = QtWidgets.QLabel(self.tab_13)
+        self.label_50 = QtWidgets.QLabel(self.tab_20)
         self.label_50.setObjectName("label_50")
         self.gridLayout_27.addWidget(self.label_50, 0, 0, 1, 1)
-        self.export_scalebar_resolution = QtWidgets.QLineEdit(self.tab_13)
+        self.export_scalebar_resolution = QtWidgets.QLineEdit(self.tab_20)
         self.export_scalebar_resolution.setMaximumSize(QtCore.QSize(200, 16777215))
         self.export_scalebar_resolution.setObjectName("export_scalebar_resolution")
         self.gridLayout_27.addWidget(self.export_scalebar_resolution, 0, 1, 1, 1)
-        self.label_55 = QtWidgets.QLabel(self.tab_13)
+        self.label_55 = QtWidgets.QLabel(self.tab_20)
         self.label_55.setObjectName("label_55")
         self.gridLayout_27.addWidget(self.label_55, 1, 0, 1, 1)
-        self.export_scalebar_size = QtWidgets.QLineEdit(self.tab_13)
+        self.export_scalebar_size = QtWidgets.QLineEdit(self.tab_20)
         self.export_scalebar_size.setMaximumSize(QtCore.QSize(200, 16777215))
         self.export_scalebar_size.setObjectName("export_scalebar_size")
         self.gridLayout_27.addWidget(self.export_scalebar_size, 1, 1, 1, 1)
-        self.export_scalebar_size_units = QtWidgets.QComboBox(self.tab_13)
+        self.export_scalebar_size_units = QtWidgets.QComboBox(self.tab_20)
         self.export_scalebar_size_units.setMaximumSize(QtCore.QSize(200, 100))
         self.export_scalebar_size_units.setObjectName("export_scalebar_size_units")
         self.export_scalebar_size_units.addItem("")
         self.export_scalebar_size_units.addItem("")
         self.gridLayout_27.addWidget(self.export_scalebar_size_units, 1, 2, 1, 1)
-        self.verticalLayout_16.addLayout(self.gridLayout_27)
+        self.verticalLayout_27.addLayout(self.gridLayout_27)
         self.formLayout_19 = QtWidgets.QFormLayout()
         self.formLayout_19.setObjectName("formLayout_19")
-        self.label_71 = QtWidgets.QLabel(self.tab_13)
+        self.label_71 = QtWidgets.QLabel(self.tab_20)
         self.label_71.setObjectName("label_71")
         self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_71)
-        self.export_scalebar_colour = QtWidgets.QComboBox(self.tab_13)
+        self.export_scalebar_colour = QtWidgets.QComboBox(self.tab_20)
         self.export_scalebar_colour.setObjectName("export_scalebar_colour")
         self.export_scalebar_colour.addItem("")
         self.export_scalebar_colour.addItem("")
         self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_scalebar_colour)
-        self.label_72 = QtWidgets.QLabel(self.tab_13)
+        self.label_72 = QtWidgets.QLabel(self.tab_20)
         self.label_72.setObjectName("label_72")
         self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_72)
-        self.export_scalebar_thickness = QtWidgets.QComboBox(self.tab_13)
+        self.export_scalebar_thickness = QtWidgets.QComboBox(self.tab_20)
         self.export_scalebar_thickness.setObjectName("export_scalebar_thickness")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.export_scalebar_thickness)
-        self.verticalLayout_16.addLayout(self.formLayout_19)
-        spacerItem37 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_16.addItem(spacerItem37)
-        self.tabWidget_4.addTab(self.tab_13, "")
+        self.verticalLayout_27.addLayout(self.formLayout_19)
+        spacerItem38 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_27.addItem(spacerItem38)
+        self.label_12 = QtWidgets.QLabel(self.tab_20)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_12.setFont(font)
+        self.label_12.setObjectName("label_12")
+        self.verticalLayout_27.addWidget(self.label_12)
+        self.gridLayout_19 = QtWidgets.QGridLayout()
+        self.gridLayout_19.setObjectName("gridLayout_19")
+        self.export_autocontrast = QtWidgets.QCheckBox(self.tab_20)
+        self.export_autocontrast.setObjectName("export_autocontrast")
+        self.gridLayout_19.addWidget(self.export_autocontrast, 1, 0, 1, 1)
+        self.export_normalise = QtWidgets.QCheckBox(self.tab_20)
+        self.export_normalise.setObjectName("export_normalise")
+        self.gridLayout_19.addWidget(self.export_normalise, 1, 1, 1, 1)
+        self.export_scalebar = QtWidgets.QCheckBox(self.tab_20)
+        self.export_scalebar.setObjectName("export_scalebar")
+        self.gridLayout_19.addWidget(self.export_scalebar, 2, 0, 1, 1)
+        self.export_invert = QtWidgets.QCheckBox(self.tab_20)
+        self.export_invert.setObjectName("export_invert")
+        self.gridLayout_19.addWidget(self.export_invert, 1, 2, 1, 1)
+        self.export_mask_background = QtWidgets.QCheckBox(self.tab_20)
+        self.export_mask_background.setObjectName("export_mask_background")
+        self.gridLayout_19.addWidget(self.export_mask_background, 2, 1, 1, 1)
+        self.export_crop_zoom = QtWidgets.QCheckBox(self.tab_20)
+        self.export_crop_zoom.setObjectName("export_crop_zoom")
+        self.gridLayout_19.addWidget(self.export_crop_zoom, 2, 2, 1, 1)
+        self.verticalLayout_27.addLayout(self.gridLayout_19)
+        self.tabWidget.addTab(self.tab_20, "")
+        self.verticalLayout_15.addWidget(self.tabWidget)
+        spacerItem39 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_15.addItem(spacerItem39)
+        self.tabWidget_4.addTab(self.tab_8, "")
+        self.tab_9 = QtWidgets.QWidget()
+        self.tab_9.setObjectName("tab_9")
+        self.verticalLayout_17 = QtWidgets.QVBoxLayout(self.tab_9)
+        self.verticalLayout_17.setObjectName("verticalLayout_17")
+        self.label_46 = QtWidgets.QLabel(self.tab_9)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_46.setFont(font)
+        self.label_46.setObjectName("label_46")
+        self.verticalLayout_17.addWidget(self.label_46)
+        self.gridLayout_11 = QtWidgets.QGridLayout()
+        self.gridLayout_11.setObjectName("gridLayout_11")
+        self.label_54 = QtWidgets.QLabel(self.tab_9)
+        self.label_54.setObjectName("label_54")
+        self.gridLayout_11.addWidget(self.label_54, 1, 0, 1, 1)
+        self.export_statistics_pixelsize = QtWidgets.QLineEdit(self.tab_9)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.export_statistics_pixelsize.sizePolicy().hasHeightForWidth())
+        self.export_statistics_pixelsize.setSizePolicy(sizePolicy)
+        self.export_statistics_pixelsize.setObjectName("export_statistics_pixelsize")
+        self.gridLayout_11.addWidget(self.export_statistics_pixelsize, 0, 1, 1, 1)
+        self.export_colicoords_mode = QtWidgets.QComboBox(self.tab_9)
+        self.export_colicoords_mode.setObjectName("export_colicoords_mode")
+        self.export_colicoords_mode.addItem("")
+        self.export_colicoords_mode.addItem("")
+        self.gridLayout_11.addWidget(self.export_colicoords_mode, 1, 1, 1, 1)
+        self.label_52 = QtWidgets.QLabel(self.tab_9)
+        self.label_52.setObjectName("label_52")
+        self.gridLayout_11.addWidget(self.label_52, 0, 0, 1, 1)
+        self.verticalLayout_17.addLayout(self.gridLayout_11)
+        spacerItem40 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_17.addItem(spacerItem40)
+        self.export_statistics_multithreaded = QtWidgets.QCheckBox(self.tab_9)
+        self.export_statistics_multithreaded.setChecked(True)
+        self.export_statistics_multithreaded.setObjectName("export_statistics_multithreaded")
+        self.verticalLayout_17.addWidget(self.export_statistics_multithreaded)
+        self.export_statistics_active = QtWidgets.QPushButton(self.tab_9)
+        self.export_statistics_active.setObjectName("export_statistics_active")
+        self.verticalLayout_17.addWidget(self.export_statistics_active)
+        self.export_statistics_all = QtWidgets.QPushButton(self.tab_9)
+        self.export_statistics_all.setObjectName("export_statistics_all")
+        self.verticalLayout_17.addWidget(self.export_statistics_all)
+        self.tabWidget_4.addTab(self.tab_9, "")
         self.verticalLayout_6.addWidget(self.tabWidget_4)
         self.formLayout_11 = QtWidgets.QFormLayout()
         self.formLayout_11.setObjectName("formLayout_11")
         self.label_33 = QtWidgets.QLabel(self.export_tab)
         self.label_33.setObjectName("label_33")
         self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_33)
         self.export_progressbar = QtWidgets.QProgressBar(self.export_tab)
         self.export_progressbar.setProperty("value", 0)
         self.export_progressbar.setObjectName("export_progressbar")
         self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_progressbar)
         self.verticalLayout_6.addLayout(self.formLayout_11)
-        spacerItem38 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_6.addItem(spacerItem38)
+        spacerItem41 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_6.addItem(spacerItem41)
         tab_widget.addTab(self.export_tab, "")
         self.tab_14 = QtWidgets.QWidget()
         self.tab_14.setObjectName("tab_14")
         self.verticalLayout_18 = QtWidgets.QVBoxLayout(self.tab_14)
         self.verticalLayout_18.setObjectName("verticalLayout_18")
         self.line_20 = QtWidgets.QFrame(self.tab_14)
         self.line_20.setFrameShape(QtWidgets.QFrame.HLine)
@@ -1931,16 +2050,16 @@
         self.verticalLayout_18.addWidget(self.modify_deleteotherimages)
         self.modify_deleteactivemasks = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteactivemasks.setObjectName("modify_deleteactivemasks")
         self.verticalLayout_18.addWidget(self.modify_deleteactivemasks)
         self.modify_deleteallmasks = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteallmasks.setObjectName("modify_deleteallmasks")
         self.verticalLayout_18.addWidget(self.modify_deleteallmasks)
-        spacerItem39 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_18.addItem(spacerItem39)
+        spacerItem42 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_18.addItem(spacerItem42)
         self.line_22 = QtWidgets.QFrame(self.tab_14)
         self.line_22.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_22.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_22.setObjectName("line_22")
         self.verticalLayout_18.addWidget(self.line_22)
         self.label_31 = QtWidgets.QLabel(self.tab_14)
         font = QtGui.QFont()
@@ -1970,16 +2089,16 @@
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_17)
         self.modify_progressbar = QtWidgets.QProgressBar(self.tab_14)
         self.modify_progressbar.setProperty("value", 0)
         self.modify_progressbar.setTextVisible(True)
         self.modify_progressbar.setObjectName("modify_progressbar")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.modify_progressbar)
         self.verticalLayout_18.addLayout(self.formLayout)
-        spacerItem40 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_18.addItem(spacerItem40)
+        spacerItem43 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_18.addItem(spacerItem43)
         self.line_23 = QtWidgets.QFrame(self.tab_14)
         self.line_23.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_23.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_23.setObjectName("line_23")
         self.verticalLayout_18.addWidget(self.line_23)
         self.label_56 = QtWidgets.QLabel(self.tab_14)
         font = QtGui.QFont()
@@ -2005,16 +2124,16 @@
         self.find_criterion = QtWidgets.QComboBox(self.tab_14)
         self.find_criterion.setObjectName("find_criterion")
         self.find_criterion.addItem("")
         self.find_criterion.addItem("")
         self.find_criterion.addItem("")
         self.gridLayout_7.addWidget(self.find_criterion, 0, 0, 1, 1)
         self.verticalLayout_18.addLayout(self.gridLayout_7)
-        spacerItem41 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_18.addItem(spacerItem41)
+        spacerItem44 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_18.addItem(spacerItem44)
         self.label_70 = QtWidgets.QLabel(self.tab_14)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_70.setFont(font)
         self.label_70.setObjectName("label_70")
@@ -2033,37 +2152,40 @@
         self.align_active_image = QtWidgets.QPushButton(self.tab_14)
         self.align_active_image.setObjectName("align_active_image")
         self.gridLayout_26.addWidget(self.align_active_image, 0, 0, 1, 1)
         self.align_all_images = QtWidgets.QPushButton(self.tab_14)
         self.align_all_images.setObjectName("align_all_images")
         self.gridLayout_26.addWidget(self.align_all_images, 0, 1, 1, 1)
         self.verticalLayout_18.addLayout(self.gridLayout_26)
-        spacerItem42 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_18.addItem(spacerItem42)
+        spacerItem45 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_18.addItem(spacerItem45)
         tab_widget.addTab(self.tab_14, "")
 
         self.retranslateUi(tab_widget)
         tab_widget.setCurrentIndex(0)
         self.import_limit.setCurrentIndex(6)
         self.import_precision.setCurrentIndex(1)
         self.zoom_.setCurrentIndex(0)
         self.unfold_tile_size.setCurrentIndex(3)
         self.unfold_tile_overlap.setCurrentIndex(3)
         self.tabWidget_3.setCurrentIndex(0)
         self.cellpose_nepochs.setCurrentIndex(3)
         self.cellpose_batchsize.setCurrentIndex(1)
+        self.cellpose_min_seg_size.setCurrentIndex(3)
         self.oufti_midline_vertexes.setCurrentIndex(0)
         self.oufti_mesh_length.setCurrentIndex(4)
         self.oufti_mesh_dilation.setCurrentIndex(6)
         self.metadata_controls.setCurrentIndex(0)
         self.tabWidget_2.setCurrentIndex(0)
         self.download_sort_order_2.setCurrentIndex(0)
         self.download_sort_order_1.setCurrentIndex(0)
         self.tabWidget_4.setCurrentIndex(0)
+        self.tabWidget.setCurrentIndex(0)
         self.export_location.setCurrentIndex(1)
+        self.export_stack_location.setCurrentIndex(1)
         self.export_scalebar_size_units.setCurrentIndex(1)
         self.export_scalebar_thickness.setCurrentIndex(3)
         QtCore.QMetaObject.connectSlotsByName(tab_widget)
 
     def retranslateUi(self, tab_widget):
         _translate = QtCore.QCoreApplication.translate
         tab_widget.setWindowTitle(_translate("tab_widget", "TabWidget"))
@@ -2076,18 +2198,19 @@
         self.import_limit.setItemText(1, _translate("tab_widget", "5"))
         self.import_limit.setItemText(2, _translate("tab_widget", "10"))
         self.import_limit.setItemText(3, _translate("tab_widget", "20"))
         self.import_limit.setItemText(4, _translate("tab_widget", "50"))
         self.import_limit.setItemText(5, _translate("tab_widget", "100"))
         self.import_limit.setItemText(6, _translate("tab_widget", "None"))
         self.label_30.setText(_translate("tab_widget", "Multi-Frame Mode"))
-        self.import_multiframe_mode.setItemText(0, _translate("tab_widget", "Keep First Frame"))
-        self.import_multiframe_mode.setItemText(1, _translate("tab_widget", "Keep Brightest Frame"))
-        self.import_multiframe_mode.setItemText(2, _translate("tab_widget", "Average Frames"))
-        self.import_multiframe_mode.setItemText(3, _translate("tab_widget", "Sum Frames"))
+        self.import_multiframe_mode.setItemText(0, _translate("tab_widget", "Keep Brightest Frame"))
+        self.import_multiframe_mode.setItemText(1, _translate("tab_widget", "Average Frames"))
+        self.import_multiframe_mode.setItemText(2, _translate("tab_widget", "Sum Frames"))
+        self.import_multiframe_mode.setItemText(3, _translate("tab_widget", "Keep First Frame"))
+        self.import_multiframe_mode.setItemText(4, _translate("tab_widget", "Keep All Frames (BETA)"))
         self.label_22.setText(_translate("tab_widget", "Image Crop Mode"))
         self.import_crop_mode.setItemText(0, _translate("tab_widget", "None"))
         self.import_crop_mode.setItemText(1, _translate("tab_widget", "Crop Left Half"))
         self.import_crop_mode.setItemText(2, _translate("tab_widget", "Crop Right Half"))
         self.import_crop_mode.setItemText(3, _translate("tab_widget", "Crop Brightest Half"))
         self.label_21.setText(_translate("tab_widget", "Import Precision"))
         self.import_precision.setItemText(0, _translate("tab_widget", "int8"))
@@ -2170,23 +2293,26 @@
         self.zoom_magnification.setItemText(8, _translate("tab_widget", "300"))
         self.zoom_magnification.setItemText(9, _translate("tab_widget", "400"))
         self.zoom_magnification.setItemText(10, _translate("tab_widget", "500"))
         self.zoom_apply.setText(_translate("tab_widget", "Apply Zoom"))
         self.zoom_.setTabText(self.zoom_.indexOf(self.tab_5), _translate("tab_widget", "Zoom"))
         tab_widget.setTabText(tab_widget.indexOf(self.tab), _translate("tab_widget", "View"))
         self.cellpose_select_custom_model.setText(_translate("tab_widget", "Select Custom Cellpose Model"))
+        self.label_97.setText(_translate("tab_widget", "Segmentation Mode"))
         self.label_2.setText(_translate("tab_widget", "Segmentation Channel"))
         self.label.setText(_translate("tab_widget", "Cellpose Model"))
         self.cellpose_segmodel.setItemText(0, _translate("tab_widget", "cyto"))
         self.cellpose_segmodel.setItemText(1, _translate("tab_widget", "nuclei"))
         self.cellpose_segmodel.setItemText(2, _translate("tab_widget", "tissuenet"))
         self.cellpose_segmodel.setItemText(3, _translate("tab_widget", "livecell"))
         self.cellpose_segmodel.setItemText(4, _translate("tab_widget", "cyto2"))
         self.cellpose_segmodel.setItemText(5, _translate("tab_widget", "general"))
         self.cellpose_segmodel.setItemText(6, _translate("tab_widget", "custom"))
+        self.cellpose_seg_mode.setItemText(0, _translate("tab_widget", "Cell Wall"))
+        self.cellpose_seg_mode.setItemText(1, _translate("tab_widget", "Nucleiod"))
         self.cellpose_segment_active.setText(_translate("tab_widget", "Segment Active Image"))
         self.cellpose_segment_all.setText(_translate("tab_widget", "Segment All Images"))
         self.label_35.setText(_translate("tab_widget", "Progress"))
         self.tabWidget_3.setTabText(self.tabWidget_3.indexOf(self.tab_6), _translate("tab_widget", "Segment"))
         self.label_8.setText(_translate("tab_widget", "Train Channel"))
         self.label_9.setText(_translate("tab_widget", "N Epochs"))
         self.cellpose_nepochs.setItemText(0, _translate("tab_widget", "1"))
@@ -2210,31 +2336,42 @@
         self.cellpose_trainmodel.setItemText(3, _translate("tab_widget", "livecell"))
         self.cellpose_trainmodel.setItemText(4, _translate("tab_widget", "cyto2"))
         self.cellpose_trainmodel.setItemText(5, _translate("tab_widget", "general"))
         self.cellpose_trainmodel.setItemText(6, _translate("tab_widget", "custom"))
         self.cellpose_save_dir.setText(_translate("tab_widget", "Select Save Directory"))
         self.cellpose_train_model.setText(_translate("tab_widget", "Train Cellpose Model (All Images)"))
         self.tabWidget_3.setTabText(self.tabWidget_3.indexOf(self.tab_11), _translate("tab_widget", "Train"))
+        self.label_94.setText(_translate("tab_widget", "Cellpose Controls"))
         self.cellpose_flowthresh_label.setText(_translate("tab_widget", "0.9"))
         self.label_3.setText(_translate("tab_widget", "Flow Threshold"))
         self.cellpose_maskthresh_label.setText(_translate("tab_widget", "0.0"))
         self.cellpose_minsize_label.setText(_translate("tab_widget", "15"))
         self.label_5.setText(_translate("tab_widget", "Mask Threshold"))
         self.label_6.setText(_translate("tab_widget", "Min Size"))
         self.label_4.setText(_translate("tab_widget", "Diameter"))
         self.cellpose_diameter_label.setText(_translate("tab_widget", "15"))
+        self.label_95.setText(_translate("tab_widget", "Cellpose Post Processing"))
+        self.label_96.setText(_translate("tab_widget", "Min Segmentation Size (Pixels)"))
+        self.cellpose_min_seg_size.setCurrentText(_translate("tab_widget", "50"))
+        self.cellpose_min_seg_size.setItemText(0, _translate("tab_widget", "1"))
+        self.cellpose_min_seg_size.setItemText(1, _translate("tab_widget", "5"))
+        self.cellpose_min_seg_size.setItemText(2, _translate("tab_widget", "10"))
+        self.cellpose_min_seg_size.setItemText(3, _translate("tab_widget", "50"))
         self.cellpose_clear_previous.setText(_translate("tab_widget", "Clear Previous Segmentations"))
         self.cellpose_usegpu.setText(_translate("tab_widget", "Use GPU (if Availiable)"))
         self.cellpose_resetimage.setText(_translate("tab_widget", "Reset Image View After Segmentation"))
         self.tabWidget_3.setTabText(self.tabWidget_3.indexOf(self.tab_12), _translate("tab_widget", "Settings"))
         tab_widget.setTabText(tab_widget.indexOf(self.segement_tab), _translate("tab_widget", "Segment"))
         self.label_7.setText(_translate("tab_widget", "Interface Modes:"))
         self.modify_panzoom.setText(_translate("tab_widget", "Pan/Zoom [F1]"))
         self.modify_classify.setText(_translate("tab_widget", "Classify [F3]"))
         self.modify_segment.setText(_translate("tab_widget", "Segment [F2]"))
+        self.label_98.setText(_translate("tab_widget", "Curate Channel"))
+        self.modify_channel.setItemText(0, _translate("tab_widget", "Segmentations (Cell Wall)"))
+        self.modify_channel.setItemText(1, _translate("tab_widget", "Nucleoid"))
         self.modify_auto_panzoom.setText(_translate("tab_widget", "Auto select Pan/Zoom after interface event"))
         self.label_16.setText(_translate("tab_widget", "Segmentation Modes:"))
         self.modify_refine.setText(_translate("tab_widget", "Refine [R]"))
         self.modify_join.setText(_translate("tab_widget", "Join [J]"))
         self.modify_add.setText(_translate("tab_widget", "Add [A]"))
         self.modify_delete.setText(_translate("tab_widget", "Delete [D]"))
         self.modify_split.setText(_translate("tab_widget", "Split [S]"))
@@ -2440,36 +2577,33 @@
         self.export_location.setItemText(1, _translate("tab_widget", "Select Directory"))
         self.label_44.setText(_translate("tab_widget", "Export Location"))
         self.export_channel.setItemText(0, _translate("tab_widget", "All Channels (Stack)"))
         self.export_channel.setItemText(1, _translate("tab_widget", "First Three Channels (RGB)"))
         self.label_45.setText(_translate("tab_widget", "Image Channel"))
         self.label_26.setText(_translate("tab_widget", "File Name Modifier"))
         self.export_modifier.setText(_translate("tab_widget", "_BacSeg"))
-        self.export_overwrite_setting.setText(_translate("tab_widget", "Overwrite Files"))
         self.export_image_setting.setText(_translate("tab_widget", "Export Image Files"))
-        self.label_12.setText(_translate("tab_widget", "Image Modifications"))
-        self.export_autocontrast.setText(_translate("tab_widget", "Auto Contrast"))
-        self.export_normalise.setText(_translate("tab_widget", "Normalise"))
-        self.export_scalebar.setText(_translate("tab_widget", "Show Scale Bar"))
-        self.export_invert.setText(_translate("tab_widget", "Invert "))
-        self.export_mask_background.setText(_translate("tab_widget", "Mask Background"))
-        self.export_crop_zoom.setText(_translate("tab_widget", "Crop to Current Zoom"))
-        self.export_active.setText(_translate("tab_widget", "Export Data From Active Image"))
-        self.export_all.setText(_translate("tab_widget", "Export Data From All Images"))
-        self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_8), _translate("tab_widget", "Export Data"))
-        self.label_46.setText(_translate("tab_widget", "Export Cell Statistics"))
-        self.label_54.setText(_translate("tab_widget", "ColiCoords Fit Mode"))
-        self.export_statistics_pixelsize.setText(_translate("tab_widget", "0.116999998688698"))
-        self.export_colicoords_mode.setItemText(0, _translate("tab_widget", "None (OpenCV Stats)"))
-        self.export_colicoords_mode.setItemText(1, _translate("tab_widget", "Mask"))
-        self.label_52.setText(_translate("tab_widget", "Pixel Size (um)"))
-        self.export_statistics_multithreaded.setText(_translate("tab_widget", "Multithreaded Processing"))
-        self.export_statistics_active.setText(_translate("tab_widget", "Export Cell Statistics From Active Image"))
-        self.export_statistics_all.setText(_translate("tab_widget", "Export Cell Statistics From All Images"))
-        self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_9), _translate("tab_widget", "Export Statistics"))
+        self.export_overwrite_setting.setText(_translate("tab_widget", "Overwrite Files"))
+        self.export_active.setText(_translate("tab_widget", "Export Data From Active Frame"))
+        self.export_all.setText(_translate("tab_widget", "Export Data From All Frames"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_18), _translate("tab_widget", "Export Frames"))
+        self.label_101.setText(_translate("tab_widget", "Image Channel"))
+        self.label_99.setText(_translate("tab_widget", "Export Mode"))
+        self.export_stack_mode.setItemText(0, _translate("tab_widget", "Export .tif Images"))
+        self.export_stack_mode.setItemText(1, _translate("tab_widget", "Export .tif Masks"))
+        self.label_100.setText(_translate("tab_widget", "Export Location"))
+        self.export_stack_location.setItemText(0, _translate("tab_widget", "Import Directory"))
+        self.export_stack_location.setItemText(1, _translate("tab_widget", "Select Directory"))
+        self.label_103.setText(_translate("tab_widget", "File Name Modifier"))
+        self.export_stack_modifier.setText(_translate("tab_widget", "_BacSeg"))
+        self.export_stack_image_setting.setText(_translate("tab_widget", "Export Image Files"))
+        self.export_stack_overwrite_setting.setText(_translate("tab_widget", "Overwrite Files"))
+        self.export_stack_active.setText(_translate("tab_widget", "Export Data Stack From Active Channel"))
+        self.export_stack_all.setText(_translate("tab_widget", "Export Data Stack From All Channels"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_19), _translate("tab_widget", "Export Stacks"))
         self.label_43.setText(_translate("tab_widget", "Export Cell Settings"))
         self.export_single.setText(_translate("tab_widget", "Single"))
         self.export_vertical.setText(_translate("tab_widget", "Vertical"))
         self.export_divided.setText(_translate("tab_widget", "Divided"))
         self.export_dividing.setText(_translate("tab_widget", "Dividing"))
         self.export_edge.setText(_translate("tab_widget", "Edge"))
         self.export_broken.setText(_translate("tab_widget", "Broken"))
@@ -2488,15 +2622,33 @@
         self.label_72.setText(_translate("tab_widget", "Scale Bar Thickness (pixels)"))
         self.export_scalebar_thickness.setItemText(0, _translate("tab_widget", "1"))
         self.export_scalebar_thickness.setItemText(1, _translate("tab_widget", "2"))
         self.export_scalebar_thickness.setItemText(2, _translate("tab_widget", "5"))
         self.export_scalebar_thickness.setItemText(3, _translate("tab_widget", "10"))
         self.export_scalebar_thickness.setItemText(4, _translate("tab_widget", "15"))
         self.export_scalebar_thickness.setItemText(5, _translate("tab_widget", "20"))
-        self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_13), _translate("tab_widget", "Export Settings"))
+        self.label_12.setText(_translate("tab_widget", "Image Modifications"))
+        self.export_autocontrast.setText(_translate("tab_widget", "Auto Contrast"))
+        self.export_normalise.setText(_translate("tab_widget", "Normalise"))
+        self.export_scalebar.setText(_translate("tab_widget", "Show Scale Bar"))
+        self.export_invert.setText(_translate("tab_widget", "Invert "))
+        self.export_mask_background.setText(_translate("tab_widget", "Mask Background"))
+        self.export_crop_zoom.setText(_translate("tab_widget", "Crop to Current Zoom"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_20), _translate("tab_widget", "Export Settings"))
+        self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_8), _translate("tab_widget", "Export Data"))
+        self.label_46.setText(_translate("tab_widget", "Export Cell Statistics"))
+        self.label_54.setText(_translate("tab_widget", "ColiCoords Fit Mode"))
+        self.export_statistics_pixelsize.setText(_translate("tab_widget", "0.116999998688698"))
+        self.export_colicoords_mode.setItemText(0, _translate("tab_widget", "None (OpenCV Stats)"))
+        self.export_colicoords_mode.setItemText(1, _translate("tab_widget", "Mask"))
+        self.label_52.setText(_translate("tab_widget", "Pixel Size (um)"))
+        self.export_statistics_multithreaded.setText(_translate("tab_widget", "Multithreaded Processing"))
+        self.export_statistics_active.setText(_translate("tab_widget", "Export Cell Statistics From Active Image"))
+        self.export_statistics_all.setText(_translate("tab_widget", "Export Cell Statistics From All Images"))
+        self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_9), _translate("tab_widget", "Export Statistics"))
         self.label_33.setText(_translate("tab_widget", "Progress "))
         tab_widget.setTabText(tab_widget.indexOf(self.export_tab), _translate("tab_widget", "Export"))
         self.modify_copymasktoall.setText(_translate("tab_widget", "Copy Mask From Active Image to All Images"))
         self.modify_deleteactiveimage.setText(_translate("tab_widget", "Delete Active Image [Control-I]"))
         self.modify_deleteotherimages.setText(_translate("tab_widget", "Delete All Images Except Active Image [Control-Shift-I]"))
         self.modify_deleteactivemasks.setText(_translate("tab_widget", "Delete All Masks, Active Image [Control-D]"))
         self.modify_deleteallmasks.setText(_translate("tab_widget", "Delete All Masks, All Images [Control-Shift-D]"))
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.ui` & `napari-bacseg-1.0.7/src/napari_bacseg/bacseg_ui.ui`

 * *Files 1% similar despite different names*

#### Comparing `napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.ui` & `napari-bacseg-1.0.7/src/napari_bacseg/bacseg_ui.ui`

```diff
@@ -188,30 +188,35 @@
                 </property>
               </widget>
             </item>
             <item row="6" column="1">
               <widget class="QComboBox" name="import_multiframe_mode">
                 <item>
                   <property name="text">
-                    <string>Keep First Frame</string>
+                    <string>Keep Brightest Frame</string>
                   </property>
                 </item>
                 <item>
                   <property name="text">
-                    <string>Keep Brightest Frame</string>
+                    <string>Average Frames</string>
                   </property>
                 </item>
                 <item>
                   <property name="text">
-                    <string>Average Frames</string>
+                    <string>Sum Frames</string>
                   </property>
                 </item>
                 <item>
                   <property name="text">
-                    <string>Sum Frames</string>
+                    <string>Keep First Frame</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>Keep All Frames (BETA)</string>
                   </property>
                 </item>
               </widget>
             </item>
             <item row="7" column="0">
               <widget class="QLabel" name="label_22">
                 <property name="text">
@@ -317,15 +322,15 @@
                 <item>
                   <property name="text">
                     <string>JSON (.txt) Segmentation(s)</string>
                   </property>
                 </item>
               </widget>
             </item>
-            <item row="1" column="0">
+            <item row="0" column="0">
               <widget class="QLabel" name="label_27">
                 <property name="text">
                   <string>Import Mode</string>
                 </property>
               </widget>
             </item>
           </layout>
@@ -1154,31 +1159,38 @@
               <attribute name="title">
                 <string>Segment</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout_10">
                 <item>
                   <layout class="QFormLayout" name="formLayout_12">
                     <item row="0" column="0">
+                      <widget class="QLabel" name="label_97">
+                        <property name="text">
+                          <string>Segmentation Mode</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="0">
                       <widget class="QLabel" name="label_2">
                         <property name="text">
                           <string>Segmentation Channel</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="0" column="1">
+                    <item row="1" column="1">
                       <widget class="QComboBox" name="cellpose_segchannel"/>
                     </item>
-                    <item row="1" column="0">
+                    <item row="2" column="0">
                       <widget class="QLabel" name="label">
                         <property name="text">
                           <string>Cellpose Model</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="1" column="1">
+                    <item row="2" column="1">
                       <widget class="QComboBox" name="cellpose_segmodel">
                         <item>
                           <property name="text">
                             <string>cyto</string>
                           </property>
                         </item>
                         <item>
@@ -1209,14 +1221,28 @@
                         <item>
                           <property name="text">
                             <string>custom</string>
                           </property>
                         </item>
                       </widget>
                     </item>
+                    <item row="0" column="1">
+                      <widget class="QComboBox" name="cellpose_seg_mode">
+                        <item>
+                          <property name="text">
+                            <string>Cell Wall</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Nucleiod</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
                   </layout>
                 </item>
                 <item>
                   <spacer name="verticalSpacer_9">
                     <property name="orientation">
                       <enum>Qt::Vertical</enum>
                     </property>
@@ -1482,14 +1508,28 @@
             </widget>
             <widget class="QWidget" name="tab_12">
               <attribute name="title">
                 <string>Settings</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout_14">
                 <item>
+                  <widget class="QLabel" name="label_94">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Cellpose Controls</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
                   <layout class="QGridLayout" name="gridLayout_2">
                     <item row="0" column="2" alignment="Qt::AlignLeft">
                       <widget class="QLabel" name="cellpose_flowthresh_label">
                         <property name="minimumSize">
                           <size>
                             <width>28</width>
                             <height>22</height>
@@ -1652,14 +1692,85 @@
                         <width>20</width>
                         <height>10</height>
                       </size>
                     </property>
                   </spacer>
                 </item>
                 <item>
+                  <widget class="QLabel" name="label_95">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Cellpose Post Processing</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QFormLayout" name="formLayout_21">
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="label_96">
+                        <property name="text">
+                          <string>Min Segmentation Size (Pixels)</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QComboBox" name="cellpose_min_seg_size">
+                        <property name="editable">
+                          <bool>true</bool>
+                        </property>
+                        <property name="currentText">
+                          <string>50</string>
+                        </property>
+                        <property name="currentIndex">
+                          <number>3</number>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string>1</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>5</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>10</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>50</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
+                <item>
+                  <spacer name="verticalSpacer_44">
+                    <property name="orientation">
+                      <enum>Qt::Vertical</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>20</width>
+                        <height>10</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
+                <item>
                   <widget class="QCheckBox" name="cellpose_clear_previous">
                     <property name="text">
                       <string>Clear Previous Segmentations</string>
                     </property>
                     <property name="checked">
                       <bool>true</bool>
                     </property>
@@ -1762,14 +1873,55 @@
                   <string>Segment [F2]</string>
                 </property>
               </widget>
             </item>
           </layout>
         </item>
         <item>
+          <spacer name="verticalSpacer_18">
+            <property name="orientation">
+              <enum>Qt::Vertical</enum>
+            </property>
+            <property name="sizeType">
+              <enum>QSizePolicy::Minimum</enum>
+            </property>
+            <property name="sizeHint" stdset="0">
+              <size>
+                <width>334</width>
+                <height>14</height>
+              </size>
+            </property>
+          </spacer>
+        </item>
+        <item>
+          <layout class="QFormLayout" name="formLayout_22">
+            <item row="0" column="0">
+              <widget class="QLabel" name="label_98">
+                <property name="text">
+                  <string>Curate Channel</string>
+                </property>
+              </widget>
+            </item>
+            <item row="0" column="1">
+              <widget class="QComboBox" name="modify_channel">
+                <item>
+                  <property name="text">
+                    <string>Segmentations (Cell Wall)</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>Nucleoid</string>
+                  </property>
+                </item>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item>
           <widget class="QCheckBox" name="modify_auto_panzoom">
             <property name="text">
               <string>Auto select Pan/Zoom after interface event</string>
             </property>
             <property name="checked">
               <bool>true</bool>
             </property>
@@ -4307,255 +4459,679 @@
             </property>
             <widget class="QWidget" name="tab_8">
               <attribute name="title">
                 <string>Export Data</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout_15">
                 <item>
-                  <layout class="QFormLayout" name="formLayout_6">
-                    <item row="1" column="1">
-                      <widget class="QComboBox" name="export_mode">
-                        <item>
-                          <property name="text">
-                            <string>Export .tif Images</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>Export .tif Masks</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>Export .tif Images and Masks</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>Export Cellpose</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>Export Oufti</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>Export ImageJ</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>Export JSON</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>Export CSV</string>
-                          </property>
-                        </item>
-                      </widget>
-                    </item>
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="label_19">
-                        <property name="text">
-                          <string>Export Mode</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="2" column="1">
-                      <widget class="QComboBox" name="export_location">
-                        <property name="currentIndex">
-                          <number>1</number>
-                        </property>
-                        <item>
-                          <property name="text">
-                            <string>Import Directory</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>Select Directory</string>
-                          </property>
-                        </item>
-                      </widget>
-                    </item>
-                    <item row="2" column="0">
-                      <widget class="QLabel" name="label_44">
-                        <property name="text">
-                          <string>Export Location</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="1">
-                      <widget class="QComboBox" name="export_channel">
-                        <item>
-                          <property name="text">
-                            <string>All Channels (Stack)</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>First Three Channels (RGB)</string>
-                          </property>
+                  <widget class="QTabWidget" name="tabWidget">
+                    <property name="currentIndex">
+                      <number>0</number>
+                    </property>
+                    <widget class="QWidget" name="tab_18">
+                      <attribute name="title">
+                        <string>Export Frames</string>
+                      </attribute>
+                      <layout class="QVBoxLayout" name="verticalLayout_26">
+                        <item>
+                          <layout class="QFormLayout" name="formLayout_6">
+                            <item row="1" column="1">
+                              <widget class="QComboBox" name="export_mode">
+                                <item>
+                                  <property name="text">
+                                    <string>Export .tif Images</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Export .tif Masks</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Export .tif Images and Masks</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Export Cellpose</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Export Oufti</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Export ImageJ</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Export JSON</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Export CSV</string>
+                                  </property>
+                                </item>
+                              </widget>
+                            </item>
+                            <item row="1" column="0">
+                              <widget class="QLabel" name="label_19">
+                                <property name="text">
+                                  <string>Export Mode</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="2" column="1">
+                              <widget class="QComboBox" name="export_location">
+                                <property name="currentIndex">
+                                  <number>1</number>
+                                </property>
+                                <item>
+                                  <property name="text">
+                                    <string>Import Directory</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Select Directory</string>
+                                  </property>
+                                </item>
+                              </widget>
+                            </item>
+                            <item row="2" column="0">
+                              <widget class="QLabel" name="label_44">
+                                <property name="text">
+                                  <string>Export Location</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="1">
+                              <widget class="QComboBox" name="export_channel">
+                                <item>
+                                  <property name="text">
+                                    <string>All Channels (Stack)</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>First Three Channels (RGB)</string>
+                                  </property>
+                                </item>
+                              </widget>
+                            </item>
+                            <item row="0" column="0">
+                              <widget class="QLabel" name="label_45">
+                                <property name="text">
+                                  <string>Image Channel</string>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <layout class="QFormLayout" name="formLayout_5">
+                            <item row="0" column="0">
+                              <widget class="QLabel" name="label_26">
+                                <property name="text">
+                                  <string>File Name Modifier</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="1">
+                              <widget class="QLineEdit" name="export_modifier">
+                                <property name="text">
+                                  <string>_BacSeg</string>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <layout class="QGridLayout" name="gridLayout_32">
+                            <item row="0" column="0">
+                              <widget class="QCheckBox" name="export_image_setting">
+                                <property name="text">
+                                  <string>Export Image Files</string>
+                                </property>
+                                <property name="checked">
+                                  <bool>true</bool>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="1">
+                              <widget class="QCheckBox" name="export_overwrite_setting">
+                                <property name="text">
+                                  <string>Overwrite Files</string>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <spacer name="verticalSpacer_12">
+                            <property name="orientation">
+                              <enum>Qt::Vertical</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>20</width>
+                                <height>40</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="export_active">
+                            <property name="text">
+                              <string>Export Data From Active Frame</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="export_all">
+                            <property name="text">
+                              <string>Export Data From All Frames</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </widget>
+                    <widget class="QWidget" name="tab_19">
+                      <attribute name="title">
+                        <string>Export Stacks</string>
+                      </attribute>
+                      <layout class="QVBoxLayout" name="verticalLayout_25">
+                        <item>
+                          <layout class="QFormLayout" name="formLayout_23">
+                            <item row="0" column="0">
+                              <widget class="QLabel" name="label_101">
+                                <property name="text">
+                                  <string>Image Channel</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="1">
+                              <widget class="QComboBox" name="export_stack_channel"/>
+                            </item>
+                            <item row="1" column="0">
+                              <widget class="QLabel" name="label_99">
+                                <property name="text">
+                                  <string>Export Mode</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="1">
+                              <widget class="QComboBox" name="export_stack_mode">
+                                <item>
+                                  <property name="text">
+                                    <string>Export .tif Images</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Export .tif Masks</string>
+                                  </property>
+                                </item>
+                              </widget>
+                            </item>
+                            <item row="2" column="0">
+                              <widget class="QLabel" name="label_100">
+                                <property name="text">
+                                  <string>Export Location</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="2" column="1">
+                              <widget class="QComboBox" name="export_stack_location">
+                                <property name="currentIndex">
+                                  <number>1</number>
+                                </property>
+                                <item>
+                                  <property name="text">
+                                    <string>Import Directory</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>Select Directory</string>
+                                  </property>
+                                </item>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <layout class="QFormLayout" name="formLayout_25">
+                            <item row="0" column="0">
+                              <widget class="QLabel" name="label_103">
+                                <property name="text">
+                                  <string>File Name Modifier</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="1">
+                              <widget class="QLineEdit" name="export_stack_modifier">
+                                <property name="text">
+                                  <string>_BacSeg</string>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <layout class="QGridLayout" name="gridLayout_33">
+                            <item row="0" column="0">
+                              <widget class="QCheckBox" name="export_stack_image_setting">
+                                <property name="text">
+                                  <string>Export Image Files</string>
+                                </property>
+                                <property name="checked">
+                                  <bool>true</bool>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="1">
+                              <widget class="QCheckBox" name="export_stack_overwrite_setting">
+                                <property name="text">
+                                  <string>Overwrite Files</string>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <spacer name="verticalSpacer_42">
+                            <property name="orientation">
+                              <enum>Qt::Vertical</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>20</width>
+                                <height>40</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="export_stack_active">
+                            <property name="text">
+                              <string>Export Data Stack From Active Channel</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="export_stack_all">
+                            <property name="text">
+                              <string>Export Data Stack From All Channels</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </widget>
+                    <widget class="QWidget" name="tab_20">
+                      <attribute name="title">
+                        <string>Export Settings</string>
+                      </attribute>
+                      <layout class="QVBoxLayout" name="verticalLayout_27">
+                        <item>
+                          <widget class="QLabel" name="label_43">
+                            <property name="font">
+                              <font>
+                                <pointsize>10</pointsize>
+                                <weight>75</weight>
+                                <bold>true</bold>
+                              </font>
+                            </property>
+                            <property name="text">
+                              <string>Export Cell Settings</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <layout class="QGridLayout" name="gridLayout">
+                            <item row="0" column="0">
+                              <widget class="QCheckBox" name="export_single">
+                                <property name="text">
+                                  <string>Single</string>
+                                </property>
+                                <property name="checked">
+                                  <bool>true</bool>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="0">
+                              <widget class="QCheckBox" name="export_vertical">
+                                <property name="text">
+                                  <string>Vertical</string>
+                                </property>
+                                <property name="checked">
+                                  <bool>true</bool>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="2">
+                              <widget class="QCheckBox" name="export_divided">
+                                <property name="text">
+                                  <string>Divided</string>
+                                </property>
+                                <property name="checked">
+                                  <bool>true</bool>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="1">
+                              <widget class="QCheckBox" name="export_dividing">
+                                <property name="text">
+                                  <string>Dividing</string>
+                                </property>
+                                <property name="checked">
+                                  <bool>true</bool>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="2">
+                              <widget class="QCheckBox" name="export_edge">
+                                <property name="text">
+                                  <string>Edge</string>
+                                </property>
+                                <property name="checked">
+                                  <bool>true</bool>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="1">
+                              <widget class="QCheckBox" name="export_broken">
+                                <property name="text">
+                                  <string>Broken</string>
+                                </property>
+                                <property name="checked">
+                                  <bool>true</bool>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <spacer name="verticalSpacer_36">
+                            <property name="orientation">
+                              <enum>Qt::Vertical</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>20</width>
+                                <height>10</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_49">
+                            <property name="font">
+                              <font>
+                                <pointsize>10</pointsize>
+                                <weight>75</weight>
+                                <bold>true</bold>
+                              </font>
+                            </property>
+                            <property name="text">
+                              <string>Scale Bar Settings</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <layout class="QGridLayout" name="gridLayout_27">
+                            <item row="0" column="2">
+                              <widget class="QComboBox" name="export_scalebar_resolution_units">
+                                <property name="maximumSize">
+                                  <size>
+                                    <width>200</width>
+                                    <height>100</height>
+                                  </size>
+                                </property>
+                                <item>
+                                  <property name="text">
+                                    <string>nm</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>um</string>
+                                  </property>
+                                </item>
+                              </widget>
+                            </item>
+                            <item row="0" column="0">
+                              <widget class="QLabel" name="label_50">
+                                <property name="text">
+                                  <string>Pixel Resolution</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="1">
+                              <widget class="QLineEdit" name="export_scalebar_resolution">
+                                <property name="maximumSize">
+                                  <size>
+                                    <width>200</width>
+                                    <height>16777215</height>
+                                  </size>
+                                </property>
+                                <property name="text">
+                                  <string>100</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="0">
+                              <widget class="QLabel" name="label_55">
+                                <property name="text">
+                                  <string>Scale Bar Size</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="1">
+                              <widget class="QLineEdit" name="export_scalebar_size">
+                                <property name="maximumSize">
+                                  <size>
+                                    <width>200</width>
+                                    <height>16777215</height>
+                                  </size>
+                                </property>
+                                <property name="text">
+                                  <string>20</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="2">
+                              <widget class="QComboBox" name="export_scalebar_size_units">
+                                <property name="maximumSize">
+                                  <size>
+                                    <width>200</width>
+                                    <height>100</height>
+                                  </size>
+                                </property>
+                                <property name="currentIndex">
+                                  <number>1</number>
+                                </property>
+                                <item>
+                                  <property name="text">
+                                    <string>nm</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>um</string>
+                                  </property>
+                                </item>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <layout class="QFormLayout" name="formLayout_19">
+                            <item row="0" column="0">
+                              <widget class="QLabel" name="label_71">
+                                <property name="text">
+                                  <string>Scale Bar Colour</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="0" column="1">
+                              <widget class="QComboBox" name="export_scalebar_colour">
+                                <item>
+                                  <property name="text">
+                                    <string>Black</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>White</string>
+                                  </property>
+                                </item>
+                              </widget>
+                            </item>
+                            <item row="1" column="0">
+                              <widget class="QLabel" name="label_72">
+                                <property name="text">
+                                  <string>Scale Bar Thickness (pixels)</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="1">
+                              <widget class="QComboBox" name="export_scalebar_thickness">
+                                <property name="currentIndex">
+                                  <number>3</number>
+                                </property>
+                                <item>
+                                  <property name="text">
+                                    <string>1</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>2</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>5</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>10</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>15</string>
+                                  </property>
+                                </item>
+                                <item>
+                                  <property name="text">
+                                    <string>20</string>
+                                  </property>
+                                </item>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <spacer name="verticalSpacer_26">
+                            <property name="orientation">
+                              <enum>Qt::Vertical</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>20</width>
+                                <height>10</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_12">
+                            <property name="font">
+                              <font>
+                                <pointsize>10</pointsize>
+                                <weight>75</weight>
+                                <bold>true</bold>
+                              </font>
+                            </property>
+                            <property name="text">
+                              <string>Image Modifications</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <layout class="QGridLayout" name="gridLayout_19">
+                            <item row="1" column="0">
+                              <widget class="QCheckBox" name="export_autocontrast">
+                                <property name="text">
+                                  <string>Auto Contrast</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="1">
+                              <widget class="QCheckBox" name="export_normalise">
+                                <property name="text">
+                                  <string>Normalise</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="2" column="0">
+                              <widget class="QCheckBox" name="export_scalebar">
+                                <property name="text">
+                                  <string>Show Scale Bar</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="1" column="2">
+                              <widget class="QCheckBox" name="export_invert">
+                                <property name="text">
+                                  <string>Invert</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="2" column="1">
+                              <widget class="QCheckBox" name="export_mask_background">
+                                <property name="text">
+                                  <string>Mask Background</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item row="2" column="2">
+                              <widget class="QCheckBox" name="export_crop_zoom">
+                                <property name="text">
+                                  <string>Crop to Current Zoom</string>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
                         </item>
-                      </widget>
-                    </item>
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="label_45">
-                        <property name="text">
-                          <string>Image Channel</string>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </item>
-                <item>
-                  <layout class="QFormLayout" name="formLayout_5">
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="label_26">
-                        <property name="text">
-                          <string>File Name Modifier</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="1">
-                      <widget class="QLineEdit" name="export_modifier">
-                        <property name="text">
-                          <string>_BacSeg</string>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </item>
-                <item>
-                  <layout class="QGridLayout" name="gridLayout_14">
-                    <item row="1" column="1">
-                      <widget class="QCheckBox" name="export_overwrite_setting">
-                        <property name="text">
-                          <string>Overwrite Files</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="0">
-                      <widget class="QCheckBox" name="export_image_setting">
-                        <property name="text">
-                          <string>Export Image Files</string>
-                        </property>
-                        <property name="checked">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </item>
-                <item>
-                  <spacer name="verticalSpacer_12">
-                    <property name="orientation">
-                      <enum>Qt::Vertical</enum>
-                    </property>
-                    <property name="sizeType">
-                      <enum>QSizePolicy::Minimum</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>20</width>
-                        <height>10</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-                <item>
-                  <widget class="QLabel" name="label_12">
-                    <property name="font">
-                      <font>
-                        <pointsize>10</pointsize>
-                        <weight>75</weight>
-                        <bold>true</bold>
-                      </font>
-                    </property>
-                    <property name="text">
-                      <string>Image Modifications</string>
-                    </property>
+                      </layout>
+                    </widget>
                   </widget>
                 </item>
                 <item>
-                  <layout class="QGridLayout" name="gridLayout_19">
-                    <item row="1" column="0">
-                      <widget class="QCheckBox" name="export_autocontrast">
-                        <property name="text">
-                          <string>Auto Contrast</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="1">
-                      <widget class="QCheckBox" name="export_normalise">
-                        <property name="text">
-                          <string>Normalise</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="2" column="0">
-                      <widget class="QCheckBox" name="export_scalebar">
-                        <property name="text">
-                          <string>Show Scale Bar</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="2">
-                      <widget class="QCheckBox" name="export_invert">
-                        <property name="text">
-                          <string>Invert</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="2" column="1">
-                      <widget class="QCheckBox" name="export_mask_background">
-                        <property name="text">
-                          <string>Mask Background</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="2" column="2">
-                      <widget class="QCheckBox" name="export_crop_zoom">
-                        <property name="text">
-                          <string>Crop to Current Zoom</string>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </item>
-                <item>
                   <spacer name="verticalSpacer_19">
                     <property name="orientation">
                       <enum>Qt::Vertical</enum>
                     </property>
                     <property name="sizeHint" stdset="0">
                       <size>
                         <width>20</width>
                         <height>10</height>
                       </size>
                     </property>
                   </spacer>
                 </item>
-                <item>
-                  <widget class="QPushButton" name="export_active">
-                    <property name="text">
-                      <string>Export Data From Active Image</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QPushButton" name="export_all">
-                    <property name="text">
-                      <string>Export Data From All Images</string>
-                    </property>
-                  </widget>
-                </item>
               </layout>
             </widget>
             <widget class="QWidget" name="tab_9">
               <attribute name="title">
                 <string>Export Statistics</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout_17">
@@ -4653,295 +5229,14 @@
                     <property name="text">
                       <string>Export Cell Statistics From All Images</string>
                     </property>
                   </widget>
                 </item>
               </layout>
             </widget>
-            <widget class="QWidget" name="tab_13">
-              <attribute name="title">
-                <string>Export Settings</string>
-              </attribute>
-              <layout class="QVBoxLayout" name="verticalLayout_16">
-                <item>
-                  <widget class="QLabel" name="label_43">
-                    <property name="font">
-                      <font>
-                        <pointsize>10</pointsize>
-                        <weight>75</weight>
-                        <bold>true</bold>
-                      </font>
-                    </property>
-                    <property name="text">
-                      <string>Export Cell Settings</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <layout class="QGridLayout" name="gridLayout">
-                    <item row="0" column="0">
-                      <widget class="QCheckBox" name="export_single">
-                        <property name="text">
-                          <string>Single</string>
-                        </property>
-                        <property name="checked">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="0">
-                      <widget class="QCheckBox" name="export_vertical">
-                        <property name="text">
-                          <string>Vertical</string>
-                        </property>
-                        <property name="checked">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="2">
-                      <widget class="QCheckBox" name="export_divided">
-                        <property name="text">
-                          <string>Divided</string>
-                        </property>
-                        <property name="checked">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="1">
-                      <widget class="QCheckBox" name="export_dividing">
-                        <property name="text">
-                          <string>Dividing</string>
-                        </property>
-                        <property name="checked">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="2">
-                      <widget class="QCheckBox" name="export_edge">
-                        <property name="text">
-                          <string>Edge</string>
-                        </property>
-                        <property name="checked">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="1">
-                      <widget class="QCheckBox" name="export_broken">
-                        <property name="text">
-                          <string>Broken</string>
-                        </property>
-                        <property name="checked">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </item>
-                <item>
-                  <spacer name="verticalSpacer_42">
-                    <property name="orientation">
-                      <enum>Qt::Vertical</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>20</width>
-                        <height>40</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-                <item>
-                  <widget class="QLabel" name="label_49">
-                    <property name="font">
-                      <font>
-                        <pointsize>10</pointsize>
-                        <weight>75</weight>
-                        <bold>true</bold>
-                      </font>
-                    </property>
-                    <property name="text">
-                      <string>Scale Bar Settings</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <layout class="QGridLayout" name="gridLayout_27">
-                    <item row="0" column="2">
-                      <widget class="QComboBox" name="export_scalebar_resolution_units">
-                        <property name="maximumSize">
-                          <size>
-                            <width>200</width>
-                            <height>100</height>
-                          </size>
-                        </property>
-                        <item>
-                          <property name="text">
-                            <string>nm</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>um</string>
-                          </property>
-                        </item>
-                      </widget>
-                    </item>
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="label_50">
-                        <property name="text">
-                          <string>Pixel Resolution</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="1">
-                      <widget class="QLineEdit" name="export_scalebar_resolution">
-                        <property name="maximumSize">
-                          <size>
-                            <width>200</width>
-                            <height>16777215</height>
-                          </size>
-                        </property>
-                        <property name="text">
-                          <string>100</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="label_55">
-                        <property name="text">
-                          <string>Scale Bar Size</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="1">
-                      <widget class="QLineEdit" name="export_scalebar_size">
-                        <property name="maximumSize">
-                          <size>
-                            <width>200</width>
-                            <height>16777215</height>
-                          </size>
-                        </property>
-                        <property name="text">
-                          <string>20</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="2">
-                      <widget class="QComboBox" name="export_scalebar_size_units">
-                        <property name="maximumSize">
-                          <size>
-                            <width>200</width>
-                            <height>100</height>
-                          </size>
-                        </property>
-                        <property name="currentIndex">
-                          <number>1</number>
-                        </property>
-                        <item>
-                          <property name="text">
-                            <string>nm</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>um</string>
-                          </property>
-                        </item>
-                      </widget>
-                    </item>
-                  </layout>
-                </item>
-                <item>
-                  <layout class="QFormLayout" name="formLayout_19">
-                    <item row="0" column="0">
-                      <widget class="QLabel" name="label_71">
-                        <property name="text">
-                          <string>Scale Bar Colour</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="0" column="1">
-                      <widget class="QComboBox" name="export_scalebar_colour">
-                        <item>
-                          <property name="text">
-                            <string>Black</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>White</string>
-                          </property>
-                        </item>
-                      </widget>
-                    </item>
-                    <item row="1" column="0">
-                      <widget class="QLabel" name="label_72">
-                        <property name="text">
-                          <string>Scale Bar Thickness (pixels)</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item row="1" column="1">
-                      <widget class="QComboBox" name="export_scalebar_thickness">
-                        <property name="currentIndex">
-                          <number>3</number>
-                        </property>
-                        <item>
-                          <property name="text">
-                            <string>1</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>2</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>5</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>10</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>15</string>
-                          </property>
-                        </item>
-                        <item>
-                          <property name="text">
-                            <string>20</string>
-                          </property>
-                        </item>
-                      </widget>
-                    </item>
-                  </layout>
-                </item>
-                <item>
-                  <spacer name="verticalSpacer_36">
-                    <property name="orientation">
-                      <enum>Qt::Vertical</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>20</width>
-                        <height>40</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-              </layout>
-            </widget>
           </widget>
         </item>
         <item>
           <layout class="QFormLayout" name="formLayout_11">
             <item row="0" column="0">
               <widget class="QLabel" name="label_33">
                 <property name="text">
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg.egg-info/PKG-INFO` & `napari-bacseg-1.0.7/src/napari_bacseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.6
+Version: 1.0.7
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.6/src/napari_bacseg.egg-info/SOURCES.txt` & `napari-bacseg-1.0.7/src/napari_bacseg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 src/_dev/deepsegmattest.py
 src/_dev/edit_database_columns.py
 src/_dev/fits_dev.py
 src/_dev/fix_alison_missing_file_list.py
 src/_dev/generate_scanr_movie.py
 src/_dev/get_akseg_stats.py
 src/_dev/get_species_info.py
+src/_dev/imagej_dev.py
+src/_dev/json_nuclei_dev.py
 src/_dev/luke__script.py
 src/_dev/matplotlib_Events.py
 src/_dev/move_AluGasketDFP.py
 src/_dev/move_AluGasketDFP_poster.py
 src/_dev/move_AluGasketv12_DFP.py
 src/_dev/move_AluGasketv12_DFP_Titration.py
 src/_dev/move_conor_nim_dfp_data.py
```

### Comparing `napari-bacseg-1.0.6/tox.ini` & `napari-bacseg-1.0.7/tox.ini`

 * *Files identical despite different names*

