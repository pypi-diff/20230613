# Comparing `tmp/ggtag-0.1.2.tar.gz` & `tmp/ggtag-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ggtag-0.1.2.tar", last modified: Fri Apr  7 07:51:40 2023, max compression
+gzip compressed data, was "ggtag-1.1.0.tar", last modified: Tue Jun 13 12:35:45 2023, max compression
```

## Comparing `ggtag-0.1.2.tar` & `ggtag-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-04-07 07:51:40.912639 ggtag-0.1.2/
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)       72 2023-03-24 11:10:45.000000 ggtag-0.1.2/MANIFEST.in
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     1378 2023-04-07 07:51:40.912639 ggtag-0.1.2/PKG-INFO
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      883 2023-04-06 14:36:27.000000 ggtag-0.1.2/README.md
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     2301 2023-03-30 06:13:07.000000 ggtag-0.1.2/cggtag.c
-drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-04-07 07:51:40.908639 ggtag-0.1.2/ggtag.egg-info/
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     1378 2023-04-07 07:51:40.000000 ggtag-0.1.2/ggtag.egg-info/PKG-INFO
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      644 2023-04-07 07:51:40.000000 ggtag-0.1.2/ggtag.egg-info/SOURCES.txt
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)        1 2023-04-07 07:51:40.000000 ggtag-0.1.2/ggtag.egg-info/dependency_links.txt
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)       13 2023-04-07 07:51:40.000000 ggtag-0.1.2/ggtag.egg-info/top_level.txt
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     4267 2023-04-06 07:34:30.000000 ggtag-0.1.2/ggtag.py
-drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-04-07 07:51:40.908639 ggtag-0.1.2/host/
-drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-04-07 07:51:40.908639 ggtag-0.1.2/host/include/
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      877 2023-04-07 07:51:40.000000 ggtag-0.1.2/host/include/ggtag.h
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      233 2023-04-07 07:51:40.000000 ggtag-0.1.2/host/include/utils.h
-drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-04-07 07:51:40.908639 ggtag-0.1.2/host/src/
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    24874 2023-04-07 07:51:40.000000 ggtag-0.1.2/host/src/ggtag.cpp
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      254 2023-04-07 07:51:40.000000 ggtag-0.1.2/host/src/rfid.cpp
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    28757 2023-04-07 07:51:40.000000 ggtag-0.1.2/host/src/utils.cpp
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)       38 2023-04-07 07:51:40.912639 ggtag-0.1.2/setup.cfg
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     1205 2023-04-06 14:53:21.000000 ggtag-0.1.2/setup.py
-drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-04-07 07:51:40.908639 ggtag-0.1.2/shared/
-drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-04-07 07:51:40.908639 ggtag-0.1.2/shared/include/
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     7274 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/include/GUI_Paint.h
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      171 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/include/debug.h
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     3107 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/include/fonts.h
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     1237 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/include/protocol.h
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    17866 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/include/qrcodegen.h
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      171 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/include/rfid.h
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)   199033 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/include/stb_truetype.h
-drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-04-07 07:51:40.912639 ggtag-0.1.2/shared/src/
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    31639 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/GUI_Paint.c
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      453 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/debug.c
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)  1250359 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/fa.c
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    25780 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/font12.c
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    47973 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/font16.c
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    64320 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/font20.c
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    96590 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/font24.c
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    17398 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/font8.c
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     8696 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/protocol.cpp
--rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    41771 2023-04-07 07:51:40.000000 ggtag-0.1.2/shared/src/qrcodegen.c
+drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-06-13 12:35:45.923387 ggtag-1.1.0/
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)       72 2023-03-24 11:10:45.000000 ggtag-1.1.0/MANIFEST.in
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     1378 2023-06-13 12:35:45.923387 ggtag-1.1.0/PKG-INFO
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      883 2023-05-26 12:12:59.000000 ggtag-1.1.0/README.md
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     2361 2023-06-05 12:34:55.000000 ggtag-1.1.0/cggtag.c
+drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-06-13 12:35:45.923387 ggtag-1.1.0/ggtag.egg-info/
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     1378 2023-06-13 12:35:45.000000 ggtag-1.1.0/ggtag.egg-info/PKG-INFO
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      725 2023-06-13 12:35:45.000000 ggtag-1.1.0/ggtag.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)        1 2023-06-13 12:35:45.000000 ggtag-1.1.0/ggtag.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)       13 2023-06-13 12:35:45.000000 ggtag-1.1.0/ggtag.egg-info/top_level.txt
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     4740 2023-06-13 12:23:19.000000 ggtag-1.1.0/ggtag.py
+drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-06-13 12:35:45.923387 ggtag-1.1.0/host/
+drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-06-13 12:35:45.923387 ggtag-1.1.0/host/include/
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     1048 2023-06-13 12:35:45.000000 ggtag-1.1.0/host/include/ggtag.h
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      233 2023-06-13 12:35:45.000000 ggtag-1.1.0/host/include/utils.h
+drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-06-13 12:35:45.923387 ggtag-1.1.0/host/src/
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    27591 2023-06-13 12:35:45.000000 ggtag-1.1.0/host/src/ggtag.cpp
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      254 2023-06-13 12:35:45.000000 ggtag-1.1.0/host/src/rfid.cpp
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    28757 2023-06-13 12:35:45.000000 ggtag-1.1.0/host/src/utils.cpp
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)       38 2023-06-13 12:35:45.923387 ggtag-1.1.0/setup.cfg
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     1322 2023-06-05 12:28:50.000000 ggtag-1.1.0/setup.py
+drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-06-13 12:35:45.923387 ggtag-1.1.0/shared/
+drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-06-13 12:35:45.923387 ggtag-1.1.0/shared/include/
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     7274 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/include/GUI_Paint.h
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      171 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/include/debug.h
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     3123 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/include/fonts.h
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     1997 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/include/protocol.h
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    17866 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/include/qrcodegen.h
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      171 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/include/rfid.h
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)   199033 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/include/stb_truetype.h
+drwxrwxr-x   0 rgerganov  (1000) rgerganov  (1000)        0 2023-06-13 12:35:45.923387 ggtag-1.1.0/shared/src/
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    31639 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/GUI_Paint.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)   609804 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/courier.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)      453 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/debug.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)  1250359 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/fa.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    25780 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/font12.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    47973 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/font16.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    64320 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/font20.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    96590 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/font24.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)   141780 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/font28.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)   167621 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/font32.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)   218952 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/font36.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    17398 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/font8.c
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)     9674 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/protocol.cpp
+-rw-rw-r--   0 rgerganov  (1000) rgerganov  (1000)    41771 2023-06-13 12:35:45.000000 ggtag-1.1.0/shared/src/qrcodegen.c
```

### Comparing `ggtag-0.1.2/PKG-INFO` & `ggtag-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ggtag
-Version: 0.1.2
+Version: 1.1.0
 Summary: Python bindings for ggtag
 Home-page: https://github.com/rgerganov/ggtag
 Author: Radoslav Gerganov
 Author-email: rgerganov@gmail.com
 License: UNKNOWN
 Description: Python bindings for `ggtag`.
