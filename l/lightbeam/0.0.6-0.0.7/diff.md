# Comparing `tmp/lightbeam-0.0.6-py3-none-any.whl.zip` & `tmp/lightbeam-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 28330 bytes, number of entries: 17
+Zip file size: 30090 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 20:03 lightbeam/__init__.py
--rw-r--r--  2.0 unx     4590 b- defN 23-Apr-07 18:45 lightbeam/__main__.py
--rw-r--r--  2.0 unx    18430 b- defN 23-Apr-07 21:15 lightbeam/api.py
+-rw-r--r--  2.0 unx     4806 b- defN 23-Jun-13 20:45 lightbeam/__main__.py
+-rw-r--r--  2.0 unx    18633 b- defN 23-Jun-13 20:45 lightbeam/api.py
 -rw-r--r--  2.0 unx     8914 b- defN 23-Jan-25 19:00 lightbeam/delete.py
 -rw-r--r--  2.0 unx      672 b- defN 22-Sep-19 14:49 lightbeam/hashlog.py
--rw-r--r--  2.0 unx    10168 b- defN 22-Sep-22 13:34 lightbeam/lightbeam.py
--rw-r--r--  2.0 unx     6329 b- defN 23-Apr-07 18:43 lightbeam/send.py
+-rw-r--r--  2.0 unx    10226 b- defN 23-Jun-13 20:45 lightbeam/lightbeam.py
+-rw-r--r--  2.0 unx    11064 b- defN 23-Jun-13 21:40 lightbeam/send.py
 -rw-r--r--  2.0 unx     1329 b- defN 22-Sep-21 16:31 lightbeam/util.py
 -rw-r--r--  2.0 unx     5888 b- defN 22-Sep-20 13:42 lightbeam/validate.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-28 14:58 lightbeam/resources/__init__.py
--rwxrwxrwx  2.0 unx    11349 b- defN 23-Apr-07 21:17 lightbeam-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    12761 b- defN 23-Apr-07 21:17 lightbeam-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 21:17 lightbeam-0.0.6.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      132 b- defN 23-Apr-07 21:17 lightbeam-0.0.6.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx       54 b- defN 23-Apr-07 21:17 lightbeam-0.0.6.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-07 21:17 lightbeam-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1367 b- defN 23-Apr-07 21:17 lightbeam-0.0.6.dist-info/RECORD
-17 files, 82085 bytes uncompressed, 26092 bytes compressed:  68.2%
+-rwxrwxrwx  2.0 unx    11349 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15234 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      132 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx       54 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1368 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/RECORD
+17 files, 89771 bytes uncompressed, 27852 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -24,29 +24,29 @@
 
 Filename: lightbeam/validate.py
 Comment: 
 
 Filename: lightbeam/resources/__init__.py
 Comment: 
 
-Filename: lightbeam-0.0.6.dist-info/LICENSE
+Filename: lightbeam-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: lightbeam-0.0.6.dist-info/METADATA
+Filename: lightbeam-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: lightbeam-0.0.6.dist-info/WHEEL
+Filename: lightbeam-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: lightbeam-0.0.6.dist-info/dependency_links.txt
+Filename: lightbeam-0.0.7.dist-info/dependency_links.txt
 Comment: 
 
-Filename: lightbeam-0.0.6.dist-info/entry_points.txt
+Filename: lightbeam-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: lightbeam-0.0.6.dist-info/top_level.txt
+Filename: lightbeam-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: lightbeam-0.0.6.dist-info/RECORD
+Filename: lightbeam-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lightbeam/__main__.py

