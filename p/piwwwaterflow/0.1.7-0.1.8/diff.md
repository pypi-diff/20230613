# Comparing `tmp/piwwwaterflow-0.1.7.tar.gz` & `tmp/piwwwaterflow-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.1.7.tar", last modified: Thu Jun  1 12:06:22 2023, max compression
+gzip compressed data, was "piwwwaterflow-0.1.8.tar", last modified: Tue Jun 13 06:54:37 2023, max compression
```

## Comparing `piwwwaterflow-0.1.7.tar` & `piwwwaterflow-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.845886 piwwwaterflow-0.1.7/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.845886 piwwwaterflow-0.1.7/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/piwwwaterflow/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/css/iepngfix.htc
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/piwwwaterflow/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/blank.gif
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/piwaterflow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/play.png
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/shadow.gif
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/img/top.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/piwwwaterflow/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/static/js/code.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.845886 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 12:06:22.000000 piwwwaterflow-0.1.7/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:22.849887 piwwwaterflow-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:06:09.000000 piwwwaterflow-0.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.769601 piwwwaterflow-0.1.8/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.769601 piwwwaterflow-0.1.8/piwwwaterflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.769601 piwwwaterflow-0.1.8/piwwwaterflow/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/css/iepngfix.htc
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/piwwwaterflow/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/blank.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/piwaterflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/shadow.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/top.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/piwwwaterflow/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/js/code.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/piwwwaterflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.769601 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/tests/__init__.py
```

### Comparing `piwwwaterflow-0.1.7/PKG-INFO` & `piwwwaterflow-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.7
+Version: 0.1.8
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/static/css/iepngfix.htc` & `piwwwaterflow-0.1.8/piwwwaterflow/static/css/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/static/css/view.css` & `piwwwaterflow-0.1.8/piwwwaterflow/static/css/view.css`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/static/img/icon-256.png` & `piwwwaterflow-0.1.8/piwwwaterflow/static/img/icon-256.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/static/img/icon-32.png` & `piwwwaterflow-0.1.8/piwwwaterflow/static/img/icon-32.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/static/img/piwaterflow.svg` & `piwwwaterflow-0.1.8/piwwwaterflow/static/img/piwaterflow.svg`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/static/img/play.png` & `piwwwaterflow-0.1.8/piwwwaterflow/static/img/play.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/static/js/code.js` & `piwwwaterflow-0.1.8/piwwwaterflow/static/js/code.js`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/templates/form.html` & `piwwwaterflow-0.1.8/piwwwaterflow/templates/form.html`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/webservice.py` & `piwwwaterflow-0.1.8/piwwwaterflow/webservice.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,42 +3,53 @@
 
 from flask import Flask, render_template, request
 from flask_compress import Compress
 from flask_socketio import SocketIO
 from importlib_metadata import version, PackageNotFoundError
 
 from piwaterflow import Waterflow
+from log_mgr import Logger, LoggerMode
 from revproxy_auth import RevProxyAuth
 
 
 class PiWWWaterflowService:
     """Class for the web service... its an interface to the real functionality in piwaterflow package.
     """
     def __init__(self,  template_folder, static_folder):
+
+        self.logger = Logger(self.class_name(), log_file_name='piwwwaterflow', mode=LoggerMode.BOTH, dry_run=False)
+        self.logger.info("Launching piwwwaterflow...")
         self.waterflow = Waterflow()
 
         self.app = Flask(__name__,  template_folder=template_folder, static_folder=static_folder)
+
         self.revproxy_auth = RevProxyAuth(self.app, root_class='piwwwaterflow')
 
         self.app.add_url_rule('/', 'index', self.waterflow_endpoint, methods=['GET', 'POST'])
         Compress(self.app)
         self.socketio = SocketIO(self.app, cors_allowed_origins='*')
         self.socketio.on_event('service_request', self.on_service_request)
         self.socketio.on_event('force', self.on_force)
         self.socketio.on_event('stop', self.on_stop)
         self.socketio.on_event('save', self.on_save)
 
+    @classmethod
+    def class_name(cls):
+        """ class name """
+        return "piwwwaterflow"
+
     def get_app(self):
         """ Returns WSGI app
         Returns:
             WSGI app:
         """
         return self.app
 
     def run(self):
+        """ Run function """
         # self.app.run()
         self.socketio.run(self.app)
 
     def waterflow_endpoint(self):
         """ Main endpoint that returns the main page for piwaterflow
         Returns:
             response: The main html content
@@ -48,15 +59,15 @@
     def on_service_request(self) -> dict:
         """ Gets all the information from the waterflow service
         Args:
             data (dict):'first_time': This value is only bypassed to the caller
         Returns:
             dict:Dictionary with all the information about the status of the waterflow system
         """
-        print('Service requested...')
+        self.logger.info('Service requested...')
         try:
             ver = version('piwaterflow')
         except PackageNotFoundError:
             ver = '?.?.?'
 
         responsedict = {'log': self.waterflow.get_log(),
                         'forced': self.waterflow.get_forced_info(),
```

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow/wsgi.py` & `piwwwaterflow-0.1.8/piwwwaterflow/wsgi.py`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.1.8/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.7
+Version: 0.1.8
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.7/piwwwaterflow.egg-info/SOURCES.txt` & `piwwwaterflow-0.1.8/piwwwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.7/setup.py` & `piwwwaterflow-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwwwaterflow",
-    version="0.1.7",
+    version="0.1.8",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwwwaterflow",
     packages=setuptools.find_packages(),
@@ -23,13 +23,13 @@
     ],
     install_requires=[
         'Flask>=1.1.2',
         'flask-compress>=1.9.0',
         'importlib-metadata>=4.5.0',
         'python-socketio>=5.8.0',
         'flask-socketio>=5.3.3',
-        'eventlet>=0.30.2',
-        'piwaterflow>=0.5.9',
-        'revproxy_auth>=0.1.6'
+        'eventlet==0.30.2', # Exact version required 0.30.2
+        'piwaterflow>=0.5.11',
+        'revproxy_auth>=0.1.7'
     ],
     python_requires='>=3.6',
 )
```

