# Comparing `tmp/livemark-0.95.0.tar.gz` & `tmp/livemark-0.96.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livemark-0.95.0.tar", last modified: Wed Aug 17 07:39:56 2022, max compression
+gzip compressed data, was "livemark-0.96.0.tar", last modified: Fri Aug 19 07:41:03 2022, max compression
```

## Comparing `livemark-0.95.0.tar` & `livemark-0.96.0.tar`

### file list

```diff
@@ -1,269 +1,269 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.596214 livemark-0.95.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-08-17 07:39:48.000000 livemark-0.95.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-17 07:39:48.000000 livemark-0.95.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-08-17 07:39:48.000000 livemark-0.95.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-08-17 07:39:56.596214 livemark-0.95.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-08-17 07:39:48.000000 livemark-0.95.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.572212 livemark-0.95.0/livemark/
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/assets/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/assets/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/assets/documents/
--rw-r--r--   0 runner    (1001) docker     (121)     3218 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/assets/documents/template.md
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/document.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4188 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/markup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/plugins/about/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/about/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/about/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/about/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/about/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/plugins/audio/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/audio/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/audio/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/audio/soundcloud.html
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/audio/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/plugins/blog/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/blog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/blog/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/blog/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/blog/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/plugins/brand/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/brand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/brand/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/brand/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/brand/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/cards/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/cards/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/cards/script.js
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/cards/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/plugins/chart/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/chart/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/chart/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark/plugins/cleanup/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/cleanup/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.580212 livemark-0.95.0/livemark/plugins/columns/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/columns/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/columns/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.580212 livemark-0.95.0/livemark/plugins/comments/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/comments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/comments/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/comments/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/comments/script.js
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/comments/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.580212 livemark-0.95.0/livemark/plugins/counter/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/counter/google.html
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/counter/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/counter/plausible.html
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/counter/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.580212 livemark-0.95.0/livemark/plugins/display/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/display/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/display/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/display/script.js
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/display/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.580212 livemark-0.95.0/livemark/plugins/file/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/file/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/file/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.580212 livemark-0.95.0/livemark/plugins/github/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/github/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.580212 livemark-0.95.0/livemark/plugins/html/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/html/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/html/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.580212 livemark-0.95.0/livemark/plugins/image/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/image/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     6996 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/image/instagram.html
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/image/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/image/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/infinity/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/infinity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/infinity/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/infinity/script.js
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/infinity/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/links/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/links/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/links/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/links/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/logic/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/logic/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/map/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/map/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/map/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/markdown/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/markdown/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/markdown/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/markup/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/markup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/markup/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/markup/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/mobile/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/mobile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/mobile/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/mobile/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/mobile/script.js
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/mobile/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/news/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/news/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/news/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/news/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/notebook/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/notebook/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/notebook/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.584213 livemark-0.95.0/livemark/plugins/notes/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/notes/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/notes/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/notes/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.588213 livemark-0.95.0/livemark/plugins/package/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/package/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/package/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.588213 livemark-0.95.0/livemark/plugins/pages/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pages/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pages/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pages/script.js
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pages/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.588213 livemark-0.95.0/livemark/plugins/pagination/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pagination/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pagination/script.js
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pagination/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.588213 livemark-0.95.0/livemark/plugins/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pipeline/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/pipeline/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.588213 livemark-0.95.0/livemark/plugins/prepare/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/prepare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/prepare/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.588213 livemark-0.95.0/livemark/plugins/rating/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/rating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/rating/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/rating/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/rating/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.588213 livemark-0.95.0/livemark/plugins/redirect/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/redirect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/redirect/missing.md
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/redirect/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.588213 livemark-0.95.0/livemark/plugins/reference/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/reference/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/reference/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/reference/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.588213 livemark-0.95.0/livemark/plugins/remark/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/remark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/remark/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/remark/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/remark/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.592213 livemark-0.95.0/livemark/plugins/report/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/report/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/report/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.592213 livemark-0.95.0/livemark/plugins/resource/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/resource/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/resource/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.592213 livemark-0.95.0/livemark/plugins/schema/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/schema/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/schema/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.592213 livemark-0.95.0/livemark/plugins/script/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/script/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.592213 livemark-0.95.0/livemark/plugins/search/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/search/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/search/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/search/script.js
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/search/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.592213 livemark-0.95.0/livemark/plugins/signs/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/signs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/signs/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/signs/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/signs/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.592213 livemark-0.95.0/livemark/plugins/site/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/site/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/site/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/site/script.js
--rw-r--r--   0 runner    (1001) docker     (121)    20194 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/site/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.592213 livemark-0.95.0/livemark/plugins/source/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/source/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/source/script.js
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/source/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.592213 livemark-0.95.0/livemark/plugins/table/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/table/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/table/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.596214 livemark-0.95.0/livemark/plugins/tabs/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/tabs/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/tabs/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/tabs/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.596214 livemark-0.95.0/livemark/plugins/task/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/task/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/task/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.596214 livemark-0.95.0/livemark/plugins/topics/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/topics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/topics/markup.html
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/topics/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/topics/script.js
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/topics/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.596214 livemark-0.95.0/livemark/plugins/video/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/video/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/video/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/video/style.css
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/plugins/video/youtube.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.596214 livemark-0.95.0/livemark/program/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/program/build.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/program/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/program/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/program/merge.py
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/program/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/program/start.py
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/server.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/snippet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-08-17 07:39:48.000000 livemark-0.95.0/livemark/system.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 07:39:56.576212 livemark-0.95.0/livemark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-08-17 07:39:56.000000 livemark-0.95.0/livemark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6967 2022-08-17 07:39:56.000000 livemark-0.95.0/livemark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 07:39:56.000000 livemark-0.95.0/livemark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-17 07:39:56.000000 livemark-0.95.0/livemark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 07:39:56.000000 livemark-0.95.0/livemark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-08-17 07:39:56.000000 livemark-0.95.0/livemark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-17 07:39:56.000000 livemark-0.95.0/livemark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-08-17 07:39:48.000000 livemark-0.95.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-17 07:39:48.000000 livemark-0.95.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-17 07:39:48.000000 livemark-0.95.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-17 07:39:56.596214 livemark-0.95.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-08-17 07:39:48.000000 livemark-0.95.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.389454 livemark-0.96.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-08-19 07:40:59.000000 livemark-0.96.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-19 07:40:59.000000 livemark-0.96.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      883 2022-08-19 07:40:59.000000 livemark-0.96.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-08-19 07:41:03.389454 livemark-0.96.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-08-19 07:40:59.000000 livemark-0.96.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.365452 livemark-0.96.0/livemark/
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/assets/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark/assets/documents/
+-rw-r--r--   0 runner    (1001) docker     (121)     3218 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/assets/documents/template.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/document.py
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4188 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/markup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark/plugins/about/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/about/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/about/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/about/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/about/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark/plugins/audio/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/audio/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/audio/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/audio/soundcloud.html
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/audio/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark/plugins/blog/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/blog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/blog/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/blog/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/blog/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark/plugins/brand/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/brand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/brand/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/brand/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/brand/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/cards/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/cards/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/cards/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/cards/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark/plugins/chart/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/chart/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/chart/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.373453 livemark-0.96.0/livemark/plugins/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/cleanup/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.373453 livemark-0.96.0/livemark/plugins/columns/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/columns/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/columns/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.373453 livemark-0.96.0/livemark/plugins/comments/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/comments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/comments/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/comments/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/comments/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/comments/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.373453 livemark-0.96.0/livemark/plugins/counter/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/counter/google.html
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/counter/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/counter/plausible.html
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/counter/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.373453 livemark-0.96.0/livemark/plugins/display/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/display/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/display/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/display/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/display/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.373453 livemark-0.96.0/livemark/plugins/file/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/file/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/file/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.373453 livemark-0.96.0/livemark/plugins/github/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/github/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.373453 livemark-0.96.0/livemark/plugins/html/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/html/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/html/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.373453 livemark-0.96.0/livemark/plugins/image/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/image/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)     6996 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/image/instagram.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/image/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/image/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/infinity/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/infinity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/infinity/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/infinity/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/infinity/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/links/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/links/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/links/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/links/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/logic/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/logic/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/map/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/map/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/map/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/markdown/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/markdown/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/markdown/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/markup/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/markup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/markup/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/markup/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/mobile/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/mobile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/mobile/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/mobile/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/mobile/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/mobile/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/news/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/news/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/news/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/news/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/notebook/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/notebook/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/notebook/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/notes/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/notes/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/notes/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/notes/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.377453 livemark-0.96.0/livemark/plugins/package/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/package/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/package/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/pages/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pages/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pages/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pages/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pages/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/pagination/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pagination/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pagination/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pagination/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pipeline/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/pipeline/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/prepare/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/prepare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/prepare/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/rating/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/rating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/rating/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/rating/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/rating/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/redirect/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/redirect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/redirect/missing.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/redirect/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/reference/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/reference/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/reference/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/remark/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/remark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/remark/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/remark/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/remark/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/report/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/report/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/report/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/resource/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/resource/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/resource/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/schema/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/schema/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.381453 livemark-0.96.0/livemark/plugins/script/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2473 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/script/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.385454 livemark-0.96.0/livemark/plugins/search/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/search/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/search/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/search/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/search/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.385454 livemark-0.96.0/livemark/plugins/signs/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/signs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/signs/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/signs/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/signs/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.385454 livemark-0.96.0/livemark/plugins/site/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/site/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/site/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/site/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)    20194 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/site/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.385454 livemark-0.96.0/livemark/plugins/source/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/source/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/source/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/source/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.385454 livemark-0.96.0/livemark/plugins/table/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/table/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/table/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.385454 livemark-0.96.0/livemark/plugins/tabs/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/tabs/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/tabs/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/tabs/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.385454 livemark-0.96.0/livemark/plugins/task/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/task/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/task/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.385454 livemark-0.96.0/livemark/plugins/topics/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/topics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/topics/markup.html
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/topics/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/topics/script.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/topics/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.389454 livemark-0.96.0/livemark/plugins/video/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/video/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/video/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/video/style.css
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/plugins/video/youtube.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.389454 livemark-0.96.0/livemark/program/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/program/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/program/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/program/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/program/merge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/program/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/program/start.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/snippet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-08-19 07:40:59.000000 livemark-0.96.0/livemark/system.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 07:41:03.369453 livemark-0.96.0/livemark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-08-19 07:41:03.000000 livemark-0.96.0/livemark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6967 2022-08-19 07:41:03.000000 livemark-0.96.0/livemark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 07:41:03.000000 livemark-0.96.0/livemark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-19 07:41:03.000000 livemark-0.96.0/livemark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 07:41:03.000000 livemark-0.96.0/livemark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-08-19 07:41:03.000000 livemark-0.96.0/livemark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-19 07:41:03.000000 livemark-0.96.0/livemark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-08-19 07:40:59.000000 livemark-0.96.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-19 07:40:59.000000 livemark-0.96.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-19 07:40:59.000000 livemark-0.96.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-19 07:41:03.389454 livemark-0.96.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-08-19 07:40:59.000000 livemark-0.96.0/setup.py
```

### Comparing `livemark-0.95.0/LICENSE.md` & `livemark-0.96.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/Makefile` & `livemark-0.96.0/Makefile`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/PKG-INFO` & `livemark-0.96.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livemark
-Version: 0.95.0
+Version: 0.96.0
 Summary: Data presentation framework for Python that generates static sites from extended Markdown with interactive charts, tables, scripts, and other features.
 Home-page: https://github.com/frictionlessdata/livemark
 Author: Evgeny Karev
 Author-email: eskarev@gmail.com
 License: MIT
 Description: # Livemark
```