```diff
@@ -71,15 +71,20 @@
         type=str,
         help='only payloads last sent after this timestamp will be processed'
         )
     parser.add_argument("-r", "--resend-status-codes",
         type=str,
         help='only payloads that returned one of these comma-delimited HTTP status codes on last send will be processed'
         )
-    defaults = { "selector":"*", "params": "", "older_than": "", "newer_than": "", "resend_status_codes": "" }
+    parser.add_argument("--results-file",
+        type=str,
+        help='produces a JSON output file with structured information about run results'
+    )
+
+    defaults = { "selector":"*", "params": "", "older_than": "", "newer_than": "", "resend_status_codes": "", "results_file": "" }
     parser.set_defaults(**defaults)
     args, remaining_argv = parser.parse_known_args()
     
     if args.version:
         lb_dir = os.path.dirname(os.path.abspath(__file__))
         version_file = os.path.join(lb_dir, 'VERSION.txt')
         with open(version_file, 'r') as f:
@@ -106,15 +111,16 @@
         logger=logger,
         selector=args.selector,
         params=args.params,
         wipe=args.wipe,
         force=args.force,
         older_than=args.older_than,
         newer_than=args.newer_than,
-        resend_status_codes=args.resend_status_codes
+        resend_status_codes=args.resend_status_codes,
+        results_file=args.results_file
         )
     try:
         logger.info("starting...")
         if args.command=='validate': lb.validator.validate()
         elif args.command=='send': lb.sender.send()
         elif args.command=='validate+send':
             lb.validator.validate()
```

## lightbeam/api.py

```diff
@@ -76,15 +76,15 @@
             self.logger.critical("selector filtering left no endpoints to process; check your selector for typos?")
 
         self.lightbeam.endpoints = selected_endpoints
 
     # Returns a client object with exponential retry and other parameters per configs
     def get_retry_client(self):
         return RetryClient(
-            timeout=aiohttp.ClientTimeout(total=self.lightbeam.config['connection']["timeout"]),
+            timeout=aiohttp.ClientTimeout(sock_connect=self.lightbeam.config['connection']["timeout"]),
             retry_options=ExponentialRetry(
                 attempts=self.lightbeam.config['connection']["num_retries"],
                 factor=self.lightbeam.config['connection']["backoff_factor"],
                 statuses=self.lightbeam.config['connection']["retry_statuses"]
                 ),
             connector=aiohttp.connector.TCPConnector(limit=self.lightbeam.config['connection']["pool_size"])
             )
@@ -150,14 +150,18 @@
                                     verify=self.lightbeam.config["connection"]["verify_ssl"])
             if response.status_code not in [ 200, 201 ]:
                 raise Exception("Dependencies URL returned status {0} ({1})".format(response.status_code, (response.content[:75] + "...") if len(response.content)>75 else response.content))
             data = response.json()
         except Exception as e:
             self.logger.critical("Unable to load dependencies from API... terminating. Check API connectivity. ({0})".format(str(e)))
         
+        # Sort `data` by order (not sorted by default in Ed-Fi 6.1)
+        data = list(filter(lambda x: "Create" in x['operations'], data))
+        data = sorted(data, key=lambda x: x['order'])
+
         ordered_endpoints = []
         for e in data:
             ordered_endpoints.append(e["resource"].replace('/' + self.lightbeam.config["namespace"] + '/', ""))
         return ordered_endpoints
     
     # Loads the Swagger JSON from the Ed-Fi API
     def load_swagger_docs(self):
```

## lightbeam/lightbeam.py

```diff
@@ -38,15 +38,15 @@
         "show_stacktrace": False
     }
     MAX_TASK_QUEUE_SIZE = 1000
     STATUS_UPDATE_WAIT = 5 # seconds
     MAX_STATUS_REASONS_TO_DISPLAY = 10
     DATA_FILE_EXTENSIONS = ['json', 'jsonl', 'ndjson']
     
-    def __init__(self, config_file, logger=None, selector="*", params="", wipe=False, force=False, older_than="", newer_than="", resend_status_codes=""):
+    def __init__(self, config_file, logger=None, selector="*", params="", wipe=False, force=False, older_than="", newer_than="", resend_status_codes="", results_file=""):
         self.config_file = config_file
         self.logger = logger
         self.errors = 0
         self.params = params
         self.force = force
         self.wipe = wipe
         self.older_than=older_than
@@ -54,14 +54,15 @@
         self.resend_status_codes=resend_status_codes
         self.endpoints = []
         self.validator = Validator(self)
         self.sender = Sender(self)
         self.deleter = Deleter(self)
         self.api = EdFiAPI(self)
         self.is_locked = False
+        self.results_file = results_file
 
         # load params and/or env vars for config YAML interpolation
         self.params = json.loads(params) if params else {}
         user_config = self.load_config_file()
         
         self.config = util.merge_dicts(user_config, self.config_defaults)
         if "state_dir" in self.config:
```

