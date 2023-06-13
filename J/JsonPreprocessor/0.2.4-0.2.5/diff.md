# Comparing `tmp/JsonPreprocessor-0.2.4.tar.gz` & `tmp/JsonPreprocessor-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonPreprocessor-0.2.4.tar", last modified: Thu Jun  8 14:01:42 2023, max compression
+gzip compressed data, was "JsonPreprocessor-0.2.5.tar", last modified: Tue Jun 13 14:59:16 2023, max compression
```

## Comparing `JsonPreprocessor-0.2.4.tar` & `JsonPreprocessor-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:01:42.327988 JsonPreprocessor-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:01:42.323988 JsonPreprocessor-0.2.4/JsonPreprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)    28767 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/JsonPreprocessor/CJsonPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)   220463 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor/JsonPreprocessor.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/JsonPreprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/JsonPreprocessor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:01:42.323988 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-08 14:01:42.327988 JsonPreprocessor-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:01:42.327988 JsonPreprocessor-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:16.157292 JsonPreprocessor-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:16.153292 JsonPreprocessor-0.2.5/JsonPreprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)    29050 2023-06-13 14:57:09.000000 JsonPreprocessor-0.2.5/JsonPreprocessor/CJsonPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220472 2023-06-13 14:59:15.000000 JsonPreprocessor-0.2.5/JsonPreprocessor/JsonPreprocessor.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-13 14:57:09.000000 JsonPreprocessor-0.2.5/JsonPreprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-13 14:57:09.000000 JsonPreprocessor-0.2.5/JsonPreprocessor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:16.153292 JsonPreprocessor-0.2.5/JsonPreprocessor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-13 14:59:16.000000 JsonPreprocessor-0.2.5/JsonPreprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 14:59:16.000000 JsonPreprocessor-0.2.5/JsonPreprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:59:16.000000 JsonPreprocessor-0.2.5/JsonPreprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 14:59:16.000000 JsonPreprocessor-0.2.5/JsonPreprocessor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-13 14:57:09.000000 JsonPreprocessor-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-13 14:59:16.157292 JsonPreprocessor-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-13 14:57:09.000000 JsonPreprocessor-0.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:59:16.157292 JsonPreprocessor-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-13 14:57:09.000000 JsonPreprocessor-0.2.5/setup.py
```

### Comparing `JsonPreprocessor-0.2.4/JsonPreprocessor/CJsonPreprocessor.py` & `JsonPreprocessor-0.2.5/JsonPreprocessor/CJsonPreprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -671,32 +671,37 @@
 
         sJsonDataUpdated = ""
         for line in sJsonData.splitlines():
             if line == '' or line.isspace():
                 continue
             if re.search("\${.+}", line):
                 items = re.split("\s*:\s*", line)
+                newLine = ""
                 if len(items) > 1:
                     if re.match("^\s*\${.+", items[0]):
                         items[0] = '"' + items[0].strip() + '"'
+                        newLine = items[0] + ": "
+                        items.pop(0)
                 else:
                     items[0] = items[0].strip()
-                newLine = ""
                 i=0
                 for item in items:
                     i+=1
-                    subItems = re.split("\s*,\s*", item)
                     newSubItem = ""
-                    j=0
-                    for subItem in subItems:
-                        j+=1
-                        if j<len(subItems):
-                            newSubItem = newSubItem + self.__checkAndUpdateKeyValue(subItem) + ", "
-                        else:
-                            newSubItem = newSubItem + self.__checkAndUpdateKeyValue(subItem)
+                    if re.search("\s*\[[^\[\]]*\]\s*,*\s*", item):
+                        subItems = re.split("\s*,\s*", item)
+                        j=0
+                        for subItem in subItems:
+                            j+=1
+                            if j<len(subItems):
+                                newSubItem = newSubItem + self.__checkAndUpdateKeyValue(subItem) + ","
+                            else:
+                                newSubItem = newSubItem + self.__checkAndUpdateKeyValue(subItem)
+                    else:
+                        newSubItem = self.__checkAndUpdateKeyValue(item)
                     if i<len(items):
                         newLine = newLine + newSubItem + " : "
                     else:
                         newLine = newLine + newSubItem
                 for nestedParam in self.lNestedParams:
                     tmpNestedParam = nestedParam.replace("$", "\$")
                     tmpNestedParam = tmpNestedParam.replace("[", "\[")
@@ -716,15 +721,15 @@
             if self.syntax == CSyntaxType.python:
                 CJSONDecoder = CPythonJSONDecoder
             else:
                 raise Exception(f"Provided syntax '{self.syntax}' is not supported.")
 
         try:
             oJson = json.loads(sJsonDataUpdated, 
-                               cls=CJSONDecoder , 
+                               cls=CJSONDecoder, 
                                object_pairs_hook=self.__processImportFiles)
         except Exception as error:
             raise Exception(f"json file '{jFile}': '{error}'")
 
         oJson = __handleStrNoneTrueFalse(oJson)        
         os.chdir(currentDir)
```

### Comparing `JsonPreprocessor-0.2.4/JsonPreprocessor/JsonPreprocessor.pdf` & `JsonPreprocessor-0.2.5/JsonPreprocessor/JsonPreprocessor.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 10% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 JsonPreprocessor
-v. 0.2.4
+v. 0.2.5
 Mai Dinh Nam Son
-08.06.2023
+13.06.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -602,19 +602,19 @@
 
 Name
 
 JsonPreprocessor
 
 Version
 
-0.2.4
+0.2.5
 
 Date
 
-08.06.2023
+13.06.2023
 
 Description
 
 Preprocessor for json files
 
 Package URL
 
@@ -681,13 +681,13 @@
 0.2.4
 
 06/2023
 
 Improved dotdict format and update log output
 
 JsonPreprocessor.pdf
-Created at 08.06.2023 - 14:01:39
+Created at 13.06.2023 - 14:59:13
 by GenPackageDoc v. 0.40.3
 
 11
```

### Comparing `JsonPreprocessor-0.2.4/JsonPreprocessor/__init__.py` & `JsonPreprocessor-0.2.5/JsonPreprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.2.4/JsonPreprocessor/version.py` & `JsonPreprocessor-0.2.5/JsonPreprocessor/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of JsonPreprocessor
 #
-VERSION      = "0.2.4"
-VERSION_DATE = "08.06.2023"
+VERSION      = "0.2.5"
+VERSION_DATE = "13.06.2023"
```

### Comparing `JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/PKG-INFO` & `JsonPreprocessor-0.2.5/JsonPreprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.2.4
+Version: 0.2.5
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.2.4/LICENSE` & `JsonPreprocessor-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.2.4/PKG-INFO` & `JsonPreprocessor-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.2.4
+Version: 0.2.5
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.2.4/README.rst` & `JsonPreprocessor-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.2.4/setup.py` & `JsonPreprocessor-0.2.5/setup.py`

 * *Files identical despite different names*