### Comparing `livemark-0.95.0/livemark/assets/documents/template.md` & `livemark-0.96.0/livemark/assets/documents/template.md`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/config.py` & `livemark-0.96.0/livemark/config.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/document.py` & `livemark-0.96.0/livemark/document.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/helpers.py` & `livemark-0.96.0/livemark/helpers.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/markup.py` & `livemark-0.96.0/livemark/markup.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugin.py` & `livemark-0.96.0/livemark/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/about/plugin.py` & `livemark-0.96.0/livemark/plugins/about/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/audio/plugin.py` & `livemark-0.96.0/livemark/plugins/audio/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/blog/index.md` & `livemark-0.96.0/livemark/plugins/blog/index.md`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/blog/plugin.py` & `livemark-0.96.0/livemark/plugins/blog/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/brand/plugin.py` & `livemark-0.96.0/livemark/plugins/brand/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/cards/markup.html` & `livemark-0.96.0/livemark/plugins/cards/markup.html`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/cards/plugin.py` & `livemark-0.96.0/livemark/plugins/cards/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/cards/script.js` & `livemark-0.96.0/livemark/plugins/cards/script.js`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/chart/plugin.py` & `livemark-0.96.0/livemark/plugins/chart/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/cleanup/plugin.py` & `livemark-0.96.0/livemark/plugins/cleanup/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/columns/plugin.py` & `livemark-0.96.0/livemark/plugins/columns/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/comments/plugin.py` & `livemark-0.96.0/livemark/plugins/comments/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/counter/plugin.py` & `livemark-0.96.0/livemark/plugins/counter/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/display/markup.html` & `livemark-0.96.0/livemark/plugins/display/markup.html`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/display/plugin.py` & `livemark-0.96.0/livemark/plugins/display/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/display/script.js` & `livemark-0.96.0/livemark/plugins/display/script.js`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/display/style.css` & `livemark-0.96.0/livemark/plugins/display/style.css`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/file/plugin.py` & `livemark-0.96.0/livemark/plugins/file/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/github/plugin.py` & `livemark-0.96.0/livemark/plugins/github/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/html/plugin.py` & `livemark-0.96.0/livemark/plugins/html/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/html/renderer.py` & `livemark-0.96.0/livemark/plugins/html/renderer.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/image/instagram.html` & `livemark-0.96.0/livemark/plugins/image/instagram.html`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/image/plugin.py` & `livemark-0.96.0/livemark/plugins/image/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/infinity/script.js` & `livemark-0.96.0/livemark/plugins/infinity/script.js`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/links/plugin.py` & `livemark-0.96.0/livemark/plugins/links/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/links/style.css` & `livemark-0.96.0/livemark/plugins/links/style.css`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/logic/plugin.py` & `livemark-0.96.0/livemark/plugins/logic/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/map/markup.html` & `livemark-0.96.0/livemark/plugins/map/markup.html`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/map/plugin.py` & `livemark-0.96.0/livemark/plugins/map/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/markdown/plugin.py` & `livemark-0.96.0/livemark/plugins/markdown/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/markdown/renderer.py` & `livemark-0.96.0/livemark/plugins/markdown/renderer.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/markup/plugin.py` & `livemark-0.96.0/livemark/plugins/markup/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/mobile/script.js` & `livemark-0.96.0/livemark/plugins/mobile/script.js`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/mobile/style.css` & `livemark-0.96.0/livemark/plugins/mobile/style.css`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/news/markup.html` & `livemark-0.96.0/livemark/plugins/news/markup.html`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/news/plugin.py` & `livemark-0.96.0/livemark/plugins/news/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/notebook/plugin.py` & `livemark-0.96.0/livemark/plugins/notebook/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/notes/plugin.py` & `livemark-0.96.0/livemark/plugins/notes/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/notes/style.css` & `livemark-0.96.0/livemark/plugins/notes/style.css`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/package/plugin.py` & `livemark-0.96.0/livemark/plugins/package/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/pages/markup.html` & `livemark-0.96.0/livemark/plugins/pages/markup.html`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/pages/plugin.py` & `livemark-0.96.0/livemark/plugins/pages/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/pages/style.css` & `livemark-0.96.0/livemark/plugins/pages/style.css`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/pagination/script.js` & `livemark-0.96.0/livemark/plugins/pagination/script.js`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/pipeline/plugin.py` & `livemark-0.96.0/livemark/plugins/pipeline/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/prepare/plugin.py` & `livemark-0.96.0/livemark/plugins/prepare/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/rating/plugin.py` & `livemark-0.96.0/livemark/plugins/rating/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/redirect/plugin.py` & `livemark-0.96.0/livemark/plugins/redirect/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/reference/plugin.py` & `livemark-0.96.0/livemark/plugins/reference/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/report/plugin.py` & `livemark-0.96.0/livemark/plugins/report/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/resource/plugin.py` & `livemark-0.96.0/livemark/plugins/resource/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/schema/plugin.py` & `livemark-0.96.0/livemark/plugins/schema/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/script/plugin.py` & `livemark-0.96.0/livemark/plugins/script/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/search/plugin.py` & `livemark-0.96.0/livemark/plugins/search/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/search/script.js` & `livemark-0.96.0/livemark/plugins/search/script.js`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/search/style.css` & `livemark-0.96.0/livemark/plugins/search/style.css`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/signs/plugin.py` & `livemark-0.96.0/livemark/plugins/signs/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/site/plugin.py` & `livemark-0.96.0/livemark/plugins/site/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/site/script.js` & `livemark-0.96.0/livemark/plugins/site/script.js`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/site/style.css` & `livemark-0.96.0/livemark/plugins/site/style.css`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/source/script.js` & `livemark-0.96.0/livemark/plugins/source/script.js`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/table/markup.html` & `livemark-0.96.0/livemark/plugins/table/markup.html`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/table/plugin.py` & `livemark-0.96.0/livemark/plugins/table/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/tabs/plugin.py` & `livemark-0.96.0/livemark/plugins/tabs/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/topics/plugin.py` & `livemark-0.96.0/livemark/plugins/topics/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/topics/script.js` & `livemark-0.96.0/livemark/plugins/topics/script.js`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/topics/style.css` & `livemark-0.96.0/livemark/plugins/topics/style.css`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/plugins/video/plugin.py` & `livemark-0.96.0/livemark/plugins/video/plugin.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/program/build.py` & `livemark-0.96.0/livemark/program/build.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/program/common.py` & `livemark-0.96.0/livemark/program/common.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/program/merge.py` & `livemark-0.96.0/livemark/program/merge.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/program/run.py` & `livemark-0.96.0/livemark/program/run.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/program/start.py` & `livemark-0.96.0/livemark/program/start.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/project.py` & `livemark-0.96.0/livemark/project.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/server.py` & `livemark-0.96.0/livemark/server.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/snippet.py` & `livemark-0.96.0/livemark/snippet.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark/system.py` & `livemark-0.96.0/livemark/system.py`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/livemark.egg-info/PKG-INFO` & `livemark-0.96.0/livemark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livemark
-Version: 0.95.0
+Version: 0.96.0
 Summary: Data presentation framework for Python that generates static sites from extended Markdown with interactive charts, tables, scripts, and other features.
 Home-page: https://github.com/frictionlessdata/livemark
 Author: Evgeny Karev
 Author-email: eskarev@gmail.com
 License: MIT
 Description: # Livemark
```

### Comparing `livemark-0.95.0/livemark.egg-info/SOURCES.txt` & `livemark-0.96.0/livemark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livemark-0.95.0/setup.py` & `livemark-0.96.0/setup.py`

 * *Files identical despite different names*

