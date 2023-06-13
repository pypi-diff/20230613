# Comparing `tmp/mapchete_xarray-2022.7.0.tar.gz` & `tmp/mapchete_xarray-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapchete_xarray-2022.7.0.tar", last modified: Tue Jul 12 13:42:53 2022, max compression
+gzip compressed data, was "mapchete_xarray-2023.6.0.tar", last modified: Tue Jun 13 12:43:32 2023, max compression
```

## Comparing `mapchete_xarray-2022.7.0.tar` & `mapchete_xarray-2023.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 13:42:53.009777 mapchete_xarray-2022.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-07-12 13:42:44.000000 mapchete_xarray-2022.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5338 2022-07-12 13:42:53.009777 mapchete_xarray-2022.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4691 2022-07-12 13:42:44.000000 mapchete_xarray-2022.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 13:42:53.009777 mapchete_xarray-2022.7.0/mapchete_xarray/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-07-12 13:42:44.000000 mapchete_xarray-2022.7.0/mapchete_xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6442 2022-07-12 13:42:44.000000 mapchete_xarray-2022.7.0/mapchete_xarray/_input.py
--rw-r--r--   0 runner    (1001) docker     (121)    21974 2022-07-12 13:42:44.000000 mapchete_xarray-2022.7.0/mapchete_xarray/_output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 13:42:53.009777 mapchete_xarray-2022.7.0/mapchete_xarray/processes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-12 13:42:44.000000 mapchete_xarray-2022.7.0/mapchete_xarray/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-07-12 13:42:44.000000 mapchete_xarray-2022.7.0/mapchete_xarray/processes/convert_to_xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 13:42:53.009777 mapchete_xarray-2022.7.0/mapchete_xarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5338 2022-07-12 13:42:52.000000 mapchete_xarray-2022.7.0/mapchete_xarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-07-12 13:42:52.000000 mapchete_xarray-2022.7.0/mapchete_xarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 13:42:52.000000 mapchete_xarray-2022.7.0/mapchete_xarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-12 13:42:52.000000 mapchete_xarray-2022.7.0/mapchete_xarray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-07-12 13:42:52.000000 mapchete_xarray-2022.7.0/mapchete_xarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-12 13:42:52.000000 mapchete_xarray-2022.7.0/mapchete_xarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-07-12 13:42:44.000000 mapchete_xarray-2022.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-07-12 13:42:53.009777 mapchete_xarray-2022.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-07-12 13:42:44.000000 mapchete_xarray-2022.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:43:32.844368 mapchete_xarray-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-13 12:43:20.000000 mapchete_xarray-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-13 12:43:32.844368 mapchete_xarray-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-13 12:43:20.000000 mapchete_xarray-2023.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:43:32.844368 mapchete_xarray-2023.6.0/mapchete_xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 12:43:20.000000 mapchete_xarray-2023.6.0/mapchete_xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-13 12:43:20.000000 mapchete_xarray-2023.6.0/mapchete_xarray/_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23185 2023-06-13 12:43:20.000000 mapchete_xarray-2023.6.0/mapchete_xarray/_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:43:32.844368 mapchete_xarray-2023.6.0/mapchete_xarray/processes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:43:20.000000 mapchete_xarray-2023.6.0/mapchete_xarray/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-13 12:43:20.000000 mapchete_xarray-2023.6.0/mapchete_xarray/processes/convert_to_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:43:32.844368 mapchete_xarray-2023.6.0/mapchete_xarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-13 12:43:32.000000 mapchete_xarray-2023.6.0/mapchete_xarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 12:43:32.000000 mapchete_xarray-2023.6.0/mapchete_xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:43:32.000000 mapchete_xarray-2023.6.0/mapchete_xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 12:43:32.000000 mapchete_xarray-2023.6.0/mapchete_xarray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 12:43:32.000000 mapchete_xarray-2023.6.0/mapchete_xarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 12:43:32.000000 mapchete_xarray-2023.6.0/mapchete_xarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-13 12:43:20.000000 mapchete_xarray-2023.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 12:43:32.844368 mapchete_xarray-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-13 12:43:20.000000 mapchete_xarray-2023.6.0/setup.py
```

### Comparing `mapchete_xarray-2022.7.0/LICENSE` & `mapchete_xarray-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete_xarray-2022.7.0/PKG-INFO` & `mapchete_xarray-2023.6.0/mapchete_xarray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
-Name: mapchete_xarray
-Version: 2022.7.0
+Name: mapchete-xarray
+Version: 2023.6.0
 Summary: Mapchete xarray output driver
 Home-page: https://github.com/ungarj/mapchete_xarray
 Author: Joachim Ungar
 Author-email: joachim.ungar@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===============
 mapchete xarray
 ===============
 
