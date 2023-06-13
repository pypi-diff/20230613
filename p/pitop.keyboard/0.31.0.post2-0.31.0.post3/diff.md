# Comparing `tmp/pitop.keyboard-0.31.0.post2.tar.gz` & `tmp/pitop.keyboard-0.31.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.keyboard-0.31.0.post2.tar", last modified: Mon May 22 19:13:11 2023, max compression
+gzip compressed data, was "dist/pitop.keyboard-0.31.0.post3.tar", last modified: Tue Jun 13 16:41:53 2023, max compression
```

## Comparing `pitop.keyboard-0.31.0.post2.tar` & `pitop.keyboard-0.31.0.post3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/keyboard_button.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/
--rw-r--r--   0 runner    (1001) docker     (122)     9451 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/darwin.py
--rw-r--r--   0 runner    (1001) docker     (122)    19147 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/win32.py
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/win32_vks.py
--rw-r--r--   0 runner    (1001) docker     (122)    14816 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/xorg.py
--rw-r--r--   0 runner    (1001) docker     (122)    67712 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/xorg_keysyms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/
--rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20508 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7941 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/_darwin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8857 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/_win32.py
--rw-r--r--   0 runner    (1001) docker     (122)    20449 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/_xorg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8486 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6799 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/_darwin.py
--rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/_win32.py
--rw-r--r--   0 runner    (1001) docker     (122)     5276 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/_xorg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop.keyboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop.keyboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop.keyboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop.keyboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop.keyboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/pitop.keyboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:11.000000 pitop.keyboard-0.31.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-05-22 19:12:55.000000 pitop.keyboard-0.31.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/keyboard_button.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/
+-rw-r--r--   0 runner    (1001) docker     (122)     9451 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/darwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19147 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/win32.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/win32_vks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14816 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/xorg.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67712 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/xorg_keysyms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/
+-rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20508 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7941 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/_darwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8857 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/_win32.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20449 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/_xorg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8486 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6799 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/_darwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/_win32.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5276 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/_xorg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop.keyboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop.keyboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop.keyboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop.keyboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop.keyboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/pitop.keyboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:53.000000 pitop.keyboard-0.31.0.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-06-13 16:41:37.000000 pitop.keyboard-0.31.0.post3/setup.py
```

### Comparing `pitop.keyboard-0.31.0.post2/PKG-INFO` & `pitop.keyboard-0.31.0.post3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.keyboard
-Version: 0.31.0.post2
+Version: 0.31.0.post3
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Keyboard
```

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/keyboard_button.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/LICENSE` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/LICENSE`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/__init__.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_info.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_info.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/__init__.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/darwin.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/darwin.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/win32.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/win32.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/win32_vks.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/win32_vks.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/xorg.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/xorg.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/_util/xorg_keysyms.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/_util/xorg_keysyms.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/__init__.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/_base.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/_base.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/_darwin.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/_darwin.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/_win32.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/_win32.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/keyboard/_xorg.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/keyboard/_xorg.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/__init__.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/_base.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/_base.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/_darwin.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/_darwin.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/_win32.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/_win32.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop/keyboard/vendor/pynput/mouse/_xorg.py` & `pitop.keyboard-0.31.0.post3/pitop/keyboard/vendor/pynput/mouse/_xorg.py`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/pitop.keyboard.egg-info/PKG-INFO` & `pitop.keyboard-0.31.0.post3/pitop.keyboard.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.keyboard
-Version: 0.31.0.post2
+Version: 0.31.0.post3
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Keyboard
```

### Comparing `pitop.keyboard-0.31.0.post2/pitop.keyboard.egg-info/SOURCES.txt` & `pitop.keyboard-0.31.0.post3/pitop.keyboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.keyboard-0.31.0.post2/setup.py` & `pitop.keyboard-0.31.0.post3/setup.py`

 * *Files identical despite different names*

