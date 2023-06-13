# Comparing `tmp/ipycc-0.0.12.tar.gz` & `tmp/ipycc-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipycc-0.0.12.tar", last modified: Tue Jun 13 03:27:05 2023, max compression
+gzip compressed data, was "ipycc-0.0.13.tar", last modified: Tue Jun 13 04:15:52 2023, max compression
```

## Comparing `ipycc-0.0.12.tar` & `ipycc-0.0.13.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.540174 ipycc-0.0.12/
--rw-r--r--   0 nick       (501) staff       (20)     7652 2023-06-13 01:47:07.000000 ipycc-0.0.12/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     3169 2023-06-13 03:27:05.540227 ipycc-0.0.12/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     2578 2023-06-13 03:12:18.000000 ipycc-0.0.12/README.md
--rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 13:18:24.000000 ipycc-0.0.12/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)      766 2023-06-13 03:27:05.540459 ipycc-0.0.12/setup.cfg
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.538042 ipycc-0.0.12/src/
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.538836 ipycc-0.0.12/src/ipycc/
--rw-r--r--   0 nick       (501) staff       (20)       62 2023-06-13 02:06:39.000000 ipycc-0.0.12/src/ipycc/__init__.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.539790 ipycc-0.0.12/src/ipycc/api/
--rw-r--r--   0 nick       (501) staff       (20)        0 2023-06-13 01:59:16.000000 ipycc-0.0.12/src/ipycc/api/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)    17524 2023-06-13 02:09:22.000000 ipycc-0.0.12/src/ipycc/api/sketch.py
--rw-r--r--   0 nick       (501) staff       (20)    24652 2023-06-13 03:10:32.000000 ipycc-0.0.12/src/ipycc/api/turtle.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.539410 ipycc-0.0.12/src/ipycc.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     3169 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      342 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       35 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)        6 2023-06-13 03:27:05.000000 ipycc-0.0.12/src/ipycc.egg-info/top_level.txt
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 03:27:05.540059 ipycc-0.0.12/test/
--rw-r--r--   0 nick       (501) staff       (20)      125 2023-04-27 13:18:24.000000 ipycc-0.0.12/test/test_sketch.py
--rw-r--r--   0 nick       (501) staff       (20)      114 2023-04-27 13:18:24.000000 ipycc-0.0.12/test/test_turtle.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 04:15:52.307166 ipycc-0.0.13/
+-rw-r--r--   0 nick       (501) staff       (20)     7652 2023-06-13 01:47:07.000000 ipycc-0.0.13/LICENSE
+-rw-r--r--   0 nick       (501) staff       (20)     3124 2023-06-13 04:15:52.307230 ipycc-0.0.13/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     2533 2023-06-13 04:15:21.000000 ipycc-0.0.13/README.md
+-rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 13:18:24.000000 ipycc-0.0.13/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)      766 2023-06-13 04:15:52.307468 ipycc-0.0.13/setup.cfg
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 04:15:52.304988 ipycc-0.0.13/src/
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 04:15:52.305787 ipycc-0.0.13/src/ipycc/
+-rw-r--r--   0 nick       (501) staff       (20)       62 2023-06-13 02:06:39.000000 ipycc-0.0.13/src/ipycc/__init__.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 04:15:52.306801 ipycc-0.0.13/src/ipycc/api/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2023-06-13 01:59:16.000000 ipycc-0.0.13/src/ipycc/api/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)    17524 2023-06-13 02:09:22.000000 ipycc-0.0.13/src/ipycc/api/sketch.py
+-rw-r--r--   0 nick       (501) staff       (20)    25121 2023-06-13 03:58:51.000000 ipycc-0.0.13/src/ipycc/api/turtle.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 04:15:52.306391 ipycc-0.0.13/src/ipycc.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     3124 2023-06-13 04:15:52.000000 ipycc-0.0.13/src/ipycc.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      342 2023-06-13 04:15:52.000000 ipycc-0.0.13/src/ipycc.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-06-13 04:15:52.000000 ipycc-0.0.13/src/ipycc.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)       35 2023-06-13 04:15:52.000000 ipycc-0.0.13/src/ipycc.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)        6 2023-06-13 04:15:52.000000 ipycc-0.0.13/src/ipycc.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-06-13 04:15:52.307052 ipycc-0.0.13/test/
+-rw-r--r--   0 nick       (501) staff       (20)      125 2023-04-27 13:18:24.000000 ipycc-0.0.13/test/test_sketch.py
+-rw-r--r--   0 nick       (501) staff       (20)      114 2023-04-27 13:18:24.000000 ipycc-0.0.13/test/test_turtle.py
```

### Comparing `ipycc-0.0.12/LICENSE` & `ipycc-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `ipycc-0.0.12/PKG-INFO` & `ipycc-0.0.13/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipycc
-Version: 0.0.12
+Version: 0.0.13
 Summary: A Python package for creative coding in Jupyter
 Home-page: https://github.com/nickmcintyre/ipycc
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/ipycc/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -16,46 +16,44 @@
 
 # ipycc
 > A Python package for creative coding in Jupyter
 
 This package makes it easy to explore creative coding in Python using Jupyter notebooks. Its design is heavily inspired by [p5.js](https://github.com/processing/p5.js) and [Turtle graphics](https://docs.python.org/3/library/turtle.html) from the Python standard library.
 
 ## Turtles
-A light blue square with a smaller square outlined in green at its center. The square is drawn one side at a time.
+A dark blue square with a sprial pattern drawn in white. The spiral is drawn one side at a time.
 ```python
 from ipycc import Turtle
 
 
 ted = Turtle()
 ted.draw()