```

### Comparing `ggtag-0.1.2/README.md` & `ggtag-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/cggtag.c` & `ggtag-1.1.0/cggtag.c`

 * *Files 8% similar despite different names*

```diff
@@ -37,23 +37,23 @@
         buff_size = (width / 8 + 1) * height;
     }
     PyObject* result = Py_BuildValue("y#", bitmap, buff_size);
     free(bitmap);
     return result;
 }
 
-static PyObject *method_dither(PyObject *self, PyObject *args) {
+static PyObject *method_monoimage(PyObject *self, PyObject *args) {
     const uint8_t *rgba;
     Py_ssize_t rgba_size;
-    int width, height;
+    int width, height, dither;
 
-    if (!PyArg_ParseTuple(args, "y#ii", &rgba, &rgba_size, &width, &height)) {
+    if (!PyArg_ParseTuple(args, "y#iip", &rgba, &rgba_size, &width, &height, &dither)) {
         return NULL;
     }
-    uint8_t *bitmap = dither(rgba, width, height);
+    uint8_t *bitmap = monoimage(rgba, width, height, dither);
     Py_ssize_t buff_size = width * height;
     if (buff_size % 8 == 0) {
         buff_size = buff_size / 8;
     } else {
         buff_size = buff_size / 8 + 1;
     }
     PyObject* result = Py_BuildValue("y#", bitmap, buff_size);
@@ -61,15 +61,15 @@
     return result;
 }
 
 static PyMethodDef EncodeMethods[] = {
     {"encode", method_encode, METH_VARARGS, "Encode text commands to ggtag's binary format"},
     {"last_error", method_lasterror, METH_VARARGS, "Returns the last error from the parser"},
     {"render", method_render, METH_VARARGS, "Render text commands to bitmap"},
-    {"dither", method_dither, METH_VARARGS, "Dither the specified RGBA image"},
+    {"monoimage", method_monoimage, METH_VARARGS, "Convert the specified RGBA image to monochrome bitmap"},
     {NULL, NULL, 0, NULL}
 };
 
 
 static struct PyModuleDef cggtagmodule = {
     PyModuleDef_HEAD_INIT,
     "cggtag",
```

### Comparing `ggtag-0.1.2/ggtag.egg-info/PKG-INFO` & `ggtag-1.1.0/ggtag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ggtag
-Version: 0.1.2
+Version: 1.1.0
 Summary: Python bindings for ggtag
 Home-page: https://github.com/rgerganov/ggtag
 Author: Radoslav Gerganov
 Author-email: rgerganov@gmail.com
 License: UNKNOWN
 Description: Python bindings for `ggtag`.
```

### Comparing `ggtag-0.1.2/ggtag.egg-info/SOURCES.txt` & `ggtag-1.1.0/ggtag.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -16,16 +16,20 @@
 shared/include/debug.h
 shared/include/fonts.h
 shared/include/protocol.h
 shared/include/qrcodegen.h
 shared/include/rfid.h
 shared/include/stb_truetype.h
 shared/src/GUI_Paint.c
+shared/src/courier.c
 shared/src/debug.c
 shared/src/fa.c
 shared/src/font12.c
 shared/src/font16.c
 shared/src/font20.c
 shared/src/font24.c
+shared/src/font28.c
+shared/src/font32.c
+shared/src/font36.c
 shared/src/font8.c
 shared/src/protocol.cpp
 shared/src/qrcodegen.c
```

### Comparing `ggtag-0.1.2/ggtag.py` & `ggtag-1.1.0/ggtag.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,28 +42,35 @@
         self._text_cmd += "\\l{},{},{},{}".format(x1, y1, x2, y2)
 
     def qrcode(self, x, y, size, text):
         """Place QR code at position (x, y) with the given size and text."""
         self._check_xy(x, y)
         self._text_cmd += "\\q{},{},{},{}".format(x, y, size, text)
 
-    def image(self, x, y, width, height, rgba_image):
+    def image(self, x, y, width, height, rgba_image, dither=False):
         """Draw image at position (x, y) with the given width and height.
         The image is given as a byte array of RGBA values in row-major order.
         """
         self._check_xy(x, y)
-        bitmap = cggtag.dither(rgba_image, width, height)
+        bitmap = cggtag.monoimage(rgba_image, width, height, dither)
         image = base64.b64encode(bitmap).decode("utf-8")
         self._text_cmd += "\\i{},{},{},{},{}".format(x, y, width, height, image)
 
-    def image_url(self, x, y, width, height, url):
+    def image_png(self, x, y, width, height, png_image, dither=False):
+        """Draw PNG image at position (x, y) with the given width and height.
+        """
+        self._check_xy(x, y)
+        b64png = base64.b64encode(png_image).decode("utf-8")
+        self._text_cmd += "\\P{},{},{},{},{},{}".format(x, y, width, height, int(dither), b64png)
+
+    def image_url(self, x, y, width, height, dither, url):
         """Place the image from the given URL at position (x, y) with the given
         width and height."""
         self._check_xy(x, y)
-        self._text_cmd += "\\I{},{},{},{},{}".format(x, y, width, height, url)
+        self._text_cmd += "\\I{},{},{},{},{},{}".format(x, y, width, height, int(dither), url)
 
     def icon(self, x, y, height, icon_name):
         """Place the icon with the given name at position (x, y) with the given
         height. Refer to https://fontawesome.com/v5/cheatsheet/free/solid for
         a list of available icons."""
         self._check_xy(x, y)
         self._text_cmd += "\\a{},{},{},{}".format(x, y, height, icon_name)
@@ -86,14 +93,16 @@
                 bit = 0x80 >> (col % 8)
                 result[row][col] = 1 if byte & bit else 0
         return result
 
     def browse(self, host='https://ggtag.io'):
         """Open the tag in a web browser."""
         url = "{}/?i={}".format(host, urllib.parse.quote(self._text_cmd, safe=''))
+        if len(url) > 8200:
+            print("Warning: URL is too long")
         webbrowser.open(url)
 
     def __bytes__(self):
         """Return the tag as a byte array. The result can be programmed into a
         ggtag device using either ggwave or pyserial."""
         return cggtag.encode(self._text_cmd)
```

### Comparing `ggtag-0.1.2/host/include/ggtag.h` & `ggtag-1.1.0/host/include/ggtag.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 #pragma once
 #include <stdint.h>
+#include <stdbool.h>
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // Allocates a buffer and encodes the input string into it. The buffer length is returned in 'length'.
 // Caller is responsible for freeing the buffer.
 uint8_t* encode(const char *input, int *length);
 
 // Returns the last error message from the parser.
 // The memory is owned by the parser and should not be freed.
 char* getLastError();
 
-// Allocates a bitmap with dimensions [ceil(width/8), height] and renders the specified input string to it.
+// Allocates a bitmap with dimensions [ceil(width/8), height] and renders the tag produced by the specified input string.
 // Caller is responsible for freeing the bitmap.
 uint8_t* render(const char *input, int width, int height);
 
-// Allocates a bitmap with size ceil(width * height / 8) and performs dithering of the specified input image.
+// Converts the specified RGBA image to a monochrome bitmap.
+// Allocates a bitmap with size ceil(width * height / 8) and renders the image into it.
+// If dither is true, the image is dithered using the Floyd-Steinberg algorithm.
 // Caller is responsible for freeing the bitmap.
-uint8_t* dither(const uint8_t *rgba, int width, int height);
+uint8_t* monoimage(const uint8_t *rgba, int width, int height, bool dither);
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `ggtag-0.1.2/host/src/ggtag.cpp` & `ggtag-1.1.0/host/src/ggtag.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 
 struct RFIDCmd {
     bool is_hid; // true means HID, false means EM4102
     int id1;
     int id2;
 };
 
+static uint8_t* rl_encode(const uint8_t *bitmap, int bitmap_size, int *rle_length);
+
 struct BitBuffer {
     uint8_t *buffer;
     int capacity; // capacity in bytes
     int ind; // current bit index
 
     BitBuffer() {
         ind = 0;
@@ -85,222 +87,265 @@
     int size() {
         int ret = ind / 8;
         if (ind % 8 != 0) {
             ret++;
         }
         return ret;
     }
-
-    bool addBits(uint32_t value, int num_bits)
+    bool ensureCapacity(int num_bits)
     {
-        if (!buffer || num_bits > 32) {
+        if (!buffer) {
             return false;
         }
         if (ind + num_bits > capacity * 8) {
             buffer = (uint8_t*) realloc(buffer, capacity * 2);
             if (!buffer) {
                 return false;
             }
             memset(buffer + capacity, 0, capacity);
             capacity *= 2;
         }
+        return true;
+    }
+    bool addBits(int8_t bit, int num_bits)
+    {
+        if (bit != 0 && bit != 1) {
+            return false;
+        }
+        if (!ensureCapacity(num_bits)) {
+            return false;
+        }
+        for (int i = 0; i < num_bits; i++) {
+            if (bit) {
+                buffer[ind / 8] |= (1 << (7 - (ind % 8)));
+            }
+            ind++;
+        }
+        return true;
+    }
+    bool addValue(uint32_t value, int num_bits)
+    {
+        if (num_bits > 32) {
+            return false;
+        }
+        if (!ensureCapacity(num_bits)) {
+            return false;
+        }
         for (int i = 0; i < num_bits; i++) {
             if (value & (1 << (num_bits - i - 1))) {
                 buffer[ind / 8] |= (1 << (7 - (ind % 8)));
             }
             ind++;
         }
         return true;
     }
     bool addCmd(const TextCmd &cmd)
     {
-        if (!addBits(TEXT_CMD, CMD_BITS)) {
+        if (!addValue(TEXT_CMD, CMD_BITS)) {
             return false;
         }
-        if (!addBits(cmd.x, X_BITS)) {
+        if (!addValue(cmd.x, X_BITS)) {
             return false;
         }
-        if (!addBits(cmd.y, Y_BITS)) {
+        if (!addValue(cmd.y, Y_BITS)) {
             return false;
         }
         // font numbers are zero-based
-        if (!addBits(cmd.font-1, FONT_BITS)) {
+        if (!addValue(cmd.font-1, FONT_BITS)) {
             return false;
         }
-        if (!addBits(cmd.text_len, LENGTH_BITS)) {
+        if (!addValue(cmd.text_len, LENGTH_BITS)) {
             return false;
         }
         const char *ptr = cmd.text;
         for (int i = 0; i < cmd.text_len; i++) {
-            if (!addBits(*ptr, CHAR_BITS)) {
+            if (!addValue(*ptr, CHAR_BITS)) {
                 return false;
             }
             if (*ptr == '\\') {
                 ptr++;
             }
             ptr++;
         }
         return true;
     }
     bool addCmd(const ImageCmd &cmd)
     {
-        if (!addBits(IMAGE_CMD, CMD_BITS)) {
+        int img_size = cmd.width * cmd.height;
+        const uint8_t *img = 0;
+        int decoded_size = cmd.b64_data_len/4*3;
+        uint8_t *bmp = (uint8_t*) malloc(decoded_size);
+        if (!bmp) {
             return false;
         }
-        if (!addBits(cmd.x, X_BITS)) {
-            return false;
+        b64_decode((const uint8_t*)cmd.b64_data, cmd.b64_data_len, bmp);
+        int rle_size = 0;
+        uint8_t *rle_image = rl_encode(bmp, img_size, &rle_size);
+        if (rle_image && rle_size < img_size) {
+            img = rle_image;
+            img_size = rle_size;
+            // run-length encoded bitmap
+            if (!addValue(RLE_IMAGE_CMD, CMD_BITS)) {
+                return false;
+            }
+        } else {
+            img = bmp;
+            // normal bitmap
+            if (!addValue(IMAGE_CMD, CMD_BITS)) {
+                return false;
+            }
         }
-        if (!addBits(cmd.y, Y_BITS)) {
+        if (!addValue(cmd.x, X_BITS)) {
             return false;
         }
-        if (!addBits(cmd.width, X_BITS)) {
+        if (!addValue(cmd.y, Y_BITS)) {
             return false;
         }
-        if (!addBits(cmd.height, Y_BITS)) {
+        if (!addValue(cmd.width, X_BITS)) {
             return false;
         }
-        int decoded_size = cmd.b64_data_len/4*3;
-        uint8_t *decoded = (uint8_t*) malloc(decoded_size);
-        if (!decoded) {
+        if (!addValue(cmd.height, Y_BITS)) {
             return false;
         }
-        b64_decode((const uint8_t*)cmd.b64_data, cmd.b64_data_len, decoded);
-        int img_size = cmd.width * cmd.height;
         for (int i = 0; i < img_size/8; i++) {
-            if (!addBits(decoded[i], 8)) {
-                free(decoded);
+            if (!addValue(img[i], 8)) {
+                free(bmp);
+                free(rle_image);
                 return false;
             }
         }
         if (img_size % 8 != 0) {
-            if (!addBits(decoded[img_size/8], img_size % 8)) {
-                free(decoded);
+            int rem_bits = img_size % 8;
+            if (!addValue(img[img_size/8] >> (8-rem_bits), rem_bits)) {
+                free(bmp);
+                free(rle_image);
                 return false;
             }
         }
-        free(decoded);
+        free(bmp);
+        free(rle_image);
         return true;
     }
     bool addCmd(const IconCmd &cmd)
     {
-        if (!addBits(ICON_CMD, CMD_BITS)) {
+        if (!addValue(ICON_CMD, CMD_BITS)) {
             return false;
         }
-        if (!addBits(cmd.x, X_BITS)) {
+        if (!addValue(cmd.x, X_BITS)) {
             return false;
         }
-        if (!addBits(cmd.y, Y_BITS)) {
+        if (!addValue(cmd.y, Y_BITS)) {
             return false;
         }
-        if (!addBits(cmd.height, Y_BITS)) {
+        if (!addValue(cmd.height, Y_BITS)) {
             return false;
         }
-        if (!addBits(cmd.codepoint, ICON_BITS)) {
+        if (!addValue(cmd.codepoint, ICON_BITS)) {
             return false;
         }
         return true;
     }
     bool addCmd(const RFIDCmd &cmd)
     {
-        if (!addBits(RFID_CMD, CMD_BITS)) {
+        if (!addValue(RFID_CMD, CMD_BITS)) {
             return false;
         }
-        if (!addBits(cmd.is_hid, 1)) {
+        if (!addValue(cmd.is_hid, 1)) {
             return false;
         }
-        if (!addBits(cmd.id1, RFID1_BITS)) {
+        if (!addValue(cmd.id1, RFID1_BITS)) {
             return false;
         }
-        if (!addBits(cmd.id2, RFID2_BITS)) {
+        if (!addValue(cmd.id2, RFID2_BITS)) {
             return false;
         }
         return true;
     }
     bool addCmd(const QRCodeCmd &cmd)
     {
-        if (!addBits(QRCODE_CMD, CMD_BITS)) {
+        if (!addValue(QRCODE_CMD, CMD_BITS)) {
             return false;
         }
-        if (!addBits(cmd.x, X_BITS)) {
+        if (!addValue(cmd.x, X_BITS)) {
             return false;
         }
-        if (!addBits(cmd.y, Y_BITS)) {
+        if (!addValue(cmd.y, Y_BITS)) {
             return false;
         }
         // pixel_width is zero-based
-        if (!addBits(cmd.pixel_width-1, QR_PIXEL_WIDTH)) {
+        if (!addValue(cmd.pixel_width-1, QR_PIXEL_WIDTH)) {
             return false;
         }
-        if (!addBits(cmd.text_len, LENGTH_BITS)) {
+        if (!addValue(cmd.text_len, LENGTH_BITS)) {
             return false;
         }
         const char *ptr = cmd.text;
         for (int i = 0; i < cmd.text_len; i++) {
-            if (!addBits(*ptr, CHAR_BITS)) {
+            if (!addValue(*ptr, CHAR_BITS)) {
                 return false;
             }
             if (*ptr == '\\') {
                 ptr++;
             }
             ptr++;
         }
         return true;
     }
     bool addCmd(const RectCmd &cmd, bool fill)
     {
         int cmd_bits = fill ? FILL_RECT_CMD : RECT_CMD;
-        if (!addBits(cmd_bits, CMD_BITS)) {
+        if (!addValue(cmd_bits, CMD_BITS)) {
             return false;
         }
-        if (!addBits(cmd.x, X_BITS)) {
+        if (!addValue(cmd.x, X_BITS)) {
             return false;
         }
-        if (!addBits(cmd.y, Y_BITS)) {
+        if (!addValue(cmd.y, Y_BITS)) {
             return false;
         }
-        if (!addBits(cmd.width, X_BITS)) {
+        if (!addValue(cmd.width, X_BITS)) {
             return false;
         }
-        if (!addBits(cmd.height, Y_BITS)) {
+        if (!addValue(cmd.height, Y_BITS)) {
             return false;
         }
         return true;
     }
     bool addCmd(const CircleCmd &cmd, bool fill)
     {
         int cmd_bits = fill ? FILL_CIRCLE_CMD : CIRCLE_CMD;
-        if (!addBits(cmd_bits, CMD_BITS)) {
+        if (!addValue(cmd_bits, CMD_BITS)) {
             return false;
         }
-        if (!addBits(cmd.x, X_BITS)) {
+        if (!addValue(cmd.x, X_BITS)) {
             return false;
         }
-        if (!addBits(cmd.y, Y_BITS)) {
+        if (!addValue(cmd.y, Y_BITS)) {
             return false;
         }
-        if (!addBits(cmd.r, R_BITS)) {
+        if (!addValue(cmd.r, R_BITS)) {
             return false;
         }
         return true;
     }
     bool addCmd(const LineCmd &cmd)
     {
-        if (!addBits(LINE_CMD, CMD_BITS)) {
+        if (!addValue(LINE_CMD, CMD_BITS)) {
             return false;
         }
-        if (!addBits(cmd.x1, X_BITS)) {
+        if (!addValue(cmd.x1, X_BITS)) {
             return false;
         }
-        if (!addBits(cmd.y1, Y_BITS)) {
+        if (!addValue(cmd.y1, Y_BITS)) {
             return false;
         }
-        if (!addBits(cmd.x2, X_BITS)) {
+        if (!addValue(cmd.x2, X_BITS)) {
             return false;
         }
-        if (!addBits(cmd.y2, Y_BITS)) {
+        if (!addValue(cmd.y2, Y_BITS)) {
             return false;
         }
         return true;
     }
     void dumpBits()
     {
         printf("Bit count: %d\n", ind);
@@ -867,15 +912,15 @@
 // Returns the last error message from the parser.
 // The memory is owned by the parser and should not be freed.
 char* getLastError()
 {
     return lastError;
 }
 
-// Allocates a bitmap with dimensions [ceil(width/8), height] and renders the specified input string to it.
+// Allocates a bitmap with dimensions [ceil(width/8), height] and renders the tag produced by the specified input string.
 // Caller is responsible for freeing the bitmap.
 uint8_t* render(const char *input, int width, int height)
 {
     if (!input || width <= 0 || height <= 0) {
         return 0;
     }
     int offset = 0;
@@ -900,45 +945,91 @@
     memset(bitmap, 0, total);
     Paint_NewImage(bitmap, width, height, 0, WHITE);
     Paint_Clear(WHITE);
     renderBits(buf.buffer, buf.ind);
     return bitmap;
 }
 
-// Allocates a bitmap with size ceil(width * height / 8) and performs dithering of the specified input image.
+static void rl_number(BitBuffer *buf, int num)
+{
+    int divider = (1 << RLE_BITS) - 1;
+    if (num < divider) {
+        buf->addValue(num, RLE_BITS);
+    } else {
+        rl_number(buf, num / divider);
+        buf->addValue(num % divider, RLE_BITS);
+    }
+}
+
+static uint8_t* rl_encode(const uint8_t *bitmap, int bitmap_size, int *rle_length)
+{
+    int divider = (1 << RLE_BITS) - 1;
+    BitBuffer buf;
+    BitReader reader(bitmap, bitmap_size);
+    uint8_t curr_value = 0;
+    int count = 0;
+    for (int i = 0 ; i < bitmap_size ; i++) {
+        int val = reader.read(1);
+        if (val == curr_value) {
+            count++;
+        } else {
+            if (count > 0) {
+                rl_number(&buf, count);
+            }
+            buf.addValue(divider, RLE_BITS);
+            curr_value = val;
+            count = 1;
+        }
+    }
+    rl_number(&buf, count);
+    debug("RLE size: %d (%.02f orig size)\n", buf.ind, (float)buf.ind / (bitmap_size));
+    uint8_t *ret = (uint8_t*) calloc(buf.size(), 1);
+    if (!ret) {
+        return 0;
+    }
+    memcpy(ret, buf.buffer, buf.size());
+    *rle_length = buf.ind;
+    return ret;
+}
+
+// Converts the specified RGBA image to a monochrome bitmap.
+// Allocates a bitmap with size ceil(width * height / 8) and renders the image into it.
+// If dither is true, the image is dithered using the Floyd-Steinberg algorithm.
 // Caller is responsible for freeing the bitmap.
-uint8_t* dither(const uint8_t *rgba, int width, int height)
+uint8_t* monoimage(const uint8_t *rgba, int width, int height, bool dither)
 {
     if (!rgba || width <= 0 || height <= 0) {
         return 0;
     }
     float *gray = (float*) malloc(width * height * sizeof(float));
     if (!gray) {
         return 0;
     }
     for (int i = 0; i < width * height; i++) {
         gray[i] = 0.2126 * rgba[i*4] + 0.7152 * rgba[i*4+1] + 0.0722 * rgba[i*4+2];
     }
-    for (int y = 0; y < height; y++) {
-        for (int x = 0; x < width; x++) {
-            float oldpixel = gray[y * width + x];
-            float newpixel = (oldpixel > 127) ? 255 : 0;
-            gray[y * width + x] = newpixel;
-            float quant_error = oldpixel - newpixel;
-            if (x < width - 1) {
-                gray[y * width + x + 1] += quant_error * 7.0 / 16.0;
-            }
-            if (x > 0 && y < height - 1) {
-                gray[(y + 1) * width + x - 1] += quant_error * 3.0 / 16.0;
-            }
-            if (y < height - 1) {
-                gray[(y + 1) * width + x] += quant_error * 5.0 / 16.0;
-            }
-            if (x < width - 1 && y < height - 1) {
-                gray[(y + 1) * width + x + 1] += quant_error * 1.0 / 16.0;
+    if (dither) {
+        for (int y = 0; y < height; y++) {
+            for (int x = 0; x < width; x++) {
+                float oldpixel = gray[y * width + x];
+                float newpixel = (oldpixel > 127) ? 255 : 0;
+                gray[y * width + x] = newpixel;
+                float quant_error = oldpixel - newpixel;
+                if (x < width - 1) {
+                    gray[y * width + x + 1] += quant_error * 7.0 / 16.0;
+                }
+                if (x > 0 && y < height - 1) {
+                    gray[(y + 1) * width + x - 1] += quant_error * 3.0 / 16.0;
+                }
+                if (y < height - 1) {
+                    gray[(y + 1) * width + x] += quant_error * 5.0 / 16.0;
+                }
+                if (x < width - 1 && y < height - 1) {
+                    gray[(y + 1) * width + x + 1] += quant_error * 1.0 / 16.0;
+                }
             }
         }
     }
     int length = width * height / 8;
     if (width * height % 8 != 0) {
         length += 1;
     }
@@ -971,9 +1062,10 @@
     free(ptr);
     ptr = render(input, 250, 122);
     free(ptr);
     const char *b64 = "aGVsbG8=";
     uint8_t data[128] = {0};
     b64_decode((const uint8_t*) b64, strlen(b64), data);
     printf("Decoded data: %s\n", data);
+    //rl_number(NULL, 9034, 4);
     return 0;
 }
```

### Comparing `ggtag-0.1.2/host/src/utils.cpp` & `ggtag-1.1.0/host/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/setup.py` & `ggtag-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, Extension
 
 def main():
     with open("README.md", "r") as fh:
         long_description = fh.read()
 
     setup(name="ggtag",
-          version="0.1.2",
+          version="1.1.0",
           description="Python bindings for ggtag",
           long_description=long_description,
           long_description_content_type="text/markdown",
           author="Radoslav Gerganov",
           author_email="rgerganov@gmail.com",
           include_dirs = ['host/include', 'shared/include'],
           py_modules = ['ggtag'],
@@ -23,13 +23,16 @@
                 "shared/src/GUI_Paint.c",
                 "shared/src/fa.c",
                 "shared/src/font8.c",
                 "shared/src/font12.c",
                 "shared/src/font16.c",
                 "shared/src/font20.c",
                 "shared/src/font24.c",
+                "shared/src/font28.c",
+                "shared/src/font32.c",
+                "shared/src/font36.c",
                 "shared/src/qrcodegen.c",
                 "shared/src/debug.c",
                 ])])
 
 if __name__ == "__main__":
     main()
