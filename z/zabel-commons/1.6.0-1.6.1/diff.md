# Comparing `tmp/zabel_commons-1.6.0-py3-none-any.whl.zip` & `tmp/zabel_commons-1.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20364 bytes, number of entries: 11
+Zip file size: 20359 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      606 b- defN 23-Jan-11 10:03 zabel/commons/__init__.py
 -rw-r--r--  2.0 unx      690 b- defN 23-Jan-11 10:03 zabel/commons/exceptions.py
 -rw-r--r--  2.0 unx    18799 b- defN 23-Mar-27 12:24 zabel/commons/interfaces.py
 -rw-r--r--  2.0 unx     5982 b- defN 23-Jan-11 10:03 zabel/commons/servers.py
 -rw-r--r--  2.0 unx     2777 b- defN 23-Jan-11 10:03 zabel/commons/sessions.py
--rw-r--r--  2.0 unx    11438 b- defN 23-Jan-11 10:03 zabel/commons/utils.py
--rw-r--r--  2.0 unx    14197 b- defN 23-Mar-27 12:25 zabel_commons-1.6.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1870 b- defN 23-Mar-27 12:25 zabel_commons-1.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-27 12:25 zabel_commons-1.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-27 12:25 zabel_commons-1.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      912 b- defN 23-Mar-27 12:25 zabel_commons-1.6.0.dist-info/RECORD
-11 files, 57369 bytes uncompressed, 18820 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx    11430 b- defN 23-Jun-13 12:49 zabel/commons/utils.py
+-rw-r--r--  2.0 unx    14197 b- defN 23-Jun-13 12:53 zabel_commons-1.6.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1870 b- defN 23-Jun-13 12:53 zabel_commons-1.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 12:53 zabel_commons-1.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-13 12:53 zabel_commons-1.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      912 b- defN 23-Jun-13 12:53 zabel_commons-1.6.1.dist-info/RECORD
+11 files, 57361 bytes uncompressed, 18815 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: zabel/commons/sessions.py
 Comment: 
 
 Filename: zabel/commons/utils.py
 Comment: 
 
-Filename: zabel_commons-1.6.0.dist-info/LICENSE.txt
+Filename: zabel_commons-1.6.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: zabel_commons-1.6.0.dist-info/METADATA
+Filename: zabel_commons-1.6.1.dist-info/METADATA
 Comment: 
 
-Filename: zabel_commons-1.6.0.dist-info/WHEEL
+Filename: zabel_commons-1.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: zabel_commons-1.6.0.dist-info/top_level.txt
+Filename: zabel_commons-1.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: zabel_commons-1.6.0.dist-info/RECORD
+Filename: zabel_commons-1.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zabel/commons/utils.py

```diff
@@ -139,15 +139,15 @@
 
 def xml_to_dict(xml: Any) -> Dict[str, Any]:
     """Convert an XML document to a corresponding dictionary.
 
     !!! important
         There should be no `'element text'` tag in the XML document.
     """
-    dct = {xml.tag: [xml_to_dict(x) for x in xml.getchildren()]}
+    dct = {xml.tag: [xml_to_dict(x) for x in list(xml)]}
     dct.update(('@%s' % key, val) for key, val in xml.attrib.items())
     dct['element text'] = xml.text
     return dct
 
 
 def dict_to_xml(dct: Mapping[str, Any]) -> str:
     """Convert a dictionary to a corresponding XML string.
```

## Comparing `zabel_commons-1.6.0.dist-info/LICENSE.txt` & `zabel_commons-1.6.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `zabel_commons-1.6.0.dist-info/METADATA` & `zabel_commons-1.6.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: zabel-commons
-Version: 1.6.0
+Version: 1.6.1
 Summary: The Zabel transverse **commons** library
 Home-page: https://github.com/engie-group/zabel
 Author: Martin Lafaix
 Author-email: martin.lafaix@external.engie.com
 License: Eclipse Public License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
-Requires-Python: >= 3.6.5
+Requires-Python: >= 3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: requests (>=2.28)
+Requires-Dist: requests (>=2.31)
 Provides-Extra: all
 Requires-Dist: bottle (>=0.12.25) ; extra == 'all'
 Provides-Extra: bottle
 Requires-Dist: bottle (>=0.12.25) ; extra == 'bottle'
 
 # zabel-commons
```

## Comparing `zabel_commons-1.6.0.dist-info/RECORD` & `zabel_commons-1.6.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 zabel/commons/__init__.py,sha256=6CYV4COMYL0n4A86gGpnzKkXX3X4jTu8T3MDaPBjDqA,606
 zabel/commons/exceptions.py,sha256=VDzqwznxEZETgejDdV-eTjPdHiAjw1ZqVfqwjigcJ-0,690
 zabel/commons/interfaces.py,sha256=L9PtaVBQDSoK9Haoy8xaPayYwbhIFlBZXAPDTdxlMyI,18799
 zabel/commons/servers.py,sha256=MD3bj67zLWDrp00TN7ivPxd58gBuwbfn8r7xUXpsaN0,5982
 zabel/commons/sessions.py,sha256=OxURUe1bzECWlJO9pQ2SzMxjL4-OsdBd7IEqm-KZr3Q,2777
-zabel/commons/utils.py,sha256=En6cTZyPyOJda9sXJDG2mePQClggd1LmRnz8R_IQAc0,11438
-zabel_commons-1.6.0.dist-info/LICENSE.txt,sha256=jDSfgHZNBkjmRfQe8jdypwyZWgkktSNfc19KPQnfEnw,14197
-zabel_commons-1.6.0.dist-info/METADATA,sha256=yHQcYRxTf5C783UVFI5WpNSH-NJ7lkm17nx7EFIJ8po,1870
-zabel_commons-1.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-zabel_commons-1.6.0.dist-info/top_level.txt,sha256=oVMEeX4nyZlbHDW9DbWu8tqH1vmQZO2Yw8C29D3tToo,6
-zabel_commons-1.6.0.dist-info/RECORD,,
+zabel/commons/utils.py,sha256=wRmwHO1tceQKQeyK0SsBJHw2DalKyJQGeUJ9lbC_Wx4,11430
+zabel_commons-1.6.1.dist-info/LICENSE.txt,sha256=jDSfgHZNBkjmRfQe8jdypwyZWgkktSNfc19KPQnfEnw,14197
+zabel_commons-1.6.1.dist-info/METADATA,sha256=w3UqkwFS5rjZuxn530tRL-96EOU1-UdrRmt8Zr2CsRs,1870
+zabel_commons-1.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+zabel_commons-1.6.1.dist-info/top_level.txt,sha256=oVMEeX4nyZlbHDW9DbWu8tqH1vmQZO2Yw8C29D3tToo,6
+zabel_commons-1.6.1.dist-info/RECORD,,
```

