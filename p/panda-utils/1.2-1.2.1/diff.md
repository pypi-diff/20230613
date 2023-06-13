# Comparing `tmp/panda_utils-1.2.tar.gz` & `tmp/panda_utils-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.2.tar", last modified: Mon Jun 12 20:27:03 2023, max compression
+gzip compressed data, was "panda_utils-1.2.1.tar", last modified: Tue Jun 13 13:13:23 2023, max compression
```

## Comparing `panda_utils-1.2.tar` & `panda_utils-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1080 2022-08-12 11:48:21.000000 panda_utils-1.2/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    15364 2023-06-12 20:27:03.047219 panda_utils-1.2/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    14636 2023-06-12 20:11:36.000000 panda_utils-1.2/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.2/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.043886 panda_utils-1.2/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.2/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.2/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.2/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3596 2023-06-12 17:37:49.000000 panda_utils-1.2/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      218 2023-06-11 09:05:00.000000 panda_utils-1.2/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.2/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     8899 2023-06-12 20:24:34.000000 panda_utils-1.2/panda_utils/assetpipeline/models.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.2/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.2/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.2/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.2/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5178 2023-06-12 15:26:37.000000 panda_utils-1.2/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.2/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.2/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.2/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.2/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3587 2023-06-10 09:05:07.000000 panda_utils-1.2/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3184 2023-06-10 09:05:07.000000 panda_utils-1.2/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.2/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2482 2023-06-12 19:50:06.000000 panda_utils-1.2/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.043886 panda_utils-1.2/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    15364 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      878 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1021 2023-06-12 18:10:06.000000 panda_utils-1.2/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.2/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-06-12 20:27:03.047219 panda_utils-1.2/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1080 2022-08-12 11:48:21.000000 panda_utils-1.2.1/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    19196 2023-06-13 13:13:23.414693 panda_utils-1.2.1/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    18466 2023-06-13 13:12:03.000000 panda_utils-1.2.1/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.2.1/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.411359 panda_utils-1.2.1/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.2.1/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.2.1/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.2.1/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3712 2023-06-13 13:13:16.000000 panda_utils-1.2.1/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.2.1/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.2.1/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     9059 2023-06-13 12:08:12.000000 panda_utils-1.2.1/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.2.1/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.2.1/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.2.1/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.2.1/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.2.1/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5178 2023-06-12 15:26:37.000000 panda_utils-1.2.1/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.2.1/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.414693 panda_utils-1.2.1/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.2.1/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.2.1/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.2.1/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.2.1/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.2.1/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.2.1/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2482 2023-06-12 19:50:06.000000 panda_utils-1.2.1/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-13 13:13:23.411359 panda_utils-1.2.1/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    19196 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      916 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-06-13 13:13:23.000000 panda_utils-1.2.1/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-06-13 10:37:23.000000 panda_utils-1.2.1/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.2.1/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-06-13 13:13:23.414693 panda_utils-1.2.1/setup.cfg
```

### Comparing `panda_utils-1.2/LICENSE` & `panda_utils-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2/PKG-INFO` & `panda_utils-1.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,8 @@
-Metadata-Version: 2.1
-Name: panda_utils
-Version: 1.2
-Summary: PandaUtils includes multiple tools for basic Panda3D automation
-Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
-Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
-Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: imagery
-Provides-Extra: autopath
-Provides-Extra: runnable
-Provides-Extra: pipeline
-Provides-Extra: everything
-License-File: LICENSE
-
-# Panda3D Utils v1.2
+# Panda3D Utils v1.2.1
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -202,32 +183,44 @@
 in order, first the node will be rescaled, and then it will be rotated.
 When a `collide[]` action is encountered, it will be called once with the given
 arguments. If a different `[]` action is encountered, it will not run.
 This method is used for easy interaction with Makefiles (if the input folder 
 is set as the makefile dependency, changing this file will cause the task
 building a given asset to be rerun).
 
+The pipeline will normally hide 
+
 The list of all currently existing steps is below.
 
 ### Preblend
 
 This step will convert OBJ or FBX models into BLEND. It requires installing
 Blender on the machine. Note that due to specifics of various modeling software,
 the model may end up scaled incorrectly at this phase. You can use the `transform`
 step to fix this. All OBJ and FBX files will be joined into the same file.
 This step takes no arguments.
 
+**Changelog**
+* 1.2 - now joins all models into the same blend file, instead of making
+  separate blend files per model
+* 1.1 - initial implementation
+
+**Examples**
 `preblend`
 
 ### BlendRename
 
 This step will rename the BLEND models into their proper name. It is required
 if the input files are in BLEND format, but not required if the Blend files are
 generated through Preblend. This step takes no arguments.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 `blendrename`
 
 ### Blend2Bam
 
 This step will use Blend2Bam to convert the BLEND moodels into an intermediate
 BAM model. It should happen after `preblend` or `blendrename`. This model
 is usually not suitable for ingame use and requires further processing through
@@ -235,37 +228,55 @@
 with Blender 3.5.1, but is likely to work on other versions as well.
 
 This is currently using the GLTF pipeline (available since Blender 2.8),
 the builtin physics system (not bullet), and disables sRGB textures due to 
 specifics of Toontown use. It takes no arguments, but these things 
 might become configurable later through optional arguments.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `blend2bam`
 
 ### Bam2Egg
 
 This step will decompile every BAM model into EGG models, which are used
 for processing through other methods. It takes no arguments.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `bam2egg`
 
 ### Optimize
 
 This step will do the following transformations to every EGG model it finds:
 
 * Removes the default cube `Cube.N` and camera `Camera` groups from the file
   if they're found inside.
 * Creates a group with the same name as the model name, containing everything
   inside of the model. This is useful if the Panda3D code is using `find()`
   while loading this model.
