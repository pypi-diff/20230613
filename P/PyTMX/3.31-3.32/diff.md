# Comparing `tmp/PyTMX-3.31.tar.gz` & `tmp/PyTMX-3.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTMX-3.31.tar", last modified: Wed Dec  1 13:30:02 2021, max compression
+gzip compressed data, was "PyTMX-3.32.tar", last modified: Tue Jun 13 15:45:45 2023, max compression
```

## Comparing `PyTMX-3.31.tar` & `PyTMX-3.32.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ltheden   (1000) ltheden   (1000)        0 2021-12-01 13:30:02.935884 PyTMX-3.31/
--rw-r--r--   0 ltheden   (1000) ltheden   (1000)     7651 2020-04-14 15:24:23.000000 PyTMX-3.31/LICENSE
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)      122 2021-04-20 13:01:31.000000 PyTMX-3.31/MANIFEST.in
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)      801 2021-12-01 13:30:02.935884 PyTMX-3.31/PKG-INFO
-drwxrwxr-x   0 ltheden   (1000) ltheden   (1000)        0 2021-12-01 13:30:02.933884 PyTMX-3.31/PyTMX.egg-info/
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)      801 2021-12-01 13:30:02.000000 PyTMX-3.31/PyTMX.egg-info/PKG-INFO
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)      296 2021-12-01 13:30:02.000000 PyTMX-3.31/PyTMX.egg-info/SOURCES.txt
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)        1 2021-12-01 13:30:02.000000 PyTMX-3.31/PyTMX.egg-info/dependency_links.txt
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)        6 2021-12-01 13:30:02.000000 PyTMX-3.31/PyTMX.egg-info/top_level.txt
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     5910 2021-11-03 13:48:54.000000 PyTMX-3.31/changelog
-drwxrwxr-x   0 ltheden   (1000) ltheden   (1000)        0 2021-12-01 13:30:02.934884 PyTMX-3.31/pytmx/
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     1055 2021-12-01 13:29:29.000000 PyTMX-3.31/pytmx/__init__.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)    46445 2021-12-01 13:28:43.000000 PyTMX-3.31/pytmx/pytmx.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)    10153 2021-11-03 15:19:56.000000 PyTMX-3.31/pytmx/util_pygame.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     2743 2021-11-03 15:19:56.000000 PyTMX-3.31/pytmx/util_pygame_sdl2.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     1986 2021-11-03 15:19:56.000000 PyTMX-3.31/pytmx/util_pyglet.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     2528 2021-11-03 15:19:56.000000 PyTMX-3.31/pytmx/util_pysdl2.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)    20336 2021-11-03 13:48:57.000000 PyTMX-3.31/readme.md
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)       79 2021-12-01 13:30:02.935884 PyTMX-3.31/setup.cfg
--rwxrwxr-x   0 ltheden   (1000) ltheden   (1000)     1013 2021-12-01 13:29:29.000000 PyTMX-3.31/setup.py
+drwxr-xr-x   0 ltheden   (1000) ltheden   (1000)        0 2023-06-13 15:45:45.456521 PyTMX-3.32/
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     7651 2023-06-13 14:05:21.000000 PyTMX-3.32/LICENSE
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)      104 2023-06-13 14:05:21.000000 PyTMX-3.32/MANIFEST.in
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)      901 2023-06-13 15:45:45.456521 PyTMX-3.32/PKG-INFO
+drwxr-xr-x   0 ltheden   (1000) ltheden   (1000)        0 2023-06-13 15:45:45.454521 PyTMX-3.32/PyTMX.egg-info/
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)      901 2023-06-13 15:45:45.000000 PyTMX-3.32/PyTMX.egg-info/PKG-INFO
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)      314 2023-06-13 15:45:45.000000 PyTMX-3.32/PyTMX.egg-info/SOURCES.txt
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)        1 2023-06-13 15:45:45.000000 PyTMX-3.32/PyTMX.egg-info/dependency_links.txt
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)       54 2023-06-13 15:45:45.000000 PyTMX-3.32/PyTMX.egg-info/requires.txt
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)        6 2023-06-13 15:45:45.000000 PyTMX-3.32/PyTMX.egg-info/top_level.txt
+drwxr-xr-x   0 ltheden   (1000) ltheden   (1000)        0 2023-06-13 15:45:45.455521 PyTMX-3.32/pytmx/
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     1055 2023-06-13 15:44:59.000000 PyTMX-3.32/pytmx/__init__.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)    51606 2023-06-13 15:43:13.000000 PyTMX-3.32/pytmx/pytmx.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)    10153 2023-06-13 14:48:08.000000 PyTMX-3.32/pytmx/util_pygame.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     2743 2023-06-13 14:05:21.000000 PyTMX-3.32/pytmx/util_pygame_sdl2.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     1986 2023-06-13 14:05:21.000000 PyTMX-3.32/pytmx/util_pyglet.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     2528 2023-06-13 14:05:21.000000 PyTMX-3.32/pytmx/util_pysdl2.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)    20266 2023-06-13 14:05:21.000000 PyTMX-3.32/readme.md
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)       79 2023-06-13 15:45:45.456521 PyTMX-3.32/setup.cfg
+-rwxr-xr-x   0 ltheden   (1000) ltheden   (1000)     1172 2023-06-13 14:41:11.000000 PyTMX-3.32/setup.py
```

### Comparing `PyTMX-3.31/LICENSE` & `PyTMX-3.32/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTMX-3.31/PKG-INFO` & `PyTMX-3.32/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: PyTMX
-Version: 3.31
+Version: 3.32
 Summary: Loads tiled tmx maps
 Home-page: UNKNOWN
 Author: bitcraft
 Author-email: leif.theden@gmail.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Requires-Python: >=3.7
+Provides-Extra: pygame
+Provides-Extra: pygame-ce
 License-File: LICENSE
 
 https://github.com/bitcraft/PyTMX
```

### Comparing `PyTMX-3.31/PyTMX.egg-info/PKG-INFO` & `PyTMX-3.32/PyTMX.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: PyTMX
-Version: 3.31
+Version: 3.32
 Summary: Loads tiled tmx maps
 Home-page: UNKNOWN
 Author: bitcraft
 Author-email: leif.theden@gmail.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Requires-Python: >=3.7
+Provides-Extra: pygame
+Provides-Extra: pygame-ce
 License-File: LICENSE
 
 https://github.com/bitcraft/PyTMX
```

### Comparing `PyTMX-3.31/pytmx/__init__.py` & `PyTMX-3.32/pytmx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (C) 2012-2021, Leif Theden <leif.theden@gmail.com>
+Copyright (C) 2012-2023, Leif Theden <leif.theden@gmail.com>
 
 This file is part of pytmx.
 
 pytmx is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as
 published by the Free Software Foundation, either version 3 of the
 License, or (at your option) any later version.
@@ -23,11 +23,11 @@
 logger = logging.getLogger(__name__)
 
 try:
     from pytmx.util_pygame import load_pygame
 except ImportError:
     logger.debug("cannot import pygame tools")
 
-__version__ = (3, 31)
+__version__ = (3, 32)
 __author__ = "bitcraft"
 __author_email__ = "leif.theden@gmail.com"
 __description__ = "Map loader for TMX Files - Python 3.3 +"
```

### Comparing `PyTMX-3.31/pytmx/pytmx.py` & `PyTMX-3.32/pytmx/pytmx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
-Copyright (C) 2012-2021, Leif Theden <leif.theden@gmail.com>
+Copyright (C) 2012-2023, Leif Theden <leif.theden@gmail.com>
 
 This file is part of pytmx.
 
 pytmx is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as
 published by the Free Software Foundation, either version 3 of the
 License, or (at your option) any later version.
 
 pytmx is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public
