# Comparing `tmp/doFolder-0.0.9.tar.gz` & `tmp/doFolder-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doFolder-0.0.9.tar", last modified: Mon Jun  5 04:37:22 2023, max compression
+gzip compressed data, was "doFolder-0.1.0.tar", last modified: Tue Jun 13 12:28:09 2023, max compression
```

## Comparing `doFolder-0.0.9.tar` & `doFolder-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 04:37:22.826742 doFolder-0.0.9/
--rw-rw-rw-   0        0        0     3351 2023-06-05 04:37:22.825742 doFolder-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2624 2023-05-30 18:05:13.000000 doFolder-0.0.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-05 04:37:22.793743 doFolder-0.0.9/doFolder/
--rw-rw-rw-   0        0        0      569 2023-05-31 14:24:09.000000 doFolder-0.0.9/doFolder/__init__.py
--rw-rw-rw-   0        0        0    10823 2023-05-31 14:59:56.000000 doFolder-0.0.9/doFolder/compare.py
--rw-rw-rw-   0        0        0    29519 2023-06-05 04:36:08.000000 doFolder-0.0.9/doFolder/main.py
--rw-rw-rw-   0        0        0    13847 2023-05-31 14:13:25.000000 doFolder-0.0.9/doFolder/terminal.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:37:22.824742 doFolder-0.0.9/doFolder.egg-info/
--rw-rw-rw-   0        0        0     3351 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 04:37:22.000000 doFolder-0.0.9/doFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 04:37:22.826742 doFolder-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-06-05 04:37:16.000000 doFolder-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:28:09.030596 doFolder-0.1.0/
+-rw-rw-rw-   0        0        0     3157 2023-06-13 12:28:09.030596 doFolder-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2430 2023-06-13 12:27:21.000000 doFolder-0.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 12:28:09.012596 doFolder-0.1.0/doFolder/
+-rw-rw-rw-   0        0        0      569 2023-05-31 14:24:09.000000 doFolder-0.1.0/doFolder/__init__.py
+-rw-rw-rw-   0        0        0    10940 2023-06-13 12:20:24.000000 doFolder-0.1.0/doFolder/compare.py
+-rw-rw-rw-   0        0        0    27772 2023-06-13 12:22:36.000000 doFolder-0.1.0/doFolder/main.py
+-rw-rw-rw-   0        0        0    13847 2023-05-31 14:13:25.000000 doFolder-0.1.0/doFolder/terminal.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:28:09.028595 doFolder-0.1.0/doFolder.egg-info/
+-rw-rw-rw-   0        0        0     3157 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 12:28:09.030596 doFolder-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-06-13 12:23:11.000000 doFolder-0.1.0/setup.py
```

### Comparing `doFolder-0.0.9/PKG-INFO` & `doFolder-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.9
+Version: 0.1.0
 Summary: Manage files more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
@@ -59,21 +59,15 @@
 
 -  ``File`` 指一个文件
 
    -  *参数* ``path`` 文件路径:``str|doFolder.Path``
    -  *方法* ``remove,copy,move`` 文件操作
    -  *属性* ``mode,ino,dev,uid,gid...`` 参见 ``os.stat``
 
--  ``Path`` 指一个路径
-
--  *参数* ``path`` 路径(绝对或相对):``str``
-
-   -  *属性* ``partition`` 将路径(不包含驱动器)切片
-   -  *方法* ``add`` 将内容加载路径后面
-   -  *方法* ``findRest`` 去除两个路径的共同部分
+-  ``Path`` 指一个路径:来自specialStr的路径 ``(0.0.10之后)``
 
 -  ``compare``\ 提供比较文件夹的API
 
    -  *函数* ``compare`` 比较两个文件夹
 
       -  *参数* ``folder1&folder2`` *比较的文件夹:``Folder``*
       -  *参数* ``compareContent``
```

### Comparing `doFolder-0.0.9/README.rst` & `doFolder-0.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -38,21 +38,15 @@
 
 -  ``File`` 指一个文件
 
    -  *参数* ``path`` 文件路径:``str|doFolder.Path``
    -  *方法* ``remove,copy,move`` 文件操作
    -  *属性* ``mode,ino,dev,uid,gid...`` 参见 ``os.stat``
 
