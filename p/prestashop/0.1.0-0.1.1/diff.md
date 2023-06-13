# Comparing `tmp/prestashop-0.1.0-py3-none-any.whl.zip` & `tmp/prestashop-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19960 bytes, number of entries: 10
--rw-r--r--  2.0 unx      105 b- defN 23-Jun-10 10:31 prestashop/__init__.py
--rw-r--r--  2.0 unx    15641 b- defN 23-Jun-12 13:21 prestashop/core.py
+Zip file size: 20600 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-13 13:52 prestashop/__init__.py
+-rw-r--r--  2.0 unx    14548 b- defN 23-Jun-13 18:25 prestashop/core.py
 -rw-r--r--  2.0 unx      660 b- defN 23-Jun-12 13:23 prestashop/exceptions.py
 -rw-r--r--  2.0 unx     3642 b- defN 23-Jun-10 13:45 prestashop/utils.py
--rw-r--r--  2.0 unx      249 b- defN 23-Jun-09 19:09 prestashop/version.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-12 14:03 prestashop-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      740 b- defN 23-Jun-12 14:03 prestashop-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 14:03 prestashop-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-12 14:03 prestashop-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      788 b- defN 23-Jun-12 14:03 prestashop-0.1.0.dist-info/RECORD
-10 files, 57077 bytes uncompressed, 18622 bytes compressed:  67.4%
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-13 18:52 prestashop/version.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3597 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      789 b- defN 23-Jun-13 18:54 prestashop-0.1.1.dist-info/RECORD
+10 files, 58739 bytes uncompressed, 19262 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: prestashop/utils.py
 Comment: 
 
 Filename: prestashop/version.py
 Comment: 
 
-Filename: prestashop-0.1.0.dist-info/LICENSE
+Filename: prestashop-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: prestashop-0.1.0.dist-info/METADATA
+Filename: prestashop-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: prestashop-0.1.0.dist-info/WHEEL
+Filename: prestashop-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: prestashop-0.1.0.dist-info/top_level.txt
+Filename: prestashop-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: prestashop-0.1.0.dist-info/RECORD
+Filename: prestashop-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prestashop/__init__.py

```diff
@@ -1,2 +1,3 @@
 from .core import Prestashop,Format
-from .exceptions import PrestaShopError,PrestaShopAuthenticationError
+from .exceptions import PrestaShopError,PrestaShopAuthenticationError
+from .version import __author__,__version__
```

## prestashop/core.py

