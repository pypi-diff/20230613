# Comparing `tmp/honkairail-1.0.1.tar.gz` & `tmp/honkairail-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honkairail-1.0.1.tar", max compression
+gzip compressed data, was "honkairail-1.0.2.tar", max compression
```

## Comparing `honkairail-1.0.1.tar` & `honkairail-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0        0 2023-06-05 03:59:10.580471 honkairail-1.0.1/honkairail/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 04:03:31.753289 honkairail-1.0.1/honkairail/src/__init__.py
--rw-r--r--   0        0        0      148 2023-06-05 09:07:32.687441 honkairail-1.0.1/honkairail/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-06-05 03:58:24.588036 honkairail-1.0.1/honkairail/src/tools/__init__.py
--rw-r--r--   0        0        0      154 2023-06-05 09:07:32.690434 honkairail-1.0.1/honkairail/src/tools/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2867 2023-06-09 11:04:04.021741 honkairail-1.0.1/honkairail/src/tools/__pycache__/api.cpython-310.pyc
--rw-r--r--   0        0        0    12087 2023-06-09 11:33:55.802274 honkairail-1.0.1/honkairail/src/tools/__pycache__/modal.cpython-310.pyc
--rw-r--r--   0        0        0     1310 2023-06-09 11:18:15.642417 honkairail-1.0.1/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc
--rw-r--r--   0        0        0     2950 2023-06-09 11:04:00.928622 honkairail-1.0.1/honkairail/src/tools/api.py
--rw-r--r--   0        0        0    11426 2023-06-09 11:33:52.556840 honkairail-1.0.1/honkairail/src/tools/modal.py
--rw-r--r--   0        0        0     1127 2023-06-09 11:14:40.320720 honkairail-1.0.1/honkairail/src/tools/utilities.py
--rw-r--r--   0        0        0     1010 2023-06-09 11:33:04.349430 honkairail-1.0.1/honkairail/starrailapi.py
--rw-r--r--   0        0        0      489 2023-06-10 09:39:23.432897 honkairail-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3892 2023-06-10 09:41:05.266404 honkairail-1.0.1/README.md
--rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 honkairail-1.0.1/setup.py
--rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 honkairail-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 03:59:10.580471 honkairail-1.0.2/honkairail/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:03:31.753289 honkairail-1.0.2/honkairail/src/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-05 09:07:32.687441 honkairail-1.0.2/honkairail/src/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-06-05 03:58:24.588036 honkairail-1.0.2/honkairail/src/tools/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-05 09:07:32.690434 honkairail-1.0.2/honkairail/src/tools/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2869 2023-06-13 09:02:25.940990 honkairail-1.0.2/honkairail/src/tools/__pycache__/api.cpython-310.pyc
+-rw-r--r--   0        0        0    12087 2023-06-09 11:33:55.802274 honkairail-1.0.2/honkairail/src/tools/__pycache__/modal.cpython-310.pyc
+-rw-r--r--   0        0        0     5919 2023-06-13 09:00:08.334290 honkairail-1.0.2/honkairail/src/tools/__pycache__/modalV1.cpython-310.pyc
+-rw-r--r--   0        0        0     7344 2023-06-13 09:03:44.338257 honkairail-1.0.2/honkairail/src/tools/__pycache__/modalV2.cpython-310.pyc
+-rw-r--r--   0        0        0     1310 2023-06-09 11:18:15.642417 honkairail-1.0.2/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc
+-rw-r--r--   0        0        0     2966 2023-06-13 09:01:56.381804 honkairail-1.0.2/honkairail/src/tools/api.py
+-rw-r--r--   0        0        0     4982 2023-06-13 08:54:13.093344 honkairail-1.0.2/honkairail/src/tools/modalV1.py
+-rw-r--r--   0        0        0     7043 2023-06-13 09:03:41.075449 honkairail-1.0.2/honkairail/src/tools/modalV2.py
+-rw-r--r--   0        0        0     1127 2023-06-09 11:14:40.320720 honkairail-1.0.2/honkairail/src/tools/utilities.py
+-rw-r--r--   0        0        0     1014 2023-06-13 09:00:38.215106 honkairail-1.0.2/honkairail/starrailapi.py
+-rw-r--r--   0        0        0      489 2023-06-13 09:33:23.107993 honkairail-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3892 2023-06-10 09:41:05.266404 honkairail-1.0.2/README.md
+-rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 honkairail-1.0.2/setup.py
+-rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 honkairail-1.0.2/PKG-INFO
```

### Comparing `honkairail-1.0.1/honkairail/src/tools/__pycache__/api.cpython-310.pyc` & `honkairail-1.0.2/honkairail/src/tools/__pycache__/api.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 11:04:00 2023 UTC, .py size: 2950 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-00000000: 6f0d 0d0a 0000 0000 2007 8364 860b 0000  o....... ..d....
+00000000: 6f0d 0d0a 0000 0000 8430 8864 960b 0000  o........0.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000e 0000 0040 0000 0073 9c00 0000 6400  .....@...s....d.
+00000020: 000e 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 6d05 5a05 6d06 5a06 0100 6402 6404 6c07  m.Z.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6405 6406 6407 6408 6409  m.Z...d.d.d.d.d.
-00000070: 640a 640b 640c 640d 640e 640f 6410 6411  d.d.d.d.d.d.d.d.
-00000080: 6412 9c0d 5a09 6413 5a0a 6414 5a0b 6415  d...Z.d.Z.d.Z.d.
-00000090: 5a0c 6416 5a0d 6417 6418 8400 5a0e 6419  Z.d.Z.d.d...Z.d.
-000000a0: 641a 8400 5a0f 641b 641c 8400 5a10 641d  d...Z.d.d...Z.d.
-000000b0: 641e 8400 5a11 641f 6420 8400 5a12 6421  d...Z.d.d ..Z.d!
-000000c0: 6422 8400 5a13 6401 5300 2923 e900 0000  d"..Z.d.S.)#....
-000000d0: 004e e901 0000 0029 03da 0f53 7461 7252  .N.....)...StarR
-000000e0: 6169 6c41 7069 4461 7461 da0a 506c 6179  ailApiData..Play
-000000f0: 6572 496e 666f da11 5374 6172 5261 696c  erInfo..StarRail
-00000100: 4170 6944 6174 6156 3229 01da 0975 7469  ApiDataV2)...uti
-00000110: 6c69 7469 6573 da03 6368 74da 0263 6eda  lities..cht..cn.
-00000120: 0264 65da 0265 6eda 0265 73da 0266 72da  .de..en..es..fr.
-00000130: 0269 64da 026a 70da 026b 72da 0270 74da  .id..jp..kr..pt.
-00000140: 0272 75da 0274 68da 0276 6929 0d72 0700  .ru..th..vi).r..
-00000150: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000160: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000170: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000180: 1100 0000 7212 0000 0072 1300 0000 7a41  ....r....r....zA
-00000190: 6874 7470 733a 2f2f 6170 692e 6d69 686f  https://api.miho
-000001a0: 6d6f 2e6d 652f 7372 5f69 6e66 6f5f 7061  mo.me/sr_info_pa
-000001b0: 7273 6564 2f7b 7569 647d 3f6c 616e 673d  rsed/{uid}?lang=
-000001c0: 7b6c 616e 677d 2676 6572 7369 6f6e 3d76  {lang}&version=v
-000001d0: 317a 3668 7474 7073 3a2f 2f61 7069 2e6d  1z6https://api.m
-000001e0: 6968 6f6d 6f2e 6d65 2f73 725f 696e 666f  ihomo.me/sr_info
-000001f0: 5f70 6172 7365 642f 7b75 6964 7d3f 6c61  _parsed/{uid}?la
-00000200: 6e67 3d7b 6c61 6e67 7d7a 3a68 7474 7073  ng={lang}z:https
-00000210: 3a2f 2f61 7069 2e6d 6968 6f6d 6f2e 6d65  ://api.mihomo.me
-00000220: 2f73 725f 696e 666f 2f7b 7569 647d 3f6c  /sr_info/{uid}?l
-00000230: 616e 673d 7b6c 616e 677d 2676 6572 7369  ang={lang}&versi
-00000240: 6f6e 3d76 317a 8168 7474 7073 3a2f 2f6d  on=v1z.https://m
-00000250: 616e 612e 7769 6b69 2f73 7461 7272 6169  ana.wiki/starrai
-00000260: 6c2f 636f 6c6c 6563 7469 6f6e 732f 6c69  l/collections/li
-00000270: 6768 7443 6f6e 6573 2f7b 6964 7d3f 5f64  ghtCones/{id}?_d
-00000280: 6174 613d 5f63 7573 746f 6d25 3246 726f  ata=_custom%2Fro
-00000290: 7574 6573 2532 4625 3234 7369 7465 4964  utes%2F%24siteId
-000002a0: 2e63 6f6c 6c65 6374 696f 6e73 2532 4225  .collections%2B%
-000002b0: 3246 6c69 6768 7443 6f6e 6573 5f2e 2532  2FlightCones_.%2
-000002c0: 3465 6e74 7279 4964 6301 0000 0000 0000  4entryIdc.......
-000002d0: 0000 0000 0004 0000 000a 0000 00c3 0000  ................
-000002e0: 0073 bc00 0000 8101 7400 a001 a100 3400  .s......t.....4.
-000002f0: 4900 6400 4800 9a48 7d01 7c01 a002 7c00  I.d.H..H}.|...|.
-00000300: a101 3400 4900 6400 4800 9a28 7d02 7c02  ..4.I.d.H..(}.|.
-00000310: a003 a100 4900 6400 4800 7d03 6401 7c03  ....I.d.H.}.d.|.
-00000320: 7600 7225 7404 7c03 6401 1900 8301 8201  v.r%t.|.d.......
-00000330: 7c03 5700 0200 6400 0400 0400 8303 4900  |.W...d.......I.
-00000340: 6400 4800 0100 5700 0200 6400 0400 0400  d.H...W...d.....
-00000350: 8303 4900 6400 4800 0100 5300 3100 4900  ..I.d.H...S.1.I.
-00000360: 6400 4800 7341 7701 0100 0100 0100 5900  d.H.sAw.......Y.
-00000370: 0100 5700 6400 0400 0400 8303 4900 6400  ..W.d.......I.d.
-00000380: 4800 0100 6400 5300 3100 4900 6400 4800  H...d.S.1.I.d.H.
-00000390: 7357 7701 0100 0100 0100 5900 0100 6400  sWw.......Y...d.
-000003a0: 5300 2902 4e5a 0664 6574 6169 6c29 05da  S.).NZ.detail)..
-000003b0: 0761 696f 6874 7470 5a0d 436c 6965 6e74  .aiohttpZ.Client
-000003c0: 5365 7373 696f 6eda 0367 6574 da04 6a73  Session..get..js
-000003d0: 6f6e da09 5479 7065 4572 726f 7229 04da  on..TypeError)..
-000003e0: 0375 726c da07 7365 7373 696f 6eda 0872  .url..session..r
-000003f0: 6573 706f 6e73 65da 0464 6174 61a9 0072  esponse..data..r
-00000400: 1c00 0000 fa37 433a 5c55 7365 7273 5c44  .....7C:\Users\D
-00000410: 6172 736f 585c 4465 736b 746f 705c 7265  arsoX\Desktop\re
-00000420: 735c 686f 6e6b 6169 7261 696c 5c73 7263  s\honkairail\src
-00000430: 5c74 6f6f 6c73 5c61 7069 2e70 79da 0a66  \tools\api.py..f
-00000440: 6574 6368 5f64 6174 611c 0000 0073 1600  etch_data....s..
-00000450: 0000 0280 1201 1401 0e01 0801 0c01 0201  ................
-00000460: 14fc 16ff 1801 2eff 721e 0000 0063 0300  ........r....c..
-00000470: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00000480: 0000 c300 0000 7346 0000 0081 0174 00a0  ......sF.....t..
-00000490: 017c 01a0 02a1 0064 01a1 027d 017c 0264  .|.....d...}.|.d
-000004a0: 026b 0272 1574 036a 047c 007c 0164 038d  .k.r.t.j.|.|.d..
-000004b0: 027d 036e 0774 056a 047c 007c 0164 038d  .}.n.t.j.|.|.d..
-000004c0: 027d 0374 067c 0383 0149 0064 0048 0053  .}.t.|...I.d.H.S
-000004d0: 0029 044e 720a 0000 0072 0200 0000 a902  .).Nr....r......
-000004e0: da03 7569 64da 046c 616e 6729 07da 1353  ..uid..lang)...S
-000004f0: 5550 504f 5254 4544 5f4c 414e 4755 4147  UPPORTED_LANGUAG
-00000500: 4553 7215 0000 00da 056c 6f77 6572 da08  ESr......lower..
-00000510: 4150 495f 4c49 4e4b da06 666f 726d 6174  API_LINK..format
-00000520: da0b 4150 495f 4c49 4e4b 5f56 3272 1e00  ..API_LINK_V2r..
-00000530: 0000 2904 7220 0000 0072 2100 0000 da01  ..).r ...r!.....
-00000540: 7672 1800 0000 721c 0000 0072 1c00 0000  vr....r....r....
-00000550: 721d 0000 00da 0d67 6574 5f75 7365 725f  r......get_user_
-00000560: 6461 7461 2400 0000 730c 0000 0002 8010  data$...s.......
-00000570: 0108 0110 010e 020e 0172 2800 0000 6302  .........r(...c.
-00000580: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000590: 0000 00c3 0000 0073 2e00 0000 8101 7400  .......s......t.
-000005a0: a001 7c01 a002 a100 6401 a102 7d01 7403  ..|.....d...}.t.
-000005b0: 6a04 7c00 7c01 6402 8d02 7d02 7405 7c02  j.|.|.d...}.t.|.
-000005c0: 8301 4900 6400 4800 5300 2903 4e72 0a00  ..I.d.H.S.).Nr..
-000005d0: 0000 721f 0000 0029 0672 2200 0000 7215  ..r....).r"...r.
-000005e0: 0000 0072 2300 0000 da0d 4655 4c4c 5f41  ...r#.....FULL_A
-000005f0: 5049 5f4c 494e 4b72 2500 0000 721e 0000  PI_LINKr%...r...
-00000600: 0029 0372 2000 0000 7221 0000 0072 1800  .).r ...r!...r..
-00000610: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000620: 00da 1267 6574 5f66 756c 6c5f 7573 6572  ...get_full_user
-00000630: 5f64 6174 612c 0000 0073 0800 0000 0280  _data,...s......
-00000640: 1001 0e01 0e01 722a 0000 0063 0100 0000  ......r*...c....
-00000650: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000660: c300 0000 731c 0000 0081 0174 006a 017c  ....s......t.j.|
-00000670: 0064 018d 017d 0174 027c 0183 0149 0064  .d...}.t.|...I.d
-00000680: 0048 0053 0029 024e 2901 720d 0000 0029  .H.S.).N).r....)
-00000690: 03da 104c 4947 4854 5f43 4f4e 4553 5f4c  ...LIGHT_CONES_L
-000006a0: 494e 4b72 2500 0000 721e 0000 0029 0272  INKr%...r....).r
-000006b0: 0d00 0000 7218 0000 0072 1c00 0000 721c  ....r....r....r.
-000006c0: 0000 0072 1d00 0000 da14 6765 745f 6c69  ...r......get_li
-000006d0: 6768 745f 636f 6e65 735f 6461 7461 3100  ght_cones_data1.
-000006e0: 0000 7306 0000 0002 800c 010e 0172 2c00  ..s..........r,.
-000006f0: 0000 6303 0000 0000 0000 0000 0000 0004  ..c.............
-00000700: 0000 0004 0000 00c3 0000 0073 4400 0000  ...........sD...
-00000710: 8101 7400 7c01 7c00 7c02 8303 4900 6400  ..t.|.|.|...I.d.
-00000720: 4800 7d03 7c02 6401 6b02 7218 7401 7c03  H.}.|.d.k.r.t.|.
-00000730: 6402 1900 7c03 6403 1900 6404 8d02 5300  d...|.d...d...S.
-00000740: 7402 7c03 6402 1900 7c03 6403 1900 6404  t.|.d...|.d...d.
-00000750: 8d02 5300 2905 4e72 0200 0000 da06 706c  ..S.).Nr......pl
-00000760: 6179 6572 da0a 6368 6172 6163 7465 7273  ayer..characters
-00000770: a902 722d 0000 0072 2e00 0000 2903 7228  ..r-...r....).r(
-00000780: 0000 0072 0300 0000 7205 0000 0029 0472  ...r....r....).r
-00000790: 2100 0000 7220 0000 0072 2700 0000 721b  !...r ...r'...r.
-000007a0: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
-000007b0: 0000 da08 6765 745f 6461 7461 3500 0000  ....get_data5...
-000007c0: 730a 0000 0002 8012 0108 0114 0114 0172  s..............r
-000007d0: 3000 0000 6303 0000 0000 0000 0000 0000  0...c...........
-000007e0: 0007 0000 0004 0000 00c3 0000 0073 fe00  .............s..
-000007f0: 0000 8101 7400 7c01 7c00 7c02 8303 4900  ....t.|.|.|...I.
-00000800: 6400 4800 7d03 7401 7c01 7c00 8302 4900  d.H.}.t.|.|...I.
-00000810: 6400 4800 7d04 7c03 6401 1900 4400 5d0c  d.H.}.|.d...D.].
-00000820: 7d05 7c05 6402 1900 6900 6b02 7222 6400  }.|.d...i.k.r"d.
-00000830: 7c05 6402 3c00 7116 7c02 6403 6b02 7275  |.d.<.q.|.d.k.ru
-00000840: 7c04 6404 1900 7d06 7c06 6405 1900 7c03  |.d...}.|.d...|.
-00000850: 6406 1900 6407 3c00 7c06 6408 1900 7c03  d...d.<.|.d...|.
-00000860: 6406 1900 6409 3c00 640a 7c03 6406 1900  d...d.<.d.|.d...
-00000870: 640b 3c00 7c06 640c 1900 640d 1900 640e  d.<.|.d...d...d.
-00000880: 1900 7c03 6406 1900 640f 3c00 7c06 640c  ..|.d...d.<.|.d.
-00000890: 1900 6410 1900 7c03 6406 1900 6402 3c00  ..d...|.d...d.<.
-000008a0: 7c06 640c 1900 6411 1900 7c03 6406 1900  |.d...d...|.d...
-000008b0: 6401 3c00 7c06 640c 1900 6412 1900 7c03  d.<.|.d...d...|.
-000008c0: 6406 1900 6413 3c00 7402 7c03 6406 1900  d...d.<.t.|.d...
-000008d0: 7c03 6401 1900 6414 8d02 5300 7403 7c03  |.d...d...S.t.|.
-000008e0: 6406 1900 7c03 6401 1900 6414 8d02 5300  d...|.d...d...S.
-000008f0: 2915 4e72 2e00 0000 da0a 6c69 6768 745f  ).Nr......light_
-00000900: 636f 6e65 7202 0000 005a 0a64 6574 6169  coner....Z.detai
-00000910: 6c49 6e66 6f5a 0b66 7269 656e 6443 6f75  lInfoZ.friendCou
-00000920: 6e74 722d 0000 005a 0766 7269 656e 6473  ntr-...Z.friends
-00000930: 5a0a 776f 726c 644c 6576 656c 5a0a 776f  Z.worldLevelZ.wo
-00000940: 726c 646c 6576 656c da01 305a 0862 6972  rldlevel..0Z.bir
-00000950: 7468 6461 795a 0a72 6563 6f72 6449 6e66  thdayZ.recordInf
-00000960: 6f5a 0d63 6861 6c6c 656e 6765 496e 666f  oZ.challengeInfo
-00000970: 5a10 7363 6865 6475 6c65 4d61 784c 6576  Z.scheduleMaxLev
-00000980: 656c 5a12 7061 7373 5f61 7265 615f 7072  elZ.pass_area_pr
-00000990: 6f67 7265 7373 5a0e 6571 7569 706d 656e  ogressZ.equipmen
-000009a0: 7443 6f75 6e74 5a0b 6176 6174 6172 436f  tCountZ.avatarCo
-000009b0: 756e 745a 1061 6368 6965 7665 6d65 6e74  untZ.achievement
-000009c0: 436f 756e 745a 0b61 6368 6965 7665 6d65  CountZ.achieveme
-000009d0: 6e74 722f 0000 0029 0472 2800 0000 722a  ntr/...).r(...r*
-000009e0: 0000 0072 0300 0000 7205 0000 0029 0772  ...r....r....).r
-000009f0: 2100 0000 7220 0000 0072 2700 0000 721b  !...r ...r'...r.
-00000a00: 0000 005a 0770 726f 6669 6c65 da03 6b65  ...Z.profile..ke
-00000a10: 795a 0b70 6c61 7965 725f 696e 666f 721c  yZ.player_infor.
-00000a20: 0000 0072 1c00 0000 721d 0000 00da 0867  ...r....r......g
-00000a30: 6574 5f66 756c 6c3b 0000 0073 2400 0000  et_full;...s$...
-00000a40: 0280 1201 1001 0c01 0c01 0801 0280 0801  ................
-00000a50: 0801 1001 1001 0c01 1801 1401 1401 1401  ................
-00000a60: 1402 1401 7234 0000 0029 1472 1400 0000  ....r4...).r....
-00000a70: da07 6173 796e 6369 6f72 1600 0000 da05  ..asyncior......
-00000a80: 6d6f 6461 6c72 0300 0000 7204 0000 0072  modalr....r....r
-00000a90: 0500 0000 da00 7206 0000 0072 2200 0000  ......r....r"...
-00000aa0: 7224 0000 0072 2600 0000 7229 0000 0072  r$...r&...r)...r
-00000ab0: 2b00 0000 721e 0000 0072 2800 0000 722a  +...r....r(...r*
-00000ac0: 0000 0072 2c00 0000 7230 0000 0072 3400  ...r,...r0...r4.
-00000ad0: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-00000ae0: 0072 1d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000af0: 0100 0000 733a 0000 0008 0008 0108 0114  ....s:..........
-00000b00: 010c 0102 0302 0102 0102 0102 0102 0102  ................
-00000b10: 0102 0102 0102 0102 0102 0102 0106 f304  ................
-00000b20: 1004 0104 0104 0108 0208 0808 0808 0508  ................
-00000b30: 040c 06                                  ...
+00000050: 0100 6402 6404 6c05 6d06 5a06 0100 6402  ..d.d.l.m.Z...d.
+00000060: 6405 6c07 6d08 5a08 0100 6406 6407 6408  d.l.m.Z...d.d.d.
+00000070: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
+00000080: 6411 6412 6413 9c0d 5a09 6414 5a0a 6415  d.d.d...Z.d.Z.d.
+00000090: 5a0b 6416 5a0c 6417 5a0d 6418 6419 8400  Z.d.Z.d.Z.d.d...
+000000a0: 5a0e 641a 641b 8400 5a0f 641c 641d 8400  Z.d.d...Z.d.d...
+000000b0: 5a10 641e 641f 8400 5a11 6420 6421 8400  Z.d.d...Z.d d!..
+000000c0: 5a12 6422 6423 8400 5a13 6401 5300 2924  Z.d"d#..Z.d.S.)$
+000000d0: e900 0000 004e e901 0000 0029 01da 0f53  .....N.....)...S
+000000e0: 7461 7252 6169 6c41 7069 4461 7461 2901  tarRailApiData).
+000000f0: da11 5374 6172 5261 696c 4170 6944 6174  ..StarRailApiDat
+00000100: 6156 3229 01da 0975 7469 6c69 7469 6573  aV2)...utilities
+00000110: da03 6368 74da 0263 6eda 0264 65da 0265  ..cht..cn..de..e
+00000120: 6eda 0265 73da 0266 72da 0269 64da 026a  n..es..fr..id..j
+00000130: 70da 026b 72da 0270 74da 0272 75da 0274  p..kr..pt..ru..t
+00000140: 68da 0276 6929 0d72 0600 0000 7207 0000  h..vi).r....r...
+00000150: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000160: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000170: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+00000180: 0000 0072 1200 0000 7a41 6874 7470 733a  ...r....zAhttps:
+00000190: 2f2f 6170 692e 6d69 686f 6d6f 2e6d 652f  //api.mihomo.me/
+000001a0: 7372 5f69 6e66 6f5f 7061 7273 6564 2f7b  sr_info_parsed/{
+000001b0: 7569 647d 3f6c 616e 673d 7b6c 616e 677d  uid}?lang={lang}
+000001c0: 2676 6572 7369 6f6e 3d76 317a 3668 7474  &version=v1z6htt
+000001d0: 7073 3a2f 2f61 7069 2e6d 6968 6f6d 6f2e  ps://api.mihomo.
+000001e0: 6d65 2f73 725f 696e 666f 5f70 6172 7365  me/sr_info_parse
+000001f0: 642f 7b75 6964 7d3f 6c61 6e67 3d7b 6c61  d/{uid}?lang={la
+00000200: 6e67 7d7a 3a68 7474 7073 3a2f 2f61 7069  ng}z:https://api
+00000210: 2e6d 6968 6f6d 6f2e 6d65 2f73 725f 696e  .mihomo.me/sr_in
+00000220: 666f 2f7b 7569 647d 3f6c 616e 673d 7b6c  fo/{uid}?lang={l
+00000230: 616e 677d 2676 6572 7369 6f6e 3d76 317a  ang}&version=v1z
+00000240: 8168 7474 7073 3a2f 2f6d 616e 612e 7769  .https://mana.wi
+00000250: 6b69 2f73 7461 7272 6169 6c2f 636f 6c6c  ki/starrail/coll
+00000260: 6563 7469 6f6e 732f 6c69 6768 7443 6f6e  ections/lightCon
+00000270: 6573 2f7b 6964 7d3f 5f64 6174 613d 5f63  es/{id}?_data=_c
+00000280: 7573 746f 6d25 3246 726f 7574 6573 2532  ustom%2Froutes%2
+00000290: 4625 3234 7369 7465 4964 2e63 6f6c 6c65  F%24siteId.colle
+000002a0: 6374 696f 6e73 2532 4225 3246 6c69 6768  ctions%2B%2Fligh
+000002b0: 7443 6f6e 6573 5f2e 2532 3465 6e74 7279  tCones_.%24entry
+000002c0: 4964 6301 0000 0000 0000 0000 0000 0004  Idc.............
+000002d0: 0000 000a 0000 00c3 0000 0073 bc00 0000  ...........s....
+000002e0: 8101 7400 a001 a100 3400 4900 6400 4800  ..t.....4.I.d.H.
+000002f0: 9a48 7d01 7c01 a002 7c00 a101 3400 4900  .H}.|...|...4.I.
+00000300: 6400 4800 9a28 7d02 7c02 a003 a100 4900  d.H..(}.|.....I.
+00000310: 6400 4800 7d03 6401 7c03 7600 7225 7404  d.H.}.d.|.v.r%t.
+00000320: 7c03 6401 1900 8301 8201 7c03 5700 0200  |.d.......|.W...
+00000330: 6400 0400 0400 8303 4900 6400 4800 0100  d.......I.d.H...
+00000340: 5700 0200 6400 0400 0400 8303 4900 6400  W...d.......I.d.
+00000350: 4800 0100 5300 3100 4900 6400 4800 7341  H...S.1.I.d.H.sA
+00000360: 7701 0100 0100 0100 5900 0100 5700 6400  w.......Y...W.d.
+00000370: 0400 0400 8303 4900 6400 4800 0100 6400  ......I.d.H...d.
+00000380: 5300 3100 4900 6400 4800 7357 7701 0100  S.1.I.d.H.sWw...
+00000390: 0100 0100 5900 0100 6400 5300 2902 4e5a  ....Y...d.S.).NZ
+000003a0: 0664 6574 6169 6c29 05da 0761 696f 6874  .detail)...aioht
+000003b0: 7470 5a0d 436c 6965 6e74 5365 7373 696f  tpZ.ClientSessio
+000003c0: 6eda 0367 6574 da04 6a73 6f6e da09 5479  n..get..json..Ty
+000003d0: 7065 4572 726f 7229 04da 0375 726c da07  peError)...url..
+000003e0: 7365 7373 696f 6eda 0872 6573 706f 6e73  session..respons
+000003f0: 65da 0464 6174 61a9 0072 1b00 0000 fa37  e..data..r.....7
+00000400: 433a 5c55 7365 7273 5c44 6172 736f 585c  C:\Users\DarsoX\
+00000410: 4465 736b 746f 705c 7265 735c 686f 6e6b  Desktop\res\honk
+00000420: 6169 7261 696c 5c73 7263 5c74 6f6f 6c73  airail\src\tools
+00000430: 5c61 7069 2e70 79da 0a66 6574 6368 5f64  \api.py..fetch_d
+00000440: 6174 611d 0000 0073 1600 0000 0280 1201  ata....s........
+00000450: 1401 0e01 0801 0c01 0201 14fc 16ff 1801  ................
+00000460: 2eff 721d 0000 0063 0300 0000 0000 0000  ..r....c........
+00000470: 0000 0000 0400 0000 0400 0000 c300 0000  ................
+00000480: 7346 0000 0081 0174 00a0 017c 01a0 02a1  sF.....t...|....
+00000490: 0064 01a1 027d 017c 0264 026b 0272 1574  .d...}.|.d.k.r.t
+000004a0: 036a 047c 007c 0164 038d 027d 036e 0774  .j.|.|.d...}.n.t
+000004b0: 056a 047c 007c 0164 038d 027d 0374 067c  .j.|.|.d...}.t.|
+000004c0: 0383 0149 0064 0048 0053 0029 044e 7209  ...I.d.H.S.).Nr.
+000004d0: 0000 0072 0200 0000 a902 da03 7569 64da  ...r........uid.
+000004e0: 046c 616e 6729 07da 1353 5550 504f 5254  .lang)...SUPPORT
+000004f0: 4544 5f4c 414e 4755 4147 4553 7214 0000  ED_LANGUAGESr...
+00000500: 00da 056c 6f77 6572 da08 4150 495f 4c49  ...lower..API_LI
+00000510: 4e4b da06 666f 726d 6174 da0b 4150 495f  NK..format..API_
+00000520: 4c49 4e4b 5f56 3272 1d00 0000 2904 721f  LINK_V2r....).r.
+00000530: 0000 0072 2000 0000 da01 7672 1700 0000  ...r .....vr....
+00000540: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00000550: 0d67 6574 5f75 7365 725f 6461 7461 2500  .get_user_data%.
+00000560: 0000 730c 0000 0002 8010 0108 0110 010e  ..s.............
+00000570: 020e 0172 2700 0000 6302 0000 0000 0000  ...r'...c.......
+00000580: 0000 0000 0003 0000 0004 0000 00c3 0000  ................
+00000590: 0073 2e00 0000 8101 7400 a001 7c01 a002  .s......t...|...
+000005a0: a100 6401 a102 7d01 7403 6a04 7c00 7c01  ..d...}.t.j.|.|.
+000005b0: 6402 8d02 7d02 7405 7c02 8301 4900 6400  d...}.t.|...I.d.
+000005c0: 4800 5300 2903 4e72 0900 0000 721e 0000  H.S.).Nr....r...
+000005d0: 0029 0672 2100 0000 7214 0000 0072 2200  .).r!...r....r".
+000005e0: 0000 da0d 4655 4c4c 5f41 5049 5f4c 494e  ....FULL_API_LIN
+000005f0: 4b72 2400 0000 721d 0000 0029 0372 1f00  Kr$...r....).r..
+00000600: 0000 7220 0000 0072 1700 0000 721b 0000  ..r ...r....r...
+00000610: 0072 1b00 0000 721c 0000 00da 1267 6574  .r....r......get
+00000620: 5f66 756c 6c5f 7573 6572 5f64 6174 612d  _full_user_data-
+00000630: 0000 0073 0800 0000 0280 1001 0e01 0e01  ...s............
+00000640: 7229 0000 0063 0100 0000 0000 0000 0000  r)...c..........
+00000650: 0000 0200 0000 0300 0000 c300 0000 731c  ..............s.
+00000660: 0000 0081 0174 006a 017c 0064 018d 017d  .....t.j.|.d...}
+00000670: 0174 027c 0183 0149 0064 0048 0053 0029  .t.|...I.d.H.S.)
+00000680: 024e 2901 720c 0000 0029 03da 104c 4947  .N).r....)...LIG
+00000690: 4854 5f43 4f4e 4553 5f4c 494e 4b72 2400  HT_CONES_LINKr$.
+000006a0: 0000 721d 0000 0029 0272 0c00 0000 7217  ..r....).r....r.
+000006b0: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
+000006c0: 0000 da14 6765 745f 6c69 6768 745f 636f  ....get_light_co
+000006d0: 6e65 735f 6461 7461 3200 0000 7306 0000  nes_data2...s...
+000006e0: 0002 800c 010e 0172 2b00 0000 6303 0000  .......r+...c...
+000006f0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00000700: 00c3 0000 0073 4400 0000 8101 7400 7c01  .....sD.....t.|.
+00000710: 7c00 7c02 8303 4900 6400 4800 7d03 7c02  |.|...I.d.H.}.|.
+00000720: 6401 6b02 7218 7401 7c03 6402 1900 7c03  d.k.r.t.|.d...|.
+00000730: 6403 1900 6404 8d02 5300 7402 7c03 6402  d...d...S.t.|.d.
+00000740: 1900 7c03 6403 1900 6404 8d02 5300 2905  ..|.d...d...S.).
+00000750: 4e72 0200 0000 da06 706c 6179 6572 da0a  Nr......player..
+00000760: 6368 6172 6163 7465 7273 a902 722c 0000  characters..r,..
+00000770: 0072 2d00 0000 2903 7227 0000 0072 0300  .r-...).r'...r..
+00000780: 0000 7204 0000 0029 0472 2000 0000 721f  ..r....).r ...r.
+00000790: 0000 0072 2600 0000 721a 0000 0072 1b00  ...r&...r....r..
+000007a0: 0000 721b 0000 0072 1c00 0000 da08 6765  ..r....r......ge
+000007b0: 745f 6461 7461 3600 0000 730a 0000 0002  t_data6...s.....
+000007c0: 8012 0108 0114 0114 0172 2f00 0000 6303  .........r/...c.
+000007d0: 0000 0000 0000 0000 0000 0007 0000 0004  ................
+000007e0: 0000 00c3 0000 0073 fe00 0000 8101 7400  .......s......t.
+000007f0: 7c01 7c00 7c02 8303 4900 6400 4800 7d03  |.|.|...I.d.H.}.
+00000800: 7c03 6401 1900 4400 5d0c 7d04 7c04 6402  |.d...D.].}.|.d.
+00000810: 1900 6900 6b02 721a 6400 7c04 6402 3c00  ..i.k.r.d.|.d.<.
+00000820: 710e 7c02 6403 6b02 7275 7401 7c01 7c00  q.|.d.k.rut.|.|.
+00000830: 8302 4900 6400 4800 7d05 7c05 6404 1900  ..I.d.H.}.|.d...
+00000840: 7d06 7c06 6405 1900 7c03 6406 1900 6407  }.|.d...|.d...d.
+00000850: 3c00 7c06 6408 1900 7c03 6406 1900 6409  <.|.d...|.d...d.
+00000860: 3c00 640a 7c03 6406 1900 640b 3c00 7c06  <.d.|.d...d.<.|.
+00000870: 640c 1900 640d 1900 640e 1900 7c03 6406  d...d...d...|.d.
+00000880: 1900 640f 3c00 7c06 640c 1900 6410 1900  ..d.<.|.d...d...
+00000890: 7c03 6406 1900 6402 3c00 7c06 640c 1900  |.d...d.<.|.d...
+000008a0: 6411 1900 7c03 6406 1900 6401 3c00 7c06  d...|.d...d.<.|.
+000008b0: 640c 1900 6412 1900 7c03 6406 1900 6413  d...d...|.d...d.
+000008c0: 3c00 7402 7c03 6406 1900 7c03 6401 1900  <.t.|.d...|.d...
+000008d0: 6414 8d02 5300 7403 7c03 6406 1900 7c03  d...S.t.|.d...|.
+000008e0: 6401 1900 6414 8d02 5300 2915 4e72 2d00  d...d...S.).Nr-.
+000008f0: 0000 da0a 6c69 6768 745f 636f 6e65 7202  ....light_coner.
+00000900: 0000 005a 0a64 6574 6169 6c49 6e66 6f5a  ...Z.detailInfoZ
+00000910: 0b66 7269 656e 6443 6f75 6e74 722c 0000  .friendCountr,..
+00000920: 005a 0766 7269 656e 6473 5a0a 776f 726c  .Z.friendsZ.worl
+00000930: 644c 6576 656c 5a0a 776f 726c 646c 6576  dLevelZ.worldlev
+00000940: 656c da01 305a 0862 6972 7468 6461 795a  el..0Z.birthdayZ
+00000950: 0a72 6563 6f72 6449 6e66 6f5a 0d63 6861  .recordInfoZ.cha
+00000960: 6c6c 656e 6765 496e 666f 5a10 7363 6865  llengeInfoZ.sche
+00000970: 6475 6c65 4d61 784c 6576 656c 5a12 7061  duleMaxLevelZ.pa
+00000980: 7373 5f61 7265 615f 7072 6f67 7265 7373  ss_area_progress
+00000990: 5a0e 6571 7569 706d 656e 7443 6f75 6e74  Z.equipmentCount
+000009a0: 5a0b 6176 6174 6172 436f 756e 745a 1061  Z.avatarCountZ.a
+000009b0: 6368 6965 7665 6d65 6e74 436f 756e 745a  chievementCountZ
+000009c0: 0b61 6368 6965 7665 6d65 6e74 722e 0000  .achievementr...
+000009d0: 0029 0472 2700 0000 7229 0000 0072 0300  .).r'...r)...r..
+000009e0: 0000 7204 0000 0029 0772 2000 0000 721f  ..r....).r ...r.
+000009f0: 0000 0072 2600 0000 721a 0000 00da 036b  ...r&...r......k
+00000a00: 6579 5a07 7072 6f66 696c 655a 0b70 6c61  eyZ.profileZ.pla
+00000a10: 7965 725f 696e 666f 721b 0000 0072 1b00  yer_infor....r..
+00000a20: 0000 721c 0000 00da 0867 6574 5f66 756c  ..r......get_ful
+00000a30: 6c3c 0000 0073 2400 0000 0280 1201 0c01  l<...s$.........
+00000a40: 0c01 0801 0280 0801 1001 0801 1001 1001  ................
+00000a50: 0c01 1801 1401 1401 1401 1402 1401 7233  ..............r3
+00000a60: 0000 0029 1472 1300 0000 da07 6173 796e  ...).r......asyn
+00000a70: 6369 6f72 1500 0000 da07 6d6f 6461 6c56  cior......modalV
+00000a80: 3172 0300 0000 5a07 6d6f 6461 6c56 3272  1r....Z.modalV2r
+00000a90: 0400 0000 da00 7205 0000 0072 2100 0000  ......r....r!...
+00000aa0: 7223 0000 0072 2500 0000 7228 0000 0072  r#...r%...r(...r
+00000ab0: 2a00 0000 721d 0000 0072 2700 0000 7229  *...r....r'...r)
+00000ac0: 0000 0072 2b00 0000 722f 0000 0072 3300  ...r+...r/...r3.
+00000ad0: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00000ae0: 0072 1c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000af0: 0100 0000 733c 0000 0008 0008 0108 010c  ....s<..........
+00000b00: 010c 010c 0102 0302 0102 0102 0102 0102  ................
+00000b10: 0102 0102 0102 0102 0102 0102 0102 0106  ................
+00000b20: f304 1004 0104 0104 0108 0208 0808 0808  ................
+00000b30: 0508 040c 06                             .....
```

### Comparing `honkairail-1.0.1/honkairail/src/tools/__pycache__/modal.cpython-310.pyc` & `honkairail-1.0.2/honkairail/src/tools/__pycache__/modal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.1/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc` & `honkairail-1.0.2/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.1/honkairail/src/tools/api.py` & `honkairail-1.0.2/honkairail/src/tools/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import aiohttp
 import asyncio
 import json
