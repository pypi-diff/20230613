# Comparing `tmp/maadstml-3.34.tar.gz` & `tmp/maadstml-3.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.34.tar", last modified: Mon Jun 12 22:57:20 2023, max compression
+gzip compressed data, was "maadstml-3.35.tar", last modified: Tue Jun 13 18:30:06 2023, max compression
```

## Comparing `maadstml-3.34.tar` & `maadstml-3.35.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 22:57:20.986688 maadstml-3.34/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.34/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.34/MANIFEST.in
--rw-rw-rw-   0        0        0   173473 2023-06-12 22:57:20.986688 maadstml-3.34/PKG-INFO
--rw-rw-rw-   0        0        0   172876 2023-06-12 22:51:47.000000 maadstml-3.34/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 22:57:20.970822 maadstml-3.34/maadstml/
--rw-rw-rw-   0        0        0     2258 2023-06-12 22:57:03.000000 maadstml-3.34/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.34/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    80259 2023-06-12 22:44:41.000000 maadstml-3.34/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.34/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-12 22:57:20.986688 maadstml-3.34/maadstml.egg-info/
--rw-rw-rw-   0        0        0   173473 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      188 2023-06-12 17:35:52.000000 maadstml-3.34/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 22:57:20.986688 maadstml-3.34/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-12 22:57:11.000000 maadstml-3.34/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:30:06.561820 maadstml-3.35/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.35/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.35/MANIFEST.in
+-rw-rw-rw-   0        0        0   174408 2023-06-13 18:30:06.559357 maadstml-3.35/PKG-INFO
+-rw-rw-rw-   0        0        0   173811 2023-06-13 18:28:52.000000 maadstml-3.35/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 18:30:06.533583 maadstml-3.35/maadstml/
+-rw-rw-rw-   0        0        0     2387 2023-06-13 18:19:41.000000 maadstml-3.35/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.35/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    81647 2023-06-13 18:18:45.000000 maadstml-3.35/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.35/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:30:06.559357 maadstml-3.35/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   174408 2023-06-13 18:30:06.000000 maadstml-3.35/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-13 18:30:06.000000 maadstml-3.35/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:30:06.000000 maadstml-3.35/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-06-13 18:30:06.000000 maadstml-3.35/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 18:30:06.000000 maadstml-3.35/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      225 2023-06-13 18:10:54.000000 maadstml-3.35/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:30:06.561820 maadstml-3.35/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-13 18:13:39.000000 maadstml-3.35/setup.py
```

### Comparing `maadstml-3.34/LICENSE.txt` & `maadstml-3.35/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.34/PKG-INFO` & `maadstml-3.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.34
+Version: 3.35
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -253,14 +253,23 @@
 
 - **viperexractpdffields**
   - Extracts fields from PDF file
 
 - **viperexractpdffieldbylabel**
   - Extracts fields from PDF file by label name.
 
+- **viperimagetotext**
+  - Extracts text from images like PNG, JPG, etc., which can then be streamed to kafka.
+
+- **viperaudiototext**
+  - Extracts text from audio files like WAV, etc., which can then be streamed to kafka.
+
+- **vipervideototext**
+  - Extracts text from video files like MP4, etc., which can then be streamed to kafka.
+
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
 
@@ -4585,7 +4594,37 @@
 - Label name in the PDF filename to search for.
 
 *pdffilename,labelname,arcotype* : string, required
 
 - Acrobyte tag in PDF i.e. LTTextLineHorizontal
 
 RETURNS: Value of the labelname - if any.
+
+**40. maadstml.viperimagetotext(imagefilename)**
+
+**Parameters:**	Extract text from images.
+
+*imagefilename* : string, required
+
+- Image filename like PNG, JPG etc.
+
+RETURNS: Text in image.
+
+**41. maadstml.vipervideototext(videofilename)**
+
+**Parameters:**	Extract text from video.
+
+*videofilename* : string, required
+
+- Video filename like MP4 etc.
+
+RETURNS: Text in video.
+
+**42. maadstml.viperaudiototext(audiofilename)**
+
+**Parameters:**	Extract text from audio
+
+*audiofilename* : string, required
+
+- Audio filename like WAV etc.
+
+RETURNS: Text in audio.
```

### Comparing `maadstml-3.34/README.md` & `maadstml-3.35/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,23 @@
 
 - **viperexractpdffields**
   - Extracts fields from PDF file
 
 - **viperexractpdffieldbylabel**
   - Extracts fields from PDF file by label name.
 
+- **viperimagetotext**
+  - Extracts text from images like PNG, JPG, etc., which can then be streamed to kafka.
+
+- **viperaudiototext**
+  - Extracts text from audio files like WAV, etc., which can then be streamed to kafka.
+
+- **vipervideototext**
+  - Extracts text from video files like MP4, etc., which can then be streamed to kafka.
+
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
 
@@ -4573,7 +4582,37 @@
 - Label name in the PDF filename to search for.
 
 *pdffilename,labelname,arcotype* : string, required
 
 - Acrobyte tag in PDF i.e. LTTextLineHorizontal
 
 RETURNS: Value of the labelname - if any.
+
+**40. maadstml.viperimagetotext(imagefilename)**
+
+**Parameters:**	Extract text from images.
+
+*imagefilename* : string, required
+
+- Image filename like PNG, JPG etc.
+
+RETURNS: Text in image.
+
+**41. maadstml.vipervideototext(videofilename)**
+
+**Parameters:**	Extract text from video.
+
+*videofilename* : string, required
+
+- Video filename like MP4 etc.
+
+RETURNS: Text in video.
+
+**42. maadstml.viperaudiototext(audiofilename)**
+
+**Parameters:**	Extract text from audio
+
+*audiofilename* : string, required
+
+- Audio filename like WAV etc.
+
+RETURNS: Text in audio.
```

### Comparing `maadstml-3.34/maadstml/__init__.py` & `maadstml-3.35/maadstml/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,8 +79,14 @@
 
 from .sendfiles import viperchatgpt
 
 from .sendfiles import viperexractpdffields
 
 from .sendfiles import viperexractpdffieldbylabel
 
+from .sendfiles import viperimagetotext
+
+from .sendfiles import viperaudiototext
+
+from .sendfiles import vipervideototext
+
 name = "maadstml"
```

### Comparing `maadstml-3.34/maadstml/readpdf.py` & `maadstml-3.35/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.34/maadstml/sendfiles.py` & `maadstml-3.35/maadstml/sendfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -4123,895 +4123,981 @@
 000101a0: 726e 2022 456e 7465 7220 5044 4620 6669  rn "Enter PDF fi
 000101b0: 6c65 6e61 6d65 2c20 6c61 6265 6c6e 616d  lename, labelnam
 000101c0: 6520 616e 6420 6163 726f 7479 7065 220d  e and acrotype".
 000101d0: 0a20 2020 200d 0a20 2020 2072 6574 7572  .    ..    retur
 000101e0: 6e20 6c61 6265 6c66 6965 6c64 7328 6669  n labelfields(fi
 000101f0: 6c65 6e61 6d65 2c6c 6162 656c 6e61 6d65  lename,labelname
 00010200: 2c61 6372 6f74 7970 6529 0d0a 0d0a 6465  ,acrotype)....de