+* Renames all textures to follow a consistent naming pattern. For example,
+  if textures `file1.png`, `Randomfile.jpg` and `otherFile.png` are provided,
+  they will be renamed into `input_folder.png`, `input_folder-1.jpg` and
+  `input_folder-2.png` (the order is not guaranteed, but it will be consistent
+  if this step is launched multiple times).
 
 This function takes one required parameter `profile`. However, the profile
 is currently ignored. In the future, there will be multiple profiles that can
 (for example) run egg-optchar, etc.
 
+**Changelog**
+* 1.2 - no longer changes the texture path prefix (now done by egg2bam)
+* 1.1 - initial implementation
+
+**Examples**
 * `optimize:stiffchar`
 * `optimize:actorchar`
 * `optimize:prop`
 
 ### Transform
 
 This step will apply the given transforms to every egg file it encounters.
@@ -275,15 +286,22 @@
 
 This will first increase the model scale 10 times, then rotate it 180 degrees
 around the Z axis (functionally setting its H angle to 180), and then translate
 it 1 unit upwards and 0.25 units backwards.
 
 It is recommended to use the `[]` syntax to load the arguments for this step.
 
+**Changelog**
+* 1.2 - now is controlled by arguments (`[]` partially restores old behavior)
+* 1.1 - initial implementation
+
+**Examples**
 * `transform[]`
+* `transform:10`
+* `transform::0,0,180`
 
 ### Collide
 
 This step will automatically add collision geometry to a model. This step
 will not automatically make decimated collision geometry, that has to be done
 separately. It can either add preset geometry types like Sphere, or Polyset
 geometry for complex shapes. Note that adding Polyset collisions is
@@ -298,51 +316,124 @@
   the given name. If not supplied (default), the collision will be added
   to a node with the name = input_folder's name (this group is automatically
   created by the optimize step).
 
 This step can appear multiple times in the pipeline if one wants to add
 multiple collision solids to different parts of the model. 
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `collide`
 * `collide:keep,descend:tube`
 * `collide:descend:polyset:optimized_geom`
 * `collide[]`
 
-### 3D-Palettize
+### Downscale
+
+This step is used to resize one texture or all PNG textures in the folder
+to a given size. Installing `Pillow` is required for this step (provided
+by the `imagery` extra).
+
+This step accepts up to four arguments.
+* The first argument `size` is required. The desired texture size, which has
+  to be a power-of-two. All affected textures will be resized to `size*size`.
+* The second parameter `bbox` is optional. If it is not present, the textures
+  will be resized as-is. If it is present, all textures will be first cropped
+  to their bounding box before resizing, with `bbox%` padding around the
+  bounding box. For example, setting `bbox=10` will use 10/12th of each
+  dimension for the source image, and 1/12th of each dimension on each side
+  for the padding.
+* The third parameter `flags` is optional. It includes zero or more words
+  separated by commas, defaults to no flags:
+  * `truecenter`: By default, textures with big width and small height will be
+    pinned to the bottom of the image. Setting this flag will instead center
+    those textures in the image. This flag does not affect the textures with
+    small width and big height, which will always be centered.
+* The fourth argument `name` is optional, and defaults to
+  an empty string. If name is empty, all textures will be resized, if name is 
+  not empty, only the texture matching the given name will be resized. 
+  This accepts Unix-style patterns (i.e. `background-*.png`).
+
+**Changelog**
+* 1.2.1 - initial implementation
+
+**Examples**
+* `downscale:256`
+* `downscale:256:10`
+* `downscale:256::truecenter:background-*.png`
+* `downscale[]`
+
+### Texture Cards
+
+This step is used to create an EGG model out of a set of png/jpg files.
+It is usually used to combine multiple related 2D images/icons together.
+It is recommended to do `downscale` before this step, and `palettize` after
+this step, but not required.
+
+By default, all parts of the model will occupy the 1x1 unit square when loaded
+in Panda3D. This is usually desired for assets such as icons, but not desired
+for assets with variable sizes or non-uniform aspect ratio, such as GUI 
+elements. In those cases, texture-cards can accept an argument for the size
+of each model, which should be an integer (usually power-of-two). For example,
+if this argument is set to `512`, 256x256 textures will have the Panda3D
+size 0.5x0.5, and 128x1024 textures will have the size 0.25x2.
+
+**Changelog**
+* 1.2.1 - initial implementation
+
+**Examples**
+* `texture_cards`
+* `texture_cards:512`
+
+### Palettize
 
-This step is used to join multiple texture files on a 3D model into one palette.
+This step is used to join multiple texture files on a model into one palette.
 It will palettize every EGG model in the folder.
 
 This step takes one parameter, the desired texture size. It must be a power
 of two. The default value is 1024, which means each produced palette will be
 1024x1024.
 
-*New in version 1.2.*
-
-* `3d_palettize`
-* `3d_palettize:2048`
+**Changelog**
+* 1.2.1 - renamed from `3d_palettize` to `palettize`
+* 1.2 - initial implementation
+
+**Examples**
+* `palettize`
+* `palettize:2048`
 
 ### Egg2Bam
 
 This step is used to assemble the EGG model into the BAM model suitable
 for ingame use. It also replaces the texture paths in the model, and 
 copies the model and every needed texture into the `built` folder.
 It takes no arguments.
 