-from .modal import StarRailApiData, PlayerInfo,StarRailApiDataV2
+from .modalV1 import StarRailApiData
+from .modalV2 import StarRailApiDataV2
 from . import utilities
 
 SUPPORTED_LANGUAGES = {
     'cht': 'cht',
     'cn': 'cn',
     'de': 'de',
     'en': 'en',
@@ -54,19 +55,19 @@
     data = await get_user_data(uid, lang, v)
     if v == 1:
         return StarRailApiData(player=data["player"], characters=data["characters"])
     return StarRailApiDataV2(player=data["player"], characters=data["characters"])
 
 async def get_full(lang, uid,v):
     data = await get_user_data(uid, lang,v)
-    profile = await get_full_user_data(uid,lang)
     for key in data["characters"]:
         if key["light_cone"] == {}:
             key["light_cone"] = None
     if v == 1:
+        profile = await get_full_user_data(uid,lang)
         player_info = profile["detailInfo"]
         data["player"]["friends"] = player_info["friendCount"]
         data["player"]["worldlevel"] = player_info["worldLevel"]
         data["player"]["birthday"] = "0"#utilities.convert_date(profile["Birthday"])
         data["player"]["pass_area_progress"] = player_info["recordInfo"]["challengeInfo"]["scheduleMaxLevel"]
         data["player"]["light_cone"] = player_info["recordInfo"]["equipmentCount"]
         data["player"]["characters"] = player_info["recordInfo"]["avatarCount"]
```

### Comparing `honkairail-1.0.1/honkairail/src/tools/modal.py` & `honkairail-1.0.2/honkairail/src/tools/modalV2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from . import utilities
 from pydantic import BaseModel
 from typing import List,Optional
-from . import utilities
 
 class Color(BaseModel):
     hex: Optional[str]
     rgba: Optional[tuple]
 
 class ElementV2(BaseModel):
     id: Optional[str]
@@ -141,46 +141,58 @@
     display: str
     percent: bool
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
 
+class SkillTrees(BaseModel):
+    id: Optional[int]
+    level: Optional[int]
+    icon: Optional[str]
+    
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
+
 class CharacterData(BaseModel):
     id: Optional[str]
     name: Optional[str]
     rarity: Optional[int]
     rank: Optional[int]
     level: Optional[int]
     promotion: Optional[int]
     icon: Optional[str]
     preview: Optional[str]
     portrait: Optional[str]
     path: Optional[PathV2]
+    rank_icons: Optional[list]
     element: Optional[ElementV2]
     skills: Optional[List[SkillV2]]
+    skill_trees: Optional[List[SkillTrees]]
     light_cone: Optional[LightConeV2]
     relics: Optional[List[RelicV2]]
     relic_sets: Optional[List[RelicSetV2]]
     additions: Optional[List[Addition]]
     attributes: Optional[List[AttributeV2]]
     properties: Optional[List[PropertyV2]]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.name = self.name.format(NICKNAME = "Trailblazer")
         self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
         self.preview = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.preview}"
         self.portrait = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.portrait}"
