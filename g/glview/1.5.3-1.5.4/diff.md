# Comparing `tmp/glview-1.5.3.tar.gz` & `tmp/glview-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glview-1.5.3.tar", last modified: Fri Apr 28 09:52:42 2023, max compression
+gzip compressed data, was "glview-1.5.4.tar", last modified: Tue Jun 13 14:00:33 2023, max compression
```

## Comparing `glview-1.5.3.tar` & `glview-1.5.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-28 09:52:42.564791 glview-1.5.3/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.5.3/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.5.3/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-28 09:52:42.564791 glview-1.5.3/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      361 2023-03-13 15:45:56.000000 glview-1.5.3/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-28 09:52:42.564791 glview-1.5.3/glview/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-03-15 12:51:16.000000 glview-1.5.3/glview/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.5.3/glview/argv.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    11545 2023-04-28 08:34:45.000000 glview-1.5.3/glview/glrenderer.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     9287 2023-04-28 08:25:57.000000 glview-1.5.3/glview/glview.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     6950 2023-03-13 15:45:56.000000 glview-1.5.3/glview/imageprovider.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      285 2023-03-13 15:45:56.000000 glview-1.5.3/glview/panzoom.vs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    17541 2023-04-28 08:34:45.000000 glview-1.5.3/glview/pygletui.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4478 2023-04-25 13:39:44.000000 glview-1.5.3/glview/texture.fs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-04-28 09:49:31.000000 glview-1.5.3/glview/version.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-28 09:52:42.564791 glview-1.5.3/glview.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-28 09:52:42.000000 glview-1.5.3/glview.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-04-28 09:52:42.000000 glview-1.5.3/glview.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-28 09:52:42.000000 glview-1.5.3/glview.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-04-28 09:52:42.000000 glview-1.5.3/glview.egg-info/entry_points.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-04-28 09:52:42.000000 glview-1.5.3/glview.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-04-28 09:52:42.000000 glview-1.5.3/glview.egg-info/top_level.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-28 09:52:42.000000 glview-1.5.3/glview.egg-info/zip-safe
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      163 2023-03-14 15:45:52.000000 glview-1.5.3/requirements.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-04-28 09:52:42.564791 glview-1.5.3/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.5.3/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-06-13 14:00:33.719439 glview-1.5.4/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.5.4/LICENSE
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.5.4/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-06-13 14:00:33.719439 glview-1.5.4/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      380 2023-05-03 12:54:40.000000 glview-1.5.4/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-06-13 14:00:33.719439 glview-1.5.4/glview/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-03-15 12:51:16.000000 glview-1.5.4/glview/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.5.4/glview/argv.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    11756 2023-05-12 14:23:54.000000 glview-1.5.4/glview/glrenderer.py
+-rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     9369 2023-06-13 13:48:47.000000 glview-1.5.4/glview/glview.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     8698 2023-06-13 13:58:46.000000 glview-1.5.4/glview/imageprovider.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      297 2023-05-09 09:52:42.000000 glview-1.5.4/glview/panzoom.vs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    17722 2023-06-13 13:48:47.000000 glview-1.5.4/glview/pygletui.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4546 2023-06-13 13:48:47.000000 glview-1.5.4/glview/texture.fs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-06-13 13:54:28.000000 glview-1.5.4/glview/version.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-06-13 14:00:33.719439 glview-1.5.4/glview.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       39 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/entry_points.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      140 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/top_level.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/zip-safe
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      175 2023-06-13 13:44:12.000000 glview-1.5.4/requirements.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-06-13 14:00:33.719439 glview-1.5.4/setup.cfg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.5.4/setup.py
```

### Comparing `glview-1.5.3/LICENSE` & `glview-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glview-1.5.3/PKG-INFO` & `glview-1.5.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.5.3
+Version: 1.5.4
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # glview
 
 [![Build Status](https://travis-ci.com/toaarnio/glview.svg?branch=master)](https://travis-ci.com/github/toaarnio/glview)
 
-Lightning-fast image viewer with smooth zooming &amp; panning + HDR exposure control.
+Lightning-fast image viewer with synchronized split-screen zooming &amp; panning + HDR exposure control.
 
 **Installing:**
 ```
 pip install glview
 ```
 
 **Usage:**
 ```
 glview --help
 ```
 
 **Building &amp; installing from source:**
 ```
-
-
```

### Comparing `glview-1.5.3/glview/argv.py` & `glview-1.5.4/glview/argv.py`

 * *Files identical despite different names*

### Comparing `glview-1.5.3/glview/glrenderer.py` & `glview-1.5.4/glview/glrenderer.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,17 +44,17 @@
         self.ctx = moderngl.create_context(require=310)
         self.ctx.enable(moderngl.DEPTH_TEST)
         self._vprint("compiling shaders...")
         shader_path = os.path.dirname(os.path.realpath(__file__))
         vshader = open(os.path.join(shader_path, "panzoom.vs"), encoding="utf-8").read()
         fshader = open(os.path.join(shader_path, "texture.fs"), encoding="utf-8").read()
         self.prog = self.ctx.program(vertex_shader=vshader, fragment_shader=fshader)
-        self.prog['scale'].value = 1.0
-        self.prog['orientation'].value = 0
-        self.prog['mousepos'].value = (0.0, 0.0)
+        self.prog['scale'] = 1.0
+        self.prog['orientation'] = 0
+        self.prog['mousepos'] = (0.0, 0.0)
         self.vbo = self.ctx.buffer(struct.pack('8f', -1.0, -1.0, -1.0, 1.0, 1.0, -1.0, 1.0, 1.0))
         self.vao = self.ctx.vertex_array(self.prog, [(self.vbo, "2f", "vert")])
         self.tprev = time.time()
         _ = self.ctx.error  # clear the GL error flag (workaround for a bug that prevents interoperability with Pyglet)
 
     def redraw(self):
         """ Redraw the tiled image view with refreshed pan & zoom, filtering, etc. """
@@ -65,33 +65,36 @@
         for i in range(self.ui.numtiles):
             imgidx = self.ui.img_per_tile[i]
             texture = self._load_texture(imgidx)
             texture.filter = self.filters[self.ui.texture_filter]
             texture.repeat_x = False
             texture.repeat_y = False
             texture.swizzle = 'RGB1'
-            texture.use()
+            texture.use(location=0)
             orientation = self.files.orientations[imgidx]
             texw, texh = texture.width, texture.height
             texw, texh = (texh, texw) if orientation in [90, 270] else (texw, texh)
             _vpx, _vpy, vpw, vph = self.ui.viewports[i]
+            maxval = self.files.metadata[imgidx]['maxval']
             self.ctx.viewport = self.ui.viewports[i]
             self.ctx.clear(*tile_colors[i], viewport=self.ctx.viewport)
-            self.prog['mousepos'].value = tuple(self.ui.mousepos)
-            self.prog['orientation'].value = orientation
-            self.prog['aspect'].value = self._get_aspect_ratio(vpw, vph, texw, texh)
-            self.prog['scale'].value = self.ui.scale
-            self.prog['grayscale'].value = (texture.components == 1)
-            self.prog['gamma'].value = self.ui.gamma
-            self.prog['ev'].value = self.ui.ev
-            self.prog['gamut.compress'].value = (self.ui.gamut_fit != 0)
-            self.prog['gamut.power'].value = self.ui.gamut_pow
-            self.prog['gamut.thr'].value = self.ui.gamut_thr
-            self.prog['gamut.scale'].value = self._gamut(imgidx)
-            self.prog['debug'].value = self.ui.debug_mode
+            self.prog['texture'] = 0
+            self.prog['mousepos'] = tuple(self.ui.mousepos)
+            self.prog['orientation'] = orientation
+            self.prog['aspect'] = self._get_aspect_ratio(vpw, vph, texw, texh)
+            self.prog['scale'] = self.ui.scale
+            self.prog['grayscale'] = (texture.components == 1)
+            self.prog['gamma'] = self.ui.gamma
+            self.prog['maxval'] = maxval if self.ui.normalize else 1.0
+            self.prog['ev'] = self.ui.ev
+            self.prog['gamut.compress'] = (self.ui.gamut_fit != 0)
+            self.prog['gamut.power'] = self.ui.gamut_pow
+            self.prog['gamut.thr'] = self.ui.gamut_thr
+            self.prog['gamut.scale'] = self._gamut(imgidx)
+            self.prog['debug'] = self.ui.debug_mode
             self.vao.render(moderngl.TRIANGLE_STRIP)
         self.ctx.finish()
         elapsed = (time.time() - t0) * 1000
         interval = (time.time() - self.tprev) * 1000
         w, h = self.ui.window.get_size()
         self.tprev = time.time()
         self._vprint(f"rendering {w} x {h} pixels took {elapsed:.1f} ms, frame-to-frame interval was {interval:.1f} ms", log_level=2)
@@ -185,42 +188,42 @@
         #   'u2': integer [0, 65535] internal format (GL_RGB16UI), uint16 input
         #   'u4': integer [0, 2^32-1] internal format (GL_RGB32UI), uint32 input
         #
         h, w = img.shape[:2]
         dtype = f"f{img.itemsize}"  # uint8 => 'f1', float16 => 'f2', float32 => 'f4'
         components = img.shape[2] if img.ndim == 3 else 1  # RGB/RGBA/grayscale
         texture = self.ctx.texture((w, h), components, img.ravel(), dtype=dtype)
+        texture.build_mipmaps()
         return texture
 
     def _create_dummy_texture(self):
         dummy = self.ctx.texture((32, 32), 3, np.random.random((32, 32, 3)).astype(np.float32), dtype='f4')
         return dummy
 
-    def _update_texture(self, texture, img):
-        # TODO: take this into use
-        texture.write(img.ravel())
-        texture.build_mipmaps()
-        return texture
-
     def _load_texture(self, idx):
         img = self.loader.get_image(idx)
-        assert isinstance(img, (np.ndarray, str))
-        if isinstance(img, np.ndarray):  # success
+        assert isinstance(img, (np.ndarray, str)), type(img)
+        if isinstance(img, np.ndarray):
+            maxval = 1.0 if img.dtype == np.uint8 else np.max(img)
             texture = self._create_texture(img)
+            self.files.metadata[idx] = {}
+            self.files.metadata[idx]['maxval'] = maxval
+            self.files.metadata[idx]['gamut_bounds'] = None
             self.files.textures[idx] = texture
-            self.files.metadata[idx] = {'gamut_bounds': None}
             self.loader.release_image(idx)
         else:  # PENDING | INVALID | RELEASED
-            texture = self.files.textures[idx]
-            if texture is None:
+            if self.files.textures[idx] is None:
                 texture = self._create_dummy_texture()
+                maxval = 1.0
+                self.files.metadata[idx] = {}
+                self.files.metadata[idx]['maxval'] = maxval
+                self.files.metadata[idx]['gamut_bounds'] = None
                 self.files.textures[idx] = texture
-                self.files.metadata[idx] = {'gamut_bounds': None}
-        if self.ui.texture_filter != "NEAREST":
-            texture.build_mipmaps()
+            else:  # RELEASED
+                texture = self.files.textures[idx]
         return texture
 
     def _get_aspect_ratio(self, vpw, vph, texw, texh):
         viewport_aspect = vpw / vph
         texture_aspect = texw / texh
         if texture_aspect > viewport_aspect:
             # image wider than window => squeeze y => black top & bottom
```

### Comparing `glview-1.5.3/glview/glview.py` & `glview-1.5.4/glview/glview.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
         print("    s                       split window into 1/2/3/4 tiles")
         print("    1 / 2 / 3 / 4           select active tile for PageUp/PageDown/r")
         print("    w                       write current tile(s) to a PNG")
         print("    h                       reset zoom/pan/exposure to initial state")
         print("    f                       toggle fullscreen <-> windowed")
         print("    t                       toggle nearest <-> linear filtering")
         print("    g                       toggle sRGB gamma correction on/off")
+        print("    n                       toggle exposure normalization on/off")
         print("    e                       slide exposure from -2EV to +2EV & back")
         print("    b                       toggle between HDR/LDR exposure control")
         print("    k                       toggle gamut compression strength")
         print("    i                       print image information (EXIF)")
         print("    d                       drop the currently shown image")
         print("    del                     delete the currently shown image")
         print("    space                   toggle debug rendering on/off")
```

### Comparing `glview-1.5.3/glview/imageprovider.py` & `glview-1.5.4/glview/imageprovider.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import urllib.request          # built-in library
 import tempfile                # built-in library
 import traceback               # built-in library
 import numpy as np             # pip install numpy
 import psutil                  # pip install psutil
 import imsize                  # pip install imsize
 import imgio                   # pip install imgio
+from pqdm.threads import pqdm  # pip install pqdm
 
 
 class ImageProvider:
     """ A multithreaded image file loader. """
 
     def __init__(self, files, verbose=False):
         """ Create a new ImageProvider with the given (hardcoded) FileList instance. """
@@ -24,15 +25,16 @@
         self.running = False
         self.estimate_size()
 
     def start(self):
         """ Start the image loader thread. """
         self._vprint(f"spawning {self.thread_name}...")
         self.running = True
-        self.loader_thread = threading.Thread(target=lambda: self._try(self._image_loader), name=self.thread_name)
+        loader = self._sequential_loader if self.verbose else self._parallel_loader
+        self.loader_thread = threading.Thread(target=lambda: self._try(loader), name=self.thread_name)
         self.loader_thread.daemon = True  # terminate when main process ends
         self.loader_thread.start()
 
     def stop(self):
         """ Stop the image loader thread. """
         self._vprint(f"killing {self.thread_name}...")
         self.running = False
@@ -65,15 +67,42 @@
 
     def release_image(self, index):
         """
         Release the image at the given index to (eventually) free up the memory.
         """
         self.files.images[index] = "RELEASED"
 
-    def _image_loader(self):
+    def _parallel_loader(self):
+        t0 = time.time()
+        ram_total = psutil.virtual_memory().total / 1024**2
+        ram_before = psutil.virtual_memory().available / 1024**2
+        nfiles = self.files.numfiles
+        verbose = self.verbose or nfiles < 200
+        splits = [2, 8, 16] + list(range(32, nfiles, 32))
+        chunks = np.split(np.arange(nfiles), splits)
+        with self.files.mutex:  # drop/delete not allowed while loading
+            for chunk in chunks:
+                batch = [(idx, verbose) for idx in chunk]
+                images = pqdm(batch, self._load_single, 8, "args", bounded=True,
+                              exception_behaviour="immediate", disable=True)
+                for idx, img in zip(chunk, images):
+                    self.files.images[idx] = img
+                time.sleep(0.01)
+        nbytes = np.sum([img.nbytes for img in self.files.images if isinstance(img, np.ndarray)])
+        if nbytes > 1e4:
+            elapsed = time.time() - t0
+            nbytes = nbytes / 1024**2
+            bandwidth = nbytes / elapsed
+            ram_after = psutil.virtual_memory().available / 1024**2
+            consumed = ram_before - ram_after
+            nfiles = self.files.numfiles
+            self._print(f"loaded {nfiles} files, {nbytes:.0f} MB of image data in {elapsed:.1f} seconds ({bandwidth:.1f} MB/sec).")
+            self._print(f"consumed {consumed:.0f} MB of system RAM, {ram_after:.0f}/{ram_total:.0f} MB remaining.")
+
+    def _sequential_loader(self):
         """
         Load all images in sequential order.
         """
         waiting_for_ram = False
         ram_total = psutil.virtual_memory().total / 1024**2
         ram_before = psutil.virtual_memory().available / 1024**2
         while self.running:  # loop until program termination
@@ -128,14 +157,17 @@
             img = np.atleast_3d(img)  # {2D, 3D} => 3D
             img = img[:, :, :3]  # scrap alpha channel, if any
             if img.dtype == np.uint16:
                 # uint16 still doesn't work in ModernGL as of 5.7.4;
                 # scale to [0, 1] and use float32 instead
                 norm = max(maxval, np.max(img))
                 img = img.astype(np.float32) / norm
+            if img.dtype == np.float64:
+                # float64 is not universally supported yet
+                img = img.astype(np.float32)
             return img
         except imgio.ImageIOError as e:
             print(f"\n{e}")
             self._vprint(e)
             return "INVALID"
 
     def _try(self, func):
```

### Comparing `glview-1.5.3/glview/pygletui.py` & `glview-1.5.4/glview/pygletui.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         self.viewports = None
         self.ui_thread = None
         self.event_loop = None
         self.renderer = None
         self.texture_filter = "NEAREST"
         self.img_per_tile = [0, 1, 2, 3]
         self.gamma = False
+        self.normalize = False
         self.ev_range = 2
         self.ev_linear = 0.0
         self.ev = 0.0
         self.gamut_fit = 0  # 0|1|2...
         self.gamut_lim = np.ones(3) * 1.1
         self.gamut_pow = np.ones(3) * 1.5
         self.gamut_thr = np.ones(3) * 0.8
@@ -286,14 +287,17 @@
                     self.need_redraw = True
                 if symbol == keys.B:  # toggle between narrow/wide (LDR/HDR) exposure control
                     self.ev_range = (self.ev_range + 6) % 12
                     self.need_redraw = True
                 if symbol == keys.K: # cycle through gamut compression modes (off/hi/lo)
                     self._switch_gamut_curve()
                     self.need_redraw = True
+                if symbol == keys.N:  # normalize
+                    self.normalize = not self.normalize
+                    self.need_redraw = True
                 if symbol == keys.T:  # texture filtering
                     self.texture_filter = "LINEAR" if self.texture_filter == "NEAREST" else "NEAREST"
                     self.need_redraw = True
                 if symbol == keys.S:  # split
                     self.numtiles = (self.numtiles % 4) + 1
                     self.tileidx = min(self.tileidx, self.numtiles - 1)
                     self.img_per_tile = np.clip(self.img_per_tile, 0, self.files.numfiles - 1)
```

### Comparing `glview-1.5.3/glview/texture.fs` & `glview-1.5.4/glview/texture.fs`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #version 130
 
 uniform int debug;
 uniform bool grayscale;
 uniform bool gamma;
 uniform float ev;
+uniform float maxval;
 uniform int orientation;
 uniform sampler2D texture;
 uniform struct {
   bool compress;
   vec3 power;
   vec3 thr;
   vec3 scale;
 } gamut;
 
-in vec2 tex;
+in vec2 texcoords;
 out vec4 color;
 
 
 const vec3 ones = vec3(1.0);
 const vec3 zeros = vec3(0.0);
 const vec3 eps = vec3(5.0 / 256);
 
@@ -137,14 +138,15 @@
       break;
   }
   return tc;
 }
 
 
 void main() {
-  color = texture2D(texture, rotate(tex, orientation));
+  color = texture2D(texture, rotate(texcoords, orientation));
+  color.rgb = color.rgb / maxval;
   color.rgb = grayscale ? color.rrr : color.rgb;
   color.rgb = gamut.compress ? compress_gamut(color.rgb) : color.rgb;
   color.rgb = color.rgb * exp(ev);  // exp(x) == 2^x
   color.rgb = debug_indicators(color.rgb);
   color.rgb = gamma ? srgb_gamma(color.rgb) : color.rgb;
 }
```

### Comparing `glview-1.5.3/glview.egg-info/PKG-INFO` & `glview-1.5.4/glview.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.5.3
+Version: 1.5.4
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # glview
 
 [![Build Status](https://travis-ci.com/toaarnio/glview.svg?branch=master)](https://travis-ci.com/github/toaarnio/glview)
 
-Lightning-fast image viewer with smooth zooming &amp; panning + HDR exposure control.
+Lightning-fast image viewer with synchronized split-screen zooming &amp; panning + HDR exposure control.
 
 **Installing:**
 ```
 pip install glview
 ```
 
 **Usage:**
 ```
 glview --help
 ```
 
 **Building &amp; installing from source:**
 ```
-
-
```

### Comparing `glview-1.5.3/setup.py` & `glview-1.5.4/setup.py`

 * *Files identical despite different names*

