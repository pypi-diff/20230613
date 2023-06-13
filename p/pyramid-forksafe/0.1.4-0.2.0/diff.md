# Comparing `tmp/pyramid_forksafe-0.1.4.tar.gz` & `tmp/pyramid_forksafe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_forksafe-0.1.4.tar", last modified: Thu Mar 25 20:30:42 2021, max compression
+gzip compressed data, was "pyramid_forksafe-0.2.0.tar", last modified: Tue Jun 13 21:01:06 2023, max compression
```

## Comparing `pyramid_forksafe-0.1.4.tar` & `pyramid_forksafe-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/
--rw-r--r--   0 jvanasco   (501) admin       (80)      726 2021-03-25 20:27:12.000000 pyramid_forksafe-0.1.4/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1849 2012-03-06 18:29:03.000000 pyramid_forksafe-0.1.4/LICENSE.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      440 2021-03-25 20:10:47.000000 pyramid_forksafe-0.1.4/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     7183 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-10-15 21:26:34.000000 pyramid_forksafe-0.1.4/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)     5295 2020-10-15 22:29:15.000000 pyramid_forksafe-0.1.4/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       38 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1694 2021-03-25 20:12:05.000000 pyramid_forksafe-0.1.4/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1440 2021-03-25 20:11:40.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/containers/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2016-11-09 16:17:52.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/containers/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1625 2019-09-19 22:13:06.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/containers/gunicorn.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1549 2020-10-15 22:44:31.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/containers/uwsgi.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/debugtoolbar/
--rwxrwxrwx   0 jvanasco   (501) admin       (80)      178 2019-09-19 22:13:06.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/debugtoolbar/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/debugtoolbar/panels/
--rwxrwxrwx   0 jvanasco   (501) admin       (80)        0 2017-12-05 16:49:40.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/debugtoolbar/panels/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      960 2020-10-15 21:57:47.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/debugtoolbar/panels/forksafe.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/debugtoolbar/panels/templates/
--rw-r--r--   0 jvanasco   (501) admin       (80)      175 2019-05-01 18:12:54.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/debugtoolbar/panels/templates/forksafe.dbtmako
--rw-r--r--   0 jvanasco   (501) admin       (80)     2038 2020-10-02 16:31:30.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/events.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1279 2019-09-19 22:13:06.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe/interfaces.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:12:21.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)     7183 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       62 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      808 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       17 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/src/pyramid_forksafe.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:30:42.000000 pyramid_forksafe-0.1.4/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)     5204 2020-10-15 22:47:19.000000 pyramid_forksafe-0.1.4/tests/test_config.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      137 2020-10-15 19:02:48.000000 pyramid_forksafe-0.1.4/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:06.807331 pyramid_forksafe-0.2.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      814 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1849 2012-03-06 18:29:03.000000 pyramid_forksafe-0.2.0/LICENSE.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      183 2021-03-25 20:32:54.000000 pyramid_forksafe-0.2.0/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6200 2023-06-13 21:01:06.807978 pyramid_forksafe-0.2.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5295 2020-10-15 22:29:15.000000 pyramid_forksafe-0.2.0/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      332 2023-06-13 21:01:06.817158 pyramid_forksafe-0.2.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2008 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:06.645135 pyramid_forksafe-0.2.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:06.680528 pyramid_forksafe-0.2.0/src/pyramid_forksafe/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1804 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:06.788699 pyramid_forksafe-0.2.0/src/pyramid_forksafe/containers/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2016-11-09 16:17:52.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/containers/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2056 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/containers/gunicorn.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1835 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/containers/uwsgi.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:06.790446 pyramid_forksafe-0.2.0/src/pyramid_forksafe/debugtoolbar/
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      431 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/debugtoolbar/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:06.799346 pyramid_forksafe-0.2.0/src/pyramid_forksafe/debugtoolbar/panels/
+-rwxrwxrwx   0 jvanasco   (501) admin       (80)        0 2017-12-05 16:49:40.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/debugtoolbar/panels/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1235 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/debugtoolbar/panels/forksafe.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:06.801012 pyramid_forksafe-0.2.0/src/pyramid_forksafe/debugtoolbar/panels/templates/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      175 2019-05-01 18:12:54.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/debugtoolbar/panels/templates/forksafe.dbtmako
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2239 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/events.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1368 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/interfaces.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe/py.typed
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:06.781515 pyramid_forksafe-0.2.0/src/pyramid_forksafe.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6200 2023-06-13 21:01:06.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      866 2023-06-13 21:01:06.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-13 21:01:06.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:12:21.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       67 2023-06-13 21:01:06.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       17 2023-06-13 21:01:06.000000 pyramid_forksafe-0.2.0/src/pyramid_forksafe.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 21:01:06.803053 pyramid_forksafe-0.2.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2021-03-26 17:15:08.000000 pyramid_forksafe-0.2.0/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5204 2020-10-15 22:47:19.000000 pyramid_forksafe-0.2.0/tests/test_config.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-06-13 21:01:00.000000 pyramid_forksafe-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyramid_forksafe-0.1.4/CHANGES.txt` & `pyramid_forksafe-0.2.0/CHANGES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.2.0
+    * drop python 2.7
+    * initial typing support
+    * added tests/__init__.py
+
 2021.03.25
 - v0.1.4
 * packaging fixes
 
 2020.10.20
 - v0.1.3
 - black
