# Comparing `tmp/mciplayer-2.0.0.tar.gz` & `tmp/mciplayer-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mciplayer-2.0.0.tar", last modified: Tue Jun 13 08:53:17 2023, max compression
+gzip compressed data, was "mciplayer-2.0.1.tar", last modified: Tue Jun 13 10:09:52 2023, max compression
```

## Comparing `mciplayer-2.0.0.tar` & `mciplayer-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:53:17.617992 mciplayer-2.0.0/
--rw-rw-rw-   0        0        0      930 2023-06-13 08:53:17.617992 mciplayer-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-06-13 08:49:45.000000 mciplayer-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 08:53:17.611108 mciplayer-2.0.0/mciplayer/
--rw-rw-rw-   0        0        0     8256 2023-06-13 08:47:19.000000 mciplayer-2.0.0/mciplayer/__init__.py
--rw-rw-rw-   0        0        0      856 2023-06-13 08:44:46.000000 mciplayer-2.0.0/mciplayer/tool.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:53:17.614486 mciplayer-2.0.0/mciplayer.egg-info/
--rw-rw-rw-   0        0        0      930 2023-06-13 08:53:17.000000 mciplayer-2.0.0/mciplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-13 08:53:17.000000 mciplayer-2.0.0/mciplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 08:53:17.000000 mciplayer-2.0.0/mciplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-13 08:53:17.000000 mciplayer-2.0.0/mciplayer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 08:53:17.000000 mciplayer-2.0.0/mciplayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5177 2023-06-06 09:39:12.000000 mciplayer-2.0.0/py_mciwnd.cpp
--rw-rw-rw-   0        0        0     5745 2023-06-13 08:50:24.000000 mciplayer-2.0.0/py_mciwnd_unicode.cpp
--rw-rw-rw-   0        0        0       42 2023-06-13 08:53:17.617992 mciplayer-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-06-13 08:53:04.000000 mciplayer-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:09:52.376503 mciplayer-2.0.1/
+-rw-rw-rw-   0        0        0      930 2023-06-13 10:09:52.375021 mciplayer-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-06-13 08:49:45.000000 mciplayer-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 10:09:52.368810 mciplayer-2.0.1/mciplayer/
+-rw-rw-rw-   0        0        0     8256 2023-06-13 08:47:19.000000 mciplayer-2.0.1/mciplayer/__init__.py
+-rw-rw-rw-   0        0        0      856 2023-06-13 08:44:46.000000 mciplayer-2.0.1/mciplayer/tool.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:09:52.375021 mciplayer-2.0.1/mciplayer.egg-info/
+-rw-rw-rw-   0        0        0      930 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5112 2023-06-13 10:07:23.000000 mciplayer-2.0.1/py_mciwnd.cpp
+-rw-rw-rw-   0        0        0     5676 2023-06-13 10:07:42.000000 mciplayer-2.0.1/py_mciwnd_unicode.cpp
+-rw-rw-rw-   0        0        0       42 2023-06-13 10:09:52.377506 mciplayer-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-06-13 10:08:38.000000 mciplayer-2.0.1/setup.py
```

### Comparing `mciplayer-2.0.0/PKG-INFO` & `mciplayer-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mciplayer
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple audio player/recorder using MCI
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package should be built AND installed in Windows
```

### Comparing `mciplayer-2.0.0/README.md` & `mciplayer-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mciplayer-2.0.0/mciplayer/__init__.py` & `mciplayer-2.0.1/mciplayer/__init__.py`

 * *Files identical despite different names*

### Comparing `mciplayer-2.0.0/mciplayer/tool.py` & `mciplayer-2.0.1/mciplayer/tool.py`

 * *Files identical despite different names*

### Comparing `mciplayer-2.0.0/mciplayer.egg-info/PKG-INFO` & `mciplayer-2.0.1/mciplayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mciplayer
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple audio player/recorder using MCI
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package should be built AND installed in Windows
```

### Comparing `mciplayer-2.0.0/py_mciwnd.cpp` & `mciplayer-2.0.1/py_mciwnd.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -118,25 +118,23 @@
     m.def("MCIWndGetEnd", &mwge);
     m.def("MCIWndGetPosition", &mwgp);
     m.def("MCIWndGetLength", &mwgl);
     m.def("MCIWndHome", &mwh);
     m.def("MCIWndEnd", &mwe);
     m.def("MCIWndRecord", &mwrc);
     m.def("MCIWndSetSpeed", &mwss);
