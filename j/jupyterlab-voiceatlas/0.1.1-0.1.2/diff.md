# Comparing `tmp/jupyterlab_voiceatlas-0.1.1.tar.gz` & `tmp/jupyterlab_voiceatlas-0.1.2.tar.gz`

## Comparing `jupyterlab_voiceatlas-0.1.1.tar` & `jupyterlab_voiceatlas-0.1.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/.eslintrc.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/babel.config.js
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/conftest.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/install.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jest.config.js
--rw-r--r--   0        0        0  1216372 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/package-lock.json
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/setup.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/tsconfig.json
--rw-r--r--   0        0        0   417710 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/yarn.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyter-config/nb-config/jupyterlab_voiceatlas.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyter-config/server-config/jupyterlab_voiceatlas.json
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/__init__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/_version.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/handlers.py
--rw-r--r--   0        0        0    20471 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/build_log.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/install.json
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/package.json
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/schemas/jupyterlab_voiceatlas/package.json.orig
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/schemas/jupyterlab_voiceatlas/plugin.json
--rw-r--r--   0        0        0    66201 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/lib_index_js.9568c4c45c4e4bb914f0.js
--rw-r--r--   0        0        0    55627 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/lib_index_js.9568c4c45c4e4bb914f0.js.map
--rw-r--r--   0        0        0    33630 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/remoteEntry.766497d5acf3f183b760.js
--rw-r--r--   0        0        0    32499 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/remoteEntry.766497d5acf3f183b760.js.map
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/style.js
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/style_index_css.3dc010fcea6a1be8fcd7.js
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/style_index_css.3dc010fcea6a1be8fcd7.js.map
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b97e434cd56da264030e.js
--rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b97e434cd56da264030e.js.map
--rw-r--r--   0        0        0   184648 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_jupyterlab_toastify_lib_index_js.adfbac397ad46008b7ab.js
--rw-r--r--   0        0        0   207247 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_jupyterlab_toastify_lib_index_js.adfbac397ad46008b7ab.js.map
--rw-r--r--   0        0        0    15886 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isempty_index_js.a8ee7ea9325597c9aff4.js
--rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isempty_index_js.a8ee7ea9325597c9aff4.js.map
--rw-r--r--   0        0        0    50214 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isequal_index_js.25147cec73a51ddc5539.js
--rw-r--r--   0        0        0    62541 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isequal_index_js.25147cec73a51ddc5539.js.map
--rw-r--r--   0        0        0    39997 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_js.f1889b0d9f4f4d4094b7.js
--rw-r--r--   0        0        0    44769 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_js.f1889b0d9f4f4d4094b7.js.map
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/tests/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/tests/test_handlers.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/schema/plugin.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/handler.ts
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/index.ts
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/svg.d.ts
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/utils.ts
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/__tests__/jupyterlab_voiceatlas.spec.ts
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/style/IconsStyle.ts
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/widgets/AboutVoiceAtlas.tsx
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/widgets/AppChatlas.ts
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/widgets/ChatlasDropdownMenuWidget.tsx
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/widgets/ChatlasWidget.tsx
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/src/widgets/EditSettingsWidget.tsx
--rw-r--r--   0        0        0    17597 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/style/VoiceAtlas_Wordmark.svg
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/style/index.css
--rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/style/voiceatlas_logo.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/ui-tests/tests/jupyterlab_voiceatlas.spec.ts
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/LICENSE
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/README.md
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/.eslintrc.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/MANIFEST.in
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/babel.config.js
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/conftest.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/install.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jest.config.js
+-rw-r--r--   0        0        0  1216372 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/package-lock.json
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/setup.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0   417710 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/yarn.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyter-config/nb-config/jupyterlab_voiceatlas.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyter-config/server-config/jupyterlab_voiceatlas.json
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/__init__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/_version.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/handlers.py
+-rw-r--r--   0        0        0    20471 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/build_log.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/install.json
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/package.json
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/schemas/jupyterlab_voiceatlas/package.json.orig
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/schemas/jupyterlab_voiceatlas/plugin.json
+-rw-r--r--   0        0        0    66201 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/lib_index_js.9568c4c45c4e4bb914f0.js
+-rw-r--r--   0        0        0    55627 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/lib_index_js.9568c4c45c4e4bb914f0.js.map
+-rw-r--r--   0        0        0    33630 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/remoteEntry.766497d5acf3f183b760.js
+-rw-r--r--   0        0        0    32499 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/remoteEntry.766497d5acf3f183b760.js.map
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/style.js
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/style_index_css.3dc010fcea6a1be8fcd7.js
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/style_index_css.3dc010fcea6a1be8fcd7.js.map
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b97e434cd56da264030e.js
+-rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b97e434cd56da264030e.js.map
+-rw-r--r--   0        0        0   184648 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_jupyterlab_toastify_lib_index_js.adfbac397ad46008b7ab.js
+-rw-r--r--   0        0        0   207247 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_jupyterlab_toastify_lib_index_js.adfbac397ad46008b7ab.js.map
+-rw-r--r--   0        0        0    15886 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isempty_index_js.a8ee7ea9325597c9aff4.js
+-rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isempty_index_js.a8ee7ea9325597c9aff4.js.map
+-rw-r--r--   0        0        0    50214 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isequal_index_js.25147cec73a51ddc5539.js
+-rw-r--r--   0        0        0    62541 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isequal_index_js.25147cec73a51ddc5539.js.map
+-rw-r--r--   0        0        0    39997 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_js.f1889b0d9f4f4d4094b7.js
+-rw-r--r--   0        0        0    44769 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_js.f1889b0d9f4f4d4094b7.js.map
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/tests/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/tests/test_handlers.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/schema/plugin.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/handler.ts
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/index.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/svg.d.ts
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/utils.ts
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/__tests__/jupyterlab_voiceatlas.spec.ts
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/style/IconsStyle.ts
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/widgets/AboutVoiceAtlas.tsx
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/widgets/AppChatlas.ts
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/widgets/ChatlasDropdownMenuWidget.tsx
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/widgets/ChatlasWidget.tsx
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/src/widgets/EditSettingsWidget.tsx
+-rw-r--r--   0        0        0    17597 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/style/VoiceAtlas_Wordmark.svg
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/style/index.css
+-rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/style/voiceatlas_logo.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/ui-tests/tests/jupyterlab_voiceatlas.spec.ts
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/README.md
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 jupyterlab_voiceatlas-0.1.2/PKG-INFO
```

### Comparing `jupyterlab_voiceatlas-0.1.1/.eslintrc.js` & `jupyterlab_voiceatlas-0.1.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/MANIFEST.in` & `jupyterlab_voiceatlas-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/RELEASE.md` & `jupyterlab_voiceatlas-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jest.config.js` & `jupyterlab_voiceatlas-0.1.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/package-lock.json` & `jupyterlab_voiceatlas-0.1.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/package.json` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/schemas/jupyterlab_voiceatlas/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.1.0'"}*

```diff
@@ -120,9 +120,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.0"
 }
