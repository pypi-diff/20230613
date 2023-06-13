# Comparing `tmp/jsoneng-1.0.2.1.tar.gz` & `tmp/jsoneng-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsoneng-1.0.2.1.tar", last modified: Sat Sep 17 03:18:18 2022, max compression
+gzip compressed data, was "jsoneng-1.0.5.tar", last modified: Tue Jun 13 18:43:56 2023, max compression
```

## Comparing `jsoneng-1.0.2.1.tar` & `jsoneng-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-09-17 03:18:18.661636 jsoneng-1.0.2.1/
--rw-rw-rw-   0        0        0     1091 2022-08-28 22:54:26.000000 jsoneng-1.0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2023 2022-09-17 03:18:18.661636 jsoneng-1.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2022-08-28 22:58:18.000000 jsoneng-1.0.2.1/README.md
--rw-rw-rw-   0        0        0      108 2022-08-28 22:24:08.000000 jsoneng-1.0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      684 2022-09-17 03:18:18.667638 jsoneng-1.0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-17 03:18:18.644632 jsoneng-1.0.2.1/src/
-drwxrwxrwx   0        0        0        0 2022-09-17 03:18:18.651634 jsoneng-1.0.2.1/src/jsoneng/
--rw-rw-rw-   0        0        0     3973 2022-09-17 03:16:51.000000 jsoneng-1.0.2.1/src/jsoneng/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-17 03:18:18.661636 jsoneng-1.0.2.1/src/jsoneng.egg-info/
--rw-rw-rw-   0        0        0     2023 2022-09-17 03:18:18.000000 jsoneng-1.0.2.1/src/jsoneng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2022-09-17 03:18:18.000000 jsoneng-1.0.2.1/src/jsoneng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-17 03:18:18.000000 jsoneng-1.0.2.1/src/jsoneng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-09-17 03:18:18.000000 jsoneng-1.0.2.1/src/jsoneng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 18:43:56.380214 jsoneng-1.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-05-13 03:44:08.000000 jsoneng-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2021 2023-06-13 18:43:56.381135 jsoneng-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-05-13 03:44:08.000000 jsoneng-1.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-13 03:44:08.000000 jsoneng-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      682 2023-06-13 18:43:56.381135 jsoneng-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 18:43:56.350785 jsoneng-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 18:43:56.366494 jsoneng-1.0.5/src/jsoneng/
+-rw-rw-rw-   0        0        0     7904 2023-06-13 18:40:04.000000 jsoneng-1.0.5/src/jsoneng/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:43:56.380214 jsoneng-1.0.5/src/jsoneng.egg-info/
+-rw-rw-rw-   0        0        0     2021 2023-06-13 18:43:56.000000 jsoneng-1.0.5/src/jsoneng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-06-13 18:43:56.000000 jsoneng-1.0.5/src/jsoneng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:43:56.000000 jsoneng-1.0.5/src/jsoneng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 18:43:56.000000 jsoneng-1.0.5/src/jsoneng.egg-info/top_level.txt
```

### Comparing `jsoneng-1.0.2.1/LICENSE` & `jsoneng-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsoneng-1.0.2.1/PKG-INFO` & `jsoneng-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoneng
-Version: 1.0.2.1
+Version: 1.0.5
 Summary: A package for a python JSON database CRUD engine
 Home-page: https://github.com/youhengzhou/jsoneng
 Author: YouHeng Zhou
 Author-email: youhengzhou@cmail.carleton.ca
 Project-URL: Bug Tracker, https://github.com/youhengzhou/jsoneng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jsoneng-1.0.2.1/README.md` & `jsoneng-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jsoneng-1.0.2.1/setup.cfg` & `jsoneng-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206a 736f 6e65 6e67 0d0a 7665 7273   = jsoneng..vers
