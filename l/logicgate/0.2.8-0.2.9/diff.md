# Comparing `tmp/logicgate-0.2.8.tar.gz` & `tmp/logicgate-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logicgate-0.2.8.tar", max compression
+gzip compressed data, was "logicgate-0.2.9.tar", max compression
```

## Comparing `logicgate-0.2.8.tar` & `logicgate-0.2.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 logicgate-0.2.8/LICENSE
--rw-r--r--   0        0        0    14816 2023-06-11 02:08:02.744878 logicgate-0.2.8/LogicGate/LogicGate.py
--rw-r--r--   0        0        0     4622 2023-06-11 02:11:16.320620 logicgate-0.2.8/LogicGate/lgEncrypt.py
--rw-r--r--   0        0        0     5568 2023-06-11 02:14:45.760318 logicgate-0.2.8/README.rst
--rw-r--r--   0        0        0      827 2023-06-11 02:15:11.204283 logicgate-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6461 1970-01-01 00:00:00.000000 logicgate-0.2.8/setup.py
--rw-r--r--   0        0        0     6386 1970-01-01 00:00:00.000000 logicgate-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 logicgate-0.2.9/LICENSE
+-rw-r--r--   0        0        0    14976 2023-06-13 05:54:38.782321 logicgate-0.2.9/LogicGate/LogicGate.py
+-rw-r--r--   0        0        0     5056 2023-06-13 06:23:58.627953 logicgate-0.2.9/LogicGate/lgEncrypt.py
+-rw-r--r--   0        0        0     6131 2023-06-13 06:38:25.686787 logicgate-0.2.9/README.rst
+-rw-r--r--   0        0        0      836 2023-06-13 06:40:26.550624 logicgate-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     7028 1970-01-01 00:00:00.000000 logicgate-0.2.9/setup.py
+-rw-r--r--   0        0        0     6958 1970-01-01 00:00:00.000000 logicgate-0.2.9/PKG-INFO
```

### Comparing `logicgate-0.2.8/LICENSE` & `logicgate-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `logicgate-0.2.8/LogicGate/LogicGate.py` & `logicgate-0.2.9/LogicGate/LogicGate.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,37 +220,39 @@
     raise FileNotFoundError(
       f'{filename} is not an existing file from given path, prehaps try moving the file to the same directory as this program?'
     )
 
 
 def compile(
   filename: str = 'main.lgeso',
-  output: str = 'Hello World!',
+  message: str = 'Hello World!',
   randomize: bool = True,
   random_range: list = [1, 5],
   write: bool = True,
+  output: bool = True,
   override: bool = False,
   BitLock: int = -1
 ) -> str | None:
   """compile string to lgeso file, random_range is needed only when randomize is true.
   filename: string, specify which file to write the data into, new file named as filename will be created if it doesn't exist
-  output: string, specify what result will be produced
+  message: string, specify what will be compiled
   randomize: boolean, if the data written is pure binary or further encrypted with gates
   random_range: list, the maximum set of gates in the written data will be the square of the second item while the minimum will be the square of the first item.
   write: boolean, if the result is returned or is written to file
+  output: boolean, determine if outputs are present
   override: boolean, safety checks are off and outputs are disabled, proceed with caution
   BitLock: integer, if the binary of a character is shorter than this value, 0 will be appended. Defalt is -1, which is off, all negative number will be counted as ignore as well"""
 
   out = ""
-  override = not override
-  if not output.isascii() and override:
+  override = not (override or not output) #variable "override" after this line is reversed for shorter code
+  if not message.isascii() and override:
     raise ValueError(
-      f'message received ({repr(output)}) is not available in ascii')
-  if not output and override:
-    output = 'Hello World!'
+      f'message received ({repr(message)}) is not available in ascii')
+  if not message and override:
+    message = 'Hello World!'
   if filename and write and override:
     if len(filename) > 6:
       if filename[-6:] != '.lgeso':
         print(f'filename is not an lgeso file, filename changed to {filename}')
         filename += '.lgeso'
     elif '.' in filename:
       print(f'filename is not an lgeso file, filename changed to {filename}')
@@ -273,28 +275,28 @@
       except ValueError:
         if override:
           print('invalid random range received, changed to 1-5')
           random_range = [1, 5]
           break
       else:
         if (check < 1 or check > (sqrt(sys.getrecursionlimit()) // 3)
-            ) and override:  #avoid overflow error when running
+            ) and override:  #avoid overflow error when decompiling
           print(
             'an item in random range is too large or too small, changed to 1-5'
           )
           random_range = [1, 5]
           break
-    for char in output:
+    for char in message:
       line = str(bin(ord(char))[2:])
       if len(line) < BitLock and BitLock >= 0:
         for _ in range(BitLock - len(line)):
           line = '0' + line
       for char in line:
         if randomize:
-          charGoal = int(char)  #the ideal final output after the randomizing
+          charGoal = int(char)  #the expected bit after the randomizing
           for _ in range(
               randint(random_range[0], random_range[1]) *
               randint(random_range[0], random_range[1])):
             gates = randint(0, 3)
             if gates == 1:
               char = ('N0' if char == '1' else 'N1' if char == '0' else
                       ('NN' + char))
@@ -308,17 +310,17 @@
           f.write(char + '\n')
         else:
           out += char
       if write:
         f.write('---\n')
       else:
         out += "-"
-    if override:
+    if output:
       print(
-        f'compilation completed and result {"written in" if write else "returned"} {filename if write else ""} with output as {output}\nrandomizaion is {"on" if randomize else "off"}\n\n\n'
+        f'compilation completed and result {"written in" if write else "returned"} {filename if write else ""} with output as {message}\nrandomizaion is {"on" if randomize else "off"}\n\n\n'
       )
     return None if write else out
 
 
 def run(
     filename: str,
     gate: bool = False,
@@ -349,8 +351,8 @@
                    gate=gate,
                    ascii=ascii,
                    debug=debug,
                    check=check,
                    out=out)
 
 if __name__ == '__main__':
-  exit(run((str(argv[1]) if len(argv) != 1 else 'main.lgeso')))
+  exit(decompile((str(argv[1]) if len(argv) != 1 else 'main.lgeso')))
```

