# Comparing `tmp/grundkurs_theme-1.0.1.tar.gz` & `tmp/grundkurs_theme-1.0.2.tar.gz`

## Comparing `grundkurs_theme-1.0.1.tar` & `grundkurs_theme-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/.copier-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/.yarnrc.yml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/babel.config.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/jest.config.js
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/tsconfig.test.json
--rw-r--r--   0        0        0   406681 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/yarn.lock
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/_version.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/handlers.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/package.json
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/schemas/grundkurs_theme/package.json.orig
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/schemas/grundkurs_theme/plugin.json
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/525.b3511822b6377fa70b30.js
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/remoteEntry.a136c23060f50b65fdb6.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    16411 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/themes/grundkurs_theme/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/themes/grundkurs_theme/index.js
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/schema/plugin.json
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/src/handler.ts
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/src/index.ts
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/src/widget.tsx
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/src/__tests__/grundkurs_theme.spec.ts
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/style/index.css
--rw-r--r--   0        0        0    14559 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/style/variables.css
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/LICENSE
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/README.md
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/.copier-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/.yarnrc.yml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/babel.config.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/jest.config.js
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/tsconfig.test.json
+-rw-r--r--   0        0        0   406681 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/yarn.lock
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/_version.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/handlers.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/labextension/package.json
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/labextension/schemas/grundkurs_theme/package.json.orig
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/labextension/schemas/grundkurs_theme/plugin.json
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/labextension/static/525.b3511822b6377fa70b30.js
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/labextension/static/remoteEntry.4449bf68d20eaa87bb99.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    16455 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/labextension/themes/grundkurs_theme/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/grundkurs_theme/labextension/themes/grundkurs_theme/index.js
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/schema/plugin.json
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/src/handler.ts
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/src/index.ts
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/src/widget.tsx
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/src/__tests__/grundkurs_theme.spec.ts
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/style/index.css
+-rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/style/variables.css
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/README.md
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.2/PKG-INFO
```

### Comparing `grundkurs_theme-1.0.1/.copier-answers.yml` & `grundkurs_theme-1.0.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/RELEASE.md` & `grundkurs_theme-1.0.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/jest.config.js` & `grundkurs_theme-1.0.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/package.json` & `grundkurs_theme-1.0.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'1.0.2'"}*

