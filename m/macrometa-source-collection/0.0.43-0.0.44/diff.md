# Comparing `tmp/macrometa-source-collection-0.0.43.tar.gz` & `tmp/macrometa-source-collection-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.43.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.44.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.43.tar` & `macrometa-source-collection-0.0.44.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9533 2023-06-12 17:15:41.145646 macrometa-source-collection-0.0.43/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     9087 2023-06-12 17:15:41.145646 macrometa-source-collection-0.0.43/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-12 17:15:41.437644 macrometa-source-collection-0.0.43/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.43/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.43/PKG-INFO
+-rw-r--r--   0        0        0     9500 2023-06-13 05:27:53.052663 macrometa-source-collection-0.0.44/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     9355 2023-06-13 05:27:53.052663 macrometa-source-collection-0.0.44/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-13 05:27:53.308670 macrometa-source-collection-0.0.44/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.44/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.44/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.43/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.44/macrometa_source_collection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,14 @@
 def main_impl():
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     conn_config = {'api_key': args.config['api_key'],
                    'gdn_host': extract_gdn_host(args.config['gdn_host']),
                    'fabric': args.config['fabric'],
                    'source_collection': args.config['source_collection']}
 
-    LOGGER.info("Testing 123..")
     if args.discover:
         do_discovery(conn_config, workflow_run=True)
     elif args.catalog:
         do_sync(conn_config, args.catalog, args.config.get('default_replication_method'))
     else:
         LOGGER.info("No properties were selected")
     return
```

### Comparing `macrometa-source-collection-0.0.43/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.44/macrometa_source_collection/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,16 @@
                             j[key] is None or (isinstance(schema_properties[key].type, list) and get_singer_data_type(j[key]) in schema_properties[key].type)
                                                  or (isinstance(schema_properties[key].type, str) and get_singer_data_type(j[key]) == schema_properties[key].type)
                             for key in j.keys()
                         ):
                             j['_sdc_deleted_at'] = None
                             singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
                             singer.write_message(singer_record)
+                        else:
+                            LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", j)
                     elif props["op"] == "DELETE":
                         # Currently, we don't have a way to validate schema here
                         j.pop('_delete', None)
                         j['_sdc_deleted_at'] = singer.utils.strftime(utils.now())
                         singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
                         singer.write_message(singer_record)
                     _consumer.acknowledge(msg.message_id())
@@ -140,14 +142,16 @@
                                      or (isinstance(schema_properties[key].type, str) and get_singer_data_type(rec[key]) == schema_properties[key].type)
                 for key in rec.keys()
             ):
                 singer_record = self.msg_to_singer_message(stream, rec, None, utils.now())
                 singer.write_message(singer_record)
                 self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(rec))
                 self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+            else:
+                LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", rec)
 
     def send_schema_message(self, stream: CatalogEntry, bookmark_properties=[]):
         schema_message = singer.SchemaMessage(stream=stream.stream,
                                               schema=stream.schema.to_dict(),
                                               key_properties=stream.key_properties,
                                               bookmark_properties=bookmark_properties)
         singer.write_message(schema_message)
```

### Comparing `macrometa-source-collection-0.0.43/pyproject.toml` & `macrometa-source-collection-0.0.44/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.43'
+version='0.0.44'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.43/setup.py` & `macrometa-source-collection-0.0.44/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.43',
+    'version': '0.0.44',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.43/PKG-INFO` & `macrometa-source-collection-0.0.44/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.43
+Version: 0.0.44
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