### Comparing `logicgate-0.2.8/LogicGate/lgEncrypt.py` & `logicgate-0.2.9/LogicGate/lgEncrypt.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 except ImportError:
   raise ImportError('module require LogicGate, LogicGate not found')
 
 
 def encrypt(filename: str = "main.lgeso",
             key_file: str = "key.lgeso",
             msg: str = "Hello World!",
-            no_output : bool = False):
+            output : bool = True):
   """
   an encryption module with the help of LogicGate main module, LogicGate.py is needed.
   Note: this encryption method is not safe, anyone with the data of the 2 files will be able to see the information. 
   filename: string, file to write the encrypted code to
   key_file: string, file to keep the key string into
   msg: string, word to encrypt
+  output: boolean, whether outputs are present or not
   """
 
   if not msg.isascii():
     raise ValueError(
       f'message received ({repr(msg)}) is not available in ascii')
   k, f, kOut, fOut = [''] * 4
   data = []
@@ -72,61 +73,67 @@
   for fChek, kChek in zip(chekF, chekK):
     for objF, objK in zip(fChek, kChek):
       if objK != objF:
         checkBuf.append(objF)
   for chek in range(0, len(checkBuf), 7):
     check.append(checkBuf[chek:chek + 7])
   for n in range(0, len(data) - 1):
