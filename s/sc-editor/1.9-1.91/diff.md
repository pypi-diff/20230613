# Comparing `tmp/sc-editor-1.9.tar.gz` & `tmp/sc-editor-1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-editor-1.9.tar", last modified: Tue Jun 13 00:16:18 2023, max compression
+gzip compressed data, was "sc-editor-1.91.tar", last modified: Tue Jun 13 01:09:55 2023, max compression
```

## Comparing `sc-editor-1.9.tar` & `sc-editor-1.91.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.983184 sc-editor-1.9/
--rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-06-08 17:53:44.000000 sc-editor-1.9/LICENSE
--rw-r--r--   0 hayun      (502) staff       (20)      120 2023-06-12 05:42:31.000000 sc-editor-1.9/MANIFEST.in
--rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-13 00:16:18.982590 sc-editor-1.9/PKG-INFO
--rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-06-08 17:53:44.000000 sc-editor-1.9/README.md
--rw-rw-r--   0 hayun      (502) staff       (20)        0 2023-06-12 03:06:57.000000 sc-editor-1.9/pyproject.toml
--rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-13 00:16:18.983319 sc-editor-1.9/setup.cfg
--rw-rw-r--   0 hayun      (502) staff       (20)     1084 2023-06-13 00:05:48.000000 sc-editor-1.9/setup.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.910382 sc-editor-1.9/src/
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.930599 sc-editor-1.9/src/SC_Editor/
--rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)    15721 2023-06-13 00:15:24.000000 sc-editor-1.9/src/SC_Editor/__main__.py
--rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/adb_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    13743 2023-06-12 02:58:41.000000 sc-editor-1.9/src/SC_Editor/config_manager.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/csv_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.930992 sc-editor-1.9/src/SC_Editor/edits/
--rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/__init__.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.940726 sc-editor-1.9/src/SC_Editor/edits/basic/
--rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8876 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/basic_items.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/catfruit.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/catseyes.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/ototo_base_mats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/talent_orbs.py
--rw-rw-r--   0 hayun      (502) staff       (20)    16530 2023-06-12 02:58:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/talent_orbs_new.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.945256 sc-editor-1.9/src/SC_Editor/edits/cats/
--rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/cat_helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/cat_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/chara_drop.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/clear_cat_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/evolve_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/get_remove_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/talents.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/upgrade_blue.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.951765 sc-editor-1.9/src/SC_Editor/edits/gamototo/
--rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/fix_gamatoto.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/gamatoto_xp.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/helpers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.965053 sc-editor-1.9/src/SC_Editor/edits/levels/
--rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/aku.py
--rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/allow_filibuster_clearing.py
--rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/behemoth_culling.py
--rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/clear_tutorial.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/enigma_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/event_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/gauntlet.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/itf_timed_scores.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/legend_quest.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/main_story.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/outbreaks.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/story_level_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/towers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/treasures.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/uncanny.py
--rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.974714 sc-editor-1.9/src/SC_Editor/edits/other/
--rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/cat_shrine.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/claim_user_rank_rewards.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/create_new_account.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/fix_elsewhere.py
--rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/fix_time_issues.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/get_gold_pass.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7138 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/meow_medals.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/missions.py
--rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/play_time.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/scheme_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/trade_progress.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/unlock_enemy_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.979684 sc-editor-1.9/src/SC_Editor/edits/save_management/
--rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/convert.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/load.py
--rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/other.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/server_upload.py
--rw-rw-r--   0 hayun      (502) staff       (20)    12620 2023-06-11 11:08:39.000000 sc-editor-1.9/src/SC_Editor/feature_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4822 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/game_data_getter.py
--rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/locale_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/managed_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/parse_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/patcher.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/root_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/serialise_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/server_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3494 2023-06-13 00:01:03.000000 sc-editor-1.9/src/SC_Editor/updater.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/user_info.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/user_input_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.982010 sc-editor-1.9/src/sc_editor.egg-info/
--rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/PKG-INFO
--rw-r--r--   0 hayun      (502) staff       (20)     3354 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/SOURCES.txt
--rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/dependency_links.txt
--rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/requires.txt
--rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/top_level.txt
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.384950 sc-editor-1.91/
+-rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-06-08 17:53:44.000000 sc-editor-1.91/LICENSE
+-rw-r--r--   0 hayun      (502) staff       (20)      120 2023-06-12 05:42:31.000000 sc-editor-1.91/MANIFEST.in
+-rw-r--r--   0 hayun      (502) staff       (20)    10977 2023-06-13 01:09:55.384426 sc-editor-1.91/PKG-INFO
+-rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-06-08 17:53:44.000000 sc-editor-1.91/README.md
+-rw-rw-r--   0 hayun      (502) staff       (20)        0 2023-06-12 03:06:57.000000 sc-editor-1.91/pyproject.toml
+-rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-13 01:09:55.385093 sc-editor-1.91/setup.cfg
+-rw-rw-r--   0 hayun      (502) staff       (20)     1085 2023-06-13 01:09:46.000000 sc-editor-1.91/setup.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:54.937079 sc-editor-1.91/src/
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.168105 sc-editor-1.91/src/SC_Editor/
+-rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    15733 2023-06-13 01:01:02.000000 sc-editor-1.91/src/SC_Editor/__main__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/adb_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    13743 2023-06-12 02:58:41.000000 sc-editor-1.91/src/SC_Editor/config_manager.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/csv_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.173633 sc-editor-1.91/src/SC_Editor/edits/
+-rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/__init__.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.218573 sc-editor-1.91/src/SC_Editor/edits/basic/
+-rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8987 2023-06-13 01:09:41.000000 sc-editor-1.91/src/SC_Editor/edits/basic/basic_items.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/catfruit.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/catseyes.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/ototo_base_mats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/talent_orbs.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    16530 2023-06-12 02:58:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/talent_orbs_new.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.283862 sc-editor-1.91/src/SC_Editor/edits/cats/
+-rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/cat_helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/cat_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/chara_drop.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/clear_cat_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/evolve_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/get_remove_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/talents.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/upgrade_blue.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/upgrade_cats.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.288700 sc-editor-1.91/src/SC_Editor/edits/gamototo/
+-rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/fix_gamatoto.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/gamatoto_xp.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/helpers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.321785 sc-editor-1.91/src/SC_Editor/edits/levels/
+-rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/aku.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/allow_filibuster_clearing.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/behemoth_culling.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/clear_tutorial.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/enigma_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/event_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/gauntlet.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/itf_timed_scores.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/legend_quest.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/main_story.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/outbreaks.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/story_level_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/towers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/treasures.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/uncanny.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/unlock_aku_realm.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.366259 sc-editor-1.91/src/SC_Editor/edits/other/
+-rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/cat_shrine.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/claim_user_rank_rewards.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/create_new_account.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/fix_elsewhere.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/fix_time_issues.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/get_gold_pass.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7138 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/meow_medals.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/missions.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/play_time.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/scheme_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/trade_progress.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/unlock_enemy_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/unlock_equip_menu.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.378980 sc-editor-1.91/src/SC_Editor/edits/save_management/
+-rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/convert.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/load.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/other.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/server_upload.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    12771 2023-06-13 01:06:35.000000 sc-editor-1.91/src/SC_Editor/feature_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4822 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/game_data_getter.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/locale_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/managed_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/parse_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/patcher.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/root_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/serialise_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/server_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3494 2023-06-13 00:01:03.000000 sc-editor-1.91/src/SC_Editor/updater.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/user_info.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/user_input_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.383093 sc-editor-1.91/src/sc_editor.egg-info/
+-rw-r--r--   0 hayun      (502) staff       (20)    10977 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/PKG-INFO
+-rw-r--r--   0 hayun      (502) staff       (20)     3354 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/requires.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/top_level.txt
```

### Comparing `sc-editor-1.9/LICENSE` & `sc-editor-1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/PKG-INFO` & `sc-editor-1.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-editor
-Version: 1.9
+Version: 1.91
 Summary: A battle cats save file editor korean version
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: cintagramabp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sc-editor-1.9/README.md` & `sc-editor-1.91/README.md`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/setup.py` & `sc-editor-1.91/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
 setuptools.setup(
     name="sc-editor",
-    version="1.9",
+    version="1.91",
     author="cintagramabp",
     description="A battle cats save file editor korean version",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fieryhenry/BCSFE-Python",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `sc-editor-1.9/src/SC_Editor/__main__.py` & `sc-editor-1.91/src/SC_Editor/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
 
 enter_default_gv=Enter the default game version. {{current_val}} Leave blank to not specify a default game version:
 select_default_save_path=Select the default save file path
 fixed_save_path=Fixed save path? (on=not based on current working directory)
 select_locale=Select the locale to use. {{current_val}}
 flag_set_config=Do you want to enable (&1&) or disable (&0&) %s. {{current_val}}:
 # 1: flag name
