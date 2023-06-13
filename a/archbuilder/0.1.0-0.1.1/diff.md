# Comparing `tmp/archbuilder-0.1.0.tar.gz` & `tmp/archbuilder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archbuilder-0.1.0.tar", last modified: Mon Jun 12 17:30:22 2023, max compression
+gzip compressed data, was "archbuilder-0.1.1.tar", last modified: Tue Jun 13 17:18:09 2023, max compression
```

## Comparing `archbuilder-0.1.0.tar` & `archbuilder-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 17:30:22.558817 archbuilder-0.1.0/
--rw-rw-rw-   0        0        0       29 2023-05-31 23:56:47.000000 archbuilder-0.1.0/.coveragerc
--rw-rw-rw-   0        0        0       80 2023-06-12 15:29:27.000000 archbuilder-0.1.0/.flake8
--rw-rw-rw-   0        0        0      295 2023-06-10 13:44:10.000000 archbuilder-0.1.0/.gitignore
--rw-rw-rw-   0        0        0        8 2023-06-10 13:45:01.000000 archbuilder-0.1.0/.python-version
--rw-rw-rw-   0        0        0     1478 2023-06-12 17:30:22.556815 archbuilder-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-12 15:11:16.000000 archbuilder-0.1.0/Pipfile
--rw-rw-rw-   0        0        0    18228 2023-06-12 15:10:51.000000 archbuilder-0.1.0/Pipfile.lock
--rw-rw-rw-   0        0        0     1182 2023-06-10 15:28:30.000000 archbuilder-0.1.0/README.md
--rw-rw-rw-   0        0        0      487 2023-06-12 17:27:01.000000 archbuilder-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      154 2023-05-31 23:59:03.000000 archbuilder-0.1.0/pytest.ini
--rw-rw-rw-   0        0        0       42 2023-06-12 17:30:22.559818 archbuilder-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 17:30:22.270767 archbuilder-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 17:30:22.472814 archbuilder-0.1.0/src/archbuilder/
--rw-rw-rw-   0        0        0      676 2023-06-12 17:22:59.000000 archbuilder-0.1.0/src/archbuilder/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:30:22.507814 archbuilder-0.1.0/src/archbuilder.egg-info/
--rw-rw-rw-   0        0        0     1478 2023-06-12 17:30:21.000000 archbuilder-0.1.0/src/archbuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-06-12 17:30:22.000000 archbuilder-0.1.0/src/archbuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 17:30:21.000000 archbuilder-0.1.0/src/archbuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-12 17:30:21.000000 archbuilder-0.1.0/src/archbuilder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-12 17:30:21.000000 archbuilder-0.1.0/src/archbuilder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 17:30:22.514815 archbuilder-0.1.0/src/builder/
--rw-rw-rw-   0        0        0       30 2023-06-12 16:35:52.000000 archbuilder-0.1.0/src/builder/__init__.py
--rw-rw-rw-   0        0        0      755 2023-06-10 12:50:12.000000 archbuilder-0.1.0/src/builder/builder.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:30:22.522818 archbuilder-0.1.0/src/template/
--rw-rw-rw-   0        0        0       32 2023-06-12 16:42:50.000000 archbuilder-0.1.0/src/template/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-06-10 12:46:22.000000 archbuilder-0.1.0/src/template/template.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:30:22.274767 archbuilder-0.1.0/tests/
-drwxrwxrwx   0        0        0        0 2023-06-12 17:30:22.553815 archbuilder-0.1.0/tests/unit/
--rw-rw-rw-   0        0        0      390 2023-06-12 15:12:19.000000 archbuilder-0.1.0/tests/unit/test_builder.py
--rw-rw-rw-   0        0        0      607 2023-06-10 15:26:53.000000 archbuilder-0.1.0/tests/unit/test_template.py
--rw-rw-rw-   0        0        0      782 2023-06-10 17:45:09.000000 archbuilder-0.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.535076 archbuilder-0.1.1/
+-rw-rw-rw-   0        0        0       29 2023-05-31 23:56:47.000000 archbuilder-0.1.1/.coveragerc
+-rw-rw-rw-   0        0        0       80 2023-06-12 15:29:27.000000 archbuilder-0.1.1/.flake8
+-rw-rw-rw-   0        0        0      295 2023-06-10 13:44:10.000000 archbuilder-0.1.1/.gitignore
+-rw-rw-rw-   0        0        0        8 2023-06-10 13:45:01.000000 archbuilder-0.1.1/.python-version
+-rw-rw-rw-   0        0        0     1497 2023-06-13 17:18:09.533078 archbuilder-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-12 17:46:00.000000 archbuilder-0.1.1/Pipfile
+-rw-rw-rw-   0        0        0    33014 2023-06-12 17:47:23.000000 archbuilder-0.1.1/Pipfile.lock
+-rw-rw-rw-   0        0        0     1195 2023-06-13 17:12:25.000000 archbuilder-0.1.1/README.md
+-rw-rw-rw-   0        0        0      493 2023-06-13 17:17:09.000000 archbuilder-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      154 2023-05-31 23:59:03.000000 archbuilder-0.1.1/pytest.ini
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:18:09.535076 archbuilder-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.415073 archbuilder-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.479076 archbuilder-0.1.1/src/archbuilder/
+-rw-rw-rw-   0        0        0      700 2023-06-13 17:06:49.000000 archbuilder-0.1.1/src/archbuilder/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.497083 archbuilder-0.1.1/src/archbuilder.egg-info/
+-rw-rw-rw-   0        0        0     1497 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.506081 archbuilder-0.1.1/src/builder/
+-rw-rw-rw-   0        0        0       30 2023-06-12 16:35:52.000000 archbuilder-0.1.1/src/builder/__init__.py
+-rw-rw-rw-   0        0        0      736 2023-06-13 17:16:18.000000 archbuilder-0.1.1/src/builder/builder.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.518077 archbuilder-0.1.1/src/template/
+-rw-rw-rw-   0        0        0       32 2023-06-12 16:42:50.000000 archbuilder-0.1.1/src/template/__init__.py
+-rw-rw-rw-   0        0        0     1270 2023-06-10 12:46:22.000000 archbuilder-0.1.1/src/template/template.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.419080 archbuilder-0.1.1/tests/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.528077 archbuilder-0.1.1/tests/unit/
+-rw-rw-rw-   0        0        0      390 2023-06-12 15:12:19.000000 archbuilder-0.1.1/tests/unit/test_builder.py
+-rw-rw-rw-   0        0        0      608 2023-06-13 17:16:18.000000 archbuilder-0.1.1/tests/unit/test_template.py
+-rw-rw-rw-   0        0        0      782 2023-06-10 17:45:09.000000 archbuilder-0.1.1/tox.ini
```

### Comparing `archbuilder-0.1.0/PKG-INFO` & `archbuilder-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: archbuilder
-Version: 0.1.0
-Summary: A tool to enable developers set up projects quickly
+Version: 0.1.1
+Summary: A tool to enable developers set up their projects quickly
 Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # Archbuilder