## lightbeam/send.py

```diff
@@ -1,49 +1,103 @@
 import os
 import time
+import json
 import asyncio
+import datetime
 
 from lightbeam import util
 from lightbeam import hashlog
 
 
 class Sender:
 
     def __init__(self, lightbeam=None):
         self.lightbeam = lightbeam
         self.lightbeam.reset_counters()
         self.logger = self.lightbeam.logger
         self.hashlog_data = {}
+        self.start_timestamp = datetime.datetime.now()
     
     # Sends all (selected) endpoints
     def send(self):
+
+        # Initialize a dictionary for tracking run metadata (for structured output)
+        self.metadata = {
+            "started_at": self.start_timestamp.isoformat(timespec='microseconds'),
+            "working_dir": os.getcwd(),
+            "config_file": self.lightbeam.config_file,
+            "data_dir": self.lightbeam.config["data_dir"],
+            "api_url": self.lightbeam.config["edfi_api"]["base_url"],
+            "namespace": self.lightbeam.config["namespace"],
+            "resources": {}
+        }
+
         # get token with which to send requests
         self.lightbeam.api.do_oauth()
 
         # send each endpoint
         for endpoint in self.lightbeam.endpoints:
             self.logger.info("sending endpoint {0} ...".format(endpoint))
             asyncio.run(self.do_send(endpoint))
             self.logger.info("finished processing endpoint {0}!".format(endpoint))
             self.logger.info("  (final status counts: {0}) ".format(self.lightbeam.status_counts))
             self.lightbeam.log_status_reasons()
+        
+        ### Create structured output results_file if necessary
+        self.end_timestamp = datetime.datetime.now()
+        self.metadata.update({
+            "completed_at": self.end_timestamp.isoformat(timespec='microseconds'),
+            "runtime_sec": (self.end_timestamp - self.start_timestamp).total_seconds(),
+            "total_records_processed": sum(item['records_processed'] for item in self.metadata["resources"].values()),
+            "total_records_skipped": sum(item['records_skipped'] for item in self.metadata["resources"].values()),
+            "total_records_failed": sum(item['records_failed'] for item in self.metadata["resources"].values())
+        })
+        # total up counts by message and status
+        for resource, resource_metadata in self.metadata["resources"].items():
+            if "failed_statuses" in resource_metadata.keys():
+                for status, status_metadata in resource_metadata["failed_statuses"].items():
+                    total_num_errs = 0
+                    for message, message_metadata in status_metadata.items():
+                        for file, file_metadata in message_metadata["files"].items():
+                            num_errs = len(file_metadata["line_numbers"])
+                            file_metadata.update({
+                                "count": num_errs,
+                                "line_numbers": ",".join(str(x) for x in file_metadata["line_numbers"])
+                            })
+                            total_num_errs += num_errs
+                    status_metadata.update({"count": total_num_errs})
+        
+        if self.lightbeam.results_file:
+            with open(self.lightbeam.results_file, 'w') as fp:
+                fp.write(json.dumps(self.metadata, indent=4))
+
+        if self.metadata["total_records_processed"] == self.metadata["total_records_skipped"]:
+            self.logger.info("all payloads skipped")
+            exit(99) # signal to downstream tasks (in Airflow) all payloads skipped
+        
+        if self.metadata["total_records_processed"] == self.metadata["total_records_failed"]:
+            self.logger.info("all payloads failed")
+            exit(1) # signal to downstream tasks (in Airflow) all payloads failed
+
 
     # Sends a single endpoint
     async def do_send(self, endpoint):
         # We try to  avoid re-POSTing JSON we've already (successfully) sent.
         # This is done by storing a few things in a file we call a hashlog:
         # - the hash of the JSON (so we can recognize it in the future)
         # - the timestamp of the last send of this JSON
         # - the returned status code for the last send
         # Using these hashlogs, we can do things like retry JSON that previously
         # failed, resend JSON older than a certain age, etc.
         if self.lightbeam.track_state:
             hashlog_file = os.path.join(self.lightbeam.config["state_dir"], f"{endpoint}.dat")
             self.hashlog_data = hashlog.load(hashlog_file)
         
+        self.metadata["resources"].update({endpoint: {}})
+
         self.lightbeam.reset_counters()
         # here we set up a smart retry client with exponential backoff and a connection pool
         async with self.lightbeam.api.get_retry_client() as client:
             # process each file
             data_files = self.lightbeam.get_data_files_for_endpoint(endpoint)
             tasks = []
             total_counter = 0
@@ -79,50 +133,75 @@
                         self.logger.info("skipped {0} of {1} payloads because they were previously processed and did not match any resend criteria".format(self.lightbeam.num_skipped, total_counter))
                         
                 await self.lightbeam.do_tasks(tasks, total_counter)
             
             # any task may have updated the hashlog, so we need to re-save it out to disk
             if self.lightbeam.track_state:
                 hashlog.save(hashlog_file, self.hashlog_data)
-        
+            
+            # update metadata counts for this endpoint
+            self.metadata["resources"][endpoint].update({
+                "records_processed": total_counter,
+                "records_skipped": self.lightbeam.num_skipped,
+                "records_failed": self.lightbeam.num_errors
+            })
+    
     
     # Posts a single data payload to a single endpoint using the client
     async def do_post(self, endpoint, file_name, data, client, line, hash):
-        try:
-            status = 401
-            while status==401:
-                
-                # wait if another process has locked lightbeam while we refresh the oauth token:
-                while self.lightbeam.is_locked:
-                    await asyncio.sleep(1)
-                
+        status = 401
+        while status==401:
+            
+            # wait if another process has locked lightbeam while we refresh the oauth token:
+            while self.lightbeam.is_locked:
+                await asyncio.sleep(1)
+            
+            try:
                 async with client.post(util.url_join(self.lightbeam.api.config["data_url"], self.lightbeam.config["namespace"], endpoint),
                                         data=data,
                                         ssl=self.lightbeam.config["connection"]["verify_ssl"],
                                         headers=self.lightbeam.api.headers) as response:
                     body = await response.text()
                     status = response.status
                     if status!=401:
                         # update status_counts (for every-second status update)
                         self.lightbeam.increment_status_counts(status)
                         self.lightbeam.num_finished += 1
                         
                         # warn about errors
                         if response.status not in [ 200, 201 ]:
                             message = str(response.status) + ": " + util.linearize(body)
+
+                            # update run metadata...
+                            failed_statuses_dict = self.metadata["resources"][endpoint].get("failed_statuses", {})
+                            if response.status not in failed_statuses_dict.keys():
+                                failed_statuses_dict.update({response.status: {}})
+                            if message not in failed_statuses_dict[response.status].keys():
+                                failed_statuses_dict[response.status].update({message: {}})
+                            if "files" not in failed_statuses_dict[response.status][message].keys():
+                                failed_statuses_dict[response.status][message].update({"files": {}})
+                            if file_name not in failed_statuses_dict[response.status][message]["files"].keys():
+                                failed_statuses_dict[response.status][message]["files"].update({file_name: {}})
+                            if "line_numbers" not in failed_statuses_dict[response.status][message]["files"][file_name].keys():
+                                failed_statuses_dict[response.status][message]["files"][file_name].update({"line_numbers": []})
+                            failed_statuses_dict[response.status][message]["files"][file_name]["line_numbers"].append(line)
+                            self.metadata["resources"][endpoint]["failed_statuses"] = failed_statuses_dict
+
+                            # update output and counters
                             self.lightbeam.increment_status_reason(message)
-                            self.lightbeam.num_errors += 1
                             if response.status==400:
                                 raise Exception(message)
+                            else: self.lightbeam.num_errors += 1
 
                         
                         # update hashlog
                         if self.lightbeam.track_state:
                             self.hashlog_data[hash] = (round(time.time()), response.status)
 
                     else:
                         self.lightbeam.api.update_oauth()
         
-        except Exception as e:
-            self.lightbeam.num_errors += 1
-            self.logger.warn("{0}  (at line {1} of {2} )".format(str(e), line, file_name))
+            except Exception as e:
+                status = 400
+                self.lightbeam.num_errors += 1
+                self.logger.warn("{0}  (at line {1} of {2} )".format(str(e), line, file_name))
```