-    m.def("MCIWndEnd", &mwe);
     m.def("MCIWndGetSpeed", &mwgsp);
     m.def("MCIWndCanPlay", &mwcp);
     m.def("MCIWndCanRecord", &mwcr);
     m.def("MCIWndSetVolume", &mwsv);
     m.def("MCIWndGetVolume", &mwgv);
     m.def("MCIWndSave", &mwsvf);
     m.def("MCIWndCanSave", &mwcs);
     m.def("MCIWndSeek", &mwsk);
     m.def("MCIWndOpen", &mwo);
-    m.def("MCIWndCanPlay", &mwcp);
     m.def("MCIWndGetError", &mwer);
     m.def("MCIWndClose", &mwcl);
     m.def("MCIWndNew", &mwn);
     m.def("MCIWndStop", &mwt);
     m.attr("WS_OVERLAPPED") = 0x00000000L;
     m.attr("WS_POPUP") = 0x80000000L;
     m.attr("WS_CHILD") = 0x40000000L;
@@ -169,8 +167,8 @@
     m.attr("MCIWNDF_NOTIFYPOS") = 0x0200;
     m.attr("MCIWNDF_NOTIFYSIZE") = 0x0400;
     m.attr("MCIWNDF_NOTIFYERROR") = 0x1000;
     m.attr("MCIWNDF_NOTIFYALL") = 0x1F00;
     m.attr("MCIWNDF_NOTIFYANSI") = 0x0080;
     m.attr("MCIWNDF_RECORD") = 0x2000;
     m.attr("MCIWNDF_NOERRORDLG") = 0x4000;
-}
+}
```

### Comparing `mciplayer-2.0.0/py_mciwnd_unicode.cpp` & `mciplayer-2.0.1/py_mciwnd_unicode.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -129,25 +129,23 @@
     m.def("uMCIWndGetEnd", &mwge);
     m.def("uMCIWndGetPosition", &mwgp);
     m.def("uMCIWndGetLength", &mwgl);
     m.def("uMCIWndHome", &mwh);
     m.def("uMCIWndEnd", &mwe);
     m.def("uMCIWndRecord", &mwrc);
     m.def("uMCIWndSetSpeed", &mwss);
-    m.def("uMCIWndEnd", &mwe);
     m.def("uMCIWndGetSpeed", &mwgsp);
     m.def("uMCIWndCanPlay", &mwcp);
     m.def("uMCIWndCanRecord", &mwcr);
     m.def("uMCIWndSetVolume", &mwsv);
     m.def("uMCIWndGetVolume", &mwgv);
     m.def("uMCIWndSave", &mwsvf);
     m.def("uMCIWndCanSave", &mwcs);
     m.def("uMCIWndSeek", &mwsk);
     m.def("uMCIWndOpen", &mwo);
-    m.def("uMCIWndCanPlay", &mwcp);
     m.def("uMCIWndGetError", &mwer);
     m.def("uMCIWndClose", &mwcl);
     m.def("uMCIWndNew", &mwn);
     m.def("uMCIWndStop", &mwt);
     m.attr("WS_OVERLAPPED") = 0x00000000L;
     m.attr("WS_POPUP") = 0x80000000L;
     m.attr("WS_CHILD") = 0x40000000L;
```

### Comparing `mciplayer-2.0.0/setup.py` & `mciplayer-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md','r') as file:
         return file.read()
 if platform.system()!='Windows': # Must be a Windows operating system.
     raise OSError("Please build in Windows!")
 else:
     setup(
         name='mciplayer',
-        version='2.0.0',
+        version='2.0.1',
         description='A simple audio player/recorder using MCI',
         long_description_content_type='text/markdown',
         ext_modules=[
             Extension('mciplayer._mciwnd',sources=['py_mciwnd.cpp'],include_dirs=[get_include()],language='c++'),
             Extension('mciplayer._mciwnd_unicode',sources=['py_mciwnd_unicode.cpp'],include_dirs=[get_include()],language='c++')
         ],
         packages=['mciplayer'],long_description=readme(),
```

