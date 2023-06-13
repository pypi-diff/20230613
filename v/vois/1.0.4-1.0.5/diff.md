# Comparing `tmp/vois-1.0.4.tar.gz` & `tmp/vois-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vois-1.0.4.tar", last modified: Fri Jun  9 16:49:15 2023, max compression
+gzip compressed data, was "vois-1.0.5.tar", last modified: Tue Jun 13 09:32:16 2023, max compression
```

## Comparing `vois-1.0.4.tar` & `vois-1.0.5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 16:49:15.372049 vois-1.0.4/
--rw-rw-rw-   0        0        0    14155 2023-06-09 08:06:09.000000 vois-1.0.4/LICENCE
--rw-rw-rw-   0        0        0      631 2023-06-09 16:48:21.000000 vois-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    73887 2023-06-09 08:06:09.000000 vois-1.0.4/Notice.txt
--rw-rw-rw-   0        0        0    19142 2023-06-09 16:49:15.370051 vois-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1335 2023-06-09 14:16:01.000000 vois-1.0.4/README.md
--rw-rw-rw-   0        0        0     6065 2023-06-09 16:34:02.000000 vois-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 16:49:15.373047 vois-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 16:49:14.897756 vois-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 16:49:15.001259 vois-1.0.4/src/vois/
--rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/__init__.py
--rw-rw-rw-   0        0        0    11918 2023-06-09 16:34:04.000000 vois-1.0.4/src/vois/colors.py
--rw-rw-rw-   0        0        0     4168 2023-06-09 16:34:04.000000 vois-1.0.4/src/vois/download.py
--rw-rw-rw-   0        0        0    17916 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/eucountries.py
--rw-rw-rw-   0        0        0    10493 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/geojsonUtils.py
--rw-rw-rw-   0        0        0    66667 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/interMap.py
--rw-rw-rw-   0        0        0     9302 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/ipytrees.py
--rw-rw-rw-   0        0        0    35732 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/leafletMap.py
--rw-rw-rw-   0        0        0    29755 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/svgBubblesChart.py
--rw-rw-rw-   0        0        0    11325 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/svgGraph.py
--rw-rw-rw-   0        0        0    18669 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/svgHeatmap.py
--rw-rw-rw-   0        0        0  1033396 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/svgMap.py
--rw-rw-rw-   0        0        0    21956 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/svgPackedCirclesChart.py
--rw-rw-rw-   0        0        0    18049 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/svgRankChart.py
--rw-rw-rw-   0        0        0    48423 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/svgUtils.py
--rw-rw-rw-   0        0        0     7363 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/treemapPlotly.py
--rw-rw-rw-   0        0        0     2290 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/urlOpen.py
--rw-rw-rw-   0        0        0     2017 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/urlUpdate.py
-drwxrwxrwx   0        0        0        0 2023-06-09 16:49:15.353058 vois-1.0.4/src/vois/vuetify/
--rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/__init__.py
--rw-rw-rw-   0        0        0    51564 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/app.py
--rw-rw-rw-   0        0        0    43073 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/basemaps.py
--rw-rw-rw-   0        0        0    13241 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/button.py
--rw-rw-rw-   0        0        0    12444 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/card.py
--rw-rw-rw-   0        0        0    10734 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/cardsGrid.py
--rw-rw-rw-   0        0        0     8770 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/colorPicker.py
--rw-rw-rw-   0        0        0    10437 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/datatable.py
--rw-rw-rw-   0        0        0     7269 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/datePicker.py
--rw-rw-rw-   0        0        0     9643 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/dialogGeneric.py
--rw-rw-rw-   0        0        0     4250 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/dialogMessage.py
--rw-rw-rw-   0        0        0     5785 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/dialogWait.py
--rw-rw-rw-   0        0        0     5369 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/dialogYesNo.py
-drwxrwxrwx   0        0        0        0 2023-06-09 16:49:15.367053 vois-1.0.4/src/vois/vuetify/extra/
--rw-rw-rw-   0        0        0       47 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/extra/__init__.py
--rw-rw-rw-   0        0        0     6838 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/extra/file_input.py
--rw-rw-rw-   0        0        0     2251 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/extra/file_input.vue
--rw-rw-rw-   0        0        0    12885 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/fab.py
--rw-rw-rw-   0        0        0      996 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/fontsettings.py
--rw-rw-rw-   0        0        0    13881 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/footer.py
--rw-rw-rw-   0        0        0     8029 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/label.py
--rw-rw-rw-   0        0        0    48546 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/layers.py
--rw-rw-rw-   0        0        0    22786 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/mainPage.py
--rw-rw-rw-   0        0        0     6454 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/menu.py
--rw-rw-rw-   0        0        0     7649 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/multiSwitch.py
--rw-rw-rw-   0        0        0    56576 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/page.py
--rw-rw-rw-   0        0        0    24701 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/paletteEditor.py
--rw-rw-rw-   0        0        0    15331 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/palettePicker.py
--rw-rw-rw-   0        0        0     8048 2023-06-09 16:34:03.000000 vois-1.0.4/src/vois/vuetify/palettePickerEx.py
--rw-rw-rw-   0        0        0     6284 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/popup.py
--rw-rw-rw-   0        0        0     6181 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/progress.py
--rw-rw-rw-   0        0        0     1821 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/queryStrings.py
--rw-rw-rw-   0        0        0     4708 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/radio.py
--rw-rw-rw-   0        0        0     4390 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/rangeSlider.py
--rw-rw-rw-   0        0        0    17054 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/rangeSliderFloat.py
--rw-rw-rw-   0        0        0     9365 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/selectImage.py
--rw-rw-rw-   0        0        0     6052 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/selectMultiple.py
--rw-rw-rw-   0        0        0     8721 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/selectSingle.py
--rw-rw-rw-   0        0        0     4816 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/settings.py
--rw-rw-rw-   0        0        0     6679 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/sidePanel.py
--rw-rw-rw-   0        0        0     5546 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/slider.py
--rw-rw-rw-   0        0        0    12119 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/sliderFloat.py
--rw-rw-rw-   0        0        0     4590 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/snackbar.py
--rw-rw-rw-   0        0        0    24635 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/sortableList.py
--rw-rw-rw-   0        0        0     6575 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/svgsGrid.py
--rw-rw-rw-   0        0        0     4695 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/switch.py
--rw-rw-rw-   0        0        0     6967 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/tabs.py
--rw-rw-rw-   0        0        0     6369 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/textlist.py
--rw-rw-rw-   0        0        0     7009 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/title.py
--rw-rw-rw-   0        0        0     7465 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/toggle.py
--rw-rw-rw-   0        0        0     3179 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/tooltip.py
--rw-rw-rw-   0        0        0    68877 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/treeview.py
--rw-rw-rw-   0        0        0     5036 2023-06-09 16:34:02.000000 vois-1.0.4/src/vois/vuetify/upload.py
-drwxrwxrwx   0        0        0        0 2023-06-09 16:49:15.125189 vois-1.0.4/src/vois.egg-info/
--rw-rw-rw-   0        0        0    19142 2023-06-09 16:49:14.000000 vois-1.0.4/src/vois.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2188 2023-06-09 16:49:14.000000 vois-1.0.4/src/vois.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 16:49:14.000000 vois-1.0.4/src/vois.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-06-09 16:49:14.000000 vois-1.0.4/src/vois.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 16:49:14.000000 vois-1.0.4/src/vois.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:16.053506 vois-1.0.5/
+-rw-rw-rw-   0        0        0    14155 2023-06-09 08:06:09.000000 vois-1.0.5/LICENCE
+-rw-rw-rw-   0        0        0      631 2023-06-09 16:48:21.000000 vois-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    73887 2023-06-09 08:06:09.000000 vois-1.0.5/Notice.txt
+-rw-rw-rw-   0        0        0    19318 2023-06-13 09:32:16.052506 vois-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1511 2023-06-13 09:22:47.000000 vois-1.0.5/README.md
+-rw-rw-rw-   0        0        0     6089 2023-06-13 09:25:30.000000 vois-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 09:32:16.053506 vois-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:14.878835 vois-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:15.267584 vois-1.0.5/src/vois/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/__init__.py
+-rw-rw-rw-   0        0        0    11918 2023-06-09 16:34:04.000000 vois-1.0.5/src/vois/colors.py
+-rw-rw-rw-   0        0        0     4168 2023-06-09 16:34:04.000000 vois-1.0.5/src/vois/download.py
+-rw-rw-rw-   0        0        0    17916 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/eucountries.py
+-rw-rw-rw-   0        0        0    10493 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/geojsonUtils.py
+-rw-rw-rw-   0        0        0    66667 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/interMap.py
+-rw-rw-rw-   0        0        0     9302 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/ipytrees.py
+-rw-rw-rw-   0        0        0    35732 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/leafletMap.py
+-rw-rw-rw-   0        0        0    29755 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgBubblesChart.py
+-rw-rw-rw-   0        0        0    11325 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgGraph.py
+-rw-rw-rw-   0        0        0    18669 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgHeatmap.py
+-rw-rw-rw-   0        0        0  1033396 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgMap.py
+-rw-rw-rw-   0        0        0    21956 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgPackedCirclesChart.py
+-rw-rw-rw-   0        0        0    18049 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgRankChart.py
+-rw-rw-rw-   0        0        0    48423 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgUtils.py
+-rw-rw-rw-   0        0        0     7363 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/treemapPlotly.py
+-rw-rw-rw-   0        0        0     2290 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/urlOpen.py
+-rw-rw-rw-   0        0        0     2017 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/urlUpdate.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:16.005533 vois-1.0.5/src/vois/vuetify/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/__init__.py
+-rw-rw-rw-   0        0        0    52950 2023-06-13 09:22:47.000000 vois-1.0.5/src/vois/vuetify/app.py
+-rw-rw-rw-   0        0        0    43073 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/basemaps.py
+-rw-rw-rw-   0        0        0    13241 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/button.py
+-rw-rw-rw-   0        0        0    12444 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/card.py
+-rw-rw-rw-   0        0        0    10734 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/cardsGrid.py
+-rw-rw-rw-   0        0        0     8770 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/colorPicker.py
+-rw-rw-rw-   0        0        0    10437 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/datatable.py
+-rw-rw-rw-   0        0        0     7269 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/datePicker.py
+-rw-rw-rw-   0        0        0     9643 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/dialogGeneric.py
+-rw-rw-rw-   0        0        0     4250 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/dialogMessage.py
+-rw-rw-rw-   0        0        0     5785 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/dialogWait.py
+-rw-rw-rw-   0        0        0     5369 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/dialogYesNo.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:16.047508 vois-1.0.5/src/vois/vuetify/extra/
+-rw-rw-rw-   0        0        0       47 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/extra/__init__.py
+-rw-rw-rw-   0        0        0     6838 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/extra/file_input.py
+-rw-rw-rw-   0        0        0     2251 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/extra/file_input.vue
+-rw-rw-rw-   0        0        0    12885 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/fab.py
+-rw-rw-rw-   0        0        0      996 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/fontsettings.py
+-rw-rw-rw-   0        0        0    13881 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/footer.py
+-rw-rw-rw-   0        0        0     8029 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/label.py
+-rw-rw-rw-   0        0        0    48546 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/layers.py
+-rw-rw-rw-   0        0        0    22786 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/mainPage.py
+-rw-rw-rw-   0        0        0     6454 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/menu.py
+-rw-rw-rw-   0        0        0     7649 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/multiSwitch.py
+-rw-rw-rw-   0        0        0    56576 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/page.py
+-rw-rw-rw-   0        0        0    24701 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/paletteEditor.py
+-rw-rw-rw-   0        0        0    15331 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/palettePicker.py
+-rw-rw-rw-   0        0        0     8048 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/palettePickerEx.py
+-rw-rw-rw-   0        0        0     6284 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/popup.py
+-rw-rw-rw-   0        0        0     6181 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/progress.py
+-rw-rw-rw-   0        0        0     1821 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/queryStrings.py
+-rw-rw-rw-   0        0        0     4708 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/radio.py
+-rw-rw-rw-   0        0        0     4390 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/rangeSlider.py
+-rw-rw-rw-   0        0        0    17054 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/rangeSliderFloat.py
+-rw-rw-rw-   0        0        0     9365 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/selectImage.py
+-rw-rw-rw-   0        0        0     6052 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/selectMultiple.py
+-rw-rw-rw-   0        0        0     8721 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/selectSingle.py
+-rw-rw-rw-   0        0        0     4816 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/settings.py
+-rw-rw-rw-   0        0        0     6679 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/sidePanel.py
+-rw-rw-rw-   0        0        0     5546 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/slider.py
+-rw-rw-rw-   0        0        0    12119 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/sliderFloat.py
+-rw-rw-rw-   0        0        0     4590 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/snackbar.py
+-rw-rw-rw-   0        0        0    24635 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/sortableList.py
+-rw-rw-rw-   0        0        0     6575 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/svgsGrid.py
+-rw-rw-rw-   0        0        0     4695 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/switch.py
+-rw-rw-rw-   0        0        0     6967 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/tabs.py
+-rw-rw-rw-   0        0        0     6369 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/textlist.py
+-rw-rw-rw-   0        0        0     7009 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/title.py
+-rw-rw-rw-   0        0        0     7465 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/toggle.py
+-rw-rw-rw-   0        0        0     3179 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/tooltip.py
+-rw-rw-rw-   0        0        0    68877 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/treeview.py
+-rw-rw-rw-   0        0        0     5036 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/upload.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:15.301129 vois-1.0.5/src/vois.egg-info/
+-rw-rw-rw-   0        0        0    19318 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2188 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/top_level.txt
```

### Comparing `vois-1.0.4/LICENCE` & `vois-1.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/MANIFEST.in` & `vois-1.0.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/Notice.txt` & `vois-1.0.5/Notice.txt`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/PKG-INFO` & `vois-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vois
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python Voilà simplification library
 Author-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 Maintainer-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 License: Copyright © European Union 2022-2023
         
         
                               EUROPEAN UNION PUBLIC LICENCE v. 1.2
@@ -320,25 +320,34 @@
 
 Python library to simplify the creation of impactful Voilà dashboards.
 
 The online documentation for the vois library is available [here](https://vois.readthedocs.io/en/latest/1_intro.html)
 
 The PDF documentation for the vois library is available [here](https://vois.readthedocs.io/_/downloads/en/latest/pdf/)
 
+The source repository is available [here](https://code.europa.eu/jrc-bdap/vois)
+
+
 The vois library contains:
 
 folder **vois**: helper functions for tasks not directly related to ipyvuetify (manage geojson files, create an interactive map to display custom geojson, simplify visualization of hierarchical data in Plotly, create custom SVG visualizations, etc.)
 
 folder **vois/vuetify**: classes to simplify the development of GUIs using ipyvuetify (each source file contains a wrapper to simplify the usage of a ipyvuetify widget)
 
 
 ## License
 
 VOIS library is released under a
 [EUPL Version 1.2](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12) license.
 
+## Setup
+
+The vois library can be installed using this command:
+
+`pip install vois`
+
 
 ## Tutorial
 
 The tutorial section of the documentation available [here](https://vois.readthedocs.io/en/latest/2_tutorial.html) provides a step by step example for the construction of a dashboard to display EUROSTAT data on Energy Consumption in Europe.
 
 ![screenshot](https://jeodpp.jrc.ec.europa.eu/services/shared/pngs/vois_example.png)
```

