# Comparing `tmp/sc-editor-1.8.tar.gz` & `tmp/sc-editor-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-editor-1.8.tar", last modified: Tue Jun 13 00:01:34 2023, max compression
+gzip compressed data, was "sc-editor-1.9.tar", last modified: Tue Jun 13 00:16:18 2023, max compression
```

## Comparing `sc-editor-1.8.tar` & `sc-editor-1.9.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.244399 sc-editor-1.8/
--rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-06-08 17:53:44.000000 sc-editor-1.8/LICENSE
--rw-r--r--   0 hayun      (502) staff       (20)      120 2023-06-12 05:42:31.000000 sc-editor-1.8/MANIFEST.in
--rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-13 00:01:34.243317 sc-editor-1.8/PKG-INFO
--rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-06-08 17:53:44.000000 sc-editor-1.8/README.md
--rw-rw-r--   0 hayun      (502) staff       (20)        0 2023-06-12 03:06:57.000000 sc-editor-1.8/pyproject.toml
--rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-13 00:01:34.244547 sc-editor-1.8/setup.cfg
--rw-rw-r--   0 hayun      (502) staff       (20)     1084 2023-06-13 00:01:27.000000 sc-editor-1.8/setup.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:33.989026 sc-editor-1.8/src/
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.105202 sc-editor-1.8/src/SC_Editor/
--rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)    15478 2023-06-13 00:01:05.000000 sc-editor-1.8/src/SC_Editor/__main__.py
--rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/adb_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    13743 2023-06-12 02:58:41.000000 sc-editor-1.8/src/SC_Editor/config_manager.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/csv_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.113099 sc-editor-1.8/src/SC_Editor/edits/
--rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/__init__.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.119951 sc-editor-1.8/src/SC_Editor/edits/basic/
--rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/basic/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8876 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/basic/basic_items.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/basic/catfruit.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/basic/catseyes.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/basic/ototo_base_mats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/basic/talent_orbs.py
--rw-rw-r--   0 hayun      (502) staff       (20)    16530 2023-06-12 02:58:44.000000 sc-editor-1.8/src/SC_Editor/edits/basic/talent_orbs_new.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.128202 sc-editor-1.8/src/SC_Editor/edits/cats/
--rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/cat_helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/cat_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/chara_drop.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/clear_cat_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/evolve_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/get_remove_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/talents.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/upgrade_blue.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.131573 sc-editor-1.8/src/SC_Editor/edits/gamototo/
--rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/gamototo/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/gamototo/fix_gamatoto.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/gamototo/gamatoto_xp.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/gamototo/helpers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.150912 sc-editor-1.8/src/SC_Editor/edits/levels/
--rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/aku.py
--rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/allow_filibuster_clearing.py
--rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/behemoth_culling.py
--rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/clear_tutorial.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/enigma_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/event_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/gauntlet.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/itf_timed_scores.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/legend_quest.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/main_story.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/outbreaks.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/story_level_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/towers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/treasures.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/uncanny.py
--rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.224884 sc-editor-1.8/src/SC_Editor/edits/other/
--rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/cat_shrine.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/claim_user_rank_rewards.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/create_new_account.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/fix_elsewhere.py
--rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/fix_time_issues.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/get_gold_pass.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7138 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/meow_medals.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/missions.py
--rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/play_time.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/scheme_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/trade_progress.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/unlock_enemy_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.231355 sc-editor-1.8/src/SC_Editor/edits/save_management/
--rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/save_management/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/save_management/convert.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/save_management/load.py
--rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/save_management/other.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/save_management/save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/edits/save_management/server_upload.py
--rw-rw-r--   0 hayun      (502) staff       (20)    12620 2023-06-11 11:08:39.000000 sc-editor-1.8/src/SC_Editor/feature_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4822 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/game_data_getter.py
--rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/locale_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/managed_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/parse_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/patcher.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/root_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/serialise_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/server_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3494 2023-06-13 00:01:03.000000 sc-editor-1.8/src/SC_Editor/updater.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/user_info.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-06-08 17:53:44.000000 sc-editor-1.8/src/SC_Editor/user_input_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:01:34.242361 sc-editor-1.8/src/sc_editor.egg-info/
--rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-13 00:01:33.000000 sc-editor-1.8/src/sc_editor.egg-info/PKG-INFO
--rw-r--r--   0 hayun      (502) staff       (20)     3354 2023-06-13 00:01:33.000000 sc-editor-1.8/src/sc_editor.egg-info/SOURCES.txt
--rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-13 00:01:33.000000 sc-editor-1.8/src/sc_editor.egg-info/dependency_links.txt
--rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-13 00:01:33.000000 sc-editor-1.8/src/sc_editor.egg-info/requires.txt
--rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-13 00:01:33.000000 sc-editor-1.8/src/sc_editor.egg-info/top_level.txt
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.983184 sc-editor-1.9/
+-rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-06-08 17:53:44.000000 sc-editor-1.9/LICENSE
+-rw-r--r--   0 hayun      (502) staff       (20)      120 2023-06-12 05:42:31.000000 sc-editor-1.9/MANIFEST.in
+-rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-13 00:16:18.982590 sc-editor-1.9/PKG-INFO
+-rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-06-08 17:53:44.000000 sc-editor-1.9/README.md
+-rw-rw-r--   0 hayun      (502) staff       (20)        0 2023-06-12 03:06:57.000000 sc-editor-1.9/pyproject.toml
+-rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-13 00:16:18.983319 sc-editor-1.9/setup.cfg
+-rw-rw-r--   0 hayun      (502) staff       (20)     1084 2023-06-13 00:05:48.000000 sc-editor-1.9/setup.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.910382 sc-editor-1.9/src/
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.930599 sc-editor-1.9/src/SC_Editor/
+-rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    15721 2023-06-13 00:15:24.000000 sc-editor-1.9/src/SC_Editor/__main__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/adb_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    13743 2023-06-12 02:58:41.000000 sc-editor-1.9/src/SC_Editor/config_manager.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/csv_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.930992 sc-editor-1.9/src/SC_Editor/edits/
+-rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/__init__.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.940726 sc-editor-1.9/src/SC_Editor/edits/basic/
+-rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8876 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/basic_items.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/catfruit.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/catseyes.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/ototo_base_mats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/talent_orbs.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    16530 2023-06-12 02:58:44.000000 sc-editor-1.9/src/SC_Editor/edits/basic/talent_orbs_new.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.945256 sc-editor-1.9/src/SC_Editor/edits/cats/
+-rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/cat_helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/cat_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/chara_drop.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/clear_cat_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/evolve_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/get_remove_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/talents.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/upgrade_blue.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/cats/upgrade_cats.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.951765 sc-editor-1.9/src/SC_Editor/edits/gamototo/
+-rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/fix_gamatoto.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/gamatoto_xp.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/helpers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.965053 sc-editor-1.9/src/SC_Editor/edits/levels/
+-rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/aku.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/allow_filibuster_clearing.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/behemoth_culling.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/clear_tutorial.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/enigma_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/event_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/gauntlet.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/itf_timed_scores.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/legend_quest.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/main_story.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/outbreaks.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/story_level_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/towers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/treasures.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/uncanny.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/levels/unlock_aku_realm.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.974714 sc-editor-1.9/src/SC_Editor/edits/other/
+-rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/cat_shrine.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/claim_user_rank_rewards.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/create_new_account.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/fix_elsewhere.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/fix_time_issues.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/get_gold_pass.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7138 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/meow_medals.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/missions.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/play_time.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/scheme_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/trade_progress.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/unlock_enemy_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/other/unlock_equip_menu.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.979684 sc-editor-1.9/src/SC_Editor/edits/save_management/
+-rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/convert.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/load.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/other.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/edits/save_management/server_upload.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    12620 2023-06-11 11:08:39.000000 sc-editor-1.9/src/SC_Editor/feature_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4822 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/game_data_getter.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/locale_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/managed_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/parse_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/patcher.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/root_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/serialise_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/server_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3494 2023-06-13 00:01:03.000000 sc-editor-1.9/src/SC_Editor/updater.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/user_info.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-06-08 17:53:44.000000 sc-editor-1.9/src/SC_Editor/user_input_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 00:16:18.982010 sc-editor-1.9/src/sc_editor.egg-info/
+-rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/PKG-INFO
+-rw-r--r--   0 hayun      (502) staff       (20)     3354 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/requires.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-13 00:16:18.000000 sc-editor-1.9/src/sc_editor.egg-info/top_level.txt
```

### Comparing `sc-editor-1.8/LICENSE` & `sc-editor-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/PKG-INFO` & `sc-editor-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-editor
-Version: 1.8
+Version: 1.9
 Summary: A battle cats save file editor korean version
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: cintagramabp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sc-editor-1.8/README.md` & `sc-editor-1.9/README.md`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/setup.py` & `sc-editor-1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
 setuptools.setup(
     name="sc-editor",
-    version="1.8",
+    version="1.9",
     author="cintagramabp",
     description="A battle cats save file editor korean version",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fieryhenry/BCSFE-Python",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `sc-editor-1.8/src/SC_Editor/__main__.py` & `sc-editor-1.9/src/SC_Editor/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -239,22 +239,22 @@
         ):
             helper.export_json(save_stats, path + ".json")
 
 
 if __name__ == "__main__":
     main_properties_string = """
 # start up text
-welcome_message=Welcome to the &Battle Cats Save File Editor&
-author_message=Made by &fieryhenry&
+welcome_message=&냥코대전쟁 한글 에디터&에 오신 것을 환영합니다.
+author_message=Made by &fieryhenry& and &SintagramABP&
 github_message=GitHub: &https://github.com/fieryhenry/BCSFE-Python&
 discord_message=Discord: &https://discord.gg/DvmMgvn5ZB& - Please report any bugs to &#bug-reports&, or any suggestions to &#suggestions&
 donate_message=Donate: &https://ko-fi.com/fieryhenry&
-config_file_message=Config file path: &%s&
+config_file_message=설정 파일 위치: &%s&
 # 1: config file path
-scam_warning_message=If you are asked to pay for this program, it is a scam. This program is free and always will be. If you have been scammed, please report it to the discord.
+scam_warning_message=이 프로그램에 대해 비용을 지불하라는 요청을 받는 것은 사기입니다. 이 프로그램은 무료이며 앞으로도 그럴 것입니다. 사기를 당하셨다면 디스코드로 신고해주세요.
 
 # update info
 beta_message=You are using a &beta& release, some things may be broken. Please report any bugs you find to &#bug-reports& on Discord and specify that you are using a beta version
 update_check_failed=Failed to check for updates
 local_version=Local version: &%s&
 # 1: local version
 latest_stable_version=Latest stable version: &%s&
@@ -287,15 +287,15 @@
 
 # misc
 press_enter=엔터를 눌러서 계속하기
 save_data_saved=파일을 저장함: &%s&
 # 1: save file path
 
 # errors
-error_save_json=Your save data seems to be in json format. Please use to import json option if you want to load json data.
+error_save_json=저장 데이터가 json 형식인 것 같습니다. json 데이터를 로드하려면 json 옵션을 가져오는 데 사용하십시오..
 generic_error=오류 발생: &%s&
 # 1: error message
 
     """
 
     item_properties_string = """
 ban_warning=!!경고!! %s를 에딧하는 것은 밴 위험이 높습니다! 
@@ -307,15 +307,15 @@
 # 1: max value
 enter_value_text=원하시는 %s의 값을 입력하세요. %s:
 # 1: item name
 # 2: max value
 success_set=성공적으로 %s의 값을 &%s&로 바꿨습니다.
 # 1: item name
 # 2: value
-item_value_changed=&%s&의 값이 &%s&에서 &%s&로 변경되었습니다..
+item_value_changed=&%s&의 값이 &%s&에서 &%s&로 변경되었습니다.
 # 1: item name
 # 2: old value
 # 3: new value
     """
 
     user_input_properties_string = """
 enter_item_name_explain=Enter %s %s:
@@ -326,35 +326,35 @@
 # 2: group name
 # 3: item name
 # 4: explanation
 all_text=all
 edit_text=edit
 enter_range_text=%s의 아이디들을 입력하세요. (&{{all_text}}& 를 입력하여 모두 선택, 범위 예시: &1&-&50&, 여러아이디를 공백으로 구분해 입력: &5 4 7&):
 # 1: group name
-select_list=What do you want to %s? (You can enter multiple values separated by spaces to %s multiple at once):
+select_list=%s할 것들을 선택하세요. (공백으로 구분하여 여러개 선택하여 %s하기):
 # 1: action (e.g. select)
 # 2: action (e.g. select)
-select_option_to=Select an option to %s:
+select_option_to=%s하기 위한 옵션을 선택하세요:
 # 1: action (e.g. edit)
-ask_individual=%s을 각각 에딧하려면 (&1&)번, 한번에 설정하려면 (&2&)을 입력해주세요:
+ask_individual=%s을 각각 에딧하려면 (&1&)번, 한번에 설정하려면 (&2&)번을 입력해주세요:
 # 1: item name
-select_all=&Select all&
-select=Select
-select_l=select
+select_all=&모두 선택&
+select=선택
+select_l=선택
 
 invalid_input=잘못된 입력.
-invalid_all={{invalid_input}} You can't use &all& here.
-invalid_range_format={{invalid_input}} Please enter a valid range of numbers separated by a dash.
-invalid_range={{invalid_input}} Please enter a valid integer between 1 and %s.
+invalid_all={{invalid_input}} 여기서는 &모두&를 쓸 수 없습니다.
+invalid_range_format={{invalid_input}} &-& 로 구분된 유효한 숫자 범위를 입력하십시오.
+invalid_range={{invalid_input}} 1에서 %s까지의 유효한 숫자를 입력하세요.
 # 1: max number
-invalid_int={{invalid_input}} Please enter a valid integer.
-invalid_yes_no={{invalid_input}} Please enter &yes& or &no&.
+invalid_int={{invalid_input}} 유효한 숫자를 입력하세요..
+invalid_yes_no={{invalid_input}} &yes& 또는 &no&를 입력하세요.
 
-error_option=Please enter a recognised option
-error_no_options=No options available to select from
+error_option=인식할 수 있는 옵션을 입력하세요.
+error_no_options=선택할 수 있는 옵션이 없습니다:
     """
 
     config_properties_string = """
 current_val=현재 보유량: &%s&
 # 1: current value
 
 enter_default_gv=Enter the default game version. {{current_val}} Leave blank to not specify a default game version:
```

### Comparing `sc-editor-1.8/src/SC_Editor/adb_handler.py` & `sc-editor-1.9/src/SC_Editor/adb_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/config_manager.py` & `sc-editor-1.9/src/SC_Editor/config_manager.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/csv_handler.py` & `sc-editor-1.9/src/SC_Editor/csv_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/basic/basic_items.py` & `sc-editor-1.9/src/SC_Editor/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/basic/catfruit.py` & `sc-editor-1.9/src/SC_Editor/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/basic/catseyes.py` & `sc-editor-1.9/src/SC_Editor/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/basic/ototo_base_mats.py` & `sc-editor-1.9/src/SC_Editor/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/basic/talent_orbs.py` & `sc-editor-1.9/src/SC_Editor/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/basic/talent_orbs_new.py` & `sc-editor-1.9/src/SC_Editor/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/cats/cat_helper.py` & `sc-editor-1.9/src/SC_Editor/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/cats/cat_id_selector.py` & `sc-editor-1.9/src/SC_Editor/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/cats/chara_drop.py` & `sc-editor-1.9/src/SC_Editor/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/cats/clear_cat_guide.py` & `sc-editor-1.9/src/SC_Editor/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/cats/evolve_cats.py` & `sc-editor-1.9/src/SC_Editor/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/cats/get_remove_cats.py` & `sc-editor-1.9/src/SC_Editor/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/cats/talents.py` & `sc-editor-1.9/src/SC_Editor/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/cats/upgrade_blue.py` & `sc-editor-1.9/src/SC_Editor/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/cats/upgrade_cats.py` & `sc-editor-1.9/src/SC_Editor/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/gamototo/gamatoto_xp.py` & `sc-editor-1.9/src/SC_Editor/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/gamototo/helpers.py` & `sc-editor-1.9/src/SC_Editor/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py` & `sc-editor-1.9/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/aku.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/behemoth_culling.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/clear_tutorial.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/enigma_stages.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/event_stages.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/gauntlet.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/itf_timed_scores.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/legend_quest.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/main_story.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/outbreaks.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/story_level_id_selector.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/towers.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/treasures.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/uncanny.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/levels/unlock_aku_realm.py` & `sc-editor-1.9/src/SC_Editor/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/cat_shrine.py` & `sc-editor-1.9/src/SC_Editor/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/claim_user_rank_rewards.py` & `sc-editor-1.9/src/SC_Editor/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/create_new_account.py` & `sc-editor-1.9/src/SC_Editor/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/fix_elsewhere.py` & `sc-editor-1.9/src/SC_Editor/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/fix_time_issues.py` & `sc-editor-1.9/src/SC_Editor/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/get_gold_pass.py` & `sc-editor-1.9/src/SC_Editor/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/meow_medals.py` & `sc-editor-1.9/src/SC_Editor/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/missions.py` & `sc-editor-1.9/src/SC_Editor/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/play_time.py` & `sc-editor-1.9/src/SC_Editor/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/scheme_item.py` & `sc-editor-1.9/src/SC_Editor/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/trade_progress.py` & `sc-editor-1.9/src/SC_Editor/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/other/unlock_enemy_guide.py` & `sc-editor-1.9/src/SC_Editor/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/save_management/convert.py` & `sc-editor-1.9/src/SC_Editor/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/save_management/load.py` & `sc-editor-1.9/src/SC_Editor/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/save_management/other.py` & `sc-editor-1.9/src/SC_Editor/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/save_management/save.py` & `sc-editor-1.9/src/SC_Editor/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/edits/save_management/server_upload.py` & `sc-editor-1.9/src/SC_Editor/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/feature_handler.py` & `sc-editor-1.9/src/SC_Editor/feature_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/game_data_getter.py` & `sc-editor-1.9/src/SC_Editor/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/helper.py` & `sc-editor-1.9/src/SC_Editor/helper.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/item.py` & `sc-editor-1.9/src/SC_Editor/item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/locale_handler.py` & `sc-editor-1.9/src/SC_Editor/locale_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/managed_item.py` & `sc-editor-1.9/src/SC_Editor/managed_item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/parse_save.py` & `sc-editor-1.9/src/SC_Editor/parse_save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/patcher.py` & `sc-editor-1.9/src/SC_Editor/patcher.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/root_handler.py` & `sc-editor-1.9/src/SC_Editor/root_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/serialise_save.py` & `sc-editor-1.9/src/SC_Editor/serialise_save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/server_handler.py` & `sc-editor-1.9/src/SC_Editor/server_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/updater.py` & `sc-editor-1.9/src/SC_Editor/updater.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/user_info.py` & `sc-editor-1.9/src/SC_Editor/user_info.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/SC_Editor/user_input_handler.py` & `sc-editor-1.9/src/SC_Editor/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.8/src/sc_editor.egg-info/PKG-INFO` & `sc-editor-1.9/src/sc_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-editor
-Version: 1.8
+Version: 1.9
 Summary: A battle cats save file editor korean version
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: cintagramabp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sc-editor-1.8/src/sc_editor.egg-info/SOURCES.txt` & `sc-editor-1.9/src/sc_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

