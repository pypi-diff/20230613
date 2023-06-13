# Comparing `tmp/rico-0.2.0.tar.gz` & `tmp/rico-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.2.0.tar", last modified: Sun Jun  4 14:23:14 2023, max compression
+gzip compressed data, was "rico-0.2.1.tar", last modified: Tue Jun 13 15:31:37 2023, max compression
```

## Comparing `rico-0.2.0.tar` & `rico-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-04 14:22:49.892705 rico-0.2.0/LICENSE
--rw-r--r--   0        0        0      706 2023-06-04 14:22:49.892705 rico-0.2.0/README.md
--rw-r--r--   0        0        0     2870 2023-06-04 14:23:14.717679 rico-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      491 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/__init__.py
--rw-r--r--   0        0        0     5483 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_config.py
--rw-r--r--   0        0        0     5605 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_container.py
--rw-r--r--   0        0        0    14768 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_content.py
--rw-r--r--   0        0        0     7015 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_html.py
--rw-r--r--   0        0        0      340 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_version.py
--rw-r--r--   0        0        0       18 2023-06-04 14:22:49.892705 rico-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-04 14:22:49.892705 rico-0.2.0/tests/test__config.py
--rw-r--r--   0        0        0    10247 2023-06-04 14:22:49.892705 rico-0.2.0/tests/test__container.py
--rw-r--r--   0        0        0    17232 2023-06-04 14:22:49.896705 rico-0.2.0/tests/test__content.py
--rw-r--r--   0        0        0     9501 2023-06-04 14:22:49.896705 rico-0.2.0/tests/test__html.py
--rw-r--r--   0        0        0      730 2023-06-04 14:22:49.896705 rico-0.2.0/tests/test__version.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-13 15:31:14.482030 rico-0.2.1/LICENSE
+-rw-r--r--   0        0        0      706 2023-06-13 15:31:14.482030 rico-0.2.1/README.md
+-rw-r--r--   0        0        0     2870 2023-06-13 15:31:37.686476 rico-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      491 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/__init__.py
+-rw-r--r--   0        0        0     5471 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_config.py
+-rw-r--r--   0        0        0     5605 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_container.py
+-rw-r--r--   0        0        0    14793 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_content.py
+-rw-r--r--   0        0        0     7015 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_html.py
+-rw-r--r--   0        0        0      340 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_version.py
+-rw-r--r--   0        0        0       18 2023-06-13 15:31:14.482030 rico-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__config.py
+-rw-r--r--   0        0        0    10251 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__container.py
+-rw-r--r--   0        0        0    17233 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__content.py
+-rw-r--r--   0        0        0     9501 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__html.py
+-rw-r--r--   0        0        0      730 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__version.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.2.1/PKG-INFO
```

### Comparing `rico-0.2.0/LICENSE` & `rico-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.2.0/README.md` & `rico-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rico-0.2.0/pyproject.toml` & `rico-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
-version = "0.2.0"
+version = "0.2.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/rico"
 "release notes" = "https://github.com/e10v/rico/releases"
