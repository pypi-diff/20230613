# Comparing `tmp/vedro-1.9.0.tar.gz` & `tmp/vedro-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-1.9.0.tar", last modified: Sun May 14 18:00:25 2023, max compression
+gzip compressed data, was "vedro-1.9.1.tar", last modified: Tue Jun 13 15:47:18 2023, max compression
```

## Comparing `vedro-1.9.0.tar` & `vedro-1.9.1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 18:00:11.000000 vedro-1.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-14 18:00:25.090307 vedro-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-14 18:00:11.000000 vedro-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-14 18:00:25.094307 vedro-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-14 18:00:11.000000 vedro-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.058306 vedro-1.9.0/vedro/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.058306 vedro-1.9.0/vedro/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/_cmd_arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.062306 vedro-1.9.0/vedro/commands/plugin_command/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/_fetch_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/_get_plugin_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/_install_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/_plugin_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.062306 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.062306 vedro-1.9.0/vedro/commands/run_command/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/run_command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/run_command/_run_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.066306 vedro-1.9.0/vedro/commands/version_command/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/version_command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/commands/version_command/_version_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.066306 vedro-1.9.0/vedro/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.070306 vedro-1.9.0/vedro/core/_config_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_config_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_config_loader/_config_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_config_loader/_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_config_loader/_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_exc_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.070306 vedro-1.9.0/vedro/core/_module_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_module_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_module_loader/_module_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_module_loader/_module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.070306 vedro-1.9.0/vedro/core/_scenario_discoverer/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_discoverer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_discoverer/_create_vscenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_discoverer/_multi_scenario_discoverer.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_discoverer/_scenario_discoverer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.070306 vedro-1.9.0/vedro/core/_scenario_finder/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_any_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_dunder_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_ext_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_hidden_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_scenario_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_finder/_scenario_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_loader/_scenario_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_loader/_scenario_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_orderer/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_orderer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_result/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_result/_aggregated_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_result/_scenario_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_result/_scenario_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.074307 vedro-1.9.0/vedro/core/_scenario_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_scenario_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_step_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_virtual_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/_virtual_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/core/scenario_orderer/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_orderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_orderer/_plain_scenario_orderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_orderer/_scenario_orderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_orderer/_stable_scenario_orderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/core/scenario_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_runner/_interrupted.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_runner/_monotonic_scenario_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_runner/_scenario_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/core/scenario_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_scheduler/_monotonic_scenario_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/core/scenario_scheduler/_scenario_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/events/
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/plugins/artifacted/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/artifacted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/artifacted/_artifacted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/plugins/assert_rewriter/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/assert_rewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/assert_rewriter/_assert_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/assert_rewriter/_scenario_assert_rewriter_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.078307 vedro-1.9.0/vedro/plugins/deferrer/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/deferrer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/deferrer/_deferrer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/director/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/_director.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/_director_init_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/director/pycharm/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/pycharm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/pycharm/_pycharm_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/director/rich/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/rich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/rich/_rich_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/rich/_rich_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/director/silent/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/silent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/director/silent/_silent_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/dry_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/dry_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/dry_runner/_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/dry_runner/_dry_runner_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.082306 vedro-1.9.0/vedro/plugins/interrupter/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/interrupter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/interrupter/_interrupter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/orderer/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/orderer_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/random_orderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/reversed_orderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/orderer/stable_orderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/repeater/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/repeater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/repeater/_repeater.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/repeater/_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/rerunner/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/rerunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/rerunner/_rerunner.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/rerunner/_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/seeder/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/seeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/seeder/_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/seeder/_seeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.086307 vedro-1.9.0/vedro/plugins/skipper/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/_only.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/_skip_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/skipper/_skipper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/vedro/plugins/slicer/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/slicer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/slicer/_slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/vedro/plugins/system_upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/system_upgrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/system_upgrade/_system_upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/vedro/plugins/tagger/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/tagger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/tagger/_tagger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.090307 vedro-1.9.0/vedro/plugins/terminator/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/terminator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/plugins/terminator/_terminator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:12.000000 vedro-1.9.0/vedro/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:00:25.058306 vedro-1.9.0/vedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-14 18:00:25.000000 vedro-1.9.0/vedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 18:00:24.000000 vedro-1.9.0/vedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.664957 vedro-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 15:47:04.000000 vedro-1.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-13 15:47:18.664957 vedro-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-13 15:47:04.000000 vedro-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-13 15:47:18.664957 vedro-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-13 15:47:04.000000 vedro-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.648957 vedro-1.9.1/vedro/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.648957 vedro-1.9.1/vedro/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/_cmd_arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.648957 vedro-1.9.1/vedro/commands/plugin_command/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/_fetch_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/_get_plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/_install_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/_plugin_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.648957 vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_config_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_config_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.648957 vedro-1.9.1/vedro/commands/run_command/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/run_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/run_command/_run_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.648957 vedro-1.9.1/vedro/commands/version_command/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/version_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/commands/version_command/_version_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.652957 vedro-1.9.1/vedro/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.652957 vedro-1.9.1/vedro/core/_config_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_config_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_config_loader/_config_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_config_loader/_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_config_loader/_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_exc_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.652957 vedro-1.9.1/vedro/core/_module_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_module_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_module_loader/_module_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_module_loader/_module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.652957 vedro-1.9.1/vedro/core/_scenario_discoverer/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_discoverer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_discoverer/_create_vscenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_discoverer/_multi_scenario_discoverer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_discoverer/_scenario_discoverer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.652957 vedro-1.9.1/vedro/core/_scenario_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_finder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.652957 vedro-1.9.1/vedro/core/_scenario_finder/_file_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_finder/_file_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_finder/_file_filters/_any_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_finder/_file_filters/_dunder_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_finder/_file_filters/_ext_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_finder/_file_filters/_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_finder/_file_filters/_hidden_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_finder/_scenario_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_finder/_scenario_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.652957 vedro-1.9.1/vedro/core/_scenario_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_loader/_scenario_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_loader/_scenario_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/core/_scenario_orderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_orderer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/core/_scenario_result/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_result/_aggregated_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_result/_scenario_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_result/_scenario_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/core/_scenario_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/core/_scenario_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_scenario_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_virtual_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/_virtual_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/core/scenario_orderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_orderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_orderer/_plain_scenario_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_orderer/_scenario_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_orderer/_stable_scenario_orderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/core/scenario_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_runner/_interrupted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_runner/_monotonic_scenario_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_runner/_scenario_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/core/scenario_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_scheduler/_monotonic_scenario_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/core/scenario_scheduler/_scenario_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/plugins/artifacted/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/artifacted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/artifacted/_artifacted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/plugins/assert_rewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/assert_rewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/assert_rewriter/_assert_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/assert_rewriter/_scenario_assert_rewriter_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.656957 vedro-1.9.1/vedro/plugins/deferrer/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/deferrer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/deferrer/_deferrer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/director/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/_director.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/_director_init_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/director/pycharm/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/pycharm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/pycharm/_pycharm_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/director/rich/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/rich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/rich/_rich_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12996 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/rich/_rich_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/director/silent/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/silent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/director/silent/_silent_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/dry_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/dry_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/dry_runner/_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/dry_runner/_dry_runner_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/interrupter/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/interrupter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/interrupter/_interrupter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/orderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/orderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/orderer/orderer_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/orderer/random_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/orderer/reversed_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/orderer/stable_orderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/repeater/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/repeater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/repeater/_repeater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/repeater/_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/rerunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/rerunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/rerunner/_rerunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/rerunner/_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.660957 vedro-1.9.1/vedro/plugins/seeder/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/seeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/seeder/_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/seeder/_seeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.664957 vedro-1.9.1/vedro/plugins/skipper/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/skipper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/skipper/_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/skipper/_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/skipper/_skip_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/skipper/_skipper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.664957 vedro-1.9.1/vedro/plugins/slicer/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/slicer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/slicer/_slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.664957 vedro-1.9.1/vedro/plugins/system_upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/system_upgrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/system_upgrade/_system_upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.664957 vedro-1.9.1/vedro/plugins/tagger/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/tagger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/tagger/_tagger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.664957 vedro-1.9.1/vedro/plugins/terminator/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/terminator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/plugins/terminator/_terminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:04.000000 vedro-1.9.1/vedro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:47:18.648957 vedro-1.9.1/vedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-13 15:47:18.000000 vedro-1.9.1/vedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-06-13 15:47:18.000000 vedro-1.9.1/vedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:47:18.000000 vedro-1.9.1/vedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 15:47:18.000000 vedro-1.9.1/vedro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 15:47:18.000000 vedro-1.9.1/vedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 15:47:18.000000 vedro-1.9.1/vedro.egg-info/top_level.txt
```

### Comparing `vedro-1.9.0/LICENSE.txt` & `vedro-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/PKG-INFO` & `vedro-1.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vedro
-Version: 1.9.0
+Version: 1.9.1
 Summary: Pragmatic BDD Framework
 Home-page: https://github.com/tsv1/vedro
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/
 Project-URL: GitHub, https://github.com/tsv1/vedro
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Vedro
```

### Comparing `vedro-1.9.0/README.md` & `vedro-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/setup.cfg` & `vedro-1.9.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.9.0
+current_version = 1.9.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-1.9.0/setup.py` & `vedro-1.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro",
-    version="1.9.0",
+    version="1.9.1",
     description="Pragmatic BDD Framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
     url="https://github.com/tsv1/vedro",