## Comparing `lightbeam-0.0.6.dist-info/LICENSE` & `lightbeam-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lightbeam-0.0.6.dist-info/METADATA` & `lightbeam-0.0.7.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightbeam
-Version: 0.0.6
+Version: 0.0.7
 Summary: Sends JSONL data into an Ed-Fi API
 Home-page: https://github.com/edanalytics/lightbeam
 Download-URL: https://github.com/edanalytics/lightbeam/archive/0.0.1.tar.gz
 Author: Tom Reitz
 Author-email: treitz@edanalytics.org
 License: Apache 2.0
 Keywords: data,transmission,api,edfi
@@ -237,14 +237,76 @@
 ## Cache
 To reduce runtime, `lightbeam` caches the resource and descriptor Swagger docs it fetches from your Ed-Fi API as well as the descriptor values for up to a month. This way, the data does not have to be re-loaded from your API on every run. The cached files are stored in the `cache` directory within your `state_dir`. You may run `lightbeam` with the `-w` or `--wipe` flag to clear the cache and force re-fetching the API metadata:
 ```bash
 lightbeam send -c path/to/config.yaml -w
 lightbeam send -c path/to/config.yaml --wipe
 ```
 
+## Structured output of run results
+To produce a JSON file with metadata about the run, invoke lightbeam with
+```bash
+lightbeam send -c path/to/config.yaml --results-file ./results.json
+```
+A sample results file could be:
+
+```json
+{
+    "started_at": "2023-06-08T17:18:25.053207",
+    "working_dir": "/home/someuser/code/sandbox/testing_lightbeam",
+    "config_file": "lightbeam.yml",
+    "data_dir": "./",
+    "api_url": "https://some-ed-fi-api.edu/api",
+    "namespace": "ed-fi",
+    "resources": {
+        "studentSchoolAssociations": {
+            "failed_statuses": {
+                "400": {
+                    "400: { \"message\": \"The request is invalid.\", \"modelState\": { \"request.schoolReference.schoolId\": [ \"JSON integer 1234567899999 is too large or small for an Int32. Path 'schoolReference.schoolId', line 1, position 328.\" ] } }": {
+                        "files": {
+                            "./studentSchoolAssociations.jsonl": {
+                                "line_numbers": "6,4,5,7,8",
+                                "count": 5
+                            }
+                        }
+                    },
+                    "400: { \"message\": \"Validation of 'StudentSchoolAssociation' failed.\\n\\tStudent reference could not be resolved.\\n\" }": {
+                        "files": {
+                            "./studentSchoolAssociations.jsonl": {
+                                "line_numbers": "1,3,2",
+                                "count": 3
+                            }
+                        }
+                    },
+                    "count": 8
+                },
+                "409": {
+                    "409: { \"message\": \"The value supplied for the related 'studentschoolassociation' resource does not exist.\" }": {
+                        "files": {
+                            "./studentSchoolAssociations.jsonl": {
+                                "line_numbers": "9,10,12,14,16,13,11,15,17,18,19,21,22,20",
+                                "count": 14
+                            }
+                        }
+                    },
+                    "count": 14
+                }
+            },
+            "records_processed": 22,
+            "records_skipped": 0,
+            "records_failed": 22
+        }
+    },
+    "completed_at": "2023-06-08T17:18:26.724699",
+    "runtime_sec": 1.671492,
+    "total_records_processed": 22,
+    "total_records_skipped": 0,
+    "total_records_failed": 22
+}
+```
+
 
 # Design
 Some details of the design of this tool are discussed below.
 
 ## Resource-dependency ordering
 JSONL files are sent to the Ed-Fi API in resource-dependency order, which avoids "missing reference" API errors when populating multiple endpoints.