+**Changelog**
+* 1.2 - now also patches the texture paths (before, this was done by optimize)
+* 1.1 - initial implementation
+
+**Examples**
 * `egg2bam`
 
 ### Script
 
 This step can be used to run scripts that are not packaged with this project.
 The script will run in the directory including (transformed versions of) all
 assets in the input directory. It will receive the name of the model as its only
 argument. This step includes one parameter with the path to the script. Note that
 due to the specifics of implementation, it has to be one file, but the type
 of the script is not limited (shell, python, etc.) as long as it's an executable.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `script:scripts/magic.sh`
 
 For example, if your directory structure looks like this:
 
 ```
 inputs
   asset_name
@@ -357,9 +448,8 @@
 ```shell
 python -m panda_utils.assetpipeline inputs/asset_name asset char script:scripts/magic.sh
 ```
 
 ## Future plans
 * Reverse palettizing based on the image coordinates
 * Automatic decimation in the Asset Pipeline for collision purposes
-* Addition of palettize functionality into the Asset Pipeline
 * Addition of toon head functionality into the Asset Pipeline
```

### Comparing `panda_utils-1.2/README.md` & `panda_utils-1.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,27 @@
-# Panda3D Utils v1.2
+Metadata-Version: 2.1
+Name: panda_utils
+Version: 1.2.1
+Summary: PandaUtils includes multiple tools for basic Panda3D automation
+Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
+Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
+Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: imagery
+Provides-Extra: autopath
+Provides-Extra: runnable
+Provides-Extra: pipeline
+Provides-Extra: everything
+License-File: LICENSE
+
+# Panda3D Utils v1.2.1
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -183,32 +202,44 @@
 in order, first the node will be rescaled, and then it will be rotated.
 When a `collide[]` action is encountered, it will be called once with the given
 arguments. If a different `[]` action is encountered, it will not run.
 This method is used for easy interaction with Makefiles (if the input folder 
 is set as the makefile dependency, changing this file will cause the task
 building a given asset to be rerun).
 
+The pipeline will normally hide 
+
 The list of all currently existing steps is below.
 
 ### Preblend
 
 This step will convert OBJ or FBX models into BLEND. It requires installing
 Blender on the machine. Note that due to specifics of various modeling software,
 the model may end up scaled incorrectly at this phase. You can use the `transform`
 step to fix this. All OBJ and FBX files will be joined into the same file.
 This step takes no arguments.
 
+**Changelog**
+* 1.2 - now joins all models into the same blend file, instead of making
+  separate blend files per model
+* 1.1 - initial implementation
+
+**Examples**
 `preblend`
 
 ### BlendRename
 
 This step will rename the BLEND models into their proper name. It is required
 if the input files are in BLEND format, but not required if the Blend files are
 generated through Preblend. This step takes no arguments.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 `blendrename`
 
 ### Blend2Bam
 
 This step will use Blend2Bam to convert the BLEND moodels into an intermediate
 BAM model. It should happen after `preblend` or `blendrename`. This model
 is usually not suitable for ingame use and requires further processing through
@@ -216,37 +247,55 @@
 with Blender 3.5.1, but is likely to work on other versions as well.
 
 This is currently using the GLTF pipeline (available since Blender 2.8),
 the builtin physics system (not bullet), and disables sRGB textures due to 
 specifics of Toontown use. It takes no arguments, but these things 
 might become configurable later through optional arguments.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `blend2bam`
 
 ### Bam2Egg
 
 This step will decompile every BAM model into EGG models, which are used
 for processing through other methods. It takes no arguments.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `bam2egg`
 
 ### Optimize
 
 This step will do the following transformations to every EGG model it finds:
 
 * Removes the default cube `Cube.N` and camera `Camera` groups from the file
   if they're found inside.
 * Creates a group with the same name as the model name, containing everything
   inside of the model. This is useful if the Panda3D code is using `find()`
   while loading this model.
+* Renames all textures to follow a consistent naming pattern. For example,
+  if textures `file1.png`, `Randomfile.jpg` and `otherFile.png` are provided,
+  they will be renamed into `input_folder.png`, `input_folder-1.jpg` and
+  `input_folder-2.png` (the order is not guaranteed, but it will be consistent
+  if this step is launched multiple times).
 
 This function takes one required parameter `profile`. However, the profile
 is currently ignored. In the future, there will be multiple profiles that can
 (for example) run egg-optchar, etc.
 
+**Changelog**
+* 1.2 - no longer changes the texture path prefix (now done by egg2bam)
+* 1.1 - initial implementation
+
+**Examples**
 * `optimize:stiffchar`
 * `optimize:actorchar`
 * `optimize:prop`
 
 ### Transform
 
 This step will apply the given transforms to every egg file it encounters.
@@ -256,15 +305,22 @@
 
 This will first increase the model scale 10 times, then rotate it 180 degrees
 around the Z axis (functionally setting its H angle to 180), and then translate
 it 1 unit upwards and 0.25 units backwards.
 
 It is recommended to use the `[]` syntax to load the arguments for this step.
 
+**Changelog**
+* 1.2 - now is controlled by arguments (`[]` partially restores old behavior)
+* 1.1 - initial implementation
+
+**Examples**
 * `transform[]`
+* `transform:10`
+* `transform::0,0,180`
 
 ### Collide
 
 This step will automatically add collision geometry to a model. This step
 will not automatically make decimated collision geometry, that has to be done
 separately. It can either add preset geometry types like Sphere, or Polyset
 geometry for complex shapes. Note that adding Polyset collisions is