-enter_new_val_config=Enter the new value for %s. {{current_val}}:
+enter_new_val_config=%s의 새로운 값을 입력하세요. {{current_val}}:
 # 1: value name
 select_config_path=Select the config file path
 enabled=Enabled
 disabled=Disabled
 
     """
     localesdir = os.path.join(os.path.join(helper.get_local_files_path(), "locales"), "en")
```

### Comparing `sc-editor-1.9/src/SC_Editor/adb_handler.py` & `sc-editor-1.91/src/SC_Editor/adb_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/config_manager.py` & `sc-editor-1.91/src/SC_Editor/config_manager.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/csv_handler.py` & `sc-editor-1.91/src/SC_Editor/csv_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/basic/basic_items.py` & `sc-editor-1.91/src/SC_Editor/edits/basic/basic_items.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ... import item, managed_item
 
 
 def edit_cat_food(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing cat food"""
 
     cat_food = item.IntItem(
-        name="Cat Food",
+        name="고양이 통조림",
         value=item.Int(save_stats["cat_food"]["Value"]),
         max_value=45000,
         bannable=item.Bannable(
             managed_item.ManagedItemType.CATFOOD, save_stats["inquiry_code"]
         ),
     )
     cat_food.edit()
@@ -32,28 +32,28 @@
     return save_stats
 
 
 def edit_normal_tickets(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing normal tickets"""
 
     normal_tickets = item.IntItem(
-        name="Normal Tickets",
+        name="냥코 티켓",
         value=item.Int(save_stats["normal_tickets"]["Value"]),
         max_value=2999,
     )
     normal_tickets.edit()
     save_stats["normal_tickets"]["Value"] = normal_tickets.get_value()
     return save_stats
 
 
 def edit_rare_tickets(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing rare tickets"""
 
     rare_tickets = item.IntItem(
-        name="Rare Tickets",
+        name="레어 티켓",
         value=item.Int(save_stats["rare_tickets"]["Value"]),
         max_value=299,
         bannable=item.Bannable(
             inquiry_code=save_stats["inquiry_code"],
             work_around='&Instead of editing rare tickets directly, use the "Normal Ticket Max Trade Progress" conversion feature instead! It is much more safe.',
             type=managed_item.ManagedItemType.RARE_TICKET,
         ),
@@ -63,15 +63,15 @@
     return save_stats
 
 
 def edit_platinum_tickets(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing platinum tickets"""
 
     platinum_tickets = item.IntItem(
-        name="Platinum Tickets",
+        name="플래티넘 티켓",
         value=item.Int(save_stats["platinum_tickets"]["Value"]),
         max_value=9,
         bannable=item.Bannable(
             inquiry_code=save_stats["inquiry_code"],
             work_around="&Instead of editing platinum tickets, edit platinum shards instead! They are much more safe. 10 platinum shards = 1 platinum ticket",
             type=managed_item.ManagedItemType.PLATINUM_TICKET,
         ),
@@ -83,15 +83,15 @@
 
 def edit_platinum_shards(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing platinum shards"""
 
     ticket_amount = save_stats["platinum_tickets"]["Value"]
     max_value = 99 - (ticket_amount * 10)
     platinum_shards = item.IntItem(
-        name="Platinum Shards",
+        name="플래티넘 조각",
         value=item.Int(save_stats["platinum_shards"]["Value"]),
         max_value=max_value,
     )
     platinum_shards.edit()
     save_stats["platinum_shards"]["Value"] = platinum_shards.get_value()
     return save_stats
 
@@ -109,84 +109,84 @@
     return save_stats
 
 
 def edit_leadership(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing leadership"""
 
     leadership = item.IntItem(
-        name="Leadership",
+        name="리더쉽",
         value=item.Int(save_stats["leadership"]["Value"]),
         max_value=9999,
     )
     leadership.edit()
     save_stats["leadership"]["Value"] = leadership.get_value()
     return save_stats
 
 
 def edit_battle_items(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing battle items"""
 
     battle_items = item.IntItemGroup.from_lists(
         names=[
-            "Speed Up",
-            "Treasure Radar",
-            "Rich Cat",
-            "Cat CPU",
-            "Cat Jobs",
-            "Sniper the Cat",
+            "스피드 업",
+            "트레져 레이더",
+            "고양이 도령",
+            "야옹컴",
+            "고양이 박사",
+            "스냥이퍼",
         ],
         values=save_stats["battle_items"],
         maxes=9999,
-        group_name="Battle Items",
+        group_name="배틀 아이템",
     )
     battle_items.edit()
     save_stats["battle_items"] = battle_items.get_values()
 
     return save_stats
 
 
 def edit_engineers(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing ototo engineers"""
 
     engineers = item.IntItem(
-        name="Ototo Engineers",
+        name="오토토 조수",
         value=item.Int(save_stats["engineers"]["Value"]),
         max_value=5,
     )
     engineers.edit()
     save_stats["engineers"]["Value"] = engineers.get_value()
     return save_stats
 
 
 def edit_catamins(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing catamins"""
 
     catamins = item.IntItemGroup.from_lists(
         names=[
-            "Catamin A",
-            "Catamin B",
-            "Catamin C",
+            "드링크 A",
+            "드링크 B",
+            "드링크 C",
         ],
         values=save_stats["catamins"],
         maxes=9999,
-        group_name="Catamins",
+        group_name="고양이 드링크",
     )
     catamins.edit()
     save_stats["catamins"] = catamins.get_values()
     return save_stats
 
 
 def edit_inquiry_code(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the inquiry code"""
 
     print(
-        "WARNING: Editing your inquiry code should only be done if you know what you are doing! Because it will lead to an elsewhere error in-game if not done correctly!"
+        "경고: 문의 코드 편집은 자신이 무엇을 하고 있는지 알고 있는 경우에만 수행해야 합니다! 올바르게 수행하지 않으면 게임 내에서 다른 오류가 발생합니다!"
     )
     inquiry_code = item.StrItem(
-        name="Inquiry Code",
+        name="문의코드",
         value=save_stats["inquiry_code"],
     )
     inquiry_code.edit()
     save_stats["inquiry_code"] = inquiry_code.get_value()
     return save_stats
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sc-editor-1.9/src/SC_Editor/edits/basic/catfruit.py` & `sc-editor-1.91/src/SC_Editor/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/basic/catseyes.py` & `sc-editor-1.91/src/SC_Editor/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/basic/ototo_base_mats.py` & `sc-editor-1.91/src/SC_Editor/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/basic/talent_orbs.py` & `sc-editor-1.91/src/SC_Editor/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/basic/talent_orbs_new.py` & `sc-editor-1.91/src/SC_Editor/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/cats/cat_helper.py` & `sc-editor-1.91/src/SC_Editor/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/cats/cat_id_selector.py` & `sc-editor-1.91/src/SC_Editor/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/cats/chara_drop.py` & `sc-editor-1.91/src/SC_Editor/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/cats/clear_cat_guide.py` & `sc-editor-1.91/src/SC_Editor/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/cats/evolve_cats.py` & `sc-editor-1.91/src/SC_Editor/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/cats/get_remove_cats.py` & `sc-editor-1.91/src/SC_Editor/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/cats/talents.py` & `sc-editor-1.91/src/SC_Editor/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/cats/upgrade_blue.py` & `sc-editor-1.91/src/SC_Editor/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/cats/upgrade_cats.py` & `sc-editor-1.91/src/SC_Editor/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/gamototo/gamatoto_xp.py` & `sc-editor-1.91/src/SC_Editor/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/gamototo/helpers.py` & `sc-editor-1.91/src/SC_Editor/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py` & `sc-editor-1.91/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/aku.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/behemoth_culling.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/clear_tutorial.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/enigma_stages.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/event_stages.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/gauntlet.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/itf_timed_scores.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/legend_quest.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/main_story.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/outbreaks.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/story_level_id_selector.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/towers.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/treasures.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/uncanny.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/levels/unlock_aku_realm.py` & `sc-editor-1.91/src/SC_Editor/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/cat_shrine.py` & `sc-editor-1.91/src/SC_Editor/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/claim_user_rank_rewards.py` & `sc-editor-1.91/src/SC_Editor/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/create_new_account.py` & `sc-editor-1.91/src/SC_Editor/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/fix_elsewhere.py` & `sc-editor-1.91/src/SC_Editor/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/fix_time_issues.py` & `sc-editor-1.91/src/SC_Editor/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/get_gold_pass.py` & `sc-editor-1.91/src/SC_Editor/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/meow_medals.py` & `sc-editor-1.91/src/SC_Editor/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/missions.py` & `sc-editor-1.91/src/SC_Editor/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/play_time.py` & `sc-editor-1.91/src/SC_Editor/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/scheme_item.py` & `sc-editor-1.91/src/SC_Editor/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/trade_progress.py` & `sc-editor-1.91/src/SC_Editor/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/other/unlock_enemy_guide.py` & `sc-editor-1.91/src/SC_Editor/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/save_management/convert.py` & `sc-editor-1.91/src/SC_Editor/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/save_management/load.py` & `sc-editor-1.91/src/SC_Editor/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/save_management/other.py` & `sc-editor-1.91/src/SC_Editor/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/save_management/save.py` & `sc-editor-1.91/src/SC_Editor/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/edits/save_management/server_upload.py` & `sc-editor-1.91/src/SC_Editor/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/feature_handler.py` & `sc-editor-1.91/src/SC_Editor/feature_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,56 +49,56 @@
         "Export save data as json": save_management.other.export,
         "Clear save data with adb (used to generate a new account without re-installing the game)": save_management.other.clear_data,
         "Upload tracked bannable items (This is done automatically when saving or exiting)": save_management.server_upload.upload_metadata,
         "Load save data": save_management.load.select,
         "Convert save data to to a different version": save_management.convert.convert_save,
         # "Manage Presets": preset_handler.preset_manager,
     },
-    "Items": {
+    "아이템": {
         "통조림": basic.basic_items.edit_cat_food,
         "XP": basic.basic_items.edit_xp,
-        "Tickets": {
-            "Normal Tickets": basic.basic_items.edit_normal_tickets,
-            "Rare Tickets": basic.basic_items.edit_rare_tickets,
-            "Platinum Tickets": basic.basic_items.edit_platinum_tickets,
-            "Platinum Shards": basic.basic_items.edit_platinum_shards,
-            "Legend Tickets": basic.basic_items.edit_legend_tickets,
+        "티켓": {
+            "냥코 티켓": basic.basic_items.edit_normal_tickets,
+            "레어 티켓": basic.basic_items.edit_rare_tickets,
+            "플래티넘 티켓": basic.basic_items.edit_platinum_tickets,
+            "플래티넘 조각": basic.basic_items.edit_platinum_shards,
+            "레전드 티켓": basic.basic_items.edit_legend_tickets,
         },
         "NP": basic.basic_items.edit_np,
-        "Leadership": basic.basic_items.edit_leadership,
-        "Battle Items": basic.basic_items.edit_battle_items,
-        "Catseyes": basic.catseyes.edit_catseyes,
-        "Cat Fruit / Behemoth Stones": basic.catfruit.edit_catfruit,
-        "Talent Orbs": basic.talent_orbs_new.edit_talent_orbs,
-        "Catamins": basic.basic_items.edit_catamins,
-        "Item Schemes (Allows you to get unbannable items)": other.scheme_item.edit_scheme_data,
+        "리더쉽": basic.basic_items.edit_leadership,
+        "배틀 아이템": basic.basic_items.edit_battle_items,
+        "캣츠아이": basic.catseyes.edit_catseyes,
+        "개다래 / 수석": basic.catfruit.edit_catfruit,
+        "본능 구슬": basic.talent_orbs_new.edit_talent_orbs,
+        "고양이 드링크": basic.basic_items.edit_catamins,
+        "항목 구성표(금지할 수 없는 항목을 얻을 수 있음)": other.scheme_item.edit_scheme_data,
     },
-    "Gamatoto / Ototo": {
-        "Ototo Engineers": basic.basic_items.edit_engineers,
-        "Base materials": basic.ototo_base_mats.edit_base_mats,
-        "Catamins": basic.basic_items.edit_catamins,
-        "Gamatoto XP / Level": gamototo.gamatoto_xp.edit_gamatoto_xp,
-        "Ototo Cat Cannon": gamototo.ototo_cat_cannon.edit_cat_cannon,
-        "Gamatoto Helpers": gamototo.helpers.edit_helpers,
-        "Fix gamatoto from crashing the game": gamototo.fix_gamatoto.fix_gamatoto,
+    "가마토토 / 오토토": {
+        "오토토 조수": basic.basic_items.edit_engineers,
+        "성 재료": basic.ototo_base_mats.edit_base_mats,
+        "고양이 드링크": basic.basic_items.edit_catamins,
+        "가마토토 XP / 레벨": gamototo.gamatoto_xp.edit_gamatoto_xp,
+        "오토토 대포": gamototo.ototo_cat_cannon.edit_cat_cannon,
+        "가마토토 대원": gamototo.helpers.edit_helpers,
+        "가마토토가 게임을 튕기는 버그 수정": gamototo.fix_gamatoto.fix_gamatoto,
     },
-    "Cats / Special Skills": {
-        "Get / Remove Cats": {
-            "Get Cats": cats.get_remove_cats.get_cat,
-            "Remove Cats": cats.get_remove_cats.remove_cats,
+    "캐릭터 / 특능": {
+        "캐릭터 획득 / 제거": {
+            "캐릭터 획득": cats.get_remove_cats.get_cat,
+            "캐릭터 제거": cats.get_remove_cats.remove_cats,
         },
-        "Upgrade Cats": cats.upgrade_cats.upgrade_cats,
-        "True Form Cats": {
-            "Get Cat True Forms": cats.evolve_cats.get_evolve,
-            "Remove Cat True Forms": cats.evolve_cats.remove_evolve,
-            "Force True Form Cats (will lead to blank cats for cats without a true form)": cats.evolve_cats.get_evolve_forced,
+        "캐릭터 업그레이드": cats.upgrade_cats.upgrade_cats,
+        "캐릭터 3단 진화": {
+            "3단 진화 획득": cats.evolve_cats.get_evolve,
+            "3단 진화 제거": cats.evolve_cats.remove_evolve,
+            "강제 3단 진화 (3단 진화가 없는 고양이의 경우 빈 고양이로 채워짐)": cats.evolve_cats.get_evolve_forced,
         },
-        "Talents": {
-            "Set talents for each selected cat individually": cats.talents.edit_talents_individual,
-            "Max / Remove all selected cat talents": cats.talents.max_all_talents,
+        "본능": {
+            "선택한 각 고양이의 본능을 개별적으로 설정": cats.talents.edit_talents_individual,
+            "선택된 모든 고양이 본능 만렙 / 제거": cats.talents.max_all_talents,
         },
         "Collect / Remove Cat Guide": {
             "Set Cat Guide Entries (does not give cf)": cats.clear_cat_guide.collect_cat_guide,
             "Unclaim Cat Guide Entries": cats.clear_cat_guide.remove_cat_guide,
         },
         'Get stage unit drops - removes the "Clear this stage to get special cat" dialog': cats.chara_drop.get_character_drops,
         "Upgrade special skills / abilities": cats.upgrade_blue.upgrade_blue,
```

### Comparing `sc-editor-1.9/src/SC_Editor/game_data_getter.py` & `sc-editor-1.91/src/SC_Editor/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/helper.py` & `sc-editor-1.91/src/SC_Editor/helper.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/item.py` & `sc-editor-1.91/src/SC_Editor/item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/locale_handler.py` & `sc-editor-1.91/src/SC_Editor/locale_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/managed_item.py` & `sc-editor-1.91/src/SC_Editor/managed_item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/parse_save.py` & `sc-editor-1.91/src/SC_Editor/parse_save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/patcher.py` & `sc-editor-1.91/src/SC_Editor/patcher.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/root_handler.py` & `sc-editor-1.91/src/SC_Editor/root_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/serialise_save.py` & `sc-editor-1.91/src/SC_Editor/serialise_save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/server_handler.py` & `sc-editor-1.91/src/SC_Editor/server_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/updater.py` & `sc-editor-1.91/src/SC_Editor/updater.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/user_info.py` & `sc-editor-1.91/src/SC_Editor/user_info.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/SC_Editor/user_input_handler.py` & `sc-editor-1.91/src/SC_Editor/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.9/src/sc_editor.egg-info/PKG-INFO` & `sc-editor-1.91/src/sc_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-editor
-Version: 1.9
+Version: 1.91
 Summary: A battle cats save file editor korean version
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: cintagramabp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sc-editor-1.9/src/sc_editor.egg-info/SOURCES.txt` & `sc-editor-1.91/src/sc_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