@@ -30,18 +30,18 @@
     package_data={"vedro": ["py.typed"]},
     entry_points={
         "console_scripts": ["vedro = vedro:run"],
     },
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
-        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development",
         "Typing :: Typed",
     ],
 )
```

### Comparing `vedro-1.9.0/vedro/__init__.py` & `vedro-1.9.1/vedro/__init__.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/_config.py` & `vedro-1.9.1/vedro/_config.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/_main.py` & `vedro-1.9.1/vedro/_main.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/_params.py` & `vedro-1.9.1/vedro/_params.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/_scenario.py` & `vedro-1.9.1/vedro/_scenario.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/_cmd_arg_parser.py` & `vedro-1.9.1/vedro/commands/_cmd_arg_parser.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/plugin_command/_fetch_plugins.py` & `vedro-1.9.1/vedro/commands/plugin_command/_fetch_plugins.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/plugin_command/_get_plugin_info.py` & `vedro-1.9.1/vedro/commands/plugin_command/_get_plugin_info.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/plugin_command/_install_plugin.py` & `vedro-1.9.1/vedro/commands/plugin_command/_install_plugin.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/plugin_command/_plugin_command.py` & `vedro-1.9.1/vedro/commands/plugin_command/_plugin_command.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_generator.py` & `vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_config_generator.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_markup.py` & `vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_config_markup.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_parser.py` & `vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_config_parser.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_config_updater.py` & `vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_config_updater.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/plugin_command/plugin_manager/_plugin_manager.py` & `vedro-1.9.1/vedro/commands/plugin_command/plugin_manager/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/run_command/_run_command.py` & `vedro-1.9.1/vedro/commands/run_command/_run_command.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/commands/version_command/_version_command.py` & `vedro-1.9.1/vedro/commands/version_command/_version_command.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/__init__.py` & `vedro-1.9.1/vedro/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_artifacts.py` & `vedro-1.9.1/vedro/core/_artifacts.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_config_loader/_config_file_loader.py` & `vedro-1.9.1/vedro/core/_config_loader/_config_file_loader.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_config_loader/_config_type.py` & `vedro-1.9.1/vedro/core/_config_loader/_config_type.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_container.py` & `vedro-1.9.1/vedro/core/_container.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_dispatcher.py` & `vedro-1.9.1/vedro/core/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_event.py` & `vedro-1.9.1/vedro/core/_event.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_module_loader/_module_file_loader.py` & `vedro-1.9.1/vedro/core/_module_loader/_module_file_loader.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_plugin.py` & `vedro-1.9.1/vedro/core/_plugin.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_report.py` & `vedro-1.9.1/vedro/core/_report.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_scenario_discoverer/_create_vscenario.py` & `vedro-1.9.1/vedro/core/_scenario_discoverer/_create_vscenario.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_scenario_discoverer/_multi_scenario_discoverer.py` & `vedro-1.9.1/vedro/core/_scenario_discoverer/_multi_scenario_discoverer.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_scenario_discoverer/_scenario_discoverer.py` & `vedro-1.9.1/vedro/core/_scenario_discoverer/_scenario_discoverer.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_scenario_finder/_file_filters/_ext_filter.py` & `vedro-1.9.1/vedro/core/_scenario_finder/_file_filters/_ext_filter.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_scenario_finder/_scenario_file_finder.py` & `vedro-1.9.1/vedro/core/_scenario_finder/_scenario_file_finder.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_scenario_loader/_scenario_file_loader.py` & `vedro-1.9.1/vedro/core/_scenario_loader/_scenario_file_loader.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_scenario_result/_aggregated_result.py` & `vedro-1.9.1/vedro/core/_scenario_result/_aggregated_result.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_scenario_result/_scenario_result.py` & `vedro-1.9.1/vedro/core/_scenario_result/_scenario_result.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_step_result.py` & `vedro-1.9.1/vedro/core/_step_result.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_virtual_scenario.py` & `vedro-1.9.1/vedro/core/_virtual_scenario.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/_virtual_step.py` & `vedro-1.9.1/vedro/core/_virtual_step.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/scenario_orderer/_stable_scenario_orderer.py` & `vedro-1.9.1/vedro/core/scenario_orderer/_stable_scenario_orderer.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/scenario_runner/_interrupted.py` & `vedro-1.9.1/vedro/core/scenario_runner/_interrupted.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/scenario_runner/_monotonic_scenario_runner.py` & `vedro-1.9.1/vedro/core/scenario_runner/_monotonic_scenario_runner.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/scenario_scheduler/_monotonic_scenario_scheduler.py` & `vedro-1.9.1/vedro/core/scenario_scheduler/_monotonic_scenario_scheduler.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/core/scenario_scheduler/_scenario_scheduler.py` & `vedro-1.9.1/vedro/core/scenario_scheduler/_scenario_scheduler.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/events/__init__.py` & `vedro-1.9.1/vedro/events/__init__.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/artifacted/_artifacted.py` & `vedro-1.9.1/vedro/plugins/artifacted/_artifacted.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/assert_rewriter/_assert_rewriter.py` & `vedro-1.9.1/vedro/plugins/assert_rewriter/_assert_rewriter.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/deferrer/_deferrer.py` & `vedro-1.9.1/vedro/plugins/deferrer/_deferrer.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/director/__init__.py` & `vedro-1.9.1/vedro/plugins/director/__init__.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/director/_director.py` & `vedro-1.9.1/vedro/plugins/director/_director.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/director/_director_init_event.py` & `vedro-1.9.1/vedro/plugins/director/_director_init_event.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/director/pycharm/_pycharm_reporter.py` & `vedro-1.9.1/vedro/plugins/director/pycharm/_pycharm_reporter.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/director/rich/_rich_printer.py` & `vedro-1.9.1/vedro/plugins/director/rich/_rich_printer.py`

 * *Files 10% similar despite different names*

```diff
@@ -135,35 +135,46 @@
             self.__filter_locals(trace)
 
         tb = self._traceback_factory(trace, max_frames=max_frames, word_wrap=word_wrap)
         self._console.print(tb)
         self.print_empty_line()
 
     def pretty_format(self, value: Any) -> Any:
+        if hasattr(value, "__rich__") or hasattr(value, "__rich_console__"):
+            return value
         try:
             return json.dumps(value, ensure_ascii=False, indent=4)
         except BaseException:
             return repr(value)
 
-    def print_scope(self, scope: Dict[str, Any]) -> None:
+    def print_scope(self, scope: Dict[str, Any], scope_width: Union[int, None] = None) -> None:
         self.print_scope_header("Scope")
         for key, val in scope.items():
             self.print_scope_key(key, indent=1)
-            self.print_scope_val(self.pretty_format(val))
+            self.print_scope_val(self.pretty_format(val), scope_width)
         self.print_empty_line()
 
     def print_scope_header(self, title: str) -> None:
         self._console.out(title, style=Style(color="blue", bold=True))
 
     def print_scope_key(self, key: str, *, indent: int = 0, line_break: bool = False) -> None:
         prepend = " " * indent
         end = "\n" if line_break else ""
         self._console.out(f"{prepend}{key}: ", end=end, style=Style(color="blue"))
 
-    def print_scope_val(self, val: Any) -> None:
+    def __truncate_line(self, line: str, width: int, separator: str = "...") -> str:
+        if len(line) <= width:
+            return line
+        width -= len(separator)
+        return line[:width // 2] + separator + line[-width // 2:]
+
+    def print_scope_val(self, val: Any, scope_width: Union[int, None] = None) -> None:
+        if isinstance(val, str) and (scope_width is None or scope_width > 0):
+            width = scope_width or self._console.size.width
+            val = os.linesep.join(self.__truncate_line(line, width) for line in val.splitlines())
         self._console.print(val)
 
     def print_interrupted(self, exc_info: ExcInfo, *, show_traceback: bool = False) -> None:
         message = f"!!! Interrupted by “{exc_info.value!r}“ !!!"
         spaces = " " * (len(message) - 6)
         multiline_message = "\n".join([
             "!!!" + spaces + "!!!",
```

### Comparing `vedro-1.9.0/vedro/plugins/director/rich/_rich_reporter.py` & `vedro-1.9.1/vedro/plugins/director/rich/_rich_reporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
                  printer_factory: Callable[[], RichPrinter] = RichPrinter) -> None:
         super().__init__(config)
         self._printer = printer_factory()
         self._verbosity = 0
         self._tb_pretty = config.tb_pretty
         self._tb_show_internal_calls = config.tb_show_internal_calls
         self._tb_show_locals = config.tb_show_locals
+        self._scope_width = config.scope_width
         self._tb_max_frames = config.tb_max_frames
         self._show_skipped = config.show_skipped
         self._show_timings = config.show_timings
         self._show_paths = config.show_paths
         self._show_steps = config.show_steps
         self._hide_namespaces = config.hide_namespaces
         self._show_scenario_spinner = config.show_scenario_spinner
@@ -177,15 +178,15 @@
         if self._verbosity > 1:
             for step_result in scenario_result.step_results:
                 if step_result.exc_info:
                     self._print_exception(step_result.exc_info)
 
         if self._verbosity > 2:
             if scenario_result.scope:
-                self._printer.print_scope(scenario_result.scope)
+                self._printer.print_scope(scenario_result.scope, scope_width=self._scope_width)
 
     def _print_scenario_skipped(self, scenario_result: ScenarioResult, *,
                                 prefix: str = "") -> None:
         if not self._show_skipped:
             return
         elapsed = scenario_result.elapsed if self._show_timings else None
         self._printer.print_scenario_subject(scenario_result.scenario.subject,
@@ -265,14 +266,20 @@
     # Show internal calls in the traceback output
     tb_show_internal_calls: bool = False
 
     # Show local variables in the traceback output
     # Available if tb_pretty is True
     tb_show_locals: bool = False
 
+    # Truncate lines in Scope based on scope_width value.
+    # If scope_width is None, lines are truncated to the terminal's width.
+    # If scope_width is -1, lines aren't truncated.
+    # Otherwise, lines are truncated to the given length.
+    scope_width: Union[int, None] = None
+
     # Max stack trace entries to show (min=4)
     tb_max_frames: int = 8
 
     # Show traceback if the execution is interrupted
     show_interrupted_traceback: bool = False
 
     # Enable new verbose levels
```

### Comparing `vedro-1.9.0/vedro/plugins/director/silent/_silent_reporter.py` & `vedro-1.9.1/vedro/plugins/director/silent/_silent_reporter.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/dry_runner/_dry_runner.py` & `vedro-1.9.1/vedro/plugins/dry_runner/_dry_runner.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/dry_runner/_dry_runner_plugin.py` & `vedro-1.9.1/vedro/plugins/dry_runner/_dry_runner_plugin.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/interrupter/_interrupter.py` & `vedro-1.9.1/vedro/plugins/interrupter/_interrupter.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/orderer/orderer_plugin.py` & `vedro-1.9.1/vedro/plugins/orderer/orderer_plugin.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/repeater/_repeater.py` & `vedro-1.9.1/vedro/plugins/repeater/_repeater.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/repeater/_scheduler.py` & `vedro-1.9.1/vedro/plugins/repeater/_scheduler.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/rerunner/_rerunner.py` & `vedro-1.9.1/vedro/plugins/rerunner/_rerunner.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/rerunner/_scheduler.py` & `vedro-1.9.1/vedro/plugins/rerunner/_scheduler.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/seeder/_random.py` & `vedro-1.9.1/vedro/plugins/seeder/_random.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/seeder/_seeder.py` & `vedro-1.9.1/vedro/plugins/seeder/_seeder.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/skipper/_only.py` & `vedro-1.9.1/vedro/plugins/skipper/_only.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/skipper/_skip.py` & `vedro-1.9.1/vedro/plugins/skipper/_skip.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/skipper/_skip_if.py` & `vedro-1.9.1/vedro/plugins/skipper/_skip_if.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/skipper/_skipper.py` & `vedro-1.9.1/vedro/plugins/skipper/_skipper.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/slicer/_slicer.py` & `vedro-1.9.1/vedro/plugins/slicer/_slicer.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/system_upgrade/_system_upgrade.py` & `vedro-1.9.1/vedro/plugins/system_upgrade/_system_upgrade.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/tagger/_tagger.py` & `vedro-1.9.1/vedro/plugins/tagger/_tagger.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro/plugins/terminator/_terminator.py` & `vedro-1.9.1/vedro/plugins/terminator/_terminator.py`

 * *Files identical despite different names*

### Comparing `vedro-1.9.0/vedro.egg-info/PKG-INFO` & `vedro-1.9.1/vedro.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vedro
-Version: 1.9.0
+Version: 1.9.1
 Summary: Pragmatic BDD Framework
 Home-page: https://github.com/tsv1/vedro
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/
 Project-URL: GitHub, https://github.com/tsv1/vedro
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Vedro
```

### Comparing `vedro-1.9.0/vedro.egg-info/SOURCES.txt` & `vedro-1.9.1/vedro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