@@ -279,51 +335,124 @@
   the given name. If not supplied (default), the collision will be added
   to a node with the name = input_folder's name (this group is automatically
   created by the optimize step).
 
 This step can appear multiple times in the pipeline if one wants to add
 multiple collision solids to different parts of the model. 
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `collide`
 * `collide:keep,descend:tube`
 * `collide:descend:polyset:optimized_geom`
 * `collide[]`
 
-### 3D-Palettize
+### Downscale
+
+This step is used to resize one texture or all PNG textures in the folder
+to a given size. Installing `Pillow` is required for this step (provided
+by the `imagery` extra).
+
+This step accepts up to four arguments.
+* The first argument `size` is required. The desired texture size, which has
+  to be a power-of-two. All affected textures will be resized to `size*size`.
+* The second parameter `bbox` is optional. If it is not present, the textures
+  will be resized as-is. If it is present, all textures will be first cropped
+  to their bounding box before resizing, with `bbox%` padding around the
+  bounding box. For example, setting `bbox=10` will use 10/12th of each
+  dimension for the source image, and 1/12th of each dimension on each side
+  for the padding.
+* The third parameter `flags` is optional. It includes zero or more words
+  separated by commas, defaults to no flags:
+  * `truecenter`: By default, textures with big width and small height will be
+    pinned to the bottom of the image. Setting this flag will instead center
+    those textures in the image. This flag does not affect the textures with
+    small width and big height, which will always be centered.
+* The fourth argument `name` is optional, and defaults to
+  an empty string. If name is empty, all textures will be resized, if name is 
+  not empty, only the texture matching the given name will be resized. 
+  This accepts Unix-style patterns (i.e. `background-*.png`).
+
+**Changelog**
+* 1.2.1 - initial implementation
+
+**Examples**
+* `downscale:256`
+* `downscale:256:10`
+* `downscale:256::truecenter:background-*.png`
+* `downscale[]`
+
+### Texture Cards
+
+This step is used to create an EGG model out of a set of png/jpg files.
+It is usually used to combine multiple related 2D images/icons together.
+It is recommended to do `downscale` before this step, and `palettize` after
+this step, but not required.
+
+By default, all parts of the model will occupy the 1x1 unit square when loaded
+in Panda3D. This is usually desired for assets such as icons, but not desired
+for assets with variable sizes or non-uniform aspect ratio, such as GUI 
+elements. In those cases, texture-cards can accept an argument for the size
+of each model, which should be an integer (usually power-of-two). For example,
+if this argument is set to `512`, 256x256 textures will have the Panda3D
+size 0.5x0.5, and 128x1024 textures will have the size 0.25x2.
+
+**Changelog**
+* 1.2.1 - initial implementation
+
+**Examples**
+* `texture_cards`
+* `texture_cards:512`
+
+### Palettize
 
-This step is used to join multiple texture files on a 3D model into one palette.
+This step is used to join multiple texture files on a model into one palette.
 It will palettize every EGG model in the folder.
 
 This step takes one parameter, the desired texture size. It must be a power
 of two. The default value is 1024, which means each produced palette will be
 1024x1024.
 
-*New in version 1.2.*
-
-* `3d_palettize`
-* `3d_palettize:2048`
+**Changelog**
+* 1.2.1 - renamed from `3d_palettize` to `palettize`
+* 1.2 - initial implementation
+
+**Examples**
+* `palettize`
+* `palettize:2048`
 
 ### Egg2Bam
 
 This step is used to assemble the EGG model into the BAM model suitable
 for ingame use. It also replaces the texture paths in the model, and 
 copies the model and every needed texture into the `built` folder.
 It takes no arguments.
 
+**Changelog**
+* 1.2 - now also patches the texture paths (before, this was done by optimize)
+* 1.1 - initial implementation
+
+**Examples**
 * `egg2bam`
 
 ### Script
 
 This step can be used to run scripts that are not packaged with this project.
 The script will run in the directory including (transformed versions of) all
 assets in the input directory. It will receive the name of the model as its only
 argument. This step includes one parameter with the path to the script. Note that
 due to the specifics of implementation, it has to be one file, but the type
 of the script is not limited (shell, python, etc.) as long as it's an executable.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `script:scripts/magic.sh`
 
 For example, if your directory structure looks like this:
 
 ```
 inputs
   asset_name
@@ -338,9 +467,8 @@
 ```shell
 python -m panda_utils.assetpipeline inputs/asset_name asset char script:scripts/magic.sh
 ```
 
 ## Future plans
 * Reverse palettizing based on the image coordinates
 * Automatic decimation in the Asset Pipeline for collision purposes
-* Addition of palettize functionality into the Asset Pipeline
 * Addition of toon head functionality into the Asset Pipeline
```

### Comparing `panda_utils-1.2/panda_utils/__main__.py` & `panda_utils-1.2.1/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.2.1/panda_utils/assetpipeline/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,22 +50,23 @@
         elif isinstance(args, list):
             for kwargs in args:
                 action(self, **kwargs)
         else:
             logger.warning("%s: Invalid configured arguments: %s (expected list or dict)", self.name, type(args))
 
 
-def main():
-    console = logging.StreamHandler()
-    console.setLevel(logging.INFO)
-    formatter = logging.Formatter("%(name)-12s: %(levelname)-8s %(message)s")
-    console.setFormatter(formatter)
-    global_logger = logging.getLogger("")
-    global_logger.setLevel(logging.INFO)
-    global_logger.addHandler(console)
+def main(enable_logging=False):
+    if False and enable_logging:
+        console = logging.StreamHandler()
+        console.setLevel(logging.INFO)
+        formatter = logging.Formatter("%(name)-12s: %(levelname)-8s %(message)s")
+        console.setFormatter(formatter)
+        global_logger = logging.getLogger("")
+        global_logger.setLevel(logging.INFO)
+        global_logger.addHandler(console)
 
     _, input_folder, output_phase, output_folder, *pipeline = sys.argv
     ctx = AssetContext(input_folder, output_phase, output_folder)
 
     intermediate_folder = "intermediate/" + ctx.intermediate_path.replace("/", "__")
     os.makedirs("intermediate", exist_ok=True)
     if os.path.exists(intermediate_folder):