-
 ted.bgcolor("midnightblue")
 ted.pencolor("ghostwhite")
-ted.pendown()
-side = 5
-while side < ted.width:
-    ted.fd(side)
-    ted.lt(90)
+for side in range(40):
+    length = side * 5
+    ted.fd(length)
+    await ted.delay(0.1)
+    ted.lt(123)
     await ted.delay(0.1)
-    side += 5
 ```
 
 ## Sketches
 A light blue square with a circle in its center. The circle is drawn with a white center and black edge.
 ```python
 from ipycc import Sketch
 
 
 p5 = Sketch(400, 400)
 p5.background("dodgerblue")
 p5.circle(200, 200, 50)
 p5.run_sketch()
 ```
 
-A dark blue square with ten circles in its center. The circles are drawn in white and move in synchrony.
+Ten white circles moving like fireflies on a dark blue background.
 ```python
 import math
 from random import uniform
 from ipycc import Sketch
 
 
 p5 = Sketch(400, 400)
```

### Comparing `ipycc-0.0.12/README.md` & `ipycc-0.0.13/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 # ipycc
 > A Python package for creative coding in Jupyter
 
 This package makes it easy to explore creative coding in Python using Jupyter notebooks. Its design is heavily inspired by [p5.js](https://github.com/processing/p5.js) and [Turtle graphics](https://docs.python.org/3/library/turtle.html) from the Python standard library.
 
 ## Turtles
-A light blue square with a smaller square outlined in green at its center. The square is drawn one side at a time.
+A dark blue square with a sprial pattern drawn in white. The spiral is drawn one side at a time.
 ```python
 from ipycc import Turtle
 
 
 ted = Turtle()
 ted.draw()
-
 ted.bgcolor("midnightblue")
 ted.pencolor("ghostwhite")
-ted.pendown()
-side = 5
-while side < ted.width:
-    ted.fd(side)
-    ted.lt(90)
+for side in range(40):
+    length = side * 5
+    ted.fd(length)
+    await ted.delay(0.1)
+    ted.lt(123)
     await ted.delay(0.1)
-    side += 5
 ```
 
 ## Sketches
 A light blue square with a circle in its center. The circle is drawn with a white center and black edge.
 ```python
 from ipycc import Sketch
 
 
 p5 = Sketch(400, 400)
 p5.background("dodgerblue")
 p5.circle(200, 200, 50)
 p5.run_sketch()
 ```
 
-A dark blue square with ten circles in its center. The circles are drawn in white and move in synchrony.
+Ten white circles moving like fireflies on a dark blue background.
 ```python
 import math
 from random import uniform
 from ipycc import Sketch
 
 
 p5 = Sketch(400, 400)
```

### Comparing `ipycc-0.0.12/setup.cfg` & `ipycc-0.0.13/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ipycc
-version = 0.0.12
+version = 0.0.13
 author = Nick McIntyre
 author_email = nick@mcintyre.io
 description = A Python package for creative coding in Jupyter
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nickmcintyre/ipycc
 project_urls =
```

### Comparing `ipycc-0.0.12/src/ipycc/api/sketch.py` & `ipycc-0.0.13/src/ipycc/api/sketch.py`

 * *Files identical despite different names*

### Comparing `ipycc-0.0.12/src/ipycc/api/turtle.py` & `ipycc-0.0.13/src/ipycc/api/turtle.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,41 @@
             self.width = args[0]
             self.height = args[0]
         elif len(args) >= 2:
             self.width = args[0]
             self.height = args[1]
         self._bg = Sketch(self.width, self.height)
         self._bgcolor = "white"
-        self._p5 = Sketch(self.width, self.height)
+        self._pen = Sketch(self.width, self.height)
         self.reset()
         self.end_poly()
 
     def _render(self):
         with hold_canvas():
             self._bg.background(self._bgcolor)
             # TODO: implement push() and pop()
             self._bg.scale(1, -1)
             self._bg.translate(0, -self.height)
-            self._bg.image(self._p5.canvas, 0, 0)
+            self._bg.image(self._pen.canvas, 0, 0)
+            self._bg.translate(self._x, self._y)
+            self._bg.rotate(self._angle)
+            self._bg.stroke(self._pencolor)
+            self._bg.stroke_weight(2)
+            self._bg.fill(self._fillcolor)
+            self._bg.triangle(0, -4, 0, 4, 8, 0)
             self._bg.reset_matrix()
 
     def draw(self):
         """Display the turtle's drawing canvas."""
         self._render()
         self._bg.run_sketch()
 
     def remove(self):
         """Remove the turtle's drawing canvas."""
-        self._p5.remove()
+        self._pen.remove()
 
     # ========================================
     #              Turtle Motion
     # ========================================
 
     def forward(self, distance):
         """Move the turtle forward by the specified distance.
@@ -64,19 +70,19 @@
         >>> turtle.forward(-75)
         >>> turtle.position()
         (-50.00,0.00)
         """
         x = self._x + distance * math.cos(self._angle)
         y = self._y + distance * math.sin(self._angle)
         if self._is_drawing:
-            self._p5.line(self._x, self._y, x, y)
+            self._pen.line(self._x, self._y, x, y)
         self._x = x
         self._y = y
         if self._is_drawing_poly:
-            self._p5.vertex(x, y)
+            self._pen.vertex(x, y)
         self._render()
 
     def fd(self, distance):
         """Move the turtle forward by the specified distance.
 
         Aliases: forward | fd
 
@@ -174,14 +180,15 @@
         >>> turtle.heading()
         22.0
         >>> turtle.right(45)
         >>> turtle.heading()
         337.0
         """
         self._angle -= math.radians(angle)
+        self._render()
 
     def rt(self, angle):
         """Turn turtle right by angle units.
 
         Aliases: right | rt
 
         Argument:
@@ -195,14 +202,15 @@
         >>> turtle.heading()
         22.0
         >>> turtle.right(45)
         >>> turtle.heading()
         337.0
         """
         self._angle -= math.radians(angle)
+        self._render()
 
     def left(self, angle):
         """Turn turtle left by angle units.
 
         Aliases: left | lt
 
         Argument:
@@ -216,14 +224,15 @@
         >>> turtle.heading()
         22.0
         >>> turtle.left(45)
         >>> turtle.heading()
         67.0
         """
         self._angle += math.radians(angle)
+        self._render()
 
     def lt(self, angle):
         """Turn turtle left by angle units.
 
         Aliases: left | lt
 
         Argument:
@@ -237,14 +246,15 @@
         >>> turtle.heading()
         22.0
         >>> turtle.left(45)
         >>> turtle.heading()
         67.0
         """
         self._angle += math.radians(angle)
+        self._render()
 
     def goto(self, x, y):
         """Move turtle to an absolute position.
 
         Aliases: setpos | setposition | goto:
 
         Arguments:
@@ -263,17 +273,17 @@
         >>> turtle.setpos(60,30)
         >>> turtle.pos()
         (60.00,30.00)
         """
         next_x = self.width * 0.5 + x
         next_y = self.height * 0.5 + y
         if self._is_drawing:
-            self._p5.line(self._x, self._y, next_x, next_y)
+            self._pen.line(self._x, self._y, next_x, next_y)
         if self._is_drawing_poly:
-            self._p5.vertex(next_x, next_y)
+            self._pen.vertex(next_x, next_y)
         self._x = next_x
         self._y = next_y
         self._render()
 
     def setpos(self, x, y):
         """Move turtle to an absolute position.
 
@@ -336,17 +346,17 @@
         (0.00, 240.00)
         >>> turtle.setx(10)
         >>> turtle.position()
         (10.00, 240.00)
         """
         next_x = self.width * 0.5 + x
         if self._is_drawing:
-            self._p5.line(self._x, self._y, next_x, self._y)
+            self._pen.line(self._x, self._y, next_x, self._y)
         if self._is_drawing_poly:
-            self._p5.vertex(next_x, self._y)
+            self._pen.vertex(next_x, self._y)
         self._x = next_x
         self._render()
 
     def sety(self, y):
         """Set the turtle's second coordinate to y
 
         Argument:
@@ -360,17 +370,17 @@
         (0.00, 40.00)
         >>> turtle.sety(-10)
         >>> turtle.position()
         (0.00, -10.00)
         """
         next_y = 0.5 * self.height + y
         if self._is_drawing:
-            self._p5.line(self._x, self._y, self._x, next_y)
+            self._pen.line(self._x, self._y, self._x, next_y)
         if self._is_drawing_poly:
-            self._p5.vertex(self._x, next_y)
+            self._pen.vertex(self._x, next_y)
         self._y = next_y
         self._render()
 
     def setheading(self, angle):
         """Set the orientation of the turtle to to_angle.
 
         Aliases:  setheading | seth
@@ -390,14 +400,15 @@
 
         Example (for a Turtle instance named turtle):
         >>> turtle.setheading(90)
         >>> turtle.heading()
         90
         """
         self._angle = math.radians(angle)
+        self._render()
 
     def seth(self, angle):
         """Set the orientation of the turtle to to_angle.
 
         Aliases:  setheading | seth
 
         Argument:
@@ -415,14 +426,15 @@
 
         Example (for a Turtle instance named turtle):
         >>> turtle.setheading(90)
         >>> turtle.heading()
         90
         """
         self._angle = math.radians(angle)
+        self._render()
 
     def home(self):
         """Move turtle to the origin - coordinates (0,0).
 
         No arguments.
 
         Move turtle to the origin - coordinates (0,0) and set its
@@ -631,15 +643,15 @@
         >>> turtle.pensize()
         1
         >>> turtle.pensize(10)   # from here on lines of width 10 are drawn
         """
         if width is None:
             return self._pensize
         self._pensize = width
-        self._p5.stroke_weight(self._pensize)
+        self._pen.stroke_weight(self._pensize)
 
     def isdown(self):
         """Return True if pen is down, False if it's up.
 
         No argument.
 
         Example (for a Turtle instance named turtle):
@@ -701,15 +713,16 @@
         >>> turtle.pencolor('red')
         >>> turtle.pencolor()
         'red'
         """
         if color is None:
             return self._pencolor
         self._pencolor = color
-        self._p5.stroke(self._pencolor)
+        self._pen.stroke(self._pencolor)
+        self._render()
 
     def fillcolor(self, color=None):
         """Return or set the fillcolor.
 
         Arguments:
         Four input formats are allowed:
           - fillcolor()
@@ -726,28 +739,29 @@
         >>> turtle.fillcolor('violet')
         >>> col = turtle.pencolor()
         >>> turtle.fillcolor(col)
         """
         if color is None:
             return self._fillcolor
         self._fillcolor = color
+        self._render()
 
     def clear(self):
         """Delete the turtle's drawings from the screen. Do not move turtle.
 
         No arguments.
 
         Delete the turtle's drawings from the screen. Do not move turtle.
         State and position of the turtle as well as drawings of other
         turtles are not affected.
 
         Examples (for a Turtle instance named turtle):
         >>> turtle.clear()
         """
-        self._p5.clear()
+        self._pen.clear()
         self._render()
 
     def reset(self):
         """Return the turtle to its initial state and clear its drawings from
         the screen.
 
         No arguments.
@@ -755,19 +769,19 @@
         Examples (for a Turtle instance named turtle):
         >>> turtle.reset()
         """
         self._is_drawing = True
         self._pencolor = "black"
         self._pensize = 1
         self._speed = 1
-        self._p5.stroke(self._pencolor)
-        self._p5.stroke_weight(self._pensize)
+        self._pen.stroke(self._pencolor)
+        self._pen.stroke_weight(self._pensize)
         self._is_filling = False
         self._fillcolor = "white"
-        self._p5.no_fill()
+        self._pen.no_fill()
         self._is_drawing_poly = False
         self._x = self.width * 0.5
         self._y = self.height * 0.5
         self._angle = 0
         self.clear()
 
     def begin_poly(self):
@@ -778,29 +792,29 @@
         Start recording the vertices of a polygon. Current turtle position
         is first point of polygon.
 
         Example (for a Turtle instance named turtle):
         >>> turtle.begin_poly()
         """
         if self._is_drawing:
-            self._p5.begin_shape()
+            self._pen.begin_shape()
             self._is_drawing_poly = True
 
     def end_poly(self):
         """Stop recording the vertices of a polygon.
 
         No argument.
 
         Stop recording the vertices of a polygon. Current turtle position is
         last point of polygon. This will be connected with the first point.
 
         Example (for a Turtle instance named turtle):
         >>> turtle.end_poly()
         """
-        self._p5.end_shape()
+        self._pen.end_shape()
         if self._is_drawing_poly:
             self._render()
         self._is_drawing_poly = False
 
     def begin_fill(self):
         """Called just before drawing a shape to be filled.
 
@@ -810,30 +824,30 @@
         >>> turtle.pencolor("black")
         >>> turtle.fillcolor("red")
         >>> turtle.begin_fill()
         >>> turtle.circle(60)
         >>> turtle.end_fill()
         """
         self._is_filling = True
-        self._p5.fill(self._fillcolor)
+        self._pen.fill(self._fillcolor)
 
     def end_fill(self):
         """Fill the shape drawn after the call begin_fill().
 
         No argument.
 
         Example (for a Turtle instance named turtle):
         >>> turtle.pencolor("black")
         >>> turtle.fillcolor("red")
         >>> turtle.begin_fill()
         >>> turtle.circle(60)
         >>> turtle.end_fill()
         """
         self._is_filling = False
-        self._p5.no_fill()
+        self._pen.no_fill()
 
     def filling(self):
         """Return fillstate (True if filling, False else).
 
         No argument.
 
         Example (for a Turtle instance named turtle):
```

### Comparing `ipycc-0.0.12/src/ipycc.egg-info/PKG-INFO` & `ipycc-0.0.13/src/ipycc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipycc
-Version: 0.0.12
+Version: 0.0.13
 Summary: A Python package for creative coding in Jupyter
 Home-page: https://github.com/nickmcintyre/ipycc
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/ipycc/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -16,46 +16,44 @@
 
 # ipycc
 > A Python package for creative coding in Jupyter
 
 This package makes it easy to explore creative coding in Python using Jupyter notebooks. Its design is heavily inspired by [p5.js](https://github.com/processing/p5.js) and [Turtle graphics](https://docs.python.org/3/library/turtle.html) from the Python standard library.
 
 ## Turtles
-A light blue square with a smaller square outlined in green at its center. The square is drawn one side at a time.
+A dark blue square with a sprial pattern drawn in white. The spiral is drawn one side at a time.
 ```python
 from ipycc import Turtle
 
 
 ted = Turtle()
 ted.draw()
-
 ted.bgcolor("midnightblue")
 ted.pencolor("ghostwhite")
-ted.pendown()
-side = 5
-while side < ted.width:
-    ted.fd(side)
-    ted.lt(90)
+for side in range(40):
+    length = side * 5
+    ted.fd(length)
+    await ted.delay(0.1)
+    ted.lt(123)
     await ted.delay(0.1)
-    side += 5
 ```
 
 ## Sketches
 A light blue square with a circle in its center. The circle is drawn with a white center and black edge.
 ```python
 from ipycc import Sketch
 
 
 p5 = Sketch(400, 400)
 p5.background("dodgerblue")
 p5.circle(200, 200, 50)
 p5.run_sketch()
 ```
 
-A dark blue square with ten circles in its center. The circles are drawn in white and move in synchrony.
+Ten white circles moving like fireflies on a dark blue background.
 ```python
 import math
 from random import uniform
 from ipycc import Sketch
 
 
 p5 = Sketch(400, 400)
```

