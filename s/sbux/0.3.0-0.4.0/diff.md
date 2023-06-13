# Comparing `tmp/sbux-0.3.0.tar.gz` & `tmp/sbux-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbux-0.3.0.tar", max compression
+gzip compressed data, was "sbux-0.4.0.tar", max compression
```

## Comparing `sbux-0.3.0.tar` & `sbux-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2022-12-30 13:48:11.486783 sbux-0.3.0/LICENSE
--rw-r--r--   0        0        0      872 2022-12-30 13:48:11.486783 sbux-0.3.0/README.md
--rw-r--r--   0        0        0     1110 2022-12-30 13:48:39.850603 sbux-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      153 2022-12-30 13:48:39.838603 sbux-0.3.0/src/sbux/__init__.py
--rw-r--r--   0        0        0     1745 2022-12-30 13:48:11.486783 sbux-0.3.0/src/sbux/main.py
--rw-r--r--   0        0        0       88 2022-12-30 13:48:11.486783 sbux-0.3.0/src/sbux/models/__init__.py
--rw-r--r--   0        0        0      581 2022-12-30 13:48:11.486783 sbux-0.3.0/src/sbux/models/base.py
--rw-r--r--   0        0        0     2366 2022-12-30 13:48:11.486783 sbux-0.3.0/src/sbux/models/item.py
--rw-r--r--   0        0        0     1357 2022-12-30 13:48:11.486783 sbux-0.3.0/src/sbux/models/store.py
--rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 sbux-0.3.0/setup.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sbux-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-13 13:43:20.647751 sbux-0.4.0/LICENSE
+-rw-r--r--   0        0        0      907 2023-06-13 13:43:20.647751 sbux-0.4.0/README.md
+-rw-r--r--   0        0        0     1136 2023-06-13 13:44:01.416388 sbux-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-06-13 13:44:01.400388 sbux-0.4.0/src/sbux/__init__.py
+-rw-r--r--   0        0        0     1686 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/main.py
+-rw-r--r--   0        0        0      210 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/models/__init__.py
+-rw-r--r--   0        0        0      581 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/models/base.py
+-rw-r--r--   0        0        0     2279 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/models/item.py
+-rw-r--r--   0        0        0     1199 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/models/store.py
+-rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 sbux-0.4.0/setup.py
+-rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 sbux-0.4.0/PKG-INFO
```

### Comparing `sbux-0.3.0/LICENSE` & `sbux-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sbux-0.3.0/README.md` & `sbux-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,10 +22,12 @@
 
 
 starbucks = Starbucks
 starbucks.get_stores()
 starbucks.get_menu_items(branch_code="13377")
 ```
 
+See more [examples](./examples/).
+
 ## Contributing
 
 For guidance on setting up a development environment and how to make a contribution, see the [contributing guidelines](./docs/CONTRIBUTING.md).
```

### Comparing `sbux-0.3.0/pyproject.toml` & `sbux-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 license = "MIT"
 name = "sbux"
 packages = [
   {include = "sbux", from = "src"},
 ]
 readme = "README.md"
 repository = "https://github.com/ngshiheng/sbux"
-version = "0.3.0"
+version = "0.4.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.1"
 dataclasses-json = "^0.5.7"
+requests-cache = "^1.0.1"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.1"
 black = "^22.12.0"
 flake8 = "^6.0.0"
 isort = "^5.11.4"
 pre-commit = "^2.21.0"
```

### Comparing `sbux-0.3.0/src/sbux/models/base.py` & `sbux-0.4.0/src/sbux/models/base.py`

 * *Files identical despite different names*

### Comparing `sbux-0.3.0/src/sbux/models/item.py` & `sbux-0.4.0/src/sbux/models/item.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,39 +6,41 @@
 from .base import BaseSBUXDataClassJsonMixin
 
 
 @dataclass
 class Modifier(BaseSBUXDataClassJsonMixin):
     """Represents a menu item modifier at Starbucks."""
 
-    item_code: Optional[str]
-    name: Optional[str]
+    item_code: str
+    name: str
     filter_code: Optional[str]
-    unit_price: Optional[int]
-    unit_price_dlvr: Optional[int]
-    sequence: Optional[float]
-    selection_range_min: Optional[int]
-    selection_range_max: Optional[int]
+    unit_price: int
+    unit_price_dlvr: int
+    sequence: float
+    selection_range_min: int
+    selection_range_max: int
     is_fixed_price: bool
     is_free: bool
     is_quantifiable: bool
     is_default: bool
     uom: Optional[str] = field(metadata=config(field_name="UOM"))
     photo_urls: Optional[list[str]] = field(metadata=config(field_name="PhotoURLs"))
+    popup_image: bool
     default_keys: Optional[list[str]]
     default_values: Optional[list[str]]
+    description: Optional[str]
 
 
 @dataclass
 class ModifierGroup(BaseSBUXDataClassJsonMixin):
     """Represents a group of modifiers that can be applied to a menu item at Starbucks."""
 
