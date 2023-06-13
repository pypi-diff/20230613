# Comparing `tmp/seatable-api-2.6.4.tar.gz` & `tmp/seatable-api-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatable-api-2.6.4.tar", last modified: Mon Mar  6 08:09:16 2023, max compression
+gzip compressed data, was "seatable-api-2.6.5.tar", last modified: Tue Jun 13 02:51:00 2023, max compression
```

## Comparing `seatable-api-2.6.4.tar` & `seatable-api-2.6.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-03-06 08:09:16.954519 seatable-api-2.6.4/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    11357 2023-01-04 02:34:58.000000 seatable-api-2.6.4/LICENSE
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-03-06 08:09:16.954238 seatable-api-2.6.4/PKG-INFO
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      300 2023-01-04 02:34:58.000000 seatable-api-2.6.4/README.md
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-03-06 08:09:16.947689 seatable-api-2.6.4/seatable_api/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      171 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/__init__.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    11418 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/column.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     1135 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/constants.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     1108 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/context.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    29097 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/convert_airtable.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    13988 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/date_utils.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      119 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/exception.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    38780 2023-03-06 07:54:22.000000 seatable-api-2.6.4/seatable_api/main.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     2876 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/message.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     9400 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/query.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     2744 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/socket_io.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     6424 2023-01-04 02:34:58.000000 seatable-api-2.6.4/seatable_api/utils.py
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-03-06 08:09:16.951397 seatable-api-2.6.4/seatable_api.egg-info/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-03-06 08:09:16.000000 seatable-api-2.6.4/seatable_api.egg-info/PKG-INFO
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      546 2023-03-06 08:09:16.000000 seatable-api-2.6.4/seatable_api.egg-info/SOURCES.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)        1 2023-03-06 08:09:16.000000 seatable-api-2.6.4/seatable_api.egg-info/dependency_links.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       47 2023-03-06 08:09:16.000000 seatable-api-2.6.4/seatable_api.egg-info/requires.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       19 2023-03-06 08:09:16.000000 seatable-api-2.6.4/seatable_api.egg-info/top_level.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       38 2023-03-06 08:09:16.954631 seatable-api-2.6.4/setup.cfg
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      723 2023-03-06 08:08:26.000000 seatable-api-2.6.4/setup.py
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-03-06 08:09:16.952352 seatable-api-2.6.4/tests/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)        0 2023-01-04 02:34:58.000000 seatable-api-2.6.4/tests/__init__.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     5261 2023-01-04 02:34:58.000000 seatable-api-2.6.4/tests/dateutils_test.py
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:51:00.398452 seatable-api-2.6.5/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    11357 2023-01-04 02:34:58.000000 seatable-api-2.6.5/LICENSE
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-06-13 02:51:00.397685 seatable-api-2.6.5/PKG-INFO
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      300 2023-01-04 02:34:58.000000 seatable-api-2.6.5/README.md
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:51:00.377592 seatable-api-2.6.5/seatable_api/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      171 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/__init__.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    11418 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/column.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     1135 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/constants.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     1108 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/context.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    29097 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/convert_airtable.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    13988 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/date_utils.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      119 2023-04-03 02:56:24.000000 seatable-api-2.6.5/seatable_api/exception.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    42359 2023-05-24 08:00:54.000000 seatable-api-2.6.5/seatable_api/main.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     2876 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/message.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     9400 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/query.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     2744 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/socket_io.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     6424 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/utils.py
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:51:00.391618 seatable-api-2.6.5/seatable_api.egg-info/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/PKG-INFO
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      546 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/SOURCES.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)        1 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/dependency_links.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)       47 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/requires.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)       19 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/top_level.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)       38 2023-06-13 02:51:00.402124 seatable-api-2.6.5/setup.cfg
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      723 2023-06-13 02:50:41.000000 seatable-api-2.6.5/setup.py
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:51:00.394290 seatable-api-2.6.5/tests/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:45:17.000000 seatable-api-2.6.5/tests/__init__.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     5261 2023-06-13 02:45:20.000000 seatable-api-2.6.5/tests/dateutils_test.py
```

### Comparing `seatable-api-2.6.4/LICENSE` & `seatable-api-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/PKG-INFO` & `seatable-api-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.4
+Version: 2.6.5
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `seatable-api-2.6.4/seatable_api/column.py` & `seatable-api-2.6.5/seatable_api/column.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/seatable_api/constants.py` & `seatable-api-2.6.5/seatable_api/constants.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/seatable_api/context.py` & `seatable-api-2.6.5/seatable_api/context.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/seatable_api/convert_airtable.py` & `seatable-api-2.6.5/seatable_api/convert_airtable.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/seatable_api/date_utils.py` & `seatable-api-2.6.5/seatable_api/date_utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/seatable_api/main.py` & `seatable-api-2.6.5/seatable_api/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,14 +143,26 @@
         return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/links/'
 
     def _batch_update_row_link_server_url(self):
         return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/batch-update-links/'
 
     def _app_download_link_url(self):
         return self.server_url + '/api/v2.1/dtable/app-download-link/'
+    
+    def _app_custom_download_link_url(self):
+        return self.server_url + '/api/v2.1/dtable/custom/app-download-link/'
+
+    def _app_custom_asset_file_url(self):
+        return self.server_url + '/api/v2.1/dtable/custom/app-asset-file/'
+
+    def _app_custom_asset_dir_url(self):
+        return self.server_url + '/api/v2.1/dtable/custom/app-asset-dir/'
+
+    def _app_custom_upload_link_url(self):
+        return self.server_url + '/api/v2.1/dtable/custom/app-upload-link/'
 
     def _app_upload_link_url(self):
         return self.server_url + '/api/v2.1/dtable/app-upload-link/'
 
     def _column_server_url(self):
         return self.dtable_server_url + '/api/v1/dtables/' + self.dtable_uuid + '/columns/'
 
@@ -504,16 +516,16 @@
             json_data['other_table_id'] = other_table_name
         response = requests.delete(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
     def update_link(self, link_id, table_name, other_table_name, row_id, other_rows_ids):
         """
         :param link_id: str
-        :param table_id: str
-        :param other_table_id: str
+        :param table_name: str
+        :param other_table_name: str
         :param row_id: str
         :param other_rows_ids: list
         """
         if not isinstance(other_rows_ids, list):
             raise ValueError('params other_rows_ids requires type list')
         url = self._row_link_server_url()
         json_data = {
@@ -529,16 +541,16 @@
             json_data['other_table_id'] = other_table_name
         response = requests.put(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
     def batch_update_links(self, link_id, table_name, other_table_name, row_id_list, other_rows_ids_map):
         """
         :param link_id: str
-        :param table_id: str
-        :param other_table_id: str
+        :param table_name: str
+        :param other_table_name: str
         :param row_id_list: []
         :param other_rows_ids_map: dict
         """
         url = self._batch_update_row_link_server_url()
         json_data = {
             'link_id': link_id,
             'table_name': table_name,
@@ -951,14 +963,95 @@
             'table_name': table_name,
             'rows': rows_data,
         }
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
         return parse_response(response)
 
 
+    ####   custom assets ######
+    def get_custom_file_download_link(self, path):
+        """
+        :param path: str
+        :return: str
+        """
+        url = self._app_custom_download_link_url()
+        params = {'path': path}
+        headers = parse_headers(self.token)
+        response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
+        data = parse_response(response)
+        return data.get('download_link')
+
+    def get_custom_file_upload_link(self, path):
+        url = self._app_custom_upload_link_url()
+        params = {'path': path}
+        headers = parse_headers(self.token)
+        response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
+        data = parse_response(response)
+        return data
+
+
+    def download_custom_file(self, path, save_path):
+        download_link = self.get_custom_file_download_link(parse.unquote(path))
+        response = requests.get(download_link, timeout=self.timeout)
+        if response.status_code != 200:
+            raise Exception('download file error')
+        with open(save_path, 'wb') as f:
+            f.write(response.content)
+
+    def upload_local_file_to_custom_folder(self, local_path, custom_folder_path = None, name=None, ):
+        if not name:
+            name = local_path.strip('/').split('/')[-1]
+        if not custom_folder_path:
+            custom_folder_path = '/'
+
+        upload_link_dict = self.get_custom_file_upload_link(parse.unquote(custom_folder_path))
+        upload_link = upload_link_dict.get('upload_link') + '?ret-json=1'
+        parent_path = upload_link_dict.get('parent_path')
+        relative_path = upload_link_dict.get('relative_path')
+
+        response = requests.post(upload_link, data={
+            'parent_dir': parent_path,
+            'relative_path': relative_path,
+            'replace': 0
+        }, files={
+            'file': (name, open(local_path, 'rb'))
+        }, timeout=self.timeout)
+        d = response.json()[0]
+
+        file_name = d.get('name')
+        return self.get_custom_file_info(custom_folder_path, file_name)
+
+
+    def get_custom_file_info(self, path, name):
+        url = self._app_custom_asset_file_url()
+        params = {'path': path, 'name': name}
+        headers = parse_headers(self.token)
+        response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
+        data = parse_response(response)
+        d = data['dirent']
+        file_name = d.get('obj_name')
+        file_name_ext = file_name.split('.')[-1]
+        asset_uuid = d.get('uuid')
+
+        return {
+            'type': 'file',
+            'size': d.get('file_size'),
+            'name': d.get('obj_name'),
+            'url': 'custom-asset://%s.%s' % (asset_uuid, file_name_ext)
+        }
+
+    def list_custom_assets(self, path):
+        url = self._app_custom_asset_dir_url()
+        params = {'path': path}
+        headers = parse_headers(self.token)
+        response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
+        data = parse_response(response)
+        return data
+
+
 
 class Account(object):
     def __init__(self, login_name, password, server_url):
         self.login_name = login_name
         self.username = None
         self.password = password
         self.server_url = server_url.strip().strip('/')
```

### Comparing `seatable-api-2.6.4/seatable_api/message.py` & `seatable-api-2.6.5/seatable_api/message.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/seatable_api/query.py` & `seatable-api-2.6.5/seatable_api/query.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/seatable_api/socket_io.py` & `seatable-api-2.6.5/seatable_api/socket_io.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/seatable_api/utils.py` & `seatable-api-2.6.5/seatable_api/utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/seatable_api.egg-info/PKG-INFO` & `seatable-api-2.6.5/seatable_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.4
+Version: 2.6.5
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `seatable-api-2.6.4/seatable_api.egg-info/SOURCES.txt` & `seatable-api-2.6.5/seatable_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.4/setup.py` & `seatable-api-2.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '2.6.4'
+__version__ = '2.6.5'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='seatable-api',
     version=__version__,
```

### Comparing `seatable-api-2.6.4/tests/dateutils_test.py` & `seatable-api-2.6.5/tests/dateutils_test.py`

 * *Files identical despite different names*