--  ``Path`` 指一个路径
-
--  *参数* ``path`` 路径(绝对或相对):``str``
-
-   -  *属性* ``partition`` 将路径(不包含驱动器)切片
-   -  *方法* ``add`` 将内容加载路径后面
-   -  *方法* ``findRest`` 去除两个路径的共同部分
+-  ``Path`` 指一个路径:来自specialStr的路径 ``(0.0.10之后)``
 
 -  ``compare``\ 提供比较文件夹的API
 
    -  *函数* ``compare`` 比较两个文件夹
 
       -  *参数* ``folder1&folder2`` *比较的文件夹:``Folder``*
       -  *参数* ``compareContent``
```

### Comparing `doFolder-0.0.9/doFolder/__init__.py` & `doFolder-0.1.0/doFolder/__init__.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.9/doFolder/compare.py` & `doFolder-0.1.0/doFolder/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
 EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
 MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
 See the Mulan PSL v2 for more details.
 """
 import doFolder.main as doFolder
 from typing import Literal,List,Union,Callable,Dict
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import ThreadPoolExecutor,_base
+import time
 class RepeatedExecutionError(Exception):
     def __init__(self,message:str):
         self.message=message
     def __str__(self):
         return self.message
 class FileMissing(doFolder._HasName):
     def __init__(self,file:doFolder.File,root:doFolder.Folder,anotherFolder:doFolder.Folder):
@@ -175,24 +176,27 @@
         }
         if compareContent in ma:
             return ma[compareContent]
         raise ValueError(f"compareContent is not valid. If you want to customize the comparison method, please pass in a comparison function")
     raise ValueError(f"compareContent must be callable or str,but \"{compareContent}\" is given")
 def compare(folder1:doFolder.Folder,folder2:doFolder.Folder,compareContent:unformatedCompareContent="ignore",threaded:bool=False,threads:Union[None,int]=10)->CompareResult:
     threadPool=ThreadPoolExecutor(max_workers=threads) if threaded else None
-    result=_compare(folder1,folder2,folder1,folder2,_normalizedCompareContent(compareContent),threadPool)
-    assert result
-    if threadPool:threadPool.shutdown(wait=True)
+    waitlist:List[_base.Future]=[]
+    result=_compare(folder1,folder2,folder1,folder2,_normalizedCompareContent(compareContent),threadPool,None,waitlist)
+    for i in waitlist:
+        while not i.done():
+            time.sleep(0.1)
     return result
 def _compareFile(result:CompareResult,file1:doFolder.File,file2:doFolder.File,compareContent:formatedCompareContent,root1:doFolder.Folder
             ,root2:doFolder.Folder)->None:
     if not compareContent(file1,file2):
         result.newDifferent(FileDifferent(file1,file2,root1,root2))
 def _compare(folder1:doFolder.Folder,folder2:doFolder.Folder,root1:doFolder.Folder
-            ,root2:doFolder.Folder,compareContent:formatedCompareContent,threadPool:Union[ThreadPoolExecutor,None]=None,parent:Union[CompareResult,None]=None)->Union[CompareResult,None]:
+            ,root2:doFolder.Folder,compareContent:formatedCompareContent,threadPool:Union[ThreadPoolExecutor,None]=None,parent:Union[CompareResult,None]=None,
+            waitlist:List[_base.Future]=[])->CompareResult:
     result=CompareResult(folder1,folder2)
     for file1 in folder1.files:
         file2=folder2.files[file1.name]
         if file2==None:
             result.newDifferent(FileMissing(file1,root1,root2))
         else:
             if threadPool:threadPool.submit(_compareFile,result,file1,file2,compareContent,root1,root2)
@@ -202,18 +206,16 @@
         if file1==None:
             result.newDifferent(FileMissing(file2,root2,root1))
     for subfolder1 in folder1.subfolder:
         subfolder2=folder2.subfolder[subfolder1.name]
         if subfolder2==None:
             result.newDifferent(FolderMissing(subfolder1,root1,root2))
         else:
-            if threadPool:threadPool.submit(_compare,subfolder1,subfolder2,root1,root2,compareContent,threadPool,result)
-            else:_compare(subfolder1,subfolder2,root1,root2,compareContent,threadPool,result)
+            if threadPool:waitlist.append(threadPool.submit(_compare,subfolder1,subfolder2,root1,root2,compareContent,threadPool,result,waitlist))
+            else:_compare(subfolder1,subfolder2,root1,root2,compareContent,threadPool,result,waitlist)
     for subfolder2 in folder2.subfolder:
         subfolder1=folder1.subfolder[subfolder2.name]
         if subfolder1==None:
             result.newDifferent(FolderMissing(subfolder2,root2,root1))
     if parent:
         parent.newDifferent(result)
-        return
-    else:
-        return result
+    return result
```

### Comparing `doFolder-0.0.9/doFolder/main.py` & `doFolder-0.1.0/doFolder/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
 EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
 MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
 See the Mulan PSL v2 for more details.
 """
 import os
 import re