@@ -188,9 +187,7 @@
 MIT License
 
 Copyright (c) 2019-2022 `EOX IT Services`_
 
 .. _`EOX IT Services`: https://eox.at/
 .. _`Zarr`: https://zarr.readthedocs.io/en/stable/index.html
 .. _`GDAL Zarr driver`: https://gdal.org/drivers/raster/zarr.html
-
-
```

### Comparing `mapchete_xarray-2022.7.0/README.rst` & `mapchete_xarray-2023.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete_xarray-2022.7.0/mapchete_xarray/_input.py` & `mapchete_xarray-2023.6.0/mapchete_xarray/_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 """
 Contains all classes required to use the xarray driver as mapchete input.
 """
 
 import numpy as np
 import xarray as xr
-import zarr
 from mapchete.config import snap_bounds
 from mapchete.formats import base, load_metadata
-from mapchete.io import path_exists
 from mapchete.io.vector import reproject_geometry
 from shapely.geometry import box
-from zarr.storage import FSStore
 
 
 class InputData(base.InputData):
     """In case this driver is used when being a readonly input to another process."""
 
     _ds = None
 
     def __init__(self, input_params, **kwargs):
         """Initialize."""
         super().__init__(input_params, **kwargs)
         self.path = input_params["path"]
-        if not path_exists(self.path):  # pragma: no cover
+        if not self.path.exists():  # pragma: no cover
             raise FileNotFoundError(f"path {self.path} does not exist")
         mapchete_params = self.ds.attrs.get("mapchete")
         if mapchete_params is None:  # pragma: no cover
             raise TypeError(
                 f"zarr archive at {self.path} exists but does not hold mapchete metadata"
             )
         mapchete_metadata = load_metadata(mapchete_params)
```

### Comparing `mapchete_xarray-2022.7.0/mapchete_xarray/_output.py` & `mapchete_xarray-2023.6.0/mapchete_xarray/_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,31 @@
 import numpy as np
 import xarray as xr
 import zarr
 from mapchete.config import snap_bounds, validate_values
 from mapchete.errors import MapcheteConfigError
 from mapchete.formats import base
 from mapchete.formats.tools import compare_metadata_params, dump_metadata, load_metadata
-from mapchete.io import fs_from_path, path_exists
 from mapchete.io.raster import bounds_to_ranges, create_mosaic, extract_from_array
+from mapchete.path import MPath
 from rasterio.transform import from_origin
 from tilematrix import Bounds
 from zarr.storage import FSStore
 
 logger = logging.getLogger(__name__)
 
 METADATA = {
     "driver_name": "xarray",
     "data_type": "raster",
     "mode": "w",
     "file_extensions": ["zarr"],
 }
 
+DEFAULT_TIME_CHUNKSIZE = 8
+
 
 class OutputDataReader(base.SingleFileOutputReader):
 
     METADATA = METADATA
     _ds = None
 
     def __init__(self, output_params, *args, **kwargs):
@@ -44,15 +46,14 @@
         self.output_params = output_params
         self.nodata = output_params.get("nodata", 0)
         self.storage = "zarr"
         self.file_extension = ".zarr"
         self.path = output_params["path"]
         if not self.path.endswith(self.file_extension):
             raise MapcheteConfigError("output path must end with .zarr")
-        self.fs = fs_from_path(self.path)
         self.output_params = output_params
         self.zoom = output_params["delimiters"]["zoom"][0]
 
         if output_params.get("band_names"):
             self.band_names = output_params.get("band_names")
             self.count = len(self.band_names)
         elif output_params.get("bands"):
@@ -243,17 +244,17 @@
 
     METADATA = METADATA
 
     def __init__(self, output_params, *args, **kwargs):
         super().__init__(output_params, *args, **kwargs)
 
     def prepare(self, **kwargs):
