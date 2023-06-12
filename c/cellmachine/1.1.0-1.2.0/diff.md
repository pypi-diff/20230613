# Comparing `tmp/cellmachine-1.1.0.tar.gz` & `tmp/cellmachine-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmachine-1.1.0.tar", max compression
+gzip compressed data, was "cellmachine-1.2.0.tar", max compression
```

## Comparing `cellmachine-1.1.0.tar` & `cellmachine-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    35149 2023-06-05 12:50:19.381034 cellmachine-1.1.0/LICENSE
--rw-r--r--   0        0        0       60 2023-06-05 12:50:19.381034 cellmachine-1.1.0/README.md
--rw-r--r--   0        0        0      339 2023-06-05 12:50:19.381034 cellmachine-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       84 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/__init__.py
--rw-r--r--   0        0        0      271 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__init__.py
--rw-r--r--   0        0        0      476 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      890 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc
--rw-r--r--   0        0        0     2034 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc
--rw-r--r--   0        0        0      885 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc
--rw-r--r--   0        0        0      747 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc
--rw-r--r--   0        0        0     1229 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc
--rw-r--r--   0        0        0      851 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc
--rw-r--r--   0        0        0      917 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc
--rw-r--r--   0        0        0      561 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/push.cpython-310.pyc
--rw-r--r--   0        0        0      766 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc
--rw-r--r--   0        0        0      719 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc
--rw-r--r--   0        0        0      538 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/ccw.py
--rw-r--r--   0        0        0     2025 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/cell.py
--rw-r--r--   0        0        0      536 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/cw.py
--rw-r--r--   0        0        0      341 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/enemy.py
--rw-r--r--   0        0        0     1266 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/generator.py
--rw-r--r--   0        0        0      294 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/immobile.py
--rw-r--r--   0        0        0      456 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/mover.py
--rw-r--r--   0        0        0      155 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/push.py
--rw-r--r--   0        0        0      354 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/slide.py
--rw-r--r--   0        0        0      277 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/cells/trash.py
--rw-r--r--   0        0        0     3652 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/level.py
--rw-r--r--   0        0        0      417 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/levelstring/__init__.py
--rw-r--r--   0        0        0      528 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2145 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc
--rw-r--r--   0        0        0     2371 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc
--rw-r--r--   0        0        0     2481 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc
--rw-r--r--   0        0        0     2719 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/levelstring/v1.py
--rw-r--r--   0        0        0     3173 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/levelstring/v2.py
--rw-r--r--   0        0        0     3528 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/levelstring/v3.py
--rw-r--r--   0        0        0     6148 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/.DS_Store
--rwxr-xr-x   0        0        0      165 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/0.png
--rwxr-xr-x   0        0        0      127 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/BGDefault.png
--rwxr-xr-x   0        0        0      494 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/ccw.png
--rwxr-xr-x   0        0        0      437 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/cw.png
--rwxr-xr-x   0        0        0      429 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/enemy.png
--rwxr-xr-x   0        0        0      522 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/generator.png
--rwxr-xr-x   0        0        0      171 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/immobile.png
--rwxr-xr-x   0        0        0      467 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/mover.png
--rwxr-xr-x   0        0        0      527 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/push.png
--rwxr-xr-x   0        0        0      481 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/slide.png
--rwxr-xr-x   0        0        0      469 2023-06-05 12:50:19.381034 cellmachine-1.1.0/src/cellmachine/textures/trash.png
--rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 cellmachine-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-12 22:41:48.141825 cellmachine-1.2.0/LICENSE
+-rw-r--r--   0        0        0       60 2023-06-12 22:41:48.141825 cellmachine-1.2.0/README.md
+-rw-r--r--   0        0        0      340 2023-06-12 22:41:48.141825 cellmachine-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__init__.py
+-rw-r--r--   0        0        0      476 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      890 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc
+-rw-r--r--   0        0        0     2034 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc
+-rw-r--r--   0        0        0      885 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc
+-rw-r--r--   0        0        0      747 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc
+-rw-r--r--   0        0        0     1229 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc
+-rw-r--r--   0        0        0      851 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc
+-rw-r--r--   0        0        0      917 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc
+-rw-r--r--   0        0        0      561 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/push.cpython-310.pyc
+-rw-r--r--   0        0        0      766 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc
+-rw-r--r--   0        0        0      719 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc
+-rw-r--r--   0        0        0      538 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/ccw.py
+-rw-r--r--   0        0        0     2025 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/cell.py
+-rw-r--r--   0        0        0      536 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/cw.py
+-rw-r--r--   0        0        0      341 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/enemy.py
+-rw-r--r--   0        0        0     1266 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/generator.py
+-rw-r--r--   0        0        0      294 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/immobile.py
+-rw-r--r--   0        0        0      456 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/mover.py
+-rw-r--r--   0        0        0      155 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/push.py
+-rw-r--r--   0        0        0      354 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/slide.py
+-rw-r--r--   0        0        0      277 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/cells/trash.py
+-rw-r--r--   0        0        0     3652 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/level.py
+-rw-r--r--   0        0        0      417 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/levelstring/__init__.py
+-rw-r--r--   0        0        0      528 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2145 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc
+-rw-r--r--   0        0        0     2371 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc
+-rw-r--r--   0        0        0     2481 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc
+-rw-r--r--   0        0        0     2719 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/levelstring/v1.py
+-rw-r--r--   0        0        0     4905 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/levelstring/v2.py
+-rw-r--r--   0        0        0     6129 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/levelstring/v3.py
+-rw-r--r--   0        0        0     6148 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/.DS_Store
+-rwxr-xr-x   0        0        0      165 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/0.png
+-rwxr-xr-x   0        0        0      127 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/BGDefault.png
+-rwxr-xr-x   0        0        0      494 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/ccw.png
+-rwxr-xr-x   0        0        0      437 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/cw.png
+-rwxr-xr-x   0        0        0      429 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/enemy.png
+-rwxr-xr-x   0        0        0      522 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/generator.png
+-rwxr-xr-x   0        0        0      171 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/immobile.png
+-rwxr-xr-x   0        0        0      467 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/mover.png
+-rwxr-xr-x   0        0        0      527 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/push.png
+-rwxr-xr-x   0        0        0      481 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/slide.png
+-rwxr-xr-x   0        0        0      469 2023-06-12 22:41:48.141825 cellmachine-1.2.0/src/cellmachine/textures/trash.png
+-rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 cellmachine-1.2.0/PKG-INFO
```

### Comparing `cellmachine-1.1.0/LICENSE` & `cellmachine-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/push.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/push.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/ccw.py` & `cellmachine-1.2.0/src/cellmachine/cells/ccw.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/cell.py` & `cellmachine-1.2.0/src/cellmachine/cells/cell.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/cw.py` & `cellmachine-1.2.0/src/cellmachine/cells/cw.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/cells/generator.py` & `cellmachine-1.2.0/src/cellmachine/cells/generator.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/level.py` & `cellmachine-1.2.0/src/cellmachine/level.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc` & `cellmachine-1.2.0/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/levelstring/v1.py` & `cellmachine-1.2.0/src/cellmachine/levelstring/v1.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/levelstring/v2.py` & `cellmachine-1.2.0/src/cellmachine/levelstring/v2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 from ..level import Level
 from ..cells import *
 
 base74_key = {char: index for index, char in enumerate("0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!$%&+-.=?^{}")}