@@ -102,8 +103,8 @@
             if use_config:
                 ctx.run_action_through_config(action, method_name)
             else:
                 action(ctx, *args)
 
 
 if __name__ == "__main__":
-    main()
+    main(os.getenv("PIPELINE_LOGGING") != "")
```

### Comparing `panda_utils-1.2/panda_utils/assetpipeline/models.py` & `panda_utils-1.2.1/panda_utils/assetpipeline/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import shutil
 import subprocess
 from pathlib import Path
 
 from panda_utils import util
 from panda_utils.eggtree import eggparse, operations
 from panda_utils.tools.convert import bam2egg, egg2bam
+from panda_utils.tools.palettize import remove_palette_indices
 from panda_utils.util import get_data_file_path
 
 preblend_regex = re.compile(r".*\.(fbx|obj)")
-image_regex = re.compile(r".*\.(jpg|png|rgb)")
 logger = logging.getLogger("panda_utils.pipeline.models")
 
 
 def build_asset_mapper(assets, name):
     output = {}
     for counter, item in enumerate(assets):
         extension = item.split(".")[-1]
@@ -171,19 +171,21 @@
                 new_node = eggparse.EggLeaf("Collide", group_name, f"{method} {flags}")
                 groups[0].children.children.insert(0, new_node)
 
             with open(file, "w") as f:
                 f.write(str(eggtree))
 
 
-def action_3d_palettize(ctx, palette_size="1024"):
+def action_palettize(ctx, palette_size="1024", flags=""):
     palette_size = int(palette_size)
     if palette_size & (palette_size - 1):
         raise ValueError("The palette size must be a power of two!")
 
+    flag_list = flags.split(",")
+
     logger.info("%s: Creating a TXA file...", ctx.name)
     txa_text = (
         f":palette {palette_size} {palette_size}\n"
         ":imagetype png\n"
         ":powertwo 1\n"
         f":group {ctx.model_name} dir .\n"
         f"*.png : force-rgba dual linear clamp_u clamp_v margin 5\n"
@@ -204,14 +206,18 @@
         *all_eggs,
         "-inplace",
         "-tn",
         f"{ctx.model_name}_palette_%p_%i",
         timeout=60,
     )
 
+    if "ordered" in flag_list:
+        for file in all_eggs:
+            remove_palette_indices(file)
+
 
 def action_egg2bam(ctx):
     files = []
     for file in ctx.files:
         if file.endswith(".egg"):
             logger.info("%s: Copying %s into the dist directory", ctx.name, file)
             files.append(file)
```

### Comparing `panda_utils-1.2/panda_utils/blender/import_model.py` & `panda_utils-1.2.1/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2/panda_utils/eggtree/eggparse.py` & `panda_utils-1.2.1/panda_utils/eggtree/eggparse.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2/panda_utils/eggtree/operations.py` & `panda_utils-1.2.1/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2/panda_utils/tools/animconvert.py` & `panda_utils-1.2.1/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2/panda_utils/tools/convert.py` & `panda_utils-1.2.1/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2/panda_utils/tools/downscale.py` & `panda_utils-1.2.1/panda_utils/tools/downscale.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import fnmatch
 import logging
 import shutil
 import pathlib
 import os
 
 try:
     from PIL import Image
@@ -17,70 +18,77 @@
     ctx: Context,
     path: str,
     scale: int,
     force: bool = False,
     bbox: int = -1,
     truecenter: bool = True,
     ignore_current_scale: bool = False,
+    pattern: str = None,
+    do_backup: bool = True,
 ) -> None:
     if Image is None:
-        logger.error("Install PIL to use downscaler: pip install -r requirements.txt")
+        logger.error("Install PIL to use downscaler: pip install panda_utils[imagery]")
         return
 
     original_path = f"{ctx.working_path}/{path}"
+
     backup_path = f"{ctx.working_path}/backup/{path}-{scale}"
-    backup_obj = pathlib.Path(backup_path)
-    backup_obj.mkdir(exist_ok=True, parents=True)
+    if do_backup:
+        backup_obj = pathlib.Path(backup_path)
+        backup_obj.mkdir(exist_ok=True, parents=True)
 
     files = os.listdir(original_path)
+    files = [file for file in files if file.endswith(".png")]
+    if pattern:
+        files = [file for file in files if fnmatch.fnmatch(file, pattern)]
     for x in files:
-        if ".png" in x:
-            img = Image.open(f"{original_path}/{x}")
-            if not ignore_current_scale and img.width == scale and img.height == scale:
-                logger.info(f"Skipping {x} as it is already resized")
-                continue
+        img = Image.open(f"{original_path}/{x}")
+        if not ignore_current_scale and img.width == scale and img.height == scale:
+            logger.info(f"Skipping {x} as it is already resized")
+            continue
 
+        if do_backup:
             if not os.path.exists(f"{backup_path}/{x}"):
                 shutil.copy(f"{original_path}/{x}", f"{backup_path}/{x}")
             else:
                 name, ext = x.rsplit(".", 1)
                 index = 1
                 while os.path.exists(f"{backup_path}/{name}-{index}.{ext}"):
                     index += 1
                 shutil.copy(f"{original_path}/{x}", f"{backup_path}/{name}-{index}.{ext}")
 