-        if path_exists(self.path):
+        if self.path.exists():
             # verify it is compatible with our output parameters / chunking
-            archive = zarr.open(FSStore(f"{self.path}"))
+            archive = zarr.open(FSStore(f"{self.path}", fs=self.path.fs))
             mapchete_params = archive.attrs.get("mapchete")
             if mapchete_params is None:  # pragma: no cover
                 raise TypeError(
                     f"zarr archive at {self.path} exists but does not hold mapchete metadata"
                 )
             existing = load_metadata(mapchete_params)
             current = load_metadata(dump_metadata(self.output_params))
@@ -273,14 +274,32 @@
                 x_axis_name=self.x_axis_name,
                 y_axis_name=self.y_axis_name,
                 time_axis_name=self.time_axis_name,
                 area_or_point=self.area_or_point,
                 output_metadata=dump_metadata(self.output_params),
             )
 
+    def _zarr_chunk_from_xy(self, x, y):
+
+        # determine row
+        pixel_y_size = _pixel_y_size(self.bounds.top, self.bounds.bottom, self.shape[0])
+        tile_y_size = round(
+            pixel_y_size * self.pyramid.tile_size * self.pyramid.metatiling, 20
+        )
+        row = abs(int((self.ds[self.y_axis_name].max() - y) / tile_y_size))
+
+        # determine column
+        pixel_x_size = _pixel_x_size(self.bounds.right, self.bounds.left, self.shape[1])
+        tile_x_size = round(
+            pixel_x_size * self.pyramid.tile_size * self.pyramid.metatiling, 20
+        )
+        col = abs(int((x - self.ds[self.x_axis_name].min()) / tile_x_size))
+
+        return row, col
+
     def tiles_exist(self, process_tile=None, output_tile=None):
         """
         Check whether output tiles of a tile (either process or output) exists.
 
         Parameters
         ----------
         process_tile : ``BufferedTile``
@@ -288,18 +307,28 @@
         output_tile : ``BufferedTile``
             must be member of output ``TilePyramid``
 
         Returns
         -------
         exists : bool
         """
-        bounds = process_tile.bounds if process_tile else output_tile.bounds
-        for var in self._read(bounds=bounds).values():
-            if np.any(var != self.nodata):
-                return True
+
+        tile = process_tile or output_tile
+        zarr_chunk_row, zarr_chunk_col = self._zarr_chunk_from_xy(
+            tile.bbox.centroid.x, tile.bbox.centroid.y
+        )
+
+        for var in self.ds:
+
+            if self.time:
+                if (self.path / var / f"0.{zarr_chunk_row}.{zarr_chunk_col}").exists():
+                    return True
+            else:
+                if (self.path / var / f"{zarr_chunk_row}.{zarr_chunk_col}").exists():
+                    return True
         return False
 
     def is_valid_with_config(self, config):
         """
         Check if output format is valid with other process parameters.
 
         Parameters
@@ -315,15 +344,15 @@
             raise ValueError("zarr output can only be used with a single zoom")
         if "time" in config:
             if "pattern" not in config["time"] and "steps" not in config["time"]:
                 raise ValueError(
                     "when using a time axis, please specify the time stamps either through "
                     "'pattern' or 'steps'"
                 )
-        return validate_values(config, [("path", str)])
+        return validate_values(config, [("path", (str, MPath))])
 
     def write(self, process_tile, data):
         """
         Write data from one or more process tiles.
 
         Parameters
         ----------
@@ -341,15 +370,15 @@
         }
 
         if self.time:
             coords[self.time_axis_name] = data.time.values
 
         def write_zarr(ds, region):
             ds.to_zarr(
-                FSStore(self.path),
+                FSStore(str(self.path), fs=self.path.fs),
                 mode="r+",
                 compute=True,
                 safe_chunks=True,
                 region=region,
             )
 
         ds = self.output_cleaned(data)
@@ -550,14 +579,22 @@
             else:  # pragma: no cover
                 raise TypeError(
                     f"band indexes must either be integers or strings, not: {i}"
                 )
         return out
 
 
+def _pixel_x_size(right, left, width):
+    return (right - left) / width
+
+
+def _pixel_y_size(top, bottom, height):
+    return (top - bottom) / -height
+
+
 def initialize_zarr(
     path=None,
     bounds=None,
     shape=None,
     crs=None,
     time=None,
     fill_value=None,
@@ -566,21 +603,22 @@
     dtype="uint8",
     x_axis_name="X",
     y_axis_name="Y",
     time_axis_name="time",
     area_or_point="Area",
     output_metadata=None,
 ):
