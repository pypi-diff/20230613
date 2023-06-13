# Comparing `tmp/sshsurf.py-0.0.1a0.tar.gz` & `tmp/sshsurf.py-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshsurf.py-0.0.1a0.tar", last modified: Tue Jun 13 21:13:37 2023, max compression
+gzip compressed data, was "sshsurf.py-0.0.1b0.tar", last modified: Tue Jun 13 21:30:47 2023, max compression
```

## Comparing `sshsurf.py-0.0.1a0.tar` & `sshsurf.py-0.0.1b0.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:13:37.555846 sshsurf.py-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 21:13:25.000000 sshsurf.py-0.0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 21:13:37.555846 sshsurf.py-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-13 21:13:25.000000 sshsurf.py-0.0.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:13:37.555846 sshsurf.py-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-13 21:13:25.000000 sshsurf.py-0.0.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:13:37.555846 sshsurf.py-0.0.1a0/sshsurf.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 21:13:37.000000 sshsurf.py-0.0.1a0/sshsurf.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 21:13:37.000000 sshsurf.py-0.0.1a0/sshsurf.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:13:37.000000 sshsurf.py-0.0.1a0/sshsurf.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 21:13:37.000000 sshsurf.py-0.0.1a0/sshsurf.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:13:37.000000 sshsurf.py-0.0.1a0/sshsurf.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:30:47.157614 sshsurf.py-0.0.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 21:30:36.000000 sshsurf.py-0.0.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 21:30:47.157614 sshsurf.py-0.0.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-13 21:30:36.000000 sshsurf.py-0.0.1b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:30:47.157614 sshsurf.py-0.0.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-13 21:30:36.000000 sshsurf.py-0.0.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:30:47.153613 sshsurf.py-0.0.1b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:30:47.153613 sshsurf.py-0.0.1b0/src/sshsurf/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 21:30:36.000000 sshsurf.py-0.0.1b0/src/sshsurf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-13 21:30:36.000000 sshsurf.py-0.0.1b0/src/sshsurf/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:30:47.157614 sshsurf.py-0.0.1b0/src/sshsurf.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 21:30:47.000000 sshsurf.py-0.0.1b0/src/sshsurf.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 21:30:47.000000 sshsurf.py-0.0.1b0/src/sshsurf.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:30:47.000000 sshsurf.py-0.0.1b0/src/sshsurf.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 21:30:47.000000 sshsurf.py-0.0.1b0/src/sshsurf.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 21:30:47.000000 sshsurf.py-0.0.1b0/src/sshsurf.py.egg-info/top_level.txt
```

### Comparing `sshsurf.py-0.0.1a0/LICENSE` & `sshsurf.py-0.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `sshsurf.py-0.0.1a0/PKG-INFO` & `sshsurf.py-0.0.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshsurf.py
-Version: 0.0.1a0
+Version: 0.0.1b0
 Summary: A wrapper for ssh.surf API
 Home-page: https://github.com/OrdinaryEnder/sshsurf.py
 Author: OrdinaryEnder
 Author-email: endergaming1458@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `sshsurf.py-0.0.1a0/setup.py` & `sshsurf.py-0.0.1b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 # requirements = ["requests<=2.21.0"]
 
 # Function that takes several arguments. It assigns these values to our package.
 setuptools.setup(
 	# Distribution name the package. Name must be unique so adding your username at the end is common.
 	name="sshsurf.py",
 	# Version number of your package. Semantic versioning is commonly used.
-	version="0.0.1a",
+	version="0.0.1b",
 	# Author name.
 	author="OrdinaryEnder",
 	# Author's email address.
 	author_email="endergaming1458@gmail.com",
 	# Short description that will show on the PyPi page.
 	description="A wrapper for ssh.surf API",
 	# Long description that will display on the PyPi page. Uses the repo's README.md to populate this.
 	long_description=long_description,
 	# Defines the content type that the long_description is using.
 	long_description_content_type="text/markdown",
 	# The URL that represents the homepage of the project. Most projects link to the repo.
 	url="https://github.com/OrdinaryEnder/sshsurf.py",
 	# Finds all packages within in the project and combines them into the distribution together.
-	packages=setuptools.find_packages(),
+        package_dir={'': 'src'},
+	packages=setuptools.find_packages(where='src'),
 	# requirements or dependencies that will be installed alongside your package when the user installs it via pip.
 	install_requires=['aiohttp'],
 	# Gives pip some metadata about the package. Also displays on the PyPi page.
 	classifiers=[
 		"Programming Language :: Python :: 3.8",
 		"License :: OSI Approved :: Apache Software License",
 		"Operating System :: OS Independent",
```

### Comparing `sshsurf.py-0.0.1a0/sshsurf.py.egg-info/PKG-INFO` & `sshsurf.py-0.0.1b0/src/sshsurf.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshsurf.py
-Version: 0.0.1a0
+Version: 0.0.1b0
 Summary: A wrapper for ssh.surf API
 Home-page: https://github.com/OrdinaryEnder/sshsurf.py
 Author: OrdinaryEnder
 Author-email: endergaming1458@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