-            if bbox >= 0:
-                left, top, right, bottom = img.getbbox()
-                bbox_w, bbox_h = (right - left) * bbox // 100, (bottom - top) * bbox // 100
-                needed_width = right - left + bbox_w
-                needed_height = bottom - top + bbox_h
-                needed_size = max(needed_width, needed_height) * 2
-                canvas = Image.new("RGBA", (needed_size, needed_size), (0, 0, 0, 0))
-                canvas.paste(img.crop((left, top, right, bottom)), (bbox_w, bbox_h))
-                img = canvas.crop((0, 0, right - left + 2 * bbox_w, bottom - top + 2 * bbox_h))
-
-            if img.width != img.height:
-                if not force and bbox == -1:
-                    logger.warning(f"Skipping {x} due to invalid size: width {img.width}, height {img.height}")
-                    continue
-
-                # if we are asked to force downscale, try to add space, and center the image horizontally
-                # but push it to the bottom vertically
-                logger.info("Force mode active, trying to add space...")
-                if img.width > img.height and not truecenter:
-                    img2 = Image.new("RGBA", (img.width, img.width))
-                    img2.paste(img, (0, img.width - img.height, img.width, img.width))
+        if bbox >= 0:
+            left, top, right, bottom = img.getbbox()
+            bbox_w, bbox_h = (right - left) * bbox // 100, (bottom - top) * bbox // 100
+            needed_width = right - left + bbox_w
+            needed_height = bottom - top + bbox_h
+            needed_size = max(needed_width, needed_height) * 2
+            canvas = Image.new("RGBA", (needed_size, needed_size), (0, 0, 0, 0))
+            canvas.paste(img.crop((left, top, right, bottom)), (bbox_w, bbox_h))
+            img = canvas.crop((0, 0, right - left + 2 * bbox_w, bottom - top + 2 * bbox_h))
+
+        if img.width != img.height:
+            if not force and bbox == -1:
+                logger.warning(f"Skipping {x} due to invalid size: width {img.width}, height {img.height}")
+                continue
+
+            # if we are asked to force downscale, try to add space, and center the image horizontally
+            # but push it to the bottom vertically
+            logger.info("Force mode active, trying to add space...")
+            if img.width > img.height and not truecenter:
+                img2 = Image.new("RGBA", (img.width, img.width))
+                img2.paste(img, (0, img.width - img.height, img.width, img.width))
+            else:
+                # pixel-perfect operations moment
+                height_delta = (img.height + img.width) % 2
+                fh, fw = max(img.height, img.width), min(img.height, img.width)
+                even_fheight = fh + height_delta
+                img2 = Image.new("RGBA", (even_fheight, even_fheight))
+                x_coord = (even_fheight - fw) // 2
+                if fh == img.height:
+                    img2.paste(img, (x_coord, height_delta, even_fheight - x_coord, even_fheight))
                 else:
-                    # pixel-perfect operations moment
-                    height_delta = (img.height + img.width) % 2
-                    fh, fw = max(img.height, img.width), min(img.height, img.width)
-                    even_fheight = fh + height_delta
-                    img2 = Image.new("RGBA", (even_fheight, even_fheight))
-                    x_coord = (even_fheight - fw) // 2
-                    if fh == img.height:
-                        img2.paste(img, (x_coord, height_delta, even_fheight - x_coord, even_fheight))
-                    else:
-                        img2.paste(img, (height_delta, x_coord, even_fheight, even_fheight - x_coord))
-                img = img2
+                    img2.paste(img, (height_delta, x_coord, even_fheight, even_fheight - x_coord))
+            img = img2
 
-            logger.info(f"Rescaling {x}")
-            img.resize((scale, scale)).save(f"{original_path}/{x}")
+        logger.info(f"Rescaling {x}")
+        img.resize((scale, scale)).save(f"{original_path}/{x}")
```

### Comparing `panda_utils-1.2/panda_utils/tools/palettize.py` & `panda_utils-1.2.1/panda_utils/tools/palettize.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,36 @@
 
 from panda_utils import util
 from panda_utils.eggtree import eggparse
 
 logger = logging.getLogger("panda_utils.palettize")
 
 
+def remove_palette_indices(egg_path):
+    with open(egg_path) as f:
+        data = f.readlines()
+
+    eggtree = eggparse.egg_tokenize(data)
+    all_groups = eggtree.findall("Group")
+    for group in all_groups:
+        if "-" not in group.node_name:
+            continue
+
+        name_split = group.node_name.split("-", 1)
+        try:
+            int(name_split[0])
+        except ValueError:
+            continue
+        else:
+            group.node_name = name_split[1]
+
+    with open(egg_path, "w") as f:
+        f.write(str(eggtree))
+
+
 def palettize(
     ctx: util.Context, output: str, phase: str, subdir: str, poly: int = None, margin: int = 0, ordered: bool = False
 ) -> None:
     map_path, model_path = f"{phase}/maps", f"{phase}/models/{subdir}"
     pathlib.Path(map_path).mkdir(exist_ok=True, parents=True)
     pathlib.Path(model_path).mkdir(exist_ok=True, parents=True)
 
@@ -60,33 +82,15 @@
         timeout=60,
     )
     logger.info("Transforming eggs...")
     util.run_panda(ctx, "egg-trans", egg_path, "-pc", map_path, "-o", egg_path)
 
     if ordered:
         logger.info("Removing ordering indices from the egg...")
