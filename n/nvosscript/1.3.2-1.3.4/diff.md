# Comparing `tmp/nvosscript-1.3.2.tar.gz` & `tmp/nvosscript-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.2.tar", last modified: Mon May 29 08:51:58 2023, max compression
+gzip compressed data, was "nvosscript-1.3.4.tar", last modified: Tue Jun 13 01:23:53 2023, max compression
```

## Comparing `nvosscript-1.3.2.tar` & `nvosscript-1.3.4.tar`

### file list

```diff
@@ -1,30 +1,46 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.495911 nvosscript-1.3.2/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.2/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-29 08:51:58.495748 nvosscript-1.3.2/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.2/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.492034 nvosscript-1.3.2/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.2/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    13399 2023-05-29 07:40:29.000000 nvosscript-1.3.2/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     8990 2023-05-29 07:40:49.000000 nvosscript-1.3.2/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     6143 2023-05-29 07:41:05.000000 nvosscript-1.3.2/nvos/run.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.493141 nvosscript-1.3.2/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-05-29 08:51:58.496017 nvosscript-1.3.2/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-05-29 07:31:27.000000 nvosscript-1.3.2/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.494119 nvosscript-1.3.2/skyeye/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.2/skyeye/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.2/skyeye/handler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      778 2023-05-29 07:35:56.000000 nvosscript-1.3.2/skyeye/loghandler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     2490 2023-05-29 07:45:23.000000 nvosscript-1.3.2/skyeye/remote.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.495022 nvosscript-1.3.2/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.2/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1663 2023-05-29 07:39:37.000000 nvosscript-1.3.2/start/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4500 2023-05-29 08:05:59.000000 nvosscript-1.3.2/start/main.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1157 2023-05-29 07:39:37.000000 nvosscript-1.3.2/start/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.495351 nvosscript-1.3.2/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.2/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 01:23:53.649223 nvosscript-1.3.4/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.4/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-06-13 01:23:53.649072 nvosscript-1.3.4/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.4/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 01:23:53.640962 nvosscript-1.3.4/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.4/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    13432 2023-05-30 09:54:45.000000 nvosscript-1.3.4/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     8487 2023-06-06 06:48:29.000000 nvosscript-1.3.4/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     6143 2023-05-30 09:54:35.000000 nvosscript-1.3.4/nvos/run.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 01:23:53.641985 nvosscript-1.3.4/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-06-13 01:23:53.000000 nvosscript-1.3.4/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      759 2023-06-13 01:23:53.000000 nvosscript-1.3.4/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-06-13 01:23:53.000000 nvosscript-1.3.4/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-06-13 01:23:53.000000 nvosscript-1.3.4/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-06-13 01:23:53.000000 nvosscript-1.3.4/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-06-13 01:23:53.000000 nvosscript-1.3.4/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-06-13 01:23:53.649262 nvosscript-1.3.4/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-06-13 01:21:14.000000 nvosscript-1.3.4/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 01:23:53.643485 nvosscript-1.3.4/skyeye/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.4/skyeye/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      502 2023-05-30 09:54:35.000000 nvosscript-1.3.4/skyeye/handler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      778 2023-05-30 09:54:35.000000 nvosscript-1.3.4/skyeye/loghandler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     2490 2023-05-30 09:54:35.000000 nvosscript-1.3.4/skyeye/remote.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 01:23:53.644222 nvosscript-1.3.4/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.4/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1663 2023-05-30 09:54:35.000000 nvosscript-1.3.4/start/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4500 2023-06-13 01:21:24.000000 nvosscript-1.3.4/start/main.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1157 2023-05-30 09:54:35.000000 nvosscript-1.3.4/start/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 01:23:53.639287 nvosscript-1.3.4/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 01:23:53.648232 nvosscript-1.3.4/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.4/venv/bin/activate_this.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-05-26 05:59:41.000000 nvosscript-1.3.4/venv/bin/jp.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      642 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2html.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      764 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2html4.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2html5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      841 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2latex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      664 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2man.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      830 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2odt.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      636 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      649 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      685 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2s5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      921 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      650 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rst2xml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      718 2023-05-26 05:59:42.000000 nvosscript-1.3.4/venv/bin/rstpep2html.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 01:23:53.648513 nvosscript-1.3.4/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.4/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.2/LICENSE` & `nvosscript-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.2/nvos/file.py` & `nvosscript-1.3.4/nvos/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
 
 def find_json_config(file_path, config_list, project_space_list):
     for file_name in os.listdir(file_path):
         if file_name == ".idea" or file_name == ".git" or file_name == ".repo" or file_name == ".ndtc" or file_name == ".DS_Store":
             continue
         if os.path.isdir(os.path.join(file_path, file_name)):
             find_json_config(os.path.join(file_path, file_name), config_list, project_space_list)
-        elif file_name.endswith(".json"):
+        elif file_name.endswith(".json") or file_name == "CMakeLists.txt":
             file_full_path = os.path.join(file_path, file_name)
             for project_space in project_space_list:
                 if file_full_path.startswith(project_space["project_space"]):
                     file_data = {"file_path": os.path.join(file_path, file_name),
                                  "file_size": os.path.getsize(os.path.join(file_path, file_name)),
                                  "git_branch": project_space["git_branch"]}
                     config_list.append(file_data)
```

### Comparing `nvosscript-1.3.2/nvos/remote.py` & `nvosscript-1.3.4/nvos/remote.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,99 +72,92 @@
     get_current_env()
     url = "%s%s" % (daemon_network, "/workspace/analyse")
     post_param = {"userId": login.get_user_id(), "fileDirectory": workspace_path, "projectSpaceList": project_list}
     data = post_data(url, post_param)
     return data
 
 def upload_file(workspace_path, file_path_list, project_space_list):
