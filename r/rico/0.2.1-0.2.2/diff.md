# Comparing `tmp/rico-0.2.1.tar.gz` & `tmp/rico-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.2.1.tar", last modified: Tue Jun 13 15:31:37 2023, max compression
+gzip compressed data, was "rico-0.2.2.tar", last modified: Tue Jun 13 17:20:45 2023, max compression
```

## Comparing `rico-0.2.1.tar` & `rico-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-13 15:31:14.482030 rico-0.2.1/LICENSE
--rw-r--r--   0        0        0      706 2023-06-13 15:31:14.482030 rico-0.2.1/README.md
--rw-r--r--   0        0        0     2870 2023-06-13 15:31:37.686476 rico-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      491 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/__init__.py
--rw-r--r--   0        0        0     5471 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_config.py
--rw-r--r--   0        0        0     5605 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_container.py
--rw-r--r--   0        0        0    14793 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_content.py
--rw-r--r--   0        0        0     7015 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_html.py
--rw-r--r--   0        0        0      340 2023-06-13 15:31:14.482030 rico-0.2.1/src/rico/_version.py
--rw-r--r--   0        0        0       18 2023-06-13 15:31:14.482030 rico-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__config.py
--rw-r--r--   0        0        0    10251 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__container.py
--rw-r--r--   0        0        0    17233 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__content.py
--rw-r--r--   0        0        0     9501 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__html.py
--rw-r--r--   0        0        0      730 2023-06-13 15:31:14.482030 rico-0.2.1/tests/test__version.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-13 17:20:06.004287 rico-0.2.2/LICENSE
+-rw-r--r--   0        0        0      706 2023-06-13 17:20:06.004287 rico-0.2.2/README.md
+-rw-r--r--   0        0        0     2870 2023-06-13 17:20:45.016727 rico-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      491 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/__init__.py
+-rw-r--r--   0        0        0     5471 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_config.py
+-rw-r--r--   0        0        0     5605 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_container.py
+-rw-r--r--   0        0        0    14546 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_content.py
+-rw-r--r--   0        0        0     7015 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_html.py
+-rw-r--r--   0        0        0      340 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_version.py
+-rw-r--r--   0        0        0       18 2023-06-13 17:20:06.008287 rico-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__config.py
+-rw-r--r--   0        0        0    10251 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__container.py
+-rw-r--r--   0        0        0    16739 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__content.py
+-rw-r--r--   0        0        0     9501 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__html.py
+-rw-r--r--   0        0        0      730 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__version.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.2.2/PKG-INFO
```

### Comparing `rico-0.2.1/LICENSE` & `rico-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.2.1/README.md` & `rico-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rico-0.2.1/pyproject.toml` & `rico-0.2.2/pyproject.toml`

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
-version = "0.2.1"
+version = "0.2.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/rico"
 "release notes" = "https://github.com/e10v/rico/releases"
```

### Comparing `rico-0.2.1/src/rico/_config.py` & `rico-0.2.2/src/rico/_config.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.1/src/rico/_container.py` & `rico-0.2.2/src/rico/_container.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.1/src/rico/_content.py` & `rico-0.2.2/src/rico/_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,30 +260,23 @@
         Args:
             data: The image data.
             format: The image format.
             class_: The container class attribute.
         """
         super().__init__(class_)
 
-        if format == "svg":
-            if isinstance(data, bytes):
-                data = data.decode()
-
-            for element in rico._html.parse_html(data):
-                self.container.append(element)
-        else:
-            if isinstance(data, str):
-                data = data.encode()
-            encoded_image = base64.b64encode(data).decode()
-
-            element = ET.Element(
-                "img",
-                attrib={"src": f"data:image/{format};base64,{encoded_image}"},
-            )
-            self.container.append(element)
+        if isinstance(data, str):
+            data = data.encode()
+        encoded_image = base64.b64encode(data).decode()
+
+        element = ET.Element(
+            "img",
+            attrib={"src": f"data:image/{format};base64,{encoded_image}"},
+        )
+        self.container.append(element)
 
 
 class Chart(ContentBase):
     """An Chart content definition.
 
     Creates content elements from a chart object and appends them to the container.
 
