# Comparing `tmp/types_wxpython-0.7.1.tar.gz` & `tmp/types_wxpython-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_wxpython-0.7.1.tar", max compression
+gzip compressed data, was "types_wxpython-0.7.2.tar", max compression
```

## Comparing `types_wxpython-0.7.1.tar` & `types_wxpython-0.7.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0    35149 2023-05-18 08:31:50.853852 types_wxpython-0.7.1/LICENSE
--rw-r--r--   0        0        0      725 2023-05-18 08:31:50.853852 types_wxpython-0.7.1/README.md
--rw-r--r--   0        0        0     1136 2023-05-18 08:31:50.853852 types_wxpython-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      117 2023-05-18 08:31:50.853852 types_wxpython-0.7.1/wx-stubs/ActivateEvent/__init__.pyi
--rw-r--r--   0        0        0      120 2023-05-18 08:31:50.853852 types_wxpython-0.7.1/wx-stubs/ConfigBase/__init__.pyi
--rw-r--r--   0        0        0      135 2023-05-18 08:31:50.853852 types_wxpython-0.7.1/wx-stubs/DataObject/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/DateTime/__init__.py
--rw-r--r--   0        0        0     2371 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/DateTime/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/FileType/__init__.py
--rw-r--r--   0        0        0     1059 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/FileType/__init__.pyi
--rw-r--r--   0        0        0      132 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/HelpEvent/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/Image/__init__.py
--rw-r--r--   0        0        0     1300 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/Image/__init__.pyi
--rw-r--r--   0        0        0      173 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/StandardPaths/__init__.pyi
--rw-r--r--   0        0        0      135 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/StaticBitmap/__init__.pyi
--rw-r--r--   0        0        0      130 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/StockPreferencesPage/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/TopLevelWindow/__init__.py
--rw-r--r--   0        0        0      277 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/TopLevelWindow/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/Window/__init__.py
--rw-r--r--   0        0        0      515 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/Window/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.857852 types_wxpython-0.7.1/wx-stubs/__init__.py
--rw-r--r--   0        0        0  1400928 2023-05-18 08:31:50.861853 types_wxpython-0.7.1/wx-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.861853 types_wxpython-0.7.1/wx-stubs/adv/__init__.py
--rw-r--r--   0        0        0   114383 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/adv/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/aui/__init__.py
--rw-r--r--   0        0        0   103369 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/aui/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/dataview/__init__.py
--rw-r--r--   0        0        0   102847 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/dataview/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/glcanvas/__init__.py
--rw-r--r--   0        0        0    11759 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/glcanvas/__init__.pyi
--rw-r--r--   0        0        0      134 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/grid/Grid/__init__.pyi
--rw-r--r--   0        0        0      132 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/grid/GridActivationSource/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/grid/GridBlocks/__init__.py
--rw-r--r--   0        0        0      235 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/grid/GridBlocks/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.865852 types_wxpython-0.7.1/wx-stubs/grid/__init__.py
--rw-r--r--   0        0        0   136304 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/grid/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/html/__init__.py
--rw-r--r--   0        0        0    80110 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/html/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/html2/__init__.py
--rw-r--r--   0        0        0    21938 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/html2/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/agw/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/buttonbar/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/buttonbar/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/gallery/__init__.py
--rw-r--r--   0        0        0     1951 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/gallery/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/toolbar/__init__.py
--rw-r--r--   0        0        0      518 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/toolbar/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/analogclock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/analogclock/lib_setup/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.py
--rw-r--r--   0        0        0      996 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/buttons/__init__.py
--rw-r--r--   0        0        0    16019 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/buttons/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/calendar/__init__.py
--rw-r--r--   0        0        0    15906 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/calendar/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/colourselect/__init__.py
--rw-r--r--   0        0        0     4270 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/colourselect/__init__.pyi
--rw-r--r--   0        0        0     2370 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/dialogs/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/newevent/__init__.py
--rw-r--r--   0        0        0      463 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/newevent/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/scrolledpanel/__init__.py
--rw-r--r--   0        0        0     1757 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/scrolledpanel/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/wxpTag/__init__.py
--rw-r--r--   0        0        0     1071 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/lib/wxpTag/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/media/__init__.py
--rw-r--r--   0        0        0     6369 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/media/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/propgrid/__init__.py
--rw-r--r--   0        0        0   189238 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/propgrid/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/ribbon/__init__.py
--rw-r--r--   0        0        0    81621 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/ribbon/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.869852 types_wxpython-0.7.1/wx-stubs/richtext/__init__.py
--rw-r--r--   0        0        0   360498 2023-05-18 08:31:50.873853 types_wxpython-0.7.1/wx-stubs/richtext/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.873853 types_wxpython-0.7.1/wx-stubs/stc/__init__.py
--rw-r--r--   0        0        0   182064 2023-05-18 08:31:50.873853 types_wxpython-0.7.1/wx-stubs/stc/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.873853 types_wxpython-0.7.1/wx-stubs/xml/__init__.py
--rw-r--r--   0        0        0    14211 2023-05-18 08:31:50.873853 types_wxpython-0.7.1/wx-stubs/xml/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-18 08:31:50.873853 types_wxpython-0.7.1/wx-stubs/xrc/__init__.py
--rw-r--r--   0        0        0    19060 2023-05-18 08:31:50.873853 types_wxpython-0.7.1/wx-stubs/xrc/__init__.pyi
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 types_wxpython-0.7.1/setup.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 types_wxpython-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3047 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/README.md
+-rw-r--r--   0        0        0     1136 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/ActivateEvent/__init__.pyi
+-rw-r--r--   0        0        0      120 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/ConfigBase/__init__.pyi
+-rw-r--r--   0        0        0      135 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/DataObject/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/DateTime/__init__.py
+-rw-r--r--   0        0        0     2371 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/DateTime/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/FileType/__init__.py
+-rw-r--r--   0        0        0     1059 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/FileType/__init__.pyi
+-rw-r--r--   0        0        0      132 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/HelpEvent/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/Image/__init__.py
+-rw-r--r--   0        0        0     1300 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/Image/__init__.pyi
+-rw-r--r--   0        0        0      173 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/StandardPaths/__init__.pyi
+-rw-r--r--   0        0        0      135 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/StaticBitmap/__init__.pyi
+-rw-r--r--   0        0        0      130 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/StockPreferencesPage/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/TopLevelWindow/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/TopLevelWindow/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/Window/__init__.py
+-rw-r--r--   0        0        0      515 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/Window/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.837732 types_wxpython-0.7.2/wx-stubs/__init__.py
+-rw-r--r--   0        0        0  1405678 2023-06-13 09:05:08.845732 types_wxpython-0.7.2/wx-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.845732 types_wxpython-0.7.2/wx-stubs/adv/__init__.py
+-rw-r--r--   0        0        0   114383 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/adv/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/aui/__init__.py
+-rw-r--r--   0        0        0   103369 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/aui/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/dataview/__init__.py
+-rw-r--r--   0        0        0   102752 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/dataview/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/glcanvas/__init__.py
+-rw-r--r--   0        0        0    11759 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/glcanvas/__init__.pyi
+-rw-r--r--   0        0        0      134 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/grid/Grid/__init__.pyi
+-rw-r--r--   0        0        0      132 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/grid/GridActivationSource/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/grid/GridBlocks/__init__.py
+-rw-r--r--   0        0        0      235 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/grid/GridBlocks/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/grid/__init__.py
+-rw-r--r--   0        0        0   137010 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/grid/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/html/__init__.py
+-rw-r--r--   0        0        0    80110 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/html/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/html2/__init__.py
+-rw-r--r--   0        0        0    21938 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/html2/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/agw/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/buttonbar/__init__.py
+-rw-r--r--   0        0        0     1052 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/buttonbar/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/gallery/__init__.py
+-rw-r--r--   0        0        0     1951 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/gallery/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/toolbar/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/toolbar/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/analogclock/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/analogclock/lib_setup/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.py
+-rw-r--r--   0        0        0      996 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/buttons/__init__.py
+-rw-r--r--   0        0        0    16019 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/buttons/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/calendar/__init__.py
+-rw-r--r--   0        0        0    15906 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/calendar/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/colourselect/__init__.py
+-rw-r--r--   0        0        0     4270 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/colourselect/__init__.pyi
+-rw-r--r--   0        0        0     2370 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/dialogs/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/newevent/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-13 09:05:08.849732 types_wxpython-0.7.2/wx-stubs/lib/newevent/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/lib/scrolledpanel/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/lib/scrolledpanel/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/lib/wxpTag/__init__.py
+-rw-r--r--   0        0        0     1071 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/lib/wxpTag/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/media/__init__.py
+-rw-r--r--   0        0        0     6369 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/media/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/propgrid/__init__.py
+-rw-r--r--   0        0        0   189238 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/propgrid/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/ribbon/__init__.py
+-rw-r--r--   0        0        0    81621 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/ribbon/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/richtext/__init__.py
+-rw-r--r--   0        0        0   360498 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/richtext/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/stc/__init__.py
+-rw-r--r--   0        0        0   182064 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/stc/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/xml/__init__.py
+-rw-r--r--   0        0        0    14211 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/xml/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/xrc/__init__.py
+-rw-r--r--   0        0        0    19060 2023-06-13 09:05:08.853732 types_wxpython-0.7.2/wx-stubs/xrc/__init__.pyi
+-rw-r--r--   0        0        0     4806 1970-01-01 00:00:00.000000 types_wxpython-0.7.2/setup.py
+-rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 types_wxpython-0.7.2/PKG-INFO
```

### Comparing `types_wxpython-0.7.1/LICENSE` & `types_wxpython-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/pyproject.toml` & `types_wxpython-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "types-wxpython"
-version = "0.7.1"
+version = "0.7.2"
 description = "Typing stubs for wxPython"
 authors = ["Alexion Software <info@alexion.nl>"]
 homepage = "https://github.com/AlexionSoftware/types-wxpython"
 repository = "https://github.com/AlexionSoftware/types-wxpython"
 keywords = ["wxPython", "typing", "stubs", "wx"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `types_wxpython-0.7.1/wx-stubs/DateTime/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/DateTime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/FileType/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/FileType/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/Image/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/Image/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/Window/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/Window/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2820,14 +2820,21 @@
     def __init__(self) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.PyApp.html
         """
 
     @staticmethod
+    def GTKAllowDiagnosticsControl() -> None:
+        """ Allows wxWidgets to selectively suppress some GTK messages.
+
+            Source: https://docs.wxpython.org/wx.PyApp.html
+        """
+
+    @staticmethod
     def GTKSuppressDiagnostics(flags: int=-1) -> None:
         """ Disables the printing of various GTK messages.
 
             Source: https://docs.wxpython.org/wx.PyApp.html
         """
 
     def GetAssertMode(self) -> 'AppAssertMode':
@@ -4548,15 +4555,15 @@
     def FromResources(name: str) -> 'BitmapBundle':
         """ Create a bundle from the bitmaps in the application resources.
 
             Source: https://docs.wxpython.org/wx.BitmapBundle.html
         """
 
     @staticmethod
-    def FromSVG(data, sizeDef) -> 'BitmapBundle':
+    def FromSVG(*args, **kw) -> 'BitmapBundle':
         """ This is an overloaded member function, provided for convenience. It differs from the above function only in what argument(s) it accepts.
 
             Source: https://docs.wxpython.org/wx.BitmapBundle.html
         """
 
     @staticmethod
     def FromSVGFile(path, sizeDef) -> 'BitmapBundle':
@@ -4976,14 +4983,20 @@
 
     def FindPage(self, page: 'Window') -> int:
         """ Returns the index of the specified tab window or  NOT_FOUND   if not found.
 
             Source: https://docs.wxpython.org/wx.BookCtrlBase.html
         """
 
+    def GetControlSizer(self) -> 'Sizer':
+        """ Returns the sizer containing the control for page selection, if any.
+
+            Source: https://docs.wxpython.org/wx.BookCtrlBase.html
+        """
+
     def GetCurrentPage(self) -> 'Window':
         """ Returns the currently selected page or None.
 
             Source: https://docs.wxpython.org/wx.BookCtrlBase.html
         """
 
     def GetPage(self, page: int) -> 'Window':
@@ -5054,14 +5067,15 @@
 
     def SetSelection(self, page: int) -> int:
         """ Sets the selection to the given page, returning the previous selection.
 
             Source: https://docs.wxpython.org/wx.BookCtrlBase.html
         """
 
+    ControlSizer: 'Sizer'  # See GetControlSizer
     CurrentPage: 'Window'  # See GetCurrentPage
     PageCount: int  # See GetPageCount
     Selection: int  # See GetSelection and SetSelection
 
 
 
 class BookCtrlEvent(NotifyEvent):
@@ -11664,15 +11678,15 @@
     def DiffAsDateSpan(self, dt: 'DateTime') -> 'DateSpan':
         """ Returns the difference between this object and dt  as a   wx.DateSpan.
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     def Format(self, format=DefaultDateTimeFormat, tz=Local) -> str:
-        """ This function does the same as the standard ANSI C  strftime(3)   function (http://www.cplusplus.com/reference/clibrary/ctime/strftime.html).
+        """ This function does the same as the standard ANSI C  strftime(3)   function (https://cplusplus.com/reference/ctime/strftime/).
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     def FormatDate(self) -> str:
         """ Identical to calling Format   with  "%x"   argument (which means âpreferred date representation for the current localeâ).
 
@@ -14685,14 +14699,20 @@
     """
     def __init__(self, parent, message=FileSelectorPromptStr, defaultDir="", defaultFile="", wildcard=FileSelectorDefaultWildcardStr, style=FD_DEFAULT_STYLE, pos=DefaultPosition, size=DefaultSize, name=FileDialogNameStr) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.FileDialog.html
         """
 
+    def AddShortcut(self, directory, flags=0) -> bool:
+        """ Add a directory to the list of shortcuts shown in the dialog.
+
+            Source: https://docs.wxpython.org/wx.FileDialog.html
+        """
+
     @staticmethod
     def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.FileDialog.html
         """
 
@@ -19095,14 +19115,79 @@
 
 PD_ELAPSED_TIME: int  # This flag tells the dialog that it should show elapsed time (since creating the dialog).
 
 PD_ESTIMATED_TIME: int  # This flag tells the dialog that it should show estimated time.
 
 PD_REMAINING_TIME: int  # This flag tells the dialog that it should show remaining time. ^^
 
+class GenericStaticBitmap(Control):
+    """ A static bitmap control displays a bitmap.
+
+        Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+    """
+    def __init__(self, *args, **kw) -> None:
+        """ Overloaded Implementations:
+
+            Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+        """
+
+    def Create(self, parent, id=ID_ANY, bitmap=NullBitmap, pos=DefaultPosition, size=DefaultSize, style=0, name=StaticBitmapNameStr) -> bool:
+        """ Creation function, for two-step construction.
+
+            Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+        """
+
+    def GetBitmap(self) -> 'Bitmap':
+        """ Returns the bitmap currently used in the control.
+
+            Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+        """
+
+    @staticmethod
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
+        """ variant (WindowVariant) â
+
+            Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+        """
+
+    def GetIcon(self) -> 'Icon':
+        """ Returns the icon currently used in the control.
+
+            Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+        """
+
+    def GetScaleMode(self) -> 'ScaleMode':
+        """ Returns the scale mode currently used in the control.
+
+            Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+        """
+
+    def SetBitmap(self, label: 'BitmapBundle') -> None:
+        """ Sets the bitmap label.
+
+            Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+        """
+
+    def SetIcon(self, label: 'Icon') -> None:
+        """ Sets the label to the given icon.
+
+            Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+        """
+
+    def SetScaleMode(self, scaleMode: ScaleMode) -> None:
+        """ Sets the scale mode.
+
+            Source: https://docs.wxpython.org/wx.GenericStaticBitmap.html
+        """
+
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
+    Icon: '_Icon'  # See GetIcon and SetIcon
+
+
+
 class GestureEvent(Event):
     """ This is the base class for all supported gesture events.
 
         Source: https://docs.wxpython.org/wx.GestureEvent.html
     """
     def __init__(self, winid=0, type=wxEVT_NULL) -> None:
         """ Constructor.
@@ -25574,15 +25659,15 @@
 
     def GetNextItem(self, item, geometry=LIST_NEXT_ALL, state=LIST_STATE_DONTCARE) -> int:
         """ Searches for an item with the given geometry or state, starting from item  but excluding the item  itself.
 
             Source: https://docs.wxpython.org/wx.ListCtrl.html
         """
 
-    def GetNextSelected(self, item) -> None:
+    def GetNextSelected(self, item) -> int:
         """ Returns subsequent selected items, or -1 when no more are selected.
 
             Source: https://docs.wxpython.org/wx.ListCtrl.html
         """
 
     def GetSelectedItemCount(self) -> int:
         """ Returns the number of selected items in the list control.
@@ -25640,15 +25725,15 @@
 
     def HitTest(self, point) -> None:
         """ Determines which item (if any) is at the specified point, giving details in flags.
 
             Source: https://docs.wxpython.org/wx.ListCtrl.html
         """
 
-    def HitTestSubItem(*args, **kwargs) -> tuple:
+    def HitTestSubItem(self, point) -> tuple:
         """ Determines which item (if any) is at the specified point, giving details in flags.
 
             Source: https://docs.wxpython.org/wx.ListCtrl.html
         """
 
     def InReportView(self) -> bool:
         """ Returns True if the control is currently using LC_REPORT  style.
@@ -35666,15 +35751,15 @@
         """
 
     Orientation: int  # See GetOrientation and SetOrientation
     Position: int  # See GetPosition and SetPosition
 
 
 
-class SearchCtrl(TextCtrl):
+class SearchCtrl(Control,TextEntry):
     """ A search control is a composite control with a search button, a text
 control, and a cancel button.
 
         Source: https://docs.wxpython.org/wx.SearchCtrl.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -37886,15 +37971,15 @@
 
     def GetIcon(self) -> 'Icon':
         """ Returns the icon currently used in the control.
 
             Source: https://docs.wxpython.org/wx.StaticBitmap.html
         """
 
-    def GetScaleMode(self) -> 'StaticBitmap.ScaleMode':
+    def GetScaleMode(self) -> 'ScaleMode':
         """ Returns the scale mode currently used in the control.
 
             Source: https://docs.wxpython.org/wx.StaticBitmap.html
         """
 
     def SetBitmap(self, label: Union['Bitmap', 'BitmapBundle']) -> None:
         """ Sets the bitmap label.
@@ -38596,15 +38681,15 @@
 
 
 SVG_SHAPE_RENDERING_AUTO: int
 
 class SysColourChangedEvent(Event):
     """ This class is used for system colour change events, which are
 generated when the user changes the colour settings or when the system
-theme changes (e.g.
+theme changes (e.g. automatic dark mode switching on macOS).
 
         Source: https://docs.wxpython.org/wx.SysColourChangedEvent.html
     """
     def __init__(self) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.SysColourChangedEvent.html
@@ -39973,14 +40058,81 @@
         """ Saves an image in the output stream.
 
             Source: https://docs.wxpython.org/wx.TGAHandler.html
         """
 
 
 
+class ThreadEvent(Event):
+    """ This class adds some simple functionality to Event to facilitate
+inter-thread communication.
+
+        Source: https://docs.wxpython.org/wx.ThreadEvent.html
+    """
+    def __init__(self, eventType=wxEVT_THREAD, id=ID_ANY) -> None:
+        """ Constructor.
+
+            Source: https://docs.wxpython.org/wx.ThreadEvent.html
+        """
+
+    def Clone(self) -> 'Event':
+        """ Clones this event making sure that all internal members which use COW (only  m_commandString   for now; see  Reference Counting) are unshared (see wx.Object.UnShare ).
+
+            Source: https://docs.wxpython.org/wx.ThreadEvent.html
+        """
+
+    def GetEventCategory(self) -> int:
+        """ Returns  wxEVT_CATEGORY_THREAD .
+
+            Source: https://docs.wxpython.org/wx.ThreadEvent.html
+        """
+
+    def GetExtraLong(self) -> int:
+        """ Returns extra information integer value.
+
+            Source: https://docs.wxpython.org/wx.ThreadEvent.html
+        """
+
+    def GetInt(self) -> int:
+        """ Returns stored integer value.
+
+            Source: https://docs.wxpython.org/wx.ThreadEvent.html
+        """
+
+    def GetString(self) -> str:
+        """ Returns stored string value.
+
+            Source: https://docs.wxpython.org/wx.ThreadEvent.html
+        """
+
+    def SetExtraLong(self, extraLong: int) -> None:
+        """ Sets the extra information value.
+
+            Source: https://docs.wxpython.org/wx.ThreadEvent.html
+        """
+
+    def SetInt(self, intCommand: int) -> None:
+        """ Sets the integer value.
+
+            Source: https://docs.wxpython.org/wx.ThreadEvent.html
+        """
+
+    def SetString(self, string: str) -> None:
+        """ Sets the string value.
+
+            Source: https://docs.wxpython.org/wx.ThreadEvent.html
+        """
+
+    EventCategory: int  # See GetEventCategory
+    ExtraLong: int  # See GetExtraLong and SetExtraLong
+    Int: int  # See GetInt and SetInt
+    String: str  # See GetString and SetString
+
+
+
 class TIFFHandler(ImageHandler):
     """ This is the image handler for the TIFF format.
 
         Source: https://docs.wxpython.org/wx.TIFFHandler.html
     """
     def __init__(self) -> None:
         """ Default constructor for   wx.TIFFHandler.
```

### Comparing `types_wxpython-0.7.1/wx-stubs/adv/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/adv/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/aui/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/aui/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/dataview/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/dataview/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
 
 EVT_DATAVIEW_ITEM_VALUE_CHANGED: int  # Process a  wxEVT_DATAVIEW_ITEM_VALUE_CHANGED   event.
 
 EVT_DATAVIEW_ITEM_CONTEXT_MENU: int  # Process a  wxEVT_DATAVIEW_ITEM_CONTEXT_MENU   event generated when the user right clicks inside the control. Notice that this menu is generated even if the click didnât occur on any valid item, in this case  wx.dataview.DataViewEvent.GetItem   simply returns an invalid item.
 
 EVT_DATAVIEW_COLUMN_HEADER_CLICK: int  # Process a  wxEVT_DATAVIEW_COLUMN_HEADER_CLICK   event.
 
-EVT_DATAVIEW_COLUMN_HEADER_RIGHT_CLICK: int  # Process a  wxEVT_DATAVIEW_COLUMN_HEADER_RIGHT_CLICK   event. Notice that currently this event is not generated in the native macOS versions of the control.
+EVT_DATAVIEW_COLUMN_HEADER_RIGHT_CLICK: int  # Process a  wxEVT_DATAVIEW_COLUMN_HEADER_RIGHT_CLICK   event.
 
 EVT_DATAVIEW_COLUMN_SORTED: int  # Process a  wxEVT_DATAVIEW_COLUMN_SORTED   event.
 
 EVT_DATAVIEW_COLUMN_REORDERED: int  # Process a  wxEVT_DATAVIEW_COLUMN_REORDERED   event.
 
 EVT_DATAVIEW_ITEM_BEGIN_DRAG: int  # Process a  wxEVT_DATAVIEW_ITEM_BEGIN_DRAG   event which is generated when the user starts dragging a valid item. This event must be processed and  wx.dataview.DataViewEvent.SetDataObject   must be called to actually start dragging the item.
```

### Comparing `types_wxpython-0.7.1/wx-stubs/glcanvas/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/glcanvas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/grid/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/grid/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1246,14 +1246,20 @@
 
     def RefreshAttr(self, row, col) -> None:
         """ Invalidates the cached attribute for the given cell.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
+    def RefreshBlock(self, *args, **kw) -> None:
+        """ Overloaded Implementations:
+
+            Source: https://docs.wxpython.org/wx.grid.Grid.html
+        """
+
     def RegisterDataType(self, typeName, renderer, editor) -> None:
         """ Register a new data type.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def Render(*args, **kwargs) -> None:
@@ -3213,15 +3219,15 @@
 
 EVT_GRID_LABEL_LEFT_DCLICK: int  # The user double-clicked a label with the left mouse button. Processes a  wxEVT_GRID_LABEL_LEFT_DCLICK   event type.
 
 EVT_GRID_LABEL_RIGHT_CLICK: int  # The user clicked a label with the right mouse button. Processes a  wxEVT_GRID_LABEL_RIGHT_CLICK   event type.
 
 EVT_GRID_LABEL_RIGHT_DCLICK: int  # The user double-clicked a label with the right mouse button. Processes a  wxEVT_GRID_LABEL_RIGHT_DCLICK   event type.
 
-EVT_GRID_SELECT_CELL: int  # The given cell was made current, either by user or by the program via a call to SetGridCursor() or GoToCell(). Processes a  wxEVT_GRID_SELECT_CELL   event type.
+EVT_GRID_SELECT_CELL: int  # The given cell is about to be made current, either by user or by the program via a call to wx.grid.Grid.SetGridCursor   or wx.grid.Grid.GoToCell . The event can be vetoed to prevent this from happening and wx.grid.Grid.GetGridCursorCoords   still returns the previous current cell coordinates during the event handler execution, while the new ones are available via the event object GetRow  and GetCol  functions. Processes a  wxEVT_GRID_SELECT_CELL   event type.
 
 EVT_GRID_ROW_MOVE: int  # The user tries to change the order of the rows in the grid by dragging the row specified by GetRow. This event can be vetoed to either prevent the user from reordering the row change completely (but notice that if you donât want to allow it at all, you simply shouldnât call wx.grid.Grid.EnableDragRowMove   in the first place), vetoed but handled in some way in the handler, e.g. by really moving the row to the new position at the associated table level, or allowed to proceed in which case wx.grid.Grid.SetRowPos   is used to reorder the rows display order without affecting the use of the row indices otherwise. This event macro corresponds to  wxEVT_GRID_ROW_MOVE   event type. It is only available since wxWidgets 3.1.7.
 
 EVT_GRID_COL_MOVE: int  # The user tries to change the order of the columns in the grid by dragging the column specified by GetCol. This event can be vetoed to either prevent the user from reordering the column change completely (but notice that if you donât want to allow it at all, you simply shouldnât call wx.grid.Grid.EnableDragColMove   in the first place), vetoed but handled in some way in the handler, e.g. by really moving the column to the new position at the associated table level, or allowed to proceed in which case wx.grid.Grid.SetColPos   is used to reorder the columns display order without affecting the use of the column indices otherwise. This event macro corresponds to  wxEVT_GRID_COL_MOVE   event type.
 
 EVT_GRID_COL_SORT: int  # This event is generated when a column is clicked by the user and its name is explained by the fact that the custom reaction to a click on a column is to sort the grid contents by this column. However the grid itself has no special support for sorting and itâs up to the handler of this event to update the associated table. But if the event is handled (and not vetoed) the grid supposes that the table was indeed resorted and updates the column to indicate the new sort order and refreshes itself. This event macro corresponds to  wxEVT_GRID_COL_SORT   event type.
 
@@ -3958,7 +3964,27 @@
 
 GridWindow: TypeAlias = Any
 
 GridCellAttrPtr: TypeAlias = Any
 
 TabBehaviour: TypeAlias = int  # Enumeration
 
+GRID_VALUE_STRING: str
+
+GRID_VALUE_BOOL: str
+
+GRID_VALUE_NUMBER: str
+
+GRID_VALUE_FLOAT: str
+
+GRID_VALUE_CHOICE: str
+
+GRID_VALUE_DATE: str
+
+GRID_VALUE_TEXT: str
+
+GRID_VALUE_LONG: str
+
+GRID_VALUE_CHOICEINT: str
+
+GRID_VALUE_DATETIME: str
+
```

### Comparing `types_wxpython-0.7.1/wx-stubs/html/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/html/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/html2/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/html2/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
 
 EVT_WEBVIEW_ERROR: int  # Process a  wxEVT_WEBVIEW_ERROR   event generated when a navigation error occurs. The integer associated with this event will be a WebNavigationError item. The string associated with this event may contain a backend-specific more precise error message/code.
 
 EVT_WEBVIEW_NEWWINDOW: int  # Process a  wxEVT_WEBVIEW_NEWWINDOW   event, generated when a new window is created. You must handle this event if you want anything to happen, for example to load the page in a new window or tab.
 
 EVT_WEBVIEW_TITLE_CHANGED: int  # Process a  wxEVT_WEBVIEW_TITLE_CHANGED   event, generated when the page title changes. Use GetString to get the title.
 
-EVT_WEBVIEW_FULL_SCREEN_CHANGED: int  # Process a  EVT_WEBVIEW_FULL_SCREEN_CHANGED   event, generated when the page wants to enter or leave fullscreen. Use GetInt to get the status. Not implemented for the IE backend and is only available in wxWidgets 3.1.5 or later.
+EVT_WEBVIEW_FULLSCREEN_CHANGED: int  # Process a  wxEVT_WEBVIEW_FULLSCREEN_CHANGED   event, generated when the page wants to enter or leave fullscreen. Use GetInt to get the status. Not implemented for the IE backend and is only available in wxWidgets 3.1.5 or later.
 
 EVT_WEBVIEW_SCRIPT_MESSAGE_RECEIVED: int  # Process a  wxEVT_WEBVIEW_SCRIPT_MESSAGE_RECEIVED   event only available in wxWidgets 3.1.5 or later. For usage details see  AddScriptMessageHandler.
 
 wxEVT_WEBVIEW_SCRIPT_RESULT: int  # Process a  wxEVT_WEBVIEW_SCRIPT_RESULT   event only available in wxWidgets 3.1.6 or later. For usage details see  RunScriptAsync. ^^
 
 WEBVIEW_INJECT_AT_DOCUMENT_START: int
```

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/buttonbar/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/buttonbar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/gallery/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/gallery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/agw/ribbon/toolbar/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/agw/ribbon/toolbar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/buttons/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/buttons/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/calendar/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/calendar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/colourselect/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/colourselect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/dialogs/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/dialogs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/scrolledpanel/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/scrolledpanel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/lib/wxpTag/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/lib/wxpTag/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/media/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/media/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/propgrid/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/propgrid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/ribbon/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/ribbon/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/richtext/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/richtext/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/stc/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/stc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/xml/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/xml/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.7.1/wx-stubs/xrc/__init__.pyi` & `types_wxpython-0.7.2/wx-stubs/xrc/__init__.pyi`

 * *Files identical despite different names*