-    s3_secret = get_s3_secret()
-    bucket_name = s3_secret["bucket"]
-    aws_ak = s3_secret["ak"]
-    aws_sk = s3_secret["sk"]
-    aws_region = s3_secret["regionId"]
-    s3 = boto3.resource('s3', region_name=aws_region, aws_access_key_id=aws_ak,
-                        aws_secret_access_key=aws_sk)
-    bucket = s3.Bucket(bucket_name)
     upload_list = []
     filter_upload_re = filter_upload_dir()
     for project_space in project_space_list:
         for file_path in file_path_list:
             flag = False
             for temp in filter_upload_re:
                 matchObj = re.match(temp, file_path["file_path"], re.M | re.I)
                 if matchObj:
                     flag = True
                     break
             if not flag:
                 continue
 
             if project_space["project_space"] in file_path["file_path"]:
-                file_name = "%s/%s/%s" % (
-                    login.get_user_id(), md5(project_space["git_branch"], project_space["project_space"]),
-                                            file_path["file_path"][file_path["file_path"]
-                .find(os.path.basename(project_space["project_space"])):])
-                file_name = file_name.replace("\\", "/")
                 local_file_path = file_path["file_path"]
-                temp_file = {"local_file_path": local_file_path, "file_name": file_name}
+                temp_file = {"local_file_path": local_file_path, "project_space": project_space["project_space"], "project_space_git_branch": project_space["git_branch"]}
                 upload_list.append(temp_file)
-    upload_process(upload_list, bucket)
+    upload_process(upload_list)
 
     file_upload_notify(workspace_path, project_space_list)
 
-def upload_process(upload_list, bucket):
+def upload_process(upload_list):
     global global_var
     multiprocessing.set_start_method('spawn', True)
     cores = multiprocessing.cpu_count()
     with concurrent.futures.ThreadPoolExecutor(max_workers=cores) as executor, tqdm(desc="uploading", total=len(upload_list)) as progress:
         for index, file in enumerate(upload_list):
-            executor.submit(uploading_file, file, bucket)
+            executor.submit(uploading_file, file)
         time_count = 0
         addition = 0
         while True:
             time.sleep(1)
             time_count += 1
             progress.update(global_var - addition)
             addition = global_var
             if (global_var == len(upload_list) or global_var >= len(upload_list) - 20):
                 break
             if time_count == 60:
                 break
 
 
-def uploading_file(file, bucket):
+def uploading_file(file):
+
     global global_var
+
+    get_current_env()
+    url = "%s%s" % (daemon_network, "/file/upload")
+
+    local_file_path = file["local_file_path"]
+
     try:
-        local_file_path = file["local_file_path"]
-        file_name = file["file_name"]
-        bucket.upload_file(local_file_path, file_name)
-        logger.info(f"upload file ossUrl:{file_name} file local full path:{local_file_path}")
+        with open(local_file_path, 'r') as f:
+            contents = f.read()
+        post_param = {"projectSpaceGitBranch": file["project_space_git_branch"], "projectSpaceFileDirectory": file["project_space"], "userId": login.get_user_id(), "filePath": local_file_path, "fileContent": contents}
+        post_data(url, post_param)
+        logger.info(f"upload file local full path:{local_file_path}")
         global_var += 1
     except Exception:
-        logger.exception("uploading_file error")
+        logger.exception('uploading_file error: %s', local_file_path)
 
 
 
 def download_file(project_space):
-    s3_secret = get_s3_secret()
-    bucket_name = s3_secret["bucket"]
-    aws_ak = s3_secret["ak"]
-    aws_sk = s3_secret["sk"]
-    aws_region = s3_secret["regionId"]
-    s3 = boto3.resource('s3', region_name=aws_region, aws_access_key_id=aws_ak,
-                        aws_secret_access_key=aws_sk)
-    bucket = s3.Bucket(bucket_name)
+    get_current_env()
+    url = "%s%s" % (daemon_network, "/file/download")
     for file in project_space["changedFileList"]:
-        ossURL = file["ossURL"]
-        fileFullPath = file["fileFullPath"]
+        file_id = file["fileId"]
+        file_full_path = file["fileFullPath"]
         try:
-            bucket.download_file(ossURL, fileFullPath)
+            post_param = {"id": file_id}
+            data = post_data(url, post_param)
+            file_content = data["fileContent"]
+            with open(file_full_path, "w") as f:
+                f.write(file_content)
         except Exception:
-            logger.info(f"this file sync fail  ossURL:{ossURL} fileFullPath:{fileFullPath}" )
+            logger.info(f"this file sync fail  id:{file_id} ")
         else:
-            logger.info(f"this file sync success  ossURL:{ossURL} fileFullPath:{fileFullPath}")
+            logger.info(f"this file sync success  id:{file_id} ")
 
 def save_workspace(workspace_path, project_list):
     get_current_env()
     url = "%s%s" % (daemon_network, "/workspace/add")
     post_param = {"userId": login.get_user_id(), "fileDirectory": workspace_path, "projectSpaceList": project_list}
     return post_data(url, post_param)
```

### Comparing `nvosscript-1.3.2/nvos/run.py` & `nvosscript-1.3.4/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.2/setup.py` & `nvosscript-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.2',
+    version='1.3.4',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.2/skyeye/loghandler.py` & `nvosscript-1.3.4/skyeye/loghandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.2/skyeye/remote.py` & `nvosscript-1.3.4/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.2/start/login.py` & `nvosscript-1.3.4/start/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.2/start/main.py` & `nvosscript-1.3.4/start/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.2")
+        print("1.3.4")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.2/start/utils.py` & `nvosscript-1.3.4/start/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.2/win/win_auto_script.py` & `nvosscript-1.3.4/win/win_auto_script.py`

 * *Files identical despite different names*