-from typing import Any,Union,Callable,Literal,List,Tuple,Iterable,TypeVar,Generic,IO
+from typing import Any,Union,Callable,Literal,List,Tuple,Iterable,TypeVar,Generic,IO,Dict
 import shutil
 import copy
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler,FileSystemEvent,FileSystemMovedEvent,EVENT_TYPE_CREATED,EVENT_TYPE_DELETED,EVENT_TYPE_MOVED,EVENT_TYPE_MODIFIED
 import hashlib
 import logging
 from concurrent.futures import ThreadPoolExecutor
-
+from specialStr import Path
+import base64
+import json
+from concurrent.futures import ThreadPoolExecutor,_base
+import time
 __all__=["File","Folder","Path"]
 
-pathTester=re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)/(?:[^/\\\*\?]+/?)*$")
-driverFinder=re.compile(r"^((?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+))/(?:[^/\\\*\?]+/?)*$")
-pathFinder=re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)(/(?:[^/\\\*\?]+/?)*)$")
+
 SearchCondition=Union[str,re.Pattern,Callable[[Union["File","Folder"]],bool]]
 FormatedMatching=Tuple[Callable[[Union["File","Folder"]],bool],int,Union[int,None]]
 UnformattedMatching=Union[SearchCondition,Tuple[SearchCondition,int,Union[int,None]]]
 _T=TypeVar("_T",bound="_HasName")
 _U=TypeVar("_U")
 class _HasName(Generic[_T]):
     name: str
@@ -138,82 +140,15 @@
     def __add__(self,var:"FileList"):
         return FileList(self.values+var.values)
 class FolderList(_ObjectListIndexedByName["Folder"]):
     def __init__(self,var:Iterable["Folder"]=[]):
         super().__init__(var)
     def __add__(self,var:"FolderList"):
         return FolderList(self.values+var.values)
