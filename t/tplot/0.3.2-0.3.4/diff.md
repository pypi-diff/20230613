# Comparing `tmp/tplot-0.3.2.tar.gz` & `tmp/tplot-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tplot-0.3.2.tar", max compression
+gzip compressed data, was "tplot-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tplot-0.3.2.tar` & `tplot-0.3.4.tar`

### file list

```diff
@@ -1,11 +1,81 @@
--rw-r--r--   0        0        0     1077 2020-07-25 10:52:30.985551 tplot-0.3.2/LICENSE
--rw-r--r--   0        0        0     2377 2022-01-16 16:56:10.984484 tplot-0.3.2/README.md
--rw-r--r--   0        0        0      830 2022-01-30 08:47:52.202211 tplot-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      216 2022-01-14 14:28:17.106225 tplot-0.3.2/tplot/__init__.py
--rw-r--r--   0        0        0     2536 2022-01-14 14:28:17.106225 tplot-0.3.2/tplot/braille.py
--rw-r--r--   0        0        0    21796 2022-01-14 14:28:17.106225 tplot-0.3.2/tplot/figure.py
--rw-r--r--   0        0        0     1267 2022-01-14 14:28:17.106225 tplot-0.3.2/tplot/img2ascii.py
--rw-r--r--   0        0        0     2214 2022-01-14 14:28:17.106225 tplot-0.3.2/tplot/scales.py
--rw-r--r--   0        0        0     5649 2022-01-16 17:02:45.837829 tplot-0.3.2/tplot/utils.py
--rw-r--r--   0        0        0     3325 2022-01-30 08:49:16.700572 tplot-0.3.2/setup.py
--rw-r--r--   0        0        0     3277 2022-01-30 08:49:16.700975 tplot-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2023-06-05 11:50:47.676503 tplot-0.3.4/.flake8
+-rw-r--r--   0        0        0      714 2023-06-13 18:34:25.958207 tplot-0.3.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     2051 2023-06-05 11:50:47.676503 tplot-0.3.4/.gitignore
+-rw-r--r--   0        0        0      520 2023-06-13 18:34:25.958207 tplot-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1077 2023-06-13 18:34:25.958207 tplot-0.3.4/LICENSE.txt
+-rw-r--r--   0        0        0     2377 2023-06-05 11:50:47.676503 tplot-0.3.4/README.md
+-rw-r--r--   0        0        0      696 2023-06-13 18:38:21.268842 tplot-0.3.4/development_notes.md
+-rw-r--r--   0        0        0      634 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/Makefile
+-rw-r--r--   0        0        0     2013 2023-06-13 18:34:25.962206 tplot-0.3.4/docs/conf.py
+-rw-r--r--   0        0        0    27486 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/advanced.png
+-rw-r--r--   0        0        0    15547 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/basic.png
+-rw-r--r--   0        0        0    15231 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/braille.png
+-rw-r--r--   0        0        0    38654 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/cameraman.png
+-rw-r--r--   0        0        0    18496 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/cameraman_blocks.png
+-rw-r--r--   0        0        0    15962 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/categorical.png
+-rw-r--r--   0        0        0    12103 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/misalignment.png
+-rw-r--r--   0        0        0    27950 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/multivariate_gaussian_ascii.png
+-rw-r--r--   0        0        0    16199 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/multivariate_gaussian_block.png
+-rw-r--r--   0        0        0    11831 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/spamspamspamspam.png
+-rw-r--r--   0        0        0    15273 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/images/twinkle_twinkle_little_star.png
+-rw-r--r--   0        0        0    11508 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/make.bat
+-rw-r--r--   0        0        0       30 2023-06-05 11:50:47.676503 tplot-0.3.4/docs/requirements.txt
+-rw-r--r--   0        0        0     1231 2023-06-13 18:53:28.881623 tplot-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-06-05 11:50:47.676503 tplot-0.3.4/readthedocs.yml
+-rw-r--r--   0        0        0        0 2023-06-13 18:34:25.962206 tplot-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0    38654 2023-06-05 11:50:47.676503 tplot-0.3.4/tests/cameraman.png
+-rw-r--r--   0        0        0     3579 2023-06-05 11:50:47.676503 tplot-0.3.4/tests/reference_figures/axis_labels.txt
+-rw-r--r--   0        0        0     2381 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/bar_anscombe.txt
+-rw-r--r--   0        0        0     2199 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/bar_cheese_or_chocolate.txt
+-rw-r--r--   0        0        0     2315 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/bar_iris.txt
+-rw-r--r--   0        0        0     3470 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_bar_anscombe.txt
+-rw-r--r--   0        0        0     2532 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_bar_cheese_or_chocolate.txt
+-rw-r--r--   0        0        0     3206 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_bar_iris.txt
+-rw-r--r--   0        0        0     2903 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_hbar_anscombe.txt
+-rw-r--r--   0        0        0     2549 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_hbar_cheese_or_chocolate.txt
+-rw-r--r--   0        0        0     2391 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_hbar_iris.txt
+-rw-r--r--   0        0        0     3360 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_line_anscombe.txt
+-rw-r--r--   0        0        0     4622 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_line_cheese_or_chocolate.txt
+-rw-r--r--   0        0        0     3602 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_line_iris.txt
+-rw-r--r--   0        0        0     2260 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_scatter_anscombe.txt
+-rw-r--r--   0        0        0     2180 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_scatter_cheese_or_chocolate.txt
+-rw-r--r--   0        0        0     2216 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/braille_scatter_iris.txt
+-rw-r--r--   0        0        0     2381 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/colors.txt
+-rw-r--r--   0        0        0     2903 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/hbar_anscombe.txt
+-rw-r--r--   0        0        0     2549 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/hbar_cheese_or_chocolate.txt
+-rw-r--r--   0        0        0     2391 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/hbar_iris.txt
+-rw-r--r--   0        0        0     5085 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/image.txt
+-rw-r--r--   0        0        0     2139 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/image_ascii.txt
+-rw-r--r--   0        0        0     4759 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/image_big_values.txt
+-rw-r--r--   0        0        0     4263 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/image_cameraman.txt
+-rw-r--r--   0        0        0     5127 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/image_small_values.txt
+-rw-r--r--   0        0        0     5219 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/image_vmin_vmax.txt
+-rw-r--r--   0        0        0     2331 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/legendloc_bottomleft.txt
+-rw-r--r--   0        0        0     2353 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/legendloc_bottomright.txt
+-rw-r--r--   0        0        0     2353 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/legendloc_topleft.txt
+-rw-r--r--   0        0        0     2353 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/legendloc_topright.txt
+-rw-r--r--   0        0        0     2361 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/line_anscombe.txt
+-rw-r--r--   0        0        0     2579 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/line_cheese_or_chocolate.txt
+-rw-r--r--   0        0        0     2387 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/line_iris.txt
+-rw-r--r--   0        0        0     2161 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/scatter_anscombe.txt
+-rw-r--r--   0        0        0     2135 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/scatter_cheese_or_chocolate.txt
+-rw-r--r--   0        0        0     2135 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/scatter_iris.txt
+-rw-r--r--   0        0        0     2139 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/text.txt
+-rw-r--r--   0        0        0     2161 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/y_axis_down_anscombe.txt
+-rw-r--r--   0        0        0     2135 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/y_axis_down_cheese_or_chocolate.txt
+-rw-r--r--   0        0        0     2135 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/y_axis_down_iris.txt
+-rw-r--r--   0        0        0     5085 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/y_axis_up.txt
+-rw-r--r--   0        0        0     2159 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/reference_figures/y_only.txt
+-rw-r--r--   0        0        0     1595 2023-06-13 18:27:53.120858 tplot-0.3.4/tests/test_braille.py
+-rw-r--r--   0        0        0      692 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/test_img2ascii.py
+-rw-r--r--   0        0        0     5986 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/test_reference_figures.py
+-rw-r--r--   0        0        0     1467 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/test_scales.py
+-rw-r--r--   0        0        0     1438 2023-06-05 11:50:47.680503 tplot-0.3.4/tests/test_xticklabels.py
+-rw-r--r--   0        0        0      136 2023-06-13 18:34:25.962206 tplot-0.3.4/tplot/__init__.py
+-rw-r--r--   0        0        0     2536 2023-06-05 11:50:47.680503 tplot-0.3.4/tplot/braille.py
+-rw-r--r--   0        0        0    21759 2023-06-13 18:34:25.962206 tplot-0.3.4/tplot/figure.py
+-rw-r--r--   0        0        0     1267 2023-06-05 11:50:47.680503 tplot-0.3.4/tplot/img2ascii.py
+-rw-r--r--   0        0        0     2214 2023-06-05 11:50:47.680503 tplot-0.3.4/tplot/scales.py
+-rw-r--r--   0        0        0     5649 2023-06-05 11:50:47.680503 tplot-0.3.4/tplot/utils.py
+-rw-r--r--   0        0        0     3795 1970-01-01 00:00:00.000000 tplot-0.3.4/PKG-INFO
```