```diff
@@ -3,14 +3,15 @@
 """
 Prestashop is a Python library to interact with PrestaShop's Web Service API.
 
 :copyright: (c) 2023 Aymen Jemi
 :copyright: (c) 2023 AISYSNEXT
 :license: GPLv3, see LICENSE for more details
 """
+import os
 from enum import Enum
 import mimetypes
 
 from http.client import HTTPConnection
 from xml.etree import ElementTree
 from xml.parsers.expat import ExpatError
 
@@ -91,16 +92,14 @@
 
     # search the first 3 taxes with 5 in the name 
     import pprint
     recs = api.search('taxes',_filter='[name]=%[5]%',limit='3')
 
     for rec in recs:
         pprint(rec)
-
-
     """
     api_key = ''
     url = ''
     client = None
     debug = False
     lang = None
     data_format = Format.JSON
@@ -308,49 +307,14 @@
             raise PrestaShopError(
                 'HTTP XML response is not parsable : %s. %s' %
                 (e, content[:512])
             )
 
         return parsed_content
     
-    def _get_content_type(self, filename):
-        """Retrieve filename mimetype.
-
-        :param filename: file name.
-        :return: mimetype.
-        """
-        return mimetypes.guess_type(filename)[0] or 'application/octet-stream'
-    
-    def _encode_multipart_formdata(self, files):
-        """Encode files to an http multipart/form-data.
-
-        :param files: a sequence of (type, filename, value)
-            elements for data to be uploaded as files.
-        :return: headers and body.
-        """
-        BOUNDARY = '----------ThIs_Is_tHe_bouNdaRY_$'
-        CRLF = b'\r\n'
-        L = []
-        for (key, filename, value) in files:
-            L.append('--' + BOUNDARY)
-            L.append(
-                'Content-Disposition: form-data; \
-                    name="%s"; filename="%s"' % (key, filename))
-            L.append('Content-Type: %s' % self._get_content_type(filename))
-            L.append('')
-            L.append(value)
-        L.append('--' + BOUNDARY + '--')
-        L.append('')
-        L = map(lambda l: l if isinstance(l, bytes) else l.encode('utf-8'), L)
-        body = CRLF.join(L)
-        headers = {
-            'Content-Type': 'multipart/form-data; boundary=%s' % BOUNDARY
-        }
-        return headers, body
-    
     def search(self,resource,display='full',_filter=None,sort=None,limit=None):
         """search from prestashop with options, for more details check the official doc \n
         https://devdocs.prestashop-project.org/1.7/webservice/tutorials/advanced-use/additional-list-parameters/
 
         Args:
             resource (str): resource to search ( taxes,customers,products ...)
             display (str, optional): display parameter (full | [field1,field2]). Defaults to 'full'.
@@ -359,30 +323,27 @@
             limit (str, optional): limit parameter ('offset,limit' , '9,2' , '5'). Defaults to None.
 
         Returns:
             dict : result of search
         """
         return self._exec(resource=resource,method='GET',display=display,_filter=_filter,sort=sort,limit=limit)
 
-    def read(self,resource:str,_id:str=None,display:str='full',sort:str=None,limit:str=None) -> dict:
-        """get one or more result from prestashop with options .
+    def read(self,resource:str,_id:str,display:str='full') -> dict:
+        """get one result from prestashop with options .
         for more details check the official doc \n
         https://devdocs.prestashop-project.org/1.7/webservice/tutorials/advanced-use/additional-list-parameters/
 
         Args:
             resource (str): resource to search ( taxes,customers,products ...)
             _id (str, optional): the id if you wan one record. Defaults to None.
             display (str, optional): display parameter (full | [field1,field2]). Defaults to 'full'.
-            sort (str, optional): sort parameter ([{fieldname}_{ASC|DESC}] ,[lastname_ASC,id_DESC] ). Defaults to None.
-            limit (str, optional): limit parameter ('offset,limit' , '9,2' , '5'). Defaults to None.
-
         Returns:
             dict : result of get request
         """
-        return self._exec(resource,_id,'GET',display=display,sort=sort,limit=limit)
+        return self._exec(resource,_id,'GET',display=display)
 
     def write(self,resource:str,data:dict):
         """update record from prestashop
 
         Args:
             resource (str): resource to search ( taxes,customers,products ...)
             data (dict): data in dict format (
@@ -422,47 +383,74 @@
             resource_ids = ','.join([str(id) for id in ids])
             resource_ids = '[{}]'.format(resource_ids)
             return self._exec(resource=resource ,ids=resource_ids, method='DELETE' , display=None)
             
         else:
             return self._exec(resource=resource ,ids=ids, method='DELETE' , display=None)
     
-    def create(self,resource:str,data:dict=None,files=None):
+    def create(self,resource:str,data:dict):
         """create record 
 
         Args:
             resource (str): resource to search ( taxes,customers,products ...).
-            files (list[tuple], optional):  a sequence of (type, filename, value). Defaults to None.
-            data (dict, optional): data (dict): data in dict format (
+            data (dict): data in dict format (
                     data = {
                         'tax':{
                             'rate' : 3.000,
                             'active': '1',
                             'name' : {
                                 'language' : {
                                     'attrs' : {'id' : '1'},
                                     'value' : '3% tax'
                                 }
                             }
                         }
                     }
-        ). Defaults to None.
-
-            
-
-        Raises:
-            PrestaShopError: raise when data and files is None.
+        )
 
         Returns:
             dict: record added.
         """
 
-        if files is not None:
-            headers , data = self._encode_multipart_formdata(files)
-            return self._exec(resource=resource, method='POST' , data=data,_headers=headers,display=None)
-        elif data is None:
-            raise PrestaShopError('Undefined data.',404)
+
         data  = {'prestashop' : data}
         _data = dict2xml(data)
         return self._exec(resource=resource,data=_data,method='POST',display=None)
 
+    def create_binary(self,resource:str, file:str,_type:str = 'image'):
+        """create binary record
+
+        Args:
+            resource (str): resource to search ( 'images/products/22' ...).
+            files (str):  a path of file ('image.png', 'image.jpg').
+            _type (str): a type of file (image,pdf ...)
+        """
+
+        params = {}
+
+        if self.lang:
+            params.update({'language' : self.lang})
+        
+        if self.data_format == Format.JSON:
+            params.update({'io_format' : 'JSON' , 'output_format' : 'JSON'})
+    
+
+        _url = '{}{}'.format(self.url,resource)
+        url = self._prepare(_url,params)
+
+
+        if os.path.exists(file):
+
+            _file = {_type : open(file,'rb')}
+        else:
+            raise PrestaShopError('File not found',404)
+
+
+        response = self.client.post(
+            url=url,
+            files=_file
+        )
+
+        if response.status_code == 200:
+            return True
+        return False
```