-class Path(str):
-    """
-    ## Represents a path. It can be used as same as a str, but it has more function about path.
-    Attributes:
-        - driver (str): The drive letter of the path.
-        - path (str): The directory and file name of the path.
-    ## Methods:
-        - partition() -> List[str]: Split the path into list.
-        - name() -> str: Return the name of the file or folder that this path points to.
-        - add(value:str) -> "Path": Add another dir name after the current path and return a new Path object.
-        - adds(value:List[str]) -> "Path": Add multiple dir names after the current path and return a new Path object.
-        - findRest(other:"Path",error:Literal["strict","ignore"]="strict"): Find the same ancestor node between two paths. If error is set to "strict" (default), raise ValueError if other is not exactly parent directory of self. Otherwise, return remaining directories in self's partition after finding different ancestor with other's partition.
-    """
-    def __new__(cls, value):
-        var=str(value)
-        if var.startswith("."):
-            var=os.path.abspath(var)
-        var=var.replace("\\","/")
-        if pathTester.match(var)==None:
-            raise ValueError(f"\"{var}\" does not appear to be a legal path")
-        return super().__new__(cls, var)
-    def __init__(self, value):
-        super().__init__()
-        self.driver:str=driverFinder.findall(self)[0]
-        self.path:str=pathFinder.findall(self)[0]
-    @property
-    def partition(self)->List[str]:
-        """split the path into list"""
-        li=self.path.split("/")
-        while "" in li:
-            li.remove("")
-        return li
-    @property
-    def name(self)->str:
-        """The name of the path points to"""
-        return self.partition[-1] if len(self.partition) else self.driver+"/"
-    def add(self, value:str):
-        """add another dir name after the path"""
-        if self[-1]!="/":
-            return Path(self+"/"+value)
-        return Path(self+value)
-    def adds(self, value:List[str])->"Path":
-        new=copy.deepcopy(self)
-        for i in value:
-            new=new.add(i)
-        return new
-    def findRest(self,other:"Path",error:Literal["strict","ignore"]="strict"):
-        """Find the same ancestor node of them
-        :param error:"strict" means if other path not exactly the parent directory of this path, raise ValueError.
-        """
-        if error=="strict" and self.driver!=other.driver:
-            raise ValueError(f"\"{self}\" and \"{other}\" has different driver")
-        retsult=copy.deepcopy(self.partition)
-        for i in other.partition:
-            if not len(retsult) or retsult[0]!=i:
-                if error=="strict":
-                    raise ValueError(f"\"{other}\" is not the ancestor folder of {self}")
-                return retsult
-            del retsult[0]
-        return retsult
-    def getAbsolutePath(self,path)->"Path":
-        """
-        Returns the absolute path of a given file or directory by joining it with the current working directory.
-        :param path: A string representing the relative path to be joined with the current working directory.
-        :return: An object of type "Path" representing the absolute path obtained after joining.
-        :raise ValueError: If input argument 'path' is not a valid string.
-        """
-        return Path(os.path.join(self, path))
+
 class File(_HasName):
     """
     Represents a file on disk.
     ## Attributes:
         - path (Path): The path of the file.
         - parent (Folder or None): The parent folder of the file.
         - mode (int): The mode of the file.
@@ -543,19 +478,23 @@
         re.Pattern[str]: match the files whose name matches the regular expression\n
         Callable[[Union["File","Folder"]],bool]: Returns a match based on the folder or file object\n
         Tuple[str | re.Pattern[str]| Callable ,int,int|None] the condition , the Minimum repetition , Maximum repetition("None" indicates that there is no limit)
         :param aim: search type
         """
         self.logger.debug(f"Searching objects in folder.{condition}")
         threadPool=ThreadPoolExecutor(max_workers=threads) if threaded else None
+        waitlist:List[_base.Future]=[]
         retsult:SearchResult=SearchResult()
-        self._match([_formatMatching(i) for i in condition],retsult,aim=aim,pool=threadPool)
-        if threadPool:threadPool.shutdown(wait=True)
+        
+        self._match([_formatMatching(i) for i in condition],retsult,aim=aim,pool=threadPool,waitlist=waitlist)
+        for i in waitlist:
+            while not i.done():
+                time.sleep(0.1)
         return retsult
-    def _match(self,condition:List[FormatedMatching],retsult:SearchResult,aim:Literal["file","folder","both"]="both",pool:Union[ThreadPoolExecutor,None]=None)->None:
+    def _match(self,condition:List[FormatedMatching],retsult:SearchResult,aim:Literal["file","folder","both"]="both",pool:Union[ThreadPoolExecutor,None]=None,waitlist:List[_base.Future]=[])->None:
         """
         This is the ultimate implementation of the search behavior, but if your criteria are not formatted, consider starting with the "search" function, which will format the criteria and complete the search for you
         :param condition: search conditions which is formatted
         :param aim: search type
         """
         for i in range(len(condition)):
             if aim!="folder":
@@ -571,15 +510,15 @@
                     if (k==len(restCondition)):
                         retsult.append(j)
             for j in self.subfolder:
                 if not condition[i][0](j):continue
                 restCondition=copy.deepcopy(condition)
                 restCondition[0]=(restCondition[0][0],max(restCondition[0][1]-1,0),None if restCondition[0][2]==None else max(restCondition[0][2]-1,0))
                 if restCondition[0][2]!=None and restCondition[0][2]<=0:del restCondition[0]
