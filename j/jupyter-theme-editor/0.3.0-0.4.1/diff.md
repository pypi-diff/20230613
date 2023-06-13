# Comparing `tmp/jupyter_theme_editor-0.3.0.tar.gz` & `tmp/jupyter_theme_editor-0.4.1.tar.gz`

## Comparing `jupyter_theme_editor-0.3.0.tar` & `jupyter_theme_editor-0.4.1.tar`

### file list

```diff
@@ -1,60 +1,57 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/.eslintrc.js
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/.stylelintrc
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/MANIFEST.in
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/babel.config.js
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/conftest.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jest.config.js
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/tsconfig.json
--rw-r--r--   0        0        0   448350 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/yarn.lock
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter-config/nb-config/jupyter_theme_editor.json
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter-config/server-config/jupyter_theme_editor.json
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/_version.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/handlers.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/package.json
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/schemas/jupyter-theme-editor/package.json.orig
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/schemas/jupyter-theme-editor/plugin.json
--rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/290.dcd1110ba978a36d1c6d.js
--rw-r--r--   0        0        0    36510 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/351.9ec43e8031fd2252d01d.js
--rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/747.a5300d89923b0c6831bf.js
--rw-r--r--   0        0        0    72320 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/785.2fc5bebd96804ab650b2.js
--rw-r--r--   0        0        0   236270 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/807.68bd5c7d28866c568e00.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/807.68bd5c7d28866c568e00.js.LICENSE.txt
--rw-r--r--   0        0        0    20335 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/861.7c8ce849384f01571a74.js
--rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/remoteEntry.bdf4fdb49ec09bfbe704.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/style.js
--rw-r--r--   0        0        0    45158 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/templates/template.css
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/tests/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/jupyter_theme_editor/tests/test_handlers.py
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/schema/plugin.json
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/src/handler.ts
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/src/icons.ts
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/src/index.ts
--rw-r--r--   0        0        0    12135 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/src/model.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/src/svg.d.ts
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/src/view.tsx
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/src/__tests__/jupyter_theme_editor.spec.ts
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/style/base.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/style/index.js
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/style/theme-editor.svg
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/ui-tests/jupyter_theme_editor.spec.ts
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   124088 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/LICENSE
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/README.md
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/.yarnrc.yml
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/babel.config.js
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/conftest.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jest.config.js
+-rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/tsconfig.test.json
+-rw-r--r--   0        0        0   364628 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/yarn.lock
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter-config/nb-config/jupyter_theme_editor.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter-config/server-config/jupyter_theme_editor.json
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/_version.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/handlers.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/package.json
+-rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/schemas/jupyter-theme-editor/package.json.orig
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/schemas/jupyter-theme-editor/plugin.json
+-rw-r--r--   0        0        0    72976 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/304.caed9225fc88627a1ade.js
+-rw-r--r--   0        0        0    36510 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/351.9ec43e8031fd2252d01d.js
+-rw-r--r--   0        0        0    11575 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/535.251e4fef15db43619f3b.js
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/747.e721e56eaf04858131e6.js
+-rw-r--r--   0        0        0   236563 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/807.deac369ec79332e05c33.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/807.deac369ec79332e05c33.js.LICENSE.txt
+-rw-r--r--   0        0        0    20335 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/861.7c8ce849384f01571a74.js
+-rw-r--r--   0        0        0     8266 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/remoteEntry.f72e9c07a70775e21991.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/style.js
+-rw-r--r--   0        0        0    45158 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/templates/template.css
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/tests/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/jupyter_theme_editor/tests/test_handlers.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/schema/plugin.json
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/src/handler.ts
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/src/icons.ts
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/src/index.ts
+-rw-r--r--   0        0        0    12135 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/src/model.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/src/svg.d.ts
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/src/view.tsx
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/src/__tests__/jupyter_theme_editor.spec.ts
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/style/base.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/style/index.js
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/style/theme-editor.svg
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/ui-tests/tests/jupyter_theme_editor.spec.ts
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/README.md
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 jupyter_theme_editor-0.4.1/PKG-INFO
```

### Comparing `jupyter_theme_editor-0.3.0/CHANGELOG.md` & `jupyter_theme_editor-0.4.1/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,59 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.4.1
+
+([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/compare/v0.3.0...ff9d52347d4b8eb1a03a3ad33b0b830586ebd3a8))
+
+### Bugs fixed
+
+- Fix linting in package.json. [#16](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/pull/16) ([@HaudinFlorence](https://github.com/HaudinFlorence))
+
+### Maintenance and upkeep improvements
+
+- Migrate extension [#14](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/pull/14) ([@HaudinFlorence](https://github.com/HaudinFlorence))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/graphs/contributors?from=2023-03-23&to=2023-06-12&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-theme-editor+involves%3Agithub-actions+updated%3A2023-03-23..2023-06-12&type=Issues) | [@HaudinFlorence](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-theme-editor+involves%3AHaudinFlorence+updated%3A2023-03-23..2023-06-12&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-theme-editor+involves%3Ajtpio+updated%3A2023-03-23..2023-06-12&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
+## 0.4.0
+
+([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/compare/v0.3.0...a7fd5cf02f6e807b82a9e74d903a454623f98ff4))
+
+### Maintenance and upkeep improvements
+
+- Migrate extension [#14](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/pull/14) ([@HaudinFlorence](https://github.com/HaudinFlorence))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/graphs/contributors?from=2023-03-23&to=2023-06-12&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-theme-editor+involves%3Agithub-actions+updated%3A2023-03-23..2023-06-12&type=Issues) | [@HaudinFlorence](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-theme-editor+involves%3AHaudinFlorence+updated%3A2023-03-23..2023-06-12&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-theme-editor+involves%3Ajtpio+updated%3A2023-03-23..2023-06-12&type=Issues)
+
 ## 0.3.0
 
 ([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/compare/v0.2.1...d18e1d4b15caefb361ce57107b55a3ab4aa8c7fc))
 
 ### Merged PRs
 
 - Update the style of the react json schema form. [#11](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/pull/11) ([@HaudinFlorence](https://github.com/HaudinFlorence))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/graphs/contributors?from=2023-03-21&to=2023-03-23&type=c))
 
 [@HaudinFlorence](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-theme-editor+involves%3AHaudinFlorence+updated%3A2023-03-21..2023-03-23&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.2.1
 
 ([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/compare/v0.2.0...c7140a1b4df0a6c2ba493a2787addc187bfa4c25))
 
 ### Merged PRs
 
 - Update parameters [#10](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/pull/10) ([@HaudinFlorence](https://github.com/HaudinFlorence))
```

### Comparing `jupyter_theme_editor-0.3.0/RELEASE.md` & `jupyter_theme_editor-0.4.1/RELEASE.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,30 +2,41 @@
 
 The extension can be published to `PyPI` and `npm` manually or using the [Jupyter Releaser](https://github.com/jupyter-server/jupyter_releaser).
 
 ## Manual release
 
 ### Python package
 
-This extension can be distributed as Python
-packages. All of the Python
-packaging instructions in the `pyproject.toml` file to wrap your extension in a
-Python package. Before generating a package, we first need to install `build`.
+This extension can be distributed as Python packages. All of the Python
+packaging instructions are in the `pyproject.toml` file to wrap your extension in a
+Python package. Before generating a package, you first need to install some tools:
 
 ```bash
 pip install build twine hatch
 ```
 
 Bump the version using `hatch`. By default this will create a tag.
 See the docs on [hatch-nodejs-version](https://github.com/agoose77/hatch-nodejs-version#semver) for details.
 
 ```bash
 hatch version <new-version>
 ```
 
+Make sure to clean up all the development files before building the package:
+
+```bash
+jlpm clean:all
+```
+
+You could also clean up the local git repository:
+
+```bash
+git clean -dfX
+```
+
 To create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory, do:
 
 ```bash
 python -m build
 ```
 
 > `python setup.py sdist bdist_wheel` is deprecated and will not work for this package.
@@ -45,24 +56,22 @@
 npm publish --access public
 ```
 
 ## Automated releases with the Jupyter Releaser
 
 The extension repository should already be compatible with the Jupyter Releaser.
 
-Check out the [workflow documentation](https://github.com/jupyter-server/jupyter_releaser#typical-workflow) for more information.
+Check out the [workflow documentation](https://jupyter-releaser.readthedocs.io/en/latest/get_started/making_release_from_repo.html) for more information.
 
 Here is a summary of the steps to cut a new release:
 
-- Fork the [`jupyter-releaser` repo](https://github.com/jupyter-server/jupyter_releaser)
-- Add `ADMIN_GITHUB_TOKEN`, `PYPI_TOKEN` and `NPM_TOKEN` to the Github Secrets in the fork
+- Add `ADMIN_GITHUB_TOKEN`, `PYPI_TOKEN` and `NPM_TOKEN` to the [Github Secrets](https://docs.github.com/en/actions/security-guides/encrypted-secrets) in the repository
 - Go to the Actions panel
-- Run the "Draft Changelog" workflow
-- Merge the Changelog PR
-- Run the "Draft Release" workflow
-- Run the "Publish Release" workflow
+- Run the "Step 1: Prep Release" workflow
+- Check the draft changelog
+- Run the "Step 2: Publish Release" workflow
 
 ## Publishing to `conda-forge`
 
 If the package is not on conda forge yet, check the documentation to learn how to add it: https://conda-forge.org/docs/maintainer/adding_pkgs.html
 
 Otherwise a bot should pick up the new version publish to PyPI, and open a new PR on the feedstock repository automatically.
```

### Comparing `jupyter_theme_editor-0.3.0/tsconfig.json` & `jupyter_theme_editor-0.4.1/tsconfig.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2018'}"}*

```diff
@@ -13,15 +13,15 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2018",
+        "target": "ES2018",
         "types": [
             "jest"
         ]
     },
     "include": [
         "src/*"
     ]
```

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/__init__.py` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/handlers.py` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/schemas/jupyter-theme-editor/plugin.json` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/schemas/jupyter-theme-editor/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/290.dcd1110ba978a36d1c6d.js` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/535.251e4fef15db43619f3b.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunkjupyter_theme_editor = self.webpackChunkjupyter_theme_editor || []).push([
-    [290], {
-        290: (t, e, o) => {
+    [535], {
+        3535: (t, e, o) => {
             o.r(e), o.d(e, {
                 default: () => N
             });
-            var r = o(2884);
-            const n = new(o(3215).LabIcon)({
+            var r = o(5350);
+            const n = new(o(2189).LabIcon)({
                 name: "@jupyterlab/jupyter-theme-editor:theme-editor",
                 svgstr: '<?xml version="1.0" encoding="UTF-8"?>\n\x3c!-- Created with Vectornator (http://vectornator.io/) --\x3e\n<svg width="32" height="32" clip-rule="evenodd" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" version="1.1" viewBox="0 0 32 32" xml:space="preserve" xmlns="http://www.w3.org/2000/svg" xmlns:vectornator="http://vectornator.io">\n<g class="jp-icon3" transform="matrix(1.12 0 0 1.12 -.79163 -1.9985)" fill="#616161">\n\n\n\n\n\n<g transform="translate(-.8135 -.70854)"><g transform="matrix(1.01 0 0 1.01 -.15908 -.16883)"><g transform="matrix(1.029 0 0 1.029 .069016 -2.7107)"><g transform="matrix(.029276 -.0020473 .0020473 .029276 -.31852 3.8499)" vectornator:layerName="Layer 1">\n<path d="m542.97 104.28c-143.31 0.702-234.82 80.755-257.91 182-29.552 129.59 9.217 224.28 117.88 251.03 108.66 26.748 157.5 36.834 181.47 69.157 75.868 102.32 39.712 167.86 61.282 211.12 52.191 104.7 226.78-47.032 284.56-270.47 57.782-223.44-36.168-361.67-255.06-423.5-47.884-13.526-92.094-19.54-132.22-19.344zm15.906 66.781c1.677 0.075 3.352 0.265 5.031 0.594 26.871 5.268 43.248 41.767 36.563 81.532-6.685 39.764-33.91 67.737-60.781 62.468-26.872-5.268-43.216-41.766-36.532-81.531 6.267-37.28 30.565-64.185 55.719-63.063zm159.44 41.75c5.104 0.119 10.07 1.248 14.719 3.5 24.795 12.016 31.319 51.261 14.563 87.657s-50.456 56.171-75.25 44.156c-24.795-12.015-31.318-51.26-14.563-87.656 13.614-29.572 38.415-48.169 60.531-47.657zm-331.62 20.938c23.491 0.977 47.909 25.358 57.718 59.688 11.211 39.233-0.916 76.593-27.094 83.437-26.177 6.844-56.477-19.423-67.687-58.656-11.211-39.234 0.916-76.563 27.094-83.407 3.272-0.855 6.613-1.201 9.969-1.062zm456.59 97.688c8.977 0.389 17.172 3.297 23.719 8.937 20.949 18.048 16.968 57.326-8.875 87.75-25.842 30.424-63.77 40.454-84.719 22.406-20.949-18.047-16.967-57.325 8.875-87.75 17.767-20.917 41.252-32.201 61-31.343z" stroke="#616161" stroke-linecap="butt" stroke-linejoin="round" stroke-width="17.775"/>\n</g><g transform="matrix(.62364 -.62364 .62366 .62366 -4.4514 16.59)"><g transform="matrix(.025113 .02183 -.02183 .025113 11.728 -5.0008)" vectornator:layerName="Layer 4">\n<path d="m324.12 592.86c-3.614 3.413-7.92 7.029-12.875 10.907-0.058 0.048-0.098 0.108-0.156 0.156-0.179 0.14-0.35 0.265-0.531 0.406-1.406 1.094-2.534 2.064-4.063 3.219 0.095-0.071-7.365 5.562-9.406 7.125-3.735 2.86-6.665 5.206-9.25 7.469-0.523 0.457-4.92 4.399-6.375 5.656-1.228 1.061-2.343 1.923-3.5 2.844 19.902 25.075 41.269 51.267 64.5 78.562 113.78 133.68 217.74 233.93 232.19 223.91 14.452-10.027-66.09-126.53-179.88-260.22-24.349-28.608-47.99-55.243-70.657-80.032z" stroke="#616161" stroke-linecap="butt" stroke-linejoin="round" stroke-width="17.775"/>\n</g><g id="Layer-4-copy" transform="matrix(.025113 .02183 -.02183 .025113 11.728 -5.0008)" vectornator:layerName="Layer 4 copy">\n<path d="m235 500.95c-8.171 10.062-18.667 19.129-32.343 28.969 16.499 24.03 37.303 52.227 61.375 83.094 14.423-7.914 30.688-21.238 45.218-36.313-27.349-29.399-52.676-55.28-74.25-75.75z" stroke="#616161" stroke-linecap="butt" stroke-linejoin="round" stroke-width="17.775"/>\n</g><g transform="matrix(.025113 .02183 -.02183 .025113 11.728 -5.0008)" vectornator:layerName="Layer 3">\n<path d="m145.1 366.55c40.96 6.246 59.443 23.082 79.348 76.653 13.046 35.111-18.332 61.686-38.681 69.832-20.35 8.145-69.142-13.169-95.537-53.739-45.607-70.1-14.564-147.68 13.388-163.34 27.951-15.658-1.862 63.98 41.482 70.59z" stroke="#616161" stroke-linecap="butt" stroke-linejoin="round" stroke-width="17.775"/>\n</g></g></g></g></g></g>\n</svg>\n'
             });
             var s = o(8185);
 
             function i(t, e, o, r) {
                 const n = [];
@@ -186,22 +186,22 @@
                         this._formDataSetter[e](o)
                     }
                     this._formData = t;
                     for (const t in this._cssProperties) document.body.style.setProperty(t, this._cssProperties[t]);
                     this.stateChanged.emit()
                 }
             }
-            var y = o(6271),
+            var y = o(6029),
                 b = o.n(y),
-                w = o(7256),
+                w = o(4957),
                 j = o.n(w),
                 S = o(6212),
-                v = o(8604),
-                _ = o(6848),
-                x = o(5613);
+                v = o(926),
+                _ = o(9993),
+                x = o(4238);
 
             function C(t) {
                 return b().createElement(j(), {
                     schema: t.schema,
                     formData: t.formData,
                     uiSchema: t.uiSchema,
                     onChange: e => {
@@ -321,15 +321,15 @@
                         uiSchema: this.uiSchema,
                         setformData: t => {
                             this.model.formData = t
                         }
                     }))
                 }
             }
-            var D = o(1194);
+            var D = o(56);
             const z = "jupyter-theme-editor:plugin",
                 N = {
                     id: z,
                     autoStart: !0,
                     requires: [r.IThemeManager],
                     optional: [D.ISettingRegistry, v.ITranslator],
                     activate: (t, e, o, r) => {
```

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/351.9ec43e8031fd2252d01d.js` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/351.9ec43e8031fd2252d01d.js`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/747.a5300d89923b0c6831bf.js` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/747.e721e56eaf04858131e6.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,179 +1,198 @@
 "use strict";
 (self.webpackChunkjupyter_theme_editor = self.webpackChunkjupyter_theme_editor || []).push([
     [747], {
         1150: (t, e, o) => {
             o.d(e, {
-                Z: () => r
+                Z: () => a
             });
-            var n = o(3645),
-                i = o.n(n)()((function(t) {
-                    return t[1]
-                }));
-            i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Courier);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Dancing+Script);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Dosis);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Helvetica);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=JetBrains+Mono);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Lobster);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Oxygen);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Pacifico);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Prompt);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Righteous);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Satisfy);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Single+Day);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Space+Mono);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Times+New+Roman);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Ultra);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Urbanist);"]), i.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Verdana);"]), i.push([t.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n\n.jp-theme-editor-panel {\n  overflow-y: auto;\n}\n\n.jp-theme-editor-button-color {\n  height: var(--jp-ui-font-size0);\n  width: 25px;\n  position: absolute;\n  right: 0;\n  margin-right: 5%;\n}\n\n.form-control {\n  right: 0;\n  width: 95%;\n}\n\n.jp-theme-editor-color-picker {\n  position: relative;\n  left: 0;\n}\n\n.form-class {\n  background-color: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  font-size: var(--jp-ui-font-size0);\n  line-height: 2em;\n}\n\n:root {\n  --jp-ui-font-family: 'Arial', 'Courier', 'Dancing Script', 'Dosis',\n    'Helvetica', 'Lobster', 'JetBrains Mono', 'Pacifico', 'Prompt', 'Righteous',\n    'Sans Serif', 'Satisfy', 'Single Day', 'system-ui', 'Times New Roman',\n    'Urbanist', 'Verdana';\n  --jp-content-font-family: 'Arial', 'Courier', 'Dancing Script', 'Helvetica',\n    'Dosis', 'Lobster', 'JetBrains Mono', 'Pacifico', 'Prompt', 'Righteous',\n    'Sans Serif', 'Satisfy', 'Single Day', 'system-ui', 'Times New Roman',\n    'Urbanist', 'Verdana';\n  --jp-code-font-family: 'monospace', 'Space Mono';\n}\n", ""]);
-            const r = i
+            var n = o(8081),
+                r = o.n(n),
+                i = o(3645),
+                s = o.n(i)()(r());
+            s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Courier);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Dancing+Script);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Dosis);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Helvetica);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=JetBrains+Mono);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Lobster);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Oxygen);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Pacifico);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Prompt);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Righteous);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Satisfy);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Single+Day);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Space+Mono);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Times+New+Roman);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Ultra);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Urbanist);"]), s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Verdana);"]), s.push([t.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n\n.jp-theme-editor-panel {\n  overflow-y: auto;\n}\n\n.jp-theme-editor-button-color {\n  height: var(--jp-ui-font-size0);\n  width: 25px;\n  position: absolute;\n  right: 0;\n  margin-right: 5%;\n}\n\n.form-control {\n  right: 0;\n  width: 95%;\n}\n\n.jp-theme-editor-color-picker {\n  position: relative;\n  left: 0;\n}\n\n.form-class {\n  background-color: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  font-size: var(--jp-ui-font-size0);\n  line-height: 2em;\n}\n\n:root {\n  --jp-ui-font-family: 'Arial', 'Courier', 'Dancing Script', 'Dosis',\n    'Helvetica', 'Lobster', 'JetBrains Mono', 'Pacifico', 'Prompt', 'Righteous',\n    'Sans Serif', 'Satisfy', 'Single Day', 'system-ui', 'Times New Roman',\n    'Urbanist', 'Verdana';\n  --jp-content-font-family: 'Arial', 'Courier', 'Dancing Script', 'Helvetica',\n    'Dosis', 'Lobster', 'JetBrains Mono', 'Pacifico', 'Prompt', 'Righteous',\n    'Sans Serif', 'Satisfy', 'Single Day', 'system-ui', 'Times New Roman',\n    'Urbanist', 'Verdana';\n  --jp-code-font-family: 'monospace', 'Space Mono';\n}\n", ""]);
+            const a = s
         },
         3645: t => {
             t.exports = function(t) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
-                        var o = t(e);
-                        return e[2] ? "@media ".concat(e[2], " {").concat(o, "}") : o
+                        var o = "",
+                            n = void 0 !== e[5];
+                        return e[4] && (o += "@supports (".concat(e[4], ") {")), e[2] && (o += "@media ".concat(e[2], " {")), n && (o += "@layer".concat(e[5].length > 0 ? " ".concat(e[5]) : "", " {")), o += t(e), n && (o += "}"), e[2] && (o += "}"), e[4] && (o += "}"), o
                     })).join("")
-                }, e.i = function(t, o, n) {
+                }, e.i = function(t, o, n, r, i) {
                     "string" == typeof t && (t = [
-                        [null, t, ""]
+                        [null, t, void 0]
                     ]);
-                    var i = {};
+                    var s = {};
                     if (n)
-                        for (var r = 0; r < this.length; r++) {
-                            var s = this[r][0];
-                            null != s && (i[s] = !0)
+                        for (var a = 0; a < this.length; a++) {
+                            var c = this[a][0];
+                            null != c && (s[c] = !0)
                         }
-                    for (var a = 0; a < t.length; a++) {
-                        var c = [].concat(t[a]);
-                        n && i[c[0]] || (o && (c[2] ? c[2] = "".concat(o, " and ").concat(c[2]) : c[2] = o), e.push(c))
+                    for (var p = 0; p < t.length; p++) {
+                        var l = [].concat(t[p]);
+                        n && s[l[0]] || (void 0 !== i && (void 0 === l[5] || (l[1] = "@layer".concat(l[5].length > 0 ? " ".concat(l[5]) : "", " {").concat(l[1], "}")), l[5] = i), o && (l[2] ? (l[1] = "@media ".concat(l[2], " {").concat(l[1], "}"), l[2] = o) : l[2] = o), r && (l[4] ? (l[1] = "@supports (".concat(l[4], ") {").concat(l[1], "}"), l[4] = r) : l[4] = "".concat(r)), e.push(l))
                     }
                 }, e
             }
         },
-        3379: (t, e, o) => {
-            var n, i = function() {
-                    var t = {};
-                    return function(e) {
-                        if (void 0 === t[e]) {
-                            var o = document.querySelector(e);
-                            if (window.HTMLIFrameElement && o instanceof window.HTMLIFrameElement) try {
-                                o = o.contentDocument.head
-                            } catch (t) {
-                                o = null
-                            }
-                            t[e] = o
-                        }
-                        return t[e]
-                    }
-                }(),
-                r = [];
+        8081: t => {
+            t.exports = function(t) {
+                return t[1]
+            }
+        },
+        3379: t => {
+            var e = [];
 
-            function s(t) {
-                for (var e = -1, o = 0; o < r.length; o++)
-                    if (r[o].identifier === t) {
-                        e = o;
+            function o(t) {
+                for (var o = -1, n = 0; n < e.length; n++)
+                    if (e[n].identifier === t) {
+                        o = n;
                         break
-                    } return e
+                    } return o
             }
 
-            function a(t, e) {
-                for (var o = {}, n = [], i = 0; i < t.length; i++) {
-                    var a = t[i],
-                        c = e.base ? a[0] + e.base : a[0],
-                        l = o[c] || 0,
-                        p = "".concat(c, " ").concat(l);
-                    o[c] = l + 1;
-                    var u = s(p),
-                        f = {
-                            css: a[1],
-                            media: a[2],
-                            sourceMap: a[3]
-                        }; - 1 !== u ? (r[u].references++, r[u].updater(f)) : r.push({
-                        identifier: p,
-                        updater: d(f, e),
-                        references: 1
-                    }), n.push(p)
+            function n(t, n) {
+                for (var i = {}, s = [], a = 0; a < t.length; a++) {
+                    var c = t[a],
+                        p = n.base ? c[0] + n.base : c[0],
+                        l = i[p] || 0,
+                        u = "".concat(p, " ").concat(l);
+                    i[p] = l + 1;
+                    var f = o(u),
+                        m = {
+                            css: c[1],
+                            media: c[2],
+                            sourceMap: c[3],
+                            supports: c[4],
+                            layer: c[5]
+                        };
+                    if (-1 !== f) e[f].references++, e[f].updater(m);
+                    else {
+                        var d = r(m, n);
+                        n.byIndex = a, e.splice(a, 0, {
+                            identifier: u,
+                            updater: d,
+                            references: 1
+                        })
+                    }
+                    s.push(u)
                 }
-                return n
+                return s
             }
 
-            function c(t) {
-                var e = document.createElement("style"),
-                    n = t.attributes || {};
-                if (void 0 === n.nonce) {
-                    var r = o.nc;
-                    r && (n.nonce = r)
-                }
-                if (Object.keys(n).forEach((function(t) {
-                        e.setAttribute(t, n[t])
-                    })), "function" == typeof t.insert) t.insert(e);
-                else {
-                    var s = i(t.insert || "head");
-                    if (!s) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    s.appendChild(e)
-                }
-                return e
+            function r(t, e) {
+                var o = e.domAPI(e);
+                return o.update(t),
+                    function(e) {
+                        if (e) {
+                            if (e.css === t.css && e.media === t.media && e.sourceMap === t.sourceMap && e.supports === t.supports && e.layer === t.layer) return;
+                            o.update(t = e)
+                        } else o.remove()
+                    }
             }
-            var l, p = (l = [], function(t, e) {
-                return l[t] = e, l.filter(Boolean).join("\n")
-            });
-
-            function u(t, e, o, n) {
-                var i = o ? "" : n.media ? "@media ".concat(n.media, " {").concat(n.css, "}") : n.css;
-                if (t.styleSheet) t.styleSheet.cssText = p(e, i);
-                else {
-                    var r = document.createTextNode(i),
-                        s = t.childNodes;
-                    s[e] && t.removeChild(s[e]), s.length ? t.insertBefore(r, s[e]) : t.appendChild(r)
+            t.exports = function(t, r) {
+                var i = n(t = t || [], r = r || {});
+                return function(t) {
+                    t = t || [];
+                    for (var s = 0; s < i.length; s++) {
+                        var a = o(i[s]);
+                        e[a].references--
+                    }
+                    for (var c = n(t, r), p = 0; p < i.length; p++) {
+                        var l = o(i[p]);
+                        0 === e[l].references && (e[l].updater(), e.splice(l, 1))
+                    }
+                    i = c
                 }
             }
-
-            function f(t, e, o) {
-                var n = o.css,
-                    i = o.media,
-                    r = o.sourceMap;
-                if (i ? t.setAttribute("media", i) : t.removeAttribute("media"), r && "undefined" != typeof btoa && (n += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), t.styleSheet) t.styleSheet.cssText = n;
-                else {
-                    for (; t.firstChild;) t.removeChild(t.firstChild);
-                    t.appendChild(document.createTextNode(n))
-                }
+        },
+        569: t => {
+            var e = {};
+            t.exports = function(t, o) {
+                var n = function(t) {
+                    if (void 0 === e[t]) {
+                        var o = document.querySelector(t);
+                        if (window.HTMLIFrameElement && o instanceof window.HTMLIFrameElement) try {
+                            o = o.contentDocument.head
+                        } catch (t) {
+                            o = null
+                        }
+                        e[t] = o
+                    }
+                    return e[t]
+                }(t);
+                if (!n) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                n.appendChild(o)
             }
-            var m = null,
-                h = 0;
-
-            function d(t, e) {
-                var o, n, i;
-                if (e.singleton) {
-                    var r = h++;
-                    o = m || (m = c(e)), n = u.bind(null, o, r, !1), i = u.bind(null, o, r, !0)
-                } else o = c(e), n = f.bind(null, o, e), i = function() {
-                    ! function(t) {
-                        if (null === t.parentNode) return !1;
-                        t.parentNode.removeChild(t)
-                    }(o)
+        },
+        9216: t => {
+            t.exports = function(t) {
+                var e = document.createElement("style");
+                return t.setAttributes(e, t.attributes), t.insert(e, t.options), e
+            }
+        },
+        3565: (t, e, o) => {
+            t.exports = function(t) {
+                var e = o.nc;
+                e && t.setAttribute("nonce", e)
+            }
+        },
+        7795: t => {
+            t.exports = function(t) {
+                if ("undefined" == typeof document) return {
+                    update: function() {},
+                    remove: function() {}
                 };
-                return n(t),
-                    function(e) {
-                        if (e) {
-                            if (e.css === t.css && e.media === t.media && e.sourceMap === t.sourceMap) return;
-                            n(t = e)
-                        } else i()
+                var e = t.insertStyleElement(t);
+                return {
+                    update: function(o) {
+                        ! function(t, e, o) {
+                            var n = "";
+                            o.supports && (n += "@supports (".concat(o.supports, ") {")), o.media && (n += "@media ".concat(o.media, " {"));
+                            var r = void 0 !== o.layer;
+                            r && (n += "@layer".concat(o.layer.length > 0 ? " ".concat(o.layer) : "", " {")), n += o.css, r && (n += "}"), o.media && (n += "}"), o.supports && (n += "}");
+                            var i = o.sourceMap;
+                            i && "undefined" != typeof btoa && (n += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), e.styleTagTransform(n, t, e.options)
+                        }(e, t, o)
+                    },
+                    remove: function() {
+                        ! function(t) {
+                            if (null === t.parentNode) return !1;
+                            t.parentNode.removeChild(t)
+                        }(e)
                     }
+                }
             }
+        },
+        4589: t => {
             t.exports = function(t, e) {
-                (e = e || {}).singleton || "boolean" == typeof e.singleton || (e.singleton = (void 0 === n && (n = Boolean(window && document && document.all && !window.atob)), n));
-                var o = a(t = t || [], e);
-                return function(t) {
-                    if (t = t || [], "[object Array]" === Object.prototype.toString.call(t)) {
-                        for (var n = 0; n < o.length; n++) {
-                            var i = s(o[n]);
-                            r[i].references--
-                        }
-                        for (var c = a(t, e), l = 0; l < o.length; l++) {
-                            var p = s(o[l]);
-                            0 === r[p].references && (r[p].updater(), r.splice(p, 1))
-                        }
-                        o = c
-                    }
+                if (e.styleSheet) e.styleSheet.cssText = t;
+                else {
+                    for (; e.firstChild;) e.removeChild(e.firstChild);
+                    e.appendChild(document.createTextNode(t))
                 }
             }
         },
         9747: (t, e, o) => {
             o.r(e);
             var n = o(3379),
-                i = o.n(n),
-                r = o(1150);
-            i()(r.Z, {
-                insert: "head",
-                singleton: !1
-            }), r.Z.locals
+                r = o.n(n),
+                i = o(7795),
+                s = o.n(i),
+                a = o(569),
+                c = o.n(a),
+                p = o(3565),
+                l = o.n(p),
+                u = o(9216),
+                f = o.n(u),
+                m = o(4589),
+                d = o.n(m),
+                h = o(1150),
+                g = {};
+            g.styleTagTransform = d(), g.setAttributes = l(), g.insert = c().bind(null, "head"), g.domAPI = s(), g.insertStyleElement = f(), r()(h.Z, g), h.Z && h.Z.locals && h.Z.locals
         }
     }
 ]);
```

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/785.2fc5bebd96804ab650b2.js` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/304.caed9225fc88627a1ade.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,257 +1,974 @@
 (self.webpackChunkjupyter_theme_editor = self.webpackChunkjupyter_theme_editor || []).push([
-    [785], {
-        8785: (e, t, r) => {
+    [304], {
+        8304: (e, t, r) => {
             "use strict";
 
             function n() {
                 return n = Object.assign ? Object.assign.bind() : function(e) {
                     for (var t = 1; t < arguments.length; t++) {
                         var r = arguments[t];
                         for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
                     }
                     return e
                 }, n.apply(this, arguments)
             }
             r.r(t), r.d(t, {
-                Alpha: () => _,
-                AlphaPicker: () => P,
-                BlockPicker: () => U,
-                Checkboard: () => A,
-                ChromePicker: () => V,
-                CirclePicker: () => Z,
-                CompactPicker: () => Q,
-                CustomPicker: () => D,
-                EditableInput: () => H,
-                GithubPicker: () => te,
-                GooglePicker: () => ie,
-                Hue: () => L,
-                HuePicker: () => le,
-                MaterialPicker: () => se,
-                PhotoshopPicker: () => ge,
-                Raised: () => z,
-                Saturation: () => T,
-                SketchPicker: () => xe,
-                SliderPicker: () => we,
-                Swatch: () => G,
-                SwatchesPicker: () => ke,
-                TwitterPicker: () => Fe
+                Alpha: () => he,
+                AlphaPicker: () => ye,
+                BlockPicker: () => Ee,
+                Checkboard: () => se,
+                ChromePicker: () => Se,
+                CirclePicker: () => Re,
+                CompactPicker: () => De,
+                CustomPicker: () => pe,
+                EditableInput: () => ge,
+                GithubPicker: () => $e,
+                GooglePicker: () => Te,
+                Hue: () => be,
+                HuePicker: () => Oe,
+                MaterialPicker: () => Pe,
+                PhotoshopPicker: () => Ve,
+                Raised: () => fe,
+                Saturation: () => xe,
+                SketchPicker: () => Ze,
+                SliderPicker: () => et,
+                Swatch: () => me,
+                SwatchesPicker: () => at,
+                TwitterPicker: () => it
             });
-            var a = r(6271),
+            var a = r(6029),
                 i = r.n(a),
                 o = r(3279),
                 l = r.n(o),
                 s = r(8446),
-                p = r.n(s),
-                h = r(6073),
-                c = r.n(h),
-                d = r(7621),
-                u = r.n(d);
+                h = r.n(s),
+                p = r(6073),
+                c = r.n(p);
 
-            function g(e) {
-                return g = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+            function d(e) {
+                return d = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                     return typeof e
                 } : function(e) {
                     return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                }, g(e)
+                }, d(e)
             }
+            var u = /^\s+/,
+                g = /\s+$/;
 
-            function b(e, t, r) {
+            function b(e, t) {
+                if (t = t || {}, (e = e || "") instanceof b) return e;
+                if (!(this instanceof b)) return new b(e, t);
+                var r = function(e) {
+                    var t, r, n, a = {
+                            r: 0,
+                            g: 0,
+                            b: 0
+                        },
+                        i = 1,
+                        o = null,
+                        l = null,
+                        s = null,
+                        h = !1,
+                        p = !1;
+                    return "string" == typeof e && (e = function(e) {
+                        e = e.replace(u, "").replace(g, "").toLowerCase();
+                        var t, r = !1;
+                        if (D[e]) e = D[e], r = !0;
+                        else if ("transparent" == e) return {
+                            r: 0,
+                            g: 0,
+                            b: 0,
+                            a: 0,
+                            format: "name"
+                        };
+                        return (t = j.rgb.exec(e)) ? {
+                            r: t[1],
+                            g: t[2],
+                            b: t[3]
+                        } : (t = j.rgba.exec(e)) ? {
+                            r: t[1],
+                            g: t[2],
+                            b: t[3],
+                            a: t[4]
+                        } : (t = j.hsl.exec(e)) ? {
+                            h: t[1],
+                            s: t[2],
+                            l: t[3]
+                        } : (t = j.hsla.exec(e)) ? {
+                            h: t[1],
+                            s: t[2],
+                            l: t[3],
+                            a: t[4]
+                        } : (t = j.hsv.exec(e)) ? {
+                            h: t[1],
+                            s: t[2],
+                            v: t[3]
+                        } : (t = j.hsva.exec(e)) ? {
+                            h: t[1],
+                            s: t[2],
+                            v: t[3],
+                            a: t[4]
+                        } : (t = j.hex8.exec(e)) ? {
+                            r: z(t[1]),
+                            g: z(t[2]),
+                            b: z(t[3]),
+                            a: P(t[4]),
+                            format: r ? "name" : "hex8"
+                        } : (t = j.hex6.exec(e)) ? {
+                            r: z(t[1]),
+                            g: z(t[2]),
+                            b: z(t[3]),
+                            format: r ? "name" : "hex"
+                        } : (t = j.hex4.exec(e)) ? {
+                            r: z(t[1] + "" + t[1]),
+                            g: z(t[2] + "" + t[2]),
+                            b: z(t[3] + "" + t[3]),
+                            a: P(t[4] + "" + t[4]),
+                            format: r ? "name" : "hex8"
+                        } : !!(t = j.hex3.exec(e)) && {
+                            r: z(t[1] + "" + t[1]),
+                            g: z(t[2] + "" + t[2]),
+                            b: z(t[3] + "" + t[3]),
+                            format: r ? "name" : "hex"
+                        }
+                    }(e)), "object" == d(e) && (W(e.r) && W(e.g) && W(e.b) ? (t = e.r, r = e.g, n = e.b, a = {
+                        r: 255 * H(t, 255),
+                        g: 255 * H(r, 255),
+                        b: 255 * H(n, 255)
+                    }, h = !0, p = "%" === String(e.r).substr(-1) ? "prgb" : "rgb") : W(e.h) && W(e.s) && W(e.v) ? (o = G(e.s), l = G(e.v), a = function(e, t, r) {
+                        e = 6 * H(e, 360), t = H(t, 100), r = H(r, 100);
+                        var n = Math.floor(e),
+                            a = e - n,
+                            i = r * (1 - t),
+                            o = r * (1 - a * t),
+                            l = r * (1 - (1 - a) * t),
+                            s = n % 6;
+                        return {
+                            r: 255 * [r, o, i, i, l, r][s],
+                            g: 255 * [l, r, r, o, i, i][s],
+                            b: 255 * [i, i, l, r, r, o][s]
+                        }
+                    }(e.h, o, l), h = !0, p = "hsv") : W(e.h) && W(e.s) && W(e.l) && (o = G(e.s), s = G(e.l), a = function(e, t, r) {
+                        var n, a, i;
+
+                        function o(e, t, r) {
+                            return r < 0 && (r += 1), r > 1 && (r -= 1), r < 1 / 6 ? e + 6 * (t - e) * r : r < .5 ? t : r < 2 / 3 ? e + (t - e) * (2 / 3 - r) * 6 : e
+                        }
+                        if (e = H(e, 360), t = H(t, 100), r = H(r, 100), 0 === t) n = a = i = r;
+                        else {
+                            var l = r < .5 ? r * (1 + t) : r + t - r * t,
+                                s = 2 * r - l;
+                            n = o(s, l, e + 1 / 3), a = o(s, l, e), i = o(s, l, e - 1 / 3)
+                        }
+                        return {
+                            r: 255 * n,
+                            g: 255 * a,
+                            b: 255 * i
+                        }
+                    }(e.h, o, s), h = !0, p = "hsl"), e.hasOwnProperty("a") && (i = e.a)), i = $(i), {
+                        ok: h,
+                        format: e.format || p,
+                        r: Math.min(255, Math.max(a.r, 0)),
+                        g: Math.min(255, Math.max(a.g, 0)),
+                        b: Math.min(255, Math.max(a.b, 0)),
+                        a: i
+                    }
+                }(e);
+                this._originalInput = e, this._r = r.r, this._g = r.g, this._b = r.b, this._a = r.a, this._roundA = Math.round(100 * this._a) / 100, this._format = t.format || r.format, this._gradientType = t.gradientType, this._r < 1 && (this._r = Math.round(this._r)), this._g < 1 && (this._g = Math.round(this._g)), this._b < 1 && (this._b = Math.round(this._b)), this._ok = r.ok
+            }
+
+            function f(e, t, r) {
+                e = H(e, 255), t = H(t, 255), r = H(r, 255);
+                var n, a, i = Math.max(e, t, r),
+                    o = Math.min(e, t, r),
+                    l = (i + o) / 2;
+                if (i == o) n = a = 0;
+                else {
+                    var s = i - o;
+                    switch (a = l > .5 ? s / (2 - i - o) : s / (i + o), i) {
+                        case e:
+                            n = (t - r) / s + (t < r ? 6 : 0);
+                            break;
+                        case t:
+                            n = (r - e) / s + 2;
+                            break;
+                        case r:
+                            n = (e - t) / s + 4
+                    }
+                    n /= 6
+                }
+                return {
+                    h: n,
+                    s: a,
+                    l
+                }
+            }
+
+            function x(e, t, r) {
+                e = H(e, 255), t = H(t, 255), r = H(r, 255);
+                var n, a, i = Math.max(e, t, r),
+                    o = Math.min(e, t, r),
+                    l = i,
+                    s = i - o;
+                if (a = 0 === i ? 0 : s / i, i == o) n = 0;
+                else {
+                    switch (i) {
+                        case e:
+                            n = (t - r) / s + (t < r ? 6 : 0);
+                            break;
+                        case t:
+                            n = (r - e) / s + 2;
+                            break;
+                        case r:
+                            n = (e - t) / s + 4
+                    }
+                    n /= 6
+                }
+                return {
+                    h: n,
+                    s: a,
+                    v: l
+                }
+            }
+
+            function m(e, t, r, n) {
+                var a = [T(Math.round(e).toString(16)), T(Math.round(t).toString(16)), T(Math.round(r).toString(16))];
+                return n && a[0].charAt(0) == a[0].charAt(1) && a[1].charAt(0) == a[1].charAt(1) && a[2].charAt(0) == a[2].charAt(1) ? a[0].charAt(0) + a[1].charAt(0) + a[2].charAt(0) : a.join("")
+            }
+
+            function v(e, t, r, n) {
+                return [T(O(n)), T(Math.round(e).toString(16)), T(Math.round(t).toString(16)), T(Math.round(r).toString(16))].join("")
+            }
+
+            function y(e, t) {
+                t = 0 === t ? 0 : t || 10;
+                var r = b(e).toHsl();
+                return r.s -= t / 100, r.s = L(r.s), b(r)
+            }
+
+            function w(e, t) {
+                t = 0 === t ? 0 : t || 10;
+                var r = b(e).toHsl();
+                return r.s += t / 100, r.s = L(r.s), b(r)
+            }
+
+            function E(e) {
+                return b(e).desaturate(100)
+            }
+
+            function C(e, t) {
+                t = 0 === t ? 0 : t || 10;
+                var r = b(e).toHsl();
+                return r.l += t / 100, r.l = L(r.l), b(r)
+            }
+
+            function k(e, t) {
+                t = 0 === t ? 0 : t || 10;
+                var r = b(e).toRgb();
+                return r.r = Math.max(0, Math.min(255, r.r - Math.round(-t / 100 * 255))), r.g = Math.max(0, Math.min(255, r.g - Math.round(-t / 100 * 255))), r.b = Math.max(0, Math.min(255, r.b - Math.round(-t / 100 * 255))), b(r)
+            }
+
+            function F(e, t) {
+                t = 0 === t ? 0 : t || 10;
+                var r = b(e).toHsl();
+                return r.l -= t / 100, r.l = L(r.l), b(r)
+            }
+
+            function S(e, t) {
+                var r = b(e).toHsl(),
+                    n = (r.h + t) % 360;
+                return r.h = n < 0 ? 360 + n : n, b(r)
+            }
+
+            function B(e) {
+                var t = b(e).toHsl();
+                return t.h = (t.h + 180) % 360, b(t)
+            }
+
+            function M(e, t) {
+                if (isNaN(t) || t <= 0) throw new Error("Argument to polyad must be a positive number");
+                for (var r = b(e).toHsl(), n = [b(e)], a = 360 / t, i = 1; i < t; i++) n.push(b({
+                    h: (r.h + i * a) % 360,
+                    s: r.s,
+                    l: r.l
+                }));
+                return n
+            }
+
+            function R(e) {
+                var t = b(e).toHsl(),
+                    r = t.h;
+                return [b(e), b({
+                    h: (r + 72) % 360,
+                    s: t.s,
+                    l: t.l
+                }), b({
+                    h: (r + 216) % 360,
+                    s: t.s,
+                    l: t.l
+                })]
+            }
+
+            function A(e, t, r) {
+                t = t || 6, r = r || 30;
+                var n = b(e).toHsl(),
+                    a = 360 / r,
+                    i = [b(e)];
+                for (n.h = (n.h - (a * t >> 1) + 720) % 360; --t;) n.h = (n.h + a) % 360, i.push(b(n));
+                return i
+            }
+
+            function _(e, t) {
+                t = t || 6;
+                for (var r = b(e).toHsv(), n = r.h, a = r.s, i = r.v, o = [], l = 1 / t; t--;) o.push(b({
+                    h: n,
+                    s: a,
+                    v: i
+                })), i = (i + l) % 1;
+                return o
+            }
+            b.prototype = {
+                isDark: function() {
+                    return this.getBrightness() < 128
+                },
+                isLight: function() {
+                    return !this.isDark()
+                },
+                isValid: function() {
+                    return this._ok
+                },
+                getOriginalInput: function() {
+                    return this._originalInput
+                },
+                getFormat: function() {
+                    return this._format
+                },
+                getAlpha: function() {
+                    return this._a
+                },
+                getBrightness: function() {
+                    var e = this.toRgb();
+                    return (299 * e.r + 587 * e.g + 114 * e.b) / 1e3
+                },
+                getLuminance: function() {
+                    var e, t, r, n = this.toRgb();
+                    return e = n.r / 255, t = n.g / 255, r = n.b / 255, .2126 * (e <= .03928 ? e / 12.92 : Math.pow((e + .055) / 1.055, 2.4)) + .7152 * (t <= .03928 ? t / 12.92 : Math.pow((t + .055) / 1.055, 2.4)) + .0722 * (r <= .03928 ? r / 12.92 : Math.pow((r + .055) / 1.055, 2.4))
+                },
+                setAlpha: function(e) {
+                    return this._a = $(e), this._roundA = Math.round(100 * this._a) / 100, this
+                },
+                toHsv: function() {
+                    var e = x(this._r, this._g, this._b);
+                    return {
+                        h: 360 * e.h,
+                        s: e.s,
+                        v: e.v,
+                        a: this._a
+                    }
+                },
+                toHsvString: function() {
+                    var e = x(this._r, this._g, this._b),
+                        t = Math.round(360 * e.h),
+                        r = Math.round(100 * e.s),
+                        n = Math.round(100 * e.v);
+                    return 1 == this._a ? "hsv(" + t + ", " + r + "%, " + n + "%)" : "hsva(" + t + ", " + r + "%, " + n + "%, " + this._roundA + ")"
+                },
+                toHsl: function() {
+                    var e = f(this._r, this._g, this._b);
+                    return {
+                        h: 360 * e.h,
+                        s: e.s,
+                        l: e.l,
+                        a: this._a
+                    }
+                },
+                toHslString: function() {
+                    var e = f(this._r, this._g, this._b),
+                        t = Math.round(360 * e.h),
+                        r = Math.round(100 * e.s),
+                        n = Math.round(100 * e.l);
+                    return 1 == this._a ? "hsl(" + t + ", " + r + "%, " + n + "%)" : "hsla(" + t + ", " + r + "%, " + n + "%, " + this._roundA + ")"
+                },
+                toHex: function(e) {
+                    return m(this._r, this._g, this._b, e)
+                },
+                toHexString: function(e) {
+                    return "#" + this.toHex(e)
+                },
+                toHex8: function(e) {
+                    return function(e, t, r, n, a) {
+                        var i = [T(Math.round(e).toString(16)), T(Math.round(t).toString(16)), T(Math.round(r).toString(16)), T(O(n))];
+                        return a && i[0].charAt(0) == i[0].charAt(1) && i[1].charAt(0) == i[1].charAt(1) && i[2].charAt(0) == i[2].charAt(1) && i[3].charAt(0) == i[3].charAt(1) ? i[0].charAt(0) + i[1].charAt(0) + i[2].charAt(0) + i[3].charAt(0) : i.join("")
+                    }(this._r, this._g, this._b, this._a, e)
+                },
+                toHex8String: function(e) {
+                    return "#" + this.toHex8(e)
+                },
+                toRgb: function() {
+                    return {
+                        r: Math.round(this._r),
+                        g: Math.round(this._g),
+                        b: Math.round(this._b),
+                        a: this._a
+                    }
+                },
+                toRgbString: function() {
+                    return 1 == this._a ? "rgb(" + Math.round(this._r) + ", " + Math.round(this._g) + ", " + Math.round(this._b) + ")" : "rgba(" + Math.round(this._r) + ", " + Math.round(this._g) + ", " + Math.round(this._b) + ", " + this._roundA + ")"
+                },
+                toPercentageRgb: function() {
+                    return {
+                        r: Math.round(100 * H(this._r, 255)) + "%",
+                        g: Math.round(100 * H(this._g, 255)) + "%",
+                        b: Math.round(100 * H(this._b, 255)) + "%",
+                        a: this._a
+                    }
+                },
+                toPercentageRgbString: function() {
+                    return 1 == this._a ? "rgb(" + Math.round(100 * H(this._r, 255)) + "%, " + Math.round(100 * H(this._g, 255)) + "%, " + Math.round(100 * H(this._b, 255)) + "%)" : "rgba(" + Math.round(100 * H(this._r, 255)) + "%, " + Math.round(100 * H(this._g, 255)) + "%, " + Math.round(100 * H(this._b, 255)) + "%, " + this._roundA + ")"
+                },
+                toName: function() {
+                    return 0 === this._a ? "transparent" : !(this._a < 1) && (N[m(this._r, this._g, this._b, !0)] || !1)
+                },
+                toFilter: function(e) {
+                    var t = "#" + v(this._r, this._g, this._b, this._a),
+                        r = t,
+                        n = this._gradientType ? "GradientType = 1, " : "";
+                    if (e) {
+                        var a = b(e);
+                        r = "#" + v(a._r, a._g, a._b, a._a)
+                    }
+                    return "progid:DXImageTransform.Microsoft.gradient(" + n + "startColorstr=" + t + ",endColorstr=" + r + ")"
+                },
+                toString: function(e) {
+                    var t = !!e;
+                    e = e || this._format;
+                    var r = !1,
+                        n = this._a < 1 && this._a >= 0;
+                    return t || !n || "hex" !== e && "hex6" !== e && "hex3" !== e && "hex4" !== e && "hex8" !== e && "name" !== e ? ("rgb" === e && (r = this.toRgbString()), "prgb" === e && (r = this.toPercentageRgbString()), "hex" !== e && "hex6" !== e || (r = this.toHexString()), "hex3" === e && (r = this.toHexString(!0)), "hex4" === e && (r = this.toHex8String(!0)), "hex8" === e && (r = this.toHex8String()), "name" === e && (r = this.toName()), "hsl" === e && (r = this.toHslString()), "hsv" === e && (r = this.toHsvString()), r || this.toHexString()) : "name" === e && 0 === this._a ? this.toName() : this.toRgbString()
+                },
+                clone: function() {
+                    return b(this.toString())
+                },
+                _applyModification: function(e, t) {
+                    var r = e.apply(null, [this].concat([].slice.call(t)));
+                    return this._r = r._r, this._g = r._g, this._b = r._b, this.setAlpha(r._a), this
+                },
+                lighten: function() {
+                    return this._applyModification(C, arguments)
+                },
+                brighten: function() {
+                    return this._applyModification(k, arguments)
+                },
+                darken: function() {
+                    return this._applyModification(F, arguments)
+                },
+                desaturate: function() {
+                    return this._applyModification(y, arguments)
+                },
+                saturate: function() {
+                    return this._applyModification(w, arguments)
+                },
+                greyscale: function() {
+                    return this._applyModification(E, arguments)
+                },
+                spin: function() {
+                    return this._applyModification(S, arguments)
+                },
+                _applyCombination: function(e, t) {
+                    return e.apply(null, [this].concat([].slice.call(t)))
+                },
+                analogous: function() {
+                    return this._applyCombination(A, arguments)
+                },
+                complement: function() {
+                    return this._applyCombination(B, arguments)
+                },
+                monochromatic: function() {
+                    return this._applyCombination(_, arguments)
+                },
+                splitcomplement: function() {
+                    return this._applyCombination(R, arguments)
+                },
+                triad: function() {
+                    return this._applyCombination(M, [3])
+                },
+                tetrad: function() {
+                    return this._applyCombination(M, [4])
+                }
+            }, b.fromRatio = function(e, t) {
+                if ("object" == d(e)) {
+                    var r = {};
+                    for (var n in e) e.hasOwnProperty(n) && (r[n] = "a" === n ? e[n] : G(e[n]));
+                    e = r
+                }
+                return b(e, t)
+            }, b.equals = function(e, t) {
+                return !(!e || !t) && b(e).toRgbString() == b(t).toRgbString()
+            }, b.random = function() {
+                return b.fromRatio({
+                    r: Math.random(),
+                    g: Math.random(),
+                    b: Math.random()
+                })
+            }, b.mix = function(e, t, r) {
+                r = 0 === r ? 0 : r || 50;
+                var n = b(e).toRgb(),
+                    a = b(t).toRgb(),
+                    i = r / 100;
+                return b({
+                    r: (a.r - n.r) * i + n.r,
+                    g: (a.g - n.g) * i + n.g,
+                    b: (a.b - n.b) * i + n.b,
+                    a: (a.a - n.a) * i + n.a
+                })
+            }, b.readability = function(e, t) {
+                var r = b(e),
+                    n = b(t);
+                return (Math.max(r.getLuminance(), n.getLuminance()) + .05) / (Math.min(r.getLuminance(), n.getLuminance()) + .05)
+            }, b.isReadable = function(e, t, r) {
+                var n, a, i, o, l, s = b.readability(e, t);
+                switch (a = !1, (i = r, "AA" !== (o = ((i = i || {
+                        level: "AA",
+                        size: "small"
+                    }).level || "AA").toUpperCase()) && "AAA" !== o && (o = "AA"), "small" !== (l = (i.size || "small").toLowerCase()) && "large" !== l && (l = "small"), n = {
+                        level: o,
+                        size: l
+                    }).level + n.size) {
+                    case "AAsmall":
+                    case "AAAlarge":
+                        a = s >= 4.5;
+                        break;
+                    case "AAlarge":
+                        a = s >= 3;
+                        break;
+                    case "AAAsmall":
+                        a = s >= 7
+                }
+                return a
+            }, b.mostReadable = function(e, t, r) {
+                var n, a, i, o, l = null,
+                    s = 0;
+                a = (r = r || {}).includeFallbackColors, i = r.level, o = r.size;
+                for (var h = 0; h < t.length; h++)(n = b.readability(e, t[h])) > s && (s = n, l = b(t[h]));
+                return b.isReadable(e, l, {
+                    level: i,
+                    size: o
+                }) || !a ? l : (r.includeFallbackColors = !1, b.mostReadable(e, ["#fff", "#000"], r))
+            };
+            var D = b.names = {
+                    aliceblue: "f0f8ff",
+                    antiquewhite: "faebd7",
+                    aqua: "0ff",
+                    aquamarine: "7fffd4",
+                    azure: "f0ffff",
+                    beige: "f5f5dc",
+                    bisque: "ffe4c4",
+                    black: "000",
+                    blanchedalmond: "ffebcd",
+                    blue: "00f",
+                    blueviolet: "8a2be2",
+                    brown: "a52a2a",
+                    burlywood: "deb887",
+                    burntsienna: "ea7e5d",
+                    cadetblue: "5f9ea0",
+                    chartreuse: "7fff00",
+                    chocolate: "d2691e",
+                    coral: "ff7f50",
+                    cornflowerblue: "6495ed",
+                    cornsilk: "fff8dc",
+                    crimson: "dc143c",
+                    cyan: "0ff",
+                    darkblue: "00008b",
+                    darkcyan: "008b8b",
+                    darkgoldenrod: "b8860b",
+                    darkgray: "a9a9a9",
+                    darkgreen: "006400",
+                    darkgrey: "a9a9a9",
+                    darkkhaki: "bdb76b",
+                    darkmagenta: "8b008b",
+                    darkolivegreen: "556b2f",
+                    darkorange: "ff8c00",
+                    darkorchid: "9932cc",
+                    darkred: "8b0000",
+                    darksalmon: "e9967a",
+                    darkseagreen: "8fbc8f",
+                    darkslateblue: "483d8b",
+                    darkslategray: "2f4f4f",
+                    darkslategrey: "2f4f4f",
+                    darkturquoise: "00ced1",
+                    darkviolet: "9400d3",
+                    deeppink: "ff1493",
+                    deepskyblue: "00bfff",
+                    dimgray: "696969",
+                    dimgrey: "696969",
+                    dodgerblue: "1e90ff",
+                    firebrick: "b22222",
+                    floralwhite: "fffaf0",
+                    forestgreen: "228b22",
+                    fuchsia: "f0f",
+                    gainsboro: "dcdcdc",
+                    ghostwhite: "f8f8ff",
+                    gold: "ffd700",
+                    goldenrod: "daa520",
+                    gray: "808080",
+                    green: "008000",
+                    greenyellow: "adff2f",
+                    grey: "808080",
+                    honeydew: "f0fff0",
+                    hotpink: "ff69b4",
+                    indianred: "cd5c5c",
+                    indigo: "4b0082",
+                    ivory: "fffff0",
+                    khaki: "f0e68c",
+                    lavender: "e6e6fa",
+                    lavenderblush: "fff0f5",
+                    lawngreen: "7cfc00",
+                    lemonchiffon: "fffacd",
+                    lightblue: "add8e6",
+                    lightcoral: "f08080",
+                    lightcyan: "e0ffff",
+                    lightgoldenrodyellow: "fafad2",
+                    lightgray: "d3d3d3",
+                    lightgreen: "90ee90",
+                    lightgrey: "d3d3d3",
+                    lightpink: "ffb6c1",
+                    lightsalmon: "ffa07a",
+                    lightseagreen: "20b2aa",
+                    lightskyblue: "87cefa",
+                    lightslategray: "789",
+                    lightslategrey: "789",
+                    lightsteelblue: "b0c4de",
+                    lightyellow: "ffffe0",
+                    lime: "0f0",
+                    limegreen: "32cd32",
+                    linen: "faf0e6",
+                    magenta: "f0f",
+                    maroon: "800000",
+                    mediumaquamarine: "66cdaa",
+                    mediumblue: "0000cd",
+                    mediumorchid: "ba55d3",
+                    mediumpurple: "9370db",
+                    mediumseagreen: "3cb371",
+                    mediumslateblue: "7b68ee",
+                    mediumspringgreen: "00fa9a",
+                    mediumturquoise: "48d1cc",
+                    mediumvioletred: "c71585",
+                    midnightblue: "191970",
+                    mintcream: "f5fffa",
+                    mistyrose: "ffe4e1",
+                    moccasin: "ffe4b5",
+                    navajowhite: "ffdead",
+                    navy: "000080",
+                    oldlace: "fdf5e6",
+                    olive: "808000",
+                    olivedrab: "6b8e23",
+                    orange: "ffa500",
+                    orangered: "ff4500",
+                    orchid: "da70d6",
+                    palegoldenrod: "eee8aa",
+                    palegreen: "98fb98",
+                    paleturquoise: "afeeee",
+                    palevioletred: "db7093",
+                    papayawhip: "ffefd5",
+                    peachpuff: "ffdab9",
+                    peru: "cd853f",
+                    pink: "ffc0cb",
+                    plum: "dda0dd",
+                    powderblue: "b0e0e6",
+                    purple: "800080",
+                    rebeccapurple: "663399",
+                    red: "f00",
+                    rosybrown: "bc8f8f",
+                    royalblue: "4169e1",
+                    saddlebrown: "8b4513",
+                    salmon: "fa8072",
+                    sandybrown: "f4a460",
+                    seagreen: "2e8b57",
+                    seashell: "fff5ee",
+                    sienna: "a0522d",
+                    silver: "c0c0c0",
+                    skyblue: "87ceeb",
+                    slateblue: "6a5acd",
+                    slategray: "708090",
+                    slategrey: "708090",
+                    snow: "fffafa",
+                    springgreen: "00ff7f",
+                    steelblue: "4682b4",
+                    tan: "d2b48c",
+                    teal: "008080",
+                    thistle: "d8bfd8",
+                    tomato: "ff6347",
+                    turquoise: "40e0d0",
+                    violet: "ee82ee",
+                    wheat: "f5deb3",
+                    white: "fff",
+                    whitesmoke: "f5f5f5",
+                    yellow: "ff0",
+                    yellowgreen: "9acd32"
+                },
+                N = b.hexNames = function(e) {
+                    var t = {};
+                    for (var r in e) e.hasOwnProperty(r) && (t[e[r]] = r);
+                    return t
+                }(D);
+
+            function $(e) {
+                return e = parseFloat(e), (isNaN(e) || e < 0 || e > 1) && (e = 1), e
+            }
+
+            function H(e, t) {
+                (function(e) {
+                    return "string" == typeof e && -1 != e.indexOf(".") && 1 === parseFloat(e)
+                })(e) && (e = "100%");
+                var r = function(e) {
+                    return "string" == typeof e && -1 != e.indexOf("%")
+                }(e);
+                return e = Math.min(t, Math.max(0, parseFloat(e))), r && (e = parseInt(e * t, 10) / 100), Math.abs(e - t) < 1e-6 ? 1 : e % t / parseFloat(t)
+            }
+
+            function L(e) {
+                return Math.min(1, Math.max(0, e))
+            }
+
+            function z(e) {
+                return parseInt(e, 16)
+            }
+
+            function T(e) {
+                return 1 == e.length ? "0" + e : "" + e
+            }
+
+            function G(e) {
+                return e <= 1 && (e = 100 * e + "%"), e
+            }
+
+            function O(e) {
+                return Math.round(255 * parseFloat(e)).toString(16)
+            }
+
+            function P(e) {
+                return z(e) / 255
+            }
+            var X, U, I, j = (U = "[\\s|\\(]+(" + (X = "(?:[-\\+]?\\d*\\.\\d+%?)|(?:[-\\+]?\\d+%?)") + ")[,|\\s]+(" + X + ")[,|\\s]+(" + X + ")\\s*\\)?", I = "[\\s|\\(]+(" + X + ")[,|\\s]+(" + X + ")[,|\\s]+(" + X + ")[,|\\s]+(" + X + ")\\s*\\)?", {
+                CSS_UNIT: new RegExp(X),
+                rgb: new RegExp("rgb" + U),
+                rgba: new RegExp("rgba" + I),
+                hsl: new RegExp("hsl" + U),
+                hsla: new RegExp("hsla" + I),
+                hsv: new RegExp("hsv" + U),
+                hsva: new RegExp("hsva" + I),
+                hex3: /^#?([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})$/,
+                hex6: /^#?([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})$/,
+                hex4: /^#?([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})$/,
+                hex8: /^#?([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})$/
+            });
+
+            function W(e) {
+                return !!j.CSS_UNIT.exec(e)
+            }
+
+            function V(e) {
+                return V = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                    return typeof e
+                } : function(e) {
+                    return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+                }, V(e)
+            }
+
+            function Y(e, t, r) {
                 return (t = function(e) {
                     var t = function(e, t) {
-                        if ("object" !== g(e) || null === e) return e;
+                        if ("object" !== V(e) || null === e) return e;
                         var r = e[Symbol.toPrimitive];
                         if (void 0 !== r) {
                             var n = r.call(e, "string");
-                            if ("object" !== g(n)) return n;
+                            if ("object" !== V(n)) return n;
                             throw new TypeError("@@toPrimitive must return a primitive value.")
                         }
                         return String(e)
                     }(e);
-                    return "symbol" === g(t) ? t : String(t)
+                    return "symbol" === V(t) ? t : String(t)
                 }(t)) in e ? Object.defineProperty(e, t, {
                     value: r,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = r, e
             }
-            var f = r(3857),
-                x = r.n(f);
-            const m = e => {
+            var q = r(3857),
+                Z = r.n(q);
+            const K = e => {
                     let t = 0,
                         r = 0;
                     return c()(["r", "g", "b", "a", "h", "s", "l", "v"], (n => {
                         e[n] && (t += 1, isNaN(e[n]) || (r += 1), "s" === n || "l" === n) && /^\d+%$/.test(e[n]) && (r += 1)
                     })), t === r && e
                 },
-                v = (e, t) => {
-                    const r = e.hex ? u()(e.hex) : u()(e),
+                J = (e, t) => {
+                    const r = e.hex ? b(e.hex) : b(e),
                         n = r.toHsl(),
                         a = r.toHsv(),
                         i = r.toRgb(),
                         o = r.toHex();
                     return 0 === n.s && (n.h = t || 0, a.h = t || 0), {
                         hsl: n,
                         hex: "000000" === o && 0 === i.a ? "transparent" : `#${o}`,
                         rgb: i,
                         hsv: a,
                         oldHue: e.h || t || n.h,
                         source: e.source
                     }
                 },
-                y = e => {
+                Q = e => {
                     if ("transparent" === e) return !0;
                     const t = "#" === String(e).charAt(0) ? 1 : 0;
-                    return e.length !== 4 + t && e.length < 7 + t && u()(e).isValid()
+                    return e.length !== 4 + t && e.length < 7 + t && b(e).isValid()
                 },
-                w = e => {
+                ee = e => {
                     if (!e) return "#fff";
-                    const t = v(e);
+                    const t = J(e);
                     return "transparent" === t.hex ? "rgba(0,0,0,0.4)" : (299 * t.rgb.r + 587 * t.rgb.g + 114 * t.rgb.b) / 1e3 >= 128 ? "#000" : "#fff"
                 },
-                E = (e, t) => {
-                    const r = e.replace("°", "");
-                    return u()(`${t} (${r})`)._ok
-                },
-                C = (0, a.createContext)(void 0);
+                te = (e, t) => b(`${t} (${e.replace("°","")})`)._ok,
+                re = (0, a.createContext)(void 0);
 
-            function k(e) {
+            function ne(e) {
                 let {
                     children: t,
                     onChangeComplete: r,
                     onChange: n,
                     onSwatchHover: o,
                     color: s,
-                    defaultColor: h = {
+                    defaultColor: p = {
                         h: 250,
                         s: .5,
                         l: .2,
                         a: 1
                     }
                 } = e;
                 const [c, d] = (0, a.useState)({
-                    ...v(s ?? h, 0)
+                    ...J(s ?? p, 0)
                 }), u = (0, a.useRef)(s);
-                p()(u.current, s) || (u.current = s), (0, a.useEffect)((() => {
+                h()(u.current, s) || (u.current = s), (0, a.useEffect)((() => {
                     s && d({
-                        ...v(s, 0)
+                        ...J(s, 0)
                     })
                 }), [u.current]);
                 const g = (e, t, r) => e(t, r),
                     b = (0, a.useMemo)((() => l()(g, 100)), []);
-                return i().createElement(C.Provider, {
+                return i().createElement(re.Provider, {
                     value: {
                         colors: c,
                         changeColor: function(e, t) {
-                            if (m(e)) {
-                                const a = v(e, ("string" != typeof e && "h" in e ? e.h : void 0) || c.oldHue);
+                            if (K(e)) {
+                                const a = J(e, ("string" != typeof e && "h" in e ? e.h : void 0) || c.oldHue);
                                 d(a), r && b(r, a, t), n && n(a, t)
                             }
                         },
                         onSwatchHover: o ? function(e, t) {
-                            if (m(e)) {
-                                const r = v(e, ("string" != typeof e && "h" in e ? e.h : void 0) || c.oldHue);
+                            if (K(e)) {
+                                const r = J(e, ("string" != typeof e && "h" in e ? e.h : void 0) || c.oldHue);
                                 o && o(r, t)
                             }
                         } : void 0
                     }
                 }, t)
             }
-            const F = () => (0, a.useContext)(C),
-                S = e => t => i().createElement(k, t, i().createElement(e, t)),
-                B = {},
-                R = (e, t, r, n) => {
+            const ae = () => (0, a.useContext)(re),
+                ie = e => t => i().createElement(ne, t, i().createElement(e, t)),
+                oe = {},
+                le = (e, t, r, n) => {
                     const a = `${e}-${t}-${r}${n?"-server":""}`;
-                    if (B[a]) return B[a];
+                    if (oe[a]) return oe[a];
                     const i = ((e, t, r, n) => {
                         if ("undefined" == typeof document && !n) return null;
                         const a = n ? new n : document.createElement("canvas");
                         a.width = 2 * r, a.height = 2 * r;
                         const i = a.getContext("2d");
                         return i ? (i.fillStyle = e, i.fillRect(0, 0, a.width, a.height), i.fillStyle = t, i.fillRect(0, 0, r, r), i.translate(r, r), i.fillRect(0, 0, r, r), a.toDataURL()) : null
                     })(e, t, r, n);
-                    return B[a] = i, i
+                    return oe[a] = i, i
                 };
 
-            function A(e) {
+            function se(e) {
                 let {
                     white: t = "transparent",
                     grey: r = "rgba(0,0,0,.08)",
                     size: n = 8,
                     renderers: o = {},
                     borderRadius: l,
                     boxShadow: s,
-                    children: p
+                    children: h
                 } = e;
-                const h = {
+                const p = {
                     grid: {
                         borderRadius: l,
                         boxShadow: s,
                         position: "absolute",
                         inset: "0px",
-                        background: `url(${R(t,r,n,o.canvas)}) center left`
+                        background: `url(${le(t,r,n,o.canvas)}) center left`
                     }
                 };
-                return (0, a.isValidElement)(p) ? i().cloneElement(p, {
-                    ...p.props,
+                return (0, a.isValidElement)(h) ? i().cloneElement(h, {
+                    ...h.props,
                     style: {
-                        ...p.props.style,
-                        ...h.grid
+                        ...h.props.style,
+                        ...p.grid
                     }
                 }) : i().createElement("div", {
-                    style: h.grid
+                    style: p.grid
                 })
             }
-            var _ = class extends(a.PureComponent || a.Component) {
+            var he = class extends(a.PureComponent || a.Component) {
                     constructor() {
-                        super(...arguments), b(this, "handleChange", (e => {
+                        super(...arguments), Y(this, "handleChange", (e => {
                             const t = ((e, t, r, n, a) => {
                                 const i = a.clientWidth,
                                     o = a.clientHeight,
                                     l = "number" == typeof e.pageX ? e.pageX : e.touches[0].pageX,
                                     s = "number" == typeof e.pageY ? e.pageY : e.touches[0].pageY,
-                                    p = l - (a.getBoundingClientRect().left + window.pageXOffset),
-                                    h = s - (a.getBoundingClientRect().top + window.pageYOffset);
+                                    h = l - (a.getBoundingClientRect().left + window.pageXOffset),
+                                    p = s - (a.getBoundingClientRect().top + window.pageYOffset);
                                 if ("vertical" === r) {
                                     let e;
-                                    if (e = h < 0 ? 0 : h > o ? 1 : Math.round(100 * h / o) / 100, t.a !== e) return {
+                                    if (e = p < 0 ? 0 : p > o ? 1 : Math.round(100 * p / o) / 100, t.a !== e) return {
                                         h: t.h,
                                         s: t.s,
                                         l: t.l,
                                         a: e,
                                         source: "rgb"
                                     }
                                 } else {
                                     let e;
-                                    if (e = p < 0 ? 0 : p > i ? 1 : Math.round(100 * p / i) / 100, n !== e) return {
+                                    if (e = h < 0 ? 0 : h > i ? 1 : Math.round(100 * h / i) / 100, n !== e) return {
                                         h: t.h,
                                         s: t.s,
                                         l: t.l,
                                         a: e,
                                         source: "rgb"
                                     }
                                 }
                                 return null
                             })(e, this.props.hsl, this.props.direction, this.props.a, this.container);
                             t && "function" == typeof this.props.onChange && this.props.onChange(t, e)
-                        })), b(this, "handleMouseDown", (e => {
+                        })), Y(this, "handleMouseDown", (e => {
                             this.handleChange(e), window.addEventListener("mousemove", this.handleChange), window.addEventListener("mouseup", this.handleMouseUp)
-                        })), b(this, "handleMouseUp", (() => {
+                        })), Y(this, "handleMouseUp", (() => {
                             this.unbindEventListeners()
-                        })), b(this, "unbindEventListeners", (() => {
+                        })), Y(this, "unbindEventListeners", (() => {
                             window.removeEventListener("mousemove", this.handleChange), window.removeEventListener("mouseup", this.handleMouseUp)
                         }))
                     }
                     componentWillUnmount() {
                         this.unbindEventListeners()
                     }
                     render() {
                         const e = this.props.rgb,
-                            t = x()({
+                            t = Z()({
                                 alpha: {
                                     position: "absolute",
                                     inset: "0px",
                                     borderRadius: this.props.radius
                                 },
                                 checkboard: {
                                     position: "absolute",
@@ -286,15 +1003,15 @@
                                     transform: "translateX(-2px)"
                                 }
                             }, this.props.style);
                         return i().createElement("div", {
                             style: t.alpha
                         }, i().createElement("div", {
                             style: t.checkboard
-                        }, i().createElement(A, {
+                        }, i().createElement(se, {
                             renderers: this.props.renderers
                         })), i().createElement("div", {
                             style: t.gradient
                         }), i().createElement("div", {
                             style: t.container,
                             ref: e => this.container = e,
                             onMouseDown: this.handleMouseDown,
@@ -303,68 +1020,68 @@
                         }, i().createElement("div", {
                             style: t.pointer
                         }, this.props.pointer ? i().createElement(this.props.pointer, this.props) : i().createElement("div", {
                             style: t.slider
                         }))))
                     }
                 },
-                D = e => S((function(t) {
+                pe = e => ie((function(t) {
                     let {
                         onSwatchHover: r,
                         onChangeComplete: a,
                         color: o,
                         defaultColor: l
                     } = t;
                     const {
                         colors: s,
-                        changeColor: p
-                    } = F();
-                    return i().createElement(k, {
+                        changeColor: h
+                    } = ae();
+                    return i().createElement(ne, {
                         color: o,
                         defaultColor: l,
                         onChangeComplete: a,
                         onSwatchHover: r
                     }, i().createElement(e, n({}, s, {
-                        onChange: p
+                        onChange: h
                     })))
                 }));
-            const M = [38, 40];
-            let N = 1;
-            class $ extends(a.PureComponent || a.Component) {
+            const ce = [38, 40];
+            let de = 1;
+            class ue extends(a.PureComponent || a.Component) {
                 constructor(e) {
-                    super(), b(this, "handleBlur", (() => {
+                    super(), Y(this, "handleBlur", (() => {
                         this.state.blurValue && this.setState({
                             value: this.state.blurValue,
                             blurValue: null
                         })
-                    })), b(this, "handleChange", (e => {
+                    })), Y(this, "handleChange", (e => {
                         this.setUpdatedValue(e.target.value, e)
-                    })), b(this, "handleKeyDown", (e => {
+                    })), Y(this, "handleKeyDown", (e => {
                         const t = (e => Number(String(e).replace(/%/g, "")))(e.target.value);
-                        if (!isNaN(t) && (r = e.keyCode, M.indexOf(r) > -1)) {
+                        if (!isNaN(t) && (r = e.keyCode, ce.indexOf(r) > -1)) {
                             const r = this.getArrowOffset(),
                                 n = 38 === e.keyCode ? t + r : t - r;
                             this.setUpdatedValue(n, e)
                         }
                         var r
-                    })), b(this, "handleDrag", (e => {
+                    })), Y(this, "handleDrag", (e => {
                         if (this.props.dragLabel) {
                             const t = Math.round(this.props.value + e.movementX);
                             t >= 0 && t <= this.props.dragMax && this.props.onChange && this.props.onChange(this.getValueObjectWithLabel(t), e)
                         }
-                    })), b(this, "handleMouseDown", (e => {
+                    })), Y(this, "handleMouseDown", (e => {
                         this.props.dragLabel && (e.preventDefault(), this.handleDrag(e), window.addEventListener("mousemove", this.handleDrag), window.addEventListener("mouseup", this.handleMouseUp))
-                    })), b(this, "handleMouseUp", (() => {
+                    })), Y(this, "handleMouseUp", (() => {
                         this.unbindEventListeners()
-                    })), b(this, "unbindEventListeners", (() => {
+                    })), Y(this, "unbindEventListeners", (() => {
                         window.removeEventListener("mousemove", this.handleDrag), window.removeEventListener("mouseup", this.handleMouseUp)
                     })), this.state = {
                         value: String(e.value).toUpperCase(),
                         blurValue: String(e.value).toUpperCase()
-                    }, this.inputId = "rc-editable-input-" + N++
+                    }, this.inputId = "rc-editable-input-" + de++
                 }
                 componentDidUpdate(e, t) {
                     this.props.value === this.state.value || e.value === this.props.value && t.value === this.state.value || (this.input === document.activeElement ? this.setState({
                         blurValue: String(this.props.value).toUpperCase()
                     }) : this.setState({
                         value: String(this.props.value).toUpperCase(),
                         blurValue: !this.state.blurValue && String(this.props.value).toUpperCase()
@@ -418,28 +1135,28 @@
                     }), this.props.label && !this.props.hideLabel ? i().createElement("label", {
                         htmlFor: this.inputId,
                         style: e.label,
                         onMouseDown: this.handleMouseDown
                     }, this.props.label) : null)
                 }
             }
-            var H = $,
-                L = class extends(a.PureComponent || a.Component) {
+            var ge = ue,
+                be = class extends(a.PureComponent || a.Component) {
                     constructor() {
-                        super(...arguments), b(this, "handleChange", (e => {
+                        super(...arguments), Y(this, "handleChange", (e => {
                             const t = ((e, t, r, n) => {
                                 const a = n.clientWidth,
                                     i = n.clientHeight,
                                     o = "number" == typeof e.pageX ? e.pageX : e.touches[0].pageX,
                                     l = "number" == typeof e.pageY ? e.pageY : e.touches[0].pageY,
                                     s = o - (n.getBoundingClientRect().left + window.pageXOffset),
-                                    p = l - (n.getBoundingClientRect().top + window.pageYOffset);
+                                    h = l - (n.getBoundingClientRect().top + window.pageYOffset);
                                 if ("vertical" === t) {
                                     let e;
-                                    if (e = p < 0 ? 359 : p > i ? 0 : 360 * (-100 * p / i + 100) / 100, r.h !== e) return {
+                                    if (e = h < 0 ? 359 : h > i ? 0 : 360 * (-100 * h / i + 100) / 100, r.h !== e) return {
                                         h: e,
                                         s: r.s,
                                         l: r.l,
                                         a: r.a,
                                         source: "hsl"
                                     }
                                 } else {
@@ -451,17 +1168,17 @@
                                         a: r.a,
                                         source: "hsl"
                                     }
                                 }
                                 return null
                             })(e, this.props.direction, this.props.hsl, this.container);
                             t && "function" == typeof this.props.onChange && this.props.onChange(t, e)
-                        })), b(this, "handleMouseDown", (e => {
+                        })), Y(this, "handleMouseDown", (e => {
                             this.handleChange(e), window.addEventListener("mousemove", this.handleChange), window.addEventListener("mouseup", this.handleMouseUp)
-                        })), b(this, "handleMouseUp", (() => {
+                        })), Y(this, "handleMouseUp", (() => {
                             this.unbindEventListeners()
                         }))
                     }
                     componentWillUnmount() {
                         this.unbindEventListeners()
                     }
                     unbindEventListeners() {
@@ -511,23 +1228,23 @@
                             style: t.pointer
                         }, this.props.pointer ? i().createElement(this.props.pointer, this.props) : i().createElement("div", {
                             style: t.slider
                         }))))
                     }
                 };
 
-            function z(e) {
+            function fe(e) {
                 let {
                     zDepth: t = 1,
                     radius: r = 2,
                     background: n = "#fff",
                     children: a,
                     styles: o = {}
                 } = e;
-                const l = x()({
+                const l = Z()({
                     wrap: {
                         position: "relative",
                         display: "inline-block"
                     },
                     content: {
                         position: "relative"
                     },
@@ -544,64 +1261,64 @@
                 }, i().createElement("div", {
                     style: l.bg
                 }), i().createElement("div", {
                     style: l.content
                 }, a))
             }
 
-            function T(e) {
+            function xe(e) {
                 let {
                     hsl: t,
                     hsv: r,
                     pointer: n,
                     onChange: o,
                     shadow: l,
                     radius: s,
-                    style: p
+                    style: h
                 } = e;
-                const h = (0, a.useRef)(null);
+                const p = (0, a.useRef)(null);
 
                 function c(e) {
                     o && o(function(e, t, r) {
                         const {
                             width: n,
                             height: a
                         } = r.getBoundingClientRect(), i = "number" == typeof e.pageX ? e.pageX : e.touches[0].pageX, o = "number" == typeof e.pageY ? e.pageY : e.touches[0].pageY;
                         let l = i - (r.getBoundingClientRect().left + window.pageXOffset),
                             s = o - (r.getBoundingClientRect().top + window.pageYOffset);
                         l < 0 ? l = 0 : l > n && (l = n), s < 0 ? s = 0 : s > a && (s = a);
-                        const p = l / n,
-                            h = 1 - s / a;
+                        const h = l / n,
+                            p = 1 - s / a;
                         return {
                             h: t.h,
-                            s: p,
-                            v: h,
+                            s: h,
+                            v: p,
                             a: t.a,
                             source: "hsv"
                         }
-                    }(e, t, h.current), e)
+                    }(e, t, p.current), e)
                 }
 
                 function d() {
                     u()
                 }
 
                 function u() {
-                    h.current && (h.current.removeEventListener("mousemove", c), h.current.removeEventListener("mouseup", d))
+                    p.current && (p.current.removeEventListener("mousemove", c), p.current.removeEventListener("mouseup", d))
                 }(0, a.useEffect)((() => () => {
                     u()
                 }), []);
                 const {
                     color: g,
                     white: b,
                     black: f,
-                    pointer: m,
-                    circle: v
-                } = p || {};
-                let y = {
+                    pointer: x,
+                    circle: m
+                } = h || {};
+                let v = {
                     color: {
                         position: "absolute",
                         inset: "0px",
                         background: `hsl(${t.h},100%, 50%)`,
                         borderRadius: s
                     },
                     white: {
@@ -626,49 +1343,49 @@
                         height: "4px",
                         boxShadow: "0 0 0 1.5px #fff, inset 0 0 1px 1px rgba(0,0,0,.3),\n            0 0 1px 2px rgba(0,0,0,.4)",
                         borderRadius: "50%",
                         cursor: "hand",
                         transform: "translate(-2px, -2px)"
                     }
                 };
-                return p && (y = x()(y, {
+                return h && (v = Z()(v, {
                     color: g,
                     white: b,
                     black: f,
-                    stylePointer: m,
-                    circle: v
+                    stylePointer: x,
+                    circle: m
                 })), i().createElement("div", {
-                    style: y.color,
-                    ref: h,
+                    style: v.color,
+                    ref: p,
                     onMouseDown: function(e) {
-                        c(e), h.current && (h.current.addEventListener("mousemove", c), h.current.addEventListener("mouseup", d))
+                        c(e), p.current && (p.current.addEventListener("mousemove", c), p.current.addEventListener("mouseup", d))
                     },
                     onTouchMove: c,
                     onTouchStart: c
                 }, i().createElement("style", null, "\n          .saturation-white {\n            background: -webkit-linear-gradient(to right, #fff, rgba(255,255,255,0));\n            background: linear-gradient(to right, #fff, rgba(255,255,255,0));\n          }\n          .saturation-black {\n            background: -webkit-linear-gradient(to top, #000, rgba(0,0,0,0));\n            background: linear-gradient(to top, #000, rgba(0,0,0,0));\n          }\n        "), i().createElement("div", {
-                    style: y.white,
+                    style: v.white,
                     className: "saturation-white"
                 }, i().createElement("div", {
-                    style: y.black,
+                    style: v.black,
                     className: "saturation-black"
                 }), i().createElement("div", {
-                    style: y.pointer
+                    style: v.pointer
                 }, n || i().createElement("div", {
-                    style: y.circle
+                    style: v.circle
                 }))))
             }
-            var G = function(e) {
+            var me = function(e) {
                 let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "span";
                 return class extends i().Component {
                     constructor() {
-                        super(...arguments), b(this, "state", {
+                        super(...arguments), Y(this, "state", {
                             focus: !1
-                        }), b(this, "handleFocus", (() => this.setState({
+                        }), Y(this, "handleFocus", (() => this.setState({
                             focus: !0
-                        }))), b(this, "handleBlur", (() => this.setState({
+                        }))), Y(this, "handleBlur", (() => this.setState({
                             focus: !1
                         })))
                     }
                     render() {
                         return i().createElement(t, {
                             onFocus: this.handleFocus,
                             onBlur: this.handleBlur
@@ -682,16 +1399,16 @@
                     onClick: n = (() => {}),
                     title: a = t,
                     children: o,
                     focus: l,
                     focusStyle: s = {}
                 } = e;
                 const {
-                    onSwatchHover: p
-                } = F(), h = "transparent" === t, c = {
+                    onSwatchHover: h
+                } = ae(), p = "transparent" === t, c = {
                     swatch: {
                         background: t,
                         height: "100%",
                         width: "100%",
                         cursor: "pointer",
                         position: "relative",
                         outline: "none",
@@ -702,23 +1419,23 @@
                 return i().createElement("div", {
                     style: c.swatch,
                     onClick: e => n(t, e),
                     title: a,
                     tabIndex: 0,
                     onKeyDown: e => 13 === e.keyCode && n(t, e),
                     onMouseOver: e => {
-                        p && p(t, e)
+                        h && h(t, e)
                     }
-                }, o, h && i().createElement(A, {
+                }, o, p && i().createElement(se, {
                     borderRadius: c.swatch.borderRadius,
                     boxShadow: "inset 0 0 0 1px rgba(0,0,0,0.1)"
                 }))
             }));
 
-            function O(e) {
+            function ve(e) {
                 let {
                     direction: t
                 } = e;
                 const r = {
                     picker: {
                         width: "18px",
                         height: "18px",
@@ -728,54 +1445,54 @@
                         boxShadow: "0 1px 4px 0 rgba(0, 0, 0, 0.37)"
                     }
                 };
                 return i().createElement("div", {
                     style: r.picker
                 })
             }
-            var P = S((function(e) {
+            var ye = ie((function(e) {
                     let {
                         width: t = "316px",
                         height: r = "16px",
                         direction: a = "horizontal",
                         style: o,
                         renderers: l,
-                        pointer: s = O,
-                        className: p = ""
+                        pointer: s = ve,
+                        className: h = ""
                     } = e;
                     const {
-                        colors: h,
+                        colors: p,
                         changeColor: c
-                    } = F(), {
+                    } = ae(), {
                         hsl: d,
                         rgb: u
-                    } = h, g = {
+                    } = p, g = {
                         picker: {
                             position: "relative",
                             width: t,
                             height: r
                         },
                         alpha: {
                             borderRadius: "2px",
                             ...o
                         }
                     };
                     return i().createElement("div", {
                         style: g.picker,
-                        className: `alpha-picker ${p}`
-                    }, i().createElement(_, n({}, g.alpha, {
+                        className: `alpha-picker ${h}`
+                    }, i().createElement(he, n({}, g.alpha, {
                         rgb: u,
                         hsl: d,
                         pointer: s,
                         renderers: l,
                         onChange: c,
                         direction: a
                     })))
                 })),
-                X = e => {
+                we = e => {
                     let {
                         colors: t,
                         onClick: r
                     } = e;
                     const n = {
                         swatches: {
                             marginRight: "-10px"
@@ -790,75 +1507,75 @@
                         },
                         clear: {
                             clear: "both"
                         }
                     };
                     return i().createElement("div", {
                         style: n.swatches
-                    }, t.map((e => i().createElement(G, {
+                    }, t.map((e => i().createElement(me, {
                         key: e,
                         color: e,
                         style: n.swatch,
                         onClick: r,
                         focusStyle: {
                             boxShadow: `0 0 4px ${e}`
                         }
                     }))), i().createElement("div", {
                         style: n.clear
                     }))
                 },
-                U = S((e => {
+                Ee = ie((e => {
                     let {
                         colors: t = ["#D9E3F0", "#F47373", "#697689", "#37D67A", "#2CCCE4", "#555555", "#dce775", "#ff8a65", "#ba68c8"],
                         width: r = 170,
                         triangle: n = "top",
                         styles: a = {},
                         className: o = ""
                     } = e;
                     const {
                         colors: l,
                         changeColor: s
-                    } = F(), {
-                        hex: p
-                    } = l, h = "transparent" === p, c = (e, t) => {
-                        y(e) && s({
+                    } = ae(), {
+                        hex: h
+                    } = l, p = "transparent" === h, c = (e, t) => {
+                        Q(e) && s({
                             hex: e,
                             source: "hex"
                         }, t)
-                    }, d = x()({
+                    }, d = Z()({
                         card: {
                             width: r,
                             background: "#fff",
                             boxShadow: "0 1px rgba(0,0,0,.1)",
                             borderRadius: "6px",
                             position: "relative"
                         },
                         head: {
                             height: "110px",
-                            background: p,
+                            background: h,
                             borderRadius: "6px 6px 0 0",
                             display: "flex",
                             alignItems: "center",
                             justifyContent: "center",
                             position: "relative"
                         },
                         body: {
                             padding: "10px"
                         },
                         label: {
                             fontSize: "18px",
-                            color: w(p),
+                            color: ee(h),
                             position: "relative"
                         },
                         triangle: {
                             width: "0px",
                             height: "0px",
                             borderStyle: "solid",
                             borderWidth: "0 10px 10px 10px",
-                            borderColor: `transparent transparent ${p} transparent`,
+                            borderColor: `transparent transparent ${h} transparent`,
                             position: "absolute",
                             top: "-10px",
                             left: "50%",
                             marginLeft: "-10px",
                             display: "hide" === n ? "none" : void 0
                         },
                         input: {
@@ -877,41 +1594,41 @@
                     return i().createElement("div", {
                         style: d.card,
                         className: `block-picker ${o}`
                     }, i().createElement("div", {
                         style: d.triangle
                     }), i().createElement("div", {
                         style: d.head
-                    }, h && i().createElement(A, {
+                    }, p && i().createElement(se, {
                         borderRadius: "6px 6px 0 0"
                     }), i().createElement("div", {
                         style: d.label
-                    }, p)), i().createElement("div", {
+                    }, h)), i().createElement("div", {
                         style: d.body
-                    }, i().createElement(X, {
+                    }, i().createElement(we, {
                         colors: t,
                         onClick: c
-                    }), i().createElement(H, {
+                    }), i().createElement(ge, {
                         style: {
                             input: d.input
                         },
-                        value: p,
+                        value: h,
                         onChange: c
                     })))
                 }));
 
-            function I(e) {
+            function Ce(e) {
                 let {
                     view: t = "hex",
                     ...r
                 } = e;
                 const [n, o] = (0, a.useState)(t);
 
                 function l(e, t) {
-                    e.hex ? y(e.hex) && r.onChange({
+                    e.hex ? Q(e.hex) && r.onChange({
                         hex: e.hex,
                         source: "hex"
                     }, t) : e.r || e.g || e.b ? r.onChange({
                         r: e.r || r.rgb.r,
                         g: e.g || r.rgb.g,
                         b: e.b || r.rgb.b,
                         source: "rgb"
@@ -932,15 +1649,15 @@
                 function s(e) {
                     e.currentTarget.style.background = "#eee"
                 }(0, a.useEffect)((() => {
                     1 !== r.hsl.a && "hex" === t && o("rgb")
                 }), []), (0, a.useEffect)((() => {
                     1 !== r.hsl.a && "hex" === n && o("rgb")
                 }), [r]);
-                const p = {
+                const h = {
                     wrap: {
                         paddingTop: "16px",
                         display: "flex"
                     },
                     fields: {
                         flex: "1",
                         display: "flex",
@@ -999,123 +1716,123 @@
                         fill: "#333",
                         width: "24px",
                         height: "24px",
                         border: "1px transparent solid",
                         borderRadius: "5px"
                     }
                 };
-                let h;
-                return "hex" === n ? h = i().createElement("div", {
-                    style: p.fields,
+                let p;
+                return "hex" === n ? p = i().createElement("div", {
+                    style: h.fields,
                     className: "flexbox-fix"
                 }, i().createElement("div", {
-                    style: p.field
-                }, i().createElement(H, {
+                    style: h.field
+                }, i().createElement(ge, {
                     style: {
-                        input: p.input,
-                        label: p.label
+                        input: h.input,
+                        label: h.label
                     },
                     label: "hex",
                     value: r.hex,
                     onChange: l
-                }))) : "rgb" === n ? h = i().createElement("div", {
-                    style: p.fields,
+                }))) : "rgb" === n ? p = i().createElement("div", {
+                    style: h.fields,
                     className: "flexbox-fix"
                 }, i().createElement("div", {
-                    style: p.field
-                }, i().createElement(H, {
+                    style: h.field
+                }, i().createElement(ge, {
                     style: {
-                        input: p.input,
-                        label: p.label
+                        input: h.input,
+                        label: h.label
                     },
                     label: "r",
                     value: r.rgb.r,
                     onChange: l
                 })), i().createElement("div", {
-                    style: p.field
-                }, i().createElement(H, {
+                    style: h.field
+                }, i().createElement(ge, {
                     style: {
-                        input: p.input,
-                        label: p.label
+                        input: h.input,
+                        label: h.label
                     },
                     label: "g",
                     value: r.rgb.g,
                     onChange: l
                 })), i().createElement("div", {
-                    style: p.field
-                }, i().createElement(H, {
+                    style: h.field
+                }, i().createElement(ge, {
                     style: {
-                        input: p.input,
-                        label: p.label
+                        input: h.input,
+                        label: h.label
                     },
                     label: "b",
                     value: r.rgb.b,
                     onChange: l
                 })), i().createElement("div", {
-                    style: p.alpha
-                }, i().createElement(H, {
+                    style: h.alpha
+                }, i().createElement(ge, {
                     style: {
-                        input: p.input,
-                        label: p.label
+                        input: h.input,
+                        label: h.label
                     },
                     label: "a",
                     value: r.rgb.a,
                     arrowOffset: .01,
                     onChange: l
-                }))) : "hsl" === n && (h = i().createElement("div", {
-                    style: p.fields,
+                }))) : "hsl" === n && (p = i().createElement("div", {
+                    style: h.fields,
                     className: "flexbox-fix"
                 }, i().createElement("div", {
-                    style: p.field
-                }, i().createElement(H, {
+                    style: h.field
+                }, i().createElement(ge, {
                     style: {
-                        input: p.input,
-                        label: p.label
+                        input: h.input,
+                        label: h.label
                     },
                     label: "h",
                     value: Math.round(r.hsl.h),
                     onChange: l
                 })), i().createElement("div", {
-                    style: p.field
-                }, i().createElement(H, {
+                    style: h.field
+                }, i().createElement(ge, {
                     style: {
-                        input: p.input,
-                        label: p.label
+                        input: h.input,
+                        label: h.label
                     },
                     label: "s",
                     value: `${Math.round(100*r.hsl.s)}%`,
                     onChange: l
                 })), i().createElement("div", {
-                    style: p.field
-                }, i().createElement(H, {
+                    style: h.field
+                }, i().createElement(ge, {
                     style: {
-                        input: p.input,
-                        label: p.label
+                        input: h.input,
+                        label: h.label
                     },
                     label: "l",
                     value: `${Math.round(100*r.hsl.l)}%`,
                     onChange: l
                 })), i().createElement("div", {
-                    style: p.alpha
-                }, i().createElement(H, {
+                    style: h.alpha
+                }, i().createElement(ge, {
                     style: {
-                        input: p.input,
-                        label: p.label
+                        input: h.input,
+                        label: h.label
                     },
                     label: "a",
                     value: r.hsl.a,
                     arrowOffset: .01,
                     onChange: l
                 })))), i().createElement("div", {
-                    style: p.wrap,
+                    style: h.wrap,
                     className: "flexbox-fix"
-                }, h, i().createElement("div", {
-                    style: p.toggle
+                }, p, i().createElement("div", {
+                    style: h.toggle
                 }, i().createElement("div", {
-                    style: p.icon,
+                    style: h.icon,
                     onClick: function() {
                         "hex" === n ? o("rgb") : "rgb" === n ? o("hsl") : "hsl" === n && (1 === r.hsl.a ? o("hex") : o("rgb"))
                     }
                 }, i().createElement("img", {
                     width: "24",
                     height: "24",
                     onMouseOver: s,
@@ -1123,56 +1840,56 @@
                     onMouseOut: function(e) {
                         e.currentTarget.style.background = "transparent"
                     },
                     src: "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZD0iTTEyLDE4LjE3TDguODMsMTVMNy40MiwxNi40MUwxMiwyMUwxNi41OSwxNi40MUwxNS4xNywxNU0xMiw1LjgzTDE1LjE3LDlMMTYuNTgsNy41OUwxMiwzTDcuNDEsNy41OUw4LjgzLDlMMTIsNS44M1oiIC8+PC9zdmc+"
                 }))))
             }
 
-            function j() {
+            function ke() {
                 return i().createElement("div", {
                     style: {
                         width: "12px",
                         height: "12px",
                         borderRadius: "6px",
                         transform: "translate(-6px, -1px)",
                         backgroundColor: "rgb(248, 248, 248)",
                         boxShadow: "0 1px 4px 0 rgba(0, 0, 0, 0.37)"
                     }
                 })
             }
 
-            function W() {
+            function Fe() {
                 return i().createElement("div", {
                     style: {
                         width: "12px",
                         height: "12px",
                         borderRadius: "6px",
                         boxShadow: "inset 0 0 0 1px #fff",
                         transform: "translate(-6px, -6px)"
                     }
                 })
             }
-            var V = S((e => {
+            var Se = ie((e => {
                 let {
                     width: t = 225,
                     disableAlpha: r = !1,
                     renderers: n,
                     styles: a = {},
                     className: o = "",
                     defaultView: l
                 } = e;
                 const {
                     colors: s,
-                    changeColor: p
-                } = F(), {
-                    rgb: h,
+                    changeColor: h
+                } = ae(), {
+                    rgb: p,
                     hex: c,
                     hsl: d,
                     hsv: u
-                } = s, g = x()({
+                } = s, g = Z()({
                     picker: {
                         width: t,
                         background: "#fff",
                         borderRadius: "2px",
                         boxShadow: "0 0 2px rgba(0,0,0,.3), 0 4px 8px rgba(0,0,0,.3)",
                         boxSizing: "initial",
                         fontFamily: "Menlo"
@@ -1205,15 +1922,15 @@
                         overflow: "hidden"
                     },
                     active: {
                         position: "absolute",
                         inset: "0px",
                         borderRadius: "8px",
                         boxShadow: "inset 0 0 0 1px rgba(0,0,0,.1)",
-                        background: `rgba(${h.r}, ${h.g}, ${h.b}, ${h.a})`,
+                        background: `rgba(${p.r}, ${p.g}, ${p.b}, ${p.a})`,
                         zIndex: "2"
                     },
                     toggles: {
                         flex: "1"
                     },
                     hue: {
                         height: "10px",
@@ -1233,73 +1950,73 @@
                     }
                 }, a);
                 return i().createElement("div", {
                     style: g.picker,
                     className: `chrome-picker ${o}`
                 }, i().createElement("div", {
                     style: g.saturation
-                }, i().createElement(T, {
+                }, i().createElement(xe, {
                     style: g.Saturation,
                     hsl: d,
                     hsv: u,
-                    pointer: i().createElement(W, null),
-                    onChange: p
+                    pointer: i().createElement(Fe, null),
+                    onChange: h
                 })), i().createElement("div", {
                     style: g.body
                 }, i().createElement("div", {
                     style: g.controls,
                     className: "flexbox-fix"
                 }, i().createElement("div", {
                     style: g.color
                 }, i().createElement("div", {
                     style: g.swatch
                 }, i().createElement("div", {
                     style: g.active
-                }), i().createElement(A, {
+                }), i().createElement(se, {
                     renderers: n
                 }))), i().createElement("div", {
                     style: g.toggles
                 }, i().createElement("div", {
                     style: g.hue
-                }, i().createElement(L, {
+                }, i().createElement(be, {
                     style: g.Hue,
                     hsl: d,
-                    pointer: j,
-                    onChange: p
+                    pointer: ke,
+                    onChange: h
                 })), i().createElement("div", {
                     style: g.alpha
-                }, i().createElement(_, {
+                }, i().createElement(he, {
                     style: g.Alpha,
-                    rgb: h,
+                    rgb: p,
                     hsl: d,
-                    pointer: j,
+                    pointer: ke,
                     renderers: n,
-                    onChange: p
-                })))), i().createElement(I, {
-                    rgb: h,
+                    onChange: h
+                })))), i().createElement(Ce, {
+                    rgb: p,
                     hsl: d,
                     hex: c,
                     view: l,
-                    onChange: p
+                    onChange: h
                 })))
             }));
-            const Y = e => t => {
+            const Be = e => t => {
                 const [r, o] = (0, a.useState)(!1);
                 return i().createElement("div", {
                     onMouseOver: () => {
                         o(!0)
                     },
                     onMouseOut: () => {
                         o(!1)
                     }
                 }, i().createElement(e, n({}, t, {
                     hover: r
                 })))
             };
-            var q = Y((e => {
+            var Me = Be((e => {
                     let {
                         color: t,
                         onClick: r,
                         hover: n,
                         active: a,
                         circleSize: o = 28,
                         circleSpacing: l = 14
@@ -1319,63 +2036,63 @@
                             boxShadow: a ? `inset 0 0 0 3px ${t}` : `inset 0 0 0 ${o/2+1}px ${t}`,
                             transition: "100ms box-shadow ease",
                             transform: n ? "scale(1.2)" : void 0
                         }
                     };
                     return i().createElement("div", {
                         style: s.swatch
-                    }, i().createElement(G, {
+                    }, i().createElement(me, {
                         style: s.Swatch,
                         color: t,
                         onClick: r,
                         focusStyle: {
                             boxShadow: `${s.Swatch.boxShadow}, 0 0 5px ${t}`
                         }
                     }))
                 })),
-                Z = S((function(e) {
+                Re = ie((function(e) {
                     let {
                         width: t = 252,
                         colors: r = ["#F44336", "#E91E63", "#9C27B0", "#673AB7", "#3F51B5", "#2196F3", "#03A9F4", "#00BCD4", "#009688", "#4CAF50", "#8BC34A", "#CDDC39", "#FFEB3B", "#FFC107", "#FF9800", "#FF5722", "#795548", "#607D8B"],
                         circleSize: n = 28,
                         styles: a = {},
                         circleSpacing: o = 14,
                         className: l = ""
                     } = e;
                     const {
                         colors: s,
-                        changeColor: p
-                    } = F(), {
-                        hex: h
-                    } = s, c = x()({
+                        changeColor: h
+                    } = ae(), {
+                        hex: p
+                    } = s, c = Z()({
                         card: {
                             width: t,
                             display: "flex",
                             flexWrap: "wrap",
                             marginRight: -o,
                             marginBottom: -o
                         }
-                    }, a), d = (e, t) => p({
+                    }, a), d = (e, t) => h({
                         hex: e,
                         source: "hex"
                     }, t);
                     return i().createElement("div", {
                         style: c.card,
                         className: `circle-picker ${l}`
-                    }, r.map((e => i().createElement(q, {
+                    }, r.map((e => i().createElement(Me, {
                         key: e,
                         color: e,
                         onClick: d,
-                        active: h === e.toLowerCase(),
+                        active: p === e.toLowerCase(),
                         circleSize: n,
                         circleSpacing: o
                     }))))
                 }));
 
-            function K(e) {
+            function Ae(e) {
                 let {
                     color: t,
                     onClick: r = (() => {}),
                     active: n
                 } = e;
                 const a = {
                     color: {
@@ -1388,32 +2105,32 @@
                         position: "relative",
                         cursor: "pointer",
                         boxShadow: "#FFFFFF" === t ? "inset 0 0 0 1px #ddd" : void 0
                     },
                     dot: {
                         position: "absolute",
                         inset: "5px",
-                        background: "#FFFFFF" === t || "transparent" === t ? "#000" : w(t),
+                        background: "#FFFFFF" === t || "transparent" === t ? "#000" : ee(t),
                         borderRadius: "50%",
                         opacity: n ? 1 : 0
                     }
                 };
-                return i().createElement(G, {
+                return i().createElement(me, {
                     style: a.color,
                     color: t,
                     onClick: r,
                     focusStyle: {
                         boxShadow: `0 0 4px ${t}`
                     }
                 }, i().createElement("div", {
                     style: a.dot
                 }))
             }
 
-            function J(e) {
+            function _e(e) {
                 let {
                     hex: t,
                     rgb: r,
                     onChange: n
                 } = e;
                 const a = {
                         fields: {
@@ -1485,103 +2202,103 @@
                         }, t)
                     };
                 return i().createElement("div", {
                     style: a.fields,
                     className: "flexbox-fix"
                 }, i().createElement("div", {
                     style: a.active
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: a.HEXwrap,
                         input: a.HEXinput,
                         label: a.HEXlabel
                     },
                     label: "hex",
                     value: t,
                     onChange: o
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: a.RGBwrap,
                         input: a.RGBinput,
                         label: a.RGBlabel
                     },
                     label: "r",
                     value: r.r,
                     onChange: o
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: a.RGBwrap,
                         input: a.RGBinput,
                         label: a.RGBlabel
                     },
                     label: "g",
                     value: r.g,
                     onChange: o
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: a.RGBwrap,
                         input: a.RGBinput,
                         label: a.RGBlabel
                     },
                     label: "b",
                     value: r.b,
                     onChange: o
                 }))
             }
-            var Q = S((function(e) {
+            var De = ie((function(e) {
                     let {
                         colors: t = ["#4D4D4D", "#999999", "#FFFFFF", "#F44E3B", "#FE9200", "#FCDC00", "#DBDF00", "#A4DD00", "#68CCCA", "#73D8FF", "#AEA1FF", "#FDA1FF", "#333333", "#808080", "#cccccc", "#D33115", "#E27300", "#FCC400", "#B0BC00", "#68BC00", "#16A5A5", "#009CE0", "#7B64FF", "#FA28FF", "#000000", "#666666", "#B3B3B3", "#9F0500", "#C45100", "#FB9E00", "#808900", "#194D33", "#0C797D", "#0062B1", "#653294", "#AB149E"],
                         styles: r = {},
                         className: n = ""
                     } = e;
                     const {
                         colors: a,
                         changeColor: o
-                    } = F(), {
+                    } = ae(), {
                         rgb: l,
                         hex: s
-                    } = a, p = x()({
+                    } = a, h = Z()({
                         Compact: {
                             background: "#f6f6f6",
                             borderRadius: "4px"
                         },
                         compact: {
                             paddingTop: "5px",
                             paddingLeft: "5px",
                             boxSizing: "initial",
                             width: "240px"
                         },
                         clear: {
                             clear: "both"
                         }
-                    }, r), h = (e, t) => {
-                        e.hex ? y(e.hex) && o({
+                    }, r), p = (e, t) => {
+                        e.hex ? Q(e.hex) && o({
                             hex: e.hex,
                             source: "hex"
                         }, t) : o(e, t)
                     };
-                    return i().createElement(z, {
+                    return i().createElement(fe, {
                         styles: r
                     }, i().createElement("div", {
-                        style: p.compact,
+                        style: h.compact,
                         className: `compact-picker ${n}`
-                    }, i().createElement("div", null, t.map((e => i().createElement(K, {
+                    }, i().createElement("div", null, t.map((e => i().createElement(Ae, {
                         key: e,
                         color: e,
                         active: e.toLowerCase() === s,
-                        onClick: h
+                        onClick: p
                     }))), i().createElement("div", {
-                        style: p.clear
-                    })), i().createElement(J, {
+                        style: h.clear
+                    })), i().createElement(_e, {
                         hex: s,
                         rgb: l,
-                        onChange: h
+                        onChange: p
                     })))
                 })),
-                ee = Y((function(e) {
+                Ne = Be((function(e) {
                     let {
                         hover: t,
                         color: r,
                         onClick: n
                     } = e;
                     const a = {
                             position: "relative",
@@ -1597,31 +2314,31 @@
                             }
                         };
                     return t && (o.swatch = {
                         ...o.swatch,
                         ...a
                     }), i().createElement("div", {
                         style: o.swatch
-                    }, i().createElement(G, {
+                    }, i().createElement(me, {
                         color: r,
                         onClick: n,
                         focusStyle: a
                     }))
                 })),
-                te = S((function(e) {
+                $e = ie((function(e) {
                     let {
                         width: t = 200,
                         colors: r = ["#B80000", "#DB3E00", "#FCCB00", "#008B02", "#006B76", "#1273DE", "#004DCF", "#5300EB", "#EB9694", "#FAD0C3", "#FEF3BD", "#C1E1C5", "#BEDADC", "#C4DEF6", "#BED3F3", "#D4C4FB"],
                         triangle: n = "top-left",
                         styles: a = {},
                         className: o = ""
                     } = e;
                     const {
                         changeColor: l
-                    } = F(), s = x()({
+                    } = ae(), s = Z()({
                         card: {
                             width: t,
                             background: "#fff",
                             border: "1px solid rgba(0,0,0,0.2)",
                             boxShadow: "0 3px 12px rgba(0,0,0,0.15)",
                             borderRadius: "4px",
                             position: "relative",
@@ -1645,65 +2362,65 @@
                             borderBottomColor: "rgba(0,0,0,0.15)",
                             display: "hide" === n ? "none" : void 0,
                             top: "top-left" === n || "top-right" === n ? "-16px" : "35px",
                             left: "top-left" === n || "bottom-left" === n ? "9px" : void 0,
                             right: "top-right" === n || "bottom-right" === n ? "9px" : void 0,
                             transform: "bottom-left" === n || "bottom-right" === n ? "rotate(180deg)" : void 0
                         }
-                    }, a), p = (e, t) => l({
+                    }, a), h = (e, t) => l({
                         hex: e,
                         source: "hex"
                     }, t);
                     return i().createElement("div", {
                         style: s.card,
                         className: `github-picker ${o}`
                     }, i().createElement("div", {
                         style: s.triangleShadow
                     }), i().createElement("div", {
                         style: s.triangle
-                    }), r.map((e => i().createElement(ee, {
+                    }), r.map((e => i().createElement(Ne, {
                         color: e,
                         key: e,
-                        onClick: p
+                        onClick: h
                     }))))
                 }));
 
-            function re(e) {
+            function He(e) {
                 let {
                     onChange: t,
                     rgb: r,
                     hsl: n,
                     hex: a,
                     hsv: o
                 } = e;
                 const l = (e, r) => {
-                        if (e.hex) y(e.hex) && t({
+                        if (e.hex) Q(e.hex) && t({
                             hex: e.hex,
                             source: "hex"
                         }, r);
                         else if (e.rgb) {
                             const n = e.rgb.split(",");
-                            E(e.rgb, "rgb") && t({
+                            te(e.rgb, "rgb") && t({
                                 r: n[0],
                                 g: n[1],
                                 b: n[2],
                                 a: 1,
                                 source: "rgb"
                             }, r)
                         } else if (e.hsv) {
                             const n = e.hsv.split(",");
-                            E(e.hsv, "hsv") && (n[2] = n[2].replace("%", ""), n[1] = n[1].replace("%", ""), n[0] = n[0].replace("°", ""), 1 == n[1] ? n[1] = .01 : 1 == n[2] && (n[2] = .01), t({
+                            te(e.hsv, "hsv") && (n[2] = n[2].replace("%", ""), n[1] = n[1].replace("%", ""), n[0] = n[0].replace("°", ""), 1 == n[1] ? n[1] = .01 : 1 == n[2] && (n[2] = .01), t({
                                 h: Number(n[0]),
                                 s: Number(n[1]),
                                 v: Number(n[2]),
                                 source: "hsv"
                             }, r))
                         } else if (e.hsl) {
                             const n = e.hsl.split(",");
-                            E(e.hsl, "hsl") && (n[2] = n[2].replace("%", ""), n[1] = n[1].replace("%", ""), n[0] = n[0].replace("°", ""), 1 == c[1] ? c[1] = .01 : 1 == c[2] && (c[2] = .01), t({
+                            te(e.hsl, "hsl") && (n[2] = n[2].replace("%", ""), n[1] = n[1].replace("%", ""), n[0] = n[0].replace("°", ""), 1 == c[1] ? c[1] = .01 : 1 == c[2] && (c[2] = .01), t({
                                 h: Number(n[0]),
                                 s: Number(n[1]),
                                 v: Number(n[2]),
                                 source: "hsl"
                             }, r))
                         }
                     },
@@ -1778,68 +2495,68 @@
                             fontFamily: "Roboto,Arial,sans-serif"
                         },
                         single: {
                             flexGrow: "1",
                             margin: "0px 4.4px"
                         }
                     },
-                    p = `${r.r}, ${r.g}, ${r.b}`,
-                    h = `${Math.round(n.h)}°, ${Math.round(100*n.s)}%, ${Math.round(100*n.l)}%`,
+                    h = `${r.r}, ${r.g}, ${r.b}`,
+                    p = `${Math.round(n.h)}°, ${Math.round(100*n.s)}%, ${Math.round(100*n.l)}%`,
                     c = `${Math.round(o.h)}°, ${Math.round(100*o.s)}%, ${Math.round(100*o.v)}%`;
                 return i().createElement("div", {
                     style: s.wrap,
                     className: "flexbox-fix"
                 }, i().createElement("div", {
                     style: s.fields
                 }, i().createElement("div", {
                     style: s.double
-                }, i().createElement(H, {
+                }, i().createElement(ge, {
                     style: {
                         input: s.input,
                         label: s.label
                     },
                     label: "hex",
                     value: a,
                     onChange: l
                 })), i().createElement("div", {
                     style: s.column
                 }, i().createElement("div", {
                     style: s.single
-                }, i().createElement(H, {
+                }, i().createElement(ge, {
                     style: {
                         input: s.input2,
                         label: s.label2
                     },
                     label: "rgb",
-                    value: p,
+                    value: h,
                     onChange: l
                 })), i().createElement("div", {
                     style: s.single
-                }, i().createElement(H, {
+                }, i().createElement(ge, {
                     style: {
                         input: s.input2,
                         label: s.label2
                     },
                     label: "hsv",
                     value: c,
                     onChange: l
                 })), i().createElement("div", {
                     style: s.single
-                }, i().createElement(H, {
+                }, i().createElement(ge, {
                     style: {
                         input: s.input2,
                         label: s.label2
                     },
                     label: "hsl",
-                    value: h,
+                    value: p,
                     onChange: l
                 })))))
             }
 
-            function ne(e) {
+            function Le(e) {
                 let {
                     hsl: t = {
                         a: 1,
                         h: 249.94,
                         l: .2,
                         s: .5
                     }
@@ -1852,15 +2569,15 @@
                         transform: "translate(-10px, -7px)",
                         background: `hsl(${Math.round(t.h)}, 100%, 50%)`,
                         border: "2px white solid"
                     }
                 })
             }
 
-            function ae(e) {
+            function ze(e) {
                 let {
                     hsl: t = {
                         a: 1,
                         h: 249.94,
                         l: .2,
                         s: .5
                     }
@@ -1872,30 +2589,30 @@
                         borderRadius: "22px",
                         border: "2px #fff solid",
                         transform: "translate(-12px, -13px)",
                         background: `hsl(${Math.round(t.h)}, ${Math.round(100*t.s)}%, ${Math.round(100*t.l)}%)`
                     }
                 })
             }
-            var ie = S((function(e) {
+            var Te = ie((function(e) {
                 let {
                     width: t = 652,
                     header: r = "Color picker",
                     styles: n = {},
                     className: a = ""
                 } = e;
                 const {
                     colors: o,
                     changeColor: l
-                } = F(), {
+                } = ae(), {
                     rgb: s,
-                    hex: p,
-                    hsl: h,
+                    hex: h,
+                    hsl: p,
                     hsv: c
-                } = o, d = x()({
+                } = o, d = Z()({
                     picker: {
                         width: t,
                         background: "#fff",
                         border: "1px solid #dfe1e5",
                         boxSizing: "initial",
                         display: "flex",
                         flexWrap: "wrap",
@@ -1953,44 +2670,44 @@
                     className: `google-picker ${a}`
                 }, i().createElement("div", {
                     style: d.head
                 }, r), i().createElement("div", {
                     style: d.swatch
                 }), i().createElement("div", {
                     style: d.saturation
-                }, i().createElement(T, {
-                    hsl: h,
+                }, i().createElement(xe, {
+                    hsl: p,
                     hsv: c,
-                    pointer: i().createElement(ae, {
-                        hsl: h
+                    pointer: i().createElement(ze, {
+                        hsl: p
                     }),
                     onChange: l
                 })), i().createElement("div", {
                     style: d.body
                 }, i().createElement("div", {
                     style: d.controls,
                     className: "flexbox-fix"
                 }, i().createElement("div", {
                     style: d.hue
-                }, i().createElement(L, {
+                }, i().createElement(be, {
                     style: d.Hue,
-                    hsl: h,
+                    hsl: p,
                     radius: "4px",
-                    pointer: ne,
+                    pointer: Le,
                     onChange: l
-                }))), i().createElement(re, {
+                }))), i().createElement(He, {
                     rgb: s,
-                    hsl: h,
-                    hex: p,
+                    hsl: p,
+                    hex: h,
                     hsv: c,
                     onChange: l
                 })))
             }));
 
-            function oe(e) {
+            function Ge(e) {
                 let {
                     direction: t
                 } = e;
                 const r = {
                     picker: {
                         width: "18px",
                         height: "18px",
@@ -2000,65 +2717,65 @@
                         boxShadow: "0 1px 4px 0 rgba(0, 0, 0, 0.37)"
                     }
                 };
                 return i().createElement("div", {
                     style: r.picker
                 })
             }
-            var le = S((function(e) {
+            var Oe = ie((function(e) {
                     let {
                         width: t = "316px",
                         height: r = "16px",
                         direction: a = "horizontal",
-                        pointer: o = oe,
+                        pointer: o = Ge,
                         styles: l = {},
                         className: s = ""
                     } = e;
                     const {
-                        colors: p,
-                        changeColor: h
-                    } = F(), {
+                        colors: h,
+                        changeColor: p
+                    } = ae(), {
                         hsl: c
-                    } = p, d = x()({
+                    } = h, d = Z()({
                         picker: {
                             position: "relative",
                             width: t,
                             height: r
                         },
                         hue: {
                             borderRadius: "2px"
                         }
                     }, l);
                     return i().createElement("div", {
                         style: d.picker,
                         className: `hue-picker ${s}`
-                    }, i().createElement(L, n({}, d.hue, {
+                    }, i().createElement(be, n({}, d.hue, {
                         hsl: c,
                         pointer: o,
-                        onChange: e => h({
+                        onChange: e => p({
                             a: 1,
                             h: "string" != typeof e && "h" in e ? e.h : 0,
                             l: .5,
                             s: 1
                         }),
                         direction: a
                     })))
                 })),
-                se = S((e => {
+                Pe = ie((e => {
                     let {
                         styles: t = {},
                         className: r = ""
                     } = e;
                     const {
                         colors: n,
                         changeColor: a
-                    } = F(), {
+                    } = ae(), {
                         rgb: o,
                         hex: l
-                    } = n, s = x()({
+                    } = n, s = Z()({
                         material: {
                             width: "98px",
                             height: "98px",
                             padding: "16px",
                             fontFamily: "Roboto"
                         },
                         HEXwrap: {
@@ -2111,79 +2828,79 @@
                             marginRight: "-10px",
                             paddingTop: "11px"
                         },
                         third: {
                             flex: "1",
                             paddingRight: "10px"
                         }
-                    }, t), p = (e, t) => {
-                        "string" != typeof e && "hex" in e ? y(e.hex) && a({
+                    }, t), h = (e, t) => {
+                        "string" != typeof e && "hex" in e ? Q(e.hex) && a({
                             hex: e.hex,
                             source: "hex"
                         }, t) : "string" != typeof e && ("r" in e || "g" in e || "b" in e) && a({
                             r: e.r || o.r,
                             g: e.g || o.g,
                             b: e.b || o.b,
                             source: "rgb"
                         }, t)
                     };
-                    return i().createElement(z, {
+                    return i().createElement(fe, {
                         styles: t
                     }, i().createElement("div", {
                         style: s.material,
                         className: `material-picker ${r}`
-                    }, i().createElement(H, {
+                    }, i().createElement(ge, {
                         style: {
                             wrap: s.HEXwrap,
                             input: s.HEXinput,
                             label: s.HEXlabel
                         },
                         label: "hex",
                         value: l,
-                        onChange: p
+                        onChange: h
                     }), i().createElement("div", {
                         style: s.split,
                         className: "flexbox-fix"
                     }, i().createElement("div", {
                         style: s.third
-                    }, i().createElement(H, {
+                    }, i().createElement(ge, {
                         style: {
                             wrap: s.RGBwrap,
                             input: s.RGBinput,
                             label: s.RGBlabel
                         },
                         label: "r",
                         value: o.r,
-                        onChange: p
+                        onChange: h
                     })), i().createElement("div", {
                         style: s.third
-                    }, i().createElement(H, {
+                    }, i().createElement(ge, {
                         style: {
                             wrap: s.RGBwrap,
                             input: s.RGBinput,
                             label: s.RGBlabel
                         },
                         label: "g",
                         value: o.g,
-                        onChange: p
+                        onChange: h
                     })), i().createElement("div", {
                         style: s.third
-                    }, i().createElement(H, {
+                    }, i().createElement(ge, {
                         style: {
                             wrap: s.RGBwrap,
                             input: s.RGBinput,
                             label: s.RGBlabel
                         },
                         label: "b",
                         value: o.b,
-                        onChange: p
+                        onChange: h
                     })))))
                 }));
 
-            function pe(e) {
+            function Xe(e) {
                 let {
                     onClick: t,
                     label: r,
                     children: n,
                     active: a
                 } = e;
                 const o = {
@@ -2203,15 +2920,15 @@
                 };
                 return i().createElement("div", {
                     style: o.button,
                     onClick: t
                 }, r || n)
             }
 
-            function he(e) {
+            function Ue(e) {
                 let {
                     onChange: t,
                     rgb: r,
                     hsv: n,
                     hex: a
                 } = e;
                 const o = {
@@ -2280,15 +2997,15 @@
                         symbol: {
                             height: "20px",
                             lineHeight: "22px",
                             paddingBottom: "7px"
                         }
                     },
                     l = (e, a) => {
-                        e["#"] ? y(e["#"]) && t({
+                        e["#"] ? Q(e["#"]) && t({
                             hex: e["#"],
                             source: "hex"
                         }, a) : e.r || e.g || e.b ? t({
                             r: e.r || r.r,
                             g: e.g || r.g,
                             b: e.b || r.b,
                             source: "rgb"
@@ -2297,73 +3014,73 @@
                             s: e.s || n.s,
                             v: e.v || n.v,
                             source: "hsv"
                         }, a)
                     };
                 return i().createElement("div", {
                     style: o.fields
-                }, i().createElement(H, {
+                }, i().createElement(ge, {
                     style: {
                         wrap: o.RGBwrap,
                         input: o.RGBinput,
                         label: o.RGBlabel
                     },
                     label: "h",
                     value: Math.round(n.h),
                     onChange: l
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: o.RGBwrap,
                         input: o.RGBinput,
                         label: o.RGBlabel
                     },
                     label: "s",
                     value: Math.round(100 * n.s),
                     onChange: l
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: o.RGBwrap,
                         input: o.RGBinput,
                         label: o.RGBlabel
                     },
                     label: "v",
                     value: Math.round(100 * n.v),
                     onChange: l
                 }), i().createElement("div", {
                     style: o.divider
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: o.RGBwrap,
                         input: o.RGBinput,
                         label: o.RGBlabel
                     },
                     label: "r",
                     value: r.r,
                     onChange: l
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: o.RGBwrap,
                         input: o.RGBinput,
                         label: o.RGBlabel
                     },
                     label: "g",
                     value: r.g,
                     onChange: l
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: o.RGBwrap,
                         input: o.RGBinput,
                         label: o.RGBlabel
                     },
                     label: "b",
                     value: r.b,
                     onChange: l
                 }), i().createElement("div", {
                     style: o.divider
-                }), i().createElement(H, {
+                }), i().createElement(ge, {
                     style: {
                         wrap: o.HEXwrap,
                         input: o.HEXinput,
                         label: o.HEXlabel
                     },
                     label: "#",
                     value: a.replace("#", ""),
@@ -2375,15 +3092,15 @@
                 }, "°"), i().createElement("div", {
                     style: o.symbol
                 }, "%"), i().createElement("div", {
                     style: o.symbol
                 }, "%")))
             }
 
-            function ce() {
+            function Ie() {
                 const e = {
                         width: 0,
                         height: 0,
                         borderStyle: "solid",
                         borderWidth: "4px 0 4px 6px",
                         borderColor: "transparent transparent transparent #fff",
                         position: "absolute",
@@ -2424,30 +3141,30 @@
                 })), i().createElement("div", {
                     style: r.right
                 }, i().createElement("div", {
                     style: r.rightInside
                 })))
             }
 
-            function de(e) {
+            function je(e) {
                 let {
                     hsl: t
                 } = e;
                 return i().createElement("div", {
                     style: {
                         width: "12px",
                         height: "12px",
                         borderRadius: "6px",
                         boxShadow: t.l > .5 ? "inset 0 0 0 1px #000" : "inset 0 0 0 1px #fff",
                         transform: "translate(-6px, -6px)"
                     }
                 })
             }
 
-            function ue(e) {
+            function We(e) {
                 let {
                     rgb: t,
                     currentColor: r
                 } = e;
                 const n = {
                     swatches: {
                         border: "1px solid #B3B3B3",
@@ -2479,31 +3196,31 @@
                     style: n.new
                 }), i().createElement("div", {
                     style: n.current
                 })), i().createElement("div", {
                     style: n.label
                 }, "current"))
             }
-            var ge = S((function(e) {
+            var Ve = ie((function(e) {
                     let {
                         header: t = "Color Picker",
                         styles: r = {},
                         className: n = "",
                         onAccept: o,
                         onCancel: l
                     } = e;
                     const {
                         colors: s,
-                        changeColor: p
-                    } = F(), {
-                        rgb: h,
+                        changeColor: h
+                    } = ae(), {
+                        rgb: p,
                         hex: c,
                         hsv: d,
                         hsl: u
-                    } = s, [g, b] = (0, a.useState)(c), f = x()({
+                    } = s, [g, b] = (0, a.useState)(c), f = Z()({
                         picker: {
                             background: "#DCDCDC",
                             borderRadius: "4px",
                             boxShadow: "0 0 0 1px rgba(0,0,0,.25), 0 8px 16px rgba(0,0,0,.15)",
                             boxSizing: "initial",
                             width: "513px"
                         },
@@ -2559,57 +3276,57 @@
                     }, i().createElement("div", {
                         style: f.head
                     }, t), i().createElement("div", {
                         style: f.body,
                         className: "flexbox-fix"
                     }, i().createElement("div", {
                         style: f.saturation
-                    }, i().createElement(T, {
+                    }, i().createElement(xe, {
                         hsl: u,
                         hsv: d,
-                        pointer: i().createElement(de, {
+                        pointer: i().createElement(je, {
                             hsl: u
                         }),
-                        onChange: p
+                        onChange: h
                     })), i().createElement("div", {
                         style: f.hue
-                    }, i().createElement(L, {
+                    }, i().createElement(be, {
                         direction: "vertical",
                         hsl: u,
-                        pointer: ce,
-                        onChange: p
+                        pointer: Ie,
+                        onChange: h
                     })), i().createElement("div", {
                         style: f.controls
                     }, i().createElement("div", {
                         style: f.top,
                         className: "flexbox-fix"
                     }, i().createElement("div", {
                         style: f.previews
-                    }, i().createElement(ue, {
-                        rgb: h,
+                    }, i().createElement(We, {
+                        rgb: p,
                         currentColor: g
                     })), i().createElement("div", {
                         style: f.actions
-                    }, i().createElement(pe, {
+                    }, i().createElement(Xe, {
                         label: "OK",
                         onClick: function() {
                             o && o(), b(c)
                         },
                         active: !0
-                    }), i().createElement(pe, {
+                    }), i().createElement(Xe, {
                         label: "Cancel",
                         onClick: l
-                    }), i().createElement(he, {
-                        onChange: p,
-                        rgb: h,
+                    }), i().createElement(Ue, {
+                        onChange: h,
+                        rgb: p,
                         hsv: d,
                         hex: c
                     }))))))
                 })),
-                be = e => {
+                Ye = e => {
                     let {
                         onChange: t = (() => {}),
                         rgb: r,
                         hsl: n,
                         hex: a,
                         disableAlpha: o
                     } = e;
@@ -2644,15 +3361,15 @@
                                 color: "#222",
                                 paddingTop: "3px",
                                 paddingBottom: "4px",
                                 textTransform: "capitalize"
                             }
                         },
                         s = (e, a) => {
-                            "string" != typeof e && "hex" in e ? y(e.hex) && t({
+                            "string" != typeof e && "hex" in e ? Q(e.hex) && t({
                                 hex: e.hex,
                                 source: "hex"
                             }, a) : "string" != typeof e && ("r" in e || "g" in e || "b" in e) ? t({
                                 r: e.r || r.r,
                                 g: e.g || r.g,
                                 b: e.b || r.b,
                                 a: r.a,
@@ -2666,74 +3383,74 @@
                             }, a))
                         };
                     return i().createElement("div", {
                         style: l.fields,
                         className: "flexbox-fix"
                     }, i().createElement("div", {
                         style: l.double
-                    }, i().createElement(H, {
+                    }, i().createElement(ge, {
                         style: {
                             input: l.input,
                             label: l.label
                         },
                         label: "hex",
                         value: a.replace("#", ""),
                         onChange: s
                     })), i().createElement("div", {
                         style: l.single
-                    }, i().createElement(H, {
+                    }, i().createElement(ge, {
                         style: {
                             input: l.input,
                             label: l.label
                         },
                         label: "r",
                         value: r.r,
                         onChange: s,
                         dragLabel: "true",
                         dragMax: "255"
                     })), i().createElement("div", {
                         style: l.single
-                    }, i().createElement(H, {
+                    }, i().createElement(ge, {
                         style: {
                             input: l.input,
                             label: l.label
                         },
                         label: "g",
                         value: r.g,
                         onChange: s,
                         dragLabel: "true",
                         dragMax: "255"
                     })), i().createElement("div", {
                         style: l.single
-                    }, i().createElement(H, {
+                    }, i().createElement(ge, {
                         style: {
                             input: l.input,
                             label: l.label
                         },
                         label: "b",
                         value: r.b,
                         onChange: s,
                         dragLabel: "true",
                         dragMax: "255"
                     })), i().createElement("div", {
                         style: l.alpha
-                    }, i().createElement(H, {
+                    }, i().createElement(ge, {
                         style: {
                             input: l.input,
                             label: l.label
                         },
                         label: "a",
                         value: Math.round(100 * (r.a ?? 1)),
                         onChange: s,
                         dragLabel: "true",
                         dragMax: "100"
                     })))
                 };
 
-            function fe(e) {
+            function qe(e) {
                 let {
                     colors: t,
                     onClick: r = (() => {})
                 } = e;
                 const a = {
                         colors: {
                             margin: "0 -10px",
@@ -2766,41 +3483,41 @@
                     const t = "string" == typeof e ? {
                             color: e
                         } : e,
                         r = `${t.color}${("title"in t?t.title:"")||""}`;
                     return i().createElement("div", {
                         key: r,
                         style: a.swatchWrap
-                    }, i().createElement(G, n({}, t, {
+                    }, i().createElement(me, n({}, t, {
                         style: a.swatch,
                         onClick: o,
                         focusStyle: {
                             boxShadow: `inset 0 0 0 1px rgba(0,0,0,.15), 0 0 4px ${t.color}`
                         }
                     })))
                 })))
             }
-            var xe = S((function(e) {
+            var Ze = ie((function(e) {
                 let {
                     width: t = 200,
                     disableAlpha: r = !1,
                     presetColors: n = ["#D0021B", "#F5A623", "#F8E71C", "#8B572A", "#7ED321", "#417505", "#BD10E0", "#9013FE", "#4A90E2", "#50E3C2", "#B8E986", "#000000", "#4A4A4A", "#9B9B9B", "#FFFFFF"],
                     renderers: a,
                     styles: o = {},
                     className: l = ""
                 } = e;
                 const {
                     colors: s,
-                    changeColor: p
-                } = F(), {
-                    rgb: h,
+                    changeColor: h
+                } = ae(), {
+                    rgb: p,
                     hex: c,
                     hsv: d,
                     hsl: u
-                } = s, g = x()({
+                } = s, g = Z()({
                     picker: {
                         width: t,
                         padding: "10px 10px 0",
                         boxSizing: "initial",
                         background: "#fff",
                         borderRadius: "4px",
                         boxShadow: "0 0 0 1px rgba(0,0,0,.15), 0 8px 16px rgba(0,0,0,.15)"
@@ -2830,15 +3547,15 @@
                         marginLeft: "4px",
                         borderRadius: "3px"
                     },
                     activeColor: {
                         position: "absolute",
                         inset: "0px",
                         borderRadius: "2px",
-                        background: `rgba(${h.r},${h.g},${h.b},${h.a})`,
+                        background: `rgba(${p.r},${p.g},${p.b},${p.a})`,
                         boxShadow: "inset 0 0 0 1px rgba(0,0,0,.15), inset 0 0 4px rgba(0,0,0,.25)"
                     },
                     hue: {
                         position: "relative",
                         height: "10px",
                         overflow: "hidden"
                     },
@@ -2860,68 +3577,68 @@
                     ...o
                 }, o);
                 return i().createElement("div", {
                     style: g.picker,
                     className: `sketch-picker ${l}`
                 }, i().createElement("div", {
                     style: g.saturation
-                }, i().createElement(T, {
+                }, i().createElement(xe, {
                     style: g.Saturation,
                     hsl: u,
                     hsv: d,
-                    onChange: p
+                    onChange: h
                 })), i().createElement("div", {
                     style: g.controls,
                     className: "flexbox-fix"
                 }, i().createElement("div", {
                     style: g.sliders
                 }, i().createElement("div", {
                     style: g.hue
-                }, i().createElement(L, {
+                }, i().createElement(be, {
                     style: g.Hue,
                     hsl: u,
-                    onChange: p
+                    onChange: h
                 })), i().createElement("div", {
                     style: g.alpha
-                }, i().createElement(_, {
+                }, i().createElement(he, {
                     style: g.Alpha,
-                    rgb: h,
+                    rgb: p,
                     hsl: u,
                     renderers: a,
-                    onChange: p
+                    onChange: h
                 }))), i().createElement("div", {
                     style: g.color
-                }, i().createElement(A, null), i().createElement("div", {
+                }, i().createElement(se, null), i().createElement("div", {
                     style: g.activeColor
-                }))), i().createElement(be, {
-                    rgb: h,
+                }))), i().createElement(Ye, {
+                    rgb: p,
                     hsl: u,
                     hex: c,
-                    onChange: p,
+                    onChange: h,
                     disableAlpha: r
-                }), i().createElement(fe, {
+                }), i().createElement(qe, {
                     colors: n,
-                    onClick: p
+                    onClick: h
                 }))
             }));
 
-            function me() {
+            function Ke() {
                 return i().createElement("div", {
                     style: {
                         width: "14px",
                         height: "14px",
                         borderRadius: "6px",
                         transform: "translate(-7px, -1px)",
                         backgroundColor: "rgb(248, 248, 248)",
                         boxShadow: "0 1px 4px 0 rgba(0, 0, 0, 0.37)"
                     }
                 })
             }
 
-            function ve(e) {
+            function Je(e) {
                 let {
                     hsl: t,
                     offset: r,
                     onClick: n = (() => {}),
                     active: a,
                     first: o,
                     last: l
@@ -2942,15 +3659,15 @@
                         s: .5,
                         l: r,
                         source: "hsl"
                     }, e)
                 })
             }
 
-            function ye(e) {
+            function Qe(e) {
                 let {
                     onClick: t,
                     hsl: r
                 } = e;
                 const n = {
                         swatches: {
                             marginTop: "20px"
@@ -2966,92 +3683,93 @@
                         }
                     },
                     a = .1;
                 return i().createElement("div", {
                     style: n.swatches
                 }, i().createElement("div", {
                     style: n.swatch
-                }, i().createElement(ve, {
+                }, i().createElement(Je, {
                     hsl: r,
                     offset: .8,
                     active: Math.abs(r.l - .8) < a && Math.abs(r.s - .5) < a,
                     onClick: t,
                     first: !0
                 })), i().createElement("div", {
                     style: n.swatch
-                }, i().createElement(ve, {
+                }, i().createElement(Je, {
                     hsl: r,
                     offset: .65,
                     active: Math.abs(r.l - .65) < a && Math.abs(r.s - .5) < a,
                     onClick: t
                 })), i().createElement("div", {
                     style: n.swatch
-                }, i().createElement(ve, {
+                }, i().createElement(Je, {
                     hsl: r,
                     offset: .5,
                     active: Math.abs(r.l - .5) < a && Math.abs(r.s - .5) < a,
                     onClick: t
                 })), i().createElement("div", {
                     style: n.swatch
-                }, i().createElement(ve, {
+                }, i().createElement(Je, {
                     hsl: r,
                     offset: .35,
                     active: Math.abs(r.l - .35) < a && Math.abs(r.s - .5) < a,
                     onClick: t
                 })), i().createElement("div", {
                     style: n.swatch
-                }, i().createElement(ve, {
+                }, i().createElement(Je, {
                     hsl: r,
                     offset: .2,
                     active: Math.abs(r.l - .2) < a && Math.abs(r.s - .5) < a,
                     onClick: t,
                     last: !0
                 })), i().createElement("div", {
                     style: n.clear
                 }))
             }
-            var we = S((e => {
-                let {
-                    pointer: t = me,
-                    styles: r = {},
-                    className: n = ""
-                } = e;
-                const {
-                    colors: a,
-                    changeColor: o
-                } = F(), {
-                    hsl: l
-                } = a, s = x()({
-                    hue: {
-                        height: "12px",
-                        position: "relative"
-                    },
-                    Hue: {
-                        borderRadius: "2px"
-                    }
-                }, r);
-                return i().createElement("div", {
-                    style: s.wrap || {},
-                    className: `slider-picker ${n}`
-                }, i().createElement("div", {
-                    style: s.hue
-                }, i().createElement(L, {
-                    style: s.Hue,
-                    hsl: l,
-                    pointer: t,
-                    onChange: o
-                })), i().createElement("div", {
-                    style: s.swatches
-                }, i().createElement(ye, {
-                    hsl: l,
-                    onClick: o
-                })))
-            }));
+            var et = ie((e => {
+                    let {
+                        pointer: t = Ke,
+                        styles: r = {},
+                        className: n = ""
+                    } = e;
+                    const {
+                        colors: a,
+                        changeColor: o
+                    } = ae(), {
+                        hsl: l
+                    } = a, s = Z()({
+                        hue: {
+                            height: "12px",
+                            position: "relative"
+                        },
+                        Hue: {
+                            borderRadius: "2px"
+                        }
+                    }, r);
+                    return i().createElement("div", {
+                        style: s.wrap || {},
+                        className: `slider-picker ${n}`
+                    }, i().createElement("div", {
+                        style: s.hue
+                    }, i().createElement(be, {
+                        style: s.Hue,
+                        hsl: l,
+                        pointer: t,
+                        onChange: o
+                    })), i().createElement("div", {
+                        style: s.swatches
+                    }, i().createElement(Qe, {
+                        hsl: l,
+                        onClick: o
+                    })))
+                })),
+                tt = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZD0iTTIxLDdMOSwxOUwzLjUsMTMuNUw0LjkxLDEyLjA5TDksMTYuMTdMMTkuNTksNS41OUwyMSw3WiIgLz48L3N2Zz4=";
 
-            function Ee(e) {
+            function rt(e) {
                 let {
                     color: t,
                     onClick: r = (() => {}),
                     first: n,
                     last: a,
                     active: o
                 } = e;
@@ -3063,20 +3781,20 @@
                         background: t,
                         marginBottom: "1px",
                         overflow: n || a ? "hidden" : void 0,
                         borderRadius: n ? "2px 2px 0 0" : a ? "0 0 2px 2px" : void 0,
                         boxShadow: "#FFFFFF" === t ? "inset 0 0 0 1px #ddd" : void 0
                     },
                     check: {
-                        color: "#FFFFFF" === t || "transparent" === t ? "#333" : w(t),
+                        color: "#FFFFFF" === t || "transparent" === t ? "#333" : ee(t),
                         marginLeft: "8px",
                         display: o ? "block" : "none"
                     }
                 };
-                return i().createElement(G, {
+                return i().createElement(me, {
                     color: t,
                     style: l.color,
                     onClick: r,
                     focusStyle: {
                         boxShadow: `0 0 4px ${t}`
                     }
                 }, i().createElement("div", {
@@ -3084,41 +3802,41 @@
                 }, i().createElement("img", {
                     width: "24",
                     height: "24",
                     style: {
                         fill: "white",
                         stroke: "white"
                     },
-                    src: "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZD0iTTIxLDdMOSwxOUwzLjUsMTMuNUw0LjkxLDEyLjA5TDksMTYuMTdMMTkuNTksNS41OUwyMSw3WiIgLz48L3N2Zz4="
+                    src: tt
                 })))
             }
 
-            function Ce(e) {
+            function nt(e) {
                 let {
                     onClick: t,
                     group: r,
                     active: n
                 } = e;
                 return i().createElement("div", {
                     style: {
                         paddingBottom: "10px",
                         width: "40px",
                         float: "left",
                         marginRight: "10px"
                     }
-                }, r.map(((e, a) => i().createElement(Ee, {
+                }, r.map(((e, a) => i().createElement(rt, {
                     key: e,
                     color: e,
                     active: e.toLowerCase() === n,
                     first: 0 === a,
                     last: a === r.length - 1,
                     onClick: t
                 }))))
             }
-            var ke = S((function(e) {
+            var at = ie((function(e) {
                     let {
                         width: t = 320,
                         height: r = 240,
                         colors: n = [
                             ["#B71C1C", "#D32F2F", "#F44336", "#E57373", "#FFCDD2"],
                             ["#880E4F", "#C2185B", "#E91E63", "#F06292", "#F8BBD0"],
                             ["#4A148C", "#7B1FA2", "#9C27B0", "#BA68C8", "#E1BEE7"],
@@ -3141,17 +3859,17 @@
                         ],
                         styles: a = {},
                         className: o = ""
                     } = e;
                     const {
                         colors: l,
                         changeColor: s
-                    } = F(), {
-                        hex: p
-                    } = l, h = x()({
+                    } = ae(), {
+                        hex: h
+                    } = l, p = Z()({
                         picker: {
                             width: t,
                             height: r
                         },
                         overflow: {
                             height: r,
                             overflowY: "scroll"
@@ -3163,43 +3881,43 @@
                             clear: "both"
                         }
                     }, a), c = (e, t) => s({
                         hex: e,
                         source: "hex"
                     }, t);
                     return i().createElement("div", {
-                        style: h.picker,
+                        style: p.picker,
                         className: `swatches-picker ${o}`
-                    }, i().createElement(z, null, i().createElement("div", {
-                        style: h.overflow
+                    }, i().createElement(fe, null, i().createElement("div", {
+                        style: p.overflow
                     }, i().createElement("div", {
-                        style: h.body
-                    }, n.map((e => i().createElement(Ce, {
+                        style: p.body
+                    }, n.map((e => i().createElement(nt, {
                         key: e.toString(),
                         group: e,
-                        active: p,
+                        active: h,
                         onClick: c
                     }))), i().createElement("div", {
-                        style: h.clear
+                        style: p.clear
                     })))))
                 })),
-                Fe = S((e => {
+                it = ie((e => {
                     let {
                         colors: t = ["#FF6900", "#FCB900", "#7BDCB5", "#00D084", "#8ED1FC", "#0693E3", "#ABB8C3", "#EB144C", "#F78DA7", "#9900EF"],
                         width: r = 276,
                         triangle: n = "top-left",
                         styles: a = {},
                         className: o = ""
                     } = e;
                     const {
                         colors: l,
                         changeColor: s
-                    } = F(), {
-                        hex: p
-                    } = l, h = x()({
+                    } = ae(), {
+                        hex: h
+                    } = l, p = Z()({
                         card: {
                             width: r,
                             background: "#fff",
                             border: "0 solid rgba(0,0,0,0.25)",
                             boxShadow: "0 1px 4px rgba(0,0,0,0.25)",
                             borderRadius: "4px",
                             position: "relative"
@@ -3264,48 +3982,48 @@
                             borderRadius: "4px",
                             margin: "0 6px 6px 0"
                         },
                         clear: {
                             clear: "both"
                         }
                     }, a), c = (e, t) => {
-                        y(e) && s({
+                        Q(e) && s({
                             hex: e,
                             source: "hex"
                         }, t)
                     };
                     return i().createElement("div", {
-                        style: h.card,
+                        style: p.card,
                         className: `twitter-picker ${o}`
                     }, i().createElement("div", {
-                        style: h.triangleShadow
+                        style: p.triangleShadow
                     }), i().createElement("div", {
-                        style: h.triangle
+                        style: p.triangle
                     }), i().createElement("div", {
-                        style: h.body
-                    }, t.map(((e, t) => i().createElement(G, {
+                        style: p.body
+                    }, t.map(((e, t) => i().createElement(me, {
                         key: t,
                         color: e,
                         hex: e,
-                        style: h.swatch,
+                        style: p.swatch,
                         onClick: c,
                         focusStyle: {
                             boxShadow: `0 0 4px ${e}`
                         }
                     }))), i().createElement("div", {
-                        style: h.hash
-                    }, "#"), i().createElement(H, {
+                        style: p.hash
+                    }, "#"), i().createElement(ge, {
                         label: null,
                         style: {
-                            input: h.input
+                            input: p.input
                         },
-                        value: p.replace("#", ""),
+                        value: h.replace("#", ""),
                         onChange: c
                     }), i().createElement("div", {
-                        style: h.clear
+                        style: p.clear
                     })))
                 }))
         },
         7561: (e, t, r) => {
             var n = r(7990),
                 a = /^\s+/;
             e.exports = function(e) {
@@ -3322,62 +4040,60 @@
         3279: (e, t, r) => {
             var n = r(3218),
                 a = r(7771),
                 i = r(4841),
                 o = Math.max,
                 l = Math.min;
             e.exports = function(e, t, r) {
-                var s, p, h, c, d, u, g = 0,
+                var s, h, p, c, d, u, g = 0,
                     b = !1,
                     f = !1,
                     x = !0;
                 if ("function" != typeof e) throw new TypeError("Expected a function");
 
                 function m(t) {
                     var r = s,
-                        n = p;
-                    return s = p = void 0, g = t, c = e.apply(n, r)
+                        n = h;
+                    return s = h = void 0, g = t, c = e.apply(n, r)
                 }
 
                 function v(e) {
-                    return g = e, d = setTimeout(w, t), b ? m(e) : c
-                }
-
-                function y(e) {
                     var r = e - u;
-                    return void 0 === u || r >= t || r < 0 || f && e - g >= h
+                    return void 0 === u || r >= t || r < 0 || f && e - g >= p
                 }
 
-                function w() {
+                function y() {
                     var e = a();
-                    if (y(e)) return E(e);
-                    d = setTimeout(w, function(e) {
+                    if (v(e)) return w(e);
+                    d = setTimeout(y, function(e) {
                         var r = t - (e - u);
-                        return f ? l(r, h - (e - g)) : r
+                        return f ? l(r, p - (e - g)) : r
                     }(e))
                 }
 
-                function E(e) {
-                    return d = void 0, x && s ? m(e) : (s = p = void 0, c)
+                function w(e) {
+                    return d = void 0, x && s ? m(e) : (s = h = void 0, c)
                 }
 
-                function C() {
+                function E() {
                     var e = a(),
-                        r = y(e);
-                    if (s = arguments, p = this, u = e, r) {
-                        if (void 0 === d) return v(u);
-                        if (f) return clearTimeout(d), d = setTimeout(w, t), m(u)
-                    }
-                    return void 0 === d && (d = setTimeout(w, t)), c
-                }
-                return t = i(t) || 0, n(r) && (b = !!r.leading, h = (f = "maxWait" in r) ? o(i(r.maxWait) || 0, t) : h, x = "trailing" in r ? !!r.trailing : x), C.cancel = function() {
-                    void 0 !== d && clearTimeout(d), g = 0, s = u = p = d = void 0
-                }, C.flush = function() {
-                    return void 0 === d ? c : E(a())
-                }, C
+                        r = v(e);
+                    if (s = arguments, h = this, u = e, r) {
+                        if (void 0 === d) return function(e) {
+                            return g = e, d = setTimeout(y, t), b ? m(e) : c
+                        }(u);
+                        if (f) return clearTimeout(d), d = setTimeout(y, t), m(u)
+                    }
+                    return void 0 === d && (d = setTimeout(y, t)), c
+                }
+                return t = i(t) || 0, n(r) && (b = !!r.leading, p = (f = "maxWait" in r) ? o(i(r.maxWait) || 0, t) : p, x = "trailing" in r ? !!r.trailing : x), E.cancel = function() {
+                    void 0 !== d && clearTimeout(d), g = 0, s = u = h = d = void 0
+                }, E.flush = function() {
+                    return void 0 === d ? c : w(a())
+                }, E
             }
         },
         6073: (e, t, r) => {
             e.exports = r(4486)
         },
         3857: (e, t, r) => {
             var n = r(2980),
@@ -3395,772 +4111,23 @@
         4841: (e, t, r) => {
             var n = r(7561),
                 a = r(3218),
                 i = r(3448),
                 o = /^[-+]0x[0-9a-f]+$/i,
                 l = /^0b[01]+$/i,
                 s = /^0o[0-7]+$/i,
-                p = parseInt;
+                h = parseInt;
             e.exports = function(e) {
                 if ("number" == typeof e) return e;
                 if (i(e)) return NaN;
                 if (a(e)) {
                     var t = "function" == typeof e.valueOf ? e.valueOf() : e;
                     e = a(t) ? t + "" : t
                 }
                 if ("string" != typeof e) return 0 === e ? e : +e;
                 e = n(e);
                 var r = l.test(e);
-                return r || s.test(e) ? p(e.slice(2), r ? 2 : 8) : o.test(e) ? NaN : +e
+                return r || s.test(e) ? h(e.slice(2), r ? 2 : 8) : o.test(e) ? NaN : +e
             }
-        },
-        7621: (e, t, r) => {
-            var n;
-            ! function(a) {
-                var i = /^\s+/,
-                    o = /\s+$/,
-                    l = 0,
-                    s = a.round,
-                    p = a.min,
-                    h = a.max,
-                    c = a.random;
-
-                function d(e, t) {
-                    if (t = t || {}, (e = e || "") instanceof d) return e;
-                    if (!(this instanceof d)) return new d(e, t);
-                    var r = function(e) {
-                        var t, r, n, l = {
-                                r: 0,
-                                g: 0,
-                                b: 0
-                            },
-                            s = 1,
-                            c = null,
-                            d = null,
-                            u = null,
-                            g = !1,
-                            b = !1;
-                        return "string" == typeof e && (e = function(e) {
-                            e = e.replace(i, "").replace(o, "").toLowerCase();
-                            var t, r = !1;
-                            if (_[e]) e = _[e], r = !0;
-                            else if ("transparent" == e) return {
-                                r: 0,
-                                g: 0,
-                                b: 0,
-                                a: 0,
-                                format: "name"
-                            };
-                            return (t = U.rgb.exec(e)) ? {
-                                r: t[1],
-                                g: t[2],
-                                b: t[3]
-                            } : (t = U.rgba.exec(e)) ? {
-                                r: t[1],
-                                g: t[2],
-                                b: t[3],
-                                a: t[4]
-                            } : (t = U.hsl.exec(e)) ? {
-                                h: t[1],
-                                s: t[2],
-                                l: t[3]
-                            } : (t = U.hsla.exec(e)) ? {
-                                h: t[1],
-                                s: t[2],
-                                l: t[3],
-                                a: t[4]
-                            } : (t = U.hsv.exec(e)) ? {
-                                h: t[1],
-                                s: t[2],
-                                v: t[3]
-                            } : (t = U.hsva.exec(e)) ? {
-                                h: t[1],
-                                s: t[2],
-                                v: t[3],
-                                a: t[4]
-                            } : (t = U.hex8.exec(e)) ? {
-                                r: H(t[1]),
-                                g: H(t[2]),
-                                b: H(t[3]),
-                                a: G(t[4]),
-                                format: r ? "name" : "hex8"
-                            } : (t = U.hex6.exec(e)) ? {
-                                r: H(t[1]),
-                                g: H(t[2]),
-                                b: H(t[3]),
-                                format: r ? "name" : "hex"
-                            } : (t = U.hex4.exec(e)) ? {
-                                r: H(t[1] + "" + t[1]),
-                                g: H(t[2] + "" + t[2]),
-                                b: H(t[3] + "" + t[3]),
-                                a: G(t[4] + "" + t[4]),
-                                format: r ? "name" : "hex8"
-                            } : !!(t = U.hex3.exec(e)) && {
-                                r: H(t[1] + "" + t[1]),
-                                g: H(t[2] + "" + t[2]),
-                                b: H(t[3] + "" + t[3]),
-                                format: r ? "name" : "hex"
-                            }
-                        }(e)), "object" == typeof e && (I(e.r) && I(e.g) && I(e.b) ? (t = e.r, r = e.g, n = e.b, l = {
-                            r: 255 * N(t, 255),
-                            g: 255 * N(r, 255),
-                            b: 255 * N(n, 255)
-                        }, g = !0, b = "%" === String(e.r).substr(-1) ? "prgb" : "rgb") : I(e.h) && I(e.s) && I(e.v) ? (c = z(e.s), d = z(e.v), l = function(e, t, r) {
-                            e = 6 * N(e, 360), t = N(t, 100), r = N(r, 100);
-                            var n = a.floor(e),
-                                i = e - n,
-                                o = r * (1 - t),
-                                l = r * (1 - i * t),
-                                s = r * (1 - (1 - i) * t),
-                                p = n % 6;
-                            return {
-                                r: 255 * [r, l, o, o, s, r][p],
-                                g: 255 * [s, r, r, l, o, o][p],
-                                b: 255 * [o, o, s, r, r, l][p]
-                            }
-                        }(e.h, c, d), g = !0, b = "hsv") : I(e.h) && I(e.s) && I(e.l) && (c = z(e.s), u = z(e.l), l = function(e, t, r) {
-                            var n, a, i;
-
-                            function o(e, t, r) {
-                                return r < 0 && (r += 1), r > 1 && (r -= 1), r < 1 / 6 ? e + 6 * (t - e) * r : r < .5 ? t : r < 2 / 3 ? e + (t - e) * (2 / 3 - r) * 6 : e
-                            }
-                            if (e = N(e, 360), t = N(t, 100), r = N(r, 100), 0 === t) n = a = i = r;
-                            else {
-                                var l = r < .5 ? r * (1 + t) : r + t - r * t,
-                                    s = 2 * r - l;
-                                n = o(s, l, e + 1 / 3), a = o(s, l, e), i = o(s, l, e - 1 / 3)
-                            }
-                            return {
-                                r: 255 * n,
-                                g: 255 * a,
-                                b: 255 * i
-                            }
-                        }(e.h, c, u), g = !0, b = "hsl"), e.hasOwnProperty("a") && (s = e.a)), s = M(s), {
-                            ok: g,
-                            format: e.format || b,
-                            r: p(255, h(l.r, 0)),
-                            g: p(255, h(l.g, 0)),
-                            b: p(255, h(l.b, 0)),
-                            a: s
-                        }
-                    }(e);
-                    this._originalInput = e, this._r = r.r, this._g = r.g, this._b = r.b, this._a = r.a, this._roundA = s(100 * this._a) / 100, this._format = t.format || r.format, this._gradientType = t.gradientType, this._r < 1 && (this._r = s(this._r)), this._g < 1 && (this._g = s(this._g)), this._b < 1 && (this._b = s(this._b)), this._ok = r.ok, this._tc_id = l++
-                }
-
-                function u(e, t, r) {
-                    e = N(e, 255), t = N(t, 255), r = N(r, 255);
-                    var n, a, i = h(e, t, r),
-                        o = p(e, t, r),
-                        l = (i + o) / 2;
-                    if (i == o) n = a = 0;
-                    else {
-                        var s = i - o;
-                        switch (a = l > .5 ? s / (2 - i - o) : s / (i + o), i) {
-                            case e:
-                                n = (t - r) / s + (t < r ? 6 : 0);
-                                break;
-                            case t:
-                                n = (r - e) / s + 2;
-                                break;
-                            case r:
-                                n = (e - t) / s + 4
-                        }
-                        n /= 6
-                    }
-                    return {
-                        h: n,
-                        s: a,
-                        l
-                    }
-                }
-
-                function g(e, t, r) {
-                    e = N(e, 255), t = N(t, 255), r = N(r, 255);
-                    var n, a, i = h(e, t, r),
-                        o = p(e, t, r),
-                        l = i,
-                        s = i - o;
-                    if (a = 0 === i ? 0 : s / i, i == o) n = 0;
-                    else {
-                        switch (i) {
-                            case e:
-                                n = (t - r) / s + (t < r ? 6 : 0);
-                                break;
-                            case t:
-                                n = (r - e) / s + 2;
-                                break;
-                            case r:
-                                n = (e - t) / s + 4
-                        }
-                        n /= 6
-                    }
-                    return {
-                        h: n,
-                        s: a,
-                        v: l
-                    }
-                }
-
-                function b(e, t, r, n) {
-                    var a = [L(s(e).toString(16)), L(s(t).toString(16)), L(s(r).toString(16))];
-                    return n && a[0].charAt(0) == a[0].charAt(1) && a[1].charAt(0) == a[1].charAt(1) && a[2].charAt(0) == a[2].charAt(1) ? a[0].charAt(0) + a[1].charAt(0) + a[2].charAt(0) : a.join("")
-                }
-
-                function f(e, t, r, n) {
-                    return [L(T(n)), L(s(e).toString(16)), L(s(t).toString(16)), L(s(r).toString(16))].join("")
-                }
-
-                function x(e, t) {
-                    t = 0 === t ? 0 : t || 10;
-                    var r = d(e).toHsl();
-                    return r.s -= t / 100, r.s = $(r.s), d(r)
-                }
-
-                function m(e, t) {
-                    t = 0 === t ? 0 : t || 10;
-                    var r = d(e).toHsl();
-                    return r.s += t / 100, r.s = $(r.s), d(r)
-                }
-
-                function v(e) {
-                    return d(e).desaturate(100)
-                }
-
-                function y(e, t) {
-                    t = 0 === t ? 0 : t || 10;
-                    var r = d(e).toHsl();
-                    return r.l += t / 100, r.l = $(r.l), d(r)
-                }
-
-                function w(e, t) {
-                    t = 0 === t ? 0 : t || 10;
-                    var r = d(e).toRgb();
-                    return r.r = h(0, p(255, r.r - s(-t / 100 * 255))), r.g = h(0, p(255, r.g - s(-t / 100 * 255))), r.b = h(0, p(255, r.b - s(-t / 100 * 255))), d(r)
-                }
-
-                function E(e, t) {
-                    t = 0 === t ? 0 : t || 10;
-                    var r = d(e).toHsl();
-                    return r.l -= t / 100, r.l = $(r.l), d(r)
-                }
-
-                function C(e, t) {
-                    var r = d(e).toHsl(),
-                        n = (r.h + t) % 360;
-                    return r.h = n < 0 ? 360 + n : n, d(r)
-                }
-
-                function k(e) {
-                    var t = d(e).toHsl();
-                    return t.h = (t.h + 180) % 360, d(t)
-                }
-
-                function F(e) {
-                    var t = d(e).toHsl(),
-                        r = t.h;
-                    return [d(e), d({
-                        h: (r + 120) % 360,
-                        s: t.s,
-                        l: t.l
-                    }), d({
-                        h: (r + 240) % 360,
-                        s: t.s,
-                        l: t.l
-                    })]
-                }
-
-                function S(e) {
-                    var t = d(e).toHsl(),
-                        r = t.h;
-                    return [d(e), d({
-                        h: (r + 90) % 360,
-                        s: t.s,
-                        l: t.l
-                    }), d({
-                        h: (r + 180) % 360,
-                        s: t.s,
-                        l: t.l
-                    }), d({
-                        h: (r + 270) % 360,
-                        s: t.s,
-                        l: t.l
-                    })]
-                }
-
-                function B(e) {
-                    var t = d(e).toHsl(),
-                        r = t.h;
-                    return [d(e), d({
-                        h: (r + 72) % 360,
-                        s: t.s,
-                        l: t.l
-                    }), d({
-                        h: (r + 216) % 360,
-                        s: t.s,
-                        l: t.l
-                    })]
-                }
-
-                function R(e, t, r) {
-                    t = t || 6, r = r || 30;
-                    var n = d(e).toHsl(),
-                        a = 360 / r,
-                        i = [d(e)];
-                    for (n.h = (n.h - (a * t >> 1) + 720) % 360; --t;) n.h = (n.h + a) % 360, i.push(d(n));
-                    return i
-                }
-
-                function A(e, t) {
-                    t = t || 6;
-                    for (var r = d(e).toHsv(), n = r.h, a = r.s, i = r.v, o = [], l = 1 / t; t--;) o.push(d({
-                        h: n,
-                        s: a,
-                        v: i
-                    })), i = (i + l) % 1;
-                    return o
-                }
-                d.prototype = {
-                    isDark: function() {
-                        return this.getBrightness() < 128
-                    },
-                    isLight: function() {
-                        return !this.isDark()
-                    },
-                    isValid: function() {
-                        return this._ok
-                    },
-                    getOriginalInput: function() {
-                        return this._originalInput
-                    },
-                    getFormat: function() {
-                        return this._format
-                    },
-                    getAlpha: function() {
-                        return this._a
-                    },
-                    getBrightness: function() {
-                        var e = this.toRgb();
-                        return (299 * e.r + 587 * e.g + 114 * e.b) / 1e3
-                    },
-                    getLuminance: function() {
-                        var e, t, r, n = this.toRgb();
-                        return e = n.r / 255, t = n.g / 255, r = n.b / 255, .2126 * (e <= .03928 ? e / 12.92 : a.pow((e + .055) / 1.055, 2.4)) + .7152 * (t <= .03928 ? t / 12.92 : a.pow((t + .055) / 1.055, 2.4)) + .0722 * (r <= .03928 ? r / 12.92 : a.pow((r + .055) / 1.055, 2.4))
-                    },
-                    setAlpha: function(e) {
-                        return this._a = M(e), this._roundA = s(100 * this._a) / 100, this
-                    },
-                    toHsv: function() {
-                        var e = g(this._r, this._g, this._b);
-                        return {
-                            h: 360 * e.h,
-                            s: e.s,
-                            v: e.v,
-                            a: this._a
-                        }
-                    },
-                    toHsvString: function() {
-                        var e = g(this._r, this._g, this._b),
-                            t = s(360 * e.h),
-                            r = s(100 * e.s),
-                            n = s(100 * e.v);
-                        return 1 == this._a ? "hsv(" + t + ", " + r + "%, " + n + "%)" : "hsva(" + t + ", " + r + "%, " + n + "%, " + this._roundA + ")"
-                    },
-                    toHsl: function() {
-                        var e = u(this._r, this._g, this._b);
-                        return {
-                            h: 360 * e.h,
-                            s: e.s,
-                            l: e.l,
-                            a: this._a
-                        }
-                    },
-                    toHslString: function() {
-                        var e = u(this._r, this._g, this._b),
-                            t = s(360 * e.h),
-                            r = s(100 * e.s),
-                            n = s(100 * e.l);
-                        return 1 == this._a ? "hsl(" + t + ", " + r + "%, " + n + "%)" : "hsla(" + t + ", " + r + "%, " + n + "%, " + this._roundA + ")"
-                    },
-                    toHex: function(e) {
-                        return b(this._r, this._g, this._b, e)
-                    },
-                    toHexString: function(e) {
-                        return "#" + this.toHex(e)
-                    },
-                    toHex8: function(e) {
-                        return function(e, t, r, n, a) {
-                            var i = [L(s(e).toString(16)), L(s(t).toString(16)), L(s(r).toString(16)), L(T(n))];
-                            return a && i[0].charAt(0) == i[0].charAt(1) && i[1].charAt(0) == i[1].charAt(1) && i[2].charAt(0) == i[2].charAt(1) && i[3].charAt(0) == i[3].charAt(1) ? i[0].charAt(0) + i[1].charAt(0) + i[2].charAt(0) + i[3].charAt(0) : i.join("")
-                        }(this._r, this._g, this._b, this._a, e)
-                    },
-                    toHex8String: function(e) {
-                        return "#" + this.toHex8(e)
-                    },
-                    toRgb: function() {
-                        return {
-                            r: s(this._r),
-                            g: s(this._g),
-                            b: s(this._b),
-                            a: this._a
-                        }
-                    },
-                    toRgbString: function() {
-                        return 1 == this._a ? "rgb(" + s(this._r) + ", " + s(this._g) + ", " + s(this._b) + ")" : "rgba(" + s(this._r) + ", " + s(this._g) + ", " + s(this._b) + ", " + this._roundA + ")"
-                    },
-                    toPercentageRgb: function() {
-                        return {
-                            r: s(100 * N(this._r, 255)) + "%",
-                            g: s(100 * N(this._g, 255)) + "%",
-                            b: s(100 * N(this._b, 255)) + "%",
-                            a: this._a
-                        }
-                    },
-                    toPercentageRgbString: function() {
-                        return 1 == this._a ? "rgb(" + s(100 * N(this._r, 255)) + "%, " + s(100 * N(this._g, 255)) + "%, " + s(100 * N(this._b, 255)) + "%)" : "rgba(" + s(100 * N(this._r, 255)) + "%, " + s(100 * N(this._g, 255)) + "%, " + s(100 * N(this._b, 255)) + "%, " + this._roundA + ")"
-                    },
-                    toName: function() {
-                        return 0 === this._a ? "transparent" : !(this._a < 1) && (D[b(this._r, this._g, this._b, !0)] || !1)
-                    },
-                    toFilter: function(e) {
-                        var t = "#" + f(this._r, this._g, this._b, this._a),
-                            r = t,
-                            n = this._gradientType ? "GradientType = 1, " : "";
-                        if (e) {
-                            var a = d(e);
-                            r = "#" + f(a._r, a._g, a._b, a._a)
-                        }
-                        return "progid:DXImageTransform.Microsoft.gradient(" + n + "startColorstr=" + t + ",endColorstr=" + r + ")"
-                    },
-                    toString: function(e) {
-                        var t = !!e;
-                        e = e || this._format;
-                        var r = !1,
-                            n = this._a < 1 && this._a >= 0;
-                        return t || !n || "hex" !== e && "hex6" !== e && "hex3" !== e && "hex4" !== e && "hex8" !== e && "name" !== e ? ("rgb" === e && (r = this.toRgbString()), "prgb" === e && (r = this.toPercentageRgbString()), "hex" !== e && "hex6" !== e || (r = this.toHexString()), "hex3" === e && (r = this.toHexString(!0)), "hex4" === e && (r = this.toHex8String(!0)), "hex8" === e && (r = this.toHex8String()), "name" === e && (r = this.toName()), "hsl" === e && (r = this.toHslString()), "hsv" === e && (r = this.toHsvString()), r || this.toHexString()) : "name" === e && 0 === this._a ? this.toName() : this.toRgbString()
-                    },
-                    clone: function() {
-                        return d(this.toString())
-                    },
-                    _applyModification: function(e, t) {
-                        var r = e.apply(null, [this].concat([].slice.call(t)));
-                        return this._r = r._r, this._g = r._g, this._b = r._b, this.setAlpha(r._a), this
-                    },
-                    lighten: function() {
-                        return this._applyModification(y, arguments)
-                    },
-                    brighten: function() {
-                        return this._applyModification(w, arguments)
-                    },
-                    darken: function() {
-                        return this._applyModification(E, arguments)
-                    },
-                    desaturate: function() {
-                        return this._applyModification(x, arguments)
-                    },
-                    saturate: function() {
-                        return this._applyModification(m, arguments)
-                    },
-                    greyscale: function() {
-                        return this._applyModification(v, arguments)
-                    },
-                    spin: function() {
-                        return this._applyModification(C, arguments)
-                    },
-                    _applyCombination: function(e, t) {
-                        return e.apply(null, [this].concat([].slice.call(t)))
-                    },
-                    analogous: function() {
-                        return this._applyCombination(R, arguments)
-                    },
-                    complement: function() {
-                        return this._applyCombination(k, arguments)
-                    },
-                    monochromatic: function() {
-                        return this._applyCombination(A, arguments)
-                    },
-                    splitcomplement: function() {
-                        return this._applyCombination(B, arguments)
-                    },
-                    triad: function() {
-                        return this._applyCombination(F, arguments)
-                    },
-                    tetrad: function() {
-                        return this._applyCombination(S, arguments)
-                    }
-                }, d.fromRatio = function(e, t) {
-                    if ("object" == typeof e) {
-                        var r = {};
-                        for (var n in e) e.hasOwnProperty(n) && (r[n] = "a" === n ? e[n] : z(e[n]));
-                        e = r
-                    }
-                    return d(e, t)
-                }, d.equals = function(e, t) {
-                    return !(!e || !t) && d(e).toRgbString() == d(t).toRgbString()
-                }, d.random = function() {
-                    return d.fromRatio({
-                        r: c(),
-                        g: c(),
-                        b: c()
-                    })
-                }, d.mix = function(e, t, r) {
-                    r = 0 === r ? 0 : r || 50;
-                    var n = d(e).toRgb(),
-                        a = d(t).toRgb(),
-                        i = r / 100;
-                    return d({
-                        r: (a.r - n.r) * i + n.r,
-                        g: (a.g - n.g) * i + n.g,
-                        b: (a.b - n.b) * i + n.b,
-                        a: (a.a - n.a) * i + n.a
-                    })
-                }, d.readability = function(e, t) {
-                    var r = d(e),
-                        n = d(t);
-                    return (a.max(r.getLuminance(), n.getLuminance()) + .05) / (a.min(r.getLuminance(), n.getLuminance()) + .05)
-                }, d.isReadable = function(e, t, r) {
-                    var n, a, i, o, l, s = d.readability(e, t);
-                    switch (a = !1, (i = r, "AA" !== (o = ((i = i || {
-                            level: "AA",
-                            size: "small"
-                        }).level || "AA").toUpperCase()) && "AAA" !== o && (o = "AA"), "small" !== (l = (i.size || "small").toLowerCase()) && "large" !== l && (l = "small"), n = {
-                            level: o,
-                            size: l
-                        }).level + n.size) {
-                        case "AAsmall":
-                        case "AAAlarge":
-                            a = s >= 4.5;
-                            break;
-                        case "AAlarge":
-                            a = s >= 3;
-                            break;
-                        case "AAAsmall":
-                            a = s >= 7
-                    }
-                    return a
-                }, d.mostReadable = function(e, t, r) {
-                    var n, a, i, o, l = null,
-                        s = 0;
-                    a = (r = r || {}).includeFallbackColors, i = r.level, o = r.size;
-                    for (var p = 0; p < t.length; p++)(n = d.readability(e, t[p])) > s && (s = n, l = d(t[p]));
-                    return d.isReadable(e, l, {
-                        level: i,
-                        size: o
-                    }) || !a ? l : (r.includeFallbackColors = !1, d.mostReadable(e, ["#fff", "#000"], r))
-                };
-                var _ = d.names = {
-                        aliceblue: "f0f8ff",
-                        antiquewhite: "faebd7",
-                        aqua: "0ff",
-                        aquamarine: "7fffd4",
-                        azure: "f0ffff",
-                        beige: "f5f5dc",
-                        bisque: "ffe4c4",
-                        black: "000",
-                        blanchedalmond: "ffebcd",
-                        blue: "00f",
-                        blueviolet: "8a2be2",
-                        brown: "a52a2a",
-                        burlywood: "deb887",
-                        burntsienna: "ea7e5d",
-                        cadetblue: "5f9ea0",
-                        chartreuse: "7fff00",
-                        chocolate: "d2691e",
-                        coral: "ff7f50",
-                        cornflowerblue: "6495ed",
-                        cornsilk: "fff8dc",
-                        crimson: "dc143c",
-                        cyan: "0ff",
-                        darkblue: "00008b",
-                        darkcyan: "008b8b",
-                        darkgoldenrod: "b8860b",
-                        darkgray: "a9a9a9",
-                        darkgreen: "006400",
-                        darkgrey: "a9a9a9",
-                        darkkhaki: "bdb76b",
-                        darkmagenta: "8b008b",
-                        darkolivegreen: "556b2f",
-                        darkorange: "ff8c00",
-                        darkorchid: "9932cc",
-                        darkred: "8b0000",
-                        darksalmon: "e9967a",
-                        darkseagreen: "8fbc8f",
-                        darkslateblue: "483d8b",
-                        darkslategray: "2f4f4f",
-                        darkslategrey: "2f4f4f",
-                        darkturquoise: "00ced1",
-                        darkviolet: "9400d3",
-                        deeppink: "ff1493",
-                        deepskyblue: "00bfff",
-                        dimgray: "696969",
-                        dimgrey: "696969",
-                        dodgerblue: "1e90ff",
-                        firebrick: "b22222",
-                        floralwhite: "fffaf0",
-                        forestgreen: "228b22",
-                        fuchsia: "f0f",
-                        gainsboro: "dcdcdc",
-                        ghostwhite: "f8f8ff",
-                        gold: "ffd700",
-                        goldenrod: "daa520",
-                        gray: "808080",
-                        green: "008000",
-                        greenyellow: "adff2f",
-                        grey: "808080",
-                        honeydew: "f0fff0",
-                        hotpink: "ff69b4",
-                        indianred: "cd5c5c",
-                        indigo: "4b0082",
-                        ivory: "fffff0",
-                        khaki: "f0e68c",
-                        lavender: "e6e6fa",
-                        lavenderblush: "fff0f5",
-                        lawngreen: "7cfc00",
-                        lemonchiffon: "fffacd",
-                        lightblue: "add8e6",
-                        lightcoral: "f08080",
-                        lightcyan: "e0ffff",
-                        lightgoldenrodyellow: "fafad2",
-                        lightgray: "d3d3d3",
-                        lightgreen: "90ee90",
-                        lightgrey: "d3d3d3",
-                        lightpink: "ffb6c1",
-                        lightsalmon: "ffa07a",
-                        lightseagreen: "20b2aa",
-                        lightskyblue: "87cefa",
-                        lightslategray: "789",
-                        lightslategrey: "789",
-                        lightsteelblue: "b0c4de",
-                        lightyellow: "ffffe0",
-                        lime: "0f0",
-                        limegreen: "32cd32",
-                        linen: "faf0e6",
-                        magenta: "f0f",
-                        maroon: "800000",
-                        mediumaquamarine: "66cdaa",
-                        mediumblue: "0000cd",
-                        mediumorchid: "ba55d3",
-                        mediumpurple: "9370db",
-                        mediumseagreen: "3cb371",
-                        mediumslateblue: "7b68ee",
-                        mediumspringgreen: "00fa9a",
-                        mediumturquoise: "48d1cc",
-                        mediumvioletred: "c71585",
-                        midnightblue: "191970",
-                        mintcream: "f5fffa",
-                        mistyrose: "ffe4e1",
-                        moccasin: "ffe4b5",
-                        navajowhite: "ffdead",
-                        navy: "000080",
-                        oldlace: "fdf5e6",
-                        olive: "808000",
-                        olivedrab: "6b8e23",
-                        orange: "ffa500",
-                        orangered: "ff4500",
-                        orchid: "da70d6",
-                        palegoldenrod: "eee8aa",
-                        palegreen: "98fb98",
-                        paleturquoise: "afeeee",
-                        palevioletred: "db7093",
-                        papayawhip: "ffefd5",
-                        peachpuff: "ffdab9",
-                        peru: "cd853f",
-                        pink: "ffc0cb",
-                        plum: "dda0dd",
-                        powderblue: "b0e0e6",
-                        purple: "800080",
-                        rebeccapurple: "663399",
-                        red: "f00",
-                        rosybrown: "bc8f8f",
-                        royalblue: "4169e1",
-                        saddlebrown: "8b4513",
-                        salmon: "fa8072",
-                        sandybrown: "f4a460",
-                        seagreen: "2e8b57",
-                        seashell: "fff5ee",
-                        sienna: "a0522d",
-                        silver: "c0c0c0",
-                        skyblue: "87ceeb",
-                        slateblue: "6a5acd",
-                        slategray: "708090",
-                        slategrey: "708090",
-                        snow: "fffafa",
-                        springgreen: "00ff7f",
-                        steelblue: "4682b4",
-                        tan: "d2b48c",
-                        teal: "008080",
-                        thistle: "d8bfd8",
-                        tomato: "ff6347",
-                        turquoise: "40e0d0",
-                        violet: "ee82ee",
-                        wheat: "f5deb3",
-                        white: "fff",
-                        whitesmoke: "f5f5f5",
-                        yellow: "ff0",
-                        yellowgreen: "9acd32"
-                    },
-                    D = d.hexNames = function(e) {
-                        var t = {};
-                        for (var r in e) e.hasOwnProperty(r) && (t[e[r]] = r);
-                        return t
-                    }(_);
-
-                function M(e) {
-                    return e = parseFloat(e), (isNaN(e) || e < 0 || e > 1) && (e = 1), e
-                }
-
-                function N(e, t) {
-                    (function(e) {
-                        return "string" == typeof e && -1 != e.indexOf(".") && 1 === parseFloat(e)
-                    })(e) && (e = "100%");
-                    var r = function(e) {
-                        return "string" == typeof e && -1 != e.indexOf("%")
-                    }(e);
-                    return e = p(t, h(0, parseFloat(e))), r && (e = parseInt(e * t, 10) / 100), a.abs(e - t) < 1e-6 ? 1 : e % t / parseFloat(t)
-                }
-
-                function $(e) {
-                    return p(1, h(0, e))
-                }
-
-                function H(e) {
-                    return parseInt(e, 16)
-                }
-
-                function L(e) {
-                    return 1 == e.length ? "0" + e : "" + e
-                }
-
-                function z(e) {
-                    return e <= 1 && (e = 100 * e + "%"), e
-                }
-
-                function T(e) {
-                    return a.round(255 * parseFloat(e)).toString(16)
-                }
-
-                function G(e) {
-                    return H(e) / 255
-                }
-                var O, P, X, U = (P = "[\\s|\\(]+(" + (O = "(?:[-\\+]?\\d*\\.\\d+%?)|(?:[-\\+]?\\d+%?)") + ")[,|\\s]+(" + O + ")[,|\\s]+(" + O + ")\\s*\\)?", X = "[\\s|\\(]+(" + O + ")[,|\\s]+(" + O + ")[,|\\s]+(" + O + ")[,|\\s]+(" + O + ")\\s*\\)?", {
-                    CSS_UNIT: new RegExp(O),
-                    rgb: new RegExp("rgb" + P),
-                    rgba: new RegExp("rgba" + X),
-                    hsl: new RegExp("hsl" + P),
-                    hsla: new RegExp("hsla" + X),
-                    hsv: new RegExp("hsv" + P),
-                    hsva: new RegExp("hsva" + X),
-                    hex3: /^#?([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})$/,
-                    hex6: /^#?([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})$/,
-                    hex4: /^#?([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})$/,
-                    hex8: /^#?([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})$/
-                });
-
-                function I(e) {
-                    return !!U.CSS_UNIT.exec(e)
-                }
-                e.exports ? e.exports = d : void 0 === (n = function() {
-                    return d
-                }.call(t, r, t, e)) || (e.exports = n)
-            }(Math)
         }
     }
 ]);
```

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/807.68bd5c7d28866c568e00.js` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/807.deac369ec79332e05c33.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
-/*! For license information please see 807.68bd5c7d28866c568e00.js.LICENSE.txt */
+/*! For license information please see 807.deac369ec79332e05c33.js.LICENSE.txt */
 (self.webpackChunkjupyter_theme_editor = self.webpackChunkjupyter_theme_editor || []).push([
     [807], {
-        6084: (e, r, t) => {
+        3807: (e, r, t) => {
             "use strict";
             t.r(r), t.d(r, {
-                default: () => Ha,
-                utils: () => Qa,
-                withTheme: () => Wa
+                default: () => Ja,
+                utils: () => Ka,
+                withTheme: () => Ha
             });
-            var a = t(6271),
+            var a = t(6029),
                 o = t.n(a),
                 n = t(5697),
                 i = t.n(n);
             const s = Array.isArray;
             var u = t(6169);
             const l = u.Z.Symbol;
             var c = Object.prototype,
@@ -63,18 +63,18 @@
                     try {
                         return e + ""
                     } catch (e) {}
                 }
                 return ""
             };
             var F = /^\[object .+?Constructor\]$/,
-                D = Function.prototype,
-                A = Object.prototype,
-                C = D.toString,
-                k = A.hasOwnProperty,
+                A = Function.prototype,
+                D = Object.prototype,
+                C = A.toString,
+                k = D.hasOwnProperty,
                 $ = RegExp("^" + C.call(k).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
             const R = function(e) {
                     return !(!P(e) || (r = e, O && O in r)) && (w(e) ? $ : F).test(_(e));
                     var r
                 },
                 I = function(e, r) {
                     var t = function(e, r) {
@@ -82,42 +82,42 @@
                     }(e, r);
                     return R(t) ? t : void 0
                 },
                 N = I(Object, "create");
             var T = Object.prototype.hasOwnProperty;
             var q = Object.prototype.hasOwnProperty;
 
-            function L(e) {
+            function U(e) {
                 var r = -1,
                     t = null == e ? 0 : e.length;
                 for (this.clear(); ++r < t;) {
                     var a = e[r];
                     this.set(a[0], a[1])
                 }
             }
-            L.prototype.clear = function() {
+            U.prototype.clear = function() {
                 this.__data__ = N ? N(null) : {}, this.size = 0
-            }, L.prototype.delete = function(e) {
+            }, U.prototype.delete = function(e) {
                 var r = this.has(e) && delete this.__data__[e];
                 return this.size -= r ? 1 : 0, r
-            }, L.prototype.get = function(e) {
+            }, U.prototype.get = function(e) {
                 var r = this.__data__;
                 if (N) {
                     var t = r[e];
                     return "__lodash_hash_undefined__" === t ? void 0 : t
                 }
                 return T.call(r, e) ? r[e] : void 0
-            }, L.prototype.has = function(e) {
+            }, U.prototype.has = function(e) {
                 var r = this.__data__;
                 return N ? void 0 !== r[e] : q.call(r, e)
-            }, L.prototype.set = function(e, r) {
+            }, U.prototype.set = function(e, r) {
                 var t = this.__data__;
                 return this.size += this.has(e) ? 0 : 1, t[e] = N && void 0 === r ? "__lodash_hash_undefined__" : r, this
             };
-            const U = L,
+            const L = U,
                 M = function(e, r) {
                     return e === r || e != e && r != r
                 },
                 V = function(e, r) {
                     for (var t = e.length; t--;)
                         if (M(e[t][0], r)) return t;
                     return -1
@@ -162,17 +162,17 @@
                 for (this.clear(); ++r < t;) {
                     var a = e[r];
                     this.set(a[0], a[1])
                 }
             }
             K.prototype.clear = function() {
                 this.size = 0, this.__data__ = {
-                    hash: new U,
+                    hash: new L,
                     map: new(Q || W),
-                    string: new U
+                    string: new L
                 }
             }, K.prototype.delete = function(e) {
                 var r = H(this, e).delete(e);
                 return this.size -= r ? 1 : 0, r
             }, K.prototype.get = function(e) {
                 return H(this, e).get(e)
             }, K.prototype.has = function(e) {
@@ -329,240 +329,241 @@
                         s = r.length;
                     for (a || (a = _e), n || (n = []); ++i < s;) {
                         var u = r[i];
                         t > 0 && a(u) ? t > 1 ? e(u, t - 1, a, o, n) : Oe(n, u) : o || (n[n.length] = u)
                     }
                     return n
                 },
-                De = function(e) {
+                Ae = function(e) {
                     return null != e && e.length ? Fe(e, 1) : []
-                },
-                Ae = function(e, r, t) {
-                    switch (t.length) {
-                        case 0:
-                            return e.call(r);
-                        case 1:
-                            return e.call(r, t[0]);
-                        case 2:
-                            return e.call(r, t[0], t[1]);
-                        case 3:
-                            return e.call(r, t[0], t[1], t[2])
-                    }
-                    return e.apply(r, t)
                 };
-            var Ce = Math.max;
-            const ke = function(e, r, t) {
-                    return r = Ce(void 0 === r ? e.length - 1 : r, 0),
+            var De = Math.max;
+            const Ce = function(e, r, t) {
+                    return r = De(void 0 === r ? e.length - 1 : r, 0),
                         function() {
-                            for (var a = arguments, o = -1, n = Ce(a.length - r, 0), i = Array(n); ++o < n;) i[o] = a[r + o];
+                            for (var a = arguments, o = -1, n = De(a.length - r, 0), i = Array(n); ++o < n;) i[o] = a[r + o];
                             o = -1;
                             for (var s = Array(r + 1); ++o < r;) s[o] = a[o];
-                            return s[r] = t(i), Ae(e, this, s)
+                            return s[r] = t(i),
+                                function(e, r, t) {
+                                    switch (t.length) {
+                                        case 0:
+                                            return e.call(r);
+                                        case 1:
+                                            return e.call(r, t[0]);
+                                        case 2:
+                                            return e.call(r, t[0], t[1]);
+                                        case 3:
+                                            return e.call(r, t[0], t[1], t[2])
+                                    }
+                                    return e.apply(r, t)
+                                }(e, this, s)
                         }
                 },
-                $e = function(e) {
+                ke = function(e) {
                     return e
                 },
-                Re = ce ? function(e, r) {
+                $e = ce ? function(e, r) {
                     return ce(e, "toString", {
                         configurable: !0,
                         enumerable: !1,
                         value: (t = r, function() {
                             return t
                         }),
                         writable: !0
                     });
                     var t
-                } : $e;
-            var Ie = Date.now;
-            const Ne = (Te = Re, qe = 0, Le = 0, function() {
-                var e = Ie(),
-                    r = 16 - (e - Le);
-                if (Le = e, r > 0) {
-                    if (++qe >= 800) return arguments[0]
-                } else qe = 0;
-                return Te.apply(void 0, arguments)
+                } : ke;
+            var Re = Date.now;
+            const Ie = (Ne = $e, Te = 0, qe = 0, function() {
+                var e = Re(),
+                    r = 16 - (e - qe);
+                if (qe = e, r > 0) {
+                    if (++Te >= 800) return arguments[0]
+                } else Te = 0;
+                return Ne.apply(void 0, arguments)
             });
-            var Te, qe, Le;
+            var Ne, Te, qe;
             const Ue = function(e) {
-                return Ne(ke(e, void 0, De), e + "")
+                return Ie(Ce(e, void 0, Ae), e + "")
             }((function(e, r) {
                 return null == e ? {} : xe(e, r)
             }));
-            var Me = Object.prototype;
-            const Ve = function(e) {
+            var Le = Object.prototype;
+            const Me = function(e) {
                     var r = e && e.constructor;
-                    return e === ("function" == typeof r && r.prototype || Me)
+                    return e === ("function" == typeof r && r.prototype || Le)
                 },
-                ze = function(e, r) {
+                Ve = function(e, r) {
                     return function(t) {
                         return e(r(t))
                     }
                 }(Object.keys, Object);
-            var Be = Object.prototype.hasOwnProperty;
-            const We = I(u.Z, "DataView"),
-                Qe = I(u.Z, "Promise"),
-                He = I(u.Z, "Set"),
-                Ke = I(u.Z, "WeakMap");
-            var Je = "[object Map]",
-                Ze = "[object Promise]",
-                Ye = "[object Set]",
-                Ge = "[object WeakMap]",
-                Xe = "[object DataView]",
-                er = _(We),
-                rr = _(Q),
+            var ze = Object.prototype.hasOwnProperty;
+            const Be = I(u.Z, "DataView"),
+                We = I(u.Z, "Promise"),
+                Qe = I(u.Z, "Set"),
+                He = I(u.Z, "WeakMap");
+            var Ke = "[object Map]",
+                Je = "[object Promise]",
+                Ze = "[object Set]",
+                Ye = "[object WeakMap]",
+                Ge = "[object DataView]",
+                Xe = _(Be),
+                er = _(Q),
+                rr = _(We),
                 tr = _(Qe),
                 ar = _(He),
-                or = _(Ke),
-                nr = v;
-            (We && nr(new We(new ArrayBuffer(1))) != Xe || Q && nr(new Q) != Je || Qe && nr(Qe.resolve()) != Ze || He && nr(new He) != Ye || Ke && nr(new Ke) != Ge) && (nr = function(e) {
+                or = v;
+            (Be && or(new Be(new ArrayBuffer(1))) != Ge || Q && or(new Q) != Ke || We && or(We.resolve()) != Je || Qe && or(new Qe) != Ze || He && or(new He) != Ye) && (or = function(e) {
                 var r = v(e),
                     t = "[object Object]" == r ? e.constructor : void 0,
                     a = t ? _(t) : "";
                 if (a) switch (a) {
+                    case Xe:
+                        return Ge;
                     case er:
-                        return Xe;
+                        return Ke;
                     case rr:
                         return Je;
                     case tr:
                         return Ze;
                     case ar:
-                        return Ye;
-                    case or:
-                        return Ge
+                        return Ye
                 }
                 return r
             });
-            const ir = nr,
-                sr = function(e) {
+            const nr = or,
+                ir = function(e) {
                     return null != e && we(e.length) && !w(e)
                 };
-            var ur = t(4002),
-                lr = {};
-            lr["[object Float32Array]"] = lr["[object Float64Array]"] = lr["[object Int8Array]"] = lr["[object Int16Array]"] = lr["[object Int32Array]"] = lr["[object Uint8Array]"] = lr["[object Uint8ClampedArray]"] = lr["[object Uint16Array]"] = lr["[object Uint32Array]"] = !0, lr["[object Arguments]"] = lr["[object Array]"] = lr["[object ArrayBuffer]"] = lr["[object Boolean]"] = lr["[object DataView]"] = lr["[object Date]"] = lr["[object Error]"] = lr["[object Function]"] = lr["[object Map]"] = lr["[object Number]"] = lr["[object Object]"] = lr["[object RegExp]"] = lr["[object Set]"] = lr["[object String]"] = lr["[object WeakMap]"] = !1;
-            var cr = t(5218),
-                dr = cr.Z && cr.Z.isTypedArray;
-            const fr = dr ? function(e) {
+            var sr = t(4002),
+                ur = {};
+            ur["[object Float32Array]"] = ur["[object Float64Array]"] = ur["[object Int8Array]"] = ur["[object Int16Array]"] = ur["[object Int32Array]"] = ur["[object Uint8Array]"] = ur["[object Uint8ClampedArray]"] = ur["[object Uint16Array]"] = ur["[object Uint32Array]"] = !0, ur["[object Arguments]"] = ur["[object Array]"] = ur["[object ArrayBuffer]"] = ur["[object Boolean]"] = ur["[object DataView]"] = ur["[object Date]"] = ur["[object Error]"] = ur["[object Function]"] = ur["[object Map]"] = ur["[object Number]"] = ur["[object Object]"] = ur["[object RegExp]"] = ur["[object Set]"] = ur["[object String]"] = ur["[object WeakMap]"] = !1;
+            var lr = t(5218),
+                cr = lr.Z && lr.Z.isTypedArray;
+            const dr = cr ? function(e) {
                 return function(r) {
                     return e(r)
                 }
-            }(dr) : function(e) {
-                return y(e) && we(e.length) && !!lr[v(e)]
+            }(cr) : function(e) {
+                return y(e) && we(e.length) && !!ur[v(e)]
             };
-            var pr = Object.prototype.hasOwnProperty;
-            const hr = function(e) {
+            var fr = Object.prototype.hasOwnProperty;
+            const pr = function(e) {
                 if (null == e) return !0;
-                if (sr(e) && (s(e) || "string" == typeof e || "function" == typeof e.splice || (0, ur.Z)(e) || fr(e) || Pe(e))) return !e.length;
-                var r = ir(e);
+                if (ir(e) && (s(e) || "string" == typeof e || "function" == typeof e.splice || (0, sr.Z)(e) || dr(e) || Pe(e))) return !e.length;
+                var r = nr(e);
                 if ("[object Map]" == r || "[object Set]" == r) return !e.size;
-                if (Ve(e)) return ! function(e) {
-                    if (!Ve(e)) return ze(e);
+                if (Me(e)) return ! function(e) {
+                    if (!Me(e)) return Ve(e);
                     var r = [];
-                    for (var t in Object(e)) Be.call(e, t) && "constructor" != t && r.push(t);
+                    for (var t in Object(e)) ze.call(e, t) && "constructor" != t && r.push(t);
                     return r
                 }(e).length;
                 for (var t in e)
-                    if (pr.call(e, t)) return !1;
+                    if (fr.call(e, t)) return !1;
                 return !0
             };
-            var mr = t(2415),
-                vr = t.n(mr),
-                yr = t(9864),
-                gr = t(9830),
-                br = t.n(gr),
-                Er = t(9554),
-                Pr = t.n(Er);
+            var hr = t(2415),
+                mr = t.n(hr),
+                vr = t(3434),
+                yr = t(4965),
+                gr = t.n(yr),
+                br = t(9554),
+                Er = t.n(br);
 
-            function wr(e) {
+            function Pr(e) {
                 var r = -1,
                     t = null == e ? 0 : e.length;
                 for (this.__data__ = new J; ++r < t;) this.add(e[r])
             }
-            wr.prototype.add = wr.prototype.push = function(e) {
+            Pr.prototype.add = Pr.prototype.push = function(e) {
                 return this.__data__.set(e, "__lodash_hash_undefined__"), this
-            }, wr.prototype.has = function(e) {
+            }, Pr.prototype.has = function(e) {
                 return this.__data__.has(e)
             };
-            const Sr = wr,
-                xr = function(e) {
+            const wr = Pr,
+                Sr = function(e) {
                     return e != e
                 },
-                Or = function(e, r) {
+                xr = function(e, r) {
                     return !(null == e || !e.length) && function(e, r, t) {
                         return r == r ? function(e, r, t) {
                             for (var a = t - 1, o = e.length; ++a < o;)
                                 if (e[a] === r) return a;
                             return -1
                         }(e, r, t) : function(e, r, t, a) {
                             for (var o = e.length, n = t + (a ? 1 : -1); a ? n-- : ++n < o;)
                                 if (r(e[n], n, e)) return n;
                             return -1
-                        }(e, xr, t)
+                        }(e, Sr, t)
                     }(e, r, 0) > -1
                 },
-                jr = function(e, r, t) {
+                Or = function(e, r, t) {
                     for (var a = -1, o = null == e ? 0 : e.length; ++a < o;)
                         if (t(r, e[a])) return !0;
                     return !1
                 },
-                _r = function(e, r) {
+                jr = function(e, r) {
                     return e.has(r)
                 },
-                Fr = function(e) {
+                _r = function(e) {
                     var r = -1,
                         t = Array(e.size);
                     return e.forEach((function(e) {
                         t[++r] = e
                     })), t
                 },
-                Dr = He && 1 / Fr(new He([, -0]))[1] == 1 / 0 ? function(e) {
-                    return new He(e)
+                Fr = Qe && 1 / _r(new Qe([, -0]))[1] == 1 / 0 ? function(e) {
+                    return new Qe(e)
                 } : function() {},
                 Ar = function(e) {
-                    return y(e) && sr(e)
+                    return y(e) && ir(e)
                 },
-                Cr = function(e, r) {
-                    return Ne(ke(e, r, $e), e + "")
+                Dr = function(e, r) {
+                    return Ie(Ce(e, r, ke), e + "")
                 }((function(e) {
                     return function(e, r, t) {
                         var a = -1,
-                            o = Or,
+                            o = xr,
                             n = e.length,
                             i = !0,
                             s = [],
                             u = s;
-                        if (t) i = !1, o = jr;
+                        if (t) i = !1, o = Or;
                         else if (n >= 200) {
-                            var l = r ? null : Dr(e);
-                            if (l) return Fr(l);
-                            i = !1, o = _r, u = new Sr
+                            var l = r ? null : Fr(e);
+                            if (l) return _r(l);
+                            i = !1, o = jr, u = new wr
                         } else u = r ? [] : s;
                         e: for (; ++a < n;) {
                             var c = e[a],
                                 d = r ? r(c) : c;
                             if (c = t || 0 !== c ? c : 0, i && d == d) {
                                 for (var f = u.length; f--;)
                                     if (u[f] === d) continue e;
                                 r && u.push(d), s.push(c)
                             } else o(u, d, t) || (u !== s && u.push(d), s.push(c))
                         }
                         return s
                     }(Fe(e, 1, Ar, !0))
                 }));
-            var kr = t(9038);
-            const $r = function(e) {
+            var Cr = t(9038);
+            const kr = function(e) {
                 return s(e) ? te(e, ue) : g(e) ? [e] : function(e, r) {
                     var t = -1,
                         a = e.length;
                     for (r || (r = Array(a)); ++t < a;) r[t] = e[t];
                     return r
                 }(X(ie(e)))
             };
-            var Rr = t(5096),
-                Ir = t.n(Rr);
+            var $r = t(233),
+                Rr = t.n($r);
+            let Ir = (e = 21) => crypto.getRandomValues(new Uint8Array(e)).reduce(((e, r) => e + ((r &= 63) < 36 ? r.toString(36) : r < 62 ? (r - 26).toString(36).toUpperCase() : r > 62 ? "-" : "_")), "");
 
             function Nr(e, r) {
                 for (var t = 0; t < r.length; t++) {
                     var a = r[t];
                     a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
                 }
             }
@@ -579,22 +580,22 @@
                         var t = arguments[r];
                         for (var a in t) Object.prototype.hasOwnProperty.call(t, a) && (e[a] = t[a])
                     }
                     return e
                 }, qr.apply(this, arguments)
             }
 
-            function Lr(e, r) {
-                e.prototype = Object.create(r.prototype), e.prototype.constructor = e, Ur(e, r)
+            function Ur(e, r) {
+                e.prototype = Object.create(r.prototype), e.prototype.constructor = e, Lr(e, r)
             }
 
-            function Ur(e, r) {
-                return Ur = Object.setPrototypeOf || function(e, r) {
+            function Lr(e, r) {
+                return Lr = Object.setPrototypeOf || function(e, r) {
                     return e.__proto__ = r, e
-                }, Ur(e, r)
+                }, Lr(e, r)
             }
 
             function Mr(e, r) {
                 if (null == e) return {};
                 var t, a, o = {},
                     n = Object.keys(e);
                 for (a = 0; a < n.length; a++) t = n[a], r.indexOf(t) >= 0 || (o[t] = e[t]);
@@ -659,15 +660,15 @@
                 }),
                 Qr = (i().bool, i().bool, i().object, i().any, i().object, i().func, i().func.isRequired, i().func, i().string, i().bool, Wr.isRequired, i().bool, i().object.isRequired, i().bool, i().bool, i().bool, Zr()),
                 Hr = null,
                 Kr = null,
                 Jr = "__rjsf_rootSchema";
 
             function Zr() {
-                var e = new(Ir())({
+                var e = new(Rr())({
                     errorDataPath: "property",
                     allErrors: !0,
                     multipleOfPrecision: 8,
                     schemaId: "auto",
                     unknownFormats: "ignore"
                 });
                 return e.addFormat("data-url", /^data:([a-z]+\/[a-z0-9-+.]+)?;(?:name=(.*);)?base64,(.*)$/), e.addFormat("color", /^(#?([0-9A-Fa-f]{3}){1,2}\b|aqua|black|blue|fuchsia|gray|green|lime|maroon|navy|olive|orange|purple|red|silver|teal|white|yellow|(rgb\(\s*\b([0-9]|[1-9][0-9]|1[0-9][0-9]|2[0-4][0-9]|25[0-5])\b\s*,\s*\b([0-9]|[1-9][0-9]|1[0-9][0-9]|2[0-4][0-9]|25[0-5])\b\s*,\s*\b([0-9]|[1-9][0-9]|1[0-9][0-9]|2[0-4][0-9]|25[0-5])\b\s*\))|(rgb\(\s*(\d?\d%|100%)+\s*,\s*(\d?\d%|100%)+\s*,\s*(\d?\d%|100%)+\s*\)))$/), e
@@ -744,15 +745,15 @@
                 c && (l = [].concat(l, [{
                     stack: u.message
                 }])), "function" == typeof a && (l = a(l));
                 var d = function(e) {
                     return e.length ? e.reduce((function(e, r) {
                         var t = r.property,
                             a = r.message,
-                            o = $r(t),
+                            o = kr(t),
                             n = e;
                         o.length > 0 && "" === o[0] && o.splice(0, 1);
                         var i = o.slice(0),
                             s = Array.isArray(i),
                             u = 0;
                         for (i = s ? i : i[Symbol.iterator]();;) {
                             var l;
@@ -862,23 +863,23 @@
                 if (!e.additionalProperties) return !1;
                 var a = ft(r).expandable;
                 return !1 === a ? a : void 0 === e.maxProperties || Object.keys(t).length < e.maxProperties
             }
 
             function it(e) {
                 var r = e.type;
-                return !r && e.const ? Dt(e.const) : !r && e.enum ? "string" : r || !e.properties && !e.additionalProperties ? r instanceof Array && 2 === r.length && r.includes("null") ? r.find((function(e) {
+                return !r && e.const ? At(e.const) : !r && e.enum ? "string" : r || !e.properties && !e.additionalProperties ? r instanceof Array && 2 === r.length && r.includes("null") ? r.find((function(e) {
                     return "null" !== e
                 })) : r : "object"
             }
 
             function st(e, r, t) {
                 void 0 === t && (t = {});
                 var a = it(e);
-                if ("function" == typeof r || (0, yr.isForwardRef)(o().createElement(r)) || (0, yr.isMemo)(r)) return function(e) {
+                if ("function" == typeof r || (0, vr.isForwardRef)(o().createElement(r)) || (0, vr.isMemo)(r)) return function(e) {
                     if (!e.MergedWidget) {
                         var r = e.defaultProps && e.defaultProps.options || {};
                         e.MergedWidget = function(t) {
                             var a = t.options,
                                 n = void 0 === a ? {} : a,
                                 i = Mr(t, ["options"]);
                             return o().createElement(e, qr({
@@ -910,18 +911,18 @@
                 var n = mt(e) ? e : {},
                     i = mt(a) ? a : {},
                     s = r;
                 if (mt(s) && mt(n.default)) s = vt(s, n.default);
                 else if ("default" in n) s = n.default;
                 else {
                     if ("$ref" in n) return lt(Ft(n.$ref, t), s, t, i, o);
-                    if ("dependencies" in n) return lt(Rt(n, t, i), s, t, i, o);
+                    if ("dependencies" in n) return lt(It(n, t, i), s, t, i, o);
                     xt(n) ? s = n.items.map((function(e, a) {
                         return lt(e, Array.isArray(r) ? r[a] : void 0, t, i, o)
-                    })) : "oneOf" in n ? n = n.oneOf[Zt(void 0, n.oneOf, t)] : "anyOf" in n && (n = n.anyOf[Zt(void 0, n.anyOf, t)])
+                    })) : "oneOf" in n ? n = n.oneOf[Yt(void 0, n.oneOf, t)] : "anyOf" in n && (n = n.anyOf[Yt(void 0, n.anyOf, t)])
                 }
                 switch (void 0 === s && (s = n.default), it(n)) {
                     case "object":
                         return Object.keys(n.properties || {}).reduce((function(e, r) {
                             var a = lt(n.properties[r], (s || {})[r], t, (i || {})[r], o);
                             return (o || void 0 !== a) && (e[r] = a), e
                         }), {});
@@ -932,25 +933,25 @@
                                 return lt(n.items, (s || {})[r], t, e)
                             }))), n.minItems) {
                             if (wt(n, t)) return s || [];
                             var u = s ? s.length : 0;
                             if (n.minItems > u) {
                                 var l = s || [],
                                     c = Array.isArray(n.items) ? n.additionalItems : n.items,
-                                    d = Pr()(new Array(n.minItems - u), lt(c, c.defaults, t));
+                                    d = Er()(new Array(n.minItems - u), lt(c, c.defaults, t));
                                 return l.concat(d)
                             }
                         }
                 }
                 return s
             }
 
             function ct(e, r, t, a) {
                 if (void 0 === t && (t = {}), void 0 === a && (a = !1), !mt(e)) throw new Error("Invalid schema: " + e);
-                var o = lt($t(e, t, r), e.default, t, r, a);
+                var o = lt(Rt(e, t, r), e.default, t, r, a);
                 return void 0 === r ? o : mt(r) || Array.isArray(r) ? dt(o, r) : 0 === r || !1 === r || "" === r ? r : r || o
             }
 
             function dt(e, r) {
                 if (Array.isArray(r)) return Array.isArray(e) || (e = []), r.map((function(r, t) {
                     return e[t] ? dt(e[t], r) : r
                 }));
@@ -1051,29 +1052,29 @@
                 if (Array.isArray(e.enum) && 1 === e.enum.length) return e.enum[0];
                 if (e.hasOwnProperty("const")) return e.const;
                 throw new Error("schema cannot be inferred as a constant")
             }
 
             function Pt(e, r) {
                 void 0 === r && (r = {});
-                var t = $t(e, r),
+                var t = Rt(e, r),
                     a = t.oneOf || t.anyOf;
                 return !!Array.isArray(t.enum) || !!Array.isArray(a) && a.every((function(e) {
                     return bt(e)
                 }))
             }
 
             function wt(e, r) {
                 return void 0 === r && (r = {}), !(!e.uniqueItems || !e.items) && Pt(e.items, r)
             }
 
             function St(e, r, t) {
                 if (void 0 === t && (t = {}), "files" === r["ui:widget"]) return !0;
                 if (e.items) {
-                    var a = $t(e.items, t);
+                    var a = Rt(e.items, t);
                     return "string" === a.type && "data-url" === a.format
                 }
                 return !1
             }
 
             function xt(e) {
                 return Array.isArray(e.items) && e.items.length > 0 && e.items.every((function(e) {
@@ -1106,107 +1107,108 @@
             }
 
             function Ft(e, r) {
                 void 0 === r && (r = {});
                 var t = e;
                 if (!e.startsWith("#")) throw new Error("Could not find a definition for " + t + ".");
                 e = decodeURIComponent(e.substring(1));
-                var a = kr.get(r, e);
+                var a = Cr.get(r, e);
                 if (void 0 === a) throw new Error("Could not find a definition for " + t + ".");
                 return a.hasOwnProperty("$ref") ? Ft(a.$ref, r) : a
             }
-            var Dt = function(e) {
+            var At = function(e) {
                 return Array.isArray(e) ? "array" : "string" == typeof e ? "string" : null == e ? "null" : "boolean" == typeof e ? "boolean" : isNaN(e) ? "object" == typeof e ? "object" : "string" : "number"
             };
 
-            function At(e, r, t) {
+            function Dt(e, r, t) {
                 return void 0 === r && (r = {}), void 0 === t && (t = {}), e = qr({}, e, {
                     properties: qr({}, e.properties)
                 }), t = mt(t) ? t : {}, Object.keys(t).forEach((function(a) {
                     var o;
-                    e.properties.hasOwnProperty(a) || (o = e.additionalProperties.hasOwnProperty("$ref") ? $t({
+                    e.properties.hasOwnProperty(a) || (o = e.additionalProperties.hasOwnProperty("$ref") ? Rt({
                         $ref: e.additionalProperties.$ref
                     }, r, t) : e.additionalProperties.hasOwnProperty("type") ? qr({}, e.additionalProperties) : {
-                        type: Dt(t[a])
+                        type: At(t[a])
                     }, e.properties[a] = o, e.properties[a][at] = !0)
                 })), e
             }
+            var Ct = function(e, r, t) {
+                var a = e.if,
+                    o = e.then,
+                    n = e.else,
+                    i = Mr(e, ["if", "then", "else"]),
+                    s = tt(a, t, r) ? o : n;
+                return Rt(s ? qt(i, Rt(s, r, t)) : i, r, t)
+            };
 
-            function Ct(e, r, t) {
-                return void 0 === r && (r = {}), void 0 === t && (t = {}), e.hasOwnProperty("$ref") ? kt(e, r, t) : e.hasOwnProperty("dependencies") ? $t(Rt(e, r, t), r, t) : e.hasOwnProperty("allOf") ? qr({}, e, {
+            function kt(e, r, t) {
+                return void 0 === r && (r = {}), void 0 === t && (t = {}), e.hasOwnProperty("$ref") ? $t(e, r, t) : e.hasOwnProperty("dependencies") ? Rt(It(e, r, t), r, t) : e.hasOwnProperty("allOf") ? qr({}, e, {
                     allOf: e.allOf.map((function(e) {
-                        return $t(e, r, t)
+                        return Rt(e, r, t)
                     }))
                 }) : e
             }
 
-            function kt(e, r, t) {
-                return $t(qr({}, Ft(e.$ref, r), Mr(e, ["$ref"])), r, t)
+            function $t(e, r, t) {
+                return Rt(qr({}, Ft(e.$ref, r), Mr(e, ["$ref"])), r, t)
             }
 
-            function $t(e, r, t) {
+            function Rt(e, r, t) {
                 if (void 0 === r && (r = {}), void 0 === t && (t = {}), !mt(e)) return {};
-                var a = Ct(e, r, t);
-                if (e.hasOwnProperty("if")) return function(e, r, t) {
-                    var a = e.if,
-                        o = e.then,
-                        n = e.else,
-                        i = Mr(e, ["if", "then", "else"]),
-                        s = tt(a, t, r) ? o : n;
-                    return $t(s ? Tt(i, $t(s, r, t)) : i, r, t)
-                }(e, r, t);
+                var a = kt(e, r, t);
+                if (e.hasOwnProperty("if")) return Ct(e, r, t);
                 if (a.properties) {
                     var o = {};
                     Object.entries(a.properties).forEach((function(e) {
                         var n = e[0],
                             i = e[1],
                             s = t && t[n],
                             u = mt(s) ? s : {},
-                            l = $t(i, r, u);
+                            l = Rt(i, r, u);
                         o[n] = l, i !== l && a.properties !== o && (a = qr({}, a, {
                             properties: o
                         }))
                     }))
                 }
                 if ("allOf" in e) try {
-                    a = br()(qr({}, a, {
+                    a = gr()(qr({}, a, {
                         allOf: a.allOf
                     }))
                 } catch (e) {
                     return console.warn("could not merge subschemas in allOf:\n" + e), Mr(a, ["allOf"])
                 }
-                return a.hasOwnProperty("additionalProperties") && !1 !== a.additionalProperties ? At(a, r, t) : a
+                return a.hasOwnProperty("additionalProperties") && !1 !== a.additionalProperties ? Dt(a, r, t) : a
             }
 
-            function Rt(e, r, t) {
+            function It(e, r, t) {
                 var a = e.dependencies,
                     o = void 0 === a ? {} : a,
                     n = Mr(e, ["dependencies"]);
-                return "oneOf" in n ? n = n.oneOf[Zt(t, n.oneOf, r)] : "anyOf" in n && (n = n.anyOf[Zt(t, n.anyOf, r)]), It(o, n, r, t)
+                return "oneOf" in n ? n = n.oneOf[Yt(t, n.oneOf, r)] : "anyOf" in n && (n = n.anyOf[Yt(t, n.anyOf, r)]), Nt(o, n, r, t)
             }
 
-            function It(e, r, t, a) {
+            function Nt(e, r, t, a) {
                 for (var o in e)
                     if (void 0 !== a[o] && (!r.properties || o in r.properties)) {
                         var n = e[o],
                             i = Mr(e, [o].map(Vr));
                         return Array.isArray(n) ? (s = r, r = (u = n) ? qr({}, s, {
                             required: Array.isArray(s.required) ? Array.from(new Set([].concat(s.required, u))) : u
-                        }) : s) : mt(n) && (r = Nt(r, t, a, o, n)), It(i, r, t, a)
+                        }) : s) : mt(n) && (r = Tt(r, t, a, o, n)), Nt(i, r, t, a)
                     } var s, u;
                 return r
             }
 
-            function Nt(e, r, t, a, o) {
-                var n = $t(o, r, t),
+            function Tt(e, r, t, a, o) {
+                var n = Rt(o, r, t),
                     i = n.oneOf;
-                if (e = Tt(e, Mr(n, ["oneOf"])), void 0 === i) return e;
+                if (e = qt(e, Mr(n, ["oneOf"])), void 0 === i) return e;
                 if (!Array.isArray(i)) throw new Error("invalid: it is some " + typeof i + " instead of an array");
                 var s = i.map((function(e) {
-                    return e.hasOwnProperty("$ref") ? kt(e, r, t) : e
+                    return e.hasOwnProperty("$ref") ? $t(e, r, t) : e
                 }));
                 return function(e, r, t, a, o) {
                     var n = o.filter((function(e) {
                         if (!e.properties) return !1;
                         var r = e.properties[a];
                         if (r) {
                             var o, n = {
@@ -1214,42 +1216,42 @@
                                 properties: (o = {}, o[a] = r, o)
                             };
                             return 0 === et(t, n).errors.length
                         }
                     }));
                     if (1 !== n.length) return console.warn("ignoring oneOf in dependencies because there isn't exactly one subschema that is valid"), e;
                     var i = n[0];
-                    return Tt(e, $t(qr({}, i, {
+                    return qt(e, Rt(qr({}, i, {
                         properties: Mr(i.properties, [a].map(Vr))
                     }), r, t))
                 }(e, r, t, a, s)
             }
 
-            function Tt(e, r) {
+            function qt(e, r) {
                 var t = Object.assign({}, e);
                 return Object.keys(r).reduce((function(t, a) {
                     var o = e ? e[a] : {},
                         n = r[a];
-                    return e && e.hasOwnProperty(a) && mt(n) ? t[a] = Tt(o, n) : e && r && ("object" === it(e) || "object" === it(r)) && "required" === a && Array.isArray(o) && Array.isArray(n) ? t[a] = Cr(o, n) : t[a] = n, t
+                    return e && e.hasOwnProperty(a) && mt(n) ? t[a] = qt(o, n) : e && r && ("object" === it(e) || "object" === it(r)) && "required" === a && Array.isArray(o) && Array.isArray(n) ? t[a] = Dr(o, n) : t[a] = n, t
                 }), t)
             }
 
-            function qt(e) {
+            function Ut(e) {
                 return "[object Arguments]" === Object.prototype.toString.call(e)
             }
 
             function Lt(e, r, t, a) {
                 if (void 0 === t && (t = []), void 0 === a && (a = []), e === r) return !0;
                 if ("function" == typeof e || "function" == typeof r) return !0;
                 if ("object" != typeof e || "object" != typeof r) return !1;
                 if (null === e || null === r) return !1;
                 if (e instanceof Date && r instanceof Date) return e.getTime() === r.getTime();
                 if (e instanceof RegExp && r instanceof RegExp) return e.source === r.source && e.global === r.global && e.multiline === r.multiline && e.lastIndex === r.lastIndex && e.ignoreCase === r.ignoreCase;
-                if (qt(e) || qt(r)) {
-                    if (!qt(e) || !qt(r)) return !1;
+                if (Ut(e) || Ut(r)) {
+                    if (!Ut(e) || !Ut(r)) return !1;
                     var o = Array.prototype.slice;
                     return Lt(o.call(e), o.call(r), t, a)
                 }
                 if (e.constructor !== r.constructor) return !1;
                 var n = Object.keys(e),
                     i = Object.keys(r);
                 if (0 === n.length && 0 === i.length) return !0;
@@ -1260,51 +1262,51 @@
                 for (var l = n.length - 1; l >= 0; l--)
                     if (n[l] !== i[l]) return !1;
                 for (var c = n.length - 1; c >= 0; c--)
                     if (!Lt(e[s = n[c]], r[s], t, a)) return !1;
                 return t.pop(), a.pop(), !0
             }
 
-            function Ut(e, r, t) {
+            function Mt(e, r, t) {
                 var a = e.props,
                     o = e.state;
                 return !Lt(a, r) || !Lt(o, t)
             }
 
-            function Mt(e, r, t, a, o, n) {
+            function Vt(e, r, t, a, o, n) {
                 void 0 === a && (a = {}), void 0 === o && (o = "root"), void 0 === n && (n = "_");
                 var i = {
                     $id: r || o
                 };
-                if ("$ref" in e || "dependencies" in e || "allOf" in e) return Mt($t(e, t, a), r, t, a, o, n);
-                if ("items" in e && !e.items.$ref) return Mt(e.items, r, t, a, o, n);
+                if ("$ref" in e || "dependencies" in e || "allOf" in e) return Vt(Rt(e, t, a), r, t, a, o, n);
+                if ("items" in e && !e.items.$ref) return Vt(e.items, r, t, a, o, n);
                 if ("object" !== e.type) return i;
                 for (var s in e.properties || {}) {
                     var u = e.properties[s],
                         l = i.$id + n + s;
-                    i[s] = Mt(mt(u) ? u : {}, l, t, (a || {})[s], o, n)
+                    i[s] = Vt(mt(u) ? u : {}, l, t, (a || {})[s], o, n)
                 }
                 return i
             }
 
-            function Vt(e, r, t, a) {
+            function zt(e, r, t, a) {
                 void 0 === r && (r = ""), void 0 === a && (a = {});
                 var o = {
                     $name: r.replace(/^\./, "")
                 };
-                if ("$ref" in e || "dependencies" in e || "allOf" in e) return Vt($t(e, t, a), r, t, a);
+                if ("$ref" in e || "dependencies" in e || "allOf" in e) return zt(Rt(e, t, a), r, t, a);
                 if (e.hasOwnProperty("additionalProperties") && (o.__rjsf_additionalProperties = !0), e.hasOwnProperty("items") && Array.isArray(a)) a.forEach((function(a, n) {
-                    o[n] = Vt(e.items, r + "." + n, t, a)
+                    o[n] = zt(e.items, r + "." + n, t, a)
                 }));
                 else if (e.hasOwnProperty("properties"))
-                    for (var n in e.properties) o[n] = Vt(e.properties[n], r + "." + n, t, (a || {})[n]);
+                    for (var n in e.properties) o[n] = zt(e.properties[n], r + "." + n, t, (a || {})[n]);
                 return o
             }
 
-            function zt(e, r) {
+            function Bt(e, r) {
                 if (void 0 === r && (r = !0), !e) return {
                     year: -1,
                     month: -1,
                     day: -1,
                     hour: r ? -1 : 0,
                     minute: r ? -1 : 0,
                     second: r ? -1 : 0
@@ -1317,15 +1319,15 @@
                     day: t.getUTCDate(),
                     hour: r ? t.getUTCHours() : 0,
                     minute: r ? t.getUTCMinutes() : 0,
                     second: r ? t.getUTCSeconds() : 0
                 }
             }
 
-            function Bt(e, r) {
+            function Wt(e, r) {
                 var t = e.year,
                     a = e.month,
                     o = e.day,
                     n = e.hour,
                     i = void 0 === n ? 0 : n,
                     s = e.minute,
                     u = void 0 === s ? 0 : s,
@@ -1333,30 +1335,30 @@
                     c = void 0 === l ? 0 : l;
                 void 0 === r && (r = !0);
                 var d = Date.UTC(t, a - 1, o, i, u, c),
                     f = new Date(d).toJSON();
                 return r ? f : f.slice(0, 10)
             }
 
-            function Wt(e) {
+            function Qt(e) {
                 if (!e) return "";
                 var r = new Date(e);
-                return Ht(r.getFullYear(), 4) + "-" + Ht(r.getMonth() + 1, 2) + "-" + Ht(r.getDate(), 2) + "T" + Ht(r.getHours(), 2) + ":" + Ht(r.getMinutes(), 2) + ":" + Ht(r.getSeconds(), 2) + "." + Ht(r.getMilliseconds(), 3)
+                return Kt(r.getFullYear(), 4) + "-" + Kt(r.getMonth() + 1, 2) + "-" + Kt(r.getDate(), 2) + "T" + Kt(r.getHours(), 2) + ":" + Kt(r.getMinutes(), 2) + ":" + Kt(r.getSeconds(), 2) + "." + Kt(r.getMilliseconds(), 3)
             }
 
-            function Qt(e) {
+            function Ht(e) {
                 if (e) return new Date(e).toJSON()
             }
 
-            function Ht(e, r) {
+            function Kt(e, r) {
                 for (var t = String(e); t.length < r;) t = "0" + t;
                 return t
             }
 
-            function Kt(e) {
+            function Jt(e) {
                 var r, t = e.split(","),
                     a = t[0].split(";"),
                     o = a[0].replace("data:", ""),
                     n = a.filter((function(e) {
                         return "name" === e.split("=")[0]
                     }));
                 r = 1 !== n.length ? "unknown" : n[0].split("=")[1];
@@ -1365,20 +1367,20 @@
                     blob: new window.Blob([new Uint8Array(s)], {
                         type: o
                     }),
                     name: r
                 }
             }
 
-            function Jt(e) {
+            function Zt(e) {
                 var r = {};
                 return e.multipleOf && (r.step = e.multipleOf), (e.minimum || 0 === e.minimum) && (r.min = e.minimum), (e.maximum || 0 === e.maximum) && (r.max = e.maximum), r
             }
 
-            function Zt(e, r, t) {
+            function Yt(e, r, t) {
                 if (void 0 === e) return 0;
                 for (var a = 0; a < r.length; a++) {
                     var o = r[a];
                     if (o.properties) {
                         var n = {
                                 anyOf: Object.keys(o.properties).map((function(e) {
                                     return {
@@ -1393,18 +1395,18 @@
                         } else i = Object.assign({}, o, n);
                         if (delete i.required, tt(i, e, t)) return a
                     } else if (tt(o, e, t)) return a
                 }
                 return 0
             }
 
-            function Yt(e) {
-                return !!e.const || !(!e.enum || 1 !== e.enum.length || !0 !== e.enum[0]) || (e.anyOf && 1 === e.anyOf.length ? Yt(e.anyOf[0]) : e.oneOf && 1 === e.oneOf.length ? Yt(e.oneOf[0]) : !!e.allOf && e.allOf.some(Yt))
+            function Gt(e) {
+                return !!e.const || !(!e.enum || 1 !== e.enum.length || !0 !== e.enum[0]) || (e.anyOf && 1 === e.anyOf.length ? Gt(e.anyOf[0]) : e.oneOf && 1 === e.oneOf.length ? Gt(e.oneOf[0]) : !!e.allOf && e.allOf.some(Gt))
             }
-            var Gt = {
+            var Xt = {
                 __proto__: null,
                 ADDITIONAL_PROPERTY_FLAG: at,
                 canExpand: nt,
                 getSchemaType: it,
                 getWidget: st,
                 hasWidget: ut,
                 getDefaultFormState: ct,
@@ -1422,61 +1424,61 @@
                 isMultiSelect: wt,
                 isFilesArray: St,
                 isFixedItems: xt,
                 isCustomWidget: Ot,
                 allowAdditionalItems: jt,
                 optionsList: _t,
                 findSchemaDefinition: Ft,
-                guessType: Dt,
-                stubExistingAdditionalProperties: At,
-                resolveSchema: Ct,
-                retrieveSchema: $t,
-                mergeSchemas: Tt,
+                guessType: At,
+                stubExistingAdditionalProperties: Dt,
+                resolveSchema: kt,
+                retrieveSchema: Rt,
+                mergeSchemas: qt,
                 deepEquals: Lt,
-                shouldRender: Ut,
-                toIdSchema: Mt,
-                toPathSchema: Vt,
-                parseDateString: zt,
-                toDateString: Bt,
-                utcToLocal: Wt,
-                localToUTC: Qt,
-                pad: Ht,
-                dataURItoBlob: Kt,
-                rangeSpec: Jt,
-                getMatchingOption: Zt,
-                schemaRequiresTrueValue: Yt
+                shouldRender: Mt,
+                toIdSchema: Vt,
+                toPathSchema: zt,
+                parseDateString: Bt,
+                toDateString: Wt,
+                utcToLocal: Qt,
+                localToUTC: Ht,
+                pad: Kt,
+                dataURItoBlob: Jt,
+                rangeSpec: Zt,
+                getMatchingOption: Yt,
+                schemaRequiresTrueValue: Gt
             };
 
-            function Xt(e) {
+            function ea(e) {
                 var r = e.TitleField,
                     t = e.idSchema,
                     a = e.title,
                     n = e.required;
                 if (!a) return null;
                 var i = t.$id + "__title";
                 return o().createElement(r, {
                     id: i,
                     title: a,
                     required: n
                 })
             }
 
-            function ea(e) {
+            function ra(e) {
                 var r = e.DescriptionField,
                     t = e.idSchema,
                     a = e.description;
                 if (!a) return null;
                 var n = t.$id + "__description";
                 return o().createElement(r, {
                     id: n,
                     description: a
                 })
             }
 
-            function ra(e) {
+            function ta(e) {
                 var r = {
                     flex: 1,
                     paddingLeft: 6,
                     paddingRight: 6,
                     fontWeight: "bold"
                 };
                 return o().createElement("div", {
@@ -1516,119 +1518,119 @@
                     tabIndex: "-1",
                     style: r,
                     disabled: e.disabled || e.readonly,
                     onClick: e.onDropIndexClick(e.index)
                 }))))
             }
 
-            function ta(e) {
+            function aa(e) {
                 return o().createElement("fieldset", {
                     className: e.className,
                     id: e.idSchema.$id
-                }, o().createElement(Xt, {
+                }, o().createElement(ea, {
                     key: "array-field-title-" + e.idSchema.$id,
                     TitleField: e.TitleField,
                     idSchema: e.idSchema,
                     title: e.uiSchema["ui:title"] || e.title,
                     required: e.required
                 }), (e.uiSchema["ui:description"] || e.schema.description) && o().createElement("div", {
                     className: "field-description",
                     key: "field-description-" + e.idSchema.$id
                 }, e.uiSchema["ui:description"] || e.schema.description), o().createElement("div", {
                     className: "row array-item-list",
                     key: "array-item-list-" + e.idSchema.$id
-                }, e.items && e.items.map(ra)), e.canAdd && o().createElement(Br, {
+                }, e.items && e.items.map(ta)), e.canAdd && o().createElement(Br, {
                     className: "array-item-add",
                     onClick: e.onAddClick,
                     disabled: e.disabled || e.readonly
                 }))
             }
 
-            function aa(e) {
+            function oa(e) {
                 return o().createElement("fieldset", {
                     className: e.className,
                     id: e.idSchema.$id
-                }, o().createElement(Xt, {
+                }, o().createElement(ea, {
                     key: "array-field-title-" + e.idSchema.$id,
                     TitleField: e.TitleField,
                     idSchema: e.idSchema,
                     title: e.uiSchema["ui:title"] || e.title,
                     required: e.required
-                }), (e.uiSchema["ui:description"] || e.schema.description) && o().createElement(ea, {
+                }), (e.uiSchema["ui:description"] || e.schema.description) && o().createElement(ra, {
                     key: "array-field-description-" + e.idSchema.$id,
                     DescriptionField: e.DescriptionField,
                     idSchema: e.idSchema,
                     description: e.uiSchema["ui:description"] || e.schema.description
                 }), o().createElement("div", {
                     className: "row array-item-list",
                     key: "array-item-list-" + e.idSchema.$id
                 }, e.items && e.items.map((function(e) {
-                    return ra(e)
+                    return ta(e)
                 }))), e.canAdd && o().createElement(Br, {
                     className: "array-item-add",
                     onClick: e.onAddClick,
                     disabled: e.disabled || e.readonly
                 }))
             }
 
-            function oa() {
-                return ((e = 21) => crypto.getRandomValues(new Uint8Array(e)).reduce(((e, r) => e + ((r &= 63) < 36 ? r.toString(36) : r < 62 ? (r - 26).toString(36).toUpperCase() : r > 62 ? "-" : "_")), ""))()
+            function na() {
+                return Ir()
             }
 
-            function na(e) {
+            function ia(e) {
                 return Array.isArray(e) ? e.map((function(e) {
                     return {
-                        key: oa(),
+                        key: na(),
                         item: e
                     }
                 })) : []
             }
 
-            function ia(e) {
+            function sa(e) {
                 return e.map((function(e) {
                     return e.item
                 }))
             }
-            var sa = function(e) {
+            var ua = function(e) {
                 function r(r) {
                     var t;
                     (t = e.call(this, r) || this)._getNewFormDataRow = function() {
                         var e = t.props,
                             r = e.schema,
                             a = e.registry.rootSchema,
                             o = r.items;
                         return xt(r) && jt(r) && (o = r.additionalItems), ct(o, void 0, a)
                     }, t.onAddClick = function(e) {
                         e && e.preventDefault();
                         var r = t.props.onChange,
                             a = {
-                                key: oa(),
+                                key: na(),
                                 item: t._getNewFormDataRow()
                             },
                             o = [].concat(t.state.keyedFormData, [a]);
                         t.setState({
                             keyedFormData: o,
                             updatedKeyedFormData: !0
                         }, (function() {
-                            return r(ia(o))
+                            return r(sa(o))
                         }))
                     }, t.onAddIndexClick = function(e) {
                         return function(r) {
                             r && r.preventDefault();
                             var a = t.props.onChange,
                                 o = {
-                                    key: oa(),
+                                    key: na(),
                                     item: t._getNewFormDataRow()
                                 },
                                 n = [].concat(t.state.keyedFormData);
                             n.splice(e, 0, o), t.setState({
                                 keyedFormData: n,
                                 updatedKeyedFormData: !0
                             }, (function() {
-                                return a(ia(n))
+                                return a(sa(n))
                             }))
                         }
                     }, t.onDropIndexClick = function(e) {
                         return function(r) {
                             r && r.preventDefault();
                             var a, o = t.props.onChange,
                                 n = t.state.keyedFormData;
@@ -1640,15 +1642,15 @@
                             var u = n.filter((function(r, t) {
                                 return t !== e
                             }));
                             t.setState({
                                 keyedFormData: u,
                                 updatedKeyedFormData: !0
                             }, (function() {
-                                return o(ia(u), a)
+                                return o(sa(u), a)
                             }))
                         }
                     }, t.onReorderClick = function(e, r) {
                         return function(a) {
                             a && (a.preventDefault(), a.target.blur());
                             var o, n = t.props.onChange;
                             if (t.props.errorSchema) {
@@ -1657,52 +1659,52 @@
                                 for (var s in i) s == e ? o[r] = i[e] : s == r ? o[e] = i[r] : o[s] = i[s]
                             }
                             var u, l = t.state.keyedFormData,
                                 c = ((u = l.slice()).splice(e, 1), u.splice(r, 0, l[e]), u);
                             t.setState({
                                 keyedFormData: c
                             }, (function() {
-                                return n(ia(c), o)
+                                return n(sa(c), o)
                             }))
                         }
                     }, t.onChangeForIndex = function(e) {
                         return function(r, a) {
                             var o, n = t.props,
                                 i = n.formData;
                             (0, n.onChange)(i.map((function(t, a) {
                                 return e === a ? void 0 === r ? null : r : t
                             })), a && t.props.errorSchema && qr({}, t.props.errorSchema, ((o = {})[e] = a, o)))
                         }
                     }, t.onSelectChange = function(e) {
                         t.props.onChange(e)
                     };
-                    var a = na(r.formData);
+                    var a = ia(r.formData);
                     return t.state = {
                         keyedFormData: a,
                         updatedKeyedFormData: !1
                     }, t
                 }
-                Lr(r, e), r.getDerivedStateFromProps = function(e, r) {
+                Ur(r, e), r.getDerivedStateFromProps = function(e, r) {
                     if (r.updatedKeyedFormData) return {
                         updatedKeyedFormData: !1
                     };
                     var t = e.formData || [],
                         a = r.keyedFormData || [];
                     return {
                         keyedFormData: t.length === a.length ? a.map((function(e, r) {
                             return {
                                 key: e.key,
                                 item: t[r]
                             }
-                        })) : na(t)
+                        })) : ia(t)
                     }
                 };
                 var t = r.prototype;
                 return t.isItemRequired = function(e) {
-                    return Array.isArray(e.type) ? !vr()(e.type, "null") : "null" !== e.type
+                    return Array.isArray(e.type) ? !mr()(e.type, "null") : "null" !== e.type
                 }, t.canAddItem = function(e) {
                     var r = this.props,
                         t = r.schema,
                         a = ft(r.uiSchema).addable;
                     return !1 !== a && (a = void 0 === t.maxItems || e.length < t.maxItems), a
                 }, t.render = function() {
                     var e = this.props,
@@ -1743,24 +1745,24 @@
                         E = void 0 === t.title ? s : t.title,
                         P = p.ArrayFieldTemplate,
                         w = p.rootSchema,
                         S = p.fields,
                         x = p.formContext,
                         O = S.TitleField,
                         j = S.DescriptionField,
-                        _ = $t(t.items, w),
-                        F = ia(this.state.keyedFormData),
-                        D = {
+                        _ = Rt(t.items, w),
+                        F = sa(this.state.keyedFormData),
+                        A = {
                             canAdd: this.canAddItem(F),
                             items: this.state.keyedFormData.map((function(r, o) {
                                 var s = r.key,
                                     u = r.item,
-                                    l = $t(t.items, w, u),
+                                    l = Rt(t.items, w, u),
                                     c = n ? n[o] : void 0,
-                                    d = Mt(l, i.$id + g + o, w, u, v, g);
+                                    d = Vt(l, i.$id + g + o, w, u, v, g);
                                 return e.renderArrayFieldItem({
                                     key: s,
                                     index: o,
                                     canMoveUp: o > 0,
                                     canMoveDown: o < F.length - 1,
                                     itemSchema: l,
                                     itemIdSchema: d,
@@ -1785,16 +1787,16 @@
                             title: E,
                             TitleField: O,
                             formContext: x,
                             formData: F,
                             rawErrors: b,
                             registry: p
                         },
-                        A = a["ui:ArrayFieldTemplate"] || P || aa;
-                    return o().createElement(A, D)
+                        D = a["ui:ArrayFieldTemplate"] || P || oa;
+                    return o().createElement(D, A)
                 }, t.renderCustomWidget = function() {
                     var e = this.props,
                         r = e.schema,
                         t = e.idSchema,
                         a = e.uiSchema,
                         n = e.disabled,
                         i = e.readonly,
@@ -1852,15 +1854,15 @@
                         p = e.registry,
                         h = e.rawErrors,
                         m = e.name,
                         v = this.props.formData,
                         y = p.widgets,
                         g = p.rootSchema,
                         b = p.formContext,
-                        E = $t(r.items, g, n),
+                        E = Rt(r.items, g, n),
                         P = r.title || m,
                         w = _t(E),
                         S = qr({}, ft(a), {
                             enumOptions: w
                         }),
                         x = S.widget,
                         O = void 0 === x ? "select" : x,
@@ -1950,30 +1952,30 @@
                         P = this.props.formData,
                         w = v.ArrayFieldTemplate,
                         S = v.rootSchema,
                         x = v.fields,
                         O = v.formContext,
                         j = x.TitleField,
                         _ = t.items.map((function(e, r) {
-                            return $t(e, S, n[r])
+                            return Rt(e, S, n[r])
                         })),
-                        F = jt(t) ? $t(t.additionalItems, S, n) : null;
+                        F = jt(t) ? Rt(t.additionalItems, S, n) : null;
                     (!P || P.length < _.length) && (P = (P = P || []).concat(new Array(_.length - P.length)));
-                    var D = {
+                    var A = {
                             canAdd: this.canAddItem(P) && F,
                             className: "field field-array field-array-fixed-items",
                             disabled: p,
                             idSchema: c,
                             formData: n,
                             items: this.state.keyedFormData.map((function(r, o) {
                                 var n = r.key,
                                     u = r.item,
                                     d = o >= _.length,
-                                    f = d ? $t(t.additionalItems, S, u) : _[o],
-                                    p = Mt(f, c.$id + l + o, S, u, s, l),
+                                    f = d ? Rt(t.additionalItems, S, u) : _[o],
+                                    p = Vt(f, c.$id + l + o, S, u, s, l),
                                     h = d ? a.additionalItems || {} : Array.isArray(a.items) ? a.items[o] : a.items || {},
                                     v = i ? i[o] : void 0;
                                 return e.renderArrayFieldItem({
                                     key: n,
                                     index: o,
                                     canRemove: d,
                                     canMoveUp: o >= _.length + 1,
@@ -1995,16 +1997,16 @@
                             schema: t,
                             uiSchema: a,
                             title: E,
                             TitleField: j,
                             formContext: O,
                             rawErrors: b
                         },
-                        A = a["ui:ArrayFieldTemplate"] || w || ta;
-                    return o().createElement(A, D)
+                        D = a["ui:ArrayFieldTemplate"] || w || aa;
+                    return o().createElement(D, A)
                 }, t.renderArrayFieldItem = function(e) {
                     var r = e.key,
                         t = e.index,
                         a = e.canRemove,
                         n = void 0 === a || a,
                         i = e.canMoveUp,
                         s = void 0 === i || i,
@@ -2074,15 +2076,15 @@
                     get: function() {
                         var e = this.props.schema;
                         return e.items.title || e.items.description || "Item"
                     }
                 }]), r
             }(a.Component);
 
-            function ua(e) {
+            function la(e) {
                 var r, t = e.schema,
                     a = e.name,
                     n = e.uiSchema,
                     i = e.idSchema,
                     s = e.formData,
                     u = e.registry,
                     l = e.required,
@@ -2129,41 +2131,41 @@
                     registry: u,
                     formContext: b,
                     autofocus: f,
                     rawErrors: v,
                     DescriptionField: E.DescriptionField
                 })
             }
-            sa.defaultProps = {
+            ua.defaultProps = {
                 uiSchema: {},
                 formData: [],
                 idSchema: {},
                 required: !1,
                 disabled: !1,
                 readonly: !1,
                 autofocus: !1
-            }, ua.defaultProps = {
+            }, la.defaultProps = {
                 uiSchema: {},
                 disabled: !1,
                 readonly: !1,
                 autofocus: !1
             };
-            var la = function(e) {
+            var ca = function(e) {
                 function r(r) {
                     var t;
                     (t = e.call(this, r) || this).onOptionChange = function(e) {
                         var r = parseInt(e, 10),
                             a = t.props,
                             o = a.formData,
                             n = a.onChange,
                             i = a.options,
                             s = a.registry.rootSchema,
-                            u = $t(i[r], s, o),
+                            u = Rt(i[r], s, o),
                             l = void 0;
-                        if ("object" === Dt(o) && ("object" === u.type || u.properties)) {
+                        if ("object" === At(o) && ("object" === u.type || u.properties)) {
                             l = Object.assign({}, o);
                             var c = i.slice();
                             c.splice(r, 1);
                             var d = c,
                                 f = Array.isArray(d),
                                 p = 0;
                             for (d = f ? d : d[Symbol.iterator]();;) {
@@ -2187,26 +2189,26 @@
                     var a = t.props,
                         o = a.formData,
                         n = a.options;
                     return t.state = {
                         selectedOption: t.getMatchingOption(o, n)
                     }, t
                 }
-                Lr(r, e);
+                Ur(r, e);
                 var t = r.prototype;
                 return t.componentDidUpdate = function(e, r) {
                     if (!Lt(this.props.formData, e.formData) && this.props.idSchema.$id === e.idSchema.$id) {
                         var t = this.getMatchingOption(this.props.formData, this.props.options);
                         if (!r || t === this.state.selectedOption) return;
                         this.setState({
                             selectedOption: t
                         })
                     }
                 }, t.getMatchingOption = function(e, r) {
-                    var t = Zt(e, r, this.props.registry.rootSchema);
+                    var t = Yt(e, r, this.props.registry.rootSchema);
                     return 0 !== t ? t : this && this.state ? this.state.selectedOption : 0
                 }, t.render = function() {
                     var e, r = this.props,
                         t = r.baseType,
                         a = r.disabled,
                         n = r.readonly,
                         i = r.hideError,
@@ -2274,38 +2276,38 @@
                         registry: v,
                         disabled: a,
                         readonly: n,
                         hideError: i
                     }))
                 }, r
             }(a.Component);
-            la.defaultProps = {
+            ca.defaultProps = {
                 disabled: !1,
                 readonly: !1,
                 hideError: !1,
                 errorSchema: {},
                 idSchema: {},
                 uiSchema: {}
             };
-            var ca = /\.([0-9]*0)*$/,
-                da = /[0.]0*$/,
-                fa = function(e) {
+            var da = /\.([0-9]*0)*$/,
+                fa = /[0.]0*$/,
+                pa = function(e) {
                     function r(r) {
                         var t;
                         return (t = e.call(this, r) || this).handleChange = function(e) {
                             t.setState({
                                 lastValue: e
                             }), "." === ("" + e).charAt(0) && (e = "0" + e);
-                            var r = "string" == typeof e && e.match(ca) ? yt(e.replace(da, "")) : yt(e);
+                            var r = "string" == typeof e && e.match(da) ? yt(e.replace(fa, "")) : yt(e);
                             t.props.onChange(r)
                         }, t.state = {
                             lastValue: r.value
                         }, t
                     }
-                    return Lr(r, e), r.prototype.render = function() {
+                    return Ur(r, e), r.prototype.render = function() {
                         var e = this.props.registry.fields.StringField,
                             r = this.props,
                             t = r.formData,
                             a = Mr(r, ["formData"]),
                             n = this.state.lastValue,
                             i = t;
                         if ("string" == typeof n && "number" == typeof i) {
@@ -2315,15 +2317,15 @@
                         return o().createElement(e, qr({}, a, {
                             formData: i,
                             onChange: this.handleChange
                         }))
                     }, r
                 }(o().Component);
 
-            function pa(e) {
+            function ha(e) {
                 var r = e.TitleField,
                     t = e.DescriptionField;
                 return o().createElement("fieldset", {
                     id: e.idSchema.$id
                 }, (e.uiSchema["ui:title"] || e.title) && o().createElement(r, {
                     id: e.idSchema.$id + "__title",
                     title: e.title || e.uiSchema["ui:title"],
@@ -2337,18 +2339,18 @@
                     return e.content
                 })), nt(e.schema, e.uiSchema, e.formData) && o().createElement(Br, {
                     className: "object-property-expand",
                     onClick: e.onAddClick(e.schema),
                     disabled: e.disabled || e.readonly
                 }))
             }
-            fa.defaultProps = {
+            pa.defaultProps = {
                 uiSchema: {}
             };
-            var ha = function(e) {
+            var ma = function(e) {
                 function r() {
                     for (var r, t = arguments.length, a = new Array(t), o = 0; o < t; o++) a[o] = arguments[o];
                     return (r = e.call.apply(e, [this].concat(a)) || this).state = {
                         wasPropertyKeyModified: !1,
                         additionalProperties: {}
                     }, r.onPropertyChange = function(e, t) {
                         return void 0 === t && (t = !1),
@@ -2388,23 +2390,23 @@
                         }
                     }, r.handleAddClick = function(e) {
                         return function() {
                             var t = e.additionalProperties.type,
                                 a = qr({}, r.props.formData);
                             if (e.additionalProperties.hasOwnProperty("$ref")) {
                                 var o = r.props.registry;
-                                t = $t({
+                                t = Rt({
                                     $ref: e.additionalProperties.$ref
                                 }, o.rootSchema, r.props.formData).type
                             }
                             a[r.getAvailableKey("newKey", a)] = r.getDefaultValue(t), r.props.onChange(a)
                         }
                     }, r
                 }
-                Lr(r, e);
+                Ur(r, e);
                 var t = r.prototype;
                 return t.isRequired = function(e) {
                     var r = this.props.schema;
                     return Array.isArray(r.required) && -1 !== r.required.indexOf(e)
                 }, t.getDefaultValue = function(e) {
                     switch (e) {
                         case "string":
@@ -2440,28 +2442,28 @@
                         y = t.registry,
                         g = y.rootSchema,
                         b = y.fields,
                         E = y.formContext,
                         P = b.SchemaField,
                         w = b.TitleField,
                         S = b.DescriptionField,
-                        x = $t(this.props.schema, g, n),
+                        x = Rt(this.props.schema, g, n),
                         O = void 0 === x.title ? u : x.title,
                         j = a["ui:description"] || x.description;
                     try {
                         e = gt(Object.keys(x.properties || {}), a["ui:order"])
                     } catch (e) {
                         return o().createElement("div", null, o().createElement("p", {
                             className: "config-error",
                             style: {
                                 color: "red"
                             }
                         }, "Invalid ", u || "root", " object field configuration:", o().createElement("em", null, e.message), "."), o().createElement("pre", null, JSON.stringify(x)))
                     }
-                    var _ = a["ui:ObjectFieldTemplate"] || y.ObjectFieldTemplate || pa,
+                    var _ = a["ui:ObjectFieldTemplate"] || y.ObjectFieldTemplate || ha,
                         F = {
                             title: a["ui:title"] || O,
                             description: j,
                             TitleField: w,
                             DescriptionField: S,
                             properties: e.map((function(e) {
                                 var t = x.properties[e].hasOwnProperty(at),
@@ -2508,107 +2510,108 @@
                             registry: y
                         };
                     return o().createElement(_, qr({}, F, {
                         onAddClick: this.handleAddClick
                     }))
                 }, r
             }(a.Component);
-            ha.defaultProps = {
+            ma.defaultProps = {
                 uiSchema: {},
                 formData: {},
                 errorSchema: {},
                 idSchema: {},
                 required: !1,
                 disabled: !1,
                 readonly: !1
             };
-            var ma = {
-                array: "ArrayField",
-                boolean: "BooleanField",
-                integer: "NumberField",
-                number: "NumberField",
-                object: "ObjectField",
-                string: "StringField",
-                null: "NullField"
-            };
+            var va = "*",
+                ya = {
+                    array: "ArrayField",
+                    boolean: "BooleanField",
+                    integer: "NumberField",
+                    number: "NumberField",
+                    object: "ObjectField",
+                    string: "StringField",
+                    null: "NullField"
+                };
 
-            function va(e) {
+            function ga(e) {
                 var r = e.label,
                     t = e.required,
                     a = e.id;
                 return r ? o().createElement("label", {
                     className: "control-label",
                     htmlFor: a
                 }, r, t && o().createElement("span", {
                     className: "required"
-                }, "*")) : null
+                }, va)) : null
             }
 
-            function ya(e) {
+            function ba(e) {
                 var r = e.id,
                     t = e.label,
                     a = e.onChange;
                 return o().createElement("input", {
                     className: "form-control",
                     type: "text",
                     id: r,
                     onBlur: function(e) {
                         return a(e.target.value)
                     },
                     defaultValue: t
                 })
             }
 
-            function ga(e) {
+            function Ea(e) {
                 var r = e.id,
                     t = e.help;
                 return t ? "string" == typeof t ? o().createElement("p", {
                     id: r,
                     className: "help-block"
                 }, t) : o().createElement("div", {
                     id: r,
                     className: "help-block"
                 }, t) : null
             }
 
-            function ba(e) {
+            function Pa(e) {
                 var r = e.errors,
                     t = void 0 === r ? [] : r;
                 return 0 === t.length ? null : o().createElement("div", null, o().createElement("ul", {
                     className: "error-detail bs-callout bs-callout-info"
                 }, t.filter((function(e) {
                     return !!e
                 })).map((function(e, r) {
                     return o().createElement("li", {
                         className: "text-danger",
                         key: r
                     }, e)
                 }))))
             }
 
-            function Ea(e) {
+            function wa(e) {
                 var r = e.id,
                     t = e.label,
                     a = e.children,
                     n = e.errors,
                     i = e.help,
                     s = e.description,
                     u = e.hidden,
                     l = e.required,
                     c = e.displayLabel;
                 return u ? o().createElement("div", {
                     className: "hidden"
-                }, a) : o().createElement(Pa, e, c && o().createElement(va, {
+                }, a) : o().createElement(Sa, e, c && o().createElement(ga, {
                     label: t,
                     required: l,
                     id: r
                 }), c && s ? s : null, a, n, i)
             }
 
-            function Pa(e) {
+            function Sa(e) {
                 var r = e.id,
                     t = e.classNames,
                     a = e.disabled,
                     n = e.label,
                     i = e.onKeyChange,
                     s = e.onDropPropertyClick,
                     u = e.readonly,
@@ -2618,19 +2621,19 @@
                     className: t
                 }, o().createElement("div", {
                     className: "row"
                 }, o().createElement("div", {
                     className: "col-xs-5 form-additional"
                 }, o().createElement("div", {
                     className: "form-group"
-                }, o().createElement(va, {
+                }, o().createElement(ga, {
                     label: c,
                     required: l,
                     id: r + "-key"
-                }), o().createElement(ya, {
+                }), o().createElement(ba, {
                     label: n,
                     required: l,
                     id: r + "-key",
                     onChange: i
                 }))), o().createElement("div", {
                     className: "form-additional form-group col-xs-5"
                 }, e.children), o().createElement("div", {
@@ -2645,25 +2648,25 @@
                     },
                     disabled: a || u,
                     onClick: s(n)
                 })))) : o().createElement("div", {
                     className: t
                 }, e.children)
             }
-            Ea.defaultProps = {
+            wa.defaultProps = {
                 hidden: !1,
                 readonly: !1,
                 required: !1,
                 displayLabel: !0
             };
-            var wa = function(e) {
+            var xa = function(e) {
                 function r() {
                     return e.apply(this, arguments) || this
                 }
-                Lr(r, e);
+                Ur(r, e);
                 var t = r.prototype;
                 return t.shouldComponentUpdate = function(e, r) {
                     return !Lt(this.props, e)
                 }, t.render = function() {
                     return function(e) {
                         var r = e.uiSchema,
                             t = e.formData,
@@ -2677,116 +2680,116 @@
                             d = e.required,
                             f = e.registry,
                             p = e.wasPropertyKeyModified,
                             h = void 0 !== p && p,
                             m = f.rootSchema,
                             v = f.fields,
                             y = f.formContext,
-                            g = r["ui:FieldTemplate"] || f.FieldTemplate || Ea,
+                            g = r["ui:FieldTemplate"] || f.FieldTemplate || wa,
                             b = e.idSchema,
-                            E = $t(e.schema, m, t),
+                            E = Rt(e.schema, m, t),
                             P = function(e, r, t, a) {
                                 var n = r["ui:field"];
                                 if ("function" == typeof n) return n;
                                 if ("string" == typeof n && n in a) return a[n];
-                                var i = ma[it(e)];
+                                var i = ya[it(e)];
                                 return i || !e.anyOf && !e.oneOf ? i in a ? a[i] : function() {
                                     var r = a.UnsupportedField;
                                     return o().createElement(r, {
                                         schema: e,
                                         idSchema: t,
                                         reason: "Unknown field type " + e.type
                                     })
                                 } : function() {
                                     return null
                                 }
-                            }(E, r, b = vt(Mt(E, null, m, t, n, i), b), v),
+                            }(E, r, b = vt(Vt(E, null, m, t, n, i), b), v),
                             w = v.DescriptionField,
                             S = Boolean(e.disabled || r["ui:disabled"]),
                             x = Boolean(e.readonly || r["ui:readonly"] || e.schema.readOnly || E.readOnly),
                             O = r["ui:hideError"],
                             j = void 0 === O ? e.hideError : Boolean(O),
                             _ = Boolean(e.autofocus || r["ui:autofocus"]);
                         if (0 === Object.keys(E).length) return null;
-                        var F, D = ht(E, r, m),
-                            A = a.__errors,
+                        var F, A = ht(E, r, m),
+                            D = a.__errors,
                             C = Mr(a, ["__errors"]),
                             k = o().createElement(P, qr({}, e, {
                                 idSchema: b,
                                 schema: E,
                                 uiSchema: qr({}, r, {
                                     classNames: void 0
                                 }),
                                 disabled: S,
                                 readonly: x,
                                 hideError: j,
                                 autofocus: _,
                                 errorSchema: C,
                                 formContext: y,
-                                rawErrors: A
+                                rawErrors: D
                             })),
                             $ = b.$id;
                         F = h ? s : r["ui:title"] || e.schema.title || E.title || s;
                         var R = r["ui:description"] || e.schema.description || E.description,
-                            I = A,
+                            I = D,
                             N = r["ui:help"],
                             T = "hidden" === r["ui:widget"],
                             q = ["form-group", "field", "field-" + E.type];
                         !j && I && I.length > 0 && q.push("field-error has-error has-danger"), q.push(r.classNames), q = q.join(" ").trim();
-                        var L = {
+                        var U = {
                                 description: o().createElement(w, {
                                     id: $ + "__description",
                                     description: R,
                                     formContext: y
                                 }),
                                 rawDescription: R,
-                                help: o().createElement(ga, {
+                                help: o().createElement(Ea, {
                                     id: $ + "__help",
                                     help: N
                                 }),
                                 rawHelp: "string" == typeof N ? N : void 0,
-                                errors: j ? void 0 : o().createElement(ba, {
+                                errors: j ? void 0 : o().createElement(Pa, {
                                     errors: I
                                 }),
                                 rawErrors: j ? void 0 : I,
                                 id: $,
                                 label: F,
                                 hidden: T,
                                 onChange: u,
                                 onKeyChange: l,
                                 onDropPropertyClick: c,
                                 required: d,
                                 disabled: S,
                                 readonly: x,
                                 hideError: j,
-                                displayLabel: D,
+                                displayLabel: A,
                                 classNames: q,
                                 formContext: y,
                                 formData: t,
                                 fields: v,
                                 schema: E,
                                 uiSchema: r,
                                 registry: f
                             },
-                            U = f.fields.AnyOfField,
+                            L = f.fields.AnyOfField,
                             M = f.fields.OneOfField;
-                        return o().createElement(g, L, o().createElement(o().Fragment, null, k, E.anyOf && !Pt(E) && o().createElement(U, {
+                        return o().createElement(g, U, o().createElement(o().Fragment, null, k, E.anyOf && !Pt(E) && o().createElement(L, {
                             disabled: S,
                             readonly: x,
                             hideError: j,
                             errorSchema: a,
                             formData: t,
                             idPrefix: n,
                             idSchema: b,
                             idSeparator: i,
                             onBlur: e.onBlur,
                             onChange: e.onChange,
                             onFocus: e.onFocus,
                             options: E.anyOf.map((function(e) {
-                                return $t(e, m, t)
+                                return Rt(e, m, t)
                             })),
                             baseType: E.type,
                             registry: f,
                             schema: E,
                             uiSchema: r
                         }), E.oneOf && !Pt(E) && o().createElement(M, {
                             disabled: S,
@@ -2797,26 +2800,26 @@
                             idPrefix: n,
                             idSchema: b,
                             idSeparator: i,
                             onBlur: e.onBlur,
                             onChange: e.onChange,
                             onFocus: e.onFocus,
                             options: E.oneOf.map((function(e) {
-                                return $t(e, m, t)
+                                return Rt(e, m, t)
                             })),
                             baseType: E.type,
                             registry: f,
                             schema: E,
                             uiSchema: r
                         })))
                     }(this.props)
                 }, r
             }(o().Component);
 
-            function Sa(e) {
+            function Oa(e) {
                 var r = e.schema,
                     t = e.name,
                     a = e.uiSchema,
                     n = e.idSchema,
                     i = e.formData,
                     s = e.required,
                     u = e.disabled,
@@ -2859,63 +2862,63 @@
                     formContext: b,
                     autofocus: c,
                     registry: h,
                     placeholder: j,
                     rawErrors: m
                 })
             }
-            wa.defaultProps = {
+            xa.defaultProps = {
                 uiSchema: {},
                 errorSchema: {},
                 idSchema: {},
                 disabled: !1,
                 readonly: !1,
                 autofocus: !1,
                 hideError: !1
-            }, Sa.defaultProps = {
+            }, Oa.defaultProps = {
                 uiSchema: {},
                 disabled: !1,
                 readonly: !1,
                 autofocus: !1
             };
-            var xa = {
-                AnyOfField: la,
-                ArrayField: sa,
-                BooleanField: ua,
+            var ja = {
+                AnyOfField: ca,
+                ArrayField: ua,
+                BooleanField: la,
                 DescriptionField: function(e) {
                     var r = e.id,
                         t = e.description;
                     return t ? "string" == typeof t ? o().createElement("p", {
                         id: r,
                         className: "field-description"
                     }, t) : o().createElement("div", {
                         id: r,
                         className: "field-description"
                     }, t) : null
                 },
-                NumberField: fa,
-                ObjectField: ha,
-                OneOfField: la,
-                SchemaField: wa,
-                StringField: Sa,
+                NumberField: pa,
+                ObjectField: ma,
+                OneOfField: ca,
+                SchemaField: xa,
+                StringField: Oa,
                 TitleField: function(e) {
                     var r = e.id,
                         t = e.title,
                         a = e.required;
                     return o().createElement("legend", {
                         id: r
                     }, t, a && o().createElement("span", {
                         className: "required"
                     }, "*"))
                 },
                 NullField: function(e) {
                     function r() {
                         return e.apply(this, arguments) || this
                     }
-                    Lr(r, e);
+                    Ur(r, e);
                     var t = r.prototype;
                     return t.componentDidMount = function() {
                         void 0 === this.props.formData && this.props.onChange(null)
                     }, t.render = function() {
                         return null
                     }, r
                 }(a.Component),
@@ -2925,23 +2928,23 @@
                         a = e.reason;
                     return o().createElement("div", {
                         className: "unsupported-field"
                     }, o().createElement("p", null, "Unsupported field schema", t && t.$id && o().createElement("span", null, " for", " field ", o().createElement("code", null, t.$id)), a && o().createElement("em", null, ": ", a), "."), r && o().createElement("pre", null, JSON.stringify(r, null, 2)))
                 }
             };
 
-            function Oa(e, r) {
+            function _a(e, r) {
                 for (var t = [], a = e; a <= r; a++) t.push({
                     value: a,
-                    label: Ht(a, 2)
+                    label: Kt(a, 2)
                 });
                 return t
             }
 
-            function ja(e) {
+            function Fa(e) {
                 var r = e.type,
                     t = e.range,
                     a = e.value,
                     n = e.select,
                     i = e.rootId,
                     s = e.disabled,
                     u = e.readonly,
@@ -2953,69 +2956,69 @@
                 return o().createElement(p, {
                     schema: {
                         type: "integer"
                     },
                     id: f,
                     className: "form-control",
                     options: {
-                        enumOptions: Oa(t[0], t[1])
+                        enumOptions: _a(t[0], t[1])
                     },
                     placeholder: r,
                     value: a,
                     disabled: s,
                     readonly: u,
                     autofocus: l,
                     onChange: function(e) {
                         return n(r, e)
                     },
                     onBlur: d
                 })
             }
-            var _a = function(e) {
+            var Aa = function(e) {
                 function r(r) {
                     var t;
                     return (t = e.call(this, r) || this).onChange = function(e, r) {
                         var a;
                         t.setState(((a = {})[e] = void 0 === r ? -1 : r, a), (function() {
                             var e;
                             e = t.state, Object.keys(e).every((function(r) {
                                 return -1 !== e[r]
-                            })) && t.props.onChange(Bt(t.state, t.props.time))
+                            })) && t.props.onChange(Wt(t.state, t.props.time))
                         }))
                     }, t.setNow = function(e) {
                         e.preventDefault();
                         var r = t.props,
                             a = r.time,
                             o = r.disabled,
                             n = r.readonly,
                             i = r.onChange;
                         if (!o && !n) {
-                            var s = zt((new Date).toJSON(), a);
+                            var s = Bt((new Date).toJSON(), a);
                             t.setState(s, (function() {
-                                return i(Bt(t.state, a))
+                                return i(Wt(t.state, a))
                             }))
                         }
                     }, t.clear = function(e) {
                         e.preventDefault();
                         var r = t.props,
                             a = r.time,
                             o = r.disabled,
                             n = r.readonly,
                             i = r.onChange;
-                        o || n || t.setState(zt("", a), (function() {
+                        o || n || t.setState(Bt("", a), (function() {
                             return i(void 0)
                         }))
-                    }, t.state = zt(r.value, r.time), t
+                    }, t.state = Bt(r.value, r.time), t
                 }
-                Lr(r, e);
+                Ur(r, e);
                 var t = r.prototype;
                 return t.componentDidUpdate = function(e, r) {
-                    e.value && e.value !== zt(this.props.value, this.props.time) && this.setState(zt(this.props.value, this.props.time))
+                    e.value && e.value !== Bt(this.props.value, this.props.time) && this.setState(Bt(this.props.value, this.props.time))
                 }, t.shouldComponentUpdate = function(e, r) {
-                    return Ut(this, e, r)
+                    return Mt(this, e, r)
                 }, t.render = function() {
                     var e = this,
                         r = this.props,
                         t = r.id,
                         a = r.disabled,
                         n = r.readonly,
                         i = r.autofocus,
@@ -3023,15 +3026,15 @@
                         u = r.onBlur,
                         l = r.options;
                     return o().createElement("ul", {
                         className: "list-inline"
                     }, this.dateElementProps.map((function(r, l) {
                         return o().createElement("li", {
                             key: l
-                        }, o().createElement(ja, qr({
+                        }, o().createElement(Fa, qr({
                             rootId: t,
                             select: e.onChange
                         }, r, {
                             disabled: a,
                             readonly: n,
                             registry: s,
                             onBlur: u,
@@ -3085,22 +3088,22 @@
                             range: [0, 59],
                             value: l
                         }), c
                     }
                 }]), r
             }(a.Component);
 
-            function Fa(e) {
+            function Da(e) {
                 var r = e.registry.widgets.AltDateWidget;
                 return o().createElement(r, qr({
                     time: !0
                 }, e))
             }
 
-            function Da(e) {
+            function Ca(e) {
                 if (!e.id) throw console.log("No id for", e), new Error("no id for props " + JSON.stringify(e));
                 var r = e.value,
                     t = e.readonly,
                     a = e.disabled,
                     n = e.autofocus,
                     i = e.onBlur,
                     s = e.onFocus,
@@ -3133,27 +3136,27 @@
                     return o().createElement("option", {
                         key: e,
                         value: e
                     })
                 }))) : null]
             }
 
-            function Aa(e) {
+            function ka(e) {
                 var r = e.schema,
                     t = e.id,
                     a = e.value,
                     n = e.disabled,
                     i = e.readonly,
                     s = e.label,
                     u = e.autofocus,
                     l = e.onBlur,
                     c = e.onFocus,
                     d = e.onChange,
                     f = e.DescriptionField,
-                    p = Yt(r);
+                    p = Gt(r);
                 return o().createElement("div", {
                     className: "checkbox " + (n || i ? "disabled" : "")
                 }, r.description && o().createElement(f, {
                     description: r.description
                 }), o().createElement("label", null, o().createElement("input", {
                     type: "checkbox",
                     id: t,
@@ -3169,15 +3172,15 @@
                     },
                     onFocus: c && function(e) {
                         return c(t, e.target.checked)
                     }
                 }), o().createElement("span", null, s)))
             }
 
-            function Ca(e) {
+            function $a(e) {
                 var r = e.id,
                     t = e.disabled,
                     a = e.options,
                     n = e.value,
                     i = e.autofocus,
                     s = e.readonly,
                     u = e.onChange,
@@ -3219,79 +3222,79 @@
                     }, m) : o().createElement("div", {
                         key: a,
                         className: "checkbox " + h
                     }, o().createElement("label", null, m))
                 })))
             }
 
-            function ka(e, r) {
+            function Ra(e, r) {
                 return e.replace(";base64", ";name=" + encodeURIComponent(r) + ";base64")
             }
 
-            function $a(e) {
+            function Ia(e) {
                 var r = e.name,
                     t = e.size,
                     a = e.type;
                 return new Promise((function(o, n) {
                     var i = new window.FileReader;
                     i.onerror = n, i.onload = function(e) {
                         o({
-                            dataURL: ka(e.target.result, r),
+                            dataURL: Ra(e.target.result, r),
                             name: r,
                             size: t,
                             type: a
                         })
                     }, i.readAsDataURL(e)
                 }))
             }
 
-            function Ra(e) {
+            function Na(e) {
                 var r = e.filesInfo;
                 return 0 === r.length ? null : o().createElement("ul", {
                     className: "file-info"
                 }, r.map((function(e, r) {
                     var t = e.name,
                         a = e.size,
                         n = e.type;
                     return o().createElement("li", {
                         key: r
                     }, o().createElement("strong", null, t), " (", n, ", ", a, " bytes)")
                 })))
             }
-            _a.defaultProps = {
+            Aa.defaultProps = {
                 time: !1,
                 disabled: !1,
                 readonly: !1,
                 autofocus: !1,
                 options: {
                     yearsRange: [1900, (new Date).getFullYear() + 2]
                 }
-            }, Fa.defaultProps = qr({}, _a.defaultProps, {
+            }, Da.defaultProps = qr({}, Aa.defaultProps, {
                 time: !0
-            }), Da.defaultProps = {
+            }), Ca.defaultProps = {
                 required: !1,
                 disabled: !1,
                 readonly: !1,
                 autofocus: !1
-            }, Aa.defaultProps = {
+            }, ka.defaultProps = {
                 autofocus: !1
-            }, Ca.defaultProps = {
+            }, $a.defaultProps = {
                 autofocus: !1,
                 options: {
                     inline: !1
                 }
             };
-            var Ia = function(e) {
+            var Ta = function(e) {
                 function r(r) {
                     var t;
                     (t = e.call(this, r) || this).onChange = function(e) {
                         var r, a = t.props,
                             o = a.multiple,
                             n = a.onChange;
-                        (r = e.target.files, Promise.all([].map.call(r, $a))).then((function(e) {
+                        (r = e.target.files, Promise.all([].map.call(r, Ia))).then((function(e) {
                             var r = {
                                 values: e.map((function(e) {
                                     return e.dataURL
                                 })),
                                 filesInfo: e
                             };
                             t.setState(r, (function() {
@@ -3302,28 +3305,28 @@
                     var a, o = r.value,
                         n = Array.isArray(o) ? o : [o];
                     return t.state = {
                         values: n,
                         filesInfo: (a = n, a.filter((function(e) {
                             return void 0 !== e
                         })).map((function(e) {
-                            var r = Kt(e),
+                            var r = Jt(e),
                                 t = r.blob;
                             return {
                                 name: r.name,
                                 size: t.size,
                                 type: t.type
                             }
                         })))
                     }, t
                 }
-                Lr(r, e);
+                Ur(r, e);
                 var t = r.prototype;
                 return t.shouldComponentUpdate = function(e, r) {
-                    return Ut(this, e, r)
+                    return Mt(this, e, r)
                 }, t.render = function() {
                     var e = this,
                         r = this.props,
                         t = r.multiple,
                         a = r.id,
                         n = r.readonly,
                         i = r.disabled,
@@ -3338,21 +3341,21 @@
                         type: "file",
                         disabled: n || i,
                         onChange: this.onChange,
                         defaultValue: "",
                         autoFocus: s,
                         multiple: t,
                         accept: u.accept
-                    })), o().createElement(Ra, {
+                    })), o().createElement(Na, {
                         filesInfo: l
                     }))
                 }, r
             }(a.Component);
 
-            function Na(e) {
+            function qa(e) {
                 var r = e.options,
                     t = e.value,
                     a = e.required,
                     n = e.disabled,
                     i = e.readonly,
                     s = e.autofocus,
                     u = e.onBlur,
@@ -3393,49 +3396,49 @@
                         className: "radio-inline " + y
                     }, g) : o().createElement("div", {
                         key: r,
                         className: "radio " + y
                     }, o().createElement("label", null, g))
                 })))
             }
-            Ia.defaultProps = {
+            Ta.defaultProps = {
                 autofocus: !1
-            }, Na.defaultProps = {
+            }, qa.defaultProps = {
                 autofocus: !1
             };
-            var Ta = new Set(["number", "integer"]);
+            var Ua = new Set(["number", "integer"]);
 
-            function qa(e, r) {
+            function La(e, r) {
                 var t = e.type,
                     a = e.items;
                 if ("" !== r) {
-                    if ("array" === t && a && Ta.has(a.type)) return r.map(yt);
+                    if ("array" === t && a && Ua.has(a.type)) return r.map(yt);
                     if ("boolean" === t) return "true" === r;
                     if ("number" === t) return yt(r);
                     if (e.enum) {
                         if (e.enum.every((function(e) {
-                                return "number" === Dt(e)
+                                return "number" === At(e)
                             }))) return yt(r);
                         if (e.enum.every((function(e) {
-                                return "boolean" === Dt(e)
+                                return "boolean" === At(e)
                             }))) return "true" === r
                     }
                     return r
                 }
             }
 
-            function La(e, r) {
+            function Ma(e, r) {
                 return r ? [].slice.call(e.target.options).filter((function(e) {
                     return e.selected
                 })).map((function(e) {
                     return e.value
                 })) : e.target.value
             }
 
-            function Ua(e) {
+            function Va(e) {
                 var r = e.schema,
                     t = e.id,
                     a = e.options,
                     n = e.value,
                     i = e.required,
                     s = e.disabled,
                     u = e.readonly,
@@ -3453,24 +3456,24 @@
                     multiple: l,
                     className: "form-control",
                     value: void 0 === n ? y : n,
                     required: i,
                     disabled: s || u,
                     autoFocus: c,
                     onBlur: f && function(e) {
-                        var a = La(e, l);
-                        f(t, qa(r, a))
+                        var a = Ma(e, l);
+                        f(t, La(r, a))
                     },
                     onFocus: p && function(e) {
-                        var a = La(e, l);
-                        p(t, qa(r, a))
+                        var a = Ma(e, l);
+                        p(t, La(r, a))
                     },
                     onChange: function(e) {
-                        var t = La(e, l);
-                        d(qa(r, t))
+                        var t = Ma(e, l);
+                        d(La(r, t))
                     }
                 }, !l && void 0 === r.default && o().createElement("option", {
                     value: ""
                 }, h), m.map((function(e, r) {
                     var t = e.value,
                         a = e.label,
                         n = v && -1 != v.indexOf(t);
@@ -3478,15 +3481,15 @@
                         key: r,
                         value: t,
                         disabled: n
                     }, a)
                 })))
             }
 
-            function Ma(e) {
+            function za(e) {
                 var r = e.id,
                     t = e.options,
                     a = e.placeholder,
                     n = e.value,
                     i = e.required,
                     s = e.disabled,
                     u = e.readonly,
@@ -3512,48 +3515,48 @@
                     },
                     onChange: function(e) {
                         var r = e.target.value;
                         return c("" === r ? t.emptyValue : r)
                     }
                 })
             }
-            Ua.defaultProps = {
+            Va.defaultProps = {
                 autofocus: !1
-            }, Ma.defaultProps = {
+            }, za.defaultProps = {
                 autofocus: !1,
                 options: {}
             };
-            var Va = {
-                BaseInput: Da,
+            var Ba = {
+                BaseInput: Ca,
                 PasswordWidget: function(e) {
                     var r = e.registry.widgets.BaseInput;
                     return o().createElement(r, qr({
                         type: "password"
                     }, e))
                 },
-                RadioWidget: Na,
+                RadioWidget: qa,
                 UpDownWidget: function(e) {
                     var r = e.registry.widgets.BaseInput;
                     return o().createElement(r, qr({
                         type: "number"
-                    }, e, Jt(e.schema)))
+                    }, e, Zt(e.schema)))
                 },
                 RangeWidget: function(e) {
                     var r = e.schema,
                         t = e.value,
                         a = e.registry.widgets.BaseInput;
                     return o().createElement("div", {
                         className: "field-range-wrapper"
                     }, o().createElement(a, qr({
                         type: "range"
-                    }, e, Jt(r))), o().createElement("span", {
+                    }, e, Zt(r))), o().createElement("span", {
                         className: "range-view"
                     }, t))
                 },
-                SelectWidget: Ua,
+                SelectWidget: Va,
                 TextWidget: function(e) {
                     var r = e.registry.widgets.BaseInput;
                     return o().createElement(r, e)
                 },
                 DateWidget: function(e) {
                     var r = e.onChange,
                         t = e.registry.widgets.BaseInput;
@@ -3568,35 +3571,35 @@
                 DateTimeWidget: function(e) {
                     var r = e.value,
                         t = e.onChange,
                         a = e.registry.widgets.BaseInput;
                     return o().createElement(a, qr({
                         type: "datetime-local"
                     }, e, {
-                        value: Wt(r),
+                        value: Qt(r),
                         onChange: function(e) {
-                            return t(Qt(e))
+                            return t(Ht(e))
                         }
                     }))
                 },
-                AltDateWidget: _a,
-                AltDateTimeWidget: Fa,
+                AltDateWidget: Aa,
+                AltDateTimeWidget: Da,
                 EmailWidget: function(e) {
                     var r = e.registry.widgets.BaseInput;
                     return o().createElement(r, qr({
                         type: "email"
                     }, e))
                 },
                 URLWidget: function(e) {
                     var r = e.registry.widgets.BaseInput;
                     return o().createElement(r, qr({
                         type: "url"
                     }, e))
                 },
-                TextareaWidget: Ma,
+                TextareaWidget: za,
                 HiddenWidget: function(e) {
                     var r = e.id,
                         t = e.value;
                     return o().createElement("input", {
                         type: "hidden",
                         id: r,
                         value: void 0 === t ? "" : t
@@ -3608,40 +3611,40 @@
                         a = e.registry.widgets.BaseInput;
                     return o().createElement(a, qr({
                         type: "color"
                     }, e, {
                         disabled: r || t
                     }))
                 },
-                FileWidget: Ia,
-                CheckboxWidget: Aa,
-                CheckboxesWidget: Ca,
+                FileWidget: Ta,
+                CheckboxWidget: ka,
+                CheckboxesWidget: $a,
                 SubmitButton: function(e) {
                     var r = pt(e.uiSchema),
                         t = r.submitText,
                         a = r.norender,
                         n = r.props;
                     return o().createElement("div", null, !a && o().createElement("button", qr({
                         type: "submit"
                     }, n, {
                         className: "btn btn-info"
                     }), t))
                 }
             };
 
-            function za() {
+            function Wa() {
                 return {
-                    fields: xa,
-                    widgets: Va,
+                    fields: ja,
+                    widgets: Ba,
                     definitions: {},
                     rootSchema: {},
                     formContext: {}
                 }
             }
-            var Ba = function(e) {
+            var Qa = function(e) {
                 function r(r) {
                     var t;
                     return (t = e.call(this, r) || this).getUsedFormData = function(e, r) {
                         if (0 === r.length && "object" != typeof e) return e;
                         var t = Ue(e, r);
                         return Array.isArray(e) ? Object.keys(t).map((function(e) {
                             return t[e]
@@ -3656,27 +3659,27 @@
                                     t[n].__rjsf_additionalProperties && "" !== t[n].$name ? a.push(t[n].$name) : e(t[n], a, i)
                                 } else "$name" === n && "" !== t[n] && o.forEach((function(e) {
                                     e = e.replace(/^\./, "");
                                     var t = function(e, r, t) {
                                         var a = null == e ? void 0 : le(e, r);
                                         return void 0 === a ? t : a
                                     }(r, e);
-                                    ("object" != typeof t || hr(t)) && a.push(e)
+                                    ("object" != typeof t || pr(t)) && a.push(e)
                                 }))
                             })), a
                         }(e)
                     }, t.onChange = function(e, r) {
                         (mt(e) || Array.isArray(e)) && (e = t.getStateFromProps(t.props, e).formData);
                         var a = !t.props.noValidate && t.props.liveValidate,
                             o = {
                                 formData: e
                             },
                             n = e;
                         if (!0 === t.props.omitExtraData && !0 === t.props.liveOmit) {
-                            var i = Vt($t(t.state.schema, t.state.schema, e), "", t.state.schema, e),
+                            var i = zt(Rt(t.state.schema, t.state.schema, e), "", t.state.schema, e),
                                 s = t.getFieldNames(i, e);
                             o = {
                                 formData: n = t.getUsedFormData(e, s)
                             }
                         }
                         if (a) {
                             var u = t.validate(n),
@@ -3709,15 +3712,15 @@
                         var e;
                         t.props.onFocus && (e = t.props).onFocus.apply(e, arguments)
                     }, t.onSubmit = function(e) {
                         if (e.preventDefault(), e.target === e.currentTarget) {
                             e.persist();
                             var r, a, o = t.state.formData;
                             if (!0 === t.props.omitExtraData) {
-                                var n = Vt($t(t.state.schema, t.state.schema, o), "", t.state.schema, o),
+                                var n = zt(Rt(t.state.schema, t.state.schema, o), "", t.state.schema, o),
                                     i = t.getFieldNames(n, o);
                                 o = t.getUsedFormData(o, i)
                             }
                             if (!t.props.noValidate) {
                                 var s = t.validate(o),
                                     u = s.errors,
                                     l = s.errorSchema,
@@ -3743,29 +3746,29 @@
                                     formData: o,
                                     status: "submitted"
                                 }), e)
                             }))
                         }
                     }, t.state = t.getStateFromProps(r, r.formData), t.props.onChange && !Lt(t.state.formData, t.props.formData) && t.props.onChange(t.state), t.formElement = null, t
                 }
-                Lr(r, e);
+                Ur(r, e);
                 var t = r.prototype;
                 return t.UNSAFE_componentWillReceiveProps = function(e) {
                     var r = this.getStateFromProps(e, e.formData);
                     Lt(r.formData, e.formData) || Lt(r.formData, this.state.formData) || !this.props.onChange || this.props.onChange(r), this.setState(r)
                 }, t.getStateFromProps = function(e, r) {
                     var t, a, o, n, i = this.state || {},
                         s = "schema" in e ? e.schema : this.props.schema,
                         u = "uiSchema" in e ? e.uiSchema : this.props.uiSchema,
                         l = void 0 !== r,
                         c = "liveValidate" in e ? e.liveValidate : this.props.liveValidate,
                         d = l && !e.noValidate && c,
                         f = s,
                         p = ct(s, r, f),
-                        h = $t(s, f, p),
+                        h = Rt(s, f, p),
                         m = e.customFormats,
                         v = e.additionalMetaSchemas;
                     if (d) {
                         var y = this.validate(p, s, v, m);
                         o = t = y.errors, n = a = y.errorSchema
                     } else {
                         var g = e.noValidate ? {
@@ -3780,30 +3783,30 @@
                         };
                         t = g.errors, a = g.errorSchema, o = i.schemaValidationErrors, n = i.schemaValidationErrorSchema
                     }
                     e.extraErrors && (t = Yr(a = vt(a, e.extraErrors, !0)));
                     var b = {
                         schema: s,
                         uiSchema: u,
-                        idSchema: Mt(h, u["ui:rootFieldId"], f, p, e.idPrefix, e.idSeparator),
+                        idSchema: Vt(h, u["ui:rootFieldId"], f, p, e.idPrefix, e.idSeparator),
                         formData: p,
                         edit: l,
                         errors: t,
                         errorSchema: a,
                         additionalMetaSchemas: v
                     };
                     return o && (b.schemaValidationErrors = o, b.schemaValidationErrorSchema = n), b
                 }, t.shouldComponentUpdate = function(e, r) {
-                    return Ut(this, e, r)
+                    return Mt(this, e, r)
                 }, t.validate = function(e, r, t, a) {
                     void 0 === r && (r = this.props.schema), void 0 === t && (t = this.props.additionalMetaSchemas), void 0 === a && (a = this.props.customFormats);
                     var o = this.props,
                         n = o.validate,
                         i = o.transformErrors;
-                    return et(e, $t(r, this.getRegistry().rootSchema, e), n, i, t, a)
+                    return et(e, Rt(r, this.getRegistry().rootSchema, e), n, i, t, a)
                 }, t.renderErrors = function() {
                     var e = this.state,
                         r = e.errors,
                         t = e.errorSchema,
                         a = e.schema,
                         n = e.uiSchema,
                         i = this.props,
@@ -3814,15 +3817,15 @@
                         errors: r,
                         errorSchema: t,
                         schema: a,
                         uiSchema: n,
                         formContext: l
                     }) : null
                 }, t.getRegistry = function() {
-                    var e = za(),
+                    var e = Wa(),
                         r = e.fields,
                         t = e.widgets;
                     return {
                         fields: qr({}, r, this.props.fields),
                         widgets: qr({}, t, this.props.widgets),
                         ArrayFieldTemplate: this.props.ArrayFieldTemplate,
                         ObjectFieldTemplate: this.props.ObjectFieldTemplate,
@@ -3860,16 +3863,16 @@
                         w = this.state,
                         S = w.schema,
                         x = w.uiSchema,
                         O = w.formData,
                         j = w.errorSchema,
                         _ = w.idSchema,
                         F = this.getRegistry(),
-                        D = F.fields.SchemaField,
-                        A = P ? u : void 0,
+                        A = F.fields.SchemaField,
+                        D = P ? u : void 0,
                         C = P || u || "form",
                         k = F.widgets.SubmitButton;
                     p && console.warn("Using autocomplete property of Form is deprecated, use autoComplete instead.");
                     var $ = h || p;
                     return o().createElement(C, {
                         className: s || "rjsf",
                         id: a,
@@ -3878,19 +3881,19 @@
                         target: d,
                         action: f,
                         autoComplete: $,
                         encType: m,
                         acceptCharset: v,
                         noValidate: y,
                         onSubmit: this.onSubmit,
-                        as: A,
+                        as: D,
                         ref: function(r) {
                             e.formElement = r
                         }
-                    }, this.renderErrors(), o().createElement(D, {
+                    }, this.renderErrors(), o().createElement(A, {
                         schema: S,
                         uiSchema: x,
                         errorSchema: j,
                         idSchema: _,
                         idPrefix: n,
                         idSeparator: i,
                         formContext: E,
@@ -3903,27 +3906,27 @@
                         readonly: b
                     }), t || o().createElement(k, {
                         uiSchema: x
                     }))
                 }, r
             }(a.Component);
 
-            function Wa(e) {
+            function Ha(e) {
                 return (0, a.forwardRef)((function(r, t) {
                     var a = r.fields,
                         n = r.widgets,
                         i = Mr(r, ["fields", "widgets"]);
-                    return a = qr({}, e.fields, a), n = qr({}, e.widgets, n), o().createElement(Ba, qr({}, e, i, {
+                    return a = qr({}, e.fields, a), n = qr({}, e.widgets, n), o().createElement(Qa, qr({}, e, i, {
                         fields: a,
                         widgets: n,
                         ref: t
                     }))
                 }))
             }
-            Ba.defaultProps = {
+            Qa.defaultProps = {
                 uiSchema: {},
                 noValidate: !1,
                 liveValidate: !1,
                 disabled: !1,
                 readonly: !1,
                 noHtml5Validate: !1,
                 ErrorList: function(e) {
@@ -3940,34 +3943,34 @@
                         return o().createElement("li", {
                             key: r,
                             className: "list-group-item text-danger"
                         }, e.stack)
                     }))))
                 },
                 omitExtraData: !1
-            }, Wa.propTypes = {
+            }, Ha.propTypes = {
                 widgets: i().object,
                 fields: i().object
             };
-            var Qa = qr({}, Gt, {
-                getDefaultRegistry: za
+            var Ka = qr({}, Xt, {
+                getDefaultRegistry: Wa
             });
-            const Ha = Ba
+            const Ja = Qa
         },
-        5096: (e, r, t) => {
+        233: (e, r, t) => {
             "use strict";
-            var a = t(7153),
-                o = t(3610),
-                n = t(7531),
-                i = t(4022),
+            var a = t(8362),
+                o = t(1817),
+                n = t(7580),
+                i = t(4414),
                 s = t(5035),
-                u = t(1516),
-                l = t(7753),
-                c = t(3978),
-                d = t(2889);
+                u = t(7488),
+                l = t(2197),
+                c = t(8548),
+                d = t(666);
             e.exports = y, y.prototype.validate = function(e, r) {
                 var t;
                 if ("string" == typeof e) {
                     if (!(t = this.getSchema(e))) throw new Error('no schema with key or ref "' + e + '"')
                 } else {
                     var a = this._addSchema(e);
                     t = a.validate || this._compile(a)
@@ -4088,18 +4091,18 @@
                 return e.validate = o, e.refs = o.refs, e.refVal = o.refVal, e.root = o.root, o;
 
                 function n() {
                     var r = e.validate,
                         t = r.apply(this, arguments);
                     return n.errors = r.errors, t
                 }
-            }, y.prototype.compileAsync = t(2931);
-            var f = t(4895);
+            }, y.prototype.compileAsync = t(5077);
+            var f = t(6041);
             y.prototype.addKeyword = f.add, y.prototype.getKeyword = f.get, y.prototype.removeKeyword = f.remove, y.prototype.validateKeyword = f.validate;
-            var p = t(7802);
+            var p = t(8989);
             y.ValidationError = p.Validation, y.MissingRefError = p.MissingRef, y.$dataMetaSchema = c;
             var h = "http://json-schema.org/draft-07/schema",
                 m = ["removeAdditional", "useDefaults", "coerceTypes", "strictDefaults"],
                 v = ["/properties"];
 
             function y(e) {
                 if (!(this instanceof y)) return new y(e);
@@ -4136,16 +4139,16 @@
                         for (var r in e._opts.keywords) {
                             var t = e._opts.keywords[r];
                             e.addKeyword(r, t)
                         }
                     }(this),
                     function(e) {
                         var r;
-                        if (e._opts.$data && (r = t(894), e.addMetaSchema(r, r.$id, !0)), !1 !== e._opts.meta) {
-                            var a = t(6680);
+                        if (e._opts.$data && (r = t(6354), e.addMetaSchema(r, r.$id, !0)), !1 !== e._opts.meta) {
+                            var a = t(6656);
                             e._opts.$data && (a = c(a, v)), e.addMetaSchema(a, h, !0), e._refs["http://json-schema.org/schema"] = h
                         }
                     }(this), "object" == typeof e.meta && this.addMetaSchema(e.meta), e.nullable && this.addKeyword("nullable", {
                         metaSchema: {
                             type: "boolean"
                         }
                     }),
@@ -4184,32 +4187,32 @@
 
             function S(e, r) {
                 if (e._schemas[r] || e._refs[r]) throw new Error('schema with key or id "' + r + '" already exists')
             }
 
             function x() {}
         },
-        7531: e => {
+        7580: e => {
             "use strict";
             var r = e.exports = function() {
                 this._cache = {}
             };
             r.prototype.put = function(e, r) {
                 this._cache[e] = r
             }, r.prototype.get = function(e) {
                 return this._cache[e]
             }, r.prototype.del = function(e) {
                 delete this._cache[e]
             }, r.prototype.clear = function() {
                 this._cache = {}
             }
         },
-        2931: (e, r, t) => {
+        5077: (e, r, t) => {
             "use strict";
-            var a = t(7802).MissingRef;
+            var a = t(8989).MissingRef;
             e.exports = function e(r, t, o) {
                 var n = this;
                 if ("function" != typeof this._opts.loadSchema) throw new Error("options.loadSchema should be a function");
                 "function" == typeof t && (o = t, t = void 0);
                 var i = s(r).then((function() {
                     var e = n._addSchema(r, void 0, t);
                     return e.validate || u(e)
@@ -4250,17 +4253,17 @@
                             }
                         }(r);
                         throw r
                     }
                 }
             }
         },
-        7802: (e, r, t) => {
+        8989: (e, r, t) => {
             "use strict";
-            var a = t(3610);
+            var a = t(1817);
 
             function o(e, r, t) {
                 this.message = t || o.message(e, r), this.missingRef = a.url(e, r), this.missingSchema = a.normalizeId(a.fullPath(this.missingRef))
             }
 
             function n(e) {
                 return e.prototype = Object.create(Error.prototype), e.prototype.constructor = e, e
@@ -4270,17 +4273,17 @@
                     this.message = "validation failed", this.errors = e, this.ajv = this.validation = !0
                 })),
                 MissingRef: n(o)
             }, o.message = function(e, r) {
                 return "can't resolve reference " + r + " from id " + e
             }
         },
-        1516: (e, r, t) => {
+        7488: (e, r, t) => {
             "use strict";
-            var a = t(2889),
+            var a = t(666),
                 o = /^(\d\d\d\d)-(\d\d)-(\d\d)$/,
                 n = [0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31],
                 i = /^(\d\d):(\d\d):(\d\d)(\.\d+)?(z|[+-]\d\d(?::?\d\d)?)?$/i,
                 s = /^(?=.{1,253}\.?$)[a-z0-9](?:[a-z0-9-]{0,61}[a-z0-9])?(?:\.[a-z0-9](?:[-0-9a-z]{0,61}[0-9a-z])?)*\.?$/i,
                 u = /^(?:[a-z][a-z0-9+\-.]*:)(?:\/?\/(?:(?:[a-z0-9\-._~!$&'()*+,;=:]|%[0-9a-f]{2})*@)?(?:\[(?:(?:(?:(?:[0-9a-f]{1,4}:){6}|::(?:[0-9a-f]{1,4}:){5}|(?:[0-9a-f]{1,4})?::(?:[0-9a-f]{1,4}:){4}|(?:(?:[0-9a-f]{1,4}:){0,1}[0-9a-f]{1,4})?::(?:[0-9a-f]{1,4}:){3}|(?:(?:[0-9a-f]{1,4}:){0,2}[0-9a-f]{1,4})?::(?:[0-9a-f]{1,4}:){2}|(?:(?:[0-9a-f]{1,4}:){0,3}[0-9a-f]{1,4})?::[0-9a-f]{1,4}:|(?:(?:[0-9a-f]{1,4}:){0,4}[0-9a-f]{1,4})?::)(?:[0-9a-f]{1,4}:[0-9a-f]{1,4}|(?:(?:25[0-5]|2[0-4]\d|[01]?\d\d?)\.){3}(?:25[0-5]|2[0-4]\d|[01]?\d\d?))|(?:(?:[0-9a-f]{1,4}:){0,5}[0-9a-f]{1,4})?::[0-9a-f]{1,4}|(?:(?:[0-9a-f]{1,4}:){0,6}[0-9a-f]{1,4})?::)|[Vv][0-9a-f]+\.[a-z0-9\-._~!$&'()*+,;=:]+)\]|(?:(?:25[0-5]|2[0-4]\d|[01]?\d\d?)\.){3}(?:25[0-5]|2[0-4]\d|[01]?\d\d?)|(?:[a-z0-9\-._~!$&'()*+,;=]|%[0-9a-f]{2})*)(?::\d*)?(?:\/(?:[a-z0-9\-._~!$&'()*+,;=:@]|%[0-9a-f]{2})*)*|\/(?:(?:[a-z0-9\-._~!$&'()*+,;=:@]|%[0-9a-f]{2})+(?:\/(?:[a-z0-9\-._~!$&'()*+,;=:@]|%[0-9a-f]{2})*)*)?|(?:[a-z0-9\-._~!$&'()*+,;=:@]|%[0-9a-f]{2})+(?:\/(?:[a-z0-9\-._~!$&'()*+,;=:@]|%[0-9a-f]{2})*)*)(?:\?(?:[a-z0-9\-._~!$&'()*+,;=:@/?]|%[0-9a-f]{2})*)?(?:#(?:[a-z0-9\-._~!$&'()*+,;=:@/?]|%[0-9a-f]{2})*)?$/i,
                 l = /^(?:(?:[^\x00-\x20"'<>%\\^`{|}]|%[0-9a-f]{2})|\{[+#./;?&=,!@|]?(?:[a-z0-9_]|%[0-9a-f]{2})+(?::[1-9][0-9]{0,3}|\*)?(?:,(?:[a-z0-9_]|%[0-9a-f]{2})+(?::[1-9][0-9]{0,3}|\*)?)*\})*$/i,
                 c = /^(?:(?:http[s\u017F]?|ftp):\/\/)(?:(?:[\0-\x08\x0E-\x1F!-\x9F\xA1-\u167F\u1681-\u1FFF\u200B-\u2027\u202A-\u202E\u2030-\u205E\u2060-\u2FFF\u3001-\uD7FF\uE000-\uFEFE\uFF00-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])+(?::(?:[\0-\x08\x0E-\x1F!-\x9F\xA1-\u167F\u1681-\u1FFF\u200B-\u2027\u202A-\u202E\u2030-\u205E\u2060-\u2FFF\u3001-\uD7FF\uE000-\uFEFE\uFF00-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])*)?@)?(?:(?!10(?:\.[0-9]{1,3}){3})(?!127(?:\.[0-9]{1,3}){3})(?!169\.254(?:\.[0-9]{1,3}){2})(?!192\.168(?:\.[0-9]{1,3}){2})(?!172\.(?:1[6-9]|2[0-9]|3[01])(?:\.[0-9]{1,3}){2})(?:[1-9][0-9]?|1[0-9][0-9]|2[01][0-9]|22[0-3])(?:\.(?:1?[0-9]{1,2}|2[0-4][0-9]|25[0-5])){2}(?:\.(?:[1-9][0-9]?|1[0-9][0-9]|2[0-4][0-9]|25[0-4]))|(?:(?:(?:[0-9a-z\xA1-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])+-)*(?:[0-9a-z\xA1-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])+)(?:\.(?:(?:[0-9a-z\xA1-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])+-)*(?:[0-9a-z\xA1-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])+)*(?:\.(?:(?:[a-z\xA1-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF]){2,})))(?::[0-9]{2,5})?(?:\/(?:[\0-\x08\x0E-\x1F!-\x9F\xA1-\u167F\u1681-\u1FFF\u200B-\u2027\u202A-\u202E\u2030-\u205E\u2060-\u2FFF\u3001-\uD7FF\uE000-\uFEFE\uFF00-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])*)?$/i,
@@ -4362,21 +4365,21 @@
                 try {
                     return new RegExp(e), !0
                 } catch (e) {
                     return !1
                 }
             }
         },
-        7153: (e, r, t) => {
+        8362: (e, r, t) => {
             "use strict";
-            var a = t(3610),
-                o = t(2889),
-                n = t(7802),
+            var a = t(1817),
+                o = t(666),
+                n = t(8989),
                 i = t(5035),
-                s = t(9508),
+                s = t(8787),
                 u = o.ucs2length,
                 l = t(4063),
                 c = n.Validation;
 
             function d(e, r, t) {
                 var a = p.call(this, e, r, t);
                 return a >= 0 ? {
@@ -4437,27 +4440,27 @@
                     _ = {},
                     F = [];
                 t = t || {
                     schema: r,
                     refVal: w,
                     refs: S
                 };
-                var D = d.call(this, r, t, b),
-                    A = this._compilations[D.index];
-                if (D.compiling) return A.callValidate = function e() {
-                    var r = A.validate,
+                var A = d.call(this, r, t, b),
+                    D = this._compilations[A.index];
+                if (A.compiling) return D.callValidate = function e() {
+                    var r = D.validate,
                         t = r.apply(this, arguments);
                     return e.errors = r.errors, t
                 };
                 var C = this._formats,
                     k = this.RULES;
                 try {
                     var $ = I(r, t, p, b);
-                    A.validate = $;
-                    var R = A.callValidate;
+                    D.validate = $;
+                    var R = D.callValidate;
                     return R && (R.schema = $.schema, R.errors = null, R.refs = $.refs, R.refVal = $.refVal, R.root = $.root, R.$async = $.$async, P.sourceCode && (R.source = $.source)), $
                 } finally {
                     f.call(this, r, t, b)
                 }
 
                 function I(r, i, d, f) {
                     var p = !i || i && i.schema == r;
@@ -4474,16 +4477,16 @@
                             errorPath: '""',
                             MissingRefError: n.MissingRef,
                             RULES: k,
                             validate: s,
                             util: o,
                             resolve: a,
                             resolveRef: N,
-                            usePattern: L,
-                            useDefault: U,
+                            usePattern: U,
+                            useDefault: L,
                             useCustomRule: M,
                             opts: P,
                             formats: C,
                             logger: E.logger,
                             self: E
                         });
                     _ = g(w, v) + g(x, h) + g(j, m) + g(F, y) + _, P.processCode && (_ = P.processCode(_, r));
@@ -4534,20 +4537,20 @@
                         inline: !0
                     } : {
                         code: r,
                         $async: e && !!e.$async
                     }
                 }
 
-                function L(e) {
+                function U(e) {
                     var r = O[e];
                     return void 0 === r && (r = O[e] = x.length, x[r] = e), "pattern" + r
                 }
 
-                function U(e) {
+                function L(e) {
                     switch (typeof e) {
                         case "boolean":
                         case "number":
                             return "" + e;
                         case "string":
                             return o.toQuotedString(e);
                         case "object":
@@ -4583,21 +4586,21 @@
                     return F[d] = s, {
                         code: "customRule" + d,
                         validate: s
                     }
                 }
             }
         },
-        3610: (e, r, t) => {
+        1817: (e, r, t) => {
             "use strict";
             var a = t(540),
                 o = t(4063),
-                n = t(2889),
-                i = t(4022),
-                s = t(9461);
+                n = t(666),
+                i = t(4414),
+                s = t(3393);
 
             function u(e, r, t) {
                 var a = this._refs[t];
                 if ("string" == typeof a) {
                     if (!this._refs[a]) return u.call(this, e, r, a);
                     a = this._refs[a]
                 }
@@ -4741,18 +4744,18 @@
                 return e ? e.replace(b, "") : ""
             }
 
             function P(e, r) {
                 return r = E(r), a.resolve(e, r)
             }
         },
-        7753: (e, r, t) => {
+        2197: (e, r, t) => {
             "use strict";
-            var a = t(6674),
-                o = t(2889).toHash;
+            var a = t(4029),
+                o = t(666).toHash;
             e.exports = function() {
                 var e = [{
                         type: "number",
                         rules: [{
                             maximum: ["exclusiveMaximum"]
                         }, {
                             minimum: ["exclusiveMinimum"]
@@ -4789,29 +4792,29 @@
                     })), e.all.$comment = {
                         keyword: "$comment",
                         code: a.$comment
                     }, t.type && (e.types[t.type] = t)
                 })), e.keywords = o(r.concat(["$schema", "$id", "id", "$data", "$async", "title", "description", "default", "definitions", "examples", "readOnly", "writeOnly", "contentMediaType", "contentEncoding", "additionalItems", "then", "else"])), e.custom = {}, e
             }
         },
-        4022: (e, r, t) => {
+        4414: (e, r, t) => {
             "use strict";
-            var a = t(2889);
+            var a = t(666);
             e.exports = function(e) {
                 a.copy(e, this)
             }
         },
-        4442: e => {
+        103: e => {
             "use strict";
             e.exports = function(e) {
                 for (var r, t = 0, a = e.length, o = 0; o < a;) t++, (r = e.charCodeAt(o++)) >= 55296 && r <= 56319 && o < a && 56320 == (64512 & (r = e.charCodeAt(o))) && o++;
                 return t
             }
         },
-        2889: (e, r, t) => {
+        666: (e, r, t) => {
             "use strict";
 
             function a(e, r, t, a) {
                 var o = a ? " !== " : " === ",
                     n = a ? " || " : " && ",
                     i = a ? "!" : "",
                     s = a ? "" : "!";
@@ -4855,15 +4858,15 @@
                         if ("array" === e && "array" === r) return ["array"]
                     }
                 },
                 toHash: n,
                 getProperty: u,
                 escapeQuotes: l,
                 equal: t(4063),
-                ucs2length: t(4442),
+                ucs2length: t(103),
                 varOccurences: function(e, r) {
                     r += "[^0-9]";
                     var t = e.match(new RegExp(r, "g"));
                     return t ? t.length : 0
                 },
                 varReplace: function(e, r, t) {
                     return r += "([^0-9])", t = t.replace(/\$/g, "$$$$"), e.replace(new RegExp(r, "g"), t + "$1")
@@ -4951,15 +4954,15 @@
                 return e.replace(/~/g, "~0").replace(/\//g, "~1")
             }
 
             function m(e) {
                 return e.replace(/~1/g, "/").replace(/~0/g, "~")
             }
         },
-        3978: e => {
+        8548: e => {
             "use strict";
             var r = ["multipleOf", "maximum", "exclusiveMaximum", "minimum", "exclusiveMinimum", "maxLength", "minLength", "pattern", "additionalItems", "maxItems", "minItems", "uniqueItems", "maxProperties", "minProperties", "required", "additionalProperties", "enum", "format", "const"];
             e.exports = function(e, t) {
                 for (var a = 0; a < t.length; a++) {
                     e = JSON.parse(JSON.stringify(e));
                     var o, n = t[a].split("/"),
                         i = e;
@@ -4973,17 +4976,17 @@
                             }]
                         })
                     }
                 }
                 return e
             }
         },
-        1128: (e, r, t) => {
+        7321: (e, r, t) => {
             "use strict";
-            var a = t(6680);
+            var a = t(6656);
             e.exports = {
                 $id: "https://github.com/ajv-validator/ajv/blob/master/lib/definition_schema.js",
                 definitions: {
                     simpleTypes: a.definitions.simpleTypes
                 },
                 type: "object",
                 dependencies: {
@@ -5031,15 +5034,15 @@
                         }, {
                             const: "full"
                         }]
                     }
                 }
             }
         },
-        8210: e => {
+        3939: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a, o = " ",
                     n = e.level,
                     i = e.dataLevel,
                     s = e.schema[r],
                     u = e.schemaPath + e.util.getProperty(r),
@@ -5069,15 +5072,15 @@
                 } else if (O = y, (x = "number" == typeof m) && f) {
                     var _ = "'" + O + "'";
                     o += " if ( ", f && (o += " (" + a + " !== undefined && typeof " + a + " != 'number') || "), o += " ( " + a + " === undefined || " + m + " " + y + "= " + a + " ? " + d + " " + g + "= " + m + " : " + d + " " + g + " " + a + " ) || " + d + " !== " + d + ") { "
                 } else x && void 0 === s ? (w = !0, b = h, l = e.errSchemaPath + "/" + h, a = m, g += "=") : (x && (a = Math[p ? "min" : "max"](m, s)), m === (!x || a) ? (w = !0, b = h, l = e.errSchemaPath + "/" + h, g += "=") : (w = !1, O += "=")), _ = "'" + O + "'", o += " if ( ", f && (o += " (" + a + " !== undefined && typeof " + a + " != 'number') || "), o += " " + d + " " + g + " " + a + " || " + d + " !== " + d + ") { ";
                 return b = b || r, (E = E || []).push(o), o = "", !1 !== e.createErrors ? (o += " { keyword: '" + (b || "_limit") + "' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(l) + " , params: { comparison: " + _ + ", limit: " + a + ", exclusive: " + w + " } ", !1 !== e.opts.messages && (o += " , message: 'should be " + O + " ", o += f ? "' + " + a : a + "'"), e.opts.verbose && (o += " , schema:  ", o += f ? "validate.schema" + u : "" + s, o += "         , parentSchema: validate.schema" + e.schemaPath + " , data: " + d + " "), o += " } ") : o += " {} ", j = o, o = E.pop(), !e.compositeRule && c ? e.async ? o += " throw new ValidationError([" + j + "]); " : o += " validate.errors = [" + j + "]; return false; " : o += " var err = " + j + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", o += " } ", c && (o += " else { "), o
             }
         },
-        3038: e => {
+        5264: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a, o = " ",
                     n = e.level,
                     i = e.dataLevel,
                     s = e.schema[r],
                     u = e.schemaPath + e.util.getProperty(r),
@@ -5090,15 +5093,15 @@
                 var p = r,
                     h = h || [];
                 h.push(o), o = "", !1 !== e.createErrors ? (o += " { keyword: '" + (p || "_limitItems") + "' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(l) + " , params: { limit: " + a + " } ", !1 !== e.opts.messages && (o += " , message: 'should NOT have ", o += "maxItems" == r ? "more" : "fewer", o += " than ", o += f ? "' + " + a + " + '" : "" + s, o += " items' "), e.opts.verbose && (o += " , schema:  ", o += f ? "validate.schema" + u : "" + s, o += "         , parentSchema: validate.schema" + e.schemaPath + " , data: " + d + " "), o += " } ") : o += " {} ";
                 var m = o;
                 return o = h.pop(), !e.compositeRule && c ? e.async ? o += " throw new ValidationError([" + m + "]); " : o += " validate.errors = [" + m + "]; return false; " : o += " var err = " + m + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", o += "} ", c && (o += " else { "), o
             }
         },
-        425: e => {
+        9921: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a, o = " ",
                     n = e.level,
                     i = e.dataLevel,
                     s = e.schema[r],
                     u = e.schemaPath + e.util.getProperty(r),
@@ -5112,15 +5115,15 @@
                 var h = r,
                     m = m || [];
                 m.push(o), o = "", !1 !== e.createErrors ? (o += " { keyword: '" + (h || "_limitLength") + "' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(l) + " , params: { limit: " + a + " } ", !1 !== e.opts.messages && (o += " , message: 'should NOT be ", o += "maxLength" == r ? "longer" : "shorter", o += " than ", o += f ? "' + " + a + " + '" : "" + s, o += " characters' "), e.opts.verbose && (o += " , schema:  ", o += f ? "validate.schema" + u : "" + s, o += "         , parentSchema: validate.schema" + e.schemaPath + " , data: " + d + " "), o += " } ") : o += " {} ";
                 var v = o;
                 return o = m.pop(), !e.compositeRule && c ? e.async ? o += " throw new ValidationError([" + v + "]); " : o += " validate.errors = [" + v + "]; return false; " : o += " var err = " + v + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", o += "} ", c && (o += " else { "), o
             }
         },
-        8204: e => {
+        9530: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a, o = " ",
                     n = e.level,
                     i = e.dataLevel,
                     s = e.schema[r],
                     u = e.schemaPath + e.util.getProperty(r),
@@ -5133,15 +5136,15 @@
                 var p = r,
                     h = h || [];
                 h.push(o), o = "", !1 !== e.createErrors ? (o += " { keyword: '" + (p || "_limitProperties") + "' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(l) + " , params: { limit: " + a + " } ", !1 !== e.opts.messages && (o += " , message: 'should NOT have ", o += "maxProperties" == r ? "more" : "fewer", o += " than ", o += f ? "' + " + a + " + '" : "" + s, o += " properties' "), e.opts.verbose && (o += " , schema:  ", o += f ? "validate.schema" + u : "" + s, o += "         , parentSchema: validate.schema" + e.schemaPath + " , data: " + d + " "), o += " } ") : o += " {} ";
                 var m = o;
                 return o = h.pop(), !e.compositeRule && c ? e.async ? o += " throw new ValidationError([" + m + "]); " : o += " validate.errors = [" + m + "]; return false; " : o += " var err = " + m + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", o += "} ", c && (o += " else { "), o
             }
         },
-        2988: e => {
+        7292: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.schema[r],
                     n = e.schemaPath + e.util.getProperty(r),
                     i = e.errSchemaPath + "/" + r,
                     s = !e.opts.allErrors,
@@ -5153,15 +5156,15 @@
                     f = !0,
                     p = o;
                 if (p)
                     for (var h, m = -1, v = p.length - 1; m < v;) h = p[m += 1], (e.opts.strictKeywords ? "object" == typeof h && Object.keys(h).length > 0 || !1 === h : e.util.schemaHasRules(h, e.RULES.all)) && (f = !1, u.schema = h, u.schemaPath = n + "[" + m + "]", u.errSchemaPath = i + "/" + m, a += "  " + e.validate(u) + " ", u.baseId = d, s && (a += " if (" + c + ") { ", l += "}"));
                 return s && (a += f ? " if (true) { " : " " + l.slice(0, -1) + " "), a
             }
         },
-        9996: e => {
+        5198: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5186,25 +5189,25 @@
                     if (b)
                         for (var E, P = -1, w = b.length - 1; P < w;) E = b[P += 1], p.schema = E, p.schemaPath = s + "[" + P + "]", p.errSchemaPath = u + "/" + P, a += "  " + e.validate(p) + " ", p.baseId = y, a += " " + d + " = " + d + " || " + m + "; if (!" + d + ") { ", h += "}";
                     e.compositeRule = p.compositeRule = g, a += " " + h + " if (!" + d + ") {   var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'anyOf' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: {} ", !1 !== e.opts.messages && (a += " , message: 'should match some schema in anyOf' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", !e.compositeRule && l && (e.async ? a += " throw new ValidationError(vErrors); " : a += " validate.errors = vErrors; return false; "), a += " } else {  errors = " + f + "; if (vErrors !== null) { if (" + f + ") vErrors.length = " + f + "; else vErrors = null; } ", e.opts.allErrors && (a += " } ")
                 } else l && (a += " if (true) { ");
                 return a
             }
         },
-        7812: e => {
+        4804: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.schema[r],
                     n = e.errSchemaPath + "/" + r,
                     i = (e.opts.allErrors, e.util.toQuotedString(o));
                 return !0 === e.opts.$comment ? a += " console.log(" + i + ");" : "function" == typeof e.opts.$comment && (a += " self._opts.$comment(" + i + ", " + e.util.toQuotedString(n) + ", validate.root.schema);"), a
             }
         },
-        5306: e => {
+        521: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5216,15 +5219,15 @@
                 f && (a += " var schema" + o + " = " + e.util.getData(i.$data, n, e.dataPathArr) + "; "), f || (a += " var schema" + o + " = validate.schema" + s + ";"), a += "var " + d + " = equal(" + c + ", schema" + o + "); if (!" + d + ") {   ";
                 var p = p || [];
                 p.push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'const' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { allowedValue: schema" + o + " } ", !1 !== e.opts.messages && (a += " , message: 'should be equal to constant' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ";
                 var h = a;
                 return a = p.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + h + "]); " : a += " validate.errors = [" + h + "]; return false; " : a += " var err = " + h + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", a += " }", l && (a += " else { "), a
             }
         },
-        2840: e => {
+        976: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5251,15 +5254,15 @@
                 } else a += " if (" + c + ".length == 0) {";
                 var S = S || [];
                 S.push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'contains' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: {} ", !1 !== e.opts.messages && (a += " , message: 'should contain a valid item' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ";
                 var x = a;
                 return a = S.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + x + "]); " : a += " validate.errors = [" + x + "]; return false; " : a += " var err = " + x + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", a += " } else { ", b && (a += "  errors = " + f + "; if (vErrors !== null) { if (" + f + ") vErrors.length = " + f + "; else vErrors = null; } "), e.opts.allErrors && (a += " } "), a
             }
         },
-        4165: e => {
+        5203: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a, o, n = " ",
                     i = e.level,
                     s = e.dataLevel,
                     u = e.schema[r],
                     l = e.schemaPath + e.util.getProperty(r),
@@ -5281,46 +5284,46 @@
                 } else {
                     if (!(b = e.useCustomRule(P, u, e.schema, e))) return;
                     o = "validate.schema" + l, E = b.code, v = S.compile, y = S.inline, g = S.macro
                 }
                 var j = E + ".errors",
                     _ = "i" + i,
                     F = "ruleErr" + i,
-                    D = S.async;
-                if (D && !e.async) throw new Error("async keyword in sync schema");
+                    A = S.async;
+                if (A && !e.async) throw new Error("async keyword in sync schema");
                 if (y || g || (n += j + " = null;"), n += "var " + h + " = errors;var " + p + ";", m && S.$data && (x += "}", n += " if (" + o + " === undefined) { " + p + " = true; } else { ", O && (x += "}", n += " " + p + " = " + w + ".validateSchema(" + o + "); if (" + p + ") { ")), y) S.statements ? n += " " + b.validate + " " : n += " " + p + " = " + b.validate + "; ";
                 else if (g) {
-                    var A = e.util.copy(e);
-                    x = "", A.level++;
-                    var C = "valid" + A.level;
-                    A.schema = b.validate, A.schemaPath = "";
+                    var D = e.util.copy(e);
+                    x = "", D.level++;
+                    var C = "valid" + D.level;
+                    D.schema = b.validate, D.schemaPath = "";
                     var k = e.compositeRule;
-                    e.compositeRule = A.compositeRule = !0;
-                    var $ = e.validate(A).replace(/validate\.schema/g, E);
-                    e.compositeRule = A.compositeRule = k, n += " " + $
+                    e.compositeRule = D.compositeRule = !0;
+                    var $ = e.validate(D).replace(/validate\.schema/g, E);
+                    e.compositeRule = D.compositeRule = k, n += " " + $
                 } else {
                     (T = T || []).push(n), n = "", n += "  " + E + ".call( ", e.opts.passContext ? n += "this" : n += "self", v || !1 === S.schema ? n += " , " + f + " " : n += " , " + o + " , " + f + " , validate.schema" + e.schemaPath + " ", n += " , (dataPath || '')", '""' != e.errorPath && (n += " + " + e.errorPath);
                     var R = s ? "data" + (s - 1 || "") : "parentData",
                         I = s ? e.dataPathArr[s] : "parentDataProperty",
                         N = n += " , " + R + " , " + I + " , rootData )  ";
-                    n = T.pop(), !1 === S.errors ? (n += " " + p + " = ", D && (n += "await "), n += N + "; ") : n += D ? " var " + (j = "customErrors" + i) + " = null; try { " + p + " = await " + N + "; } catch (e) { " + p + " = false; if (e instanceof ValidationError) " + j + " = e.errors; else throw e; } " : " " + j + " = null; " + p + " = " + N + "; "
+                    n = T.pop(), !1 === S.errors ? (n += " " + p + " = ", A && (n += "await "), n += N + "; ") : n += A ? " var " + (j = "customErrors" + i) + " = null; try { " + p + " = await " + N + "; } catch (e) { " + p + " = false; if (e instanceof ValidationError) " + j + " = e.errors; else throw e; } " : " " + j + " = null; " + p + " = " + N + "; "
                 }
                 if (S.modifying && (n += " if (" + R + ") " + f + " = " + R + "[" + I + "];"), n += "" + x, S.valid) d && (n += " if (true) { ");
                 else {
                     var T;
                     n += " if ( ", void 0 === S.valid ? (n += " !", n += g ? "" + C : "" + p) : n += " " + !S.valid + " ", n += ") { ", a = P.keyword, (T = T || []).push(n), n = "", (T = T || []).push(n), n = "", !1 !== e.createErrors ? (n += " { keyword: '" + (a || "custom") + "' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(c) + " , params: { keyword: '" + P.keyword + "' } ", !1 !== e.opts.messages && (n += " , message: 'should pass \"" + P.keyword + "\" keyword validation' "), e.opts.verbose && (n += " , schema: validate.schema" + l + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + f + " "), n += " } ") : n += " {} ";
                     var q = n;
                     n = T.pop(), !e.compositeRule && d ? e.async ? n += " throw new ValidationError([" + q + "]); " : n += " validate.errors = [" + q + "]; return false; " : n += " var err = " + q + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ";
-                    var L = n;
-                    n = T.pop(), y ? S.errors ? "full" != S.errors && (n += "  for (var " + _ + "=" + h + "; " + _ + "<errors; " + _ + "++) { var " + F + " = vErrors[" + _ + "]; if (" + F + ".dataPath === undefined) " + F + ".dataPath = (dataPath || '') + " + e.errorPath + "; if (" + F + ".schemaPath === undefined) { " + F + '.schemaPath = "' + c + '"; } ', e.opts.verbose && (n += " " + F + ".schema = " + o + "; " + F + ".data = " + f + "; "), n += " } ") : !1 === S.errors ? n += " " + L + " " : (n += " if (" + h + " == errors) { " + L + " } else {  for (var " + _ + "=" + h + "; " + _ + "<errors; " + _ + "++) { var " + F + " = vErrors[" + _ + "]; if (" + F + ".dataPath === undefined) " + F + ".dataPath = (dataPath || '') + " + e.errorPath + "; if (" + F + ".schemaPath === undefined) { " + F + '.schemaPath = "' + c + '"; } ', e.opts.verbose && (n += " " + F + ".schema = " + o + "; " + F + ".data = " + f + "; "), n += " } } ") : g ? (n += "   var err =   ", !1 !== e.createErrors ? (n += " { keyword: '" + (a || "custom") + "' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(c) + " , params: { keyword: '" + P.keyword + "' } ", !1 !== e.opts.messages && (n += " , message: 'should pass \"" + P.keyword + "\" keyword validation' "), e.opts.verbose && (n += " , schema: validate.schema" + l + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + f + " "), n += " } ") : n += " {} ", n += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", !e.compositeRule && d && (e.async ? n += " throw new ValidationError(vErrors); " : n += " validate.errors = vErrors; return false; ")) : !1 === S.errors ? n += " " + L + " " : (n += " if (Array.isArray(" + j + ")) { if (vErrors === null) vErrors = " + j + "; else vErrors = vErrors.concat(" + j + "); errors = vErrors.length;  for (var " + _ + "=" + h + "; " + _ + "<errors; " + _ + "++) { var " + F + " = vErrors[" + _ + "]; if (" + F + ".dataPath === undefined) " + F + ".dataPath = (dataPath || '') + " + e.errorPath + ";  " + F + '.schemaPath = "' + c + '";  ', e.opts.verbose && (n += " " + F + ".schema = " + o + "; " + F + ".data = " + f + "; "), n += " } } else { " + L + " } "), n += " } ", d && (n += " else { ")
+                    var U = n;
+                    n = T.pop(), y ? S.errors ? "full" != S.errors && (n += "  for (var " + _ + "=" + h + "; " + _ + "<errors; " + _ + "++) { var " + F + " = vErrors[" + _ + "]; if (" + F + ".dataPath === undefined) " + F + ".dataPath = (dataPath || '') + " + e.errorPath + "; if (" + F + ".schemaPath === undefined) { " + F + '.schemaPath = "' + c + '"; } ', e.opts.verbose && (n += " " + F + ".schema = " + o + "; " + F + ".data = " + f + "; "), n += " } ") : !1 === S.errors ? n += " " + U + " " : (n += " if (" + h + " == errors) { " + U + " } else {  for (var " + _ + "=" + h + "; " + _ + "<errors; " + _ + "++) { var " + F + " = vErrors[" + _ + "]; if (" + F + ".dataPath === undefined) " + F + ".dataPath = (dataPath || '') + " + e.errorPath + "; if (" + F + ".schemaPath === undefined) { " + F + '.schemaPath = "' + c + '"; } ', e.opts.verbose && (n += " " + F + ".schema = " + o + "; " + F + ".data = " + f + "; "), n += " } } ") : g ? (n += "   var err =   ", !1 !== e.createErrors ? (n += " { keyword: '" + (a || "custom") + "' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(c) + " , params: { keyword: '" + P.keyword + "' } ", !1 !== e.opts.messages && (n += " , message: 'should pass \"" + P.keyword + "\" keyword validation' "), e.opts.verbose && (n += " , schema: validate.schema" + l + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + f + " "), n += " } ") : n += " {} ", n += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", !e.compositeRule && d && (e.async ? n += " throw new ValidationError(vErrors); " : n += " validate.errors = vErrors; return false; ")) : !1 === S.errors ? n += " " + U + " " : (n += " if (Array.isArray(" + j + ")) { if (vErrors === null) vErrors = " + j + "; else vErrors = vErrors.concat(" + j + "); errors = vErrors.length;  for (var " + _ + "=" + h + "; " + _ + "<errors; " + _ + "++) { var " + F + " = vErrors[" + _ + "]; if (" + F + ".dataPath === undefined) " + F + ".dataPath = (dataPath || '') + " + e.errorPath + ";  " + F + '.schemaPath = "' + c + '";  ', e.opts.verbose && (n += " " + F + ".schema = " + o + "; " + F + ".data = " + f + "; "), n += " } } else { " + U + " } "), n += " } ", d && (n += " else { ")
                 }
                 return n
             }
         },
-        6659: e => {
+        4548: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5344,42 +5347,42 @@
                 var E = e.errorPath;
                 for (var P in a += "var missing" + o + ";", v)
                     if ((b = v[P]).length) {
                         if (a += " if ( " + c + e.util.getProperty(P) + " !== undefined ", y && (a += " && Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(P) + "') "), l) {
                             a += " && ( ";
                             var w = b;
                             if (w)
-                                for (var S = -1, x = w.length - 1; S < x;) A = w[S += 1], S && (a += " || "), a += " ( ( " + (R = c + ($ = e.util.getProperty(A))) + " === undefined ", y && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(A) + "') "), a += ") && (missing" + o + " = " + e.util.toQuotedString(e.opts.jsonPointers ? A : $) + ") ) ";
+                                for (var S = -1, x = w.length - 1; S < x;) D = w[S += 1], S && (a += " || "), a += " ( ( " + (R = c + ($ = e.util.getProperty(D))) + " === undefined ", y && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(D) + "') "), a += ") && (missing" + o + " = " + e.util.toQuotedString(e.opts.jsonPointers ? D : $) + ") ) ";
                             a += ")) {  ";
                             var O = "missing" + o,
                                 j = "' + " + O + " + '";
                             e.opts._errorDataPathProperty && (e.errorPath = e.opts.jsonPointers ? e.util.getPathExpr(E, O, !0) : E + " + " + O);
                             var _ = _ || [];
                             _.push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'dependencies' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { property: '" + e.util.escapeQuotes(P) + "', missingProperty: '" + j + "', depsCount: " + b.length + ", deps: '" + e.util.escapeQuotes(1 == b.length ? b[0] : b.join(", ")) + "' } ", !1 !== e.opts.messages && (a += " , message: 'should have ", 1 == b.length ? a += "property " + e.util.escapeQuotes(b[0]) : a += "properties " + e.util.escapeQuotes(b.join(", ")), a += " when property " + e.util.escapeQuotes(P) + " is present' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ";
                             var F = a;
                             a = _.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + F + "]); " : a += " validate.errors = [" + F + "]; return false; " : a += " var err = " + F + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; "
                         } else {
                             a += " ) { ";
-                            var D = b;
-                            if (D)
-                                for (var A, C = -1, k = D.length - 1; C < k;) {
-                                    A = D[C += 1];
-                                    var $ = e.util.getProperty(A),
-                                        R = (j = e.util.escapeQuotes(A), c + $);
-                                    e.opts._errorDataPathProperty && (e.errorPath = e.util.getPath(E, A, e.opts.jsonPointers)), a += " if ( " + R + " === undefined ", y && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(A) + "') "), a += ") {  var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'dependencies' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { property: '" + e.util.escapeQuotes(P) + "', missingProperty: '" + j + "', depsCount: " + b.length + ", deps: '" + e.util.escapeQuotes(1 == b.length ? b[0] : b.join(", ")) + "' } ", !1 !== e.opts.messages && (a += " , message: 'should have ", 1 == b.length ? a += "property " + e.util.escapeQuotes(b[0]) : a += "properties " + e.util.escapeQuotes(b.join(", ")), a += " when property " + e.util.escapeQuotes(P) + " is present' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; } "
+                            var A = b;
+                            if (A)
+                                for (var D, C = -1, k = A.length - 1; C < k;) {
+                                    D = A[C += 1];
+                                    var $ = e.util.getProperty(D),
+                                        R = (j = e.util.escapeQuotes(D), c + $);
+                                    e.opts._errorDataPathProperty && (e.errorPath = e.util.getPath(E, D, e.opts.jsonPointers)), a += " if ( " + R + " === undefined ", y && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(D) + "') "), a += ") {  var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'dependencies' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { property: '" + e.util.escapeQuotes(P) + "', missingProperty: '" + j + "', depsCount: " + b.length + ", deps: '" + e.util.escapeQuotes(1 == b.length ? b[0] : b.join(", ")) + "' } ", !1 !== e.opts.messages && (a += " , message: 'should have ", 1 == b.length ? a += "property " + e.util.escapeQuotes(b[0]) : a += "properties " + e.util.escapeQuotes(b.join(", ")), a += " when property " + e.util.escapeQuotes(P) + " is present' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; } "
                                 }
                         }
                         a += " }   ", l && (p += "}", a += " else { ")
                     } e.errorPath = E;
                 var I = f.baseId;
                 for (var P in m) g = m[P], (e.opts.strictKeywords ? "object" == typeof g && Object.keys(g).length > 0 || !1 === g : e.util.schemaHasRules(g, e.RULES.all)) && (a += " " + h + " = true; if ( " + c + e.util.getProperty(P) + " !== undefined ", y && (a += " && Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(P) + "') "), a += ") { ", f.schema = g, f.schemaPath = s + e.util.getProperty(P), f.errSchemaPath = u + "/" + e.util.escapeFragment(P), a += "  " + e.validate(f) + " ", f.baseId = I, a += " }  ", l && (a += " if (" + h + ") { ", p += "}"));
                 return l && (a += "   " + p + " if (" + d + " == errors) {"), a
             }
         },
-        1740: e => {
+        4143: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5394,15 +5397,15 @@
                 f || (a += " var " + h + " = validate.schema" + s + ";"), a += "var " + d + ";", f && (a += " if (schema" + o + " === undefined) " + d + " = true; else if (!Array.isArray(schema" + o + ")) " + d + " = false; else {"), a += d + " = false;for (var " + p + "=0; " + p + "<" + h + ".length; " + p + "++) if (equal(" + c + ", " + h + "[" + p + "])) { " + d + " = true; break; }", f && (a += "  }  "), a += " if (!" + d + ") {   ";
                 var m = m || [];
                 m.push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'enum' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { allowedValues: schema" + o + " } ", !1 !== e.opts.messages && (a += " , message: 'should be equal to one of the allowed values' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ";
                 var v = a;
                 return a = m.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + v + "]); " : a += " validate.errors = [" + v + "]; return false; " : a += " var err = " + v + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", a += " }", l && (a += " else { "), a
             }
         },
-        9014: e => {
+        9413: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5439,15 +5442,15 @@
                 }
                 var E = E || [];
                 E.push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'format' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { format:  ", a += f ? "" + d : "" + e.util.toQuotedString(i), a += "  } ", !1 !== e.opts.messages && (a += " , message: 'should match format \"", a += f ? "' + " + d + " + '" : "" + e.util.escapeQuotes(i), a += "\"' "), e.opts.verbose && (a += " , schema:  ", a += f ? "validate.schema" + s : "" + e.util.toQuotedString(i), a += "         , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ";
                 var P = a;
                 return a = E.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + P + "]); " : a += " validate.errors = [" + P + "]; return false; " : a += " var err = " + P + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", a += " } ", l && (a += " else { "), a
             }
         },
-        7231: e => {
+        7372: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5469,48 +5472,48 @@
                     p.createErrors = !1, p.schema = i, p.schemaPath = s, p.errSchemaPath = u, a += " var " + f + " = errors; var " + d + " = true;  ";
                     var P = e.compositeRule;
                     e.compositeRule = p.compositeRule = !0, a += "  " + e.validate(p) + " ", p.baseId = b, p.createErrors = !0, a += "  errors = " + f + "; if (vErrors !== null) { if (" + f + ") vErrors.length = " + f + "; else vErrors = null; }  ", e.compositeRule = p.compositeRule = P, y ? (a += " if (" + h + ") {  ", p.schema = e.schema.then, p.schemaPath = e.schemaPath + ".then", p.errSchemaPath = e.errSchemaPath + "/then", a += "  " + e.validate(p) + " ", p.baseId = b, a += " " + d + " = " + h + "; ", y && g ? a += " var " + (E = "ifClause" + o) + " = 'then'; " : E = "'then'", a += " } ", g && (a += " else { ")) : a += " if (!" + h + ") { ", g && (p.schema = e.schema.else, p.schemaPath = e.schemaPath + ".else", p.errSchemaPath = e.errSchemaPath + "/else", a += "  " + e.validate(p) + " ", p.baseId = b, a += " " + d + " = " + h + "; ", y && g ? a += " var " + (E = "ifClause" + o) + " = 'else'; " : E = "'else'", a += " } "), a += " if (!" + d + ") {   var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'if' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { failingKeyword: " + E + " } ", !1 !== e.opts.messages && (a += " , message: 'should match \"' + " + E + " + '\" schema' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", !e.compositeRule && l && (e.async ? a += " throw new ValidationError(vErrors); " : a += " validate.errors = vErrors; return false; "), a += " }   ", l && (a += " else { ")
                 } else l && (a += " if (true) { ");
                 return a
             }
         },
-        6674: (e, r, t) => {
+        4029: (e, r, t) => {
             "use strict";
             e.exports = {
-                $ref: t(2392),
-                allOf: t(2988),
-                anyOf: t(9996),
-                $comment: t(7812),
-                const: t(5306),
-                contains: t(2840),
-                dependencies: t(6659),
-                enum: t(1740),
-                format: t(9014),
-                if: t(7231),
-                items: t(7482),
-                maximum: t(8210),
-                minimum: t(8210),
-                maxItems: t(3038),
-                minItems: t(3038),
-                maxLength: t(425),
-                minLength: t(425),
-                maxProperties: t(8204),
-                minProperties: t(8204),
-                multipleOf: t(3673),
-                not: t(8528),
-                oneOf: t(9709),
-                pattern: t(9614),
-                properties: t(1175),
-                propertyNames: t(8441),
-                required: t(1287),
-                uniqueItems: t(3603),
-                validate: t(9508)
+                $ref: t(5686),
+                allOf: t(7292),
+                anyOf: t(5198),
+                $comment: t(4804),
+                const: t(521),
+                contains: t(976),
+                dependencies: t(4548),
+                enum: t(4143),
+                format: t(9413),
+                if: t(7372),
+                items: t(6319),
+                maximum: t(3939),
+                minimum: t(3939),
+                maxItems: t(5264),
+                minItems: t(5264),
+                maxLength: t(9921),
+                minLength: t(9921),
+                maxProperties: t(9530),
+                minProperties: t(9530),
+                multipleOf: t(7682),
+                not: t(6608),
+                oneOf: t(2796),
+                pattern: t(8968),
+                properties: t(574),
+                propertyNames: t(5073),
+                required: t(2843),
+                uniqueItems: t(5737),
+                validate: t(8787)
             }
         },
-        7482: e => {
+        6319: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5541,23 +5544,23 @@
                     var x = i;
                     if (x)
                         for (var O, j = -1, _ = x.length - 1; j < _;)
                             if (O = x[j += 1], e.opts.strictKeywords ? "object" == typeof O && Object.keys(O).length > 0 || !1 === O : e.util.schemaHasRules(O, e.RULES.all)) {
                                 a += " " + m + " = true; if (" + c + ".length > " + j + ") { ";
                                 var F = c + "[" + j + "]";
                                 p.schema = O, p.schemaPath = s + "[" + j + "]", p.errSchemaPath = u + "/" + j, p.errorPath = e.util.getPathExpr(e.errorPath, j, e.opts.jsonPointers, !0), p.dataPathArr[y] = j;
-                                var D = e.validate(p);
-                                p.baseId = b, e.util.varOccurences(D, g) < 2 ? a += " " + e.util.varReplace(D, g, F) + " " : a += " var " + g + " = " + F + "; " + D + " ", a += " }  ", l && (a += " if (" + m + ") { ", h += "}")
+                                var A = e.validate(p);
+                                p.baseId = b, e.util.varOccurences(A, g) < 2 ? a += " " + e.util.varReplace(A, g, F) + " " : a += " var " + g + " = " + F + "; " + A + " ", a += " }  ", l && (a += " if (" + m + ") { ", h += "}")
                             }
-                    "object" == typeof E && (e.opts.strictKeywords ? "object" == typeof E && Object.keys(E).length > 0 || !1 === E : e.util.schemaHasRules(E, e.RULES.all)) && (p.schema = E, p.schemaPath = e.schemaPath + ".additionalItems", p.errSchemaPath = e.errSchemaPath + "/additionalItems", a += " " + m + " = true; if (" + c + ".length > " + i.length + ") {  for (var " + v + " = " + i.length + "; " + v + " < " + c + ".length; " + v + "++) { ", p.errorPath = e.util.getPathExpr(e.errorPath, v, e.opts.jsonPointers, !0), F = c + "[" + v + "]", p.dataPathArr[y] = v, D = e.validate(p), p.baseId = b, e.util.varOccurences(D, g) < 2 ? a += " " + e.util.varReplace(D, g, F) + " " : a += " var " + g + " = " + F + "; " + D + " ", l && (a += " if (!" + m + ") break; "), a += " } }  ", l && (a += " if (" + m + ") { ", h += "}"))
-                } else(e.opts.strictKeywords ? "object" == typeof i && Object.keys(i).length > 0 || !1 === i : e.util.schemaHasRules(i, e.RULES.all)) && (p.schema = i, p.schemaPath = s, p.errSchemaPath = u, a += "  for (var " + v + " = 0; " + v + " < " + c + ".length; " + v + "++) { ", p.errorPath = e.util.getPathExpr(e.errorPath, v, e.opts.jsonPointers, !0), F = c + "[" + v + "]", p.dataPathArr[y] = v, D = e.validate(p), p.baseId = b, e.util.varOccurences(D, g) < 2 ? a += " " + e.util.varReplace(D, g, F) + " " : a += " var " + g + " = " + F + "; " + D + " ", l && (a += " if (!" + m + ") break; "), a += " }");
+                    "object" == typeof E && (e.opts.strictKeywords ? "object" == typeof E && Object.keys(E).length > 0 || !1 === E : e.util.schemaHasRules(E, e.RULES.all)) && (p.schema = E, p.schemaPath = e.schemaPath + ".additionalItems", p.errSchemaPath = e.errSchemaPath + "/additionalItems", a += " " + m + " = true; if (" + c + ".length > " + i.length + ") {  for (var " + v + " = " + i.length + "; " + v + " < " + c + ".length; " + v + "++) { ", p.errorPath = e.util.getPathExpr(e.errorPath, v, e.opts.jsonPointers, !0), F = c + "[" + v + "]", p.dataPathArr[y] = v, A = e.validate(p), p.baseId = b, e.util.varOccurences(A, g) < 2 ? a += " " + e.util.varReplace(A, g, F) + " " : a += " var " + g + " = " + F + "; " + A + " ", l && (a += " if (!" + m + ") break; "), a += " } }  ", l && (a += " if (" + m + ") { ", h += "}"))
+                } else(e.opts.strictKeywords ? "object" == typeof i && Object.keys(i).length > 0 || !1 === i : e.util.schemaHasRules(i, e.RULES.all)) && (p.schema = i, p.schemaPath = s, p.errSchemaPath = u, a += "  for (var " + v + " = 0; " + v + " < " + c + ".length; " + v + "++) { ", p.errorPath = e.util.getPathExpr(e.errorPath, v, e.opts.jsonPointers, !0), F = c + "[" + v + "]", p.dataPathArr[y] = v, A = e.validate(p), p.baseId = b, e.util.varOccurences(A, g) < 2 ? a += " " + e.util.varReplace(A, g, F) + " " : a += " var " + g + " = " + F + "; " + A + " ", l && (a += " if (!" + m + ") break; "), a += " }");
                 return l && (a += " " + h + " if (" + f + " == errors) {"), a
             }
         },
-        3673: e => {
+        7682: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a, o = " ",
                     n = e.level,
                     i = e.dataLevel,
                     s = e.schema[r],
                     u = e.schemaPath + e.util.getProperty(r),
@@ -5569,15 +5572,15 @@
                 o += "var division" + n + ";if (", f && (o += " " + a + " !== undefined && ( typeof " + a + " != 'number' || "), o += " (division" + n + " = " + d + " / " + a + ", ", e.opts.multipleOfPrecision ? o += " Math.abs(Math.round(division" + n + ") - division" + n + ") > 1e-" + e.opts.multipleOfPrecision + " " : o += " division" + n + " !== parseInt(division" + n + ") ", o += " ) ", f && (o += "  )  "), o += " ) {   ";
                 var p = p || [];
                 p.push(o), o = "", !1 !== e.createErrors ? (o += " { keyword: 'multipleOf' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(l) + " , params: { multipleOf: " + a + " } ", !1 !== e.opts.messages && (o += " , message: 'should be multiple of ", o += f ? "' + " + a : a + "'"), e.opts.verbose && (o += " , schema:  ", o += f ? "validate.schema" + u : "" + s, o += "         , parentSchema: validate.schema" + e.schemaPath + " , data: " + d + " "), o += " } ") : o += " {} ";
                 var h = o;
                 return o = p.pop(), !e.compositeRule && c ? e.async ? o += " throw new ValidationError([" + h + "]); " : o += " validate.errors = [" + h + "]; return false; " : o += " var err = " + h + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", o += "} ", c && (o += " else { "), o
             }
         },
-        8528: e => {
+        6608: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5596,15 +5599,15 @@
                     v.push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'not' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: {} ", !1 !== e.opts.messages && (a += " , message: 'should NOT be valid' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ";
                     var y = a;
                     a = v.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + y + "]); " : a += " validate.errors = [" + y + "]; return false; " : a += " var err = " + y + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", a += " } else {  errors = " + d + "; if (vErrors !== null) { if (" + d + ") vErrors.length = " + d + "; else vErrors = null; } ", e.opts.allErrors && (a += " } ")
                 } else a += "  var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'not' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: {} ", !1 !== e.opts.messages && (a += " , message: 'should NOT be valid' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", l && (a += " if (false) { ");
                 return a
             }
         },
-        9709: e => {
+        2796: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5625,15 +5628,15 @@
                 e.compositeRule = p.compositeRule = !0;
                 var E = i;
                 if (E)
                     for (var P, w = -1, S = E.length - 1; w < S;) P = E[w += 1], (e.opts.strictKeywords ? "object" == typeof P && Object.keys(P).length > 0 || !1 === P : e.util.schemaHasRules(P, e.RULES.all)) ? (p.schema = P, p.schemaPath = s + "[" + w + "]", p.errSchemaPath = u + "/" + w, a += "  " + e.validate(p) + " ", p.baseId = v) : a += " var " + m + " = true; ", w && (a += " if (" + m + " && " + y + ") { " + d + " = false; " + g + " = [" + g + ", " + w + "]; } else { ", h += "}"), a += " if (" + m + ") { " + d + " = " + y + " = true; " + g + " = " + w + "; }";
                 return e.compositeRule = p.compositeRule = b, a += h + "if (!" + d + ") {   var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'oneOf' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { passingSchemas: " + g + " } ", !1 !== e.opts.messages && (a += " , message: 'should match exactly one schema in oneOf' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", !e.compositeRule && l && (e.async ? a += " throw new ValidationError(vErrors); " : a += " validate.errors = vErrors; return false; "), a += "} else {  errors = " + f + "; if (vErrors !== null) { if (" + f + ") vErrors.length = " + f + "; else vErrors = null; }", e.opts.allErrors && (a += " } "), a
             }
         },
-        9614: e => {
+        8968: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a, o = " ",
                     n = e.level,
                     i = e.dataLevel,
                     s = e.schema[r],
                     u = e.schemaPath + e.util.getProperty(r),
@@ -5644,15 +5647,15 @@
                 f ? (o += " var schema" + n + " = " + e.util.getData(s.$data, i, e.dataPathArr) + "; ", a = "schema" + n) : a = s, o += "if ( ", f && (o += " (" + a + " !== undefined && typeof " + a + " != 'string') || "), o += " !" + (f ? "(new RegExp(" + a + "))" : e.usePattern(s)) + ".test(" + d + ") ) {   ";
                 var p = p || [];
                 p.push(o), o = "", !1 !== e.createErrors ? (o += " { keyword: 'pattern' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(l) + " , params: { pattern:  ", o += f ? "" + a : "" + e.util.toQuotedString(s), o += "  } ", !1 !== e.opts.messages && (o += " , message: 'should match pattern \"", o += f ? "' + " + a + " + '" : "" + e.util.escapeQuotes(s), o += "\"' "), e.opts.verbose && (o += " , schema:  ", o += f ? "validate.schema" + u : "" + e.util.toQuotedString(s), o += "         , parentSchema: validate.schema" + e.schemaPath + " , data: " + d + " "), o += " } ") : o += " {} ";
                 var h = o;
                 return o = p.pop(), !e.compositeRule && c ? e.async ? o += " throw new ValidationError([" + h + "]); " : o += " validate.errors = [" + h + "]; return false; " : o += " var err = " + h + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", o += "} ", c && (o += " else { "), o
             }
         },
-        1175: e => {
+        574: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5674,40 +5677,40 @@
                     w = Object.keys(P).filter($),
                     S = e.schema.additionalProperties,
                     x = E.length || w.length,
                     O = !1 === S,
                     j = "object" == typeof S && Object.keys(S).length,
                     _ = e.opts.removeAdditional,
                     F = O || j || _,
-                    D = e.opts.ownProperties,
-                    A = e.baseId,
+                    A = e.opts.ownProperties,
+                    D = e.baseId,
                     C = e.schema.required;
                 if (C && (!e.opts.$data || !C.$data) && C.length < e.opts.loopRequired) var k = e.util.toHash(C);
 
                 function $(e) {
                     return "__proto__" !== e
                 }
-                if (a += "var " + d + " = errors;var " + h + " = true;", D && (a += " var " + b + " = undefined;"), F) {
-                    if (a += D ? " " + b + " = " + b + " || Object.keys(" + c + "); for (var " + v + "=0; " + v + "<" + b + ".length; " + v + "++) { var " + m + " = " + b + "[" + v + "]; " : " for (var " + m + " in " + c + ") { ", x) {
+                if (a += "var " + d + " = errors;var " + h + " = true;", A && (a += " var " + b + " = undefined;"), F) {
+                    if (a += A ? " " + b + " = " + b + " || Object.keys(" + c + "); for (var " + v + "=0; " + v + "<" + b + ".length; " + v + "++) { var " + m + " = " + b + "[" + v + "]; " : " for (var " + m + " in " + c + ") { ", x) {
                         if (a += " var isAdditional" + o + " = !(false ", E.length)
                             if (E.length > 8) a += " || validate.schema" + s + ".hasOwnProperty(" + m + ") ";
                             else {
                                 var R = E;
                                 if (R)
                                     for (var I = -1, N = R.length - 1; I < N;) J = R[I += 1], a += " || " + m + " == " + e.util.toQuotedString(J) + " "
                             } if (w.length) {
                             var T = w;
                             if (T)
-                                for (var q = -1, L = T.length - 1; q < L;) ne = T[q += 1], a += " || " + e.usePattern(ne) + ".test(" + m + ") "
+                                for (var q = -1, U = T.length - 1; q < U;) ne = T[q += 1], a += " || " + e.usePattern(ne) + ".test(" + m + ") "
                         }
                         a += " ); if (isAdditional" + o + ") { "
                     }
                     if ("all" == _) a += " delete " + c + "[" + m + "]; ";
                     else {
-                        var U = e.errorPath,
+                        var L = e.errorPath,
                             M = "' + " + m + " + '";
                         if (e.opts._errorDataPathProperty && (e.errorPath = e.util.getPathExpr(e.errorPath, m, e.opts.jsonPointers)), O)
                             if (_) a += " delete " + c + "[" + m + "]; ";
                             else {
                                 a += " " + h + " = false; ";
                                 var V = u;
                                 u = e.errSchemaPath + "/additionalProperties", (te = te || []).push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'additionalProperties' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { additionalProperty: '" + M + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is an invalid additional property" : a += "should NOT have additional properties", a += "' "), e.opts.verbose && (a += " , schema: false , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ";
@@ -5718,55 +5721,55 @@
                             if ("failing" == _) {
                                 a += " var " + d + " = errors;  ";
                                 var B = e.compositeRule;
                                 e.compositeRule = f.compositeRule = !0, f.schema = S, f.schemaPath = e.schemaPath + ".additionalProperties", f.errSchemaPath = e.errSchemaPath + "/additionalProperties", f.errorPath = e.opts._errorDataPathProperty ? e.errorPath : e.util.getPathExpr(e.errorPath, m, e.opts.jsonPointers);
                                 var W = c + "[" + m + "]";
                                 f.dataPathArr[y] = m;
                                 var Q = e.validate(f);
-                                f.baseId = A, e.util.varOccurences(Q, g) < 2 ? a += " " + e.util.varReplace(Q, g, W) + " " : a += " var " + g + " = " + W + "; " + Q + " ", a += " if (!" + h + ") { errors = " + d + "; if (validate.errors !== null) { if (errors) validate.errors.length = errors; else validate.errors = null; } delete " + c + "[" + m + "]; }  ", e.compositeRule = f.compositeRule = B
-                            } else f.schema = S, f.schemaPath = e.schemaPath + ".additionalProperties", f.errSchemaPath = e.errSchemaPath + "/additionalProperties", f.errorPath = e.opts._errorDataPathProperty ? e.errorPath : e.util.getPathExpr(e.errorPath, m, e.opts.jsonPointers), W = c + "[" + m + "]", f.dataPathArr[y] = m, Q = e.validate(f), f.baseId = A, e.util.varOccurences(Q, g) < 2 ? a += " " + e.util.varReplace(Q, g, W) + " " : a += " var " + g + " = " + W + "; " + Q + " ", l && (a += " if (!" + h + ") break; ");
-                        e.errorPath = U
+                                f.baseId = D, e.util.varOccurences(Q, g) < 2 ? a += " " + e.util.varReplace(Q, g, W) + " " : a += " var " + g + " = " + W + "; " + Q + " ", a += " if (!" + h + ") { errors = " + d + "; if (validate.errors !== null) { if (errors) validate.errors.length = errors; else validate.errors = null; } delete " + c + "[" + m + "]; }  ", e.compositeRule = f.compositeRule = B
+                            } else f.schema = S, f.schemaPath = e.schemaPath + ".additionalProperties", f.errSchemaPath = e.errSchemaPath + "/additionalProperties", f.errorPath = e.opts._errorDataPathProperty ? e.errorPath : e.util.getPathExpr(e.errorPath, m, e.opts.jsonPointers), W = c + "[" + m + "]", f.dataPathArr[y] = m, Q = e.validate(f), f.baseId = D, e.util.varOccurences(Q, g) < 2 ? a += " " + e.util.varReplace(Q, g, W) + " " : a += " var " + g + " = " + W + "; " + Q + " ", l && (a += " if (!" + h + ") break; ");
+                        e.errorPath = L
                     }
                     x && (a += " } "), a += " }  ", l && (a += " if (" + h + ") { ", p += "}")
                 }
                 var H = e.opts.useDefaults && !e.compositeRule;
                 if (E.length) {
                     var K = E;
                     if (K)
                         for (var J, Z = -1, Y = K.length - 1; Z < Y;) {
                             var G = i[J = K[Z += 1]];
                             if (e.opts.strictKeywords ? "object" == typeof G && Object.keys(G).length > 0 || !1 === G : e.util.schemaHasRules(G, e.RULES.all)) {
                                 var X = e.util.getProperty(J),
                                     ee = (W = c + X, H && void 0 !== G.default);
-                                if (f.schema = G, f.schemaPath = s + X, f.errSchemaPath = u + "/" + e.util.escapeFragment(J), f.errorPath = e.util.getPath(e.errorPath, J, e.opts.jsonPointers), f.dataPathArr[y] = e.util.toQuotedString(J), Q = e.validate(f), f.baseId = A, e.util.varOccurences(Q, g) < 2) {
+                                if (f.schema = G, f.schemaPath = s + X, f.errSchemaPath = u + "/" + e.util.escapeFragment(J), f.errorPath = e.util.getPath(e.errorPath, J, e.opts.jsonPointers), f.dataPathArr[y] = e.util.toQuotedString(J), Q = e.validate(f), f.baseId = D, e.util.varOccurences(Q, g) < 2) {
                                     Q = e.util.varReplace(Q, g, W);
                                     var re = W
                                 } else re = g, a += " var " + g + " = " + W + "; ";
                                 if (ee) a += " " + Q + " ";
                                 else {
                                     if (k && k[J]) {
-                                        a += " if ( " + re + " === undefined ", D && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(J) + "') "), a += ") { " + h + " = false; ", U = e.errorPath, V = u;
+                                        a += " if ( " + re + " === undefined ", A && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(J) + "') "), a += ") { " + h + " = false; ", L = e.errorPath, V = u;
                                         var te, ae = e.util.escapeQuotes(J);
-                                        e.opts._errorDataPathProperty && (e.errorPath = e.util.getPath(U, J, e.opts.jsonPointers)), u = e.errSchemaPath + "/required", (te = te || []).push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + ae + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + ae + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", z = a, a = te.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + z + "]); " : a += " validate.errors = [" + z + "]; return false; " : a += " var err = " + z + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", u = V, e.errorPath = U, a += " } else { "
-                                    } else l ? (a += " if ( " + re + " === undefined ", D && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(J) + "') "), a += ") { " + h + " = true; } else { ") : (a += " if (" + re + " !== undefined ", D && (a += " &&   Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(J) + "') "), a += " ) { ");
+                                        e.opts._errorDataPathProperty && (e.errorPath = e.util.getPath(L, J, e.opts.jsonPointers)), u = e.errSchemaPath + "/required", (te = te || []).push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + ae + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + ae + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", z = a, a = te.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + z + "]); " : a += " validate.errors = [" + z + "]; return false; " : a += " var err = " + z + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", u = V, e.errorPath = L, a += " } else { "
+                                    } else l ? (a += " if ( " + re + " === undefined ", A && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(J) + "') "), a += ") { " + h + " = true; } else { ") : (a += " if (" + re + " !== undefined ", A && (a += " &&   Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(J) + "') "), a += " ) { ");
                                     a += " " + Q + " } "
                                 }
                             }
                             l && (a += " if (" + h + ") { ", p += "}")
                         }
                 }
                 if (w.length) {
                     var oe = w;
                     if (oe)
-                        for (var ne, ie = -1, se = oe.length - 1; ie < se;) G = P[ne = oe[ie += 1]], (e.opts.strictKeywords ? "object" == typeof G && Object.keys(G).length > 0 || !1 === G : e.util.schemaHasRules(G, e.RULES.all)) && (f.schema = G, f.schemaPath = e.schemaPath + ".patternProperties" + e.util.getProperty(ne), f.errSchemaPath = e.errSchemaPath + "/patternProperties/" + e.util.escapeFragment(ne), a += D ? " " + b + " = " + b + " || Object.keys(" + c + "); for (var " + v + "=0; " + v + "<" + b + ".length; " + v + "++) { var " + m + " = " + b + "[" + v + "]; " : " for (var " + m + " in " + c + ") { ", a += " if (" + e.usePattern(ne) + ".test(" + m + ")) { ", f.errorPath = e.util.getPathExpr(e.errorPath, m, e.opts.jsonPointers), W = c + "[" + m + "]", f.dataPathArr[y] = m, Q = e.validate(f), f.baseId = A, e.util.varOccurences(Q, g) < 2 ? a += " " + e.util.varReplace(Q, g, W) + " " : a += " var " + g + " = " + W + "; " + Q + " ", l && (a += " if (!" + h + ") break; "), a += " } ", l && (a += " else " + h + " = true; "), a += " }  ", l && (a += " if (" + h + ") { ", p += "}"))
+                        for (var ne, ie = -1, se = oe.length - 1; ie < se;) G = P[ne = oe[ie += 1]], (e.opts.strictKeywords ? "object" == typeof G && Object.keys(G).length > 0 || !1 === G : e.util.schemaHasRules(G, e.RULES.all)) && (f.schema = G, f.schemaPath = e.schemaPath + ".patternProperties" + e.util.getProperty(ne), f.errSchemaPath = e.errSchemaPath + "/patternProperties/" + e.util.escapeFragment(ne), a += A ? " " + b + " = " + b + " || Object.keys(" + c + "); for (var " + v + "=0; " + v + "<" + b + ".length; " + v + "++) { var " + m + " = " + b + "[" + v + "]; " : " for (var " + m + " in " + c + ") { ", a += " if (" + e.usePattern(ne) + ".test(" + m + ")) { ", f.errorPath = e.util.getPathExpr(e.errorPath, m, e.opts.jsonPointers), W = c + "[" + m + "]", f.dataPathArr[y] = m, Q = e.validate(f), f.baseId = D, e.util.varOccurences(Q, g) < 2 ? a += " " + e.util.varReplace(Q, g, W) + " " : a += " var " + g + " = " + W + "; " + Q + " ", l && (a += " if (!" + h + ") break; "), a += " } ", l && (a += " else " + h + " = true; "), a += " }  ", l && (a += " if (" + h + ") { ", p += "}"))
                 }
                 return l && (a += " " + p + " if (" + d + " == errors) {"), a
             }
         },
-        8441: e => {
+        5073: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5793,15 +5796,15 @@
                     e.compositeRule = f.compositeRule = !0;
                     var x = e.validate(f);
                     f.baseId = P, e.util.varOccurences(x, g) < 2 ? a += " " + e.util.varReplace(x, g, w) + " " : a += " var " + g + " = " + w + "; " + x + " ", e.compositeRule = f.compositeRule = S, a += " if (!" + p + ") { for (var " + v + "=startErrs" + o + "; " + v + "<errors; " + v + "++) { vErrors[" + v + "].propertyName = " + h + "; }   var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'propertyNames' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { propertyName: '" + y + "' } ", !1 !== e.opts.messages && (a += " , message: 'property name \\'" + y + "\\' is invalid' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", !e.compositeRule && l && (e.async ? a += " throw new ValidationError(vErrors); " : a += " validate.errors = vErrors; return false; "), l && (a += " break; "), a += " } }"
                 }
                 return l && (a += "  if (" + d + " == errors) {"), a
             }
         },
-        2392: e => {
+        5686: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a, o, n = " ",
                     i = e.level,
                     s = e.dataLevel,
                     u = e.schema[r],
                     l = e.errSchemaPath + "/" + r,
@@ -5836,15 +5839,15 @@
                         if (!e.async) throw new Error("async schema referenced by sync schema");
                         c && (n += " var " + f + "; "), n += " try { await " + b + "; ", c && (n += " " + f + " = true; "), n += " } catch (e) { if (!(e instanceof ValidationError)) throw e; if (vErrors === null) vErrors = e.errors; else vErrors = vErrors.concat(e.errors); errors = vErrors.length; ", c && (n += " " + f + " = false; "), n += " } ", c && (n += " if (" + f + ") { ")
                     } else n += " if (!" + b + ") { if (vErrors === null) vErrors = " + o + ".errors; else vErrors = vErrors.concat(" + o + ".errors); errors = vErrors.length; } ", c && (n += " else { ")
                 }
                 return n
             }
         },
-        1287: e => {
+        2843: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = " ",
                     o = e.level,
                     n = e.dataLevel,
                     i = e.schema[r],
                     s = e.schemaPath + e.util.getProperty(r),
@@ -5869,44 +5872,44 @@
                 if (f || h.length) {
                     var E = e.errorPath,
                         P = f || h.length >= e.opts.loopRequired,
                         w = e.opts.ownProperties;
                     if (l)
                         if (a += " var missing" + o + "; ", P) {
                             f || (a += " var " + p + " = validate.schema" + s + "; ");
-                            var S = "' + " + (D = "schema" + o + "[" + (_ = "i" + o) + "]") + " + '";
-                            e.opts._errorDataPathProperty && (e.errorPath = e.util.getPathExpr(E, D, e.opts.jsonPointers)), a += " var " + d + " = true; ", f && (a += " if (schema" + o + " === undefined) " + d + " = true; else if (!Array.isArray(schema" + o + ")) " + d + " = false; else {"), a += " for (var " + _ + " = 0; " + _ + " < " + p + ".length; " + _ + "++) { " + d + " = " + c + "[" + p + "[" + _ + "]] !== undefined ", w && (a += " &&   Object.prototype.hasOwnProperty.call(" + c + ", " + p + "[" + _ + "]) "), a += "; if (!" + d + ") break; } ", f && (a += "  }  "), a += "  if (!" + d + ") {   ", (O = O || []).push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + S + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + S + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ";
+                            var S = "' + " + (A = "schema" + o + "[" + (_ = "i" + o) + "]") + " + '";
+                            e.opts._errorDataPathProperty && (e.errorPath = e.util.getPathExpr(E, A, e.opts.jsonPointers)), a += " var " + d + " = true; ", f && (a += " if (schema" + o + " === undefined) " + d + " = true; else if (!Array.isArray(schema" + o + ")) " + d + " = false; else {"), a += " for (var " + _ + " = 0; " + _ + " < " + p + ".length; " + _ + "++) { " + d + " = " + c + "[" + p + "[" + _ + "]] !== undefined ", w && (a += " &&   Object.prototype.hasOwnProperty.call(" + c + ", " + p + "[" + _ + "]) "), a += "; if (!" + d + ") break; } ", f && (a += "  }  "), a += "  if (!" + d + ") {   ", (O = O || []).push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + S + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + S + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ";
                             var x = a;
                             a = O.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + x + "]); " : a += " validate.errors = [" + x + "]; return false; " : a += " var err = " + x + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", a += " } else { "
                         } else {
                             a += " if ( ";
                             var O, j = h;
                             if (j)
                                 for (var _ = -1, F = j.length - 1; _ < F;) C = j[_ += 1], _ && (a += " || "), a += " ( ( " + (I = c + (R = e.util.getProperty(C))) + " === undefined ", w && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(C) + "') "), a += ") && (missing" + o + " = " + e.util.toQuotedString(e.opts.jsonPointers ? C : R) + ") ) ";
-                            a += ") {  ", S = "' + " + (D = "missing" + o) + " + '", e.opts._errorDataPathProperty && (e.errorPath = e.opts.jsonPointers ? e.util.getPathExpr(E, D, !0) : E + " + " + D), (O = O || []).push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + S + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + S + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", x = a, a = O.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + x + "]); " : a += " validate.errors = [" + x + "]; return false; " : a += " var err = " + x + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", a += " } else { "
+                            a += ") {  ", S = "' + " + (A = "missing" + o) + " + '", e.opts._errorDataPathProperty && (e.errorPath = e.opts.jsonPointers ? e.util.getPathExpr(E, A, !0) : E + " + " + A), (O = O || []).push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + S + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + S + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", x = a, a = O.pop(), !e.compositeRule && l ? e.async ? a += " throw new ValidationError([" + x + "]); " : a += " validate.errors = [" + x + "]; return false; " : a += " var err = " + x + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", a += " } else { "
                         }
                     else if (P) {
-                        var D;
-                        f || (a += " var " + p + " = validate.schema" + s + "; "), S = "' + " + (D = "schema" + o + "[" + (_ = "i" + o) + "]") + " + '", e.opts._errorDataPathProperty && (e.errorPath = e.util.getPathExpr(E, D, e.opts.jsonPointers)), f && (a += " if (" + p + " && !Array.isArray(" + p + ")) {  var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + S + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + S + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; } else if (" + p + " !== undefined) { "), a += " for (var " + _ + " = 0; " + _ + " < " + p + ".length; " + _ + "++) { if (" + c + "[" + p + "[" + _ + "]] === undefined ", w && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", " + p + "[" + _ + "]) "), a += ") {  var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + S + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + S + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; } } ", f && (a += "  }  ")
+                        var A;
+                        f || (a += " var " + p + " = validate.schema" + s + "; "), S = "' + " + (A = "schema" + o + "[" + (_ = "i" + o) + "]") + " + '", e.opts._errorDataPathProperty && (e.errorPath = e.util.getPathExpr(E, A, e.opts.jsonPointers)), f && (a += " if (" + p + " && !Array.isArray(" + p + ")) {  var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + S + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + S + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; } else if (" + p + " !== undefined) { "), a += " for (var " + _ + " = 0; " + _ + " < " + p + ".length; " + _ + "++) { if (" + c + "[" + p + "[" + _ + "]] === undefined ", w && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", " + p + "[" + _ + "]) "), a += ") {  var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + S + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + S + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; } } ", f && (a += "  }  ")
                     } else {
-                        var A = h;
-                        if (A)
-                            for (var C, k = -1, $ = A.length - 1; k < $;) {
-                                C = A[k += 1];
+                        var D = h;
+                        if (D)
+                            for (var C, k = -1, $ = D.length - 1; k < $;) {
+                                C = D[k += 1];
                                 var R = e.util.getProperty(C),
                                     I = (S = e.util.escapeQuotes(C), c + R);
                                 e.opts._errorDataPathProperty && (e.errorPath = e.util.getPath(E, C, e.opts.jsonPointers)), a += " if ( " + I + " === undefined ", w && (a += " || ! Object.prototype.hasOwnProperty.call(" + c + ", '" + e.util.escapeQuotes(C) + "') "), a += ") {  var err =   ", !1 !== e.createErrors ? (a += " { keyword: 'required' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(u) + " , params: { missingProperty: '" + S + "' } ", !1 !== e.opts.messages && (a += " , message: '", e.opts._errorDataPathProperty ? a += "is a required property" : a += "should have required property \\'" + S + "\\'", a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + s + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + c + " "), a += " } ") : a += " {} ", a += ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; } "
                             }
                     }
                     e.errorPath = E
                 } else l && (a += " if (true) {");
                 return a
             }
         },
-        3603: e => {
+        5737: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a, o = " ",
                     n = e.level,
                     i = e.dataLevel,
                     s = e.schema[r],
                     u = e.schemaPath + e.util.getProperty(r),
@@ -5930,15 +5933,15 @@
                     y.push(o), o = "", !1 !== e.createErrors ? (o += " { keyword: 'uniqueItems' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(l) + " , params: { i: i, j: j } ", !1 !== e.opts.messages && (o += " , message: 'should NOT have duplicate items (items ## ' + j + ' and ' + i + ' are identical)' "), e.opts.verbose && (o += " , schema:  ", o += p ? "validate.schema" + u : "" + s, o += "         , parentSchema: validate.schema" + e.schemaPath + " , data: " + d + " "), o += " } ") : o += " {} ";
                     var g = o;
                     o = y.pop(), !e.compositeRule && c ? e.async ? o += " throw new ValidationError([" + g + "]); " : o += " validate.errors = [" + g + "]; return false; " : o += " var err = " + g + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", o += " } ", c && (o += " else { ")
                 } else c && (o += " if (true) { ");
                 return o
             }
         },
-        9508: e => {
+        8787: e => {
             "use strict";
             e.exports = function(e, r, t) {
                 var a = "",
                     o = !0 === e.schema.$async,
                     n = e.util.schemaHasRulesExcept(e.schema, e.RULES.all, "$ref"),
                     i = e.self._getId(e.schema);
                 if (e.opts.strictKeywords) {
@@ -5993,17 +5996,17 @@
                     if (x || S || !0 === O || O && !Y(O)) {
                         f = e.schemaPath + ".type", p = e.errSchemaPath + "/type", f = e.schemaPath + ".type", p = e.errSchemaPath + "/type";
                         var j = S ? "checkDataTypes" : "checkDataType";
                         if (a += " if (" + e.util[j](w, m, e.opts.strictNumbers, !0) + ") { ", x) {
                             var _ = "dataType" + l,
                                 F = "coerced" + l;
                             a += " var " + _ + " = typeof " + m + "; var " + F + " = undefined; ", "array" == e.opts.coerceTypes && (a += " if (" + _ + " == 'object' && Array.isArray(" + m + ") && " + m + ".length == 1) { " + m + " = " + m + "[0]; " + _ + " = typeof " + m + "; if (" + e.util.checkDataType(e.schema.type, m, e.opts.strictNumbers) + ") " + F + " = " + m + "; } "), a += " if (" + F + " !== undefined) ; ";
-                            var D = x;
-                            if (D)
-                                for (var A, C = -1, k = D.length - 1; C < k;) "string" == (A = D[C += 1]) ? a += " else if (" + _ + " == 'number' || " + _ + " == 'boolean') " + F + " = '' + " + m + "; else if (" + m + " === null) " + F + " = ''; " : "number" == A || "integer" == A ? (a += " else if (" + _ + " == 'boolean' || " + m + " === null || (" + _ + " == 'string' && " + m + " && " + m + " == +" + m + " ", "integer" == A && (a += " && !(" + m + " % 1)"), a += ")) " + F + " = +" + m + "; ") : "boolean" == A ? a += " else if (" + m + " === 'false' || " + m + " === 0 || " + m + " === null) " + F + " = false; else if (" + m + " === 'true' || " + m + " === 1) " + F + " = true; " : "null" == A ? a += " else if (" + m + " === '' || " + m + " === 0 || " + m + " === false) " + F + " = null; " : "array" == e.opts.coerceTypes && "array" == A && (a += " else if (" + _ + " == 'string' || " + _ + " == 'number' || " + _ + " == 'boolean' || " + m + " == null) " + F + " = [" + m + "]; ");
+                            var A = x;
+                            if (A)
+                                for (var D, C = -1, k = A.length - 1; C < k;) "string" == (D = A[C += 1]) ? a += " else if (" + _ + " == 'number' || " + _ + " == 'boolean') " + F + " = '' + " + m + "; else if (" + m + " === null) " + F + " = ''; " : "number" == D || "integer" == D ? (a += " else if (" + _ + " == 'boolean' || " + m + " === null || (" + _ + " == 'string' && " + m + " && " + m + " == +" + m + " ", "integer" == D && (a += " && !(" + m + " % 1)"), a += ")) " + F + " = +" + m + "; ") : "boolean" == D ? a += " else if (" + m + " === 'false' || " + m + " === 0 || " + m + " === null) " + F + " = false; else if (" + m + " === 'true' || " + m + " === 1) " + F + " = true; " : "null" == D ? a += " else if (" + m + " === '' || " + m + " === 0 || " + m + " === false) " + F + " = null; " : "array" == e.opts.coerceTypes && "array" == D && (a += " else if (" + _ + " == 'string' || " + _ + " == 'number' || " + _ + " == 'boolean' || " + m + " == null) " + F + " = [" + m + "]; ");
                             a += " else {   ", (W = W || []).push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'type' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(p) + " , params: { type: '", a += S ? "" + w.join(",") : "" + w, a += "' } ", !1 !== e.opts.messages && (a += " , message: 'should be ", a += S ? "" + w.join(",") : "" + w, a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + f + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + m + " "), a += " } ") : a += " {} ", y = a, a = W.pop(), !e.compositeRule && h ? e.async ? a += " throw new ValidationError([" + y + "]); " : a += " validate.errors = [" + y + "]; return false; " : a += " var err = " + y + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ", a += " } if (" + F + " !== undefined) {  ";
                             var $ = c ? "data" + (c - 1 || "") : "parentData";
                             a += " " + m + " = " + F + "; ", c || (a += "if (" + $ + " !== undefined)"), a += " " + $ + "[" + (c ? e.dataPathArr[c] : "parentDataProperty") + "] = " + F + "; } "
                         } else(W = W || []).push(a), a = "", !1 !== e.createErrors ? (a += " { keyword: 'type' , dataPath: (dataPath || '') + " + e.errorPath + " , schemaPath: " + e.util.toQuotedString(p) + " , params: { type: '", a += S ? "" + w.join(",") : "" + w, a += "' } ", !1 !== e.opts.messages && (a += " , message: 'should be ", a += S ? "" + w.join(",") : "" + w, a += "' "), e.opts.verbose && (a += " , schema: validate.schema" + f + " , parentSchema: validate.schema" + e.schemaPath + " , data: " + m + " "), a += " } ") : a += " {} ", y = a, a = W.pop(), !e.compositeRule && h ? e.async ? a += " throw new ValidationError([" + y + "]); " : a += " validate.errors = [" + y + "]; return false; " : a += " var err = " + y + ";  if (vErrors === null) vErrors = [err]; else vErrors.push(err); errors++; ";
                         a += " } "
                     }
                 }
@@ -6014,16 +6017,16 @@
                         for (var I = -1, N = R.length - 1; I < N;)
                             if (Y(O = R[I += 1])) {
                                 if (O.type && (a += " if (" + e.util.checkDataType(O.type, m, e.opts.strictNumbers) + ") { "), e.opts.useDefaults)
                                     if ("object" == O.type && e.schema.properties) {
                                         d = e.schema.properties;
                                         var T = Object.keys(d);
                                         if (T)
-                                            for (var q, L = -1, U = T.length - 1; L < U;)
-                                                if (void 0 !== (z = d[q = T[L += 1]]).default) {
+                                            for (var q, U = -1, L = T.length - 1; U < L;)
+                                                if (void 0 !== (z = d[q = T[U += 1]]).default) {
                                                     var M = m + e.util.getProperty(q);
                                                     if (e.compositeRule) {
                                                         if (e.opts.strictDefaults) {
                                                             if (b = "default is ignored for: " + M, "log" !== e.opts.strictDefaults) throw new Error(b);
                                                             e.logger.warn(b)
                                                         }
                                                     } else a += " if (" + M + " === undefined ", "empty" == e.opts.useDefaults && (a += " || " + M + " === null || " + M + " === '' "), a += " ) " + M + " = ", "shared" == e.opts.useDefaults ? a += " " + e.useDefault(z.default) + " " : a += " " + JSON.stringify(z.default) + " ", a += "; "
@@ -6063,19 +6066,19 @@
                         for (var t = r.implements, a = 0; a < t.length; a++)
                             if (void 0 !== e.schema[t[a]]) return !0
                     }(r)
                 }
                 return h && (a += " " + P + " "), g ? (o ? (a += " if (errors === 0) return data;           ", a += " else throw new ValidationError(vErrors); ") : (a += " validate.errors = vErrors; ", a += " return errors === 0;       "), a += " }; return validate;") : a += " var " + v + " = errors === errs_" + l + ";", a
             }
         },
-        4895: (e, r, t) => {
+        6041: (e, r, t) => {
             "use strict";
             var a = /^[a-z_$][a-z0-9_$-]*$/i,
-                o = t(4165),
-                n = t(1128);
+                o = t(5203),
+                n = t(7321);
             e.exports = {
                 add: function(e, r) {
                     var t = this.RULES;
                     if (t.keywords[e]) throw new Error("Keyword " + e + " is already defined");
                     if (!a.test(e)) throw new Error("Keyword " + e + " is not a valid identifier");
                     if (r) {
                         this.validateKeyword(r, !0);
@@ -6133,14 +6136,422 @@
                     var a = this._validateKeyword = this._validateKeyword || this.compile(n, !0);
                     if (a(r)) return !0;
                     if (e.errors = a.errors, t) throw new Error("custom keyword definition is invalid: " + this.errorsText(a.errors));
                     return !1
                 }
             }
         },
+        4965: (e, r, t) => {
+            var a = t(361),
+                o = t(6602),
+                n = t(1735),
+                i = t(6913),
+                s = t(5564),
+                u = t(2348),
+                l = t(5325),
+                c = t(3856),
+                d = t(8446),
+                f = t(8630),
+                p = t(5604),
+                h = t(9734),
+                m = t(4486),
+                v = t(4908),
+                y = t(7185),
+                g = t(2569),
+                b = (e, ...r) => g.apply(null, [e].concat(s(r))),
+                E = e => w(B, e),
+                P = e => w(W, e),
+                w = (e, r) => -1 !== e.indexOf(r),
+                S = e => !T(e).length && !1 !== e && !0 !== e,
+                x = e => f(e) || !0 === e || !1 === e,
+                O = e => !1 === e,
+                j = e => !0 === e,
+                _ = (e, r, t) => t(e),
+                F = e => h(v(u(e))),
+                A = e => void 0 !== e,
+                D = e => v(u(e.map(T))),
+                C = e => e[0],
+                k = e => Math.max.apply(Math, e),
+                $ = e => Math.min.apply(Math, e);
+
+            function R(e) {
+                if (Array.isArray(e.allOf)) {
+                    var r = e.allOf;
+                    return delete e.allOf, [e].concat(r.map((function(e) {
+                        return R(e)
+                    })))
+                }
+                return [e]
+            }
+
+            function I(e, r) {
+                return e.map((function(e) {
+                    return e && e[r]
+                }))
+            }
+
+            function N(e, r) {
+                return e.map((function(e) {
+                    if (e) {
+                        if (!Array.isArray(e.items)) return e.items;
+                        var t = e.items[r];
+                        return x(t) ? t : e.hasOwnProperty("additionalItems") ? e.additionalItems : void 0
+                    }
+                }))
+            }
+
+            function T(e) {
+                return f(e) || Array.isArray(e) ? Object.keys(e) : []
+            }
+
+            function q(e, r) {
+                if (r = r || [], !e.length) return r;
+                var t = e.slice(0).shift(),
+                    a = e.slice(1);
+                return r.length ? q(a, s(r.map((e => t.map((r => [r].concat(e))))))) : q(a, t.map((e => e)))
+            }
+
+            function U(e, r) {
+                var t;
+                try {
+                    t = e.map((function(e) {
+                        return JSON.stringify(e, null, 2)
+                    })).join("\n")
+                } catch (r) {
+                    t = e.join(", ")
+                }
+                throw new Error('Could not resolve values for path:"' + r.join(".") + '". They are probably incompatible. Values: \n' + t)
+            }
+
+            function L(e, r, t) {
+                return function(a, o) {
+                    if (void 0 === o) throw new Error("You need to call merger with a key for the property name or index if array.");
+                    return o = String(o), e(a, null, t.concat(r, o))
+                }
+            }
+
+            function M(e, r, t, a, n, i) {
+                if (e.length) {
+                    var s = n.resolvers[r];
+                    if (!s) throw new Error("No resolver found for " + r);
+                    var u = y(t.map((function(r) {
+                            return e.reduce((function(e, t) {
+                                return void 0 !== r[t] && (e[t] = r[t]), e
+                            }), {})
+                        })).filter(A), o),
+                        l = ("properties" === r ? B : W).reduce((function(e, r) {
+                            return w(Q, r) ? e[r] = L(a, r, i) : e[r] = function(e) {
+                                return a(e, null, i.concat(r))
+                            }, e
+                        }), {});
+                    "items" === r && (l.itemsArray = L(a, "items", i), l.items = function(e) {
+                        return a(e, null, i.concat("items"))
+                    });
+                    var c = s(u, i.concat(r), l, n);
+                    return f(c) || U(u, i.concat(r)),
+                        function(e) {
+                            for (var r in e) e.hasOwnProperty(r) && S(e[r]) && delete e[r];
+                            return e
+                        }(c)
+                }
+            }
+
+            function V(e, r, t) {
+                var a = D(t || e),
+                    n = t ? N : I;
+                return a.reduce((function(t, a) {
+                    var i = n(e, a),
+                        s = y(i.filter(A), o);
+                    return t[a] = r(s, a), t
+                }), t ? [] : {})
+            }
+
+            function z(e) {
+                return {
+                    required: e
+                }
+            }
+            var B = ["properties", "patternProperties", "additionalProperties"],
+                W = ["items", "additionalItems"],
+                Q = ["properties", "patternProperties", "definitions", "dependencies"],
+                H = ["anyOf", "oneOf"],
+                K = ["additionalProperties", "additionalItems", "contains", "propertyNames", "not", "items"],
+                J = {
+                    type(e) {
+                        if (e.some(Array.isArray)) {
+                            var r = e.map((function(e) {
+                                    return Array.isArray(e) ? e : [e]
+                                })),
+                                t = l.apply(null, r);
+                            if (1 === t.length) return t[0];
+                            if (t.length > 1) return v(t)
+                        }
+                    },
+                    properties(e, r, t, a) {
+                        a.ignoreAdditionalProperties || (e.forEach((function(r) {
+                            var a = e.filter((e => e !== r)),
+                                o = T(r.properties),
+                                n = T(r.patternProperties).map((e => new RegExp(e)));
+                            a.forEach((function(e) {
+                                var a = T(e.properties),
+                                    i = a.filter((e => n.some((r => r.test(e)))));
+                                b(a, o, i).forEach((function(a) {
+                                    e.properties[a] = t.properties([e.properties[a], r.additionalProperties], a)
+                                }))
+                            }))
+                        })), e.forEach((function(r) {
+                            var t = e.filter((e => e !== r)),
+                                a = T(r.patternProperties);
+                            !1 === r.additionalProperties && t.forEach((function(e) {
+                                var r = T(e.patternProperties);
+                                b(r, a).forEach((r => delete e.patternProperties[r]))
+                            }))
+                        })));
+                        var o, n = {
+                            additionalProperties: t.additionalProperties(e.map((e => e.additionalProperties))),
+                            patternProperties: V(e.map((e => e.patternProperties)), t.patternProperties),
+                            properties: V(e.map((e => e.properties)), t.properties)
+                        };
+                        return !1 === n.additionalProperties && m(o = n.properties, (function(e, r) {
+                            !1 === e && delete o[r]
+                        })), n
+                    },
+                    dependencies: (e, r, t) => D(e).reduce((function(r, a) {
+                        var n = I(e, a),
+                            i = y(n.filter(A), d),
+                            s = i.filter(Array.isArray);
+                        if (s.length) {
+                            if (s.length === i.length) r[a] = F(i);
+                            else {
+                                var u = i.filter(x),
+                                    l = s.map(z);
+                                r[a] = t(u.concat(l), a)
+                            }
+                            return r
+                        }
+                        return i = y(i, o), r[a] = t(i, a), r
+                    }), {}),
+                    items(e, r, t) {
+                        var a, o, n = e.map((e => e.items)),
+                            i = n.filter(A),
+                            s = {};
+                        return i.every(x) ? s.items = t.items(n) : s.items = V(e, t.itemsArray, n), i.every(Array.isArray) ? a = e.map((e => e.additionalItems)) : i.some(Array.isArray) && (a = e.map((function(e) {
+                            if (e) return Array.isArray(e.items) ? e.additionalItems : e.items
+                        }))), a && (s.additionalItems = t.additionalItems(a)), !1 === s.additionalItems && Array.isArray(s.items) && (o = s.items, m(o, (function(e, r) {
+                            !1 === e && o.splice(r, 1)
+                        }))), s
+                    },
+                    oneOf(e, r, t) {
+                        var n = function(e, r) {
+                                return e.map((function(e, t) {
+                                    try {
+                                        return r(e, t)
+                                    } catch (e) {
+                                        return
+                                    }
+                                })).filter(A)
+                            }(q(a(e)), t),
+                            i = y(n, o);
+                        if (i.length) return i
+                    },
+                    not: e => ({
+                        anyOf: e
+                    }),
+                    pattern(e, r, t, a, o) {
+                        var n = r.pop();
+                        o(e.map((function(e) {
+                            return {
+                                [n]: e
+                            }
+                        })))
+                    },
+                    multipleOf(e) {
+                        for (var r = e.slice(0), t = 1; r.some((e => !Number.isInteger(e)));) r = r.map((e => 10 * e)), t *= 10;
+                        return n(r) / t
+                    },
+                    enum(e) {
+                        var r = c.apply(null, e.concat(d));
+                        if (r.length) return h(r)
+                    }
+                };
+
+            function Z(e, r, t) {
+                return t = t || [], r = i(r, {
+                        ignoreAdditionalProperties: !1,
+                        resolvers: J
+                    }),
+                    function e(n, i, s) {
+                        n = a(n.filter(A)), s = s || [];
+                        var u = f(i) ? i : {};
+                        if (n.length) {
+                            if (n.some(O)) return !1;
+                            if (n.every(j)) return !0;
+                            n = n.filter(f);
+                            var l = D(n);
+                            if (w(l, "allOf")) return Z({
+                                allOf: n
+                            }, r, t);
+                            var c = l.filter(E);
+                            p(l, c);
+                            var d = l.filter(P);
+                            return p(l, d), l.forEach((function(t) {
+                                var a = I(n, t),
+                                    i = y(a.filter(A), function(e) {
+                                        return function(r, t) {
+                                            return o({
+                                                [e]: r
+                                            }, {
+                                                [e]: t
+                                            })
+                                        }
+                                    }(t));
+                                if (1 === i.length && w(H, t)) u[t] = i[0].map((function(r) {
+                                    return e([r], r)
+                                }));
+                                else if (1 !== i.length || w(Q, t) || w(K, t)) {
+                                    var l, c = r.resolvers[t] || r.resolvers.defaultResolver;
+                                    if (!c) throw new Error("No resolver found for key " + t + ". You can provide a resolver for this keyword in the options, or provide a default resolver.");
+                                    l = w(Q, t) || w(H, t) ? L(e, t, s) : function(r) {
+                                        return e(r, null, s.concat(t))
+                                    };
+                                    var d = !1;
+                                    u[t] = c(i, s.concat(t), l, r, (function(e) {
+                                        return d = Array.isArray(e),
+                                            function(e) {
+                                                u.allOf = function(e, r) {
+                                                    return Array.isArray(e) ? (e.splice.apply(e, [0, 0].concat(r)), e) : r
+                                                }(u.allOf, e)
+                                            }(e)
+                                    })), void 0 !== u[t] || d ? void 0 === u[t] && delete u[t] : U(i, s.concat(t))
+                                } else u[t] = i[0]
+                            })), Object.assign(u, M(c, "properties", n, e, r, s)), Object.assign(u, M(d, "items", n, e, r, s)), u
+                        }
+                    }(u(R(e)), e)
+            }
+            J.$id = C, J.$ref = C, J.$schema = C, J.additionalItems = _, J.additionalProperties = _, J.anyOf = J.oneOf, J.contains = _, J.default = C, J.definitions = J.dependencies, J.description = C, J.examples = e => y(s(e), d), J.exclusiveMaximum = $, J.exclusiveMinimum = k, J.maximum = $, J.maxItems = $, J.maxLength = $, J.maxProperties = $, J.minimum = k, J.minItems = k, J.minLength = k, J.minProperties = k, J.propertyNames = _, J.required = e => F(e), J.title = C, J.uniqueItems = e => e.some(j), Z.options = {
+                resolvers: J
+            }, e.exports = Z
+        },
+        3393: e => {
+            "use strict";
+            var r = e.exports = function(e, r, a) {
+                "function" == typeof r && (a = r, r = {}), t(r, "function" == typeof(a = r.cb || a) ? a : a.pre || function() {}, a.post || function() {}, e, "", e)
+            };
+
+            function t(e, a, o, n, i, s, u, l, c, d) {
+                if (n && "object" == typeof n && !Array.isArray(n)) {
+                    for (var f in a(n, i, s, u, l, c, d), n) {
+                        var p = n[f];
+                        if (Array.isArray(p)) {
+                            if (f in r.arrayKeywords)
+                                for (var h = 0; h < p.length; h++) t(e, a, o, p[h], i + "/" + f + "/" + h, s, i, f, n, h)
+                        } else if (f in r.propsKeywords) {
+                            if (p && "object" == typeof p)
+                                for (var m in p) t(e, a, o, p[m], i + "/" + f + "/" + m.replace(/~/g, "~0").replace(/\//g, "~1"), s, i, f, n, m)
+                        } else(f in r.keywords || e.allKeys && !(f in r.skipKeywords)) && t(e, a, o, p, i + "/" + f, s, i, f, n)
+                    }
+                    o(n, i, s, u, l, c, d)
+                }
+            }
+            r.keywords = {
+                additionalItems: !0,
+                items: !0,
+                contains: !0,
+                additionalProperties: !0,
+                propertyNames: !0,
+                not: !0
+            }, r.arrayKeywords = {
+                items: !0,
+                allOf: !0,
+                anyOf: !0,
+                oneOf: !0
+            }, r.propsKeywords = {
+                definitions: !0,
+                properties: !0,
+                patternProperties: !0,
+                dependencies: !0
+            }, r.skipKeywords = {
+                default: !0,
+                enum: !0,
+                const: !0,
+                required: !0,
+                maximum: !0,
+                minimum: !0,
+                exclusiveMaximum: !0,
+                exclusiveMinimum: !0,
+                multipleOf: !0,
+                maxLength: !0,
+                minLength: !0,
+                pattern: !0,
+                format: !0,
+                maxItems: !0,
+                minItems: !0,
+                uniqueItems: !0,
+                maxProperties: !0,
+                minProperties: !0
+            }
+        },
+        5744: (e, r) => {
+            "use strict";
+            var t = "function" == typeof Symbol && Symbol.for,
+                a = t ? Symbol.for("react.element") : 60103,
+                o = t ? Symbol.for("react.portal") : 60106,
+                n = t ? Symbol.for("react.fragment") : 60107,
+                i = t ? Symbol.for("react.strict_mode") : 60108,
+                s = t ? Symbol.for("react.profiler") : 60114,
+                u = t ? Symbol.for("react.provider") : 60109,
+                l = t ? Symbol.for("react.context") : 60110,
+                c = t ? Symbol.for("react.async_mode") : 60111,
+                d = t ? Symbol.for("react.concurrent_mode") : 60111,
+                f = t ? Symbol.for("react.forward_ref") : 60112,
+                p = t ? Symbol.for("react.suspense") : 60113,
+                h = (t && Symbol.for("react.suspense_list"), t ? Symbol.for("react.memo") : 60115),
+                m = t ? Symbol.for("react.lazy") : 60116;
+            t && Symbol.for("react.fundamental"), t && Symbol.for("react.responder");
+
+            function v(e) {
+                if ("object" == typeof e && null !== e) {
+                    var r = e.$$typeof;
+                    switch (r) {
+                        case a:
+                            switch (e = e.type) {
+                                case c:
+                                case d:
+                                case n:
+                                case s:
+                                case i:
+                                case p:
+                                    return e;
+                                default:
+                                    switch (e = e && e.$$typeof) {
+                                        case l:
+                                        case f:
+                                        case u:
+                                            return e;
+                                        default:
+                                            return r
+                                    }
+                            }
+                        case m:
+                        case h:
+                        case o:
+                            return r
+                    }
+                }
+            }
+            r.isForwardRef = function(e) {
+                return v(e) === f
+            }, r.isMemo = function(e) {
+                return v(e) === h
+            }
+        },
+        3434: (e, r, t) => {
+            "use strict";
+            e.exports = t(5744)
+        },
         1252: (e, r, t) => {
             "use strict";
             var a = t(4653),
                 o = t(9158),
                 n = t(9882),
                 i = Math.pow(2, 31) - 1;
 
@@ -6225,15 +6636,15 @@
             }
         },
         4198: (e, r, t) => {
             var a = t(2897);
             e.exports = a
         },
         4771: (e, r, t) => {
-            t(8412);
+            t(290);
             var a = t(5379);
             e.exports = a("Array", "fill")
         },
         2415: (e, r, t) => {
             t(7690);
             var a = t(5379);
             e.exports = a("Array", "includes")
@@ -6262,24 +6673,24 @@
                 if (a(e)) return e;
                 throw n(o(e) + " is not an object")
             }
         },
         1860: (e, r, t) => {
             "use strict";
             var a = t(9678),
-                o = t(9413),
+                o = t(1164),
                 n = t(623);
             e.exports = function(e) {
                 for (var r = a(this), t = n(r), i = arguments.length, s = o(i > 1 ? arguments[1] : void 0, t), u = i > 2 ? arguments[2] : void 0, l = void 0 === u ? t : o(u, t); l > s;) r[s++] = e;
                 return r
             }
         },
         1692: (e, r, t) => {
             var a = t(4529),
-                o = t(9413),
+                o = t(1164),
                 n = t(623),
                 i = function(e) {
                     return function(r, t, i) {
                         var s, u = a(r),
                             l = n(u),
                             c = o(i, l);
                         if (e && t != t) {
@@ -6363,17 +6774,16 @@
                 o = t(941),
                 n = a.document,
                 i = o(n) && o(n.createElement);
             e.exports = function(e) {
                 return i ? n.createElement(e) : {}
             }
         },
-        2861: (e, r, t) => {
-            var a = t(626);
-            e.exports = a("navigator", "userAgent") || ""
+        2861: e => {
+            e.exports = "undefined" != typeof navigator && String(navigator.userAgent) || ""
         },
         3385: (e, r, t) => {
             var a, o, n = t(1899),
                 i = t(2861),
                 s = n.process,
                 u = n.Deno,
                 l = s && s.versions || u && u.version,
@@ -6410,22 +6820,22 @@
                             return new e(t, a, n)
                         }
                         return o(e, this, arguments)
                     };
                     return r.prototype = e.prototype, r
                 };
             e.exports = function(e, r) {
-                var t, o, h, m, v, y, g, b, E = e.target,
-                    P = e.global,
-                    w = e.stat,
-                    S = e.proto,
-                    x = P ? a : w ? a[E] : (a[E] || {}).prototype,
-                    O = P ? l : l[E] || d(l, E, {})[E],
-                    j = O.prototype;
-                for (h in r) t = !u(P ? h : E + (w ? "." : "#") + h, e.forced) && x && f(x, h), v = O[h], t && (y = e.dontCallGetSet ? (b = s(x, h)) && b.value : x[h]), m = t && y ? y : r[h], t && typeof v == typeof m || (g = e.bind && t ? c(m, a) : e.wrap && t ? p(m) : S && i(m) ? n(m) : m, (e.sham || m && m.sham || v && v.sham) && d(g, "sham", !0), d(O, h, g), S && (f(l, o = E + "Prototype") || d(l, o, {}), d(l[o], h, m), e.real && j && !j[h] && d(j, h, m)))
+                var t, o, h, m, v, y, g, b, E, P = e.target,
+                    w = e.global,
+                    S = e.stat,
+                    x = e.proto,
+                    O = w ? a : S ? a[P] : (a[P] || {}).prototype,
+                    j = w ? l : l[P] || d(l, P, {})[P],
+                    _ = j.prototype;
+                for (m in r) o = !(t = u(w ? m : P + (S ? "." : "#") + m, e.forced)) && O && f(O, m), y = j[m], o && (g = e.dontCallGetSet ? (E = s(O, m)) && E.value : O[m]), v = o && g ? g : r[m], o && typeof y == typeof v || (b = e.bind && o ? c(v, a) : e.wrap && o ? p(v) : x && i(v) ? n(v) : v, (e.sham || v && v.sham || y && y.sham) && d(b, "sham", !0), d(j, m, b), x && (f(l, h = P + "Prototype") || d(l, h, {}), d(l[h], m, v), e.real && _ && (t || !_[m]) && d(_, m, v)))
             }
         },
         5981: e => {
             e.exports = function(e) {
                 try {
                     return !!e()
                 } catch (e) {
@@ -6500,31 +6910,31 @@
             var a = t(4883),
                 o = t(2119);
             e.exports = function(e, r) {
                 var t = e[r];
                 return o(t) ? void 0 : a(t)
             }
         },
-        1899: (e, r, t) => {
+        1899: function(e, r, t) {
             var a = function(e) {
                 return e && e.Math == Math && e
             };
             e.exports = a("object" == typeof globalThis && globalThis) || a("object" == typeof window && window) || a("object" == typeof self && self) || a("object" == typeof t.g && t.g) || function() {
                 return this
-            }() || Function("return this")()
+            }() || this || Function("return this")()
         },
         953: (e, r, t) => {
             var a = t(5329),
                 o = t(9678),
                 n = a({}.hasOwnProperty);
             e.exports = Object.hasOwn || function(e, r) {
                 return n(o(e), r)
             }
         },
-        4731: (e, r, t) => {
+        2840: (e, r, t) => {
             var a = t(5746),
                 o = t(5981),
                 n = t(1333);
             e.exports = !a && !o((function() {
                 return 7 != Object.defineProperty(n("div"), "a", {
                     get: function() {
                         return 7
@@ -6612,15 +7022,15 @@
             e.exports = Math.trunc || function(e) {
                 var a = +e;
                 return (a > 0 ? t : r)(a)
             }
         },
         5988: (e, r, t) => {
             var a = t(5746),
-                o = t(4731),
+                o = t(2840),
                 n = t(3937),
                 i = t(6059),
                 s = t(3894),
                 u = TypeError,
                 l = Object.defineProperty,
                 c = Object.getOwnPropertyDescriptor,
                 d = "enumerable",
@@ -6648,15 +7058,15 @@
             var a = t(5746),
                 o = t(8834),
                 n = t(6760),
                 i = t(1887),
                 s = t(4529),
                 u = t(3894),
                 l = t(953),
-                c = t(4731),
+                c = t(2840),
                 d = Object.getOwnPropertyDescriptor;
             r.f = a ? d : function(e, r) {
                 if (e = s(e), r = u(r), c) try {
                     return d(e, r)
                 } catch (e) {}
                 if (l(e, r)) return i(!o(n.f, e, r), e[r])
             }
@@ -6710,30 +7120,31 @@
         },
         8726: (e, r, t) => {
             var a = t(2529),
                 o = t(3030);
             (e.exports = function(e, r) {
                 return o[e] || (o[e] = void 0 !== r ? r : {})
             })("versions", []).push({
-                version: "3.26.1",
+                version: "3.30.2",
                 mode: a ? "pure" : "global",
-                copyright: "© 2014-2022 Denis Pushkarev (zloirock.ru)",
-                license: "https://github.com/zloirock/core-js/blob/v3.26.1/LICENSE",
+                copyright: "© 2014-2023 Denis Pushkarev (zloirock.ru)",
+                license: "https://github.com/zloirock/core-js/blob/v3.30.2/LICENSE",
                 source: "https://github.com/zloirock/core-js"
             })
         },
         3405: (e, r, t) => {
             var a = t(3385),
-                o = t(5981);
+                o = t(5981),
+                n = t(1899).String;
             e.exports = !!Object.getOwnPropertySymbols && !o((function() {
                 var e = Symbol();
-                return !String(e) || !(Object(e) instanceof Symbol) || !Symbol.sham && a && a < 41
+                return !n(e) || !(Object(e) instanceof Symbol) || !Symbol.sham && a && a < 41
             }))
         },
-        9413: (e, r, t) => {
+        1164: (e, r, t) => {
             var a = t(2435),
                 o = Math.max,
                 n = Math.min;
             e.exports = function(e, r) {
                 var t = a(e);
                 return t < 0 ? o(t + r, 0) : n(t, r)
             }
@@ -6829,27 +7240,22 @@
         9813: (e, r, t) => {
             var a = t(1899),
                 o = t(8726),
                 n = t(953),
                 i = t(9418),
                 s = t(3405),
                 u = t(2302),
-                l = o("wks"),
-                c = a.Symbol,
-                d = c && c.for,
-                f = u ? c : c && c.withoutSetter || i;
+                l = a.Symbol,
+                c = o("wks"),
+                d = u ? l.for || l : l && l.withoutSetter || i;
             e.exports = function(e) {
-                if (!n(l, e) || !s && "string" != typeof l[e]) {
-                    var r = "Symbol." + e;
-                    s && n(c, e) ? l[e] = c[e] : l[e] = u && d ? d(r) : f(r)
-                }
-                return l[e]
+                return n(c, e) || (c[e] = s && n(l, e) ? l[e] : d("Symbol." + e)), c[e]
             }
         },
-        8412: (e, r, t) => {
+        290: (e, r, t) => {
             var a = t(6887),
                 o = t(1860),
                 n = t(8479);
             a({
                 target: "Array",
                 proto: !0
             }, {
@@ -7038,365 +7444,14 @@
                     if (-1 === O.indexOf(n) && (!h(r, n) && h(t, n) || h(r, n) && !h(t, n))) return i === s;
                     var d = l(i, s, n, u);
                     if (!c(d)) throw new Error("Comparer must return true or false");
                     return d
                 }))
             }
         },
-        9830: (e, r, t) => {
-            var a = t(361),
-                o = t(6602),
-                n = t(1735),
-                i = t(6913),
-                s = t(5564),
-                u = t(2348),
-                l = t(5325),
-                c = t(3856),
-                d = t(8446),
-                f = t(8630),
-                p = t(5604),
-                h = t(9734),
-                m = t(4486),
-                v = t(4908),
-                y = t(7185),
-                g = t(2569),
-                b = (e, ...r) => g.apply(null, [e].concat(s(r))),
-                E = e => w(B, e),
-                P = e => w(W, e),
-                w = (e, r) => -1 !== e.indexOf(r),
-                S = e => f(e) || !0 === e || !1 === e,
-                x = e => !1 === e,
-                O = e => !0 === e,
-                j = (e, r, t) => t(e),
-                _ = e => h(v(u(e))),
-                F = e => void 0 !== e,
-                D = e => v(u(e.map(N))),
-                A = e => e[0],
-                C = e => Math.max.apply(Math, e),
-                k = e => Math.min.apply(Math, e);
-
-            function $(e) {
-                if (Array.isArray(e.allOf)) {
-                    var r = e.allOf;
-                    return delete e.allOf, [e].concat(r.map((function(e) {
-                        return $(e)
-                    })))
-                }
-                return [e]
-            }
-
-            function R(e, r) {
-                return e.map((function(e) {
-                    return e && e[r]
-                }))
-            }
-
-            function I(e, r) {
-                return e.map((function(e) {
-                    if (e) {
-                        if (!Array.isArray(e.items)) return e.items;
-                        var t = e.items[r];
-                        return S(t) ? t : e.hasOwnProperty("additionalItems") ? e.additionalItems : void 0
-                    }
-                }))
-            }
-
-            function N(e) {
-                return f(e) || Array.isArray(e) ? Object.keys(e) : []
-            }
-
-            function T(e, r) {
-                if (r = r || [], !e.length) return r;
-                var t = e.slice(0).shift(),
-                    a = e.slice(1);
-                return r.length ? T(a, s(r.map((e => t.map((r => [r].concat(e))))))) : T(a, t.map((e => e)))
-            }
-
-            function q(e, r) {
-                var t;
-                try {
-                    t = e.map((function(e) {
-                        return JSON.stringify(e, null, 2)
-                    })).join("\n")
-                } catch (r) {
-                    t = e.join(", ")
-                }
-                throw new Error('Could not resolve values for path:"' + r.join(".") + '". They are probably incompatible. Values: \n' + t)
-            }
-
-            function L(e) {
-                for (var r in e) e.hasOwnProperty(r) && !N(t = e[r]).length && !1 !== t && !0 !== t && delete e[r];
-                var t;
-                return e
-            }
-
-            function U(e, r, t) {
-                return function(a, o) {
-                    if (void 0 === o) throw new Error("You need to call merger with a key for the property name or index if array.");
-                    return o = String(o), e(a, null, t.concat(r, o))
-                }
-            }
-
-            function M(e, r, t, a, n, i) {
-                if (e.length) {
-                    var s = n.resolvers[r];
-                    if (!s) throw new Error("No resolver found for " + r);
-                    var u = y(t.map((function(r) {
-                            return e.reduce((function(e, t) {
-                                return void 0 !== r[t] && (e[t] = r[t]), e
-                            }), {})
-                        })).filter(F), o),
-                        l = ("properties" === r ? B : W).reduce((function(e, r) {
-                            return w(Q, r) ? e[r] = U(a, r, i) : e[r] = function(e) {
-                                return a(e, null, i.concat(r))
-                            }, e
-                        }), {});
-                    "items" === r && (l.itemsArray = U(a, "items", i), l.items = function(e) {
-                        return a(e, null, i.concat("items"))
-                    });
-                    var c = s(u, i.concat(r), l, n);
-                    return f(c) || q(u, i.concat(r)), L(c)
-                }
-            }
-
-            function V(e, r, t) {
-                var a = D(t || e),
-                    n = t ? I : R;
-                return a.reduce((function(t, a) {
-                    var i = n(e, a),
-                        s = y(i.filter(F), o);
-                    return t[a] = r(s, a), t
-                }), t ? [] : {})
-            }
-
-            function z(e) {
-                return {
-                    required: e
-                }
-            }
-            var B = ["properties", "patternProperties", "additionalProperties"],
-                W = ["items", "additionalItems"],
-                Q = ["properties", "patternProperties", "definitions", "dependencies"],
-                H = ["anyOf", "oneOf"],
-                K = ["additionalProperties", "additionalItems", "contains", "propertyNames", "not", "items"],
-                J = {
-                    type(e) {
-                        if (e.some(Array.isArray)) {
-                            var r = e.map((function(e) {
-                                    return Array.isArray(e) ? e : [e]
-                                })),
-                                t = l.apply(null, r);
-                            if (1 === t.length) return t[0];
-                            if (t.length > 1) return v(t)
-                        }
-                    },
-                    properties(e, r, t, a) {
-                        a.ignoreAdditionalProperties || (e.forEach((function(r) {
-                            var a = e.filter((e => e !== r)),
-                                o = N(r.properties),
-                                n = N(r.patternProperties).map((e => new RegExp(e)));
-                            a.forEach((function(e) {
-                                var a = N(e.properties),
-                                    i = a.filter((e => n.some((r => r.test(e)))));
-                                b(a, o, i).forEach((function(a) {
-                                    e.properties[a] = t.properties([e.properties[a], r.additionalProperties], a)
-                                }))
-                            }))
-                        })), e.forEach((function(r) {
-                            var t = e.filter((e => e !== r)),
-                                a = N(r.patternProperties);
-                            !1 === r.additionalProperties && t.forEach((function(e) {
-                                var r = N(e.patternProperties);
-                                b(r, a).forEach((r => delete e.patternProperties[r]))
-                            }))
-                        })));
-                        var o, n = {
-                            additionalProperties: t.additionalProperties(e.map((e => e.additionalProperties))),
-                            patternProperties: V(e.map((e => e.patternProperties)), t.patternProperties),
-                            properties: V(e.map((e => e.properties)), t.properties)
-                        };
-                        return !1 === n.additionalProperties && m(o = n.properties, (function(e, r) {
-                            !1 === e && delete o[r]
-                        })), n
-                    },
-                    dependencies: (e, r, t) => D(e).reduce((function(r, a) {
-                        var n = R(e, a),
-                            i = y(n.filter(F), d),
-                            s = i.filter(Array.isArray);
-                        if (s.length) {
-                            if (s.length === i.length) r[a] = _(i);
-                            else {
-                                var u = i.filter(S),
-                                    l = s.map(z);
-                                r[a] = t(u.concat(l), a)
-                            }
-                            return r
-                        }
-                        return i = y(i, o), r[a] = t(i, a), r
-                    }), {}),
-                    items(e, r, t) {
-                        var a, o, n = e.map((e => e.items)),
-                            i = n.filter(F),
-                            s = {};
-                        return i.every(S) ? s.items = t.items(n) : s.items = V(e, t.itemsArray, n), i.every(Array.isArray) ? a = e.map((e => e.additionalItems)) : i.some(Array.isArray) && (a = e.map((function(e) {
-                            if (e) return Array.isArray(e.items) ? e.additionalItems : e.items
-                        }))), a && (s.additionalItems = t.additionalItems(a)), !1 === s.additionalItems && Array.isArray(s.items) && (o = s.items, m(o, (function(e, r) {
-                            !1 === e && o.splice(r, 1)
-                        }))), s
-                    },
-                    oneOf(e, r, t) {
-                        var n = function(e, r) {
-                                return e.map((function(e, t) {
-                                    try {
-                                        return r(e, t)
-                                    } catch (e) {
-                                        return
-                                    }
-                                })).filter(F)
-                            }(T(a(e)), t),
-                            i = y(n, o);
-                        if (i.length) return i
-                    },
-                    not: e => ({
-                        anyOf: e
-                    }),
-                    pattern(e, r, t, a, o) {
-                        var n = r.pop();
-                        o(e.map((function(e) {
-                            return {
-                                [n]: e
-                            }
-                        })))
-                    },
-                    multipleOf(e) {
-                        for (var r = e.slice(0), t = 1; r.some((e => !Number.isInteger(e)));) r = r.map((e => 10 * e)), t *= 10;
-                        return n(r) / t
-                    },
-                    enum(e) {
-                        var r = c.apply(null, e.concat(d));
-                        if (r.length) return h(r)
-                    }
-                };
-
-            function Z(e, r, t) {
-                return t = t || [], r = i(r, {
-                        ignoreAdditionalProperties: !1,
-                        resolvers: J
-                    }),
-                    function e(n, i, s) {
-                        n = a(n.filter(F)), s = s || [];
-                        var u = f(i) ? i : {};
-                        if (n.length) {
-                            if (n.some(x)) return !1;
-                            if (n.every(O)) return !0;
-                            n = n.filter(f);
-                            var l = D(n);
-                            if (w(l, "allOf")) return Z({
-                                allOf: n
-                            }, r, t);
-                            var c = l.filter(E);
-                            p(l, c);
-                            var d = l.filter(P);
-                            return p(l, d), l.forEach((function(t) {
-                                var a = R(n, t),
-                                    i = y(a.filter(F), function(e) {
-                                        return function(r, t) {
-                                            return o({
-                                                [e]: r
-                                            }, {
-                                                [e]: t
-                                            })
-                                        }
-                                    }(t));
-                                if (1 === i.length && w(H, t)) u[t] = i[0].map((function(r) {
-                                    return e([r], r)
-                                }));
-                                else if (1 !== i.length || w(Q, t) || w(K, t)) {
-                                    var l, c = r.resolvers[t] || r.resolvers.defaultResolver;
-                                    if (!c) throw new Error("No resolver found for key " + t + ". You can provide a resolver for this keyword in the options, or provide a default resolver.");
-                                    l = w(Q, t) || w(H, t) ? U(e, t, s) : function(r) {
-                                        return e(r, null, s.concat(t))
-                                    };
-                                    var d = !1;
-                                    u[t] = c(i, s.concat(t), l, r, (function(e) {
-                                        return d = Array.isArray(e),
-                                            function(e) {
-                                                u.allOf = function(e, r) {
-                                                    return Array.isArray(e) ? (e.splice.apply(e, [0, 0].concat(r)), e) : r
-                                                }(u.allOf, e)
-                                            }(e)
-                                    })), void 0 !== u[t] || d ? void 0 === u[t] && delete u[t] : q(i, s.concat(t))
-                                } else u[t] = i[0]
-                            })), Object.assign(u, M(c, "properties", n, e, r, s)), Object.assign(u, M(d, "items", n, e, r, s)), u
-                        }
-                    }(u($(e)), e)
-            }
-            J.$id = A, J.$ref = A, J.$schema = A, J.additionalItems = j, J.additionalProperties = j, J.anyOf = J.oneOf, J.contains = j, J.default = A, J.definitions = J.dependencies, J.description = A, J.examples = e => y(s(e), d), J.exclusiveMaximum = k, J.exclusiveMinimum = C, J.maximum = k, J.maxItems = k, J.maxLength = k, J.maxProperties = k, J.minimum = C, J.minItems = C, J.minLength = C, J.minProperties = C, J.propertyNames = j, J.required = e => _(e), J.title = A, J.uniqueItems = e => e.some(O), Z.options = {
-                resolvers: J
-            }, e.exports = Z
-        },
-        9461: e => {
-            "use strict";
-            var r = e.exports = function(e, r, a) {
-                "function" == typeof r && (a = r, r = {}), t(r, "function" == typeof(a = r.cb || a) ? a : a.pre || function() {}, a.post || function() {}, e, "", e)
-            };
-
-            function t(e, a, o, n, i, s, u, l, c, d) {
-                if (n && "object" == typeof n && !Array.isArray(n)) {
-                    for (var f in a(n, i, s, u, l, c, d), n) {
-                        var p = n[f];
-                        if (Array.isArray(p)) {
-                            if (f in r.arrayKeywords)
-                                for (var h = 0; h < p.length; h++) t(e, a, o, p[h], i + "/" + f + "/" + h, s, i, f, n, h)
-                        } else if (f in r.propsKeywords) {
-                            if (p && "object" == typeof p)
-                                for (var m in p) t(e, a, o, p[m], i + "/" + f + "/" + m.replace(/~/g, "~0").replace(/\//g, "~1"), s, i, f, n, m)
-                        } else(f in r.keywords || e.allKeys && !(f in r.skipKeywords)) && t(e, a, o, p, i + "/" + f, s, i, f, n)
-                    }
-                    o(n, i, s, u, l, c, d)
-                }
-            }
-            r.keywords = {
-                additionalItems: !0,
-                items: !0,
-                contains: !0,
-                additionalProperties: !0,
-                propertyNames: !0,
-                not: !0
-            }, r.arrayKeywords = {
-                items: !0,
-                allOf: !0,
-                anyOf: !0,
-                oneOf: !0
-            }, r.propsKeywords = {
-                definitions: !0,
-                properties: !0,
-                patternProperties: !0,
-                dependencies: !0
-            }, r.skipKeywords = {
-                default: !0,
-                enum: !0,
-                const: !0,
-                required: !0,
-                maximum: !0,
-                minimum: !0,
-                exclusiveMaximum: !0,
-                exclusiveMinimum: !0,
-                multipleOf: !0,
-                maxLength: !0,
-                minLength: !0,
-                pattern: !0,
-                format: !0,
-                maxItems: !0,
-                minItems: !0,
-                uniqueItems: !0,
-                maxProperties: !0,
-                minProperties: !0
-            }
-        },
         9038: (e, r) => {
             var t = /~/,
                 a = /~[01]/g;
 
             function o(e) {
                 switch (e) {
                     case "~1":
@@ -7561,45 +7616,45 @@
                 w = t(2928),
                 S = t(3674),
                 x = t(1704),
                 O = "[object Arguments]",
                 j = "[object Function]",
                 _ = "[object Object]",
                 F = {};
-            F[O] = F["[object Array]"] = F["[object ArrayBuffer]"] = F["[object DataView]"] = F["[object Boolean]"] = F["[object Date]"] = F["[object Float32Array]"] = F["[object Float64Array]"] = F["[object Int8Array]"] = F["[object Int16Array]"] = F["[object Int32Array]"] = F["[object Map]"] = F["[object Number]"] = F[_] = F["[object RegExp]"] = F["[object Set]"] = F["[object String]"] = F["[object Symbol]"] = F["[object Uint8Array]"] = F["[object Uint8ClampedArray]"] = F["[object Uint16Array]"] = F["[object Uint32Array]"] = !0, F["[object Error]"] = F[j] = F["[object WeakMap]"] = !1, e.exports = function e(r, t, D, A, C, k) {
+            F[O] = F["[object Array]"] = F["[object ArrayBuffer]"] = F["[object DataView]"] = F["[object Boolean]"] = F["[object Date]"] = F["[object Float32Array]"] = F["[object Float64Array]"] = F["[object Int8Array]"] = F["[object Int16Array]"] = F["[object Int32Array]"] = F["[object Map]"] = F["[object Number]"] = F[_] = F["[object RegExp]"] = F["[object Set]"] = F["[object String]"] = F["[object Symbol]"] = F["[object Uint8Array]"] = F["[object Uint8ClampedArray]"] = F["[object Uint16Array]"] = F["[object Uint32Array]"] = !0, F["[object Error]"] = F[j] = F["[object WeakMap]"] = !1, e.exports = function e(r, t, A, D, C, k) {
                 var $, R = 1 & t,
                     I = 2 & t,
                     N = 4 & t;
-                if (D && ($ = C ? D(r, A, C, k) : D(r)), void 0 !== $) return $;
+                if (A && ($ = C ? A(r, D, C, k) : A(r)), void 0 !== $) return $;
                 if (!P(r)) return r;
                 var T = g(r);
                 if (T) {
                     if ($ = m(r), !R) return l(r, $)
                 } else {
                     var q = h(r),
-                        L = q == j || "[object GeneratorFunction]" == q;
+                        U = q == j || "[object GeneratorFunction]" == q;
                     if (b(r)) return u(r, R);
-                    if (q == _ || q == O || L && !C) {
-                        if ($ = I || L ? {} : y(r), !R) return I ? d(r, s($, r)) : c(r, i($, r))
+                    if (q == _ || q == O || U && !C) {
+                        if ($ = I || U ? {} : y(r), !R) return I ? d(r, s($, r)) : c(r, i($, r))
                     } else {
                         if (!F[q]) return C ? r : {};
                         $ = v(r, q, R)
                     }
                 }
                 k || (k = new a);
-                var U = k.get(r);
-                if (U) return U;
+                var L = k.get(r);
+                if (L) return L;
                 k.set(r, $), w(r) ? r.forEach((function(a) {
-                    $.add(e(a, t, D, a, r, k))
+                    $.add(e(a, t, A, a, r, k))
                 })) : E(r) && r.forEach((function(a, o) {
-                    $.set(o, e(a, t, D, o, r, k))
+                    $.set(o, e(a, t, A, o, r, k))
                 }));
                 var M = T ? void 0 : (N ? I ? p : f : I ? x : S)(r);
                 return o(M || r, (function(a, o) {
-                    M && (a = r[o = a]), n($, o, e(a, t, D, o, r, k))
+                    M && (a = r[o = a]), n($, o, e(a, t, A, o, r, k))
                 })), $
             }
         },
         731: (e, r, t) => {
             var a = t(8668),
                 o = t(7443),
                 n = t(1196),
@@ -8422,72 +8477,14 @@
         5697: (e, r, t) => {
             e.exports = t(2703)()
         },
         414: e => {
             "use strict";
             e.exports = "SECRET_DO_NOT_PASS_THIS_OR_YOU_WILL_BE_FIRED"
         },
-        9921: (e, r) => {
-            "use strict";
-            var t = "function" == typeof Symbol && Symbol.for,
-                a = t ? Symbol.for("react.element") : 60103,
-                o = t ? Symbol.for("react.portal") : 60106,
-                n = t ? Symbol.for("react.fragment") : 60107,
-                i = t ? Symbol.for("react.strict_mode") : 60108,
-                s = t ? Symbol.for("react.profiler") : 60114,
-                u = t ? Symbol.for("react.provider") : 60109,
-                l = t ? Symbol.for("react.context") : 60110,
-                c = t ? Symbol.for("react.async_mode") : 60111,
-                d = t ? Symbol.for("react.concurrent_mode") : 60111,
-                f = t ? Symbol.for("react.forward_ref") : 60112,
-                p = t ? Symbol.for("react.suspense") : 60113,
-                h = (t && Symbol.for("react.suspense_list"), t ? Symbol.for("react.memo") : 60115),
-                m = t ? Symbol.for("react.lazy") : 60116;
-            t && Symbol.for("react.fundamental"), t && Symbol.for("react.responder");
-
-            function v(e) {
-                if ("object" == typeof e && null !== e) {
-                    var r = e.$$typeof;
-                    switch (r) {
-                        case a:
-                            switch (e = e.type) {
-                                case c:
-                                case d:
-                                case n:
-                                case s:
-                                case i:
-                                case p:
-                                    return e;
-                                default:
-                                    switch (e = e && e.$$typeof) {
-                                        case l:
-                                        case f:
-                                        case u:
-                                            return e;
-                                        default:
-                                            return r
-                                    }
-                            }
-                        case m:
-                        case h:
-                        case o:
-                            return r
-                    }
-                }
-            }
-            r.isForwardRef = function(e) {
-                return v(e) === f
-            }, r.isMemo = function(e) {
-                return v(e) === h
-            }
-        },
-        9864: (e, r, t) => {
-            "use strict";
-            e.exports = t(9921)
-        },
         540: function(e, r) {
             ! function(e) {
                 "use strict";
 
                 function r() {
                     for (var e = arguments.length, r = Array(e), t = 0; t < e; t++) r[t] = arguments[t];
                     if (r.length > 1) {
@@ -8533,36 +8530,36 @@
                         w = t(t(t(m + "\\:") + "{0,3}" + m) + "?\\:\\:" + m + "\\:" + v),
                         S = t(t(t(m + "\\:") + "{0,4}" + m) + "?\\:\\:" + v),
                         x = t(t(t(m + "\\:") + "{0,5}" + m) + "?\\:\\:" + m),
                         O = t(t(t(m + "\\:") + "{0,6}" + m) + "?\\:\\:"),
                         j = t([y, g, b, E, P, w, S, x, O].join("|")),
                         _ = t(t(c + "|" + i) + "+"),
                         F = (t(j + "\\%25" + _), t(j + t("\\%25|\\%(?!" + n + "{2})") + _)),
-                        D = t("[vV]" + n + "+\\." + r(c, s, "[\\:]") + "+"),
-                        A = t("\\[" + t(F + "|" + j + "|" + D) + "\\]"),
+                        A = t("[vV]" + n + "+\\." + r(c, s, "[\\:]") + "+"),
+                        D = t("\\[" + t(F + "|" + j + "|" + A) + "\\]"),
                         C = t(t(i + "|" + r(c, s)) + "*"),
-                        k = t(A + "|" + h + "(?!" + C + ")|" + C),
+                        k = t(D + "|" + h + "(?!" + C + ")|" + C),
                         $ = t(o + "*"),
                         R = t(t(f + "@") + "?" + k + t("\\:" + $) + "?"),
                         I = t(i + "|" + r(c, s, "[\\:\\@]")),
                         N = t(I + "*"),
                         T = t(I + "+"),
                         q = t(t(i + "|" + r(c, s, "[\\@]")) + "+"),
-                        L = t(t("\\/" + N) + "*"),
-                        U = t("\\/" + t(T + L) + "?"),
-                        M = t(q + L),
-                        V = t(T + L),
+                        U = t(t("\\/" + N) + "*"),
+                        L = t("\\/" + t(T + U) + "?"),
+                        M = t(q + U),
+                        V = t(T + U),
                         z = "(?!" + I + ")",
-                        B = (t(L + "|" + U + "|" + M + "|" + V + "|" + z), t(t(I + "|" + r("[\\/\\?]", l)) + "*")),
+                        B = (t(U + "|" + L + "|" + M + "|" + V + "|" + z), t(t(I + "|" + r("[\\/\\?]", l)) + "*")),
                         W = t(t(I + "|[\\/\\?]") + "*"),
-                        Q = t(t("\\/\\/" + R + L) + "|" + U + "|" + V + "|" + z),
+                        Q = t(t("\\/\\/" + R + U) + "|" + L + "|" + V + "|" + z),
                         H = t(d + "\\:" + Q + t("\\?" + B) + "?" + t("\\#" + W) + "?"),
-                        K = t(t("\\/\\/" + R + L) + "|" + U + "|" + M + "|" + z),
+                        K = t(t("\\/\\/" + R + U) + "|" + L + "|" + M + "|" + z),
                         J = t(K + t("\\?" + B) + "?" + t("\\#" + W) + "?");
-                    return t(H + "|" + J), t(d + "\\:" + Q + t("\\?" + B) + "?"), t(t("\\/\\/(" + t("(" + f + ")@") + "?(" + k + ")" + t("\\:(" + $ + ")") + "?)") + "?(" + L + "|" + U + "|" + V + "|" + z + ")"), t("\\?(" + B + ")"), t("\\#(" + W + ")"), t(t("\\/\\/(" + t("(" + f + ")@") + "?(" + k + ")" + t("\\:(" + $ + ")") + "?)") + "?(" + L + "|" + U + "|" + M + "|" + z + ")"), t("\\?(" + B + ")"), t("\\#(" + W + ")"), t(t("\\/\\/(" + t("(" + f + ")@") + "?(" + k + ")" + t("\\:(" + $ + ")") + "?)") + "?(" + L + "|" + U + "|" + V + "|" + z + ")"), t("\\?(" + B + ")"), t("\\#(" + W + ")"), t("(" + f + ")@"), t("\\:(" + $ + ")"), {
+                    return t(H + "|" + J), t(d + "\\:" + Q + t("\\?" + B) + "?"), t(t("\\/\\/(" + t("(" + f + ")@") + "?(" + k + ")" + t("\\:(" + $ + ")") + "?)") + "?(" + U + "|" + L + "|" + V + "|" + z + ")"), t("\\?(" + B + ")"), t("\\#(" + W + ")"), t(t("\\/\\/(" + t("(" + f + ")@") + "?(" + k + ")" + t("\\:(" + $ + ")") + "?)") + "?(" + U + "|" + L + "|" + M + "|" + z + ")"), t("\\?(" + B + ")"), t("\\#(" + W + ")"), t(t("\\/\\/(" + t("(" + f + ")@") + "?(" + k + ")" + t("\\:(" + $ + ")") + "?)") + "?(" + U + "|" + L + "|" + V + "|" + z + ")"), t("\\?(" + B + ")"), t("\\#(" + W + ")"), t("(" + f + ")@"), t("\\:(" + $ + ")"), {
                         NOT_SCHEME: new RegExp(r("[^]", a, o, "[\\+\\-\\.]"), "g"),
                         NOT_USERINFO: new RegExp(r("[^\\%\\:]", c, s), "g"),
                         NOT_HOST: new RegExp(r("[^\\%\\[\\]\\:]", c, s), "g"),
                         NOT_PATH: new RegExp(r("[^\\%\\/\\:\\@]", c, s), "g"),
                         NOT_PATH_NOSCHEME: new RegExp(r("[^\\%\\/\\@]", c, s), "g"),
                         NOT_QUERY: new RegExp(r("[^\\%]", c, s, "[\\:\\@\\/\\?]", l), "g"),
                         NOT_FRAGMENT: new RegExp(r("[^\\%]", c, s, "[\\:\\@\\/\\?]"), "g"),
@@ -8706,63 +8703,80 @@
                             } finally {
                                 try {
                                     !S && _.return && _.return()
                                 } finally {
                                     if (x) throw O
                                 }
                             }
-                            var D = g + 1;
-                            w - a > m((l - o) / D) && y("overflow"), o += (w - a) * D, a = w;
-                            var A = !0,
+                            var A = g + 1;
+                            w - a > m((l - o) / A) && y("overflow"), o += (w - a) * A, a = w;
+                            var D = !0,
                                 C = !1,
                                 k = void 0;
                             try {
-                                for (var $, R = e[Symbol.iterator](); !(A = ($ = R.next()).done); A = !0) {
+                                for (var $, R = e[Symbol.iterator](); !(D = ($ = R.next()).done); D = !0) {
                                     var I = $.value;
                                     if (I < a && ++o > l && y("overflow"), I == a) {
                                         for (var N = o, T = c;; T += c) {
                                             var q = T <= n ? 1 : T >= n + 26 ? 26 : T - n;
                                             if (N < q) break;
-                                            var L = N - q,
-                                                U = c - q;
-                                            r.push(v(E(q + L % U, 0))), N = m(L / U)
+                                            var U = N - q,
+                                                L = c - q;
+                                            r.push(v(E(q + U % L, 0))), N = m(U / L)
                                         }
-                                        r.push(v(E(N, 0))), n = P(o, D, g == h), o = 0, ++g
+                                        r.push(v(E(N, 0))), n = P(o, A, g == h), o = 0, ++g
                                     }
                                 }
                             } catch (e) {
                                 C = !0, k = e
                             } finally {
                                 try {
-                                    !A && R.return && R.return()
+                                    !D && R.return && R.return()
                                 } finally {
                                     if (C) throw k
                                 }
                             }++o, ++a
                         }
                         return r.join("")
                     },
-                    x = function(e) {
-                        return g(e, (function(e) {
-                            return f.test(e) ? "xn--" + S(e) : e
-                        }))
-                    },
-                    O = function(e) {
-                        return g(e, (function(e) {
-                            return d.test(e) ? w(e.slice(4).toLowerCase()) : e
-                        }))
+                    x = {
+                        version: "2.1.0",
+                        ucs2: {
+                            decode: b,
+                            encode: function(e) {
+                                return String.fromCodePoint.apply(String, function(e) {
+                                    if (Array.isArray(e)) {
+                                        for (var r = 0, t = Array(e.length); r < e.length; r++) t[r] = e[r];
+                                        return t
+                                    }
+                                    return Array.from(e)
+                                }(e))
+                            }
+                        },
+                        decode: w,
+                        encode: S,
+                        toASCII: function(e) {
+                            return g(e, (function(e) {
+                                return f.test(e) ? "xn--" + S(e) : e
+                            }))
+                        },
+                        toUnicode: function(e) {
+                            return g(e, (function(e) {
+                                return d.test(e) ? w(e.slice(4).toLowerCase()) : e
+                            }))
+                        }
                     },
-                    j = {};
+                    O = {};
 
-                function _(e) {
+                function j(e) {
                     var r = e.charCodeAt(0);
                     return r < 16 ? "%0" + r.toString(16).toUpperCase() : r < 128 ? "%" + r.toString(16).toUpperCase() : r < 2048 ? "%" + (r >> 6 | 192).toString(16).toUpperCase() + "%" + (63 & r | 128).toString(16).toUpperCase() : "%" + (r >> 12 | 224).toString(16).toUpperCase() + "%" + (r >> 6 & 63 | 128).toString(16).toUpperCase() + "%" + (63 & r | 128).toString(16).toUpperCase()
                 }
 
-                function F(e) {
+                function _(e) {
                     for (var r = "", t = 0, a = e.length; t < a;) {
                         var o = parseInt(e.substr(t + 1, 2), 16);
                         if (o < 128) r += String.fromCharCode(o), t += 3;
                         else if (o >= 194 && o < 224) {
                             if (a - t >= 6) {
                                 var n = parseInt(e.substr(t + 4, 2), 16);
                                 r += String.fromCharCode((31 & o) << 6 | 63 & n)
@@ -8776,40 +8790,40 @@
                             } else r += e.substr(t, 9);
                             t += 9
                         } else r += e.substr(t, 3), t += 3
                     }
                     return r
                 }
 
-                function D(e, r) {
+                function F(e, r) {
                     function t(e) {
-                        var t = F(e);
+                        var t = _(e);
                         return t.match(r.UNRESERVED) ? t : e
                     }
-                    return e.scheme && (e.scheme = String(e.scheme).replace(r.PCT_ENCODED, t).toLowerCase().replace(r.NOT_SCHEME, "")), void 0 !== e.userinfo && (e.userinfo = String(e.userinfo).replace(r.PCT_ENCODED, t).replace(r.NOT_USERINFO, _).replace(r.PCT_ENCODED, o)), void 0 !== e.host && (e.host = String(e.host).replace(r.PCT_ENCODED, t).toLowerCase().replace(r.NOT_HOST, _).replace(r.PCT_ENCODED, o)), void 0 !== e.path && (e.path = String(e.path).replace(r.PCT_ENCODED, t).replace(e.scheme ? r.NOT_PATH : r.NOT_PATH_NOSCHEME, _).replace(r.PCT_ENCODED, o)), void 0 !== e.query && (e.query = String(e.query).replace(r.PCT_ENCODED, t).replace(r.NOT_QUERY, _).replace(r.PCT_ENCODED, o)), void 0 !== e.fragment && (e.fragment = String(e.fragment).replace(r.PCT_ENCODED, t).replace(r.NOT_FRAGMENT, _).replace(r.PCT_ENCODED, o)), e
+                    return e.scheme && (e.scheme = String(e.scheme).replace(r.PCT_ENCODED, t).toLowerCase().replace(r.NOT_SCHEME, "")), void 0 !== e.userinfo && (e.userinfo = String(e.userinfo).replace(r.PCT_ENCODED, t).replace(r.NOT_USERINFO, j).replace(r.PCT_ENCODED, o)), void 0 !== e.host && (e.host = String(e.host).replace(r.PCT_ENCODED, t).toLowerCase().replace(r.NOT_HOST, j).replace(r.PCT_ENCODED, o)), void 0 !== e.path && (e.path = String(e.path).replace(r.PCT_ENCODED, t).replace(e.scheme ? r.NOT_PATH : r.NOT_PATH_NOSCHEME, j).replace(r.PCT_ENCODED, o)), void 0 !== e.query && (e.query = String(e.query).replace(r.PCT_ENCODED, t).replace(r.NOT_QUERY, j).replace(r.PCT_ENCODED, o)), void 0 !== e.fragment && (e.fragment = String(e.fragment).replace(r.PCT_ENCODED, t).replace(r.NOT_FRAGMENT, j).replace(r.PCT_ENCODED, o)), e
                 }
 
                 function A(e) {
                     return e.replace(/^0*(.*)/, "$1") || "0"
                 }
 
-                function C(e, r) {
+                function D(e, r) {
                     var t = e.match(r.IPV4ADDRESS) || [],
                         a = u(t, 2)[1];
                     return a ? a.split(".").map(A).join(".") : e
                 }
 
-                function k(e, r) {
+                function C(e, r) {
                     var t = e.match(r.IPV6ADDRESS) || [],
                         a = u(t, 3),
                         o = a[1],
                         n = a[2];
                     if (o) {
                         for (var i = o.toLowerCase().split("::").reverse(), s = u(i, 2), l = s[0], c = s[1], d = c ? c.split(":").map(A) : [], f = l.split(":").map(A), p = r.IPV4ADDRESS.test(f[f.length - 1]), h = p ? 7 : 8, m = f.length - h, v = Array(h), y = 0; y < h; ++y) v[y] = d[y] || f[m + y] || "";
-                        p && (v[h - 1] = C(v[h - 1], r));
+                        p && (v[h - 1] = D(v[h - 1], r));
                         var g = v.reduce((function(e, r, t) {
                                 if (!r || "0" === r) {
                                     var a = e[e.length - 1];
                                     a && a.index + a.length === t ? a.length++ : e.push({
                                         index: t,
                                         length: 1
                                     })
@@ -8824,275 +8838,273 @@
                                 P = v.slice(g.index + g.length);
                             b = E.join(":") + "::" + P.join(":")
                         } else b = v.join(":");
                         return n && (b += "%" + n), b
                     }
                     return e
                 }
-                var $ = /^(?:([^:\/?#]+):)?(?:\/\/((?:([^\/?#@]*)@)?(\[[^\/?#\]]+\]|[^\/?#:]*)(?:\:(\d*))?))?([^?#]*)(?:\?([^#]*))?(?:#((?:.|\n|\r)*))?/i,
-                    R = void 0 === "".match(/(){0}/)[1];
+                var k = /^(?:([^:\/?#]+):)?(?:\/\/((?:([^\/?#@]*)@)?(\[[^\/?#\]]+\]|[^\/?#:]*)(?:\:(\d*))?))?([^?#]*)(?:\?([^#]*))?(?:#((?:.|\n|\r)*))?/i,
+                    $ = void 0 === "".match(/(){0}/)[1];
 
-                function I(e) {
+                function R(e) {
                     var r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                         t = {},
                         a = !1 !== r.iri ? s : i;
                     "suffix" === r.reference && (e = (r.scheme ? r.scheme + ":" : "") + "//" + e);
-                    var o = e.match($);
+                    var o = e.match(k);
                     if (o) {
-                        R ? (t.scheme = o[1], t.userinfo = o[3], t.host = o[4], t.port = parseInt(o[5], 10), t.path = o[6] || "", t.query = o[7], t.fragment = o[8], isNaN(t.port) && (t.port = o[5])) : (t.scheme = o[1] || void 0, t.userinfo = -1 !== e.indexOf("@") ? o[3] : void 0, t.host = -1 !== e.indexOf("//") ? o[4] : void 0, t.port = parseInt(o[5], 10), t.path = o[6] || "", t.query = -1 !== e.indexOf("?") ? o[7] : void 0, t.fragment = -1 !== e.indexOf("#") ? o[8] : void 0, isNaN(t.port) && (t.port = e.match(/\/\/(?:.|\n)*\:(?:\/|\?|\#|$)/) ? o[4] : void 0)), t.host && (t.host = k(C(t.host, a), a)), void 0 !== t.scheme || void 0 !== t.userinfo || void 0 !== t.host || void 0 !== t.port || t.path || void 0 !== t.query ? void 0 === t.scheme ? t.reference = "relative" : void 0 === t.fragment ? t.reference = "absolute" : t.reference = "uri" : t.reference = "same-document", r.reference && "suffix" !== r.reference && r.reference !== t.reference && (t.error = t.error || "URI is not a " + r.reference + " reference.");
-                        var n = j[(r.scheme || t.scheme || "").toLowerCase()];
-                        if (r.unicodeSupport || n && n.unicodeSupport) D(t, a);
+                        $ ? (t.scheme = o[1], t.userinfo = o[3], t.host = o[4], t.port = parseInt(o[5], 10), t.path = o[6] || "", t.query = o[7], t.fragment = o[8], isNaN(t.port) && (t.port = o[5])) : (t.scheme = o[1] || void 0, t.userinfo = -1 !== e.indexOf("@") ? o[3] : void 0, t.host = -1 !== e.indexOf("//") ? o[4] : void 0, t.port = parseInt(o[5], 10), t.path = o[6] || "", t.query = -1 !== e.indexOf("?") ? o[7] : void 0, t.fragment = -1 !== e.indexOf("#") ? o[8] : void 0, isNaN(t.port) && (t.port = e.match(/\/\/(?:.|\n)*\:(?:\/|\?|\#|$)/) ? o[4] : void 0)), t.host && (t.host = C(D(t.host, a), a)), void 0 !== t.scheme || void 0 !== t.userinfo || void 0 !== t.host || void 0 !== t.port || t.path || void 0 !== t.query ? void 0 === t.scheme ? t.reference = "relative" : void 0 === t.fragment ? t.reference = "absolute" : t.reference = "uri" : t.reference = "same-document", r.reference && "suffix" !== r.reference && r.reference !== t.reference && (t.error = t.error || "URI is not a " + r.reference + " reference.");
+                        var n = O[(r.scheme || t.scheme || "").toLowerCase()];
+                        if (r.unicodeSupport || n && n.unicodeSupport) F(t, a);
                         else {
                             if (t.host && (r.domainHost || n && n.domainHost)) try {
-                                t.host = x(t.host.replace(a.PCT_ENCODED, F).toLowerCase())
+                                t.host = x.toASCII(t.host.replace(a.PCT_ENCODED, _).toLowerCase())
                             } catch (e) {
                                 t.error = t.error || "Host's domain name can not be converted to ASCII via punycode: " + e
                             }
-                            D(t, i)
+                            F(t, i)
                         }
                         n && n.parse && n.parse(t, r)
                     } else t.error = t.error || "URI can not be parsed.";
                     return t
                 }
+                var I = /^\.\.?\//,
+                    N = /^\/\.(\/|$)/,
+                    T = /^\/\.\.(\/|$)/,
+                    q = /^\/?(?:.|\n)*?(?=\/|$)/;
 
-                function N(e, r) {
-                    var t = !1 !== r.iri ? s : i,
-                        a = [];
-                    return void 0 !== e.userinfo && (a.push(e.userinfo), a.push("@")), void 0 !== e.host && a.push(k(C(String(e.host), t), t).replace(t.IPV6ADDRESS, (function(e, r, t) {
-                        return "[" + r + (t ? "%25" + t : "") + "]"
-                    }))), "number" != typeof e.port && "string" != typeof e.port || (a.push(":"), a.push(String(e.port))), a.length ? a.join("") : void 0
-                }
-                var T = /^\.\.?\//,
-                    q = /^\/\.(\/|$)/,
-                    L = /^\/\.\.(\/|$)/,
-                    U = /^\/?(?:.|\n)*?(?=\/|$)/;
-
-                function M(e) {
+                function U(e) {
                     for (var r = []; e.length;)
-                        if (e.match(T)) e = e.replace(T, "");
-                        else if (e.match(q)) e = e.replace(q, "/");
-                    else if (e.match(L)) e = e.replace(L, "/"), r.pop();
+                        if (e.match(I)) e = e.replace(I, "");
+                        else if (e.match(N)) e = e.replace(N, "/");
+                    else if (e.match(T)) e = e.replace(T, "/"), r.pop();
                     else if ("." === e || ".." === e) e = "";
                     else {
-                        var t = e.match(U);
+                        var t = e.match(q);
                         if (!t) throw new Error("Unexpected dot segment condition");
                         var a = t[0];
                         e = e.slice(a.length), r.push(a)
                     }
                     return r.join("")
                 }
 
-                function V(e) {
+                function L(e) {
                     var r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                         t = r.iri ? s : i,
                         a = [],
-                        o = j[(r.scheme || e.scheme || "").toLowerCase()];
+                        o = O[(r.scheme || e.scheme || "").toLowerCase()];
                     if (o && o.serialize && o.serialize(e, r), e.host)
                         if (t.IPV6ADDRESS.test(e.host));
                         else if (r.domainHost || o && o.domainHost) try {
-                        e.host = r.iri ? O(e.host) : x(e.host.replace(t.PCT_ENCODED, F).toLowerCase())
+                        e.host = r.iri ? x.toUnicode(e.host) : x.toASCII(e.host.replace(t.PCT_ENCODED, _).toLowerCase())
                     } catch (t) {
                         e.error = e.error || "Host's domain name can not be converted to " + (r.iri ? "Unicode" : "ASCII") + " via punycode: " + t
                     }
-                    D(e, t), "suffix" !== r.reference && e.scheme && (a.push(e.scheme), a.push(":"));
-                    var n = N(e, r);
+                    F(e, t), "suffix" !== r.reference && e.scheme && (a.push(e.scheme), a.push(":"));
+                    var n = function(e, r) {
+                        var t = !1 !== r.iri ? s : i,
+                            a = [];
+                        return void 0 !== e.userinfo && (a.push(e.userinfo), a.push("@")), void 0 !== e.host && a.push(C(D(String(e.host), t), t).replace(t.IPV6ADDRESS, (function(e, r, t) {
+                            return "[" + r + (t ? "%25" + t : "") + "]"
+                        }))), "number" != typeof e.port && "string" != typeof e.port || (a.push(":"), a.push(String(e.port))), a.length ? a.join("") : void 0
+                    }(e, r);
                     if (void 0 !== n && ("suffix" !== r.reference && a.push("//"), a.push(n), e.path && "/" !== e.path.charAt(0) && a.push("/")), void 0 !== e.path) {
                         var u = e.path;
-                        r.absolutePath || o && o.absolutePath || (u = M(u)), void 0 === n && (u = u.replace(/^\/\//, "/%2F")), a.push(u)
+                        r.absolutePath || o && o.absolutePath || (u = U(u)), void 0 === n && (u = u.replace(/^\/\//, "/%2F")), a.push(u)
                     }
                     return void 0 !== e.query && (a.push("?"), a.push(e.query)), void 0 !== e.fragment && (a.push("#"), a.push(e.fragment)), a.join("")
                 }
 
-                function z(e, r) {
+                function M(e, r) {
                     var t = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {},
                         a = {};
-                    return arguments[3] || (e = I(V(e, t), t), r = I(V(r, t), t)), !(t = t || {}).tolerant && r.scheme ? (a.scheme = r.scheme, a.userinfo = r.userinfo, a.host = r.host, a.port = r.port, a.path = M(r.path || ""), a.query = r.query) : (void 0 !== r.userinfo || void 0 !== r.host || void 0 !== r.port ? (a.userinfo = r.userinfo, a.host = r.host, a.port = r.port, a.path = M(r.path || ""), a.query = r.query) : (r.path ? ("/" === r.path.charAt(0) ? a.path = M(r.path) : (void 0 === e.userinfo && void 0 === e.host && void 0 === e.port || e.path ? e.path ? a.path = e.path.slice(0, e.path.lastIndexOf("/") + 1) + r.path : a.path = r.path : a.path = "/" + r.path, a.path = M(a.path)), a.query = r.query) : (a.path = e.path, void 0 !== r.query ? a.query = r.query : a.query = e.query), a.userinfo = e.userinfo, a.host = e.host, a.port = e.port), a.scheme = e.scheme), a.fragment = r.fragment, a
+                    return arguments[3] || (e = R(L(e, t), t), r = R(L(r, t), t)), !(t = t || {}).tolerant && r.scheme ? (a.scheme = r.scheme, a.userinfo = r.userinfo, a.host = r.host, a.port = r.port, a.path = U(r.path || ""), a.query = r.query) : (void 0 !== r.userinfo || void 0 !== r.host || void 0 !== r.port ? (a.userinfo = r.userinfo, a.host = r.host, a.port = r.port, a.path = U(r.path || ""), a.query = r.query) : (r.path ? ("/" === r.path.charAt(0) ? a.path = U(r.path) : (void 0 === e.userinfo && void 0 === e.host && void 0 === e.port || e.path ? e.path ? a.path = e.path.slice(0, e.path.lastIndexOf("/") + 1) + r.path : a.path = r.path : a.path = "/" + r.path, a.path = U(a.path)), a.query = r.query) : (a.path = e.path, void 0 !== r.query ? a.query = r.query : a.query = e.query), a.userinfo = e.userinfo, a.host = e.host, a.port = e.port), a.scheme = e.scheme), a.fragment = r.fragment, a
                 }
 
-                function B(e, r) {
-                    return e && e.toString().replace(r && r.iri ? s.PCT_ENCODED : i.PCT_ENCODED, F)
+                function V(e, r) {
+                    return e && e.toString().replace(r && r.iri ? s.PCT_ENCODED : i.PCT_ENCODED, _)
                 }
-                var W = {
+                var z = {
                         scheme: "http",
                         domainHost: !0,
                         parse: function(e, r) {
                             return e.host || (e.error = e.error || "HTTP URIs must have a host."), e
                         },
                         serialize: function(e, r) {
                             var t = "https" === String(e.scheme).toLowerCase();
                             return e.port !== (t ? 443 : 80) && "" !== e.port || (e.port = void 0), e.path || (e.path = "/"), e
                         }
                     },
-                    Q = {
+                    B = {
                         scheme: "https",
-                        domainHost: W.domainHost,
-                        parse: W.parse,
-                        serialize: W.serialize
+                        domainHost: z.domainHost,
+                        parse: z.parse,
+                        serialize: z.serialize
                     };
 
-                function H(e) {
+                function W(e) {
                     return "boolean" == typeof e.secure ? e.secure : "wss" === String(e.scheme).toLowerCase()
                 }
-                var K = {
+                var Q = {
                         scheme: "ws",
                         domainHost: !0,
                         parse: function(e, r) {
                             var t = e;
-                            return t.secure = H(t), t.resourceName = (t.path || "/") + (t.query ? "?" + t.query : ""), t.path = void 0, t.query = void 0, t
+                            return t.secure = W(t), t.resourceName = (t.path || "/") + (t.query ? "?" + t.query : ""), t.path = void 0, t.query = void 0, t
                         },
                         serialize: function(e, r) {
-                            if (e.port !== (H(e) ? 443 : 80) && "" !== e.port || (e.port = void 0), "boolean" == typeof e.secure && (e.scheme = e.secure ? "wss" : "ws", e.secure = void 0), e.resourceName) {
+                            if (e.port !== (W(e) ? 443 : 80) && "" !== e.port || (e.port = void 0), "boolean" == typeof e.secure && (e.scheme = e.secure ? "wss" : "ws", e.secure = void 0), e.resourceName) {
                                 var t = e.resourceName.split("?"),
                                     a = u(t, 2),
                                     o = a[0],
                                     n = a[1];
                                 e.path = o && "/" !== o ? o : void 0, e.query = n, e.resourceName = void 0
                             }
                             return e.fragment = void 0, e
                         }
                     },
-                    J = {
+                    H = {
                         scheme: "wss",
-                        domainHost: K.domainHost,
-                        parse: K.parse,
-                        serialize: K.serialize
-                    },
-                    Z = {},
-                    Y = "[A-Za-z0-9\\-\\.\\_\\~\\xA0-\\u200D\\u2010-\\u2029\\u202F-\\uD7FF\\uF900-\\uFDCF\\uFDF0-\\uFFEF]",
-                    G = "[0-9A-Fa-f]",
-                    X = t(t("%[EFef]" + G + "%" + G + G + "%" + G + G) + "|" + t("%[89A-Fa-f]" + G + "%" + G + G) + "|" + t("%" + G + G)),
-                    ee = r("[\\!\\$\\%\\'\\(\\)\\*\\+\\,\\-\\.0-9\\<\\>A-Z\\x5E-\\x7E]", '[\\"\\\\]'),
-                    re = new RegExp(Y, "g"),
-                    te = new RegExp(X, "g"),
-                    ae = new RegExp(r("[^]", "[A-Za-z0-9\\!\\$\\%\\'\\*\\+\\-\\^\\_\\`\\{\\|\\}\\~]", "[\\.]", '[\\"]', ee), "g"),
-                    oe = new RegExp(r("[^]", Y, "[\\!\\$\\'\\(\\)\\*\\+\\,\\;\\:\\@]"), "g"),
-                    ne = oe;
-
-                function ie(e) {
-                    var r = F(e);
-                    return r.match(re) ? r : e
+                        domainHost: Q.domainHost,
+                        parse: Q.parse,
+                        serialize: Q.serialize
+                    },
+                    K = {},
+                    J = "[A-Za-z0-9\\-\\.\\_\\~\\xA0-\\u200D\\u2010-\\u2029\\u202F-\\uD7FF\\uF900-\\uFDCF\\uFDF0-\\uFFEF]",
+                    Z = "[0-9A-Fa-f]",
+                    Y = t(t("%[EFef]" + Z + "%" + Z + Z + "%" + Z + Z) + "|" + t("%[89A-Fa-f]" + Z + "%" + Z + Z) + "|" + t("%" + Z + Z)),
+                    G = r("[\\!\\$\\%\\'\\(\\)\\*\\+\\,\\-\\.0-9\\<\\>A-Z\\x5E-\\x7E]", '[\\"\\\\]'),
+                    X = new RegExp(J, "g"),
+                    ee = new RegExp(Y, "g"),
+                    re = new RegExp(r("[^]", "[A-Za-z0-9\\!\\$\\%\\'\\*\\+\\-\\^\\_\\`\\{\\|\\}\\~]", "[\\.]", '[\\"]', G), "g"),
+                    te = new RegExp(r("[^]", J, "[\\!\\$\\'\\(\\)\\*\\+\\,\\;\\:\\@]"), "g"),
+                    ae = te;
+
+                function oe(e) {
+                    var r = _(e);
+                    return r.match(X) ? r : e
                 }
-                var se = {
+                var ne = {
                         scheme: "mailto",
                         parse: function(e, r) {
                             var t = e,
                                 a = t.to = t.path ? t.path.split(",") : [];
                             if (t.path = void 0, t.query) {
                                 for (var o = !1, n = {}, i = t.query.split("&"), s = 0, u = i.length; s < u; ++s) {
                                     var l = i[s].split("=");
                                     switch (l[0]) {
                                         case "to":
                                             for (var c = l[1].split(","), d = 0, f = c.length; d < f; ++d) a.push(c[d]);
                                             break;
                                         case "subject":
-                                            t.subject = B(l[1], r);
+                                            t.subject = V(l[1], r);
                                             break;
                                         case "body":
-                                            t.body = B(l[1], r);
+                                            t.body = V(l[1], r);
                                             break;
                                         default:
-                                            o = !0, n[B(l[0], r)] = B(l[1], r)
+                                            o = !0, n[V(l[0], r)] = V(l[1], r)
                                     }
                                 }
                                 o && (t.headers = n)
                             }
                             t.query = void 0;
                             for (var p = 0, h = a.length; p < h; ++p) {
                                 var m = a[p].split("@");
-                                if (m[0] = B(m[0]), r.unicodeSupport) m[1] = B(m[1], r).toLowerCase();
+                                if (m[0] = V(m[0]), r.unicodeSupport) m[1] = V(m[1], r).toLowerCase();
                                 else try {
-                                    m[1] = x(B(m[1], r).toLowerCase())
+                                    m[1] = x.toASCII(V(m[1], r).toLowerCase())
                                 } catch (e) {
                                     t.error = t.error || "Email address's domain name can not be converted to ASCII via punycode: " + e
                                 }
                                 a[p] = m.join("@")
                             }
                             return t
                         },
                         serialize: function(e, r) {
                             var t, a = e,
                                 n = null != (t = e.to) ? t instanceof Array ? t : "number" != typeof t.length || t.split || t.setInterval || t.call ? [t] : Array.prototype.slice.call(t) : [];
                             if (n) {
                                 for (var i = 0, s = n.length; i < s; ++i) {
                                     var u = String(n[i]),
                                         l = u.lastIndexOf("@"),
-                                        c = u.slice(0, l).replace(te, ie).replace(te, o).replace(ae, _),
+                                        c = u.slice(0, l).replace(ee, oe).replace(ee, o).replace(re, j),
                                         d = u.slice(l + 1);
                                     try {
-                                        d = r.iri ? O(d) : x(B(d, r).toLowerCase())
+                                        d = r.iri ? x.toUnicode(d) : x.toASCII(V(d, r).toLowerCase())
                                     } catch (e) {
                                         a.error = a.error || "Email address's domain name can not be converted to " + (r.iri ? "Unicode" : "ASCII") + " via punycode: " + e
                                     }
                                     n[i] = c + "@" + d
                                 }
                                 a.path = n.join(",")
                             }
                             var f = e.headers = e.headers || {};
                             e.subject && (f.subject = e.subject), e.body && (f.body = e.body);
                             var p = [];
-                            for (var h in f) f[h] !== Z[h] && p.push(h.replace(te, ie).replace(te, o).replace(oe, _) + "=" + f[h].replace(te, ie).replace(te, o).replace(ne, _));
+                            for (var h in f) f[h] !== K[h] && p.push(h.replace(ee, oe).replace(ee, o).replace(te, j) + "=" + f[h].replace(ee, oe).replace(ee, o).replace(ae, j));
                             return p.length && (a.query = p.join("&")), a
                         }
                     },
-                    ue = /^([^\:]+)\:(.*)/,
-                    le = {
+                    ie = /^([^\:]+)\:(.*)/,
+                    se = {
                         scheme: "urn",
                         parse: function(e, r) {
-                            var t = e.path && e.path.match(ue),
+                            var t = e.path && e.path.match(ie),
                                 a = e;
                             if (t) {
                                 var o = r.scheme || a.scheme || "urn",
                                     n = t[1].toLowerCase(),
                                     i = t[2],
                                     s = o + ":" + (r.nid || n),
-                                    u = j[s];
+                                    u = O[s];
                                 a.nid = n, a.nss = i, a.path = void 0, u && (a = u.parse(a, r))
                             } else a.error = a.error || "URN can not be parsed.";
                             return a
                         },
                         serialize: function(e, r) {
                             var t = r.scheme || e.scheme || "urn",
                                 a = e.nid,
                                 o = t + ":" + (r.nid || a),
-                                n = j[o];
+                                n = O[o];
                             n && (e = n.serialize(e, r));
                             var i = e,
                                 s = e.nss;
                             return i.path = (a || r.nid) + ":" + s, i
                         }
                     },
-                    ce = /^[0-9A-Fa-f]{8}(?:\-[0-9A-Fa-f]{4}){3}\-[0-9A-Fa-f]{12}$/,
-                    de = {
+                    ue = /^[0-9A-Fa-f]{8}(?:\-[0-9A-Fa-f]{4}){3}\-[0-9A-Fa-f]{12}$/,
+                    le = {
                         scheme: "urn:uuid",
                         parse: function(e, r) {
                             var t = e;
-                            return t.uuid = t.nss, t.nss = void 0, r.tolerant || t.uuid && t.uuid.match(ce) || (t.error = t.error || "UUID is not valid."), t
+                            return t.uuid = t.nss, t.nss = void 0, r.tolerant || t.uuid && t.uuid.match(ue) || (t.error = t.error || "UUID is not valid."), t
                         },
                         serialize: function(e, r) {
                             var t = e;
                             return t.nss = (e.uuid || "").toLowerCase(), t
                         }
                     };
-                j[W.scheme] = W, j[Q.scheme] = Q, j[K.scheme] = K, j[J.scheme] = J, j[se.scheme] = se, j[le.scheme] = le, j[de.scheme] = de, e.SCHEMES = j, e.pctEncChar = _, e.pctDecChars = F, e.parse = I, e.removeDotSegments = M, e.serialize = V, e.resolveComponents = z, e.resolve = function(e, r, t) {
+                O[z.scheme] = z, O[B.scheme] = B, O[Q.scheme] = Q, O[H.scheme] = H, O[ne.scheme] = ne, O[se.scheme] = se, O[le.scheme] = le, e.SCHEMES = O, e.pctEncChar = j, e.pctDecChars = _, e.parse = R, e.removeDotSegments = U, e.serialize = L, e.resolveComponents = M, e.resolve = function(e, r, t) {
                     var a = function(e, r) {
                         var t = e;
                         if (r)
                             for (var a in r) t[a] = r[a];
                         return t
                     }({
                         scheme: "null"
                     }, t);
-                    return V(z(I(e, a), I(r, a), a, !0), a)
+                    return L(M(R(e, a), R(r, a), a, !0), a)
                 }, e.normalize = function(e, r) {
-                    return "string" == typeof e ? e = V(I(e, r), r) : "object" === a(e) && (e = I(V(e, r), r)), e
+                    return "string" == typeof e ? e = L(R(e, r), r) : "object" === a(e) && (e = R(L(e, r), r)), e
                 }, e.equal = function(e, r, t) {
-                    return "string" == typeof e ? e = V(I(e, t), t) : "object" === a(e) && (e = V(e, t)), "string" == typeof r ? r = V(I(r, t), t) : "object" === a(r) && (r = V(r, t)), e === r
+                    return "string" == typeof e ? e = L(R(e, t), t) : "object" === a(e) && (e = L(e, t)), "string" == typeof r ? r = L(R(r, t), t) : "object" === a(r) && (r = L(r, t)), e === r
                 }, e.escapeComponent = function(e, r) {
-                    return e && e.toString().replace(r && r.iri ? s.ESCAPE : i.ESCAPE, _)
-                }, e.unescapeComponent = B, Object.defineProperty(e, "__esModule", {
+                    return e && e.toString().replace(r && r.iri ? s.ESCAPE : i.ESCAPE, j)
+                }, e.unescapeComponent = V, Object.defineProperty(e, "__esModule", {
                     value: !0
                 })
             }(r)
         },
         4653: e => {
             "use strict";
             e.exports = Array.isArray || function(e) {
@@ -9127,17 +9139,17 @@
         },
         6953: e => {
             "use strict";
             e.exports = function(e) {
                 return ("number" == typeof e || "[object Number]" === Object.prototype.toString.call(e)) && e.valueOf() == e.valueOf()
             }
         },
-        894: e => {
+        6354: e => {
             "use strict";
             e.exports = JSON.parse('{"$schema":"http://json-schema.org/draft-07/schema#","$id":"https://raw.githubusercontent.com/ajv-validator/ajv/master/lib/refs/data.json#","description":"Meta-schema for $data reference (JSON Schema extension proposal)","type":"object","required":["$data"],"properties":{"$data":{"type":"string","anyOf":[{"format":"relative-json-pointer"},{"format":"json-pointer"}]}},"additionalProperties":false}')
         },
-        6680: e => {
+        6656: e => {
             "use strict";
             e.exports = JSON.parse('{"$schema":"http://json-schema.org/draft-07/schema#","$id":"http://json-schema.org/draft-07/schema#","title":"Core schema meta-schema","definitions":{"schemaArray":{"type":"array","minItems":1,"items":{"$ref":"#"}},"nonNegativeInteger":{"type":"integer","minimum":0},"nonNegativeIntegerDefault0":{"allOf":[{"$ref":"#/definitions/nonNegativeInteger"},{"default":0}]},"simpleTypes":{"enum":["array","boolean","integer","null","number","object","string"]},"stringArray":{"type":"array","items":{"type":"string"},"uniqueItems":true,"default":[]}},"type":["object","boolean"],"properties":{"$id":{"type":"string","format":"uri-reference"},"$schema":{"type":"string","format":"uri"},"$ref":{"type":"string","format":"uri-reference"},"$comment":{"type":"string"},"title":{"type":"string"},"description":{"type":"string"},"default":true,"readOnly":{"type":"boolean","default":false},"examples":{"type":"array","items":true},"multipleOf":{"type":"number","exclusiveMinimum":0},"maximum":{"type":"number"},"exclusiveMaximum":{"type":"number"},"minimum":{"type":"number"},"exclusiveMinimum":{"type":"number"},"maxLength":{"$ref":"#/definitions/nonNegativeInteger"},"minLength":{"$ref":"#/definitions/nonNegativeIntegerDefault0"},"pattern":{"type":"string","format":"regex"},"additionalItems":{"$ref":"#"},"items":{"anyOf":[{"$ref":"#"},{"$ref":"#/definitions/schemaArray"}],"default":true},"maxItems":{"$ref":"#/definitions/nonNegativeInteger"},"minItems":{"$ref":"#/definitions/nonNegativeIntegerDefault0"},"uniqueItems":{"type":"boolean","default":false},"contains":{"$ref":"#"},"maxProperties":{"$ref":"#/definitions/nonNegativeInteger"},"minProperties":{"$ref":"#/definitions/nonNegativeIntegerDefault0"},"required":{"$ref":"#/definitions/stringArray"},"additionalProperties":{"$ref":"#"},"definitions":{"type":"object","additionalProperties":{"$ref":"#"},"default":{}},"properties":{"type":"object","additionalProperties":{"$ref":"#"},"default":{}},"patternProperties":{"type":"object","additionalProperties":{"$ref":"#"},"propertyNames":{"format":"regex"},"default":{}},"dependencies":{"type":"object","additionalProperties":{"anyOf":[{"$ref":"#"},{"$ref":"#/definitions/stringArray"}]}},"propertyNames":{"$ref":"#"},"const":true,"enum":{"type":"array","items":true,"minItems":1,"uniqueItems":true},"type":{"anyOf":[{"$ref":"#/definitions/simpleTypes"},{"type":"array","items":{"$ref":"#/definitions/simpleTypes"},"minItems":1,"uniqueItems":true}]},"format":{"type":"string"},"contentMediaType":{"type":"string"},"contentEncoding":{"type":"string"},"if":{"$ref":"#"},"then":{"$ref":"#"},"else":{"$ref":"#"},"allOf":{"$ref":"#/definitions/schemaArray"},"anyOf":{"$ref":"#/definitions/schemaArray"},"oneOf":{"$ref":"#/definitions/schemaArray"},"not":{"$ref":"#"}},"default":true}')
         }
     }
 ]);
```

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/861.7c8ce849384f01571a74.js` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/861.7c8ce849384f01571a74.js`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/remoteEntry.bdf4fdb49ec09bfbe704.js` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/remoteEntry.f72e9c07a70775e21991.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, o, n, a, i, l, u, s, d, f, c, p, h, v, m, b, g = {
+    var e, r, t, o, n, a, i, l, f, u, s, d, c, p, h, v, m, b, g, y = {
             982: (e, r, t) => {
                 var o = {
-                        "./index": () => Promise.all([t.e(271), t.e(290)]).then((() => () => t(290))),
-                        "./extension": () => Promise.all([t.e(271), t.e(290)]).then((() => () => t(290))),
+                        "./index": () => Promise.all([t.e(29), t.e(535)]).then((() => () => t(3535))),
+                        "./extension": () => Promise.all([t.e(29), t.e(535)]).then((() => () => t(3535))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -21,129 +21,130 @@
                     };
                 t.d(r, {
                     get: () => n,
                     init: () => a
                 })
             }
         },
-        y = {};
+        j = {};
 
-    function j(e) {
-        var r = y[e];
+    function w(e) {
+        var r = j[e];
         if (void 0 !== r) return r.exports;
-        var t = y[e] = {
+        var t = j[e] = {
             id: e,
             loaded: !1,
             exports: {}
         };
-        return g[e].call(t.exports, t, t.exports, j), t.loaded = !0, t.exports
+        return y[e].call(t.exports, t, t.exports, w), t.loaded = !0, t.exports
     }
-    j.m = g, j.c = y, j.n = e => {
+    w.m = y, w.c = j, w.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return j.d(r, {
+        return w.d(r, {
             a: r
         }), r
-    }, j.d = (e, r) => {
-        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
+    }, w.d = (e, r) => {
+        for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
-        271: "3d790e9acffb4bcf9540",
-        290: "dcd1110ba978a36d1c6d",
+    }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
+        29: "94522abc80017ef83d9b",
+        304: "caed9225fc88627a1ade",
         351: "9ec43e8031fd2252d01d",
-        747: "a5300d89923b0c6831bf",
-        785: "2fc5bebd96804ab650b2",
-        807: "68bd5c7d28866c568e00",
+        535: "251e4fef15db43619f3b",
+        747: "e721e56eaf04858131e6",
+        807: "deac369ec79332e05c33",
         861: "7c8ce849384f01571a74"
     } [e] + ".js?v=" + {
-        271: "3d790e9acffb4bcf9540",
-        290: "dcd1110ba978a36d1c6d",
+        29: "94522abc80017ef83d9b",
+        304: "caed9225fc88627a1ade",
         351: "9ec43e8031fd2252d01d",
-        747: "a5300d89923b0c6831bf",
-        785: "2fc5bebd96804ab650b2",
-        807: "68bd5c7d28866c568e00",
+        535: "251e4fef15db43619f3b",
+        747: "e721e56eaf04858131e6",
+        807: "deac369ec79332e05c33",
         861: "7c8ce849384f01571a74"
-    } [e], j.g = function() {
+    } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), j.hmd = e => ((e = Object.create(e)).children || (e.children = []), Object.defineProperty(e, "exports", {
+    }(), w.hmd = e => ((e = Object.create(e)).children || (e.children = []), Object.defineProperty(e, "exports", {
         enumerable: !0,
         set: () => {
             throw new Error("ES Modules may not assign module.exports or exports.*, Use ESM export syntax, instead: " + e.id)
         }
-    }), e), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyter-theme-editor:", j.l = (t, o, n, a) => {
+    }), e), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyter-theme-editor:", w.l = (t, o, n, a) => {
         if (e[t]) e[t].push(o);
         else {
             var i, l;
             if (void 0 !== n)
-                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var d = u[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
+                    var s = f[u];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
+                        i = s;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [o];
-            var f = (r, o) => {
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [o];
+            var d = (r, o) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(o))), r) return r(o)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
-    }, j.r = e => {
+    }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, j.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
-        j.S = {};
+    }, w.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
+        w.S = {};
         var e = {},
             r = {};
-        j.I = (t, o) => {
+        w.I = (t, o) => {
             o || (o = []);
             var n = r[t];
             if (n || (n = r[t] = {}), !(o.indexOf(n) >= 0)) {
                 if (o.push(n), e[t]) return e[t];
-                j.o(j.S, t) || (j.S[t] = {});
-                var a = j.S[t],
+                w.o(w.S, t) || (w.S[t] = {});
+                var a = w.S[t],
                     i = "jupyter-theme-editor",
                     l = (e, r, t, o) => {
                         var n = a[e] = a[e] || {},
                             l = n[r];
                         (!l || !l.loaded && (!o != !l.eager ? o : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
-                    u = [];
-                return "default" === t && (l("@hello-pangea/color-picker", "3.2.2", (() => Promise.all([j.e(861), j.e(785), j.e(271)]).then((() => () => j(8785))))), l("@microsoft/fast-colors", "5.3.1", (() => j.e(351).then((() => () => j(3351))))), l("@rjsf/core", "4.2.3", (() => Promise.all([j.e(861), j.e(807), j.e(271)]).then((() => () => j(6084))))), l("jupyter-theme-editor", "0.3.0", (() => Promise.all([j.e(271), j.e(290)]).then((() => () => j(290)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (l("@hello-pangea/color-picker", "3.2.2", (() => Promise.all([w.e(861), w.e(304), w.e(29)]).then((() => () => w(8304))))), l("@microsoft/fast-colors", "5.3.1", (() => w.e(351).then((() => () => w(3351))))), l("@rjsf/core", "4.2.3", (() => Promise.all([w.e(861), w.e(807), w.e(29)]).then((() => () => w(3807))))), l("jupyter-theme-editor", "0.4.1", (() => Promise.all([w.e(29), w.e(535)]).then((() => () => w(3535)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        j.g.importScripts && (e = j.g.location + "");
-        var r = j.g.document;
+        w.g.importScripts && (e = w.g.location + "");
+        var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var o = t.length - 1; o > -1 && !e;) e = t[o--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), w.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             o = t[1] ? r(t[1]) : [];
         return t[2] && (o.length++, o.push.apply(o, r(t[2]))), t[3] && (o.push([]), o.push.apply(o, r(t[3]))), o
     }, o = (e, r) => {
         e = t(e), r = t(r);
@@ -166,141 +167,141 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var o = 1, a = 1; a < e.length; a++) o--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (o > 0 ? "." : "") + (o = 2, l);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
             var l = e[a];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : n(l))
+            i.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? i.pop() + " " + i.pop() : n(l))
         }
-        return u();
+        return f();
 
-        function u() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var o = e[0],
                 n = o < 0;
             n && (o = -o - 1);
-            for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var s, d, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !u || ("u" == f ? l > o && !n : "" == f != n);
-                if ("u" == d) {
-                    if (!u || "u" != f) return !1
-                } else if (u)
-                    if (f == d)
+            for (var i = 0, l = 1, f = !0;; l++, i++) {
+                var u, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(u = r[i]))[0])) return !f || ("u" == d ? l > o && !n : "" == d != n);
+                if ("u" == s) {
+                    if (!f || "u" != d) return !1
+                } else if (f)
+                    if (d == s)
                         if (l <= o) {
-                            if (s != e[l]) return !1
+                            if (u != e[l]) return !1
                         } else {
-                            if (n ? s > e[l] : s < e[l]) return !1;
-                            s != e[l] && (u = !1)
+                            if (n ? u > e[l] : u < e[l]) return !1;
+                            u != e[l] && (f = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (n || l <= o) return !1;
-                    u = !1, l--
+                    f = !1, l--
                 } else {
-                    if (l <= o || d < f != n) return !1;
-                    u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                    if (l <= o || s < d != n) return !1;
+                    f = !1
+                } else "s" != d && "n" != d && (f = !1, l--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
-        var t = j.S[e];
-        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = w.S[e];
+        if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, u = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", s = (e, r, t, o) => {
+    }, f = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", u = (e, r, t, o) => {
         var n = l(e, t);
-        return a(o, n) || "undefined" != typeof console && console.warn && console.warn(u(e, t, n, o)), f(e[t][n])
-    }, d = (e, r, t) => {
+        return a(o, n) || d(f(e, t, n, o)), c(e[t][n])
+    }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !a(t, r) || e && !o(e, r) ? e : r), 0)) && n[r]
-    }, f = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, o, n) {
-        var a = j.I(r);
-        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, o, n)) : e(r, j.S[r], t, o, n)
-    })(((e, r, t, o) => (i(e, t), s(r, 0, t, o)))), h = c(((e, r, t, o, n) => {
-        var a = r && j.o(r, t) && d(r, t, o);
-        return a ? f(a) : n()
-    })), v = {}, m = {
-        6271: () => p("default", "react", [1, 17, 0, 1]),
-        1194: () => p("default", "@jupyterlab/settingregistry", [1, 3, 6, 2]),
-        2884: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 2]),
-        3215: () => p("default", "@jupyterlab/ui-components", [1, 3, 6, 2]),
-        5613: () => p("default", "@jupyterlab/services", [1, 6, 6, 2]),
-        6212: () => h("default", "@hello-pangea/color-picker", [1, 3, 2, 2], (() => Promise.all([j.e(861), j.e(785)]).then((() => () => j(8785))))),
-        6848: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 2]),
-        7256: () => h("default", "@rjsf/core", [, [1, 4, 2, 0],
-            [1, 3, 1, 0], 1
-        ], (() => Promise.all([j.e(861), j.e(807)]).then((() => () => j(6084))))),
-        8185: () => h("default", "@microsoft/fast-colors", [1, 5, 3, 1], (() => j.e(351).then((() => () => j(3351))))),
-        8604: () => p("default", "@jupyterlab/translation", [1, 3, 6, 2])
-    }, b = {
-        271: [6271],
-        290: [1194, 2884, 3215, 5613, 6212, 6848, 7256, 8185, 8604]
-    }, j.f.consumes = (e, r) => {
-        j.o(b, e) && b[e].forEach((e => {
-            if (j.o(v, e)) return r.push(v[e]);
+    }, d = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, o, n) {
+        var a = w.I(r);
+        return a && a.then ? a.then(e.bind(e, r, w.S[r], t, o, n)) : e(r, w.S[r], t, o, n)
+    })(((e, r, t, o) => (i(e, t), u(r, 0, t, o)))), v = p(((e, r, t, o, n) => {
+        var a = r && w.o(r, t) && s(r, t, o);
+        return a ? c(a) : n()
+    })), m = {}, b = {
+        6029: () => h("default", "react", [1, 18, 2, 0]),
+        56: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 2]),
+        926: () => h("default", "@jupyterlab/translation", [1, 4, 0, 2]),
+        2189: () => h("default", "@jupyterlab/ui-components", [1, 4, 0, 2]),
+        4238: () => h("default", "@jupyterlab/services", [1, 7, 0, 2]),
+        4957: () => v("default", "@rjsf/core", [1, 4, 2, 0], (() => Promise.all([w.e(861), w.e(807)]).then((() => () => w(3807))))),
+        5350: () => h("default", "@jupyterlab/apputils", [1, 4, 1, 2]),
+        6212: () => v("default", "@hello-pangea/color-picker", [1, 3, 2, 2], (() => Promise.all([w.e(861), w.e(304)]).then((() => () => w(8304))))),
+        8185: () => v("default", "@microsoft/fast-colors", [1, 5, 3, 1], (() => w.e(351).then((() => () => w(3351))))),
+        9993: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 2])
+    }, g = {
+        29: [6029],
+        535: [56, 926, 2189, 4238, 4957, 5350, 6212, 8185, 9993]
+    }, w.f.consumes = (e, r) => {
+        w.o(g, e) && g[e].forEach((e => {
+            if (w.o(m, e)) return r.push(m[e]);
             var t = r => {
-                    v[e] = 0, j.m[e] = t => {
-                        delete j.c[e], t.exports = r()
+                    m[e] = 0, w.m[e] = t => {
+                        delete w.c[e], t.exports = r()
                     }
                 },
                 o = r => {
-                    delete v[e], j.m[e] = t => {
-                        throw delete j.c[e], r
+                    delete m[e], w.m[e] = t => {
+                        throw delete w.c[e], r
                     }
                 };
             try {
-                var n = m[e]();
-                n.then ? r.push(v[e] = n.then(t).catch(o)) : t(n)
+                var n = b[e]();
+                n.then ? r.push(m[e] = n.then(t).catch(o)) : t(n)
             } catch (e) {
                 o(e)
             }
         }))
     }, (() => {
         var e = {
             112: 0
         };
-        j.f.j = (r, t) => {
-            var o = j.o(e, r) ? e[r] : void 0;
+        w.f.j = (r, t) => {
+            var o = w.o(e, r) ? e[r] : void 0;
             if (0 !== o)
                 if (o) t.push(o[2]);
-                else if (271 != r) {
+                else if (29 != r) {
                 var n = new Promise(((t, n) => o = e[r] = [t, n]));
                 t.push(o[2] = n);
-                var a = j.p + j.u(r),
+                var a = w.p + w.u(r),
                     i = new Error;
-                j.l(a, (t => {
-                    if (j.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
+                w.l(a, (t => {
+                    if (w.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
                         var n = t && ("load" === t.type ? "missing" : t.type),
                             a = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + a + ")", i.name = "ChunkLoadError", i.type = n, i.request = a, o[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var o, n, [a, i, l] = t,
-                    u = 0;
+                    f = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (o in i) j.o(i, o) && (j.m[o] = i[o]);
-                    l && l(j)
+                    for (o in i) w.o(i, o) && (w.m[o] = i[o]);
+                    l && l(w)
                 }
-                for (r && r(t); u < a.length; u++) n = a[u], j.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); f < a.length; f++) n = a[f], w.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunkjupyter_theme_editor = self.webpackChunkjupyter_theme_editor || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), j.nc = void 0;
-    var w = j(982);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyter-theme-editor"] = w
+    })(), w.nc = void 0;
+    var P = w(982);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyter-theme-editor"] = P
 })();
```

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/labextension/static/third-party-licenses.json` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '7.22.3'}, 7: {'versionInfo': '3.30.2', 'extractedText': "*

 * *               "'Copyright (c) 2014-2023 Denis Pushkarev\\n\\nPermission is hereby granted, free "*

 * *               'of charge, to any person obtaining a copy\\nof this software and associated '*

 * *               'documentation files (the "Software"), to deal\\nin the Software without '*

 * *               'restriction, including without limitation the rights\\nto use, copy, modify, '*

 * *               'merge, publish, distrib […]*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "MIT License\n\nCopyright (c) 2014-present Sebastian McKenzie and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@babel/runtime",
-            "versionInfo": "7.20.6"
+            "versionInfo": "7.22.3"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2022 Reece Carolan\nCopyright (c) 2015 Case Sandberg\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@hello-pangea/color-picker",
             "versionInfo": "3.2.2"
         },
@@ -39,24 +39,24 @@
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014-2015 Athan Reines.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "compute-lcm",
             "versionInfo": "1.1.2"
         },
         {
-            "extractedText": "Copyright (c) 2014-2022 Denis Pushkarev\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
+            "extractedText": "Copyright (c) 2014-2023 Denis Pushkarev\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "core-js-pure",
-            "versionInfo": "3.26.1"
+            "versionInfo": "3.30.2"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "5.2.7"
+            "versionInfo": "6.8.1"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2017 Evgeny Poberezkin\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "fast-deep-equal",
             "versionInfo": "3.1.3"
         },
@@ -102,15 +102,15 @@
             "name": "lodash-es",
             "versionInfo": "4.17.21"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright 2017 Andrey Sitnik <andrey@sitnik.ru>\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of\nthis software and associated documentation files (the \"Software\"), to deal in\nthe Software without restriction, including without limitation the rights to\nuse, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of\nthe Software, and to permit persons to whom the Software is furnished to do so,\nsubject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS\nFOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR\nCOPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER\nIN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN\nCONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "nanoid",
-            "versionInfo": "3.3.4"
+            "versionInfo": "3.3.6"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2013-present, Facebook, Inc.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "prop-types",
             "versionInfo": "15.8.1"
         },
@@ -120,21 +120,21 @@
             "name": "react-is",
             "versionInfo": "16.9.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "2.0.0"
+            "versionInfo": "3.3.3"
         },
         {
             "extractedText": "Copyright (c), Brian Grinstead, http://briangrinstead.com\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.",
             "licenseId": "MIT",
             "name": "tinycolor2",
-            "versionInfo": "1.4.2"
+            "versionInfo": "1.6.0"
         },
         {
             "extractedText": "Copyright 2011 Gary Court. All rights reserved.\n\nRedistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:\n\n1.\tRedistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.\n\n2.\tRedistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.\n\nTHIS SOFTWARE IS PROVIDED BY GARY COURT \"AS IS\" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL GARY COURT OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n\nThe views and conclusions contained in the software and documentation are those of the authors and should not be interpreted as representing official policies, either expressed or implied, of Gary Court.\n",
             "licenseId": "BSD-2-Clause",
             "name": "uri-js",
             "versionInfo": "4.4.1"
         },
```

### Comparing `jupyter_theme_editor-0.3.0/jupyter_theme_editor/templates/template.css` & `jupyter_theme_editor-0.4.1/jupyter_theme_editor/templates/template.css`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/schema/plugin.json` & `jupyter_theme_editor-0.4.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/src/handler.ts` & `jupyter_theme_editor-0.4.1/src/handler.ts`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     endPoint
   );
 
   let response: Response;
   try {
     response = await ServerConnection.makeRequest(requestUrl, init, settings);
   } catch (error) {
-    throw new ServerConnection.NetworkError(error);
+    throw new ServerConnection.NetworkError(error as TypeError);
   }
 
   let data: any = await response.text();
 
   if (data.length > 0) {
     try {
       data = JSON.parse(data);
```

### Comparing `jupyter_theme_editor-0.3.0/src/index.ts` & `jupyter_theme_editor-0.4.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/src/model.ts` & `jupyter_theme_editor-0.4.1/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/src/view.tsx` & `jupyter_theme_editor-0.4.1/src/view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/style/base.css` & `jupyter_theme_editor-0.4.1/style/base.css`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 /*
     See the JupyterLab Developer Guide for useful CSS Patterns:
 
     https://jupyterlab.readthedocs.io/en/stable/developer/css.html
 */
-@import url('https://fonts.googleapis.com/css2?family=Courier');
-@import url('https://fonts.googleapis.com/css2?family=Dancing+Script');
-@import url('https://fonts.googleapis.com/css2?family=Dosis');
-@import url('https://fonts.googleapis.com/css2?family=Helvetica');
-@import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono');
-@import url('https://fonts.googleapis.com/css2?family=Lobster');
-@import url('https://fonts.googleapis.com/css2?family=Oxygen');
-@import url('https://fonts.googleapis.com/css2?family=Pacifico');
-@import url('https://fonts.googleapis.com/css2?family=Prompt');
-@import url('https://fonts.googleapis.com/css2?family=Righteous');
-@import url('https://fonts.googleapis.com/css2?family=Satisfy');
-@import url('https://fonts.googleapis.com/css2?family=Single+Day');
-@import url('https://fonts.googleapis.com/css2?family=Space+Mono');
-@import url('https://fonts.googleapis.com/css2?family=Times+New+Roman');
-@import url('https://fonts.googleapis.com/css2?family=Ultra');
-@import url('https://fonts.googleapis.com/css2?family=Urbanist');
-@import url('https://fonts.googleapis.com/css2?family=Verdana');
+@import 'https://fonts.googleapis.com/css2?family=Courier';
+@import 'https://fonts.googleapis.com/css2?family=Dancing+Script';
+@import 'https://fonts.googleapis.com/css2?family=Dosis';
+@import 'https://fonts.googleapis.com/css2?family=Helvetica';
+@import 'https://fonts.googleapis.com/css2?family=JetBrains+Mono';
+@import 'https://fonts.googleapis.com/css2?family=Lobster';
+@import 'https://fonts.googleapis.com/css2?family=Oxygen';
+@import 'https://fonts.googleapis.com/css2?family=Pacifico';
+@import 'https://fonts.googleapis.com/css2?family=Prompt';
+@import 'https://fonts.googleapis.com/css2?family=Righteous';
+@import 'https://fonts.googleapis.com/css2?family=Satisfy';
+@import 'https://fonts.googleapis.com/css2?family=Single+Day';
+@import 'https://fonts.googleapis.com/css2?family=Space+Mono';
+@import 'https://fonts.googleapis.com/css2?family=Times+New+Roman';
+@import 'https://fonts.googleapis.com/css2?family=Ultra';
+@import 'https://fonts.googleapis.com/css2?family=Urbanist';
+@import 'https://fonts.googleapis.com/css2?family=Verdana';
 
 .jp-theme-editor-panel {
   overflow-y: auto;
 }
 
 .jp-theme-editor-button-color {
   height: var(--jp-ui-font-size0);
```

### Comparing `jupyter_theme_editor-0.3.0/style/theme-editor.svg` & `jupyter_theme_editor-0.4.1/style/theme-editor.svg`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/ui-tests/README.md` & `jupyter_theme_editor-0.4.1/ui-tests/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Integration Testing
 
 This folder contains the integration tests of the extension.
 
-They are defined using [Playwright](https://playwright.dev/docs/intro/) test runner
+They are defined using [Playwright](https://playwright.dev/docs/intro) test runner
 and [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) helper.
 
-The Playwright configuration is defined in [playwright.config.js](../playwright.config.js)
-in the root directory.
+The Playwright configuration is defined in [playwright.config.js](./playwright.config.js).
 
 The JupyterLab server configuration to use for the integration test is defined
-in [jupyter_server_test_config.py](../jupyter_server_test_config.py) in the root directory.
+in [jupyter_server_test_config.py](./jupyter_server_test_config.py).
 
 The default configuration will produce video for failing tests and an HTML report.
 
+> There is a new experimental UI mode that you may fall in love with; see [that video](https://www.youtube.com/watch?v=jF0yA-JLQW0).
+
 ## Run the tests
 
 > All commands are assumed to be executed from the root directory
 
 To run the tests, you need to:
 
 1. Compile the extension:
@@ -40,15 +41,18 @@
 3. Execute the [Playwright](https://playwright.dev/docs/intro) tests:
 
 ```sh
 cd ./ui-tests
 jlpm playwright test
 ```
 
-The report will be opened in your browser at the end of the tests execution.
+Test results will be shown in the terminal. In case of any test failures, the test report
+will be opened in your browser at the end of the tests execution; see
+[Playwright documentation](https://playwright.dev/docs/test-reporters#html-reporter)
+for configuring that behavior.
 
 ## Update the tests snapshots
 
 > All commands are assumed to be executed from the root directory
 
 If you are comparing snapshots to validate your tests, you may need to update
 the reference snapshots stored in the repository. To do that, you need to:
@@ -103,15 +107,22 @@
 ```sh
 cd ./ui-tests
 jlpm install
 jlpm playwright install
 cd ..
 ```
 
-3. Execute the [Playwright code generator](https://playwright.dev/docs/codegen):
+3. Start the server:
+
+```sh
+cd ./ui-tests
+jlpm start
+```
+
+4. Execute the [Playwright code generator](https://playwright.dev/docs/codegen) in **another terminal**:
 
 ```sh
 cd ./ui-tests
 jlpm playwright codegen localhost:8888
 ```
 
 ## Debug tests
@@ -138,9 +149,19 @@
 cd ..
 ```
 
 3. Execute the Playwright tests in [debug mode](https://playwright.dev/docs/debug):
 
 ```sh
 cd ./ui-tests
-PWDEBUG=1 jlpm playwright test
+jlpm playwright test --debug
+```
+
+## Upgrade Playwright and the browsers
+
+To update the web browser versions, you must update the package `@playwright/test`:
+
+```sh
+cd ./ui-tests
+jlpm up "@playwright/test"
+jlpm playwright install
 ```
```

### Comparing `jupyter_theme_editor-0.3.0/ui-tests/jupyter_theme_editor.spec.ts` & `jupyter_theme_editor-0.4.1/ui-tests/tests/jupyter_theme_editor.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_theme_editor-0.3.0/.gitignore` & `jupyter_theme_editor-0.4.1/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 *.bundle.*
 lib/
 node_modules/
+*.log
 .eslintcache
 .stylelintcache
 *.egg-info/
 .ipynb_checkpoints
 *.tsbuildinfo
 jupyter_theme_editor/labextension
 # Version file is handled by hatchling
@@ -115,7 +116,10 @@
 # Pyre type checker
 .pyre/
 
 # End of https://www.gitignore.io/api/python
 
 # OSX files
 .DS_Store
+
+# Yarn cache
+.yarn/
```

### Comparing `jupyter_theme_editor-0.3.0/LICENSE` & `jupyter_theme_editor-0.4.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Florence Haudin
+Copyright (c) 2023, Florence Haudin
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `jupyter_theme_editor-0.3.0/README.md` & `jupyter_theme_editor-0.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # jupyter_theme_editor
 
-[![Extension status](https://img.shields.io/badge/status-draft-critical 'Not yet working')](https://jupyterlab-contrib.github.io/index.html)[![Github Actions Status](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/workflows/Build/badge.svg)](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/actions/workflows/build.yml)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab-contrib/jupyterlab-theme-editor/main?urlpath=lab)
-
-Extension to create a theme
+[![Github Actions Status](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/workflows/Build/badge.svg)](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/actions/workflows/build.yml)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab-contrib/jupyterlab-theme-editor/main?urlpath=lab)
+Extension to create a theme.
 
 This extension is composed of a Python package named `jupyter_theme_editor`
 for the server extension and a NPM package named `jupyter-theme-editor`
 for the frontend extension.
 
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyter_theme_editor
@@ -54,15 +53,15 @@
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
 # Change directory to the jupyter_theme_editor directory
 # Install package in development mode
-pip install -e .
+pip install -e ".[test]"
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Server extension must be manually installed in develop mode
 jupyter server extension enable jupyter_theme_editor
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
@@ -102,14 +101,16 @@
 
 This extension is using [Pytest](https://docs.pytest.org/) for Python code testing.
 
 Install test dependencies (needed only once):
 
 ```sh
 pip install -e ".[test]"
+# Each time you install the Python package, you need to restore the front-end extension link
+jupyter labextension develop . --overwrite
 ```
 
 To execute them, run:
 
 ```sh
 pytest -vv -r ap --cov jupyter_theme_editor
 ```
@@ -123,15 +124,15 @@
 ```sh
 jlpm
 jlpm test
 ```
 
 #### Integration tests
 
-This extension uses [Playwright](https://playwright.dev/docs/intro/) for the integration tests (aka user level tests).
+This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
 More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
 
 More information are provided within the [ui-tests](./ui-tests/README.md) README.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

### Comparing `jupyter_theme_editor-0.3.0/pyproject.toml` & `jupyter_theme_editor-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [build-system]
-requires = ["hatchling>=1.4.0", "jupyterlab>=3.1.0,<5.0.0", "hatch-nodejs-version"]
+requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_theme_editor"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
-    "Framework :: Jupyter :: JupyterLab :: 3",
+    "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "jupyter_server>=1.21,<3"
+    "jupyter_server>=2.0.1,<3"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
@@ -74,9 +73,16 @@
 source_dir = "src"
 build_dir = "jupyter_theme_editor/labextension"
 
 [tool.jupyter-releaser.options]
 version_cmd = "hatch version"
 
 [tool.jupyter-releaser.hooks]
-before-build-npm = ["python -m pip install jupyterlab~=3.1", "jlpm", "jlpm build:prod"]
+before-build-npm = [
+    "python -m pip install 'jupyterlab>=4.0.0,<5'",
+    "jlpm",
+    "jlpm build:prod"
+]
 before-build-python = ["jlpm clean:all"]
+
+[tool.check-wheel-contents]
+ignore = ["W002"]
```

### Comparing `jupyter_theme_editor-0.3.0/PKG-INFO` & `jupyter_theme_editor-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: jupyter_theme_editor
-Version: 0.3.0
-Summary: Extension to create a theme
+Version: 0.4.1
+Summary: Extension to create a theme.
 Project-URL: Homepage, https://github.com/jupyterlab-contrib/jupyterlab-theme-editor
 Project-URL: Bug Tracker, https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/issues
 Project-URL: Repository, https://github.com/jupyterlab-contrib/jupyterlab-theme-editor.git
 Author-email: Florence Haudin <haudin.florence@gmail.com>
 License: BSD 3-Clause License
         
-        Copyright (c) 2022, Florence Haudin
+        Copyright (c) 2023, Florence Haudin
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -34,48 +34,46 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Requires-Dist: jupyter-server<3,>=1.21
+Requires-Python: >=3.8
+Requires-Dist: jupyter-server<3,>=2.0.1
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-jupyter[server]>=0.6.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # jupyter_theme_editor
 
-[![Extension status](https://img.shields.io/badge/status-draft-critical 'Not yet working')](https://jupyterlab-contrib.github.io/index.html)[![Github Actions Status](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/workflows/Build/badge.svg)](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/actions/workflows/build.yml)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab-contrib/jupyterlab-theme-editor/main?urlpath=lab)
-
-Extension to create a theme
+[![Github Actions Status](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/workflows/Build/badge.svg)](https://github.com/jupyterlab-contrib/jupyterlab-theme-editor/actions/workflows/build.yml)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab-contrib/jupyterlab-theme-editor/main?urlpath=lab)
+Extension to create a theme.
 
 This extension is composed of a Python package named `jupyter_theme_editor`
 for the server extension and a NPM package named `jupyter-theme-editor`
 for the frontend extension.
 
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyter_theme_editor
@@ -115,15 +113,15 @@
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
 # Change directory to the jupyter_theme_editor directory
 # Install package in development mode
-pip install -e .
+pip install -e ".[test]"
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Server extension must be manually installed in develop mode
 jupyter server extension enable jupyter_theme_editor
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
@@ -163,14 +161,16 @@
 
 This extension is using [Pytest](https://docs.pytest.org/) for Python code testing.
 
 Install test dependencies (needed only once):
 
 ```sh
 pip install -e ".[test]"
+# Each time you install the Python package, you need to restore the front-end extension link
+jupyter labextension develop . --overwrite
 ```
 
 To execute them, run:
 
 ```sh
 pytest -vv -r ap --cov jupyter_theme_editor
 ```
@@ -184,15 +184,15 @@
 ```sh
 jlpm
 jlpm test
 ```
 
 #### Integration tests
 
-This extension uses [Playwright](https://playwright.dev/docs/intro/) for the integration tests (aka user level tests).
+This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
 More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
 
 More information are provided within the [ui-tests](./ui-tests/README.md) README.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