```

### Comparing `rico-0.2.0/src/rico/_config.py` & `rico-0.2.1/src/rico/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,18 +72,17 @@
 
     Args:
         param: Paramater name.
 
     Returns:
         Parameter value if `param` is not None, or dict with all parameters otherwise.
     """
-    config = _global_config.copy()
     if param is not None:
-        return config[param]
-    return config
+        return _global_config[param]
+    return _global_config.copy()
 
 
 def set_config(
     bootstrap_css: str | None = None,
     bootstrap_js: str | None = None,
     dataframe_style: str | None = None,
     image_format: Literal["svg", "png"] | None = None,
```

### Comparing `rico-0.2.0/src/rico/_container.py` & `rico-0.2.1/src/rico/_container.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.0/src/rico/_content.py` & `rico-0.2.1/src/rico/_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,18 +322,18 @@
             stream = io.StringIO() if format == "svg" else io.BytesIO()
             obj.savefig(stream, format=format, **kwargs)
             image = stream.getvalue()
         elif so is not None and isinstance(obj, so.Plot):
             stream = io.StringIO() if format == "svg" else io.BytesIO()
             obj.save(stream, format=format, **kwargs)
             image = stream.getvalue()
-        elif alt is not None and isinstance(obj, alt.Chart):
+        elif alt is not None and isinstance(obj, alt.TopLevelMixin):
             convert = vlc.vegalite_to_svg if format == "svg" else vlc.vegalite_to_png  # type: ignore  # noqa: E501
             image = convert(  # type: ignore
-                obj.to_json(),
+                obj.to_json(),  # type: ignore
                 vl_version="_".join(alt.SCHEMA_VERSION.split(".")[:2]),
                 **kwargs,
             )
         else:
             error_msg = (
                 f"Chart type {type(obj)} is not supported "
                 "or required extra package is not installed."
@@ -482,15 +482,15 @@
         if inline and src is not None:
             with urllib.request.urlopen(src) as response:
                 text = response.read().decode()
             src = None
 
         if src is not None:
             tag = "link"
-            attrib = {"src": src, **attrib}
+            attrib = {"href": src, **attrib}
             if "rel" not in attrib:
                 attrib = {**attrib, "rel": "stylesheet"}
         else:
             tag = "style"
 
         self.container = ET.Element(tag, {**attrib, **extra})
         self.container.text = text
```

### Comparing `rico-0.2.0/src/rico/_html.py` & `rico-0.2.1/src/rico/_html.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.0/tests/test__config.py` & `rico-0.2.1/tests/test__config.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.0/tests/test__container.py` & `rico-0.2.1/tests/test__container.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     assert viewport.tail is None
     assert len(viewport) == 0
 
     bootstrap_css = tuple(head)[2]
     assert isinstance(bootstrap_css, ET.Element)
     assert bootstrap_css.tag == "link"
     assert bootstrap_css.attrib == {
-        "src": rico._config.BOOTSTRAP_CSS,
+        "href": rico._config.BOOTSTRAP_CSS,
         "rel": "stylesheet",
     }
     assert bootstrap_css.text is None
     assert bootstrap_css.tail is None
     assert len(bootstrap_css) == 0
 
     df_style = tuple(head)[3]
@@ -232,15 +232,15 @@
         meta_charset="",
         meta_viewport="",
         dataframe_style="",
     ):
         doc = rico._container.Doc(
             "Hello world",
             title="Title",
-           bootstrap="full",
+            bootstrap="full",
             extra_styles=(extra_style,),
             extra_scripts=(extra_script,),
             class_=None,
         )
 
     html = doc.html
     assert isinstance(html, ET.Element)
@@ -267,26 +267,26 @@
     assert title.tail is None
     assert len(title) == 0
 
     bootstrap_css = tuple(head)[1]
     assert isinstance(bootstrap_css, ET.Element)
     assert bootstrap_css.tag == "link"
     assert bootstrap_css.attrib == {
-        "src": rico._config.BOOTSTRAP_CSS,
+        "href": rico._config.BOOTSTRAP_CSS,
         "rel": "stylesheet",
     }
     assert bootstrap_css.text is None
     assert bootstrap_css.tail is None
     assert len(bootstrap_css) == 0
 
     style = tuple(head)[2]
     style = extra_style.container
     assert isinstance(style, ET.Element)
     assert style.tag == "link"
-    assert style.attrib == {"src": "style.css", "rel": "stylesheet"}
+    assert style.attrib == {"href": "style.css", "rel": "stylesheet"}
     assert style.text is None
     assert style.tail is None
     assert len(style) == 0
 
     bootstrap_js = tuple(head)[3]
     assert isinstance(bootstrap_js, ET.Element)
     assert bootstrap_js.tag == "script"
```

### Comparing `rico-0.2.0/tests/test__content.py` & `rico-0.2.1/tests/test__content.py`

 * *Files 0% similar despite different names*

```diff
@@ -560,15 +560,15 @@
 
 
 def test_style_src():
     src = "style.css"
     attrib = {"crossorigin": "anonymous"}
     content = rico._content.Style(src=src, attrib=attrib)
 
-    attrib = {"src": src, **attrib, "rel": "stylesheet"}
+    attrib = {"href": src, **attrib, "rel": "stylesheet"}
 
     link = content.container
     assert isinstance(link, ET.Element)
     assert link.tag == "link"
     assert link.attrib == attrib
     assert link.text is None
     assert link.tail is None
```

### Comparing `rico-0.2.0/tests/test__html.py` & `rico-0.2.1/tests/test__html.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.0/tests/test__version.py` & `rico-0.2.1/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.0/PKG-INFO` & `rico-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rico
-Version: 0.2.0
+Version: 0.2.1
 Summary: Rich content to HTML as easy as Doc(df, plot).
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