-00000020: 696f 6e20 3d20 312e 302e 322e 310d 0a61  ion = 1.0.2.1..a
-00000030: 7574 686f 7220 3d20 596f 7548 656e 6720  uthor = YouHeng 
-00000040: 5a68 6f75 0d0a 6175 7468 6f72 5f65 6d61  Zhou..author_ema
-00000050: 696c 203d 2079 6f75 6865 6e67 7a68 6f75  il = youhengzhou
-00000060: 4063 6d61 696c 2e63 6172 6c65 746f 6e2e  @cmail.carleton.
-00000070: 6361 0d0a 6465 7363 7269 7074 696f 6e20  ca..description 
-00000080: 3d20 4120 7061 636b 6167 6520 666f 7220  = A package for 
-00000090: 6120 7079 7468 6f6e 204a 534f 4e20 6461  a python JSON da
-000000a0: 7461 6261 7365 2043 5255 4420 656e 6769  tabase CRUD engi
-000000b0: 6e65 0d0a 6c6f 6e67 5f64 6573 6372 6970  ne..long_descrip
-000000c0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-000000d0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-000000e0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-000000f0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000100: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
-00000110: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000120: 796f 7568 656e 677a 686f 752f 6a73 6f6e  youhengzhou/json
-00000130: 656e 670d 0a70 726f 6a65 6374 5f75 726c  eng..project_url
-00000140: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000150: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
-00000160: 6875 622e 636f 6d2f 796f 7568 656e 677a  hub.com/youhengz
-00000170: 686f 752f 6a73 6f6e 656e 672f 6973 7375  hou/jsoneng/issu
-00000180: 6573 0d0a 636c 6173 7369 6669 6572 7320  es..classifiers 
-00000190: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
-000001a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000001b0: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
-000001c0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-000001d0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-000001e0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
-000001f0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000200: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
-00000210: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-00000220: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
-00000230: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
-00000240: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-00000250: 203e 3d33 2e36 0d0a 0d0a 5b6f 7074 696f   >=3.6....[optio
-00000260: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000270: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
-00000280: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000290: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000002a0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000020: 696f 6e20 3d20 312e 302e 350d 0a61 7574  ion = 1.0.5..aut
+00000030: 686f 7220 3d20 596f 7548 656e 6720 5a68  hor = YouHeng Zh
+00000040: 6f75 0d0a 6175 7468 6f72 5f65 6d61 696c  ou..author_email
+00000050: 203d 2079 6f75 6865 6e67 7a68 6f75 4063   = youhengzhou@c
+00000060: 6d61 696c 2e63 6172 6c65 746f 6e2e 6361  mail.carleton.ca
+00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+00000080: 4120 7061 636b 6167 6520 666f 7220 6120  A package for a 
+00000090: 7079 7468 6f6e 204a 534f 4e20 6461 7461  python JSON data
+000000a0: 6261 7365 2043 5255 4420 656e 6769 6e65  base CRUD engine
+000000b0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000c0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+000000d0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
+000000e0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+000000f0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+00000100: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
+00000110: 3a2f 2f67 6974 6875 622e 636f 6d2f 796f  ://github.com/yo
+00000120: 7568 656e 677a 686f 752f 6a73 6f6e 656e  uhengzhou/jsonen
+00000130: 670d 0a70 726f 6a65 6374 5f75 726c 7320  g..project_urls 
+00000140: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
+00000150: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000160: 622e 636f 6d2f 796f 7568 656e 677a 686f  b.com/youhengzho
+00000170: 752f 6a73 6f6e 656e 672f 6973 7375 6573  u/jsoneng/issues
+00000180: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+00000190: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000001a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001b0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
+000001c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001d0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
+000001e0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+000001f0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000200: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
+00000210: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
+00000220: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
+00000230: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+00000240: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000250: 3d33 2e36 0d0a 0d0a 5b6f 7074 696f 6e73  =3.6....[options
+00000260: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+00000270: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+00000280: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000290: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000002a0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `jsoneng-1.0.2.1/src/jsoneng.egg-info/PKG-INFO` & `jsoneng-1.0.5/src/jsoneng.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoneng
-Version: 1.0.2.1
+Version: 1.0.5
 Summary: A package for a python JSON database CRUD engine
 Home-page: https://github.com/youhengzhou/jsoneng
 Author: YouHeng Zhou
 Author-email: youhengzhou@cmail.carleton.ca
 Project-URL: Bug Tracker, https://github.com/youhengzhou/jsoneng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

