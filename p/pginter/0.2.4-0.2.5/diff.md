# Comparing `tmp/pginter-0.2.4.tar.gz` & `tmp/pginter-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pginter-0.2.4.tar", last modified: Thu Jun  1 19:06:29 2023, max compression
+gzip compressed data, was "pginter-0.2.5.tar", last modified: Tue Jun 13 14:29:47 2023, max compression
```

## Comparing `pginter-0.2.4.tar` & `pginter-0.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.790060 pginter-0.2.4/
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.4/LICENSE
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.4/MANIFEST.in
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-01 19:06:29.790060 pginter-0.2.4/PKG-INFO
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.4/README.md
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.4/pyproject.toml
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-01 19:06:29.790060 pginter-0.2.4/setup.cfg
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-05-31 21:17:56.000000 pginter-0.2.4/setup.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.780060 pginter-0.2.4/src/
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.780060 pginter-0.2.4/src/pginter/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    21906 2023-06-01 19:00:08.000000 pginter-0.2.4/src/pginter/_pg_root.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/icon.png
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.783393 pginter-0.2.4/src/pginter/theme/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/theme/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.4/src/pginter/theme/_manager.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.783393 pginter-0.2.4/src/pginter/theme/themes/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      663 2023-05-25 20:39:17.000000 pginter-0.2.4/src/pginter/theme/themes/default.json
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.786726 pginter-0.2.4/src/pginter/types/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.4/src/pginter/types/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/types/_better_dict.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.4/src/pginter/types/_binds.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.4/src/pginter/types/_color.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.4/src/pginter/types/_constants.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.4/src/pginter/types/_geo_types.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.4/src/pginter/types/_notifications.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.4/src/pginter/types/_scheme.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.4/src/pginter/types/_style.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.4/src/pginter/types/_tk_vars.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.786726 pginter-0.2.4/src/pginter/utils/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.4/src/pginter/utils/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.4/src/pginter/utils/_funcs.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.790060 pginter-0.2.4/src/pginter/widgets/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.4/src/pginter/widgets/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.4/src/pginter/widgets/_button.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.4/src/pginter/widgets/_entry.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26515 2023-05-31 20:53:29.000000 pginter-0.2.4/src/pginter/widgets/_frame.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.4/src/pginter/widgets/_geo_manager.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.4/src/pginter/widgets/_label.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/widgets/_supports_children.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.4/src/pginter/widgets/_surface_frame.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.783393 pginter-0.2.4/src/pginter.egg-info/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/PKG-INFO
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1028 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/SOURCES.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/dependency_links.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/requires.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/top_level.txt
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.682923 pginter-0.2.5/
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.5/LICENSE
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.5/MANIFEST.in
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-13 14:29:47.682923 pginter-0.2.5/PKG-INFO
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.5/README.md
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.5/pyproject.toml
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-13 14:29:47.682923 pginter-0.2.5/setup.cfg
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-06-01 19:06:50.000000 pginter-0.2.5/setup.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.676256 pginter-0.2.5/src/
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.676256 pginter-0.2.5/src/pginter/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     8707 2023-06-01 19:29:58.000000 pginter-0.2.5/src/pginter/_pg_root.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/icon.png
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter/theme/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/theme/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.5/src/pginter/theme/_manager.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter/theme/themes/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      673 2023-06-01 19:26:32.000000 pginter-0.2.5/src/pginter/theme/themes/default.json
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter/types/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.5/src/pginter/types/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/types/_better_dict.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.5/src/pginter/types/_binds.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.5/src/pginter/types/_color.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.5/src/pginter/types/_constants.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.5/src/pginter/types/_geo_types.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.5/src/pginter/types/_notifications.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.5/src/pginter/types/_scheme.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.5/src/pginter/types/_style.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.5/src/pginter/types/_tk_vars.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter/utils/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.5/src/pginter/utils/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.5/src/pginter/utils/_funcs.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.682923 pginter-0.2.5/src/pginter/widgets/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.5/src/pginter/widgets/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.5/src/pginter/widgets/_button.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.5/src/pginter/widgets/_entry.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    28167 2023-06-13 14:28:55.000000 pginter-0.2.5/src/pginter/widgets/_frame.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.5/src/pginter/widgets/_geo_manager.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.5/src/pginter/widgets/_label.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/widgets/_supports_children.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.5/src/pginter/widgets/_surface_frame.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter.egg-info/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/PKG-INFO
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1028 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/SOURCES.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/dependency_links.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/requires.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/top_level.txt
```

### Comparing `pginter-0.2.4/LICENSE` & `pginter-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/setup.py` & `pginter-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pginter",
-    version="0.2.4",
+    version="0.2.5",
     author="Nilusink",
     author_email="nilusink@protonmail.com",
     description="A python GUI interface, based on pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nilusink/PgInter",
     # project_urls={
```

### Comparing `pginter-0.2.4/src/pginter/_pg_root.py` & `pginter-0.2.5/src/pginter/widgets/_geo_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,599 +1,768 @@
 """
-_pg_root.py
+_geo_manager.py
 04. February 2023
 
-the root of the window
+How children are placed
 
 Author:
 Nilusink
 """
-from concurrent.futures import ThreadPoolExecutor as Pool, Future
-from .widgets import GeometryManager
-from .theme import ThemeManager
-from time import perf_counter
+from ..types import Layout, BetterDict, TOP, BOTTOM, LEFT, RIGHT, GeoNotes
+from ._supports_children import SupportsChildren
+from ..utils import point_in_box
 from copy import deepcopy
-from .types import *
 import typing as tp
 import pygame as pg
-import os.path
 
 
-DEFAULT_TITLE: str = "Window"
-DEFAULT_ICON: str = os.path.dirname(__file__) + "/icon.png"
+if tp.TYPE_CHECKING:
+    from ._frame import Frame
 
 
-RES_T = tp.TypeVar("RES_T")
-
-
-class _TimeoutCandidate(tp.TypedDict):
-    timeout_left: float
-    function: tp.Callable[[tp.Any], RES_T]
-    future: Future[RES_T]
-    args: tuple[tp.Any, ...]
-    kwargs: dict[str, tp.Any]
-
-
-class PgRoot(GeometryManager):
-    _focus_item: GeometryManager | None = None
-    _running: bool = True
-    _theme: ThemeManager = ...
-    __background: pg.Surface = ...
+class GeometryManager(SupportsChildren):
+    """
+    Manages how children are placed inside a parent container
+    """
+    _layout: Layout = Layout.Absolute
+    _width: float = 0   # -1 means not configured -> takes minimum size
+    # required by its children
+    _height: float = 0  # or the size it gets by the parents geometry manager
+    assigned_width: float = 0
+    assigned_height: float = 0
+    _width_configured: bool = False
+    _height_configured: bool = False
+    _child_params: list[tuple[tp.Any, BetterDict]] = ...
     layout_params: BetterDict = ...
