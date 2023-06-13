# Comparing `tmp/ipycc-0.0.11.tar.gz` & `tmp/ipycc-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipycc-0.0.11.tar", last modified: Tue Feb 28 02:24:18 2023, max compression
+gzip compressed data, was "ipycc-0.0.12.tar", last modified: Tue Jun 13 03:27:05 2023, max compression
```

## Comparing `ipycc-0.0.11.tar` & `ipycc-0.0.12.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-02-28 02:24:18.365486 ipycc-0.0.11/
--rw-r--r--   0 nick       (501) staff       (20)    24480 2022-12-07 01:30:12.000000 ipycc-0.0.11/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     2899 2023-02-28 02:24:18.365532 ipycc-0.0.11/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     2294 2022-12-07 01:30:12.000000 ipycc-0.0.11/README.md
--rw-r--r--   0 nick       (501) staff       (20)      104 2022-12-07 01:30:12.000000 ipycc-0.0.11/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)      780 2023-02-28 02:24:18.365751 ipycc-0.0.11/setup.cfg
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-02-28 02:24:18.363726 ipycc-0.0.11/src/
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-02-28 02:24:18.364618 ipycc-0.0.11/src/ipycc/
--rw-r--r--   0 nick       (501) staff       (20)       54 2022-12-07 01:30:12.000000 ipycc-0.0.11/src/ipycc/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)    17450 2022-12-07 01:30:12.000000 ipycc-0.0.11/src/ipycc/sketch.py
--rw-r--r--   0 nick       (501) staff       (20)     5469 2023-02-28 02:24:06.000000 ipycc-0.0.11/src/ipycc/turtle.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-02-28 02:24:18.365156 ipycc-0.0.11/src/ipycc.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     2899 2023-02-28 02:24:18.000000 ipycc-0.0.11/src/ipycc.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      308 2023-02-28 02:24:18.000000 ipycc-0.0.11/src/ipycc.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-02-28 02:24:18.000000 ipycc-0.0.11/src/ipycc.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       35 2023-02-28 02:24:18.000000 ipycc-0.0.11/src/ipycc.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)        6 2023-02-28 02:24:18.000000 ipycc-0.0.11/src/ipycc.egg-info/top_level.txt
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-02-28 02:24:18.365397 ipycc-0.0.11/test/
--rw-r--r--   0 nick       (501) staff       (20)      125 2022-12-07 01:30:12.000000 ipycc-0.0.11/test/test_sketch.py
--rw-r--r--   0 nick       (501) staff       (20)      114 2022-12-07 01:30:12.000000 ipycc-0.0.11/test/test_turtle.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.540174 ipycc-0.0.12/
+-rw-r--r--   0 nick       (501) staff       (20)     7652 2023-06-13 01:47:07.000000 ipycc-0.0.12/LICENSE
+-rw-r--r--   0 nick       (501) staff       (20)     3169 2023-06-13 03:27:05.540227 ipycc-0.0.12/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     2578 2023-06-13 03:12:18.000000 ipycc-0.0.12/README.md
+-rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 13:18:24.000000 ipycc-0.0.12/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)      766 2023-06-13 03:27:05.540459 ipycc-0.0.12/setup.cfg
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.538042 ipycc-0.0.12/src/
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.538836 ipycc-0.0.12/src/ipycc/
+-rw-r--r--   0 nick       (501) staff       (20)       62 2023-06-13 02:06:39.000000 ipycc-0.0.12/src/ipycc/__init__.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.539790 ipycc-0.0.12/src/ipycc/api/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2023-06-13 01:59:16.000000 ipycc-0.0.12/src/ipycc/api/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)    17524 2023-06-13 02:09:22.000000 ipycc-0.0.12/src/ipycc/api/sketch.py
+-rw-r--r--   0 nick       (501) staff       (20)    24652 2023-06-13 03:10:32.000000 ipycc-0.0.12/src/ipycc/api/turtle.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.539410 ipycc-0.0.12/src/ipycc.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     3169 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      342 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)       35 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)        6 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.540059 ipycc-0.0.12/test/
+-rw-r--r--   0 nick       (501) staff       (20)      125 2023-04-27 13:18:24.000000 ipycc-0.0.12/test/test_sketch.py
+-rw-r--r--   0 nick       (501) staff       (20)      114 2023-04-27 13:18:24.000000 ipycc-0.0.12/test/test_turtle.py
```

### Comparing `ipycc-0.0.11/PKG-INFO` & `ipycc-0.0.12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ipycc
-Version: 0.0.11
+Version: 0.0.12
 Summary: A Python package for creative coding in Jupyter
 Home-page: https://github.com/nickmcintyre/ipycc
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/ipycc/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipycc
 > A Python package for creative coding in Jupyter
 