```

### Comparing `ggtag-0.1.2/shared/include/GUI_Paint.h` & `ggtag-1.1.0/shared/include/GUI_Paint.h`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/include/fonts.h` & `ggtag-1.1.0/shared/include/fonts.h`

 * *Files 3% similar despite different names*

```diff
@@ -73,23 +73,23 @@
   uint16_t size;
   uint16_t ASCII_Width;
   uint16_t Width;
   uint16_t Height;
 
 }cFONT;
 
+extern sFONT Font36;
+extern sFONT Font32;
+extern sFONT Font28;
 extern sFONT Font24;
 extern sFONT Font20;
 extern sFONT Font16;
 extern sFONT Font12;
 extern sFONT Font8;
 
-extern cFONT Font12CN;
-extern cFONT Font24CN;
-
 extern const uint8_t fa_solid_900_ttf[];
 extern unsigned int fa_solid_900_ttf_len;
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `ggtag-0.1.2/shared/include/qrcodegen.h` & `ggtag-1.1.0/shared/include/qrcodegen.h`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/include/stb_truetype.h` & `ggtag-1.1.0/shared/include/stb_truetype.h`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/src/GUI_Paint.c` & `ggtag-1.1.0/shared/src/GUI_Paint.c`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/src/fa.c` & `ggtag-1.1.0/shared/src/fa.c`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/src/font12.c` & `ggtag-1.1.0/shared/src/font12.c`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/src/font16.c` & `ggtag-1.1.0/shared/src/font16.c`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/src/font20.c` & `ggtag-1.1.0/shared/src/font20.c`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/src/font24.c` & `ggtag-1.1.0/shared/src/font24.c`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/src/font8.c` & `ggtag-1.1.0/shared/src/font8.c`

 * *Files identical despite different names*

### Comparing `ggtag-0.1.2/shared/src/protocol.cpp` & `ggtag-1.1.0/shared/src/protocol.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -3,44 +3,14 @@
 #include "rfid.h"
 #include "debug.h"
 #include "protocol.h"
 #include "GUI_Paint.h"
 #define STB_TRUETYPE_IMPLEMENTATION
 #include "stb_truetype.h" /* http://nothings.org/stb/stb_truetype.h */
 
