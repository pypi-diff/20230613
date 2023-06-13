# Comparing `tmp/fast_captcha-0.2.0.tar.gz` & `tmp/fast_captcha-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_captcha-0.2.0.tar", max compression
+gzip compressed data, was "fast_captcha-0.2.1.tar", max compression
```

## Comparing `fast_captcha-0.2.0.tar` & `fast_captcha-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      284 2023-06-09 06:40:13.831760 fast_captcha-0.2.0/fast_captcha/__init__.py
--rw-r--r--   0        0        0   142224 2023-06-09 04:25:41.492202 fast_captcha-0.2.0/fast_captcha/fonts/3Dumb.ttf
--rw-r--r--   0        0        0    34944 2023-06-09 04:25:41.521475 fast_captcha-0.2.0/fast_captcha/fonts/actionj.ttf
--rw-r--r--   0        0        0    62080 2023-06-09 04:25:41.493203 fast_captcha-0.2.0/fast_captcha/fonts/ApothecaryFont.ttf
--rw-r--r--   0        0        0   472660 2023-06-09 04:25:41.496444 fast_captcha-0.2.0/fast_captcha/fonts/BY-Easy-love-2.ttf
--rw-r--r--   0        0        0    32800 2023-06-09 04:25:41.496957 fast_captcha-0.2.0/fast_captcha/fonts/D3Parallelism.ttf
--rw-r--r--   0        0        0    83188 2023-06-09 04:25:41.497471 fast_captcha-0.2.0/fast_captcha/fonts/DENNEthree-dee.ttf
--rw-r--r--   0        0        0   283156 2023-06-09 04:25:41.507475 fast_captcha-0.2.0/fast_captcha/fonts/Esquisito.ttf
--rw-r--r--   0        0        0   140576 2023-06-09 04:25:41.508476 fast_captcha-0.2.0/fast_captcha/fonts/Flim-Flam.ttf
--rw-r--r--   0        0        0    29368 2023-06-09 04:25:41.509475 fast_captcha-0.2.0/fast_captcha/fonts/Frizon.ttf
--rw-r--r--   0        0        0    69292 2023-06-09 04:25:41.509475 fast_captcha-0.2.0/fast_captcha/fonts/KREMLINGEORGIANI3D.ttf
--rw-r--r--   0        0        0   935888 2023-06-09 04:25:41.516475 fast_captcha-0.2.0/fast_captcha/fonts/Maler.ttf
--rw-r--r--   0        0        0   427596 2023-06-09 04:25:41.519475 fast_captcha-0.2.0/fast_captcha/fonts/MoonRocks.ttf
--rw-r--r--   0        0        0    69896 2023-06-09 04:25:41.520475 fast_captcha-0.2.0/fast_captcha/fonts/Shojumaru.ttf
--rw-r--r--   0        0        0     3418 2023-06-09 07:09:31.572554 fast_captcha-0.2.0/fast_captcha/img_captcha.py
--rw-r--r--   0        0        0      303 2023-06-09 05:21:49.915846 fast_captcha-0.2.0/fast_captcha/text_captcha.py
--rw-r--r--   0        0        0     1084 2023-06-09 04:25:41.480203 fast_captcha-0.2.0/LICENSE
--rw-r--r--   0        0        0     1160 2023-06-09 06:59:39.686082 fast_captcha-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2205 2023-06-09 04:25:41.480203 fast_captcha-0.2.0/README.MD
--rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fast_captcha-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-06-13 11:42:04.471452 fast_captcha-0.2.1/fast_captcha/__init__.py
+-rw-r--r--   0        0        0   142224 2023-06-13 10:47:51.100045 fast_captcha-0.2.1/fast_captcha/fonts/3Dumb.ttf
+-rw-r--r--   0        0        0    34944 2023-06-13 10:47:51.121552 fast_captcha-0.2.1/fast_captcha/fonts/actionj.ttf
+-rw-r--r--   0        0        0    62080 2023-06-13 10:47:51.101044 fast_captcha-0.2.1/fast_captcha/fonts/ApothecaryFont.ttf
+-rw-r--r--   0        0        0   472660 2023-06-13 10:47:51.103551 fast_captcha-0.2.1/fast_captcha/fonts/BY-Easy-love-2.ttf
+-rw-r--r--   0        0        0    32800 2023-06-13 10:47:51.104551 fast_captcha-0.2.1/fast_captcha/fonts/D3Parallelism.ttf
+-rw-r--r--   0        0        0    83188 2023-06-13 10:47:51.105551 fast_captcha-0.2.1/fast_captcha/fonts/DENNEthree-dee.ttf
+-rw-r--r--   0        0        0   283156 2023-06-13 10:47:51.107551 fast_captcha-0.2.1/fast_captcha/fonts/Esquisito.ttf
+-rw-r--r--   0        0        0   140576 2023-06-13 10:47:51.109551 fast_captcha-0.2.1/fast_captcha/fonts/Flim-Flam.ttf
+-rw-r--r--   0        0        0    29368 2023-06-13 10:47:51.110551 fast_captcha-0.2.1/fast_captcha/fonts/Frizon.ttf
+-rw-r--r--   0        0        0    69292 2023-06-13 10:47:51.110551 fast_captcha-0.2.1/fast_captcha/fonts/KREMLINGEORGIANI3D.ttf
+-rw-r--r--   0        0        0   935888 2023-06-13 10:47:51.117552 fast_captcha-0.2.1/fast_captcha/fonts/Maler.ttf
+-rw-r--r--   0        0        0   427596 2023-06-13 10:47:51.120551 fast_captcha-0.2.1/fast_captcha/fonts/MoonRocks.ttf
+-rw-r--r--   0        0        0    69896 2023-06-13 10:47:51.121552 fast_captcha-0.2.1/fast_captcha/fonts/Shojumaru.ttf
+-rw-r--r--   0        0        0     3417 2023-06-13 11:42:04.472453 fast_captcha-0.2.1/fast_captcha/img_captcha.py
+-rw-r--r--   0        0        0      303 2023-06-13 10:47:51.122552 fast_captcha-0.2.1/fast_captcha/text_captcha.py
+-rw-r--r--   0        0        0     1084 2023-06-13 10:47:51.091044 fast_captcha-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1141 2023-06-13 11:42:04.472453 fast_captcha-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2205 2023-06-13 10:47:51.091044 fast_captcha-0.2.1/README.MD
+-rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 fast_captcha-0.2.1/PKG-INFO
```

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/3Dumb.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/3Dumb.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/actionj.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/actionj.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/ApothecaryFont.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/ApothecaryFont.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/BY-Easy-love-2.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/BY-Easy-love-2.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/D3Parallelism.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/D3Parallelism.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/DENNEthree-dee.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/DENNEthree-dee.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/Esquisito.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/Esquisito.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/Flim-Flam.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/Flim-Flam.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/Frizon.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/Frizon.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/KREMLINGEORGIANI3D.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/KREMLINGEORGIANI3D.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/Maler.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/Maler.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/MoonRocks.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/MoonRocks.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/fonts/Shojumaru.ttf` & `fast_captcha-0.2.1/fast_captcha/fonts/Shojumaru.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/fast_captcha/img_captcha.py` & `fast_captcha-0.2.1/fast_captcha/img_captcha.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import random
 from io import BytesIO
 from pathlib import Path
-from typing import Tuple, Literal
+from typing import Literal
 
 from PIL import Image, ImageDraw, ImageFont
 
 from fast_captcha import text_captcha
 
 
-def use_rgb() -> Tuple[int, ...]:
+def use_rgb() -> tuple[int, ...]:
     """
     random colors for captcha text and distractions
 
     :return:
     """
     return tuple((random.randint(0, 255) for _ in range(3)))
 
@@ -40,15 +40,15 @@
     font_type: str = random.choice(get_ttf()),
     font_size: int = 32,
     draw_lines: bool = True,
     lines_num: int = 4,
     draw_points: bool = False,
     points_density: int = 4,
     img_type: str = 'jpeg',
-    img_byte: Literal['file', 'bytesio', 'base64'] = 'bytesio',
+    img_byte: str | Literal['file', 'bytesio', 'base64'] = 'bytesio',
 ) -> tuple[Image.Image | BytesIO | bytes, str]:
     """
     img captcha
 
     :param code_num: number of codes.
     :param width: picture width, default 120.
     :param height: picture height, default 40.
```

### Comparing `fast_captcha-0.2.0/LICENSE` & `fast_captcha-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/pyproject.toml` & `fast_captcha-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast_captcha"
-version = "0.2.0"
+version = "0.2.1"
 description = "Fast to use captcha"
 authors = ["wu <jianhengwu0407@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/wu-clan/fast_captcha"
 repository = "https://github.com/wu-clan/fast_captcha"
 classifiers = [
@@ -19,15 +19,14 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 Pillow = "^9.2.0"
-pytest = "^7.3.1"
 
 [tool.poetry.dev-dependencies]
 pytest = '^7.0.0'
 
 [tool.ruff]
 line-length = 120
 cache-dir = "./.ruff_cache"
```

### Comparing `fast_captcha-0.2.0/README.MD` & `fast_captcha-0.2.1/README.MD`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.2.0/PKG-INFO` & `fast_captcha-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-captcha
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fast to use captcha
 Home-page: https://github.com/wu-clan/fast_captcha
 License: MIT
 Author: wu
 Author-email: jianhengwu0407@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Project-URL: Repository, https://github.com/wu-clan/fast_captcha
 Description-Content-Type: text/markdown
 
 # fast_captcha
 
 fast to use captcha
```

