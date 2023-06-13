# Comparing `tmp/sciqlop-0.4.0.tar.gz` & `tmp/sciqlop-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciqlop-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sciqlop-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sciqlop-0.4.0.tar` & `sciqlop-0.4.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    35147 2023-06-12 09:19:03.833722 sciqlop-0.4.0/COPYING
--rw-r--r--   0        0        0     4594 2023-06-12 09:19:03.833722 sciqlop-0.4.0/README.md
--rw-r--r--   0        0        0       23 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/__init__.py
--rw-r--r--   0        0        0     1276 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/app.py
--rw-r--r--   0        0        0     1510 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/__init__.py
--rw-r--r--   0        0        0      532 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/enums.py
--rw-r--r--   0        0        0      831 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/logging/__init__.py
--rw-r--r--   0        0        0      172 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/models.py
--rw-r--r--   0        0        0        1 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/pipelines_model/__init__.py
--rw-r--r--   0        0        0     5204 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/pipelines_model/auto_register.py
--rw-r--r--   0        0        0      128 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/pipelines_model/base/__init__.py
--rw-r--r--   0        0        0     6909 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/pipelines_model/base/model.py
--rw-r--r--   0        0        0     2925 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/pipelines_model/base/pipeline_node.py
--rw-r--r--   0        0        0     5352 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/pipelines_model/data_pipeline.py
--rw-r--r--   0        0        0      718 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/pipelines_model/data_provider.py
--rw-r--r--   0        0        0     3310 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/pipelines_model/easy_provider.py
--rw-r--r--   0        0        0     3820 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/pipelines_model/graph.py
--rw-r--r--   0        0        0        0 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/products_model/__init__.py
--rw-r--r--   0        0        0     6549 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/products_model/model.py
--rw-r--r--   0        0        0     3195 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/products_model/product_node.py
--rw-r--r--   0        0        0        0 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/resampling/__init__.py
--rw-r--r--   0        0        0     1365 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/resampling/spectro_regrid.py
--rw-r--r--   0        0        0      186 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/backend/unique_names.py
--rw-r--r--   0        0        0     1645 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/mime/__init__.py
--rw-r--r--   0        0        0      120 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/mime/types.py
--rw-r--r--   0        0        0     2279 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/__init__.py
--rw-r--r--   0        0        0      181 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/catalogs/__init__.py
--rw-r--r--   0        0        0     1555 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/catalogs/catalogs.py
--rw-r--r--   0        0        0     7828 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/__init__.py
--rw-r--r--   0        0        0    10334 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/catalog_selector.py
--rw-r--r--   0        0        0     1045 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/event.py
--rw-r--r--   0        0        0     3208 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/event_selector.py
--rw-r--r--   0        0        0     1060 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/event_span.py
--rw-r--r--   0        0        0     3906 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/speasy.py
--rw-r--r--   0        0        0     1419 2023-06-12 09:19:03.833722 sciqlop-0.4.0/SciQLop/plugins/test_plugin.py
--rw-r--r--   0        0        0   641256 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/__init__.py
--rw-r--r--   0        0        0     8256 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/MPL.png
--rw-r--r--   0        0        0    20841 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/QCP.png
--rw-r--r--   0        0        0   118794 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/SciQLop.png
--rw-r--r--   0        0        0     3191 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/Simple_icon_time.svg
--rw-r--r--   0        0        0     1956 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/add.png
--rw-r--r--   0        0        0     2001 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/allEvents.png
--rw-r--r--   0        0        0      615 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/catalogue.png
--rw-r--r--   0        0        0     1003 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/chart.png
--rw-r--r--   0        0        0     1047 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/cursor.png
--rw-r--r--   0        0        0     2150 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/dataSourceComponent.png
--rw-r--r--   0        0        0      882 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/dataSourceNode.png
--rw-r--r--   0        0        0     1213 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/dataSourceProduct.png
--rw-r--r--   0        0        0     4821 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/dataSourceRoot.png
--rw-r--r--   0        0        0      788 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/database.png
--rw-r--r--   0        0        0      834 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/delete.png
--rwxr-xr-x   0        0        0     1266 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/discard.png
--rw-r--r--   0        0        0     1231 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/down.png
--rw-r--r--   0        0        0     1731 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/drag.png
--rw-r--r--   0        0        0     4413 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/next.png
--rwxr-xr-x   0        0        0     1450 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/openInspector.png
--rw-r--r--   0        0        0     2319 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/plot.png
--rw-r--r--   0        0        0     2114 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/pointer.png
--rw-r--r--   0        0        0     4377 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/previous.png
--rw-r--r--   0        0        0     4841 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/rectangle.png
--rw-r--r--   0        0        0     1916 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/remove.png
--rw-r--r--   0        0        0    10041 2023-06-12 09:19:03.837722 sciqlop-0.4.0/SciQLop/resources/icons/satellite.svg
--rw-r--r--   0        0        0     1334 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/resources/icons/save.png
--rw-r--r--   0        0        0    85300 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/resources/icons/sciqlop2PNG_1024.png
--rw-r--r--   0        0        0     3714 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/resources/icons/time.png
--rw-r--r--   0        0        0     1084 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/resources/icons/trash.png
--rw-r--r--   0        0        0     2234 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/resources/icons/unplot.png
--rw-r--r--   0        0        0     1197 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/resources/icons/up.png
--rw-r--r--   0        0        0     4056 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/resources/icons/zoom.png
--rw-r--r--   0        0        0     1319 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/resources/resources.qrc
--rw-r--r--   0        0        0        0 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/__init__.py
--rw-r--r--   0        0        0     4161 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/central_widget.py
--rw-r--r--   0        0        0       31 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/common/__init__.py
--rw-r--r--   0        0        0     1005 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/common/tree_view.py
--rw-r--r--   0        0        0     2499 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/console.py
--rw-r--r--   0        0        0     3102 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/datetime_range.py
--rw-r--r--   0        0        0      157 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/drag_and_drop/__init__.py
--rw-r--r--   0        0        0      282 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/drag_and_drop/drop_handler.py
--rw-r--r--   0        0        0     2450 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/drag_and_drop/helper.py
--rw-r--r--   0        0        0     3120 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/drag_and_drop/place_holder_manager.py
--rw-r--r--   0        0        0     1134 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/drag_and_drop/placeholder.py
--rw-r--r--   0        0        0     4955 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/mainwindow.py
--rw-r--r--   0        0        0       39 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/pipelines/__init__.py
--rw-r--r--   0        0        0     2085 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/pipelines/pipeline_tree.py
--rw-r--r--   0        0        0        0 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/plots/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/plots/abstract_plot_panel.py
--rw-r--r--   0        0        0     3684 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/plots/colormap_graph.py
--rw-r--r--   0        0        0     1720 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/plots/line_graph.py
--rw-r--r--   0        0        0     5504 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/plots/mpl_panel.py
--rw-r--r--   0        0        0    10643 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/plots/time_series_plot.py
--rw-r--r--   0        0        0     2936 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/plots/time_span.py
--rw-r--r--   0        0        0     1201 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/plots/time_span_controller.py
--rw-r--r--   0        0        0     8234 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/plots/time_sync_panel.py
--rw-r--r--   0        0        0       39 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/products_tree/__init__.py
--rw-r--r--   0        0        0     1378 2023-06-12 09:19:03.841722 sciqlop-0.4.0/SciQLop/widgets/products_tree/products_tree.py
--rw-r--r--   0        0        0     1378 2023-06-12 09:19:03.845722 sciqlop-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5788 1970-01-01 00:00:00.000000 sciqlop-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-06-13 11:12:27.685482 sciqlop-0.4.1/COPYING
+-rw-r--r--   0        0        0     4594 2023-06-13 11:12:27.685482 sciqlop-0.4.1/README.md
+-rw-r--r--   0        0        0       23 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/__init__.py
+-rw-r--r--   0        0        0     1276 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/app.py
+-rw-r--r--   0        0        0     1510 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/__init__.py
+-rw-r--r--   0        0        0      532 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/enums.py
+-rw-r--r--   0        0        0      831 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/logging/__init__.py
+-rw-r--r--   0        0        0      172 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/models.py
+-rw-r--r--   0        0        0        1 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/pipelines_model/__init__.py
+-rw-r--r--   0        0        0     5204 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/pipelines_model/auto_register.py
+-rw-r--r--   0        0        0      128 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/pipelines_model/base/__init__.py
+-rw-r--r--   0        0        0     6909 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/pipelines_model/base/model.py
+-rw-r--r--   0        0        0     2925 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/pipelines_model/base/pipeline_node.py
+-rw-r--r--   0        0        0     5352 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/pipelines_model/data_pipeline.py
+-rw-r--r--   0        0        0      718 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/pipelines_model/data_provider.py
+-rw-r--r--   0        0        0     4764 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/pipelines_model/easy_provider.py
+-rw-r--r--   0        0        0     3820 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/pipelines_model/graph.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/products_model/__init__.py
+-rw-r--r--   0        0        0     6549 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/products_model/model.py
+-rw-r--r--   0        0        0     3195 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/products_model/product_node.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/resampling/__init__.py
+-rw-r--r--   0        0        0     1493 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/resampling/spectro_regrid.py
+-rw-r--r--   0        0        0      186 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/backend/unique_names.py
+-rw-r--r--   0        0        0     1645 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/mime/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/mime/types.py
+-rw-r--r--   0        0        0     2279 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/plugins/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/plugins/catalogs/__init__.py
+-rw-r--r--   0        0        0     1555 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/plugins/catalogs/catalogs.py
+-rw-r--r--   0        0        0     7828 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/__init__.py
+-rw-r--r--   0        0        0    10334 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/catalog_selector.py
+-rw-r--r--   0        0        0     1045 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/event.py
+-rw-r--r--   0        0        0     3208 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/event_selector.py
+-rw-r--r--   0        0        0     1060 2023-06-13 11:12:27.685482 sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/event_span.py
+-rw-r--r--   0        0        0     4023 2023-06-13 11:12:27.689482 sciqlop-0.4.1/SciQLop/plugins/speasy.py
+-rw-r--r--   0        0        0     1419 2023-06-13 11:12:27.689482 sciqlop-0.4.1/SciQLop/plugins/test_plugin.py
+-rw-r--r--   0        0        0   641256 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/__init__.py
+-rw-r--r--   0        0        0     8256 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/MPL.png
+-rw-r--r--   0        0        0    20841 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/QCP.png
+-rw-r--r--   0        0        0   118794 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/SciQLop.png
+-rw-r--r--   0        0        0     3191 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/Simple_icon_time.svg
+-rw-r--r--   0        0        0     1956 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/add.png
+-rw-r--r--   0        0        0     2001 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/allEvents.png
+-rw-r--r--   0        0        0      615 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/catalogue.png
+-rw-r--r--   0        0        0     1003 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/chart.png
+-rw-r--r--   0        0        0     1047 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/cursor.png
+-rw-r--r--   0        0        0     2150 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/dataSourceComponent.png
+-rw-r--r--   0        0        0      882 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/dataSourceNode.png
+-rw-r--r--   0        0        0     1213 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/dataSourceProduct.png
+-rw-r--r--   0        0        0     4821 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/dataSourceRoot.png
+-rw-r--r--   0        0        0      788 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/database.png
+-rw-r--r--   0        0        0      834 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/delete.png
+-rwxr-xr-x   0        0        0     1266 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/discard.png
+-rw-r--r--   0        0        0     1231 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/down.png
+-rw-r--r--   0        0        0     1731 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/drag.png
+-rw-r--r--   0        0        0     4413 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/next.png
+-rwxr-xr-x   0        0        0     1450 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/openInspector.png
+-rw-r--r--   0        0        0     2319 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/plot.png
+-rw-r--r--   0        0        0     2114 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/pointer.png
+-rw-r--r--   0        0        0     4377 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/previous.png
+-rw-r--r--   0        0        0     4841 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/rectangle.png
+-rw-r--r--   0        0        0     1916 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/remove.png
+-rw-r--r--   0        0        0    10041 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/satellite.svg
+-rw-r--r--   0        0        0     1334 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/save.png
+-rw-r--r--   0        0        0    85300 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/sciqlop2PNG_1024.png
+-rw-r--r--   0        0        0     3714 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/time.png
+-rw-r--r--   0        0        0     1084 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/trash.png
+-rw-r--r--   0        0        0     2234 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/unplot.png
+-rw-r--r--   0        0        0     1197 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/up.png
+-rw-r--r--   0        0        0     4056 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/icons/zoom.png
+-rw-r--r--   0        0        0     1319 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/resources/resources.qrc
+-rw-r--r--   0        0        0        0 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/__init__.py
+-rw-r--r--   0        0        0     4161 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/central_widget.py
+-rw-r--r--   0        0        0       31 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/common/__init__.py
+-rw-r--r--   0        0        0     1005 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/common/tree_view.py
+-rw-r--r--   0        0        0     2499 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/console.py
+-rw-r--r--   0        0        0     3102 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/datetime_range.py
+-rw-r--r--   0        0        0      157 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/drag_and_drop/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/drag_and_drop/drop_handler.py
+-rw-r--r--   0        0        0     2450 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/drag_and_drop/helper.py
+-rw-r--r--   0        0        0     3120 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/drag_and_drop/place_holder_manager.py
+-rw-r--r--   0        0        0     1134 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/drag_and_drop/placeholder.py
+-rw-r--r--   0        0        0     4955 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/mainwindow.py
+-rw-r--r--   0        0        0       39 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/pipelines/__init__.py
+-rw-r--r--   0        0        0     2085 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/pipelines/pipeline_tree.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/plots/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/plots/abstract_plot_panel.py
+-rw-r--r--   0        0        0     3684 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/plots/colormap_graph.py
+-rw-r--r--   0        0        0     1720 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/plots/line_graph.py
+-rw-r--r--   0        0        0     5504 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/plots/mpl_panel.py
+-rw-r--r--   0        0        0    10643 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/plots/time_series_plot.py
+-rw-r--r--   0        0        0     2936 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/plots/time_span.py
+-rw-r--r--   0        0        0     1201 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/plots/time_span_controller.py
+-rw-r--r--   0        0        0     8234 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/plots/time_sync_panel.py
+-rw-r--r--   0        0        0       39 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/products_tree/__init__.py
+-rw-r--r--   0        0        0     1378 2023-06-13 11:12:27.693482 sciqlop-0.4.1/SciQLop/widgets/products_tree/products_tree.py
+-rw-r--r--   0        0        0     1378 2023-06-13 11:12:27.697482 sciqlop-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5788 1970-01-01 00:00:00.000000 sciqlop-0.4.1/PKG-INFO
```

### Comparing `sciqlop-0.4.0/COPYING` & `sciqlop-0.4.1/COPYING`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/README.md` & `sciqlop-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/app.py` & `sciqlop-0.4.1/SciQLop/app.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/__init__.py` & `sciqlop-0.4.1/SciQLop/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/enums.py` & `sciqlop-0.4.1/SciQLop/backend/enums.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/logging/__init__.py` & `sciqlop-0.4.1/SciQLop/backend/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/pipelines_model/auto_register.py` & `sciqlop-0.4.1/SciQLop/backend/pipelines_model/auto_register.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/pipelines_model/base/model.py` & `sciqlop-0.4.1/SciQLop/backend/pipelines_model/base/model.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/pipelines_model/base/pipeline_node.py` & `sciqlop-0.4.1/SciQLop/backend/pipelines_model/base/pipeline_node.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/pipelines_model/data_pipeline.py` & `sciqlop-0.4.1/SciQLop/backend/pipelines_model/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/pipelines_model/data_provider.py` & `sciqlop-0.4.1/SciQLop/backend/pipelines_model/data_provider.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/pipelines_model/graph.py` & `sciqlop-0.4.1/SciQLop/backend/pipelines_model/graph.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/products_model/model.py` & `sciqlop-0.4.1/SciQLop/backend/products_model/model.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/products_model/product_node.py` & `sciqlop-0.4.1/SciQLop/backend/products_model/product_node.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/backend/resampling/spectro_regrid.py` & `sciqlop-0.4.1/SciQLop/backend/resampling/spectro_regrid.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 def regrid(v: SpeasyVariable) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     t: np.ndarray = v.time.astype(np.timedelta64) / np.timedelta64(1, 's')
     resampled_t = np.linspace(t[0], t[-1], num=min(10000, len(t)), endpoint=False)
     values = v.values
 
     if len(v.axes) == 1:
-        y = np.arange(v.values.shape[1]) * 1.
+        new_y = np.arange(v.values.shape[1]) * 1.
+        y = np.tile(new_y, len(t)).reshape((len(t), -1))
     elif len(v.axes[1].values.shape) == 1:
-        y = np.nan_to_num(v.axes[1].values.astype(np.float64), nan=0., copy=False)
+        new_y = np.nan_to_num(v.axes[1].values.astype(np.float64), nan=0., copy=False)
+        y = np.tile(new_y, len(t)).reshape((len(t), -1))
     elif v.axes[1].values.shape[0] == 1:
-        y = np.nan_to_num(v.axes[1].values.astype(np.float64), nan=0., copy=False)
-        y = y.flatten()
+        new_y = np.nan_to_num(v.axes[1].values.astype(np.float64), nan=0., copy=False)[0]
+        y = np.tile(new_y, len(t)).reshape((len(t), -1))
     else:
         y = v.axes[1].values.astype(np.float64)
         new_y = np.logspace(np.log10(np.nanmin(y)), np.log10(np.nanmax(y)), num=int(4 * y.shape[1]))
         y = np.nan_to_num(y, nan=0., copy=False)
 
-        values = griddata((np.repeat(t, y.shape[1]), y.ravel()),
-                          values.ravel(),
-                          (np.repeat(resampled_t, len(new_y)), np.tile(new_y, len(resampled_t))),
-                          method='nearest',
-                          fill_value=np.nan)
-        y = new_y
+    values = griddata((np.repeat(t, y.shape[1]), y.ravel()),
+                      values.ravel(),
+                      (np.repeat(resampled_t, len(new_y)), np.tile(new_y, len(resampled_t))),
+                      method='nearest',
+                      fill_value=np.nan)
 
     if values.dtype != np.float64:
         values = values.astype(np.float64)
 
-    return resampled_t, y, values
+    return resampled_t, new_y, values
```

