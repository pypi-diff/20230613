# Comparing `tmp/self-unzip-html-0.1.1.tar.gz` & `tmp/self-unzip-html-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "self-unzip-html-0.1.1.tar", last modified: Mon Apr 18 13:10:18 2022, max compression
+gzip compressed data, was "self-unzip-html-0.1.2.tar", last modified: Tue Jun 13 10:14:42 2023, max compression
```

## Comparing `self-unzip-html-0.1.1.tar` & `self-unzip-html-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-04-18 13:10:18.102745 self-unzip-html-0.1.1/
--rw-r--r--   0 user      (1000) user      (1000)     1063 2022-04-18 13:02:23.000000 self-unzip-html-0.1.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)       63 2022-04-14 20:59:05.000000 self-unzip-html-0.1.1/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3035 2022-04-18 13:10:18.102745 self-unzip-html-0.1.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2435 2022-04-18 13:08:36.000000 self-unzip-html-0.1.1/README.md
--rw-r--r--   0 user      (1000) user      (1000)       85 2022-04-14 20:09:58.000000 self-unzip-html-0.1.1/pyproject.toml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-04-18 13:10:18.099411 self-unzip-html-0.1.1/python/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-04-18 13:10:18.099411 self-unzip-html-0.1.1/python/bin/
--rwxr-xr-x   0 user      (1000) user      (1000)      182 2022-04-14 21:00:06.000000 self-unzip-html-0.1.1/python/bin/self-unzip-html.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-04-18 13:10:18.099411 self-unzip-html-0.1.1/python/self_unzip_html/
--rwxr-xr-x   0 user      (1000) user      (1000)     2769 2022-04-14 20:29:13.000000 self-unzip-html-0.1.1/python/self_unzip_html/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     6130 2022-04-14 20:31:25.000000 self-unzip-html-0.1.1/python/self_unzip_html/template.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-04-18 13:10:18.102745 self-unzip-html-0.1.1/python/self_unzip_html.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3035 2022-04-18 13:10:17.000000 self-unzip-html-0.1.1/python/self_unzip_html.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      340 2022-04-18 13:10:18.000000 self-unzip-html-0.1.1/python/self_unzip_html.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-04-18 13:10:17.000000 self-unzip-html-0.1.1/python/self_unzip_html.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       16 2022-04-18 13:10:18.000000 self-unzip-html-0.1.1/python/self_unzip_html.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)      775 2022-04-18 13:10:18.102745 self-unzip-html-0.1.1/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-13 10:14:42.091955 self-unzip-html-0.1.2/
+-rw-r--r--   0 user       (501) staff       (20)     1063 2023-02-22 16:28:51.000000 self-unzip-html-0.1.2/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       63 2023-02-22 16:28:51.000000 self-unzip-html-0.1.2/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     4827 2023-06-13 10:14:42.092009 self-unzip-html-0.1.2/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     4221 2023-06-13 10:13:56.000000 self-unzip-html-0.1.2/README.md
+-rw-r--r--   0 user       (501) staff       (20)       85 2023-02-22 16:28:51.000000 self-unzip-html-0.1.2/pyproject.toml
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-13 10:14:42.089433 self-unzip-html-0.1.2/python/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-13 10:14:42.091132 self-unzip-html-0.1.2/python/self_unzip_html/
+-rwxr-xr-x   0 user       (501) staff       (20)     8825 2023-06-13 10:04:14.000000 self-unzip-html-0.1.2/python/self_unzip_html/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1817 2023-06-04 16:47:19.000000 self-unzip-html-0.1.2/python/self_unzip_html/crypto.py
+-rw-r--r--   0 user       (501) staff       (20)     6655 2023-06-11 16:47:40.000000 self-unzip-html-0.1.2/python/self_unzip_html/minified_js.py
+-rw-r--r--   0 user       (501) staff       (20)      819 2023-06-04 17:34:15.000000 self-unzip-html-0.1.2/python/self_unzip_html/template.html
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-13 10:14:42.091849 self-unzip-html-0.1.2/python/self_unzip_html.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     4827 2023-06-13 10:14:42.000000 self-unzip-html-0.1.2/python/self_unzip_html.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      430 2023-06-13 10:14:42.000000 self-unzip-html-0.1.2/python/self_unzip_html.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-06-13 10:14:42.000000 self-unzip-html-0.1.2/python/self_unzip_html.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       99 2023-06-13 10:14:42.000000 self-unzip-html-0.1.2/python/self_unzip_html.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       16 2023-06-13 10:14:42.000000 self-unzip-html-0.1.2/python/self_unzip_html.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)      885 2023-06-13 10:14:42.092260 self-unzip-html-0.1.2/setup.cfg
```

### Comparing `self-unzip-html-0.1.1/LICENSE` & `self-unzip-html-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `self-unzip-html-0.1.1/PKG-INFO` & `self-unzip-html-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: self-unzip-html
-Version: 0.1.1
-Summary: Create self-extracting HTML pages with arbitrary contents
+Version: 0.1.2
+Summary: Create self-extracting and/or password protected HTML pages with arbitrary contents
 Home-page: https://github.com/six-two/self-unzip.html
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -23,46 +22,90 @@
 
 This [repo](https://github.com/six-two/self-unzip.html) contains tools to create self-extracting HTML pages.
 It works by taking a payload, compressing it, and encoding the results using ASCII85.
 It then puts the resulting string in a template file, that contains the code to decode and decompress the payload again.
 
 Currently there are three actions implemented, that can be executed, after the payload is decoded:
 
-- Execute payload as JavaScript code (example usecase: obfuscate malicious JS code)
-- Show payload as HTML page (example usecase: compress a big web page)
-- Download the payload as a file (example usecase: bypass antivirus / filters)
+- `eval`: Execute payload as JavaScript code (example usecase: obfuscate malicious JS code)
+- `replace`: Show payload as HTML page (example usecase: compress a big web page)
+- `download`: Download the payload as a file (example usecase: bypass antivirus / filters)
 
 ## Demo
 
 You can try the online demo at [self-extracting-html.six-two.dev](https://self-extracting-html.six-two.dev/).
 This version is the same as the web version described below.
 It is entirely client-site, your files do not get uploaded to a server.
 
 ## Installation
 
+### Current feature comparision
+
+Currently the python version has the most features.
+
+Feature | Web version | Python version
+---|---|---
+Base64 encoding | no | yes
+Ascii85 encoding | yes | yes
+GZIP compression | yes, always | yes, can be disabled
+AES-GCM encryption | no | yes
+Automatic detection of most efficient algorithms | no | yes
+
 ### Web version
 
 There is a bare-bones page generator written in plain HTML and JavaScript.
 To use it, just clone the repo and put the contents of the `site` directory somewhere in your web server directory.
 
+You can of course also use it with Python's built in web server:
+```bash
+python3 -m http.server --directory ./site/
+```
+
 ### Python version
 
 A Python script to generate self extracting web pages is under `python/main.py`.
-It just requires a modern Python version (probably Python3.9+) and has no external dependencies.
+It just requires a modern Python version (probably Python3.9+) and has no required external dependencies (but you need to install `pycryptodomex` if you want to encrypt contents).
 
 You can also install it with `pip`:
 
+```bash
+python3 -m pip install -U self-unzip-html
 ```
-python3 -m pip install self-unzip-html
+
+Example usage of the pip package:
+```bash
+self-unzip-html -t download -o psexec.html ~/Downloads/SysinternalsSuite/PsExec.exe
 ```
 
+Or if you wanted to password-protect it:
+```bash
+self-unzip-html -t download -o psexec.html -p YourPasswordHere ~/Downloads/SysinternalsSuite/PsExec.exe
+```
+
+## Encryption
+
+Encryption uses AES-GCM for encryption and tamper detection and PBKDF2 with slightly over 1 million rounds of SHA-256 for password derivation.
+The code has not been audited, so use it with caution.
+If data security is very important to you may want to manually encrypt it beforehand (for example using `gpg`).
+
+You can automatically decrypt a page by adding the password as the hash in a URL like `encrypted.html#monkey123!`.
+The hash will not be sent to the server, so your password may only be stored locally (in your browsing history).
+Otherwise a prompt will ask you for the password.
+
+## JavaScript code
 
-## template.html
+### Python
 
-This basically just explains, how I generated the obfuscated script in `template.html`.
+The JavaScript code is modular to decrease size and allow mixing and matching different algorithms.
+The unminified files are in `code_to_minify/`.
+They are minified by running `code_to_minify/build.sh`, which updates `python/self_unzip_html/minified_js.py`.
+
+### template.html
+
+This basically just explains, how I generated the obfuscated script in `template.html` (JavaScript version).
 In case you are paranoid, you can reproduce the steps.
 Or if there is an important update to `fflate` or `ascii85`, I will have to run them again.
 
 Install with npm:
 
 ```bash
 npm install .
@@ -79,9 +122,7 @@
 The next step is optional.
 If you want to skip it, just rename `main.min.js` to `main.js` in the `output` directory.
 Otherwise minify the code (may require you to install an external minifier like closure-compiler).
 
 ```bash
 closure-compiler output/main.js --js_output_file output/main.min.js
 ```
-
-
```

