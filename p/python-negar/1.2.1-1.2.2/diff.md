# Comparing `tmp/python-negar-1.2.1.tar.gz` & `tmp/python-negar-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-negar-1.2.1.tar", last modified: Fri May 19 07:45:40 2023, max compression
+gzip compressed data, was "python-negar-1.2.2.tar", last modified: Tue Jun 13 07:25:33 2023, max compression
```

## Comparing `python-negar-1.2.1.tar` & `python-negar-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-19 07:45:40.341991 python-negar-1.2.1/
--rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2.1/AUTHORS
--rw-r--r--   0 javad     (1000) javad     (1000)     6531 2023-05-19 07:44:53.000000 python-negar-1.2.1/Changelog.txt
--rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2.1/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1000)      149 2022-03-28 12:06:56.000000 python-negar-1.2.1/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-05-19 07:45:40.338657 python-negar-1.2.1/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2.1/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-19 07:45:40.338657 python-negar-1.2.1/negar/
--rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2.1/negar/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)     5047 2023-05-19 07:23:16.000000 python-negar-1.2.1/negar/constants.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-19 07:45:40.338657 python-negar-1.2.1/negar/data/
--rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2.1/negar/data/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2.1/negar/data/untouchable.dat
--rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2.1/negar/gui.py
--rw-r--r--   0 javad     (1000) javad     (1000)    14546 2023-05-19 07:36:41.000000 python-negar-1.2.1/negar/virastar.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-19 07:45:40.338657 python-negar-1.2.1/python_negar.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)      396 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       42 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/entry_points.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/requires.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-05-19 07:45:40.341991 python-negar-1.2.1/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1000)     1541 2022-05-30 08:43:57.000000 python-negar-1.2.1/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:25:33.562564 python-negar-1.2.2/
+-rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2.2/AUTHORS
+-rw-r--r--   0 javad     (1000) javad     (1000)     6628 2023-06-13 07:21:27.000000 python-negar-1.2.2/Changelog.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2.2/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1000)      149 2022-03-28 12:06:56.000000 python-negar-1.2.2/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-06-13 07:25:33.562564 python-negar-1.2.2/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2.2/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:25:33.562564 python-negar-1.2.2/negar/
+-rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2.2/negar/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     5047 2023-06-13 07:19:47.000000 python-negar-1.2.2/negar/constants.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:25:33.562564 python-negar-1.2.2/negar/data/
+-rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2.2/negar/data/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2.2/negar/data/untouchable.dat
+-rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2.2/negar/gui.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    14615 2023-06-13 07:24:29.000000 python-negar-1.2.2/negar/virastar.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:25:33.562564 python-negar-1.2.2/python_negar.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-06-13 07:25:33.000000 python-negar-1.2.2/python_negar.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)      396 2023-06-13 07:25:33.000000 python-negar-1.2.2/python_negar.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-06-13 07:25:33.000000 python-negar-1.2.2/python_negar.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       42 2023-06-13 07:25:33.000000 python-negar-1.2.2/python_negar.egg-info/entry_points.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-06-13 07:25:33.000000 python-negar-1.2.2/python_negar.egg-info/requires.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-06-13 07:25:33.000000 python-negar-1.2.2/python_negar.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-06-13 07:25:33.562564 python-negar-1.2.2/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1000)     1541 2022-05-30 08:43:57.000000 python-negar-1.2.2/setup.py
```

### Comparing `python-negar-1.2.1/Changelog.txt` & `python-negar-1.2.2/Changelog.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+1.2.2 - 2023-06-13
+-- Fix the issue with the triple dots that was caused by the previous update
+
 1.2.1 - 2023-05-23
 -- Fix an issue with punctuation like  '،ساختمان'
 
 1.2 - 2023-03-28
 -- Fix GUI execution issue
 
 1.1.17 - 2022-12-21
```

### Comparing `python-negar-1.2.1/LICENSE` & `python-negar-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.1/PKG-INFO` & `python-negar-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2.1
+Version: 1.2.2
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2.1/README.md` & `python-negar-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.1/negar/constants.py` & `python-negar-1.2.2/negar/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 DATAFILE = Path(__file__).parent.absolute() / "data/untouchable.dat"
 USERFILE = Path.home() / ".python-negar"
 
 INFO = f"""قابلیت های ویراستار ' نگار  ' -- نسخه {__version__} :
 * جایگزینی
 	╛═ خط تیره های پیاپی نظیر (--) و (---) با معادل های استاندارد شان
```

### Comparing `python-negar-1.2.1/negar/data/untouchable.dat` & `python-negar-1.2.2/negar/data/untouchable.dat`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.1/negar/virastar.py` & `python-negar-1.2.2/negar/virastar.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,24 +46,25 @@
         UnTouchable() # to generate the untouchable words
         self.cleanup()
 
     def cleanup(self):
         self._handle_urls(State.save)
         # fix punctuation spaces at first
         # : ; , ! ? and their Persian counterparts should have one space after and no space before
+        # An exception is triple dots, which should be handled first
+        self.fix_three_dots()       if self._fix_three_dots else None
         self.text = re.sub(
             r'[ ‌ ]*([:;,؛،.؟!]{1})[ ‌ ]*',
             r'\1 ',
             self.text
         )
         if self._trim_leading_trailing_whitespaces:
             self.text = '\n'.join([line.strip() for line in self.text.split('\n')])
         self.cleanup_spacing()      if self._cleanup_spacing else None
         self.fix_dashes()           if self._fix_dashes else None
-        self.fix_three_dots()       if self._fix_three_dots else None
         self.fix_english_quotes()   if self._fix_english_quotes else None
         self.fix_hamzeh()           if self._fix_hamzeh else None
         self.cleanup_zwnj()         if self._cleanup_zwnj else None
         self.char_validator()       if self._fix_misc_non_persian_chars else None
         self.fix_arabic_numbers()   if self._fix_arabic_numbers else None
         self.fix_english_numbers()  if self._fix_english_numbers else None
         self.fix_prefix_spacing()   if self._fix_prefix_spacing else None
```

### Comparing `python-negar-1.2.1/python_negar.egg-info/PKG-INFO` & `python-negar-1.2.2/python_negar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2.1
+Version: 1.2.2
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2.1/setup.py` & `python-negar-1.2.2/setup.py`

 * *Files identical despite different names*

