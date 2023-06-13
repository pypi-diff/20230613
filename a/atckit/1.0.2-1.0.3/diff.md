# Comparing `tmp/atckit-1.0.2.tar.gz` & `tmp/atckit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atckit-1.0.2.tar", last modified: Sat Jun 10 20:54:22 2023, max compression
+gzip compressed data, was "atckit-1.0.3.tar", last modified: Tue Jun 13 08:24:09 2023, max compression
```

## Comparing `atckit-1.0.2.tar` & `atckit-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:54:22.764107 atckit-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-03 09:08:12.000000 atckit-1.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-10 20:52:22.000000 atckit-1.0.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 09:08:12.000000 atckit-1.0.2/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-03 09:08:12.000000 atckit-1.0.2/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)   115208 2023-06-10 20:36:02.000000 atckit-1.0.2/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-03 09:08:12.000000 atckit-1.0.2/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-03 09:08:12.000000 atckit-1.0.2/Makefile
--rw-r--r--   0 root         (0) root         (0)     2873 2023-06-10 20:54:22.764107 atckit-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-10 20:36:02.000000 atckit-1.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-03 09:08:12.000000 atckit-1.0.2/build_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-03 09:08:12.000000 atckit-1.0.2/git-tags.sh
--rwxrwxrwx   0 root         (0) root         (0)    23443 2023-06-03 09:08:12.000000 atckit-1.0.2/icon.png
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-10 20:54:16.000000 atckit-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 20:54:22.764107 atckit-1.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:54:22.760107 atckit-1.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:54:22.764107 atckit-1.0.2/src/atckit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-10 20:53:34.000000 atckit-1.0.2/src/atckit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-06-10 20:40:43.000000 atckit-1.0.2/src/atckit/subscriber.py
--rw-rw-rw-   0 root         (0) root         (0)     4804 2023-06-03 09:44:24.000000 atckit-1.0.2/src/atckit/utilfuncs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:54:22.764107 atckit-1.0.2/src/atckit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2873 2023-06-10 20:54:22.000000 atckit-1.0.2/src/atckit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-10 20:54:22.000000 atckit-1.0.2/src/atckit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 20:54:22.000000 atckit-1.0.2/src/atckit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 20:54:22.000000 atckit-1.0.2/src/atckit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:24:09.478747 atckit-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-03 09:08:12.000000 atckit-1.0.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-10 20:52:22.000000 atckit-1.0.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 09:08:12.000000 atckit-1.0.3/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-03 09:08:12.000000 atckit-1.0.3/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)   115208 2023-06-13 08:14:33.000000 atckit-1.0.3/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-03 09:08:12.000000 atckit-1.0.3/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-03 09:08:12.000000 atckit-1.0.3/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-06-13 08:24:09.478747 atckit-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-10 20:36:02.000000 atckit-1.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-03 09:08:12.000000 atckit-1.0.3/build_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-03 09:08:12.000000 atckit-1.0.3/git-tags.sh
+-rwxrwxrwx   0 root         (0) root         (0)    23443 2023-06-03 09:08:12.000000 atckit-1.0.3/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-13 08:23:59.000000 atckit-1.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 08:24:09.478747 atckit-1.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:24:09.470747 atckit-1.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:24:09.474747 atckit-1.0.3/src/atckit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 08:22:32.000000 atckit-1.0.3/src/atckit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-06-10 20:40:43.000000 atckit-1.0.3/src/atckit/subscriber.py
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2023-06-13 08:14:33.000000 atckit-1.0.3/src/atckit/utilfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:24:09.478747 atckit-1.0.3/src/atckit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-06-13 08:24:09.000000 atckit-1.0.3/src/atckit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-13 08:24:09.000000 atckit-1.0.3/src/atckit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:24:09.000000 atckit-1.0.3/src/atckit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-13 08:24:09.000000 atckit-1.0.3/src/atckit.egg-info/top_level.txt
```

### Comparing `atckit-1.0.2/.gitlab-ci.yml` & `atckit-1.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `atckit-1.0.2/.pylintrc` & `atckit-1.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `atckit-1.0.2/Doxyfile` & `atckit-1.0.3/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "AccidentallyTheCable's Utility Kit"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.0.2"
+PROJECT_NUMBER = "1.0.3"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `atckit-1.0.2/LICENSE.md` & `atckit-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `atckit-1.0.2/Makefile` & `atckit-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `atckit-1.0.2/PKG-INFO` & `atckit-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atckit
-Version: 1.0.2
+Version: 1.0.3
 Summary: AccidentallyTheCable's Utility Kit
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atckit-1.0.2/README.md` & `atckit-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `atckit-1.0.2/git-tags.sh` & `atckit-1.0.3/git-tags.sh`

 * *Files identical despite different names*

### Comparing `atckit-1.0.2/icon.png` & `atckit-1.0.3/icon.png`

 * *Files identical despite different names*

### Comparing `atckit-1.0.2/pyproject.toml` & `atckit-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atckit"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "AccidentallyTheCable's Utility Kit"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `atckit-1.0.2/src/atckit/subscriber.py` & `atckit-1.0.3/src/atckit/subscriber.py`

 * *Files identical despite different names*

### Comparing `atckit-1.0.2/src/atckit/utilfuncs.py` & `atckit-1.0.3/src/atckit/utilfuncs.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     """Utility Functions
     """
 
     shutdown:bool = False
     restart:bool = False
 
     @staticmethod
-    def scan_dir(target_path:Path,callback:typing.Callable[[Path,dict[str,str]],None],callback_data:dict[str,str],exclude_dirs:list[re.Pattern],exclude_files:list[re.Pattern]) -> None:
+    def scan_dir(target_path:Path,callback:typing.Callable[[Path,dict[str,typing.Any]],None],callback_data:dict[str,typing.Any],exclude_dirs:list[re.Pattern],exclude_files:list[re.Pattern]) -> None:
         """Scan A Directory, and Execute callback on discovered files, that do not match the exclusions
         @param Path \c target_path Path to Scan for Files
-        @param typing.Callable[[Path,dict[str,str]],None] \c callback Callback function to execute on each file
-        @param dict[str,str] \c callback_data Data to pass to the callback function
+        @param typing.Callable[[Path,dict[str,Any]],None] \c callback Callback function to execute on each file
+        @param dict[str,Any] \c callback_data Data to pass to the callback function
         @param list[re.Pattern] \c exclude_dirs Regex Compiled list of directory patterns to exclude
         @param list[re.Pattern] \c exclude_files Regex Compiled list of file patterns to exclude
         """
         files:typing.Generator[Path, None, None] = target_path.glob("*")
         skip:bool = False
         for file in files:
             file_path:Path = Path(file)
```

### Comparing `atckit-1.0.2/src/atckit.egg-info/PKG-INFO` & `atckit-1.0.3/src/atckit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atckit
-Version: 1.0.2
+Version: 1.0.3
 Summary: AccidentallyTheCable's Utility Kit
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