### Comparing `self-unzip-html-0.1.1/python/self_unzip_html/template.html` & `self-unzip-html-0.1.2/python/self_unzip_html/minified_js.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,384 +1,416 @@
-00000000: 3c21 444f 4354 5950 4520 6874 6d6c 3e0a  <!DOCTYPE html>.
-00000010: 3c68 746d 6c20 6c61 6e67 3d22 656e 223e  <html lang="en">
-00000020: 0a3c 6865 6164 3e0a 2020 2020 3c6d 6574  .<head>.    <met
-00000030: 6120 6368 6172 7365 743d 2255 5446 2d38  a charset="UTF-8
-00000040: 223e 0a20 2020 203c 6d65 7461 2068 7474  ">.    <meta htt
-00000050: 702d 6571 7569 763d 2258 2d55 412d 436f  p-equiv="X-UA-Co
-00000060: 6d70 6174 6962 6c65 2220 636f 6e74 656e  mpatible" conten
-00000070: 743d 2249 453d 6564 6765 223e 0a20 2020  t="IE=edge">.   
-00000080: 203c 6d65 7461 206e 616d 653d 2276 6965   <meta name="vie
-00000090: 7770 6f72 7422 2063 6f6e 7465 6e74 3d22  wport" content="
-000000a0: 7769 6474 683d 6465 7669 6365 2d77 6964  width=device-wid
-000000b0: 7468 2c20 696e 6974 6961 6c2d 7363 616c  th, initial-scal
-000000c0: 653d 312e 3022 3e0a 2020 2020 3c74 6974  e=1.0">.    <tit
-000000d0: 6c65 3e53 656c 6620 4578 7472 6163 7469  le>Self Extracti
-000000e0: 6e67 2050 6167 653c 2f74 6974 6c65 3e0a  ng Page</title>.
-000000f0: 3c2f 6865 6164 3e0a 3c62 6f64 793e 0a20  </head>.<body>. 
-00000100: 2020 203c 6831 3e55 6e70 6163 6b69 6e67     <h1>Unpacking
-00000110: 2e2e 2e3c 2f68 313e 0a20 2020 203c 703e  ...</h1>.    <p>
-00000120: 4966 2079 6f75 2063 616e 2072 6561 6420  If you can read 
-00000130: 7468 6973 2c20 7468 6520 6578 7472 6163  this, the extrac
-00000140: 7469 6f6e 2070 726f 6261 626c 7920 6469  tion probably di
-00000150: 6420 6e6f 7420 776f 726b 2e0a 2020 2020  d not work..    
-00000160: 506c 6561 7365 2064 6973 6162 6c65 2070  Please disable p
-00000170: 6c75 6769 6e73 2028 7375 6368 2061 7320  lugins (such as 
-00000180: 4e6f 5363 7269 7074 292c 2077 6869 6368  NoScript), which
-00000190: 206d 6179 2062 6c6f 636b 2074 6869 7320   may block this 
-000001a0: 7061 6765 2066 726f 6d20 7275 6e6e 696e  page from runnin
-000001b0: 6720 7468 6520 6578 7472 6163 7469 6f6e  g the extraction
-000001c0: 2063 6f64 652e 3c2f 703e 0a20 2020 203c   code.</p>.    <
-000001d0: 703e 4966 2079 6f75 2068 6176 6520 736f  p>If you have so
-000001e0: 6d65 2065 7870 6572 6965 6e63 6520 7769  me experience wi
-000001f0: 7468 2048 544d 4c2c 206f 7065 6e20 796f  th HTML, open yo
-00000200: 7572 2062 726f 7773 6572 7320 636f 6e73  ur browsers cons
-00000210: 6f6c 6520 616e 6420 616e 6420 6368 6563  ole and and chec
-00000220: 6b20 7768 6174 2074 6865 2065 726f 6f72  k what the eroor
-00000230: 206d 6573 7361 6765 2073 6179 732e 0a20   message says.. 
-00000240: 2020 204d 6179 6265 2069 7427 7320 6561     Maybe it's ea
-00000250: 7369 6c79 2066 6978 6162 6c65 203b 293c  sily fixable ;)<
-00000260: 2f70 3e0a 0a20 2020 203c 7363 7269 7074  /p>..    <script
-00000270: 3e0a 2020 2020 2f2f 2043 6f6e 7461 696e  >.    // Contain
-00000280: 7320 6d69 6e69 6669 6564 2063 6f64 6520  s minified code 
-00000290: 6672 6f6d 3a0a 2020 2020 2f2f 202d 2068  from:.    // - h
-000002a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000002b0: 6d2f 3130 3161 7272 6f77 7a2f 6666 6c61  m/101arrowz/ffla
-000002c0: 7465 2c20 4d49 5420 4c69 6365 6e73 652c  te, MIT License,
-000002d0: 2043 6f70 7972 6967 6874 2028 6329 2032   Copyright (c) 2
-000002e0: 3032 3020 4172 6a75 6e20 4261 7272 6574  020 Arjun Barret
-000002f0: 740a 2020 2020 2f2f 202d 2068 7474 7073  t.    // - https
-00000300: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e45  ://github.com/nE
-00000310: 3073 4967 6854 2f61 7363 6969 3835 2e6a  0sIghT/ascii85.j
-00000320: 732c 204d 4954 204c 6963 656e 7365 2c20  s, MIT License, 
-00000330: 436f 7079 7269 6768 7420 2843 2920 3230  Copyright (C) 20
-00000340: 3138 2020 5975 7269 204b 6f6e 6f74 6f70  18  Yuri Konotop
-00000350: 6f76 2028 d0ae d180 d0b8 d0b9 20d0 9ad0  ov (........ ...
-00000360: bed0 bdd0 bed1 82d0 bed0 bfd0 bed0 b229  ...............)
-00000370: 203c 796b 6f6e 6f74 6f70 6f76 4067 6e6f   <ykonotopov@gno
-00000380: 6d65 2e6f 7267 3e0a 2020 2020 2866 756e  me.org>.    (fun
-00000390: 6374 696f 6e28 297b 6675 6e63 7469 6f6e  ction(){function
-000003a0: 2053 2861 2c63 3d34 297b 6c65 7420 623d   S(a,c=4){let b=
-000003b0: 6e65 7720 5569 6e74 3841 7272 6179 2863  new Uint8Array(c
-000003c0: 293b 666f 7228 6c65 7420 653d 303b 653c  );for(let e=0;e<
-000003d0: 633b 652b 2b29 625b 655d 3d61 3e3e 545b  c;e++)b[e]=a>>T[
-000003e0: 655d 2632 3535 3b72 6574 7572 6e20 627d  e]&255;return b}
-000003f0: 6675 6e63 7469 6f6e 2055 2861 297b 6675  function U(a){fu
-00000400: 6e63 7469 6f6e 2063 2829 7b6c 6574 2064  nction c(){let d
-00000410: 3d53 2867 2c70 2d31 293b 666f 7228 6c65  =S(g,p-1);for(le
-00000420: 7420 683d 303b 683c 642e 6c65 6e67 7468  t h=0;h<d.length
-00000430: 3b68 2b2b 2962 2e70 7573 6828 645b 685d  ;h++)b.push(d[h]
-00000440: 293b 673d 703d 307d 6c65 7420 623d 5b5d  );g=p=0}let b=[]
-00000450: 3b76 6172 2065 3d21 313b 6c65 7420 673d  ;var e=!1;let g=
-00000460: 302c 703d 302c 713d 612e 7374 6172 7473  0,p=0,q=a.starts
-00000470: 5769 7468 2822 3c7e 2229 2626 323c 612e  With("<~")&&2<a.
-00000480: 6c65 6e67 7468 3f32 3a30 3b64 6f20 6966  length?2:0;do if
-00000490: 2830 213d 3d61 2e63 6861 7241 7428 7129  (0!==a.charAt(q)
-000004a0: 2e74 7269 6d28 292e 6c65 6e67 7468 297b  .trim().length){
-000004b0: 7661 7220 6d3d 612e 6368 6172 436f 6465  var m=a.charCode
-000004c0: 4174 2871 293b 7377 6974 6368 286d 297b  At(q);switch(m){
-000004d0: 6361 7365 2031 3232 3a30 213d 7026 2663  case 122:0!=p&&c
-000004e0: 6f6e 736f 6c65 2e65 7272 6f72 2822 556e  onsole.error("Un
-000004f0: 6578 7065 6374 6564 2027 7a27 2063 6861  expected 'z' cha
-00000500: 7261 6374 6572 2061 7420 706f 7369 7469  racter at positi
-00000510: 6f6e 2022 2b71 293b 666f 7228 6d3d 303b  on "+q);for(m=0;
-00000520: 343e 6d3b 6d2b 2b29 622e 7075 7368 2830  4>m;m++)b.push(0
-00000530: 293b 6272 6561 6b3b 6361 7365 2031 3236  );break;case 126
-00000540: 3a65 3d22 223b 666f 7228 6d3d 712b 313b  :e="";for(m=q+1;
-00000550: 6d3c 612e 6c65 6e67 7468 2626 303d 3d65  m<a.length&&0==e
-00000560: 2e74 7269 6d28 292e 6c65 6e67 7468 3b29  .trim().length;)
-00000570: 653d 612e 6368 6172 4174 286d 2b2b 293b  e=a.charAt(m++);
-00000580: 223e 2221 3d0a 2020 2020 6526 2663 6f6e  ">"!=.    e&&con
-00000590: 736f 6c65 2e65 7272 6f72 2822 4272 6f6b  sole.error("Brok
-000005a0: 656e 2045 4f44 2061 7420 706f 7369 7469  en EOD at positi
-000005b0: 6f6e 2022 2b6d 293b 7026 2628 672b 3d4c  on "+m);p&&(g+=L
-000005c0: 5b70 2d31 5d2c 6328 2929 3b65 3d21 303b  [p-1],c());e=!0;
-000005d0: 6272 6561 6b3b 6465 6661 756c 743a 2833  break;default:(3
-000005e0: 333e 6d7c 7c31 3137 3c6d 2926 2663 6f6e  3>m||117<m)&&con
-000005f0: 736f 6c65 2e65 7272 6f72 2822 556e 6578  sole.error("Unex
-00000600: 7065 6374 6564 2063 6861 7261 6374 6572  pected character
-00000610: 2077 6974 6820 636f 6465 2022 2b6d 2b22   with code "+m+"
-00000620: 2061 7420 706f 7369 7469 6f6e 2022 2b71   at position "+q
-00000630: 292c 672b 3d28 6d2d 3333 292a 4c5b 702b  ),g+=(m-33)*L[p+
-00000640: 2b5d 2c35 3c3d 7026 2663 2829 7d7d 7768  +],5<=p&&c()}}wh
-00000650: 696c 6528 712b 2b3c 612e 6c65 6e67 7468  ile(q++<a.length
-00000660: 2626 2165 293b 7265 7475 726e 206e 6577  &&!e);return new
-00000670: 2055 696e 7438 4172 7261 7928 6229 7d76   Uint8Array(b)}v
-00000680: 6172 2072 3d55 696e 7438 4172 7261 792c  ar r=Uint8Array,
-00000690: 433d 5569 6e74 3136 4172 7261 792c 4d3d  C=Uint16Array,M=
-000006a0: 5569 6e74 3332 4172 7261 792c 4e3d 6e65  Uint32Array,N=ne
-000006b0: 7720 7228 5b30 2c30 2c30 2c30 2c30 2c30  w r([0,0,0,0,0,0
-000006c0: 2c30 2c30 2c31 2c31 2c31 2c31 2c32 2c32  ,0,0,1,1,1,1,2,2
-000006d0: 2c32 2c32 2c33 2c33 2c33 2c33 2c34 2c34  ,2,2,3,3,3,3,4,4
-000006e0: 2c34 2c34 2c35 2c35 2c35 2c35 2c30 2c30  ,4,4,5,5,5,5,0,0
-000006f0: 2c30 2c30 5d29 2c4f 3d6e 6577 2072 285b  ,0,0]),O=new r([
-00000700: 302c 302c 302c 302c 312c 312c 322c 322c  0,0,0,0,1,1,2,2,
-00000710: 332c 332c 342c 342c 352c 352c 362c 362c  3,3,4,4,5,5,6,6,
-00000720: 372c 372c 382c 382c 392c 392c 3130 2c31  7,7,8,8,9,9,10,1
-00000730: 302c 3131 2c31 312c 3132 2c31 322c 3133  0,11,11,12,12,13
-00000740: 2c31 332c 302c 305d 292c 563d 6e65 7720  ,13,0,0]),V=new 
-00000750: 7228 5b31 362c 3137 2c31 382c 302c 382c  r([16,17,18,0,8,
-00000760: 372c 392c 362c 3130 2c35 2c31 312c 342c  7,9,6,10,5,11,4,
-00000770: 3132 2c33 2c31 332c 322c 3134 2c31 2c0a  12,3,13,2,14,1,.
-00000780: 2020 2020 3135 5d29 2c6b 3d66 756e 6374      15]),k=funct
-00000790: 696f 6e28 612c 6329 7b66 6f72 2876 6172  ion(a,c){for(var
-000007a0: 2062 3d6e 6577 2043 2833 3129 2c65 3d30   b=new C(31),e=0
-000007b0: 3b33 313e 653b 2b2b 6529 625b 655d 3d63  ;31>e;++e)b[e]=c
-000007c0: 2b3d 313c 3c61 5b65 2d31 5d3b 613d 6e65  +=1<<a[e-1];a=ne
-000007d0: 7720 4d28 625b 3330 5d29 3b66 6f72 2865  w M(b[30]);for(e
-000007e0: 3d31 3b33 303e 653b 2b2b 6529 666f 7228  =1;30>e;++e)for(
-000007f0: 633d 625b 655d 3b63 3c62 5b65 2b31 5d3b  c=b[e];c<b[e+1];
-00000800: 2b2b 6329 615b 635d 3d63 2d62 5b65 5d3c  ++c)a[c]=c-b[e]<
-00000810: 3c35 7c65 3b72 6574 7572 6e5b 622c 615d  <5|e;return[b,a]
-00000820: 7d2c 6c3d 6b28 4e2c 3229 2c50 3d6c 5b30  },l=k(N,2),P=l[0
-00000830: 5d3b 6c3d 6c5b 315d 3b50 5b32 385d 3d32  ];l=l[1];P[28]=2
-00000840: 3538 3b6c 5b32 3538 5d3d 3238 3b76 6172  58;l[258]=28;var
-00000850: 2057 3d6b 284f 2c30 295b 305d 2c46 3d6e   W=k(O,0)[0],F=n
-00000860: 6577 2043 2833 3237 3638 293b 666f 7228  ew C(32768);for(
-00000870: 6b3d 303b 3332 3736 383e 6b3b 2b2b 6b29  k=0;32768>k;++k)
-00000880: 6c3d 286b 2634 3336 3930 293e 3e3e 317c  l=(k&43690)>>>1|
-00000890: 286b 2632 3138 3435 293c 3c31 2c6c 3d28  (k&21845)<<1,l=(
-000008a0: 6c26 3532 3432 3829 3e3e 3e32 7c28 6c26  l&52428)>>>2|(l&
-000008b0: 3133 3130 3729 3c3c 322c 6c3d 286c 2636  13107)<<2,l=(l&6
-000008c0: 3136 3830 293e 3e3e 347c 286c 2633 3835  1680)>>>4|(l&385
-000008d0: 3529 3c3c 342c 465b 6b5d 3d28 286c 2636  5)<<4,F[k]=((l&6
-000008e0: 3532 3830 293e 3e3e 387c 286c 2632 3535  5280)>>>8|(l&255
-000008f0: 293c 3c38 293e 3e3e 313b 7661 7220 443d  )<<8)>>>1;var D=
-00000900: 6675 6e63 7469 6f6e 2861 2c63 2c62 297b  function(a,c,b){
-00000910: 666f 7228 7661 7220 653d 612e 6c65 6e67  for(var e=a.leng
-00000920: 7468 2c67 3d30 2c70 3d6e 6577 2043 2863  th,g=0,p=new C(c
-00000930: 293b 673c 653b 2b2b 6729 615b 675d 2626  );g<e;++g)a[g]&&
-00000940: 2b2b 705b 615b 675d 2d31 5d3b 7661 7220  ++p[a[g]-1];var 
-00000950: 713d 6e65 7720 4328 6329 3b66 6f72 2867  q=new C(c);for(g
-00000960: 3d30 3b67 3c63 3b2b 2b67 2971 5b67 5d3d  =0;g<c;++g)q[g]=
-00000970: 715b 672d 315d 2b70 5b67 2d0a 2020 2020  q[g-1]+p[g-.    
-00000980: 315d 3c3c 313b 6966 2862 2966 6f72 2862  1]<<1;if(b)for(b
-00000990: 3d6e 6577 2043 2831 3c3c 6329 2c70 3d31  =new C(1<<c),p=1
-000009a0: 352d 632c 673d 303b 673c 653b 2b2b 6729  5-c,g=0;g<e;++g)
-000009b0: 7b69 6628 615b 675d 297b 7661 7220 6d3d  {if(a[g]){var m=
-000009c0: 673c 3c34 7c61 5b67 5d2c 643d 632d 615b  g<<4|a[g],d=c-a[
-000009d0: 675d 2c68 3d71 5b61 5b67 5d2d 315d 2b2b  g],h=q[a[g]-1]++
-000009e0: 3c3c 643b 666f 7228 643d 687c 2831 3c3c  <<d;for(d=h|(1<<
-000009f0: 6429 2d31 3b68 3c3d 643b 2b2b 6829 625b  d)-1;h<=d;++h)b[
-00000a00: 465b 685d 3e3e 3e70 5d3d 6d7d 7d65 6c73  F[h]>>>p]=m}}els
-00000a10: 6520 666f 7228 623d 6e65 7720 4328 6529  e for(b=new C(e)
-00000a20: 2c67 3d30 3b67 3c65 3b2b 2b67 2961 5b67  ,g=0;g<e;++g)a[g
-00000a30: 5d26 2628 625b 675d 3d46 5b71 5b61 5b67  ]&&(b[g]=F[q[a[g
-00000a40: 5d2d 315d 2b2b 5d3e 3e3e 3135 2d61 5b67  ]-1]++]>>>15-a[g
-00000a50: 5d29 3b72 6574 7572 6e20 627d 3b6c 3d6e  ]);return b};l=n
-00000a60: 6577 2072 2832 3838 293b 666f 7228 6b3d  ew r(288);for(k=
-00000a70: 303b 3134 343e 6b3b 2b2b 6b29 6c5b 6b5d  0;144>k;++k)l[k]
-00000a80: 3d38 3b66 6f72 286b 3d31 3434 3b32 3536  =8;for(k=144;256
-00000a90: 3e6b 3b2b 2b6b 296c 5b6b 5d3d 393b 666f  >k;++k)l[k]=9;fo
-00000aa0: 7228 6b3d 3235 363b 3238 303e 6b3b 2b2b  r(k=256;280>k;++
-00000ab0: 6b29 6c5b 6b5d 3d37 3b66 6f72 286b 3d32  k)l[k]=7;for(k=2
-00000ac0: 3830 3b32 3838 3e6b 3b2b 2b6b 296c 5b6b  80;288>k;++k)l[k
-00000ad0: 5d3d 383b 7661 7220 513d 6e65 7720 7228  ]=8;var Q=new r(
-00000ae0: 3332 293b 666f 7228 6b3d 303b 3332 3e6b  32);for(k=0;32>k
-00000af0: 3b2b 2b6b 2951 5b6b 5d3d 353b 7661 7220  ;++k)Q[k]=5;var 
-00000b00: 583d 4428 6c2c 392c 3129 2c59 3d44 2851  X=D(l,9,1),Y=D(Q
-00000b10: 2c35 2c31 292c 473d 6675 6e63 7469 6f6e  ,5,1),G=function
-00000b20: 2861 297b 666f 7228 7661 7220 633d 615b  (a){for(var c=a[
-00000b30: 305d 2c62 3d31 3b62 3c61 2e6c 656e 6774  0],b=1;b<a.lengt
-00000b40: 683b 2b2b 6229 615b 625d 3e63 2626 2863  h;++b)a[b]>c&&(c
-00000b50: 3d61 5b62 5d29 3b72 6574 7572 6e20 637d  =a[b]);return c}
-00000b60: 2c76 3d66 756e 6374 696f 6e28 612c 632c  ,v=function(a,c,
-00000b70: 6229 7b76 6172 2065 3d0a 2020 2020 632f  b){var e=.    c/
-00000b80: 387c 303b 7265 7475 726e 2861 5b65 5d7c  8|0;return(a[e]|
-00000b90: 615b 652b 315d 3c3c 3829 3e3e 2863 2637  a[e+1]<<8)>>(c&7
-00000ba0: 2926 627d 2c48 3d66 756e 6374 696f 6e28  )&b},H=function(
-00000bb0: 612c 6329 7b76 6172 2062 3d63 2f38 7c30  a,c){var b=c/8|0
-00000bc0: 3b72 6574 7572 6e28 615b 625d 7c61 5b62  ;return(a[b]|a[b
-00000bd0: 2b31 5d3c 3c38 7c61 5b62 2b32 5d3c 3c31  +1]<<8|a[b+2]<<1
-00000be0: 3629 3e3e 2863 2637 297d 2c5a 3d66 756e  6)>>(c&7)},Z=fun
-00000bf0: 6374 696f 6e28 612c 632c 6229 7b69 6628  ction(a,c,b){if(
-00000c00: 6e75 6c6c 3d3d 637c 7c30 3e63 2963 3d30  null==c||0>c)c=0
-00000c10: 3b69 6628 6e75 6c6c 3d3d 627c 7c62 3e61  ;if(null==b||b>a
-00000c20: 2e6c 656e 6774 6829 623d 612e 6c65 6e67  .length)b=a.leng
-00000c30: 7468 3b76 6172 2065 3d6e 6577 2028 323d  th;var e=new (2=
-00000c40: 3d61 2e42 5954 4553 5f50 4552 5f45 4c45  =a.BYTES_PER_ELE
-00000c50: 4d45 4e54 3f43 3a34 3d3d 612e 4259 5445  MENT?C:4==a.BYTE
-00000c60: 535f 5045 525f 454c 454d 454e 543f 4d3a  S_PER_ELEMENT?M:
-00000c70: 7229 2862 2d63 293b 652e 7365 7428 612e  r)(b-c);e.set(a.
-00000c80: 7375 6261 7272 6179 2863 2c62 2929 3b72  subarray(c,b));r
-00000c90: 6574 7572 6e20 657d 2c61 613d 5b22 756e  eturn e},aa=["un
-00000ca0: 6578 7065 6374 6564 2045 4f46 222c 2269  expected EOF","i
-00000cb0: 6e76 616c 6964 2062 6c6f 636b 2074 7970  nvalid block typ
-00000cc0: 6522 2c22 696e 7661 6c69 6420 6c65 6e67  e","invalid leng
-00000cd0: 7468 2f6c 6974 6572 616c 222c 2269 6e76  th/literal","inv
-00000ce0: 616c 6964 2064 6973 7461 6e63 6522 2c22  alid distance","
-00000cf0: 7374 7265 616d 2066 696e 6973 6865 6422  stream finished"
-00000d00: 2c22 6e6f 2073 7472 6561 6d20 6861 6e64  ,"no stream hand
-00000d10: 6c65 7222 2c2c 226e 6f20 6361 6c6c 6261  ler",,"no callba
-00000d20: 636b 222c 2269 6e76 616c 6964 2055 5446  ck","invalid UTF
-00000d30: 2d38 2064 6174 6122 2c22 6578 7472 6120  -8 data","extra 
-00000d40: 6669 656c 6420 746f 6f20 6c6f 6e67 222c  field too long",
-00000d50: 2264 6174 6520 6e6f 7420 696e 2072 616e  "date not in ran
-00000d60: 6765 2031 3938 302d 3230 3939 222c 2266  ge 1980-2099","f
-00000d70: 696c 656e 616d 6520 746f 6f20 6c6f 6e67  ilename too long
-00000d80: 222c 0a20 2020 2022 7374 7265 616d 2066  ",.    "stream f
-00000d90: 696e 6973 6869 6e67 222c 2269 6e76 616c  inishing","inval
-00000da0: 6964 207a 6970 2064 6174 6122 5d2c 773d  id zip data"],w=
-00000db0: 6675 6e63 7469 6f6e 2861 2c63 2c62 297b  function(a,c,b){
-00000dc0: 633d 4572 726f 7228 637c 7c61 615b 615d  c=Error(c||aa[a]
-00000dd0: 293b 632e 636f 6465 3d61 3b45 7272 6f72  );c.code=a;Error
-00000de0: 2e63 6170 7475 7265 5374 6163 6b54 7261  .captureStackTra
-00000df0: 6365 2626 4572 726f 722e 6361 7074 7572  ce&&Error.captur
-00000e00: 6553 7461 636b 5472 6163 6528 632c 7729  eStackTrace(c,w)
-00000e10: 3b69 6628 2162 2974 6872 6f77 2063 3b72  ;if(!b)throw c;r
-00000e20: 6574 7572 6e20 637d 2c4b 3d66 756e 6374  eturn c},K=funct
-00000e30: 696f 6e28 612c 632c 6229 7b76 6172 2065  ion(a,c,b){var e
-00000e40: 3d61 2e6c 656e 6774 683b 6966 2821 657c  =a.length;if(!e|
-00000e50: 7c62 2626 622e 6626 2621 622e 6c29 7265  |b&&b.f&&!b.l)re
-00000e60: 7475 726e 2063 7c7c 6e65 7720 7228 3029  turn c||new r(0)
-00000e70: 3b76 6172 2067 3d21 637c 7c62 2c70 3d21  ;var g=!c||b,p=!
-00000e80: 627c 7c62 2e69 3b62 7c7c 3d7b 7d3b 637c  b||b.i;b||={};c|
-00000e90: 7c3d 6e65 7720 7228 332a 6529 3b76 6172  |=new r(3*e);var
-00000ea0: 2071 3d66 756e 6374 696f 6e28 4529 7b76   q=function(E){v
-00000eb0: 6172 2052 3d63 2e6c 656e 6774 683b 453e  ar R=c.length;E>
-00000ec0: 5226 2628 453d 6e65 7720 7228 4d61 7468  R&&(E=new r(Math
-00000ed0: 2e6d 6178 2832 2a52 2c45 2929 2c45 2e73  .max(2*R,E)),E.s
-00000ee0: 6574 2863 292c 633d 4529 7d2c 6d3d 622e  et(c),c=E)},m=b.
-00000ef0: 667c 7c30 2c64 3d62 2e70 7c7c 302c 683d  f||0,d=b.p||0,h=
-00000f00: 622e 627c 7c30 2c74 3d62 2e6c 2c79 3d62  b.b||0,t=b.l,y=b
-00000f10: 2e64 2c7a 3d62 2e6d 2c78 3d62 2e6e 2c49  .d,z=b.m,x=b.n,I
-00000f20: 3d38 2a65 3b64 6f7b 6966 2821 7429 7b6d  =8*e;do{if(!t){m
-00000f30: 3d76 2861 2c64 2c31 293b 7661 7220 663d  =v(a,d,1);var f=
-00000f40: 7628 612c 642b 312c 3329 3b64 2b3d 333b  v(a,d+1,3);d+=3;
-00000f50: 6966 2866 2969 6628 313d 3d66 2974 3d58  if(f)if(1==f)t=X
-00000f60: 2c79 3d59 2c7a 3d39 2c78 3d35 3b65 6c73  ,y=Y,z=9,x=5;els
-00000f70: 6520 6966 2832 3d3d 6629 7b7a 3d0a 2020  e if(2==f){z=.  
-00000f80: 2020 7628 612c 642c 3331 292b 3235 373b    v(a,d,31)+257;
-00000f90: 793d 7628 612c 642b 3130 2c31 3529 2b34  y=v(a,d+10,15)+4
-00000fa0: 3b74 3d7a 2b76 2861 2c64 2b35 2c33 3129  ;t=z+v(a,d+5,31)
-00000fb0: 2b31 3b64 2b3d 3134 3b78 3d6e 6577 2072  +1;d+=14;x=new r
-00000fc0: 2874 293b 7661 7220 6e3d 6e65 7720 7228  (t);var n=new r(
-00000fd0: 3139 293b 666f 7228 663d 303b 663c 793b  19);for(f=0;f<y;
-00000fe0: 2b2b 6629 6e5b 565b 665d 5d3d 7628 612c  ++f)n[V[f]]=v(a,
-00000ff0: 642b 332a 662c 3729 3b64 2b3d 332a 793b  d+3*f,7);d+=3*y;
-00001000: 663d 4728 6e29 3b79 3d28 313c 3c66 292d  f=G(n);y=(1<<f)-
-00001010: 313b 7661 7220 4a3d 4428 6e2c 662c 3129  1;var J=D(n,f,1)
-00001020: 3b66 6f72 2866 3d30 3b66 3c74 3b29 6966  ;for(f=0;f<t;)if
-00001030: 286e 3d4a 5b76 2861 2c64 2c79 295d 2c64  (n=J[v(a,d,y)],d
-00001040: 2b3d 6e26 3135 2c75 3d6e 3e3e 3e34 2c31  +=n&15,u=n>>>4,1
-00001050: 363e 7529 785b 662b 2b5d 3d75 3b65 6c73  6>u)x[f++]=u;els
-00001060: 657b 7661 7220 423d 6e3d 303b 3136 3d3d  e{var B=n=0;16==
-00001070: 753f 2842 3d33 2b76 2861 2c64 2c33 292c  u?(B=3+v(a,d,3),
-00001080: 642b 3d32 2c6e 3d78 5b66 2d31 5d29 3a31  d+=2,n=x[f-1]):1
-00001090: 373d 3d75 3f28 423d 332b 7628 612c 642c  7==u?(B=3+v(a,d,
-000010a0: 3729 2c64 2b3d 3329 3a31 383d 3d75 2626  7),d+=3):18==u&&
-000010b0: 2842 3d31 312b 7628 612c 642c 3132 3729  (B=11+v(a,d,127)
-000010c0: 2c64 2b3d 3729 3b66 6f72 283b 422d 2d3b  ,d+=7);for(;B--;
-000010d0: 2978 5b66 2b2b 5d3d 6e7d 743d 782e 7375  )x[f++]=n}t=x.su
-000010e0: 6261 7272 6179 2830 2c7a 293b 663d 782e  barray(0,z);f=x.
-000010f0: 7375 6261 7272 6179 287a 293b 7a3d 4728  subarray(z);z=G(
-00001100: 7429 3b78 3d47 2866 293b 743d 4428 742c  t);x=G(f);t=D(t,
-00001110: 7a2c 3129 3b79 3d44 2866 2c78 2c31 297d  z,1);y=D(f,x,1)}
-00001120: 656c 7365 2077 2831 293b 656c 7365 7b76  else w(1);else{v
-00001130: 6172 2075 3d28 2864 2b37 292f 387c 3029  ar u=((d+7)/8|0)
-00001140: 2b34 3b64 3d61 5b75 2d34 5d7c 615b 752d  +4;d=a[u-4]|a[u-
-00001150: 335d 3c3c 383b 663d 752b 643b 6966 2866  3]<<8;f=u+d;if(f
-00001160: 3e65 297b 7026 2677 2830 293b 6272 6561  >e){p&&w(0);brea
-00001170: 6b7d 6726 2671 2868 2b0a 2020 2020 6429  k}g&&q(h+.    d)
-00001180: 3b63 2e73 6574 2861 2e73 7562 6172 7261  ;c.set(a.subarra
-00001190: 7928 752c 6629 2c68 293b 622e 623d 682b  y(u,f),h);b.b=h+
-000011a0: 3d64 3b62 2e70 3d64 3d38 2a66 3b62 2e66  =d;b.p=d=8*f;b.f
-000011b0: 3d6d 3b63 6f6e 7469 6e75 657d 6966 2864  =m;continue}if(d
-000011c0: 3e49 297b 7026 2677 2830 293b 6272 6561  >I){p&&w(0);brea
-000011d0: 6b7d 7d67 2626 7128 682b 3133 3130 3732  k}}g&&q(h+131072
-000011e0: 293b 753d 2831 3c3c 7a29 2d31 3b4a 3d28  );u=(1<<z)-1;J=(
-000011f0: 313c 3c78 292d 313b 666f 7228 423d 643b  1<<x)-1;for(B=d;
-00001200: 3b42 3d64 297b 6e3d 745b 4828 612c 6429  ;B=d){n=t[H(a,d)
-00001210: 2675 5d3b 663d 6e3e 3e3e 343b 642b 3d6e  &u];f=n>>>4;d+=n
-00001220: 2631 353b 6966 2864 3e49 297b 7026 2677  &15;if(d>I){p&&w
-00001230: 2830 293b 6272 6561 6b7d 6e7c 7c77 2832  (0);break}n||w(2
-00001240: 293b 6966 2832 3536 3e66 2963 5b68 2b2b  );if(256>f)c[h++
-00001250: 5d3d 663b 656c 7365 2069 6628 3235 363d  ]=f;else if(256=
-00001260: 3d66 297b 423d 643b 743d 6e75 6c6c 3b62  =f){B=d;t=null;b
-00001270: 7265 616b 7d65 6c73 657b 6e3d 662d 3235  reak}else{n=f-25
-00001280: 343b 6966 2832 3634 3c66 297b 662d 3d32  4;if(264<f){f-=2
-00001290: 3537 3b76 6172 2041 3d4e 5b66 5d3b 6e3d  57;var A=N[f];n=
-000012a0: 7628 612c 642c 2831 3c3c 4129 2d31 292b  v(a,d,(1<<A)-1)+
-000012b0: 505b 665d 3b64 2b3d 417d 663d 795b 4828  P[f];d+=A}f=y[H(
-000012c0: 612c 6429 264a 5d3b 413d 663e 3e3e 343b  a,d)&J];A=f>>>4;
-000012d0: 667c 7c77 2833 293b 642b 3d66 2631 353b  f||w(3);d+=f&15;
-000012e0: 663d 575b 415d 3b33 3c41 2626 2841 3d4f  f=W[A];3<A&&(A=O
-000012f0: 5b41 5d2c 662b 3d48 2861 2c64 2926 2831  [A],f+=H(a,d)&(1
-00001300: 3c3c 4129 2d31 2c64 2b3d 4129 3b69 6628  <<A)-1,d+=A);if(
-00001310: 643e 4929 7b70 2626 7728 3029 3b62 7265  d>I){p&&w(0);bre
-00001320: 616b 7d67 2626 7128 682b 3133 3130 3732  ak}g&&q(h+131072
-00001330: 293b 666f 7228 6e3d 682b 6e3b 683c 6e3b  );for(n=h+n;h<n;
-00001340: 682b 3d34 2963 5b68 5d3d 635b 682d 665d  h+=4)c[h]=c[h-f]
-00001350: 2c63 5b68 2b31 5d3d 635b 682b 312d 665d  ,c[h+1]=c[h+1-f]
-00001360: 2c63 5b68 2b32 5d3d 635b 682b 322d 665d  ,c[h+2]=c[h+2-f]
-00001370: 2c63 5b68 2b0a 2020 2020 335d 3d63 5b68  ,c[h+.    3]=c[h
-00001380: 2b33 2d66 5d3b 683d 6e7d 7d62 2e6c 3d74  +3-f];h=n}}b.l=t
-00001390: 3b62 2e70 3d42 3b62 2e62 3d68 3b62 2e66  ;b.p=B;b.b=h;b.f
-000013a0: 3d6d 3b74 2626 286d 3d31 2c62 2e6d 3d7a  =m;t&&(m=1,b.m=z
-000013b0: 2c62 2e64 3d79 2c62 2e6e 3d78 297d 7768  ,b.d=y,b.n=x)}wh
-000013c0: 696c 6528 216d 293b 7265 7475 726e 2068  ile(!m);return h
-000013d0: 3d3d 632e 6c65 6e67 7468 3f63 3a5a 2863  ==c.length?c:Z(c
-000013e0: 2c30 2c68 297d 3b6b 3d6e 6577 2072 2830  ,0,h)};k=new r(0
-000013f0: 293b 6c3d 2275 6e64 6566 696e 6564 2221  );l="undefined"!
-00001400: 3d74 7970 656f 6620 5465 7874 4465 636f  =typeof TextDeco
-00001410: 6465 7226 266e 6577 2054 6578 7444 6563  der&&new TextDec
-00001420: 6f64 6572 3b74 7279 7b6c 2e64 6563 6f64  oder;try{l.decod
-00001430: 6528 6b2c 7b73 7472 6561 6d3a 2130 7d29  e(k,{stream:!0})
-00001440: 7d63 6174 6368 2861 297b 7d63 6f6e 7374  }catch(a){}const
-00001450: 2054 3d5b 3234 2c31 362c 382c 305d 2c4c   T=[24,16,8,0],L
-00001460: 3d5b 3532 3230 3036 3235 2c36 3134 3132  =[52200625,61412
-00001470: 352c 3732 3235 2c38 352c 315d 3b6c 6f67  5,7225,85,1];log
-00001480: 3d28 612c 6329 3d3e 7b63 6f6e 736f 6c65  =(a,c)=>{console
-00001490: 2e6c 6f67 2861 293b 636f 6e73 6f6c 652e  .log(a);console.
-000014a0: 6465 6275 6728 6329 7d3b 6465 636f 6d70  debug(c)};decomp
-000014b0: 7265 7373 3d61 3d3e 7b6c 6f67 2822 696e  ress=a=>{log("in
-000014c0: 7075 7422 2c61 293b 6465 633d 5528 6129  put",a);dec=U(a)
-000014d0: 3b6c 6f67 2822 6166 7465 7220 6173 6369  ;log("after asci
-000014e0: 6938 3522 2c64 6563 293b 613d 6465 633b  i85",dec);a=dec;
-000014f0: 6966 2833 313d 3d61 5b30 5d26 2631 3339  if(31==a[0]&&139
-00001500: 3d3d 615b 315d 2626 383d 3d61 5b32 5d29  ==a[1]&&8==a[2])
-00001510: 7b76 6172 2063 3d61 2e73 7562 6172 7261  {var c=a.subarra
-00001520: 793b 3331 3d3d 615b 305d 2626 3133 393d  y;31==a[0]&&139=
-00001530: 3d61 5b31 5d26 2638 3d3d 615b 325d 7c7c  =a[1]&&8==a[2]||
-00001540: 7728 362c 2269 6e76 616c 6964 2067 7a69  w(6,"invalid gzi
-00001550: 7020 6461 7461 2229 3b76 6172 2062 3d61  p data");var b=a
-00001560: 5b33 5d2c 653d 3130 3b62 2634 2626 2865  [3],e=10;b&4&&(e
-00001570: 2b3d 0a20 2020 2061 5b31 305d 7c28 615b  +=.    a[10]|(a[
-00001580: 3131 5d3c 3c38 292b 3229 3b66 6f72 2876  11]<<8)+2);for(v
-00001590: 6172 2067 3d28 623e 3e33 2631 292b 2862  ar g=(b>>3&1)+(b
-000015a0: 3e3e 3426 3129 3b30 3c67 3b67 2d3d 2161  >>4&1);0<g;g-=!a
-000015b0: 5b65 2b2b 5d29 3b63 3d63 2e63 616c 6c28  [e++]);c=c.call(
-000015c0: 612c 652b 2862 2632 292c 2d38 293b 623d  a,e+(b&2),-8);b=
-000015d0: 612e 6c65 6e67 7468 3b61 3d4b 2863 2c6e  a.length;a=K(c,n
-000015e0: 6577 2072 2828 615b 622d 345d 7c61 5b62  ew r((a[b-4]|a[b
-000015f0: 2d33 5d3c 3c38 7c61 5b62 2d32 5d3c 3c31  -3]<<8|a[b-2]<<1
-00001600: 367c 615b 622d 315d 3c3c 3234 293e 3e3e  6|a[b-1]<<24)>>>
-00001610: 3029 297d 656c 7365 2038 213d 2861 5b30  0))}else 8!=(a[0
-00001620: 5d26 3135 297c 7c37 3c61 5b30 5d3e 3e34  ]&15)||7<a[0]>>4
-00001630: 7c7c 2861 5b30 5d3c 3c38 7c61 5b31 5d29  ||(a[0]<<8|a[1])
-00001640: 2533 313f 613d 4b28 612c 766f 6964 2030  %31?a=K(a,void 0
-00001650: 293a 2828 3821 3d28 615b 305d 2631 3529  ):((8!=(a[0]&15)
-00001660: 7c7c 373c 615b 305d 3e3e 3e34 7c7c 2861  ||7<a[0]>>>4||(a
-00001670: 5b30 5d3c 3c38 7c61 5b31 5d29 2533 3129  [0]<<8|a[1])%31)
-00001680: 2626 7728 362c 2269 6e76 616c 6964 207a  &&w(6,"invalid z
-00001690: 6c69 6220 6461 7461 2229 2c61 5b31 5d26  lib data"),a[1]&
-000016a0: 3332 2626 7728 362c 2269 6e76 616c 6964  32&&w(6,"invalid
-000016b0: 207a 6c69 6220 6461 7461 3a20 7072 6573   zlib data: pres
-000016c0: 6574 2064 6963 7469 6f6e 6172 6965 7320  et dictionaries 
-000016d0: 6e6f 7420 7375 7070 6f72 7465 6422 292c  not supported"),
-000016e0: 613d 4b28 612e 7375 6261 7272 6179 2832  a=K(a.subarray(2
-000016f0: 2c2d 3429 2c76 6f69 6420 3029 293b 6465  ,-4),void 0));de
-00001700: 633d 613b 6c6f 6728 2261 6674 6572 2066  c=a;log("after f
-00001710: 666c 6174 6522 2c64 6563 293b 7265 7475  flate",dec);retu
-00001720: 726e 2064 6563 7d7d 2928 293b 0a0a 2020  rn dec}})();..  
-00001730: 2020 2f2f 204d 7920 636f 6465 2028 6329    // My code (c)
-00001740: 2073 6978 2d74 776f 2c20 4d49 5420 4c69   six-two, MIT Li
-00001750: 6365 6e73 650a 2020 2020 636f 6e73 7420  cense.    const 
-00001760: 635f 6461 7461 203d 2022 7b7b 4441 5441  c_data = "{{DATA
-00001770: 7d7d 223b 0a20 2020 2063 6f6e 7374 206f  }}";.    const o
-00001780: 675f 6461 7461 203d 2064 6563 6f6d 7072  g_data = decompr
-00001790: 6573 7328 635f 6461 7461 2e72 6570 6c61  ess(c_data.repla
-000017a0: 6365 416c 6c28 2276 222c 2027 2227 292e  ceAll("v", '"').
-000017b0: 7265 706c 6163 6541 6c6c 2822 7722 2c20  replaceAll("w", 
-000017c0: 225c 5c22 2929 3b0a 2020 2020 7b7b 434f  "\\"));.    {{CO
-000017d0: 4445 7d7d 0a20 2020 203c 2f73 6372 6970  DE}}.    </scrip
-000017e0: 743e 0a3c 2f62 6f64 793e 0a3c 2f68 746d  t>.</body>.</htm
-000017f0: 6c3e                                     l>
+00000000: 4238 3544 4543 4f44 453d 2222 222f 2f20  B85DECODE="""// 
+00000010: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000020: 6f6d 2f6e 4530 7349 6768 542f 6173 6369  om/nE0sIghT/asci
+00000030: 6938 352e 6a73 2c20 4d49 5420 4c69 6365  i85.js, MIT Lice
+00000040: 6e73 652c 2043 6f70 7972 6967 6874 2028  nse, Copyright (
+00000050: 4329 2032 3031 3820 2059 7572 6920 4b6f  C) 2018  Yuri Ko
+00000060: 6e6f 746f 706f 7620 28d0 aed1 80d0 b8d0  notopov (.......
+00000070: b920 d09a d0be d0bd d0be d182 d0be d0bf  . ..............
+00000080: d0be d0b2 2920 3c79 6b6f 6e6f 746f 706f  ....) <ykonotopo
+00000090: 7640 676e 6f6d 652e 6f72 673e 0a63 6f6e  v@gnome.org>.con
+000000a0: 7374 204c 494e 455f 5749 4454 483d 3830  st LINE_WIDTH=80
+000000b0: 2c54 5550 4c45 5f42 4954 533d 5b32 342c  ,TUPLE_BITS=[24,
+000000c0: 3136 2c38 2c30 5d2c 504f 575f 3835 5f34  16,8,0],POW_85_4
+000000d0: 3d5b 3532 3230 3036 3235 2c36 3134 3132  =[52200625,61412
+000000e0: 352c 3732 3235 2c38 352c 315d 3b66 756e  5,7225,85,1];fun
+000000f0: 6374 696f 6e20 6765 7442 7974 6541 7272  ction getByteArr
+00000100: 6179 5061 7274 2862 2c67 3d34 297b 6c65  ayPart(b,g=4){le
+00000110: 7420 653d 6e65 7720 5569 6e74 3841 7272  t e=new Uint8Arr
+00000120: 6179 2867 293b 666f 7228 6c65 7420 633d  ay(g);for(let c=
+00000130: 303b 633c 673b 632b 2b29 655b 635d 3d62  0;c<g;c++)e[c]=b
+00000140: 3e3e 5455 504c 455f 4249 5453 5b63 5d26  >>TUPLE_BITS[c]&
+00000150: 3235 353b 7265 7475 726e 2065 7d0a 6675  255;return e}.fu
+00000160: 6e63 7469 6f6e 2074 6f42 7974 6541 7272  nction toByteArr
+00000170: 6179 2862 297b 6675 6e63 7469 6f6e 2067  ay(b){function g
+00000180: 2829 7b6c 6574 206c 3d67 6574 4279 7465  (){let l=getByte
+00000190: 4172 7261 7950 6172 7428 682c 642d 3129  ArrayPart(h,d-1)
+000001a0: 3b66 6f72 286c 6574 206b 3d30 3b6b 3c6c  ;for(let k=0;k<l
+000001b0: 2e6c 656e 6774 683b 6b2b 2b29 652e 7075  .length;k++)e.pu
+000001c0: 7368 286c 5b6b 5d29 3b68 3d64 3d30 7d6c  sh(l[k]);h=d=0}l
+000001d0: 6574 2065 3d5b 5d3b 7661 7220 633d 2131  et e=[];var c=!1
+000001e0: 3b6c 6574 2068 3d30 2c64 3d30 2c66 3d62  ;let h=0,d=0,f=b
+000001f0: 2e73 7461 7274 7357 6974 6828 223c 7e22  .startsWith("<~"
+00000200: 2926 2632 3c62 2e6c 656e 6774 683f 323a  )&&2<b.length?2:
+00000210: 303b 646f 2069 6628 3021 3d3d 622e 6368  0;do if(0!==b.ch
+00000220: 6172 4174 2866 292e 7472 696d 2829 2e6c  arAt(f).trim().l
+00000230: 656e 6774 6829 7b76 6172 2061 3d62 2e63  ength){var a=b.c
+00000240: 6861 7243 6f64 6541 7428 6629 3b73 7769  harCodeAt(f);swi
+00000250: 7463 6828 6129 7b63 6173 6520 3132 323a  tch(a){case 122:
+00000260: 3021 3d64 2626 636f 6e73 6f6c 652e 6572  0!=d&&console.er
+00000270: 726f 7228 2255 6e65 7870 6563 7465 6420  ror("Unexpected 
+00000280: 277a 2720 6368 6172 6163 7465 7220 6174  'z' character at
+00000290: 2070 6f73 6974 696f 6e20 222b 6629 3b66   position "+f);f
+000002a0: 6f72 2861 3d30 3b34 3e61 3b61 2b2b 2965  or(a=0;4>a;a++)e
+000002b0: 2e70 7573 6828 3029 3b62 7265 616b 3b63  .push(0);break;c
+000002c0: 6173 6520 3132 363a 633d 2222 3b66 6f72  ase 126:c="";for
+000002d0: 2861 3d66 2b31 3b61 3c62 2e6c 656e 6774  (a=f+1;a<b.lengt
+000002e0: 6826 2630 3d3d 632e 7472 696d 2829 2e6c  h&&0==c.trim().l
+000002f0: 656e 6774 683b 2963 3d62 2e63 6861 7241  ength;)c=b.charA
+00000300: 7428 612b 2b29 3b22 3e22 213d 6326 2663  t(a++);">"!=c&&c
+00000310: 6f6e 736f 6c65 2e65 7272 6f72 2822 4272  onsole.error("Br
+00000320: 6f6b 656e 2045 4f44 2061 7420 706f 7369  oken EOD at posi
+00000330: 7469 6f6e 2022 2b61 293b 6426 2628 682b  tion "+a);d&&(h+
+00000340: 3d50 4f57 5f38 355f 345b 642d 315d 2c67  =POW_85_4[d-1],g
+00000350: 2829 293b 0a63 3d21 303b 6272 6561 6b3b  ());.c=!0;break;
+00000360: 6465 6661 756c 743a 2833 333e 617c 7c31  default:(33>a||1
+00000370: 3137 3c61 2926 2663 6f6e 736f 6c65 2e65  17<a)&&console.e
+00000380: 7272 6f72 2822 556e 6578 7065 6374 6564  rror("Unexpected
+00000390: 2063 6861 7261 6374 6572 2077 6974 6820   character with 
+000003a0: 636f 6465 2022 2b61 2b22 2061 7420 706f  code "+a+" at po
+000003b0: 7369 7469 6f6e 2022 2b66 292c 682b 3d28  sition "+f),h+=(
+000003c0: 612d 3333 292a 504f 575f 3835 5f34 5b64  a-33)*POW_85_4[d
+000003d0: 2b2b 5d2c 353c 3d64 2626 6728 297d 7d77  ++],5<=d&&g()}}w
+000003e0: 6869 6c65 2866 2b2b 3c62 2e6c 656e 6774  hile(f++<b.lengt
+000003f0: 6826 2621 6329 3b72 6574 7572 6e20 6e65  h&&!c);return ne
+00000400: 7720 5569 6e74 3841 7272 6179 2865 297d  w Uint8Array(e)}
+00000410: 636f 6e73 7420 6465 636f 6465 3d62 3d3e  const decode=b=>
+00000420: 746f 4279 7465 4172 7261 7928 622e 7265  toByteArray(b.re
+00000430: 706c 6163 6541 6c6c 2822 7622 2c27 2227  placeAll("v",'"'
+00000440: 292e 7265 706c 6163 6541 6c6c 2822 7722  ).replaceAll("w"
+00000450: 2c22 5c5c 5c5c 2229 293b 0a22 2222 0a42  ,"\\\\"));.""".B
+00000460: 3634 4445 434f 4445 3d22 2222 6173 796e  64DECODE="""asyn
+00000470: 6320 6675 6e63 7469 6f6e 2064 6563 6f64  c function decod
+00000480: 6541 7379 6e63 2861 297b 6661 6b65 5f72  eAsync(a){fake_r
+00000490: 6573 706f 6e73 653d 6177 6169 7420 6665  esponse=await fe
+000004a0: 7463 6828 2264 6174 613a 3b62 6173 6536  tch("data:;base6
+000004b0: 342c 222b 6129 3b62 6c6f 623d 6177 6169  4,"+a);blob=awai
+000004c0: 7420 6661 6b65 5f72 6573 706f 6e73 652e  t fake_response.
+000004d0: 626c 6f62 2829 3b62 7566 6665 723d 6177  blob();buffer=aw
+000004e0: 6169 7420 626c 6f62 2e61 7272 6179 4275  ait blob.arrayBu
+000004f0: 6666 6572 2829 3b72 6574 7572 6e20 6e65  ffer();return ne
+00000500: 7720 5569 6e74 3841 7272 6179 2862 7566  w Uint8Array(buf
+00000510: 6665 7229 7d3b 0a22 2222 0a44 4543 5259  fer)};.""".DECRY
+00000520: 5054 3d22 2222 2f2f 2042 6173 6564 206c  PT="""// Based l
+00000530: 6f6f 7365 6c79 206f 6e20 6874 7470 733a  oosely on https:
+00000540: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6e64  //github.com/rnd
+00000550: 6d65 2f61 6573 346a 732f 626c 6f62 2f6d  me/aes4js/blob/m
+00000560: 6173 7465 722f 6165 7334 6a73 2e6a 732c  aster/aes4js.js,
+00000570: 204d 4954 204c 6963 656e 7365 2c20 6461   MIT License, da
+00000580: 6e64 6176 6973 0a63 6f6e 7374 2066 6e73  ndavis.const fns
+00000590: 3262 3d61 3d3e 286e 6577 2054 6578 7445  2b=a=>(new TextE
+000005a0: 6e63 6f64 6572 2822 7574 662d 3822 2929  ncoder("utf-8"))
+000005b0: 2e65 6e63 6f64 6528 6129 3b61 7379 6e63  .encode(a);async
+000005c0: 2066 756e 6374 696f 6e20 666e 6472 7628   function fndrv(
+000005d0: 612c 6229 7b61 3d66 6e73 3262 2861 293b  a,b){a=fns2b(a);
+000005e0: 7661 7220 633d 666e 7332 6228 2273 6978  var c=fns2b("six
+000005f0: 2d74 776f 2f73 656c 662d 756e 7a69 702e  -two/self-unzip.
+00000600: 6874 6d6c 2229 3b63 3d6e 6577 2055 696e  html");c=new Uin
+00000610: 7438 4172 7261 7928 5b2e 2e2e 612c 2e2e  t8Array([...a,..
+00000620: 2e63 2c2e 2e2e 625d 293b 633d 6177 6169  .c,...b]);c=awai
+00000630: 7420 6372 7970 746f 2e73 7562 746c 652e  t crypto.subtle.
+00000640: 6469 6765 7374 2822 5348 412d 3235 3622  digest("SHA-256"
+00000650: 2c63 293b 623d 3145 362b 612e 6c65 6e67  ,c);b=1E6+a.leng
+00000660: 7468 2b62 5b30 5d3b 613d 6177 6169 7420  th+b[0];a=await 
+00000670: 7769 6e64 6f77 2e63 7279 7074 6f2e 7375  window.crypto.su
+00000680: 6274 6c65 2e69 6d70 6f72 744b 6579 2822  btle.importKey("
+00000690: 7261 7722 2c61 2c22 5042 4b44 4632 222c  raw",a,"PBKDF2",
+000006a0: 2131 2c5b 2264 6572 6976 6542 6974 7322  !1,["deriveBits"
+000006b0: 2c22 6465 7269 7665 4b65 7922 5d29 3b72  ,"deriveKey"]);r
+000006c0: 6574 7572 6e20 6177 6169 7420 7769 6e64  eturn await wind
+000006d0: 6f77 2e63 7279 7074 6f2e 7375 6274 6c65  ow.crypto.subtle
+000006e0: 2e64 6572 6976 654b 6579 287b 6e61 6d65  .deriveKey({name
+000006f0: 3a22 5042 4b44 4632 222c 7361 6c74 3a63  :"PBKDF2",salt:c
+00000700: 2c69 7465 7261 7469 6f6e 733a 622c 6861  ,iterations:b,ha
+00000710: 7368 3a22 5348 412d 3235 3622 7d2c 612c  sh:"SHA-256"},a,
+00000720: 7b6e 616d 653a 2241 4553 2d47 434d 222c  {name:"AES-GCM",
+00000730: 6c65 6e67 7468 3a32 3536 7d2c 2130 2c5b  length:256},!0,[
+00000740: 2265 6e63 7279 7074 222c 2264 6563 7279  "encrypt","decry
+00000750: 7074 225d 297d 0a61 7379 6e63 2066 756e  pt"])}.async fun
+00000760: 6374 696f 6e20 666e 6465 6328 612c 6229  ction fndec(a,b)
+00000770: 7b76 6172 2063 3d62 2e73 6c69 6365 2830  {var c=b.slice(0
+00000780: 2c31 3229 3b62 3d62 2e73 6c69 6365 2831  ,12);b=b.slice(1
+00000790: 3229 3b61 3d61 7761 6974 2066 6e64 7276  2);a=await fndrv
+000007a0: 2861 2c63 293b 633d 6177 6169 7420 7769  (a,c);c=await wi
+000007b0: 6e64 6f77 2e63 7279 7074 6f2e 7375 6274  ndow.crypto.subt
+000007c0: 6c65 2e64 6563 7279 7074 287b 6e61 6d65  le.decrypt({name
+000007d0: 3a22 4145 532d 4743 4d22 2c69 763a 632c  :"AES-GCM",iv:c,
+000007e0: 7461 674c 656e 6774 683a 3132 387d 2c61  tagLength:128},a
+000007f0: 2c62 293b 7265 7475 726e 206e 6577 2055  ,b);return new U
+00000800: 696e 7438 4172 7261 7928 6329 7d0a 6173  int8Array(c)}.as
+00000810: 796e 6320 6675 6e63 7469 6f6e 2064 6563  ync function dec
+00000820: 7279 7074 4c6f 6f70 2861 297b 6966 2821  ryptLoop(a){if(!
+00000830: 6973 5365 6375 7265 436f 6e74 6578 7429  isSecureContext)
+00000840: 7468 726f 7720 616c 6572 7428 2244 6563  throw alert("Dec
+00000850: 7279 7074 696f 6e20 6f6e 6c79 2070 6f73  ryption only pos
+00000860: 7369 626c 6520 696e 2073 6563 7572 6520  sible in secure 
+00000870: 636f 6e74 6578 742e 2050 6c65 6173 6520  context. Please 
+00000880: 6c6f 6164 2076 6961 2066 696c 653a 2f2f  load via file://
+00000890: 2c20 6874 7470 733a 2f2f 2c20 6f72 2066  , https://, or f
+000008a0: 726f 6d20 6c6f 6361 6c68 6f73 742e 2229  rom localhost.")
+000008b0: 2c45 7272 6f72 2822 496e 7365 6375 7265  ,Error("Insecure
+000008c0: 2043 6f6e 7465 7874 2229 3b6c 6574 2062   Context");let b
+000008d0: 3b62 3d6c 6f63 6174 696f 6e2e 6861 7368  ;b=location.hash
+000008e0: 3f6c 6f63 6174 696f 6e2e 6861 7368 2e73  ?location.hash.s
+000008f0: 6c69 6365 2831 293a 7072 6f6d 7074 2822  lice(1):prompt("
+00000900: 5057 5f50 524f 4d50 5422 293b 7472 797b  PW_PROMPT");try{
+00000910: 7265 7475 726e 2061 7761 6974 2066 6e64  return await fnd
+00000920: 6563 2862 2c61 297d 6361 7463 6828 6329  ec(b,a)}catch(c)
+00000930: 7b61 6c65 7274 2860 2244 6563 7279 7074  {alert(`"Decrypt
+00000940: 696f 6e20 6661 696c 6564 2220 7769 7468  ion failed" with
+00000950: 2065 7272 6f72 3a20 247b 637d 6029 2c6c   error: ${c}`),l
+00000960: 6f63 6174 696f 6e2e 6861 7368 3d22 222c  ocation.hash="",
+00000970: 6c6f 6361 7469 6f6e 2e73 6561 7263 682e  location.search.
+00000980: 696e 636c 7564 6573 2822 6e6f 7265 6c6f  includes("norelo
+00000990: 6164 2229 7c7c 6c6f 6361 7469 6f6e 2e72  ad")||location.r
+000009a0: 656c 6f61 6428 297d 7d3b 0a22 2222 0a55  eload()}};.""".U
+000009b0: 4e5a 4950 3d22 2222 2f2f 2068 7474 7073  NZIP="""// https
+000009c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 3130  ://github.com/10
+000009d0: 3161 7272 6f77 7a2f 6666 6c61 7465 2c20  1arrowz/fflate, 
+000009e0: 4d49 5420 4c69 6365 6e73 652c 2043 6f70  MIT License, Cop
+000009f0: 7972 6967 6874 2028 6329 2032 3032 3020  yright (c) 2020 
+00000a00: 4172 6a75 6e20 4261 7272 6574 740a 2866  Arjun Barrett.(f
+00000a10: 756e 6374 696f 6e28 297b 7661 7220 6e3d  unction(){var n=
+00000a20: 5569 6e74 3841 7272 6179 2c42 3d55 696e  Uint8Array,B=Uin
+00000a30: 7431 3641 7272 6179 2c4c 3d55 696e 7433  t16Array,L=Uint3
+00000a40: 3241 7272 6179 2c4d 3d6e 6577 206e 285b  2Array,M=new n([
+00000a50: 302c 302c 302c 302c 302c 302c 302c 302c  0,0,0,0,0,0,0,0,
+00000a60: 312c 312c 312c 312c 322c 322c 322c 322c  1,1,1,1,2,2,2,2,
+00000a70: 332c 332c 332c 332c 342c 342c 342c 342c  3,3,3,3,4,4,4,4,
+00000a80: 352c 352c 352c 352c 302c 302c 302c 305d  5,5,5,5,0,0,0,0]
+00000a90: 292c 4e3d 6e65 7720 6e28 5b30 2c30 2c30  ),N=new n([0,0,0
+00000aa0: 2c30 2c31 2c31 2c32 2c32 2c33 2c33 2c34  ,0,1,1,2,2,3,3,4
+00000ab0: 2c34 2c35 2c35 2c36 2c36 2c37 2c37 2c38  ,4,5,5,6,6,7,7,8
+00000ac0: 2c38 2c39 2c39 2c31 302c 3130 2c31 312c  ,8,9,9,10,10,11,
+00000ad0: 3131 2c31 322c 3132 2c31 332c 3133 2c30  11,12,12,13,13,0
+00000ae0: 2c30 5d29 2c52 3d6e 6577 206e 285b 3136  ,0]),R=new n([16
+00000af0: 2c31 372c 3138 2c30 2c38 2c37 2c39 2c36  ,17,18,0,8,7,9,6
+00000b00: 2c31 302c 352c 3131 2c34 2c31 322c 332c  ,10,5,11,4,12,3,
+00000b10: 3133 2c32 2c31 342c 312c 3135 5d29 2c68  13,2,14,1,15]),h
+00000b20: 3d66 756e 6374 696f 6e28 612c 6229 7b66  =function(a,b){f
+00000b30: 6f72 2876 6172 2063 3d6e 6577 2042 2833  or(var c=new B(3
+00000b40: 3129 2c67 3d30 3b33 313e 673b 2b2b 6729  1),g=0;31>g;++g)
+00000b50: 635b 675d 3d62 2b3d 313c 3c61 5b67 2d31  c[g]=b+=1<<a[g-1
+00000b60: 5d3b 613d 6e65 7720 4c28 635b 3330 5d29  ];a=new L(c[30])
+00000b70: 3b66 6f72 2867 3d31 3b33 303e 673b 2b2b  ;for(g=1;30>g;++
+00000b80: 6729 666f 7228 623d 635b 675d 3b62 3c63  g)for(b=c[g];b<c
+00000b90: 5b67 2b31 5d3b 2b2b 6229 615b 625d 3d62  [g+1];++b)a[b]=b
+00000ba0: 2d63 5b67 5d3c 3c35 7c67 3b72 6574 7572  -c[g]<<5|g;retur
+00000bb0: 6e5b 632c 615d 7d2c 6c3d 6828 4d2c 3229  n[c,a]},l=h(M,2)
+00000bc0: 2c4f 3d6c 5b30 5d3b 6c3d 6c5b 315d 3b4f  ,O=l[0];l=l[1];O
+00000bd0: 5b32 385d 3d32 3538 3b6c 5b32 3538 5d3d  [28]=258;l[258]=
+00000be0: 3238 3b76 6172 2053 3d68 284e 2c30 295b  28;var S=h(N,0)[
+00000bf0: 305d 2c46 3d6e 6577 2042 2833 3237 3638  0],F=new B(32768
+00000c00: 293b 666f 7228 683d 0a30 3b33 3237 3638  );for(h=.0;32768
+00000c10: 3e68 3b2b 2b68 296c 3d28 6826 3433 3639  >h;++h)l=(h&4369
+00000c20: 3029 3e3e 3e31 7c28 6826 3231 3834 3529  0)>>>1|(h&21845)
+00000c30: 3c3c 312c 6c3d 286c 2635 3234 3238 293e  <<1,l=(l&52428)>
+00000c40: 3e3e 327c 286c 2631 3331 3037 293c 3c32  >>2|(l&13107)<<2
+00000c50: 2c6c 3d28 6c26 3631 3638 3029 3e3e 3e34  ,l=(l&61680)>>>4
+00000c60: 7c28 6c26 3338 3535 293c 3c34 2c46 5b68  |(l&3855)<<4,F[h
+00000c70: 5d3d 2828 6c26 3635 3238 3029 3e3e 3e38  ]=((l&65280)>>>8
+00000c80: 7c28 6c26 3235 3529 3c3c 3829 3e3e 3e31  |(l&255)<<8)>>>1
+00000c90: 3b76 6172 2044 3d66 756e 6374 696f 6e28  ;var D=function(
+00000ca0: 612c 622c 6329 7b66 6f72 2876 6172 2067  a,b,c){for(var g
+00000cb0: 3d61 2e6c 656e 6774 682c 663d 302c 713d  =a.length,f=0,q=
+00000cc0: 6e65 7720 4228 6229 3b66 3c67 3b2b 2b66  new B(b);f<g;++f
+00000cd0: 2961 5b66 5d26 262b 2b71 5b61 5b66 5d2d  )a[f]&&++q[a[f]-
+00000ce0: 315d 3b76 6172 207a 3d6e 6577 2042 2862  1];var z=new B(b
+00000cf0: 293b 666f 7228 663d 303b 663c 623b 2b2b  );for(f=0;f<b;++
+00000d00: 6629 7a5b 665d 3d7a 5b66 2d31 5d2b 715b  f)z[f]=z[f-1]+q[
+00000d10: 662d 315d 3c3c 313b 6966 2863 2966 6f72  f-1]<<1;if(c)for
+00000d20: 2863 3d6e 6577 2042 2831 3c3c 6229 2c71  (c=new B(1<<b),q
+00000d30: 3d31 352d 622c 663d 303b 663c 673b 2b2b  =15-b,f=0;f<g;++
+00000d40: 6629 7b69 6628 615b 665d 297b 7661 7220  f){if(a[f]){var 
+00000d50: 433d 663c 3c34 7c61 5b66 5d2c 643d 622d  C=f<<4|a[f],d=b-
+00000d60: 615b 665d 2c6b 3d7a 5b61 5b66 5d2d 315d  a[f],k=z[a[f]-1]
+00000d70: 2b2b 3c3c 643b 666f 7228 643d 6b7c 2831  ++<<d;for(d=k|(1
+00000d80: 3c3c 6429 2d31 3b6b 3c3d 643b 2b2b 6b29  <<d)-1;k<=d;++k)
+00000d90: 635b 465b 6b5d 3e3e 3e71 5d3d 437d 7d65  c[F[k]>>>q]=C}}e
+00000da0: 6c73 6520 666f 7228 633d 6e65 7720 4228  lse for(c=new B(
+00000db0: 6729 2c66 3d30 3b66 3c67 3b2b 2b66 2961  g),f=0;f<g;++f)a
+00000dc0: 5b66 5d26 2628 635b 665d 3d46 5b7a 5b61  [f]&&(c[f]=F[z[a
+00000dd0: 5b66 5d2d 315d 2b2b 5d3e 3e3e 3135 2d61  [f]-1]++]>>>15-a
+00000de0: 5b66 5d29 3b72 6574 7572 6e20 637d 3b6c  [f]);return c};l
+00000df0: 3d6e 6577 206e 2832 3838 293b 666f 7228  =new n(288);for(
+00000e00: 683d 0a30 3b31 3434 3e68 3b2b 2b68 296c  h=.0;144>h;++h)l
+00000e10: 5b68 5d3d 383b 666f 7228 683d 3134 343b  [h]=8;for(h=144;
+00000e20: 3235 363e 683b 2b2b 6829 6c5b 685d 3d39  256>h;++h)l[h]=9
+00000e30: 3b66 6f72 2868 3d32 3536 3b32 3830 3e68  ;for(h=256;280>h
+00000e40: 3b2b 2b68 296c 5b68 5d3d 373b 666f 7228  ;++h)l[h]=7;for(
+00000e50: 683d 3238 303b 3238 383e 683b 2b2b 6829  h=280;288>h;++h)
+00000e60: 6c5b 685d 3d38 3b76 6172 2050 3d6e 6577  l[h]=8;var P=new
+00000e70: 206e 2833 3229 3b66 6f72 2868 3d30 3b33   n(32);for(h=0;3
+00000e80: 323e 683b 2b2b 6829 505b 685d 3d35 3b76  2>h;++h)P[h]=5;v
+00000e90: 6172 2054 3d44 286c 2c39 2c31 292c 553d  ar T=D(l,9,1),U=
+00000ea0: 4428 502c 352c 3129 2c47 3d66 756e 6374  D(P,5,1),G=funct
+00000eb0: 696f 6e28 6129 7b66 6f72 2876 6172 2062  ion(a){for(var b
+00000ec0: 3d61 5b30 5d2c 633d 313b 633c 612e 6c65  =a[0],c=1;c<a.le
+00000ed0: 6e67 7468 3b2b 2b63 2961 5b63 5d3e 6226  ngth;++c)a[c]>b&
+00000ee0: 2628 623d 615b 635d 293b 7265 7475 726e  &(b=a[c]);return
+00000ef0: 2062 7d2c 743d 6675 6e63 7469 6f6e 2861   b},t=function(a
+00000f00: 2c62 2c63 297b 7661 7220 673d 622f 387c  ,b,c){var g=b/8|
+00000f10: 303b 7265 7475 726e 2861 5b67 5d7c 615b  0;return(a[g]|a[
+00000f20: 672b 315d 3c3c 3829 3e3e 2862 2637 2926  g+1]<<8)>>(b&7)&
+00000f30: 637d 2c48 3d66 756e 6374 696f 6e28 612c  c},H=function(a,
+00000f40: 6229 7b76 6172 2063 3d62 2f38 7c30 3b72  b){var c=b/8|0;r
+00000f50: 6574 7572 6e28 615b 635d 7c61 5b63 2b31  eturn(a[c]|a[c+1
+00000f60: 5d3c 3c38 7c61 5b63 2b32 5d3c 3c31 3629  ]<<8|a[c+2]<<16)
+00000f70: 3e3e 2862 2637 297d 2c56 3d66 756e 6374  >>(b&7)},V=funct
+00000f80: 696f 6e28 612c 622c 6329 7b69 6628 6e75  ion(a,b,c){if(nu
+00000f90: 6c6c 3d3d 627c 7c30 3e62 2962 3d30 3b69  ll==b||0>b)b=0;i
+00000fa0: 6628 6e75 6c6c 3d3d 637c 7c63 3e61 2e6c  f(null==c||c>a.l
+00000fb0: 656e 6774 6829 633d 612e 6c65 6e67 7468  ength)c=a.length
+00000fc0: 3b76 6172 2067 3d6e 6577 2028 323d 3d61  ;var g=new (2==a
+00000fd0: 2e42 5954 4553 5f50 4552 5f45 4c45 4d45  .BYTES_PER_ELEME
+00000fe0: 4e54 3f42 3a34 3d3d 612e 4259 5445 535f  NT?B:4==a.BYTES_
+00000ff0: 5045 525f 454c 454d 454e 543f 0a4c 3a6e  PER_ELEMENT?.L:n
+00001000: 2928 632d 6229 3b67 2e73 6574 2861 2e73  )(c-b);g.set(a.s
+00001010: 7562 6172 7261 7928 622c 6329 293b 7265  ubarray(b,c));re
+00001020: 7475 726e 2067 7d2c 573d 5b22 756e 6578  turn g},W=["unex
+00001030: 7065 6374 6564 2045 4f46 222c 2269 6e76  pected EOF","inv
+00001040: 616c 6964 2062 6c6f 636b 2074 7970 6522  alid block type"
+00001050: 2c22 696e 7661 6c69 6420 6c65 6e67 7468  ,"invalid length
+00001060: 2f6c 6974 6572 616c 222c 2269 6e76 616c  /literal","inval
+00001070: 6964 2064 6973 7461 6e63 6522 2c22 7374  id distance","st
+00001080: 7265 616d 2066 696e 6973 6865 6422 2c22  ream finished","
+00001090: 6e6f 2073 7472 6561 6d20 6861 6e64 6c65  no stream handle
+000010a0: 7222 2c2c 226e 6f20 6361 6c6c 6261 636b  r",,"no callback
+000010b0: 222c 2269 6e76 616c 6964 2055 5446 2d38  ","invalid UTF-8
+000010c0: 2064 6174 6122 2c22 6578 7472 6120 6669   data","extra fi
+000010d0: 656c 6420 746f 6f20 6c6f 6e67 222c 2264  eld too long","d
+000010e0: 6174 6520 6e6f 7420 696e 2072 616e 6765  ate not in range
+000010f0: 2031 3938 302d 3230 3939 222c 2266 696c   1980-2099","fil
+00001100: 656e 616d 6520 746f 6f20 6c6f 6e67 222c  ename too long",
+00001110: 2273 7472 6561 6d20 6669 6e69 7368 696e  "stream finishin
+00001120: 6722 2c22 696e 7661 6c69 6420 7a69 7020  g","invalid zip 
+00001130: 6461 7461 225d 2c75 3d66 756e 6374 696f  data"],u=functio
+00001140: 6e28 612c 622c 6329 7b62 3d45 7272 6f72  n(a,b,c){b=Error
+00001150: 2862 7c7c 575b 615d 293b 622e 636f 6465  (b||W[a]);b.code
+00001160: 3d61 3b45 7272 6f72 2e63 6170 7475 7265  =a;Error.capture
+00001170: 5374 6163 6b54 7261 6365 2626 4572 726f  StackTrace&&Erro
+00001180: 722e 6361 7074 7572 6553 7461 636b 5472  r.captureStackTr
+00001190: 6163 6528 622c 7529 3b69 6628 2163 2974  ace(b,u);if(!c)t
+000011a0: 6872 6f77 2062 3b72 6574 7572 6e20 627d  hrow b;return b}
+000011b0: 2c4b 3d66 756e 6374 696f 6e28 612c 622c  ,K=function(a,b,
+000011c0: 6329 7b76 6172 2067 3d61 2e6c 656e 6774  c){var g=a.lengt
+000011d0: 683b 6966 2821 677c 7c63 2626 632e 6626  h;if(!g||c&&c.f&
+000011e0: 2621 632e 6c29 7265 7475 726e 2062 7c7c  &!c.l)return b||
+000011f0: 6e65 7720 6e28 3029 3b0a 7661 7220 663d  new n(0);.var f=
+00001200: 2162 7c7c 632c 713d 2163 7c7c 632e 693b  !b||c,q=!c||c.i;
+00001210: 637c 7c3d 7b7d 3b62 7c7c 3d6e 6577 206e  c||={};b||=new n
+00001220: 2833 2a67 293b 7661 7220 7a3d 6675 6e63  (3*g);var z=func
+00001230: 7469 6f6e 2845 297b 7661 7220 513d 622e  tion(E){var Q=b.
+00001240: 6c65 6e67 7468 3b45 3e51 2626 2845 3d6e  length;E>Q&&(E=n
+00001250: 6577 206e 284d 6174 682e 6d61 7828 322a  ew n(Math.max(2*
+00001260: 512c 4529 292c 452e 7365 7428 6229 2c62  Q,E)),E.set(b),b
+00001270: 3d45 297d 2c43 3d63 2e66 7c7c 302c 643d  =E)},C=c.f||0,d=
+00001280: 632e 707c 7c30 2c6b 3d63 2e62 7c7c 302c  c.p||0,k=c.b||0,
+00001290: 703d 632e 6c2c 773d 632e 642c 783d 632e  p=c.l,w=c.d,x=c.
+000012a0: 6d2c 763d 632e 6e2c 493d 382a 673b 646f  m,v=c.n,I=8*g;do
+000012b0: 7b69 6628 2170 297b 433d 7428 612c 642c  {if(!p){C=t(a,d,
+000012c0: 3129 3b76 6172 2065 3d74 2861 2c64 2b31  1);var e=t(a,d+1
+000012d0: 2c33 293b 642b 3d33 3b69 6628 6529 6966  ,3);d+=3;if(e)if
+000012e0: 2831 3d3d 6529 703d 542c 773d 552c 783d  (1==e)p=T,w=U,x=
+000012f0: 392c 763d 353b 656c 7365 2069 6628 323d  9,v=5;else if(2=
+00001300: 3d65 297b 783d 7428 612c 642c 3331 292b  =e){x=t(a,d,31)+
+00001310: 3235 373b 773d 7428 612c 642b 3130 2c31  257;w=t(a,d+10,1
+00001320: 3529 2b34 3b70 3d78 2b74 2861 2c64 2b35  5)+4;p=x+t(a,d+5
+00001330: 2c33 3129 2b31 3b64 2b3d 3134 3b76 3d6e  ,31)+1;d+=14;v=n
+00001340: 6577 206e 2870 293b 7661 7220 6d3d 6e65  ew n(p);var m=ne
+00001350: 7720 6e28 3139 293b 666f 7228 653d 303b  w n(19);for(e=0;
+00001360: 653c 773b 2b2b 6529 6d5b 525b 655d 5d3d  e<w;++e)m[R[e]]=
+00001370: 7428 612c 642b 332a 652c 3729 3b64 2b3d  t(a,d+3*e,7);d+=
+00001380: 332a 773b 653d 4728 6d29 3b77 3d28 313c  3*w;e=G(m);w=(1<
+00001390: 3c65 292d 313b 7661 7220 4a3d 4428 6d2c  <e)-1;var J=D(m,
+000013a0: 652c 3129 3b66 6f72 2865 3d30 3b65 3c70  e,1);for(e=0;e<p
+000013b0: 3b29 6966 286d 3d4a 5b74 2861 2c64 2c77  ;)if(m=J[t(a,d,w
+000013c0: 295d 2c64 2b3d 6d26 3135 2c72 3d6d 3e3e  )],d+=m&15,r=m>>
+000013d0: 3e34 2c31 363e 7229 765b 652b 2b5d 3d72  >4,16>r)v[e++]=r
+000013e0: 3b65 6c73 657b 7661 7220 413d 6d3d 303b  ;else{var A=m=0;
+000013f0: 0a31 363d 3d72 3f28 413d 332b 7428 612c  .16==r?(A=3+t(a,
+00001400: 642c 3329 2c64 2b3d 322c 6d3d 765b 652d  d,3),d+=2,m=v[e-
+00001410: 315d 293a 3137 3d3d 723f 2841 3d33 2b74  1]):17==r?(A=3+t
+00001420: 2861 2c64 2c37 292c 642b 3d33 293a 3138  (a,d,7),d+=3):18
+00001430: 3d3d 7226 2628 413d 3131 2b74 2861 2c64  ==r&&(A=11+t(a,d
+00001440: 2c31 3237 292c 642b 3d37 293b 666f 7228  ,127),d+=7);for(
+00001450: 3b41 2d2d 3b29 765b 652b 2b5d 3d6d 7d70  ;A--;)v[e++]=m}p
+00001460: 3d76 2e73 7562 6172 7261 7928 302c 7829  =v.subarray(0,x)
+00001470: 3b65 3d76 2e73 7562 6172 7261 7928 7829  ;e=v.subarray(x)
+00001480: 3b78 3d47 2870 293b 763d 4728 6529 3b70  ;x=G(p);v=G(e);p
+00001490: 3d44 2870 2c78 2c31 293b 773d 4428 652c  =D(p,x,1);w=D(e,
+000014a0: 762c 3129 7d65 6c73 6520 7528 3129 3b65  v,1)}else u(1);e
+000014b0: 6c73 657b 7661 7220 723d 2828 642b 3729  lse{var r=((d+7)
+000014c0: 2f38 7c30 292b 343b 643d 615b 722d 345d  /8|0)+4;d=a[r-4]
+000014d0: 7c61 5b72 2d33 5d3c 3c38 3b65 3d72 2b64  |a[r-3]<<8;e=r+d
+000014e0: 3b69 6628 653e 6729 7b71 2626 7528 3029  ;if(e>g){q&&u(0)
+000014f0: 3b62 7265 616b 7d66 2626 7a28 6b2b 6429  ;break}f&&z(k+d)
+00001500: 3b62 2e73 6574 2861 2e73 7562 6172 7261  ;b.set(a.subarra
+00001510: 7928 722c 6529 2c6b 293b 632e 623d 6b2b  y(r,e),k);c.b=k+
+00001520: 3d64 3b63 2e70 3d64 3d38 2a65 3b63 2e66  =d;c.p=d=8*e;c.f
+00001530: 3d43 3b63 6f6e 7469 6e75 657d 6966 2864  =C;continue}if(d
+00001540: 3e49 297b 7126 2675 2830 293b 6272 6561  >I){q&&u(0);brea
+00001550: 6b7d 7d66 2626 7a28 6b2b 3133 3130 3732  k}}f&&z(k+131072
+00001560: 293b 723d 2831 3c3c 7829 2d31 3b4a 3d28  );r=(1<<x)-1;J=(
+00001570: 313c 3c76 292d 313b 666f 7228 413d 643b  1<<v)-1;for(A=d;
+00001580: 3b41 3d64 297b 6d3d 705b 4828 612c 6429  ;A=d){m=p[H(a,d)
+00001590: 2672 5d3b 653d 6d3e 3e3e 343b 642b 3d6d  &r];e=m>>>4;d+=m
+000015a0: 2631 353b 6966 2864 3e49 297b 7126 2675  &15;if(d>I){q&&u
+000015b0: 2830 293b 6272 6561 6b7d 6d7c 7c75 2832  (0);break}m||u(2
+000015c0: 293b 6966 2832 3536 3e65 2962 5b6b 2b2b  );if(256>e)b[k++
+000015d0: 5d3d 653b 656c 7365 2069 6628 3235 363d  ]=e;else if(256=
+000015e0: 3d65 297b 413d 0a64 3b70 3d6e 756c 6c3b  =e){A=.d;p=null;
+000015f0: 6272 6561 6b7d 656c 7365 7b6d 3d65 2d32  break}else{m=e-2
+00001600: 3534 3b69 6628 3236 343c 6529 7b65 2d3d  54;if(264<e){e-=
+00001610: 3235 373b 7661 7220 793d 4d5b 655d 3b6d  257;var y=M[e];m
+00001620: 3d74 2861 2c64 2c28 313c 3c79 292d 3129  =t(a,d,(1<<y)-1)
+00001630: 2b4f 5b65 5d3b 642b 3d79 7d65 3d77 5b48  +O[e];d+=y}e=w[H
+00001640: 2861 2c64 2926 4a5d 3b79 3d65 3e3e 3e34  (a,d)&J];y=e>>>4
+00001650: 3b65 7c7c 7528 3329 3b64 2b3d 6526 3135  ;e||u(3);d+=e&15
+00001660: 3b65 3d53 5b79 5d3b 333c 7926 2628 793d  ;e=S[y];3<y&&(y=
+00001670: 4e5b 795d 2c65 2b3d 4828 612c 6429 2628  N[y],e+=H(a,d)&(
+00001680: 313c 3c79 292d 312c 642b 3d79 293b 6966  1<<y)-1,d+=y);if
+00001690: 2864 3e49 297b 7126 2675 2830 293b 6272  (d>I){q&&u(0);br
+000016a0: 6561 6b7d 6626 267a 286b 2b31 3331 3037  eak}f&&z(k+13107
+000016b0: 3229 3b66 6f72 286d 3d6b 2b6d 3b6b 3c6d  2);for(m=k+m;k<m
+000016c0: 3b6b 2b3d 3429 625b 6b5d 3d62 5b6b 2d65  ;k+=4)b[k]=b[k-e
+000016d0: 5d2c 625b 6b2b 315d 3d62 5b6b 2b31 2d65  ],b[k+1]=b[k+1-e
+000016e0: 5d2c 625b 6b2b 325d 3d62 5b6b 2b32 2d65  ],b[k+2]=b[k+2-e
+000016f0: 5d2c 625b 6b2b 335d 3d62 5b6b 2b33 2d65  ],b[k+3]=b[k+3-e
+00001700: 5d3b 6b3d 6d7d 7d63 2e6c 3d70 3b63 2e70  ];k=m}}c.l=p;c.p
+00001710: 3d41 3b63 2e62 3d6b 3b63 2e66 3d43 3b70  =A;c.b=k;c.f=C;p
+00001720: 2626 2843 3d31 2c63 2e6d 3d78 2c63 2e64  &&(C=1,c.m=x,c.d
+00001730: 3d77 2c63 2e6e 3d76 297d 7768 696c 6528  =w,c.n=v)}while(
+00001740: 2143 293b 7265 7475 726e 206b 3d3d 622e  !C);return k==b.
+00001750: 6c65 6e67 7468 3f62 3a56 2862 2c30 2c6b  length?b:V(b,0,k
+00001760: 297d 3b68 3d6e 6577 206e 2830 293b 6c3d  )};h=new n(0);l=
+00001770: 2275 6e64 6566 696e 6564 2221 3d74 7970  "undefined"!=typ
+00001780: 656f 6620 5465 7874 4465 636f 6465 7226  eof TextDecoder&
+00001790: 266e 6577 2054 6578 7444 6563 6f64 6572  &new TextDecoder
+000017a0: 3b74 7279 7b6c 2e64 6563 6f64 6528 682c  ;try{l.decode(h,
+000017b0: 7b73 7472 6561 6d3a 2130 7d29 7d63 6174  {stream:!0})}cat
+000017c0: 6368 2861 297b 7d77 696e 646f 772e 756e  ch(a){}window.un
+000017d0: 7a69 703d 6675 6e63 7469 6f6e 2861 2c0a  zip=function(a,.
+000017e0: 6229 7b69 6628 3331 3d3d 615b 305d 2626  b){if(31==a[0]&&
+000017f0: 3133 393d 3d61 5b31 5d26 2638 3d3d 615b  139==a[1]&&8==a[
+00001800: 325d 297b 7661 7220 633d 612e 7375 6261  2]){var c=a.suba
+00001810: 7272 6179 3b33 313d 3d61 5b30 5d26 2631  rray;31==a[0]&&1
+00001820: 3339 3d3d 615b 315d 2626 383d 3d61 5b32  39==a[1]&&8==a[2
+00001830: 5d7c 7c75 2836 2c22 696e 7661 6c69 6420  ]||u(6,"invalid 
+00001840: 677a 6970 2064 6174 6122 293b 7661 7220  gzip data");var 
+00001850: 673d 615b 335d 2c66 3d31 303b 6726 3426  g=a[3],f=10;g&4&
+00001860: 2628 662b 3d61 5b31 305d 7c28 615b 3131  &(f+=a[10]|(a[11
+00001870: 5d3c 3c38 292b 3229 3b66 6f72 2876 6172  ]<<8)+2);for(var
+00001880: 2071 3d28 673e 3e33 2631 292b 2867 3e3e   q=(g>>3&1)+(g>>
+00001890: 3426 3129 3b30 3c71 3b71 2d3d 2161 5b66  4&1);0<q;q-=!a[f
+000018a0: 2b2b 5d29 3b63 3d63 2e63 616c 6c28 612c  ++]);c=c.call(a,
+000018b0: 662b 2867 2632 292c 2d38 293b 627c 7c28  f+(g&2),-8);b||(
+000018c0: 623d 612e 6c65 6e67 7468 2c62 3d6e 6577  b=a.length,b=new
+000018d0: 206e 2828 615b 622d 345d 7c61 5b62 2d33   n((a[b-4]|a[b-3
+000018e0: 5d3c 3c38 7c61 5b62 2d32 5d3c 3c31 367c  ]<<8|a[b-2]<<16|
+000018f0: 615b 622d 315d 3c3c 3234 293e 3e3e 3029  a[b-1]<<24)>>>0)
+00001900: 293b 613d 4b28 632c 6229 7d65 6c73 6520  );a=K(c,b)}else 
+00001910: 3821 3d28 615b 305d 2631 3529 7c7c 373c  8!=(a[0]&15)||7<
+00001920: 615b 305d 3e3e 347c 7c28 615b 305d 3c3c  a[0]>>4||(a[0]<<
+00001930: 387c 615b 315d 2925 3331 3f61 3d4b 2861  8|a[1])%31?a=K(a
+00001940: 2c62 293a 2828 3821 3d28 615b 305d 2631  ,b):((8!=(a[0]&1
+00001950: 3529 7c7c 373c 615b 305d 3e3e 3e34 7c7c  5)||7<a[0]>>>4||
+00001960: 2861 5b30 5d3c 3c38 7c61 5b31 5d29 2533  (a[0]<<8|a[1])%3
+00001970: 3129 2626 7528 362c 2269 6e76 616c 6964  1)&&u(6,"invalid
+00001980: 207a 6c69 6220 6461 7461 2229 2c61 5b31   zlib data"),a[1
+00001990: 5d26 3332 2626 7528 362c 2269 6e76 616c  ]&32&&u(6,"inval
+000019a0: 6964 207a 6c69 6220 6461 7461 3a20 7072  id zlib data: pr
+000019b0: 6573 6574 2064 6963 7469 6f6e 6172 6965  eset dictionarie
+000019c0: 7320 6e6f 7420 7375 7070 6f72 7465 6422  s not supported"
+000019d0: 292c 613d 4b28 612e 7375 6261 7272 6179  ),a=K(a.subarray
+000019e0: 2832 2c0a 2d34 292c 6229 293b 7265 7475  (2,.-4),b));retu
+000019f0: 726e 2061 7d7d 2928 293b 0a22 2222 0a    rn a}})();.""".
```

### Comparing `self-unzip-html-0.1.1/python/self_unzip_html.egg-info/PKG-INFO` & `self-unzip-html-0.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,94 @@
-Metadata-Version: 2.1
-Name: self-unzip-html
-Version: 0.1.1
-Summary: Create self-extracting HTML pages with arbitrary contents
-Home-page: https://github.com/six-two/self-unzip.html
-Author: six-two
-Author-email: pip@six-two.dev
-License: MIT License
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # self-unzip.html
 [![PyPI version](https://img.shields.io/pypi/v/self-unzip-html)](https://pypi.org/project/self-unzip-html/)
 ![License](https://img.shields.io/pypi/l/self-unzip-html)
 ![Python versions](https://img.shields.io/pypi/pyversions/self-unzip-html)
 
 This [repo](https://github.com/six-two/self-unzip.html) contains tools to create self-extracting HTML pages.
 It works by taking a payload, compressing it, and encoding the results using ASCII85.
 It then puts the resulting string in a template file, that contains the code to decode and decompress the payload again.
 
 Currently there are three actions implemented, that can be executed, after the payload is decoded:
 
-- Execute payload as JavaScript code (example usecase: obfuscate malicious JS code)
-- Show payload as HTML page (example usecase: compress a big web page)
-- Download the payload as a file (example usecase: bypass antivirus / filters)
+- `eval`: Execute payload as JavaScript code (example usecase: obfuscate malicious JS code)
+- `replace`: Show payload as HTML page (example usecase: compress a big web page)
+- `download`: Download the payload as a file (example usecase: bypass antivirus / filters)
 
 ## Demo
 
 You can try the online demo at [self-extracting-html.six-two.dev](https://self-extracting-html.six-two.dev/).
 This version is the same as the web version described below.
 It is entirely client-site, your files do not get uploaded to a server.
 
 ## Installation
 
+### Current feature comparision
+
+Currently the python version has the most features.
+
+Feature | Web version | Python version
+---|---|---
+Base64 encoding | no | yes
+Ascii85 encoding | yes | yes
+GZIP compression | yes, always | yes, can be disabled
+AES-GCM encryption | no | yes
+Automatic detection of most efficient algorithms | no | yes
+
 ### Web version
 
 There is a bare-bones page generator written in plain HTML and JavaScript.
 To use it, just clone the repo and put the contents of the `site` directory somewhere in your web server directory.
 
+You can of course also use it with Python's built in web server:
+```bash
+python3 -m http.server --directory ./site/
+```
+
 ### Python version
 
 A Python script to generate self extracting web pages is under `python/main.py`.
-It just requires a modern Python version (probably Python3.9+) and has no external dependencies.
+It just requires a modern Python version (probably Python3.9+) and has no required external dependencies (but you need to install `pycryptodomex` if you want to encrypt contents).
 
 You can also install it with `pip`:
 
+```bash
+python3 -m pip install -U self-unzip-html
+```
+
+Example usage of the pip package:
+```bash
+self-unzip-html -t download -o psexec.html ~/Downloads/SysinternalsSuite/PsExec.exe
 ```
-python3 -m pip install self-unzip-html
+
+Or if you wanted to password-protect it:
+```bash
+self-unzip-html -t download -o psexec.html -p YourPasswordHere ~/Downloads/SysinternalsSuite/PsExec.exe
 ```
 
+## Encryption
+
+Encryption uses AES-GCM for encryption and tamper detection and PBKDF2 with slightly over 1 million rounds of SHA-256 for password derivation.
+The code has not been audited, so use it with caution.
+If data security is very important to you may want to manually encrypt it beforehand (for example using `gpg`).
+
+You can automatically decrypt a page by adding the password as the hash in a URL like `encrypted.html#monkey123!`.
+The hash will not be sent to the server, so your password may only be stored locally (in your browsing history).
+Otherwise a prompt will ask you for the password.
 
-## template.html
+## JavaScript code
 
-This basically just explains, how I generated the obfuscated script in `template.html`.
+### Python
+
+The JavaScript code is modular to decrease size and allow mixing and matching different algorithms.
+The unminified files are in `code_to_minify/`.
+They are minified by running `code_to_minify/build.sh`, which updates `python/self_unzip_html/minified_js.py`.
+
+### template.html
+
+This basically just explains, how I generated the obfuscated script in `template.html` (JavaScript version).
 In case you are paranoid, you can reproduce the steps.
 Or if there is an important update to `fflate` or `ascii85`, I will have to run them again.
 
 Install with npm:
 
 ```bash
 npm install .
@@ -79,9 +105,7 @@
 The next step is optional.
 If you want to skip it, just rename `main.min.js` to `main.js` in the `output` directory.
 Otherwise minify the code (may require you to install an external minifier like closure-compiler).
 
 ```bash
 closure-compiler output/main.js --js_output_file output/main.min.js
 ```
-
-
```

### Comparing `self-unzip-html-0.1.1/setup.cfg` & `self-unzip-html-0.1.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = self-unzip-html
-version = 0.1.1
+version = 0.1.2
 author = six-two
 author_email = pip@six-two.dev
-description = Create self-extracting HTML pages with arbitrary contents
+description = Create self-extracting and/or password protected HTML pages with arbitrary contents
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/six-two/self-unzip.html
 license = MIT License
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
@@ -17,18 +17,21 @@
 
 [options]
 include_package_data = True
 package_dir = 
 	= python
 packages = find:
 python_requires = >=3.9
-scripts = 
-	python/bin/self-unzip-html.py
 install_requires = 
 
 [options.packages.find]
 where = python
 
+[options.entry_points]
+console_scripts = 
+	self-unzip-html.py = self_unzip_html:main
+	self-unzip-html = self_unzip_html:main
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

