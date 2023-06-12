# Comparing `tmp/sc-editor-1.5.tar.gz` & `tmp/sc-editor-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-editor-1.5.tar", last modified: Mon Jun 12 09:17:07 2023, max compression
+gzip compressed data, was "sc-editor-1.6.tar", last modified: Mon Jun 12 23:54:32 2023, max compression
```

## Comparing `sc-editor-1.5.tar` & `sc-editor-1.6.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.404189 sc-editor-1.5/
--rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-06-08 17:53:44.000000 sc-editor-1.5/LICENSE
--rw-r--r--   0 hayun      (502) staff       (20)      120 2023-06-12 05:42:31.000000 sc-editor-1.5/MANIFEST.in
--rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-12 09:17:07.403757 sc-editor-1.5/PKG-INFO
--rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-06-08 17:53:44.000000 sc-editor-1.5/README.md
--rw-rw-r--   0 hayun      (502) staff       (20)        0 2023-06-12 03:06:57.000000 sc-editor-1.5/pyproject.toml
--rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-12 09:17:07.404301 sc-editor-1.5/setup.cfg
--rw-rw-r--   0 hayun      (502) staff       (20)     1084 2023-06-12 09:16:34.000000 sc-editor-1.5/setup.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.172069 sc-editor-1.5/src/
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.298392 sc-editor-1.5/src/SC_Editor/
--rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)    15455 2023-06-12 09:16:55.000000 sc-editor-1.5/src/SC_Editor/__main__.py
--rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/adb_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    13743 2023-06-12 02:58:41.000000 sc-editor-1.5/src/SC_Editor/config_manager.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/csv_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.300113 sc-editor-1.5/src/SC_Editor/edits/
--rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/__init__.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.307795 sc-editor-1.5/src/SC_Editor/edits/basic/
--rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/basic/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8876 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/basic/basic_items.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/basic/catfruit.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/basic/catseyes.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/basic/ototo_base_mats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/basic/talent_orbs.py
--rw-rw-r--   0 hayun      (502) staff       (20)    16530 2023-06-12 02:58:44.000000 sc-editor-1.5/src/SC_Editor/edits/basic/talent_orbs_new.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.323495 sc-editor-1.5/src/SC_Editor/edits/cats/
--rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/cat_helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/cat_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/chara_drop.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/clear_cat_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/evolve_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/get_remove_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/talents.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/upgrade_blue.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.334823 sc-editor-1.5/src/SC_Editor/edits/gamototo/
--rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/gamototo/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/gamototo/fix_gamatoto.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/gamototo/gamatoto_xp.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/gamototo/helpers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.368040 sc-editor-1.5/src/SC_Editor/edits/levels/
--rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/aku.py
--rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/allow_filibuster_clearing.py
--rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/behemoth_culling.py
--rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/clear_tutorial.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/enigma_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/event_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/gauntlet.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/itf_timed_scores.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/legend_quest.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/main_story.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/outbreaks.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/story_level_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/towers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/treasures.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/uncanny.py
--rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.388671 sc-editor-1.5/src/SC_Editor/edits/other/
--rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/cat_shrine.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/claim_user_rank_rewards.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/create_new_account.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/fix_elsewhere.py
--rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/fix_time_issues.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/get_gold_pass.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7138 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/meow_medals.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/missions.py
--rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/play_time.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/scheme_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/trade_progress.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/unlock_enemy_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.394887 sc-editor-1.5/src/SC_Editor/edits/save_management/
--rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/save_management/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/save_management/convert.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/save_management/load.py
--rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/save_management/other.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/save_management/save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/edits/save_management/server_upload.py
--rw-rw-r--   0 hayun      (502) staff       (20)    12620 2023-06-11 11:08:39.000000 sc-editor-1.5/src/SC_Editor/feature_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4822 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/game_data_getter.py
--rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/locale_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/managed_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/parse_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/patcher.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/root_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/serialise_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/server_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3544 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/updater.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/user_info.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-06-08 17:53:44.000000 sc-editor-1.5/src/SC_Editor/user_input_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 09:17:07.402843 sc-editor-1.5/src/sc_editor.egg-info/
--rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-12 09:17:07.000000 sc-editor-1.5/src/sc_editor.egg-info/PKG-INFO
--rw-r--r--   0 hayun      (502) staff       (20)     3354 2023-06-12 09:17:07.000000 sc-editor-1.5/src/sc_editor.egg-info/SOURCES.txt
--rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-12 09:17:07.000000 sc-editor-1.5/src/sc_editor.egg-info/dependency_links.txt
--rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-12 09:17:07.000000 sc-editor-1.5/src/sc_editor.egg-info/requires.txt
--rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-12 09:17:07.000000 sc-editor-1.5/src/sc_editor.egg-info/top_level.txt
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.267499 sc-editor-1.6/
+-rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-06-08 17:53:44.000000 sc-editor-1.6/LICENSE
+-rw-r--r--   0 hayun      (502) staff       (20)      120 2023-06-12 05:42:31.000000 sc-editor-1.6/MANIFEST.in
+-rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-12 23:54:32.266198 sc-editor-1.6/PKG-INFO
+-rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-06-08 17:53:44.000000 sc-editor-1.6/README.md
+-rw-rw-r--   0 hayun      (502) staff       (20)        0 2023-06-12 03:06:57.000000 sc-editor-1.6/pyproject.toml
+-rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-12 23:54:32.267691 sc-editor-1.6/setup.cfg
+-rw-rw-r--   0 hayun      (502) staff       (20)     1084 2023-06-12 23:52:34.000000 sc-editor-1.6/setup.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:31.996123 sc-editor-1.6/src/
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.021566 sc-editor-1.6/src/SC_Editor/
+-rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    15515 2023-06-12 23:54:17.000000 sc-editor-1.6/src/SC_Editor/__main__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/adb_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    13743 2023-06-12 02:58:41.000000 sc-editor-1.6/src/SC_Editor/config_manager.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/csv_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.021979 sc-editor-1.6/src/SC_Editor/edits/
+-rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/__init__.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.043844 sc-editor-1.6/src/SC_Editor/edits/basic/
+-rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/basic/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8876 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/basic/basic_items.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/basic/catfruit.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/basic/catseyes.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/basic/ototo_base_mats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/basic/talent_orbs.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    16530 2023-06-12 02:58:44.000000 sc-editor-1.6/src/SC_Editor/edits/basic/talent_orbs_new.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.053832 sc-editor-1.6/src/SC_Editor/edits/cats/
+-rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/cat_helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/cat_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/chara_drop.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/clear_cat_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/evolve_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/get_remove_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/talents.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/upgrade_blue.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/cats/upgrade_cats.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.062733 sc-editor-1.6/src/SC_Editor/edits/gamototo/
+-rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/gamototo/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/gamototo/fix_gamatoto.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/gamototo/gamatoto_xp.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/gamototo/helpers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.218654 sc-editor-1.6/src/SC_Editor/edits/levels/
+-rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/aku.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/allow_filibuster_clearing.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/behemoth_culling.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/clear_tutorial.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/enigma_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/event_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/gauntlet.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/itf_timed_scores.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/legend_quest.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/main_story.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/outbreaks.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/story_level_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/towers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/treasures.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/uncanny.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/levels/unlock_aku_realm.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.249582 sc-editor-1.6/src/SC_Editor/edits/other/
+-rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/cat_shrine.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/claim_user_rank_rewards.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/create_new_account.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/fix_elsewhere.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/fix_time_issues.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/get_gold_pass.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7138 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/meow_medals.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/missions.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/play_time.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/scheme_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/trade_progress.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/unlock_enemy_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/other/unlock_equip_menu.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.256745 sc-editor-1.6/src/SC_Editor/edits/save_management/
+-rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/save_management/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/save_management/convert.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/save_management/load.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/save_management/other.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/save_management/save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/edits/save_management/server_upload.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    12620 2023-06-11 11:08:39.000000 sc-editor-1.6/src/SC_Editor/feature_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4822 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/game_data_getter.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/locale_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/managed_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/parse_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/patcher.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/root_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/serialise_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/server_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3544 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/updater.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/user_info.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-06-08 17:53:44.000000 sc-editor-1.6/src/SC_Editor/user_input_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-12 23:54:32.264915 sc-editor-1.6/src/sc_editor.egg-info/
+-rw-r--r--   0 hayun      (502) staff       (20)    10976 2023-06-12 23:54:31.000000 sc-editor-1.6/src/sc_editor.egg-info/PKG-INFO
+-rw-r--r--   0 hayun      (502) staff       (20)     3354 2023-06-12 23:54:31.000000 sc-editor-1.6/src/sc_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-12 23:54:31.000000 sc-editor-1.6/src/sc_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-12 23:54:31.000000 sc-editor-1.6/src/sc_editor.egg-info/requires.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-12 23:54:31.000000 sc-editor-1.6/src/sc_editor.egg-info/top_level.txt
```

### Comparing `sc-editor-1.5/LICENSE` & `sc-editor-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/PKG-INFO` & `sc-editor-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-editor
-Version: 1.5
+Version: 1.6
 Summary: A battle cats save file editor korean version
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: cintagramabp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sc-editor-1.5/README.md` & `sc-editor-1.6/README.md`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/setup.py` & `sc-editor-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
 setuptools.setup(
     name="sc-editor",
-    version="1.5",
+    version="1.6",
     author="cintagramabp",
     description="A battle cats save file editor korean version",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fieryhenry/BCSFE-Python",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `sc-editor-1.5/src/SC_Editor/__main__.py` & `sc-editor-1.6/src/SC_Editor/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,21 +369,21 @@
 # 1: value name
 select_config_path=Select the config file path
 enabled=Enabled
 disabled=Disabled
 
     """
     localesdir = os.path.join(os.path.join(helper.get_local_files_path(), "locales"), "en")
-    with open(localesdir+"main.properties", "w+", encoding="utf-8") as main_properties:
+    with open(os.path.join(localesdir, "main.properties"), "w+", encoding="utf-8") as main_properties:
         main_properties.write(main_properties_string)
-    with open(localesdir+"item.properties", "w+", encoding="utf-8") as item_properties:
+    with open(os.path.join(localesdir, "item.properties"), "w+", encoding="utf-8") as item_properties:
         main_properties.write(item_properties_string)
-    with open(localesdir+"config.properties", "w+", encoding="utf-8") as config_properties:
+    with open(os.path.join(localesdir, "config.properties"), "w+", encoding="utf-8") as config_properties:
         main_properties.write(config_properties_string)
-    with open(localesdir+"user_input.properties", "w+", encoding="utf-8") as user_input_properties:
+    with open(os.path.join(localesdir, "user_input.properties"), "w+", encoding="utf-8") as user_input_properties:
         main_properties.write(user_input_properties_string)
 
     try:
         main()
     except KeyboardInterrupt:
         sys.exit()
     except Exception as e:  # pylint: disable=broad-except
```

### Comparing `sc-editor-1.5/src/SC_Editor/adb_handler.py` & `sc-editor-1.6/src/SC_Editor/adb_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/config_manager.py` & `sc-editor-1.6/src/SC_Editor/config_manager.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/csv_handler.py` & `sc-editor-1.6/src/SC_Editor/csv_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/basic/basic_items.py` & `sc-editor-1.6/src/SC_Editor/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/basic/catfruit.py` & `sc-editor-1.6/src/SC_Editor/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/basic/catseyes.py` & `sc-editor-1.6/src/SC_Editor/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/basic/ototo_base_mats.py` & `sc-editor-1.6/src/SC_Editor/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/basic/talent_orbs.py` & `sc-editor-1.6/src/SC_Editor/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/basic/talent_orbs_new.py` & `sc-editor-1.6/src/SC_Editor/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/cats/cat_helper.py` & `sc-editor-1.6/src/SC_Editor/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/cats/cat_id_selector.py` & `sc-editor-1.6/src/SC_Editor/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/cats/chara_drop.py` & `sc-editor-1.6/src/SC_Editor/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/cats/clear_cat_guide.py` & `sc-editor-1.6/src/SC_Editor/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/cats/evolve_cats.py` & `sc-editor-1.6/src/SC_Editor/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/cats/get_remove_cats.py` & `sc-editor-1.6/src/SC_Editor/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/cats/talents.py` & `sc-editor-1.6/src/SC_Editor/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/cats/upgrade_blue.py` & `sc-editor-1.6/src/SC_Editor/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/cats/upgrade_cats.py` & `sc-editor-1.6/src/SC_Editor/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/gamototo/gamatoto_xp.py` & `sc-editor-1.6/src/SC_Editor/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/gamototo/helpers.py` & `sc-editor-1.6/src/SC_Editor/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py` & `sc-editor-1.6/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/aku.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/behemoth_culling.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/clear_tutorial.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/enigma_stages.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/event_stages.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/gauntlet.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/itf_timed_scores.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/legend_quest.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/main_story.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/outbreaks.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/story_level_id_selector.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/towers.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/treasures.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/uncanny.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/levels/unlock_aku_realm.py` & `sc-editor-1.6/src/SC_Editor/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/cat_shrine.py` & `sc-editor-1.6/src/SC_Editor/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/claim_user_rank_rewards.py` & `sc-editor-1.6/src/SC_Editor/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/create_new_account.py` & `sc-editor-1.6/src/SC_Editor/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/fix_elsewhere.py` & `sc-editor-1.6/src/SC_Editor/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/fix_time_issues.py` & `sc-editor-1.6/src/SC_Editor/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/get_gold_pass.py` & `sc-editor-1.6/src/SC_Editor/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/meow_medals.py` & `sc-editor-1.6/src/SC_Editor/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/missions.py` & `sc-editor-1.6/src/SC_Editor/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/play_time.py` & `sc-editor-1.6/src/SC_Editor/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/scheme_item.py` & `sc-editor-1.6/src/SC_Editor/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/trade_progress.py` & `sc-editor-1.6/src/SC_Editor/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/other/unlock_enemy_guide.py` & `sc-editor-1.6/src/SC_Editor/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/save_management/convert.py` & `sc-editor-1.6/src/SC_Editor/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/save_management/load.py` & `sc-editor-1.6/src/SC_Editor/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/save_management/other.py` & `sc-editor-1.6/src/SC_Editor/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/save_management/save.py` & `sc-editor-1.6/src/SC_Editor/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/edits/save_management/server_upload.py` & `sc-editor-1.6/src/SC_Editor/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/feature_handler.py` & `sc-editor-1.6/src/SC_Editor/feature_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/game_data_getter.py` & `sc-editor-1.6/src/SC_Editor/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/helper.py` & `sc-editor-1.6/src/SC_Editor/helper.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/item.py` & `sc-editor-1.6/src/SC_Editor/item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/locale_handler.py` & `sc-editor-1.6/src/SC_Editor/locale_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/managed_item.py` & `sc-editor-1.6/src/SC_Editor/managed_item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/parse_save.py` & `sc-editor-1.6/src/SC_Editor/parse_save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/patcher.py` & `sc-editor-1.6/src/SC_Editor/patcher.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/root_handler.py` & `sc-editor-1.6/src/SC_Editor/root_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/serialise_save.py` & `sc-editor-1.6/src/SC_Editor/serialise_save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/server_handler.py` & `sc-editor-1.6/src/SC_Editor/server_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/updater.py` & `sc-editor-1.6/src/SC_Editor/updater.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/user_info.py` & `sc-editor-1.6/src/SC_Editor/user_info.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/SC_Editor/user_input_handler.py` & `sc-editor-1.6/src/SC_Editor/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.5/src/sc_editor.egg-info/PKG-INFO` & `sc-editor-1.6/src/sc_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-editor
-Version: 1.5
+Version: 1.6
 Summary: A battle cats save file editor korean version
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: cintagramabp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sc-editor-1.5/src/sc_editor.egg-info/SOURCES.txt` & `sc-editor-1.6/src/sc_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

