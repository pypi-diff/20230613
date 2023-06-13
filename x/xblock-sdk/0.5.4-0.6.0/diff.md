# Comparing `tmp/xblock-sdk-0.5.4.tar.gz` & `tmp/xblock-sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-sdk-0.5.4.tar", last modified: Mon Jan 30 15:09:24 2023, max compression
+gzip compressed data, was "xblock-sdk-0.6.0.tar", last modified: Tue Jun 13 08:15:47 2023, max compression
```

## Comparing `xblock-sdk-0.5.4.tar` & `xblock-sdk-0.6.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.068751 xblock-sdk-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      543 2023-01-30 15:09:24.068751 xblock-sdk-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7853 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.052751 xblock-sdk-0.5.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/requirements/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.052751 xblock-sdk-0.5.4/sample_xblocks/
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.052751 xblock-sdk-0.5.4/sample_xblocks/basic/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8847 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/content.py
--rw-r--r--   0 runner    (1001) docker     (122)    21273 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.048751 xblock-sdk-0.5.4/sample_xblocks/basic/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.052751 xblock-sdk-0.5.4/sample_xblocks/basic/public/images/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/public/images/correct-icon.png
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/public/images/incorrect-icon.png
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/slider.py
--rw-r--r--   0 runner    (1001) docker     (122)     2953 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/basic/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/templates/problem.html
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/templates/sequence.html
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/templates/vertical.html
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/basic/view_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/filethumbs/
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/filethumbs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/css/thumbs.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/html/
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/html/thumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/SpecRunner.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    20765 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js
--rw-r--r--   0 runner    (1001) docker     (122)     6537 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.css
--rw-r--r--   0 runner    (1001) docker     (122)    70892 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.js
--rw-r--r--   0 runner    (1001) docker     (122)    20000 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-jquery.js
--rw-r--r--   0 runner    (1001) docker     (122)    92629 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jquery-1.9.1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/spec/
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/spec/thumbs_spec.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/src/thumbs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/thumbs/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/css/thumbs.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/html/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/html/thumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.056751 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/SpecRunner.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.060751 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.060751 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    20765 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js
--rw-r--r--   0 runner    (1001) docker     (122)     6537 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.css
--rw-r--r--   0 runner    (1001) docker     (122)    70892 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.js
--rw-r--r--   0 runner    (1001) docker     (122)    20000 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-jquery.js
--rw-r--r--   0 runner    (1001) docker     (122)    92629 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jquery-1.9.1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.060751 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/spec/
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/spec/thumbs_spec.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.060751 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (122)      879 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/src/thumbs.js
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/sample_xblocks/thumbs/thumbs.py
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-01-30 15:09:24.068751 xblock-sdk-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.060751 xblock-sdk-0.5.4/workbench/
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     4529 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    17975 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/runtime.py
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/services.py
--rw-r--r--   0 runner    (1001) docker     (122)     7051 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.052751 xblock-sdk-0.5.4/workbench/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.052751 xblock-sdk-0.5.4/workbench/static/workbench/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.060751 xblock-sdk-0.5.4/workbench/static/workbench/css/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/static/workbench/css/workbench.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.060751 xblock-sdk-0.5.4/workbench/static/workbench/images/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1546 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/static/workbench/images/header-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.052751 xblock-sdk-0.5.4/workbench/static/workbench/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.060751 xblock-sdk-0.5.4/workbench/static/workbench/js/runtime/
--rw-r--r--   0 runner    (1001) docker     (122)     4540 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/static/workbench/js/runtime/1.js
--rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/static/workbench/js/runtime/logger.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.064751 xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (122)     9459 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/jquery-migrate.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/jquery.cookie.js
--rw-r--r--   0 runner    (1001) docker     (122)    85659 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (122)    16449 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/underscore-min.js
--rw-r--r--   0 runner    (1001) docker     (122)    27589 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/underscore-min.map
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.064751 xblock-sdk-0.5.4/workbench/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/templates/500.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.064751 xblock-sdk-0.5.4/workbench/templates/workbench/
--rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/templates/workbench/block.html
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/templates/workbench/blockview.html
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/templates/workbench/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/templates/workbench/settings.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.064751 xblock-sdk-0.5.4/workbench/test/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/test/selenium_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/test/test_filethumbs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/test/test_problems.py
--rw-r--r--   0 runner    (1001) docker     (122)     6771 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (122)     3013 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/test/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/test/test_thumbs.py
--rw-r--r--   0 runner    (1001) docker     (122)    12325 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/test/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     4617 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     5544 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-01-30 15:09:19.000000 xblock-sdk-0.5.4/workbench/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 15:09:24.064751 xblock-sdk-0.5.4/xblock_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      543 2023-01-30 15:09:24.000000 xblock-sdk-0.5.4/xblock_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3614 2023-01-30 15:09:24.000000 xblock-sdk-0.5.4/xblock_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-30 15:09:24.000000 xblock-sdk-0.5.4/xblock_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-01-30 15:09:24.000000 xblock-sdk-0.5.4/xblock_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-30 15:09:24.000000 xblock-sdk-0.5.4/xblock_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-01-30 15:09:24.000000 xblock-sdk-0.5.4/xblock_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.978473 xblock-sdk-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-06-13 08:15:47.978473 xblock-sdk-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7853 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.966473 xblock-sdk-0.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/requirements/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.966473 xblock-sdk-0.6.0/sample_xblocks/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.966473 xblock-sdk-0.6.0/sample_xblocks/basic/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8847 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/content.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21273 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.962473 xblock-sdk-0.6.0/sample_xblocks/basic/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.966473 xblock-sdk-0.6.0/sample_xblocks/basic/public/images/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/public/images/correct-icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/public/images/incorrect-icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/slider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2953 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/basic/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/templates/problem.html
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/templates/sequence.html
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/templates/vertical.html
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/basic/view_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/filethumbs/
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/filethumbs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/css/thumbs.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/html/thumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/SpecRunner.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    20765 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6537 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.css
+-rw-r--r--   0 runner    (1001) docker     (122)    70892 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.js
+-rw-r--r--   0 runner    (1001) docker     (122)    20000 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-jquery.js
+-rw-r--r--   0 runner    (1001) docker     (122)    92629 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jquery-1.9.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/spec/
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/spec/thumbs_spec.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/src/thumbs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/thumbs/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/css/thumbs.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/html/thumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/SpecRunner.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.970473 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.974473 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    20765 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6537 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.css
+-rw-r--r--   0 runner    (1001) docker     (122)    70892 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.js
+-rw-r--r--   0 runner    (1001) docker     (122)    20000 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-jquery.js
+-rw-r--r--   0 runner    (1001) docker     (122)    92629 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jquery-1.9.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.974473 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/spec/
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/spec/thumbs_spec.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.974473 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/src/thumbs.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/sample_xblocks/thumbs/thumbs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-13 08:15:47.978473 xblock-sdk-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.974473 xblock-sdk-0.6.0/workbench/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4529 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17975 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/services.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7051 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.966473 xblock-sdk-0.6.0/workbench/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.966473 xblock-sdk-0.6.0/workbench/static/workbench/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.974473 xblock-sdk-0.6.0/workbench/static/workbench/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/static/workbench/css/workbench.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.974473 xblock-sdk-0.6.0/workbench/static/workbench/images/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1546 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/static/workbench/images/header-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.966473 xblock-sdk-0.6.0/workbench/static/workbench/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.974473 xblock-sdk-0.6.0/workbench/static/workbench/js/runtime/
+-rw-r--r--   0 runner    (1001) docker     (122)     4540 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/static/workbench/js/runtime/1.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/static/workbench/js/runtime/logger.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.978473 xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)     9459 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/jquery-migrate.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/jquery.cookie.js
+-rw-r--r--   0 runner    (1001) docker     (122)    85659 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    16449 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/underscore-min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    27589 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/underscore-min.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.978473 xblock-sdk-0.6.0/workbench/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/templates/500.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.978473 xblock-sdk-0.6.0/workbench/templates/workbench/
+-rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/templates/workbench/block.html
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/templates/workbench/blockview.html
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/templates/workbench/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/templates/workbench/settings.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.978473 xblock-sdk-0.6.0/workbench/test/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/test/selenium_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/test/test_filethumbs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/test/test_problems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6771 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3013 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/test/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/test/test_thumbs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12325 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/test/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4617 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5544 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-06-13 08:15:34.000000 xblock-sdk-0.6.0/workbench/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:15:47.978473 xblock-sdk-0.6.0/xblock_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-06-13 08:15:47.000000 xblock-sdk-0.6.0/xblock_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3614 2023-06-13 08:15:47.000000 xblock-sdk-0.6.0/xblock_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:15:47.000000 xblock-sdk-0.6.0/xblock_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-06-13 08:15:47.000000 xblock-sdk-0.6.0/xblock_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-13 08:15:47.000000 xblock-sdk-0.6.0/xblock_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-13 08:15:47.000000 xblock-sdk-0.6.0/xblock_sdk.egg-info/top_level.txt
```

### Comparing `xblock-sdk-0.5.4/CHANGELOG.rst` & `xblock-sdk-0.6.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 =============================
 Change history for XBlock SDK
 =============================
 
 These are notable changes in XBlock.
 