```

## Comparing `lightbeam-0.0.6.dist-info/RECORD` & `lightbeam-0.0.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 lightbeam/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lightbeam/__main__.py,sha256=lZbT__6sBLy_Rxs-WPsGegmeqRjx9oKuAIDHS6kcHcg,4590
-lightbeam/api.py,sha256=OiemDGP7z3NQvlDAI8J7rQdSG298ocJMLCMd-u08dtg,18430
+lightbeam/__main__.py,sha256=n_GcH5OcHNr0LyU5o8dGbVrDEQwlEK6SsAxpKLM4voA,4806
+lightbeam/api.py,sha256=Hj-_8AXi74iK0b1guiIVwALaE9YeKseTgoI3UFJ11fM,18633
 lightbeam/delete.py,sha256=_2AfXRswfFsV3dhd0ZYHFnEPJMxCmWaUwSK8a_vF8os,8914
 lightbeam/hashlog.py,sha256=K6A0xXhkoWgOpjg6WlF5_bp-YvinH27lOhPb815shrs,672
-lightbeam/lightbeam.py,sha256=9w-LfAKEE-8Yef8h2T5nMaWR4Q8St9RsD-VVighCNAY,10168
-lightbeam/send.py,sha256=2Q4ZkOrK-pAzpeyfvIgy46rX3KyFtYKumYZhXIWGNIA,6329
+lightbeam/lightbeam.py,sha256=MOS11VQfQIInDz2aU0P7VESaeB4hwKAIr1mT6NvLhGA,10226
+lightbeam/send.py,sha256=Otn3dO-YKbwJfappmMswHhBTIUduz_yfBtEVO0pwV-k,11064
 lightbeam/util.py,sha256=Nem1rzVdcPya1g6rY_fxGm3QRQnrqHR4PAHy9KOdE9I,1329
 lightbeam/validate.py,sha256=96fcQAMT8jAcp_pz3uDTAoc9YHbQJbSE_GYc88siFO4,5888
 lightbeam/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lightbeam-0.0.6.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