### Comparing `tplot-0.3.2/LICENSE` & `tplot-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tplot-0.3.2/README.md` & `tplot-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `tplot-0.3.2/tplot/braille.py` & `tplot-0.3.4/tplot/braille.py`

 * *Files identical despite different names*

### Comparing `tplot-0.3.2/tplot/figure.py` & `tplot-0.3.4/tplot/figure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from functools import partial
+from functools import cached_property, partial
 from numbers import Number
 from shutil import get_terminal_size
 from typing import Callable, Iterable, List, Optional, Tuple
 
 import numpy as np
-from backports.cached_property import cached_property
 from colorama import init
 from termcolor import colored
 
 from . import utils
 from .braille import draw_braille, is_braille
 from .img2ascii import img2ascii
 from .scales import CategoricalScale, LinearScale
```

### Comparing `tplot-0.3.2/tplot/img2ascii.py` & `tplot-0.3.4/tplot/img2ascii.py`

 * *Files identical despite different names*

### Comparing `tplot-0.3.2/tplot/scales.py` & `tplot-0.3.4/tplot/scales.py`

 * *Files identical despite different names*

### Comparing `tplot-0.3.2/tplot/utils.py` & `tplot-0.3.4/tplot/utils.py`

 * *Files identical despite different names*

### Comparing `tplot-0.3.2/PKG-INFO` & `tplot-0.3.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: tplot
-Version: 0.3.2
+Version: 0.3.4
 Summary: Create text-based graphs