### Comparing `sciqlop-0.4.0/SciQLop/mime/__init__.py` & `sciqlop-0.4.1/SciQLop/mime/__init__.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/plugins/__init__.py` & `sciqlop-0.4.1/SciQLop/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/plugins/catalogs/catalogs.py` & `sciqlop-0.4.1/SciQLop/plugins/catalogs/catalogs.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/__init__.py` & `sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/catalog_selector.py` & `sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/catalog_selector.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/event.py` & `sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/event.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/event_selector.py` & `sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/event_selector.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/plugins/catalogs/lightweight_manager/event_span.py` & `sciqlop-0.4.1/SciQLop/plugins/catalogs/lightweight_manager/event_span.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/plugins/speasy.py` & `sciqlop-0.4.1/SciQLop/plugins/speasy.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,16 @@
             return ParameterType.SPECTROGRAM
         else:
             if components_cnt == 0 or components_cnt == 1:
                 return ParameterType.SCALAR
             if components_cnt == 3:
                 return ParameterType.VECTOR
             return ParameterType.MULTICOMPONENT
-
+    if 'amda' in param.spz_provider().lower():
+        return ParameterType.MULTICOMPONENT  # should be a safe backup
     return ParameterType.NONE
 
 
 def get_node_meta(node):
     meta = {}
     for name, child in node.__dict__.items():
         if isinstance(child, str):