@@ -357,15 +350,15 @@
         Args:
             *objects: The objects which are used to create a content.
             class_: The container class attribute.
         """
         super().__init__(class_=class_)
         for obj in objects:
             if (
-                alt is not None and isinstance(obj, alt.Chart) or
+                alt is not None and isinstance(obj, alt.TopLevelMixin) or
                 plt is not None and isinstance(obj, plt.Axes | plt.Figure) or  # type: ignore  # noqa: E501
                 so is not None and isinstance(obj, so.Plot)
             ):
                 content = Chart(obj)
             elif hasattr(obj, "_repr_html_") and callable(obj._repr_html_):
                 content = HTML(obj._repr_html_(), strip_dataframe_borders=True)
             else:
```

### Comparing `rico-0.2.1/src/rico/_html.py` & `rico-0.2.2/src/rico/_html.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.1/tests/test__config.py` & `rico-0.2.2/tests/test__config.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.1/tests/test__container.py` & `rico-0.2.2/tests/test__container.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.1/tests/test__content.py` & `rico-0.2.2/tests/test__content.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,46 +313,33 @@
     "</svg>"
 )
 
 @pytest.mark.parametrize("data", [svg_data, svg_data.encode()], ids=["str", "bytes"])
 def test_image_svg(data: str | bytes):
     content = rico._content.Image(data, format="svg", class_="row")
 
+    if isinstance(data, str):
+        data = data.encode()
+    encoded_image = base64.b64encode(data).decode()
+
     div = content.container
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
-    svg = tuple(div)[0]
-    assert isinstance(svg, ET.Element)
-    assert svg.tag == "svg"
-    assert svg.attrib == {
-        "xmlns": "http://www.w3.org/2000/svg",
-        "xmlns:xlink": "http://www.w3.org/1999/xlink",
-        "width": "16",
-        "height": "16",
-        "fill": "currentColor",
-        "class": "bi bi-dash",
-    }
-    assert svg.text is None
-    assert svg.tail is None
-    assert len(svg) == 1
-
-    path = tuple(svg)[0]
-    assert isinstance(path, ET.Element)
-    assert path.tag == "path"
-    assert path.attrib == {
-        "d": "M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z",
-    }
-    assert path.text is None
-    assert path.tail is None
-    assert len(path) == 0
+    img = tuple(div)[0]
+    assert isinstance(img, ET.Element)
+    assert img.tag == "img"
+    assert img.attrib == {"src": f"data:image/svg;base64,{encoded_image}"}
+    assert img.text is None
+    assert img.tail is None
+    assert len(img) == 0
 
 
 @pytest.mark.parametrize("data", [svg_data, svg_data.encode()], ids=["str", "bytes"])
 def test_image_png(data: str | bytes):
     content = rico._content.Image(data, format="png")
 
     if isinstance(data, str):
@@ -404,22 +391,17 @@
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
-    if format is None:
-        svg = tuple(div)[0]
-        assert isinstance(svg, ET.Element)
-        assert svg.tag == "svg"
-    else:
-        img = tuple(div)[0]
-        assert isinstance(img, ET.Element)
-        assert img.tag == "img"
+    img = tuple(div)[0]
+    assert isinstance(img, ET.Element)
+    assert img.tag == "img"
 
 
 @pytest.mark.parametrize(
     ("module", "err_chart", "chart"),
     [
         ("alt", altair_chart, seaborn_plot),
         ("plt", pyplot_axes, altair_chart),
@@ -464,17 +446,17 @@
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "world"
     assert p.tail is None
     assert len(p) == 0
 
-    svg = tuple(div)[2]
-    assert isinstance(svg, ET.Element)
-    assert svg.tag == "svg"
+    img = tuple(div)[2]
+    assert isinstance(img, ET.Element)
+    assert img.tag == "img"
 
 
 @pytest.mark.parametrize("defer", [True, False], ids=["defer", "not defer"])
 def test_script_text(defer: bool):
     text = "alert('Hello World!');"
     attrib = {"async": True}
     content = rico._content.Script(text=text, defer=defer, attrib=attrib)
```

### Comparing `rico-0.2.1/tests/test__html.py` & `rico-0.2.2/tests/test__html.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.1/tests/test__version.py` & `rico-0.2.2/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.1/PKG-INFO` & `rico-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rico
-Version: 0.2.1
+Version: 0.2.2
 Summary: Rich content to HTML as easy as Doc(df, plot).
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

