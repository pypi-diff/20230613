# Comparing `tmp/dash_deckgl-0.1.2.tar.gz` & `tmp/dash_deckgl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_deckgl-0.1.2.tar", last modified: Thu May 25 21:05:45 2023, max compression
+gzip compressed data, was "dash_deckgl-0.1.3.tar", last modified: Tue Jun 13 04:46:09 2023, max compression
```

## Comparing `dash_deckgl-0.1.2.tar` & `dash_deckgl-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-25 21:05:45.953740 dash_deckgl-0.1.2/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.1.2/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.1.2/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     2092 2023-05-25 21:05:45.953740 dash_deckgl-0.1.2/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.1.2/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-25 21:05:45.949741 dash_deckgl-0.1.2/dash_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2849 2023-05-25 20:45:14.000000 dash_deckgl-0.1.2/dash_deckgl/DashDeckgl.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.1.2/dash_deckgl/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-05-25 20:45:14.000000 dash_deckgl-0.1.2/dash_deckgl/_imports_.py
--rw-rw-r--   0 dave      (1000) dave      (1000)  1202621 2023-05-25 20:45:12.000000 dash_deckgl-0.1.2/dash_deckgl/dash_deckgl.min.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    17642 2023-05-25 20:45:12.000000 dash_deckgl-0.1.2/dash_deckgl/deckgl.js
--rw-rw-r--   0 dave      (1000) dave      (1000)     2796 2023-05-25 20:45:14.000000 dash_deckgl-0.1.2/dash_deckgl/metadata.json
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-05-25 20:45:13.000000 dash_deckgl-0.1.2/dash_deckgl/package-info.json
--rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.1.2/dash_deckgl/vendor.js
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-25 21:05:45.953740 dash_deckgl-0.1.2/dash_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2092 2023-05-25 21:05:45.000000 dash_deckgl-0.1.2/dash_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      397 2023-05-25 21:05:45.000000 dash_deckgl-0.1.2/dash_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-25 21:05:45.000000 dash_deckgl-0.1.2/dash_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-05-25 21:05:45.000000 dash_deckgl-0.1.2/dash_deckgl.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-05-25 21:05:37.000000 dash_deckgl-0.1.2/package.json
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-25 21:05:45.953740 dash_deckgl-0.1.2/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      653 2023-05-25 20:56:07.000000 dash_deckgl-0.1.2/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.1.3/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.1.3/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.1.3/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-13 04:46:09.980181 dash_deckgl-0.1.3/dash_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2849 2023-06-13 04:37:29.000000 dash_deckgl-0.1.3/dash_deckgl/DashDeckgl.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.1.3/dash_deckgl/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-06-13 04:37:29.000000 dash_deckgl-0.1.3/dash_deckgl/_imports_.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)  1202621 2023-06-13 04:44:39.000000 dash_deckgl-0.1.3/dash_deckgl/dash_deckgl.min.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    17693 2023-06-13 04:44:39.000000 dash_deckgl-0.1.3/dash_deckgl/deckgl.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2796 2023-06-13 04:37:29.000000 dash_deckgl-0.1.3/dash_deckgl/metadata.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-06-13 04:37:29.000000 dash_deckgl-0.1.3/dash_deckgl/package-info.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.1.3/dash_deckgl/vendor.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/dash_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-06-13 04:46:09.000000 dash_deckgl-0.1.3/dash_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      417 2023-06-13 04:46:09.000000 dash_deckgl-0.1.3/dash_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-13 04:46:09.000000 dash_deckgl-0.1.3/dash_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-06-13 04:46:09.000000 dash_deckgl-0.1.3/dash_deckgl.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-06-13 04:19:09.000000 dash_deckgl-0.1.3/package.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      653 2023-05-25 20:56:07.000000 dash_deckgl-0.1.3/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      329 2023-05-25 21:17:05.000000 dash_deckgl-0.1.3/tests/test_usage.py
```

### Comparing `dash_deckgl-0.1.2/README.md` & `dash_deckgl-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.2/dash_deckgl/DashDeckgl.py` & `dash_deckgl-0.1.3/dash_deckgl/DashDeckgl.py`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.2/dash_deckgl/__init__.py` & `dash_deckgl-0.1.3/dash_deckgl/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.2/dash_deckgl/dash_deckgl.min.js` & `dash_deckgl-0.1.3/dash_deckgl/dash_deckgl.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -50007,15 +50007,15 @@
         var l = jsonpScriptSrc;
         jsonpScriptSrc = function(t) {
             var e, n = (e = A(), /\/_dash-component-suites\//.test(e.src)),
                 i = l(t);
             if (!n) return i;
             var r = i.split("/"),
                 s = r.slice(-1)[0].split(".");
-            return s.splice(1, 0, "v0_1_0m1685047493"), r.splice(-1, 1, s.join(".")), r.join("/")
+            return s.splice(1, 0, "v0_1_3m1686631460"), r.splice(-1, 1, s.join(".")), r.join("/")
         }
     }(() => {
         var t = {
             179: 0
         };
         o.f.j = (e, n) => {
             var i = o.o(t, e) ? t[e] : void 0;
```

