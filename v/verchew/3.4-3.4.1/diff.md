# Comparing `tmp/verchew-3.4.tar.gz` & `tmp/verchew-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verchew-3.4.tar", max compression
+gzip compressed data, was "verchew-3.4.1.tar", max compression
```

## Comparing `verchew-3.4.tar` & `verchew-3.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1088 2020-10-23 17:28:02.191465 verchew-3.4/LICENSE.md
--rw-r--r--   0        0        0     3064 2023-06-03 20:17:02.276081 verchew-3.4/README.md
--rw-r--r--   0        0        0     2038 2023-06-03 20:21:25.127676 verchew-3.4/pyproject.toml
--rw-r--r--   0        0        0       60 2020-10-23 17:28:02.195541 verchew-3.4/verchew/__init__.py
--rw-r--r--   0        0        0      124 2020-10-23 17:28:02.195675 verchew-3.4/verchew/__main__.py
--rwxr-xr-x   0        0        0    10571 2023-06-03 21:34:08.124188 verchew-3.4/verchew/script.py
--rw-r--r--   0        0        0       34 2020-10-23 17:28:02.195975 verchew-3.4/verchew/tests/__init__.py
--rw-r--r--   0        0        0      291 2020-10-23 17:28:02.196080 verchew-3.4/verchew/tests/conftest.py
--rw-r--r--   0        0        0     6288 2023-06-03 21:34:26.121376 verchew-3.4/verchew/tests/test_script.py
--rwxr-xr-x   0        0        0      393 2022-09-12 19:07:47.825706 verchew-3.4/verchew/wrapper.sh
--rw-r--r--   0        0        0     4796 1970-01-01 00:00:00.000000 verchew-3.4/PKG-INFO
+-rw-r--r--   0        0        0     1088 2018-03-29 20:56:27.000000 verchew-3.4.1/LICENSE.md
+-rw-r--r--   0        0        0     3064 2023-06-04 14:09:25.836432 verchew-3.4.1/README.md
+-rw-r--r--   0        0        0     2040 2023-06-13 20:38:44.486129 verchew-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0       60 2016-10-17 21:38:01.000000 verchew-3.4.1/verchew/__init__.py
+-rw-r--r--   0        0        0      124 2020-11-25 23:10:46.000000 verchew-3.4.1/verchew/__main__.py
+-rwxr-xr-x   0        0        0    10586 2023-06-13 20:41:46.541358 verchew-3.4.1/verchew/script.py
+-rw-r--r--   0        0        0       34 2016-10-12 14:39:17.000000 verchew-3.4.1/verchew/tests/__init__.py
+-rw-r--r--   0        0        0      291 2020-11-25 23:10:52.000000 verchew-3.4.1/verchew/tests/conftest.py
+-rw-r--r--   0        0        0     6381 2023-06-13 20:41:24.264232 verchew-3.4.1/verchew/tests/test_script.py
+-rwxr-xr-x   0        0        0      393 2022-07-22 17:49:18.423787 verchew-3.4.1/verchew/wrapper.sh
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 verchew-3.4.1/PKG-INFO
```

### Comparing `verchew-3.4/LICENSE.md` & `verchew-3.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `verchew-3.4/README.md` & `verchew-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `verchew-3.4/pyproject.toml` & `verchew-3.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "verchew"
-version = "3.4"  # also update verchew/script.py
+version = "3.4.1"  # also update verchew/script.py
 description = "System dependency version checker."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `verchew-3.4/verchew/script.py` & `verchew-3.4.1/verchew/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 if PY2:
     import ConfigParser as configparser
     from urllib import urlretrieve
 else:
     import configparser
     from urllib.request import urlretrieve
 
-__version__ = '3.4'
+__version__ = '3.4.1'
 
 SCRIPT_URL = (
     "https://raw.githubusercontent.com/jacebrowning/verchew/main/verchew/script.py"
 )
 WRAPPER_URL = (
     "https://raw.githubusercontent.com/jacebrowning/verchew/main/verchew/wrapper.sh"
 )
@@ -307,15 +307,15 @@
         show("<nothing>")
 
     return output
 
 
 def match_version(pattern, output):
     lines = output.splitlines()
-    if "not found" in lines[0]:
+    if not lines or "not found" in lines[0]:
         return False
 
     regex = pattern.replace('.', r'\.') + r'(\b|/)'
 
     for line in lines:
         log.debug("Matching %s: %s", regex, line)
         match = re.match(regex, line)
```

### Comparing `verchew-3.4/verchew/tests/test_script.py` & `verchew-3.4.1/verchew/tests/test_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,17 @@
     def when_mismatch_with_missing_program():
         expect(match_version("", "program not found")) == False
         expect(match_version("", "v1.2.3\nother not found")) == True
 
     def when_match_with_multiple_lines():
         expect(match_version("1.2", "Foobar\nVersion 1.2.3")) == True
 
+    def when_mismatch_with_no_output():
+        expect(match_version("1.2.3", "")) == False
+
 
 def describe_format():
     def default():
         expect(_('~')) == "~"
 
     @pytest.mark.parametrize(
         "is_tty,supports_utf8,supports_ansi,formatted",
```

### Comparing `verchew-3.4/PKG-INFO` & `verchew-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verchew
-Version: 3.4
+Version: 3.4.1
 Summary: System dependency version checker.
 Home-page: https://pypi.org/project/verchew
 License: MIT
 Keywords: dependencies,configuration management,continuous integration
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.6,<4.0
```

