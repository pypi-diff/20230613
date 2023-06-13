# Comparing `tmp/cloudpy_org-1.3.2.tar.gz` & `tmp/cloudpy_org-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.3.2.tar", last modified: Sat May 27 04:56:41 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.3.3.tar", last modified: Tue Jun 13 06:20:23 2023, max compression
```

## Comparing `cloudpy_org-1.3.2.tar` & `cloudpy_org-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 04:56:41.278685 cloudpy_org-1.3.2/
--rw-rw-rw-   0        0        0      935 2023-05-27 04:56:41.278137 cloudpy_org-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 04:56:41.180301 cloudpy_org-1.3.2/cloudpy_org/
--rw-rw-rw-   0        0        0       82 2023-05-27 04:35:22.000000 cloudpy_org-1.3.2/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    71203 2023-05-27 04:54:59.000000 cloudpy_org-1.3.2/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-27 04:56:41.257295 cloudpy_org-1.3.2/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2023-05-27 04:56:40.000000 cloudpy_org-1.3.2/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-27 04:56:41.000000 cloudpy_org-1.3.2/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 04:56:40.000000 cloudpy_org-1.3.2/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-27 04:56:40.000000 cloudpy_org-1.3.2/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-27 04:56:40.000000 cloudpy_org-1.3.2/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 04:56:41.278685 cloudpy_org-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-05-27 04:53:32.000000 cloudpy_org-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:20:23.540289 cloudpy_org-1.3.3/
+-rw-rw-rw-   0        0        0      935 2023-06-13 06:20:23.539791 cloudpy_org-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 06:20:23.440835 cloudpy_org-1.3.3/cloudpy_org/
+-rw-rw-rw-   0        0        0       82 2023-05-27 04:35:22.000000 cloudpy_org-1.3.3/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    76159 2023-06-13 06:16:57.000000 cloudpy_org-1.3.3/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:20:23.519392 cloudpy_org-1.3.3/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-06-13 06:20:22.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-13 06:20:23.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:20:22.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-13 06:20:22.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 06:20:22.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:20:23.540289 cloudpy_org-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2023-06-13 06:18:43.000000 cloudpy_org-1.3.3/setup.py
```

### Comparing `cloudpy_org-1.3.2/PKG-INFO` & `cloudpy_org-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.3.2
+Version: 1.3.3
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.2/cloudpy_org/tools.py` & `cloudpy_org-1.3.3/cloudpy_org/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Find documentation at https://www.cloudpy.org
 """
+cloudpy_org_version='1.3.3'
 import os
 import json
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings('ignore')
 warnings.simplefilter('ignore')
 import pandas as pd
@@ -378,22 +379,35 @@
         ***
         Decrypts a given emctrypted str input and with a given encryption key also in str datatype.
         Return the decrypted data as str.
         ***
         '''
         return Fernet(keyStr.encode('utf-8')).decrypt(inputStr.encode('utf-8')).decode()
     #__________________________________________________________________________
+    def __do(self,a,n):
+        a = a[::-1]
+        b,c = "",""
+        r = int(len(a)/n) + 1
+        for i in range(0,r):
+            b += a[2*i*n:(2*i+1)*n]
+            c += (a[(2*i+1)*n:(2*i+2)*n][::-1])
+            if i == r-1:
+                b += c[::-1][0:n]
+                c = c.replace(c[::-1][0:n][::-1],'')
+        c = c.upper()
+        return c,b
     def __set_aws_session(self,region_name:str="us-east-2")->None:
         '''
         Sets a session with given AWS credentials.
         '''
         self.__session = None
         self.__s3_client = None
         if type(self.__tdata) == dict and self.__tdata != {}:
-            spd = self.decrypt_before_expiration(self.__tdata).split("*_xxx_*")
+            spd = self.__do(self.decrypt_before_expiration(self.__tdata),10)
+            
             try:
                 self.__session = boto3.Session(aws_access_key_id=spd[0]
                                          ,aws_secret_access_key=spd[1])
                 self.__s3_client = boto3.client('s3'
                                                 ,aws_access_key_id=spd[0]
                                                 ,aws_secret_access_key=spd[1]
                                                 ,region_name=region_name)
@@ -1093,87 +1107,137 @@
         self.aux[keyname] = {}
         dc = "self.aux['@keyname'] = " + dictstr
         dc = dc.replace("@keyname",keyname)
         exec(dc)
         rslt = self.aux[keyname] 
         self.aux.pop(keyname, None)
         return rslt
+#xdata = {}
+#class aws_settings():
+#    def __init__(self,this_xdata:dict={},user_key:str=None,secret:str=None,minutes_to_expire:int=0):
+#        self.pt = processing_tools()
+#        if this_xdata != None and this_xdata != {} and type(this_xdata) == dict:
+#            self.xdata = this_xdata
+#        elif user_key != None and secret != None:
+#            self.xdata = self.__gen_xdata(user_key=user_key,secret=secret,minutes_to_expire=minutes_to_expire)
+#    def __gen_xdata(self,user_key:str,secret:str,minutes_to_expire:int):
+#        return self.pt.gen_encrypted_data_with_expiration(original_message = self.__of(user_key,secret,10),minutes_to_expire=minutes_to_expire)
+#    def __of(self,user_key,secret,n):
+#        user_key = user_key[0:5].upper() + user_key[5:10].lower() + user_key[10:len(user_key)].upper()
+#        a = ""
+#        r = int(len(secret+user_key)/n) +1
+#        for i in range(0,r):
+#            a += secret[i*n:(i+1)*n] + user_key[i*n:(i+1)*n][::-1]
+#        return a[::-1]
 
 xpt = processing_tools()
 xs3 = boto3.client('s3')
 xpt.environment = "s3"
 class aws_framework_manager:
-    def __init__(self,secret_pair:list=[]):
-        self.__cppt_construction(secret_pair)
+    def __init__(self,secret_key:str):
+        self.__cppt_construction(secret_key)
         self.cppt.environment = "s3"
         self.general_info = {}
         self.service_name = "cloudpy-org-service-beta"
         self.delimiters = ["pZo-9xH9oEO2B2OEo","2nZzN01wtktk10N","VhMxT-9xVVZzN01w","_Shv-4F86Co981h"]
         self.general_separators = {'user_email_sep': '-0-', '@': '-1-', '.': '-2-'}
         self.special_separators = self.general_separators
         self.__service_initialized = False
         self.__not_initialized_message ='Service not initialized yet.\n'\
         'Use initialize_service(service_token="<your service_token>") function to active the service.\n'
     #___________________________________________________________________
-    def __cppt_construction(self,secret_pair:list=[]):
-        if len(secret_pair) == 2:
-            self.cppt = processing_tools(data=xpt.basic_dicstr_to_dict(xpt.decrypt(secret_pair[0],secret_pair[1])))
+    def __do(self,a,n,upper:bool=True):
+        a = a[::-1]
+        b,c = "",""
+        r = int(len(a)/n) + 1
+        for i in range(0,r):
+            b += a[2*i*n:(2*i+1)*n]
+            c += (a[(2*i+1)*n:(2*i+2)*n][::-1])
+            if i == r-1:
+                b += c[::-1][0:n]
+                c = c.replace(c[::-1][0:n][::-1],'')
+        if upper:
+            c = c.upper()
+        return c,b
+    def __cppt_construction(self,secret_key:str=""):
+        if len(secret_key) > 10:
+            k = 'JQxrs8sWqn3JIWlIL8nTlw-302SfmV7RmlZ-T-gB5c4=oiwn8TU5-NcDKzVq'
+            self.cppt = processing_tools(data=xpt.basic_dicstr_to_dict(xpt.decrypt(secret_key,self.__do(k,10,False)[1] + self.__do(k,10,False)[0][0:4])))
         else:
             self.cppt = processing_tools()
     #___________________________________________________________________
-    def initialize_service(self,service_token:str,version:float=1.30,test:bool=False):
+    def initialize_service(self,service_token:str,version:str=cloudpy_org_version,test_file_name:str=None):
         error_message = 'Could not initialize the service. Please verify you are using the right service token.'
         try:
             for i in range(0,2):
                 self.args_by_key,self.dx = {},{}
-                self.__api_encrypted_caller = 'gAAAAABkbtchCJzu1TG2Ap2qvSxyTaBx7q1kuEOsVWoo7bcDZQVNhT_'\
-                '4lOxMvo3AKpb6sbf9VNIiCLz4NeSglNgWAAtR-FXNDNavSzyxXAKq7342Rphb1NinG9nbBozYY8SAJmGkZlhSF'\
-                'dur391PjRe_TKhrD_5doWvyPsYTa5GhazljtuuNu1U4c4hoc-LMrmRYhFmwVZjVZkK-GciCXdFnW-5qcAJrVRvd'\
-                '2q5TnyTKThR64WZ0b4QTkPr8-HNHhSr0ZjwwVp_yRDejMleLeCQUhMI6J5O-_4_jzKrbsBSnLnaguXswGSNA-4xR'\
-                'OkTEMfappNO_3qSDWnTMT8oqhVUhM_v750vVelIMgSFOrSkM6-5it-cyUK657B9j_rWDy0Scd4mp5p3x1VYHDic8N'\
-                '77DtZFn5xJMxCbgdhwf7ApqhIazR9LkiDJcx8Mb48W07yQRmx8Q8bc4izLGJEG-O7_3G-TXiaJUFaOcGyNsLJcxC4x'\
-                'PBSpIeIAfv2kAmzZemdPxaNvAsrajIoX5fTxzH7jxk-txATYN9wJpX0Vl3M0hQPTLXxd2NweRSgcoJZM7Spjt9o95mE'\
-                'LbCwbXEi3bESeRCGOJz7HBB4La-mimwWJm0dLusl43u6N5qN_7AAw0lV1WCsZhrI-LWG7hw9OyBpgu5dn7YP9tM94nnR'\
-                'YaWNan0Fjc59Dci8ZY9s8cLfR6CDiyHxFHiY9KyiPDrTUH_aU1-O5T62C4tWzcaFbzdgW9-3Bq-czaAXg8WHiehHt7GtK'\
-                'oATX1O9vfbRK-GtYZbQ8VH9Q93aVUObgXu7zA4mXJhkBN1ZeU0ziCyzLrwRcpIgPAWFThcztOl7r_5ANnHuwF9f1dH2h5O'\
-                'GNVSv0M6pmCrHNuLVD6gy3KGIh-lI2W3mY9C_0b4Z2zr-4jGp8fxnO2yES-41iH8pS_Esvr5h7eaEv50kzi3TU='
-                self.__get_dynamic_response(service_token=service_token,version=version,test=test)
+                self.__api_encrypted_caller = ''\
+                'gAAAAABkh-dZKOI8qSh47zj54htxA_Ib_ag4gI99hdxDuHo7oWktIOaQ7U63M13qURWqXrbxJ-X8ZFXXn7Lmifq_uI8Sqe_l1CE-'\
+                'BHe39zTrwk6ZJWaDrUwDeXi1Xm_7SEYffuZ75hp7yV9x8qMRTo2nhYFs4chOlTU-gojLp3iosWzlAaxtS8WE6mnxxOn8u7RAcoxg'\
+                'H-Omya51HagtAL3Ho2137D5qIf3LDhr_IFSlnZTkNw-WgMjS3LwUdXgAsSRddZQSzxNlsa7ame28tyGee4Qwg4dg2PCuegG9_1r8'\
+                'WTXYm_U8QVySZt5fRt1qDUzLl9MFDmlMCnjUn5GknLqXYvCY3z4GNNlfBqaxZUpbFE4pV3OZ6NI-cb6V0JiX6rACvxjDIIwecDg2'\
+                'oaEa1Jw-xKBQ86EnFx2j1PcMMtvJlX75xCCR789-v75GfAejN6ZWVjzDwanI2qy5IL63tigukTnufpDuesc3NZUMM4V0B_LbSw0a'\
+                'Ic7tzFKAaRxE3uFiz9J8yAbAkbOGu6pGpWcEXgtvtQe0A4l1fiQznqAhE23o4R0QJ3YHTC7JTuTfi32S3Sjel9jexsyOyRFUdcuO'\
+                'zeminNCLLpIUDG8BYFhy0-jwMvrWnUB2b_NPqlBpKx9EJZwHrga2XgVhRxfHgnSD3vcZqNv4jLhGZdCwfUuRIArKTbmwzddthPZN'\
+                'f8W21ejufOxcvR2JWw7MfKiPpTNlunRsdEq8QLHAwNawjuEiYlK-vrGm0MsSIZmP55nOwzE5SbHNtPgLomZMVDxgKh2xixfq59Ux'\
+                'uVyieJozGM-XPJhjziU6AlAdboUHyo6LJeBV95sdF7VomSLBWbFokTFBKOaY7upqtt7ix1WquS4JwrCRRJcUL4AYrM3njJe9U4Cv'\
+                '9ZGAO5bpKOOwRJRiXkMtLpCCoLg-NqioU59zAgEnGVuT85MqZYzJiH7Xeu9LcEqZ1UDff3kkxpol8piry73P5Jip6hJ9GwW1CulV'\
+                'd8uT-CR_EoVxM9qy0bpY49yMLfq8SmgKz2iKVDo-DOw4IG2UvQ4sr21j242MWT36lwVhl6LZpiFjTTc8vGGogrGcpRclzitVjmEd'\
+                '3zx7TTtHg_Z6SuT8KyNyO6tUsLci9CsPPWJMgjdA-UZgDYuMCYbLWxffZmK1SYg1zDAutfVf6DOlKIwnJOa3QPWyM8SBBT68nxu0'\
+                '20DEgsRt1kPjDiLsbK_TU6PB0H5pUJcTG4Z2JdHmFzgb6uBsUPrrSMcx2BCGxjrggpAC-v5mPO5_RU2IMWVNDLhiAzBKdv1ivtCu'\
+                'H_tDJdfneJHVZ1ucxS8vc7Jz26OUDfT7oDoxLRerO8o6Prm_zKdrVbNgvACpl3fWATCv2nJYyV-PBI_uupWJ6nz-X56Rb3KMt64_'\
+                'HY8BL-3QQclPw1vv05LUGkeGmHgFcJKzS6L6EbkVLCAf3Ar3Z6JeeaZ0Mi77zvaUofaoab7XLatBHg0z7wHpsiynESTKlafaZRTA'\
+                'rH_1U5Au9KWV0kWSxXRu8unqCpfs_okOVuYaoBvqc4Reo2i6NPthfXYqagNlGfYuLYLhsx1szF2Cg86_7KedwMtU8c2roAAN3eGN'\
+                'hhTkLS6xQOK_'
+                self.__get_dynamic_response(service_token=service_token,version=version,test_file_name=test_file_name)
                 self.find_methods_arguments()
                 self.set_valid_characters()
                 self.version = self.get_version()
             if self.__service_initialized:   
                 return 'Service initialized.'
             else:
                 return error_message
-        except:
+        except Exception as e:
+            print("error 01:",str(e))
             return error_message
     #___________________________________________________________________
-    def load_local_code(self):
-        with open(os.getcwd() + "/aws_framework_manager_dynamic_code_0128.json", 'r') as f:
+    def __load_local_code(self,file_name):
+        with open(os.getcwd() + "/" + file_name, 'r') as f:
             rslt = json.loads(f.read())
         return rslt
     #___________________________________________________________________
-    def __get_dynamic_response(self,service_token:str,version:float,test:bool=False):
+    def __k(self,tagStr:str):
+        self.last_k = self.cppt.gen_encrypted_data_with_expiration(self.cppt.get_s3_file_content(referenceName=tagStr,s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/"),0.2)
+    
+    #___________________________________________________________________
+    def __get_dynamic_response(self,service_token:str,version:str,test_file_name:str=None):
+        self.__k("service_key")
+        dc = self.cppt.decrypt(self.__api_encrypted_caller,self.cppt.decrypt_before_expiration(self.last_k))\
+        .replace("@version",version)\
+        .replace("@gsm",self.__gsm(service_token))
+        self.__k("cloudpy_org_2023")
+        #dc += "\nprint(\'self.ddkk:\\n\',self.ddkk)"
         try:
-            s3FullFolderPath = "s3://" + self.service_name + "/settings/secrets/"
-            enc_key = self.cppt.get_s3_file_content(referenceName="service_key",s3FullFolderPath=s3FullFolderPath)
-            m = 'gAAAAABkcBT5Pw2_4O4jZe2RJv-9MCa91rfeRHCbDalo2O4E8wqyAn7YVkuyAv6IZgctEDPwpHBoSTNQdqt15BDCzhRmLg8BK9rxBbinlHd0xSIs-2jbHjk='
-            dc = self.cppt.decrypt(self.__api_encrypted_caller,enc_key).replace("@version",str(version))\
-            .replace(self.cppt.decrypt(m,enc_key),str(self.__gsm(service_token))).replace("pt.","self.cppt.")
-            if test:
+            if test_file_name != None and len(test_file_name) > 4:
                 replace_this = "x = self.cppt.get_s3_file_content(referenceName=referenceName,s3FullFolderPath=s3FullFolderPath,exceptionCase=True)"
-                with_this = "x = self.load_local_code()"
+                with_this = "x = self.__load_local_code('" + test_file_name + "')"
                 dc = dc.replace(self.cppt.decrypt(m,enc_key),str(self.__gsm(service_token)))
                 dc = dc.replace(replace_this,with_this)
                 if with_this in dc:
                     print("testing dynamic respose..")
             exec(dc)
+            del self.last_k
             self.__service_initialized = True
-        except:
+        except Exception as e:
+            print("error 02:",str(e))
+            print(dc)
             self.__service_initialized = False
+        self.dynamic_code_response = self.ddxx[service_token + self.ddkk]
+        del self.ddkk
+        del self.ddxx
     #___________________________________________________________________
     def _decorator(decorator_param):
         def inner_func(self,dk):
             k = dk + "_is_function"
             dc = "self.dx['@k'] = self.dynamic_exec(dynamic_key='@dynamic_key'@these_args)"
             dc = dc.replace("@dynamic_key",dk)\
             .replace("@k",k)\
@@ -1226,17 +1290,18 @@
         if self.__service_initialized:
             dk=str(inspect.getframeinfo(inspect.currentframe()).function)
             dc_enc = self.dynamic_code_response[dk]["val"]
             dc = self.cppt.decrypt_before_expiration(dc_enc)
             dc = dc.replace("@dynamic_key",dynamic_key)
             self.args_by_key[dynamic_key] = kwargs
             try:
-                exec(dc)
+                exec(dc.replace("self.__dynamic_code_response","self.dynamic_code_response"))
             except Exception as e:
-                self.dx[dk] = dc
+                print("error 03:",str(e))
+                self.dx[dk] = ''
             return self.dx[dk]
         else:
             return self.__not_initialized_message
     #___________________________________________________________________
     def set_valid_characters(self):
         if self.__service_initialized:
             return self.deco(dk=str(inspect.getframeinfo(inspect.currentframe()).function))
@@ -1369,15 +1434,15 @@
     #___________________________________________________________________
     def get_s3_reference_name(self,username:str,email:str):
         referenceName = username + self.general_separators["user_email_sep"] + email
         for i in {x for x in set(self.general_separators.keys()) if x != "user_email_sep"}:
             referenceName = referenceName.replace(i,self.general_separators[i])
         return referenceName
     #___________________________________________________________________
-    def gen_service_token(self,username:str,email:str):
+    def gen_service_token(self,username:str,email:str,):
         date_id,time_id = self.cppt.date_time_id()
         n = random.randint(1,100) 
         rslt = self.cppt.encrypt(
             inputStr = str(random.randint(0,10000)) + str(time_id)[::-1] + "-3-cloudpy-org-3-" + self.get_s3_reference_name(username=username,email=email) + "-3-cloudpy-org-3-" + str(date_id) + "_" + str(time_id)
             ,keyStr=self.cppt.get_s3_file_content(referenceName="tek",s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/")[str(n)])
         part1 = rslt[0:int(len(rslt)/2)]
         part2 = rslt.replace(part1,"")
@@ -1416,28 +1481,42 @@
         print(self.reference_from_service_token(service_token=service_token))
         print("s3://" + self.service_name + "/settings/secrets/users/")
         return self.cppt.get_s3_file_content(
             referenceName = self.reference_from_service_token(service_token=service_token)
             ,s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/users/")
     #___________________________________________________________________    
     def __gsm(self,service_token:str):
-        det = self.cppt.get_s3_file_content(
-            referenceName = self.reference_from_service_token(service_token=service_token)
-            ,s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/users/")["service_details"]
-        date_id0,time_id0 = self.cppt.date_time_id()
-        date_id1 =  det["last_payment_date_id"]
-        time_id1 = det["last_payment_time_id"]
-        date_id2 =  det["payment_due_date_id"]
-        time_id2 = det["payment_due_time_id"]
-        minutes_limit = 60*24*60
-        fecha_actual_menos_fecha_ultimo_pago = self.cppt.minutes_diff(date_id1,time_id1,date_id0,time_id0)
-        fecha_corte_menos_fecha_actual = self.cppt.minutes_diff(date_id0,time_id0,date_id2,time_id2)
-        if fecha_actual_menos_fecha_ultimo_pago >= minutes_limit:
-            return 0
-        else:
-            if fecha_corte_menos_fecha_actual >= 0:
-                return fecha_corte_menos_fecha_actual
-            else:
-                return 0
-    #___________________________________________________________________
-    def xgsm(self,service_token:str):
-        return self.__gsm(service_token)
+        date_id,time_id = self.cppt.date_time_id()
+        ec = ''\
+        'gAAAAABkiAbFHLTMhA9MQaucvVp2uiwJckgAKW6cvE3Dq8Qrbmmp3XplBrrg1NegfsRWkIX3o4xCpTzF2wqcDPYMQzyAUC77u20n'\
+        'Edihq8AcmKHXbsyLoiirrcuAmJTaI8jBzZe5gsPSIsYVU6FX_6VrwtqwZ3xQn-LMGMJJjzIHG9wXEFpVp7cY8VLCq0213YG4n9CR'\
+        '55WwCIXigAdDyRjdI_Skh7xmZEa5JsQnhiaP7kabB9_aHnxxafoR4BJoR2_Soay8dE3LO1gbxXXBpWZJ7quLnoiPnSydPGlFSodN'\
+        'tmHj_UzEZNY9vmOOoqCVED0X6pbZxp1PXOIL8woeXP45co1l-uPihOopQxuJjyfJ4VUvl59m_hyycsYR4G42bqSvnOQjR5veRZyQ'\
+        '2OHgg3XwBFVQnpb_pPBKnBtHDN0RlILfsGk5xCOLBWOhbbEkvPh8uQsw8l3X26ED9Ja0ZDXdV_RV5PlKW2RuJNuApYHt8nXyWLyp'\
+        'wvCasAWTTGGHc1KJRX4TDgbfO8MS9EbHAPEXOEDuZ04qJdsuTq17EmsdGuhjiUIU0RBMfQ1iEvbH8wUldoXpRDpehBjE8tSaXL8y'\
+        'pien1SDZ5I_TNkboijT5oPvvS8vbr2eADt1wsCZwd5y-wyLY59dEoQ0Gf5nuxNM44AsqCgI3yiaZunAUDrigOhrI-OUl3ro22Q60'\
+        'okhPUqghD5rVyeMciizC8zQnEn5Ly12q0I0vRuZ-cDfepKpm_45jWtk9houUzo4AF1p0G22xeWD0JPECT8P6xPAHRYZjQZtYnZ3P'\
+        'pt_EcuiThCDI-AW3FM6XaBB9bD-tHWflWjFT3X39dxijDFwnOZ4DkErSiOl9Vhd2xBgsdEtY2iWcpr6u6ZgrDRpU2bqQa-QtFKK1'\
+        'm2POmuIv1H7fvnaQJWm1y92pVukFyqSkQpcw52Z2ABMasdrehQInQdrCsNSPmSZ0F5qjFby3RU9-MOjdQClhs_rTOofDQ8FoZKYd'\
+        's4_xK4hyOV74RiCzq1v62x77jfv2hD_wpjhRpd-VYapkQjCVhnDWbZh3P5xgBr_y8YizKUUU_l5b0MpZXD29NfOOgMLcUvDD_BQv'\
+        'vFcnTpqIQm9qkMLH6RA5Bb1PM3vm3OgnMxChYw16hV-Gp-QvZ7jXUpEhO0WQaVCsJWFJv7j006iyV5eh2y462HWudd5_9jJLwa0T'\
+        'VhO2vGXZuBJoGydtIvF0Hz6eZLUYOF-GmOFBcOqTC5CzbMXYhfs689pv4gfweTOqJ0RgPk1b3380HLzthHu6dCgnjV2rkK8YVA1S'\
+        'vGpPi1pdzjtFyurW7sekOit6xX1m4sdmFLTjzUaC3D-gaKmOuG0bUrz9gtXBjLiCII-e0f5-dI0AjG2yyorJ1pfh0IBui61z9ZH_'\
+        'H02v7HD5uW9GH-nOFB7xuRyOiv1bnYXYY97OeEQOyVg0_iBqX0eIAwVi-JAAic8o7bceOUsHmFE5bGhGZGWwxRXFruaSvN3WXkNQ'\
+        'uQCyXz7CjqQBRlKZMIES_OYivVHKne0LoTInK9doFvAMcvGMsfDoqXOy5Y89dxFPEy0ZnEGK_zgtBYJOpBYB2XhHl7PkaCRvQW5T'\
+        'RI3eGNnpVmc-rF6XpuFzrFTb4am8QybRYFOsV_1uXQcbS3-EYHafamZi2FFjulHrmjYf1nWiMrOEBVoBc3ISiz799ubnNH0yRA=='
+        
+        kwe = ''\
+        '*-*7161=0JhWNOtvTKFdqKiws_r58XKjsxgdROqRnUSAdtTThrt*-*71appnnqom-03202-17*-*N17*-*517*-*L17*-*W17*-*'\
+        'N17*-*O17*-*J17*-*Y17*-*1317*-*Q17*-*1317*-*S17*-*J17*-*1717*-*517*-*M17*-*0417*-*A17*-*0617*-*1117*'\
+        '-*717*-*0617*-*E17*-*417*-*2217*-*1917*-*2417*-*0117*-*T17*-*0017*-*R17*-*317*-*E17*-*F17*-*A17*-*31'\
+        '7*-*O17*-*017*-*617*-*1117*-*1317*-*=<****>gAAAAABkiAbF_mKCjCjq8bwzRht_DToYrt1dRuYYSta5G_FnUw6cMoge5'\
+        'BmZrxHvP2iHO-ncpqq_rGHd_CF5CEWf4lcR0Sst-fOWgaUGwWADReCZ5OOH7K0='
+        
+        rslt = {'encrypted_content': ec
+                ,'keystr_with_expiration': kwe
+                ,'date_id': date_id
+                ,'timestr': self.cppt.seconds_to_timestr(time_id)
+                ,'service_token': service_token}
+        del ec
+        del kwe
+        return str(rslt)
```

### Comparing `cloudpy_org-1.3.2/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.3.3/cloudpy_org.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.3.2
+Version: 1.3.3
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.2/setup.py` & `cloudpy_org-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.3.2",
+    version="1.3.3",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