+0.6.0
+-----
+* Removed boto usage.
+* openedx-django-pyf is now using boto3 to generate URL.
+
 0.5.0
 -----
 * Removed Django22, 30 and 31 support
 * Added Django40 support
 * Renamed CI job so that our modernizers work fine
 * Code changes related to things removed in Django40
```

### Comparing `xblock-sdk-0.5.4/LICENSE.TXT` & `xblock-sdk-0.6.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/PKG-INFO` & `xblock-sdk-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-sdk
-Version: 0.5.4
+Version: 0.6.0
 Summary: XBlock SDK
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `xblock-sdk-0.5.4/README.rst` & `xblock-sdk-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/requirements/test.txt` & `xblock-sdk-0.6.0/requirements/test.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,70 +10,66 @@
     # via
     #   -r requirements/base.txt
     #   fs
 arrow==1.2.3
     # via
     #   -r requirements/base.txt
     #   jinja2-time
-asgiref==3.6.0
+asgiref==3.7.2
     # via
     #   -r requirements/base.txt
     #   django
-attrs==22.2.0
-    # via pytest
 binaryornot==0.4.4
     # via
     #   -r requirements/base.txt
     #   cookiecutter
 bok-choy==0.7.1
     # via -r requirements/test.in
-boto==2.49.0
-    # via -r requirements/base.txt
-boto3==1.26.58
+boto3==1.26.146
     # via
     #   -r requirements/base.txt
     #   fs-s3fs
-botocore==1.29.58
+botocore==1.29.146
     # via
     #   -r requirements/base.txt
     #   boto3
     #   s3transfer
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   -r requirements/base.txt
     #   requests
 chardet==5.1.0
     # via
     #   -r requirements/base.txt
     #   binaryornot
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via
     #   -r requirements/base.txt
     #   requests
 click==8.1.3
     # via
     #   -r requirements/base.txt
     #   cookiecutter
 cookiecutter==2.1.1
     # via -r requirements/base.txt
-coverage[toml]==7.1.0
+coverage[toml]==7.2.7
     # via
     #   -r requirements/test.in
     #   pytest-cov
 ddt==1.6.0
     # via -r requirements/test.in
 distlib==0.3.6
     # via virtualenv
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/base.txt
     #   openedx-django-pyfs
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
-filelock==3.9.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 fs==2.4.16
     # via
     #   -r requirements/base.txt
     #   fs-s3fs
@@ -111,102 +107,102 @@
     #   xblock
 lxml==4.9.2
     # via
     #   -r requirements/base.txt
     #   xblock
 mako==1.2.4
     # via acid-xblock
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   -r requirements/base.txt
     #   jinja2
     #   mako
     #   xblock
-mock==5.0.1
+mock==5.0.2
     # via -r requirements/test.in
 needle==0.5.0
     # via bok-choy
 nose==1.3.7
     # via needle
-openedx-django-pyfs==3.2.1
+openedx-django-pyfs==3.3.0
     # via
     #   -r requirements/base.txt
     #   xblock
-packaging==23.0
+packaging==23.1
     # via
     #   pytest
     #   pytest-rerunfailures
     #   tox
-pillow==9.4.0
+pillow==9.5.0
     # via needle
-platformdirs==2.6.2
+platformdirs==3.5.1
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 py==1.11.0
     # via tox
 pypng==0.20220715.0
     # via -r requirements/base.txt
-pytest==7.2.1
+pytest==7.3.1
     # via
     #   pytest-cov
     #   pytest-django
     #   pytest-rerunfailures
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements/test.in
 pytest-django==4.5.2
     # via -r requirements/test.in
-pytest-rerunfailures==11.0
+pytest-rerunfailures==11.1.2
     # via -r requirements/test.in
 python-dateutil==2.8.2
     # via
     #   -r requirements/base.txt
     #   arrow
     #   botocore
     #   xblock
-python-slugify==7.0.0
+python-slugify==8.0.1
     # via
     #   -r requirements/base.txt
     #   cookiecutter
-pytz==2022.7.1
+pytz==2023.3
     # via
     #   -r requirements/base.txt
     #   django
     #   xblock
 pyyaml==6.0
     # via
     #   -r requirements/base.txt
     #   cookiecutter
     #   xblock
-requests==2.28.2
+requests==2.31.0
     # via
     #   -r requirements/base.txt
     #   cookiecutter
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via
     #   -r requirements/base.txt
     #   boto3
 selenium==3.4.1
     # via
     #   -r requirements/test.in
     #   bok-choy
     #   needle
-simplejson==3.18.1
+simplejson==3.19.1
     # via -r requirements/base.txt
 six==1.16.0
     # via
     #   -r requirements/base.txt
     #   bok-choy
     #   fs
     #   fs-s3fs
     #   python-dateutil
     #   tox
-sqlparse==0.4.3
+sqlparse==0.4.4
     # via
     #   -r requirements/base.txt
     #   django
 text-unidecode==1.3
     # via
     #   -r requirements/base.txt
     #   python-slugify
@@ -218,20 +214,24 @@
 tox==3.28.0
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/test.in
     #   tox-battery
 tox-battery==0.6.1
     # via -r requirements/test.in
-urllib3==1.26.14
+typing-extensions==4.6.3
+    # via
+    #   -r requirements/base.txt
+    #   asgiref
+urllib3==1.26.16
     # via
     #   -r requirements/base.txt
     #   botocore
     #   requests
-virtualenv==20.17.1
+virtualenv==20.23.0
     # via tox
 web-fragments==2.0.0
     # via
     #   -r requirements/base.txt
     #   xblock
 webob==1.8.7
     # via
```

