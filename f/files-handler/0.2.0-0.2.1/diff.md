# Comparing `tmp/files-handler-0.2.0.tar.gz` & `tmp/files-handler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "files-handler-0.2.0.tar", last modified: Wed Apr 19 17:47:30 2023, max compression
+gzip compressed data, was "files-handler-0.2.1.tar", last modified: Tue Jun 13 18:38:42 2023, max compression
```

## Comparing `files-handler-0.2.0.tar` & `files-handler-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 17:47:30.573364 files-handler-0.2.0/
--rw-rw-rw-   0        0        0     3343 2023-04-19 17:47:30.569367 files-handler-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2558 2023-04-19 17:34:33.000000 files-handler-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 17:47:30.513810 files-handler-0.2.0/files_handler/
--rw-rw-rw-   0        0        0      106 2023-02-24 14:24:15.000000 files-handler-0.2.0/files_handler/__init__.py
--rw-rw-rw-   0        0        0     1454 2023-03-17 14:33:39.000000 files-handler-0.2.0/files_handler/folders_handler.py
--rw-rw-rw-   0        0        0     5315 2023-04-19 17:45:42.000000 files-handler-0.2.0/files_handler/s3_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:47:30.566367 files-handler-0.2.0/files_handler.egg-info/
--rw-rw-rw-   0        0        0     3343 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-19 17:47:30.000000 files-handler-0.2.0/files_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 17:47:30.574365 files-handler-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-04-19 17:47:20.000000 files-handler-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:38:42.405671 files-handler-0.2.1/
+-rw-rw-rw-   0        0        0     3343 2023-06-13 18:38:42.404700 files-handler-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2558 2023-05-05 14:13:27.000000 files-handler-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 18:38:42.378669 files-handler-0.2.1/files_handler/
+-rw-rw-rw-   0        0        0      108 2023-05-30 19:39:31.000000 files-handler-0.2.1/files_handler/__init__.py
+-rw-rw-rw-   0        0        0     1873 2023-06-13 18:36:45.000000 files-handler-0.2.1/files_handler/folders_handler.py
+-rw-rw-rw-   0        0        0     6763 2023-06-13 18:36:45.000000 files-handler-0.2.1/files_handler/s3_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:38:42.403701 files-handler-0.2.1/files_handler.egg-info/
+-rw-rw-rw-   0        0        0     3343 2023-06-13 18:38:42.000000 files-handler-0.2.1/files_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-06-13 18:38:42.000000 files-handler-0.2.1/files_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:38:42.000000 files-handler-0.2.1/files_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 18:38:42.000000 files-handler-0.2.1/files_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 18:38:42.000000 files-handler-0.2.1/files_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:38:42.405671 files-handler-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-06-13 18:36:45.000000 files-handler-0.2.1/setup.py
```

### Comparing `files-handler-0.2.0/PKG-INFO` & `files-handler-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: files-handler
-Version: 0.2.0
+Version: 0.2.1
 Summary: Files Handler Library
 Home-page: 
 Author: Bhryan Henderson
 Author-email: bhryan.perpetuo@concert.com.br
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `files-handler-0.2.0/README.md` & `files-handler-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `files-handler-0.2.0/files_handler/s3_handler.py` & `files-handler-0.2.1/files_handler/s3_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,189 @@
 # Importing libraries
 import boto3
 import botocore
 import os
 import tqdm
 from files_handler.folders_handler import folders_handler
 
+
 class s3_handler:
     """
     Deal with files and connection to S3.
-    
+
     :param bucket: The Bucket.
     :type bucket: string
     :param path_ref: Reference Path to manage the files and folders.
     :type path_ref: string
     """
 
-    def __init__(self, bucket, path_ref, input_path='input', result_path='output'):
+    def __init__(self, bucket, path_ref, input_path="input", result_path="output"):
         self.session = boto3.Session()
         self.bucket = bucket
         self.path_ref = path_ref
         self.path_to_predict_images = os.path.join(path_ref, input_path)
