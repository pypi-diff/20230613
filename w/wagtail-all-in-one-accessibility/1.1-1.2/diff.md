# Comparing `tmp/wagtail-all-in-one-accessibility-1.1.tar.gz` & `tmp/wagtail-all-in-one-accessibility-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-all-in-one-accessibility-1.1.tar", last modified: Tue Jun 13 06:54:52 2023, max compression
+gzip compressed data, was "wagtail-all-in-one-accessibility-1.2.tar", last modified: Tue Jun 13 09:26:44 2023, max compression
```

## Comparing `wagtail-all-in-one-accessibility-1.1.tar` & `wagtail-all-in-one-accessibility-1.2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:54:52.022575 wagtail-all-in-one-accessibility-1.1/
--rw-rw-rw-   0        0        0      960 2023-06-13 06:54:52.022575 wagtail-all-in-one-accessibility-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-13 06:54:38.000000 wagtail-all-in-one-accessibility-1.1/Readme.md
-drwxrwxrwx   0        0        0        0 2023-06-13 06:54:51.998640 wagtail-all-in-one-accessibility-1.1/search/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.1/search/__init__.py
--rw-rw-rw-   0        0        0     1057 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.1/search/views.py
--rw-rw-rw-   0        0        0     1008 2023-06-13 06:54:52.023573 wagtail-all-in-one-accessibility-1.1/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-13 06:47:38.000000 wagtail-all-in-one-accessibility-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:54:52.004624 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-06-12 10:02:50.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/admin.py
--rw-rw-rw-   0        0        0      198 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/apps.py
--rw-rw-rw-   0        0        0     1138 2023-06-12 13:12:27.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/context_processors.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:54:52.011606 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/migrations/
--rw-rw-rw-   0        0        0     2067 2023-06-12 10:04:21.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      648 2023-06-12 12:22:09.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/migrations/0002_alter_wagtail_all_in_one_accessibility_aioa_license_key.py
--rw-rw-rw-   0        0        0        0 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/migrations/__init__.py
--rw-rw-rw-   0        0        0     1921 2023-06-12 13:12:35.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/models.py
--rw-rw-rw-   0        0        0       63 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/tests.py
--rw-rw-rw-   0        0        0      548 2023-06-12 10:03:16.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/urls.py
--rw-rw-rw-   0        0        0      108 2023-06-12 10:02:19.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/views.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:54:52.008613 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility.egg-info/
--rw-rw-rw-   0        0        0      960 2023-06-13 06:54:51.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2023-06-13 06:54:51.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:54:51.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-13 06:54:51.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-06-13 06:54:51.000000 wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 06:54:52.019584 wagtail-all-in-one-accessibility-1.1/wagtail_package/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.1/wagtail_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:54:52.022575 wagtail-all-in-one-accessibility-1.1/wagtail_package/settings/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.1/wagtail_package/settings/__init__.py
--rw-rw-rw-   0        0        0     4791 2023-06-12 12:18:51.000000 wagtail-all-in-one-accessibility-1.1/wagtail_package/settings/base.py
--rw-rw-rw-   0        0        0      478 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.1/wagtail_package/settings/dev.py
--rw-rw-rw-   0        0        0      103 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.1/wagtail_package/settings/production.py
--rw-rw-rw-   0        0        0     1447 2023-06-12 10:07:02.000000 wagtail-all-in-one-accessibility-1.1/wagtail_package/urls.py
--rw-rw-rw-   0        0        0      427 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.1/wagtail_package/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:44.903145 wagtail-all-in-one-accessibility-1.2/
+-rw-rw-rw-   0        0        0      973 2023-06-13 09:26:44.903145 wagtail-all-in-one-accessibility-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:44.866424 wagtail-all-in-one-accessibility-1.2/search/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.2/search/__init__.py
+-rw-rw-rw-   0        0        0     1057 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.2/search/views.py
+-rw-rw-rw-   0        0        0     1021 2023-06-13 09:26:44.904140 wagtail-all-in-one-accessibility-1.2/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-13 06:47:38.000000 wagtail-all-in-one-accessibility-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:44.875405 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/__init__.py
+-rw-rw-rw-   0        0        0     1042 2023-06-12 10:02:50.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/admin.py
+-rw-rw-rw-   0        0        0      198 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/apps.py
+-rw-rw-rw-   0        0        0     1138 2023-06-12 13:12:27.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/context_processors.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:44.884376 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/migrations/
+-rw-rw-rw-   0        0        0     2067 2023-06-12 10:04:21.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      648 2023-06-12 12:22:09.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/migrations/0002_alter_wagtail_all_in_one_accessibility_aioa_license_key.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1921 2023-06-12 13:12:35.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/models.py
+-rw-rw-rw-   0        0        0       63 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/tests.py
+-rw-rw-rw-   0        0        0      548 2023-06-12 10:03:16.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/urls.py
+-rw-rw-rw-   0        0        0      108 2023-06-12 10:02:19.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/views.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:44.881383 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility.egg-info/
+-rw-rw-rw-   0        0        0      973 2023-06-13 09:26:44.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1124 2023-06-13 09:26:44.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:26:44.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-13 09:26:44.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-06-13 09:26:44.000000 wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:44.898182 wagtail-all-in-one-accessibility-1.2/wagtail_package/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.2/wagtail_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:26:44.902146 wagtail-all-in-one-accessibility-1.2/wagtail_package/settings/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.2/wagtail_package/settings/__init__.py
+-rw-rw-rw-   0        0        0     4791 2023-06-12 12:18:51.000000 wagtail-all-in-one-accessibility-1.2/wagtail_package/settings/base.py
+-rw-rw-rw-   0        0        0      478 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.2/wagtail_package/settings/dev.py
+-rw-rw-rw-   0        0        0      103 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.2/wagtail_package/settings/production.py
+-rw-rw-rw-   0        0        0     1447 2023-06-12 10:07:02.000000 wagtail-all-in-one-accessibility-1.2/wagtail_package/urls.py
+-rw-rw-rw-   0        0        0      427 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.2/wagtail_package/wsgi.py
```

### Comparing `wagtail-all-in-one-accessibility-1.1/PKG-INFO` & `wagtail-all-in-one-accessibility-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-all-in-one-accessibility
-Version: 1.1
+Version: 1.2
 Summary: All in One Accessibility that helps organizations enhance the accessibility and usability of their website
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: developer3@skynettechnologies.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -14,9 +14,8 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
-
-# All in One Accessibility
+Description-Content-Type: file: Readme.md
```

### Comparing `wagtail-all-in-one-accessibility-1.1/search/views.py` & `wagtail-all-in-one-accessibility-1.2/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.1/setup.cfg` & `wagtail-all-in-one-accessibility-1.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 2d61 6c6c 2d69   = wagtail-all-i
 00000020: 6e2d 6f6e 652d 6163 6365 7373 6962 696c  n-one-accessibil
 00000030: 6974 790d 0a76 6572 7369 6f6e 203d 2031  ity..version = 1