+        new_rank_icons = []
+        for key in self.rank_icons:
+            new_rank_icons.append(f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{key}")
+        self.rank_icons = new_rank_icons
 
-    
 
 
-
-#===================================
 class Avatar(BaseModel):
     id: Optional[str]
     name: Optional[str]
     icon: Optional[str]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -188,188 +200,21 @@
 
 class SpaceInfo(BaseModel):
     pass_area_progress: Optional[int]
     light_cone_count: Optional[int]
     avatar_count: Optional[int]
     achievement_count: Optional[int]
 
-
 class PlayerV2(BaseModel):
     uid: Optional[str]
     nickname: Optional[str]
     level: Optional[int]
     avatar: Optional[Avatar]
     signature: Optional[str]
     friend_count: Optional[int]
     world_level: Optional[int]
     birthday: Optional[str]
     space_info: Optional[SpaceInfo]
 
-
-class Player(BaseModel):
-    uid: str
-    name: str
-    level: int
-    icon: str
-    signature: str
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
-
-
-
-
-class RankIcon(BaseModel):
-    icon: str
-    unlock: bool
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
-
-class Skill(BaseModel):
-    name: str
-    level: int
-    type: str
-    icon: str
-    
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
-
-class MainProperty(BaseModel):
-    name: str
-    value: str
-    icon: str
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
-
-class SubProperty(BaseModel):
-    name: str
-    value: str
-    icon: str
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
-
-class Relic(BaseModel):
-    name: str
-    rarity: int
-    level: int
-    main_property: MainProperty
-    sub_property: List[SubProperty]
-    icon: str
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
-
-class RelicSet(BaseModel):
-    name: str
-    icon: str
-    desc: str
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
-
-class Property(BaseModel):
-    name: str
-    base: str
-    addition: Optional[str]
-    icon: str
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
-
-class PatchInfo(BaseModel):
-    name: Optional[str]
-    url: Optional[str]
-
-class LightConeInfo(BaseModel):
-    atk: Optional[int]
-    hp: Optional[int]
-    defense: Optional[int]
-    patch: Optional[PatchInfo]
-
-class LightCone(BaseModel):
-    id: Optional[int]
-    name: Optional[str]
-    rarity: Optional[int]
-    rank: Optional[int]
-    level: Optional[int]
-    icon: Optional[str] = "icon/light_cone/24000.png"
-    portrait: Optional[str]
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.id = self.icon.split('/')[2][:-4]
-        portrait = self.icon.replace("icon/light_cone/", "image/light_cone_portrait/")
-        self.portrait = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{portrait}"
-        self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
-        
-
-class Character(BaseModel):
-    id: Optional[str]
-    name: Optional[str]
-    rarity: Optional[int]
-    level: Optional[int]
-    rank: Optional[int]
-    rank_text: Optional[str]
-    rank_icons: List[RankIcon]
-    preview: Optional[str]
-    portrait: Optional[str]
-    path: Optional[str]
-    path_icon: Optional[str]
-    element: Optional[str]
-    element_icon: Optional[str]
-    color: Optional[str]
-    skill: List[Skill]
-    light_cone: Optional[LightCone]
-    relic: dict[str, Relic]
-    relic_set: List[RelicSet]
-    property: List[Property]
-    
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.name = self.name.format(NICKNAME = "Trailblazer")
-        self.element_icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.element_icon}"
-        self.path_icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.path_icon}"
-        self.preview = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.preview}"
-        self.portrait = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.portrait}"
-
-
 class StarRailApiDataV2(BaseModel):
     player: PlayerV2