-License along with pytmx.  If not, see <http://www.gnu.org/licenses/>.
+License along with pytmx.  If not, see <https://www.gnu.org/licenses/>.
+
 """
 from __future__ import annotations
 
 
 import gzip
 import logging
 import os
@@ -27,31 +28,35 @@
 from base64 import b64decode
 from collections import defaultdict, namedtuple
 from itertools import chain, product
 from math import cos, radians, sin
 from operator import attrgetter
 from typing import List, Tuple, Optional, Sequence, Union, Dict, Iterable
 from xml.etree import ElementTree
+import json
+from copy import deepcopy
 
 # for type hinting
 try:
     import pygame
 except ImportError:
     pygame = None
 
 __all__ = (
+    "TileFlags",
     "TiledElement",
+    "TiledImageLayer",
     "TiledMap",
-    "TiledTileset",
-    "TiledTileLayer",
     "TiledObject",
     "TiledObjectGroup",
-    "TiledImageLayer",
-    "TileFlags",
+    "TiledTileLayer",
+    "TiledClassType",
+    "TiledTileset",
     "convert_to_bool",
+    "resolve_to_class",
     "parse_properties",
 )
 
 logger = logging.getLogger(__name__)
 
 # internal flags
 TRANS_FLIPX = 1
@@ -75,44 +80,49 @@
 AnimationFrame = namedtuple("AnimationFrame", ["gid", "duration"])
 Point = namedtuple("Point", ["x", "y"])
 TileFlags = namedtuple("TileFlags", flag_names)
 empty_flags = TileFlags(False, False, False)
 ColorLike = Union[Tuple[int, int, int, int], Tuple[int, int, int], int, str]
 MapPoint = Tuple[int, int, int]
 
-# need a more graceful way to handle annotations for optional dependancies
+# need a more graceful way to handle annotations for optional dependencies
 if pygame:
     PointLike = Union[Tuple[int, int], pygame.Vector2, Point]
 else:
     PointLike = Union[Tuple[int, int], Point]
 
 
 def default_image_loader(filename: str, flags, **kwargs):
-    """
-    This default image loader just returns filename, rect, and any flags
+    """This default image loader just returns filename, rect, and any flags.
+    Suitable for loading a map without the images.
+
+    Args:
+        filename (str): The file's name.
+        flags (???): ???
+        **kwargs: Additional kwargs.
 
-    Suitable for loading a map without the images
+    Returns:
+        Tuple[str, ???, ???]: A tuple of the file name, rect, and flags.
 
     """
 
     def load(rect=None, flags=None):
         return filename, rect, flags
 
     return load
 
 
 def decode_gid(raw_gid: int) -> Tuple[int, TileFlags]:
-    """
-    Decode a GID from TMX data
+    """Decode a GID from TMX data.
 
     Args:
-        raw_gid: GID, as reported by Tiled
+        raw_gid (int): GID, as reported by Tiled.
 
     Returns:
-        Tuple of the GID after rotation flags, and TileFlags object
+        Tuple[int, TileFlags]: Tuple of the GID after rotation flags, and TileFlags object
 
     """
     if raw_gid < GID_TRANS_ROT:
         return raw_gid, empty_flags
     return (
         raw_gid & ~GID_MASK,
         # TODO: cache all combinations of flags
@@ -124,43 +134,41 @@
     )
 
 
 def reshape_data(
     gids: List[int],
     width: int,
 ) -> List[List[int]]:
-    """
-    Change 1d list to 2d list
+    """Change 1D list to 2d list
 
     Args:
-        gids: list of gid ints
-        width: width of each row
+        gids (List[int]): List of gid ints.
+        width (int): Width of each row.
 
     Returns:
-        2d nested list object
+        List[List[int]]: 2D nested list object.
 
     """
     return [gids[i : i + width] for i in range(0, len(gids), width)]
 
 
 def unpack_gids(
     text: str,
     encoding: Optional[str] = None,
     compression: Optional[str] = None,
 ) -> List[int]:
-    """
-    Return all gids from encoded/compressed layer data
+    """Return all gids from encoded/compressed layer data
 
     Args:
-        text: layer data in text format
-        encoding: encoding used
-        compression: compression used
+        text (str): Layer data in text format.
+        encoding (Optional[str]): Encoding used.
+        compression (Optional[str]): Compression used.
 
     Returns:
-        list of all the GIDs in the layer
+        List[int]: List of all the GIDs in the layer.
 
     """
     if encoding == "base64":
         data = b64decode(text)
         if compression == "gzip":
             data = gzip.decompress(data)
         elif compression == "zlib":
@@ -172,50 +180,69 @@
     elif encoding == "csv":
         return [int(i) for i in text.split(",")]
     elif encoding:
         raise ValueError(f"layer encoding {encoding} is not supported.")
 
 
 def convert_to_bool(value: str) -> bool:
-    """
-    Convert a few common variations of "true" and "false" to boolean
+    """Convert a few common variations of "true" and "false" to boolean
 
     Args:
-        value: string to test
+        value (str): String to test.
 
     Raises:
-        ValueError: if `value` cannot be converted to a bool
+        ValueError: If `value` cannot be converted to a boolean.
+
+    Returns:
+        bool: The converted boolean.
+
     """
     value = str(value).strip()
     if value:
         value = value.lower()[0]
         if value in ("1", "y", "t"):
             return True
         if value in ("-", "0", "n", "f"):
             return False
     else:
         return False
     raise ValueError('cannot parse "{}" as bool'.format(value))
 
 
+def resolve_to_class(value: str, custom_types: dict) -> TiledClassType:
+    """Converts tiled custom types to a python class.
+
+    Args:
+        value (str): name of the class.
+        custom_types (dict): A dictionary with the custom types created by users.
+
+    Raises:
+        ValueError: if `value` cannot be converted to a class.
+
+    Returns:
+        TiledClassType: The converted python class type.
+
+    """
+    return deepcopy(custom_types[value])
+
+
 def rotate(
     points: Sequence[Point],
     origin: Point,
     angle: Union[int, float],
 ) -> List[Point]:
-    """
-    Rotate a sequence of points around an axis
+    """Rotate a sequence of points around an axis.
 
     Args:
-        points: sequence of points
-        origin: point where points are rotated around
-        angle: angle in degrees
+        points (Sequence[Point]): sequence of points.
+        origin (Point): point where points are rotated around.
+        angle (Union[int, float]): angle in degrees.
 
     Returns:
-        list of rotated points
+        List[Point]: List of rotated points.
 
     """
     sin_t = sin(radians(angle))
     cos_t = cos(radians(angle))
     new_points = list()
     for point in points:
         p = (
@@ -228,91 +255,92 @@
 
 # used to change the unicode string returned from xml to
 # proper python variable types.
 types = defaultdict(lambda: str)
 
 types.update(
     {
-        "version": str,
-        "tiledversion": str,
-        "orientation": str,
-        "renderorder": str,
-        "width": float,
-        "height": float,
-        "tilewidth": int,
-        "tileheight": int,
-        "hexsidelength": float,
-        "staggeraxis": str,
-        "staggerindex": str,
         "backgroundcolor": str,
-        "nextobjectid": int,
-        "firstgid": int,
-        "source": str,
-        "name": str,
-        "spacing": int,
-        "margin": int,
-        "tilecount": int,
+        "bold": convert_to_bool,
+        "color": str,
         "columns": int,
-        "format": str,
-        "trans": str,
-        "tile": int,
-        "terrain": str,
-        "probability": float,
-        "tileid": int,
+        "compression": str,
+        "draworder": str,
         "duration": int,
-        "color": str,
+        "encoding": str,
+        "firstgid": int,
+        "fontfamily": str,
+        "format": str,
+        "gid": int,
+        "halign": str,
+        "height": float,
+        "hexsidelength": float,
         "id": int,
-        "opacity": float,
-        "visible": convert_to_bool,
+        "italic": convert_to_bool,
+        "kerning": convert_to_bool,
+        "margin": int,
+        "name": str,
+        "nextobjectid": int,
         "offsetx": int,
         "offsety": int,
-        "encoding": str,
-        "compression": str,
-        "draworder": str,
-        "points": str,
-        "fontfamily": str,
+        "opacity": float,
+        "orientation": str,
         "pixelsize": float,
-        "wrap": convert_to_bool,
-        "bold": convert_to_bool,
-        "italic": convert_to_bool,
-        "underline": convert_to_bool,
+        "points": str,
+        "probability": float,
+        "renderorder": str,
+        "rotation": float,
+        "source": str,
+        "spacing": int,
+        "staggeraxis": str,
+        "staggerindex": str,
         "strikeout": convert_to_bool,
-        "kerning": convert_to_bool,
-        "halign": str,
-        "valign": str,
-        "gid": int,
+        "terrain": str,
+        "tile": int,
+        "tilecount": int,
+        "tiledversion": str,
+        "tileheight": int,
+        "tileid": int,
+        "tilewidth": int,
+        "trans": str,
         "type": str,
+        "underline": convert_to_bool,
+        "valign": str,
+        "value": str,
+        "version": str,
+        "visible": convert_to_bool,
+        "width": float,
+        "wrap": convert_to_bool,
         "x": float,
         "y": float,
-        "value": str,
-        "rotation": float,
     }
 )
 
 # casting for properties type
 prop_type = {
-    "string": str,
-    "int": int,
-    "float": float,
     "bool": convert_to_bool,
     "color": str,
     "file": str,
+    "float": float,
+    "int": int,
     "object": int,
+    "string": str,
+    "class": resolve_to_class,
+    "enum": str,
 }
 
 
-def parse_properties(node: ElementTree.Element) -> Dict:
-    """
-    Parse a Tiled xml node and return a dict that represents a Tiled "property"
+def parse_properties(node: ElementTree.Element, customs: dict = None) -> Dict:
+    """Parse a Tiled xml node and return a dict.
 
     Args:
-        node: etree element to inspect
+        node (ElementTree.Element): Etree element to inspect.
 
     Returns:
-        dict of the properties, as set in the Tiled editor for the object
+        Dict: Dictionary of the properties, as set in the Tiled editor.
 
     """
     d = dict()
     for child in node.findall("properties"):
         for subnode in child.findall("property"):
             cls = None
             try:
@@ -320,43 +348,50 @@
                     cls = prop_type[subnode.get("type")]
             except AttributeError:
                 logger.info(
                     "Type {} Not a built-in type. Defaulting to string-cast.".format(
                         subnode.get("type")
                     )
                 )
-            d[subnode.get("name")] = subnode.get("value") or subnode.text
-            if cls is not None:
-                d[subnode.get("name")] = cls(subnode.get("value"))
+            if "class" == subnode.get("type"):
+                new = resolve_to_class(subnode.get("propertytype"), customs)
+                properties = parse_properties(subnode, customs)
+                for key in properties.keys():
+                    setattr(new, key, properties[key])
+
+                d[subnode.get("name")] = new
+            else:
+                d[subnode.get("name")] = subnode.get("value") or subnode.text
+                if cls is not None:
+                    d[subnode.get("name")] = cls(subnode.get("value"))
     return d
 
 
 class TiledElement:
-    """
-    Base class for all pytmx types
-
-    """
+    """Base class for all pytmx types."""
 
     allow_duplicate_names = False
 
     def __init__(self):
         self.properties = dict()
 
     @classmethod
     def from_xml_string(cls, xml_string: str) -> TiledElement:
-        """
-        Return a TiledElement object from a xml string
+        """Return a TiledElement object from a xml string.
 
         Args:
-            xml_string: string containing xml data
+            xml_string (str): String containing xml data.
+
+        Returns:
+            TiledElement: The TiledElement from the xml string.
 
         """
         return cls().parse_xml(ElementTree.fromstring(xml_string))
 
-    def _cast_and_set_attributes_from_node_items(self, items):
+    def _cast_and_set_attributes_from_node_items(self, items) -> None:
         for key, value in items:
             casted_value = types[key](value)
             setattr(self, key, casted_value)
 
     def _contains_invalid_property_name(self, items) -> bool:
         if self.allow_duplicate_names:
             return False
@@ -373,38 +408,34 @@
             if _hasattr:
                 msg = duplicate_name_fmt.format(k, self.__class__.__name__, self.name)
                 logger.error(msg)
                 return True
         return False
 
     @staticmethod
-    def _log_property_error_message():
+    def _log_property_error_message() -> None:
         msg = "Some name are reserved for {0} objects and cannot be used."
         logger.error(msg)
 
-    def _set_properties(self, node: ElementTree.Element) -> None:
-        """
-        Set properties from xml data
+    def _set_properties(self, node: ElementTree.Element, customs=None) -> None:
+        """Set properties from xml data
 
-        Read the xml attributes and tiled "properties" from a xml node and fill
-        in the values into the object's dictionary.  Names will be checked to
+        Reads the xml attributes and Tiled "properties" from an XML node and fills
+        in the values into the object's dictionary. Names will be checked to
         make sure that they do not conflict with reserved names.
 
-        Args:
-            node: etree element
-
         """
         self._cast_and_set_attributes_from_node_items(node.items())
-        properties = parse_properties(node)
+        properties = parse_properties(node, customs)
         if not self.allow_duplicate_names and self._contains_invalid_property_name(
             properties.items()
         ):
             self._log_property_error_message()
             raise ValueError(
-                "Reserved names and duplicate names are not allowed. Please rename your property inside the .tmx-file"
+                "Reserved names and duplicate names are not allowed. Please rename your property inside the .tmx file"
             )
 
         self.properties = properties
 
     def __getattr__(self, item):
         try:
             return self.properties[item]
@@ -419,42 +450,54 @@
     def __repr__(self):
         if hasattr(self, "id"):
             return '<{}[{}]: "{}">'.format(self.__class__.__name__, self.id, self.name)
         else:
             return '<{}: "{}">'.format(self.__class__.__name__, self.name)
 
 
-class TiledMap(TiledElement):
-    """
-    Contains the layers, objects, and images from a Tiled TMX map
+class TiledClassType:
+    """Contains custom Tiled types."""
 
-    This class is meant to handle most of the work you need to do to use a map.
-    """
+    def __init__(self, name: str, members: List[dict]) -> None:
+        """Creates the TiledClassType.
+
+        Args:
+            name (str): The name of the class type.
+            members (List[dict]): The members of the class type.
+
+        """
+        self.name = name
+        for member in members:
+            setattr(self, member["name"], member["value"])
+
+
+class TiledMap(TiledElement):
+    """Contains the layers, objects, and images from a Tiled .tmx map."""
 
     def __init__(
         self,
         filename: Optional[str] = None,
+        custom_property_filename: Optional[List[str]] = None,
         image_loader=default_image_loader,
         **kwargs,
     ) -> None:
-        """
-        Load new Tiled map from a .tmx file
+        """Load new Tiled map from a .tmx file.
 
         Args:
-            filename: filename of tiled map to load
-            image_loader: function that will load images (see below)
-            optional_gids: load specific tile image GID, even if never used
-            invert_y: invert the y axis
-            load_all_tiles: load all tile images, even if never used
-            allow_duplicate_names: allow duplicates in objects' metadata
-            image_loader: function to load the images
+            filename (Optional[str]): Filename of tiled map to load.
+            image_loader (Optional[List[str]]): Function that will load images (see below).
+            optional_gids (???): Load specific tile image GID, even if never used.
+            invert_y (bool): Invert the y axis.
+            load_all_tiles (bool): Load all tile images, even if never used.
+            allow_duplicate_names (bool): Allow duplicates in objects' metadata.
 
         """
         TiledElement.__init__(self)
         self.filename = filename
+        self.custom_property_filename = custom_property_filename
         self.image_loader = image_loader
 
         # optional keyword arguments checked here
         self.optional_gids = kwargs.get("optional_gids", set())
         self.load_all_tiles = kwargs.get("load_all", True)
         self.invert_y = kwargs.get("invert_y", True)
 
@@ -490,17 +533,22 @@
         self.tileheight = 0  # height of a tile in pixels
         self.hexsidelength = 0
         self.staggeraxis = None
         self.staggerindex = None
         self.background_color = None
         self.nextobjectid = 0
 
+        self.custom_types = dict()
+
         # initialize the gid mapping
         self.imagemap[(0, 0)] = 0
 
+        if custom_property_filename:
+            self.parse_json(json.load(open(custom_property_filename)))
+
         if filename:
             self.parse_xml(ElementTree.parse(self.filename).getroot())
 
     def __repr__(self):
         return '<{0}: "{1}">'.format(self.__class__.__name__, self.filename)
 
     # iterate over layers and objects in map
@@ -512,20 +560,32 @@
 
         # TODO: make class/layer-specific type casting
         # layer height and width must be int, but TiledElement.set_properties()
         # make a float by default, so recast as int here
         self.height = int(self.height)
         self.width = int(self.width)
 
-    def parse_xml(self, node: ElementTree.Element):
+    def parse_json(self, data: dict) -> None:
+        """Parse custom data types from a JSON object
+
+        Args:
+            data (dict): Dictionary from JSON object to parse
+
         """
-        Parse a map from ElementTree xml node
+        for custom_type in data:
+            if custom_type["type"] == "class":
+                new = TiledClassType(custom_type["name"], custom_type["members"])
+
+                self.custom_types[custom_type["name"]] = new
+
+    def parse_xml(self, node: ElementTree.Element) -> None:
+        """Parse a map from ElementTree xml node.
 
         Args:
-            node: ElementTree xml node to parse
+            node (ElementTree.Element): ElementTree xml node to parse.
 
         """
         self._set_properties(node)
         self.background_color = node.get("backgroundcolor", self.background_color)
 
         # ***         do not change this load order!         *** #
         # ***    gid mapping errors will occur if changed    *** #
@@ -536,15 +596,15 @@
             self.add_layer(TiledTileLayer(self, subnode))
 
         for subnode in node.findall(".//imagelayer"):
             self.add_layer(TiledImageLayer(self, subnode))
 
         # this will only find objectgroup layers, not including tile colliders
         for subnode in node.findall(".//objectgroup"):
-            objectgroup = TiledObjectGroup(self, subnode)
+            objectgroup = TiledObjectGroup(self, subnode, self.custom_types)
             self.add_layer(objectgroup)
             for obj in objectgroup:
                 self.objects_by_id[obj.id] = obj
                 self.objects_by_name[obj.name] = obj
 
         for subnode in node.findall(".//tileset"):
             self.add_tileset(TiledTileset(self, subnode))
@@ -570,16 +630,15 @@
             if self.invert_y:
                 o.y -= o.height
 
         self.reload_images()
         return self
 
     def reload_images(self) -> None:
-        """
-        Load or reload the map images from disk
+        """Load or reload the map images from disk.
 
         This method will use the image loader passed in the constructor
         to do the loading or will use a generic default, in which case no
         images will be loaded.
 
         """
         self.images = [None] * self.maxgid
@@ -653,28 +712,27 @@
                 colorkey = props.get("trans", None)
                 path = os.path.join(os.path.dirname(self.filename), source)
                 loader = self.image_loader(path, colorkey)
                 image = loader()
                 self.images[real_gid] = image
 
     def get_tile_image(self, x: int, y: int, layer: int):
-        """
-        Return the tile image for this location
+        """Return the tile image for this location.
 
         Args:
-            x: x coordinate
-            y: y coordinate
-            layer: layer number
+            x (int): The x coordinate.
+            y (int): The y coordinate.
+            layer (int): The layer's number.
 
         Returns:
-            the image object type will depend on the loader (ie. pygame surface)
+            ???: the image object type will depend on the loader (ie. pygame surface).
 
         Raises:
-            TypeError: if coordinates are not integers
-            ValueError: if the coordinates are out of bounds, or GID not found
+            TypeError: if coordinates are not integers.
+            ValueError: if the coordinates are out of bounds, or GID not found.
 
         """
         if not (x >= 0 and y >= 0):
             raise ValueError(
                 "Tile coordinates must be non-negative, were ({0}, {1})".format(x, y)
             )
 
@@ -694,26 +752,25 @@
             logger.debug(msg)
             raise TypeError(msg)
 
         else:
             return self.get_tile_image_by_gid(gid)
 
     def get_tile_image_by_gid(self, gid: int):
-        """
-        Return the tile image for this location
+        """Return the tile image for this location.
 
         Args:
-            gid: GID of image
+            gid (int): GID of image.
 
         Returns:
-            the image object type will depend on the loader (ie. pygame surface)
+            ???: The image object type will depend on the loader (ie. pygame.Surface).
 
         Raises:
-            TypeError: if `gid` is not an integer
-            ValueError: if there is no image for this GID
+            TypeError: if `gid` is not an integer.
+            ValueError: if there is no image for this GID.
 
         """
         try:
             assert int(gid) >= 0
             return self.images[gid]
         except TypeError:
             msg = "GIDs must be expressed as a number.  Got: {0}"
@@ -721,27 +778,26 @@
             raise TypeError(msg.format(gid))
         except (AssertionError, IndexError):
             msg = "Coords: ({0},{1}) in layer {2} has invalid GID: {3}"
             logger.debug(msg.format(gid))
             raise ValueError(msg.format(gid))
 
     def get_tile_gid(self, x: int, y: int, layer: int) -> int:
-        """
-        Return the tile image GID for this location
+        """Return the tile image GID for this location.
 
         Args:
-            x: x coordinate
-            y: y coordinate
-            layer: layer number
+            x (int): The x coordinate.
+            y (int): The y coordinate.
+            layer (int): The layer's number.
 
         Returns:
-            the image object type will depend on the loader (ie. pygame surface)
+            ???: The image object type will depend on the loader (ie. pygame.Surface).
 
         Raises:
-            ValueError: if coordinates are out of bounds
+            ValueError: If coordinates are out of bounds.
 
         """
         if not (x >= 0 and y >= 0 and layer >= 0):
             raise ValueError(
                 "Tile coordinates and layers must be non-negative, were ({0}, {1}), layer={2}".format(
                     x, y, layer
                 )
@@ -751,26 +807,26 @@
             return self.layers[int(layer)].data[int(y)][int(x)]
         except (IndexError, ValueError):
             msg = "Coords: ({0},{1}) in layer {2} is invalid"
             logger.debug(msg.format(x, y, layer))
             raise ValueError(msg.format(x, y, layer))
 
     def get_tile_properties(self, x: int, y: int, layer: int) -> Optional[Dict]:
-        """Return the tile image GID for this location
+        """Return the tile image GID for this location.
 
         Args:
-            x: x coordinate
-            y: y coordinate
-            layer: layer number
+            x (int): The x coordinate.
+            y (int): The y coordinate.
+            layer (int): The layer number.
 
         Returns:
-            dict of the properties for tile in this location, or None
+            Optional[dict]: Dictionary of the properties for tile in this location or None.
 
         Raises:
-            ValueError: if coordinates are out of bounds
+            ValueError: If coordinates are out of bounds
 
         """
         if not (x >= 0 and y >= 0 and layer >= 0):
             raise ValueError(
                 "Tile coordinates and layers must be non-negative, were ({0}, {1}), layer={2}".format(
                     x, y, layer
                 )
@@ -790,63 +846,62 @@
                 msg = "Coords: ({0},{1}) in layer {2} has invalid GID: {3}"
                 logger.debug(msg.format(x, y, layer, gid))
                 raise Exception(msg.format(x, y, layer, gid))
             except KeyError:
                 return None
 
     def get_tile_locations_by_gid(self, gid: int) -> Iterable[MapPoint]:
-        """
-        Search map for tile locations by the GID
-
-        Return (int, int, int) tuples, where the layer is index of
-        the visible tile layers.
+        """Search map for tile locations by the GID.
 
         Note: Not a fast operation.  Cache results if used often.
 
         Args:
-            gid: GID to be searched for
+            gid (int): GID to be searched for.
+
+        Returns:
+            Iterable[MapPoint]: (int, int, int) tuples, where the layer is index of the visible tile layers.
 
         """
         for l in self.visible_tile_layers:
             for x, y, _gid in [i for i in self.layers[l].iter_data() if i[2] == gid]:
                 yield x, y, l
 
     def get_tile_properties_by_gid(self, gid: int) -> Optional[Dict]:
-        """
-        Get the tile properties of a tile GID
+        """Get the tile properties of a tile GID.
 
         Args:
-            gid: GID
+            gid (int): GID.
 
         Returns:
-            dict of properties for GID, or None
+            Optional[dict]: Dictionary of properties for GID, or None.
 
         """
         try:
             return self.tile_properties[gid]
         except KeyError:
             return None
 
     def set_tile_properties(self, gid: int, properties: dict) -> None:
-        """
-        Set the tile properties of a tile GID
+        """Set the tile properties of a tile GID.
 
         Args:
-            gid: GID
-            properties: python dict of properties for GID
+            gid (int): GID.
+            properties (dict): Python dictionary of properties for GID.
 
         """
         self.tile_properties[gid] = properties
 
     def get_tile_properties_by_layer(self, layer: int):
-        """
-        Get the tile properties of each GID in layer
+        """Get the tile properties of each GID in layer.
 
         Args:
-            layer: layer number
+            layer (int): The layer number.
+
+        Returns:
+            ???: ???
 
         """
         try:
             assert int(layer) >= 0
             layer = int(layer)
         except (TypeError, AssertionError):
             msg = "Layer must be a positive integer.  Got {0} instead."
@@ -864,80 +919,87 @@
 
     def add_layer(
         self,
         layer: Union[
             TiledTileLayer, TiledImageLayer, TiledGroupLayer, TiledObjectGroup
         ],
     ) -> None:
-        """
-        Add a layer to the map
+        """Add a layer to the map.
+
+        Args:
+            layer (Union[TiledTileLayer, TiledImageLayer, TiledGroupLayer, TiledObjectGroup]): The layer.
 
         """
         assert isinstance(
             layer, (TiledGroupLayer, TiledTileLayer, TiledImageLayer, TiledObjectGroup)
         )
 
         self.layers.append(layer)
         self.layernames[layer.name] = layer
 
     def add_tileset(self, tileset: TiledTileset) -> None:
-        """
-        Add a tileset to the map
-
-        """
+        """Add a tileset to the map."""
         assert isinstance(tileset, TiledTileset)
         self.tilesets.append(tileset)
 
-    def get_layer_by_name(self, name: str):
-        """
-        Return a layer by name
+    def get_layer_by_name(self, name: str) -> int:
+        """Return a layer by name.
 
         Args:
-            name: Name of layer.  Case-sensitive.
+            name (str): The layer's name. Case-sensitive!
+
+        Returns:
+            int: The layer number.
 
         Raises:
             ValueError: if layer by name does not exist
 
         """
         try:
             return self.layernames[name]
         except KeyError:
             msg = 'Layer "{0}" not found.'
             logger.debug(msg.format(name))
             raise ValueError(msg.format(name))
 
     def get_object_by_id(self, obj_id: int) -> TiledObject:
-        """
-        Find an object by the object id
+        """Find an object by the object id.
 
         Args:
-            obj_id: ID of the object, from Tiled
+            obj_id (int): ID of the object, from Tiled.
+
+        Returns:
+            TiledObject: The found object.
 
         """
         return self.objects_by_id[obj_id]
 
-    def get_object_by_name(self, name) -> TiledObject:
-        """
-        Find an object by name, case-sensitive
+    def get_object_by_name(self, name: str) -> TiledObject:
+        """Find an object by name, case-sensitive.
 
         Args:
-            name: name of object
+            name (str): The object's name.
+
+        Returns:
+            TiledObject: The found object.
 
         """
         return self.objects_by_name[name]
 
     def get_tileset_from_gid(self, gid: int) -> TiledTileset:
-        """
-        Return tileset that owns the gid
+        """Return tileset that owns the gid.
 
         Note: this is a slow operation, so if you are expecting to do this
               often, it would be worthwhile to cache the results of this.
 
         Args:
-            gid: gid of tile image
+            gid (int): GID of tile image.
+
+        Returns:
+            TiledTileset: The tileset that owns the GID.
 
         Raises:
             ValueError: if the tileset for gid is not found
 
         """
         try:
             tiled_gid = self.tiledgidmap[gid]
@@ -947,82 +1009,97 @@
         for tileset in sorted(self.tilesets, key=attrgetter("firstgid"), reverse=True):
             if tiled_gid >= tileset.firstgid:
                 return tileset
 
         raise ValueError("Tileset not found")
 
     def get_tile_colliders(self) -> Iterable[Tuple[int, List[Dict]]]:
-        """
-        Return iterator of (gid, dict) pairs of tiles with colliders
+        """Return iterator of (gid, dict) pairs of tiles with colliders.
+
+        Returns:
+            Iterable[Tuple[int, List[Dict]]]: The tile colliders.
 
         """
         for gid, props in self.tile_properties.items():
             colliders = props.get("colliders")
             if colliders:
                 yield gid, colliders
 
     @property
     def objectgroups(self) -> Iterable[TiledObjectGroup]:
-        """
-        Return iterator of all object groups
+        """Returns iterator of all object groups.
+
+        Returns:
+            Iterable[TiledObjectGroup]: ???.
 
         """
         return (layer for layer in self.layers if isinstance(layer, TiledObjectGroup))
 
     @property
     def objects(self) -> Iterable[TiledObject]:
-        """
-        Return iterator of all the objects associated with this map
+        """Returns iterator of all the objects associated with the map.
+
+        Returns:
+            Iterable[TiledObject]: All objects associated with the map.
 
         """
         return chain(*self.objectgroups)
 
     @property
     def visible_layers(self):
-        """
-        Return iterator of Layer objects that are set 'visible'
+        """Returns iterator of Layer objects that are set "visible".
+
+        Returns:
+            ???: Iterator of Layer objects that are set "visible".
 
         """
+
         return (l for l in self.layers if l.visible)
 
     @property
     def visible_tile_layers(self) -> Iterable[TiledTileLayer]:
-        """
-        Return iterator of layer indexes that are set 'visible'
+        """Return iterator of layer indexes that are set "visible".
+
+        Returns:
+            Iterable[TiledTileLayer]: A list of layer indexes.
 
         """
         return (
             i
             for (i, l) in enumerate(self.layers)
             if l.visible and isinstance(l, TiledTileLayer)
         )
 
     @property
     def visible_object_groups(self) -> Iterable[TiledObjectGroup]:
-        """Return iterator of object group indexes that are set 'visible'"""
+        """Return iterator of object group indexes that are set "visible".
+
+        Returns:
+            Iterable[TiledObjectGroup]: A list of object group indexes that are set to "visible".
+
+        """
         return (
             i
             for (i, l) in enumerate(self.layers)
             if l.visible and isinstance(l, TiledObjectGroup)
         )
 
     def register_gid(
         self,
         tiled_gid: int,
         flags: Optional[TileFlags] = None,
     ) -> int:
-        """
-        Used to manage the mapping of GIDs between the tmx and pytmx
+        """Used to manage the mapping of GIDs between .tmx and pytmx.
 
         Args:
-            tiled_gid: GID that is found in TMX data
-            flags: TileFlags
+            tiled_gid (int): GID that is found in TMX data.
+            flags (???): TileFlags.
 
         Returns:
-            New or existing GID for pytmx use
+            int: New or existing GID for pytmx use.
 
         """
         if flags is None:
             flags = TileFlags(0, 0, 0)
 
         if tiled_gid:
             try:
@@ -1034,54 +1111,84 @@
                 self.gidmap[tiled_gid].append((gid, flags))
                 self.tiledgidmap[gid] = tiled_gid
                 return gid
 
         else:
             return 0
 
-    def map_gid(self, tiled_gid: int) -> Optional[List[int]]:
+    def register_gid_check_flags(
+            self,
+            tiled_gid: int,
+    ) -> int:
+        """Used to manage the mapping of GIDs between .tmx and pytmx.
+
+        Checks the GID for rotation/flip flags
+
+        Args:
+            tiled_gid (int): GID that is found in TMX data.
+
+        Returns:
+            int: New or existing GID for pytmx use.
+
         """
-        Used to lookup a GID read from a TMX file's data
+        # NOTE: the register* methods are getting really spaghetti-like
+        if tiled_gid == 0:
+            return 0
+        elif tiled_gid < GID_TRANS_ROT:
+            return self.register_gid(tiled_gid)
+        else:
+            return self.register_gid(*decode_gid(tiled_gid))
+
+    def map_gid(self, tiled_gid: int) -> Optional[List[int]]:
+        """Used to lookup a GID read from a TMX file's data.
 
         Args:
-            tiled_gid: GID that is found in TMX data
+            tiled_gid (int): GID. that is found in the .tmx file data.
+
+        Returns:
+            Optional[List[int]]: ???
 
         """
         try:
             return self.gidmap[int(tiled_gid)]
         except KeyError:
             return None
         except TypeError:
             msg = "GIDs must be an integer"
             logger.debug(msg)
             raise TypeError(msg)
 
     def map_gid2(self, tiled_gid: int) -> List[Tuple[int, Optional[int]]]:
-        """
-        WIP.  need to refactor the gid code
-
-        """
+        """WIP.  need to refactor the gid code"""
         tiled_gid = int(tiled_gid)
 
         # gidmap is a default dict, so cannot trust to raise KeyError
         if tiled_gid in self.gidmap:
             return self.gidmap[tiled_gid]
         else:
             gid = self.register_gid(tiled_gid)
             return [(gid, None)]
 
 
 class TiledTileset(TiledElement):
     """Represents a Tiled Tileset
 
-    External tilesets are supported.  GID/ID's from Tiled are not guaranteed to
-    be the same after loaded.
+    External tilesets are supported.  GID/ID's from Tiled are not
+    guaranteed to be the same after loaded.
+
     """
 
-    def __init__(self, parent, node):
+    def __init__(self, parent, node) -> None:
+        """Represents a Tiled Tileset
+
+        Args:
+            parent (???): ???.
+            node (ElementTree.Element): ???.
+
+        """
         TiledElement.__init__(self)
         self.parent = parent
         self.offset = (0, 0)
 
         # defaults from the specification
         self.firstgid = 0
         self.source = None
@@ -1096,23 +1203,25 @@
         # image properties
         self.trans = None
         self.width = 0
         self.height = 0
 
         self.parse_xml(node)
 
-    def parse_xml(self, node):
-        """
-        Parse a Tileset from ElementTree xml element
+    def parse_xml(self, node: ElementTree.Element) -> "TiledTileset":
+        """Parse a Tileset from ElementTree xml element.
 
-        A bit of mangling is done here so that tilesets that have external
-        TSX files appear the same as those that don't
+        A bit of mangling is done here so that tilesets that have
+        external TSX files appear the same as those that don't.
 
         Args:
-            node: node to parse
+            node (ElementTree.Element): Node to parse.
+
+        Returns:
+            TiledTileset:
 
         """
         # if true, then node references an external tileset
         source = node.get("source", None)
         if source:
             if source[-4:].lower() == ".tsx":
 
@@ -1178,15 +1287,15 @@
             if anim is not None:
                 for frame in anim.findall("frame"):
                     duration = int(frame.get("duration"))
                     gid = register_gid(int(frame.get("tileid")) + self.firstgid)
                     frames.append(AnimationFrame(gid, duration))
 
             for objgrp_node in child.findall("objectgroup"):
-                objectgroup = TiledObjectGroup(self.parent, objgrp_node)
+                objectgroup = TiledObjectGroup(self.parent, objgrp_node, None)
                 p["colliders"] = objectgroup
 
             for gid, flags in self.parent.map_gid2(tiled_gid + self.firstgid):
                 self.parent.set_tile_properties(gid, p)
 
         # handle the optional 'tileoffset' node
         self.offset = node.find("tileoffset")
@@ -1207,41 +1316,52 @@
             self.width = int(image_node.get("width"))
             self.height = int(image_node.get("height"))
 
         return self
 
 
 class TiledGroupLayer(TiledElement):
-    def __init__(self, parent, node):
+    def __init__(self, parent, node: ElementTree.Element) -> None:
+        """
+
+        Args:
+            parent (???): ???.
+            node (ElementTree.Element): ???.
+
+        """
         TiledElement.__init__(self)
         self.parent = parent
         self.name = None
         self.visible = 1
         self.parse_xml(node)
 
-    def parse_xml(self, node):
+    def parse_xml(self, node) -> "TiledGroupLayer":
         """
-        Parse a TiledGroup Layer from ElementTree xml node
+        Parse a TiledGroup layer from ElementTree xml node.
 
         Args:
-            node: node to parse
+            node (ElementTree.Element): Node to parse.
+
+        Returns:
+            TiledGroupLayer: The parsed TiledGroup layer.
 
         """
         self._set_properties(node)
         self.name = node.get("name", None)
         return self
 
 
 class TiledTileLayer(TiledElement):
-    """Represents a TileLayer
+    """Represents a TileLayer.
+
+    To just get the tile images, use TiledTileLayer.tiles().
 
-    To just get the tile images, use TiledTileLayer.tiles()
     """
 
-    def __init__(self, parent, node):
+    def __init__(self, parent, node) -> None:
         TiledElement.__init__(self)
         self.parent = parent
         self.data = list()
 
         # defaults from the specification
         self.name = None
         self.width = 0
@@ -1253,52 +1373,52 @@
 
         self.parse_xml(node)
 
     def __iter__(self):
         return self.iter_data()
 
     def iter_data(self) -> Iterable[Tuple[int, int, int]]:
-        """
-        Yields X, Y, GID tuples for each tile in the layer
+        """Yields X, Y, GID tuples for each tile in the layer.
 
         Returns:
-            Iterator of X, Y, GID tuples for each tile in the layer
+            Iterable[Tuple[int, int, int]]: Iterator of X, Y, GID tuples for each tile in the layer.
 
         """
         for y, row in enumerate(self.data):
             for x, gid in enumerate(row):
                 yield x, y, gid
 
     def tiles(self):
-        """
-        Yields X, Y, Image tuples for each tile in the layer
+        """Yields X, Y, Image tuples for each tile in the layer.
 
-        Returns:
-            Iterator of X, Y, Image tuples for each tile in the layer
+        Yields:
+            ???: Iterator of X, Y, Image tuples for each tile in the layer
 
         """
         images = self.parent.images
         for x, y, gid in [i for i in self.iter_data() if i[2]]:
             yield x, y, images[gid]
 
-    def _set_properties(self, node):
+    def _set_properties(self, node) -> None:
         TiledElement._set_properties(self, node)
 
         # TODO: make class/layer-specific type casting
         # layer height and width must be int, but TiledElement.set_properties()
         # make a float by default, so recast as int here
         self.height = int(self.height)
         self.width = int(self.width)
 
-    def parse_xml(self, node: ElementTree.Element):
-        """
-        Parse a Tile Layer from ElementTree xml node
+    def parse_xml(self, node: ElementTree.Element) -> "TiledTileLayer":
+        """Parse a Tile Layer from ElementTree xml node.
 
         Args:
-            node: node to parse
+            node (ElementTree.Element): Node to parse.
+
+        Returns:
+            TiledTileLayer: The parsed tile layer.
 
         """
         self._set_properties(node)
         data_node = node.find("data")
         chunk_nodes = data_node.findall("chunk")
         if chunk_nodes:
             msg = "TMX map size: infinite is not supported."
@@ -1307,78 +1427,74 @@
 
         child = data_node.find("tile")
         if child is not None:
             raise ValueError(
                 "XML tile elements are no longer supported. Must use base64 or csv map formats."
             )
 
-        reg = self.parent.register_gid
-        temp = list()
-        temp_append = temp.append
-        for gid in unpack_gids(
-            text=data_node.text.strip(),
-            encoding=data_node.get("encoding", None),
-            compression=data_node.get("compression", None),
-        ):
-            if gid == 0:
-                temp_append(0)
-            elif gid < GID_TRANS_ROT:
-                gid = reg(gid)
-                temp_append(gid)
-            else:
-                gid, flags = decode_gid(gid)
-                gid = reg(gid, flags)
-                temp_append(gid)
+        temp = [
+            self.parent.register_gid_check_flags(gid) for gid in
+            unpack_gids(
+                text=data_node.text.strip(),
+                encoding=data_node.get("encoding", None),
+                compression=data_node.get("compression", None),
+            )
+        ]
 
         self.data = reshape_data(temp, self.width)
         return self
 
 
 class TiledObjectGroup(TiledElement, list):
     """Represents a Tiled ObjectGroup
 
     Supports any operation of a normal list.
+
     """
 
-    def __init__(self, parent, node):
+    def __init__(self, parent, node, customs) -> None:
         TiledElement.__init__(self)
         self.parent = parent
 
         # defaults from the specification
         self.name = None
         self.color = None
         self.opacity = 1
         self.visible = 1
         self.offsetx = 0
         self.offsety = 0
+        self.custom_types = customs
         self.draworder = "index"
 
         self.parse_xml(node)
 
-    def parse_xml(self, node: ElementTree.Element):
-        """
-        Parse an Object Group from ElementTree xml node
+    def parse_xml(self, node: ElementTree.Element) -> "TiledObjectGroup":
+        """Parse an Object Group from ElementTree xml node
 
         Args:
-            node: node to parse
+            node (ElementTree.Element): Node to parse.
 
         """
-        self._set_properties(node)
-        self.extend(TiledObject(self.parent, child) for child in node.findall("object"))
+        self._set_properties(node, self.custom_types)
+        self.extend(
+            TiledObject(self.parent, child, self.custom_types)
+            for child in node.findall("object")
+        )
 
         return self
 
 
 class TiledObject(TiledElement):
-    """Represents a any Tiled Object
+    """Represents any Tiled Object.
+
+    Supported types: Box, Ellipse, Tile Object, Polyline, Polygon.
 
-    Supported types: Box, Ellipse, Tile Object, Polyline, Polygon
     """
 
-    def __init__(self, parent, node):
+    def __init__(self, parent, node, custom_types) -> None:
         TiledElement.__init__(self)
         self.parent = parent
 
         # defaults from the specification
         self.id = 0
         self.name = None
         self.type = None
@@ -1387,48 +1503,53 @@
         self.width = 0
         self.height = 0
         self.rotation = 0
         self.gid = 0
         self.visible = 1
         self.closed = True
         self.template = None
+        self.custom_types = custom_types
 
         self.parse_xml(node)
 
     @property
     def image(self):
-        """
-        Image for the object, if assigned
+        """Image for the object, if assigned.
 
         Returns:
-            the image object type will depend on the loader (ie. pygame surface)
+            ???: The image object type will depend on the loader (ie. pygame.Surface).
 
         """
         if self.gid:
             return self.parent.images[self.gid]
         return None
 
-    def parse_xml(self, node: ElementTree.Element):
-        """
-        Parse an Object from ElementTree xml node
+    def parse_xml(self, node: ElementTree.Element) -> "TiledObject":
+        """Parse an Object from ElementTree xml node.
 
         Args:
-            node: the node to be parsed
+            node (ElementTree.Element): The node to be parsed.
+
+        Returns:
+            TiledObject: The parsed xml node.
 
         """
 
         def read_points(text):
-            """parse a text string of float tuples and return [(x,...),...]"""
+            """
+            Parse a text string of float tuples and return [(x,...),...]
+
+            """
             return tuple(tuple(map(float, i.split(","))) for i in text.split())
 
-        self._set_properties(node)
+        self._set_properties(node, self.custom_types)
 
         # correctly handle "tile objects" (object with gid set)
         if self.gid:
-            self.gid = self.parent.register_gid(self.gid)
+            self.gid = self.parent.register_gid_check_flags(self.gid)
 
         points = None
         polygon = node.find("polygon")
         if polygon is not None:
             points = read_points(polygon.get("points"))
             self.closed = True
 
@@ -1450,41 +1571,44 @@
                     y2 = y
             self.width = abs(x1) + abs(x2)
             self.height = abs(y1) + abs(y2)
             self.points = tuple([Point(i[0] + self.x, i[1] + self.y) for i in points])
 
         return self
 
-    def apply_transformations(self):
-        """Return all points for object, taking in account rotation"""
+    def apply_transformations(self) -> List[Point]:
+        """Return all points for object, taking in account rotation."""
         if hasattr(self, "points"):
             return rotate(self.points, self, self.rotation)
         else:
             return rotate(self.as_points, self, self.rotation)
 
     @property
-    def as_points(self):
+    def as_points(
+        self,
+    ) -> List[Point]:
         return [
             Point(*i)
             for i in [
                 (self.x, self.y),
                 (self.x, self.y + self.height),
                 (self.x + self.width, self.y + self.height),
                 (self.x + self.width, self.y),
             ]
         ]
 
 
 class TiledImageLayer(TiledElement):
-    """Represents Tiled Image Layer
+    """Represents Tiled Image Layer.
 
     The image associated with this layer will be loaded and assigned a GID.
+
     """
 
-    def __init__(self, parent, node):
+    def __init__(self, parent, node: ElementTree.Element) -> None:
         TiledElement.__init__(self)
         self.parent = parent
         self.source = None
         self.trans = None
         self.gid = 0
 
         # defaults from the specification
@@ -1492,51 +1616,44 @@
         self.opacity = 1
         self.visible = 1
 
         self.parse_xml(node)
 
     @property
     def image(self):
-        """
-        Image for the object, if assigned
+        """Image for the object, if assigned.
 
         Returns:
-            the image object type will depend on the loader (ie. pygame surface)
+            ???: the image object type will depend on the loader (ie. pygame.Surface).
 
         """
         if self.gid:
             return self.parent.images[self.gid]
         return None
 
     def parse_xml(self, node: ElementTree.Element):
-        """
-        Parse an Image Layer from ElementTree xml node
-
-        """
+        """Parse an Image Layer from ElementTree xml node."""
         self._set_properties(node)
         self.name = node.get("name", None)
         self.opacity = node.get("opacity", self.opacity)
         self.visible = node.get("visible", self.visible)
         image_node = node.find("image")
         self.source = image_node.get("source", None)
         self.trans = image_node.get("trans", None)
         return self
 
 
 class TiledProperty(TiledElement):
-    """
-    Represents Tiled Property
-
-    """
+    """Represents Tiled Property."""
 
-    def __init__(self, parent, node):
+    def __init__(self, parent, node: ElementTree.Element) -> None:
         TiledElement.__init__(self)
 
         # defaults from the specification
         self.name = None
         self.type = None
         self.value = None
 
         self.parse_xml(node)
 
-    def parse_xml(self, node):
+    def parse_xml(self, node: ElementTree.Element) -> None:
         pass
```

### Comparing `PyTMX-3.31/pytmx/util_pygame.py` & `PyTMX-3.32/pytmx/util_pygame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright (C) 2012-2017, Leif Theden <leif.theden@gmail.com>
+Copyright (C) 2012-2023, Leif Theden <leif.theden@gmail.com>
 
 This file is part of pytmx.
 
 pytmx is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as
 published by the Free Software Foundation, either version 3 of the
 License, or (at your option) any later version.
```

### Comparing `PyTMX-3.31/pytmx/util_pygame_sdl2.py` & `PyTMX-3.32/pytmx/util_pygame_sdl2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (C) 2012-2021, Leif Theden <leif.theden@gmail.com>
+Copyright (C) 2012-2022, Leif Theden <leif.theden@gmail.com>
 
 This file is part of pytmx.
 
 pytmx is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as
 published by the Free Software Foundation, either version 3 of the
 License, or (at your option) any later version.
```

### Comparing `PyTMX-3.31/pytmx/util_pyglet.py` & `PyTMX-3.32/pytmx/util_pyglet.py`

 * *Files identical despite different names*

### Comparing `PyTMX-3.31/pytmx/util_pysdl2.py` & `PyTMX-3.32/pytmx/util_pysdl2.py`

 * *Files identical despite different names*

### Comparing `PyTMX-3.31/readme.md` & `PyTMX-3.32/readme.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,74 @@
-## PyTMX
-##### For Python 3.7+
+<div align="center">
 
-If you have any problems or suggestions, please open an issue.
+# pytmx
 
-If you find this useful, please consider making a donation to help support it
-https://liberapay.com/ltheden/donate
+A map loader for Python/pygame, designed for video games
 
-*Released under the LGPL v3*
+![pypi version](https://img.shields.io/pypi/v/pytmx)
+![license](https://img.shields.io/github/license/bitcraft/pytmx)
+![code style](https://img.shields.io/badge/code%20style-black-000000.svg)
+![pypi downloads](https://img.shields.io/pypi/dm/pytmx)
 
-### See the "apps" folder for example use and cut/paste code.
+</div>
 
-News
+About
 ===============================================================================
-
-__09/21/21__ - Support pygame._sdl2  
-__09/08/21__ - Much faster loading, especially for large maps  
-__12/04/20__ - Support tile colliders  
-__08/28/20__ - Python 2.7 support removed.  Use the "py27-legacy" branch.  
-__11/13/15__ - Animations are now loaded  
-__07/08/15__ - Documentation overhaul  
-__04/18/15__ - Document support for pysdl2 and pyglet  
-__09/14/14__ - Merge python3 branch.  Now 100% compatible with 2.7 and 3.3+  
-__07/26/14__ - New python3/2 release.  Check it out in the python3 branch.  
-__05/29/14__ - Added support for rotated objects and floating point  
-__04/04/14__ - New Six Branch created  
-__02/28/14__ - Image layer support, object points changed, new test.py!  
-__02/24/14__ - New Python 3 Support: see python3 branch  
-__02/06/14__ - Python 3 support coming soon  
-
-
-Introduction
-===============================================================================
-
-PyTMX is a map loader for python/pygame designed for games.  It provides smart
-tile loading with a fast and efficient storage base.  Not only does it
+**For Python 3.7+**
+A map loader for python/pygame designed for games. It provides smart
+tile loading with a fast and efficient storage base. Not only does it
 correctly handle most Tiled object types, it also will load metadata for
 them so you can modify your maps and objects in Tiled instead of modifying
-your source code.
+your source code. See the "apps" folder for example use and cut/paste code.
 
-New support for pysdl2 and pyglet!  Check it out!
-
-Because PyTMX was built with games in mind, it differs slightly from Tiled in
+Since pytmx was built with games in mind, it differs slightly from Tiled in
 a few minor aspects:
+ - Layers not aligned to the grid are not supported.
+ - Some object metadata attribute names are not supported (see "Reserved Names").
+ - pytmx is not a rendering engine or Tiled Map Editor.
 
-- Layers not aligned to the grid are not supported.
-- Some object metadata attribute names are not supported (see "Reserved Names")
-
-PyTMX strives to balance performance and flexibility.  Feel free to use the
+pytmx strives to balance performance and flexibility. Feel free to use the
 classes provided in pytmx.py as superclasses for your own maps, or simply
-load the data with PyTMX and copy the data into your own classes with the api.
+load the data with pytmx and copy the data into your own classes with the API.
 
-There is no save feature.  Once the map is loaded, it will be up to
-you to provide a way to save changes to the map.  I've used the pickle module
+**There is no save feature.** Once the map is loaded, it will be up to
+you to provide a way to save changes to the map. I've used the pickle module
 with good results.
 
-I need to clarify a few things:
-- pytmx is not a rendering engine
-- pytmx is not the Tiled Map Editor
+**As Python 2.7 is now EOL**, any changes moving forward past version 3.21.7 will
+not take python 2.7 support into consideration and any breaking changes will not be 
+fixed.
 
+If you have any problems or suggestions, please open an issue or join the Discord server.
+https://discord.gg/2taTP4aYR6
 
-Python 2.7 Support
+If you find this useful, please consider making a donation to help support it.
+https://liberapay.com/ltheden/donate
+
+*Released under the LGPL V3*
+
+News
 ===============================================================================
-As Python 2.7 is now EOL, any changes moving forward past version 3.21.7 will
-not take python 2.7 support into consideration and any breaking changes will
-not be fixed.
+
+| Date     | Changes
+| -------- | --------
+| 09/21/21 | Supports pygame._sdl2.
+| 09/08/21 | Much faster loading, especially for large maps.
+| 12/04/20 | Support tile colliders.
+| 08/28/20 | Python 2.7 support removed. Use the "py27-legacy" branch.
+| 11/13/15 | Animations are now loaded.
+| 07/08/15 | Documentation overhaul.
+| 04/18/15 | Document support for pysdl2 and pyglet.
+| 09/14/14 | Merge python3 branch. Now 100% compatible with 2.7 and 3.3+.
+| 07/26/14 | New python3/2 release. Check it out in the python3 branch.
+| 05/29/14 | Added support for rotated objects and floating point.
+| 04/04/14 | New Six Branch created.
+| 02/28/14 | Image layer support, object points changed, new test.py!
+| 02/24/14 | New Python 3 Support: see python3 branch.
+| 02/06/14 | Python 3 support coming soon.
 
 
 Documentation
 ===============================================================================
 
 This readme does include some detailed documentation, but the full API reference
 and documentation can be found at the site below.  For examples of real use,
@@ -86,21 +87,14 @@
 6. [Custom Image Loading](#custom-image-loading)
 7. [Working with Tile Layers](#working-with-tile-layers)
 8. [Getting Tile Animations](#getting-tile-animations)
 9. [Working with Objects](#working-with-objects)
 10. [Understanding Properties](#understanding-properties)
 
 
-Getting Help
-===============================================================================
-
-For bugs or feature requests, please use the issues feature of github.  For
-all other general questions, join me on IRC at freenode.net #pygame.
-
-
 Design Goals and Features
 ===============================================================================
 
 * API with many handy functions
 * Memory efficient and performant
 * Loads data, "properties" metadata, and images from Tiled's TMX format
 * Supports base64, csv, gzip, zlib and uncompressed XML formats
@@ -108,32 +102,32 @@
 * Point data for polygon and polyline objects
 * Automatic flipping and rotation of tiles
 * Tile collider groups
 * Built-in image loading with pygame, pysdl2, and pyglet
 * Loads animation information
 
 
-Why use PyTMX?
+Why use pytmx?
 ===============================================================================
 
-### PyTMX is efficient:
+### pytmx is efficient:
 * Map information is stored as integers, not python objects (32+kb)
 * Extensive use of generators and iterators make it easy on memory
 * Code is designed for compact size and readability
 
-### PyTMX is flexible:
+### pytmx is flexible:
 * Supports all major Tiled features and object types
-* PyTMX data classes can be extended
+* pytmx data classes can be extended
 * Does not force you to render data in any particular way
 * Includes many checks to give useful debugging information
 * Supports pygame, pyglet, and pysdl2 image loading
 
-### PyTMX is supported:
+### pytmx is supported:
 * GitHub hosting allows for community participation
-* I have kept PyTMX current with new versions of Tiled since v.7
+* I have kept pytmx current with new versions of Tiled since v.7
 
 
 Installation
 ===============================================================================
 
 Install from pip
 
@@ -347,15 +341,15 @@
     ...
 ```
 
 
 Working with Tile Layers
 ===============================================================================
 
-Pytmx loads tile layers and their data:
+pytmx loads tile layers and their data:
 
 - name
 - opacity
 - visible: indicates if user has hidden the layer
 - data: 2d array of all tile gids (normally not needed to use!)
 - properties
 
@@ -442,15 +436,15 @@
 layer[y][x] = new_gid
 ```
 
 Working with Objects
 ===============================================================================
 
 Tiled "objects" are things that are created in object layers, and include
-polygons, polylings, boxes, ellipses, and tile objects.  Pytmx loads all objects
+polygons, polylings, boxes, ellipses, and tile objects.  pytmx loads all objects
 and their data:
 
 - name
 - type
 - x
 - y
 - width
@@ -497,15 +491,15 @@
     ...
 ```
 
 Understanding Properties
 ===============================================================================
 
 Properties are a powerful feature of Tiled that allows the level designer to
-assign key/value data to individual maps, tilesets, tiles, and objects.  Pytmx
+assign key/value data to individual maps, tilesets, tiles, and objects.  pytmx
 includes full support for reading this data so you can set parameters for stuff
 in Tiled, instead of maintaining external data files, or even values in source.
 
 Properties are created by the user in tiled.  There is also another set of data
 that is part of each object, accessed by normal object attributes.  This other
 data is not set directly by the user, but is instead set by tiled.  Typical
 data that is object attributes are: 'name', 'x', 'opacity', or 'id'.
@@ -547,15 +541,15 @@
 ================================================================================
 
 Tiled supports user created metadata called "properties" for all the built-in
 objects, like the map, tileset, objects, etc.  Due to how the Tiled XML data is
 stored, there are situations where Tiled internal metadata might have the same
 name as user-created properties.
 
-Pytmx will raise a ValueError if it detects any conflicts.  This check is
+pytmx will raise a ValueError if it detects any conflicts.  This check is
 performed in order to prevent any situations where a level change might be made
 in Tiled, but the programmer/designer doesn't know or forgets if the change was
 made in the Tiled metadata or the user properties.
 
 I realize that it creates problems with certain common names like "id", or
 "color".  Overall, this check will help enforce clean design. 
  
@@ -585,15 +579,15 @@
 
 object:      id, name, type, x, y, width, height, gid, properties, polygon,  
              polyline, image
 
 
 #### Please consider the following:
 
-PyTMX is a map __loader__.  Pytmx takes the pain out of parsing XML, variable type conversion, shape loading, properties, and of course image loading.  When asking for help, please understand that I want people to make their own games or utilities, and that PyTMX is able to make Tiled Maps easy to use.
+pytmx is a map __loader__.  pytmx takes the pain out of parsing XML, variable type conversion, shape loading, properties, and of course image loading.  When asking for help, please understand that I want people to make their own games or utilities, and that pytmx is able to make Tiled Maps easy to use.
 
 pytmx is not going to make your JRPG for you.  You will need to do that yourself, and I, the author, cannot simply respond to every new developer who expects pytmx, pygame, or any other game library to simply make it work for them.  Programming is a learned skill, and for most it takes practice and diligent study to get proficient at.  I'm generally open to help, so before you flame me on your blog or reddit, understand what pytmx is used for, read the documentation and copy/paste the demo code if you have to.  Thank you.
 
 I have a working solution to using Tiled Maps and Pygame ready for you.  If you simply want a library to render the maps for you, please check it out, as they are designed to work together.
 
 http://github.com/bitcraft/pyscroll
```