-lightbeam-0.0.6.dist-info/METADATA,sha256=QGF8-2vpcCLy_qg0NaQpb8swUB1NUEpk6B9_qQ5dkTI,12761
-lightbeam-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-lightbeam-0.0.6.dist-info/dependency_links.txt,sha256=zaXVnhNfDDVKDG63P2d5g3NMI6enCOEsVLmo7bmHAjA,132
-lightbeam-0.0.6.dist-info/entry_points.txt,sha256=BbLylxOffnTGU7NfApSlFKDf_C0S-fqE_mcvz0iuuKA,54
-lightbeam-0.0.6.dist-info/top_level.txt,sha256=k8DpVRedspxz4O88pMNN_ClMaC22KtuvkF1HHsxiUow,10
-lightbeam-0.0.6.dist-info/RECORD,,
+lightbeam-0.0.7.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
+lightbeam-0.0.7.dist-info/METADATA,sha256=bqvweTpVjqlhHiR4DIIG97KsIZmpjpozvmsx-mYT9DI,15234
+lightbeam-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+lightbeam-0.0.7.dist-info/dependency_links.txt,sha256=zaXVnhNfDDVKDG63P2d5g3NMI6enCOEsVLmo7bmHAjA,132
+lightbeam-0.0.7.dist-info/entry_points.txt,sha256=BbLylxOffnTGU7NfApSlFKDf_C0S-fqE_mcvz0iuuKA,54
+lightbeam-0.0.7.dist-info/top_level.txt,sha256=k8DpVRedspxz4O88pMNN_ClMaC22KtuvkF1HHsxiUow,10
+lightbeam-0.0.7.dist-info/RECORD,,
```