-    if path_exists(path):  # pragma: no cover
+    path = MPath.from_inp(path)
+    if path.exists():  # pragma: no cover
         raise IOError(f"cannot initialize zarr storage as path already exists: {path}")
 
     height, width = shape
     bounds = Bounds(*bounds)
-    pixel_x_size = (bounds.right - bounds.left) / width
-    pixel_y_size = (bounds.top - bounds.bottom) / -height
+    pixel_x_size = _pixel_x_size(bounds.right, bounds.left, width)
+    pixel_y_size = _pixel_y_size(bounds.top, bounds.bottom, height)
 
     coord_x = [bounds.left + pixel_x_size / 2 + i * pixel_x_size for i in range(width)]
     coord_y = [bounds.top + pixel_y_size / 2 + i * pixel_y_size for i in range(height)]
 
     axis_names = [y_axis_name, x_axis_name]
     coords = {
         x_axis_name: ([x_axis_name], coord_x),
@@ -621,34 +659,38 @@
         else:  # pragma: no cover
             raise ValueError(
                 "timestamps have to be provied either as list in 'steps' or a pattern in 'pattern'"
             )
         coords[time_axis_name] = coord_time
 
         output_shape = (len(coord_time), *shape)
-        output_chunks = (time.get("chunksize", 8), chunksize, chunksize)
+        output_chunks = (
+            time.get("chunksize", DEFAULT_TIME_CHUNKSIZE),
+            chunksize,
+            chunksize,
+        )
         axis_names = [time_axis_name] + axis_names
 
     else:
         output_shape = shape
         output_chunks = (chunksize, chunksize)
 
     try:
         # write zarr
         ds = xr.Dataset(coords=coords)
         ds.to_zarr(
-            FSStore(path),
+            FSStore(path, fs=path.fs),
             compute=False,
             encoding={var: {"_FillValue": fill_value} for var in ds.data_vars},
             safe_chunks=True,
         )
 
         # add GDAL metadata for each band
         for band_name in band_names:
-            store = FSStore(f"{path}/{band_name}")
+            store = FSStore(f"{path}/{band_name}", fs=path.fs)
             zarr.creation.create(
                 shape=output_shape,
                 chunks=output_chunks,
                 dtype=dtype,
                 store=store,
             )
 
@@ -660,12 +702,9 @@
         # add global metadata
         if output_metadata:
             zarr.open(FSStore(f"{path}")).attrs.update(mapchete=output_metadata)
         zarr.consolidate_metadata(path)
 
     except Exception:  # pragma: no cover
         # remove leftovers if something failed during initialization
-        try:
-            fs_from_path(path).rm(path, recursive=True)
-        except FileNotFoundError:
-            pass
+        path.rm(recursive=True, ignore_errors=True)
         raise
```

### Comparing `mapchete_xarray-2022.7.0/mapchete_xarray/processes/convert_to_xarray.py` & `mapchete_xarray-2023.6.0/mapchete_xarray/processes/convert_to_xarray.py`

 * *Files identical despite different names*

### Comparing `mapchete_xarray-2022.7.0/mapchete_xarray.egg-info/PKG-INFO` & `mapchete_xarray-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
-Name: mapchete-xarray
-Version: 2022.7.0
+Name: mapchete_xarray
+Version: 2023.6.0
 Summary: Mapchete xarray output driver
 Home-page: https://github.com/ungarj/mapchete_xarray
 Author: Joachim Ungar
 Author-email: joachim.ungar@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===============
 mapchete xarray
 ===============
 
@@ -188,9 +187,7 @@
 MIT License
 
 Copyright (c) 2019-2022 `EOX IT Services`_
 
 .. _`EOX IT Services`: https://eox.at/
 .. _`Zarr`: https://zarr.readthedocs.io/en/stable/index.html
 .. _`GDAL Zarr driver`: https://gdal.org/drivers/raster/zarr.html
-
-
```

### Comparing `mapchete_xarray-2022.7.0/setup.py` & `mapchete_xarray-2023.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,14 @@
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: GIS",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
 )
```

