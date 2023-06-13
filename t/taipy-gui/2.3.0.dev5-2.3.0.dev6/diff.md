# Comparing `tmp/taipy-gui-2.3.0.dev5.tar.gz` & `tmp/taipy-gui-2.3.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-gui-2.3.0.dev5.tar", last modified: Mon Jun 12 10:27:38 2023, max compression
+gzip compressed data, was "taipy-gui-2.3.0.dev6.tar", last modified: Tue Jun 13 17:34:24 2023, max compression
```

## Comparing `taipy-gui-2.3.0.dev5.tar` & `taipy-gui-2.3.0.dev6.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.793365 taipy-gui-2.3.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-12 10:27:38.793365 taipy-gui-2.3.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 10:27:38.793365 taipy-gui-2.3.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-12 10:23:21.000000 taipy-gui-2.3.0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.741365 taipy-gui-2.3.0.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.745365 taipy-gui-2.3.0.dev5/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.749365 taipy-gui-2.3.0.dev5/src/taipy/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/_gui_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/_gui_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.753365 taipy-gui-2.3.0.dev5/src/taipy/gui/data/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/array_dict_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/content_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/data_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.757365 taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/lttb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/minmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/rdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/scatter_decimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/numpy_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/pandas_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.757365 taipy-gui-2.3.0.dev5/src/taipy/gui/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/extension/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    91761 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/gui_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/partial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.757365 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.757365 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_html/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_html/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_html/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.761365 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/blocproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/postproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    41559 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.769365 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_locals_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_map_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_runtime_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_variable_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/chart_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/clientvarname.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/expr_var_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/filename.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/filter_locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/get_imported_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/get_module_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/getdatecolstrname.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/is_debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/isnotebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/table_col_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/utils/varnamefromcontent.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/version.json
--rw-r--r--   0 runner    (1001) docker     (123)    56258 2023-06-12 10:23:11.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/viselements.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.785365 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-12 10:26:48.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/227.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)   204350 2023-06-12 10:26:48.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/499.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)  3591394 2023-06-12 10:26:48.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/660.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-12 10:26:48.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.785365 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.789365 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/base/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/base/fontfaces.css
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/base/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.789365 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/blocks/layout.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.789365 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/button.css
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/date.css
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/expandable.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/image.css
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/input.css
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/navbar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/number.css
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/selector.css
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/slider.css
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/table.css
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/toggle.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.789365 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/elements/card.css
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/elements/container.css
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/elements/header.css
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/elements/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/stylekit.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.789365 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/utilities/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/utilities/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/utilities/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/utilities/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.789365 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/elements.css
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/shapes.css
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/typography.css
--rw-r--r--   0 runner    (1001) docker     (123)   218114 2023-06-12 10:24:37.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)  5259716 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui-deps.dll.js
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-12 10:24:37.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui-dom.js
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)  1085147 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-12 10:26:48.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 10:27:30.000000 taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy.status.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:27:38.793365 taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-12 10:27:38.000000 taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-06-12 10:27:38.000000 taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:27:38.000000 taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:27:31.000000 taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-12 10:27:38.000000 taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 10:27:38.000000 taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-13 17:29:30.000000 taipy-gui-2.3.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.625065 taipy-gui-2.3.0.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.629065 taipy-gui-2.3.0.dev6/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.629065 taipy-gui-2.3.0.dev6/src/taipy/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_gui_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_gui_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/array_dict_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/content_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/lttb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/scatter_decimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/numpy_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/pandas_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/extension/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91973 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/gui_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/partial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/blocproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/postproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41559 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.637065 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_locals_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_map_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_runtime_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_variable_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/chart_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/clientvarname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/expr_var_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/filter_locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/get_imported_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/get_module_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/getdatecolstrname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/is_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/isnotebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/table_col_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/varnamefromcontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56258 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/viselements.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.653065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/227.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)   204350 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/499.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3591394 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/660.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.653065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.653065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/fontfaces.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.653065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/blocks/layout.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/button.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/date.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/expandable.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/image.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/number.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/selector.css
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/toggle.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/card.css
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/container.css
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/header.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/stylekit.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/elements.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/shapes.css
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/typography.css
+-rw-r--r--   0 runner    (1001) docker     (123)   218114 2023-06-13 17:30:57.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5259716 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps.dll.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-13 17:30:57.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-dom.js
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)  1085147 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy.status.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:34:14.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/top_level.txt
```

### Comparing `taipy-gui-2.3.0.dev5/LICENSE` & `taipy-gui-2.3.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/PKG-INFO` & `taipy-gui-2.3.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.3.0.dev5
+Version: 2.3.0.dev6
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-gui-2.3.0.dev5/README.md` & `taipy-gui-2.3.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/setup.py` & `taipy-gui-2.3.0.dev6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "python-dotenv>=0.19,<0.21",
     "pytz>=2021.3,<2022.2",
     "tzlocal>=3.0,<5.0",
     "backports.zoneinfo>=0.2.1,<0.3;python_version<'3.9'",
     "gevent>=22.10.2,<23.0",
     "gevent-websocket>=0.10.1,<0.11",
     "kthread>=0.2.3,<0.3",