## prestashop/version.py

```diff
@@ -1,9 +1,3 @@
 # -*- coding: utf-8 -*-
-
-try:
-    from importlib.metadata import PackageNotFoundError,version
-    __version__ = version('prestashop')
-except PackageNotFoundError:
-    __version__ = '0.1.0'
-
-__author__= "Aymen Jemi <jemiaymen@gmail.com> (AISYSNEXT)"
+__version__="0.1.1"
+__author__="Aymen Jemi <jemiaymen@gmail.com> (AISYSNEXT)"
```

## Comparing `prestashop-0.1.0.dist-info/LICENSE` & `prestashop-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `prestashop-0.1.0.dist-info/RECORD` & `prestashop-0.1.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-prestashop/__init__.py,sha256=M_lQrjyVjfMDfndy23ZwQDjOJ_QkyWrtUzFztWnfH5s,105
-prestashop/core.py,sha256=8RTMTXR_HUBgTKn1EBwudKRoFHofPU2Fyv57nZzREcI,15641
+prestashop/__init__.py,sha256=a6LT2Hg7nHgalB_KMPQ-Anch5Eld8tiWfbinewQ3mTQ,149
+prestashop/core.py,sha256=uu1L6xfB0b2WKwgvAJGrGDrV-apmf7emCqsFuIHJFkc,14548
 prestashop/exceptions.py,sha256=eQdfgz7bCB5p9IiNsGEJHnB0ojVA1UQtMKy9yR3qlZ8,660
 prestashop/utils.py,sha256=iQ8MKyhYJH3rjG7-WqCNklHno-eGOEGaH7GkBvhjGng,3642
-prestashop/version.py,sha256=vCC9rBPbBgjzdWtxx6PhHz-i8PZ5txyRakr7duO66F0,249
-prestashop-0.1.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-prestashop-0.1.0.dist-info/METADATA,sha256=DeVlpFllwX28Ogy5XyTTtRLTBNz93SFm6lq_JOnRczs,740
-prestashop-0.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-prestashop-0.1.0.dist-info/top_level.txt,sha256=ERBv-4esnLO-q9c0lGE1TpfzzCT-075zZJAClhwIVbA,11
-prestashop-0.1.0.dist-info/RECORD,,
+prestashop/version.py,sha256=ClOuEjoMIpZZ82BTtd0DYW6sYv_JREqYaoW6qWFSx_Q,102
+prestashop-0.1.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+prestashop-0.1.1.dist-info/METADATA,sha256=KztpQ86_V1j2kGHQvJCj-ghpQyfQ5mTZXzygc40vs6Y,3597
+prestashop-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+prestashop-0.1.1.dist-info/top_level.txt,sha256=ERBv-4esnLO-q9c0lGE1TpfzzCT-075zZJAClhwIVbA,11
+prestashop-0.1.1.dist-info/RECORD,,
```

