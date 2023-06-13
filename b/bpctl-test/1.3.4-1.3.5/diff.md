# Comparing `tmp/bpctl-test-1.3.4.tar.gz` & `tmp/bpctl-test-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpctl-test-1.3.4.tar", last modified: Tue Jun 13 05:06:30 2023, max compression
+gzip compressed data, was "bpctl-test-1.3.5.tar", last modified: Tue Jun 13 13:17:09 2023, max compression
```

## Comparing `bpctl-test-1.3.4.tar` & `bpctl-test-1.3.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/MANIFEST.in
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      380 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/PKG-INFO
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)       86 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/README.md
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.826432 bpctl-test-1.3.4/bin/
--rwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)      118 2023-06-13 05:06:03.000000 bpctl-test-1.3.4/bin/bpctl
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/bpctl_test.egg-info/
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      380 2023-06-13 05:06:30.000000 bpctl-test-1.3.4/bpctl_test.egg-info/PKG-INFO
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      390 2023-06-13 05:06:30.000000 bpctl-test-1.3.4/bpctl_test.egg-info/SOURCES.txt
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)        1 2023-06-13 05:06:30.000000 bpctl-test-1.3.4/bpctl_test.egg-info/dependency_links.txt
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)        4 2023-06-13 05:06:30.000000 bpctl-test-1.3.4/bpctl_test.egg-info/top_level.txt
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/lib/
--rwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-12 07:35:49.000000 bpctl-test-1.3.4/lib/__init__.py
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/lib/bpctl/
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/__init__.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)      901 2023-05-29 10:05:57.000000 bpctl-test-1.3.4/lib/bpctl/authenticate.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     2777 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/base.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     6909 2023-06-01 11:08:39.000000 bpctl-test-1.3.4/lib/bpctl/bp_manifest.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     1695 2023-05-30 12:33:17.000000 bpctl-test-1.3.4/lib/bpctl/bpctl.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)      457 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/config.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     3341 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/load_data.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)       51 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/read_bp_yaml.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/utils.py
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)       38 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/setup.cfg
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     1618 2023-06-13 05:05:57.000000 bpctl-test-1.3.4/setup.py
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 13:17:09.914507 bpctl-test-1.3.5/
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.5/MANIFEST.in
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      380 2023-06-13 13:17:09.914507 bpctl-test-1.3.5/PKG-INFO
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)       86 2023-05-29 09:51:37.000000 bpctl-test-1.3.5/README.md
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 13:17:09.902507 bpctl-test-1.3.5/bin/
+-rwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)      118 2023-06-13 05:06:03.000000 bpctl-test-1.3.5/bin/bpctl
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 13:17:09.906507 bpctl-test-1.3.5/bpctl_test.egg-info/
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      380 2023-06-13 13:17:09.000000 bpctl-test-1.3.5/bpctl_test.egg-info/PKG-INFO
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      390 2023-06-13 13:17:09.000000 bpctl-test-1.3.5/bpctl_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)        1 2023-06-13 13:17:09.000000 bpctl-test-1.3.5/bpctl_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)        4 2023-06-13 13:17:09.000000 bpctl-test-1.3.5/bpctl_test.egg-info/top_level.txt
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 13:17:09.906507 bpctl-test-1.3.5/lib/
+-rwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-12 07:35:49.000000 bpctl-test-1.3.5/lib/__init__.py
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 13:17:09.910507 bpctl-test-1.3.5/lib/bpctl/
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.5/lib/bpctl/__init__.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)      901 2023-05-29 10:05:57.000000 bpctl-test-1.3.5/lib/bpctl/authenticate.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     2777 2023-05-29 09:51:37.000000 bpctl-test-1.3.5/lib/bpctl/base.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     6814 2023-06-13 11:36:26.000000 bpctl-test-1.3.5/lib/bpctl/bp_manifest.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     1695 2023-05-30 12:33:17.000000 bpctl-test-1.3.5/lib/bpctl/bpctl.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)      457 2023-05-29 09:51:37.000000 bpctl-test-1.3.5/lib/bpctl/config.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     3341 2023-05-29 09:51:37.000000 bpctl-test-1.3.5/lib/bpctl/load_data.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)       51 2023-05-29 09:51:37.000000 bpctl-test-1.3.5/lib/bpctl/read_bp_yaml.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.5/lib/bpctl/utils.py
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)       38 2023-06-13 13:17:09.914507 bpctl-test-1.3.5/setup.cfg
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     1618 2023-06-13 13:16:50.000000 bpctl-test-1.3.5/setup.py
```

### Comparing `bpctl-test-1.3.4/lib/bpctl/authenticate.py` & `bpctl-test-1.3.5/lib/bpctl/authenticate.py`

 * *Files identical despite different names*

### Comparing `bpctl-test-1.3.4/lib/bpctl/base.py` & `bpctl-test-1.3.5/lib/bpctl/base.py`

 * *Files identical despite different names*

### Comparing `bpctl-test-1.3.4/lib/bpctl/bp_manifest.py` & `bpctl-test-1.3.5/lib/bpctl/bp_manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             for key in response_json.keys():
                 if key != 'execution_id' and len(response_json[key]) != 0:
                     if key == "kind_created" or key == "kind_updated":
                         for i in response_json[key]:
                             self.print_response(key, i)
                     if key == "kind_failed":
                         for i in response_json[key]:
-                            print(f"Cannot perform create/update on {i['kind']}/{i['name']} due to the following error: {i['error']}")
+                            print(f"Cannot perform create/update details: {i}")
         elif response.status_code == 401:
             print('Invalid Credentials')
             quit()
         else:
             print('Login response code: '+str(response.status_code))
             quit()
 
@@ -116,17 +116,17 @@
     #         else:
     #             flag = 'updated'
     #         print(f"{res['kind']}/{res['metadata']['name']}\t{flag}")
     #     return True
 
     def print_response(self, key, i):
         if key == 'kind_created':
-             print(f"Successfully created {i['kind']}/{i['name']}")
+             print(f"Successfully created {i}")
         else:
-            print(f"Successfully updated {i['kind']}/{i['name']}")
+            print(f"Successfully updated {i}")
         
 
 
     def yaml_parse_into_json(self, file_content):
         """
         version: api/v1
         kind: BPGitRepo
```

### Comparing `bpctl-test-1.3.4/lib/bpctl/bpctl.py` & `bpctl-test-1.3.5/lib/bpctl/bpctl.py`

 * *Files identical despite different names*

### Comparing `bpctl-test-1.3.4/lib/bpctl/load_data.py` & `bpctl-test-1.3.5/lib/bpctl/load_data.py`

 * *Files identical despite different names*

### Comparing `bpctl-test-1.3.4/setup.py` & `bpctl-test-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 
 setuptools.setup(
     name="bpctl-test",
-    version="1.3.4",
+    version="1.3.5",
     author="BP Team",
     author_email="shikhar.maheshwari@opstree.com",
     description="It is private package of bpctl",
     url="https://bitbucket.org/okts/bpctl/src/",
     packages=setuptools.find_packages(),
     include_package_data=True,
     scripts=['bin/bpctl'],
```

