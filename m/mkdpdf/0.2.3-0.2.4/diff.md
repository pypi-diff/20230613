# Comparing `tmp/mkdpdf-0.2.3.tar.gz` & `tmp/mkdpdf-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdpdf-0.2.3.tar", last modified: Sun May 21 19:44:40 2023, max compression
+gzip compressed data, was "mkdpdf-0.2.4.tar", last modified: Mon Jun 12 22:10:29 2023, max compression
```

## Comparing `mkdpdf-0.2.3.tar` & `mkdpdf-0.2.4.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.838466 mkdpdf-0.2.3/
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-21 19:44:40.837466 mkdpdf-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.830466 mkdpdf-0.2.3/mkdpdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.832466 mkdpdf-0.2.3/mkdpdf/document/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/document/document.md
--rw-rw-rw-   0 root         (0) root         (0)    11386 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/document/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.828466 mkdpdf-0.2.3/mkdpdf/document/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.828466 mkdpdf-0.2.3/mkdpdf/document/templates/pdf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.833466 mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/header.css
--rw-rw-rw-   0 root         (0) root         (0)     6683 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/mermaid.css
--rw-rw-rw-   0 root         (0) root         (0)     2193 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/pdf.css
--rw-rw-rw-   0 root         (0) root         (0)     3199 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/reset.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.833466 mkdpdf-0.2.3/mkdpdf/documentation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8053 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/documentation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.828466 mkdpdf-0.2.3/mkdpdf/documentation/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.833466 mkdpdf-0.2.3/mkdpdf/documentation/templates/md/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.834466 mkdpdf-0.2.3/mkdpdf/documentation/templates/md/class/
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/templates/md/class/header.md
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/templates/md/class/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.834466 mkdpdf-0.2.3/mkdpdf/documentation/templates/md/functions/
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/templates/md/functions/header.md
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/templates/md/functions/main.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/templates/md/header.md
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/templates/md/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.828466 mkdpdf-0.2.3/mkdpdf/documentation/templates/pdf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.835466 mkdpdf-0.2.3/mkdpdf/documentation/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/documentation/templates/pdf/style/header.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.835466 mkdpdf-0.2.3/mkdpdf/md/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/md/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/md/md.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.835466 mkdpdf-0.2.3/mkdpdf/pdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/pdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4763 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/pdf/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/pdf/publisher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.836466 mkdpdf-0.2.3/mkdpdf/report/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.829466 mkdpdf-0.2.3/mkdpdf/report/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.836466 mkdpdf-0.2.3/mkdpdf/report/templates/md/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/templates/md/footer.md
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/templates/md/header.md
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/templates/md/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.837466 mkdpdf-0.2.3/mkdpdf/report/templates/pdf/
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/templates/pdf/footer.html
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/templates/pdf/header.html
--rw-rw-rw-   0 root         (0) root         (0)     1338 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/templates/pdf/main.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.837466 mkdpdf-0.2.3/mkdpdf/report/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)     1518 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/report/templates/pdf/style/header.css
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/mkdpdf/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:44:40.831466 mkdpdf-0.2.3/mkdpdf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-21 19:44:40.000000 mkdpdf-0.2.3/mkdpdf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1723 2023-05-21 19:44:40.000000 mkdpdf-0.2.3/mkdpdf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 19:44:40.000000 mkdpdf-0.2.3/mkdpdf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-21 19:44:40.000000 mkdpdf-0.2.3/mkdpdf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-21 19:44:40.000000 mkdpdf-0.2.3/mkdpdf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 19:44:40.000000 mkdpdf-0.2.3/mkdpdf.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 19:44:40.838466 mkdpdf-0.2.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      976 2023-05-21 19:44:33.000000 mkdpdf-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.709650 mkdpdf-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-12 22:10:29.708649 mkdpdf-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.701650 mkdpdf-0.2.4/mkdpdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.703650 mkdpdf-0.2.4/mkdpdf/document/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11411 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.699650 mkdpdf-0.2.4/mkdpdf/document/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.699650 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.704650 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/header.css
+-rw-rw-rw-   0 root         (0) root         (0)     6683 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/mermaid.css
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/pdf.css
+-rw-rw-rw-   0 root         (0) root         (0)     3199 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/reset.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.704650 mkdpdf-0.2.4/mkdpdf/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8053 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/documentation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.699650 mkdpdf-0.2.4/mkdpdf/documentation/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.704650 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.705650 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/class/
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/class/header.md
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/class/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.705650 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/functions/
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/functions/header.md
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/functions/main.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/header.md
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.699650 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.706650 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/style/header.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.706650 mkdpdf-0.2.4/mkdpdf/md/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/md/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/md/md.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.706650 mkdpdf-0.2.4/mkdpdf/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/pdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4763 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/pdf/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/pdf/publisher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.707650 mkdpdf-0.2.4/mkdpdf/report/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.700650 mkdpdf-0.2.4/mkdpdf/report/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.707650 mkdpdf-0.2.4/mkdpdf/report/templates/md/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/md/footer.md
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/md/header.md
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/md/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.708649 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/header.html
+-rw-rw-rw-   0 root         (0) root         (0)     1338 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/main.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.708649 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/header.css
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.702650 mkdpdf-0.2.4/mkdpdf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 22:10:29.709650 mkdpdf-0.2.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      976 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/setup.py
```

### Comparing `mkdpdf-0.2.3/mkdpdf/configuration.py` & `mkdpdf-0.2.4/mkdpdf/configuration.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/document/document.py` & `mkdpdf-0.2.4/mkdpdf/document/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             email_host (string): email domain from which to send
             filename (string): name of output file
             format (enum): md || pdf
         """
 
         # determine where submodule is
         # package or console script
-        stack_callers = [d[1] for d in inspect.stack() if d[1].startswith("/tmp/ipykernel_") or not d[1].endswith(".py")]
+        stack_callers = [d[1] for d in inspect.stack() if d[1].startswith("/tmp/ipykernel_") or (not d[1].endswith(".py") and d[1] != "<string>")]
         run_from_stack = len([d for d in stack_callers if "bin" not in d]) > 0
 
         # if running from stack
         if run_from_stack:
 
             stack_kernel_file = stack_callers[0]
             index_of_stack_kernel = [d[1] for d in inspect.stack()].index(stack_kernel_file)
```

### Comparing `mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/mermaid.css` & `mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/mermaid.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/pdf.css` & `mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/pdf.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/document/templates/pdf/style/reset.css` & `mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/reset.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/documentation/documentation.py` & `mkdpdf-0.2.4/mkdpdf/documentation/documentation.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/documentation/templates/md/class/header.md` & `mkdpdf-0.2.4/mkdpdf/documentation/templates/md/class/header.md`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/documentation/templates/md/functions/header.md` & `mkdpdf-0.2.4/mkdpdf/documentation/templates/md/functions/header.md`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/md/md.py` & `mkdpdf-0.2.4/mkdpdf/md/md.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/pdf/pdf.py` & `mkdpdf-0.2.4/mkdpdf/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/pdf/publisher.py` & `mkdpdf-0.2.4/mkdpdf/pdf/publisher.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/report/report.py` & `mkdpdf-0.2.4/mkdpdf/report/report.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/report/templates/pdf/header.html` & `mkdpdf-0.2.4/mkdpdf/report/templates/pdf/header.html`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/report/templates/pdf/main.html` & `mkdpdf-0.2.4/mkdpdf/report/templates/pdf/main.html`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/report/templates/pdf/style/footer.css` & `mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/footer.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/report/templates/pdf/style/header.css` & `mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/header.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf/utilities.py` & `mkdpdf-0.2.4/mkdpdf/utilities.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.3/mkdpdf.egg-info/SOURCES.txt` & `mkdpdf-0.2.4/mkdpdf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 mkdpdf.egg-info/PKG-INFO
 mkdpdf.egg-info/SOURCES.txt
 mkdpdf.egg-info/dependency_links.txt
 mkdpdf.egg-info/entry_points.txt
 mkdpdf.egg-info/requires.txt
 mkdpdf.egg-info/top_level.txt
 mkdpdf/document/__init__.py
-mkdpdf/document/document.md
 mkdpdf/document/document.py
 mkdpdf/document/templates/pdf/style/document.css
 mkdpdf/document/templates/pdf/style/footer.css
 mkdpdf/document/templates/pdf/style/header.css
 mkdpdf/document/templates/pdf/style/mermaid.css
 mkdpdf/document/templates/pdf/style/pdf.css
 mkdpdf/document/templates/pdf/style/reset.css
```

### Comparing `mkdpdf-0.2.3/setup.py` & `mkdpdf-0.2.4/setup.py`

 * *Files identical despite different names*