-                if pool:pool.submit(j._match,restCondition,retsult,aim,pool)
+                if pool:waitlist.append(pool.submit(j._match,restCondition,retsult,aim,pool))
                 else:j._match(restCondition,retsult,aim,pool)
                 if aim=="file":continue
                 k=i
                 while k<len(restCondition):
                     if restCondition[k][1]!=0:
                         break
                     k+=1
@@ -615,8 +554,48 @@
         os.makedirs(path)
         return path
     def add(self,aim:Union["File","Folder"],move:bool=False):
         "add a file or folder to this folder"
         if move:
             aim.move(self.path)
         else:
-            aim.copy(self.path)
+            aim.copy(self.path)
+    def _normalizedToDictIncludeFiles(self,includeFiles:Union[Literal["info","base64","bytes","keep"],Callable[[File],Any]])->Callable[[File],Any]:
+        if callable(includeFiles):
+            return includeFiles
+        ma:Dict[str,Callable[[File],Any]]={
+            "base64":lambda x:{
+                "name":x.name,
+                "base64":base64.b64encode(x.content).decode(),    
+            },
+            "info":lambda x:{
+                "name":x.name,
+                "size":x.size,
+                "dev":x.dev,
+                "uid":x.uid,
+                "gid":x.gid,
+                "ctime":x.ctime,
+                "atime":x.atime,
+                "mtime":x.mtime,
+                "ino":x.ino,
+                "mode":x.mode
+            },
+            "bytes":lambda x:{
+                "name":x.name,
+                "bytes":x.content
+            },
+            "keep":lambda x:x
+        }
+        if includeFiles in ma:
+            return ma[includeFiles]
+        raise ValueError(f"Invalid value for includeFiles: {includeFiles}")
+    def toDict(self,includeFiles:Union[Literal["ignore","info","base64","bytes","keep"],Callable[[File],Any]]="keep")->Dict[str,Any]:
+        result={}
+        result["type"]="Folder"
+        result["name"]=self.name
+        if includeFiles!="ignore":
+            includeFiles=self._normalizedToDictIncludeFiles(includeFiles)
+            result["files"]=[includeFiles(i) for i in self.files]
+        result["subfolder"]={i.name:i.toDict(includeFiles) for i in self.subfolder}
+        return result
+    def toJson(self,**kw)->str:
+        return json.dumps(self.toDict("base64"),**kw)
```

### Comparing `doFolder-0.0.9/doFolder/terminal.py` & `doFolder-0.1.0/doFolder/terminal.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.9/doFolder.egg-info/PKG-INFO` & `doFolder-0.1.0/doFolder.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.9
+Version: 0.1.0
 Summary: Manage files more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
@@ -59,21 +59,15 @@
 
 -  ``File`` 指一个文件
 
    -  *参数* ``path`` 文件路径:``str|doFolder.Path``
    -  *方法* ``remove,copy,move`` 文件操作
    -  *属性* ``mode,ino,dev,uid,gid...`` 参见 ``os.stat``
 
--  ``Path`` 指一个路径
-
--  *参数* ``path`` 路径(绝对或相对):``str``
-
-   -  *属性* ``partition`` 将路径(不包含驱动器)切片
-   -  *方法* ``add`` 将内容加载路径后面
-   -  *方法* ``findRest`` 去除两个路径的共同部分
+-  ``Path`` 指一个路径:来自specialStr的路径 ``(0.0.10之后)``
 
 -  ``compare``\ 提供比较文件夹的API
 
    -  *函数* ``compare`` 比较两个文件夹
 
       -  *参数* ``folder1&folder2`` *比较的文件夹:``Folder``*
       -  *参数* ``compareContent``
```

### Comparing `doFolder-0.0.9/setup.py` & `doFolder-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'doFolder',
-    version = '0.0.9',
+    version = '0.1.0',
     keywords = ['file',"foler","path","filesystem"],
     description = 'Manage files more easily',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
         'watchdog',
         "rich",
+        "specialStr"
     ],
     packages = ['doFolder'],
     
     license = 'Mulan PSL v2',
     platforms=[
         "windows",
         "linux",
```

