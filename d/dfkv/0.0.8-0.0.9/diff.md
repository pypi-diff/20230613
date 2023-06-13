# Comparing `tmp/dfkv-0.0.8.tar.gz` & `tmp/dfkv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfkv-0.0.8.tar", last modified: Wed Apr 12 08:15:34 2023, max compression
+gzip compressed data, was "dfkv-0.0.9.tar", last modified: Tue Jun 13 07:05:30 2023, max compression
```

## Comparing `dfkv-0.0.8.tar` & `dfkv-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 08:15:34.760583 dfkv-0.0.8/
--rw-rw-rw-   0        0        0    11558 2023-03-30 02:37:23.000000 dfkv-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      380 2023-04-12 08:15:34.759112 dfkv-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      945 2023-03-30 02:37:23.000000 dfkv-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 08:15:34.748578 dfkv-0.0.8/dfkv/
--rw-rw-rw-   0        0        0      209 2023-04-06 07:33:30.000000 dfkv-0.0.8/dfkv/__init__.py
--rw-rw-rw-   0        0        0       55 2023-03-30 02:37:23.000000 dfkv-0.0.8/dfkv/common.py
--rw-rw-rw-   0        0        0     3355 2023-03-31 02:15:05.000000 dfkv-0.0.8/dfkv/dfkv.py
--rw-rw-rw-   0        0        0      853 2023-04-06 08:04:55.000000 dfkv-0.0.8/dfkv/ext.py
-drwxrwxrwx   0        0        0        0 2023-04-12 08:15:34.758499 dfkv-0.0.8/dfkv.egg-info/
--rw-rw-rw-   0        0        0      380 2023-04-12 08:15:34.000000 dfkv-0.0.8/dfkv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-04-12 08:15:34.000000 dfkv-0.0.8/dfkv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 08:15:34.000000 dfkv-0.0.8/dfkv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-12 08:15:34.000000 dfkv-0.0.8/dfkv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 08:15:34.761586 dfkv-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-04-12 08:15:14.000000 dfkv-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:05:30.607490 dfkv-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-03-30 02:37:23.000000 dfkv-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      380 2023-06-13 07:05:30.606495 dfkv-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      945 2023-03-30 02:37:23.000000 dfkv-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 07:05:30.597268 dfkv-0.0.9/dfkv/
+-rw-rw-rw-   0        0        0      231 2023-06-12 10:07:24.000000 dfkv-0.0.9/dfkv/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-30 02:37:23.000000 dfkv-0.0.9/dfkv/common.py
+-rw-rw-rw-   0        0        0     3355 2023-03-31 02:15:05.000000 dfkv-0.0.9/dfkv/dfkv.py
+-rw-rw-rw-   0        0        0     1097 2023-06-13 00:29:08.000000 dfkv-0.0.9/dfkv/dt.py
+-rw-rw-rw-   0        0        0      195 2023-06-13 01:06:26.000000 dfkv-0.0.9/dfkv/ext.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:05:30.605489 dfkv-0.0.9/dfkv.egg-info/
+-rw-rw-rw-   0        0        0      380 2023-06-13 07:05:30.000000 dfkv-0.0.9/dfkv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-06-13 07:05:30.000000 dfkv-0.0.9/dfkv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:05:30.000000 dfkv-0.0.9/dfkv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-13 07:05:30.000000 dfkv-0.0.9/dfkv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:05:30.607769 dfkv-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-06-13 00:50:37.000000 dfkv-0.0.9/setup.py
```

### Comparing `dfkv-0.0.8/LICENSE` & `dfkv-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dfkv-0.0.8/README.md` & `dfkv-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dfkv-0.0.8/dfkv/dfkv.py` & `dfkv-0.0.9/dfkv/dfkv.py`

 * *Files identical despite different names*

### Comparing `dfkv-0.0.8/dfkv/ext.py` & `dfkv-0.0.9/dfkv/dt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# this is ext utils
 from datetime import datetime, date
+import time
 
 def now(type = 1) -> str:
     """1: 2023-04-06 15:38:34.267
     2: 2023-04-06 15:38:34.267
     3: 20230406153834267
     4: 20230406153834
     5: 2023-04-06
@@ -21,11 +21,20 @@
         return date.today().strftime("%Y-%m-%d")
     elif type == 6:
         return date.today().strftime("%Y%m%d")
     
     else:
         return datetime.now()
 
+def timestamp(type = 1) -> int:
+    """
+    1: 1686615980262 -> (ms)
+    2: 1686616065 -> (s)
+    """
+    if type == 1:
+        return int(time.time() * 1000)
+    elif type == 2:
+        return int(time.time())
+    else:
+        return time.time()
 if __name__ == "__main__":
-    print(now(5))
-    print(now(6))
-    print(now(99))
+    print(timestamp(), timestamp(2), timestamp())
```

### Comparing `dfkv-0.0.8/setup.py` & `dfkv-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 from io import open
 from setuptools import setup, find_packages
 # from distutils.core import setup
 # setup(name="dfkv", version="0.0.6", description="test to install module", author="someone", py_modules=['dfkv.common'])
 setup(
     name='dfkv',
-    version='0.0.8',
+    version='0.0.9',
     description='a expand for dict',
     long_description='expand dict, can use a.b, can set value more than 1-level a.b.c.d="xyz"',
     author='fred deng',
     author_email='dfgeoff@qq.com',
     license='Apache License 2.0',
     url='https://gitee.com/hifong45/dkv.git',
     download_url='https://gitee.com/hifong45/dkv/master.zip',
     packages=find_packages(exclude=["examples", "project", "tests", "*.tests", "*.tests.*"]),  # 必填
     # package_dir={'': 'src'},  # 必填
     install_requires=[]
 )
-# 本地测试时，使用： rd /s /q dist && python setup.py sdist && pip uninstall -y dfkv && pip install dist\dfkv-0.0.8.tar.gz
+# 本地测试时，使用： rd /s /q dist && python setup.py sdist && pip uninstall -y dfkv && pip install dist\dfkv-0.0.9.tar.gz
 # 要上传时，用：rd /s /q dist && python setup.py sdist && twine upload dist/*
 # 指定用标准中心库： pip install -i https://pypi.Python.org/simple/ dfkv
 # 2023-01-28 16:16:52.993077
```