-        self.s3_client = boto3.client('s3')
-        self.folders_handler = folders_handler('')
+        self.s3_client = boto3.client("s3")
+        self.folders_handler = folders_handler("")
 
-    # Get image from s3 bucket 
-    def get_image_from_s3_bucket(self, s3_image_path, local_download_path='', progress_bar=True):
+    # Get image from s3 bucket
+    def get_image_from_s3_bucket(
+        self,
+        s3_image_path,
+        local_download_path="",
+        progress_bar=True,
+        create_folder=True,
+        quiet=False,
+    ):
         """
         Get an image from S3 passing the image path on s3 and saving on reference path + input
-        
+
         :param s3_image_path: The s3 path of image with the image name.
         :type s3_image_path: string
         :param local_download_path: Local path to download image, if you desire to use a different path than "input_path"
         :type local_download_path: string
         :param progress_bar: Enable progress bar for download
         :type progress_bar: boolean
-    
+        :param create_folder: Enable folder creation for downloaded file
+        :type create_folder: boolean
+        :param quiet: Disable print of messages along code
+        :type quiet: boolean
+
         :return: If the image was downloaded or not.
-        :rtype: boolean
+        :type: boolean
         """
         try:
-
-            if local_download_path == '':
+            if local_download_path == "":
                 download_path = self.path_to_predict_images
             else:
                 download_path = local_download_path
 
-            self.folders_handler.verify_and_create_folder(download_path, 'Creating input directory...')
+            if create_folder:
+                self.folders_handler.verify_and_create_folder(
+                    download_path, "Creating input directory...", quiet=quiet
+                )
 
             image_name = os.path.basename(s3_image_path)
-            local_image_path = os.path.join(download_path, image_name).replace("\\", "/")
-
-            print(f'Downloading file: {image_name} to {download_path} folder') 
-            s3 = self.session.resource('s3')
+            local_image_path = os.path.join(download_path, image_name).replace(
+                "\\", "/"
+            )
+
+            if not quiet:
+                print(f"Downloading file: {image_name} to {download_path} folder")
+            s3 = self.session.resource("s3")
             bucket = s3.Bucket(self.bucket)
 
             if progress_bar:
-                meta_data = self.s3_client.head_object(Bucket=self.bucket, Key=s3_image_path)
-                total_length = int(meta_data.get('ContentLength', 0))
-                with tqdm.tqdm(total=total_length, unit="B", unit_scale=True, desc=s3_image_path) as pbar:
-                    bucket.download_file(s3_image_path, local_image_path, Callback=lambda bytes_transferred: pbar.update(bytes_transferred))
+                meta_data = self.s3_client.head_object(
+                    Bucket=self.bucket, Key=s3_image_path
+                )
+                total_length = int(meta_data.get("ContentLength", 0))
+                with tqdm.tqdm(
+                    total=total_length, unit="B", unit_scale=True, desc=s3_image_path
+                ) as pbar:
+                    bucket.download_file(
+                        s3_image_path,
+                        local_image_path,
+                        Callback=lambda bytes_transferred: pbar.update(
+                            bytes_transferred
+                        ),
+                    )
 
             else:
                 bucket.download_file(s3_image_path, local_image_path)
 
-
-            print(f'File Downloaded')
+            if not quiet:
+                print("File Downloaded")
             return True
-        
+
         except botocore.exceptions.ClientError as e:
             print(e)
             return False
 
     # Upload resulting image to s3 bucket
-    def upload_image_to_s3_bucket(self, local_image_path, s3_output_path, progress_bar=True):
+    def upload_image_to_s3_bucket(
+        self, local_image_path, s3_output_path, progress_bar=True, quiet=False
+    ):
         """
         Upload an image to S3 passing the image path on s3 and the S3 Output Path
-        
-        :param local_image_path: the path of the image locally with the image name
+
+        :param local_image_path: The path of the image locally with the image name
         :type local_image_path: string
-        :param s3_output_path: the path of the image on S3
+        :param s3_output_path: The path of the image on S3
         :type s3_output_path: string
         :param progress_bar: Enable progress bar for upload
         :type progress_bar: boolean
-    
+        :param quiet: Disable print of messages along code
+        :type quiet: boolean
+
         :return: If the image was uploaded or not.
         :rtype: boolean
         """
         try:
-            print(f'Uploading results to {s3_output_path}')
-            s3 = self.session.resource('s3')
+            if not quiet:
+                print(f"Uploading results to {s3_output_path}")
+            s3 = self.session.resource("s3")
             bucket = s3.Bucket(self.bucket)
 
             image_name = os.path.basename(local_image_path)
             s3_image_path = os.path.join(s3_output_path, image_name).replace("\\", "/")
-            print(f'Complete path: {s3_image_path}')
+            if not quiet:
+                print(f"Complete path: {s3_image_path}")
 
             if progress_bar:
-                with tqdm.tqdm(total=os.stat(local_image_path).st_size, unit="B", unit_scale=True, desc=image_name) as pbar:
-                    bucket.upload_file(local_image_path, s3_image_path, Callback=lambda bytes_transferred: pbar.update(bytes_transferred))
+                with tqdm.tqdm(
+                    total=os.stat(local_image_path).st_size,
+                    unit="B",
+                    unit_scale=True,
+                    desc=image_name,
+                ) as pbar:
+                    bucket.upload_file(
+                        local_image_path,
+                        s3_image_path,
+                        Callback=lambda bytes_transferred: pbar.update(
+                            bytes_transferred
+                        ),
+                    )
 
             else:
                 bucket.upload_file(local_image_path, s3_image_path)
 
             return True
 
         except botocore.exceptions.ClientError as e:
+            print(e)
             return False
 
-    def check_if_file_exists(self, file_name, s3_path):
+    def check_if_file_exists(self, file_name, s3_path, quiet=False):
         """
         Check if file exists in s3 bucket
-        
-        :param file_name: the name of the file 
+
+        :param file_name: The name of the file
         :type file_name: string
-        :param s3_path: the path of the file on S3
+        :param s3_path: The path of the file on S3
         :type s3_path: string
-    
+        :param quiet: Disable print of messages along code
+        :type quiet: boolean
+
         :return: If the file exists or not.
         :rtype: boolean
         """
         try:
-            s3 = self.session.resource('s3')
+            s3 = self.session.resource("s3")
             try:
-                s3.Object(self.bucket, os.path.join(s3_path, file_name).replace("\\", "/")).load()
+                s3.Object(
+                    self.bucket, os.path.join(s3_path, file_name).replace("\\", "/")
+                ).load()
+                if not quiet:
+                    print("File exists")
                 return True
             except botocore.exceptions.ClientError as e:
-                if e.response['Error']['Code'] == "404":
+                if e.response["Error"]["Code"] == "404":
                     # The object does not exist.
+                    if not quiet:
+                        print("File does not exist")
                     return False
                 else:
                     # Something else has gone wrong.
                     raise
         except botocore.exceptions.ClientError as e:
+            print(e)
             return False
```

### Comparing `files-handler-0.2.0/files_handler.egg-info/PKG-INFO` & `files-handler-0.2.1/files_handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: files-handler
-Version: 0.2.0
+Version: 0.2.1
 Summary: Files Handler Library
 Home-page: 
 Author: Bhryan Henderson
 Author-email: bhryan.perpetuo@concert.com.br
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `files-handler-0.2.0/setup.py` & `files-handler-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Always prefer setuptools over distutils
-from setuptools import setup, find_packages
+from setuptools import setup
 
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
+with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="files-handler",
-    version="0.2.0",
+    version="0.2.1",
     description="Files Handler Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Bhryan Henderson",
     author_email="bhryan.perpetuo@concert.com.br",
     license="MIT",
@@ -29,13 +29,13 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Operating System :: OS Independent"
+        "Operating System :: OS Independent",
     ],
     packages=["files_handler"],
     include_package_data=True,
-    install_requires=["boto3", "tdqm"]
-)
+    install_requires=["boto3", "tdqm"],
+)
```

