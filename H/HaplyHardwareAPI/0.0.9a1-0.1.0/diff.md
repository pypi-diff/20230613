# Comparing `tmp/HaplyHardwareAPI-0.0.9a1-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip` & `tmp/HaplyHardwareAPI-0.1.0-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1078918 bytes, number of entries: 7
--rwxr-xr-x  2.0 unx   377888 b- defN 23-Feb-22 15:41 HaplyHardwareAPI.cpython-311-darwin.so
--rw-rw-r--  2.0 unx      648 b- defN 23-Feb-22 15:41 HaplyHardwareAPI-0.0.9a1.dist-info/RECORD
--rw-r--r--  2.0 unx      115 b- defN 23-Feb-22 20:41 HaplyHardwareAPI-0.0.9a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Feb-22 20:41 HaplyHardwareAPI-0.0.9a1.dist-info/top_level.txt
--rw-r--r--  2.0 unx      374 b- defN 23-Feb-22 20:41 HaplyHardwareAPI-0.0.9a1.dist-info/METADATA
--rw-r--r--  2.0 unx  3456944 b- defN 23-Feb-22 15:41 HaplyHardwareAPI.dylibs/libstdc++.6.dylib
--rw-r--r--  2.0 unx   157520 b- defN 23-Feb-22 15:41 HaplyHardwareAPI.dylibs/libgcc_s.1.1.dylib
-7 files, 3993506 bytes uncompressed, 1077778 bytes compressed:  73.0%
+Zip file size: 1078897 bytes, number of entries: 7
+-rwxr-xr-x  2.0 unx   377888 b- defN 23-Feb-27 16:50 HaplyHardwareAPI.cpython-311-darwin.so
+-rw-rw-r--  2.0 unx      640 b- defN 23-Feb-27 16:50 HaplyHardwareAPI-0.1.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      115 b- defN 23-Feb-27 21:50 HaplyHardwareAPI-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Feb-27 21:50 HaplyHardwareAPI-0.1.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      372 b- defN 23-Feb-27 21:50 HaplyHardwareAPI-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx  3456944 b- defN 23-Feb-27 16:50 HaplyHardwareAPI.dylibs/libstdc++.6.dylib
+-rw-r--r--  2.0 unx   157520 b- defN 23-Feb-27 16:50 HaplyHardwareAPI.dylibs/libgcc_s.1.1.dylib
+7 files, 3993496 bytes uncompressed, 1077773 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
 Filename: HaplyHardwareAPI.cpython-311-darwin.so
 Comment: 
 
-Filename: HaplyHardwareAPI-0.0.9a1.dist-info/RECORD
+Filename: HaplyHardwareAPI-0.1.0.dist-info/RECORD
 Comment: 
 
-Filename: HaplyHardwareAPI-0.0.9a1.dist-info/WHEEL
+Filename: HaplyHardwareAPI-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: HaplyHardwareAPI-0.0.9a1.dist-info/top_level.txt
+Filename: HaplyHardwareAPI-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: HaplyHardwareAPI-0.0.9a1.dist-info/METADATA
+Filename: HaplyHardwareAPI-0.1.0.dist-info/METADATA
 Comment: 
 
 Filename: HaplyHardwareAPI.dylibs/libstdc++.6.dylib
 Comment: 
 
 Filename: HaplyHardwareAPI.dylibs/libgcc_s.1.1.dylib
 Comment:
```

## HaplyHardwareAPI.cpython-311-darwin.so

### aarch64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit arm64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL|WEAK_DEFINES|BINDS_TO_WEAK>*

```diff
@@ -104,15 +104,15 @@
 00000670: 0200 0000 1800 0000 d803 0500 bf01 0000  ................
 00000680: 2829 0500 a848 0000 0b00 0000 5000 0000  ()...H......P...
 00000690: 0000 0000 0100 0000 0100 0000 8d00 0000  ................
 000006a0: 8e00 0000 3101 0000 0000 0000 0000 0000  ....1...........
 000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: c81f 0500 5802 0000 0000 0000 0000 0000  ....X...........
 000006d0: 0000 0000 0000 0000 1b00 0000 1800 0000  ................