-        with open(egg_path) as f:
-            data = f.readlines()
-
-        eggtree = eggparse.egg_tokenize(data)
-        all_groups = eggtree.findall("Group")
-        for group in all_groups:
-            if "-" not in group.node_name:
-                continue
-
-            name_split = group.node_name.split("-", 1)
-            try:
-                int(name_split[0])
-            except ValueError:
-                continue
-            else:
-                group.node_name = name_split[1]
-
-        with open(egg_path, "w") as f:
-            f.write(str(eggtree))
+        remove_palette_indices(egg_path)
 
     logger.info("Converting to BAM...")
     util.run_panda(ctx, "egg2bam", egg_path, "-o", egg_path.replace(".egg", ".bam"), timeout=10)
     logger.info("Cleaning up...")
     shutil.rmtree(f"{model_path}/{phase}", ignore_errors=True)  # happens due to a bug
     # os.unlink(egg_path)
     os.unlink("textures.txa")
```

### Comparing `panda_utils-1.2/panda_utils/tools/toontown.py` & `panda_utils-1.2.1/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2/panda_utils/util.py` & `panda_utils-1.2.1/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.2/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.2.1/panda_utils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.2
+Version: 1.2.1
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: imagery
 Provides-Extra: autopath
 Provides-Extra: runnable
 Provides-Extra: pipeline
 Provides-Extra: everything
 License-File: LICENSE
 
-# Panda3D Utils v1.2
+# Panda3D Utils v1.2.1
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -202,32 +202,44 @@
 in order, first the node will be rescaled, and then it will be rotated.
 When a `collide[]` action is encountered, it will be called once with the given
 arguments. If a different `[]` action is encountered, it will not run.
 This method is used for easy interaction with Makefiles (if the input folder 
 is set as the makefile dependency, changing this file will cause the task
 building a given asset to be rerun).
 
+The pipeline will normally hide 
+
 The list of all currently existing steps is below.
 
 ### Preblend
 
 This step will convert OBJ or FBX models into BLEND. It requires installing
 Blender on the machine. Note that due to specifics of various modeling software,
 the model may end up scaled incorrectly at this phase. You can use the `transform`
 step to fix this. All OBJ and FBX files will be joined into the same file.
 This step takes no arguments.
 
+**Changelog**
+* 1.2 - now joins all models into the same blend file, instead of making
+  separate blend files per model
+* 1.1 - initial implementation
+
+**Examples**
 `preblend`
 
 ### BlendRename
 
 This step will rename the BLEND models into their proper name. It is required
 if the input files are in BLEND format, but not required if the Blend files are
 generated through Preblend. This step takes no arguments.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 `blendrename`
 
 ### Blend2Bam
 
 This step will use Blend2Bam to convert the BLEND moodels into an intermediate
 BAM model. It should happen after `preblend` or `blendrename`. This model
 is usually not suitable for ingame use and requires further processing through
@@ -235,37 +247,55 @@
 with Blender 3.5.1, but is likely to work on other versions as well.
 
 This is currently using the GLTF pipeline (available since Blender 2.8),
 the builtin physics system (not bullet), and disables sRGB textures due to 
 specifics of Toontown use. It takes no arguments, but these things 
 might become configurable later through optional arguments.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `blend2bam`
 
 ### Bam2Egg
 
 This step will decompile every BAM model into EGG models, which are used
 for processing through other methods. It takes no arguments.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `bam2egg`
 
 ### Optimize
 
 This step will do the following transformations to every EGG model it finds:
 
 * Removes the default cube `Cube.N` and camera `Camera` groups from the file
   if they're found inside.
 * Creates a group with the same name as the model name, containing everything
   inside of the model. This is useful if the Panda3D code is using `find()`
   while loading this model.
+* Renames all textures to follow a consistent naming pattern. For example,
+  if textures `file1.png`, `Randomfile.jpg` and `otherFile.png` are provided,
+  they will be renamed into `input_folder.png`, `input_folder-1.jpg` and
+  `input_folder-2.png` (the order is not guaranteed, but it will be consistent
+  if this step is launched multiple times).
 
 This function takes one required parameter `profile`. However, the profile
 is currently ignored. In the future, there will be multiple profiles that can
 (for example) run egg-optchar, etc.
 
+**Changelog**
+* 1.2 - no longer changes the texture path prefix (now done by egg2bam)
+* 1.1 - initial implementation
+
+**Examples**
 * `optimize:stiffchar`
 * `optimize:actorchar`
 * `optimize:prop`
 
 ### Transform
 
 This step will apply the given transforms to every egg file it encounters.
@@ -275,15 +305,22 @@
 
 This will first increase the model scale 10 times, then rotate it 180 degrees
 around the Z axis (functionally setting its H angle to 180), and then translate
 it 1 unit upwards and 0.25 units backwards.
 
 It is recommended to use the `[]` syntax to load the arguments for this step.
 
+**Changelog**
+* 1.2 - now is controlled by arguments (`[]` partially restores old behavior)
+* 1.1 - initial implementation
+
+**Examples**
 * `transform[]`
+* `transform:10`
+* `transform::0,0,180`
 
 ### Collide
 
 This step will automatically add collision geometry to a model. This step
 will not automatically make decimated collision geometry, that has to be done
 separately. It can either add preset geometry types like Sphere, or Polyset
 geometry for complex shapes. Note that adding Polyset collisions is