-    "taipy-config==2.3.0.dev2",
+    "taipy-config==2.3.0.dev3",
     "gitignore-parser>=0.1,<0.2",
     "simple-websocket>=0.9,<1.0",
     "twisted>=22.10",
 ]
 
 test_requirements = ["pytest>=3.8"]
```

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/__init__.py` & `taipy-gui-2.3.0.dev6/src/taipy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,17 @@
         from taipy.core.task.task import Task
         from taipy.core.task.task_id import TaskId
 
     if find_spec("taipy.gui"):
         from taipy.gui import Gui
 
         if find_spec("taipy.gui_core"):
-            from taipy.gui_core.GuiCoreLib import GuiCore
+            from taipy.gui_core.GuiCoreLib import _GuiCore
 
-            Gui.add_library(GuiCore())
+            Gui.add_library(_GuiCore())
 
         if find_spec("taipy.enterprise") and find_spec("taipy.enterprise.gui"):
             from taipy.enterprise.gui import _init_gui_enterprise
 
             _init_gui_enterprise(Gui)
 
     if find_spec("taipy.rest"):
```

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/__init__.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/_default_config.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/_default_config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/_gui_cli.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/_gui_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/_gui_section.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/_gui_section.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/_page.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/_page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/config.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/__init__.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/array_dict_data_accessor.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/array_dict_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/content_accessor.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/content_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/data_accessor.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/data_format.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_format.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/data_scope.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_scope.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/__init__.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/lttb.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/lttb.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/minmax.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/minmax.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/rdp.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/rdp.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/decimator/scatter_decimator.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/scatter_decimator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/numpy_data_accessor.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/numpy_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/pandas_data_accessor.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/pandas_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/data/utils.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/data/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/extension/__init__.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/extension/library.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/extension/library.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/gui.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1677,18 +1677,22 @@
 
     def _register_data_accessor(self, data_accessor_class: t.Type[_DataAccessor]) -> None:
         self._accessors._register(data_accessor_class)
 
     def get_flask_app(self) -> Flask:
         """Get the internal Flask application.
 
+        This method must be called **after** (Gui.)run^ method was invoked.
+
         Returns:
             The Flask instance used.
         """
-        return self._server.get_flask()
+        if hasattr(self, "_server"):
+            return self._server.get_flask()
+        raise RuntimeError("get_flask_app() cannot be invoked before run() has been called.")
 
     def _set_frame(self, frame: FrameType):
         if not isinstance(frame, FrameType):  # pragma: no cover
             raise RuntimeError("frame must be a FrameType where Gui can collect the local variables.")
         self.__frame = frame
         self.__default_module_name = _get_module_name_from_frame(self.__frame)