-    characters: List[CharacterData]
-
-class StarRailApiData(BaseModel):
-    player: Player
-    characters: List[Character]
-
-class PlayerSpaceInfo(BaseModel):
-    PassAreaProgress: Optional[int]
-    LightConeCount: Optional[int]
-    AvatarCount: Optional[int]
-    AchievementCount: Optional[int]
-
-
-class PlayerDetailInfo(BaseModel):
-    UID: int
-    CurFriendCount: Optional[int]
-    WorldLevel: Optional[int]
-    Signature: Optional[str]
-    NickName: Optional[str]
-    Birthday: Optional[int]
-    Level: Optional[int]
-    PlayerSpaceInfo: Optional[PlayerSpaceInfo]
-
-
-class PlayerInfo(BaseModel):
-    PlayerDetailInfo: PlayerDetailInfo
-  
-
+    characters: List[CharacterData]
```

### Comparing `honkairail-1.0.1/honkairail/src/tools/utilities.py` & `honkairail-1.0.2/honkairail/src/tools/utilities.py`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.1/honkairail/starrailapi.py` & `honkairail-1.0.2/honkairail/starrailapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .src.tools import api, modal,utilities
+from .src.tools import api, modalV1,utilities
 
 class StarRailApi():
     def __init__(self,lang, v = 1) -> None:
         self.lang = lang
         if not v in [1,2]:
             v = 1
         self.v = v
@@ -24,8 +24,8 @@
         data = utilities.get_stats_light_cone(stats["defaultData"]["stats_csv"], instance.level)
         patch = stats["defaultData"]["path"]
         icon = patch["icon"]
         data["patch"] = {
             "name": patch["name"],
             "url": icon["url"]
         }
-        return modal.LightConeInfo(**data)
+        return modalV1.LightConeInfo(**data)
```