```diff
@@ -175,12 +175,12 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1",
+    "version": "1.0.2",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `grundkurs_theme-1.0.1/tsconfig.json` & `grundkurs_theme-1.0.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/yarn.lock` & `grundkurs_theme-1.0.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/grundkurs_theme/handlers.py` & `grundkurs_theme-1.0.2/grundkurs_theme/handlers.py`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/grundkurs_theme/labextension/package.json` & `grundkurs_theme-1.0.2/grundkurs_theme/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9777173913043479%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.4449bf68d20eaa87bb99.js'}}",*

 * * "'version'": "'1.0.2'"}*

```diff
@@ -106,15 +106,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/grundkurs-programmieren/grundkurs_theme",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a136c23060f50b65fdb6.js"
+            "load": "static/remoteEntry.4449bf68d20eaa87bb99.js"
         },
         "extension": true,
         "outputDir": "grundkurs_theme/labextension",
         "schemaDir": "schema",
         "themePath": "style/index.css"
     },
     "keywords": [
@@ -179,12 +179,12 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1",
+    "version": "1.0.2",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `grundkurs_theme-1.0.1/grundkurs_theme/labextension/schemas/grundkurs_theme/package.json.orig` & `grundkurs_theme-1.0.2/grundkurs_theme/labextension/schemas/grundkurs_theme/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'1.0.2'"}*

```diff
@@ -175,12 +175,12 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1",
+    "version": "1.0.2",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/525.b3511822b6377fa70b30.js` & `grundkurs_theme-1.0.2/grundkurs_theme/labextension/static/525.b3511822b6377fa70b30.js`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/remoteEntry.a136c23060f50b65fdb6.js` & `grundkurs_theme-1.0.2/grundkurs_theme/labextension/static/remoteEntry.4449bf68d20eaa87bb99.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -98,15 +98,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => b.e(525).then((() => () => b(525))),
                         from: i,
                         eager: !1
                     })
-                })("grundkurs_theme", "1.0.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("grundkurs_theme", "1.0.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         b.g.importScripts && (e = b.g.location + "");
         var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `grundkurs_theme-1.0.1/grundkurs_theme/labextension/themes/grundkurs_theme/index.css` & `grundkurs_theme-1.0.2/grundkurs_theme/labextension/themes/grundkurs_theme/index.css`

 * *Files 1% similar despite different names*

```diff
@@ -209,18 +209,18 @@
   --jp-inverse-layout-color1: var(--md-grey-900);
   --jp-inverse-layout-color2: var(--md-grey-800);
   --jp-inverse-layout-color3: var(--md-grey-700);
   --jp-inverse-layout-color4: var(--md-grey-600);
 
   /* Brand/accent */
 
-  --jp-brand-color0: #ec0c4b;
-  --jp-brand-color1: #ed225d;
-  --jp-brand-color2: #ee376b;
-  --jp-brand-color3: #ee3b6e;
+  --jp-brand-color0: var(--md-blue-700);
+  --jp-brand-color1: var(--md-blue-500);
+  --jp-brand-color2: var(--md-blue-300);
+  --jp-brand-color3: var(--md-blue-100);
   --jp-accent-color0: var(--md-green-700);
   --jp-accent-color1: var(--md-green-500);
   --jp-accent-color2: var(--md-green-300);
   --jp-accent-color3: var(--md-green-100);
 
   /* State colors (warn, error, success, info) */
```

### Comparing `grundkurs_theme-1.0.1/src/handler.ts` & `grundkurs_theme-1.0.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/src/index.ts` & `grundkurs_theme-1.0.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/src/widget.tsx` & `grundkurs_theme-1.0.2/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/style/index.css` & `grundkurs_theme-1.0.2/style/index.css`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/style/variables.css` & `grundkurs_theme-1.0.2/style/variables.css`

 * *Files 1% similar despite different names*

```diff
@@ -209,18 +209,18 @@
   --jp-inverse-layout-color1: var(--md-grey-900);
   --jp-inverse-layout-color2: var(--md-grey-800);
   --jp-inverse-layout-color3: var(--md-grey-700);
   --jp-inverse-layout-color4: var(--md-grey-600);
 
   /* Brand/accent */
 
-  --jp-brand-color0: #ec0c4b;
-  --jp-brand-color1: #ed225d;
-  --jp-brand-color2: #ee376b;
-  --jp-brand-color3: #ee3b6e;
+  --jp-brand-color0: var(--md-blue-700);
+  --jp-brand-color1: var(--md-blue-500);
+  --jp-brand-color2: var(--md-blue-300);
+  --jp-brand-color3: var(--md-blue-100);
   --jp-accent-color0: var(--md-green-700);
   --jp-accent-color1: var(--md-green-500);
   --jp-accent-color2: var(--md-green-300);
   --jp-accent-color3: var(--md-green-100);
 
   /* State colors (warn, error, success, info) */
```

### Comparing `grundkurs_theme-1.0.1/.gitignore` & `grundkurs_theme-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/LICENSE` & `grundkurs_theme-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/README.md` & `grundkurs_theme-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/pyproject.toml` & `grundkurs_theme-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-1.0.1/PKG-INFO` & `grundkurs_theme-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grundkurs_theme
-Version: 1.0.1
+Version: 1.0.2
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/grundkurs-programmieren/grundkurs_theme
 Project-URL: Bug Tracker, https://github.com/grundkurs-programmieren/grundkurs_theme/issues
 Project-URL: Repository, https://github.com/grundkurs-programmieren/grundkurs_theme.git
 Author-email: Noe Thalheim <noe@thalheim.email>
 License: BSD 3-Clause License
```

