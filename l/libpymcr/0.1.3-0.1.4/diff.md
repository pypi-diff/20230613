# Comparing `tmp/libpymcr-0.1.3-cp39-cp39-win_amd64.whl.zip` & `tmp/libpymcr-0.1.4-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 194258 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     5010 b- defN 23-Jun-10 12:39 libpymcr/Matlab.py
--rw-rw-rw-  2.0 fat     9690 b- defN 23-Jun-10 12:39 libpymcr/MatlabProxyObject.py
--rw-rw-rw-  2.0 fat      175 b- defN 23-Jun-10 12:39 libpymcr/__init__.py
--rw-rw-rw-  2.0 fat   450048 b- defN 23-Jun-10 12:47 libpymcr/_libpymcr.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      518 b- defN 23-Jun-10 12:46 libpymcr/_version.py
--rw-rw-rw-  2.0 fat     8382 b- defN 23-Jun-10 12:39 libpymcr/utils.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2586 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      875 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/RECORD
-11 files, 513216 bytes uncompressed, 192790 bytes compressed:  62.4%
+Zip file size: 198295 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat    11938 b- defN 23-Jun-13 11:21 libpymcr/IPythonMagics.py
+-rw-rw-rw-  2.0 fat     6599 b- defN 23-Jun-13 11:21 libpymcr/Matlab.py
+-rw-rw-rw-  2.0 fat     9690 b- defN 23-Jun-13 11:21 libpymcr/MatlabProxyObject.py
+-rw-rw-rw-  2.0 fat      175 b- defN 23-Jun-13 11:21 libpymcr/__init__.py
+-rw-rw-rw-  2.0 fat   450048 b- defN 23-Jun-13 11:27 libpymcr/_libpymcr.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      518 b- defN 23-Jun-13 11:26 libpymcr/_version.py
+-rw-rw-rw-  2.0 fat     8382 b- defN 23-Jun-13 11:21 libpymcr/utils.py
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-13 11:27 libpymcr-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-Jun-13 11:27 libpymcr-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-13 11:27 libpymcr-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-13 11:27 libpymcr-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      958 b- defN 23-Jun-13 11:27 libpymcr-0.1.4.dist-info/RECORD
+12 files, 526826 bytes uncompressed, 196701 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: libpymcr/IPythonMagics.py
+Comment: 
+
 Filename: libpymcr/Matlab.py
 Comment: 
 
 Filename: libpymcr/MatlabProxyObject.py
 Comment: 
 
 Filename: libpymcr/__init__.py
@@ -12,23 +15,23 @@
 
 Filename: libpymcr/_version.py
 Comment: 
 
 Filename: libpymcr/utils.py
 Comment: 
 
-Filename: libpymcr-0.1.3.dist-info/LICENSE
+Filename: libpymcr-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: libpymcr-0.1.3.dist-info/METADATA
+Filename: libpymcr-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: libpymcr-0.1.3.dist-info/WHEEL
+Filename: libpymcr-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: libpymcr-0.1.3.dist-info/top_level.txt
+Filename: libpymcr-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: libpymcr-0.1.3.dist-info/RECORD
+Filename: libpymcr-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libpymcr/Matlab.py

```diff
@@ -5,14 +5,16 @@
 from .MatlabProxyObject import wrap, unwrap
 from .utils import get_version_from_ctf, checkPath, get_nlhs
 
 # Store the Matlab engine as a module global wrapped inside a class
 # When the global ref is deleted (e.g. when Python exits) the __del__ method is called
 # Which then gracefully shutsdown Matlab, else we get a segfault.
 _global_matlab_ref = None
+_has_registered_magic = None
+
 
 class _MatlabInstance(object):
     def __init__(self, ctffile, matlab_dir=None, options=None):
         ctffile = os.path.abspath(ctffile)
         if not os.path.exists(ctffile):
             raise RuntimeError('CTF file {} does not exist'.format(ctffile))
         if matlab_dir is None:
@@ -59,25 +61,27 @@
 
     def getdoc(self):
         # To avoid error message printing in Spyder
         raise NotImplementedError
 
 
 class Matlab(object):
-    def __init__(self, ctffile, mlPath=None):
+    def __init__(self, ctffile=None, mlPath=None):
         """
         Create an interface to a matlab compiled python library and treat the objects in a python/matlab way instead of
         the ugly way it is done by default.
 
         :param mlPath: Path to the SDK i.e. '/MATLAB/MATLAB_Runtime/v96' or to the location where matlab is installed
                        (MATLAB root directory). If omitted, will attempt to find Matlab folder automatically
         """
 
         global _global_matlab_ref
         if _global_matlab_ref is None:
+            if ctffile is None:
+                raise RuntimeError('Matlab is not initialised, please provide a CTF path')
             _global_matlab_ref = _MatlabInstance(ctffile, mlPath)
         self._interface = _global_matlab_ref.interface
 
     def __getattr__(self, name):
         """
         Override for the get attribute. We don't want to call the process but the interface, so redirect calls there and
         return a MatlabProxyObject
@@ -110,7 +114,40 @@
                 except ValueError:
                     inputs = []
                 try:
                     outputs = [_get_xml_val(v) for v in _get_xml_tag(info, 'outputs', '/outputs')]
                 except ValueError:
                     outputs = []
                 print('[{}] = {}({})'.format(','.join(outputs), ml_name, ','.join(inputs)))
+
+
+def register_ipython_magics():
+    try:
+        import IPython
+    except ImportError:
+        return None
+    else:
+        running_kernel = IPython.get_ipython()
+        # Only register these magics when running in a notebook / lab
+        # Other values seen are: 'TerminalInteractiveShell' and 'InteractiveShellEmbed'
+        if (running_kernel.__class__.__name__ != 'ZMQInteractiveShell'
+            and running_kernel.__class__.__name__ != 'SpyderShell'):
+            return None
+    global _has_registered_magic
+    _has_registered_magic = True
+    if running_kernel is None or sys.__stdout__ is None or sys.__stderr__ is None:
+        return None
+    from . import IPythonMagics
+    from traitlets import Instance
+    shell = Instance('IPython.core.interactiveshell.InteractiveShellABC', allow_none=True)
+    magics = IPythonMagics.MatlabMagics(shell, None)
+    running_kernel.register_magics(magics)
+    running_kernel.events.register('post_run_cell', IPythonMagics.showPlot)
+    # Only do redirection for Jupyter notebooks - causes errors on Spyder
+    if running_kernel == 'ZMQInteractiveShell':
+        redirect_stdout = IPythonMagics.Redirection(target='stdout')
+        running_kernel.events.register('pre_run_cell', redirect_stdout.pre)
+        running_kernel.events.register('post_run_cell', redirect_stdout.post)
+
+
+if not _has_registered_magic:
+    register_ipython_magics()
```

## libpymcr/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-06-10T13:38:34+0100",
+ "date": "2023-06-13T12:20:09+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "64efaca1fe8fbd4db077242cba100cd70dc40db8",
- "version": "0.1.3"
+ "full-revisionid": "38ea9ecded327300820c84c8f35a829689273724",
+ "version": "0.1.4"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `libpymcr-0.1.3.dist-info/LICENSE` & `libpymcr-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libpymcr-0.1.3.dist-info/METADATA` & `libpymcr-0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpymcr
-Version: 0.1.3
+Version: 0.1.4
 Summary: A module to allow Python to call functions from a compiled Matlab archive
 Home-page: https://github.com/pace-neutrons/libpymcr
 Author: Duc Le
 Author-email: duc.le@stfc.ac.uk
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