-    if str(data[n]) != ''.join(check[n]) and not no_output:
+    if str(data[n]) != ''.join(check[n]) and output:
 
       print('BitWarning: bit unaligned\ndata bit : compile bit\n' +
             str(data[n]) + ' : ' + ''.join(check[n]) + '\n')
   lg.compile(filename,
              fOut,
              random_range=(10, sqrt(maxcur()) // 3),
+             output=output,
              override=True,
              BitLock=7)
   lg.compile(key_file,
              kOut,
              random_range=(10, sqrt(maxcur()) // 3),
+             output=output,
              override=True,
              BitLock=7)
 
 
-def decrypt(filename: str, key_file: str, sause: bool = False):
+def decrypt(filename: str, key_file: str, sause: bool = False, debug: bool = False, debug_ALL: bool = False):
   """basic decryption, filename and keyfile is required.
   If sause is True, no output will be give pn out but result returned, normally used for another module's extra encryption
+  If debug is on, all hidden outout will be outputted.
+  If debug_ALL is on, every single coded output sentense except warning or error will be outputted, this will create a massive lag and do not recommend
+
   NOTE: file __decrypt__.lgeso and will be used for temperary data store and bypasser for LogicGate.decompile lgeso file locker.
   THE FILE WILL BE CLEARED, WRITTEN AND DELETED AFTER USING THIS FUNCTON"""
   if exists(filename) and exists(key_file):
     with open(filename, 'r') as f, open(key_file, 'r') as k:
       dk = open('__decrypt__.lgeso', 'w')
       Fdt = f.read()
       Kdt = k.read()
       dk.write(Kdt)
       dk.close()
-      CheckStr = lg.decompile('__decrypt__.lgeso', ascii=True, out=False)
+      CheckStr = lg.decompile('__decrypt__.lgeso', ascii=True, debug=debug_ALL, out=debug)
       df = open('__decrypt__.lgeso', 'w')
       df.write(Fdt)
       df.close()
       out = lg.decompile('__decrypt__.lgeso',
                    ascii=True,
                    gate=True,
                    check=CheckStr,
-                   out=False).split('-')
+                   debug=debug_ALL,
+                   out=debug).split('-')
       do = open('__decrypt__.lgeso', 'w')
       out = ''.join(out)
       outP = []
       for O in range(0, len(out), 7):
         outP.append(out[O:O + 7])
       for n in outP:
         do.write("\n".join(n))
         do.write("\n---\n")
       do.close()
-      out = lg.decompile('__decrypt__.lgeso', gate=True, out=not sause)
+      out = lg.decompile('__decrypt__.lgeso', gate=True, debug=debug_ALL, out=(debug or not sause))
       remove('__decrypt__.lgeso')
       return out
   else:
     print("filename or key_file doesn't exist, exiting")
 
 
 if __name__ == '__main__':
```

### Comparing `logicgate-0.2.8/README.rst` & `logicgate-0.2.9/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,46 +2,49 @@
 =========
 
 This language is inspired by logic gates, by using simple alphabet you could make a program.
 
 It is designed as a way for manual encryption, which kinda failed
 
 All you can do in this language is to make a program with logic gates,
-sounds difficult and indeed it is.
+sounds difficult but it depends.
 
 Startup
 -------
 
 First, make a logic gate file. The file extension should be .lgeso
 
-Runner
-------
+Functions
+---------
+
+*Note, this README may sometimes be outdated due to how lazy and busy the dev is, for the most updated description of the function arguments please use "help({func})" and replace {func} with the function you want to check, thank you.*
 
 To use it, import **LogicGate** in your python script.
 
 Remember for the decompile function, only the filename argument is needed.
 
-The decompile function will return the incorrect bits if check, gate and ascii is True, decompiled result if ascii is True, and 0 if otherwise.
+The *decompile* function will return the incorrect bits if check, gate and ascii is True, decompiled result if ascii is True, and 0 if otherwise.
 
 Outputs of the file will be printed(binary to ascii, and logical binary if enabled) if out is True (true by defalt).
 
 
-The compile function does the otherwise, it normally doesn't return anything but it can write code into lgeso file, or if write is False(defalt on) then the compiled result will be returned instead of writing into file.
+The *compile* function does the otherwise, it normally doesn't return anything but it can write code into lgeso file, or if write is False(defalt True) then the compiled result will be returned instead of writing into file.
 
 Special encrypt module
 ----------------------
 a special encrypt module is included in this package, which is **lgEncrypt**.
 
 it contain two functions, encrypt() and decrypt().
 
-encrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt(). 
-encrypt() have 4 arguments, data file name, key file name, message, no_output. They are very self explainatory
+*encrypt()* generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt(). 
+encrypt() have 4 arguments, data file name, key file name, message, output. They are very self explainatory
 
-decrypt() have 3 arguments, data file, key file, sause. 
-the first 2 is very self explainatory, for sause parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand
+*decrypt()* have 5 arguments, data file, key file, sause, debug, debug_ALL. 
+the first 2 is very self explainatory, for *sause* parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand.
+For *debug*, it shows the print output that is hidden, it can be enabled for you to check which bit is wrong. For *debug_ALL* it purposely enable everything that is coded with printing(output) except warnings and errors, this will definatly cause massive lag so it is not recommended to enable.
 
 syntax
 ------
 
 For syntax it is very straight forward. It process each character in
 every line as individual command.
```

### Comparing `logicgate-0.2.8/pyproject.toml` & `logicgate-0.2.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LogicGate"
-version = "0.2.8"
+version = "0.2.9"
 description = "an esolang designed for manual encryption with logic gates"
 license = "MIT"
 authors = ["Taokyle <taokyle415@gmail.com>"]
 readme = "README.rst"
 repository = "https://replit.com/@s3D27ZHOU/LogicGate"
 keywords = ["logic", "gate", "encrypt", "encryption"]
 packages = [
@@ -21,8 +21,8 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "github" = "https://github.com/TaokyleYT/LogicGate"
 "up-to-date source code(replit)" = "https://replit.com/@s3D27ZHOU/LogicGate"
-"esolang wiki" = "https://esolangs.org/wiki/LogicGate"
+"outdated esolang wiki" = "https://esolangs.org/wiki/LogicGate"
```

### Comparing `logicgate-0.2.8/setup.py` & `logicgate-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 package_dir = \
 {'': 'LogicGate'}
 
 modules = \
 ['LogicGate', 'lgEncrypt']
 setup_kwargs = {
     'name': 'logicgate',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'an esolang designed for manual encryption with logic gates',
-    'long_description': "LogicGate\n=========\n\nThis language is inspired by logic gates, by using simple alphabet you could make a program.\n\nIt is designed as a way for manual encryption, which kinda failed\n\nAll you can do in this language is to make a program with logic gates,\nsounds difficult and indeed it is.\n\nStartup\n-------\n\nFirst, make a logic gate file. The file extension should be .lgeso\n\nRunner\n------\n\nTo use it, import **LogicGate** in your python script.\n\nRemember for the decompile function, only the filename argument is needed.\n\nThe decompile function will return the incorrect bits if check, gate and ascii is True, decompiled result if ascii is True, and 0 if otherwise.\n\nOutputs of the file will be printed(binary to ascii, and logical binary if enabled) if out is True (true by defalt).\n\n\nThe compile function does the otherwise, it normally doesn't return anything but it can write code into lgeso file, or if write is False(defalt on) then the compiled result will be returned instead of writing into file.\n\nSpecial encrypt module\n----------------------\na special encrypt module is included in this package, which is **lgEncrypt**.\n\nit contain two functions, encrypt() and decrypt().\n\nencrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt(). \nencrypt() have 4 arguments, data file name, key file name, message, no_output. They are very self explainatory\n\ndecrypt() have 3 arguments, data file, key file, sause. \nthe first 2 is very self explainatory, for sause parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand\n\nsyntax\n------\n\nFor syntax it is very straight forward. It process each character in\nevery line as individual command.\n\nFor gates with multiple inputs (such as or,\nand) type like other syntax, the quota for the gate will automatically be processed. Any invalid command will raise SyntaxError, in almost all scenarios, the case of the gate does not matter.\n\nBasic gates(gates that doesn’t require includes, include feature is in progress):\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nA (and gate): the next **2** results will be accepted as inputs. If both\ninputs are 1, output is 1, else 0\n\nO (or gate): the next **2** results will be accepted as inputs. If one\nof the inputs are 1, output is 1, else 0\n\nN (not gate): the next **1** result will be accepted as inputs. If the\ninput is 1, output is 0, else 0\n\n1 and 0 (True and False): **NO** result will be accepted as inputs. They\nare the results, self explanatory\n\nspecial syntax\n~~~~~~~~~~~~~~\n\nThere are 2 special syntax\n\n—-- (three hyphens): new word, used for the ascii output separating the binary for ascii translation. Everything else on the line with this syntax will be ignored.\n\n### (three hashes): comment everything after the syntax\n\nFor any of the special syntax, they are not being interpreted as special syntax unless the entire syntax appears. They can be anywhere in a line, and that line will act like what the syntax shows (if more tham one special syntax appears in the same line, they will be scanned and processed according\nto here)\n\nexamples\n========\n\nThis is a hello world in LogicGate\n\n``1\\n 0\\n 0\\n 1\\n 0\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 0\\n ---\\n 1\\n 0\\n 1\\n 0\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 0\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 1\\n``\n\nanother version generated by LogicGate.compile():\n``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\\n NNANNAAAO0O000001\\n OO0NNN10\\n O1O1NNA1O01\\n NNOONNA0O0000\\n 0\\n AA0NNANNOONNNNAO0A1O0000001\\n ---\\n OO1O1OAO1NNAO111111\\n NNNNO0NNAA1O0N01\\n OANNOA0O00000\\n ANNNNA001\\n NNA11\\n NNANNA1ANNO0001\\n NNAANNAOOA1NNAO10110111\\n ---\\n OA111\\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\\n A1O0A00\\n A1O0NNAO0O0A111\\n NNAO1NNONNNNA1O1111\\n O0A1OANNA0NNOO0ON10000\\n 0\\n ---\\n O0NNN0\\n A1ANNNNNNNNNNO101\\n O00\\n NNA1OO1ONNAO10110\\n OAA1110\\n OO0AAO0AAONNO0O0NNO00001100\\n NNO0A0ONNN10\\n ---\\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\\n NNANNO1ONNNNNNNNNNO0AO11101\\n O0OONNNNAAO0N11000\\n A1O0N0\\n OONNNNOA1ONNOO0AA11100100\\n NNO0ON00\\n O0OA1NNA1O100\\n ---\\n O0OO1OO1A1O1000\\n NNOO0AONNONNO0A0NNA0NNA010010\\n NNAA0OOOA0O000001\\n A0NNNNN1\\n AO0NNNNA1OO0001\\n O0OA1O0O0OO0OA1O00000\\n ---\\n 1\\n A0NNAO0A0OA0NNA1A0000\\n NNO0NNA1NNOO011\\n NNO0NNA0A0A0NNOO000\\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\\n NNA1ANNA1OAO1O11111\\n A1A1NNA1O1NNANNA1AA1111\\n ---\\n ONNNNAOO11110\\n OANNOONNA1AA1110111\\n AA0NNNNNNO0O0A0O0N10\\n NNNNNNOA110\\n O1OONNA1101\\n A1NNNNA11\\n ANNOONNAAO1A1ANNA11111011\\n ---\\n O0NNO0AO0A111\\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\\n NNO11\\n AO0AN101\\n OAA1000\\n 1\\n O0A0NNO0O0NNA0A0NNA1ON10\\n ---\\n O0N0\\n NNNNNNO0ONNA1N00\\n O00\\n O0AN01\\n NNONNNNNNNNA111\\n NNNNONNOO0000\\n AONNO0ANNO00101\\n ---\\n O1ONNANNNNA1111\\n NNNNOOOO0NNAA1NNONNO1011111\\n NNA0A0A01\\n AA1N10\\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\\n 0\\n OOAO0NNO0A0OAANNA0AONNO0001100000\\n ---\\n A1A1NNO0NNA11\\n OA100\\n NNANNOA1001\\n 0\\n NNO0OA0O000\\n ANNO0OONNA1O11001\\n ---``\n\nSources\n-------\n\n`gitbub\n<https://github.com/TaokyleYT/LogicGate/>`__\\\n\nEsolang seldom outdated wiki:\n`LogicGate <https://esolangs.org/wiki/LogicGate>`__\\\n\nReplit up-to-date version:\n`replit <https://replit.com/@s3D27ZHOU/LogicGate>`__\n",
+    'long_description': 'LogicGate\n=========\n\nThis language is inspired by logic gates, by using simple alphabet you could make a program.\n\nIt is designed as a way for manual encryption, which kinda failed\n\nAll you can do in this language is to make a program with logic gates,\nsounds difficult but it depends.\n\nStartup\n-------\n\nFirst, make a logic gate file. The file extension should be .lgeso\n\nFunctions\n---------\n\n*Note, this README may sometimes be outdated due to how lazy and busy the dev is, for the most updated description of the function arguments please use "help({func})" and replace {func} with the function you want to check, thank you.*\n\nTo use it, import **LogicGate** in your python script.\n\nRemember for the decompile function, only the filename argument is needed.\n\nThe *decompile* function will return the incorrect bits if check, gate and ascii is True, decompiled result if ascii is True, and 0 if otherwise.\n\nOutputs of the file will be printed(binary to ascii, and logical binary if enabled) if out is True (true by defalt).\n\n\nThe *compile* function does the otherwise, it normally doesn\'t return anything but it can write code into lgeso file, or if write is False(defalt True) then the compiled result will be returned instead of writing into file.\n\nSpecial encrypt module\n----------------------\na special encrypt module is included in this package, which is **lgEncrypt**.\n\nit contain two functions, encrypt() and decrypt().\n\n*encrypt()* generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt(). \nencrypt() have 4 arguments, data file name, key file name, message, output. They are very self explainatory\n\n*decrypt()* have 5 arguments, data file, key file, sause, debug, debug_ALL. \nthe first 2 is very self explainatory, for *sause* parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand.\nFor *debug*, it shows the print output that is hidden, it can be enabled for you to check which bit is wrong. For *debug_ALL* it purposely enable everything that is coded with printing(output) except warnings and errors, this will definatly cause massive lag so it is not recommended to enable.\n\nsyntax\n------\n\nFor syntax it is very straight forward. It process each character in\nevery line as individual command.\n\nFor gates with multiple inputs (such as or,\nand) type like other syntax, the quota for the gate will automatically be processed. Any invalid command will raise SyntaxError, in almost all scenarios, the case of the gate does not matter.\n\nBasic gates(gates that doesn’t require includes, include feature is in progress):\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nA (and gate): the next **2** results will be accepted as inputs. If both\ninputs are 1, output is 1, else 0\n\nO (or gate): the next **2** results will be accepted as inputs. If one\nof the inputs are 1, output is 1, else 0\n\nN (not gate): the next **1** result will be accepted as inputs. If the\ninput is 1, output is 0, else 0\n\n1 and 0 (True and False): **NO** result will be accepted as inputs. They\nare the results, self explanatory\n\nspecial syntax\n~~~~~~~~~~~~~~\n\nThere are 2 special syntax\n\n—-- (three hyphens): new word, used for the ascii output separating the binary for ascii translation. Everything else on the line with this syntax will be ignored.\n\n### (three hashes): comment everything after the syntax\n\nFor any of the special syntax, they are not being interpreted as special syntax unless the entire syntax appears. They can be anywhere in a line, and that line will act like what the syntax shows (if more tham one special syntax appears in the same line, they will be scanned and processed according\nto here)\n\nexamples\n========\n\nThis is a hello world in LogicGate\n\n``1\\n 0\\n 0\\n 1\\n 0\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 0\\n ---\\n 1\\n 0\\n 1\\n 0\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 0\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 1\\n``\n\nanother version generated by LogicGate.compile():\n``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\\n NNANNAAAO0O000001\\n OO0NNN10\\n O1O1NNA1O01\\n NNOONNA0O0000\\n 0\\n AA0NNANNOONNNNAO0A1O0000001\\n ---\\n OO1O1OAO1NNAO111111\\n NNNNO0NNAA1O0N01\\n OANNOA0O00000\\n ANNNNA001\\n NNA11\\n NNANNA1ANNO0001\\n NNAANNAOOA1NNAO10110111\\n ---\\n OA111\\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\\n A1O0A00\\n A1O0NNAO0O0A111\\n NNAO1NNONNNNA1O1111\\n O0A1OANNA0NNOO0ON10000\\n 0\\n ---\\n O0NNN0\\n A1ANNNNNNNNNNO101\\n O00\\n NNA1OO1ONNAO10110\\n OAA1110\\n OO0AAO0AAONNO0O0NNO00001100\\n NNO0A0ONNN10\\n ---\\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\\n NNANNO1ONNNNNNNNNNO0AO11101\\n O0OONNNNAAO0N11000\\n A1O0N0\\n OONNNNOA1ONNOO0AA11100100\\n NNO0ON00\\n O0OA1NNA1O100\\n ---\\n O0OO1OO1A1O1000\\n NNOO0AONNONNO0A0NNA0NNA010010\\n NNAA0OOOA0O000001\\n A0NNNNN1\\n AO0NNNNA1OO0001\\n O0OA1O0O0OO0OA1O00000\\n ---\\n 1\\n A0NNAO0A0OA0NNA1A0000\\n NNO0NNA1NNOO011\\n NNO0NNA0A0A0NNOO000\\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\\n NNA1ANNA1OAO1O11111\\n A1A1NNA1O1NNANNA1AA1111\\n ---\\n ONNNNAOO11110\\n OANNOONNA1AA1110111\\n AA0NNNNNNO0O0A0O0N10\\n NNNNNNOA110\\n O1OONNA1101\\n A1NNNNA11\\n ANNOONNAAO1A1ANNA11111011\\n ---\\n O0NNO0AO0A111\\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\\n NNO11\\n AO0AN101\\n OAA1000\\n 1\\n O0A0NNO0O0NNA0A0NNA1ON10\\n ---\\n O0N0\\n NNNNNNO0ONNA1N00\\n O00\\n O0AN01\\n NNONNNNNNNNA111\\n NNNNONNOO0000\\n AONNO0ANNO00101\\n ---\\n O1ONNANNNNA1111\\n NNNNOOOO0NNAA1NNONNO1011111\\n NNA0A0A01\\n AA1N10\\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\\n 0\\n OOAO0NNO0A0OAANNA0AONNO0001100000\\n ---\\n A1A1NNO0NNA11\\n OA100\\n NNANNOA1001\\n 0\\n NNO0OA0O000\\n ANNO0OONNA1O11001\\n ---``\n\nSources\n-------\n\n`gitbub\n<https://github.com/TaokyleYT/LogicGate/>`__\\\n\nEsolang seldom outdated wiki:\n`LogicGate <https://esolangs.org/wiki/LogicGate>`__\\\n\nReplit up-to-date version:\n`replit <https://replit.com/@s3D27ZHOU/LogicGate>`__\n',
     'author': 'Taokyle',
     'author_email': 'taokyle415@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://replit.com/@s3D27ZHOU/LogicGate',
     'package_dir': package_dir,
     'py_modules': modules,
```

### Comparing `logicgate-0.2.8/PKG-INFO` & `logicgate-0.2.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 Metadata-Version: 2.1
 Name: logicgate
-Version: 0.2.8
+Version: 0.2.9
 Summary: an esolang designed for manual encryption with logic gates
 Home-page: https://replit.com/@s3D27ZHOU/LogicGate
 License: MIT
 Keywords: logic,gate,encrypt,encryption
 Author: Taokyle
 Author-email: taokyle415@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://replit.com/@s3D27ZHOU/LogicGate
-Project-URL: esolang wiki, https://esolangs.org/wiki/LogicGate
 Project-URL: github, https://github.com/TaokyleYT/LogicGate
+Project-URL: outdated esolang wiki, https://esolangs.org/wiki/LogicGate
 Project-URL: up-to-date source code(replit), https://replit.com/@s3D27ZHOU/LogicGate
 Description-Content-Type: text/x-rst
 
 LogicGate
 =========
 
 This language is inspired by logic gates, by using simple alphabet you could make a program.
 
 It is designed as a way for manual encryption, which kinda failed
 
 All you can do in this language is to make a program with logic gates,
-sounds difficult and indeed it is.
+sounds difficult but it depends.
 
 Startup
 -------
 
 First, make a logic gate file. The file extension should be .lgeso
 
-Runner
-------
+Functions
+---------
+
+*Note, this README may sometimes be outdated due to how lazy and busy the dev is, for the most updated description of the function arguments please use "help({func})" and replace {func} with the function you want to check, thank you.*
 
 To use it, import **LogicGate** in your python script.
 
 Remember for the decompile function, only the filename argument is needed.
 
-The decompile function will return the incorrect bits if check, gate and ascii is True, decompiled result if ascii is True, and 0 if otherwise.
+The *decompile* function will return the incorrect bits if check, gate and ascii is True, decompiled result if ascii is True, and 0 if otherwise.
 
 Outputs of the file will be printed(binary to ascii, and logical binary if enabled) if out is True (true by defalt).
 
 
-The compile function does the otherwise, it normally doesn't return anything but it can write code into lgeso file, or if write is False(defalt on) then the compiled result will be returned instead of writing into file.
+The *compile* function does the otherwise, it normally doesn't return anything but it can write code into lgeso file, or if write is False(defalt True) then the compiled result will be returned instead of writing into file.
 
 Special encrypt module
 ----------------------
 a special encrypt module is included in this package, which is **lgEncrypt**.
 
 it contain two functions, encrypt() and decrypt().
 
-encrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt(). 
-encrypt() have 4 arguments, data file name, key file name, message, no_output. They are very self explainatory
+*encrypt()* generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt(). 
+encrypt() have 4 arguments, data file name, key file name, message, output. They are very self explainatory
 
-decrypt() have 3 arguments, data file, key file, sause. 
-the first 2 is very self explainatory, for sause parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand
+*decrypt()* have 5 arguments, data file, key file, sause, debug, debug_ALL. 
+the first 2 is very self explainatory, for *sause* parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand.
+For *debug*, it shows the print output that is hidden, it can be enabled for you to check which bit is wrong. For *debug_ALL* it purposely enable everything that is coded with printing(output) except warnings and errors, this will definatly cause massive lag so it is not recommended to enable.
 
 syntax
 ------
 
 For syntax it is very straight forward. It process each character in
 every line as individual command.
```