-00010210: 6620 6172 6579 6f75 6275 7379 2868 6f73  f areyoubusy(hos
-00010220: 742c 706f 7274 3d2d 3939 392c 6d69 6372  t,port=-999,micr
-00010230: 6f73 6572 7669 6365 6964 3d27 2729 3a0d  oserviceid=''):.
-00010240: 0a20 2020 2067 6c6f 6261 6c20 636f 6e6e  .    global conn
-00010250: 6563 7469 6f6e 6572 726f 720d 0a0d 0a20  ectionerror.... 
-00010260: 2020 2069 6620 286c 656e 2868 6f73 7429     if (len(host)
-00010270: 3d3d 3020 6f72 2070 6f72 743d 3d2d 3939  ==0 or port==-99
-00010280: 3920 293a 0d0a 2020 2020 2020 2020 2072  9 ):..         r
-00010290: 6574 7572 6e20 2250 6c65 6173 6520 656e  eturn "Please en
-000102a0: 7465 7220 686f 7374 2c70 6f72 7422 0d0a  ter host,port"..
-000102b0: 2020 2020 7661 6c75 653d 2822 6172 6579      value=("arey
-000102c0: 6f75 6275 7379 2229 0d0a 0d0a 2020 2020  oubusy")....    
-000102d0: 7661 6c3d 6c6f 6f70 2e72 756e 5f75 6e74  val=loop.run_unt
-000102e0: 696c 5f63 6f6d 706c 6574 6528 7463 705f  il_complete(tcp_
-000102f0: 6563 686f 5f63 6c69 656e 7476 6970 6572  echo_clientviper
-00010300: 2876 616c 7565 2c20 6c6f 6f70 2c68 6f73  (value, loop,hos
-00010310: 742c 706f 7274 2c6d 6963 726f 7365 7276  t,port,microserv
-00010320: 6963 6569 6429 290d 0a20 2020 2069 6620  iceid))..    if 
-00010330: 636f 6e6e 6563 7469 6f6e 6572 726f 723a  connectionerror:
-00010340: 0d0a 2020 2020 2020 2020 2072 6574 7572  ..         retur
-00010350: 6e20 636f 6e6e 6563 7469 6f6e 6572 726f  n connectionerro
-00010360: 720d 0a0d 0a20 2020 2072 6574 7572 6e20  r....    return 
-00010370: 7661 6c0d 0a0d 0a23 2323 2323 2323 2323  val....#########
-00010380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000103a0: 2323 2323 2323 2323 2323 230d 0a69 6d70  ###########..imp
-000103b0: 6f72 7420 7379 730d 0a66 726f 6d20 7064  ort sys..from pd
-000103c0: 666d 696e 6572 2e70 6466 7061 7273 6572  fminer.pdfparser
-000103d0: 2069 6d70 6f72 7420 5044 4650 6172 7365   import PDFParse
-000103e0: 720d 0a66 726f 6d20 7064 666d 696e 6572  r..from pdfminer
-000103f0: 2e70 6466 646f 6375 6d65 6e74 2069 6d70  .pdfdocument imp
-00010400: 6f72 7420 5044 4644 6f63 756d 656e 740d  ort PDFDocument.
-00010410: 0a66 726f 6d20 7064 666d 696e 6572 2e70  .from pdfminer.p
-00010420: 6466 7061 6765 2069 6d70 6f72 7420 5044  dfpage import PD
-00010430: 4650 6167 650d 0a66 726f 6d20 7064 666d  FPage..from pdfm
-00010440: 696e 6572 2e70 6466 7061 6765 2069 6d70  iner.pdfpage imp
-00010450: 6f72 7420 5044 4654 6578 7445 7874 7261  ort PDFTextExtra
-00010460: 6374 696f 6e4e 6f74 416c 6c6f 7765 640d  ctionNotAllowed.
-00010470: 0a66 726f 6d20 7064 666d 696e 6572 2e70  .from pdfminer.p
-00010480: 6466 696e 7465 7270 2069 6d70 6f72 7420  dfinterp import 
-00010490: 5044 4652 6573 6f75 7263 654d 616e 6167  PDFResourceManag
-000104a0: 6572 0d0a 6672 6f6d 2070 6466 6d69 6e65  er..from pdfmine
-000104b0: 722e 7064 6669 6e74 6572 7020 696d 706f  r.pdfinterp impo
-000104c0: 7274 2050 4446 5061 6765 496e 7465 7270  rt PDFPageInterp
-000104d0: 7265 7465 720d 0a23 6672 6f6d 2053 7472  reter..#from Str
-000104e0: 696e 6749 4f20 696d 706f 7274 2053 7472  ingIO import Str
-000104f0: 696e 6749 4f0d 0a66 726f 6d20 696f 2069  ingIO..from io i
-00010500: 6d70 6f72 7420 5374 7269 6e67 494f 0d0a  mport StringIO..
-00010510: 696d 706f 7274 2075 726c 6c69 622e 7265  import urllib.re
-00010520: 7175 6573 7420 200d 0a23 696d 706f 7274  quest  ..#import
-00010530: 2074 6d6c 7465 7874 7375 6d6d 6172 790d   tmltextsummary.
-00010540: 0a69 6d70 6f72 7420 6f73 0d0a 696d 706f  .import os..impo
-00010550: 7274 2064 6174 6574 696d 650d 0a23 696d  rt datetime..#im
-00010560: 706f 7274 2067 6c6f 620d 0a0d 0a0d 0a66  port glob......f
-00010570: 726f 6d20 7064 666d 696e 6572 2e6c 6179  rom pdfminer.lay
-00010580: 6f75 7420 696d 706f 7274 204c 4150 6172  out import LAPar
-00010590: 616d 730d 0a66 726f 6d20 7064 666d 696e  ams..from pdfmin
-000105a0: 6572 2e63 6f6e 7665 7274 6572 2069 6d70  er.converter imp
-000105b0: 6f72 7420 5465 7874 436f 6e76 6572 7465  ort TextConverte
-000105c0: 720d 0a20 0d0a 636c 6173 7320 4d79 5061  r.. ..class MyPa
-000105d0: 7273 6572 286f 626a 6563 7429 3a0d 0a20  rser(object):.. 
-000105e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000105f0: 7365 6c66 2c20 7064 6629 3a0d 0a20 2020  self, pdf):..   
-00010600: 2020 2020 2023 2320 536e 6970 7065 6420       ## Snipped 
-00010610: 6164 6170 7465 6420 6672 6f6d 2059 7573  adapted from Yus
-00010620: 756b 6520 5368 696e 7961 6d61 7320 0d0a  uke Shinyamas ..
-00010630: 2020 2020 2020 2020 2350 4446 4d69 6e65          #PDFMine
-00010640: 7220 646f 6375 6d65 6e74 6174 696f 6e0d  r documentation.
-00010650: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
-00010660: 6520 7468 6520 646f 6375 6d65 6e74 206d  e the document m
-00010670: 6f64 656c 2066 726f 6d20 7468 6520 6669  odel from the fi
-00010680: 6c65 0d0a 2020 2020 2020 2020 7061 7273  le..        pars
-00010690: 6572 203d 2050 4446 5061 7273 6572 286f  er = PDFParser(o
-000106a0: 7065 6e28 7064 662c 2027 7262 2729 290d  pen(pdf, 'rb')).
-000106b0: 0a20 2020 2020 2020 2064 6f63 756d 656e  .        documen
-000106c0: 7420 3d20 5044 4644 6f63 756d 656e 7428  t = PDFDocument(
-000106d0: 7061 7273 6572 290d 0a20 2020 2020 2020  parser)..       
-000106e0: 2023 2054 7279 2074 6f20 7061 7273 6520   # Try to parse 
-000106f0: 7468 6520 646f 6375 6d65 6e74 0d0a 2020  the document..  
-00010700: 2020 2020 2020 6966 206e 6f74 2064 6f63        if not doc
-00010710: 756d 656e 742e 6973 5f65 7874 7261 6374  ument.is_extract
-00010720: 6162 6c65 3a0d 0a20 2020 2020 2020 2020  able:..         
-00010730: 2020 2072 6169 7365 2050 4446 5465 7874     raise PDFText
-00010740: 4578 7472 6163 7469 6f6e 4e6f 7441 6c6c  ExtractionNotAll
-00010750: 6f77 6564 0d0a 2020 2020 2020 2020 2320  owed..        # 
-00010760: 4372 6561 7465 2061 2050 4446 2072 6573  Create a PDF res
-00010770: 6f75 7263 6520 6d61 6e61 6765 7220 6f62  ource manager ob
-00010780: 6a65 6374 200d 0a20 2020 2020 2020 2023  ject ..        #
-00010790: 2074 6861 7420 7374 6f72 6573 2073 6861   that stores sha
-000107a0: 7265 6420 7265 736f 7572 6365 732e 0d0a  red resources...
-000107b0: 2020 2020 2020 2020 7273 7263 6d67 7220          rsrcmgr 
-000107c0: 3d20 5044 4652 6573 6f75 7263 654d 616e  = PDFResourceMan
-000107d0: 6167 6572 2829 0d0a 2020 2020 2020 2020  ager()..        
-000107e0: 2320 4372 6561 7465 2061 2062 7566 6665  # Create a buffe
-000107f0: 7220 666f 7220 7468 6520 7061 7273 6564  r for the parsed
-00010800: 2074 6578 740d 0a20 2020 2020 2020 2072   text..        r
-00010810: 6574 7374 7220 3d20 5374 7269 6e67 494f  etstr = StringIO
-00010820: 2829 0d0a 2020 2020 2020 2020 2320 5370  ()..        # Sp
-00010830: 6163 696e 6720 7061 7261 6d65 7465 7273  acing parameters
-00010840: 2066 6f72 2070 6172 7369 6e67 0d0a 2020   for parsing..  
-00010850: 2020 2020 2020 6c61 7061 7261 6d73 203d        laparams =
-00010860: 204c 4150 6172 616d 7328 290d 0a20 2020   LAParams()..   
-00010870: 2020 2020 2063 6f64 6563 203d 2027 7574       codec = 'ut
-00010880: 662d 3827 0d0a 200d 0a20 2020 2020 2020  f-8'.. ..       
-00010890: 2023 2043 7265 6174 6520 6120 5044 4620   # Create a PDF 
-000108a0: 6465 7669 6365 206f 626a 6563 740d 0a20  device object.. 
-000108b0: 2020 2020 2020 2064 6576 6963 6520 3d20         device = 
-000108c0: 5465 7874 436f 6e76 6572 7465 7228 7273  TextConverter(rs
-000108d0: 7263 6d67 722c 2072 6574 7374 722c 0d0a  rcmgr, retstr,..
-000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00010900: 6170 6172 616d 7320 3d20 6c61 7061 7261  aparams = lapara
-00010910: 6d73 290d 0a20 2020 2020 2020 2023 2043  ms)..        # C
-00010920: 7265 6174 6520 6120 5044 4620 696e 7465  reate a PDF inte
-00010930: 7270 7265 7465 7220 6f62 6a65 6374 0d0a  rpreter object..
-00010940: 2020 2020 2020 2020 696e 7465 7270 7265          interpre
-00010950: 7465 7220 3d20 5044 4650 6167 6549 6e74  ter = PDFPageInt
-00010960: 6572 7072 6574 6572 2872 7372 636d 6772  erpreter(rsrcmgr
-00010970: 2c20 6465 7669 6365 290d 0a20 2020 2020  , device)..     
-00010980: 2020 2023 2050 726f 6365 7373 2065 6163     # Process eac
-00010990: 6820 7061 6765 2063 6f6e 7461 696e 6564  h page contained
-000109a0: 2069 6e20 7468 6520 646f 6375 6d65 6e74   in the document
-000109b0: 2e0d 0a20 2020 2020 2020 2066 6f72 2070  ...        for p
-000109c0: 6167 6520 696e 2050 4446 5061 6765 2e63  age in PDFPage.c
-000109d0: 7265 6174 655f 7061 6765 7328 646f 6375  reate_pages(docu
-000109e0: 6d65 6e74 293a 0d0a 2020 2020 2020 2020  ment):..        
-000109f0: 2020 2020 696e 7465 7270 7265 7465 722e      interpreter.
-00010a00: 7072 6f63 6573 735f 7061 6765 2870 6167  process_page(pag
-00010a10: 6529 0d0a 2020 2020 2020 2020 200d 0a20  e)..         .. 
-00010a20: 2020 2020 2020 2073 656c 662e 7265 636f         self.reco
-00010a30: 7264 7320 2020 2020 2020 2020 2020 203d  rds            =
-00010a40: 205b 5d0d 0a20 2020 2020 2020 2020 0d0a   []..         ..
-00010a50: 2020 2020 2020 2020 6c69 6e65 7320 3d20          lines = 
-00010a60: 7265 7473 7472 2e67 6574 7661 6c75 6528  retstr.getvalue(
-00010a70: 292e 7370 6c69 746c 696e 6573 2829 0d0a  ).splitlines()..
-00010a80: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
-00010a90: 2069 6e20 6c69 6e65 733a 0d0a 2020 2020   in lines:..    
-00010aa0: 2020 2020 2020 2020 7365 6c66 2e68 616e          self.han
-00010ab0: 646c 655f 6c69 6e65 286c 696e 6529 0d0a  dle_line(line)..
-00010ac0: 2020 2020 200d 0a20 2020 2064 6566 2068       ..    def h
-00010ad0: 616e 646c 655f 6c69 6e65 2873 656c 662c  andle_line(self,
-00010ae0: 206c 696e 6529 3a0d 0a20 2020 2020 2020   line):..       
-00010af0: 2023 2043 7573 746f 6d69 7a65 2079 6f75   # Customize you
-00010b00: 7220 6c69 6e65 2d62 792d 6c69 6e65 2070  r line-by-line p
-00010b10: 6172 7365 7220 6865 7265 0d0a 2020 2020  arser here..    
-00010b20: 2020 2020 7365 6c66 2e72 6563 6f72 6473      self.records
-00010b30: 2e61 7070 656e 6428 6c69 6e65 290d 0a0d  .append(line)...
-00010b40: 0a64 6566 2073 6372 6170 6570 6466 2874  .def scrapepdf(t
-00010b50: 6865 7572 6c2c 666e 293a 0d0a 2020 2020  heurl,fn):..    
-00010b60: 7363 7261 7065 645f 6461 7461 203d 2075  scraped_data = u
-00010b70: 726c 6c69 622e 7265 7175 6573 742e 7572  rllib.request.ur
-00010b80: 6c6f 7065 6e28 7468 6575 726c 2920 200d  lopen(theurl)  .
-00010b90: 0a20 2020 2066 696c 6520 3d20 6f70 656e  .    file = open
-00010ba0: 2866 6e2c 2027 7762 2729 0d0a 2020 2020  (fn, 'wb')..    
-00010bb0: 6669 6c65 2e77 7269 7465 2873 6372 6170  file.write(scrap
-00010bc0: 6564 5f64 6174 612e 7265 6164 2829 290d  ed_data.read()).
-00010bd0: 0a20 2020 2066 696c 652e 636c 6f73 6528  .    file.close(
-00010be0: 290d 0a20 2020 2023 7265 7475 726e 2061  )..    #return a
-00010bf0: 7274 6963 6c65 5f74 6578 740d 0a0d 0a64  rticle_text....d
-00010c00: 6566 2073 7461 7274 7064 6672 6561 6469  ef startpdfreadi
-00010c10: 6e67 2866 696c 656e 616d 652c 6676 616c  ng(filename,fval
-00010c20: 7565 2c6b 6579 636f 756e 7429 3a0d 0a20  ue,keycount):.. 
-00010c30: 2023 6f73 2e70 6174 682e 6162 7370 6174   #os.path.abspat
-00010c40: 6828 6f73 2e67 6574 6377 6428 2929 0d0a  h(os.getcwd())..
-00010c50: 2020 7468 6573 697a 653d 726f 756e 6428    thesize=round(
-00010c60: 6f73 2e70 6174 682e 6765 7473 697a 6528  os.path.getsize(
-00010c70: 6669 6c65 6e61 6d65 292f 3130 3030 3030  filename)/100000
-00010c80: 302c 3229 0d0a 2020 6d5f 7469 6d65 203d  0,2)..  m_time =
-00010c90: 206f 732e 7061 7468 2e67 6574 6d74 696d   os.path.getmtim
-00010ca0: 6528 6669 6c65 6e61 6d65 290d 0a20 2064  e(filename)..  d
-00010cb0: 745f 6d20 3d20 6461 7465 7469 6d65 2e64  t_m = datetime.d
-00010cc0: 6174 6574 696d 652e 6672 6f6d 7469 6d65  atetime.fromtime
-00010cd0: 7374 616d 7028 6d5f 7469 6d65 290d 0a20  stamp(m_time).. 
-00010ce0: 2063 5f74 696d 6520 3d20 6f73 2e70 6174   c_time = os.pat
-00010cf0: 682e 6765 7463 7469 6d65 2866 696c 656e  h.getctime(filen
-00010d00: 616d 6529 0d0a 2020 2320 636f 6e76 6572  ame)..  # conver
-00010d10: 7420 6372 6561 7469 6f6e 2074 696d 6573  t creation times
-00010d20: 7461 6d70 2069 6e74 6f20 4461 7465 5469  tamp into DateTi
-00010d30: 6d65 206f 626a 6563 740d 0a20 2064 745f  me object..  dt_
-00010d40: 6320 3d20 6461 7465 7469 6d65 2e64 6174  c = datetime.dat
-00010d50: 6574 696d 652e 6672 6f6d 7469 6d65 7374  etime.fromtimest
-00010d60: 616d 7028 635f 7469 6d65 290d 0a20 2063  amp(c_time)..  c
-00010d70: 6f20 3d20 7374 7228 6474 5f63 2920 5b30  o = str(dt_c) [0
-00010d80: 3a31 395d 0d0a 2020 6d6f 203d 2073 7472  :19]..  mo = str
-00010d90: 2864 745f 6d29 205b 303a 3139 5d0d 0a0d  (dt_m) [0:19]...
-00010da0: 0a20 2070 203d 204d 7950 6172 7365 7228  .  p = MyParser(
-00010db0: 6669 6c65 6e61 6d65 290d 0a20 2074 6865  filename)..  the
-00010dc0: 7465 7874 3d27 5c6e 272e 6a6f 696e 2870  text='\n'.join(p
-00010dd0: 2e72 6563 6f72 6473 290d 0a20 2061 7274  .records)..  art
-00010de0: 6963 6c65 5f74 6578 743d 7468 6574 6578  icle_text=thetex
-00010df0: 742e 656e 636f 6465 2827 7574 6638 2729  t.encode('utf8')
-00010e00: 0d0a 2020 7375 6d6d 6172 697a 6564 3d22  ..  summarized="
-00010e10: 7b5c 2266 696c 656e 616d 655c 223a 5c22  {\"filename\":\"
-00010e20: 2220 2b20 6669 6c65 6e61 6d65 202b 2022  " + filename + "
-00010e30: 5c22 2c5c 2266 696c 6573 697a 6528 4d42  \",\"filesize(MB
-00010e40: 295c 223a 222b 7374 7228 7468 6573 697a  )\":"+str(thesiz
-00010e50: 6529 2b22 2c5c 2266 696c 6563 7265 6174  e)+",\"filecreat
-00010e60: 6564 6f6e 5c22 3a5c 2222 202b 2063 6f20  edon\":\"" + co 
-00010e70: 2b20 225c 222c 5c22 6669 6c65 6d6f 6469  + "\",\"filemodi
-00010e80: 6669 6564 6f6e 5c22 3a5c 2222 202b 206d  fiedon\":\"" + m
-00010e90: 6f20 2b20 225c 222c 5c22 6b65 7977 6f72  o + "\",\"keywor
-00010ea0: 6473 5c22 3a22 202b 2020 7374 6172 7473  ds\":" +  starts
-00010eb0: 756d 6d61 7279 2874 6865 7465 7874 2c66  ummary(thetext,f
-00010ec0: 7661 6c75 652c 6b65 7963 6f75 6e74 290d  value,keycount).
-00010ed0: 0a20 2320 7072 696e 7428 7375 6d6d 6172  . # print(summar
-00010ee0: 697a 6564 290d 0a20 2072 6574 7572 6e20  ized)..  return 
-00010ef0: 7375 6d6d 6172 697a 6564 0d0a 0d0a 0d0a  summarized......
-00010f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010f10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010f20: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-00010f30: 0a23 2044 6576 656c 6f70 6564 2062 7920  .# Developed by 
-00010f40: 4f54 4943 5320 4164 7661 6e63 6564 2041  OTICS Advanced A
-00010f50: 6e61 6c79 7469 6373 0d0a 2320 5365 6261  nalytics..# Seba
-00010f60: 7374 6961 6e20 4d61 7572 6963 650d 0a0d  stian Maurice...
-00010f70: 0a69 6d70 6f72 7420 6273 3420 6173 2062  .import bs4 as b
-00010f80: 7320 200d 0a69 6d70 6f72 7420 7572 6c6c  s  ..import urll
-00010f90: 6962 2e72 6571 7565 7374 2020 0d0a 696d  ib.request  ..im
-00010fa0: 706f 7274 2072 650d 0a69 6d70 6f72 7420  port re..import 
-00010fb0: 6e6c 746b 0d0a 6672 6f6d 206e 6c74 6b2e  nltk..from nltk.
-00010fc0: 746f 6b65 6e69 7a65 2069 6d70 6f72 7420  tokenize import 
-00010fd0: 5265 6765 7870 546f 6b65 6e69 7a65 720d  RegexpTokenizer.
-00010fe0: 0a69 6d70 6f72 7420 6865 6170 710d 0a69  .import heapq..i
-00010ff0: 6d70 6f72 7420 7379 730d 0a69 6d70 6f72  mport sys..impor
-00011000: 7420 6f73 0d0a 6672 6f6d 2072 616b 655f  t os..from rake_
-00011010: 6e6c 746b 2069 6d70 6f72 7420 4d65 7472  nltk import Metr
-00011020: 6963 2c52 616b 650d 0a69 6d70 6f72 7420  ic,Rake..import 
-00011030: 6a73 6f6e 0d0a 696d 706f 7274 2070 616e  json..import pan
-00011040: 6461 7320 6173 2070 640d 0a69 6d70 6f72  das as pd..impor
-00011050: 7420 6e6c 746b 2e63 6f72 7075 730d 0a66  t nltk.corpus..f
-00011060: 726f 6d20 6e6c 746b 2e63 6f72 7075 7320  rom nltk.corpus 
-00011070: 696d 706f 7274 2073 746f 7077 6f72 6473  import stopwords
-00011080: 0d0a 6672 6f6d 2074 6578 7462 6c6f 6220  ..from textblob 
-00011090: 696d 706f 7274 2054 6578 7442 6c6f 620d  import TextBlob.
-000110a0: 0a66 726f 6d20 7465 7874 626c 6f62 2069  .from textblob i
-000110b0: 6d70 6f72 7420 576f 7264 0d0a 6672 6f6d  mport Word..from
-000110c0: 2073 6b6c 6561 726e 2e66 6561 7475 7265   sklearn.feature
-000110d0: 5f65 7874 7261 6374 696f 6e2e 7465 7874  _extraction.text
-000110e0: 2069 6d70 6f72 7420 5466 6964 6654 7261   import TfidfTra
-000110f0: 6e73 666f 726d 6572 2c54 6669 6466 5665  nsformer,TfidfVe
-00011100: 6374 6f72 697a 6572 0d0a 6672 6f6d 2073  ctorizer..from s
-00011110: 6b6c 6561 726e 2e66 6561 7475 7265 5f65  klearn.feature_e
-00011120: 7874 7261 6374 696f 6e2e 7465 7874 2069  xtraction.text i
-00011130: 6d70 6f72 7420 436f 756e 7456 6563 746f  mport CountVecto
-00011140: 7269 7a65 720d 0a23 6e6c 746b 2e64 6f77  rizer..#nltk.dow
-00011150: 6e6c 6f61 6428 2770 756e 6b74 2729 0d0a  nload('punkt')..
-00011160: 696d 706f 7274 2077 6172 6e69 6e67 730d  import warnings.
-00011170: 0a77 6172 6e69 6e67 732e 6669 6c74 6572  .warnings.filter
-00011180: 7761 726e 696e 6773 2822 6967 6e6f 7265  warnings("ignore
-00011190: 2229 0d0a 0d0a 236e 6c74 6b2e 646f 776e  ")....#nltk.down
-000111a0: 6c6f 6164 2827 7374 6f70 776f 7264 7327  load('stopwords'
-000111b0: 290d 0a0d 0a64 6566 2067 6574 5f73 746f  )....def get_sto
-000111c0: 705f 776f 7264 7328 293a 0d0a 2020 2020  p_words():..    
-000111d0: 2222 226c 6f61 6420 7374 6f70 2077 6f72  """load stop wor
-000111e0: 6473 2022 2222 0d0a 2020 2020 7265 7475  ds """..    retu
-000111f0: 726e 2073 746f 7077 6f72 6473 2e77 6f72  rn stopwords.wor
-00011200: 6473 2827 656e 676c 6973 6827 290d 0a20  ds('english').. 
-00011210: 2020 200d 0a23 2320 2020 2077 6974 6820     ..##    with 
-00011220: 6f70 656e 2827 7374 6f70 776f 7264 732e  open('stopwords.
-00011230: 7478 7427 2c20 2772 272c 2065 6e63 6f64  txt', 'r', encod
-00011240: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
-00011250: 663a 0d0a 2323 2020 2020 2020 2020 7374  f:..##        st
-00011260: 6f70 776f 7264 7320 3d20 662e 7265 6164  opwords = f.read
-00011270: 6c69 6e65 7328 290d 0a23 2320 2020 2020  lines()..##     
-00011280: 2020 2073 746f 705f 7365 7420 3d20 7365     stop_set = se
-00011290: 7428 6d2e 7374 7269 7028 2920 666f 7220  t(m.strip() for 
-000112a0: 6d20 696e 2073 746f 7077 6f72 6473 290d  m in stopwords).
-000112b0: 0a23 2320 2020 2020 2023 2020 7072 696e  .##      #  prin
-000112c0: 7428 6672 6f7a 656e 7365 7428 7374 6f70  t(frozenset(stop
-000112d0: 5f73 6574 2929 0d0a 2323 2020 2020 2020  _set))..##      
-000112e0: 2020 7265 7475 726e 2066 726f 7a65 6e73    return frozens
-000112f0: 6574 2873 746f 705f 7365 7429 0d0a 0d0a  et(stop_set)....
-00011300: 6465 6620 7363 7261 7065 7765 6228 7468  def scrapeweb(th
-00011310: 6575 726c 293a 0d0a 2020 2020 7363 7261  eurl):..    scra
-00011320: 7065 645f 6461 7461 203d 2075 726c 6c69  ped_data = urlli
-00011330: 622e 7265 7175 6573 742e 7572 6c6f 7065  b.request.urlope
-00011340: 6e28 7468 6575 726c 2920 200d 0a20 2020  n(theurl)  ..   
-00011350: 2061 7274 6963 6c65 203d 2073 6372 6170   article = scrap
-00011360: 6564 5f64 6174 612e 7265 6164 2829 0d0a  ed_data.read()..
-00011370: 0d0a 2020 2020 7061 7273 6564 5f61 7274  ..    parsed_art
-00011380: 6963 6c65 203d 2062 732e 4265 6175 7469  icle = bs.Beauti
-00011390: 6675 6c53 6f75 7028 6172 7469 636c 652c  fulSoup(article,
-000113a0: 276c 786d 6c27 290d 0a0d 0a20 2020 2070  'lxml')....    p
-000113b0: 6172 6167 7261 7068 7320 3d20 7061 7273  aragraphs = pars
-000113c0: 6564 5f61 7274 6963 6c65 2e66 696e 645f  ed_article.find_
-000113d0: 616c 6c28 2770 2729 0d0a 0d0a 2020 2020  all('p')....    
-000113e0: 6172 7469 636c 655f 7465 7874 203d 2022  article_text = "
-000113f0: 220d 0a0d 0a20 2020 2066 6f72 2070 2069  "....    for p i
-00011400: 6e20 7061 7261 6772 6170 6873 3a20 200d  n paragraphs:  .
-00011410: 0a20 2020 2020 2020 2061 7274 6963 6c65  .        article
-00011420: 5f74 6578 7420 2b3d 2070 2e74 6578 740d  _text += p.text.
-00011430: 0a20 2020 2072 6574 7572 6e20 6172 7469  .    return arti
-00011440: 636c 655f 7465 7874 200d 0a0d 0a64 6566  cle_text ....def
-00011450: 2063 6f6e 7665 7274 746f 6c6f 7765 7263   converttolowerc
-00011460: 6173 6528 6466 2c63 6f6c 293a 0d0a 2020  ase(df,col):..  
-00011470: 2020 2020 6466 5b63 6f6c 5d20 3d20 6466      df[col] = df
-00011480: 5b63 6f6c 5d2e 6170 706c 7928 6c61 6d62  [col].apply(lamb
-00011490: 6461 2078 3a20 2220 222e 6a6f 696e 2878  da x: " ".join(x
-000114a0: 2e6c 6f77 6572 2829 2066 6f72 2078 2069  .lower() for x i
-000114b0: 6e20 782e 7370 6c69 7428 2929 290d 0a20  n x.split())).. 
-000114c0: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
-000114d0: 2020 2020 0d0a 6465 6620 7265 6d6f 7665      ..def remove
-000114e0: 7075 6e63 7475 6174 696f 6e28 6466 2c63  punctuation(df,c
-000114f0: 6f6c 293a 0d0a 2020 2020 2020 6466 5b63  ol):..      df[c
-00011500: 6f6c 5d20 3d20 6466 5b63 6f6c 5d2e 7374  ol] = df[col].st
-00011510: 722e 7265 706c 6163 6528 275b 5e5c 775c  r.replace('[^\w\
-00011520: 735d 272c 2727 290d 0a20 2020 2020 2072  s]','')..      r
-00011530: 6574 7572 6e20 6466 0d0a 0d0a 6465 6620  eturn df....def 
-00011540: 7265 6d6f 7665 7374 6f70 776f 7264 7328  removestopwords(
-00011550: 6466 2c63 6f6c 293a 0d0a 2020 2020 2020  df,col):..      
-00011560: 7374 6f70 203d 2073 746f 7077 6f72 6473  stop = stopwords
-00011570: 2e77 6f72 6473 2827 656e 676c 6973 6827  .words('english'
-00011580: 290d 0a20 2020 2020 2064 665b 636f 6c5d  )..      df[col]
-00011590: 203d 2064 665b 636f 6c5d 2e61 7070 6c79   = df[col].apply
-000115a0: 286c 616d 6264 6120 783a 2022 2022 2e6a  (lambda x: " ".j
-000115b0: 6f69 6e28 7820 666f 7220 7820 696e 2078  oin(x for x in x
-000115c0: 2e73 706c 6974 2829 2069 6620 7820 6e6f  .split() if x no
-000115d0: 7420 696e 2073 746f 7029 290d 0a20 2020  t in stop))..   
-000115e0: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
-000115f0: 6465 6620 7265 6d6f 7665 636f 6d6d 6f6e  def removecommon
-00011600: 776f 7264 7328 6466 2c63 6f6c 293a 0d0a  words(df,col):..
-00011610: 2020 2020 2020 6672 6571 203d 2070 642e        freq = pd.
-00011620: 5365 7269 6573 2827 2027 2e6a 6f69 6e28  Series(' '.join(
-00011630: 6466 5b63 6f6c 5d29 2e73 706c 6974 2829  df[col]).split()
-00011640: 292e 7661 6c75 655f 636f 756e 7473 2829  ).value_counts()
-00011650: 5b3a 3130 5d0d 0a20 2020 2020 2066 7265  [:10]..      fre
-00011660: 7120 3d20 6c69 7374 2866 7265 712e 696e  q = list(freq.in
-00011670: 6465 7829 0d0a 2020 2020 2020 6466 5b63  dex)..      df[c
-00011680: 6f6c 5d20 3d20 6466 5b63 6f6c 5d2e 6170  ol] = df[col].ap
-00011690: 706c 7928 6c61 6d62 6461 2078 3a20 2220  ply(lambda x: " 
-000116a0: 222e 6a6f 696e 2878 2066 6f72 2078 2069  ".join(x for x i
-000116b0: 6e20 782e 7370 6c69 7428 2920 6966 2078  n x.split() if x
-000116c0: 206e 6f74 2069 6e20 6672 6571 2929 0d0a   not in freq))..
-000116d0: 2020 2020 2020 7265 7475 726e 2064 660d        return df.
-000116e0: 0a0d 0a64 6566 2072 656d 6f76 6572 6172  ...def removerar
-000116f0: 6577 6f72 6473 2864 662c 636f 6c29 3a0d  ewords(df,col):.
-00011700: 0a20 2020 2020 2066 7265 7120 3d20 7064  .      freq = pd
-00011710: 2e53 6572 6965 7328 2720 272e 6a6f 696e  .Series(' '.join
-00011720: 2864 665b 636f 6c5d 292e 7370 6c69 7428  (df[col]).split(
-00011730: 2929 2e76 616c 7565 5f63 6f75 6e74 7328  )).value_counts(
-00011740: 295b 2d31 303a 5d0d 0a20 2020 2020 2066  )[-10:]..      f
-00011750: 7265 7120 3d20 6c69 7374 2866 7265 712e  req = list(freq.
-00011760: 696e 6465 7829 0d0a 2020 2020 2020 6466  index)..      df
-00011770: 5b63 6f6c 5d20 3d20 6466 5b63 6f6c 5d2e  [col] = df[col].
-00011780: 6170 706c 7928 6c61 6d62 6461 2078 3a20  apply(lambda x: 
-00011790: 2220 222e 6a6f 696e 2878 2066 6f72 2078  " ".join(x for x
-000117a0: 2069 6e20 782e 7370 6c69 7428 2920 6966   in x.split() if
-000117b0: 2078 206e 6f74 2069 6e20 6672 6571 2929   x not in freq))
-000117c0: 0d0a 2020 2020 2020 7265 7475 726e 2064  ..      return d
-000117d0: 660d 0a0d 0a64 6566 2063 6f72 7265 6374  f....def correct
-000117e0: 7370 656c 6c69 6e67 2864 662c 636f 6c29  spelling(df,col)
-000117f0: 3a0d 0a20 2020 2020 2064 665b 636f 6c5d  :..      df[col]
-00011800: 5b3a 355d 2e61 7070 6c79 286c 616d 6264  [:5].apply(lambd
-00011810: 6120 783a 2073 7472 2854 6578 7442 6c6f  a x: str(TextBlo
-00011820: 6228 7829 2e63 6f72 7265 6374 2829 2929  b(x).correct()))
-00011830: 0d0a 2020 2020 2020 7265 7475 726e 2064  ..      return d
-00011840: 660d 0a0d 0a64 6566 206c 656d 6d61 7469  f....def lemmati
-00011850: 7a61 7469 6f6e 2864 662c 636f 6c29 3a0d  zation(df,col):.
-00011860: 0a20 2020 2020 2064 665b 636f 6c5d 203d  .      df[col] =
-00011870: 2064 665b 636f 6c5d 2e61 7070 6c79 286c   df[col].apply(l
-00011880: 616d 6264 6120 783a 2022 2022 2e6a 6f69  ambda x: " ".joi
-00011890: 6e28 5b57 6f72 6428 776f 7264 292e 6c65  n([Word(word).le
-000118a0: 6d6d 6174 697a 6528 2920 666f 7220 776f  mmatize() for wo
-000118b0: 7264 2069 6e20 782e 7370 6c69 7428 295d  rd in x.split()]
-000118c0: 2929 0d0a 2020 2020 2020 7265 7475 726e  ))..      return
-000118d0: 2064 660d 0a0d 0a64 6566 2074 7261 696e   df....def train
-000118e0: 7665 6374 2863 762c 7462 6f77 2c64 662c  vect(cv,tbow,df,
-000118f0: 636f 6c2c 6d61 786b 6579 776f 7264 7329  col,maxkeywords)
-00011900: 3a0d 0a20 2020 2020 2074 6578 743d 6466  :..      text=df
-00011910: 5b63 6f6c 5d2e 746f 6c69 7374 2829 0d0a  [col].tolist()..
-00011920: 2020 2020 2020 7466 6964 6620 3d20 5466        tfidf = Tf
-00011930: 6964 6654 7261 6e73 666f 726d 6572 2873  idfTransformer(s
-00011940: 6d6f 6f74 685f 6964 663d 5472 7565 2c75  mooth_idf=True,u
-00011950: 7365 5f69 6466 3d54 7275 6529 0d0a 2020  se_idf=True)..  
-00011960: 2020 2020 7466 6964 662e 6669 7428 7462      tfidf.fit(tb
-00011970: 6f77 290d 0a20 2020 2020 2074 665f 6964  ow)..      tf_id
-00011980: 665f 7665 6374 6f72 3d74 6669 6466 2e74  f_vector=tfidf.t
-00011990: 7261 6e73 666f 726d 2863 762e 7472 616e  ransform(cv.tran
-000119a0: 7366 6f72 6d28 7465 7874 2929 0d0a 2020  sform(text))..  
-000119b0: 2020 2020 736f 7274 6564 6974 656d 733d      sorteditems=
-000119c0: 736f 7274 5f63 6f6f 2874 665f 6964 665f  sort_coo(tf_idf_
-000119d0: 7665 6374 6f72 2e74 6f63 6f6f 2829 290d  vector.tocoo()).
-000119e0: 0a20 2020 2020 2066 6561 7475 7265 6e61  .      featurena
-000119f0: 6d65 733d 6376 2e67 6574 5f66 6561 7475  mes=cv.get_featu
-00011a00: 7265 5f6e 616d 6573 5f6f 7574 2829 0d0a  re_names_out()..
-00011a10: 2020 2020 2020 6b65 7977 6f72 6473 3d65        keywords=e
-00011a20: 7874 7261 6374 5f74 6f70 6e5f 6672 6f6d  xtract_topn_from
-00011a30: 5f76 6563 746f 7228 6665 6174 7572 656e  _vector(featuren
-00011a40: 616d 6573 2c73 6f72 7465 6469 7465 6d73  ames,sorteditems
-00011a50: 2c6d 6178 6b65 7977 6f72 6473 290d 0a20  ,maxkeywords).. 
-00011a60: 2020 2020 206b 6579 776f 7264 733d 6a73       keywords=js
-00011a70: 6f6e 2e64 756d 7073 286b 6579 776f 7264  on.dumps(keyword
-00011a80: 7329 0d0a 2020 2020 2023 2070 7269 6e74  s)..     # print
-00011a90: 286b 6579 776f 7264 7329 0d0a 2020 2020  (keywords)..    
-00011aa0: 2020 7265 7475 726e 206b 6579 776f 7264    return keyword
-00011ab0: 730d 0a0d 0a64 6566 2074 7261 696e 626f  s....def trainbo
-00011ac0: 7728 6466 2c63 6f6c 293a 0d0a 2020 2020  w(df,col):..    
-00011ad0: 2020 6d79 6c69 7374 3d64 665b 636f 6c5d    mylist=df[col]
-00011ae0: 2e74 6f6c 6973 7428 290d 0a20 2020 2020  .tolist()..     
-00011af0: 2073 746f 7077 6f72 6473 3d67 6574 5f73   stopwords=get_s
-00011b00: 746f 705f 776f 7264 7328 290d 0a20 2020  top_words()..   
-00011b10: 2020 2063 7620 3d20 436f 756e 7456 6563     cv = CountVec
-00011b20: 746f 7269 7a65 7228 7374 6f70 5f77 6f72  torizer(stop_wor
-00011b30: 6473 3d73 746f 7077 6f72 6473 290d 0a20  ds=stopwords).. 
-00011b40: 2020 2020 2074 7261 696e 5f62 6f77 203d       train_bow =
-00011b50: 2063 762e 6669 745f 7472 616e 7366 6f72   cv.fit_transfor
-00011b60: 6d28 6d79 6c69 7374 290d 0a20 2020 2020  m(mylist)..     
-00011b70: 2023 7072 696e 7428 6c69 7374 2863 762e   #print(list(cv.
-00011b80: 766f 6361 6275 6c61 7279 5f2e 6b65 7973  vocabulary_.keys
-00011b90: 2829 2929 0d0a 2020 2020 2020 7265 7475  ()))..      retu
-00011ba0: 726e 2063 762c 7472 6169 6e5f 626f 770d  rn cv,train_bow.
-00011bb0: 0a0d 0a20 0d0a 6465 6620 736f 7274 5f63  ... ..def sort_c
-00011bc0: 6f6f 2863 6f6f 5f6d 6174 7269 7829 3a0d  oo(coo_matrix):.
-00011bd0: 0a20 2020 2074 7570 6c65 7320 3d20 7a69  .    tuples = zi
-00011be0: 7028 636f 6f5f 6d61 7472 6978 2e63 6f6c  p(coo_matrix.col
-00011bf0: 2c20 636f 6f5f 6d61 7472 6978 2e64 6174  , coo_matrix.dat
-00011c00: 6129 0d0a 2020 2020 7265 7475 726e 2073  a)..    return s
-00011c10: 6f72 7465 6428 7475 706c 6573 2c20 6b65  orted(tuples, ke
-00011c20: 793d 6c61 6d62 6461 2078 3a20 2878 5b31  y=lambda x: (x[1
-00011c30: 5d2c 2078 5b30 5d29 2c20 7265 7665 7273  ], x[0]), revers
-00011c40: 653d 5472 7565 290d 0a0d 0a64 6566 2065  e=True)....def e
-00011c50: 7874 7261 6374 5f74 6f70 6e5f 6672 6f6d  xtract_topn_from
-00011c60: 5f76 6563 746f 7228 6665 6174 7572 655f  _vector(feature_
-00011c70: 6e61 6d65 732c 2073 6f72 7465 645f 6974  names, sorted_it
-00011c80: 656d 732c 2074 6f70 6e3d 3130 293a 0d0a  ems, topn=10):..
-00011c90: 2020 2020 2222 2267 6574 2074 6865 2066      """get the f
-00011ca0: 6561 7475 7265 206e 616d 6573 2061 6e64  eature names and
-00011cb0: 2074 662d 6964 6620 7363 6f72 6520 6f66   tf-idf score of
-00011cc0: 2074 6f70 206e 2069 7465 6d73 2222 220d   top n items""".
-00011cd0: 0a20 2020 200d 0a20 2020 2023 7573 6520  .    ..    #use 
-00011ce0: 6f6e 6c79 2074 6f70 6e20 6974 656d 7320  only topn items 
-00011cf0: 6672 6f6d 2076 6563 746f 720d 0a20 2020  from vector..   
-00011d00: 2073 6f72 7465 645f 6974 656d 7320 3d20   sorted_items = 
-00011d10: 736f 7274 6564 5f69 7465 6d73 5b3a 746f  sorted_items[:to
-00011d20: 706e 5d0d 0a0d 0a20 2020 2073 636f 7265  pn]....    score
-00011d30: 5f76 616c 7320 3d20 5b5d 0d0a 2020 2020  _vals = []..    
-00011d40: 6665 6174 7572 655f 7661 6c73 203d 205b  feature_vals = [
-00011d50: 5d0d 0a0d 0a20 2020 2066 6f72 2069 6478  ]....    for idx
-00011d60: 2c20 7363 6f72 6520 696e 2073 6f72 7465  , score in sorte
-00011d70: 645f 6974 656d 733a 2020 2020 2020 2020  d_items:        
-00011d80: 0d0a 2020 2020 2020 2020 2020 666e 616d  ..          fnam
-00011d90: 6520 3d20 6665 6174 7572 655f 6e61 6d65  e = feature_name
-00011da0: 735b 6964 785d 0d0a 2020 2020 2020 2020  s[idx]..        
-00011db0: 2020 6966 206c 656e 2866 6e61 6d65 293e    if len(fname)>
-00011dc0: 333a 0d0a 2020 2020 2020 2020 236b 6565  3:..        #kee
-00011dd0: 7020 7472 6163 6b20 6f66 2066 6561 7475  p track of featu
-00011de0: 7265 206e 616d 6520 616e 6420 6974 7320  re name and its 
-00011df0: 636f 7272 6573 706f 6e64 696e 6720 7363  corresponding sc
-00011e00: 6f72 650d 0a20 2020 2020 2020 2020 2020  ore..           
-00011e10: 2073 636f 7265 5f76 616c 732e 6170 7065   score_vals.appe
-00011e20: 6e64 2872 6f75 6e64 2873 636f 7265 2c20  nd(round(score, 
-00011e30: 3329 290d 0a20 2020 2020 2020 2020 2020  3))..           
-00011e40: 2066 6561 7475 7265 5f76 616c 732e 6170   feature_vals.ap
-00011e50: 7065 6e64 2866 6561 7475 7265 5f6e 616d  pend(feature_nam
-00011e60: 6573 5b69 6478 5d29 0d0a 0d0a 2020 2020  es[idx])....    
-00011e70: 2363 7265 6174 6520 6120 7475 706c 6573  #create a tuples
-00011e80: 206f 6620 6665 6174 7572 652c 7363 6f72   of feature,scor
-00011e90: 650d 0a20 2020 2023 7265 7375 6c74 7320  e..    #results 
-00011ea0: 3d20 7a69 7028 6665 6174 7572 655f 7661  = zip(feature_va
-00011eb0: 6c73 2c73 636f 7265 5f76 616c 7329 0d0a  ls,score_vals)..
-00011ec0: 2020 2020 7265 7375 6c74 733d 207b 7d0d      results= {}.
-00011ed0: 0a20 2020 2066 6f72 2069 6478 2069 6e20  .    for idx in 
-00011ee0: 7261 6e67 6528 6c65 6e28 6665 6174 7572  range(len(featur
-00011ef0: 655f 7661 6c73 2929 3a0d 0a20 2020 2020  e_vals)):..     
-00011f00: 2020 2072 6573 756c 7473 5b66 6561 7475     results[featu
-00011f10: 7265 5f76 616c 735b 6964 785d 5d3d 7363  re_vals[idx]]=sc
-00011f20: 6f72 655f 7661 6c73 5b69 6478 5d0d 0a20  ore_vals[idx].. 
-00011f30: 2020 200d 0a20 2020 2072 6574 7572 6e20     ..    return 
-00011f40: 7265 7375 6c74 730d 0a0d 0a64 6566 2067  results....def g
-00011f50: 6574 6b65 7977 6f72 6473 286d 7974 6578  etkeywords(mytex
-00011f60: 742c 6d61 786b 6579 776f 7264 7329 3a0d  t,maxkeywords):.
-00011f70: 0a20 2020 2072 3d52 616b 6528 6d61 785f  .    r=Rake(max_
-00011f80: 6c65 6e67 7468 3d31 3029 0d0a 2020 2020  length=10)..    
-00011f90: 7220 3d20 5261 6b65 2872 616e 6b69 6e67  r = Rake(ranking
-00011fa0: 5f6d 6574 7269 633d 4d65 7472 6963 2e44  _metric=Metric.D
-00011fb0: 4547 5245 455f 544f 5f46 5245 5155 454e  EGREE_TO_FREQUEN
-00011fc0: 4359 5f52 4154 494f 290d 0a20 2020 2023  CY_RATIO)..    #
-00011fd0: 7220 3d20 5261 6b65 2872 616e 6b69 6e67  r = Rake(ranking
-00011fe0: 5f6d 6574 7269 633d 4d65 7472 6963 2e57  _metric=Metric.W
-00011ff0: 4f52 445f 4445 4752 4545 290d 0a20 2020  ORD_DEGREE)..   
-00012000: 2023 7220 3d20 5261 6b65 2872 616e 6b69   #r = Rake(ranki
-00012010: 6e67 5f6d 6574 7269 633d 4d65 7472 6963  ng_metric=Metric
-00012020: 2e57 4f52 445f 4652 4551 5545 4e43 5929  .WORD_FREQUENCY)
-00012030: 0d0a 2020 2020 643d 7b27 696e 7075 7427  ..    d={'input'
-00012040: 3a5b 6d79 7465 7874 5d7d 0d0a 2020 2020  :[mytext]}..    
-00012050: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
-00012060: 6528 6429 0d0a 2020 2020 6466 3d63 6f6e  e(d)..    df=con
-00012070: 7665 7274 746f 6c6f 7765 7263 6173 6528  verttolowercase(
-00012080: 6466 2c27 696e 7075 7427 290d 0a20 2020  df,'input')..   
-00012090: 2064 663d 7265 6d6f 7665 7075 6e63 7475   df=removepunctu
-000120a0: 6174 696f 6e28 6466 2c27 696e 7075 7427  ation(df,'input'
-000120b0: 290d 0a20 2020 2064 663d 7265 6d6f 7665  )..    df=remove
-000120c0: 7374 6f70 776f 7264 7328 6466 2c27 696e  stopwords(df,'in
-000120d0: 7075 7427 290d 0a20 2020 2064 663d 7265  put')..    df=re
-000120e0: 6d6f 7665 636f 6d6d 6f6e 776f 7264 7328  movecommonwords(
-000120f0: 6466 2c27 696e 7075 7427 290d 0a20 2020  df,'input')..   
-00012100: 2064 663d 7265 6d6f 7665 7261 7265 776f   df=removerarewo
-00012110: 7264 7328 6466 2c27 696e 7075 7427 290d  rds(df,'input').
-00012120: 0a20 2020 2064 663d 636f 7272 6563 7473  .    df=corrects
-00012130: 7065 6c6c 696e 6728 6466 2c27 696e 7075  pelling(df,'inpu
-00012140: 7427 290d 0a20 2020 2064 663d 6c65 6d6d  t')..    df=lemm
-00012150: 6174 697a 6174 696f 6e28 6466 2c27 696e  atization(df,'in
-00012160: 7075 7427 290d 0a20 2020 206d 7974 6578  put')..    mytex
-00012170: 743d 6466 5b27 696e 7075 7427 5d5b 305d  t=df['input'][0]
-00012180: 0d0a 2020 2020 6376 2c74 773d 7472 6169  ..    cv,tw=trai
-00012190: 6e62 6f77 2864 662c 2769 6e70 7574 2729  nbow(df,'input')
-000121a0: 0d0a 2020 2020 6b65 7977 6f72 6473 3d74  ..    keywords=t
-000121b0: 7261 696e 7665 6374 2863 762c 7477 2c64  rainvect(cv,tw,d
-000121c0: 662c 2769 6e70 7574 272c 6d61 786b 6579  f,'input',maxkey
-000121d0: 776f 7264 7329 0d0a 0d0a 2020 2020 0d0a  words)....    ..
-000121e0: 2020 2020 6b65 7962 7566 203d 2022 220d      keybuf = "".
-000121f0: 0a20 2020 206b 6a73 6f6e 203d 206a 736f  .    kjson = jso
-00012200: 6e2e 6c6f 6164 7328 6b65 7977 6f72 6473  n.loads(keywords
-00012210: 290d 0a20 2020 2066 6f72 206b 6579 2c20  )..    for key, 
-00012220: 7661 6c75 6520 696e 206b 6a73 6f6e 2e69  value in kjson.i
-00012230: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00012240: 206b 6579 6275 6620 3d20 6b65 7962 7566   keybuf = keybuf
-00012250: 202b 206b 6579 202b 222c 2220 2b20 7374   + key +"," + st
-00012260: 7228 7661 6c75 6529 202b 2022 3a22 0d0a  r(value) + ":"..
-00012270: 2020 2020 6b65 7962 7566 203d 206b 6579      keybuf = key
-00012280: 6275 665b 3a2d 315d 0d0a 0d0a 2020 2020  buf[:-1]....    
-00012290: 7265 7475 726e 206b 6579 6275 660d 0a20  return keybuf.. 
-000122a0: 0d0a 6465 6620 646f 7375 6d6d 6172 7928  ..def dosummary(
-000122b0: 6172 7469 636c 655f 7465 7874 2c69 293a  article_text,i):
-000122c0: 0d0a 0d0a 0d0a 2020 2020 6172 7469 636c  ......    articl
-000122d0: 655f 7465 7874 203d 2072 652e 7375 6228  e_text = re.sub(
-000122e0: 7227 5c5b 5b30 2d39 5d2a 5c5d 272c 2027  r'\[[0-9]*\]', '
-000122f0: 2027 2c20 6172 7469 636c 655f 7465 7874   ', article_text
-00012300: 2920 200d 0a20 2020 2061 7274 6963 6c65  )  ..    article
-00012310: 5f74 6578 7420 3d20 7265 2e73 7562 2872  _text = re.sub(r
-00012320: 275c 732b 272c 2027 2027 2c20 6172 7469  '\s+', ' ', arti
-00012330: 636c 655f 7465 7874 290d 0a0d 0a20 2020  cle_text)....   
-00012340: 2023 2052 656d 6f76 696e 6720 7370 6563   # Removing spec
-00012350: 6961 6c20 6368 6172 6163 7465 7273 2061  ial characters a
-00012360: 6e64 2064 6967 6974 730d 0a20 2020 2066  nd digits..    f
-00012370: 6f72 6d61 7474 6564 5f61 7274 6963 6c65  ormatted_article
-00012380: 5f74 6578 7420 3d20 7265 2e73 7562 2827  _text = re.sub('
-00012390: 5b5e 612d 7a41 2d5a 5d27 2c20 2720 272c  [^a-zA-Z]', ' ',
-000123a0: 2061 7274 6963 6c65 5f74 6578 7420 2920   article_text ) 
-000123b0: 200d 0a20 2020 2066 6f72 6d61 7474 6564   ..    formatted
-000123c0: 5f61 7274 6963 6c65 5f74 6578 7420 3d20  _article_text = 
-000123d0: 7265 2e73 7562 2872 275c 732b 272c 2027  re.sub(r'\s+', '
-000123e0: 2027 2c20 666f 726d 6174 7465 645f 6172   ', formatted_ar
-000123f0: 7469 636c 655f 7465 7874 2920 200d 0a0d  ticle_text)  ...
-00012400: 0a20 2020 2073 656e 7465 6e63 655f 6c69  .    sentence_li
-00012410: 7374 203d 206e 6c74 6b2e 7365 6e74 5f74  st = nltk.sent_t
-00012420: 6f6b 656e 697a 6528 6172 7469 636c 655f  okenize(article_
-00012430: 7465 7874 2920 200d 0a20 2020 2023 7072  text)  ..    #pr
-00012440: 696e 7428 7365 6e74 656e 6365 5f6c 6973  int(sentence_lis
-00012450: 7429 0d0a 0d0a 2020 2020 7374 6f70 776f  t)....    stopwo
-00012460: 7264 7320 3d20 6e6c 746b 2e63 6f72 7075  rds = nltk.corpu
-00012470: 732e 7374 6f70 776f 7264 732e 776f 7264  s.stopwords.word
-00012480: 7328 2765 6e67 6c69 7368 2729 0d0a 0d0a  s('english')....
-00012490: 2020 2020 776f 7264 5f66 7265 7175 656e      word_frequen
-000124a0: 6369 6573 203d 207b 7d20 200d 0a20 2020  cies = {}  ..   
-000124b0: 2066 6f72 2077 6f72 6420 696e 206e 6c74   for word in nlt
-000124c0: 6b2e 776f 7264 5f74 6f6b 656e 697a 6528  k.word_tokenize(
-000124d0: 666f 726d 6174 7465 645f 6172 7469 636c  formatted_articl
-000124e0: 655f 7465 7874 293a 2020 0d0a 2020 2020  e_text):  ..    
-000124f0: 2020 2020 6966 2077 6f72 6420 6e6f 7420      if word not 
-00012500: 696e 2073 746f 7077 6f72 6473 3a0d 0a20  in stopwords:.. 
-00012510: 2020 2020 2020 2020 2020 2069 6620 776f             if wo
-00012520: 7264 206e 6f74 2069 6e20 776f 7264 5f66  rd not in word_f
-00012530: 7265 7175 656e 6369 6573 2e6b 6579 7328  requencies.keys(
-00012540: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00012550: 2020 2020 776f 7264 5f66 7265 7175 656e      word_frequen
-00012560: 6369 6573 5b77 6f72 645d 203d 2031 0d0a  cies[word] = 1..
-00012570: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00012580: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00012590: 2020 2077 6f72 645f 6672 6571 7565 6e63     word_frequenc
-000125a0: 6965 735b 776f 7264 5d20 2b3d 2031 0d0a  ies[word] += 1..
-000125b0: 0d0a 2020 2020 6d61 7869 6d75 6d5f 6672  ..    maximum_fr
-000125c0: 6571 756e 6379 203d 206d 6178 2877 6f72  equncy = max(wor
-000125d0: 645f 6672 6571 7565 6e63 6965 732e 7661  d_frequencies.va
-000125e0: 6c75 6573 2829 290d 0a0d 0a20 2020 2066  lues())....    f
-000125f0: 6f72 2077 6f72 6420 696e 2077 6f72 645f  or word in word_
-00012600: 6672 6571 7565 6e63 6965 732e 6b65 7973  frequencies.keys
-00012610: 2829 3a20 200d 0a20 2020 2020 2020 2077  ():  ..        w
-00012620: 6f72 645f 6672 6571 7565 6e63 6965 735b  ord_frequencies[
-00012630: 776f 7264 5d20 3d20 2877 6f72 645f 6672  word] = (word_fr
-00012640: 6571 7565 6e63 6965 735b 776f 7264 5d2f  equencies[word]/
-00012650: 6d61 7869 6d75 6d5f 6672 6571 756e 6379  maximum_frequncy
-00012660: 290d 0a0d 0a20 2020 2023 7072 696e 7428  )....    #print(
-00012670: 776f 7264 5f66 7265 7175 656e 6369 6573  word_frequencies
-00012680: 290d 0a0d 0a20 2020 2073 656e 7465 6e63  )....    sentenc
-00012690: 655f 7363 6f72 6573 203d 207b 7d20 200d  e_scores = {}  .
-000126a0: 0a20 2020 2066 6f72 2073 656e 7420 696e  .    for sent in
-000126b0: 2073 656e 7465 6e63 655f 6c69 7374 3a20   sentence_list: 
-000126c0: 200d 0a20 2020 2020 2020 2066 6f72 2077   ..        for w
-000126d0: 6f72 6420 696e 206e 6c74 6b2e 776f 7264  ord in nltk.word
-000126e0: 5f74 6f6b 656e 697a 6528 7365 6e74 2e6c  _tokenize(sent.l
-000126f0: 6f77 6572 2829 293a 0d0a 2020 2020 2020  ower()):..      
-00012700: 2020 2020 2020 6966 2077 6f72 6420 696e        if word in
-00012710: 2077 6f72 645f 6672 6571 7565 6e63 6965   word_frequencie
-00012720: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
-00012730: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00012740: 6e28 7365 6e74 2e73 706c 6974 2827 2027  n(sent.split(' '
-00012750: 2929 203c 2032 353a 0d0a 2020 2020 2020  )) < 25:..      
-00012760: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012770: 2073 656e 7420 6e6f 7420 696e 2073 656e   sent not in sen
-00012780: 7465 6e63 655f 7363 6f72 6573 2e6b 6579  tence_scores.key
-00012790: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-000127a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000127b0: 6e74 656e 6365 5f73 636f 7265 735b 7365  ntence_scores[se
-000127c0: 6e74 5d20 3d20 776f 7264 5f66 7265 7175  nt] = word_frequ
-000127d0: 656e 6369 6573 5b77 6f72 645d 0d0a 2020  encies[word]..  
-000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127f0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00012800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012810: 2073 656e 7465 6e63 655f 7363 6f72 6573   sentence_scores
-00012820: 5b73 656e 745d 202b 3d20 776f 7264 5f66  [sent] += word_f
-00012830: 7265 7175 656e 6369 6573 5b77 6f72 645d  requencies[word]
-00012840: 0d0a 0d0a 2020 2020 2370 7269 6e74 2873  ....    #print(s
-00012850: 656e 7465 6e63 655f 7363 6f72 6573 290d  entence_scores).
-00012860: 0a0d 0a20 2020 2073 756d 6d61 7279 5f73  ...    summary_s
-00012870: 656e 7465 6e63 6573 203d 2068 6561 7071  entences = heapq
-00012880: 2e6e 6c61 7267 6573 7428 692c 2073 656e  .nlargest(i, sen
-00012890: 7465 6e63 655f 7363 6f72 6573 2c20 6b65  tence_scores, ke
-000128a0: 793d 7365 6e74 656e 6365 5f73 636f 7265  y=sentence_score
-000128b0: 732e 6765 7429 0d0a 2020 2020 2370 7269  s.get)..    #pri
-000128c0: 6e74 2873 756d 6d61 7279 5f73 656e 7465  nt(summary_sente
-000128d0: 6e63 6573 290d 0a20 2020 2073 756d 6d61  nces)..    summa
-000128e0: 7279 203d 2027 2027 2e6a 6f69 6e28 7375  ry = ' '.join(su
-000128f0: 6d6d 6172 795f 7365 6e74 656e 6365 7329  mmary_sentences)
-00012900: 0d0a 2020 2020 2370 7269 6e74 2822 4149  ..    #print("AI
-00012910: 2053 756d 6d61 7279 2229 0d0a 2020 2020   Summary")..    
-00012920: 7265 7475 726e 2073 756d 6d61 7279 0d0a  return summary..
-00012930: 0d0a 6465 6620 7374 6172 7473 756d 6d61  ..def startsumma
-00012940: 7279 2861 7274 6963 6c65 5f74 6578 742c  ry(article_text,
-00012950: 6676 616c 7565 2c6d 6178 6b65 7977 6f72  fvalue,maxkeywor
-00012960: 6473 293a 0d0a 2020 2020 2020 0d0a 2023  ds):..      .. #
-00012970: 2074 7279 3a0d 0a20 2020 6f72 6967 696e   try:..   origin
-00012980: 616c 776f 7264 7320 3d20 6c65 6e28 6172  alwords = len(ar
-00012990: 7469 636c 655f 7465 7874 2e73 706c 6974  ticle_text.split
-000129a0: 2822 2022 2929 0d0a 0d0a 2020 2066 6f72  (" "))....   for
-000129b0: 2069 2069 6e20 7261 6e67 6528 312c 3130   i in range(1,10
-000129c0: 3030 3029 3a0d 0a20 2020 2020 7375 6d6d  000):..     summ
-000129d0: 6172 793d 646f 7375 6d6d 6172 7928 6172  ary=dosummary(ar
-000129e0: 7469 636c 655f 7465 7874 2c69 290d 0a20  ticle_text,i).. 
-000129f0: 2020 2020 7265 7320 3d20 6c65 6e28 7375      res = len(su
-00012a00: 6d6d 6172 792e 7370 6c69 7428 2929 0d0a  mmary.split())..
-00012a10: 2020 2020 2069 6620 7265 7320 3e3d 2066       if res >= f
-00012a20: 7661 6c75 653a 0d0a 2020 2020 2020 2020  value:..        
-00012a30: 2062 7265 616b 0d0a 0d0a 2020 2073 756d   break....   sum
-00012a40: 6d61 7279 203d 2020 7265 2e73 7562 2822  mary =  re.sub("
-00012a50: 5c5c 5c5c 785b 612d 6630 2d39 5d5b 612d  \\\\x[a-f0-9][a-
-00012a60: 6630 2d39 5d22 2c20 2220 222c 7375 6d6d  f0-9]", " ",summ
-00012a70: 6172 7929 0d0a 2020 2073 756d 6d61 7279  ary)..   summary
-00012a80: 203d 2072 652e 7375 6228 225c 5c78 6532   = re.sub("\\xe2
-00012a90: 5c5c 7838 305c 5c78 3939 222c 2227 222c  \\x80\\x99","'",
-00012aa0: 2073 756d 6d61 7279 290d 0a20 2020 7375   summary)..   su
-00012ab0: 6d6d 6172 793d 7375 6d6d 6172 792e 7265  mmary=summary.re
-00012ac0: 706c 6163 6528 225c 5c78 6532 5c5c 7838  place("\\xe2\\x8
-00012ad0: 305c 5c78 3939 222c 2227 2229 0d0a 2020  0\\x99","'")..  
-00012ae0: 2073 756d 6d61 7279 3d73 756d 6d61 7279   summary=summary
-00012af0: 2e72 6570 6c61 6365 2822 5c5c 7865 325c  .replace("\\xe2\
-00012b00: 5c78 3830 5c5c 7839 3022 2c22 2d22 290d  \x80\\x90","-").
-00012b10: 0a20 2020 7375 6d6d 6172 793d 7375 6d6d  .   summary=summ
-00012b20: 6172 792e 7265 706c 6163 6528 225c 5c78  ary.replace("\\x
-00012b30: 6532 5c5c 7838 305c 5c78 3931 222c 222d  e2\\x80\\x91","-
-00012b40: 2229 0d0a 2020 2073 756d 6d61 7279 3d73  ")..   summary=s
-00012b50: 756d 6d61 7279 2e72 6570 6c61 6365 2822  ummary.replace("
-00012b60: 5c5c 7865 325c 5c78 3830 5c5c 7839 3222  \\xe2\\x80\\x92"
-00012b70: 2c22 2d22 290d 0a20 2020 7375 6d6d 6172  ,"-")..   summar
-00012b80: 793d 7375 6d6d 6172 792e 7265 706c 6163  y=summary.replac
-00012b90: 6528 225c 5c78 6532 5c5c 7838 305c 5c78  e("\\xe2\\x80\\x
-00012ba0: 3933 222c 222d 2229 0d0a 2020 2073 756d  93","-")..   sum
-00012bb0: 6d61 7279 3d73 756d 6d61 7279 2e72 6570  mary=summary.rep
-00012bc0: 6c61 6365 2822 5c5c 7865 325c 5c78 3830  lace("\\xe2\\x80
-00012bd0: 5c5c 7839 3422 2c22 2d22 290d 0a20 2020  \\x94","-")..   
-00012be0: 7375 6d6d 6172 793d 7375 6d6d 6172 792e  summary=summary.
-00012bf0: 7265 706c 6163 6528 225c 5c78 6532 5c5c  replace("\\xe2\\
-00012c00: 7838 305c 5c78 3935 222c 222d 2229 0d0a  x80\\x95","-")..
-00012c10: 2020 2073 756d 6d61 7279 3d73 756d 6d61     summary=summa
-00012c20: 7279 2e72 6570 6c61 6365 2822 5c5c 7865  ry.replace("\\xe
-00012c30: 325c 5c78 3830 5c5c 7862 3322 2c27 2227  2\\x80\\xb3",'"'
-00012c40: 290d 0a20 2020 7375 6d6d 6172 7920 3d20  )..   summary = 
-00012c50: 7375 6d6d 6172 792e 7265 706c 6163 6528  summary.replace(
-00012c60: 27e2 809c 272c 2027 2227 290d 0a20 2020  '...', '"')..   
-00012c70: 7375 6d6d 6172 7920 3d20 7375 6d6d 6172  summary = summar
-00012c80: 792e 7265 706c 6163 6528 27e2 809d 272c  y.replace('...',
-00012c90: 2027 2227 290d 0a20 2020 7375 6d6d 6172   '"')..   summar
-00012ca0: 7920 3d20 7375 6d6d 6172 792e 7265 706c  y = summary.repl
-00012cb0: 6163 6528 27e2 8099 272c 2022 2722 290d  ace('...', "'").
-00012cc0: 0a20 2020 7375 6d6d 6172 7920 3d20 7375  .   summary = su
-00012cd0: 6d6d 6172 792e 7265 706c 6163 6528 27e2  mmary.replace('.
-00012ce0: 8098 272c 2022 2722 290d 0a20 2020 7375  ..', "'")..   su
-00012cf0: 6d6d 6172 7920 3d20 7375 6d6d 6172 792e  mmary = summary.
-00012d00: 7265 706c 6163 6528 27e2 8093 272c 2022  replace('...', "
-00012d10: 2d22 290d 0a20 2020 7375 6d6d 6172 7920  -")..   summary 
-00012d20: 3d20 7375 6d6d 6172 792e 7265 706c 6163  = summary.replac
-00012d30: 6528 27e2 80a6 272c 2022 2e2e 2e22 290d  e('...', "...").
-00012d40: 0a20 2020 7375 6d6d 6172 7920 3d20 7375  .   summary = su
-00012d50: 6d6d 6172 792e 7265 706c 6163 6528 27e2  mmary.replace('.
-00012d60: 8094 272c 2022 2d22 290d 0a20 2020 7375  ..', "-")..   su
-00012d70: 6d6d 6172 7920 3d20 7375 6d6d 6172 792e  mmary = summary.
-00012d80: 7265 706c 6163 6528 2722 272c 2022 2229  replace('"', "")
-00012d90: 0d0a 0d0a 2020 2073 756d 6d61 7279 203d  ....   summary =
-00012da0: 2073 756d 6d61 7279 2e72 6570 6c61 6365   summary.replace
-00012db0: 2827 5c5c 7527 2c27 552b 2729 0d0a 2020  ('\\u','U+')..  
-00012dc0: 2073 756d 6d61 7279 203d 2072 652e 7375   summary = re.su
-00012dd0: 6228 7227 3c55 5c2b 285b 302d 3961 2d66  b(r'<U\+([0-9a-f
-00012de0: 412d 465d 7b34 2c36 7d29 3e27 2c20 6c61  A-F]{4,6})>', la
-00012df0: 6d62 6461 2078 3a20 6368 7228 696e 7428  mbda x: chr(int(
-00012e00: 782e 6772 6f75 7028 3129 2c31 3629 292c  x.group(1),16)),
-00012e10: 2073 756d 6d61 7279 290d 0a0d 0a20 2020   summary)....   
-00012e20: 6b65 7977 6f72 6473 3d67 6574 6b65 7977  keywords=getkeyw
-00012e30: 6f72 6473 2873 756d 6d61 7279 2c6d 6178  ords(summary,max
-00012e40: 6b65 7977 6f72 6473 290d 0a0d 0a20 2020  keywords)....   
-00012e50: 7375 6d6d 6172 7977 6f72 6473 203d 206c  summarywords = l
-00012e60: 656e 2873 756d 6d61 7279 2e73 706c 6974  en(summary.split
-00012e70: 2822 2022 2929 0d0a 200d 0a20 2020 6d61  (" ")).. ..   ma
-00012e80: 696e 6f75 743d 225c 2222 202b 206b 6579  inout="\"" + key
-00012e90: 776f 7264 7320 2b20 225c 222c 5c22 6f72  words + "\",\"or
-00012ea0: 6967 696e 616c 776f 7264 636f 756e 745c  iginalwordcount\
-00012eb0: 223a 2220 2b20 7374 7228 6f72 6967 696e  ":" + str(origin
-00012ec0: 616c 776f 7264 7329 202b 2022 2c5c 2273  alwords) + ",\"s
-00012ed0: 756d 6d61 7279 776f 7264 636f 756e 745c  ummarywordcount\
-00012ee0: 223a 222b 2073 7472 2873 756d 6d61 7279  ":"+ str(summary
-00012ef0: 776f 7264 7329 202b 222c 5c22 6d61 696e  words) +",\"main
-00012f00: 7375 6d6d 6172 795c 223a 7b5c 2273 756d  summary\":{\"sum
-00012f10: 6d61 7279 5c22 3a20 5c22 2220 2b20 7375  mary\": \"" + su
-00012f20: 6d6d 6172 7920 2b20 225c 227d 7d22 0d0a  mmary + "\"}}"..
-00012f30: 2020 2072 6574 7572 6e20 6d61 696e 6f75     return mainou
-00012f40: 740d 0a20 2020 0d0a 2323 2323 2323 2323  t..   ..########
-00012f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012f70: 2323 2323 2323 2323 230d 0a0d 0a66 726f  #########....fro
-00012f80: 6d20 6c61 6e67 6368 6169 6e2e 656d 6265  m langchain.embe
-00012f90: 6464 696e 6773 2e6f 7065 6e61 6920 696d  ddings.openai im
-00012fa0: 706f 7274 204f 7065 6e41 4945 6d62 6564  port OpenAIEmbed
-00012fb0: 6469 6e67 730d 0a66 726f 6d20 6c61 6e67  dings..from lang
-00012fc0: 6368 6169 6e2e 7465 7874 5f73 706c 6974  chain.text_split
-00012fd0: 7465 7220 696d 706f 7274 2043 6861 7261  ter import Chara
-00012fe0: 6374 6572 5465 7874 5370 6c69 7474 6572  cterTextSplitter
-00012ff0: 0d0a 6672 6f6d 206c 616e 6763 6861 696e  ..from langchain
-00013000: 2e76 6563 746f 7273 746f 7265 732e 6661  .vectorstores.fa
-00013010: 6973 7320 696d 706f 7274 2046 4149 5353  iss import FAISS
-00013020: 0d0a 0d0a 6672 6f6d 206c 616e 6763 6861  ....from langcha
-00013030: 696e 2e63 6861 696e 732e 7175 6573 7469  in.chains.questi
-00013040: 6f6e 5f61 6e73 7765 7269 6e67 2069 6d70  on_answering imp
-00013050: 6f72 7420 6c6f 6164 5f71 615f 6368 6169  ort load_qa_chai
-00013060: 6e0d 0a66 726f 6d20 6c61 6e67 6368 6169  n..from langchai
-00013070: 6e2e 6c6c 6d73 2069 6d70 6f72 7420 5072  n.llms import Pr
-00013080: 6f6d 7074 4c61 7965 724f 7065 6e41 4943  omptLayerOpenAIC
-00013090: 6861 740d 0a66 726f 6d20 6c61 6e67 6368  hat..from langch
-000130a0: 6169 6e2e 6368 6174 5f6d 6f64 656c 7320  ain.chat_models 
-000130b0: 696d 706f 7274 2043 6861 744f 7065 6e41  import ChatOpenA
-000130c0: 490d 0a66 726f 6d20 6c61 6e67 6368 6169  I..from langchai
-000130d0: 6e2e 6c6c 6d73 2069 6d70 6f72 7420 4f70  n.llms import Op
-000130e0: 656e 4149 0d0a 696d 706f 7274 2068 6173  enAI..import has
-000130f0: 686c 6962 0d0a 0d0a 2320 416e 7377 6572  hlib....# Answer
-00013100: 2071 7565 7374 696f 6e73 2061 626f 7574   questions about
-00013110: 2074 6865 2068 6561 646c 696e 6573 0d0a   the headlines..
-00013120: 6465 6620 7374 6172 745f 636f 6e76 6572  def start_conver
-00013130: 7361 7469 6f6e 286f 7065 6e61 696b 6579  sation(openaikey
-00013140: 2c71 7565 7279 2c74 6578 742c 7465 6d70  ,query,text,temp
-00013150: 6572 6174 7572 652c 6d6f 6465 6c29 3a0d  erature,model):.
-00013160: 0a20 2020 2023 2047 7261 6220 7468 6520  .    # Grab the 
-00013170: 696e 7075 7420 6672 6f6d 2074 6865 2041  input from the A
-00013180: 5049 0d0a 2020 2020 2020 2020 2371 7565  PI..        #que
-00013190: 7279 203d 2069 6e70 7574 735b 2271 7565  ry = inputs["que
-000131a0: 7279 220d 0a0d 0a0d 0a20 2020 2020 2020  ry"......       
-000131b0: 2074 6578 745f 7370 6c69 7474 6572 203d   text_splitter =
-000131c0: 2043 6861 7261 6374 6572 5465 7874 5370   CharacterTextSp
-000131d0: 6c69 7474 6572 280d 0a20 2020 2020 2020  litter(..       
-000131e0: 2020 2020 2073 6570 6172 6174 6f72 3d22       separator="
-000131f0: 2022 2c0d 0a20 2020 2020 2020 2020 2020   ",..           
-00013200: 2063 6875 6e6b 5f73 697a 653d 3130 3030   chunk_size=1000
-00013210: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-00013220: 6875 6e6b 5f6f 7665 726c 6170 3d32 3030  hunk_overlap=200
-00013230: 2c0d 0a20 2020 2020 2020 2020 2020 206c  ,..            l
-00013240: 656e 6774 685f 6675 6e63 7469 6f6e 3d6c  ength_function=l
-00013250: 656e 2c0d 0a20 2020 2020 2020 2029 0d0a  en,..        )..
-00013260: 0d0a 2020 2020 2020 2020 7465 7874 7320  ..        texts 
-00013270: 3d20 7465 7874 5f73 706c 6974 7465 722e  = text_splitter.
-00013280: 7370 6c69 745f 7465 7874 2874 6578 7429  split_text(text)
-00013290: 0d0a 2020 2020 2020 2020 656d 6265 6464  ..        embedd
-000132a0: 696e 6773 203d 204f 7065 6e41 4945 6d62  ings = OpenAIEmb
-000132b0: 6564 6469 6e67 7328 290d 0a20 2020 2020  eddings()..     
-000132c0: 2020 2064 6f63 7365 6172 6368 203d 2046     docsearch = F
-000132d0: 4149 5353 2e66 726f 6d5f 7465 7874 7328  AISS.from_texts(
-000132e0: 7465 7874 732c 2065 6d62 6564 6469 6e67  texts, embedding
-000132f0: 7329 0d0a 2020 2020 2020 2020 646f 6373  s)..        docs
-00013300: 203d 2064 6f63 7365 6172 6368 2e73 696d   = docsearch.sim
-00013310: 696c 6172 6974 795f 7365 6172 6368 2871  ilarity_search(q
-00013320: 7565 7279 290d 0a20 2020 2020 2020 200d  uery)..        .
-00013330: 0a20 2020 2020 2020 2063 6861 696e 203d  .        chain =
-00013340: 206c 6f61 645f 7161 5f63 6861 696e 284f   load_qa_chain(O
-00013350: 7065 6e41 4928 6d6f 6465 6c5f 6e61 6d65  penAI(model_name
-00013360: 3d6d 6f64 656c 2c20 7465 6d70 6572 6174  =model, temperat
-00013370: 7572 653d 7465 6d70 6572 6174 7572 652c  ure=temperature,
-00013380: 6f70 656e 6169 5f61 7069 5f6b 6579 3d6f  openai_api_key=o
-00013390: 7065 6e61 696b 6579 292c 2063 6861 696e  penaikey), chain
-000133a0: 5f74 7970 653d 2273 7475 6666 2229 0d0a  _type="stuff")..
-000133b0: 2020 2020 2020 2020 7265 7320 3d20 6368          res = ch
-000133c0: 6169 6e28 7b22 696e 7075 745f 646f 6375  ain({"input_docu
-000133d0: 6d65 6e74 7322 3a20 646f 6373 2c20 2271  ments": docs, "q
-000133e0: 7565 7374 696f 6e22 3a20 7175 6572 797d  uestion": query}
-000133f0: 2c20 7265 7475 726e 5f6f 6e6c 795f 6f75  , return_only_ou
-00013400: 7470 7574 733d 5472 7565 290d 0a0d 0a20  tputs=True).... 
-00013410: 2020 2020 2020 2023 7265 7475 726e 207b         #return {
-00013420: 2270 7265 6422 3a20 7265 737d 0d0a 2020  "pred": res}..  
-00013430: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00013440: 0d0a 0d0a 2323 2323 2323 2323 2323 2323  ....############
-00013450: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013460: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013470: 2323 2323 2323 2323 0d0a 6672 6f6d 2070  ########..from p
-00013480: 6466 7175 6572 7920 696d 706f 7274 2050  dfquery import P
-00013490: 4446 5175 6572 790d 0a69 6d70 6f72 7420  DFQuery..import 
-000134a0: 786d 6c74 6f64 6963 740d 0a0d 0a0d 0a64  xmltodict......d
-000134b0: 6566 206c 6162 656c 6669 656c 6473 2866  ef labelfields(f
-000134c0: 696c 656e 616d 652c 6c61 6265 6c6e 616d  ilename,labelnam
-000134d0: 652c 6163 726f 7479 7065 293a 0d0a 2020  e,acrotype):..  
-000134e0: 2020 2070 6466 203d 2050 4446 5175 6572     pdf = PDFQuer
-000134f0: 7928 6669 6c65 6e61 6d65 290d 0a20 2020  y(filename)..   
-00013500: 2020 7064 662e 6c6f 6164 2829 0d0a 2020    pdf.load()..  
-00013510: 2020 2023 4c54 5465 7874 4c69 6e65 486f     #LTTextLineHo
-00013520: 7269 7a6f 6e74 616c 0d0a 2020 2020 206c  rizontal..     l
-00013530: 6162 656c 203d 2070 6466 2e70 7128 6163  abel = pdf.pq(ac
-00013540: 726f 7479 7065 2b27 3a63 6f6e 7461 696e  rotype+':contain
-00013550: 7328 2227 2b6c 6162 656c 6e61 6d65 202b  s("'+labelname +
-00013560: 2027 2229 2729 0d0a 2020 2020 206c 6566   '")')..     lef
-00013570: 745f 636f 726e 6572 203d 2066 6c6f 6174  t_corner = float
-00013580: 286c 6162 656c 2e61 7474 7228 2778 3027  (label.attr('x0'
-00013590: 2929 0d0a 2020 2020 2062 6f74 746f 6d5f  ))..     bottom_
-000135a0: 636f 726e 6572 203d 2066 6c6f 6174 286c  corner = float(l
-000135b0: 6162 656c 2e61 7474 7228 2779 3027 2929  abel.attr('y0'))
-000135c0: 0d0a 2020 2020 206e 616d 6520 3d20 7064  ..     name = pd
-000135d0: 662e 7071 2861 6372 6f74 7970 6520 2b27  f.pq(acrotype +'
-000135e0: 3a69 6e5f 6262 6f78 2822 2573 2c20 2573  :in_bbox("%s, %s
-000135f0: 2c20 2573 2c20 2573 2229 2720 2520 286c  , %s, %s")' % (l
-00013600: 6566 745f 636f 726e 6572 2c20 626f 7474  eft_corner, bott
-00013610: 6f6d 5f63 6f72 6e65 722d 3330 2c20 6c65  om_corner-30, le
-00013620: 6674 5f63 6f72 6e65 722b 3135 302c 2062  ft_corner+150, b
-00013630: 6f74 746f 6d5f 636f 726e 6572 2929 2e74  ottom_corner)).t
-00013640: 6578 7428 290d 0a20 2020 2020 7265 7475  ext()..     retu
-00013650: 726e 206e 616d 650d 0a0d 0a0d 0a64 6566  rn name......def
-00013660: 2065 7874 7261 6374 6669 656c 6473 2866   extractfields(f
-00013670: 696c 656e 616d 6529 3a0d 0a20 2020 2020  ilename):..     
-00013680: 2023 7265 6164 2074 6865 2050 4446 0d0a   #read the PDF..
-00013690: 2020 2020 2020 7064 6620 3d20 5044 4651        pdf = PDFQ
-000136a0: 7565 7279 2866 696c 656e 616d 6529 0d0a  uery(filename)..
-000136b0: 2020 2020 2020 7064 662e 6c6f 6164 2829        pdf.load()
-000136c0: 0d0a 0d0a 2020 2020 2020 236f 203d 2078  ....      #o = x
-000136d0: 6d6c 746f 6469 6374 2e70 6172 7365 2827  mltodict.parse('
-000136e0: 3c65 3e20 3c61 3e74 6578 743c 2f61 3e20  <e> <a>text</a> 
-000136f0: 3c61 3e74 6578 743c 2f61 3e20 3c2f 653e  <a>text</a> </e>
-00013700: 2729 0d0a 0d0a 2020 2020 2020 2363 6f6e  ')....      #con
-00013710: 7665 7274 2074 6865 2070 6466 2074 6f20  vert the pdf to 
-00013720: 584d 4c0d 0a20 2020 2020 2078 6d6c 6669  XML..      xmlfi
-00013730: 6c65 3d20 6669 6c65 6e61 6d65 202b 2027  le= filename + '
-00013740: 2e78 6d6c 270d 0a20 2020 2020 2070 6466  .xml'..      pdf
-00013750: 2e74 7265 652e 7772 6974 6528 786d 6c66  .tree.write(xmlf
-00013760: 696c 652c 2070 7265 7474 795f 7072 696e  ile, pretty_prin
-00013770: 7420 3d20 5472 7565 290d 0a20 2020 2020  t = True)..     
-00013780: 2077 6974 6820 6f70 656e 2878 6d6c 6669   with open(xmlfi
-00013790: 6c65 2920 6173 2066 3a20 7320 3d20 662e  le) as f: s = f.
-000137a0: 7265 6164 2829 0d0a 0d0a 2020 2020 2020  read()....      
-000137b0: 2370 7269 6e74 2873 290d 0a20 2020 2020  #print(s)..     
-000137c0: 206a 736f 6e62 7566 3d78 6d6c 746f 6a73   jsonbuf=xmltojs
-000137d0: 6f6e 2873 2c78 6d6c 6669 6c65 290d 0a0d  on(s,xmlfile)...
-000137e0: 0a20 2020 2020 2072 6574 7572 6e20 6a73  .      return js
-000137f0: 6f6e 6275 660d 0a20 2020 2020 200d 0a0d  onbuf..      ...
-00013800: 0a64 6566 2078 6d6c 746f 6a73 6f6e 2878  .def xmltojson(x
-00013810: 6d6c 6275 6666 6572 2c78 6d6c 6669 6c65  mlbuffer,xmlfile
-00013820: 293a 0d0a 0d0a 2020 2020 2020 6f20 3d20  ):....      o = 
-00013830: 786d 6c74 6f64 6963 742e 7061 7273 6528  xmltodict.parse(
-00013840: 786d 6c62 7566 6665 7229 0d0a 2020 2020  xmlbuffer)..    
-00013850: 2020 786d 6c6a 736f 6e3d 6a73 6f6e 2e64    xmljson=json.d
-00013860: 756d 7073 286f 290d 0a20 2020 2020 2023  umps(o)..      #
-00013870: 7072 696e 7428 786d 6c6a 736f 6e29 0d0a  print(xmljson)..
-00013880: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00013890: 786d 6c66 696c 6520 2b20 272e 6a73 6f6e  xmlfile + '.json
-000138a0: 272c 2277 2229 2061 7320 663a 0d0a 2020  ',"w") as f:..  
-000138b0: 2020 2020 2020 662e 7772 6974 6528 786d        f.write(xm
-000138c0: 6c6a 736f 6e29 0d0a 0d0a 2020 2020 2020  ljson)....      
-000138d0: 7265 7475 726e 2078 6d6c 6a73 6f6e 2020  return xmljson  
-000138e0: 0d0a 0d0a 2366 696c 656e 616d 653d 2774  ....#filename='t
-000138f0: 6573 742d 7461 782e 7064 6627 2020 2020  est-tax.pdf'    
-00013900: 200d 0a23 7064 666a 736f 6e3d 6578 7472   ..#pdfjson=extr
-00013910: 6163 7466 6965 6c64 7328 6669 6c65 6e61  actfields(filena
-00013920: 6d65 290d 0a23 6e61 6d65 7465 7874 3d6c  me)..#nametext=l
-00013930: 6162 656c 6669 656c 6473 2866 696c 656e  abelfields(filen
-00013940: 616d 652c 2242 7573 696e 6573 7320 6e75  ame,"Business nu
-00013950: 6d62 6572 222c 224c 5454 6578 744c 696e  mber","LTTextLin
-00013960: 6548 6f72 697a 6f6e 7461 6c22 290d 0a23  eHorizontal")..#
-00013970: 7072 696e 7428 6e61 6d65 7465 7874 290d  print(nametext).
-00013980: 0a0d 0a                                  ...
+00010210: 6620 7669 7065 7269 6d61 6765 746f 7465  f viperimagetote
+00010220: 7874 2866 696c 656e 616d 6529 3a0d 0a20  xt(filename):.. 
+00010230: 2020 2069 6620 6669 6c65 6e61 6d65 3d3d     if filename==
+00010240: 2222 3a0d 0a20 2020 2020 2020 2072 6574  "":..        ret
+00010250: 7572 6e20 2245 6e74 6572 2049 4d41 4745  urn "Enter IMAGE
+00010260: 2028 706e 672c 206a 7067 2c20 6574 632e   (png, jpg, etc.
+00010270: 2920 6669 6c65 6e61 6d65 220d 0a20 2020  ) filename"..   
+00010280: 200d 0a20 2020 2072 6574 7572 6e20 646f   ..    return do
+00010290: 6f63 726d 6169 6e28 6669 6c65 6e61 6d65  ocrmain(filename
+000102a0: 290d 0a0d 0a64 6566 2076 6970 6572 6175  )....def viperau
+000102b0: 6469 6f74 6f74 6578 7428 6669 6c65 6e61  diototext(filena
+000102c0: 6d65 293a 0d0a 2020 2020 6966 2066 696c  me):..    if fil
+000102d0: 656e 616d 653d 3d22 223a 0d0a 2020 2020  ename=="":..    
+000102e0: 2020 2020 7265 7475 726e 2022 456e 7465      return "Ente
+000102f0: 7220 4155 4449 4f20 4669 6c65 2028 5741  r AUDIO File (WA
+00010300: 5629 2066 696c 656e 616d 6522 0d0a 2020  V) filename"..  
+00010310: 2020 0d0a 2020 2020 7265 7475 726e 2061    ..    return a
+00010320: 7564 696f 746f 7465 7874 2866 696c 656e  udiototext(filen
+00010330: 616d 6529 0d0a 0d0a 6465 6620 7669 7065  ame)....def vipe
+00010340: 7276 6964 656f 746f 7465 7874 2866 696c  rvideototext(fil
+00010350: 656e 616d 6529 3a0d 0a20 2020 2069 6620  ename):..    if 
+00010360: 6669 6c65 6e61 6d65 3d3d 2222 3a0d 0a20  filename=="":.. 
+00010370: 2020 2020 2020 2072 6574 7572 6e20 2245         return "E
+00010380: 6e74 6572 2056 4944 454f 2046 696c 6520  nter VIDEO File 
+00010390: 284d 5034 2920 6669 6c65 6e61 6d65 220d  (MP4) filename".
+000103a0: 0a20 2020 200d 0a20 2020 2072 6574 7572  .    ..    retur
+000103b0: 6e20 636f 6e76 6572 7476 6964 656f 746f  n convertvideoto
+000103c0: 7465 7874 2866 696c 656e 616d 6529 0d0a  text(filename)..
+000103d0: 2020 2020 0d0a 6465 6620 6172 6579 6f75      ..def areyou
+000103e0: 6275 7379 2868 6f73 742c 706f 7274 3d2d  busy(host,port=-
+000103f0: 3939 392c 6d69 6372 6f73 6572 7669 6365  999,microservice
+00010400: 6964 3d27 2729 3a0d 0a20 2020 2067 6c6f  id=''):..    glo
+00010410: 6261 6c20 636f 6e6e 6563 7469 6f6e 6572  bal connectioner
+00010420: 726f 720d 0a0d 0a20 2020 2069 6620 286c  ror....    if (l
+00010430: 656e 2868 6f73 7429 3d3d 3020 6f72 2070  en(host)==0 or p
+00010440: 6f72 743d 3d2d 3939 3920 293a 0d0a 2020  ort==-999 ):..  
+00010450: 2020 2020 2020 2072 6574 7572 6e20 2250         return "P
+00010460: 6c65 6173 6520 656e 7465 7220 686f 7374  lease enter host
+00010470: 2c70 6f72 7422 0d0a 2020 2020 7661 6c75  ,port"..    valu
+00010480: 653d 2822 6172 6579 6f75 6275 7379 2229  e=("areyoubusy")
+00010490: 0d0a 0d0a 2020 2020 7661 6c3d 6c6f 6f70  ....    val=loop
+000104a0: 2e72 756e 5f75 6e74 696c 5f63 6f6d 706c  .run_until_compl
+000104b0: 6574 6528 7463 705f 6563 686f 5f63 6c69  ete(tcp_echo_cli
+000104c0: 656e 7476 6970 6572 2876 616c 7565 2c20  entviper(value, 
+000104d0: 6c6f 6f70 2c68 6f73 742c 706f 7274 2c6d  loop,host,port,m
+000104e0: 6963 726f 7365 7276 6963 6569 6429 290d  icroserviceid)).
+000104f0: 0a20 2020 2069 6620 636f 6e6e 6563 7469  .    if connecti
+00010500: 6f6e 6572 726f 723a 0d0a 2020 2020 2020  onerror:..      
+00010510: 2020 2072 6574 7572 6e20 636f 6e6e 6563     return connec
+00010520: 7469 6f6e 6572 726f 720d 0a0d 0a20 2020  tionerror....   
+00010530: 2072 6574 7572 6e20 7661 6c0d 0a0d 0a23   return val....#
+00010540: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010550: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010560: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010570: 2323 230d 0a69 6d70 6f72 7420 7379 730d  ###..import sys.
+00010580: 0a66 726f 6d20 7064 666d 696e 6572 2e70  .from pdfminer.p
+00010590: 6466 7061 7273 6572 2069 6d70 6f72 7420  dfparser import 
+000105a0: 5044 4650 6172 7365 720d 0a66 726f 6d20  PDFParser..from 
+000105b0: 7064 666d 696e 6572 2e70 6466 646f 6375  pdfminer.pdfdocu
+000105c0: 6d65 6e74 2069 6d70 6f72 7420 5044 4644  ment import PDFD
+000105d0: 6f63 756d 656e 740d 0a66 726f 6d20 7064  ocument..from pd
+000105e0: 666d 696e 6572 2e70 6466 7061 6765 2069  fminer.pdfpage i
+000105f0: 6d70 6f72 7420 5044 4650 6167 650d 0a66  mport PDFPage..f
+00010600: 726f 6d20 7064 666d 696e 6572 2e70 6466  rom pdfminer.pdf
+00010610: 7061 6765 2069 6d70 6f72 7420 5044 4654  page import PDFT
+00010620: 6578 7445 7874 7261 6374 696f 6e4e 6f74  extExtractionNot
+00010630: 416c 6c6f 7765 640d 0a66 726f 6d20 7064  Allowed..from pd
+00010640: 666d 696e 6572 2e70 6466 696e 7465 7270  fminer.pdfinterp
+00010650: 2069 6d70 6f72 7420 5044 4652 6573 6f75   import PDFResou
+00010660: 7263 654d 616e 6167 6572 0d0a 6672 6f6d  rceManager..from
+00010670: 2070 6466 6d69 6e65 722e 7064 6669 6e74   pdfminer.pdfint
+00010680: 6572 7020 696d 706f 7274 2050 4446 5061  erp import PDFPa
+00010690: 6765 496e 7465 7270 7265 7465 720d 0a23  geInterpreter..#
+000106a0: 6672 6f6d 2053 7472 696e 6749 4f20 696d  from StringIO im
+000106b0: 706f 7274 2053 7472 696e 6749 4f0d 0a66  port StringIO..f
+000106c0: 726f 6d20 696f 2069 6d70 6f72 7420 5374  rom io import St
+000106d0: 7269 6e67 494f 0d0a 696d 706f 7274 2075  ringIO..import u
+000106e0: 726c 6c69 622e 7265 7175 6573 7420 200d  rllib.request  .
+000106f0: 0a23 696d 706f 7274 2074 6d6c 7465 7874  .#import tmltext
+00010700: 7375 6d6d 6172 790d 0a69 6d70 6f72 7420  summary..import 
+00010710: 6f73 0d0a 696d 706f 7274 2064 6174 6574  os..import datet
+00010720: 696d 650d 0a23 696d 706f 7274 2067 6c6f  ime..#import glo
+00010730: 620d 0a0d 0a0d 0a66 726f 6d20 7064 666d  b......from pdfm
+00010740: 696e 6572 2e6c 6179 6f75 7420 696d 706f  iner.layout impo
+00010750: 7274 204c 4150 6172 616d 730d 0a66 726f  rt LAParams..fro
+00010760: 6d20 7064 666d 696e 6572 2e63 6f6e 7665  m pdfminer.conve
+00010770: 7274 6572 2069 6d70 6f72 7420 5465 7874  rter import Text
+00010780: 436f 6e76 6572 7465 720d 0a20 0d0a 636c  Converter.. ..cl
+00010790: 6173 7320 4d79 5061 7273 6572 286f 626a  ass MyParser(obj
+000107a0: 6563 7429 3a0d 0a20 2020 2064 6566 205f  ect):..    def _
+000107b0: 5f69 6e69 745f 5f28 7365 6c66 2c20 7064  _init__(self, pd
+000107c0: 6629 3a0d 0a20 2020 2020 2020 2023 2320  f):..        ## 
+000107d0: 536e 6970 7065 6420 6164 6170 7465 6420  Snipped adapted 
+000107e0: 6672 6f6d 2059 7573 756b 6520 5368 696e  from Yusuke Shin
+000107f0: 7961 6d61 7320 0d0a 2020 2020 2020 2020  yamas ..        
+00010800: 2350 4446 4d69 6e65 7220 646f 6375 6d65  #PDFMiner docume
+00010810: 6e74 6174 696f 6e0d 0a20 2020 2020 2020  ntation..       
+00010820: 2023 2043 7265 6174 6520 7468 6520 646f   # Create the do
+00010830: 6375 6d65 6e74 206d 6f64 656c 2066 726f  cument model fro
+00010840: 6d20 7468 6520 6669 6c65 0d0a 2020 2020  m the file..    
+00010850: 2020 2020 7061 7273 6572 203d 2050 4446      parser = PDF
+00010860: 5061 7273 6572 286f 7065 6e28 7064 662c  Parser(open(pdf,
+00010870: 2027 7262 2729 290d 0a20 2020 2020 2020   'rb'))..       
+00010880: 2064 6f63 756d 656e 7420 3d20 5044 4644   document = PDFD
+00010890: 6f63 756d 656e 7428 7061 7273 6572 290d  ocument(parser).
+000108a0: 0a20 2020 2020 2020 2023 2054 7279 2074  .        # Try t
+000108b0: 6f20 7061 7273 6520 7468 6520 646f 6375  o parse the docu
+000108c0: 6d65 6e74 0d0a 2020 2020 2020 2020 6966  ment..        if
+000108d0: 206e 6f74 2064 6f63 756d 656e 742e 6973   not document.is
+000108e0: 5f65 7874 7261 6374 6162 6c65 3a0d 0a20  _extractable:.. 
+000108f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00010900: 2050 4446 5465 7874 4578 7472 6163 7469   PDFTextExtracti
+00010910: 6f6e 4e6f 7441 6c6c 6f77 6564 0d0a 2020  onNotAllowed..  
+00010920: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
+00010930: 2050 4446 2072 6573 6f75 7263 6520 6d61   PDF resource ma
+00010940: 6e61 6765 7220 6f62 6a65 6374 200d 0a20  nager object .. 
+00010950: 2020 2020 2020 2023 2074 6861 7420 7374         # that st
+00010960: 6f72 6573 2073 6861 7265 6420 7265 736f  ores shared reso
+00010970: 7572 6365 732e 0d0a 2020 2020 2020 2020  urces...        
+00010980: 7273 7263 6d67 7220 3d20 5044 4652 6573  rsrcmgr = PDFRes
+00010990: 6f75 7263 654d 616e 6167 6572 2829 0d0a  ourceManager()..
+000109a0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+000109b0: 2061 2062 7566 6665 7220 666f 7220 7468   a buffer for th
+000109c0: 6520 7061 7273 6564 2074 6578 740d 0a20  e parsed text.. 
+000109d0: 2020 2020 2020 2072 6574 7374 7220 3d20         retstr = 
+000109e0: 5374 7269 6e67 494f 2829 0d0a 2020 2020  StringIO()..    
+000109f0: 2020 2020 2320 5370 6163 696e 6720 7061      # Spacing pa
+00010a00: 7261 6d65 7465 7273 2066 6f72 2070 6172  rameters for par
+00010a10: 7369 6e67 0d0a 2020 2020 2020 2020 6c61  sing..        la
+00010a20: 7061 7261 6d73 203d 204c 4150 6172 616d  params = LAParam
+00010a30: 7328 290d 0a20 2020 2020 2020 2063 6f64  s()..        cod
+00010a40: 6563 203d 2027 7574 662d 3827 0d0a 200d  ec = 'utf-8'.. .
+00010a50: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+00010a60: 6520 6120 5044 4620 6465 7669 6365 206f  e a PDF device o
+00010a70: 626a 6563 740d 0a20 2020 2020 2020 2064  bject..        d
+00010a80: 6576 6963 6520 3d20 5465 7874 436f 6e76  evice = TextConv
+00010a90: 6572 7465 7228 7273 7263 6d67 722c 2072  erter(rsrcmgr, r
+00010aa0: 6574 7374 722c 0d0a 2020 2020 2020 2020  etstr,..        
+00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ac0: 2020 2020 2020 206c 6170 6172 616d 7320         laparams 
+00010ad0: 3d20 6c61 7061 7261 6d73 290d 0a20 2020  = laparams)..   
+00010ae0: 2020 2020 2023 2043 7265 6174 6520 6120       # Create a 
+00010af0: 5044 4620 696e 7465 7270 7265 7465 7220  PDF interpreter 
+00010b00: 6f62 6a65 6374 0d0a 2020 2020 2020 2020  object..        
+00010b10: 696e 7465 7270 7265 7465 7220 3d20 5044  interpreter = PD
+00010b20: 4650 6167 6549 6e74 6572 7072 6574 6572  FPageInterpreter
+00010b30: 2872 7372 636d 6772 2c20 6465 7669 6365  (rsrcmgr, device
+00010b40: 290d 0a20 2020 2020 2020 2023 2050 726f  )..        # Pro
+00010b50: 6365 7373 2065 6163 6820 7061 6765 2063  cess each page c
+00010b60: 6f6e 7461 696e 6564 2069 6e20 7468 6520  ontained in the 
+00010b70: 646f 6375 6d65 6e74 2e0d 0a20 2020 2020  document...     
+00010b80: 2020 2066 6f72 2070 6167 6520 696e 2050     for page in P
+00010b90: 4446 5061 6765 2e63 7265 6174 655f 7061  DFPage.create_pa
+00010ba0: 6765 7328 646f 6375 6d65 6e74 293a 0d0a  ges(document):..
+00010bb0: 2020 2020 2020 2020 2020 2020 696e 7465              inte
+00010bc0: 7270 7265 7465 722e 7072 6f63 6573 735f  rpreter.process_
+00010bd0: 7061 6765 2870 6167 6529 0d0a 2020 2020  page(page)..    
+00010be0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+00010bf0: 656c 662e 7265 636f 7264 7320 2020 2020  elf.records     
+00010c00: 2020 2020 2020 203d 205b 5d0d 0a20 2020         = []..   
+00010c10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00010c20: 6c69 6e65 7320 3d20 7265 7473 7472 2e67  lines = retstr.g
+00010c30: 6574 7661 6c75 6528 292e 7370 6c69 746c  etvalue().splitl
+00010c40: 696e 6573 2829 0d0a 2020 2020 2020 2020  ines()..        
+00010c50: 666f 7220 6c69 6e65 2069 6e20 6c69 6e65  for line in line
+00010c60: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00010c70: 7365 6c66 2e68 616e 646c 655f 6c69 6e65  self.handle_line
+00010c80: 286c 696e 6529 0d0a 2020 2020 200d 0a20  (line)..     .. 
+00010c90: 2020 2064 6566 2068 616e 646c 655f 6c69     def handle_li
+00010ca0: 6e65 2873 656c 662c 206c 696e 6529 3a0d  ne(self, line):.
+00010cb0: 0a20 2020 2020 2020 2023 2043 7573 746f  .        # Custo
+00010cc0: 6d69 7a65 2079 6f75 7220 6c69 6e65 2d62  mize your line-b
+00010cd0: 792d 6c69 6e65 2070 6172 7365 7220 6865  y-line parser he
+00010ce0: 7265 0d0a 2020 2020 2020 2020 7365 6c66  re..        self
+00010cf0: 2e72 6563 6f72 6473 2e61 7070 656e 6428  .records.append(
+00010d00: 6c69 6e65 290d 0a0d 0a64 6566 2073 6372  line)....def scr
+00010d10: 6170 6570 6466 2874 6865 7572 6c2c 666e  apepdf(theurl,fn
+00010d20: 293a 0d0a 2020 2020 7363 7261 7065 645f  ):..    scraped_
+00010d30: 6461 7461 203d 2075 726c 6c69 622e 7265  data = urllib.re
+00010d40: 7175 6573 742e 7572 6c6f 7065 6e28 7468  quest.urlopen(th
+00010d50: 6575 726c 2920 200d 0a20 2020 2066 696c  eurl)  ..    fil
+00010d60: 6520 3d20 6f70 656e 2866 6e2c 2027 7762  e = open(fn, 'wb
+00010d70: 2729 0d0a 2020 2020 6669 6c65 2e77 7269  ')..    file.wri
+00010d80: 7465 2873 6372 6170 6564 5f64 6174 612e  te(scraped_data.
+00010d90: 7265 6164 2829 290d 0a20 2020 2066 696c  read())..    fil
+00010da0: 652e 636c 6f73 6528 290d 0a20 2020 2023  e.close()..    #
+00010db0: 7265 7475 726e 2061 7274 6963 6c65 5f74  return article_t
+00010dc0: 6578 740d 0a0d 0a64 6566 2073 7461 7274  ext....def start
+00010dd0: 7064 6672 6561 6469 6e67 2866 696c 656e  pdfreading(filen
+00010de0: 616d 652c 6676 616c 7565 2c6b 6579 636f  ame,fvalue,keyco
+00010df0: 756e 7429 3a0d 0a20 2023 6f73 2e70 6174  unt):..  #os.pat
+00010e00: 682e 6162 7370 6174 6828 6f73 2e67 6574  h.abspath(os.get
+00010e10: 6377 6428 2929 0d0a 2020 7468 6573 697a  cwd())..  thesiz
+00010e20: 653d 726f 756e 6428 6f73 2e70 6174 682e  e=round(os.path.
+00010e30: 6765 7473 697a 6528 6669 6c65 6e61 6d65  getsize(filename
+00010e40: 292f 3130 3030 3030 302c 3229 0d0a 2020  )/1000000,2)..  
+00010e50: 6d5f 7469 6d65 203d 206f 732e 7061 7468  m_time = os.path
+00010e60: 2e67 6574 6d74 696d 6528 6669 6c65 6e61  .getmtime(filena
+00010e70: 6d65 290d 0a20 2064 745f 6d20 3d20 6461  me)..  dt_m = da
+00010e80: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
+00010e90: 6672 6f6d 7469 6d65 7374 616d 7028 6d5f  fromtimestamp(m_
+00010ea0: 7469 6d65 290d 0a20 2063 5f74 696d 6520  time)..  c_time 
+00010eb0: 3d20 6f73 2e70 6174 682e 6765 7463 7469  = os.path.getcti
+00010ec0: 6d65 2866 696c 656e 616d 6529 0d0a 2020  me(filename)..  
+00010ed0: 2320 636f 6e76 6572 7420 6372 6561 7469  # convert creati
+00010ee0: 6f6e 2074 696d 6573 7461 6d70 2069 6e74  on timestamp int
+00010ef0: 6f20 4461 7465 5469 6d65 206f 626a 6563  o DateTime objec
+00010f00: 740d 0a20 2064 745f 6320 3d20 6461 7465  t..  dt_c = date
+00010f10: 7469 6d65 2e64 6174 6574 696d 652e 6672  time.datetime.fr
+00010f20: 6f6d 7469 6d65 7374 616d 7028 635f 7469  omtimestamp(c_ti
+00010f30: 6d65 290d 0a20 2063 6f20 3d20 7374 7228  me)..  co = str(
+00010f40: 6474 5f63 2920 5b30 3a31 395d 0d0a 2020  dt_c) [0:19]..  
+00010f50: 6d6f 203d 2073 7472 2864 745f 6d29 205b  mo = str(dt_m) [
+00010f60: 303a 3139 5d0d 0a0d 0a20 2070 203d 204d  0:19]....  p = M
+00010f70: 7950 6172 7365 7228 6669 6c65 6e61 6d65  yParser(filename
+00010f80: 290d 0a20 2074 6865 7465 7874 3d27 5c6e  )..  thetext='\n
+00010f90: 272e 6a6f 696e 2870 2e72 6563 6f72 6473  '.join(p.records
+00010fa0: 290d 0a20 2061 7274 6963 6c65 5f74 6578  )..  article_tex
+00010fb0: 743d 7468 6574 6578 742e 656e 636f 6465  t=thetext.encode
+00010fc0: 2827 7574 6638 2729 0d0a 2020 7375 6d6d  ('utf8')..  summ
+00010fd0: 6172 697a 6564 3d22 7b5c 2266 696c 656e  arized="{\"filen
+00010fe0: 616d 655c 223a 5c22 2220 2b20 6669 6c65  ame\":\"" + file
+00010ff0: 6e61 6d65 202b 2022 5c22 2c5c 2266 696c  name + "\",\"fil
+00011000: 6573 697a 6528 4d42 295c 223a 222b 7374  esize(MB)\":"+st
+00011010: 7228 7468 6573 697a 6529 2b22 2c5c 2266  r(thesize)+",\"f
+00011020: 696c 6563 7265 6174 6564 6f6e 5c22 3a5c  ilecreatedon\":\
+00011030: 2222 202b 2063 6f20 2b20 225c 222c 5c22  "" + co + "\",\"
+00011040: 6669 6c65 6d6f 6469 6669 6564 6f6e 5c22  filemodifiedon\"
+00011050: 3a5c 2222 202b 206d 6f20 2b20 225c 222c  :\"" + mo + "\",
+00011060: 5c22 6b65 7977 6f72 6473 5c22 3a22 202b  \"keywords\":" +
+00011070: 2020 7374 6172 7473 756d 6d61 7279 2874    startsummary(t
+00011080: 6865 7465 7874 2c66 7661 6c75 652c 6b65  hetext,fvalue,ke
+00011090: 7963 6f75 6e74 290d 0a20 2320 7072 696e  ycount).. # prin
+000110a0: 7428 7375 6d6d 6172 697a 6564 290d 0a20  t(summarized).. 
+000110b0: 2072 6574 7572 6e20 7375 6d6d 6172 697a   return summariz
+000110c0: 6564 0d0a 0d0a 0d0a 2323 2323 2323 2323  ed......########
+000110d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000110e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000110f0: 2323 2323 2323 230d 0a23 2044 6576 656c  #######..# Devel
+00011100: 6f70 6564 2062 7920 4f54 4943 5320 4164  oped by OTICS Ad
+00011110: 7661 6e63 6564 2041 6e61 6c79 7469 6373  vanced Analytics
+00011120: 0d0a 2320 5365 6261 7374 6961 6e20 4d61  ..# Sebastian Ma
+00011130: 7572 6963 650d 0a0d 0a69 6d70 6f72 7420  urice....import 
+00011140: 6273 3420 6173 2062 7320 200d 0a69 6d70  bs4 as bs  ..imp
+00011150: 6f72 7420 7572 6c6c 6962 2e72 6571 7565  ort urllib.reque
+00011160: 7374 2020 0d0a 696d 706f 7274 2072 650d  st  ..import re.
+00011170: 0a69 6d70 6f72 7420 6e6c 746b 0d0a 6672  .import nltk..fr
+00011180: 6f6d 206e 6c74 6b2e 746f 6b65 6e69 7a65  om nltk.tokenize
+00011190: 2069 6d70 6f72 7420 5265 6765 7870 546f   import RegexpTo
+000111a0: 6b65 6e69 7a65 720d 0a69 6d70 6f72 7420  kenizer..import 
+000111b0: 6865 6170 710d 0a69 6d70 6f72 7420 7379  heapq..import sy
+000111c0: 730d 0a69 6d70 6f72 7420 6f73 0d0a 6672  s..import os..fr
+000111d0: 6f6d 2072 616b 655f 6e6c 746b 2069 6d70  om rake_nltk imp
+000111e0: 6f72 7420 4d65 7472 6963 2c52 616b 650d  ort Metric,Rake.
+000111f0: 0a69 6d70 6f72 7420 6a73 6f6e 0d0a 696d  .import json..im
+00011200: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
+00011210: 640d 0a69 6d70 6f72 7420 6e6c 746b 2e63  d..import nltk.c
+00011220: 6f72 7075 730d 0a66 726f 6d20 6e6c 746b  orpus..from nltk
+00011230: 2e63 6f72 7075 7320 696d 706f 7274 2073  .corpus import s
+00011240: 746f 7077 6f72 6473 0d0a 6672 6f6d 2074  topwords..from t
+00011250: 6578 7462 6c6f 6220 696d 706f 7274 2054  extblob import T
+00011260: 6578 7442 6c6f 620d 0a66 726f 6d20 7465  extBlob..from te
+00011270: 7874 626c 6f62 2069 6d70 6f72 7420 576f  xtblob import Wo
+00011280: 7264 0d0a 6672 6f6d 2073 6b6c 6561 726e  rd..from sklearn
+00011290: 2e66 6561 7475 7265 5f65 7874 7261 6374  .feature_extract
+000112a0: 696f 6e2e 7465 7874 2069 6d70 6f72 7420  ion.text import 
+000112b0: 5466 6964 6654 7261 6e73 666f 726d 6572  TfidfTransformer
+000112c0: 2c54 6669 6466 5665 6374 6f72 697a 6572  ,TfidfVectorizer
+000112d0: 0d0a 6672 6f6d 2073 6b6c 6561 726e 2e66  ..from sklearn.f
+000112e0: 6561 7475 7265 5f65 7874 7261 6374 696f  eature_extractio
+000112f0: 6e2e 7465 7874 2069 6d70 6f72 7420 436f  n.text import Co
+00011300: 756e 7456 6563 746f 7269 7a65 720d 0a23  untVectorizer..#
+00011310: 6e6c 746b 2e64 6f77 6e6c 6f61 6428 2770  nltk.download('p
+00011320: 756e 6b74 2729 0d0a 696d 706f 7274 2077  unkt')..import w
+00011330: 6172 6e69 6e67 730d 0a77 6172 6e69 6e67  arnings..warning
+00011340: 732e 6669 6c74 6572 7761 726e 696e 6773  s.filterwarnings
+00011350: 2822 6967 6e6f 7265 2229 0d0a 0d0a 236e  ("ignore")....#n
+00011360: 6c74 6b2e 646f 776e 6c6f 6164 2827 7374  ltk.download('st
+00011370: 6f70 776f 7264 7327 290d 0a0d 0a64 6566  opwords')....def
+00011380: 2067 6574 5f73 746f 705f 776f 7264 7328   get_stop_words(
+00011390: 293a 0d0a 2020 2020 2222 226c 6f61 6420  ):..    """load 
+000113a0: 7374 6f70 2077 6f72 6473 2022 2222 0d0a  stop words """..
+000113b0: 2020 2020 7265 7475 726e 2073 746f 7077      return stopw
+000113c0: 6f72 6473 2e77 6f72 6473 2827 656e 676c  ords.words('engl
+000113d0: 6973 6827 290d 0a20 2020 200d 0a23 2320  ish')..    ..## 
+000113e0: 2020 2077 6974 6820 6f70 656e 2827 7374     with open('st
+000113f0: 6f70 776f 7264 732e 7478 7427 2c20 2772  opwords.txt', 'r
+00011400: 272c 2065 6e63 6f64 696e 673d 2275 7466  ', encoding="utf
+00011410: 2d38 2229 2061 7320 663a 0d0a 2323 2020  -8") as f:..##  
+00011420: 2020 2020 2020 7374 6f70 776f 7264 7320        stopwords 
+00011430: 3d20 662e 7265 6164 6c69 6e65 7328 290d  = f.readlines().
+00011440: 0a23 2320 2020 2020 2020 2073 746f 705f  .##        stop_
+00011450: 7365 7420 3d20 7365 7428 6d2e 7374 7269  set = set(m.stri
+00011460: 7028 2920 666f 7220 6d20 696e 2073 746f  p() for m in sto
+00011470: 7077 6f72 6473 290d 0a23 2320 2020 2020  pwords)..##     
+00011480: 2023 2020 7072 696e 7428 6672 6f7a 656e   #  print(frozen
+00011490: 7365 7428 7374 6f70 5f73 6574 2929 0d0a  set(stop_set))..
+000114a0: 2323 2020 2020 2020 2020 7265 7475 726e  ##        return
+000114b0: 2066 726f 7a65 6e73 6574 2873 746f 705f   frozenset(stop_
+000114c0: 7365 7429 0d0a 0d0a 6465 6620 7363 7261  set)....def scra
+000114d0: 7065 7765 6228 7468 6575 726c 293a 0d0a  peweb(theurl):..
+000114e0: 2020 2020 7363 7261 7065 645f 6461 7461      scraped_data
+000114f0: 203d 2075 726c 6c69 622e 7265 7175 6573   = urllib.reques
+00011500: 742e 7572 6c6f 7065 6e28 7468 6575 726c  t.urlopen(theurl
+00011510: 2920 200d 0a20 2020 2061 7274 6963 6c65  )  ..    article
+00011520: 203d 2073 6372 6170 6564 5f64 6174 612e   = scraped_data.
+00011530: 7265 6164 2829 0d0a 0d0a 2020 2020 7061  read()....    pa
+00011540: 7273 6564 5f61 7274 6963 6c65 203d 2062  rsed_article = b
+00011550: 732e 4265 6175 7469 6675 6c53 6f75 7028  s.BeautifulSoup(
+00011560: 6172 7469 636c 652c 276c 786d 6c27 290d  article,'lxml').
+00011570: 0a0d 0a20 2020 2070 6172 6167 7261 7068  ...    paragraph
+00011580: 7320 3d20 7061 7273 6564 5f61 7274 6963  s = parsed_artic
+00011590: 6c65 2e66 696e 645f 616c 6c28 2770 2729  le.find_all('p')
+000115a0: 0d0a 0d0a 2020 2020 6172 7469 636c 655f  ....    article_
+000115b0: 7465 7874 203d 2022 220d 0a0d 0a20 2020  text = ""....   
+000115c0: 2066 6f72 2070 2069 6e20 7061 7261 6772   for p in paragr
+000115d0: 6170 6873 3a20 200d 0a20 2020 2020 2020  aphs:  ..       
+000115e0: 2061 7274 6963 6c65 5f74 6578 7420 2b3d   article_text +=
+000115f0: 2070 2e74 6578 740d 0a20 2020 2072 6574   p.text..    ret
+00011600: 7572 6e20 6172 7469 636c 655f 7465 7874  urn article_text
+00011610: 200d 0a0d 0a64 6566 2063 6f6e 7665 7274   ....def convert
+00011620: 746f 6c6f 7765 7263 6173 6528 6466 2c63  tolowercase(df,c
+00011630: 6f6c 293a 0d0a 2020 2020 2020 6466 5b63  ol):..      df[c
+00011640: 6f6c 5d20 3d20 6466 5b63 6f6c 5d2e 6170  ol] = df[col].ap
+00011650: 706c 7928 6c61 6d62 6461 2078 3a20 2220  ply(lambda x: " 
+00011660: 222e 6a6f 696e 2878 2e6c 6f77 6572 2829  ".join(x.lower()
+00011670: 2066 6f72 2078 2069 6e20 782e 7370 6c69   for x in x.spli
+00011680: 7428 2929 290d 0a20 2020 2020 2072 6574  t()))..      ret
+00011690: 7572 6e20 6466 0d0a 2020 2020 0d0a 6465  urn df..    ..de
+000116a0: 6620 7265 6d6f 7665 7075 6e63 7475 6174  f removepunctuat
+000116b0: 696f 6e28 6466 2c63 6f6c 293a 0d0a 2020  ion(df,col):..  
+000116c0: 2020 2020 6466 5b63 6f6c 5d20 3d20 6466      df[col] = df
+000116d0: 5b63 6f6c 5d2e 7374 722e 7265 706c 6163  [col].str.replac
+000116e0: 6528 275b 5e5c 775c 735d 272c 2727 290d  e('[^\w\s]','').
+000116f0: 0a20 2020 2020 2072 6574 7572 6e20 6466  .      return df
+00011700: 0d0a 0d0a 6465 6620 7265 6d6f 7665 7374  ....def removest
+00011710: 6f70 776f 7264 7328 6466 2c63 6f6c 293a  opwords(df,col):
+00011720: 0d0a 2020 2020 2020 7374 6f70 203d 2073  ..      stop = s
+00011730: 746f 7077 6f72 6473 2e77 6f72 6473 2827  topwords.words('
+00011740: 656e 676c 6973 6827 290d 0a20 2020 2020  english')..     
+00011750: 2064 665b 636f 6c5d 203d 2064 665b 636f   df[col] = df[co
+00011760: 6c5d 2e61 7070 6c79 286c 616d 6264 6120  l].apply(lambda 
+00011770: 783a 2022 2022 2e6a 6f69 6e28 7820 666f  x: " ".join(x fo
+00011780: 7220 7820 696e 2078 2e73 706c 6974 2829  r x in x.split()
+00011790: 2069 6620 7820 6e6f 7420 696e 2073 746f   if x not in sto
+000117a0: 7029 290d 0a20 2020 2020 2072 6574 7572  p))..      retur
+000117b0: 6e20 6466 0d0a 0d0a 6465 6620 7265 6d6f  n df....def remo
+000117c0: 7665 636f 6d6d 6f6e 776f 7264 7328 6466  vecommonwords(df
+000117d0: 2c63 6f6c 293a 0d0a 2020 2020 2020 6672  ,col):..      fr
+000117e0: 6571 203d 2070 642e 5365 7269 6573 2827  eq = pd.Series('
+000117f0: 2027 2e6a 6f69 6e28 6466 5b63 6f6c 5d29   '.join(df[col])
+00011800: 2e73 706c 6974 2829 292e 7661 6c75 655f  .split()).value_
+00011810: 636f 756e 7473 2829 5b3a 3130 5d0d 0a20  counts()[:10].. 
+00011820: 2020 2020 2066 7265 7120 3d20 6c69 7374       freq = list
+00011830: 2866 7265 712e 696e 6465 7829 0d0a 2020  (freq.index)..  
+00011840: 2020 2020 6466 5b63 6f6c 5d20 3d20 6466      df[col] = df
+00011850: 5b63 6f6c 5d2e 6170 706c 7928 6c61 6d62  [col].apply(lamb
+00011860: 6461 2078 3a20 2220 222e 6a6f 696e 2878  da x: " ".join(x
+00011870: 2066 6f72 2078 2069 6e20 782e 7370 6c69   for x in x.spli
+00011880: 7428 2920 6966 2078 206e 6f74 2069 6e20  t() if x not in 
+00011890: 6672 6571 2929 0d0a 2020 2020 2020 7265  freq))..      re
+000118a0: 7475 726e 2064 660d 0a0d 0a64 6566 2072  turn df....def r
+000118b0: 656d 6f76 6572 6172 6577 6f72 6473 2864  emoverarewords(d
+000118c0: 662c 636f 6c29 3a0d 0a20 2020 2020 2066  f,col):..      f
+000118d0: 7265 7120 3d20 7064 2e53 6572 6965 7328  req = pd.Series(
+000118e0: 2720 272e 6a6f 696e 2864 665b 636f 6c5d  ' '.join(df[col]
+000118f0: 292e 7370 6c69 7428 2929 2e76 616c 7565  ).split()).value
+00011900: 5f63 6f75 6e74 7328 295b 2d31 303a 5d0d  _counts()[-10:].
+00011910: 0a20 2020 2020 2066 7265 7120 3d20 6c69  .      freq = li
+00011920: 7374 2866 7265 712e 696e 6465 7829 0d0a  st(freq.index)..
+00011930: 2020 2020 2020 6466 5b63 6f6c 5d20 3d20        df[col] = 
+00011940: 6466 5b63 6f6c 5d2e 6170 706c 7928 6c61  df[col].apply(la
+00011950: 6d62 6461 2078 3a20 2220 222e 6a6f 696e  mbda x: " ".join
+00011960: 2878 2066 6f72 2078 2069 6e20 782e 7370  (x for x in x.sp
+00011970: 6c69 7428 2920 6966 2078 206e 6f74 2069  lit() if x not i
+00011980: 6e20 6672 6571 2929 0d0a 2020 2020 2020  n freq))..      
+00011990: 7265 7475 726e 2064 660d 0a0d 0a64 6566  return df....def
+000119a0: 2063 6f72 7265 6374 7370 656c 6c69 6e67   correctspelling
+000119b0: 2864 662c 636f 6c29 3a0d 0a20 2020 2020  (df,col):..     
+000119c0: 2064 665b 636f 6c5d 5b3a 355d 2e61 7070   df[col][:5].app
+000119d0: 6c79 286c 616d 6264 6120 783a 2073 7472  ly(lambda x: str
+000119e0: 2854 6578 7442 6c6f 6228 7829 2e63 6f72  (TextBlob(x).cor
+000119f0: 7265 6374 2829 2929 0d0a 2020 2020 2020  rect()))..      
+00011a00: 7265 7475 726e 2064 660d 0a0d 0a64 6566  return df....def
+00011a10: 206c 656d 6d61 7469 7a61 7469 6f6e 2864   lemmatization(d
+00011a20: 662c 636f 6c29 3a0d 0a20 2020 2020 2064  f,col):..      d
+00011a30: 665b 636f 6c5d 203d 2064 665b 636f 6c5d  f[col] = df[col]
+00011a40: 2e61 7070 6c79 286c 616d 6264 6120 783a  .apply(lambda x:
+00011a50: 2022 2022 2e6a 6f69 6e28 5b57 6f72 6428   " ".join([Word(
+00011a60: 776f 7264 292e 6c65 6d6d 6174 697a 6528  word).lemmatize(
+00011a70: 2920 666f 7220 776f 7264 2069 6e20 782e  ) for word in x.
+00011a80: 7370 6c69 7428 295d 2929 0d0a 2020 2020  split()]))..    
+00011a90: 2020 7265 7475 726e 2064 660d 0a0d 0a64    return df....d
+00011aa0: 6566 2074 7261 696e 7665 6374 2863 762c  ef trainvect(cv,
+00011ab0: 7462 6f77 2c64 662c 636f 6c2c 6d61 786b  tbow,df,col,maxk
+00011ac0: 6579 776f 7264 7329 3a0d 0a20 2020 2020  eywords):..     
+00011ad0: 2074 6578 743d 6466 5b63 6f6c 5d2e 746f   text=df[col].to
+00011ae0: 6c69 7374 2829 0d0a 2020 2020 2020 7466  list()..      tf
+00011af0: 6964 6620 3d20 5466 6964 6654 7261 6e73  idf = TfidfTrans
+00011b00: 666f 726d 6572 2873 6d6f 6f74 685f 6964  former(smooth_id
+00011b10: 663d 5472 7565 2c75 7365 5f69 6466 3d54  f=True,use_idf=T
+00011b20: 7275 6529 0d0a 2020 2020 2020 7466 6964  rue)..      tfid
+00011b30: 662e 6669 7428 7462 6f77 290d 0a20 2020  f.fit(tbow)..   
+00011b40: 2020 2074 665f 6964 665f 7665 6374 6f72     tf_idf_vector
+00011b50: 3d74 6669 6466 2e74 7261 6e73 666f 726d  =tfidf.transform
+00011b60: 2863 762e 7472 616e 7366 6f72 6d28 7465  (cv.transform(te
+00011b70: 7874 2929 0d0a 2020 2020 2020 736f 7274  xt))..      sort
+00011b80: 6564 6974 656d 733d 736f 7274 5f63 6f6f  editems=sort_coo
+00011b90: 2874 665f 6964 665f 7665 6374 6f72 2e74  (tf_idf_vector.t
+00011ba0: 6f63 6f6f 2829 290d 0a20 2020 2020 2066  ocoo())..      f
+00011bb0: 6561 7475 7265 6e61 6d65 733d 6376 2e67  eaturenames=cv.g
+00011bc0: 6574 5f66 6561 7475 7265 5f6e 616d 6573  et_feature_names
+00011bd0: 5f6f 7574 2829 0d0a 2020 2020 2020 6b65  _out()..      ke
+00011be0: 7977 6f72 6473 3d65 7874 7261 6374 5f74  ywords=extract_t
+00011bf0: 6f70 6e5f 6672 6f6d 5f76 6563 746f 7228  opn_from_vector(
+00011c00: 6665 6174 7572 656e 616d 6573 2c73 6f72  featurenames,sor
+00011c10: 7465 6469 7465 6d73 2c6d 6178 6b65 7977  teditems,maxkeyw
+00011c20: 6f72 6473 290d 0a20 2020 2020 206b 6579  ords)..      key
+00011c30: 776f 7264 733d 6a73 6f6e 2e64 756d 7073  words=json.dumps
+00011c40: 286b 6579 776f 7264 7329 0d0a 2020 2020  (keywords)..    
+00011c50: 2023 2070 7269 6e74 286b 6579 776f 7264   # print(keyword
+00011c60: 7329 0d0a 2020 2020 2020 7265 7475 726e  s)..      return
+00011c70: 206b 6579 776f 7264 730d 0a0d 0a64 6566   keywords....def
+00011c80: 2074 7261 696e 626f 7728 6466 2c63 6f6c   trainbow(df,col
+00011c90: 293a 0d0a 2020 2020 2020 6d79 6c69 7374  ):..      mylist
+00011ca0: 3d64 665b 636f 6c5d 2e74 6f6c 6973 7428  =df[col].tolist(
+00011cb0: 290d 0a20 2020 2020 2073 746f 7077 6f72  )..      stopwor
+00011cc0: 6473 3d67 6574 5f73 746f 705f 776f 7264  ds=get_stop_word
+00011cd0: 7328 290d 0a20 2020 2020 2063 7620 3d20  s()..      cv = 
+00011ce0: 436f 756e 7456 6563 746f 7269 7a65 7228  CountVectorizer(
+00011cf0: 7374 6f70 5f77 6f72 6473 3d73 746f 7077  stop_words=stopw
+00011d00: 6f72 6473 290d 0a20 2020 2020 2074 7261  ords)..      tra
+00011d10: 696e 5f62 6f77 203d 2063 762e 6669 745f  in_bow = cv.fit_
+00011d20: 7472 616e 7366 6f72 6d28 6d79 6c69 7374  transform(mylist
+00011d30: 290d 0a20 2020 2020 2023 7072 696e 7428  )..      #print(
+00011d40: 6c69 7374 2863 762e 766f 6361 6275 6c61  list(cv.vocabula
+00011d50: 7279 5f2e 6b65 7973 2829 2929 0d0a 2020  ry_.keys()))..  
+00011d60: 2020 2020 7265 7475 726e 2063 762c 7472      return cv,tr
+00011d70: 6169 6e5f 626f 770d 0a0d 0a20 0d0a 6465  ain_bow.... ..de
+00011d80: 6620 736f 7274 5f63 6f6f 2863 6f6f 5f6d  f sort_coo(coo_m
+00011d90: 6174 7269 7829 3a0d 0a20 2020 2074 7570  atrix):..    tup
+00011da0: 6c65 7320 3d20 7a69 7028 636f 6f5f 6d61  les = zip(coo_ma
+00011db0: 7472 6978 2e63 6f6c 2c20 636f 6f5f 6d61  trix.col, coo_ma
+00011dc0: 7472 6978 2e64 6174 6129 0d0a 2020 2020  trix.data)..    
+00011dd0: 7265 7475 726e 2073 6f72 7465 6428 7475  return sorted(tu
+00011de0: 706c 6573 2c20 6b65 793d 6c61 6d62 6461  ples, key=lambda
+00011df0: 2078 3a20 2878 5b31 5d2c 2078 5b30 5d29   x: (x[1], x[0])
+00011e00: 2c20 7265 7665 7273 653d 5472 7565 290d  , reverse=True).
+00011e10: 0a0d 0a64 6566 2065 7874 7261 6374 5f74  ...def extract_t
+00011e20: 6f70 6e5f 6672 6f6d 5f76 6563 746f 7228  opn_from_vector(
+00011e30: 6665 6174 7572 655f 6e61 6d65 732c 2073  feature_names, s
+00011e40: 6f72 7465 645f 6974 656d 732c 2074 6f70  orted_items, top
+00011e50: 6e3d 3130 293a 0d0a 2020 2020 2222 2267  n=10):..    """g
+00011e60: 6574 2074 6865 2066 6561 7475 7265 206e  et the feature n
+00011e70: 616d 6573 2061 6e64 2074 662d 6964 6620  ames and tf-idf 
+00011e80: 7363 6f72 6520 6f66 2074 6f70 206e 2069  score of top n i
+00011e90: 7465 6d73 2222 220d 0a20 2020 200d 0a20  tems"""..    .. 
+00011ea0: 2020 2023 7573 6520 6f6e 6c79 2074 6f70     #use only top
+00011eb0: 6e20 6974 656d 7320 6672 6f6d 2076 6563  n items from vec
+00011ec0: 746f 720d 0a20 2020 2073 6f72 7465 645f  tor..    sorted_
+00011ed0: 6974 656d 7320 3d20 736f 7274 6564 5f69  items = sorted_i
+00011ee0: 7465 6d73 5b3a 746f 706e 5d0d 0a0d 0a20  tems[:topn].... 
+00011ef0: 2020 2073 636f 7265 5f76 616c 7320 3d20     score_vals = 
+00011f00: 5b5d 0d0a 2020 2020 6665 6174 7572 655f  []..    feature_
+00011f10: 7661 6c73 203d 205b 5d0d 0a0d 0a20 2020  vals = []....   
+00011f20: 2066 6f72 2069 6478 2c20 7363 6f72 6520   for idx, score 
+00011f30: 696e 2073 6f72 7465 645f 6974 656d 733a  in sorted_items:
+00011f40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00011f50: 2020 2020 666e 616d 6520 3d20 6665 6174      fname = feat
+00011f60: 7572 655f 6e61 6d65 735b 6964 785d 0d0a  ure_names[idx]..
+00011f70: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00011f80: 2866 6e61 6d65 293e 333a 0d0a 2020 2020  (fname)>3:..    
+00011f90: 2020 2020 236b 6565 7020 7472 6163 6b20      #keep track 
+00011fa0: 6f66 2066 6561 7475 7265 206e 616d 6520  of feature name 
+00011fb0: 616e 6420 6974 7320 636f 7272 6573 706f  and its correspo
+00011fc0: 6e64 696e 6720 7363 6f72 650d 0a20 2020  nding score..   
+00011fd0: 2020 2020 2020 2020 2073 636f 7265 5f76           score_v
+00011fe0: 616c 732e 6170 7065 6e64 2872 6f75 6e64  als.append(round
+00011ff0: 2873 636f 7265 2c20 3329 290d 0a20 2020  (score, 3))..   
+00012000: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+00012010: 5f76 616c 732e 6170 7065 6e64 2866 6561  _vals.append(fea
+00012020: 7475 7265 5f6e 616d 6573 5b69 6478 5d29  ture_names[idx])
+00012030: 0d0a 0d0a 2020 2020 2363 7265 6174 6520  ....    #create 
+00012040: 6120 7475 706c 6573 206f 6620 6665 6174  a tuples of feat
+00012050: 7572 652c 7363 6f72 650d 0a20 2020 2023  ure,score..    #
+00012060: 7265 7375 6c74 7320 3d20 7a69 7028 6665  results = zip(fe
+00012070: 6174 7572 655f 7661 6c73 2c73 636f 7265  ature_vals,score
+00012080: 5f76 616c 7329 0d0a 2020 2020 7265 7375  _vals)..    resu
+00012090: 6c74 733d 207b 7d0d 0a20 2020 2066 6f72  lts= {}..    for
+000120a0: 2069 6478 2069 6e20 7261 6e67 6528 6c65   idx in range(le
+000120b0: 6e28 6665 6174 7572 655f 7661 6c73 2929  n(feature_vals))
+000120c0: 3a0d 0a20 2020 2020 2020 2072 6573 756c  :..        resul
+000120d0: 7473 5b66 6561 7475 7265 5f76 616c 735b  ts[feature_vals[
+000120e0: 6964 785d 5d3d 7363 6f72 655f 7661 6c73  idx]]=score_vals
+000120f0: 5b69 6478 5d0d 0a20 2020 200d 0a20 2020  [idx]..    ..   
+00012100: 2072 6574 7572 6e20 7265 7375 6c74 730d   return results.
+00012110: 0a0d 0a64 6566 2067 6574 6b65 7977 6f72  ...def getkeywor
+00012120: 6473 286d 7974 6578 742c 6d61 786b 6579  ds(mytext,maxkey
+00012130: 776f 7264 7329 3a0d 0a20 2020 2072 3d52  words):..    r=R
+00012140: 616b 6528 6d61 785f 6c65 6e67 7468 3d31  ake(max_length=1
+00012150: 3029 0d0a 2020 2020 7220 3d20 5261 6b65  0)..    r = Rake
+00012160: 2872 616e 6b69 6e67 5f6d 6574 7269 633d  (ranking_metric=
+00012170: 4d65 7472 6963 2e44 4547 5245 455f 544f  Metric.DEGREE_TO
+00012180: 5f46 5245 5155 454e 4359 5f52 4154 494f  _FREQUENCY_RATIO
+00012190: 290d 0a20 2020 2023 7220 3d20 5261 6b65  )..    #r = Rake
+000121a0: 2872 616e 6b69 6e67 5f6d 6574 7269 633d  (ranking_metric=
+000121b0: 4d65 7472 6963 2e57 4f52 445f 4445 4752  Metric.WORD_DEGR
+000121c0: 4545 290d 0a20 2020 2023 7220 3d20 5261  EE)..    #r = Ra
+000121d0: 6b65 2872 616e 6b69 6e67 5f6d 6574 7269  ke(ranking_metri
+000121e0: 633d 4d65 7472 6963 2e57 4f52 445f 4652  c=Metric.WORD_FR
+000121f0: 4551 5545 4e43 5929 0d0a 2020 2020 643d  EQUENCY)..    d=
+00012200: 7b27 696e 7075 7427 3a5b 6d79 7465 7874  {'input':[mytext
+00012210: 5d7d 0d0a 2020 2020 6466 203d 2070 642e  ]}..    df = pd.
+00012220: 4461 7461 4672 616d 6528 6429 0d0a 2020  DataFrame(d)..  
+00012230: 2020 6466 3d63 6f6e 7665 7274 746f 6c6f    df=converttolo
+00012240: 7765 7263 6173 6528 6466 2c27 696e 7075  wercase(df,'inpu
+00012250: 7427 290d 0a20 2020 2064 663d 7265 6d6f  t')..    df=remo
+00012260: 7665 7075 6e63 7475 6174 696f 6e28 6466  vepunctuation(df
+00012270: 2c27 696e 7075 7427 290d 0a20 2020 2064  ,'input')..    d
+00012280: 663d 7265 6d6f 7665 7374 6f70 776f 7264  f=removestopword
+00012290: 7328 6466 2c27 696e 7075 7427 290d 0a20  s(df,'input').. 
+000122a0: 2020 2064 663d 7265 6d6f 7665 636f 6d6d     df=removecomm
+000122b0: 6f6e 776f 7264 7328 6466 2c27 696e 7075  onwords(df,'inpu
+000122c0: 7427 290d 0a20 2020 2064 663d 7265 6d6f  t')..    df=remo
+000122d0: 7665 7261 7265 776f 7264 7328 6466 2c27  verarewords(df,'
+000122e0: 696e 7075 7427 290d 0a20 2020 2064 663d  input')..    df=
+000122f0: 636f 7272 6563 7473 7065 6c6c 696e 6728  correctspelling(
+00012300: 6466 2c27 696e 7075 7427 290d 0a20 2020  df,'input')..   
+00012310: 2064 663d 6c65 6d6d 6174 697a 6174 696f   df=lemmatizatio
+00012320: 6e28 6466 2c27 696e 7075 7427 290d 0a20  n(df,'input').. 
+00012330: 2020 206d 7974 6578 743d 6466 5b27 696e     mytext=df['in
+00012340: 7075 7427 5d5b 305d 0d0a 2020 2020 6376  put'][0]..    cv
+00012350: 2c74 773d 7472 6169 6e62 6f77 2864 662c  ,tw=trainbow(df,
+00012360: 2769 6e70 7574 2729 0d0a 2020 2020 6b65  'input')..    ke
+00012370: 7977 6f72 6473 3d74 7261 696e 7665 6374  ywords=trainvect
+00012380: 2863 762c 7477 2c64 662c 2769 6e70 7574  (cv,tw,df,'input
+00012390: 272c 6d61 786b 6579 776f 7264 7329 0d0a  ',maxkeywords)..
+000123a0: 0d0a 2020 2020 0d0a 2020 2020 6b65 7962  ..    ..    keyb
+000123b0: 7566 203d 2022 220d 0a20 2020 206b 6a73  uf = ""..    kjs
+000123c0: 6f6e 203d 206a 736f 6e2e 6c6f 6164 7328  on = json.loads(
+000123d0: 6b65 7977 6f72 6473 290d 0a20 2020 2066  keywords)..    f
+000123e0: 6f72 206b 6579 2c20 7661 6c75 6520 696e  or key, value in
+000123f0: 206b 6a73 6f6e 2e69 7465 6d73 2829 3a0d   kjson.items():.
+00012400: 0a20 2020 2020 2020 206b 6579 6275 6620  .        keybuf 
+00012410: 3d20 6b65 7962 7566 202b 206b 6579 202b  = keybuf + key +
+00012420: 222c 2220 2b20 7374 7228 7661 6c75 6529  "," + str(value)
+00012430: 202b 2022 3a22 0d0a 2020 2020 6b65 7962   + ":"..    keyb
+00012440: 7566 203d 206b 6579 6275 665b 3a2d 315d  uf = keybuf[:-1]
+00012450: 0d0a 0d0a 2020 2020 7265 7475 726e 206b  ....    return k
+00012460: 6579 6275 660d 0a20 0d0a 6465 6620 646f  eybuf.. ..def do
+00012470: 7375 6d6d 6172 7928 6172 7469 636c 655f  summary(article_
+00012480: 7465 7874 2c69 293a 0d0a 0d0a 0d0a 2020  text,i):......  
+00012490: 2020 6172 7469 636c 655f 7465 7874 203d    article_text =
+000124a0: 2072 652e 7375 6228 7227 5c5b 5b30 2d39   re.sub(r'\[[0-9
+000124b0: 5d2a 5c5d 272c 2027 2027 2c20 6172 7469  ]*\]', ' ', arti
+000124c0: 636c 655f 7465 7874 2920 200d 0a20 2020  cle_text)  ..   
+000124d0: 2061 7274 6963 6c65 5f74 6578 7420 3d20   article_text = 
+000124e0: 7265 2e73 7562 2872 275c 732b 272c 2027  re.sub(r'\s+', '
+000124f0: 2027 2c20 6172 7469 636c 655f 7465 7874   ', article_text
+00012500: 290d 0a0d 0a20 2020 2023 2052 656d 6f76  )....    # Remov
+00012510: 696e 6720 7370 6563 6961 6c20 6368 6172  ing special char
+00012520: 6163 7465 7273 2061 6e64 2064 6967 6974  acters and digit
+00012530: 730d 0a20 2020 2066 6f72 6d61 7474 6564  s..    formatted
+00012540: 5f61 7274 6963 6c65 5f74 6578 7420 3d20  _article_text = 
+00012550: 7265 2e73 7562 2827 5b5e 612d 7a41 2d5a  re.sub('[^a-zA-Z
+00012560: 5d27 2c20 2720 272c 2061 7274 6963 6c65  ]', ' ', article
+00012570: 5f74 6578 7420 2920 200d 0a20 2020 2066  _text )  ..    f
+00012580: 6f72 6d61 7474 6564 5f61 7274 6963 6c65  ormatted_article
+00012590: 5f74 6578 7420 3d20 7265 2e73 7562 2872  _text = re.sub(r
+000125a0: 275c 732b 272c 2027 2027 2c20 666f 726d  '\s+', ' ', form
+000125b0: 6174 7465 645f 6172 7469 636c 655f 7465  atted_article_te
+000125c0: 7874 2920 200d 0a0d 0a20 2020 2073 656e  xt)  ....    sen
+000125d0: 7465 6e63 655f 6c69 7374 203d 206e 6c74  tence_list = nlt
+000125e0: 6b2e 7365 6e74 5f74 6f6b 656e 697a 6528  k.sent_tokenize(
+000125f0: 6172 7469 636c 655f 7465 7874 2920 200d  article_text)  .
+00012600: 0a20 2020 2023 7072 696e 7428 7365 6e74  .    #print(sent
+00012610: 656e 6365 5f6c 6973 7429 0d0a 0d0a 2020  ence_list)....  
+00012620: 2020 7374 6f70 776f 7264 7320 3d20 6e6c    stopwords = nl
+00012630: 746b 2e63 6f72 7075 732e 7374 6f70 776f  tk.corpus.stopwo
+00012640: 7264 732e 776f 7264 7328 2765 6e67 6c69  rds.words('engli
+00012650: 7368 2729 0d0a 0d0a 2020 2020 776f 7264  sh')....    word
+00012660: 5f66 7265 7175 656e 6369 6573 203d 207b  _frequencies = {
+00012670: 7d20 200d 0a20 2020 2066 6f72 2077 6f72  }  ..    for wor
+00012680: 6420 696e 206e 6c74 6b2e 776f 7264 5f74  d in nltk.word_t
+00012690: 6f6b 656e 697a 6528 666f 726d 6174 7465  okenize(formatte
+000126a0: 645f 6172 7469 636c 655f 7465 7874 293a  d_article_text):
+000126b0: 2020 0d0a 2020 2020 2020 2020 6966 2077    ..        if w
+000126c0: 6f72 6420 6e6f 7420 696e 2073 746f 7077  ord not in stopw
+000126d0: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
+000126e0: 2020 2069 6620 776f 7264 206e 6f74 2069     if word not i
+000126f0: 6e20 776f 7264 5f66 7265 7175 656e 6369  n word_frequenci
+00012700: 6573 2e6b 6579 7328 293a 0d0a 2020 2020  es.keys():..    
+00012710: 2020 2020 2020 2020 2020 2020 776f 7264              word
+00012720: 5f66 7265 7175 656e 6369 6573 5b77 6f72  _frequencies[wor
+00012730: 645d 203d 2031 0d0a 2020 2020 2020 2020  d] = 1..        
+00012740: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00012750: 2020 2020 2020 2020 2020 2077 6f72 645f             word_
+00012760: 6672 6571 7565 6e63 6965 735b 776f 7264  frequencies[word
+00012770: 5d20 2b3d 2031 0d0a 0d0a 2020 2020 6d61  ] += 1....    ma
+00012780: 7869 6d75 6d5f 6672 6571 756e 6379 203d  ximum_frequncy =
+00012790: 206d 6178 2877 6f72 645f 6672 6571 7565   max(word_freque
+000127a0: 6e63 6965 732e 7661 6c75 6573 2829 290d  ncies.values()).
+000127b0: 0a0d 0a20 2020 2066 6f72 2077 6f72 6420  ...    for word 
+000127c0: 696e 2077 6f72 645f 6672 6571 7565 6e63  in word_frequenc
+000127d0: 6965 732e 6b65 7973 2829 3a20 200d 0a20  ies.keys():  .. 
+000127e0: 2020 2020 2020 2077 6f72 645f 6672 6571         word_freq
+000127f0: 7565 6e63 6965 735b 776f 7264 5d20 3d20  uencies[word] = 
+00012800: 2877 6f72 645f 6672 6571 7565 6e63 6965  (word_frequencie
+00012810: 735b 776f 7264 5d2f 6d61 7869 6d75 6d5f  s[word]/maximum_
+00012820: 6672 6571 756e 6379 290d 0a0d 0a20 2020  frequncy)....   
+00012830: 2023 7072 696e 7428 776f 7264 5f66 7265   #print(word_fre
+00012840: 7175 656e 6369 6573 290d 0a0d 0a20 2020  quencies)....   
+00012850: 2073 656e 7465 6e63 655f 7363 6f72 6573   sentence_scores
+00012860: 203d 207b 7d20 200d 0a20 2020 2066 6f72   = {}  ..    for
+00012870: 2073 656e 7420 696e 2073 656e 7465 6e63   sent in sentenc
+00012880: 655f 6c69 7374 3a20 200d 0a20 2020 2020  e_list:  ..     
+00012890: 2020 2066 6f72 2077 6f72 6420 696e 206e     for word in n
+000128a0: 6c74 6b2e 776f 7264 5f74 6f6b 656e 697a  ltk.word_tokeniz
+000128b0: 6528 7365 6e74 2e6c 6f77 6572 2829 293a  e(sent.lower()):
+000128c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000128d0: 2077 6f72 6420 696e 2077 6f72 645f 6672   word in word_fr
+000128e0: 6571 7565 6e63 6965 732e 6b65 7973 2829  equencies.keys()
+000128f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012900: 2020 2069 6620 6c65 6e28 7365 6e74 2e73     if len(sent.s
+00012910: 706c 6974 2827 2027 2929 203c 2032 353a  plit(' ')) < 25:
+00012920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012930: 2020 2020 2020 6966 2073 656e 7420 6e6f        if sent no
+00012940: 7420 696e 2073 656e 7465 6e63 655f 7363  t in sentence_sc
+00012950: 6f72 6573 2e6b 6579 7328 293a 0d0a 2020  ores.keys():..  
+00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012970: 2020 2020 2020 7365 6e74 656e 6365 5f73        sentence_s
+00012980: 636f 7265 735b 7365 6e74 5d20 3d20 776f  cores[sent] = wo
+00012990: 7264 5f66 7265 7175 656e 6369 6573 5b77  rd_frequencies[w
+000129a0: 6f72 645d 0d0a 2020 2020 2020 2020 2020  ord]..          
+000129b0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+000129c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000129d0: 2020 2020 2020 2020 2073 656e 7465 6e63           sentenc
+000129e0: 655f 7363 6f72 6573 5b73 656e 745d 202b  e_scores[sent] +
+000129f0: 3d20 776f 7264 5f66 7265 7175 656e 6369  = word_frequenci
+00012a00: 6573 5b77 6f72 645d 0d0a 0d0a 2020 2020  es[word]....    
+00012a10: 2370 7269 6e74 2873 656e 7465 6e63 655f  #print(sentence_
+00012a20: 7363 6f72 6573 290d 0a0d 0a20 2020 2073  scores)....    s
+00012a30: 756d 6d61 7279 5f73 656e 7465 6e63 6573  ummary_sentences
+00012a40: 203d 2068 6561 7071 2e6e 6c61 7267 6573   = heapq.nlarges
+00012a50: 7428 692c 2073 656e 7465 6e63 655f 7363  t(i, sentence_sc
+00012a60: 6f72 6573 2c20 6b65 793d 7365 6e74 656e  ores, key=senten
+00012a70: 6365 5f73 636f 7265 732e 6765 7429 0d0a  ce_scores.get)..
+00012a80: 2020 2020 2370 7269 6e74 2873 756d 6d61      #print(summa
+00012a90: 7279 5f73 656e 7465 6e63 6573 290d 0a20  ry_sentences).. 
+00012aa0: 2020 2073 756d 6d61 7279 203d 2027 2027     summary = ' '
+00012ab0: 2e6a 6f69 6e28 7375 6d6d 6172 795f 7365  .join(summary_se
+00012ac0: 6e74 656e 6365 7329 0d0a 2020 2020 2370  ntences)..    #p
+00012ad0: 7269 6e74 2822 4149 2053 756d 6d61 7279  rint("AI Summary
+00012ae0: 2229 0d0a 2020 2020 7265 7475 726e 2073  ")..    return s
+00012af0: 756d 6d61 7279 0d0a 0d0a 6465 6620 7374  ummary....def st
+00012b00: 6172 7473 756d 6d61 7279 2861 7274 6963  artsummary(artic
+00012b10: 6c65 5f74 6578 742c 6676 616c 7565 2c6d  le_text,fvalue,m
+00012b20: 6178 6b65 7977 6f72 6473 293a 0d0a 2020  axkeywords):..  
+00012b30: 2020 2020 0d0a 2023 2074 7279 3a0d 0a20      .. # try:.. 
+00012b40: 2020 6f72 6967 696e 616c 776f 7264 7320    originalwords 
+00012b50: 3d20 6c65 6e28 6172 7469 636c 655f 7465  = len(article_te
+00012b60: 7874 2e73 706c 6974 2822 2022 2929 0d0a  xt.split(" "))..
+00012b70: 0d0a 2020 2066 6f72 2069 2069 6e20 7261  ..   for i in ra
+00012b80: 6e67 6528 312c 3130 3030 3029 3a0d 0a20  nge(1,10000):.. 
+00012b90: 2020 2020 7375 6d6d 6172 793d 646f 7375      summary=dosu
+00012ba0: 6d6d 6172 7928 6172 7469 636c 655f 7465  mmary(article_te
+00012bb0: 7874 2c69 290d 0a20 2020 2020 7265 7320  xt,i)..     res 
+00012bc0: 3d20 6c65 6e28 7375 6d6d 6172 792e 7370  = len(summary.sp
+00012bd0: 6c69 7428 2929 0d0a 2020 2020 2069 6620  lit())..     if 
+00012be0: 7265 7320 3e3d 2066 7661 6c75 653a 0d0a  res >= fvalue:..
+00012bf0: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
+00012c00: 0d0a 2020 2073 756d 6d61 7279 203d 2020  ..   summary =  
+00012c10: 7265 2e73 7562 2822 5c5c 5c5c 785b 612d  re.sub("\\\\x[a-
+00012c20: 6630 2d39 5d5b 612d 6630 2d39 5d22 2c20  f0-9][a-f0-9]", 
+00012c30: 2220 222c 7375 6d6d 6172 7929 0d0a 2020  " ",summary)..  
+00012c40: 2073 756d 6d61 7279 203d 2072 652e 7375   summary = re.su
+00012c50: 6228 225c 5c78 6532 5c5c 7838 305c 5c78  b("\\xe2\\x80\\x
+00012c60: 3939 222c 2227 222c 2073 756d 6d61 7279  99","'", summary
+00012c70: 290d 0a20 2020 7375 6d6d 6172 793d 7375  )..   summary=su
+00012c80: 6d6d 6172 792e 7265 706c 6163 6528 225c  mmary.replace("\
+00012c90: 5c78 6532 5c5c 7838 305c 5c78 3939 222c  \xe2\\x80\\x99",
+00012ca0: 2227 2229 0d0a 2020 2073 756d 6d61 7279  "'")..   summary
+00012cb0: 3d73 756d 6d61 7279 2e72 6570 6c61 6365  =summary.replace
+00012cc0: 2822 5c5c 7865 325c 5c78 3830 5c5c 7839  ("\\xe2\\x80\\x9
+00012cd0: 3022 2c22 2d22 290d 0a20 2020 7375 6d6d  0","-")..   summ
+00012ce0: 6172 793d 7375 6d6d 6172 792e 7265 706c  ary=summary.repl
+00012cf0: 6163 6528 225c 5c78 6532 5c5c 7838 305c  ace("\\xe2\\x80\
+00012d00: 5c78 3931 222c 222d 2229 0d0a 2020 2073  \x91","-")..   s
+00012d10: 756d 6d61 7279 3d73 756d 6d61 7279 2e72  ummary=summary.r
+00012d20: 6570 6c61 6365 2822 5c5c 7865 325c 5c78  eplace("\\xe2\\x
+00012d30: 3830 5c5c 7839 3222 2c22 2d22 290d 0a20  80\\x92","-").. 
+00012d40: 2020 7375 6d6d 6172 793d 7375 6d6d 6172    summary=summar
+00012d50: 792e 7265 706c 6163 6528 225c 5c78 6532  y.replace("\\xe2
+00012d60: 5c5c 7838 305c 5c78 3933 222c 222d 2229  \\x80\\x93","-")
+00012d70: 0d0a 2020 2073 756d 6d61 7279 3d73 756d  ..   summary=sum
+00012d80: 6d61 7279 2e72 6570 6c61 6365 2822 5c5c  mary.replace("\\
+00012d90: 7865 325c 5c78 3830 5c5c 7839 3422 2c22  xe2\\x80\\x94","
+00012da0: 2d22 290d 0a20 2020 7375 6d6d 6172 793d  -")..   summary=
+00012db0: 7375 6d6d 6172 792e 7265 706c 6163 6528  summary.replace(
+00012dc0: 225c 5c78 6532 5c5c 7838 305c 5c78 3935  "\\xe2\\x80\\x95
+00012dd0: 222c 222d 2229 0d0a 2020 2073 756d 6d61  ","-")..   summa
+00012de0: 7279 3d73 756d 6d61 7279 2e72 6570 6c61  ry=summary.repla
+00012df0: 6365 2822 5c5c 7865 325c 5c78 3830 5c5c  ce("\\xe2\\x80\\
+00012e00: 7862 3322 2c27 2227 290d 0a20 2020 7375  xb3",'"')..   su
+00012e10: 6d6d 6172 7920 3d20 7375 6d6d 6172 792e  mmary = summary.
+00012e20: 7265 706c 6163 6528 27e2 809c 272c 2027  replace('...', '
+00012e30: 2227 290d 0a20 2020 7375 6d6d 6172 7920  "')..   summary 
+00012e40: 3d20 7375 6d6d 6172 792e 7265 706c 6163  = summary.replac
+00012e50: 6528 27e2 809d 272c 2027 2227 290d 0a20  e('...', '"').. 
+00012e60: 2020 7375 6d6d 6172 7920 3d20 7375 6d6d    summary = summ
+00012e70: 6172 792e 7265 706c 6163 6528 27e2 8099  ary.replace('...
+00012e80: 272c 2022 2722 290d 0a20 2020 7375 6d6d  ', "'")..   summ
+00012e90: 6172 7920 3d20 7375 6d6d 6172 792e 7265  ary = summary.re
+00012ea0: 706c 6163 6528 27e2 8098 272c 2022 2722  place('...', "'"
+00012eb0: 290d 0a20 2020 7375 6d6d 6172 7920 3d20  )..   summary = 
+00012ec0: 7375 6d6d 6172 792e 7265 706c 6163 6528  summary.replace(
+00012ed0: 27e2 8093 272c 2022 2d22 290d 0a20 2020  '...', "-")..   
+00012ee0: 7375 6d6d 6172 7920 3d20 7375 6d6d 6172  summary = summar
+00012ef0: 792e 7265 706c 6163 6528 27e2 80a6 272c  y.replace('...',
+00012f00: 2022 2e2e 2e22 290d 0a20 2020 7375 6d6d   "...")..   summ
+00012f10: 6172 7920 3d20 7375 6d6d 6172 792e 7265  ary = summary.re
+00012f20: 706c 6163 6528 27e2 8094 272c 2022 2d22  place('...', "-"
+00012f30: 290d 0a20 2020 7375 6d6d 6172 7920 3d20  )..   summary = 
+00012f40: 7375 6d6d 6172 792e 7265 706c 6163 6528  summary.replace(
+00012f50: 2722 272c 2022 2229 0d0a 0d0a 2020 2073  '"', "")....   s
+00012f60: 756d 6d61 7279 203d 2073 756d 6d61 7279  ummary = summary
+00012f70: 2e72 6570 6c61 6365 2827 5c5c 7527 2c27  .replace('\\u','
+00012f80: 552b 2729 0d0a 2020 2073 756d 6d61 7279  U+')..   summary
+00012f90: 203d 2072 652e 7375 6228 7227 3c55 5c2b   = re.sub(r'<U\+
+00012fa0: 285b 302d 3961 2d66 412d 465d 7b34 2c36  ([0-9a-fA-F]{4,6
+00012fb0: 7d29 3e27 2c20 6c61 6d62 6461 2078 3a20  })>', lambda x: 
+00012fc0: 6368 7228 696e 7428 782e 6772 6f75 7028  chr(int(x.group(
+00012fd0: 3129 2c31 3629 292c 2073 756d 6d61 7279  1),16)), summary
+00012fe0: 290d 0a0d 0a20 2020 6b65 7977 6f72 6473  )....   keywords
+00012ff0: 3d67 6574 6b65 7977 6f72 6473 2873 756d  =getkeywords(sum
+00013000: 6d61 7279 2c6d 6178 6b65 7977 6f72 6473  mary,maxkeywords
+00013010: 290d 0a0d 0a20 2020 7375 6d6d 6172 7977  )....   summaryw
+00013020: 6f72 6473 203d 206c 656e 2873 756d 6d61  ords = len(summa
+00013030: 7279 2e73 706c 6974 2822 2022 2929 0d0a  ry.split(" "))..
+00013040: 200d 0a20 2020 6d61 696e 6f75 743d 225c   ..   mainout="\
+00013050: 2222 202b 206b 6579 776f 7264 7320 2b20  "" + keywords + 
+00013060: 225c 222c 5c22 6f72 6967 696e 616c 776f  "\",\"originalwo
+00013070: 7264 636f 756e 745c 223a 2220 2b20 7374  rdcount\":" + st
+00013080: 7228 6f72 6967 696e 616c 776f 7264 7329  r(originalwords)
+00013090: 202b 2022 2c5c 2273 756d 6d61 7279 776f   + ",\"summarywo
+000130a0: 7264 636f 756e 745c 223a 222b 2073 7472  rdcount\":"+ str
+000130b0: 2873 756d 6d61 7279 776f 7264 7329 202b  (summarywords) +
+000130c0: 222c 5c22 6d61 696e 7375 6d6d 6172 795c  ",\"mainsummary\
+000130d0: 223a 7b5c 2273 756d 6d61 7279 5c22 3a20  ":{\"summary\": 
+000130e0: 5c22 2220 2b20 7375 6d6d 6172 7920 2b20  \"" + summary + 
+000130f0: 225c 227d 7d22 0d0a 2020 2072 6574 7572  "\"}}"..   retur
+00013100: 6e20 6d61 696e 6f75 740d 0a20 2020 0d0a  n mainout..   ..
+00013110: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013130: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013140: 230d 0a0d 0a66 726f 6d20 6c61 6e67 6368  #....from langch
+00013150: 6169 6e2e 656d 6265 6464 696e 6773 2e6f  ain.embeddings.o
+00013160: 7065 6e61 6920 696d 706f 7274 204f 7065  penai import Ope
+00013170: 6e41 4945 6d62 6564 6469 6e67 730d 0a66  nAIEmbeddings..f
+00013180: 726f 6d20 6c61 6e67 6368 6169 6e2e 7465  rom langchain.te
+00013190: 7874 5f73 706c 6974 7465 7220 696d 706f  xt_splitter impo
+000131a0: 7274 2043 6861 7261 6374 6572 5465 7874  rt CharacterText
+000131b0: 5370 6c69 7474 6572 0d0a 6672 6f6d 206c  Splitter..from l
+000131c0: 616e 6763 6861 696e 2e76 6563 746f 7273  angchain.vectors
+000131d0: 746f 7265 732e 6661 6973 7320 696d 706f  tores.faiss impo
+000131e0: 7274 2046 4149 5353 0d0a 0d0a 6672 6f6d  rt FAISS....from
+000131f0: 206c 616e 6763 6861 696e 2e63 6861 696e   langchain.chain
+00013200: 732e 7175 6573 7469 6f6e 5f61 6e73 7765  s.question_answe
+00013210: 7269 6e67 2069 6d70 6f72 7420 6c6f 6164  ring import load
+00013220: 5f71 615f 6368 6169 6e0d 0a66 726f 6d20  _qa_chain..from 
+00013230: 6c61 6e67 6368 6169 6e2e 6c6c 6d73 2069  langchain.llms i
+00013240: 6d70 6f72 7420 5072 6f6d 7074 4c61 7965  mport PromptLaye
+00013250: 724f 7065 6e41 4943 6861 740d 0a66 726f  rOpenAIChat..fro
+00013260: 6d20 6c61 6e67 6368 6169 6e2e 6368 6174  m langchain.chat
+00013270: 5f6d 6f64 656c 7320 696d 706f 7274 2043  _models import C
+00013280: 6861 744f 7065 6e41 490d 0a66 726f 6d20  hatOpenAI..from 
+00013290: 6c61 6e67 6368 6169 6e2e 6c6c 6d73 2069  langchain.llms i
+000132a0: 6d70 6f72 7420 4f70 656e 4149 0d0a 696d  mport OpenAI..im
+000132b0: 706f 7274 2068 6173 686c 6962 0d0a 0d0a  port hashlib....
+000132c0: 2320 416e 7377 6572 2071 7565 7374 696f  # Answer questio
+000132d0: 6e73 2061 626f 7574 2074 6865 2068 6561  ns about the hea
+000132e0: 646c 696e 6573 0d0a 6465 6620 7374 6172  dlines..def star
+000132f0: 745f 636f 6e76 6572 7361 7469 6f6e 286f  t_conversation(o
+00013300: 7065 6e61 696b 6579 2c71 7565 7279 2c74  penaikey,query,t
+00013310: 6578 742c 7465 6d70 6572 6174 7572 652c  ext,temperature,
+00013320: 6d6f 6465 6c29 3a0d 0a20 2020 2023 2047  model):..    # G
+00013330: 7261 6220 7468 6520 696e 7075 7420 6672  rab the input fr
+00013340: 6f6d 2074 6865 2041 5049 0d0a 2020 2020  om the API..    
+00013350: 2020 2020 2371 7565 7279 203d 2069 6e70      #query = inp
+00013360: 7574 735b 2271 7565 7279 220d 0a0d 0a0d  uts["query".....
+00013370: 0a20 2020 2020 2020 2074 6578 745f 7370  .        text_sp
+00013380: 6c69 7474 6572 203d 2043 6861 7261 6374  litter = Charact
+00013390: 6572 5465 7874 5370 6c69 7474 6572 280d  erTextSplitter(.
+000133a0: 0a20 2020 2020 2020 2020 2020 2073 6570  .            sep
+000133b0: 6172 6174 6f72 3d22 2022 2c0d 0a20 2020  arator=" ",..   
+000133c0: 2020 2020 2020 2020 2063 6875 6e6b 5f73           chunk_s
+000133d0: 697a 653d 3130 3030 2c0d 0a20 2020 2020  ize=1000,..     
+000133e0: 2020 2020 2020 2063 6875 6e6b 5f6f 7665         chunk_ove
+000133f0: 726c 6170 3d32 3030 2c0d 0a20 2020 2020  rlap=200,..     
+00013400: 2020 2020 2020 206c 656e 6774 685f 6675         length_fu
+00013410: 6e63 7469 6f6e 3d6c 656e 2c0d 0a20 2020  nction=len,..   
+00013420: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+00013430: 2020 7465 7874 7320 3d20 7465 7874 5f73    texts = text_s
+00013440: 706c 6974 7465 722e 7370 6c69 745f 7465  plitter.split_te
+00013450: 7874 2874 6578 7429 0d0a 2020 2020 2020  xt(text)..      
+00013460: 2020 656d 6265 6464 696e 6773 203d 204f    embeddings = O
+00013470: 7065 6e41 4945 6d62 6564 6469 6e67 7328  penAIEmbeddings(
+00013480: 290d 0a20 2020 2020 2020 2064 6f63 7365  )..        docse
+00013490: 6172 6368 203d 2046 4149 5353 2e66 726f  arch = FAISS.fro
+000134a0: 6d5f 7465 7874 7328 7465 7874 732c 2065  m_texts(texts, e
+000134b0: 6d62 6564 6469 6e67 7329 0d0a 2020 2020  mbeddings)..    
+000134c0: 2020 2020 646f 6373 203d 2064 6f63 7365      docs = docse
+000134d0: 6172 6368 2e73 696d 696c 6172 6974 795f  arch.similarity_
+000134e0: 7365 6172 6368 2871 7565 7279 290d 0a20  search(query).. 
+000134f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00013500: 2063 6861 696e 203d 206c 6f61 645f 7161   chain = load_qa
+00013510: 5f63 6861 696e 284f 7065 6e41 4928 6d6f  _chain(OpenAI(mo
+00013520: 6465 6c5f 6e61 6d65 3d6d 6f64 656c 2c20  del_name=model, 
+00013530: 7465 6d70 6572 6174 7572 653d 7465 6d70  temperature=temp
+00013540: 6572 6174 7572 652c 6f70 656e 6169 5f61  erature,openai_a
+00013550: 7069 5f6b 6579 3d6f 7065 6e61 696b 6579  pi_key=openaikey
+00013560: 292c 2063 6861 696e 5f74 7970 653d 2273  ), chain_type="s
+00013570: 7475 6666 2229 0d0a 2020 2020 2020 2020  tuff")..        
+00013580: 7265 7320 3d20 6368 6169 6e28 7b22 696e  res = chain({"in
+00013590: 7075 745f 646f 6375 6d65 6e74 7322 3a20  put_documents": 
+000135a0: 646f 6373 2c20 2271 7565 7374 696f 6e22  docs, "question"
+000135b0: 3a20 7175 6572 797d 2c20 7265 7475 726e  : query}, return
+000135c0: 5f6f 6e6c 795f 6f75 7470 7574 733d 5472  _only_outputs=Tr
+000135d0: 7565 290d 0a0d 0a20 2020 2020 2020 2023  ue)....        #
+000135e0: 7265 7475 726e 207b 2270 7265 6422 3a20  return {"pred": 
+000135f0: 7265 737d 0d0a 2020 2020 2020 2020 7265  res}..        re
+00013600: 7475 726e 2072 6573 0d0a 0d0a 2323 2323  turn res....####
+00013610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013640: 0d0a 6672 6f6d 2070 6466 7175 6572 7920  ..from pdfquery 
+00013650: 696d 706f 7274 2050 4446 5175 6572 790d  import PDFQuery.
+00013660: 0a69 6d70 6f72 7420 786d 6c74 6f64 6963  .import xmltodic
+00013670: 740d 0a0d 0a0d 0a64 6566 206c 6162 656c  t......def label
+00013680: 6669 656c 6473 2866 696c 656e 616d 652c  fields(filename,
+00013690: 6c61 6265 6c6e 616d 652c 6163 726f 7479  labelname,acroty
+000136a0: 7065 293a 0d0a 2020 2020 2070 6466 203d  pe):..     pdf =
+000136b0: 2050 4446 5175 6572 7928 6669 6c65 6e61   PDFQuery(filena
+000136c0: 6d65 290d 0a20 2020 2020 7064 662e 6c6f  me)..     pdf.lo
+000136d0: 6164 2829 0d0a 2020 2020 2023 4c54 5465  ad()..     #LTTe
+000136e0: 7874 4c69 6e65 486f 7269 7a6f 6e74 616c  xtLineHorizontal
+000136f0: 0d0a 2020 2020 206c 6162 656c 203d 2070  ..     label = p
+00013700: 6466 2e70 7128 6163 726f 7479 7065 2b27  df.pq(acrotype+'
+00013710: 3a63 6f6e 7461 696e 7328 2227 2b6c 6162  :contains("'+lab
+00013720: 656c 6e61 6d65 202b 2027 2229 2729 0d0a  elname + '")')..
+00013730: 2020 2020 206c 6566 745f 636f 726e 6572       left_corner
+00013740: 203d 2066 6c6f 6174 286c 6162 656c 2e61   = float(label.a
+00013750: 7474 7228 2778 3027 2929 0d0a 2020 2020  ttr('x0'))..    
+00013760: 2062 6f74 746f 6d5f 636f 726e 6572 203d   bottom_corner =
+00013770: 2066 6c6f 6174 286c 6162 656c 2e61 7474   float(label.att
+00013780: 7228 2779 3027 2929 0d0a 2020 2020 206e  r('y0'))..     n
+00013790: 616d 6520 3d20 7064 662e 7071 2861 6372  ame = pdf.pq(acr
+000137a0: 6f74 7970 6520 2b27 3a69 6e5f 6262 6f78  otype +':in_bbox
+000137b0: 2822 2573 2c20 2573 2c20 2573 2c20 2573  ("%s, %s, %s, %s
+000137c0: 2229 2720 2520 286c 6566 745f 636f 726e  ")' % (left_corn
+000137d0: 6572 2c20 626f 7474 6f6d 5f63 6f72 6e65  er, bottom_corne
+000137e0: 722d 3330 2c20 6c65 6674 5f63 6f72 6e65  r-30, left_corne
+000137f0: 722b 3135 302c 2062 6f74 746f 6d5f 636f  r+150, bottom_co
+00013800: 726e 6572 2929 2e74 6578 7428 290d 0a20  rner)).text().. 
+00013810: 2020 2020 7265 7475 726e 206e 616d 650d      return name.
+00013820: 0a0d 0a0d 0a64 6566 2065 7874 7261 6374  .....def extract
+00013830: 6669 656c 6473 2866 696c 656e 616d 6529  fields(filename)
+00013840: 3a0d 0a20 2020 2020 2023 7265 6164 2074  :..      #read t
+00013850: 6865 2050 4446 0d0a 2020 2020 2020 7064  he PDF..      pd
+00013860: 6620 3d20 5044 4651 7565 7279 2866 696c  f = PDFQuery(fil
+00013870: 656e 616d 6529 0d0a 2020 2020 2020 7064  ename)..      pd
+00013880: 662e 6c6f 6164 2829 0d0a 0d0a 2020 2020  f.load()....    
+00013890: 2020 236f 203d 2078 6d6c 746f 6469 6374    #o = xmltodict
+000138a0: 2e70 6172 7365 2827 3c65 3e20 3c61 3e74  .parse('<e> <a>t
+000138b0: 6578 743c 2f61 3e20 3c61 3e74 6578 743c  ext</a> <a>text<
+000138c0: 2f61 3e20 3c2f 653e 2729 0d0a 0d0a 2020  /a> </e>')....  
+000138d0: 2020 2020 2363 6f6e 7665 7274 2074 6865      #convert the
+000138e0: 2070 6466 2074 6f20 584d 4c0d 0a20 2020   pdf to XML..   
+000138f0: 2020 2078 6d6c 6669 6c65 3d20 6669 6c65     xmlfile= file
+00013900: 6e61 6d65 202b 2027 2e78 6d6c 270d 0a20  name + '.xml'.. 
+00013910: 2020 2020 2070 6466 2e74 7265 652e 7772       pdf.tree.wr
+00013920: 6974 6528 786d 6c66 696c 652c 2070 7265  ite(xmlfile, pre
+00013930: 7474 795f 7072 696e 7420 3d20 5472 7565  tty_print = True
+00013940: 290d 0a20 2020 2020 2077 6974 6820 6f70  )..      with op
+00013950: 656e 2878 6d6c 6669 6c65 2920 6173 2066  en(xmlfile) as f
+00013960: 3a20 7320 3d20 662e 7265 6164 2829 0d0a  : s = f.read()..
+00013970: 0d0a 2020 2020 2020 2370 7269 6e74 2873  ..      #print(s
+00013980: 290d 0a20 2020 2020 206a 736f 6e62 7566  )..      jsonbuf
+00013990: 3d78 6d6c 746f 6a73 6f6e 2873 2c78 6d6c  =xmltojson(s,xml
+000139a0: 6669 6c65 290d 0a0d 0a20 2020 2020 2072  file)....      r
+000139b0: 6574 7572 6e20 6a73 6f6e 6275 660d 0a20  eturn jsonbuf.. 
+000139c0: 2020 2020 200d 0a0d 0a64 6566 2078 6d6c       ....def xml
+000139d0: 746f 6a73 6f6e 2878 6d6c 6275 6666 6572  tojson(xmlbuffer
+000139e0: 2c78 6d6c 6669 6c65 293a 0d0a 0d0a 2020  ,xmlfile):....  
+000139f0: 2020 2020 6f20 3d20 786d 6c74 6f64 6963      o = xmltodic
+00013a00: 742e 7061 7273 6528 786d 6c62 7566 6665  t.parse(xmlbuffe
+00013a10: 7229 0d0a 2020 2020 2020 786d 6c6a 736f  r)..      xmljso
+00013a20: 6e3d 6a73 6f6e 2e64 756d 7073 286f 290d  n=json.dumps(o).
+00013a30: 0a20 2020 2020 2023 7072 696e 7428 786d  .      #print(xm
+00013a40: 6c6a 736f 6e29 0d0a 2020 2020 2020 7769  ljson)..      wi
+00013a50: 7468 206f 7065 6e28 786d 6c66 696c 6520  th open(xmlfile 
+00013a60: 2b20 272e 6a73 6f6e 272c 2277 2229 2061  + '.json',"w") a
+00013a70: 7320 663a 0d0a 2020 2020 2020 2020 662e  s f:..        f.
+00013a80: 7772 6974 6528 786d 6c6a 736f 6e29 0d0a  write(xmljson)..
+00013a90: 0d0a 2020 2020 2020 7265 7475 726e 2078  ..      return x
+00013aa0: 6d6c 6a73 6f6e 2020 0d0a 0d0a 2323 2323  mljson  ....####
+00013ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013ad0: 2323 2323 2323 2323 2323 230d 0a69 6d70  ###########..imp
+00013ae0: 6f72 7420 6561 7379 6f63 720d 0a69 6d70  ort easyocr..imp
+00013af0: 6f72 7420 7370 6565 6368 5f72 6563 6f67  ort speech_recog
+00013b00: 6e69 7469 6f6e 2061 7320 7372 0d0a 696d  nition as sr..im
+00013b10: 706f 7274 206d 6f76 6965 7079 2e65 6469  port moviepy.edi
+00013b20: 746f 7220 6173 206d 7065 0d0a 0d0a 6465  tor as mpe....de
+00013b30: 6620 636f 6e76 6572 7476 6964 656f 746f  f convertvideoto
+00013b40: 7465 7874 2866 696c 656e 616d 6529 3a0d  text(filename):.
+00013b50: 0a20 2020 2020 2020 2023 636f 6e76 6572  .        #conver
+00013b60: 7420 746f 2061 7564 696f 0d0a 2020 2020  t to audio..    
+00013b70: 2020 2020 7669 6465 6f20 3d20 6d70 652e      video = mpe.
+00013b80: 5669 6465 6f46 696c 6543 6c69 7028 6669  VideoFileClip(fi
+00013b90: 6c65 6e61 6d65 290d 0a20 2020 2020 2020  lename)..       
+00013ba0: 2061 7564 696f 6669 6c65 3d66 696c 656e   audiofile=filen
+00013bb0: 616d 6520 2b20 222e 7761 7622 0d0a 2020  ame + ".wav"..  
+00013bc0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00013bd0: 7669 6465 6f2e 6175 6469 6f2e 7772 6974  video.audio.writ
+00013be0: 655f 6175 6469 6f66 696c 6528 6175 6469  e_audiofile(audi
+00013bf0: 6f66 696c 6529 0d0a 2020 2020 2020 2020  ofile)..        
+00013c00: 7265 7375 6c74 203d 2061 7564 696f 746f  result = audioto
+00013c10: 7465 7874 2861 7564 696f 6669 6c65 290d  text(audiofile).
+00013c20: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00013c30: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00013c40: 0d0a 0d0a 6465 6620 6175 6469 6f74 6f74  ....def audiotot
+00013c50: 6578 7428 6669 6c65 6e61 6d65 293a 0d0a  ext(filename):..
+00013c60: 2020 2020 2020 2020 7220 3d20 7372 2e52          r = sr.R
+00013c70: 6563 6f67 6e69 7a65 7228 290d 0a20 2020  ecognizer()..   
+00013c80: 2020 2020 2061 7564 696f 203d 2073 722e       audio = sr.
+00013c90: 4175 6469 6f46 696c 6528 6669 6c65 6e61  AudioFile(filena
+00013ca0: 6d65 290d 0a20 2020 2020 2020 2077 6974  me)..        wit
+00013cb0: 6820 6175 6469 6f20 6173 2073 6f75 7263  h audio as sourc
+00013cc0: 653a 0d0a 2020 2020 2020 2020 2020 6175  e:..          au
+00013cd0: 6469 6f5f 6669 6c65 203d 2072 2e72 6563  dio_file = r.rec
+00013ce0: 6f72 6428 736f 7572 6365 290d 0a20 2020  ord(source)..   
+00013cf0: 2020 2020 2072 6573 756c 7420 3d20 722e       result = r.
+00013d00: 7265 636f 676e 697a 655f 676f 6f67 6c65  recognize_google
+00013d10: 2861 7564 696f 5f66 696c 6529 0d0a 2020  (audio_file)..  
+00013d20: 2020 2020 2020 7370 6565 6368 6669 6c65        speechfile
+00013d30: 203d 2066 696c 656e 616d 6520 2b20 272e   = filename + '.
+00013d40: 7370 6565 6368 2e74 7874 270d 0a20 2020  speech.txt'..   
+00013d50: 2020 2020 2077 6974 6820 6f70 656e 2866       with open(f
+00013d60: 696c 656e 616d 6520 2b20 272e 7370 6565  ilename + '.spee
+00013d70: 6368 2e74 7874 272c 6d6f 6465 203d 2777  ch.txt',mode ='w
+00013d80: 2729 2061 7320 6669 6c65 3a20 0d0a 2020  ') as file: ..  
+00013d90: 2020 2020 2020 2020 2066 696c 652e 7772           file.wr
+00013da0: 6974 6528 7265 7375 6c74 290d 0a0d 0a20  ite(result).... 
+00013db0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00013dc0: 7375 6c74 2020 200d 0a0d 0a0d 0a64 6566  sult   ......def
+00013dd0: 2064 6f6f 6372 6d61 696e 2866 696c 656e   doocrmain(filen
+00013de0: 616d 6529 3a0d 0a0d 0a20 2020 2072 6561  ame):....    rea
+00013df0: 6465 7220 3d20 6561 7379 6f63 722e 5265  der = easyocr.Re
+00013e00: 6164 6572 285b 2765 6e27 5d29 2020 200d  ader(['en'])   .
+00013e10: 0a20 2020 2062 6f75 6e64 203d 2072 6561  .    bound = rea
+00013e20: 6465 722e 7265 6164 7465 7874 2866 696c  der.readtext(fil
+00013e30: 656e 616d 6529 0d0a 2020 2020 7265 7475  ename)..    retu
+00013e40: 726e 2062 6f75 6e64 0d0a 2020 2020 0d0a  rn bound..    ..
+00013e50: 2366 696c 656e 616d 653d 2774 6573 742d  #filename='test-
+00013e60: 7461 782e 7064 6627 2020 2020 200d 0a23  tax.pdf'     ..#
+00013e70: 7064 666a 736f 6e3d 6578 7472 6163 7466  pdfjson=extractf
+00013e80: 6965 6c64 7328 6669 6c65 6e61 6d65 290d  ields(filename).
+00013e90: 0a23 6e61 6d65 7465 7874 3d6c 6162 656c  .#nametext=label
+00013ea0: 6669 656c 6473 2866 696c 656e 616d 652c  fields(filename,
+00013eb0: 2242 7573 696e 6573 7320 6e75 6d62 6572  "Business number
+00013ec0: 222c 224c 5454 6578 744c 696e 6548 6f72  ","LTTextLineHor
+00013ed0: 697a 6f6e 7461 6c22 290d 0a23 7072 696e  izontal")..#prin
+00013ee0: 7428 6e61 6d65 7465 7874 290d 0a0d 0a    t(nametext)....
```

### Comparing `maadstml-3.34/maadstml/tmltextsummary.py` & `maadstml-3.35/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.34/maadstml.egg-info/PKG-INFO` & `maadstml-3.35/maadstml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.34
+Version: 3.35
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -253,14 +253,23 @@
 
 - **viperexractpdffields**
   - Extracts fields from PDF file
 
 - **viperexractpdffieldbylabel**
   - Extracts fields from PDF file by label name.
 
+- **viperimagetotext**
+  - Extracts text from images like PNG, JPG, etc., which can then be streamed to kafka.
+
+- **viperaudiototext**
+  - Extracts text from audio files like WAV, etc., which can then be streamed to kafka.
+
+- **vipervideototext**
+  - Extracts text from video files like MP4, etc., which can then be streamed to kafka.
+
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
 
@@ -4585,7 +4594,37 @@
 - Label name in the PDF filename to search for.
 
 *pdffilename,labelname,arcotype* : string, required
 
 - Acrobyte tag in PDF i.e. LTTextLineHorizontal
 
 RETURNS: Value of the labelname - if any.
+
+**40. maadstml.viperimagetotext(imagefilename)**
+
+**Parameters:**	Extract text from images.
+
+*imagefilename* : string, required
+
+- Image filename like PNG, JPG etc.
+
+RETURNS: Text in image.
+
+**41. maadstml.vipervideototext(videofilename)**
+
+**Parameters:**	Extract text from video.
+
+*videofilename* : string, required
+
+- Video filename like MP4 etc.
+
+RETURNS: Text in video.
+
+**42. maadstml.viperaudiototext(audiofilename)**
+
+**Parameters:**	Extract text from audio
+
+*audiofilename* : string, required
+
+- Audio filename like WAV etc.
+
+RETURNS: Text in audio.
```

### Comparing `maadstml-3.34/setup.py` & `maadstml-3.35/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.34',
+    version='3.35',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