```

### Comparing `jupyterlab_voiceatlas-0.1.1/tsconfig.json` & `jupyterlab_voiceatlas-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/yarn.lock` & `jupyterlab_voiceatlas-0.1.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/__init__.py` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/handlers.py` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/build_log.json` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/package.json` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/schemas/jupyterlab_voiceatlas/package.json.orig` & `jupyterlab_voiceatlas-0.1.2/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.93125%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/navteca/jupyterlab_voiceatlas/issues'}",*

 * * "'homepage'": "'https://github.com/navteca/jupyterlab_voiceatlas'",*

 * * "'repository'": "{'url': 'https://github.com/navteca/jupyterlab_voiceatlas.git'}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": {
         "email": "info@navteca.com",
         "name": "Navteca LLC"
     },
     "bugs": {
-        "url": "https://github.com/github_username/jupyterlab_voiceatlas/issues"
+        "url": "https://github.com/navteca/jupyterlab_voiceatlas/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.0.11",
         "@jupyterlab/coreutils": "^5.0.3",
         "@jupyterlab/mainmenu": "^3.0.10",
         "@jupyterlab/notebook": "^3.0.11",
         "@jupyterlab/services": "^6.0.5",
@@ -47,15 +47,15 @@
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
-    "homepage": "https://github.com/github_username/jupyterlab_voiceatlas",
+    "homepage": "https://github.com/navteca/jupyterlab_voiceatlas",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
             ],
             "before-build-python": [
@@ -87,15 +87,15 @@
     "main": "lib/index.js",
     "name": "jupyterlab_voiceatlas",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
-        "url": "https://github.com/github_username/jupyterlab_voiceatlas.git"
+        "url": "https://github.com/navteca/jupyterlab_voiceatlas.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
@@ -120,9 +120,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/lib_index_js.9568c4c45c4e4bb914f0.js` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/lib_index_js.9568c4c45c4e4bb914f0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/lib_index_js.9568c4c45c4e4bb914f0.js.map` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/lib_index_js.9568c4c45c4e4bb914f0.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/remoteEntry.766497d5acf3f183b760.js` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/remoteEntry.766497d5acf3f183b760.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/remoteEntry.766497d5acf3f183b760.js.map` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/remoteEntry.766497d5acf3f183b760.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/style_index_css.3dc010fcea6a1be8fcd7.js` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/style_index_css.3dc010fcea6a1be8fcd7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/style_index_css.3dc010fcea6a1be8fcd7.js.map` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/style_index_css.3dc010fcea6a1be8fcd7.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b97e434cd56da264030e.js` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b97e434cd56da264030e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b97e434cd56da264030e.js.map` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b97e434cd56da264030e.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_jupyterlab_toastify_lib_index_js.adfbac397ad46008b7ab.js` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_jupyterlab_toastify_lib_index_js.adfbac397ad46008b7ab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_jupyterlab_toastify_lib_index_js.adfbac397ad46008b7ab.js.map` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_jupyterlab_toastify_lib_index_js.adfbac397ad46008b7ab.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isempty_index_js.a8ee7ea9325597c9aff4.js` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isempty_index_js.a8ee7ea9325597c9aff4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isempty_index_js.a8ee7ea9325597c9aff4.js.map` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isempty_index_js.a8ee7ea9325597c9aff4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isequal_index_js.25147cec73a51ddc5539.js` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isequal_index_js.25147cec73a51ddc5539.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isequal_index_js.25147cec73a51ddc5539.js.map` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_lodash_isequal_index_js.25147cec73a51ddc5539.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_js.f1889b0d9f4f4d4094b7.js` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_js.f1889b0d9f4f4d4094b7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_js.f1889b0d9f4f4d4094b7.js.map` & `jupyterlab_voiceatlas-0.1.2/jupyterlab_voiceatlas/labextension/static/vendors-node_modules_react-toastify_dist_react-toastify_esm_js.f1889b0d9f4f4d4094b7.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/src/handler.ts` & `jupyterlab_voiceatlas-0.1.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/src/index.ts` & `jupyterlab_voiceatlas-0.1.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/src/utils.ts` & `jupyterlab_voiceatlas-0.1.2/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/src/widgets/AboutVoiceAtlas.tsx` & `jupyterlab_voiceatlas-0.1.2/src/widgets/AboutVoiceAtlas.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/src/widgets/AppChatlas.ts` & `jupyterlab_voiceatlas-0.1.2/src/widgets/AppChatlas.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/src/widgets/ChatlasDropdownMenuWidget.tsx` & `jupyterlab_voiceatlas-0.1.2/src/widgets/ChatlasDropdownMenuWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/src/widgets/ChatlasWidget.tsx` & `jupyterlab_voiceatlas-0.1.2/src/widgets/ChatlasWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/src/widgets/EditSettingsWidget.tsx` & `jupyterlab_voiceatlas-0.1.2/src/widgets/EditSettingsWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/style/VoiceAtlas_Wordmark.svg` & `jupyterlab_voiceatlas-0.1.2/style/VoiceAtlas_Wordmark.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/style/voiceatlas_logo.svg` & `jupyterlab_voiceatlas-0.1.2/style/voiceatlas_logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/ui-tests/README.md` & `jupyterlab_voiceatlas-0.1.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/ui-tests/jupyter_server_test_config.py` & `jupyterlab_voiceatlas-0.1.2/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/ui-tests/tests/jupyterlab_voiceatlas.spec.ts` & `jupyterlab_voiceatlas-0.1.2/ui-tests/tests/jupyterlab_voiceatlas.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/.gitignore` & `jupyterlab_voiceatlas-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/LICENSE` & `jupyterlab_voiceatlas-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/README.md` & `jupyterlab_voiceatlas-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/pyproject.toml` & `jupyterlab_voiceatlas-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_voiceatlas-0.1.1/PKG-INFO` & `jupyterlab_voiceatlas-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jupyterlab_voiceatlas
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JupyterLab Extension for Voice Atlas.
-Project-URL: Homepage, https://github.com/github_username/jupyterlab_voiceatlas
-Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_voiceatlas/issues
-Project-URL: Repository, https://github.com/github_username/jupyterlab_voiceatlas.git
+Project-URL: Homepage, https://github.com/navteca/jupyterlab_voiceatlas
+Project-URL: Bug Tracker, https://github.com/navteca/jupyterlab_voiceatlas/issues
+Project-URL: Repository, https://github.com/navteca/jupyterlab_voiceatlas.git
 Author-email: Navteca LLC <info@navteca.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Navteca LLC
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