```

### Comparing `pyramid_forksafe-0.1.4/LICENSE.txt` & `pyramid_forksafe-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyramid_forksafe-0.1.4/PKG-INFO` & `pyramid_forksafe-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,173 +1,178 @@
 Metadata-Version: 2.1
 Name: pyramid_forksafe
-Version: 0.1.4
+Version: 0.2.0
 Summary: Standardizes server `fork` events into Pyrmamid events
 Home-page: https://github.com/jvanasco/pyramid_forksafe
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
-Description: pyramid_forksafe
-        ================
-        
-        Build Status: ![Python package](https://github.com/jvanasco/pyramid_forksafe/workflows/Python%20package/badge.svg)
-        
-        This package creates standardized Pyramid events for various forking hooks in popular deployment containers.
-        
-        Using `pyramid_forksafe` allows a developer to write generic routines for forking events, allowing them to easily swap containers during deployment or development.
-        
-        Each event is invoked with the application's `registry`, through which one can access `registry.settings`
-        
-        ## Why?
-        
-        Pyramid is Thread Safe, which is different than Fork Safe.
-        
-        Several popular libraries are not fork-safe:
-        
-        * SqlAlchemy's connection pool is not fork-safe.  Your deployment *must* call `engine.dispose()` after a fork.
-        * PyMongo's connections and locks are not fork-safe.  The entire client must be replaced after a fork.
-        * PyCrypto's Random generator will only work correctly if Random.atfork() is called.
-        
-        In some situations, a developer may need to access the registry and/or settings during postfork actions. Getting this information into a custom hook can be a hassle, as one will need to write against each container's API instead of Pyramid's. 
-        
-        This blog posting describes the difference between fork-safe and thread-safe pretty well  http://www.dctrwatson.com/2010/09/python-thread-safe-does-not-mean-fork-safe/
-        
-        
-        ## Usage - Generic
-        
-        Define a GENERIC hook.  
-        
-        	from pyramid_forksafe.events import ApplicationPostFork
-        
-            def post_fork_hook(event):
-            	"""
-            	The event has an attribute for the Pyramid Application's `registry`
-            		`event.registry`
-            	""""
-                cyrpto_atfork()
-                models.engine.dispose()
-        
-            config.add_subscriber(post_fork_hook, ApplicationPostFork)
-        
-        You can import the generic package in your `environment.ini` file (or main config), and this will try to enable services if possible:
-        
-        	# development.ini
-            pyramid.includes = pyramid_forksafe
-        
-        or you may wish to import a SPECIFIC container package in your `environment.ini` file (or main config)
-        
-        	# development.ini
-            pyramid.includes = pyramid_forksafe.containers.uwsgi
-        
-        Currently, this approach only works for `uWSGI`.  `gunicorn` requires another approach.
-        
-        
-        ## Usage - uWSGI
-        
-        simply include the package and uwsgi will be automatically enabled:
-        
-        in your `__init__.py`:
-        
-            config.include('pyramid_forksafe')
-        
-        or your `{environment}.ini`
-        
-            pyramid.includes = pyramid_forksafe
-        
-        important note:
-        
-        you MUST run uWSGI with the `--master` argument.
-        
-        
-        ## Usage - gunicorn
-        
-        `gunicorn` will need some hooks imported into it's python configuration file
-        
-        assuming you invoke gunicorn like this:
-        
-        	gunicorn --paste production.ini -c config.py
-        
-        then your `config.py` just needs to import the container hooks:
-        
-            from pyramid_forksafe.containers.gunicorn import (
-                pre_fork,
-                post_fork,
-                post_worker_init,
-            )
-        
-        those hooks are written to the `gunicorn` api, and will invoke the notification
-        
-        you can also update the debug tool by running after configuration:
-        
-        	from pyramid_forksafe.containers.gunicorn import mark_configured
-        	mark_configured(config.registry)
-        
-        
-        ## Container Support
-        
-        Currently `uwsgi` and `gunicorn` are supported with the hooks outlined below.   Celery integration is planned.  Pull requests are very welcome.
-        
-        
-        | container | pyramid\_forksafe event      | container hook |
-        |-----------|-----------------------------|------|
-        | uWSGI     | `ApplicationPostFork`       | [`postfork`](http://uwsgi-docs.readthedocs.io/en/latest/PythonDecorators.html#uwsgidecorators.postfork) |
-        | gunicorn  | `ApplicationPostFork`       | [`post_fork`](http://docs.gunicorn.org/en/latest/settings.html#post-fork) |
-        | gunicorn  | `ApplicationPreFork`        | [`pre_fork`](http://docs.gunicorn.org/en/latest/settings.html#pre-fork) |
-        | gunicorn  | `ApplicationPostWorkerInit` | [`post_worker_init`](http://docs.gunicorn.org/en/latest/settings.html#post-worker-init) |
-        
-        
-        ## The Debug Object
-        
-        including this package will put an informative dict into `registry.pyramid_forksafe`
-        
-        under waitress, it will look like this:
-        
-        	[('status', 'attempting auto-configure'),
-        	 ('environment', None),
-        	 ('autoconfigure.log', ['uWSGI not available']),
-        	 ('executed_hooks', set([]))]
-        
-        under uWSGI without master, it will look like this:
-        
-        	[('status', 'uWSGI error'),
-        	 ('environment', None),
-        	 ('autoconfigure.log',
-        	  ['uWSGI error: you have to enable the uWSGI master process to use this module']),
-        	 ('executed_hooks', set([]))]
-        
-        under uWSGI properly configured, it will look like this:
-        
-        	[('status', 'uWSGI hook configured'),
-        	 ('environment', 'uWSGI'),
-        	 ('autoconfigure.log', ['uWSGI available', 'uWSGI hook configured']),
-        	 ('executed_hooks',
-        	  set([('containers.uwsgi.post_fork_hook', 'ApplicationPostFork')]))]
-        
-        
-        ## Debugtoolbar support
-        
-        to enable the debugtoobar support, you can configure your `development.ini` with:
-        
-        	debugtoolbar.includes = pyramid_forksafe.debugtoolbar
-        
-        The toolbar just shows the debug object `request.registry.pyramid_forksafe` on the toolbar
-        
-        This should always show an error, because the debugtoolbar does not run under forking servers.
-        
-        
-        
-        ## Status
-        2019.05.01 - debugtoolbar
-        2019.04.30 - debug object
-        2019.04.29 - Python3 Support. This has been production safe for uWSGI for a while now.
-        2016.11.09 - this is experimental
-        
 Keywords: web pyramid fork uwsgi nginx
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE.txt
+
+pyramid_forksafe
+================
+
+Build Status: ![Python package](https://github.com/jvanasco/pyramid_forksafe/workflows/Python%20package/badge.svg)
+
+This package creates standardized Pyramid events for various forking hooks in popular deployment containers.
+
+Using `pyramid_forksafe` allows a developer to write generic routines for forking events, allowing them to easily swap containers during deployment or development.
+
+Each event is invoked with the application's `registry`, through which one can access `registry.settings`
+
+## Why?
+
+Pyramid is Thread Safe, which is different than Fork Safe.
+
+Several popular libraries are not fork-safe:
+
+* SqlAlchemy's connection pool is not fork-safe.  Your deployment *must* call `engine.dispose()` after a fork.
+* PyMongo's connections and locks are not fork-safe.  The entire client must be replaced after a fork.
+* PyCrypto's Random generator will only work correctly if Random.atfork() is called.
+
+In some situations, a developer may need to access the registry and/or settings during postfork actions. Getting this information into a custom hook can be a hassle, as one will need to write against each container's API instead of Pyramid's. 
+
+This blog posting describes the difference between fork-safe and thread-safe pretty well  http://www.dctrwatson.com/2010/09/python-thread-safe-does-not-mean-fork-safe/
+
+
+## Usage - Generic
+
+Define a GENERIC hook.  
+
+	from pyramid_forksafe.events import ApplicationPostFork
+
+    def post_fork_hook(event):
+    	"""
+    	The event has an attribute for the Pyramid Application's `registry`
+    		`event.registry`
+    	""""
+        cyrpto_atfork()
+        models.engine.dispose()
+
+    config.add_subscriber(post_fork_hook, ApplicationPostFork)
+
+You can import the generic package in your `environment.ini` file (or main config), and this will try to enable services if possible:
+
+	# development.ini
+    pyramid.includes = pyramid_forksafe
+
+or you may wish to import a SPECIFIC container package in your `environment.ini` file (or main config)
+
+	# development.ini
+    pyramid.includes = pyramid_forksafe.containers.uwsgi
+
+Currently, this approach only works for `uWSGI`.  `gunicorn` requires another approach.
+
+
+## Usage - uWSGI
+
+simply include the package and uwsgi will be automatically enabled:
+
+in your `__init__.py`:
+
+    config.include('pyramid_forksafe')
+
+or your `{environment}.ini`
+
+    pyramid.includes = pyramid_forksafe
+
+important note:
+
+you MUST run uWSGI with the `--master` argument.
+
+
+## Usage - gunicorn
+
+`gunicorn` will need some hooks imported into it's python configuration file
+
+assuming you invoke gunicorn like this:
+
+	gunicorn --paste production.ini -c config.py
+
+then your `config.py` just needs to import the container hooks:
+
+    from pyramid_forksafe.containers.gunicorn import (
+        pre_fork,
+        post_fork,
+        post_worker_init,
+    )
+
+those hooks are written to the `gunicorn` api, and will invoke the notification
+
+you can also update the debug tool by running after configuration:
+
+	from pyramid_forksafe.containers.gunicorn import mark_configured
+	mark_configured(config.registry)
+
+
+## Container Support
+
+Currently `uwsgi` and `gunicorn` are supported with the hooks outlined below.   Celery integration is planned.  Pull requests are very welcome.
+
+
+| container | pyramid\_forksafe event      | container hook |
+|-----------|-----------------------------|------|
+| uWSGI     | `ApplicationPostFork`       | [`postfork`](http://uwsgi-docs.readthedocs.io/en/latest/PythonDecorators.html#uwsgidecorators.postfork) |
+| gunicorn  | `ApplicationPostFork`       | [`post_fork`](http://docs.gunicorn.org/en/latest/settings.html#post-fork) |
+| gunicorn  | `ApplicationPreFork`        | [`pre_fork`](http://docs.gunicorn.org/en/latest/settings.html#pre-fork) |
+| gunicorn  | `ApplicationPostWorkerInit` | [`post_worker_init`](http://docs.gunicorn.org/en/latest/settings.html#post-worker-init) |
+
+
+## The Debug Object
+
+including this package will put an informative dict into `registry.pyramid_forksafe`
+
+under waitress, it will look like this:
+
+	[('status', 'attempting auto-configure'),
+	 ('environment', None),
+	 ('autoconfigure.log', ['uWSGI not available']),
+	 ('executed_hooks', set([]))]
+
+under uWSGI without master, it will look like this:
+
+	[('status', 'uWSGI error'),
+	 ('environment', None),
+	 ('autoconfigure.log',
+	  ['uWSGI error: you have to enable the uWSGI master process to use this module']),
+	 ('executed_hooks', set([]))]
+
+under uWSGI properly configured, it will look like this:
+
+	[('status', 'uWSGI hook configured'),
+	 ('environment', 'uWSGI'),
+	 ('autoconfigure.log', ['uWSGI available', 'uWSGI hook configured']),
+	 ('executed_hooks',
+	  set([('containers.uwsgi.post_fork_hook', 'ApplicationPostFork')]))]
+
+
+## Debugtoolbar support
+
+to enable the debugtoobar support, you can configure your `development.ini` with:
+
+	debugtoolbar.includes = pyramid_forksafe.debugtoolbar
+
+The toolbar just shows the debug object `request.registry.pyramid_forksafe` on the toolbar
+
+This should always show an error, because the debugtoolbar does not run under forking servers.
+
+
+
+## Status
+2019.05.01 - debugtoolbar
+2019.04.30 - debug object
+2019.04.29 - Python3 Support. This has been production safe for uWSGI for a while now.
+2016.11.09 - this is experimental
```

### Comparing `pyramid_forksafe-0.1.4/README.md` & `pyramid_forksafe-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyramid_forksafe-0.1.4/setup.py` & `pyramid_forksafe-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 requires = [
     "pyramid",
     "zope.interface",  # should be in pyramid
 ]
 tests_require = [
+    "mypy",
     "pytest",
     "pyramid_debugtoolbar",
 ]
 testing_extras = tests_require + []
 
 
 setup(
@@ -39,24 +40,30 @@
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Intended Audience :: Developers",
         "Framework :: Pyramid",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     keywords="web pyramid fork uwsgi nginx",
     license="MIT",
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
+    package_data={"pyramid_forksafe": ["py.typed"]},
     include_package_data=True,
     zip_safe=False,
     install_requires=requires,
     tests_require=requires,
     extras_require={
         "testing": testing_extras,
     },
```

### Comparing `pyramid_forksafe-0.1.4/src/pyramid_forksafe/__init__.py` & `pyramid_forksafe-0.2.0/src/pyramid_forksafe/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+# stydlib
 import logging
+from typing import TYPE_CHECKING
 
-log = logging.getLogger(__name__)
+# typing
+if TYPE_CHECKING:
+    from pyramid.config import Configurator  # type: ignore[import]
 
+# ==============================================================================
 
-__VERSION__ = "0.1.4"
+__VERSION__ = "0.2.0"
 
+# ------------------------------------------------------------------------------
 
-# ==============================================================================
+log = logging.getLogger(__name__)
+
+# ------------------------------------------------------------------------------
 
 
-def registry_setup(config):
+def registry_setup(config: "Configurator") -> None:
     """
     This function does the initial setup.
     Originally it was part of `includeme`, but has been migrated away so
     per-container setups can be used instead.
     """
     log.debug("registry_setup")
     config.registry.pyramid_forksafe = {
         "status": "attempting auto-configure",
         "autoconfigure.log": [],
         "environment": None,
         "executed_hooks": set([]),
     }
 
 
-def includeme(config):
+def includeme(config: "Configurator") -> None:
     """
     this will try to auto-detect supported containers
 
     uWSGI will only load when run under that environment.
 
     gunicorn must run with the hooks enabled in it's own startup
     """
@@ -46,8 +54,12 @@
         config.registry.pyramid_forksafe["autoconfigure.log"].append(
             "uWSGI error: %s" % exc
         )
         config.registry.pyramid_forksafe["status"] = "uWSGI error"
         log.error("- uWSGI EXCEPTION | %s", exc)
 
 
-__all__ = ("__VERSION__", "includeme", "registry_setup")
+__all__ = (
+    "__VERSION__",
+    "includeme",
+    "registry_setup",
+)
```

### Comparing `pyramid_forksafe-0.1.4/src/pyramid_forksafe/containers/gunicorn.py` & `pyramid_forksafe-0.2.0/src/pyramid_forksafe/containers/gunicorn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,62 @@
+# stdlib
 import logging
-
-log = logging.getLogger(__name__)
-
+from typing import TYPE_CHECKING
 
 # local
-from pyramid_forksafe.events import (
-    ApplicationPostFork,
-    ApplicationPreFork,
-    ApplicationPostWorkerInit,
-)
-
+from pyramid_forksafe.events import ApplicationPostFork
+from pyramid_forksafe.events import ApplicationPostWorkerInit
+from pyramid_forksafe.events import ApplicationPreFork
+
+# typing
+if TYPE_CHECKING:
+    from pyramid.registry import Registry  # type: ignore[import]
+    from gunicorn.workers.base import Worker  # type: ignore[import]
 
 # ==============================================================================
 
+log = logging.getLogger(__name__)
+
+# ------------------------------------------------------------------------------
 
-def mark_configured(registry):
+
+def mark_configured(registry: "Registry") -> None:
     """utility for developers to update the status"""
     log.debug("mark_configured")
     registry.pyramid_forksafe["environment"] = "gunicorn"
     registry.pyramid_forksafe["autoconfigure.log"].append("gunicorn mark_configured")
     registry.pyramid_forksafe["status"] = "gunicorn mark_configured"
 
 
-def pre_fork(server, worker):
+def pre_fork(server, worker: "Worker") -> None:
     log.debug("ApplicationPreFork(gunicorn) - pre_fork")
     registry = server.app.wsgi().registry
     registry.notify(ApplicationPreFork(registry))
     registry.pyramid_forksafe["executed_hooks"].add(
         ("containers.gunicorn.pre_fork", "ApplicationPreFork")
     )
 
 
-def post_fork(server, worker):
+def post_fork(server, worker: "Worker") -> None:
     log.debug("ApplicationPostFork(gunicorn) - post_fork")
     registry = server.app.wsgi().registry
     registry.notify(ApplicationPostFork(registry))
     registry.pyramid_forksafe["executed_hooks"].add(
         ("containers.gunicorn.post_fork", "ApplicationPostFork")
     )
 
 
-def post_worker_init(worker):
+def post_worker_init(worker: "Worker") -> None:
     log.debug("ApplicationPostWorkerInit(gunicorn) - post_worker_init")
     registry = worker.app.wsgi().registry
     registry.notify(ApplicationPostWorkerInit(registry))
     registry.pyramid_forksafe["executed_hooks"].add(
         ("containers.gunicorn.post_worker_init", "ApplicationPostWorkerInit")
     )
 
 
-__all__ = ("mark_configured", "pre_fork", "post_fork", "post_worker_init")
+__all__ = (
+    "mark_configured",
+    "post_fork",
+    "post_worker_init",
+    "pre_fork",
+)
```

### Comparing `pyramid_forksafe-0.1.4/src/pyramid_forksafe/debugtoolbar/panels/forksafe.py` & `pyramid_forksafe-0.2.0/src/pyramid_forksafe/debugtoolbar/panels/forksafe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,18 @@
-from pyramid_debugtoolbar.panels import DebugPanel
+# stdlib
+from typing import TYPE_CHECKING
 
-_ = lambda x: x
+# pypi
+from pyramid_debugtoolbar.panels import DebugPanel  # type: ignore[import]
+
+# typing
+if TYPE_CHECKING:
+    from pyramid.request import Request  # type: ignore[import]
+
+# ==============================================================================
 
 
 class PyramidForksafeDebugPanel(DebugPanel):
     """
     Sample debug panel
     """
 
@@ -14,28 +22,28 @@
 
     # only query the policy once
     _policy = None
 
     # stash
     _cookie_names = None
 
-    def __init__(self, request):
+    def __init__(self, request: "Request"):
         if hasattr(request.registry, "pyramid_forksafe"):
             self.data = {"registry_data": request.registry.pyramid_forksafe}
         else:
             # this can happen if we include the toolbar, but not the library
             self.data = {"registry_data": None}
 
     @property
-    def nav_title(self):
-        return _(self.name)
+    def nav_title(self) -> str:
+        return self.name
 
     @property
-    def title(self):
-        return _(self.name)
+    def title(self) -> str:
+        return self.name
 
     @property
-    def url(self):
+    def url(self) -> str:
         return ""
 
-    def render_content(self, request):
+    def render_content(self, request: "Request") -> str:
         return DebugPanel.render_content(self, request)
```

### Comparing `pyramid_forksafe-0.1.4/src/pyramid_forksafe/events.py` & `pyramid_forksafe-0.2.0/src/pyramid_forksafe/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from __future__ import print_function
+# stdlib
+from typing import TYPE_CHECKING
 
 # pypi
-from zope.interface import implementer
+from zope.interface import implementer  # type: ignore[import]
 
 # local
-from .interfaces import (
-    IApplicationPostFork,
-    IApplicationPreFork,
-    IApplicationPostWorkerInit,
-)
-
+from .interfaces import IApplicationPostFork
+from .interfaces import IApplicationPostWorkerInit
+from .interfaces import IApplicationPreFork
+
+# typing
+if TYPE_CHECKING:
+    from pyramid.registry import Registry  # type: ignore[import]
 
 # ==============================================================================
 
 
 @implementer(IApplicationPostFork)
 class ApplicationPostFork(object):
     """An instance of this class is emitted as an :term:`event` when
@@ -25,15 +27,15 @@
     The instance has an attribute, ``registry``, which corresponds to
     the current registry.
 
     This class implements the
     :class:`pyramid_forksafe.interfaces.IApplicationPostFork` interface.
     """
 
-    def __init__(self, registry):
+    def __init__(self, registry: "Registry"):
         print("ApplicationPostFork")
         self.registry = registry
 
 
 @implementer(IApplicationPreFork)
 class ApplicationPreFork(object):
     """An instance of this class is emitted as an :term:`event` when
@@ -44,15 +46,15 @@
     The instance has an attribute, ``registry``, which corresponds to
     the current registry.
 
     This class implements the
     :class:`pyramid_forksafe.interfaces.IApplicationPreFork` interface.
     """
 
-    def __init__(self, registry):
+    def __init__(self, registry: "Registry"):
         print("ApplicationPreFork")
         self.registry = registry
 
 
 @implementer(IApplicationPostWorkerInit)
 class ApplicationPostWorkerInit(object):
     """An instance of this class is emitted as an :term:`event` when
@@ -63,13 +65,17 @@
     The instance has an attribute, ``registry``, which corresponds to
     the current registry.
 
     This class implements the
     :class:`pyramid_forksafe.interfaces.IApplicationPostWorkerInit` interface.
     """
 
-    def __init__(self, registry):
+    def __init__(self, registry: "Registry"):
         print("ApplicationPostWorkerInit")
         self.registry = registry
 
 
-__all__ = ("ApplicationPostFork", "ApplicationPreFork", "ApplicationPostWorkerInit")
+__all__ = (
+    "ApplicationPostFork",
+    "ApplicationPreFork",
+    "ApplicationPostWorkerInit",
+)
```

### Comparing `pyramid_forksafe-0.1.4/src/pyramid_forksafe.egg-info/PKG-INFO` & `pyramid_forksafe-0.2.0/src/pyramid_forksafe.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,173 +1,178 @@
 Metadata-Version: 2.1
 Name: pyramid-forksafe
-Version: 0.1.4
+Version: 0.2.0
 Summary: Standardizes server `fork` events into Pyrmamid events
 Home-page: https://github.com/jvanasco/pyramid_forksafe
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
-Description: pyramid_forksafe
-        ================
-        
-        Build Status: ![Python package](https://github.com/jvanasco/pyramid_forksafe/workflows/Python%20package/badge.svg)
-        
-        This package creates standardized Pyramid events for various forking hooks in popular deployment containers.
-        
-        Using `pyramid_forksafe` allows a developer to write generic routines for forking events, allowing them to easily swap containers during deployment or development.
-        
-        Each event is invoked with the application's `registry`, through which one can access `registry.settings`
-        
-        ## Why?
-        
-        Pyramid is Thread Safe, which is different than Fork Safe.
-        
-        Several popular libraries are not fork-safe:
-        
-        * SqlAlchemy's connection pool is not fork-safe.  Your deployment *must* call `engine.dispose()` after a fork.
-        * PyMongo's connections and locks are not fork-safe.  The entire client must be replaced after a fork.
-        * PyCrypto's Random generator will only work correctly if Random.atfork() is called.
-        
-        In some situations, a developer may need to access the registry and/or settings during postfork actions. Getting this information into a custom hook can be a hassle, as one will need to write against each container's API instead of Pyramid's. 
-        
-        This blog posting describes the difference between fork-safe and thread-safe pretty well  http://www.dctrwatson.com/2010/09/python-thread-safe-does-not-mean-fork-safe/
-        
-        
-        ## Usage - Generic
-        
-        Define a GENERIC hook.  
-        
-        	from pyramid_forksafe.events import ApplicationPostFork
-        
-            def post_fork_hook(event):
-            	"""
-            	The event has an attribute for the Pyramid Application's `registry`
-            		`event.registry`
-            	""""
-                cyrpto_atfork()
-                models.engine.dispose()
-        
-            config.add_subscriber(post_fork_hook, ApplicationPostFork)
-        
-        You can import the generic package in your `environment.ini` file (or main config), and this will try to enable services if possible:
-        
-        	# development.ini
-            pyramid.includes = pyramid_forksafe
-        
-        or you may wish to import a SPECIFIC container package in your `environment.ini` file (or main config)
-        
-        	# development.ini
-            pyramid.includes = pyramid_forksafe.containers.uwsgi
-        
-        Currently, this approach only works for `uWSGI`.  `gunicorn` requires another approach.
-        
-        
-        ## Usage - uWSGI
-        
-        simply include the package and uwsgi will be automatically enabled:
-        
-        in your `__init__.py`:
-        
-            config.include('pyramid_forksafe')
-        
-        or your `{environment}.ini`
-        
-            pyramid.includes = pyramid_forksafe
-        
-        important note:
-        
-        you MUST run uWSGI with the `--master` argument.
-        
-        
-        ## Usage - gunicorn
-        
-        `gunicorn` will need some hooks imported into it's python configuration file
-        
-        assuming you invoke gunicorn like this:
-        
-        	gunicorn --paste production.ini -c config.py
-        
-        then your `config.py` just needs to import the container hooks:
-        
-            from pyramid_forksafe.containers.gunicorn import (
-                pre_fork,
-                post_fork,
-                post_worker_init,
-            )
-        
-        those hooks are written to the `gunicorn` api, and will invoke the notification
-        
-        you can also update the debug tool by running after configuration:
-        
-        	from pyramid_forksafe.containers.gunicorn import mark_configured
-        	mark_configured(config.registry)
-        
-        
-        ## Container Support
-        
-        Currently `uwsgi` and `gunicorn` are supported with the hooks outlined below.   Celery integration is planned.  Pull requests are very welcome.
-        
-        
-        | container | pyramid\_forksafe event      | container hook |
-        |-----------|-----------------------------|------|
-        | uWSGI     | `ApplicationPostFork`       | [`postfork`](http://uwsgi-docs.readthedocs.io/en/latest/PythonDecorators.html#uwsgidecorators.postfork) |
-        | gunicorn  | `ApplicationPostFork`       | [`post_fork`](http://docs.gunicorn.org/en/latest/settings.html#post-fork) |
-        | gunicorn  | `ApplicationPreFork`        | [`pre_fork`](http://docs.gunicorn.org/en/latest/settings.html#pre-fork) |
-        | gunicorn  | `ApplicationPostWorkerInit` | [`post_worker_init`](http://docs.gunicorn.org/en/latest/settings.html#post-worker-init) |
-        
-        
-        ## The Debug Object
-        
-        including this package will put an informative dict into `registry.pyramid_forksafe`
-        
-        under waitress, it will look like this:
-        
-        	[('status', 'attempting auto-configure'),
-        	 ('environment', None),
-        	 ('autoconfigure.log', ['uWSGI not available']),
-        	 ('executed_hooks', set([]))]
-        
-        under uWSGI without master, it will look like this:
-        
-        	[('status', 'uWSGI error'),
-        	 ('environment', None),
-        	 ('autoconfigure.log',
-        	  ['uWSGI error: you have to enable the uWSGI master process to use this module']),
-        	 ('executed_hooks', set([]))]
-        
-        under uWSGI properly configured, it will look like this:
-        
-        	[('status', 'uWSGI hook configured'),
-        	 ('environment', 'uWSGI'),
-        	 ('autoconfigure.log', ['uWSGI available', 'uWSGI hook configured']),
-        	 ('executed_hooks',
-        	  set([('containers.uwsgi.post_fork_hook', 'ApplicationPostFork')]))]
-        
-        
-        ## Debugtoolbar support
-        
-        to enable the debugtoobar support, you can configure your `development.ini` with:
-        
-        	debugtoolbar.includes = pyramid_forksafe.debugtoolbar
-        
-        The toolbar just shows the debug object `request.registry.pyramid_forksafe` on the toolbar
-        
-        This should always show an error, because the debugtoolbar does not run under forking servers.
-        
-        
-        
-        ## Status
-        2019.05.01 - debugtoolbar
-        2019.04.30 - debug object
-        2019.04.29 - Python3 Support. This has been production safe for uWSGI for a while now.
-        2016.11.09 - this is experimental
-        
 Keywords: web pyramid fork uwsgi nginx
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE.txt
+
+pyramid_forksafe
+================
+
+Build Status: ![Python package](https://github.com/jvanasco/pyramid_forksafe/workflows/Python%20package/badge.svg)
+
+This package creates standardized Pyramid events for various forking hooks in popular deployment containers.
+
+Using `pyramid_forksafe` allows a developer to write generic routines for forking events, allowing them to easily swap containers during deployment or development.
+
+Each event is invoked with the application's `registry`, through which one can access `registry.settings`
+
+## Why?
+
+Pyramid is Thread Safe, which is different than Fork Safe.
+
+Several popular libraries are not fork-safe:
+
+* SqlAlchemy's connection pool is not fork-safe.  Your deployment *must* call `engine.dispose()` after a fork.
+* PyMongo's connections and locks are not fork-safe.  The entire client must be replaced after a fork.
+* PyCrypto's Random generator will only work correctly if Random.atfork() is called.
+
+In some situations, a developer may need to access the registry and/or settings during postfork actions. Getting this information into a custom hook can be a hassle, as one will need to write against each container's API instead of Pyramid's. 
+
+This blog posting describes the difference between fork-safe and thread-safe pretty well  http://www.dctrwatson.com/2010/09/python-thread-safe-does-not-mean-fork-safe/
+
+
+## Usage - Generic
+
+Define a GENERIC hook.  
+
+	from pyramid_forksafe.events import ApplicationPostFork
+
+    def post_fork_hook(event):
+    	"""
+    	The event has an attribute for the Pyramid Application's `registry`
+    		`event.registry`
+    	""""
+        cyrpto_atfork()
+        models.engine.dispose()
+
+    config.add_subscriber(post_fork_hook, ApplicationPostFork)
+
+You can import the generic package in your `environment.ini` file (or main config), and this will try to enable services if possible:
+
+	# development.ini
+    pyramid.includes = pyramid_forksafe
+
+or you may wish to import a SPECIFIC container package in your `environment.ini` file (or main config)
+
+	# development.ini
+    pyramid.includes = pyramid_forksafe.containers.uwsgi
+
+Currently, this approach only works for `uWSGI`.  `gunicorn` requires another approach.
+
+
+## Usage - uWSGI
+
+simply include the package and uwsgi will be automatically enabled:
+
+in your `__init__.py`:
+
+    config.include('pyramid_forksafe')
+
+or your `{environment}.ini`
+
+    pyramid.includes = pyramid_forksafe
+
+important note:
+
+you MUST run uWSGI with the `--master` argument.
+
+
+## Usage - gunicorn
+
+`gunicorn` will need some hooks imported into it's python configuration file
+
+assuming you invoke gunicorn like this:
+
+	gunicorn --paste production.ini -c config.py
+
+then your `config.py` just needs to import the container hooks:
+
+    from pyramid_forksafe.containers.gunicorn import (
+        pre_fork,
+        post_fork,
+        post_worker_init,
+    )
+
+those hooks are written to the `gunicorn` api, and will invoke the notification
+
+you can also update the debug tool by running after configuration:
+
+	from pyramid_forksafe.containers.gunicorn import mark_configured
+	mark_configured(config.registry)
+
+
+## Container Support
+
+Currently `uwsgi` and `gunicorn` are supported with the hooks outlined below.   Celery integration is planned.  Pull requests are very welcome.
+
+
+| container | pyramid\_forksafe event      | container hook |
+|-----------|-----------------------------|------|
+| uWSGI     | `ApplicationPostFork`       | [`postfork`](http://uwsgi-docs.readthedocs.io/en/latest/PythonDecorators.html#uwsgidecorators.postfork) |
+| gunicorn  | `ApplicationPostFork`       | [`post_fork`](http://docs.gunicorn.org/en/latest/settings.html#post-fork) |
+| gunicorn  | `ApplicationPreFork`        | [`pre_fork`](http://docs.gunicorn.org/en/latest/settings.html#pre-fork) |
+| gunicorn  | `ApplicationPostWorkerInit` | [`post_worker_init`](http://docs.gunicorn.org/en/latest/settings.html#post-worker-init) |
+
+
+## The Debug Object
+
+including this package will put an informative dict into `registry.pyramid_forksafe`
+
+under waitress, it will look like this:
+
+	[('status', 'attempting auto-configure'),
+	 ('environment', None),
+	 ('autoconfigure.log', ['uWSGI not available']),
+	 ('executed_hooks', set([]))]
+
+under uWSGI without master, it will look like this:
+
+	[('status', 'uWSGI error'),
+	 ('environment', None),
+	 ('autoconfigure.log',
+	  ['uWSGI error: you have to enable the uWSGI master process to use this module']),
+	 ('executed_hooks', set([]))]
+
+under uWSGI properly configured, it will look like this:
+
+	[('status', 'uWSGI hook configured'),
+	 ('environment', 'uWSGI'),
+	 ('autoconfigure.log', ['uWSGI available', 'uWSGI hook configured']),
+	 ('executed_hooks',
+	  set([('containers.uwsgi.post_fork_hook', 'ApplicationPostFork')]))]
+
+
+## Debugtoolbar support
+
+to enable the debugtoobar support, you can configure your `development.ini` with:
+
+	debugtoolbar.includes = pyramid_forksafe.debugtoolbar
+
+The toolbar just shows the debug object `request.registry.pyramid_forksafe` on the toolbar
+
+This should always show an error, because the debugtoolbar does not run under forking servers.
+
+
+
+## Status
+2019.05.01 - debugtoolbar
+2019.04.30 - debug object
+2019.04.29 - Python3 Support. This has been production safe for uWSGI for a while now.
+2016.11.09 - this is experimental
```

### Comparing `pyramid_forksafe-0.1.4/src/pyramid_forksafe.egg-info/SOURCES.txt` & `pyramid_forksafe-0.2.0/src/pyramid_forksafe.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 CHANGES.txt
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 tox.ini
 src/pyramid_forksafe/__init__.py
 src/pyramid_forksafe/events.py
 src/pyramid_forksafe/interfaces.py
+src/pyramid_forksafe/py.typed
 src/pyramid_forksafe.egg-info/PKG-INFO
 src/pyramid_forksafe.egg-info/SOURCES.txt
 src/pyramid_forksafe.egg-info/dependency_links.txt
 src/pyramid_forksafe.egg-info/not-zip-safe
 src/pyramid_forksafe.egg-info/requires.txt
 src/pyramid_forksafe.egg-info/top_level.txt
 src/pyramid_forksafe/containers/__init__.py
 src/pyramid_forksafe/containers/gunicorn.py
 src/pyramid_forksafe/containers/uwsgi.py
 src/pyramid_forksafe/debugtoolbar/__init__.py
 src/pyramid_forksafe/debugtoolbar/panels/__init__.py
 src/pyramid_forksafe/debugtoolbar/panels/forksafe.py
 src/pyramid_forksafe/debugtoolbar/panels/templates/forksafe.dbtmako
+tests/__init__.py
 tests/test_config.py
```

### Comparing `pyramid_forksafe-0.1.4/tests/test_config.py` & `pyramid_forksafe-0.2.0/tests/test_config.py`

 * *Files identical despite different names*