### Comparing `vois-1.0.4/README.md` & `vois-1.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,34 @@
 
 Python library to simplify the creation of impactful Voilà dashboards.
 
 The online documentation for the vois library is available [here](https://vois.readthedocs.io/en/latest/1_intro.html)
 
 The PDF documentation for the vois library is available [here](https://vois.readthedocs.io/_/downloads/en/latest/pdf/)
 
+The source repository is available [here](https://code.europa.eu/jrc-bdap/vois)
+
+
 The vois library contains:
 
 folder **vois**: helper functions for tasks not directly related to ipyvuetify (manage geojson files, create an interactive map to display custom geojson, simplify visualization of hierarchical data in Plotly, create custom SVG visualizations, etc.)
 
 folder **vois/vuetify**: classes to simplify the development of GUIs using ipyvuetify (each source file contains a wrapper to simplify the usage of a ipyvuetify widget)
 
 
 ## License
 
 VOIS library is released under a
 [EUPL Version 1.2](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12) license.
 
+## Setup
+
+The vois library can be installed using this command:
+
+`pip install vois`
+
 
 ## Tutorial
 
 The tutorial section of the documentation available [here](https://vois.readthedocs.io/en/latest/2_tutorial.html) provides a step by step example for the construction of a dashboard to display EUROSTAT data on Energy Consumption in Europe.
 
 ![screenshot](https://jeodpp.jrc.ec.europa.eu/services/shared/pngs/vois_example.png)
```

### Comparing `vois-1.0.4/pyproject.toml` & `vois-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 name = "vois"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.4"  # Required
+version = "1.0.5"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A Python Voilà simplification library"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -111,14 +111,15 @@
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [ # Optional
   "Pillow >= 9.4.0",
   "traitlets >= 5.9.0",
   "ipywidgets >= 8.0.0",
   "requests >= 2.28.0",
   "urllib3 >= 1.26.0",
+  "sphinx-copybutton",
   "ipykernel",
   "pandas",
   "ipyvuetify",
   "ipytree",
   "ipyevents",
   "plotly",
   "ipyleaflet",
```

### Comparing `vois-1.0.4/src/vois/colors.py` & `vois-1.0.5/src/vois/colors.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/download.py` & `vois-1.0.5/src/vois/download.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/eucountries.py` & `vois-1.0.5/src/vois/eucountries.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/geojsonUtils.py` & `vois-1.0.5/src/vois/geojsonUtils.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/interMap.py` & `vois-1.0.5/src/vois/interMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/ipytrees.py` & `vois-1.0.5/src/vois/ipytrees.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/leafletMap.py` & `vois-1.0.5/src/vois/leafletMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/svgBubblesChart.py` & `vois-1.0.5/src/vois/svgBubblesChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/svgGraph.py` & `vois-1.0.5/src/vois/svgGraph.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/svgHeatmap.py` & `vois-1.0.5/src/vois/svgHeatmap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/svgMap.py` & `vois-1.0.5/src/vois/svgMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/svgPackedCirclesChart.py` & `vois-1.0.5/src/vois/svgPackedCirclesChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/svgRankChart.py` & `vois-1.0.5/src/vois/svgRankChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/svgUtils.py` & `vois-1.0.5/src/vois/svgUtils.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/treemapPlotly.py` & `vois-1.0.5/src/vois/treemapPlotly.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/urlOpen.py` & `vois-1.0.5/src/vois/urlOpen.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/urlUpdate.py` & `vois-1.0.5/src/vois/urlUpdate.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/app.py` & `vois-1.0.5/src/vois/vuetify/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,17 @@
     title : str, optional
         Main title of the application to be displayed on the title bar (default is 'Title of the dashboard')
     titlesvg : str, optional
         SVG string to use as application title when the title string is empty (default is '')
     titlesvgclass : str, optional
         Class margins and padding to apply to the titlesvg drawing (default is 'pa-0 ma-0')
     titlecredits : str, optional
-        Credits string to be displayed on the left side of the title bar (default is '')
+        Credits string to be displayed on the right side of the title bar (default is '')
+    titlecredits2 : str, optional
+        Secondary credits string to be displayed on the right side of the title bar (default is '')
     titlestyle : str, optional
         CSS style to apply to the main title of the dashboard (default is '', an example could be: 'font-family: "Times New Roman", Times, serif; font-weight: bold; font-size: 22px;')
     titlespacestyle : str, optional
         CSS style to apply to the space at the left of the title (default is 'width: 50px; min-width: 50px;'). It can be useful to move the title more on the centre of the title bar, by providing a titlespacestyle like 'width: 200px;'
     titleheight : int, optional
         Height of the title bar in pixels (default is 70 pixels)
     totalheight : int, optional
@@ -177,14 +179,16 @@
          Color of the 'three vertical points icon' that opens/closes the minipanel (default is the textcolor_notdark defined in the settings.py module)
     minipaneliconscolor : str, optional
          Color of the icons in the minipanel (default is the textcolor_notdark defined in the settings.py module)
     onclicktab : function, optional
         Python function to call when the user clicks on one of the tabs of the title bar. The function will receive a parameter of type string containing the text of the tab
     onclickcredits : function, optional
         Python function to call when the user clicks on the credits button on the title bar. The function will receive no parameters
+    onclickcredits2 : function, optional
+        Python function to call when the user clicks on the secondary credits button on the title bar. The function will receive no parameters
     onclicklogo : function, optional
         Python function to call when the user clicks on the logo image on the title bar. The function will receive no parameters
     onclickfooter : function, optional
         Python function to call when the user clicks on one of the buttons of the footer bar. The function will receive a parameter of type string containing the text of the button
     onclickminipanel : function, optional
         Python function to call when the user clicks on one of the icons of the minipanel in the footer bar. The function will receive a parameter of type int containing the index of the icon
     fullscreen : bool, optional
@@ -278,14 +282,15 @@
    """
         
     def __init__(self, 
                  title='Title of the dashboard',
                  titlesvg='',
                  titlesvgclass='pa-0 ma-0',
                  titlecredits='',
+                 titlecredits2='',
                  titlestyle='',      # 'font-family: "Times New Roman", Times, serif; font-weight: bold; font-size: 22px;'
                  titlespacestyle='width: 50px; min-width: 50px;',
                  titleheight=70,
                  totalheight=985,
                  dark=settings.dark_mode,
                  backcolor=settings.color_second,
                  titlewidth= '600px',    # '50%'
@@ -325,22 +330,24 @@
                  minipanelopen=False,
                  minipanellarge=True,
                  minipanelbuttoncolor=settings.textcolor_notdark,
                  minipaneliconscolor=settings.textcolor_notdark,
 
                  onclicktab=None,            # Function with 1 string argument string containing the text of the tab
                  onclickcredits=None,        # Function with 0 arguments
+                 onclickcredits2=None,       # Function with 0 arguments
                  onclicklogo=None,           # Function with 0 arguments
                  onclickfooter=None,         # Function with 1 string argument string containing the text of the button
                  onclickminipanel=None,      # Function with 1 string argument integer containing the index of the icon
                  fullscreen=False):          # If True the App will fill all the page!
         
         # Storing input parameters
         self.title = title
         self.titlecredits = titlecredits
+        self.titlecredits2 = titlecredits2
         self.titlestyle = titlestyle
         self.titleheight = measure2str(titleheight)
         self.totalheight = measure2str(totalheight)
         self.dark = dark
         self.backcolor = backcolor
         self.titlewidth = measure2str(titlewidth)
         self.footercolor = footercolor
@@ -370,14 +377,15 @@
         self.sidepaneltext = sidepaneltext
         self.sidepanelcontent = sidepanelcontent
         self.sidepaneldark = sidepaneldark
         self.sidepanelbackdark = sidepanelbackdark
 
         self.onclicktab = onclicktab
         self.onclickcredits = onclickcredits
+        self.onclickcredits2 = onclickcredits2
         self.onclicklogo = onclicklogo
         self.onclickfooter = onclickfooter
         
         self.fullscreen = fullscreen
         
         self.content_vbackground = None     # v.Html object to display an image in the background
         self.content_panels_dict = {}       # Dict to retrieve panels by name
@@ -444,14 +452,22 @@
         
         if self.onclickcredits is None:
             self.credits = v.Btn(text=True, color=buttontext, dark=self.dark, children=[self.titlecredits], rounded=settings.button_rounded, style_='text-transform: none; cursor: initial;')
         else:
             self.credits = v.Btn(text=True, color=buttontext, dark=self.dark, children=[self.titlecredits], rounded=settings.button_rounded, style_='text-transform: none;')
             self.credits.on_event('click', self.__internal_onclickCredits)
 
+        self.credits2 = v.Html(tag='div', children=[''])
+        if len(self.titlecredits2) > 0:
+            if self.onclickcredits2 is None:
+                self.credits2 = v.Btn(text=True, color=buttontext, dark=self.dark, children=[self.titlecredits2], rounded=settings.button_rounded, style_='text-transform: none; cursor: initial;')
+            else:
+                self.credits2 = v.Btn(text=True, color=buttontext, dark=self.dark, children=[self.titlecredits2], rounded=settings.button_rounded, style_='text-transform: none;')
+                self.credits2.on_event('click', self.__internal_onclickCredits2)
+            
         self.tlist = []
         for t in self.titletabs:
             telem = v.Tab(style_='%s %s' % ('', self.titletabsstile), children=[t])
             telem.on_event('click', self.__internal_onclickTab)
             self.tlist.append(telem)
         self.tabs = v.Tabs(v_model=self.titletabsactive, dark=titletabsdark, color=self.titletabscolor, background_color='transparent', 
                            align_with_title=True, children=self.tlist, height=self.titleheight, min_height=self.titleheight, max_height=self.titleheight)
@@ -461,15 +477,15 @@
         if not self.onclicklogo is None: logostyle = 'cursor: pointer;'
         self.logoimg = v.Img(src=self.logourl, class_='pa-0 ma-0', style_=logostyle, contain=True, height=self.logomaxheight, width=self.logomaxwidth, max_height=self.logomaxheight, max_width=self.logomaxwidth)
         self.logoimg.on_event('click', self.__internal_onclickLogo)
         
         card1 = v.Card(height=titleheight, color='transparent', elevation=0, children=[self.abih],    class_="d-flex align-center")
         card2 = v.Card(height=titleheight, color='transparent', elevation=0, children=[self.abt],     class_="d-flex align-center", style_='overflow: hidden; width: %s;' % self.titlewidth)
         card3 = v.Card(height=titleheight, color='transparent', elevation=0, children=[self.tabs],    class_="d-flex align-center")
-        card4 = v.Card(height=titleheight, color='transparent', elevation=0, children=[self.credits], class_="d-flex align-center")
+        card4 = v.Card(height=titleheight, color='transparent', elevation=0, children=[self.credits, self.credits2], class_="d-flex align-center")
         card5 = v.Card(height=titleheight, color='transparent', elevation=0, children=[self.logoimg], class_="d-flex align-center mr-1")
         
         if len(self.titletabs) > 0:
             r = v.Row(justify="space-between", children=[card1,card2,card3,s,card4,card5], class_="pa-0 ma-0")
         else:
             r = v.Row(justify="space-between", no_gutters=True, children=[card1,card2,s,card4,card5], class_="pa-0 ma-0")
         if (not self.backgroundimageurl is None) and (len(self.backgroundimageurl) > 0):
@@ -764,14 +780,19 @@
             self.onclicktab(self.titletabs[i])
             
     # Manage click on the title credits button
     def __internal_onclickCredits(self, widget, event, data):
         if not self.onclickcredits is None:
             self.onclickcredits()
         
+    # Manage click on the title credits2 button
+    def __internal_onclickCredits2(self, widget, event, data):
+        if not self.onclickcredits2 is None:
+            self.onclickcredits2()
+            
     # When the panel has bee closed
     def __internal_panelclosed(self):
         self.outpanel.clear_output()
         with self.outpanel:
             display(self.panel.nav)
             
     # Manage click on the footer credits button
```

### Comparing `vois-1.0.4/src/vois/vuetify/basemaps.py` & `vois-1.0.5/src/vois/vuetify/basemaps.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/button.py` & `vois-1.0.5/src/vois/vuetify/button.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/card.py` & `vois-1.0.5/src/vois/vuetify/card.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/cardsGrid.py` & `vois-1.0.5/src/vois/vuetify/cardsGrid.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/colorPicker.py` & `vois-1.0.5/src/vois/vuetify/colorPicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/datatable.py` & `vois-1.0.5/src/vois/vuetify/datatable.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/datePicker.py` & `vois-1.0.5/src/vois/vuetify/datePicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/dialogGeneric.py` & `vois-1.0.5/src/vois/vuetify/dialogGeneric.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/dialogMessage.py` & `vois-1.0.5/src/vois/vuetify/dialogMessage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/dialogWait.py` & `vois-1.0.5/src/vois/vuetify/dialogWait.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/dialogYesNo.py` & `vois-1.0.5/src/vois/vuetify/dialogYesNo.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/extra/file_input.py` & `vois-1.0.5/src/vois/vuetify/extra/file_input.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/extra/file_input.vue` & `vois-1.0.5/src/vois/vuetify/extra/file_input.vue`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/fab.py` & `vois-1.0.5/src/vois/vuetify/fab.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/fontsettings.py` & `vois-1.0.5/src/vois/vuetify/fontsettings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/footer.py` & `vois-1.0.5/src/vois/vuetify/footer.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/label.py` & `vois-1.0.5/src/vois/vuetify/label.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/layers.py` & `vois-1.0.5/src/vois/vuetify/layers.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/mainPage.py` & `vois-1.0.5/src/vois/vuetify/mainPage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/menu.py` & `vois-1.0.5/src/vois/vuetify/menu.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/multiSwitch.py` & `vois-1.0.5/src/vois/vuetify/multiSwitch.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/page.py` & `vois-1.0.5/src/vois/vuetify/page.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/paletteEditor.py` & `vois-1.0.5/src/vois/vuetify/paletteEditor.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/palettePicker.py` & `vois-1.0.5/src/vois/vuetify/palettePicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/palettePickerEx.py` & `vois-1.0.5/src/vois/vuetify/palettePickerEx.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/popup.py` & `vois-1.0.5/src/vois/vuetify/popup.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/progress.py` & `vois-1.0.5/src/vois/vuetify/progress.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/queryStrings.py` & `vois-1.0.5/src/vois/vuetify/queryStrings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/radio.py` & `vois-1.0.5/src/vois/vuetify/radio.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/rangeSlider.py` & `vois-1.0.5/src/vois/vuetify/rangeSlider.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/rangeSliderFloat.py` & `vois-1.0.5/src/vois/vuetify/rangeSliderFloat.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/selectImage.py` & `vois-1.0.5/src/vois/vuetify/selectImage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/selectMultiple.py` & `vois-1.0.5/src/vois/vuetify/selectMultiple.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/selectSingle.py` & `vois-1.0.5/src/vois/vuetify/selectSingle.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/settings.py` & `vois-1.0.5/src/vois/vuetify/settings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/sidePanel.py` & `vois-1.0.5/src/vois/vuetify/sidePanel.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/slider.py` & `vois-1.0.5/src/vois/vuetify/slider.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/sliderFloat.py` & `vois-1.0.5/src/vois/vuetify/sliderFloat.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/snackbar.py` & `vois-1.0.5/src/vois/vuetify/snackbar.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/sortableList.py` & `vois-1.0.5/src/vois/vuetify/sortableList.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/svgsGrid.py` & `vois-1.0.5/src/vois/vuetify/svgsGrid.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/switch.py` & `vois-1.0.5/src/vois/vuetify/switch.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/tabs.py` & `vois-1.0.5/src/vois/vuetify/tabs.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/textlist.py` & `vois-1.0.5/src/vois/vuetify/textlist.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/title.py` & `vois-1.0.5/src/vois/vuetify/title.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/toggle.py` & `vois-1.0.5/src/vois/vuetify/toggle.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/tooltip.py` & `vois-1.0.5/src/vois/vuetify/tooltip.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/treeview.py` & `vois-1.0.5/src/vois/vuetify/treeview.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois/vuetify/upload.py` & `vois-1.0.5/src/vois/vuetify/upload.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.4/src/vois.egg-info/PKG-INFO` & `vois-1.0.5/src/vois.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vois
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python Voilà simplification library
 Author-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 Maintainer-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 License: Copyright © European Union 2022-2023
         
         
                               EUROPEAN UNION PUBLIC LICENCE v. 1.2
@@ -320,25 +320,34 @@
 
 Python library to simplify the creation of impactful Voilà dashboards.
 
 The online documentation for the vois library is available [here](https://vois.readthedocs.io/en/latest/1_intro.html)
 
 The PDF documentation for the vois library is available [here](https://vois.readthedocs.io/_/downloads/en/latest/pdf/)
 
+The source repository is available [here](https://code.europa.eu/jrc-bdap/vois)
+
+
 The vois library contains:
 
 folder **vois**: helper functions for tasks not directly related to ipyvuetify (manage geojson files, create an interactive map to display custom geojson, simplify visualization of hierarchical data in Plotly, create custom SVG visualizations, etc.)
 
 folder **vois/vuetify**: classes to simplify the development of GUIs using ipyvuetify (each source file contains a wrapper to simplify the usage of a ipyvuetify widget)
 
 
 ## License
 
 VOIS library is released under a
 [EUPL Version 1.2](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12) license.
 
+## Setup
+
+The vois library can be installed using this command:
+
+`pip install vois`
+
 
 ## Tutorial
 
 The tutorial section of the documentation available [here](https://vois.readthedocs.io/en/latest/2_tutorial.html) provides a step by step example for the construction of a dashboard to display EUROSTAT data on Energy Consumption in Europe.
 
 ![screenshot](https://jeodpp.jrc.ec.europa.eu/services/shared/pngs/vois_example.png)
```

### Comparing `vois-1.0.4/src/vois.egg-info/SOURCES.txt` & `vois-1.0.5/src/vois.egg-info/SOURCES.txt`

 * *Files identical despite different names*