-00000040: 2e31 0d0a 6465 7363 7269 7074 696f 6e20  .1..description 
+00000040: 2e32 0d0a 6465 7363 7269 7074 696f 6e20  .2..description 
 00000050: 3d20 416c 6c20 696e 204f 6e65 2041 6363  = All in One Acc
 00000060: 6573 7369 6269 6c69 7479 2074 6861 7420  essibility that 
 00000070: 6865 6c70 7320 6f72 6761 6e69 7a61 7469  helps organizati
 00000080: 6f6e 7320 656e 6861 6e63 6520 7468 6520  ons enhance the 
 00000090: 6163 6365 7373 6962 696c 6974 7920 616e  accessibility an
 000000a0: 6420 7573 6162 696c 6974 7920 6f66 2074  d usability of t
 000000b0: 6865 6972 2077 6562 7369 7465 0d0a 6c6f  heir website..lo
-000000c0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
-000000d0: 2066 696c 653a 2052 6561 646d 652e 6d64   file: Readme.md
-000000e0: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-000000f0: 7777 772e 736b 796e 6574 7465 6368 6e6f  www.skynettechno
-00000100: 6c6f 6769 6573 2e63 6f6d 0d0a 6175 7468  logies.com..auth
-00000110: 6f72 203d 2053 6b79 6e65 7420 5465 6368  or = Skynet Tech
-00000120: 6e6f 6c6f 6769 6573 2055 5341 204c 4c43  nologies USA LLC
-00000130: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000140: 2064 6576 656c 6f70 6572 3340 736b 796e   developer3@skyn
-00000150: 6574 7465 6368 6e6f 6c6f 6769 6573 2e63  ettechnologies.c
-00000160: 6f6d 0d0a 636c 6173 7369 6669 6572 7320  om..classifiers 
-00000170: 3d20 0d0a 0945 6e76 6972 6f6e 6d65 6e74  = ...Environment
-00000180: 203a 3a20 5765 6220 456e 7669 726f 6e6d   :: Web Environm
-00000190: 656e 740d 0a09 4672 616d 6577 6f72 6b20  ent...Framework 
-000001a0: 3a3a 2044 6a61 6e67 6f0d 0a09 496e 7465  :: Django...Inte
-000001b0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-000001c0: 2044 6576 656c 6f70 6572 730d 0a09 4c69   Developers...Li
-000001d0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000001e0: 726f 7665 6420 3a3a 2042 5344 204c 6963  roved :: BSD Lic
-000001f0: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
-00000200: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000210: 6465 7065 6e64 656e 740d 0a09 5072 6f67  dependent...Prog
-00000220: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000230: 203a 3a20 5079 7468 6f6e 0d0a 0950 726f   :: Python...Pro
-00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000250: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000260: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000270: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000280: 6e20 3a3a 2033 203a 3a20 4f6e 6c79 0d0a  n :: 3 :: Only..
-00000290: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002b0: 3a3a 2033 2e38 0d0a 0950 726f 6772 616d  :: 3.8...Program
-000002c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002d0: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
-000002e0: 0954 6f70 6963 203a 3a20 496e 7465 726e  .Topic :: Intern
-000002f0: 6574 203a 3a20 5757 572f 4854 5450 0d0a  et :: WWW/HTTP..
-00000300: 0954 6f70 6963 203a 3a20 496e 7465 726e  .Topic :: Intern
-00000310: 6574 203a 3a20 5757 572f 4854 5450 203a  et :: WWW/HTTP :
-00000320: 3a20 4479 6e61 6d69 6320 436f 6e74 656e  : Dynamic Conten
-00000330: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000340: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-00000350: 6461 7461 203d 2074 7275 650d 0a70 6163  data = true..pac
-00000360: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
-00000370: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-00000380: 203e 3d33 2e38 0d0a 696e 7374 616c 6c5f   >=3.8..install_
-00000390: 7265 7175 6972 6573 203d 200d 0a09 7761  requires = ...wa
-000003a0: 6774 6169 6c3e 3d35 2e30 2c3c 352e 310d  gtail>=5.0,<5.1.
-000003b0: 0a09 446a 616e 676f 3e3d 342e 322c 3c34  ..Django>=4.2,<4
-000003c0: 2e33 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  .3....[egg_info]
-000003d0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000003e0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000000c0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+000000d0: 6f6e 7465 6e74 5f74 7970 6520 3d20 6669  ontent_type = fi
+000000e0: 6c65 3a20 5265 6164 6d65 2e6d 640d 0a75  le: Readme.md..u
+000000f0: 726c 203d 2068 7474 7073 3a2f 2f77 7777  rl = https://www
+00000100: 2e73 6b79 6e65 7474 6563 686e 6f6c 6f67  .skynettechnolog
+00000110: 6965 732e 636f 6d0d 0a61 7574 686f 7220  ies.com..author 
+00000120: 3d20 536b 796e 6574 2054 6563 686e 6f6c  = Skynet Technol
+00000130: 6f67 6965 7320 5553 4120 4c4c 430d 0a61  ogies USA LLC..a
+00000140: 7574 686f 725f 656d 6169 6c20 3d20 6465  uthor_email = de
+00000150: 7665 6c6f 7065 7233 4073 6b79 6e65 7474  veloper3@skynett
+00000160: 6563 686e 6f6c 6f67 6965 732e 636f 6d0d  echnologies.com.
+00000170: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+00000180: 0a09 456e 7669 726f 6e6d 656e 7420 3a3a  ..Environment ::
+00000190: 2057 6562 2045 6e76 6972 6f6e 6d65 6e74   Web Environment
+000001a0: 0d0a 0946 7261 6d65 776f 726b 203a 3a20  ...Framework :: 
+000001b0: 446a 616e 676f 0d0a 0949 6e74 656e 6465  Django...Intende
+000001c0: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+000001d0: 7665 6c6f 7065 7273 0d0a 094c 6963 656e  velopers...Licen
+000001e0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000001f0: 6564 203a 3a20 4253 4420 4c69 6365 6e73  ed :: BSD Licens
+00000200: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+00000210: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000220: 656e 6465 6e74 0d0a 0950 726f 6772 616d  endent...Program
+00000230: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000240: 2050 7974 686f 6e0d 0a09 5072 6f67 7261   Python...Progra
+00000250: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000260: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
+00000270: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000280: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000290: 3a20 3320 3a3a 204f 6e6c 790d 0a09 5072  : 3 :: Only...Pr
+000002a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000002b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002c0: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
+000002d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002e0: 7468 6f6e 203a 3a20 332e 390d 0a09 546f  thon :: 3.9...To
+000002f0: 7069 6320 3a3a 2049 6e74 6572 6e65 7420  pic :: Internet 
+00000300: 3a3a 2057 5757 2f48 5454 500d 0a09 546f  :: WWW/HTTP...To
+00000310: 7069 6320 3a3a 2049 6e74 6572 6e65 7420  pic :: Internet 
+00000320: 3a3a 2057 5757 2f48 5454 5020 3a3a 2044  :: WWW/HTTP :: D
+00000330: 796e 616d 6963 2043 6f6e 7465 6e74 0d0a  ynamic Content..
+00000340: 0d0a 5b6f 7074 696f 6e73 5d0d 0a69 6e63  ..[options]..inc
+00000350: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+00000360: 6120 3d20 7472 7565 0d0a 7061 636b 6167  a = true..packag
+00000370: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+00000380: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000390: 332e 380d 0a69 6e73 7461 6c6c 5f72 6571  3.8..install_req
+000003a0: 7569 7265 7320 3d20 0d0a 0977 6167 7461  uires = ...wagta
+000003b0: 696c 3e3d 352e 302c 3c35 2e31 0d0a 0944  il>=5.0,<5.1...D
+000003c0: 6a61 6e67 6f3e 3d34 2e32 2c3c 342e 330d  jango>=4.2,<4.3.
+000003d0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+000003e0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000003f0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/admin.py` & `wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/admin.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/context_processors.py` & `wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/context_processors.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/migrations/0001_initial.py` & `wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/migrations/0002_alter_wagtail_all_in_one_accessibility_aioa_license_key.py` & `wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/migrations/0002_alter_wagtail_all_in_one_accessibility_aioa_license_key.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/models.py` & `wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility/urls.py` & `wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility.egg-info/PKG-INFO` & `wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-all-in-one-accessibility
-Version: 1.1
+Version: 1.2
 Summary: All in One Accessibility that helps organizations enhance the accessibility and usability of their website
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: developer3@skynettechnologies.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -14,9 +14,8 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
-
-# All in One Accessibility
+Description-Content-Type: file: Readme.md
```

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_all_in_one_accessibility.egg-info/SOURCES.txt` & `wagtail-all-in-one-accessibility-1.2/wagtail_all_in_one_accessibility.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-Readme.md
 setup.cfg
 setup.py
 search/__init__.py
 search/views.py
 wagtail_all_in_one_accessibility/__init__.py
 wagtail_all_in_one_accessibility/admin.py
 wagtail_all_in_one_accessibility/apps.py
```

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_package/settings/base.py` & `wagtail-all-in-one-accessibility-1.2/wagtail_package/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.1/wagtail_package/urls.py` & `wagtail-all-in-one-accessibility-1.2/wagtail_package/urls.py`

 * *Files identical despite different names*

