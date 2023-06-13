# Comparing `tmp/pypi_python_translator-2.5.0rc1.tar.gz` & `tmp/pypi_python_translator-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_python_translator-2.5.0rc1.tar", last modified: Mon Jun 12 18:19:32 2023, max compression
+gzip compressed data, was "pypi_python_translator-2.5.1.tar", last modified: Mon Jun 12 18:31:21 2023, max compression
```

## Comparing `pypi_python_translator-2.5.0rc1.tar` & `pypi_python_translator-2.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:19:32.524263 pypi_python_translator-2.5.0rc1/
--rw-rw-rw-   0        0        0     5417 2023-06-12 18:19:32.524263 pypi_python_translator-2.5.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0     4971 2023-06-12 18:04:29.000000 pypi_python_translator-2.5.0rc1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 18:19:32.508091 pypi_python_translator-2.5.0rc1/pypi_python_translator.egg-info/
--rw-rw-rw-   0        0        0     5417 2023-06-12 18:19:32.000000 pypi_python_translator-2.5.0rc1/pypi_python_translator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-06-12 18:19:32.000000 pypi_python_translator-2.5.0rc1/pypi_python_translator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:19:32.000000 pypi_python_translator-2.5.0rc1/pypi_python_translator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 18:19:32.000000 pypi_python_translator-2.5.0rc1/pypi_python_translator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 18:19:32.525258 pypi_python_translator-2.5.0rc1/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-06-12 18:19:14.000000 pypi_python_translator-2.5.0rc1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:19:32.522259 pypi_python_translator-2.5.0rc1/translator/
--rw-rw-rw-   0        0        0      700 2023-06-12 18:06:45.000000 pypi_python_translator-2.5.0rc1/translator/ExampleUsages.py
--rw-rw-rw-   0        0        0     4945 2023-06-12 18:19:23.000000 pypi_python_translator-2.5.0rc1/translator/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.5.0rc1/translator/languageExamples.py
--rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.5.0rc1/translator/messages.py
--rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.5.0rc1/translator/services.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:31:21.099105 pypi_python_translator-2.5.1/
+-rw-rw-rw-   0        0        0     5414 2023-06-12 18:31:21.098110 pypi_python_translator-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4971 2023-06-12 18:04:29.000000 pypi_python_translator-2.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:31:21.075864 pypi_python_translator-2.5.1/pypi_python_translator.egg-info/
+-rw-rw-rw-   0        0        0     5414 2023-06-12 18:31:20.000000 pypi_python_translator-2.5.1/pypi_python_translator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-12 18:31:21.000000 pypi_python_translator-2.5.1/pypi_python_translator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:31:20.000000 pypi_python_translator-2.5.1/pypi_python_translator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 18:31:20.000000 pypi_python_translator-2.5.1/pypi_python_translator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 18:31:21.100111 pypi_python_translator-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-06-12 18:31:11.000000 pypi_python_translator-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:31:21.095973 pypi_python_translator-2.5.1/translator/
+-rw-rw-rw-   0        0        0      700 2023-06-12 18:06:45.000000 pypi_python_translator-2.5.1/translator/ExampleUsages.py
+-rw-rw-rw-   0        0        0     4941 2023-06-12 18:31:07.000000 pypi_python_translator-2.5.1/translator/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.5.1/translator/languageExamples.py
+-rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.5.1/translator/messages.py
+-rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.5.1/translator/services.py
```

### Comparing `pypi_python_translator-2.5.0rc1/PKG-INFO` & `pypi_python_translator-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi_python_translator
-Version: 2.5.0rc1
+Version: 2.5.1
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypi_python_translator-2.5.0rc1/README.md` & `pypi_python_translator-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.5.0rc1/pypi_python_translator.egg-info/PKG-INFO` & `pypi_python_translator-2.5.1/pypi_python_translator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-python-translator
-Version: 2.5.0rc1
+Version: 2.5.1
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypi_python_translator-2.5.0rc1/setup.py` & `pypi_python_translator-2.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypi_python_translator",
-    version="2.5.0-rc1",
+    version="2.5.1",
     author="SForces",
     author_email="osmntn08@gmail.com",
     description="A Python package for translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/pypi_python_translator",
     packages=["translator"],
```

### Comparing `pypi_python_translator-2.5.0rc1/translator/ExampleUsages.py` & `pypi_python_translator-2.5.1/translator/ExampleUsages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.5.0rc1/translator/__init__.py` & `pypi_python_translator-2.5.1/translator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     print("https://github.com/SForces/PyPi_Python_Translator/blob/main/README.md")
 def version():
     """
     VERSION
     ~~~
     Returns package version.
     """
-    return "Current Package Version: 2.5.0-rc1"
+    return "Current Package Version: 2.5.1"
 def init(langg:str) -> any:
     """
     TRANSLATOR MAIN FUNCTION
     ~~~
     This is the function you will use to start this translation application.
     
     The interface translates itself, and then prompts the user for the desired exit language.
```

### Comparing `pypi_python_translator-2.5.0rc1/translator/messages.py` & `pypi_python_translator-2.5.1/translator/messages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.5.0rc1/translator/services.py` & `pypi_python_translator-2.5.1/translator/services.py`

 * *Files identical despite different names*