@@ -298,51 +335,124 @@
   the given name. If not supplied (default), the collision will be added
   to a node with the name = input_folder's name (this group is automatically
   created by the optimize step).
 
 This step can appear multiple times in the pipeline if one wants to add
 multiple collision solids to different parts of the model. 
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `collide`
 * `collide:keep,descend:tube`
 * `collide:descend:polyset:optimized_geom`
 * `collide[]`
 
-### 3D-Palettize
+### Downscale
+
+This step is used to resize one texture or all PNG textures in the folder
+to a given size. Installing `Pillow` is required for this step (provided
+by the `imagery` extra).
+
+This step accepts up to four arguments.
+* The first argument `size` is required. The desired texture size, which has
+  to be a power-of-two. All affected textures will be resized to `size*size`.
+* The second parameter `bbox` is optional. If it is not present, the textures
+  will be resized as-is. If it is present, all textures will be first cropped
+  to their bounding box before resizing, with `bbox%` padding around the
+  bounding box. For example, setting `bbox=10` will use 10/12th of each
+  dimension for the source image, and 1/12th of each dimension on each side
+  for the padding.
+* The third parameter `flags` is optional. It includes zero or more words
+  separated by commas, defaults to no flags:
+  * `truecenter`: By default, textures with big width and small height will be
+    pinned to the bottom of the image. Setting this flag will instead center
+    those textures in the image. This flag does not affect the textures with
+    small width and big height, which will always be centered.
+* The fourth argument `name` is optional, and defaults to
+  an empty string. If name is empty, all textures will be resized, if name is 
+  not empty, only the texture matching the given name will be resized. 
+  This accepts Unix-style patterns (i.e. `background-*.png`).
+
+**Changelog**
+* 1.2.1 - initial implementation
+
+**Examples**
+* `downscale:256`
+* `downscale:256:10`
+* `downscale:256::truecenter:background-*.png`
+* `downscale[]`
+
+### Texture Cards
+
+This step is used to create an EGG model out of a set of png/jpg files.
+It is usually used to combine multiple related 2D images/icons together.
+It is recommended to do `downscale` before this step, and `palettize` after
+this step, but not required.
+
+By default, all parts of the model will occupy the 1x1 unit square when loaded
+in Panda3D. This is usually desired for assets such as icons, but not desired
+for assets with variable sizes or non-uniform aspect ratio, such as GUI 
+elements. In those cases, texture-cards can accept an argument for the size
+of each model, which should be an integer (usually power-of-two). For example,
+if this argument is set to `512`, 256x256 textures will have the Panda3D
+size 0.5x0.5, and 128x1024 textures will have the size 0.25x2.
+
+**Changelog**
+* 1.2.1 - initial implementation
+
+**Examples**
+* `texture_cards`
+* `texture_cards:512`
+
+### Palettize
 
-This step is used to join multiple texture files on a 3D model into one palette.
+This step is used to join multiple texture files on a model into one palette.
 It will palettize every EGG model in the folder.
 
 This step takes one parameter, the desired texture size. It must be a power
 of two. The default value is 1024, which means each produced palette will be
 1024x1024.
 
-*New in version 1.2.*
-
-* `3d_palettize`
-* `3d_palettize:2048`
+**Changelog**
+* 1.2.1 - renamed from `3d_palettize` to `palettize`
+* 1.2 - initial implementation
+
+**Examples**
+* `palettize`
+* `palettize:2048`
 
 ### Egg2Bam
 
 This step is used to assemble the EGG model into the BAM model suitable
 for ingame use. It also replaces the texture paths in the model, and 
 copies the model and every needed texture into the `built` folder.
 It takes no arguments.
 
+**Changelog**
+* 1.2 - now also patches the texture paths (before, this was done by optimize)
+* 1.1 - initial implementation
+
+**Examples**
 * `egg2bam`
 
 ### Script
 
 This step can be used to run scripts that are not packaged with this project.
 The script will run in the directory including (transformed versions of) all
 assets in the input directory. It will receive the name of the model as its only
 argument. This step includes one parameter with the path to the script. Note that
 due to the specifics of implementation, it has to be one file, but the type
 of the script is not limited (shell, python, etc.) as long as it's an executable.
 
+**Changelog**
+* 1.1 - initial implementation
+
+**Examples**
 * `script:scripts/magic.sh`
 
 For example, if your directory structure looks like this:
 
 ```
 inputs
   asset_name
@@ -357,9 +467,8 @@
 ```shell
 python -m panda_utils.assetpipeline inputs/asset_name asset char script:scripts/magic.sh
 ```
 
 ## Future plans
 * Reverse palettizing based on the image coordinates
 * Automatic decimation in the Asset Pipeline for collision purposes
-* Addition of palettize functionality into the Asset Pipeline
 * Addition of toon head functionality into the Asset Pipeline
```

### Comparing `panda_utils-1.2/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.2.1/panda_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 panda_utils.egg-info/requires.txt
 panda_utils.egg-info/top_level.txt
 panda_utils/assetpipeline/__init__.py
 panda_utils/assetpipeline/__main__.py
 panda_utils/assetpipeline/imports.py
 panda_utils/assetpipeline/misc.py
 panda_utils/assetpipeline/models.py
+panda_utils/assetpipeline/textures.py
 panda_utils/blender/__init__.py
 panda_utils/blender/import_model.py
 panda_utils/blender/patch_paths.py
 panda_utils/eggtree/__init__.py
 panda_utils/eggtree/eggparse.py
 panda_utils/eggtree/operations.py
 panda_utils/tools/__init__.py
```

### Comparing `panda_utils-1.2/pyproject.toml` & `panda_utils-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.2"
+version = "1.2.1"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