-    menu_id: Optional[str]
-    name: Optional[str]
-    description: Optional[str]
+    menu_id: str
+    name: str
+    description: str
     photo_urls: Optional[list[str]] = field(metadata=config(field_name="PhotoURLs"))
     sequence: Optional[float]
     selection_range_min: Optional[int]
     selection_range_max: Optional[int]
     is_fixed_price: bool
     is_free: bool
     is_quantifiable: bool
@@ -46,20 +48,20 @@
     modifiers: Optional[list[Modifier]]
 
 
 @dataclass
 class Item(BaseSBUXDataClassJsonMixin):
     """Represents a menu item at Starbucks."""
 
-    item_id: Optional[str]
+    item_id: str
     item_code: Optional[str]
-    name: Optional[str]
+    name: str
     description: Optional[str]
-    base_price: Optional[int]
-    base_price_dlvr: Optional[int]
+    base_price: int
+    base_price_dlvr: int
     photo_urls: Optional[list[str]] = field(metadata=config(field_name="PhotoURLs"))
     sequence: Optional[float]
     modifier_group: Optional[list[ModifierGroup]]
     pmt_no: Optional[str] = field(metadata=config(field_name="PMTNo"))
     pmt_ref_no: Optional[str] = field(metadata=config(field_name="PMTRefNo"))
     pmt_amount: Optional[int] = field(metadata=config(field_name="PMTAmount"))
     pmt_line: Optional[int] = field(metadata=config(field_name="PMTLine"))
```

### Comparing `sbux-0.3.0/setup.py` & `sbux-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 packages = \
 ['sbux', 'sbux.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['dataclasses-json>=0.5.7,<0.6.0', 'requests>=2.28.1,<3.0.0']
+['dataclasses-json>=0.5.7,<0.6.0',
+ 'requests-cache>=1.0.1,<2.0.0',
+ 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'sbux',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'An unofficial Starbucks Singapore (SG) software development kit (SDK).',
-    'long_description': '# sbux\n\n[![CI](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml)\n[![Semantic Release](https://github.com/ngshiheng/sbux/actions/workflows/release.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/release.yml)\n\n`sbux` is an unofficial Starbucks Singapore (SG) software development kit (SDK).\n\n`sbux` is named after the ticker symbol of Starbucks Corporation (SBUX) on the NASDAQ.\n\n## Installing\n\nInstall and update using `pip`;\n\n```sh\npip install sbux\n```\n\n## A Simple Example\n\n```python\nfrom sbux import Starbucks\n\n\nstarbucks = Starbucks\nstarbucks.get_stores()\nstarbucks.get_menu_items(branch_code="13377")\n```\n\n## Contributing\n\nFor guidance on setting up a development environment and how to make a contribution, see the [contributing guidelines](./docs/CONTRIBUTING.md).\n',
+    'long_description': '# sbux\n\n[![CI](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml)\n[![Semantic Release](https://github.com/ngshiheng/sbux/actions/workflows/release.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/release.yml)\n\n`sbux` is an unofficial Starbucks Singapore (SG) software development kit (SDK).\n\n`sbux` is named after the ticker symbol of Starbucks Corporation (SBUX) on the NASDAQ.\n\n## Installing\n\nInstall and update using `pip`;\n\n```sh\npip install sbux\n```\n\n## A Simple Example\n\n```python\nfrom sbux import Starbucks\n\n\nstarbucks = Starbucks\nstarbucks.get_stores()\nstarbucks.get_menu_items(branch_code="13377")\n```\n\nSee more [examples](./examples/).\n\n## Contributing\n\nFor guidance on setting up a development environment and how to make a contribution, see the [contributing guidelines](./docs/CONTRIBUTING.md).\n',
     'author': 'Jerry Ng',
     'author_email': 'ngshiheng@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ngshiheng/sbux',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `sbux-0.3.0/PKG-INFO` & `sbux-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: sbux
-Version: 0.3.0
+Version: 0.4.0
 Summary: An unofficial Starbucks Singapore (SG) software development kit (SDK).
 Home-page: https://github.com/ngshiheng/sbux
 License: MIT
 Author: Jerry Ng
 Author-email: ngshiheng@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
 Project-URL: Repository, https://github.com/ngshiheng/sbux
 Description-Content-Type: text/markdown
 
 # sbux
 
 [![CI](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml)
 [![Semantic Release](https://github.com/ngshiheng/sbux/actions/workflows/release.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/release.yml)
@@ -41,11 +42,13 @@
 
 
 starbucks = Starbucks
 starbucks.get_stores()
 starbucks.get_menu_items(branch_code="13377")
 ```
 
+See more [examples](./examples/).
+
 ## Contributing
 
 For guidance on setting up a development environment and how to make a contribution, see the [contributing guidelines](./docs/CONTRIBUTING.md).
```