### Comparing `xblock-sdk-0.5.4/sample_xblocks/basic/content.py` & `xblock-sdk-0.6.0/sample_xblocks/basic/content.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/basic/problem.py` & `xblock-sdk-0.6.0/sample_xblocks/basic/problem.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/basic/slider.py` & `xblock-sdk-0.6.0/sample_xblocks/basic/slider.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/basic/structure.py` & `xblock-sdk-0.6.0/sample_xblocks/basic/structure.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/basic/view_counter.py` & `xblock-sdk-0.6.0/sample_xblocks/basic/view_counter.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/filethumbs.py` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/filethumbs.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/SpecRunner.html` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/SpecRunner.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.css` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.css`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.js` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jasmine-jquery.js` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jasmine-jquery.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/lib/jquery-1.9.1.min.js` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/lib/jquery-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/spec/thumbs_spec.js` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/spec/thumbs_spec.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/filethumbs/static/js/src/thumbs.js` & `xblock-sdk-0.6.0/sample_xblocks/filethumbs/static/js/src/thumbs.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/SpecRunner.html` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/SpecRunner.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.css` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.css`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.js` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jasmine-jquery.js` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jasmine-jquery.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/lib/jquery-1.9.1.min.js` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/lib/jquery-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/spec/thumbs_spec.js` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/spec/thumbs_spec.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/static/js/src/thumbs.js` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/static/js/src/thumbs.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/sample_xblocks/thumbs/thumbs.py` & `xblock-sdk-0.6.0/sample_xblocks/thumbs/thumbs.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/setup.py` & `xblock-sdk-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/admin.py` & `xblock-sdk-0.6.0/workbench/admin.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/blocks.py` & `xblock-sdk-0.6.0/workbench/blocks.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/models.py` & `xblock-sdk-0.6.0/workbench/models.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/runtime.py` & `xblock-sdk-0.6.0/workbench/runtime.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/scenarios.py` & `xblock-sdk-0.6.0/workbench/scenarios.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/services.py` & `xblock-sdk-0.6.0/workbench/services.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/settings.py` & `xblock-sdk-0.6.0/workbench/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/static/workbench/css/workbench.css` & `xblock-sdk-0.6.0/workbench/static/workbench/css/workbench.css`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/static/workbench/images/header-logo.png` & `xblock-sdk-0.6.0/workbench/static/workbench/images/header-logo.png`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/static/workbench/js/runtime/1.js` & `xblock-sdk-0.6.0/workbench/static/workbench/js/runtime/1.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/static/workbench/js/runtime/logger.js` & `xblock-sdk-0.6.0/workbench/static/workbench/js/runtime/logger.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/jquery-migrate.min.js` & `xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/jquery-migrate.min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/jquery.cookie.js` & `xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/jquery.min.js` & `xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/jquery.min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/underscore-min.js` & `xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/underscore-min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/static/workbench/js/vendor/underscore-min.map` & `xblock-sdk-0.6.0/workbench/static/workbench/js/vendor/underscore-min.map`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/templates/workbench/block.html` & `xblock-sdk-0.6.0/workbench/templates/workbench/block.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/templates/workbench/blockview.html` & `xblock-sdk-0.6.0/workbench/templates/workbench/blockview.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/templates/workbench/index.html` & `xblock-sdk-0.6.0/workbench/templates/workbench/index.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/test/selenium_test.py` & `xblock-sdk-0.6.0/workbench/test/selenium_test.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/test/test_filethumbs.py` & `xblock-sdk-0.6.0/workbench/test/test_filethumbs.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/test/test_problems.py` & `xblock-sdk-0.6.0/workbench/test/test_problems.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/test/test_runtime.py` & `xblock-sdk-0.6.0/workbench/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/test/test_scenarios.py` & `xblock-sdk-0.6.0/workbench/test/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/test/test_thumbs.py` & `xblock-sdk-0.6.0/workbench/test/test_thumbs.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/test/test_views.py` & `xblock-sdk-0.6.0/workbench/test/test_views.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/test_utils.py` & `xblock-sdk-0.6.0/workbench/test_utils.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/urls.py` & `xblock-sdk-0.6.0/workbench/urls.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/views.py` & `xblock-sdk-0.6.0/workbench/views.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/workbench/wsgi.py` & `xblock-sdk-0.6.0/workbench/wsgi.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/xblock_sdk.egg-info/PKG-INFO` & `xblock-sdk-0.6.0/xblock_sdk.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-sdk
-Version: 0.5.4
+Version: 0.6.0
 Summary: XBlock SDK
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `xblock-sdk-0.5.4/xblock_sdk.egg-info/SOURCES.txt` & `xblock-sdk-0.6.0/xblock_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.5.4/xblock_sdk.egg-info/entry_points.txt` & `xblock-sdk-0.6.0/xblock_sdk.egg-info/entry_points.txt`

 * *Files identical despite different names*