-000006e0: ce87 6dfc e2ac 3c1a a2f3 7886 aa77 343d  ..m...<...x..w4=
+000006e0: aaf6 7f3d 9d12 364b a086 9e34 fc6b 5ce7  ...=..6K...4.k\.
 000006f0: 3200 0000 2000 0000 0100 0000 0000 0b00  2... ...........
 00000700: 0001 0d00 0100 0000 0300 0000 0001 3403  ..............4.
 00000710: 2a00 0000 1000 0000 0000 0000 0000 0000  *...............
 00000720: 0c00 0000 5000 0000 1800 0000 0200 0000  ....P...........
 00000730: 001e 0700 0000 0700 406c 6f61 6465 725f  ........@loader_
 00000740: 7061 7468 2f48 6170 6c79 4861 7264 7761  path/HaplyHardwa
 00000750: 7265 4150 492e 6479 6c69 6273 2f6c 6962  reAPI.dylibs/lib
@@ -12859,15 +12859,15 @@
 000323a0: 5d20 2573 0a00 0000 7374 643a 3a66 7574  ] %s....std::fut
 000323b0: 7572 655f 6572 726f 723a 2000 0000 0000  ure_error: .....
 000323c0: 0000 0000 0000 0000 7665 6374 6f72 3a3a  ........vector::
 000323d0: 5f4d 5f72 6561 6c6c 6f63 5f69 6e73 6572  _M_realloc_inser
 000323e0: 7400 0000 0000 0000 6578 6365 7074 696f  t.......exceptio
 000323f0: 6e3a 2025 730a 0000 4c69 6272 6172 7920  n: %s...Library 
 00032400: 7665 7273 696f 6e3a 2000 0000 0000 0000  version: .......
-00032410: 302e 302e 3800 0000 4e6f 2070 6f72 7473  0.0.8...No ports
+00032410: 302e 312e 3000 0000 4e6f 2070 6f72 7473  0.1.0...No ports
 00032420: 2066 6f75 6e64 202e 202e 202e 0000 0000   found . . .....
 00032430: 5b65 7272 5d20 2573 3a25 753e 2075 6e61  [err] %s:%u> una
 00032440: 626c 6520 746f 206f 7065 6e20 706f 7274  ble to open port
 00032450: 2027 2573 273a 205b 2564 5d20 2573 0a00   '%s': [%d] %s..
 00032460: 2f55 7365 7273 2f68 6170 6c79 2f62 7569  /Users/haply/bui
 00032470: 6c64 732f 3559 6e6b 6131 696b 2f30 2f48  lds/5Ynka1ik/0/H
 00032480: 6170 6c79 2f49 6e74 6572 6e61 6c2f 6861  aply/Internal/ha
@@ -22309,16 +22309,16 @@
 00057240: 0004 0000 0000 0000 0000 0000 4861 706c  ............Hapl
 00057250: 7948 6172 6477 6172 6541 5049 2e63 7079  yHardwareAPI.cpy
 00057260: 7468 6f6e 2d33 3131 2d64 6172 7769 6e00  thon-311-darwin.
 00057270: 9879 2090 4eab 650e 7578 8c05 4aa0 b052  .y .N.e.ux..J..R
 00057280: 4e6a 80bf c71a a32d f8d2 37a6 1743 f986  Nj.....-..7..C..
 00057290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000572a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000572b0: d348 e51b 8bb3 3233 2084 bf83 ca81 55f7  .H....23 .....U.