```

### Comparing `sciqlop-0.4.0/SciQLop/plugins/test_plugin.py` & `sciqlop-0.4.1/SciQLop/plugins/test_plugin.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/__init__.py` & `sciqlop-0.4.1/SciQLop/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/MPL.png` & `sciqlop-0.4.1/SciQLop/resources/icons/MPL.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/QCP.png` & `sciqlop-0.4.1/SciQLop/resources/icons/QCP.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/SciQLop.png` & `sciqlop-0.4.1/SciQLop/resources/icons/SciQLop.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/Simple_icon_time.svg` & `sciqlop-0.4.1/SciQLop/resources/icons/Simple_icon_time.svg`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/add.png` & `sciqlop-0.4.1/SciQLop/resources/icons/add.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/allEvents.png` & `sciqlop-0.4.1/SciQLop/resources/icons/allEvents.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/catalogue.png` & `sciqlop-0.4.1/SciQLop/resources/icons/catalogue.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/chart.png` & `sciqlop-0.4.1/SciQLop/resources/icons/chart.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/cursor.png` & `sciqlop-0.4.1/SciQLop/resources/icons/cursor.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/dataSourceComponent.png` & `sciqlop-0.4.1/SciQLop/resources/icons/dataSourceComponent.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/dataSourceNode.png` & `sciqlop-0.4.1/SciQLop/resources/icons/dataSourceNode.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/dataSourceProduct.png` & `sciqlop-0.4.1/SciQLop/resources/icons/dataSourceProduct.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/dataSourceRoot.png` & `sciqlop-0.4.1/SciQLop/resources/icons/dataSourceRoot.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/database.png` & `sciqlop-0.4.1/SciQLop/resources/icons/database.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/delete.png` & `sciqlop-0.4.1/SciQLop/resources/icons/delete.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/discard.png` & `sciqlop-0.4.1/SciQLop/resources/icons/discard.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/down.png` & `sciqlop-0.4.1/SciQLop/resources/icons/down.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/drag.png` & `sciqlop-0.4.1/SciQLop/resources/icons/drag.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/next.png` & `sciqlop-0.4.1/SciQLop/resources/icons/next.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/openInspector.png` & `sciqlop-0.4.1/SciQLop/resources/icons/openInspector.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/plot.png` & `sciqlop-0.4.1/SciQLop/resources/icons/plot.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/pointer.png` & `sciqlop-0.4.1/SciQLop/resources/icons/pointer.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/previous.png` & `sciqlop-0.4.1/SciQLop/resources/icons/previous.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/rectangle.png` & `sciqlop-0.4.1/SciQLop/resources/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/remove.png` & `sciqlop-0.4.1/SciQLop/resources/icons/remove.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/satellite.svg` & `sciqlop-0.4.1/SciQLop/resources/icons/satellite.svg`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/save.png` & `sciqlop-0.4.1/SciQLop/resources/icons/save.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/sciqlop2PNG_1024.png` & `sciqlop-0.4.1/SciQLop/resources/icons/sciqlop2PNG_1024.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/time.png` & `sciqlop-0.4.1/SciQLop/resources/icons/time.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/trash.png` & `sciqlop-0.4.1/SciQLop/resources/icons/trash.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/unplot.png` & `sciqlop-0.4.1/SciQLop/resources/icons/unplot.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/up.png` & `sciqlop-0.4.1/SciQLop/resources/icons/up.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/icons/zoom.png` & `sciqlop-0.4.1/SciQLop/resources/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/resources/resources.qrc` & `sciqlop-0.4.1/SciQLop/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/central_widget.py` & `sciqlop-0.4.1/SciQLop/widgets/central_widget.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/common/tree_view.py` & `sciqlop-0.4.1/SciQLop/widgets/common/tree_view.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/console.py` & `sciqlop-0.4.1/SciQLop/widgets/console.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/datetime_range.py` & `sciqlop-0.4.1/SciQLop/widgets/datetime_range.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/drag_and_drop/helper.py` & `sciqlop-0.4.1/SciQLop/widgets/drag_and_drop/helper.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/drag_and_drop/place_holder_manager.py` & `sciqlop-0.4.1/SciQLop/widgets/drag_and_drop/place_holder_manager.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/drag_and_drop/placeholder.py` & `sciqlop-0.4.1/SciQLop/widgets/drag_and_drop/placeholder.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/mainwindow.py` & `sciqlop-0.4.1/SciQLop/widgets/mainwindow.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/pipelines/pipeline_tree.py` & `sciqlop-0.4.1/SciQLop/widgets/pipelines/pipeline_tree.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/plots/abstract_plot_panel.py` & `sciqlop-0.4.1/SciQLop/widgets/plots/abstract_plot_panel.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/plots/colormap_graph.py` & `sciqlop-0.4.1/SciQLop/widgets/plots/colormap_graph.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/plots/line_graph.py` & `sciqlop-0.4.1/SciQLop/widgets/plots/line_graph.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/plots/mpl_panel.py` & `sciqlop-0.4.1/SciQLop/widgets/plots/mpl_panel.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/plots/time_series_plot.py` & `sciqlop-0.4.1/SciQLop/widgets/plots/time_series_plot.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/plots/time_span.py` & `sciqlop-0.4.1/SciQLop/widgets/plots/time_span.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/plots/time_span_controller.py` & `sciqlop-0.4.1/SciQLop/widgets/plots/time_span_controller.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/plots/time_sync_panel.py` & `sciqlop-0.4.1/SciQLop/widgets/plots/time_sync_panel.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/SciQLop/widgets/products_tree/products_tree.py` & `sciqlop-0.4.1/SciQLop/widgets/products_tree/products_tree.py`

 * *Files identical despite different names*

### Comparing `sciqlop-0.4.0/pyproject.toml` & `sciqlop-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core"]
 
 [project]
 name = 'SciQLop'
-version = "0.4.0"
+version = "0.4.1"
 description = "An ergonomic and efficient application to browse and label in situ plasma measurements from multi-mission satellite data."
 keywords = ["machine-learning", "satellite", "plasma-physics", "nasa-data", "amda", "cdpp"]
 authors = [
     { name = "Alexis Jeandet", email = "alexis.jeandet@member.fsf.org" }
 ]
 
 maintainers = [
```

### Comparing `sciqlop-0.4.0/PKG-INFO` & `sciqlop-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciQLop
-Version: 0.4.0
+Version: 0.4.1
 Summary: An ergonomic and efficient application to browse and label in situ plasma measurements from multi-mission satellite data.
 Keywords: machine-learning,satellite,plasma-physics,nasa-data,amda,cdpp
 Author-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Maintainer-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
```

