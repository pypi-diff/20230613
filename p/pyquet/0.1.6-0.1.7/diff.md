# Comparing `tmp/pyquet-0.1.6.tar.gz` & `tmp/pyquet-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquet-0.1.6.tar", last modified: Mon Jun 12 20:39:08 2023, max compression
+gzip compressed data, was "pyquet-0.1.7.tar", last modified: Mon Jun 12 21:04:37 2023, max compression
```

## Comparing `pyquet-0.1.6.tar` & `pyquet-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.136924 pyquet-0.1.6/
--rw-rw-rw-   0        0        0     1086 2023-05-26 12:18:55.000000 pyquet-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      546 2023-06-12 20:39:08.136924 pyquet-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-05-26 12:18:55.000000 pyquet-0.1.6/README.md
--rw-rw-rw-   0        0        0      104 2023-06-11 07:58:49.000000 pyquet-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      674 2023-06-12 20:39:08.140913 pyquet-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.120416 pyquet-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.126906 pyquet-0.1.6/src/pyquet/
--rw-rw-rw-   0        0        0        0 2023-05-26 10:40:59.000000 pyquet-0.1.6/src/pyquet/__init__.py
--rw-rw-rw-   0        0        0      628 2023-06-12 19:39:16.000000 pyquet-0.1.6/src/pyquet/common.py
--rw-rw-rw-   0        0        0     1867 2023-06-11 09:50:23.000000 pyquet-0.1.6/src/pyquet/editor.py
--rw-rw-rw-   0        0        0     3088 2023-06-12 20:32:51.000000 pyquet-0.1.6/src/pyquet/editor_ui.py
--rw-rw-rw-   0        0        0     6599 2023-06-11 09:50:23.000000 pyquet-0.1.6/src/pyquet/generator.py
--rw-rw-rw-   0        0        0     2176 2023-05-27 09:33:39.000000 pyquet-0.1.6/src/pyquet/schemas.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.135927 pyquet-0.1.6/src/pyquet.egg-info/
--rw-rw-rw-   0        0        0      546 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.135927 pyquet-0.1.6/tests/
--rw-rw-rw-   0        0        0     2078 2023-05-27 09:31:42.000000 pyquet-0.1.6/tests/test_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:04:37.070296 pyquet-0.1.7/
+-rw-rw-rw-   0        0        0     1086 2023-05-26 12:18:55.000000 pyquet-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      546 2023-06-12 21:04:37.070296 pyquet-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-05-26 12:18:55.000000 pyquet-0.1.7/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-11 07:58:49.000000 pyquet-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      760 2023-06-12 21:04:37.074792 pyquet-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 21:04:37.052240 pyquet-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 21:04:37.059316 pyquet-0.1.7/src/pyquet/
+-rw-rw-rw-   0        0        0        0 2023-05-26 10:40:59.000000 pyquet-0.1.7/src/pyquet/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-06-12 19:39:16.000000 pyquet-0.1.7/src/pyquet/common.py
+-rw-rw-rw-   0        0        0     1867 2023-06-11 09:50:23.000000 pyquet-0.1.7/src/pyquet/editor.py
+-rw-rw-rw-   0        0        0     3073 2023-06-12 21:03:03.000000 pyquet-0.1.7/src/pyquet/editor_ui.py
+-rw-rw-rw-   0        0        0     6599 2023-06-11 09:50:23.000000 pyquet-0.1.7/src/pyquet/generator.py
+-rw-rw-rw-   0        0        0     2176 2023-05-27 09:33:39.000000 pyquet-0.1.7/src/pyquet/schemas.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:04:37.069299 pyquet-0.1.7/src/pyquet.egg-info/
+-rw-rw-rw-   0        0        0      546 2023-06-12 21:04:37.000000 pyquet-0.1.7/src/pyquet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-06-12 21:04:37.000000 pyquet-0.1.7/src/pyquet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 21:04:37.000000 pyquet-0.1.7/src/pyquet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-12 21:04:37.000000 pyquet-0.1.7/src/pyquet.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 21:04:37.000000 pyquet-0.1.7/src/pyquet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 21:04:37.000000 pyquet-0.1.7/src/pyquet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 21:04:37.070296 pyquet-0.1.7/tests/
+-rw-rw-rw-   0        0        0     2078 2023-05-27 09:31:42.000000 pyquet-0.1.7/tests/test_reader.py
```

### Comparing `pyquet-0.1.6/LICENSE` & `pyquet-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.6/PKG-INFO` & `pyquet-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.6
+Version: 0.1.7
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.6/setup.cfg` & `pyquet-0.1.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7971 7565 740d 0a76 6572 7369   = pyquet..versi
-00000020: 6f6e 203d 2030 2e31 2e36 0d0a 6175 7468  on = 0.1.6..auth
+00000020: 6f6e 203d 2030 2e31 2e37 0d0a 6175 7468  on = 0.1.7..auth
 00000030: 6f72 203d 2052 6963 6172 646f 204d 7567  or = Ricardo Mug
 00000040: 6963 610d 0a61 7574 686f 725f 656d 6169  ica..author_emai
 00000050: 6c20 3d20 726d 7567 6963 6167 4067 6d61  l = rmugicag@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5465 7874 2063 6f6d 7061  ion = Text compa
 00000080: 7261 746f 7220 5549 0d0a 6c6f 6e67 5f64  rator UI..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
@@ -33,11 +33,16 @@
 00000200: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
 00000210: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
 00000220: 3d33 2e36 0d0a 696e 7374 616c 6c5f 7265  =3.6..install_re
 00000230: 7175 6972 6573 203d 200d 0a09 7061 6e64  quires = ...pand
 00000240: 6173 0d0a 0970 7961 7272 6f77 0d0a 0d0a  as...pyarrow....
 00000250: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
 00000260: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000270: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
-00000280: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000290: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000002a0: 0d0a                                     ..
+00000270: 2073 7263 0d0a 0d0a 5b6f 7074 696f 6e73   src....[options
+00000280: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
+00000290: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
+000002a0: 3d20 0d0a 0970 7971 7565 742d 6564 6974  = ...pyquet-edit
+000002b0: 6f72 203d 2070 7971 7565 742e 6564 6974  or = pyquet.edit
+000002c0: 6f72 5f75 693a 6d61 696e 0d0a 0d0a 5b65  or_ui:main....[e
+000002d0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000002e0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000002f0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `pyquet-0.1.6/src/pyquet/common.py` & `pyquet-0.1.7/src/pyquet/common.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.6/src/pyquet/editor.py` & `pyquet-0.1.7/src/pyquet/editor.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.6/src/pyquet/editor_ui.py` & `pyquet-0.1.7/src/pyquet/editor_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.table.load_csv()
         self.table.redraw()
 
     def save_csv(self):
         self.table.save_csv()
 
 
-if __name__ == "__main__":
+def main():
     root = tk.Tk()
 
     table_frame = tk.Frame(root)
     table_frame.pack(fill=tk.BOTH, expand=True)
 
     table = CustomTable(table_frame)
     table.show()
```

### Comparing `pyquet-0.1.6/src/pyquet/generator.py` & `pyquet-0.1.7/src/pyquet/generator.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.6/src/pyquet/schemas.py` & `pyquet-0.1.7/src/pyquet/schemas.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.6/src/pyquet.egg-info/PKG-INFO` & `pyquet-0.1.7/src/pyquet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.6
+Version: 0.1.7
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.6/tests/test_reader.py` & `pyquet-0.1.7/tests/test_reader.py`

 * *Files identical despite different names*