-000572c0: 556a e864 97e6 1ce4 3e83 4974 606f 4c05  Uj.d....>.It`oL.
+000572b0: 0ef2 4daf 6c4b 3ade a576 0407 4b01 2d89  ..M.lK:..v..K.-.
+000572c0: 6950 b461 1de5 18af 0117 e47b 8220 1d18  iP.a.......{. ..
 000572d0: ad7f acb2 586f c6e9 66c0 04d7 d1d1 6b02  ....Xo..f.....k.
 000572e0: 4f58 05ff 7cb4 7c7a 85da bd8b 4889 2ca7  OX..|.|z....H.,.
 000572f0: bb65 64da 9c38 895a ec86 929f 7397 c3a8  .ed..8.Z....s...
 00057300: dbc2 9867 20ec 190a 8a2b 55bd bff8 2858  ...g ....+U...(X
 00057310: cb78 1df3 b42d 435f 8818 8529 7ae2 cbfe  .x...-C_...)z...
 00057320: b4c0 c33d de9a 6fb9 c940 a3d2 0e5e b028  ...=..o..@...^.(
 00057330: 733f aff3 1897 09ac b1d3 052a 56d8 6914  s?.........*V.i.
@@ -22409,16 +22409,16 @@
 00057880: 7df5 1b91 e54f a462 efb5 59fa db79 0f16  }....O.b..Y..y..
 00057890: 39b7 51bb 904f b057 bf4b dc0e da9d 707d  9.Q..O.W.K....p}
 000578a0: df95 8510 7c3e e3e9 688c 97d7 9020 bfe4  ....|>..h.... ..
 000578b0: d5c1 564d 9707 5752 1095 7a4b dc4b 13c4  ..VM..WR..zK.K..
 000578c0: ed15 ab06 61ef 2ffa 1155 d673 0e11 5063  ....a./..U.s..Pc
 000578d0: c4be 3d28 1612 47c3 dbfe 9e6a d786 5024  ..=(..G....j..P$
 000578e0: 7b15 dcf7 852a 8fa2 a2fc bec1 83d1 6fe9  {....*........o.
-000578f0: 2139 c4b0 4585 0031 6b3f 61a6 77de 37f4  !9..E..1k?a.w.7.
-00057900: 4d3e c8c9 b941 3e25 e4a4 dc51 fe43 e40b  M>...A>%...Q.C..
+000578f0: 3b4a 7b51 1d68 c7db c575 c588 5f9d e7a9  ;J{Q.h...u.._...
+00057900: 4d76 be82 8b97 ab73 279f a258 2bd3 cf34  Mv.....s'..X+..4
 00057910: cf0e 5bf9 a4ed 5c6f e94d d7bf 3524 8fb4  ..[...\o.M..5$..
 00057920: 715e c1ca 1c55 acb3 b733 f0df e6af b595  q^...U...3......
 00057930: 0efc e518 629b c8e4 364d 45d1 0c3f 9b86  ....b...6ME..?..
 00057940: 7831 42cc 7a90 e493 9d4b 7cec dae8 d596  x1B.z....K|.....
 00057950: f914 a444 5a83 be15 e0fe 4c64 9568 9312  ...DZ.....Ld.h..
 00057960: c2a5 fcd8 4165 42aa cc3a b362 a0ac f30f  ....AeB..:.b....
 00057970: 285f 2ccd c816 d786 5a3a 533f 1cef 7568  (_,.....Z:S?..uh
```

## Comparing `HaplyHardwareAPI-0.0.9a1.dist-info/RECORD` & `HaplyHardwareAPI-0.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-HaplyHardwareAPI.cpython-311-darwin.so,sha256=Sox0z-uUq0K-1hZMrQR-3f9fJBLIjhw_GO8O35tZGfg,377888
-HaplyHardwareAPI-0.0.9a1.dist-info/RECORD,,
-HaplyHardwareAPI-0.0.9a1.dist-info/WHEEL,sha256=lqQembEA5Dgk8Q6Sva9ekdNjOdchfitukwwZ3fZC9PM,115
-HaplyHardwareAPI-0.0.9a1.dist-info/top_level.txt,sha256=9tQSwxupQlp5Hw8ThRpBm8e1wxIF_nuEh79N3QyFuUc,17
-HaplyHardwareAPI-0.0.9a1.dist-info/METADATA,sha256=6wrYpgUi9leZs56SA4ENwm_xloH2CuzRZHkZSLzzpAE,374
+HaplyHardwareAPI.cpython-311-darwin.so,sha256=8sukSGgAL3Baf-Oj1Y0DNAZucObNIACpJ7UVr9N2yv0,377888
+HaplyHardwareAPI-0.1.0.dist-info/RECORD,,
+HaplyHardwareAPI-0.1.0.dist-info/WHEEL,sha256=lqQembEA5Dgk8Q6Sva9ekdNjOdchfitukwwZ3fZC9PM,115
+HaplyHardwareAPI-0.1.0.dist-info/top_level.txt,sha256=9tQSwxupQlp5Hw8ThRpBm8e1wxIF_nuEh79N3QyFuUc,17
+HaplyHardwareAPI-0.1.0.dist-info/METADATA,sha256=vbvMr3ywiJO64KKu41c28dOthNBAEsopGmJn1KuEYoI,372
 HaplyHardwareAPI.dylibs/libstdc++.6.dylib,sha256=mGooXKDOP7sPymd0biBJyKkiVPACbahrQR1b2bhuGAo,3456944
 HaplyHardwareAPI.dylibs/libgcc_s.1.1.dylib,sha256=kKb7owKNPkOJTpx8TMrvfnSWwcHjd9kBdx9r9JwzLMI,157520
```