-    _min_size: tuple[int, int] = ...
-    _bg_configured: bool = False
-    _mouse_pos: tuple[int, int] = ...
-    _max_framerate: int = ...
-
-    __timeouts: list[_TimeoutCandidate]
-    _last_it_call: float
-    _tpool: Pool
+    _grid_params: BetterDict = ...
 
-    show_wireframe: bool = False
+    _child_override: bool = False
+    _is_active: bool = False
+    _is_hover: bool = False
+
+    _last_rows: list[dict[
+        str,
+        list[tuple[tp.Any, BetterDict, bool]] | float
+    ]] = ...
+    _last_columns: list[dict[
+        str,
+        list[tuple[tp.Any, BetterDict, bool]] | float
+    ]] = ...
 
     def __init__(
             self,
-            title: str = ...,
-            icon_path: str = ...,
-            size: tuple[int, int] = ...,
-            bg_color: Color = ...,
-            padding: int = 0,
+            layout: Layout = ...,
             margin: int = 0,
-            max_framerate: int = 30
+            padding: int = 0
     ):
-        self._last_it_call = perf_counter()
-        self._max_framerate = max_framerate
-        self._tpool = Pool(max_workers=10)
-        self.__timeouts = []
-
         super().__init__()
-        self._theme = ThemeManager()
-        self._theme.notify_on(ThemeManager.NotifyEvent.theme_reload, self.notify)
-        self._min_size = (0, 0)
-
-        # args
-        self._bg_configured = bg_color is not ...
-        self._bg = self._theme.root.bg.hex if bg_color is ... else bg_color
 