### Comparing `dash_deckgl-0.1.2/dash_deckgl/deckgl.js` & `dash_deckgl-0.1.3/dash_deckgl/deckgl.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -688,15 +688,15 @@
                     S = v[1],
                     w = J((0, o.useState)({}), 2),
                     O = w[0],
                     T = w[1],
                     P = J((0, o.useState)(!1), 2),
                     C = (P[0], P[1], J((0, o.useState)(!1), 2)),
                     _ = (C[0], C[1], (0, o.useContext)(E)),
-                    j = J((0, o.useState)({}), 2),
+                    j = J((0, o.useState)(null), 2),
                     A = j[0],
                     x = j[1],
                     I = [];
                 if (m)
                     for (var D in m)
                         if (["top-right", "top-left", "bottom-right", "bottom-left"].includes(D)) {
                             var N = D.split("-");
@@ -744,18 +744,18 @@
                 (0, o.useEffect)((function() {
                     ! function() {
                         var e, r;
                         e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "https://api.tiles.mapbox.com/mapbox-gl-js/v1.13.2/mapbox-gl.css", (r = document.createElement("link")).type = "text/css", r.rel = "stylesheet", r.href = e, document.getElementsByTagName("head")[0].appendChild(r)
                     }()
                 }), []), (0, o.useEffect)((function() {
                     var e = _.convert(r);
-                    x(e.initialViewState), S(e)
+                    !A && e.initialViewState && x(e.initialViewState), S(B(B({}, L), e))
                 }), [r, _]), (0, o.useEffect)((function() {
                     var e = _.convert(g);
-                    T(e)
+                    T(B(B({}, O), e))
                 }), [g, _]);
                 var z = (0, o.useCallback)((function(e) {
                     var r = e.viewState;
                     x(r)
                 }), []);
                 return b ? a().createElement("div", null, "Google map overlays not supported") : a().createElement("div", {
                     className: "deckgl-map",
@@ -767,15 +767,15 @@
                 }, a().createElement("div", {
                     id: "deckgl-primary",
                     style: {
                         width: "100%",
                         height: "100%",
                         position: "relative"
                     }
-                }, a().createElement(i.Z, U({
+                }, A && a().createElement(i.Z, U({
                     viewState: A,
                     onViewStateChange: z
                 }, H, L), a().createElement(c.D5, {
                     mapStyle: L.mapStyle || l.Z.POSITRON,
                     mapboxAccessToken: d
                 }))), g && a().createElement("div", {
                     id: "deckgl-overlay",
```

### Comparing `dash_deckgl-0.1.2/dash_deckgl/metadata.json` & `dash_deckgl-0.1.3/dash_deckgl/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.2/dash_deckgl/package-info.json` & `dash_deckgl-0.1.3/dash_deckgl/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.3'"}*

```diff
@@ -66,9 +66,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_deckgl -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.0"
+    "version": "0.1.3"
 }
```

### Comparing `dash_deckgl-0.1.2/dash_deckgl/vendor.js` & `dash_deckgl-0.1.3/dash_deckgl/vendor.js`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.2/package.json` & `dash_deckgl-0.1.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.3'"}*

```diff
@@ -66,9 +66,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_deckgl -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `dash_deckgl-0.1.2/setup.py` & `dash_deckgl-0.1.3/setup.py`

 * *Files identical despite different names*