+base74_encodes = list(base74_key.keys())
+
 def base74_decode(string):
     result = 0
     for char in string:
         result *= 74
         result += base74_key[char]
     return result
 
+def base74_encode(num):
+    if num < 74: return base74_encodes[num]
+    
+    result = ""
+    while num:
+        result = base74_encodes[num % 74] + result
+        num = num // 74
+    return result
+
 # data){distance}
 # data(distance)
 #    ^ cell
 
 def decode_data(encoded_data):
     decoded_data = []
 
@@ -102,8 +113,55 @@
         size=level_data['size'],
         cells=level_data['cells'],
         placeables=level_data['placeables'],
         name=level_data['name'],
         tutorial_text=level_data['tutorial_text'],
     )
 
-    return lvl
+    return lvl
+
+def export_level(level):
+    celltype = {
+        "generator": 0,
+        "cw": 1,
+        "ccw": 2,
+        "mover": 3,
+        "slide": 4,
+        "push": 5,
+        "immobile": 6,
+        "enemy": 7,
+        "trash": 8,
+        "BGDefault": 9,
+        "0": 10,
+    }
+
+    cell_data = [72] * (level.size[0] * level.size[1])
+    
+    for placeable in level.placeables:
+        cell_data[placeable[0] + ((level.size[1] - placeable[1] - 1) * level.size[0])] = 73
+        
+    for cell in level.cells.values():
+        cell_data[cell.position[0] + \
+            ((level.size[1] - cell.position[1] - 1) * level.size[0])] += \
+            (2 * celltype[cell.celltype]) + (18 * cell.rotation) - 72
+    
+    run_length = 1
+    
+    cells = ""
+    
+    for data_index, cell_value in enumerate(cell_data):
+        if data_index + 1 < len(cell_data) and cell_value == cell_data[data_index + 1]:
+            run_length += 1
+        else:
+            if run_length > 3:
+                encoded = base74_encode(run_length - 1)
+                if len(encoded) > 1:
+                    cells += base74_encodes[cell_value] + "(" + encoded + ")"
+                else:
+                    cells += base74_encodes[cell_value] + ")" + encoded
+            else:
+                cells += base74_encodes[cell_value] * run_length
+            run_length = 1
+
+    level_string = f'V2;{base74_encode(level.size[0])};{base74_encode(level.size[1])};{cells};{level.tutorial_text};{level.name}'
+
+    return level_string
```

### Comparing `cellmachine-1.1.0/src/cellmachine/textures/.DS_Store` & `cellmachine-1.2.0/src/cellmachine/textures/.DS_Store`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/textures/generator.png` & `cellmachine-1.2.0/src/cellmachine/textures/generator.png`

 * *Files identical despite different names*

### Comparing `cellmachine-1.1.0/src/cellmachine/textures/push.png` & `cellmachine-1.2.0/src/cellmachine/textures/push.png`

 * *Files identical despite different names*