-struct BitReader {
-    const uint8_t *buffer;
-    int bits_count;
-    int ind;
-
-    BitReader(const uint8_t *buffer, int bits_count)
-        : buffer(buffer), bits_count(bits_count), ind(0)
-    {
-    }
-
-    uint32_t read(int num_bits)
-    {
-        if (num_bits > 32) {
-            return -1;
-        }
-        if (ind + num_bits > bits_count) {
-            return -1;
-        }
-        uint32_t result = 0;
-        for (int i = 0; i < num_bits; i++) {
-            result <<= 1;
-            if (buffer[ind / 8] & (1 << (7 - (ind % 8)))) {
-                result |= 1;
-            }
-            ind++;
-        }
-        return result;
-    }
-};
-
 // Renders the specified codepoint on a 1D bitmap with size ceil(out_width*out_height/8).
 // Caller is responsible for freeing the bitmap.
 static uint8_t* renderCodepoint(int codepoint, int height, int *out_width, int *out_height)
 {
     stbtt_fontinfo info;
     if (!stbtt_InitFont(&info, fa_solid_900_ttf, 0)) {
         printf("failed to load ttf font\n");
@@ -65,14 +35,44 @@
         int bit_n = 7 - (i % 8);
         bitmap[byte_n] |= bit << bit_n;
     }
     free(bytemap);
     return bitmap;
 }
 
