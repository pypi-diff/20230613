# Comparing `tmp/zpenv-1.3.0.tar.gz` & `tmp/zpenv-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpenv-1.3.0.tar", last modified: Wed Jun  7 13:25:59 2023, max compression
+gzip compressed data, was "zpenv-1.3.1.tar", last modified: Tue Jun 13 08:37:41 2023, max compression
```

## Comparing `zpenv-1.3.0.tar` & `zpenv-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 13:25:59.402000 zpenv-1.3.0/
--rw-rw-rw-   0        0        0     1106 2023-06-06 20:57:27.000000 zpenv-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     5576 2023-06-07 13:25:59.373000 zpenv-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2023-06-07 09:51:42.000000 zpenv-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 13:25:59.394000 zpenv-1.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-07 13:25:58.944000 zpenv-1.3.0/zpenv/
--rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.3.0/zpenv/__init__.py
--rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.3.0/zpenv/__main__.py
--rw-rw-rw-   0        0        0    33328 2023-06-07 13:24:08.000000 zpenv-1.3.0/zpenv/zpenv.py
-drwxrwxrwx   0        0        0        0 2023-06-07 13:25:59.295000 zpenv-1.3.0/zpenv.egg-info/
--rw-rw-rw-   0        0        0     5576 2023-06-07 13:25:57.000000 zpenv-1.3.0/zpenv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-07 13:25:58.000000 zpenv-1.3.0/zpenv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 13:25:57.000000 zpenv-1.3.0/zpenv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-07 13:25:57.000000 zpenv-1.3.0/zpenv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-06-07 13:25:57.000000 zpenv-1.3.0/zpenv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 13:25:58.000000 zpenv-1.3.0/zpenv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 08:37:41.393000 zpenv-1.3.1/
+-rw-rw-rw-   0        0        0     1106 2023-06-06 20:57:27.000000 zpenv-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5726 2023-06-13 08:37:41.388000 zpenv-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5119 2023-06-07 13:28:05.000000 zpenv-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 08:37:41.391000 zpenv-1.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 08:37:41.349000 zpenv-1.3.1/zpenv/
+-rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.3.1/zpenv/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.3.1/zpenv/__main__.py
+-rw-rw-rw-   0        0        0    33385 2023-06-13 08:35:44.000000 zpenv-1.3.1/zpenv/zpenv.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:37:41.384000 zpenv-1.3.1/zpenv.egg-info/
+-rw-rw-rw-   0        0        0     5726 2023-06-13 08:37:40.000000 zpenv-1.3.1/zpenv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-13 08:37:41.000000 zpenv-1.3.1/zpenv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:37:40.000000 zpenv-1.3.1/zpenv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-13 08:37:41.000000 zpenv-1.3.1/zpenv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-13 08:37:41.000000 zpenv-1.3.1/zpenv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 08:37:41.000000 zpenv-1.3.1/zpenv.egg-info/top_level.txt
```

### Comparing `zpenv-1.3.0/LICENSE` & `zpenv-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zpenv-1.3.0/PKG-INFO` & `zpenv-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpenv
-Version: 1.3.0
+Version: 1.3.1
 Summary: Gestionnaire d'environnement virtuel
 Home-page: https://github.com/ZephyrOff/py-zpenv
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
 Keywords: venv virtualenv terminal zephyroff
 Platform: ALL
@@ -109,14 +109,19 @@
 [user@host ~]$ zpenv --removemodule [package]
 ```
 
 ### Mettre Ã  jour un package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
 ```
+
+### Installation de pip
+```console
+[user@host ~]$ zpenv --installpip
+```
 <br><br>
 
 # EN - Informations
 Cross-platform Python virtual environment management tool for creating, editing, deleting, or working with a virtual environment.<br>
 Everything happens directly in console.<br>
 It is possible to migrate these old virtual environments to this solution.
 ## Prerequisites
@@ -206,7 +211,12 @@
 ```
 
 ### Update a package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
 ```
 
+### Install pip
+```console
+[user@host ~]$ zpenv --installpip
+```
+
```

### Comparing `zpenv-1.3.0/README.md` & `zpenv-1.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -92,14 +92,19 @@
 [user@host ~]$ zpenv --removemodule [package]
 ```
 
 ### Mettre à jour un package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
 ```
+
+### Installation de pip
+```console
+[user@host ~]$ zpenv --installpip
+```
 <br><br>
 
 # EN - Informations
 Cross-platform Python virtual environment management tool for creating, editing, deleting, or working with a virtual environment.<br>
 Everything happens directly in console.<br>
 It is possible to migrate these old virtual environments to this solution.
 ## Prerequisites
@@ -187,8 +192,13 @@
 ```console
 [user@host ~]$ zpenv --removemodule [package]
 ```
 
 ### Update a package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
+```
+
+### Install pip
+```console
+[user@host ~]$ zpenv --installpip
 ```
```

### Comparing `zpenv-1.3.0/zpenv/zpenv.py` & `zpenv-1.3.1/zpenv/zpenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 			self.prompt = f'({self.env_name}) '
 		self.executable = sys.executable
 		self.python_dir = os.path.dirname(sys.executable)
 		self.python_exe = sys.executable.replace(self.python_dir,"").replace(path_rep[0],"")
 		self.inc_path = virtdir + path_rep[0] +'Include'
 		self.lib_path = virtdir + path_rep[0] +'Lib'
 		self.bin_path = virtdir + path_rep[0] +'Scripts'
-		self.bin_name = 'Scripts'
+		self.bin_name = 'bin'
+		if sys.platform == 'win32':
+			self.bin_name = 'Scripts'
 		self.env_exe = self.bin_path + path_rep[0] + self.python_exe
 		self.env_exec_cmd = self.env_exe
 		self.cfg_path = virtdir + path_rep[0] + 'pyvenv.cfg'
 
 #Affiche les logs
 def print_log(message):
 	if not argument.nolog:
```

### Comparing `zpenv-1.3.0/zpenv.egg-info/PKG-INFO` & `zpenv-1.3.1/zpenv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpenv
-Version: 1.3.0
+Version: 1.3.1
 Summary: Gestionnaire d'environnement virtuel
 Home-page: https://github.com/ZephyrOff/py-zpenv
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
 Keywords: venv virtualenv terminal zephyroff
 Platform: ALL
@@ -109,14 +109,19 @@
 [user@host ~]$ zpenv --removemodule [package]
 ```
 
 ### Mettre Ã  jour un package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
 ```
+
+### Installation de pip
+```console
+[user@host ~]$ zpenv --installpip
+```
 <br><br>
 
 # EN - Informations
 Cross-platform Python virtual environment management tool for creating, editing, deleting, or working with a virtual environment.<br>
 Everything happens directly in console.<br>
 It is possible to migrate these old virtual environments to this solution.
 ## Prerequisites
@@ -206,7 +211,12 @@
 ```
 
 ### Update a package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
 ```
 
+### Install pip
+```console
+[user@host ~]$ zpenv --installpip
+```
+
```

