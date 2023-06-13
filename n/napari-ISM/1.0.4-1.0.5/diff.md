# Comparing `tmp/napari-ISM-1.0.4.tar.gz` & `tmp/napari-ISM-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-ISM-1.0.4.tar", last modified: Mon Feb 13 13:54:07 2023, max compression
+gzip compressed data, was "napari-ISM-1.0.5.tar", last modified: Tue Jun 13 18:02:32 2023, max compression
```

## Comparing `napari-ISM-1.0.4.tar` & `napari-ISM-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 13:54:07.955379 napari-ISM-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-02-06 08:34:28.000000 napari-ISM-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      101 2023-01-24 15:53:43.000000 napari-ISM-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6683 2023-02-13 13:54:07.955379 napari-ISM-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5791 2023-02-07 12:50:54.000000 napari-ISM-1.0.4/README.md
--rw-rw-rw-   0        0        0      986 2023-02-13 13:05:30.000000 napari-ISM-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1637 2023-02-13 13:54:07.961359 napari-ISM-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 napari-ISM-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-13 13:54:07.870587 napari-ISM-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-02-13 13:54:07.899526 napari-ISM-1.0.4/src/napari_ISM.egg-info/
--rw-rw-rw-   0        0        0     6683 2023-02-13 13:54:07.000000 napari-ISM-1.0.4/src/napari_ISM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      873 2023-02-13 13:54:07.000000 napari-ISM-1.0.4/src/napari_ISM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 13:54:07.000000 napari-ISM-1.0.4/src/napari_ISM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-02-13 13:54:07.000000 napari-ISM-1.0.4/src/napari_ISM.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2023-02-13 13:54:07.000000 napari-ISM-1.0.4/src/napari_ISM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-13 13:54:07.000000 napari-ISM-1.0.4/src/napari_ISM.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-13 13:54:07.928449 napari-ISM-1.0.4/src/napari_ism/
--rw-rw-rw-   0        0        0      171 2023-01-24 15:53:43.000000 napari-ISM-1.0.4/src/napari_ism/__init__.py
--rw-rw-rw-   0        0        0     4213 2023-02-10 11:00:26.000000 napari-ISM-1.0.4/src/napari_ism/_reader.py
--rw-rw-rw-   0        0        0     2289 2023-02-06 08:34:28.000000 napari-ISM-1.0.4/src/napari_ism/_sample_data.py
-drwxrwxrwx   0        0        0        0 2023-02-13 13:54:07.954377 napari-ISM-1.0.4/src/napari_ism/_tests/
--rw-rw-rw-   0        0        0        0 2023-01-24 15:53:43.000000 napari-ISM-1.0.4/src/napari_ism/_tests/__init__.py
--rw-rw-rw-   0        0        0     1001 2023-01-24 15:53:43.000000 napari-ISM-1.0.4/src/napari_ism/_tests/test_reader.py
--rw-rw-rw-   0        0        0      108 2023-01-24 15:53:43.000000 napari-ISM-1.0.4/src/napari_ism/_tests/test_sample_data.py
--rw-rw-rw-   0        0        0     1275 2023-01-24 15:53:43.000000 napari-ISM-1.0.4/src/napari_ism/_tests/test_widget.py
--rw-rw-rw-   0        0        0      126 2023-01-24 15:53:43.000000 napari-ISM-1.0.4/src/napari_ism/_tests/test_writer.py
--rw-rw-rw-   0        0        0     6238 2023-02-06 08:34:28.000000 napari-ISM-1.0.4/src/napari_ism/_widget.py
--rw-rw-rw-   0        0        0      937 2023-01-24 15:53:43.000000 napari-ISM-1.0.4/src/napari_ism/_writer.py
--rw-rw-rw-   0        0        0     2569 2023-02-13 13:48:55.000000 napari-ISM-1.0.4/src/napari_ism/napari.yaml
+drwxrwxrwx   0        0        0        0 2023-06-13 18:02:32.117714 napari-ISM-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-02-06 08:34:28.000000 napari-ISM-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-01-24 15:53:43.000000 napari-ISM-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6691 2023-06-13 18:02:32.117714 napari-ISM-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5799 2023-06-10 14:23:20.000000 napari-ISM-1.0.5/README.md
+-rw-rw-rw-   0        0        0     1004 2023-06-13 17:58:32.000000 napari-ISM-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1652 2023-06-13 18:02:32.118710 napari-ISM-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 napari-ISM-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:02:32.098759 napari-ISM-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 18:02:32.110726 napari-ISM-1.0.5/src/napari_ISM.egg-info/
+-rw-rw-rw-   0        0        0     6691 2023-06-13 18:02:32.000000 napari-ISM-1.0.5/src/napari_ISM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-06-13 18:02:32.000000 napari-ISM-1.0.5/src/napari_ISM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:02:32.000000 napari-ISM-1.0.5/src/napari_ISM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-13 18:02:32.000000 napari-ISM-1.0.5/src/napari_ISM.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      101 2023-06-13 18:02:32.000000 napari-ISM-1.0.5/src/napari_ISM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 18:02:32.000000 napari-ISM-1.0.5/src/napari_ISM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 18:02:32.115719 napari-ISM-1.0.5/src/napari_ism/
+-rw-rw-rw-   0        0        0      171 2023-01-24 15:53:43.000000 napari-ISM-1.0.5/src/napari_ism/__init__.py
+-rw-rw-rw-   0        0        0     3938 2023-06-10 14:26:37.000000 napari-ISM-1.0.5/src/napari_ism/_reader.py
+-rw-rw-rw-   0        0        0     2088 2023-06-13 17:26:00.000000 napari-ISM-1.0.5/src/napari_ism/_sample_data.py
+-rw-rw-rw-   0        0        0     7270 2023-06-13 17:36:43.000000 napari-ISM-1.0.5/src/napari_ism/_widget.py
+-rw-rw-rw-   0        0        0      715 2023-06-10 14:26:37.000000 napari-ISM-1.0.5/src/napari_ism/_writer.py
+-rw-rw-rw-   0        0        0     2891 2023-06-13 17:34:10.000000 napari-ISM-1.0.5/src/napari_ism/napari.yaml
```

### Comparing `napari-ISM-1.0.4/LICENSE` & `napari-ISM-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-ISM-1.0.4/PKG-INFO` & `napari-ISM-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-ISM
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Napari plugin for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/napari-ISM
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/napari-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Framework :: napari
@@ -27,15 +27,15 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-ISM.svg?color=green)](https://python.org)
 
 
 This plugin is built upon the python package [BrightEyes-ISM]. Napari-ISM enables the simulation, loading, and analysis of ISM datasets.
 More in detail, it performs:
 
 * Loading and compression of .h5 files generated by the [MCS software].
-* Simulation of a relistic dataset of tubulin filaments.
+* Simulation of a realistic dataset of tubulin filaments.
 * Simulation of realistic ISM Point Spread Functions.
 * Summing over the detector array dimension
 * Adaptive Pixel Reassignment
 * Multi-image deconvolution
 * Focus-ISM
 
 ----------------------------------
@@ -57,15 +57,15 @@
 or by using [napari hub].
 
 It requires the following Python packages
 
     numpy
     scipy
     h5py
-    brighteyes-ism
+    brighteyes-ism>=1.2.0
 
 ## Documentation
 
 To generate a simulated dataset, go to `File > Open Sample > ISM dataset`. 
 
 ![](https://github.com/VicidominiLab/napari-ISM/raw/main/docs/sample.png)
```

### Comparing `napari-ISM-1.0.4/README.md` & `napari-ISM-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-ISM.svg?color=green)](https://python.org)
 
 
 This plugin is built upon the python package [BrightEyes-ISM]. Napari-ISM enables the simulation, loading, and analysis of ISM datasets.
 More in detail, it performs:
 
 * Loading and compression of .h5 files generated by the [MCS software].
-* Simulation of a relistic dataset of tubulin filaments.
+* Simulation of a realistic dataset of tubulin filaments.
 * Simulation of realistic ISM Point Spread Functions.
 * Summing over the detector array dimension
 * Adaptive Pixel Reassignment
 * Multi-image deconvolution
 * Focus-ISM
 
 ----------------------------------
@@ -36,15 +36,15 @@
 or by using [napari hub].
 
 It requires the following Python packages
 
     numpy
     scipy
     h5py
-    brighteyes-ism
+    brighteyes-ism>=1.2.0
 
 ## Documentation
 
 To generate a simulated dataset, go to `File > Open Sample > ISM dataset`. 
 
 ![](https://github.com/VicidominiLab/napari-ISM/raw/main/docs/sample.png)
```

### Comparing `napari-ISM-1.0.4/pyproject.toml` & `napari-ISM-1.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools", "wheel", "h5py", "brighteyes-ism"]
+requires = ["setuptools", "wheel", "h5py", "PyQt5", "brighteyes-ism >= 1.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "napari-ISM"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Alessandro Zunino", email="alessandro.zunino@iit.it" },
 ]
 description = "A Napari plugin for analysing and simulating ISM images"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
```

### Comparing `napari-ISM-1.0.4/setup.cfg` & `napari-ISM-1.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 4953 4d0d 0a76   = napari-ISM..v
-00000020: 6572 7369 6f6e 203d 2031 2e30 2e34 0d0a  ersion = 1.0.4..
+00000020: 6572 7369 6f6e 203d 2031 2e30 2e35 0d0a  ersion = 1.0.5..
 00000030: 6175 7468 6f72 203d 2041 6c65 7373 616e  author = Alessan
 00000040: 6472 6f20 5a75 6e69 6e6f 0d0a 6175 7468  dro Zunino..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6c65 7373  or_email = aless
 00000060: 616e 6472 6f2e 7a75 6e69 6e6f 4069 6974  andro.zunino@iit
 00000070: 2e69 740d 0a75 726c 203d 2068 7474 7073  .it..url = https
 00000080: 3a2f 2f67 6974 6875 622e 636f 6d2f 5669  ://github.com/Vi
 00000090: 6369 646f 6d69 6e69 4c61 622f 6e61 7061  cidominiLab/napa
@@ -67,37 +67,38 @@
 00000420: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
 00000430: 2054 7275 650d 0a70 7974 686f 6e5f 7265   True..python_re
 00000440: 7175 6972 6573 203d 203e 3d33 2e37 0d0a  quires = >=3.7..
 00000450: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
 00000460: 093d 7372 630d 0a69 6e73 7461 6c6c 5f72  .=src..install_r
 00000470: 6571 7569 7265 7320 3d20 0d0a 096e 756d  equires = ...num
 00000480: 7079 0d0a 0973 6369 7079 0d0a 0968 3570  py...scipy...h5p
-00000490: 790d 0a09 6272 6967 6874 6579 6573 2d69  y...brighteyes-i
-000004a0: 736d 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  sm....[options.e
-000004b0: 7874 7261 735f 7265 7175 6972 655d 0d0a  xtras_require]..
-000004c0: 7465 7374 696e 6720 3d20 0d0a 0974 6f78  testing = ...tox
-000004d0: 0d0a 0970 7974 6573 7420 2023 2068 7474  ...pytest  # htt
-000004e0: 7073 3a2f 2f64 6f63 732e 7079 7465 7374  ps://docs.pytest
-000004f0: 2e6f 7267 2f65 6e2f 6c61 7465 7374 2f63  .org/en/latest/c
-00000500: 6f6e 7465 6e74 732e 6874 6d6c 0d0a 0970  ontents.html...p
-00000510: 7974 6573 742d 636f 7620 2023 2068 7474  ytest-cov  # htt
-00000520: 7073 3a2f 2f70 7974 6573 742d 636f 762e  ps://pytest-cov.
-00000530: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00000540: 6e2f 6c61 7465 7374 2f0d 0a09 7079 7465  n/latest/...pyte
-00000550: 7374 2d71 7420 2023 2068 7474 7073 3a2f  st-qt  # https:/
-00000560: 2f70 7974 6573 742d 7174 2e72 6561 6474  /pytest-qt.readt
-00000570: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000580: 6573 742f 0d0a 096e 6170 6172 690d 0a09  est/...napari...
-00000590: 7079 7174 350d 0a0d 0a5b 6f70 7469 6f6e  pyqt5....[option
-000005a0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-000005b0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-000005c0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000005d0: 655f 6461 7461 5d0d 0a2a 203d 202a 2e79  e_data]..* = *.y
-000005e0: 616d 6c0d 0a0d 0a5b 6f70 7469 6f6e 732e  aml....[options.
-000005f0: 656e 7472 795f 706f 696e 7473 5d0d 0a6e  entry_points]..n
-00000600: 6170 6172 692e 6d61 6e69 6665 7374 203d  apari.manifest =
-00000610: 200d 0a09 6e61 7061 7269 2d49 534d 203d   ...napari-ISM =
-00000620: 206e 6170 6172 695f 6973 6d3a 6e61 7061   napari_ism:napa
-00000630: 7269 2e79 616d 6c0d 0a0d 0a5b 6567 675f  ri.yaml....[egg_
-00000640: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000650: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000660: 300d 0a0d 0a                             0....
+00000490: 790d 0a09 5079 5174 350d 0a09 6272 6967  y...PyQt5...brig
+000004a0: 6874 6579 6573 2d69 736d 3e3d 312e 322e  hteyes-ism>=1.2.
+000004b0: 300d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  0....[options.ex
+000004c0: 7472 6173 5f72 6571 7569 7265 5d0d 0a74  tras_require]..t
+000004d0: 6573 7469 6e67 203d 200d 0a09 746f 780d  esting = ...tox.
+000004e0: 0a09 7079 7465 7374 2020 2320 6874 7470  ..pytest  # http
+000004f0: 733a 2f2f 646f 6373 2e70 7974 6573 742e  s://docs.pytest.
+00000500: 6f72 672f 656e 2f6c 6174 6573 742f 636f  org/en/latest/co
+00000510: 6e74 656e 7473 2e68 746d 6c0d 0a09 7079  ntents.html...py
+00000520: 7465 7374 2d63 6f76 2020 2320 6874 7470  test-cov  # http
+00000530: 733a 2f2f 7079 7465 7374 2d63 6f76 2e72  s://pytest-cov.r
+00000540: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000550: 2f6c 6174 6573 742f 0d0a 0970 7974 6573  /latest/...pytes
+00000560: 742d 7174 2020 2320 6874 7470 733a 2f2f  t-qt  # https://
+00000570: 7079 7465 7374 2d71 742e 7265 6164 7468  pytest-qt.readth
+00000580: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00000590: 7374 2f0d 0a09 6e61 7061 7269 0d0a 0970  st/...napari...p
+000005a0: 7971 7435 0d0a 0d0a 5b6f 7074 696f 6e73  yqt5....[options
+000005b0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+000005c0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+000005d0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000005e0: 5f64 6174 615d 0d0a 2a20 3d20 2a2e 7961  _data]..* = *.ya
+000005f0: 6d6c 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  ml....[options.e
+00000600: 6e74 7279 5f70 6f69 6e74 735d 0d0a 6e61  ntry_points]..na
+00000610: 7061 7269 2e6d 616e 6966 6573 7420 3d20  pari.manifest = 
+00000620: 0d0a 096e 6170 6172 692d 4953 4d20 3d20  ...napari-ISM = 
+00000630: 6e61 7061 7269 5f69 736d 3a6e 6170 6172  napari_ism:napar
+00000640: 692e 7961 6d6c 0d0a 0d0a 5b65 6767 5f69  i.yaml....[egg_i
+00000650: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000660: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000670: 0d0a 0d0a                                ....
```

### Comparing `napari-ISM-1.0.4/src/napari_ISM.egg-info/PKG-INFO` & `napari-ISM-1.0.5/src/napari_ISM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-ISM
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Napari plugin for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/napari-ISM
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/napari-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Framework :: napari
@@ -27,15 +27,15 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-ISM.svg?color=green)](https://python.org)
 
 
 This plugin is built upon the python package [BrightEyes-ISM]. Napari-ISM enables the simulation, loading, and analysis of ISM datasets.
 More in detail, it performs:
 
 * Loading and compression of .h5 files generated by the [MCS software].
-* Simulation of a relistic dataset of tubulin filaments.
+* Simulation of a realistic dataset of tubulin filaments.
 * Simulation of realistic ISM Point Spread Functions.
 * Summing over the detector array dimension
 * Adaptive Pixel Reassignment
 * Multi-image deconvolution
 * Focus-ISM
 
 ----------------------------------
@@ -57,15 +57,15 @@
 or by using [napari hub].
 
 It requires the following Python packages
 
     numpy
     scipy
     h5py
-    brighteyes-ism
+    brighteyes-ism>=1.2.0
 
 ## Documentation
 
 To generate a simulated dataset, go to `File > Open Sample > ISM dataset`. 
 
 ![](https://github.com/VicidominiLab/napari-ISM/raw/main/docs/sample.png)
```

### Comparing `napari-ISM-1.0.4/src/napari_ISM.egg-info/SOURCES.txt` & `napari-ISM-1.0.5/src/napari_ISM.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,13 +17,8 @@
 src/napari_ism/_writer.py
 src/napari_ism/napari.yaml
 src/napari_ism.egg-info/PKG-INFO
 src/napari_ism.egg-info/SOURCES.txt
 src/napari_ism.egg-info/dependency_links.txt
 src/napari_ism.egg-info/entry_points.txt
 src/napari_ism.egg-info/requires.txt
-src/napari_ism.egg-info/top_level.txt
-src/napari_ism/_tests/__init__.py
-src/napari_ism/_tests/test_reader.py
-src/napari_ism/_tests/test_sample_data.py
-src/napari_ism/_tests/test_widget.py
-src/napari_ism/_tests/test_writer.py
+src/napari_ism.egg-info/top_level.txt
```

### Comparing `napari-ISM-1.0.4/src/napari_ism/_reader.py` & `napari-ISM-1.0.5/src/napari_ism/_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-"""
-This module is an example of a barebones numpy reader plugin for napari.
-
-It implements the Reader specification, but your plugin may choose to
-implement multiple readers or even other plugin contributions. see:
-https://napari.org/plugins/guides.html?#readers
-"""
 import numpy as np
 import h5py
     
 import brighteyes_ism.dataio.mcs as mcs
 
 def napari_get_reader(path):
     """A basic implementation of a Reader contribution.
```

### Comparing `napari-ISM-1.0.4/src/napari_ism/_sample_data.py` & `napari-ISM-1.0.5/src/napari_ism/_sample_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,69 @@
-"""
-This module is an example of a barebones sample data provider for napari.
-
-It implements the "sample data" specification.
-see: https://napari.org/plugins/guides.html?#sample-data
-
-Replace code below according to your needs.
-"""
-# from __future__ import annotations
-
 import numpy as np
 from numpy.random import poisson
 from scipy.signal import convolve
 
 import brighteyes_ism.simulation.PSF_sim as ism
 import brighteyes_ism.simulation.Tubulin_sim as simTub
 
 
 def make_sample_data():
     """Generates an image"""
-    
-    N = 5 # number of detector elements in each dimension
-    Nx = 201 # number of pixels of the simulation space
-    pxsizex = 25 # pixel size of the simulation space (nm)
-    pxdim = 50e3 # detector element size in real space (nm)
-    pxpitch = 75e3 # detector element pitch in real space (nm)
-    M = 500 # total magnification of the optical system (e.g. 100x objective follewd by 5x telescope)
+
+    grid = ism.GridParameters()
+
+    grid.N = 5 # number of detector elements in each dimension
+    grid.Nx = 201 # number of pixels of the simulation space
+    grid.pxsizex = 25 # pixel size of the simulation space (nm)
+    grid.pxdim = 50e3 # detector element size in real space (nm)
+    grid.pxpitch = 75e3 # detector element pitch in real space (nm)
+    grid.M = 500 # total magnification of the optical system (e.g. 100x objective follewd by 5x telescope)
     
     
     exPar = ism.simSettings()
     exPar.wl = 640 # excitation wavelength (nm)
     exPar.mask_sampl = 31
     
     emPar = exPar.copy()
     emPar.wl = 660 # emission wavelength (nm)
     
     z_shift = 0 #nm
     
     ###
     
-    PSF, detPSF, exPSF = ism.SPAD_PSF_2D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, z_shift=z_shift)
-
-    PSF /= np.max(PSF)
+    PSF, detPSF, exPSF = ism.SPAD_PSF_2D(grid, exPar, emPar, z_shift=z_shift, normalize=True)
 
     ### Generate tubulin
 
     tubulin = simTub.tubSettings()
-    tubulin.xy_pixel_size = pxsizex
-    tubulin.xy_dimension = Nx
-    tubulin.xz_dimension = 1     
+    tubulin.xy_pixel_size = grid.pxsizex
+    tubulin.xy_dimension = grid.Nx
+    tubulin.xz_dimension = 1
     tubulin.z_pixel = 1     
     tubulin.n_filament = 5
-    tubulin.radius_filament = pxsizex*0.6
-    tubulin.intensity_filament = [0.5,0.9]  
+    tubulin.radius_filament = grid.pxsizex*0.6
+    tubulin.intensity_filament = [0.5, 0.9]
     phTub = simTub.functionPhTub(tubulin)
     
-    TubDec = phTub[:,:,0]
-    
+    TubDec = phTub[:, :, 0]
+    flux = 1e4
+    obj = TubDec * flux
+
     # Convolve tubulin with psf
 
     img = np.empty(PSF.shape)
     
-    for n in range(N**2):
-        img[:, :, n] = convolve(TubDec, PSF[:, :, n] ,mode = 'same')
+    for n in range(grid.N**2):
+        img[:, :, n] = convolve(obj, PSF[:, :, n], mode='same')
     
     # Convert to photons and add Poisson noise
-    
-    img *= 1e2
+    img[img < 0] = 0
     img = np.uint16(img)
     img = poisson(img)
     
     # optional kwargs for the corresponding viewer.add_* method
-    scale = (pxsizex, pxsizex, 1)
-    add_kwargs = {'colormap': 'magma', 'scale' : scale}
+    scale = (grid.pxsizex, grid.pxsizex, 1)
+    add_kwargs = {'colormap': 'magma', 'scale': scale}
 
     layer_type = "image"  # optional, default is "image"
     
     return [(img, add_kwargs, layer_type)]
```

### Comparing `napari-ISM-1.0.4/src/napari_ism/_widget.py` & `napari-ISM-1.0.5/src/napari_ism/_widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-"""
-This module is an example of a barebones QWidget plugin for napari
-
-It implements the Widget specification.
-see: https://napari.org/plugins/guides.html?#widgets
-
-Replace code below according to your needs.
-"""
 # import napari
 import numpy as np
+import napari
 
 from brighteyes_ism.analysis.APR_lib import APR
 from brighteyes_ism.analysis.Deconv_lib import MultiImg_RL_FFT
 from brighteyes_ism.analysis.FocusISM_lib import focusISM
 
+from brighteyes_ism.analysis.Graph_lib import PlotShiftVectors, ShowFingerprint
+from brighteyes_ism.analysis.Tools_lib import fingerprint
+
 import brighteyes_ism.simulation.PSF_sim as ism
 
+from matplotlib.backends.backend_qt5agg import FigureCanvas
+from PyQt5 import QtWidgets
+
 # Uses the `autogenerate: true` flag in the plugin manifest
 # to indicate it should be wrapped as a magicgui to autogenerate
 # a widget.
 
 def Focus_ISM(img_layer: "napari.layers.Image", shape_layer: "napari.layers.Shapes", sigma_B_bound = 2, threshold = 25) -> "napari.types.LayerDataTuple":
     
     data = img_layer.data_raw
@@ -132,48 +131,84 @@
     add_kwargs = {'colormap': 'magma', 'scale': scale, 'name': 'PSFs'}
 
     layer_type = "image"  # optional, default is "image"
     
     return [(PSF, add_kwargs, layer_type)]
 
 
+def Fingerprint(img_layer: "napari.layers.Image"):
+
+    viewer = napari.current_viewer()
+    data = img_layer.data_raw
+
+    fig, ax = ShowFingerprint(data)
+
+    canvas = FigureCanvas(fig)
+
+    viewer.window.add_dock_widget(canvas, name='Fingerprint', area='right')
+
+    screen = QtWidgets.QDesktopWidget().screenGeometry()
+    width = screen.width()
+
+    canvas.setMinimumHeight(int(width / 6))
+    canvas.setMinimumWidth(int(width / 6))
+
 def APR_stack(img_layer: "napari.layers.Image", usf = 10, ref = 12) -> "napari.types.LayerDataTuple":
 
     data = img_layer.data_raw
     scale = img_layer.scale
     
     if data.ndim < 4:
         data = np.expand_dims(data, axis=0)
         scalenew = [ scale[0], scale[1] ]
     else:
         scalenew = [ 1, scale[0], scale[1] ]
         
     sz = data.shape
     
-    data2 = np.empty( sz )
+    data2 = np.empty(sz)
+    shifts = np.empty( [sz[0], sz[-1], 2] )
     
     for n in range(sz[0]):
-        data2[n,:,:,:] = APR(data[n,:,:,:], usf, ref)[1]
-    
-    data_apr = np.squeeze( np.sum(data2, axis = -1) )
-    
-    data_apr[data_apr<0] = 0
-    
+        shifts[n], data2[n] = APR(data[n], usf, ref)
+
+    shifts = np.squeeze(shifts)
+    data_apr = np.squeeze(data2.sum(axis=-1))
+    data_apr[data_apr < 0] = 0
+
+    # Plot shift vectors
+
+    if sz[0] < 2:
+        viewer = napari.current_viewer()
+
+        fing = fingerprint(data)
+        fig, ax = PlotShiftVectors( shifts, color = fing )
+
+        canvas = FigureCanvas(fig)
+
+        viewer.window.add_dock_widget(canvas, name='Shift Vectors', area='right')
+
+        screen = QtWidgets.QDesktopWidget().screenGeometry()
+        width = screen.width()
+
+        canvas.setMinimumHeight(int(width/6))
+        canvas.setMinimumWidth(int(width/6))
+
     # replicate results to match input dimensions
     
     result = np.expand_dims(data_apr, axis = -1)
     result = np.repeat(result, sz[-1], axis = -1)
     scalenew.append(1)
     
     # create layer
     
     add_kwargs = {'colormap': 'magma', 'scale': scalenew, 'name': 'APR'}
 
     layer_type = "image"  # optional, default is "image"
-    
+
     return [(result, add_kwargs, layer_type)]
 
 
 def SumSPAD(img_layer: "napari.layers.Image") -> "napari.types.LayerDataTuple":
     
     data = img_layer.data_raw
     scale = img_layer.scale
```

### Comparing `napari-ISM-1.0.4/src/napari_ism/napari.yaml` & `napari-ISM-1.0.5/src/napari_ism/napari.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -12,30 +12,33 @@
       python_name: napari_ism._writer:write_single_image
       title: Save image data with Adaptive Pixel Reassignment
     - id: napari-ISM.make_sample_data
       python_name: napari_ism._sample_data:make_sample_data
       title: Load sample data from Adaptive Pixel Reassignment 
     - id: napari-ISM.APR_stack
       python_name: napari_ism._widget:APR_stack
-      title: Make example function widget
+      title: Calculate adaptive pixel reassignment on a single dataset or a z-stack
+    - id: napari-ISM.Fingerprint
+      python_name: napari_ism._widget:Fingerprint
+      title: Calculate the fingeprint of a dataset
     - id: napari-ISM.SumSPAD
       python_name: napari_ism._widget:SumSPAD
-      title: Make example function widget
+      title: Generate an image by summing all the channels
     - id: napari-ISM.MultiImgDeconvolution
       python_name: napari_ism._widget:MultiImgDeconvolution
-      title: Make example function widget
+      title: Perform multi-image deconvolution
     - id: napari-ISM.SimulatePSFs
       python_name: napari_ism._widget:SimulatePSFs
-      title: Make example function widget
+      title: Simulate a dataset of PSFs
     - id: napari-ISM.integrateDims
       python_name: napari_ism._widget:integrateDims
-      title: Make example function widget
+      title: Sum the dataset along the specified dimensions
     - id: napari-ISM.Focus_ISM
       python_name: napari_ism._widget:Focus_ISM
-      title: Make example function widget
+      title: Apply focus-ISM on a single dataset
   readers:
     - command: napari-ISM.get_reader
       accepts_directories: false
       filename_patterns: ['*.npy', '*.h5'] 
   writers:
     - command: napari-ISM.write_multiple
       layer_types: ['image*','labels*']
@@ -47,14 +50,17 @@
     - command: napari-ISM.make_sample_data
       display_name: ISM dataset
       key: unique_id.1 
   widgets:
     - command: napari-ISM.APR_stack
       autogenerate: true
       display_name: APR_stack
+    - command: napari-ISM.Fingerprint
+      autogenerate: true
+      display_name: Fingerprint
     - command: napari-ISM.SumSPAD
       autogenerate: true
       display_name: Sum
     - command: napari-ISM.MultiImgDeconvolution
       autogenerate: true
       display_name: Deconvolution
     - command: napari-ISM.SimulatePSFs
```