-Home-page: https://github.com/JeroenDelcour/tplot
-License: MIT
-Author: Jeroen Delcour
-Author-email: jeroendelcour@gmail.com
-Requires-Python: >=3.6.2,<4.0.0
+Author-email: Jeroen Delcour <jeroendelcour@gmail.com>
+Requires-Python: >=3.8,<4
+Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: backports.cached-property (>=1.0.1,<2.0.0)
-Requires-Dist: colorama (>=0.4.3,<0.5.0)
-Requires-Dist: importlib-metadata (>=3.1.0,<4.0.0); python_version < "3.8"
-Requires-Dist: numpy (>=1.11,<2.0)
-Requires-Dist: termcolor-whl (>=1.1.0,<2.0.0)
-Project-URL: Repository, https://github.com/JeroenDelcour/tplot
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: colorama >=0.4.3
+Requires-Dist: numpy >=1.11
+Requires-Dist: termcolor-whl >=1.1.0
+Requires-Dist: flit >=3.9.0 ; extra == "dev"
+Requires-Dist: pytest >=7.3.2 ; extra == "dev"
+Requires-Dist: pytest-cov >=4.1.0 ; extra == "dev"
+Requires-Dist: coverage >=6.2 ; extra == "dev"
+Requires-Dist: black >=23.0.0 ; extra == "dev"
+Requires-Dist: isort >=5.12.0 ; extra == "dev"
+Requires-Dist: flake8 >=4.0.1 ; extra == "dev"
+Requires-Dist: pillow >=8.3.2 ; extra == "dev"
+Requires-Dist: pre-commit >=2.16.0 ; extra == "dev"
+Requires-Dist: mypy >=0.931 ; extra == "dev"
+Requires-Dist: Sphinx >=4.3.2 ; extra == "dev"
+Requires-Dist: sphinx-rtd-theme >=1.0.0 ; extra == "dev"
+Project-URL: Documentation, https://tplot.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/JeroenDelcour/tplot
+Provides-Extra: dev
 
 # tplot
 
 [![Documentation status](https://readthedocs.org/projects/tplot/badge/)](https://tplot.readthedocs.io/en/latest/)
 [![Tests status](https://github.com/JeroenDelcour/tplot/actions/workflows/tests.yml/badge.svg)](https://github.com/JeroenDelcour/tplot/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/JeroenDelcour/tplot/branch/master/graph/badge.svg?token=WXH7I3BGEO)](https://codecov.io/gh/JeroenDelcour/tplot)
```

