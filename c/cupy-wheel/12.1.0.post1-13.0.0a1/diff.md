# Comparing `tmp/cupy-wheel-12.1.0.post1.tar.gz` & `tmp/cupy-wheel-13.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupy-wheel-12.1.0.post1.tar", last modified: Tue Jun 13 10:11:38 2023, max compression
+gzip compressed data, was "cupy-wheel-13.0.0a1.tar", last modified: Thu May 25 04:30:06 2023, max compression
```

## Comparing `cupy-wheel-12.1.0.post1.tar` & `cupy-wheel-13.0.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0     2180     2180        0 2023-06-13 10:11:38.292921 cupy-wheel-12.1.0.post1/
--rw-r--r--   0     2180     2180       61 2023-06-13 10:11:38.292921 cupy-wheel-12.1.0.post1/PKG-INFO
-drwxr-xr-x   0     2180     2180        0 2023-06-13 10:11:38.292921 cupy-wheel-12.1.0.post1/cupy_wheel.egg-info/
--rw-r--r--   0     2180     2180       61 2023-06-13 10:11:38.000000 cupy-wheel-12.1.0.post1/cupy_wheel.egg-info/PKG-INFO
--rw-r--r--   0     2180     2180      144 2023-06-13 10:11:38.000000 cupy-wheel-12.1.0.post1/cupy_wheel.egg-info/SOURCES.txt
--rw-r--r--   0     2180     2180        1 2023-06-13 10:11:38.000000 cupy-wheel-12.1.0.post1/cupy_wheel.egg-info/dependency_links.txt
--rw-r--r--   0     2180     2180        1 2023-06-13 10:11:38.000000 cupy-wheel-12.1.0.post1/cupy_wheel.egg-info/top_level.txt
--rw-r--r--   0     2180     2180       38 2023-06-13 10:11:38.292921 cupy-wheel-12.1.0.post1/setup.cfg
--rw-rw-r--   0     2180     2180     7774 2023-06-13 10:11:13.000000 cupy-wheel-12.1.0.post1/setup.py
+drwxr-xr-x   0     2758     2758        0 2023-05-25 04:30:06.237297 cupy-wheel-13.0.0a1/
+-rw-r--r--   0     2758     2758       57 2023-05-25 04:30:06.237297 cupy-wheel-13.0.0a1/PKG-INFO
+drwxr-xr-x   0     2758     2758        0 2023-05-25 04:30:06.237297 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/
+-rw-r--r--   0     2758     2758       57 2023-05-25 04:30:06.000000 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/PKG-INFO
+-rw-r--r--   0     2758     2758      144 2023-05-25 04:30:06.000000 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/SOURCES.txt
+-rw-r--r--   0     2758     2758        1 2023-05-25 04:30:06.000000 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/dependency_links.txt
+-rw-r--r--   0     2758     2758        1 2023-05-25 04:30:06.000000 cupy-wheel-13.0.0a1/cupy_wheel.egg-info/top_level.txt
+-rw-r--r--   0     2758     2758       38 2023-05-25 04:30:06.237297 cupy-wheel-13.0.0a1/setup.cfg
+-rw-rw-r--   0     2758     2758     8240 2023-05-25 03:52:58.000000 cupy-wheel-13.0.0a1/setup.py
```

### Comparing `cupy-wheel-12.1.0.post1/setup.py` & `cupy-wheel-13.0.0a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import ctypes
 import pkg_resources
 import os
 import sys
-from typing import List, Optional
+from typing import Dict, List, Optional
 
 from setuptools import setup
 
 
-VERSION = '12.1.0'
-META_VERSION = f'{VERSION}.post1'
+VERSION = '13.0.0a1'
 
 # List of packages supported by this version of CuPy.
 PACKAGES = [
     'cupy-cuda102',
     'cupy-cuda110',
     'cupy-cuda111',
     'cupy-cuda11x',
@@ -256,30 +255,47 @@
     if version is not None:
         return _rocm_version_to_package(version)
 
     raise AutoDetectionFailed(
         'Unable to detect NVIDIA CUDA or AMD ROCm installation.')
 
 
+def _get_cmdclass(tag: str) -> Dict[str, type]:
+    try:
+        import wheel.bdist_wheel
+    except ModuleNotFoundError:
+        return {}
+
+    class bdist_wheel_with_tag(wheel.bdist_wheel.bdist_wheel):  # type: ignore[misc] # NOQA
+        def initialize_options(self) -> None:
+            super().initialize_options()
+            self.build_number = f'0_{tag}'
+
+    return {"bdist_wheel": bdist_wheel_with_tag}
+
+
 #
 # Entrypoint
 #
 
 def main() -> None:
     if os.environ.get('CUPY_UNIVERSAL_PKG_BUILD', None) is None:
         package = infer_best_package()
         requires = f'{package}=={VERSION}'
         _log(f'Installing package: {requires}')
         install_requires = [requires]
+        tag = package
     else:
         _log('Building cupy-wheel package for release.')
         install_requires = []
+        tag = '0'
 
     setup(
         name='cupy-wheel',
-        version=META_VERSION,
+        version=f'{VERSION}',
         install_requires=install_requires,
+        cmdclass=_get_cmdclass(tag),
     )
 
 
 if __name__ == '__main__':
     main()
```