### Comparing `honkairail-1.0.1/README.md` & `honkairail-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.1/setup.py` & `honkairail-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['honkairail', 'honkairail.src', 'honkairail.src.tools']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'honkairail',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'A simple and convenient model for Mihoyo API which is complemented by other resources',
     'long_description': '# HonkaiRail\n A simple and convenient model for Mihoyo API which is complemented by other resources\n\n\n## Install:\n\n```\npip install honkairail\n```\n\n## Uses:\n``` py\nfrom honkairail import starrailapi\nimport asyncio\n\n#The sample code below matches version 1 (v = 1), but you can set it to 1 or 2. The second version is newer and contains a bit more data.\nasync def main(uid,lang):\n    r = starrailapi.StarRailApi(lang, v = 1)\n    data = await r.get_full_data(uid)\n    print(data)\n\nasyncio.run(main(700649319,"en"))\n```\n\n## Usage example:\n\n```py\nfrom honkairail import starrailapi\nimport asyncio\n\n\nasync def main(uid,lang):\n    r = starrailapi.StarRailApi(lang)\n    data = await r.get_full_data(uid)\n    print("====Player====")\n    print(f"Name: {data.player.name}")\n    print(f"UID: {data.player.uid}")\n    print(f"Level: {data.player.level}")\n    print(f"World Level: {data.player.worldlevel}")\n    \n    print(f"Friends: {data.player.friends}")\n\n    print(f"Pass Area Progress: {data.player.pass_area_progress}")\n    print(f"Achievement: {data.player.achievement}")\n\n    print(f"Characters: {data.player.characters}")\n    print(f"Light Cone: {data.player.light_cone}")\n\n    print(f"Icon: {data.player.icon}")\n    print(f"Signature: {data.player.signature}")\n    print(\'\\n\\n\')\n    print("====Characters====")\n    for character in data.characters:\n        print(f"Name: {character.name} | {character.id}")\n        print(f"Rarity: {\'★\'*character.rarity}")\n        print(f"LVL: {character.level}")\n        print(f"===={character.rank_text}====")\n        for rank in character.rank_icons:\n            print(f"Icon: {rank.icon}\\nUnlock: {rank.unlock}")\n        print("====Skill====")\n        for skill in character.skill:\n            print(f"Icon: {skill.icon}\\nLVL:{skill.level}")\n        print("=============")\n        if not character.light_cone is None:\n            print(f"Light Cone: {character.light_cone.name}")\n            print(f"Rarity: {\'★\'*character.light_cone.rarity}")\n            print(f"LVL: {character.light_cone.level} | R{character.light_cone.rank}")\n            print(f"Icon: {character.light_cone.icon}")\n            print(f"Portrait: {character.light_cone.portrait}")\n            light_cone = await r.get_light_cone_info(character.light_cone)\n            print(f"ATK: {light_cone.atk} | HP: {light_cone.hp} | DEF: {light_cone.defense}")\n            print(f"Path: {light_cone.patch.name}\\nImage: {light_cone.patch.url}")\n        print("====Stats====")\n        for property in character.property:\n            if property.addition is None:\n                print(f"{property.name}: {property.base}\\nIcon: {property.icon}")\n            else:\n                print(f"{property.name}: {property.base} ({property.addition})\\n==Icon: {property.icon}")\n        print(\'\\n\\n\')\n        print("====Relic====")\n        for i in character.relic:\n            print(f"{character.relic[i].name}: {character.relic[i].level} lvl | {\'★\'*character.relic[i].rarity}")\n            print(f"{character.relic[i].main_property.name}: {character.relic[i].main_property.value}")\n            for sub_property in character.relic[i].sub_property:\n                print(f"=={sub_property.name}: {sub_property.value}\\n====Icon: {sub_property.icon}")\n            print(\'\\n\')\n        print("\\n\\n")\n\nasyncio.run(main(700649319, "en"))\n```\n\n\n### Languages Supported\n| Languege    |  Code   | Languege    |  Code   | Languege    |  Code   |\n|-------------|---------|-------------|---------|-------------|---------|\n|  English    |     en  |  русский    |     ru  |  Chinese    |    chs  |\n|  Tiếng Việt |     vi  |  ไทย        |     th  | Taiwan     |    cn  |\n|  português  |     pt  | 한국어      |     kr  | deutsch    |     de  |\n|  日本語      |     jp  | 中文        |     zh  | español    |     es  |\n|  中文        |     zh  | Indonesian |     id  | français   |     fr  |\n\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DEViantUA/HonkaiRail',
```

### Comparing `honkairail-1.0.1/PKG-INFO` & `honkairail-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honkairail
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple and convenient model for Mihoyo API which is complemented by other resources
 Home-page: https://github.com/DEViantUA/HonkaiRail
 Author: None
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