+static void draw_bits(int x, int y, int offset, int w, int val, int count)
+{
+    for (int i = 0; i < count; i++) {
+        int col = x + (i + offset) % w;
+        int row = y + (i + offset) / w;
+        Paint_SetPixel(col, row, val ? BLACK : WHITE);
+    }
+}
+
+static void rle_img_render(BitReader *br, int x, int y, int width, int height)
+{
+    int divider = (1 << RLE_BITS) - 1;
+    uint8_t curr_value = 0;
+    int count = 0;
+    int offset = 0;
+    int img_size = width * height;
+    while (count+offset < img_size) {
+        int val = br->read(RLE_BITS);
+        if (val == divider) {
+            draw_bits(x, y, offset, width, curr_value, count);
+            curr_value = 1 - curr_value;
+            offset += count;
+            count = 0;
+        } else {
+            count = count * divider + val;
+        }
+    }
+    draw_bits(x, y, offset, width, curr_value, count);
+}
+
 void renderBits(const uint8_t *input, int bits_count)
 {
     BitReader br(input, bits_count);
     while (true) {
         int cmd = br.read(CMD_BITS);
         switch (cmd) {
             case TEXT_CMD: {
@@ -99,14 +99,20 @@
                     font = &Font12;
                 } else if (fontNum == 2) {
                     font = &Font16;
                 } else if (fontNum == 3) {
                     font = &Font20;
                 } else if (fontNum == 4) {
                     font = &Font24;
+                } else if (fontNum == 5) {
+                    font = &Font28;
+                } else if (fontNum == 6) {
+                    font = &Font32;
+                } else if (fontNum == 7) {
+                    font = &Font36;
                 }
                 Paint_DrawString_EN(x, y, text, font, WHITE, BLACK);
                 free(text);
                 break;
             }
             case RECT_CMD:
             case FILL_RECT_CMD: {
@@ -190,14 +196,26 @@
                             return;
                         }
                         Paint_SetPixel(x + j, y + i, color ? BLACK : WHITE);
                     }
                 }
                 break;
             }
+            case RLE_IMAGE_CMD: {
+                int x = br.read(X_BITS);
+                int y = br.read(Y_BITS);
+                int width = br.read(X_BITS);
+                int height = br.read(Y_BITS);
+                if (x < 0 || y < 0 || width < 0 || height < 0) {
+                    return;
+                }
+                debug("Render RLE image x=%d y=%d width=%d height=%d\n", x, y, width, height);
+                rle_img_render(&br, x, y, width, height);
+                break;
+            }
             case ICON_CMD: {
                 int x = br.read(X_BITS);
                 int y = br.read(Y_BITS);
                 int height = br.read(Y_BITS);
                 int codepoint = br.read(ICON_BITS);
                 if (codepoint < 0 || x < 0 || y < 0 || height < 0) {
                     return;
```

### Comparing `ggtag-0.1.2/shared/src/qrcodegen.c` & `ggtag-1.1.0/shared/src/qrcodegen.c`

 * *Files identical despite different names*