@@ -19,30 +19,32 @@
   pip install archbuilder
 ```
     
 ## Usage
 
 ##### 1. By using a python script
 ```python
-# Import the following classes
-from builder import Builder, Template
+# Import archbuilder
+from builder import Builder
+from template import Template
 
 # Create a template from a json file
 template = Template('sass.json')
 
 # Create the project tree from the template
 project = Builder('sass', template)
 project.build()
 ```
 
 ##### 2. By using the command-line
 Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
 ```bash
 archbuilder sass sass.json
 ```
+
 ## Contributing
 
 Contributions are always welcome!
 
 For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `archbuilder-0.1.0/README.md` & `archbuilder-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,30 +10,32 @@
   pip install archbuilder
 ```
     
 ## Usage
 
 ##### 1. By using a python script
 ```python
-# Import the following classes
-from builder import Builder, Template
+# Import archbuilder
+from builder import Builder
+from template import Template
 
 # Create a template from a json file
 template = Template('sass.json')
 
 # Create the project tree from the template
 project = Builder('sass', template)
 project.build()
 ```
 
 ##### 2. By using the command-line
 Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
 ```bash
 archbuilder sass sass.json
 ```
+
 ## Contributing
 
 Contributions are always welcome!
 
 For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `archbuilder-0.1.0/src/archbuilder/__main__.py` & `archbuilder-0.1.1/src/archbuilder/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+from pathlib import Path
 
 from builder import Builder
 from template import Template
 
 
 def get_args():
     parser = argparse.ArgumentParser(
@@ -17,13 +18,12 @@
 
 
 def main():
     args = get_args()
 
     template = Template(args.template)
     project = Builder(args.project, template, args.output)
-
     project.build()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `archbuilder-0.1.0/src/archbuilder.egg-info/PKG-INFO` & `archbuilder-0.1.1/src/archbuilder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: archbuilder
-Version: 0.1.0
-Summary: A tool to enable developers set up projects quickly
+Version: 0.1.1
+Summary: A tool to enable developers set up their projects quickly
 Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # Archbuilder
@@ -19,30 +19,32 @@
   pip install archbuilder
 ```
     
 ## Usage
 
 ##### 1. By using a python script
 ```python
-# Import the following classes
-from builder import Builder, Template
+# Import archbuilder
+from builder import Builder
+from template import Template
 
 # Create a template from a json file
 template = Template('sass.json')
 
 # Create the project tree from the template
 project = Builder('sass', template)
 project.build()
 ```
 
 ##### 2. By using the command-line
 Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
 ```bash
 archbuilder sass sass.json
 ```
+
 ## Contributing
 
 Contributions are always welcome!
 
 For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `archbuilder-0.1.0/src/builder/builder.py` & `archbuilder-0.1.1/src/builder/builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
 """
-
 from pathlib import Path
 
 
 class Builder:
     """"""
 
-    root = Path(__file__).resolve().parent.parent.parent
-
-    def __init__(self, project, template, output="build"):
+    def __init__(self, project, template, output="build", root=Path.cwd()):
         """"""
         self.project = project
-        self.output = output
         self.template = template
+        self.output = output
+        self.root = root
 
     def build(self):
         """"""
         for path in self.paths():
             if not path.exists():
                 path.parent.mkdir(parents=True, exist_ok=True)
                 path.touch(exist_ok=True)
```

### Comparing `archbuilder-0.1.0/src/template/template.py` & `archbuilder-0.1.1/src/template/template.py`

 * *Files identical despite different names*

### Comparing `archbuilder-0.1.0/tests/unit/test_template.py` & `archbuilder-0.1.1/tests/unit/test_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 """
 
 import pytest
 
-from builder import Template
+from template import Template
 
 
 def test_template_initialization():
     """"""
     template = Template("sass.json")
     assert template.name == "sass.json"
```

### Comparing `archbuilder-0.1.0/tox.ini` & `archbuilder-0.1.1/tox.ini`

 * *Files identical despite different names*