```

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/gui_actions.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/gui_actions.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/icon.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/icon.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/page.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/partial.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/partial.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/__init__.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_html/__init__.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_html/factory.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_html/parser.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/parser.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/__init__.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/blocproc.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/blocproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/control.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/control.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/factory.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/postproc.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/postproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/_markdown/preproc.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/preproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/builder.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/factory.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/json.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/json.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/renderers/utils.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/server.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/server.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/state.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/state.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/types.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/types.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/__init__.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_adapter.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,31 +56,34 @@
 
     def _get_elt_per_ids(self, var_name: str, lov: t.List[t.Any]) -> t.Dict[str, t.Any]:
         dict_res = {}
         adapter = self.__get_for_var(var_name, lov[0] if lov else None)
         for value in lov:
             try:
                 result = adapter(value._dict if isinstance(value, _MapDict) else value) if adapter else value
-                dict_res[self.__get_id(result)] = value
-                children = self.__get_children(result)
-                if children is not None:
-                    dict_res.update(self._get_elt_per_ids(var_name, children))
+                if result is not None:
+                    dict_res[self.__get_id(result)] = value
+                    children = self.__get_children(result)
+                    if children is not None:
+                        dict_res.update(self._get_elt_per_ids(var_name, children))
             except Exception as e:
                 _warn(f"Cannot run adapter for {var_name}:\n{e}")
         return dict_res
 
     def _run(
         self, adapter: t.Optional[t.Callable], value: t.Any, var_name: str, id_only=False
     ) -> t.Union[t.Tuple[str, ...], str, None]:
         if value is None:
             return None
         try:
             result = value._dict if isinstance(value, _MapDict) else value
             if adapter:
                 result = adapter(result)
+                if result is None:
+                    return result
             elif isinstance(result, str):
                 return result
             tpl_res = self._get_valid_result(result, id_only)
             if tpl_res is None:
                 _warn(
                     f"Adapter for {var_name} did not return a valid result. Please check the documentation on List of Values Adapters."
                 )
```

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_attributes.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_attributes.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_bindings.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_bindings.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_evaluator.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_evaluator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_locals_context.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_locals_context.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_map_dict.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_map_dict.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_runtime_manager.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_runtime_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/_variable_directory.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_variable_directory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/boolean.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/boolean.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/chart_config_builder.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/chart_config_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/clientvarname.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/clientvarname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/datatype.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/date.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/date.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/expr_var_name.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/expr_var_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/filename.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/filename.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/filter_locals.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/filter_locals.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/get_imported_var.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/get_imported_var.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/get_module_name.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/get_module_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/getdatecolstrname.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/getdatecolstrname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/html.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/html.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/is_debugging.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/is_debugging.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/isnotebook.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/isnotebook.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/proxy.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/singleton.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/table_col_builder.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/table_col_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/types.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/types.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/utils/varnamefromcontent.py` & `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/varnamefromcontent.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/viselements.json` & `taipy-gui-2.3.0.dev6/src/taipy/gui/viselements.json`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/227.taipy-gui.js` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/227.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/499.taipy-gui.js` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/499.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/660.taipy-gui.js` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/660.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/favicon.ico` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/favicon.ico`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/favicon.png` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/favicon.png`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/index.html` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/index.html`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/base/base.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/base.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/base/fontfaces.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/fontfaces.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/base/typography.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/blocks/layout.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/blocks/layout.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/button.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/button.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/chart.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/chart.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/date.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/date.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/expandable.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/expandable.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/image.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/image.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/input.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/input.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/navbar.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/navbar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/number.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/number.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/selector.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/selector.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/slider.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/slider.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/table.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/table.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/controls/toggle.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/toggle.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/elements/card.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/card.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/elements/container.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/container.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/elements/header.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/header.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/elements/sidebar.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/sidebar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/stylekit.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/stylekit.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/utilities/colors.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/utilities/misc.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/utilities/spacing.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/utilities/typography.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/colors.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/elements.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/elements.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/misc.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/shapes.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/shapes.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/spacing.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/stylekit/variables/typography.css` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui-deps-manifest.json` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps-manifest.json`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui-deps.dll.js` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps.dll.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui-dom.js` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-dom.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui.d.ts` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.d.ts`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui.js` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt` & `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/PKG-INFO` & `taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.3.0.dev5
+Version: 2.3.0.dev6
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/SOURCES.txt` & `taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev5/src/taipy_gui.egg-info/requires.txt` & `taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 pandas<2.0,>=1.5.1
 python-dotenv<0.21,>=0.19
 pytz<2022.2,>=2021.3
 tzlocal<5.0,>=3.0
 gevent<23.0,>=22.10.2
 gevent-websocket<0.11,>=0.10.1
 kthread<0.3,>=0.2.3
-taipy-config==2.3.0.dev2
+taipy-config==2.3.0.dev3
 gitignore-parser<0.2,>=0.1
 simple-websocket<1.0,>=0.9
 twisted>=22.10
 
 [:python_version < "3.9"]
 backports.zoneinfo<0.3,>=0.2.1
```