@@ -21,37 +21,38 @@
 
 ## Turtles
 A light blue square with a smaller square outlined in green at its center. The square is drawn one side at a time.
 ```python
 from ipycc import Turtle
 
 
-t = Turtle()
-t.draw()
-t.bgcolor('midnightblue')
-t.pencolor('ghostwhite')
-t.pendown()
+ted = Turtle()
+ted.draw()
+
+ted.bgcolor("midnightblue")
+ted.pencolor("ghostwhite")
+ted.pendown()
 side = 5
-while side < t.width:
-    t.forward(side)
-    t.left(90)
-    await t.delay(0.1)
+while side < ted.width:
+    ted.fd(side)
+    ted.lt(90)
+    await ted.delay(0.1)
     side += 5
 ```
 
 ## Sketches
 A light blue square with a circle in its center. The circle is drawn with a white center and black edge.
 ```python
 from ipycc import Sketch
 
 
 p5 = Sketch(400, 400)
-p5.background('dodgerblue')
+p5.background("dodgerblue")
 p5.circle(200, 200, 50)
-p5.draw()
+p5.run_sketch()
 ```
 
 A dark blue square with ten circles in its center. The circles are drawn in white and move in synchrony.
 ```python
 import math
 from random import uniform
 from ipycc import Sketch
@@ -69,15 +70,15 @@
         self.r = 5
         self.angle = uniform(0, math.tau)
         self.freq = uniform(5, 10)
         self.da_dt = 0
         self.dt = 0.01
     
     def render(self):
-        p5.fill('ghostwhite')
+        p5.fill("ghostwhite")
         p5.no_stroke()
         p5.circle(self.x, self.y, 2 * self.r)
     
     def update(self):
         self.angle += self.da_dt * self.dt
         dx = math.cos(self.angle)
         dy = math.sin(self.angle)
@@ -88,19 +89,24 @@
         self.da_dt = self.freq
         for bug in bugs:
             self.da_dt += k_n * math.sin(bug.angle - self.angle)
 
 bugs = [Bug() for _ in range(num_bugs)]
 
 def draw():
-    p5.background('#1919706F')
+    p5.background("#1919706F")
     for bug in bugs:
         bug.sync(bugs)
     
     for bug in bugs:
         bug.update()
         bug.render()
 
-p5.draw(draw, 10) # loop for 10 seconds
+# Loop for 10 seconds.
+p5.run_sketch(draw, 10) 
 ```
 
 ipycc provides a simplified interface to the HTML canvas by wrapping [ipycanvas](https://ipycanvas.readthedocs.io/en/latest/index.html) in a beginner-friendly API.
+
+## Acknowledgements
+- Portions of the `Sketch` class are lovingly borrowed from their [p5.js](https://p5js.org) and [proceso](https://proceso.cc) counterparts.
+- Portions of the `Turtle` class are lovingly borrowed from their standard library counterparts.
```

### Comparing `ipycc-0.0.11/README.md` & `ipycc-0.0.12/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,37 +5,38 @@
 
 ## Turtles
 A light blue square with a smaller square outlined in green at its center. The square is drawn one side at a time.
 ```python
 from ipycc import Turtle
 
 
-t = Turtle()
-t.draw()
-t.bgcolor('midnightblue')
-t.pencolor('ghostwhite')
-t.pendown()
+ted = Turtle()
+ted.draw()
+
+ted.bgcolor("midnightblue")
+ted.pencolor("ghostwhite")
+ted.pendown()
 side = 5
-while side < t.width:
-    t.forward(side)
-    t.left(90)
-    await t.delay(0.1)
+while side < ted.width:
+    ted.fd(side)
+    ted.lt(90)
+    await ted.delay(0.1)
     side += 5
 ```
 
 ## Sketches
 A light blue square with a circle in its center. The circle is drawn with a white center and black edge.
 ```python
 from ipycc import Sketch
 
 
 p5 = Sketch(400, 400)
-p5.background('dodgerblue')
+p5.background("dodgerblue")
 p5.circle(200, 200, 50)
-p5.draw()
+p5.run_sketch()
 ```
 
 A dark blue square with ten circles in its center. The circles are drawn in white and move in synchrony.
 ```python
 import math
 from random import uniform
 from ipycc import Sketch
@@ -53,15 +54,15 @@
         self.r = 5
         self.angle = uniform(0, math.tau)
         self.freq = uniform(5, 10)
         self.da_dt = 0
         self.dt = 0.01
     
     def render(self):
-        p5.fill('ghostwhite')
+        p5.fill("ghostwhite")
         p5.no_stroke()
         p5.circle(self.x, self.y, 2 * self.r)
     
     def update(self):
         self.angle += self.da_dt * self.dt
         dx = math.cos(self.angle)
         dy = math.sin(self.angle)
@@ -72,19 +73,24 @@
         self.da_dt = self.freq
         for bug in bugs:
             self.da_dt += k_n * math.sin(bug.angle - self.angle)
 
 bugs = [Bug() for _ in range(num_bugs)]
 
 def draw():
-    p5.background('#1919706F')
+    p5.background("#1919706F")
     for bug in bugs:
         bug.sync(bugs)
     
     for bug in bugs:
         bug.update()
         bug.render()
 
-p5.draw(draw, 10) # loop for 10 seconds
+# Loop for 10 seconds.
+p5.run_sketch(draw, 10) 
 ```
 
 ipycc provides a simplified interface to the HTML canvas by wrapping [ipycanvas](https://ipycanvas.readthedocs.io/en/latest/index.html) in a beginner-friendly API.
+
+## Acknowledgements
+- Portions of the `Sketch` class are lovingly borrowed from their [p5.js](https://p5js.org) and [proceso](https://proceso.cc) counterparts.
+- Portions of the `Turtle` class are lovingly borrowed from their standard library counterparts.
```

### Comparing `ipycc-0.0.11/setup.cfg` & `ipycc-0.0.12/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = ipycc
-version = 0.0.11
+version = 0.0.12
 author = Nick McIntyre
 author_email = nick@mcintyre.io
 description = A Python package for creative coding in Jupyter
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nickmcintyre/ipycc
 project_urls = 
 	Bug Tracker = https://github.com/nickmcintyre/ipycc/issues
 classifiers = 
+	Development Status :: 3 - Alpha
+	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Programming Language :: Python :: 3
-	License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 	Operating System :: OS Independent
-	Development Status :: 2 - Pre-Alpha
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 install_requires =
```

### Comparing `ipycc-0.0.11/src/ipycc/sketch.py` & `ipycc-0.0.12/src/ipycc/api/sketch.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,67 +5,67 @@
 from ipyevents import Event
 from IPython.display import display
 import ipywidgets as widgets
 import numpy as np
 
 
 class Sketch:
-
     # Constants
     DELAY = 0.02
     HALF_PI = math.pi * 0.5
     PI = math.pi
     QUARTER_PI = math.pi * 0.25
     TAU = math.tau
     TWO_PI = math.tau
-    DEGREES = 'degrees'
-    RADIANS = 'radians'
-    NORMAL = 'normal'
-    ITALIC = 'italic'
-    BOLD = 'bold'
-    BOLDITALIC = 'bolditalic'
-    _DEFAULT_STROKE = 'black'
+    DEGREES = "degrees"
+    RADIANS = "radians"
+    NORMAL = "normal"
+    ITALIC = "italic"
+    BOLD = "bold"
+    BOLDITALIC = "bolditalic"
+    _DEFAULT_STROKE = "black"
     _DEFAULT_STROKE_WEIGHT = 1
-    _DEFAULT_FILL = 'white'
-    _DEFAULT_TEXT_FILL = 'black'
+    _DEFAULT_FILL = "white"
+    _DEFAULT_TEXT_FILL = "black"
     _DEFAULT_TEXT_WEIGHT = 0.3
-    _TRANSPARENT = '#00000000'
-    _DEFAULT_FONT = 'Arial'
+    _TRANSPARENT = "#00000000"
+    _DEFAULT_FONT = "Arial"
     _DEFAULT_FONT_SIZE = 12
-    _DEFAULT_FONT_STYLE = 'normal'
-    _DEFAULT_FONT_WEIGHT = 'normal'
+    _DEFAULT_FONT_STYLE = "normal"
+    _DEFAULT_FONT_WEIGHT = "normal"
 
     def __init__(self, width, height):
         self.width = width
         self.height = height
         self.canvas = Canvas(width=width, height=height)
         self.canvas.fill_style = Sketch._DEFAULT_FILL
         self.canvas.stroke_style = Sketch._DEFAULT_STROKE
         self.canvas.line_width = Sketch._DEFAULT_STROKE_WEIGHT
         self._is_looping = False
-        self._fill_set = False
-        self._stroke_set = False
+        self._is_fill_set = False
+        self._is_stroke_set = False
         self._stroke_weight_set = False
         self.frame_count = 0
         self._start_time = 0
         self._vertices = []
         self._font = Sketch._DEFAULT_FONT
         self._font_size = Sketch._DEFAULT_FONT_SIZE
         self._font_style = Sketch._DEFAULT_FONT_STYLE
         self._font_weight = Sketch._DEFAULT_FONT_WEIGHT
-        self.canvas.font = f'{self._font_style} {self._font_weight} {self._font_size}px {self._font}'
-        self._events = Event(
-            source=self.canvas, watched_events=['keydown', 'keyup'])
+        self.canvas.font = (
+            f"{self._font_style} {self._font_weight} {self._font_size}px {self._font}"
+        )
+        self._events = Event(source=self.canvas, watched_events=["keydown", "keyup"])
         self.pmouse_x = 0
         self.pmouse_y = 0
         self.mouse_x = 0
         self.mouse_y = 0
-        self.key = ''
-        self.key_code = ''
-        self.key_is_pressed = False
+        self.key = ""
+        self.key_code = ""
+        self.is_key_pressed = False
         self._keys_pressed = set()
         self._register_base_events()
         self._widgets = []
         self._matrix = np.eye(3)
 
     # ========================================
     #                 Color
@@ -84,31 +84,31 @@
         self.canvas.stroke_rect(0, 0, self.canvas.width, self.canvas.height)
         self.canvas.fill_style = old_fill
         self.canvas.stroke_style = old_stroke
         self.canvas.line_width = old_weight
         self.canvas.restore()
 
     def fill(self, color):
-        if not self._fill_set:
-            self._fill_set = True
+        if not self._is_fill_set:
+            self._is_fill_set = True
         self.canvas.fill_style = color
 
     def no_fill(self):
-        if not self._fill_set:
-            self._fill_set = True
+        if not self._is_fill_set:
+            self._is_fill_set = True
         self.canvas.fill_style = Sketch._TRANSPARENT
 
     def no_stroke(self):
-        if not self._stroke_set:
-            self._stroke_set = True
+        if not self._is_stroke_set:
+            self._is_stroke_set = True
         self.canvas.stroke_style = Sketch._TRANSPARENT
 
     def stroke(self, color):
-        if not self._stroke_set:
-            self._stroke_set = True
+        if not self._is_stroke_set:
+            self._is_stroke_set = True
         self.canvas.stroke_style = color
 
     def clear(self):
         self.canvas.clear()
 
     def remove(self):
         self.canvas.close()
@@ -130,22 +130,22 @@
         cos_phi = math.cos(phi)
         sin_phi = math.sin(phi)
         lam = (4.0 - cos_alpha) / 3
         mu = sin_alpha + (cos_alpha - lam) * cot_alpha
 
         # Return rotated waypoints.
         return {
-            'ax': round(math.cos(start), 7),
-            'ay': round(math.sin(start), 7),
-            'bx': round((lam * cos_phi + mu * sin_phi), 7),
-            'by': round((lam * sin_phi - mu * cos_phi), 7),
-            'cx': round((lam * cos_phi - mu * sin_phi), 7),
-            'cy': round((lam * sin_phi + mu * cos_phi), 7),
-            'dx': round(math.cos(start + size), 7),
-            'dy': round(math.sin(start + size), 7),
+            "ax": round(math.cos(start), 7),
+            "ay": round(math.sin(start), 7),
+            "bx": round((lam * cos_phi + mu * sin_phi), 7),
+            "by": round((lam * sin_phi - mu * cos_phi), 7),
+            "cx": round((lam * cos_phi - mu * sin_phi), 7),
+            "cy": round((lam * sin_phi + mu * cos_phi), 7),
+            "dx": round(math.cos(start + size), 7),
+            "dy": round(math.sin(start + size), 7),
         }
 
     def arc(self, x, y, w, h, start, stop):
         rx = w * 0.5
         ry = h * 0.5
         epsilon = 0.00001  # Smallest visible angle on displays up to 4K.
         arc_to_draw = 0
@@ -158,19 +158,23 @@
             arc_to_draw = min(stop - start, Sketch.HALF_PI)
             curves.append(self._acute_arc_to_bezier(start, arc_to_draw))
             start += arc_to_draw
 
         self.canvas.begin_path()
         for index, curve in enumerate(curves):
             if index == 0:
-                self.canvas.move_to(x + curve['ax'] * rx, y + curve['ay'] * ry)
-            self.canvas.bezier_curve_to(x + curve['bx'] * rx, y + curve['by'] * ry,
-                                        x + curve['cx'] * rx, y +
-                                        curve['cy'] * ry,
-                                        x + curve['dx'] * rx, y + curve['dy'] * ry)
+                self.canvas.move_to(x + curve["ax"] * rx, y + curve["ay"] * ry)
+            self.canvas.bezier_curve_to(
+                x + curve["bx"] * rx,
+                y + curve["by"] * ry,
+                x + curve["cx"] * rx,
+                y + curve["cy"] * ry,
+                x + curve["dx"] * rx,
+                y + curve["dy"] * ry,
+            )
         # if mode == constants['PIE'] or mode == None:
         self.canvas.line_to(x, y)
         self.canvas.close_path()
         self.canvas.fill()
         self.canvas.stroke()
 
     def ellipse(self, x, y, w, h):
@@ -207,20 +211,19 @@
         self.canvas.fill_circle(x, y, r)
         self.canvas.stroke_circle(x, y, r)
 
     def line(self, x1, y1, x2, y2):
         self.canvas.stroke_line(x1, y1, x2, y2)
 
     def point(self, x, y):
-        s = f'{self.canvas.stroke_style}'
-        f = f'{self.canvas.fill_style}'
+        s = f"{self.canvas.stroke_style}"
+        f = f"{self.canvas.fill_style}"
         self.canvas.fill_style = s
         self.canvas.begin_path()
-        self.canvas.arc(x, y, self.canvas.line_width *
-                        0.5, 0, self.TWO_PI, False)
+        self.canvas.arc(x, y, self.canvas.line_width * 0.5, 0, self.TWO_PI, False)
         self.canvas.fill()
         self.canvas.fill_style = f
 
     def quad(self, x1, y1, x2, y2, x3, y3, x4, y4):
         self.begin_shape()
         self.vertex(x1, y1)
         self.vertex(x2, y2)
@@ -260,29 +263,29 @@
         self.canvas.move_to(x1, y1)
         self.canvas.bezier_curve_to(x2, y2, x3, y3, x4, y4)
         self.canvas.stroke()
 
     def bezier_point(self, a, b, c, d, t):
         adjusted_t = 1 - t
         return (
-            pow(adjusted_t, 3) * a +
-            3 * pow(adjusted_t, 2) * t * b +
-            3 * adjusted_t * pow(t, 2) * c +
-            pow(t, 3) * d
+            pow(adjusted_t, 3) * a
+            + 3 * pow(adjusted_t, 2) * t * b
+            + 3 * adjusted_t * pow(t, 2) * c
+            + pow(t, 3) * d
         )
 
     def bezier_tangent(self, a, b, c, d, t):
         adjusted_t = 1 - t
         return (
-            3 * d * pow(t, 2) -
-            3 * c * pow(t, 2) +
-            6 * c * adjusted_t * t -
-            6 * b * adjusted_t * t +
-            3 * b * pow(adjusted_t, 2) -
-            3 * a * pow(adjusted_t, 2)
+            3 * d * pow(t, 2)
+            - 3 * c * pow(t, 2)
+            + 6 * c * adjusted_t * t
+            - 6 * b * adjusted_t * t
+            + 3 * b * pow(adjusted_t, 2)
+            - 3 * a * pow(adjusted_t, 2)
         )
 
     # ========================================
     #                Vertex
     # ========================================
 
     def begin_shape(self):
@@ -296,18 +299,18 @@
     def vertex(self, x, y):
         self._vertices.append((x, y))
 
     # ========================================
     #                Structure
     # ========================================
 
-    def draw(self, *args):
+    def run_sketch(self, *args):
         canvas_layout = widgets.Layout(
-            width=f'{self.width}px',
-            height=f'{self.height}px')
+            width=f"{self.width}px", height=f"{self.height}px"
+        )
         canvas_box = widgets.Box([self.canvas], layout=canvas_layout)
         widget_box = widgets.VBox(self._widgets)
         sketch_box = widgets.HBox([canvas_box, widget_box])
         display(sketch_box)
         if len(args) == 0:
             return
         draw = args[0]
@@ -325,14 +328,15 @@
                     if now - self._start_time > args[1]:
                         self._is_looping = False
                 with hold_canvas():
                     draw()
                     self._vertices.clear()
                 self.reset_matrix()
                 await asyncio.sleep(Sketch.DELAY)
+
         asyncio.create_task(loop())
 
     def stop(self):
         self._is_looping = False
 
     async def delay(self, secs):
         await asyncio.sleep(secs)
@@ -457,25 +461,27 @@
     def _register_base_events(self):
         # FIXME: pmouse
         def get_mouse_position(x, y):
             self.pmouse_x = self.mouse_x
             self.pmouse_y = self.mouse_y
             self.mouse_x = x
             self.mouse_y = y
+
         self.canvas.on_mouse_move(get_mouse_position)
 
         def get_key(event):
-            if event['event'] == 'keydown':
-                self.key = event['key']
-                self.key_code = event['code']
+            if event["event"] == "keydown":
+                self.key = event["key"]
+                self.key_code = event["code"]
                 self._keys_pressed.add(self.key)
-            elif event['event'] == 'keyup':
-                key = event['key']
+            elif event["event"] == "keyup":
+                key = event["key"]
                 self._keys_pressed.remove(key)
-            self.key_is_pressed = len(self._keys_pressed) > 0
+            self.is_key_pressed = len(self._keys_pressed) > 0
+
         self._events.on_dom_event(get_key)
 
     # ========================================
     #                  Image
     # ========================================
 
     def load_image(self, path):
@@ -483,52 +489,57 @@
 
     def image(self, img, x, y, *args):
         if len(args) == 0:
             self.canvas.draw_image(img, x=x, y=y)
         elif len(args) == 1:
             self.canvas.draw_image(img, x=x, y=y, width=args[0])
         elif len(args) == 2:
-            self.canvas.draw_image(
-                img, x=x, y=y, width=args[0], height=args[1])
+            self.canvas.draw_image(img, x=x, y=y, width=args[0], height=args[1])
 
     # ========================================
     #                Typography
     # ========================================
 
     def text(self, text, x, y):
-        if self._fill_set:
+        if self._is_fill_set:
             self.canvas.fill_text(text, x, y)
         else:
             self.canvas.fill_style = Sketch._DEFAULT_TEXT_FILL
             self.canvas.fill_text(text, x, y)
             self.canvas.fill_style = Sketch._DEFAULT_FILL
 
-        if self._stroke_set:
+        if self._is_stroke_set:
             if self._stroke_weight_set:
                 self.canvas.stroke_text(text, x, y)
             else:
                 self.canvas.line_width = Sketch._DEFAULT_TEXT_WEIGHT
                 self.canvas.stroke_text(text, x, y)
                 self.canvas.line_width = Sketch._DEFAULT_STROKE_WEIGHT
 
     def text_font(self, font):
         self._font = font
-        self.canvas.font = f'{self._font_style} {self._font_weight} {self._font_size}px {self._font}'
+        self.canvas.font = (
+            f"{self._font_style} {self._font_weight} {self._font_size}px {self._font}"
+        )
 
     def text_size(self, size):
         self._font_size = size
-        self.canvas.font = f'{self._font_style} {self._font_weight} {self._font_size}px {self._font}'
+        self.canvas.font = (
+            f"{self._font_style} {self._font_weight} {self._font_size}px {self._font}"
+        )
 
     def text_style(self, style):
         if style == Sketch.NORMAL:
             self._font_weight = Sketch.NORMAL
             self._font_style = Sketch.NORMAL
         elif style == Sketch.ITALIC:
             self._font_weight = Sketch.NORMAL
             self._font_style = Sketch.ITALIC
         elif style == Sketch.BOLD:
             self._font_weight = Sketch.BOLD
             self._font_style = Sketch.NORMAL
         elif style == Sketch.BOLDITALIC:
             self._font_weight = Sketch.BOLD
             self._font_style = Sketch.ITALIC
-        self.canvas.font = f'{self._font_style} {self._font_weight} {self._font_size}px {self._font}'
+        self.canvas.font = (
+            f"{self._font_style} {self._font_weight} {self._font_size}px {self._font}"
+        )
```

### Comparing `ipycc-0.0.11/src/ipycc.egg-info/PKG-INFO` & `ipycc-0.0.12/src/ipycc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ipycc
-Version: 0.0.11
+Version: 0.0.12
 Summary: A Python package for creative coding in Jupyter
 Home-page: https://github.com/nickmcintyre/ipycc
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/ipycc/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipycc
 > A Python package for creative coding in Jupyter
 
@@ -21,37 +21,38 @@
 
 ## Turtles
 A light blue square with a smaller square outlined in green at its center. The square is drawn one side at a time.
 ```python
 from ipycc import Turtle
 
 
-t = Turtle()
-t.draw()
-t.bgcolor('midnightblue')
-t.pencolor('ghostwhite')
-t.pendown()
+ted = Turtle()
+ted.draw()
+
+ted.bgcolor("midnightblue")
+ted.pencolor("ghostwhite")
+ted.pendown()
 side = 5
-while side < t.width:
-    t.forward(side)
-    t.left(90)
-    await t.delay(0.1)
+while side < ted.width:
+    ted.fd(side)
+    ted.lt(90)
+    await ted.delay(0.1)
     side += 5
 ```
 
 ## Sketches
 A light blue square with a circle in its center. The circle is drawn with a white center and black edge.
 ```python
 from ipycc import Sketch
 
 
 p5 = Sketch(400, 400)
-p5.background('dodgerblue')
+p5.background("dodgerblue")
 p5.circle(200, 200, 50)
-p5.draw()
+p5.run_sketch()
 ```
 
 A dark blue square with ten circles in its center. The circles are drawn in white and move in synchrony.
 ```python
 import math
 from random import uniform
 from ipycc import Sketch
@@ -69,15 +70,15 @@
         self.r = 5
         self.angle = uniform(0, math.tau)
         self.freq = uniform(5, 10)
         self.da_dt = 0
         self.dt = 0.01
     
     def render(self):
-        p5.fill('ghostwhite')
+        p5.fill("ghostwhite")
         p5.no_stroke()
         p5.circle(self.x, self.y, 2 * self.r)
     
     def update(self):
         self.angle += self.da_dt * self.dt
         dx = math.cos(self.angle)
         dy = math.sin(self.angle)
@@ -88,19 +89,24 @@
         self.da_dt = self.freq
         for bug in bugs:
             self.da_dt += k_n * math.sin(bug.angle - self.angle)
 
 bugs = [Bug() for _ in range(num_bugs)]
 
 def draw():
-    p5.background('#1919706F')
+    p5.background("#1919706F")
     for bug in bugs:
         bug.sync(bugs)
     
     for bug in bugs:
         bug.update()
         bug.render()
 
-p5.draw(draw, 10) # loop for 10 seconds
+# Loop for 10 seconds.
+p5.run_sketch(draw, 10) 
 ```
 
 ipycc provides a simplified interface to the HTML canvas by wrapping [ipycanvas](https://ipycanvas.readthedocs.io/en/latest/index.html) in a beginner-friendly API.
+
+## Acknowledgements
+- Portions of the `Sketch` class are lovingly borrowed from their [p5.js](https://p5js.org) and [proceso](https://proceso.cc) counterparts.
+- Portions of the `Turtle` class are lovingly borrowed from their standard library counterparts.
```

