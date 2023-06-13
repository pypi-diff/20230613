# Comparing `tmp/zpp_args-1.3.1.tar.gz` & `tmp/zpp_args-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpp_args-1.3.1.tar", last modified: Mon Dec 26 19:06:46 2022, max compression
+gzip compressed data, was "zpp_args-1.3.2.tar", last modified: Tue Jun 13 07:53:40 2023, max compression
```

## Comparing `zpp_args-1.3.1.tar` & `zpp_args-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-12-26 19:06:46.138000 zpp_args-1.3.1/
--rw-rw-rw-   0        0        0     3345 2022-12-26 19:06:46.135000 zpp_args-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2718 2022-12-23 08:35:38.000000 zpp_args-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2022-12-26 19:06:46.137000 zpp_args-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      777 2022-08-05 08:05:17.000000 zpp_args-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-26 19:06:46.108000 zpp_args-1.3.1/zpp_args/
--rw-rw-rw-   0        0        0      246 2022-12-26 19:03:24.000000 zpp_args-1.3.1/zpp_args/__init__.py
--rw-rw-rw-   0        0        0    11718 2022-12-26 19:02:55.000000 zpp_args-1.3.1/zpp_args/args.py
-drwxrwxrwx   0        0        0        0 2022-12-26 19:06:46.130000 zpp_args-1.3.1/zpp_args.egg-info/
--rw-rw-rw-   0        0        0     3345 2022-12-26 19:06:45.000000 zpp_args-1.3.1/zpp_args.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2022-12-26 19:06:45.000000 zpp_args-1.3.1/zpp_args.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-26 19:06:45.000000 zpp_args-1.3.1/zpp_args.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-12-26 19:06:45.000000 zpp_args-1.3.1/zpp_args.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 07:53:40.610000 zpp_args-1.3.2/
+-rw-rw-rw-   0        0        0     1106 2023-06-13 07:51:54.000000 zpp_args-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-06-13 07:53:40.606000 zpp_args-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2718 2022-12-23 08:35:38.000000 zpp_args-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:53:40.609000 zpp_args-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      777 2022-08-05 08:05:21.000000 zpp_args-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:53:40.577000 zpp_args-1.3.2/zpp_args/
+-rw-rw-rw-   0        0        0      246 2022-12-26 19:03:30.000000 zpp_args-1.3.2/zpp_args/__init__.py
+-rw-rw-rw-   0        0        0    10766 2023-06-13 07:49:11.000000 zpp_args-1.3.2/zpp_args/args.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:53:40.602000 zpp_args-1.3.2/zpp_args.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-06-13 07:53:40.000000 zpp_args-1.3.2/zpp_args.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-13 07:53:40.000000 zpp_args-1.3.2/zpp_args.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:53:40.000000 zpp_args-1.3.2/zpp_args.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 07:53:40.000000 zpp_args-1.3.2/zpp_args.egg-info/top_level.txt
```

### Comparing `zpp_args-1.3.1/PKG-INFO` & `zpp_args-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: zpp_args
-Version: 1.3.1
+Version: 1.3.2
 Summary: Module pour le traitement des arguments d'une ligne de commande
 Home-page: https://github.com/ZephyrOff/py-zpp_args
-Author: ZephyrOff
-Author-email: contact@apajak.fr
-License: MIT
+Author: 
+License: MIT License
+Project-URL: Documentation, https://github.com/ZephyrOff/py-zpp_args
 Keywords: terminal args zephyroff
 Platform: ALL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # zpp-args
 ## Informations
 Module pour le traitement des arguments d'une ligne de commande.
 <br>Trois sources possibles:
 - sys.argv
 - une chaÃ®ne de caractÃ¨re
```

### Comparing `zpp_args-1.3.1/README.md` & `zpp_args-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `zpp_args-1.3.1/setup.py` & `zpp_args-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `zpp_args-1.3.1/zpp_args/args.py` & `zpp_args-1.3.2/zpp_args/args.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-####################################################################
-#/ Nom du projet: py-zpp_args                                     /#
-#/ Nom du fichier: args.py                                        /#
-#/ Type de fichier: fichier principal                             /#
-#/ Fichier annexe:                                                /#
-#/                                                                /#
-#/ Auteur: ZephyrOff  (Alexandre Pajak)                           /#
-#/ Version: 1.3.1                                                 /#
-#/ Description: Module pour le traitement des arguments d'une     /#
-#/              ligne de commande                                 /#
-#/ Date: 26/12/2022                                               /#
-####################################################################
-
 import sys
 import inspect
 import re
 
 def get_origin_value():
 	frame = inspect.currentframe()
 	frame = inspect.getouterframes(frame)[2]
@@ -55,19 +42,15 @@
 		self.error_lock = error_lock
 		self.check_parameter = True
 
 		if source==None:
 			self.command = sys.argv[0]
 			self.source=sys.argv[1:]
 		else:
-			if "sys.argv" in get_origin_value()[0]:
-				self.command = source[0]
-				self.source = source[1:]
-			else:
-				self.command, self.source = self.arg_parse(source)
+			self.command, self.source = self.arg_parse(source)
 
 	def search(self, option):
 		for element in self.available_arg:
 			if element['longname']==option:
 				return element
 		return None
 
@@ -430,15 +413,15 @@
 							ins[1]+=" "
 
 						if a['default']==True:
 							ins[1]+=" (Default Value: True)"
 						elif a['default']==False:
 							ins[1]+=" (Default Value: False)"
 						else:
-							ins[1]+=" (Default Value: "+a['default']+")"
+							ins[1]+=" (Default Value: "+str(a['default'])+")"
 
 					ar.append(ins)
 
 				for a in ar:
 					print(padding+a[0]+" "*((maxsize-len(a[0]))+3)+a[1])
 
 		if len(self.available_param)!=0:
```

### Comparing `zpp_args-1.3.1/zpp_args.egg-info/PKG-INFO` & `zpp_args-1.3.2/zpp_args.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: zpp-args
-Version: 1.3.1
+Version: 1.3.2
 Summary: Module pour le traitement des arguments d'une ligne de commande
 Home-page: https://github.com/ZephyrOff/py-zpp_args
-Author: ZephyrOff
-Author-email: contact@apajak.fr
-License: MIT
+Author: 
+License: MIT License
+Project-URL: Documentation, https://github.com/ZephyrOff/py-zpp_args
 Keywords: terminal args zephyroff
 Platform: ALL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # zpp-args
 ## Informations
 Module pour le traitement des arguments d'une ligne de commande.
 <br>Trois sources possibles:
 - sys.argv
 - une chaÃ®ne de caractÃ¨re
```