-        self._layout_params = BetterDict({
-            "padding": padding,
+        if layout is not ...:
+            if layout not in (Layout.Grid, Layout.Pack, Layout.Absolute):
+                raise ValueError(f"Invalid layout type: {layout}")
+
+        self._layout = Layout.Absolute if layout is ... else layout
+        self.layout_params = BetterDict({
             "margin": margin,
+            "padding": padding
+        })
+        self._child_params = []
+        self._grid_params = BetterDict({
+            "rows": {},
+            "columns": {}
         })
 
-        # pg init
-        pg.init()
-        pg.font.init()
-        self._clk = pg.time.Clock()
-
-        if size is not ...:
-            self.__background = pg.display.set_mode(size, flags=pg.RESIZABLE)
-
-        else:
-            self.__background = pg.display.set_mode(flags=pg.RESIZABLE)
-
-        # set icon and caption
-        pg.display.set_caption(DEFAULT_TITLE if title is ... else title)
-        img = pg.image.load(
-            DEFAULT_ICON if icon_path is ... else icon_path, "icon"
-        )
-        pg.display.set_icon(img)
-
-    # config
     @property
-    def title(self) -> str:
-        return pg.display.get_caption()[0]
-
-    @title.setter
-    def title(self, value: str) -> None:
-        pg.display.set_caption(value)
+    def layout(self) -> Layout:
+        """
+        the containers layout type
+        """
+        return self._layout
 
     @property
-    def theme(self) -> ThemeManager:
-        return self._theme
+    def width(self) -> float:
+        return self._width
+    
+    @width.setter
+    def width(self, value: float) -> None:
+        self._width = value
+        self._width_configured = True
 
-    @property
-    def mouse_pos(self) -> tuple[int, int]:
-        return self._mouse_pos
+    def unset_width(self) -> None:
+        """
+        act as if the width has never been set
+        """
+        self._width_configured = False
 
     @property
-    def root(self) -> tp.Self:
-        return self
+    def height(self) -> float:
+        return self._height
 
-    @property
-    def _height_configured(self) -> bool:
-        return True
+    @height.setter
+    def height(self, value: float) -> None:
+        self._height = value
+        self._height_configured = True
+
+    def unset_height(self) -> None:
+        """
+        act as if the height has never been set
+        """
+        self._height_configured = False
 
     @property
-    def _width_configured(self) -> bool:
-        return True
+    def is_hover(self) -> bool:
+        return self._is_hover
 
     @property
-    def _height(self) -> int:
-        return pg.display.get_window_size()[1]
+    def is_active(self) -> bool:
+        return self._is_active
 
-    @_height.setter
-    def _height(self, *_) -> None:
+    def set_focus(self, widget: tp.Union["GeometryManager", None]):
         """
-        value should not be set, but no error should occur
+        set this item as currently focused
         """
-        pass
 
-    @property
-    def _width(self) -> int:
-        return pg.display.get_window_size()[0]
+    def stop_focus(self):
+        """
+        remove focus from this item
+        """
 
-    @_width.setter
-    def _width(self, *_) -> None:
+    def _on_active(self) -> None:
         """
-        value should not be set, but no error should occur
+        called when button is clicked
+        not implemented by default
         """
-        pass
 
-    def get_focus(self) -> GeometryManager | None:
+    def _on_hover(self) -> None:
         """
-        get the currently focused item
+        called on hover
+        not implemented by default
         """
-        return self._focus_item
 
-    def set_focus(
+    def _on_no_active_hover(
             self,
-            widget: tp.Union["GeometryManager", None, tp.Any] = None
+            from_active: bool = False,
+            from_hover: bool = False
     ) -> None:
         """
-        set the focused item
+        called when either hover or active goes back to normal
+        not implemented by default
         """
-        if self._focus_item is not None:
-            self._focus_item.stop_focus()
 
-        if widget is not None:
-            widget.set_focus()
-            self._focus_item = widget
+    def set_active(self, override: bool = False) -> None:
+        """
+        change the widget to an active state
+        """
+        if not self._child_override:
+            if not self._is_active:  # only call on new event
+                self._on_active()
+
+            self._is_hover = False
+            self._is_active = True
 
-    def notify_focus(self, widget: tp.Union["GeometryManager", None] = None):
+        self._child_override = self._child_override or override
+
+    def set_hover(self, override: bool = False) -> None:
         """
-        notify the root that a widget has been set as focus
+        set the widget to a hover state
         """
-        if self._focus_item != widget:
-            self.set_focus(widget)
+        if not self._child_override:
+            if not self._is_hover:  # only call on new event
+                self._on_hover()
+
+            self._is_hover = True
+            self._is_active = False
 
-    # interfacing
-    def notify(self, event: ThemeManager.NotifyEvent, _info=...) -> None:
+        self._child_override = self._child_override or override
+
+    def set_no_hover_active(self, override: bool = False) -> None:
         """
-        gets called by another class
+        set the widget to "normal" mode
         """
+        if not self._child_override:
+            if self._is_hover or self._is_active:  # only call no new event
+                self._on_no_active_hover(self._is_active, self._is_hover)
+
+            self._is_hover = False
+            self._is_active = False
+
+        self._child_override = self._child_override or override
+
+    def _notify_child_active_hover(self, mouse_pos: tuple[int, int]) -> bool:
+        has_hit: bool = False
+
+        for child in self._children:
+            child: Frame
+
+            pos = child.get_position()
+            size = child.get_size()
+
+            # noinspection PyTypeChecker
+            if point_in_box(mouse_pos, (*pos, *size)):
+                has_hit = True
+                child.notify(
+                    GeoNotes.SetActive if pg.mouse.get_pressed(3)[0]
+                    else GeoNotes.SetHover,
+                    (mouse_pos[0] - pos[0], mouse_pos[1] - pos[1])
+                )
+                continue
+
+            child.notify(GeoNotes.SetNormal)
+
+        return has_hit
+
+    def notify(self, event, info) -> None:
+        """
+        for notifications from child / parent classes
+        """
+        self._child_override = False
         match event:
-            case ThemeManager.NotifyEvent.theme_reload:
-                # the theme has been reloaded
-                if not self._bg_configured:
-                    self._bg = self.theme.root.bg.rgba
-
-    # pygame stuff
-    def _event_handler(self) -> None:
-        """
-        handle the events raised by pygame
-        """
-        for event in pg.event.get():
-            match event.type:
-                case pg.QUIT:
-                    self._running = False
-
-                case pg.KEYDOWN:
-                    if self._focus_item is not None:
-                        self._focus_item.notify(
-                            KeyboardNotifyEvent.key_down,
-                            event
-                        )
-
-                case pg.KEYUP:
-                    if self._focus_item is not None:
-                        self._focus_item.notify(
-                            KeyboardNotifyEvent.key_up,
-                            event
-                        )
-
-                # case pg.VIDEORESIZE:  # window size changed
-                #     width, height = event.size
-                #
-                #     print("updating size: ", (width, height), "\t", self._min_size)
-                #
-                #     width = max([width, self._min_size[0]])
-                #     height = max([height, self._min_size[1]])
-                #
-                #     # self.__background = pg.display.set_mode((width, height), flags=pg.RESIZABLE | pg.HWSURFACE | pg.DOUBLEBUF)
-
-        self._mouse_pos = pg.mouse.get_pos()
-
-        self._notify_child_active_hover(self.mouse_pos)
-
-    def update_idletasks(self) -> None:
-        """
-        updates all the functional tasks
-        """
-        self._event_handler()
-
-        # handle timeouts
-        for to in self.__timeouts.copy():
-            # calculate time since last function call
-            now = perf_counter()
-            delta = now - self._last_it_call
-            self._last_it_call = now
-
-            # remove time from timeout
-            to["timeout_left"] -= delta * 1000
-
-            # if the timeout is finished, execute the function
-            if to["timeout_left"] <= 0:
-                # create a function that populates the timeout future's result
-                # with the function return value
-                def curr_func():
-                    to["future"].set_result(to["function"](
-                        *to["args"], **to["kwargs"]
-                    ))
-
-                # submit the created function to the threadpool
-                # and remove it from the active timeouts
-                self._tpool.submit(curr_func)
-                self.__timeouts.remove(to)
+            case GeoNotes.SetHover:
+                if self._notify_child_active_hover(info):
+                    self.set_no_hover_active()
+                else:
+                    self.set_hover()
+
+            case GeoNotes.SetActive:
+                if self._notify_child_active_hover(info):
+                    self.set_no_hover_active()
+                else:
+                    self.set_active()
 
-    def update(self) -> None:
+            case GeoNotes.SetNormal:
+                # also set children to inactive
+                self._notify_child_active_hover((-1, -1))
+
+                self.set_no_hover_active()
+
+    # layout configuration
+    def set_layout(self, layout: Layout) -> None:
         """
-        update the screen
+        set the container's layout type
         """
-        self.__background.fill(self._bg)
+        if layout not in Layout:
+            raise ValueError("Invalid container layout: ", layout)
 
-        self.calculate_geometry()
-        for child, params in self._child_params:
-            child.draw(self.__background)
+        if self._layout != layout:
+            if len(self._child_params) > 0:
+                # if children are already present, delete them
+                for child, _param in self._child_params:
+                    child.delete()
+
+                self._child_params.clear()
 
-        pg.display.flip()
+                raise RuntimeWarning(
+                    "changing layout with children already present!"
+                )
 
-    def mainloop(self):
+            self._layout = layout
+
+    def check_set_layout(self, layout: Layout) -> bool:
         """
-        run the windows main loop
+        checks if the layout can be changed
         """
-        while self._running:
-            self.update_idletasks()
-            self.update()
-
-            self._clk.tick(self._max_framerate)
-
-    # def calculate_geometry(self):
-    #     """
-    #     calculate how each individual child should be placed
-    #     """
-    #     match self._layout:
-    #         case Layout.Absolute:  # Absolute
-    #             # since the positioning is absolute, the children should not influence the parents size
-    #             for child, params in self._child_params:
-    #                 child.set_position(params.x, params.y)
-    #
-    #             return
-    #
-    #         case Layout.Pack:
-    #             directional_dict: dict[str, int | list] = {"total_x": 0, "total_y": 0, "children": [], "sizes": []}
-    #             top = deepcopy(directional_dict)
-    #             bottom = deepcopy(directional_dict)
-    #             left = deepcopy(directional_dict)
-    #             right = deepcopy(directional_dict)
-    #
-    #             # get all sizes and group by anchor
-    #             for child, param in self._child_params:
-    #                 child_size = child.calculate_size()
-    #
-    #                 if param.anchor == TOP:
-    #                     top["children"].append(child)
-    #                     top["sizes"].append(child_size)
-    #                     top["total_x"] += child_size[0]
-    #                     top["total_y"] += child_size[1]
-    #
-    #                 elif param.anchor == BOTTOM:
-    #                     bottom["children"].append(child)
-    #                     bottom["sizes"].append(child_size)
-    #                     bottom["total_x"] += child_size[0]
-    #                     bottom["total_y"] += child_size[1]
-    #
-    #                 elif param.anchor == LEFT:
-    #                     left["children"].append(child)
-    #                     left["sizes"].append(child_size)
-    #                     left["total_x"] += child_size[0]
-    #                     left["total_y"] += child_size[1]
-    #
-    #                 elif param.anchor == RIGHT:
-    #                     right["children"].append(child)
-    #                     right["sizes"].append(child_size)
-    #                     right["total_x"] += child_size[0]
-    #                     right["total_y"] += child_size[1]
-    #
-    #             top["total_y"] += self._layout_params.padding * len(top["children"]) - 1
-    #             bottom["total_y"] += self._layout_params.padding * len(bottom["children"]) - 1
-    #
-    #             left["total_x"] += self._layout_params.padding * len(left["children"]) - 1
-    #             right["total_x"] += self._layout_params.padding * len(right["children"]) - 1
-    #
-    #             min_x = max([top["total_x"], bottom["total_x"], left["total_x"] + right["total_x"]])
-    #             min_y = max([left["total_y"], right["total_y"], top["total_y"] + bottom["total_y"]])
-    #
-    #             # add margin
-    #             min_x += self.layout_params.margin * 2
-    #             min_y += self.layout_params.margin * 2
-    #
-    #             self._min_size = min_x, min_y
-    #
-    #             total_x, total_y = self.calculate_size()
-    #
-    #             # tell the children where they should be
-    #             y_cen = total_y / 2
-    #             x_cen = total_x / 2
-    #
-    #             # left
-    #             x_now = self._layout_params.margin
-    #             for child, size in zip(left["children"], left["sizes"]):
-    #                 child.set_position(x_now, y_cen - size[1] / 2)
-    #                 x_now += size[0] + self._layout_params.padding
-    #
-    #                 # right
-    #             x_now = total_x - self._layout_params.margin
-    #             for child, size in zip(right["children"], right["sizes"]):
-    #                 child.set_position(x_now - size[0], y_cen - size[1] / 2)
-    #                 x_now -= size[0] + self._layout_params.padding
-    #
-    #                 # top
-    #             y_now = self._layout_params.margin
-    #             for child, size in zip(top["children"], top["sizes"]):
-    #                 child.set_position(x_cen - size[0] / 2, y_now)
-    #                 y_now += size[1] + self._layout_params.padding
-    #
-    #                 # bottom
-    #             y_now = total_y - self._layout_params.margin
-    #             for child, size in zip(bottom["children"], bottom["sizes"]):
-    #                 child.set_position(x_cen - size[0] / 2, y_now - size[1])
-    #                 y_now -= size[1] + self._layout_params.padding
-    #
-    #         case Layout.Grid:
-    #             rows: list[dict[str, tp.Any | float]] = []
-    #             columns: list[dict[str, tp.Any | float]] = []
-    #
-    #             for child, params in self._child_params:
-    #                 row, column = params["row"], params["column"]
-    #
-    #                 # if row was not yet made, make all previous ones
-    #                 if len(rows) <= row:
-    #                     for n_row in range(len(rows), row + 1):
-    #                         out = {
-    #                             "weight": 0,
-    #                             "children": []
-    #                         }
-    #
-    #                         if n_row in self._grid_params.rows:
-    #                             config = self._grid_params.rows[n_row]
-    #
-    #                             if "weight" in config:
-    #                                 out["weight"] = config["weight"]
-    #
-    #                         rows.append(out)
-    #
-    #                 if len(columns) <= column:
-    #                     for n_col in range(len(columns), column + 1):
-    #                         out = {
-    #                             "weight": 0,
-    #                             "children": []
-    #                         }
-    #
-    #                         if n_col in self._grid_params.columns:
-    #                             config = self._grid_params.columns[n_col]
-    #
-    #                             if "weight" in config:
-    #                                 out["weight"] = config["weight"]
-    #
-    #                         columns.append(out)
-    #
-    #                 rows[row]["children"].append((child, params))
-    #                 columns[column]["children"].append((child, params))
-    #
-    #             matrix: list[list] = []
-    #
-    #             for r in range(len(rows)):
-    #                 matrix.append([])
-    #
-    #                 for c in range(len(columns)):
-    #                     # child = set(rows[r]["children"]) & set(columns[c]["children"])
-    #                     child = [chi for chi in rows[r]["children"] if chi in columns[c]["children"]]
-    #                     child = list(child)
-    #
-    #                     if len(child) > 1:
-    #                         raise ValueError(f"{len(child)} children assigned to row {r} column {c}!")
-    #
-    #                     if child:
-    #                         matrix[r].append(child[0])
-    #
-    #                     else:
-    #                         matrix[r].append(...)
-    #
-    #             # calculate the minimal size for each row
-    #             for r, row in enumerate(rows):
-    #                 rows[r]["max_size"] = 0
-    #
-    #                 for child, params in row["children"]:
-    #                     _, y = child.calculate_size()
-    #
-    #                     y += 2 * params.margin
-    #
-    #                     if y > rows[r]["max_size"]:
-    #                         rows[r]["max_size"] = y
-    #
-    #             # calculate the minimal size for each column
-    #             for c, column in enumerate(columns):
-    #                 columns[c]["max_size"] = 0
-    #
-    #                 for child, params in column["children"]:
-    #                     x, _ = child.calculate_size()
-    #
-    #                     x += 2 * params.margin
-    #
-    #                     if x > columns[c]["max_size"]:
-    #                         columns[c]["max_size"] = x
-    #
-    #                 # calculate the container size
-    #             width, height = self.calculate_size()
-    #
-    #             # only subtract rows that don't have a weight
-    #             min_width = sum([c["max_size"] for c in columns])
-    #             min_height = sum([r["max_size"] for r in rows])
-    #
-    #             # set the windows minimal size
-    #             self._min_size = min_width, min_height
-    #
-    #             # assign extra space
-    #             extra_width = width - sum([c["max_size"] for c in columns if c["weight"] == 0])
-    #             extra_height = height - sum([r["max_size"] for r in rows if r["weight"] == 0])
-    #
-    #             total_row_weight = sum([row["weight"] for row in rows])
-    #             total_column_weight = sum([column["weight"] for column in columns])
-    #
-    #             # print(f"\n\nwindow_size=[{width}, {height}]\tmin_size={[min_width, min_height]}")
-    #             # print(f"{total_row_weight=}")
-    #             # print(f"{total_column_weight=}")
-    #             # print(f"{extra_height=}")
-    #             # print(f"{extra_width=}")
-    #
-    #             # assign each row and column a specific size
-    #             for r in range(len(rows)):
-    #                 if total_row_weight == 0:
-    #                     rows[r]["height"] = 0
-    #                 else:
-    #                     # assign either the minimum size or the calculated dynamic one
-    #                     w_size = ((rows[r]["weight"] / total_row_weight) * extra_height).__floor__()
-    #                     rows[r]["height"] = max([w_size, rows[r]["max_size"]])
-    #                     # print(f"{w_size=}\t{rows[r]['max_size']=}")
-    #
-    #                 # rows[r]["height"] += rows[r]["max_size"]
-    #                 rows[r]["y_start"] = sum([prev_row["height"] for prev_row in rows[:r]])
-    #
-    #                 for c in range(len(columns)):
-    #                     if total_column_weight == 0:
-    #                         columns[c]["width"] = 0
-    #                     else:
-    #                         # assign either the minimum size or the calculated dynamic one
-    #                         w_size = ((columns[c]["weight"] / total_column_weight) * extra_width).__floor__()
-    #                         columns[c]["width"] = max([w_size, columns[c]["max_size"]])
-    #                         # print(f"{w_size=}\t{columns[c]['max_size']=}")
-    #
-    #                     # columns[c]["width"] += columns[c]["max_size"]
-    #                     columns[c]["x_start"] = sum([prev_col["width"] for prev_col in columns[:c]])
-    #
-    #                     # pg.draw.rect(
-    #                     #     self.__background,
-    #                     #     (255, 0, 0, 255),
-    #                     #     pg.Rect(columns[c]["x_start"], rows[r]["y_start"], columns[c]["width"], rows[r]["height"]),
-    #                     #     width=1
-    #                     # )
-    #
-    #             # place children
-    #             for child, params in self._child_params:
-    #                 # place the child proportional to the table and stickiness
-    #                 # size = list(child.calculate_size())
-    #                 size = [child._width, child._height]
-    #
-    #                 row, column = params["row"], params["column"]
-    #                 sticky = params["sticky"]
-    #
-    #                 width = columns[column]["width"]
-    #                 height = rows[row]["height"]
-    #
-    #                 x = columns[column]["x_start"]
-    #                 y = rows[row]["y_start"]
-    #
-    #                 x_cen = x + width / 2
-    #                 y_cen = y + height / 2
-    #
-    #                 x_diff = width - size[0]
-    #                 y_diff = height - size[1]
-    #
-    #                 # print(f"calc: {x_diff}, {y_diff}\t{size}\t{width},{height}")
-    #                 # print(f"{sticky=}")
-    #
-    #                 box_x = x_cen - size[0] / 2
-    #                 box_y = y_cen - size[1] / 2
-    #
-    #                 # assign stickiness
-    #                 if not child._width_configured:
-    #                     if "w" in sticky:
-    #                         size[0] += (x_diff / 2) - params.margin
-    #                         box_x = x + params.margin
-    #
-    #                     if "e" in sticky:
-    #                         size[0] += (x_diff / 2) - params.margin
-    #
-    #                     child.assigned_width = size[0]
-    #
-    #                 if not child._height_configured:
-    #                     if "n" in sticky:
-    #                         size[1] += (y_diff / 2) - params.margin
-    #                         box_y = y + params.margin
-    #                         # print("north: ", size, box_x, box_y, "\t\t", width, height)
-    #
-    #                     if "s" in sticky:
-    #                         size[1] += (y_diff / 2) - params.margin
-    #                         # print("south: ", size, box_x, box_y, "\t\t", width, height)
-    #
-    #                     child.assigned_height = size[1]
-    #
-    #                 child.set_position(box_x, box_y)
-    #
-    #         case _:
-    #             raise ValueError(f"Invalid geometry type: {self._layout.__class__.__name__}")
+        # not a real layout type
+        if layout not in Layout:
+            return False
+
+        # is already the same layout
+        if self._layout == layout:
+            return True
+
+        # no children present - can be easily changed
+        if len(self._children) == 0:
+            return True
+
+        return False
+
+    def grid_columnconfigure(
+            self,
+            column: int | tp.Iterable[int],
+            weight: float = 1
+    ) -> None:
+        """
+        configure one or more grid columns
+        """
+        # if the column is given as a list,
+        # call this function with an integer as parameter
+        if isinstance(column, tp.Iterable):
+            for c in column:
+                self.grid_columnconfigure(c, weight=weight)
+
+            return
+
+        # check if the layout is "grid"
+        if not self.check_set_layout(Layout.Grid):
+            raise ValueError("Invalid geometry type for grid-configuration")
+
+        self.set_layout(Layout.Grid)
+
+        self._grid_params["columns"][column] = {
+            "weight": weight
+        }
+
+    def grid_rowconfigure(
+            self,
+            row: int | tp.Iterable[int],
+            weight: float = 1
+    ) -> None:
+        """
+        configure one or more grid rows
+        """
+        # if the row is given a list, call this
+        # function with an integer as parameter
+        if isinstance(row, tp.Iterable):
+            for r in row:
+                self.grid_rowconfigure(r, weight=weight)
+
+            return
+
+        # check if the layout is "grid"
+        if not self.check_set_layout(Layout.Grid):
+            raise ValueError("Invalid geometry type for grid-configuration")
+
+        self.set_layout(Layout.Grid)
+
+        self._grid_params["rows"][row] = {
+            "weight": weight
+        }
+
+    # other stuff
+    def add_child(self, child: tp.Any, **params) -> None:
+        """
+        add a child to the collection
+        """
+        if child not in self._children:
+            super().add_child(child)
+            self._child_params.append((child, BetterDict(params)))
+
+    def calculate_geometry(self):
+        """
+        calculate how each individual child should be placed
+        """
+        match self._layout:
+            case Layout.Absolute:
+                # since the positioning is absolute,
+                # the children should not influence the parents size
+                for child, params in self._child_params:
+                    child.set_position(params.x, params.y)
+
+            case Layout.Pack:
+                directional_dict: dict[str, int | list] = {
+                    "total_x": 0,
+                    "total_y": 0,
+                    "children": [],
+                    "sizes": []
+                }
+                top = deepcopy(directional_dict)
+                bottom = deepcopy(directional_dict)
+                left = deepcopy(directional_dict)
+                right = deepcopy(directional_dict)
+
+                # get all sizes and group by anchor
+                for child, param in self._child_params:
+                    child_size = child.calculate_size()
+
+                    if param.anchor == TOP:
+                        top["children"].append(child)
+                        top["sizes"].append(child_size)
+                        top["total_x"] += child_size[0]
+                        top["total_y"] += child_size[1]
+
+                    elif param.anchor == BOTTOM:
+                        bottom["children"].append(child)
+                        bottom["sizes"].append(child_size)
+                        bottom["total_x"] += child_size[0]
+                        bottom["total_y"] += child_size[1]
+
+                    elif param.anchor == LEFT:
+                        left["children"].append(child)
+                        left["sizes"].append(child_size)
+                        left["total_x"] += child_size[0]
+                        left["total_y"] += child_size[1]
+
+                    elif param.anchor == RIGHT:
+                        right["children"].append(child)
+                        right["sizes"].append(child_size)
+                        right["total_x"] += child_size[0]
+                        right["total_y"] += child_size[1]
+
+                top["total_y"] += self.layout_params.padding * len(
+                    top["children"]
+                ) - 1
+                bottom["total_y"] += self.layout_params.padding * len(
+                    bottom["children"]
+                ) - 1
+
+                left["total_x"] += self.layout_params.padding * len(
+                    left["children"]
+                ) - 1
+                right["total_x"] += self.layout_params.padding * len(
+                    right["children"]
+                ) - 1
+
+                # if not configured, set own size
+                total_x = max([top["total_x"], bottom["total_x"],
+                               left["total_x"] + right["total_x"]])
+                total_y = max([left["total_y"], right["total_y"],
+                               top["total_y"] + bottom["total_y"]])
+
+                # add margin
+                total_x += self.layout_params.margin * 2
+                total_y += self.layout_params.margin * 2
+
+                if not self._width_configured:
+                    self._width = total_x
+
+                    if hasattr(self, "debug_this"):
+                        print("setting width: ", total_x)
+
+                else:
+                    total_x = self._width
+    
+                if not self._height_configured:
+                    if hasattr(self, "debug_this"):
+                        print("setting height: ", total_y)
+
+                    self._height = total_y
+
+                else:
+                    total_y = self.height
+
+                # tell the children where they should be
+                y_cen = total_y / 2
+                x_cen = total_x / 2
+
+                # left
+                x_now = self.layout_params.margin
+                for child, size in zip(left["children"], left["sizes"]):
+                    child.set_position(x_now, y_cen - size[1] / 2)
+                    x_now += size[0] + self.layout_params.padding
+
+                # right
+                x_now = total_x - self.layout_params.margin
+                for child, size in zip(right["children"], right["sizes"]):
+                    child.set_position(x_now - size[0], y_cen - size[1] / 2)
+                    x_now -= size[0] + self.layout_params.padding
+
+                # top
+                y_now = self.layout_params.margin
+                for child, size in zip(top["children"], top["sizes"]):
+                    child.set_position(x_cen - size[0] / 2, y_now)
+                    y_now += size[1] + self.layout_params.padding
+
+                # bottom
+                y_now = total_y - self.layout_params.margin
+                for child, size in zip(bottom["children"], bottom["sizes"]):
+                    child.set_position(x_cen - size[0] / 2, y_now - size[1])
+                    y_now -= size[1] + self.layout_params.padding
+
+            case Layout.Grid:
+                rows: list[dict[
+                    str,
+                    list[tuple[tp.Any, BetterDict, bool]] | float
+                ]] = []
+                columns: list[dict[
+                    str,
+                    list[tuple[tp.Any, BetterDict, bool]] | float
+                ]] = []
+
+                for child, params in self._child_params:
+                    row, column = params["row"], params["column"]
+
+                    # if row was not yet made, make all previous ones
+                    min_rows = row + params.rowspan - 1
+                    min_columns = column + params.columnspan - 1
+
+                    if len(rows) <= min_rows:
+                        for n_row in range(len(rows), min_rows+1):
+                            out = {
+                                "weight": 0,
+                                "children": []
+                            }
+
+                            if n_row in self._grid_params.rows:
+                                config = self._grid_params.rows[n_row]
+
+                                if "weight" in config:
+                                    out["weight"] = config["weight"]
+
+                            rows.append(out)
+
+                    if len(columns) <= min_columns:
+                        for n_col in range(len(columns), min_columns+1):
+                            out = {
+                                "weight": 0,
+                                "children": []
+                            }
+
+                            if n_col in self._grid_params.columns:
+                                config = self._grid_params.columns[n_col]
+
+                                if "weight" in config:
+                                    out["weight"] = config["weight"]
+
+                            columns.append(out)
+
+                    rows[row]["children"].append((child, params, True))
+                    
+                    # if rowspan is given, also add the widget to all the
+                    # corresponding other rows
+                    if "rowspan" in params:
+                        for row_incrementor in range(1, params.rowspan):
+                            rows[row + row_incrementor]["children"]\
+                                .append(
+                                (child, params, False)
+                            )
+
+                    columns[column]["children"].append((child, params, True))
+
+                    if "columnspan" in params:
+                        for column_incrementor in range(1, params.columnspan):
+                            columns[column + column_incrementor]["children"]\
+                                .append(
+                                (child, params, False)
+                            )
+
+                matrix: list[list] = []
+
+                # append all the children to a 2d matrix and check if one
+                # cell has multiple children
+                for r in range(len(rows)):
+                    matrix.append([])
+
+                    for c in range(len(columns)):
+                        child = [
+                            chi for chi in rows[r]["children"]
+                            if chi in columns[c]["children"]
+                        ]
+                        child = list(child)
+
+                        if len(child) > 1:
+                            raise ValueError(
+                                f"{len(child)} children assigned "
+                                f"to row {r} column {c}!"
+                            )
+
+                        if child:
+                            matrix[r].append(child[0])
+
+                        else:
+                            matrix[r].append(...)
+
+                # calculate the minimal size for each row
+                for r, row in enumerate(rows):
+                    rows[r]["max_size"] = 0
+
+                    for child, params, _is_widget in row["children"]:
+                        child.calculate_size()
+                        _, y = child.get_size()
+
+                        y += 2 * params.margin
+
+                        # split size between rows
+                        y /= params.rowspan
+
+                        if y > rows[r]["max_size"]:
+                            rows[r]["max_size"] = y
+
+                # calculate the minimal size for each column
+                for c, column in enumerate(columns):
+                    columns[c]["max_size"] = 0
+
+                    for child, params, _is_widget in column["children"]:
+                        child.calculate_size()
+                        x, _ = child.get_size()
+
+                        x += 2 * params.margin
+
+                        # split size between columns
+                        x /= params.columnspan
+
+                        if x > columns[c]["max_size"]:
+                            columns[c]["max_size"] = x
+
+                # calculate the container size
+                columns_width, rows_height = self.assigned_width, self.assigned_height
+
+                # only subtract rows that don't have a weight
+                min_width = sum([c["max_size"] for c in columns])
+                min_height = sum([r["max_size"] for r in rows])
+
+                # if children exist, set min size
+                if len(columns) + len(rows) > 0:
+                    if columns_width == 0 or rows_height == 0 and not\
+                            self._width_configured:
+
+                        # only set if child requires greater width
+                        if min_width > self._width:
+                            if hasattr(self, "debug_this"):
+                                print(
+                                    "setting width (children min): ", min_width
+                                    )
+                            self._width = min_width
+
+                    if columns_width == 0\
+                            or rows_height == 0\
+                            and not self._height_configured:
+
+                        # only set if child requires greater height
+                        if min_height > self._height:
+                            if hasattr(self, "debug_this"):
+                                print(
+                                    "setting height (children min): ",
+                                    min_height
+                                    )
+                            self._height = min_height
+
+                # if a size has been set by the user, overwrite the calculated
+                # size
+                if self._width_configured:
+                    columns_width = self._width
+
+                if self._height_configured:
+                    rows_height = self.height
+
+                # assign extra space
+                extra_width = columns_width - sum(
+                    [c["max_size"] for c in columns if c["weight"] == 0]
+                )
+                extra_height = rows_height - sum(
+                    [r["max_size"] for r in rows if r["weight"] == 0]
+                )
+
+                total_row_weight = sum(
+                    [row["weight"] for row in rows]
+                )
+                total_column_weight = sum(
+                    [column["weight"] for column in columns]
+                )
+
+                # assign each row and column a specific size
+                for r in range(len(rows)):
+                    if total_row_weight == 0:
+                        rows[r]["height"] = 0
+
+                    else:
+                        # assign either the minimum size or the
+                        # calculated dynamic one
+                        w_size = (
+                            (rows[r]["weight"] / total_row_weight)
+                            * extra_height
+                        ).__floor__()
+                        rows[r]["height"] = w_size
+
+                    rows[r]["y_start"] = self.layout_params.padding / 2 + sum(
+                        [prev_row["height"] for prev_row in rows[:r]]
+                    )
+
+                for c in range(len(columns)):
+                    if total_column_weight == 0:
+                        columns[c]["width"] = 0
+
+                    else:
+                        # assign either the minimum size or the
+                        # calculated dynamic one
+                        w_size = (
+                            (
+                                columns[c]["weight"]
+                                / total_column_weight
+                            )
+                            * extra_width
+                        ).__floor__()
+                        columns[c]["width"] = w_size
+
+                    columns[c]["x_start"] = self.layout_params.padding / 2\
+                        + sum(
+                        [prev_col["width"] for prev_col in columns[:c]]
+                    )
+
+                if hasattr(self, "debug_this"):
+                    print(self.width, extra_width, min_width)
+                    print([f"width: {c['width']}" for c in columns])
+
+                # place children
+                for child, params in self._child_params:
+                    # place the child proportional to the table and stickiness
+                    # size = list(child.calculate_size())
+                    size = [child._width, child._height]
+
+                    row, column = params.row, params.column
+                    sticky = params.sticky
+                    margin = params.margin
+
+                    columns_width = sum([
+                        columns[c]["width"] for c in
+                        range(column, column + params.columnspan)
+                    ])
+                    rows_height = sum([
+                        rows[r]["height"] for r in
+                        range(row, row + params.rowspan)
+                    ])
+
+                    x = columns[column]["x_start"]
+                    y = rows[row]["y_start"]
+
+                    x_diff = columns_width - size[0]
+                    y_diff = rows_height - size[1]
+
+                    # offsets for width / height configured
+                    x_position_offset = 0
+                    y_position_offset = 0
+
+                    if hasattr(self, "debug_this"):
+                        print("cw: ", columns_width, params.columnspan)
+
+                    # assign stickiness
+                    if not child._width_configured:
+                        if "w" in sticky:
+                            size[0] += (x_diff / 2) - params.margin
+
+                        if "e" in sticky:
+                            size[0] += (x_diff / 2) - params.margin
+
+                        child.assigned_width = size[0]
+
+                    else:
+                        # if width is configured, center the widget based
+                        # on its configured width
+                        x_position_offset += x_diff / 2 - params.margin
+
+                    if not child._height_configured:
+                        if "n" in sticky:
+                            size[1] += (y_diff / 2) - params.margin
+
+                        if "s" in sticky:
+                            size[1] += (y_diff / 2) - params.margin
+
+                        child.assigned_height = size[1]
+
+                    else:
+                        # if height is configured, center the widget based
+                        # on its configured height
+                        y_position_offset += y_diff / 2 - params.margin
+
+                    child.set_position(
+                        x + margin + max([x_position_offset, 0]),
+                        y + margin + max([y_position_offset, 0])
+                    )
+
+                self._last_rows = rows
+                self._last_columns = columns
+
+            case _:
+                raise ValueError(f"Invalid geometry type: {self._layout}")
 
     def calculate_size(self) -> tuple[int, int]:
         """
         calculate how big the container should be
         """
         # make sure the geometry is up-to-date
-        return pg.display.get_window_size()
+        self.calculate_geometry()
 
-    # tool functions
-    def after(
-            self,
-            timeout: int,
-            function: tp.Callable[[tp.Any], RES_T],
-            *args,
-            **kwargs
-    ) -> Future[RES_T]:
-        """
-        calls the given function after timeout milliseconds
-
-        :param timeout: timeout in milliseconds
-        :param function: the function to call
-        :param args: the given functions positional arguments
-        :param kwargs: the given functions keyword arguments
-        :returns: a future with the function's result
-        """
-        n_future = Future[RES_T]()
-
-        self.__timeouts.append({
-            "timeout_left": timeout,
-            "function": function,
-            "future": n_future,
-            "args": args,
-            "kwargs": kwargs
-        })
+        width = self._width
+        height = self._height
+
+        width = round(width)
+        height = round(height)
 
-        return n_future
+        return width, height
```

### Comparing `pginter-0.2.4/src/pginter/icon.png` & `pginter-0.2.5/src/pginter/icon.png`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/theme/_manager.py` & `pginter-0.2.5/src/pginter/theme/_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/theme/themes/default.json` & `pginter-0.2.5/src/pginter/theme/themes/default.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666666%*

 * *Differences: {"'entry'": "{'border_color': ['#777', '#eee']}"}*

```diff
@@ -20,15 +20,18 @@
         "active_border_color": "#aaa",
         "bg": [
             50,
             50,
             50,
             100
         ],
-        "border_color": "#777",
+        "border_color": [
+            "#777",
+            "#eee"
+        ],
         "border_width": 3,
         "fg": [
             "#fff",
             "#000"
         ],
         "hover_border_color": "#888"
     },
```

### Comparing `pginter-0.2.4/src/pginter/types/_color.py` & `pginter-0.2.5/src/pginter/types/_color.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/types/_scheme.py` & `pginter-0.2.5/src/pginter/types/_scheme.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/types/_style.py` & `pginter-0.2.5/src/pginter/types/_style.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/types/_tk_vars.py` & `pginter-0.2.5/src/pginter/types/_tk_vars.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/utils/_funcs.py` & `pginter-0.2.5/src/pginter/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/widgets/_button.py` & `pginter-0.2.5/src/pginter/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/widgets/_entry.py` & `pginter-0.2.5/src/pginter/widgets/_entry.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/widgets/_frame.py` & `pginter-0.2.5/src/pginter/widgets/_frame.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,28 +15,71 @@
 import pygame as pg
 
 # try importing pil. The user shouldn't be forced to install pil, but
 # will get an error if they try to use the image widget without having it
 # installed
 try:
     # noinspection PyUnresolvedReferences
-    from PIL import Image
+    from PIL import Image, ImageDraw
     PIL_EXISTS = True
 
 except ImportError:
     PIL_EXISTS = False
 
 
 if tp.TYPE_CHECKING:
     from .._pg_root import PgRoot
 
 
 RES_T = tp.TypeVar("RES_T")
 
 
+# utility functions
+def add_corners(
+        im: Image,
+        ulr: int,
+        urr: int,
+        llr: int,
+        lrr: int
+) -> Image:
+    alpha = Image.new('L', im.size, 255)
+    w, h = im.size
+
+    # upper left corner
+    ulc = Image.new("L", (ulr * 2, ulr * 2), 0)
+    draw = ImageDraw.Draw(ulc)
+    draw.ellipse((0, 0, ulr * 2 - 1, ulr * 2 - 1), fill=255)
+    ulc = ulc.crop((0, 0, ulr, urr))
+    alpha.paste(ulc, (0, 0))
+
+    # upper right corner
+    urc = Image.new("L", (urr * 2, urr * 2), 0)
+    draw = ImageDraw.Draw(urc)
+    draw.ellipse((0, 0, urr * 2 - 1, urr * 2 - 1), fill=255)
+    urc = urc.crop((urr, 0, 2 * urr, urr))
+    alpha.paste(urc, (w - urr, 0))
+
+    # lower left radius
+    llc = Image.new("L", (llr * 2, llr * 2), 0)
+    draw = ImageDraw.Draw(llc)
+    draw.ellipse((0, 0, llr * 2 - 1, llr * 2 - 1), fill=255)
+    llc = llc.crop((0, llr, llr, llr * 2))
+    alpha.paste(llc, (0, h - llr))
+
+    # lower right radius
+    lrc = Image.new("L", (lrr * 2, lrr * 2), 0)
+    draw = ImageDraw.Draw(lrc)
+    draw.ellipse((0, 0, lrr * 2 - 1, lrr * 2 - 1), fill=255)
+    lrc = lrc.crop((lrr, lrr, lrr * 2, lrr * 2))
+    alpha.paste(lrc, (w - lrr, h - lrr))
+
+    im.putalpha(alpha)
+    return im
+
+
 def display_configurify(key: str) -> str:
     """
     convert a Frame init key to it's corresponding DisplayConfig key
     """
     replaces = [
         ("bg_color", "bg"),
         ("border_bottom_left_radius", "blr"),
@@ -556,17 +599,31 @@
                 self.assigned_height / 2 - height / 2
             )
 
             pos = (
                 pos[0] if pos[0] >= 0 else 0,
                 pos[1] if pos[1] >= 0 else 0
             )
-            now_image = pil_image_to_surface(
-                self._image.resize((width, height))
+
+            # resize image
+            tmp_image = self._image.resize((width, height))
+
+            # add round edges
+            tmp_image = add_corners(
+                tmp_image,
+                current_style.borderTopLeftRadius,
+                current_style.borderTopRightRadius,
+                current_style.borderBottomLeftRadius,
+                current_style.borderBottomRightRadius
             )
+
+            # convert to pygame image
+            now_image = pil_image_to_surface(tmp_image)
+
+            # draw image to surface
             _surface.blit(now_image, pos)
 
         if current_style.borderWidth > 0:
             # print(f"drawing border, {current_style.borderColor}")
             pg.draw.rect(
                 _surface,
                 current_style.borderColor.irgba,
```

### Comparing `pginter-0.2.4/src/pginter/widgets/_label.py` & `pginter-0.2.5/src/pginter/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter/widgets/_surface_frame.py` & `pginter-0.2.5/src/pginter/widgets/_surface_frame.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.4/src/pginter.egg-info/SOURCES.txt` & `pginter-0.2.5/src/pginter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

