# Comparing `tmp/ibmpairs-0.2.7.tar.gz` & `tmp/ibmpairs-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibmpairs-0.2.7.tar", last modified: Wed Mar 15 13:26:35 2023, max compression
+gzip compressed data, was "ibmpairs-0.2.8.tar", last modified: Tue Jun 13 14:28:44 2023, max compression
```

## Comparing `ibmpairs-0.2.7.tar` & `ibmpairs-0.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-03-15 13:26:35.268056 ibmpairs-0.2.7/
--rw-r--r--   0 staylor    (501) staff       (20)     6699 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/CONTRIBUTING.md
--rw-r--r--   0 staylor    (501) staff       (20)     1488 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/LICENSE
--rw-r--r--   0 staylor    (501) staff       (20)      335 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/MAINTAINERS.md
--rw-r--r--   0 staylor    (501) staff       (20)      281 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/MANIFEST.in
--rw-r--r--   0 staylor    (501) staff       (20)     3270 2023-03-15 13:26:35.268142 ibmpairs-0.2.7/PKG-INFO
--rw-r--r--   0 staylor    (501) staff       (20)     2520 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/README.md
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-03-15 13:26:35.266557 ibmpairs-0.2.7/ibmpairs/
--rw-r--r--   0 staylor    (501) staff       (20)    46025 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/authentication.py
--rw-r--r--   0 staylor    (501) staff       (20)   412432 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/catalog.py
--rw-r--r--   0 staylor    (501) staff       (20)    31564 2023-03-15 13:21:11.000000 ibmpairs-0.2.7/ibmpairs/client.py
--rw-r--r--   0 staylor    (501) staff       (20)    13012 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/common.py
--rw-r--r--   0 staylor    (501) staff       (20)     1112 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/config.py
--rw-r--r--   0 staylor    (501) staff       (20)     4664 2023-03-15 13:21:44.000000 ibmpairs-0.2.7/ibmpairs/constants.py
--rw-r--r--   0 staylor    (501) staff       (20)    15323 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/dashboard.py
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-03-15 13:26:35.267659 ibmpairs-0.2.7/ibmpairs/external/
--rw-r--r--   0 staylor    (501) staff       (20)   102439 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/external/ibm.py
--rw-r--r--   0 staylor    (501) staff       (20)      391 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/logger.py
--rw-r--r--   0 staylor    (501) staff       (20)    25284 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/messages.py
--rw-r--r--   0 staylor    (501) staff       (20)   125490 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/paw.py
--rw-r--r--   0 staylor    (501) staff       (20)   357370 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/query.py
--rw-r--r--   0 staylor    (501) staff       (20)   164223 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/upload.py
--rw-r--r--   0 staylor    (501) staff       (20)    11334 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/ibmpairs/utils.py
--rw-r--r--   0 staylor    (501) staff       (20)       42 2023-03-15 13:26:35.000000 ibmpairs-0.2.7/ibmpairs/version.py
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-03-15 13:26:35.267446 ibmpairs-0.2.7/ibmpairs.egg-info/
--rw-r--r--   0 staylor    (501) staff       (20)     3270 2023-03-15 13:26:35.000000 ibmpairs-0.2.7/ibmpairs.egg-info/PKG-INFO
--rw-r--r--   0 staylor    (501) staff       (20)      619 2023-03-15 13:26:35.000000 ibmpairs-0.2.7/ibmpairs.egg-info/SOURCES.txt
--rw-r--r--   0 staylor    (501) staff       (20)        1 2023-03-15 13:26:35.000000 ibmpairs-0.2.7/ibmpairs.egg-info/dependency_links.txt
--rw-r--r--   0 staylor    (501) staff       (20)        1 2023-03-15 13:26:35.000000 ibmpairs-0.2.7/ibmpairs.egg-info/not-zip-safe
--rw-r--r--   0 staylor    (501) staff       (20)      187 2023-03-15 13:26:35.000000 ibmpairs-0.2.7/ibmpairs.egg-info/requires.txt
--rw-r--r--   0 staylor    (501) staff       (20)        9 2023-03-15 13:26:35.000000 ibmpairs-0.2.7/ibmpairs.egg-info/top_level.txt
--rw-r--r--   0 staylor    (501) staff       (20)       60 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/requirements-development.txt
--rw-r--r--   0 staylor    (501) staff       (20)      184 2023-03-15 13:18:57.000000 ibmpairs-0.2.7/requirements.txt
--rw-r--r--   0 staylor    (501) staff       (20)      103 2023-03-15 13:26:35.268385 ibmpairs-0.2.7/setup.cfg
--rwxr-xr-x   0 staylor    (501) staff       (20)     1838 2023-03-15 13:19:33.000000 ibmpairs-0.2.7/setup.py
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-13 14:28:44.599039 ibmpairs-0.2.8/
+-rw-r--r--   0 staylor    (501) staff       (20)     6699 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/CONTRIBUTING.md
+-rw-r--r--   0 staylor    (501) staff       (20)     1488 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/LICENSE
+-rw-r--r--   0 staylor    (501) staff       (20)      335 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/MAINTAINERS.md
+-rw-r--r--   0 staylor    (501) staff       (20)      281 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/MANIFEST.in
+-rw-r--r--   0 staylor    (501) staff       (20)     3270 2023-06-13 14:28:44.599115 ibmpairs-0.2.8/PKG-INFO
+-rw-r--r--   0 staylor    (501) staff       (20)     2520 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/README.md
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-13 14:28:44.597690 ibmpairs-0.2.8/ibmpairs/
+-rw-r--r--   0 staylor    (501) staff       (20)    63867 2023-06-13 13:01:01.000000 ibmpairs-0.2.8/ibmpairs/authentication.py
+-rw-r--r--   0 staylor    (501) staff       (20)   412432 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/catalog.py
+-rw-r--r--   0 staylor    (501) staff       (20)    40851 2023-06-13 08:16:26.000000 ibmpairs-0.2.8/ibmpairs/client.py
+-rw-r--r--   0 staylor    (501) staff       (20)    13679 2023-06-09 08:29:50.000000 ibmpairs-0.2.8/ibmpairs/common.py
+-rw-r--r--   0 staylor    (501) staff       (20)     1112 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/config.py
+-rw-r--r--   0 staylor    (501) staff       (20)     5189 2023-06-08 14:13:08.000000 ibmpairs-0.2.8/ibmpairs/constants.py
+-rw-r--r--   0 staylor    (501) staff       (20)    16020 2023-06-09 13:08:53.000000 ibmpairs-0.2.8/ibmpairs/dashboard.py
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-13 14:28:44.598803 ibmpairs-0.2.8/ibmpairs/external/
+-rw-r--r--   0 staylor    (501) staff       (20)   102439 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/external/ibm.py
+-rw-r--r--   0 staylor    (501) staff       (20)      391 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/logger.py
+-rw-r--r--   0 staylor    (501) staff       (20)    26501 2023-06-13 09:33:56.000000 ibmpairs-0.2.8/ibmpairs/messages.py
+-rw-r--r--   0 staylor    (501) staff       (20)   166380 2023-05-19 08:50:17.000000 ibmpairs-0.2.8/ibmpairs/paw.py
+-rw-r--r--   0 staylor    (501) staff       (20)   357366 2023-05-18 11:15:15.000000 ibmpairs-0.2.8/ibmpairs/query.py
+-rw-r--r--   0 staylor    (501) staff       (20)   164223 2023-05-18 11:15:34.000000 ibmpairs-0.2.8/ibmpairs/upload.py
+-rw-r--r--   0 staylor    (501) staff       (20)    11334 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/utils.py
+-rw-r--r--   0 staylor    (501) staff       (20)       42 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs/version.py
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-13 14:28:44.598534 ibmpairs-0.2.8/ibmpairs.egg-info/
+-rw-r--r--   0 staylor    (501) staff       (20)     3270 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/PKG-INFO
+-rw-r--r--   0 staylor    (501) staff       (20)      619 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/SOURCES.txt
+-rw-r--r--   0 staylor    (501) staff       (20)        1 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/dependency_links.txt
+-rw-r--r--   0 staylor    (501) staff       (20)        1 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/not-zip-safe
+-rw-r--r--   0 staylor    (501) staff       (20)      187 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/requires.txt
+-rw-r--r--   0 staylor    (501) staff       (20)        9 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/top_level.txt
+-rw-r--r--   0 staylor    (501) staff       (20)       60 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/requirements-development.txt
+-rw-r--r--   0 staylor    (501) staff       (20)      184 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/requirements.txt
+-rw-r--r--   0 staylor    (501) staff       (20)      103 2023-06-13 14:28:44.599427 ibmpairs-0.2.8/setup.cfg
+-rwxr-xr-x   0 staylor    (501) staff       (20)     1838 2023-06-13 14:24:49.000000 ibmpairs-0.2.8/setup.py
```

### Comparing `ibmpairs-0.2.7/CONTRIBUTING.md` & `ibmpairs-0.2.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.7/LICENSE` & `ibmpairs-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.7/PKG-INFO` & `ibmpairs-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmpairs
-Version: 0.2.7
+Version: 0.2.8
 Summary: open source Python modules for the IBM PAIRS Geoscope platform
 Home-page: https://ibmpairs.mybluemix.net
 Author: Physical Analytics, IBM Research
 Author-email: pairs@us.ibm.com
 Maintainer: cmalbrec
 License: BSD-Clause-3
 Project-URL: Documentation, https://pairs.res.ibm.com/tutorial
```

### Comparing `ibmpairs-0.2.7/README.md` & `ibmpairs-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.7/ibmpairs/authentication.py` & `ibmpairs-0.2.8/ibmpairs/authentication.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,32 +27,41 @@
 #}}}
 
 # fold: String Literals {{{
 PAIRS_DEFAULT_PASSWORD_FILE_NAME    = u'auth/basic.txt'
 PAIRS_PASSWORD_FILE_COMMENT_REG_EX  = re.compile(r'^\s*#')
 #}}}
 
+GLOBAL_LEGACY_ENVIRONMENT      = os.environ.get('GLOBAL_LEGACY_ENVIRONMENT', "True")
+if GLOBAL_LEGACY_ENVIRONMENT.lower() in ('true', 't', 'yes', 'y'):
+    GLOBAL_LEGACY_ENVIRONMENT  = True
+else:
+    GLOBAL_LEGACY_ENVIRONMENT  = False
+
 # fold: Basic Class {{{
 class Basic:
     #_host: str
     #_username: str
     #_password: str
     #_password_file: str
+    #_legacy: bool
     
     """
     An object to represent basic credentials and recovery from a file.
 
-    :param host:             IBM PAIRS host, defaults to https://pairs.res.ibm.com
+    :param host:             IBM PAIRS host
     :type host:              str
     :param username:         IBM PAIRS username
     :type username:          str
     :param password:         IBM PAIRS password
     :type password:          str
     :param password_file:    IBM PAIRS password file, defaults to auth/basic.txt
     :type password_file:     str
+    :param legacy:           IBM EIS GA Legacy Environment selector override
+    :type legacy:            bool
     :raises Exception:       if username and password are not present
     """
     
     #
     def __str__(self):
         
         """
@@ -88,23 +97,41 @@
         
         return json.dumps(return_dict, 
                           indent    = constants.GLOBAL_JSON_REPR_INDENT, 
                           sort_keys = constants.GLOBAL_JSON_REPR_SORT_KEYS)
     
     #
     def __init__(self,
-                 host: str          = constants.CLIENT_PAIRS_URL,
+                 host: str          = None,
                  username: str      = None,
                  password: str      = None,
-                 password_file: str = "auth/basic.txt"
+                 password_file: str = "auth/basic.txt",
+                 legacy: bool       = None
                 ):
-        self._host          = common.strip_protocol(host)
+        
+        if legacy is not None:
+            self._legacy = legacy
+        else:
+            self._legacy = GLOBAL_LEGACY_ENVIRONMENT
+        
+        if host is not None:
+            self._host = common.strip_protocol(host)
+        else:
+            if self._legacy is True:
+                self._host = common.strip_protocol(constants.CLIENT_LEGACY_URL)
+            else:
+                self._host = common.strip_protocol(constants.CLIENT_URL)
+        
         self._username      = username
         self._password      = password
-        self._password_file = password_file
+        
+        if password_file is not None:
+            self._password_file = password_file
+        else:
+            self._password_file = "auth/basic.txt"
         
         if ((self._password is None) and (self._username is not None)):
             try:
                 self.set_credentials_from_file(self._username, self._password_file, self._host)
             except Exception as e:
                 msg = messages.INFO_AUTHENTICATION_PASSWORD_NOT_FOUND_IN_FILE.format(self._username, self._password_file, self._host)
                 logger.info(msg)
@@ -179,14 +206,29 @@
         
     #    
     def del_password_file(self): 
         del self._password_file
 
     #    
     password_file = property(get_password_file, set_password_file, del_password_file)
+    
+    #
+    def get_legacy(self):
+        return self._legacy
+    
+    #
+    def set_legacy(self, legacy):
+        self._legacy = common.check_bool(legacy)
+        
+    #    
+    def del_legacy(self): 
+        del self._legacy
+        
+    #    
+    legacy = property(get_legacy, set_legacy, del_legacy)
 
     #
     def set_credentials(self, username, password):
         self.set_username(username)
         self.set_password(password)
         
     #
@@ -253,33 +295,37 @@
         
         :param authentication_dict: A dictionary that contains the keys of a Basic object.
         :type authentication_dict:  Any             
         :rtype:                     ibmpairs.authentication.Basic
         :raises Exception:          if not a dictionary.
         """
         
-        username = None
-        password = None
+        username      = None
+        password      = None
         password_file = None
-        host = None
+        host          = None
+        legacy        = None
         
         common.check_dict(authentication_dict)
         if "host" in authentication_dict:
             host = common.check_str(authentication_dict.get("host"))
         if "username" in authentication_dict:
             username = common.check_str(authentication_dict.get("username"))
         if "password" in authentication_dict:
             password = common.check_str(authentication_dict.get("password"))
         if "password_file" in authentication_dict:
             password_file = common.check_str(authentication_dict.get("password_file"))
+        if "legacy" in authentication_dict:
+            legacy = common.check_bool(authentication_dict.get("legacy"))
             
         return Basic(host          = host,
                      username      = username,
                      password      = password,
-                     password_file = password_file
+                     password_file = password_file,
+                     legacy        = legacy
                     )
 
     #
     def to_dict(self):
       
         """
         Create a dictionary from the objects structure.  
@@ -292,14 +338,16 @@
             authentication_dict["host"] = self._host
         if self._username is not None:
             authentication_dict["username"] = self._username
         if self._password is not None:
             authentication_dict["password"] = self._password
         if self._password_file is not None:
             authentication_dict["password_file"] = self._password_file
+        if self._legacy is not None:
+            authentication_dict["legacy"] = self._legacy
         return authentication_dict
     
     #
     def from_json(basic_json: Any):
 
         """
         Create an Basic object from json (dictonary or str).
@@ -336,14 +384,16 @@
 class OAuth2Return:
     #_access_token: str
     #_expires_in: int
     #_token_type: str
     #_refresh_token: str
     #_scope: str
     #_error: str
+    #_expiration: int
+    #_ims_user_id: int
     
     """
     An object to represent the return provided by a Phoenix OAuth2 call.
 
     :param access_token:     An access_token (JWT)
     :type access_token:      str
     :param expires_in:       An expiration time (seconds)
@@ -352,14 +402,18 @@
     :type token_type:        str
     :param refresh_token:    A refresh token
     :type refresh_token:     str
     :param scope:            The scope of the token
     :type scope:             str
     :param error:            An error message
     :type error:             str
+    :param expiration:       The expiration timestamp (UNIX)
+    :type expiration:        int
+    :param ims_user_id:      IMS User Id
+    :type ims_user_id:       int
     :raises Exception:       if username and password are not present
     """
     
     #
     def __str__(self):
         
         """
@@ -389,22 +443,26 @@
     
     def __init__(self,
                  access_token: str  = None,
                  expires_in: int    = None,
                  token_type: str    = None,
                  refresh_token: str = None,
                  scope: str         = None,
-                 error: str         = None
+                 error: str         = None,
+                 expiration: int    = None,
+                 ims_user_id: int   = None
                 ):
         self._access_token  = access_token
         self._expires_in    = expires_in
         self._token_type    = token_type
         self._refresh_token = refresh_token
         self._scope         = scope
         self._error         = error
+        self._expiration    = expiration
+        self._ims_user_id   = ims_user_id
         
     #
     def get_access_token(self):
         return self._access_token
 
     #
     def set_access_token(self, access_token):
@@ -487,14 +545,44 @@
         
     #    
     def del_error(self): 
         del self._error
 
     #    
     error = property(get_error, set_error, del_error)
+
+    #
+    def get_expiration(self):
+        return self._expiration
+    
+    #
+    def set_expiration(self, expiration):
+        self._expiration = common.check_int(expiration)
+        
+    #    
+    def del_expiration(self): 
+        del self._expiration
+        
+    #    
+    expiration = property(get_expiration, set_expiration, del_expiration)
+    
+    #
+    def get_ims_user_id(self):
+        return self._ims_user_id
+    
+    #
+    def set_ims_user_id(self, ims_user_id):
+        self._ims_user_id = common.check_int(ims_user_id)
+        
+    #    
+    def del_ims_user_id(self): 
+        del self._ims_user_id
+        
+    #    
+    ims_user_id = property(get_ims_user_id, set_ims_user_id, del_ims_user_id)
     
     #
     def from_dict(oauth2_return_dict: Any):
         
         """
         Create an OAuth2Return object from a dictionary.
         
@@ -506,14 +594,16 @@
         
         access_token  = None
         expires_in    = None
         token_type    = None
         refresh_token = None
         scope         = None
         error         = None
+        expiration    = None
+        ims_user_id   = None
         
         common.check_dict(oauth2_return_dict)
         if "access_token" in oauth2_return_dict:
             if oauth2_return_dict.get("access_token") is not None:
                 access_token = common.check_str(oauth2_return_dict.get("access_token"))
         if "expires_in" in oauth2_return_dict:
             if oauth2_return_dict.get("expires_in") is not None:
@@ -526,21 +616,29 @@
                 refresh_token = common.check_str(oauth2_return_dict.get("refresh_token"))
         if "scope" in oauth2_return_dict:
             if oauth2_return_dict.get("scope") is not None:
                 scope = common.check_str(oauth2_return_dict.get("scope"))
         if "error" in oauth2_return_dict:
             if oauth2_return_dict.get("error") is not None:
                 error = common.check_str(oauth2_return_dict.get("error"))
+        if "expiration" in oauth2_return_dict:
+            if oauth2_return_dict.get("expiration") is not None:
+                expiration = common.check_int(oauth2_return_dict.get("expiration"))
+        if "ims_user_id" in oauth2_return_dict:
+            if oauth2_return_dict.get("ims_user_id") is not None:
+                ims_user_id = common.check_int(oauth2_return_dict.get("ims_user_id"))
             
         return OAuth2Return(access_token  = access_token,
                             expires_in    = expires_in,
                             token_type    = token_type,
                             refresh_token = refresh_token,
                             scope         = scope,
-                            error         = error
+                            error         = error,
+                            expiration    = expiration,
+                            ims_user_id   = ims_user_id
                            )
 
     #
     def to_dict(self):
       
         """
         Create a dictionary from the objects structure. 
@@ -557,23 +655,27 @@
             oauth2_return_dict["token_type"] = self._token_type
         if self._refresh_token is not None:
             oauth2_return_dict["refresh_token"] = self._refresh_token
         if self._scope is not None:
             oauth2_return_dict["scope"] = self._scope
         if self._error is not None:
             oauth2_return_dict["error"] = self._error
+        if self._expiration is not None:
+            oauth2_return_dict["expiration"] = self._expiration
+        if self._ims_user_id is not None:
+            oauth2_return_dict["ims_user_id"] = self._ims_user_id
         return oauth2_return_dict
         
     #
     def from_json(oauth2_return_json: Any):
 
         """
-        Create an OAuth2Return object from json (dictonary or str).
+        Create a OAuth2Return object from json (dictonary or str).
         
-        :param oauth2_return_dict: A json dictionary that contains the keys of an OAuth2Return or a string representation of a json dictionary.
+        :param oauth2_return_dict: A json dictionary that contains the keys of a OAuth2Return or a string representation of a json dictionary.
         :type oauth2_return_dict:  Any             
         :rtype:                    ibmpairs.authentication.OAuth2Return
         :raises Exception:         if not a dictionary or a string.
         """
 
         if isinstance(oauth2_return_json, dict):
             oauth2_return = OAuth2Return.from_dict(oauth2_return_json)
@@ -603,34 +705,45 @@
     #_host: str
     #_username: str
     #_api_key: str
     #_api_key_file: str
     #_client_id: str
     #_endpoint: str
     #_jwt_token: str
-    
     #_oauth2_return: OAuth2Return
+    #_iam_endpoint: str
+    #_org_id: str
+    #_tenant_id: str
+    #_legacy: bool
     
     """
     An object to represent OAuth2 credentials and recovery from a file.
     
-    :param host:         IBM PAIRS host, defaults to https://pairs.res.ibm.com
+    :param host:         IBM PAIRS host
     :type host:          str
     :param username:     IBM PAIRS username
     :type username:      str
     :param api_key:      IBM PAIRS API key
     :type api_key:       str
     :param api_key_file: IBM PAIRS API key file, defaults to auth/oauth2.txt
     :type api_key_file:  str
-    :param client_id:    A client id for the authentication system, defaults to 'ibm-pairs'.
+    :param client_id:    A client id for the authentication system, defaults to 'ibm-pairs' if legacy.
     :type client_id:     str
     :param endpoint:     The authentication endpoint.
     :type endpoint:      str
     :param jwt_token:    A jwt token for authentication.
     :type jwt_token:     str
+    :param iam_endpoint: IBM Cloud IAM Endpoint
+    :type iam_endpoint:  str
+    :param org_id:       IBM EIS GA API Connect Org Id
+    :type org_id:        str
+    :param tenant_id:    IBM EIS GA API Connect Tenant Id
+    :type tenant_id:     str
+    :param legacy:       IBM EIS GA Legacy Environment selector override
+    :type legacy:        bool
     :returns:            None
     :rtype:              None
     :raises Exception:   if an api key cannot be acquired from the information provided
     """
     
     #
     def __str__(self):
@@ -672,48 +785,118 @@
         
         return json.dumps(return_dict, 
                           indent    = constants.GLOBAL_JSON_REPR_INDENT, 
                           sort_keys = constants.GLOBAL_JSON_REPR_SORT_KEYS)
 
     #
     def __init__(self,
-                 host: str         = constants.CLIENT_PAIRS_URL,
+                 host: str         = None,
                  username: str     = None,
                  api_key: str      = None,
                  api_key_file: str = "auth/oauth2.txt",
-                 client_id: str    = "ibm-pairs",
-                 endpoint: str     = "auth-b2b-twc.ibm.com",
+                 client_id: str    = None,
+                 endpoint: str     = None, #"auth-b2b-twc.ibm.com", #"api.ibm.com"
                  jwt_token: str    = None,
+                 iam_endpoint: str = "iam.cloud.ibm.com",
+                 org_id: str       = None, 
+                 tenant_id: str    = None,
+                 legacy: bool      = None
                 ):
-
-        self._host          = common.strip_protocol(host)
+        
+        if legacy is not None:
+            self._legacy = legacy
+        else:
+            self._legacy = GLOBAL_LEGACY_ENVIRONMENT
+        
+        if host is not None:
+            self._host = common.strip_protocol(host)
+        else:
+            if self._legacy is True:
+                self._host = common.strip_protocol(constants.CLIENT_LEGACY_URL)
+            else:
+                self._host = common.strip_protocol(constants.CLIENT_URL)
+        
         self._username      = username
         self._api_key       = api_key
         self._api_key_file  = api_key_file
-        self._client_id     = client_id
-        self._endpoint      = endpoint
+        
+        if self._legacy is True:
+            if client_id is not None:
+                self._client_id = client_id
+            else:
+                self._client_id = 'ibm-pairs'
+            self._tenant_id = tenant_id
+        else:
+            if (client_id is not None) and (tenant_id is not None):
+                msg = messages.INFO_BOTH_CLIENT_ID_AND_TENANT_ID.format(client_id, tenant_id)
+                logger.info(msg)
+                if client_id.startswith('geospatial-'):
+                    msg = messages.INFO_STARTS_WITH_GEOSPATIAL
+                    logger.info(msg)
+                    self._client_id = 'saascore-' + common.get_tenant_id(client_id)
+                else:
+                    self._client_id = client_id
+                self._tenant_id = common.get_tenant_id(client_id)
+            elif (client_id is not None) and (tenant_id is None):
+                if client_id.startswith('geospatial-'):
+                    msg = messages.INFO_STARTS_WITH_GEOSPATIAL
+                    logger.info(msg)
+                    self._client_id = 'saascore-' + common.get_tenant_id(client_id)
+                else:
+                    self._client_id = client_id
+                self._tenant_id = common.get_tenant_id(client_id)
+            elif (client_id is None) and (tenant_id is not None):
+                self._tenant_id = common.get_tenant_id(tenant_id)
+                self._client_id = 'saascore-' + self._tenant_id
+            else:
+                msg = messages.ERROR_NO_CLIENT_OR_TENANT_ID
+                logger.error(msg)
+                raise common.PAWException(msg)
+                
+        if endpoint is not None:
+            self._endpoint = endpoint
+        else:
+            if self._legacy is True:
+                self._endpoint = 'auth-b2b-twc.ibm.com'
+            else:
+                self._endpoint = 'api.ibm.com'
+
         self._jwt_token     = jwt_token
         
         self._oauth2_return = OAuth2Return()
         
+        self._iam_endpoint  = iam_endpoint
+        
+        if self._legacy is True:
+            self._org_id = org_id
+        else:
+            if org_id is not None:
+                self._org_id = org_id
+            else:
+                msg = messages.ERROR_NO_ORG_ID
+                logger.error(msg)
+                raise common.PAWException(msg)
+        
         if ((self._api_key is None) and (self._username is not None)):
             try:
                 self.set_credentials_from_file(self._username,
                                                self._api_key_file, 
                                                self._host
                                               )
             except:
                 msg = messages.INFO_AUTHENTICATION_API_KEY_NOT_FOUND_IN_FILE.format(self._username, self._api_key_file, self._host)
                 logger.info(msg)
         
         if (self._api_key is not None):
             try:
-                self.get_auth_token(api_key   = self._api_key,
-                                    client_id = self._client_id, 
-                                    endpoint  = self._endpoint
+                self.get_auth_token(api_key      = self._api_key,
+                                    client_id    = self._client_id, 
+                                    endpoint     = self._endpoint,
+                                    iam_endpoint = self._iam_endpoint,
+                                    org_id       = self._org_id
                                    )
             except Exception as ex:
                 msg = messages.INFO_AUTHENTICATION_COULD_NOT_GET_AUTH_TOKEN.format(api_key, ex)
                 logger.info(msg)
                 
         if self._jwt_token is None:
             msg = messages.ERROR_AUTHENTICATION_FAILED.format("JWT token")
@@ -845,14 +1028,78 @@
     def del_oauth2_return(self): 
         del self._oauth2_return
 
     #    
     oauth2_return = property(get_oauth2_return, set_oauth2_return, del_oauth2_return) 
     
     #
+    def get_iam_endpoint(self):
+        return self._iam_endpoint
+    
+    #
+    def get_iam_endpoint(self):
+        return self._iam_endpoint
+    
+    #
+    def set_iam_endpoint(self, iam_endpoint):
+        self._iam_endpoint = common.check_str(iam_endpoint)
+        
+    #    
+    def del_iam_endpoint(self): 
+        del self._iam_endpoint
+        
+    #    
+    iam_endpoint = property(get_iam_endpoint, set_iam_endpoint, del_iam_endpoint)
+    
+    #
+    def get_org_id(self):
+        return self._org_id
+    
+    #
+    def set_org_id(self, org_id):
+        self._org_id = common.check_str(org_id)
+        
+    #    
+    def del_org_id(self): 
+        del self._org_id
+        
+    #    
+    org_id = property(get_org_id, set_org_id, del_org_id)
+    
+    #
+    def get_tenant_id(self):
+        return self._tenant_id
+    
+    #
+    def set_tenant_id(self, tenant_id):
+        self._tenant_id = common.check_str(tenant_id)
+        
+    #    
+    def del_tenant_id(self): 
+        del self._tenant_id
+        
+    #    
+    tenant_id = property(get_tenant_id, set_tenant_id, del_tenant_id)
+    
+    #
+    def get_legacy(self):
+        return self._legacy
+    
+    #
+    def set_legacy(self, legacy):
+        self._legacy = common.check_bool(legacy)
+        
+    #    
+    def del_legacy(self): 
+        del self._legacy
+        
+    #    
+    legacy = property(get_legacy, set_legacy, del_legacy)
+    
+    #
     def set_credentials_from_file(self, 
                                   username, 
                                   api_key_file, 
                                   host
                                  ):
         
         """
@@ -872,30 +1119,32 @@
         self.set_api_key(get_password_from_file(server   = self._host,
                                                 user     = self._username,
                                                 passFile = self._api_key_file
                                                )
                         )
     
     #
-    def get_auth_token(self, 
-                       api_key   = None, 
-                       client_id = None, 
-                       endpoint  = None,
-                       verify    = constants.GLOBAL_SSL_VERIFY
-                      ):
+    def phoenix_get_auth_token(self, 
+                               api_key   = None, 
+                               client_id = None, 
+                               endpoint  = None,
+                               verify    = constants.GLOBAL_SSL_VERIFY
+                              ):
         
         """
         The method submits a request to the authentication system and obtains a response.
         
         :param api_key:   An api key for the authentication system.
         :type api_key:    str
         :param client_id: A client id for the authentication system.
         :type client_id:  str
         :param endpoint:  The authentication endpoint.
         :type endpoint:   str
+        :param verify:    Verify ssl.
+        :type verify:     boolean
         """
         
         response               = None
         response_oauth2_return = None
         
         if api_key is not None:
             self.set_api_key(api_key)
@@ -928,37 +1177,41 @@
             logger.error(msg)
             raise common.PAWException(msg)
             
         if response.status_code == 200:
             try:
                 response_oauth2_return = oauth2_return_from_dict(response.json())
             except Exception as ex:
-                msg = messages.ERROR_AUTHENTICATION_PHOENIX_RETURN_NOT_OAUTH2RETURN.format("Phoenix GetBearerForClient", response.json(), ex)
+                msg = messages.ERROR_AUTHENTICATION_RETURN_NOT_OAUTH2RETURN.format("Phoenix GetBearerForClient", response.json(), ex)
                 logger.error(msg)
                 raise common.PAWException(msg)
             
             if response_oauth2_return.error is None:
                 self.set_jwt_token(response_oauth2_return.access_token)
                 self.set_oauth2_return(response_oauth2_return)
             else:
-                msg = messages.ERROR_AUTHENTICATION_PHOENIX_200_RETURN_ERROR.format("Phoenix GetBearerForClient", response_oauth2_return.error)
+                msg = messages.ERROR_AUTHENTICATION_200_RETURN_ERROR.format("Phoenix GetBearerForClient", response_oauth2_return.error)
                 logger.error(msg)
                 raise common.PAWException(msg)
                 
         else:
-            msg = messages.ERROR_AUTHENTICATION_PHOENIX_NOT_SUCCESSFUL.format("Phoenix GetBearerForClient", str(response))
+            msg = messages.ERROR_AUTHENTICATION_NOT_SUCCESSFUL.format("Phoenix GetBearerForClient", str(response))
             logger.error(msg)
             raise common.PAWException(msg)
 
-    def refresh_auth_token(self,
-                           verify    = constants.GLOBAL_SSL_VERIFY
-                          ):
+    #
+    def phoenix_refresh_auth_token(self,
+                                   verify    = constants.GLOBAL_SSL_VERIFY
+                                  ):
         
         """
         The method submits a request to the authentication system for a refreshed token, gets a response and updates the internal self._oauth2_return and self._jwt_token objects.
+
+        :param verify:       Verify ssl.
+        :type verify:        boolean
         """
         
         msg = messages.INFO_AUTHENTICATION_TOKEN_REFRESH
         logger.info(msg)
         
         response               = None
         response_oauth2_return = None
@@ -985,32 +1238,204 @@
             logger.error(msg)
             raise common.PAWException(msg)
             
         if response.status_code == 200:
             try:
                 response_oauth2_return = oauth2_return_from_dict(response.json())
             except:
-                msg = messages.ERROR_AUTHENTICATION_PHOENIX_RETURN_NOT_OAUTH2RETURN.format("/connect/token", response.json())
+                msg = messages.ERROR_AUTHENTICATION_RETURN_NOT_OAUTH2RETURN.format("/connect/token", response.json())
                 logger.error(msg)
                 raise common.PAWException(msg)
             
             if response_oauth2_return.error is None:
                 self.set_jwt_token(response_oauth2_return.access_token)
                 self.set_oauth2_return(response_oauth2_return)
                 msg = messages.INFO_AUTHENTICATION_TOKEN_REFRESH_SUCCESS
                 logger.info(msg)
             else:
-                msg = messages.ERROR_AUTHENTICATION_PHOENIX_REFRESH_200_RETURN_ERROR.format("/connect/token", response_oauth2_return.error)
+                msg = messages.ERROR_AUTHENTICATION_REFRESH_200_RETURN_ERROR.format("/connect/token", response_oauth2_return.error)
+                logger.error(msg)
+                raise common.PAWException(msg)
+                
+        else:
+            msg = messages.ERROR_AUTHENTICATION_NOT_SUCCESSFUL.format("/connect/token", str(response))
+            logger.error(msg)
+            raise common.PAWException(msg)
+            
+    #
+    def api_connect_get_auth_token(self, 
+                                   api_key      = None, 
+                                   client_id    = None, 
+                                   endpoint     = None,
+                                   verify       = constants.GLOBAL_SSL_VERIFY,
+                                   iam_endpoint = None,
+                                   org_id       = None,
+                                   tenant_id    = None
+                                  ):
+        
+        """
+        The method submits a request to the authentication system and obtains a response.
+        
+        :param api_key:      An api key for the authentication system.
+        :type api_key:       str
+        :param client_id:    A client id for the authentication system.
+        :type client_id:     str
+        :param endpoint:     The authentication endpoint.
+        :type endpoint:      str
+        :param verify:       Verify ssl.
+        :type verify:        boolean
+        :param iam_endpoint: IBM Cloud IAM Endpoint
+        :type iam_endpoint:  str
+        :param org_id:       IBM EIS GA API Connect Org Id
+        :type org_id:        str
+        :param tenant_id:    IBM EIS GA API Connect Tenant Id
+        :type tenant_id:     str
+        """
+
+        response               = None
+        response_oauth2_return = None
+        
+        if api_key is not None:
+            self.set_api_key(api_key)
+        if client_id is not None:
+            self.set_client_id(client_id)
+        if tenant_id is not None:
+            self.set_tenant_id(tenant_id)
+            self.set_client_id('saascore-'+tenant_id)
+        if endpoint is not None:
+            self.set_endpoint(endpoint)
+        if iam_endpoint is not None:
+            self.set_iam_endpoint(iam_endpoint)
+        if org_id is not None:
+            self.set_org_id(org_id)
+
+        if (self._api_key is not None) and (self._client_id is not None) and (self._org_id is not None):
+            
+            iam_request_headers: dict           = {}
+            iam_request_headers["Content-Type"] = "application/x-www-form-urlencoded"
+            
+            body = 'grant_type=urn:ibm:params:oauth:grant-type:apikey&apikey={}'.format(self.get_api_key())
+
+            iam_response = requests.post("https://" + 
+                                             self.get_iam_endpoint() +
+                                             "/identity/token",
+                                         headers = iam_request_headers,
+                                         data    = body,
+                                         verify  = verify
+                                        )
+        else:
+            msg = messages.ERROR_AUTHENTICATION_IAM_NO_API_KEY_OR_CLIENT_ID
+            logger.error(msg)
+            raise common.PAWException(msg)
+            
+        if iam_response.status_code == 200:
+            try:
+                response_oauth2_return = oauth2_return_from_dict(iam_response.json())
+            except Exception as ex:
+                msg = messages.ERROR_AUTHENTICATION_RETURN_NOT_OAUTH2RETURN.format("IBM Cloud IAM", iam_response.json(), ex)
+                logger.error(msg)
+                raise common.PAWException(msg)
+
+            if response_oauth2_return.error is None:
+                self.set_oauth2_return(response_oauth2_return)
+            else:
+                msg = messages.ERROR_AUTHENTICATION_200_RETURN_ERROR.format("IBM Cloud IAM", iam_response.status_code)
                 logger.error(msg)
                 raise common.PAWException(msg)
                 
+            if (self.get_oauth2_return().get_access_token() is not None):
+                
+                request_headers: dict              = {}
+                request_headers["X-IBM-Client-Id"] = self.get_client_id()
+                token = 'Bearer ' + response_oauth2_return.get_access_token()
+                request_headers["Authorization"] = token
+                
+                response = requests.get("https://" + 
+                                            self.get_endpoint() +
+                                            "/saascore/run/authentication-retrieve?orgId=" +
+                                            self.get_org_id(),
+                                        headers = request_headers,
+                                        verify  = verify
+                                       )
+
+                if response.status_code == 200:
+                    self.set_jwt_token(response.text)
+                else:
+                    oauth_error_json = {"error": str(response.json()["httpMessage"]) + ': ' + str(response.json()["moreInformation"])}
+                    self.set_oauth2_return(oauth2_return_from_json(oauth_error_json))
+                    
+                    msg = messages.ERROR_AUTHENTICATION_NOT_SUCCESSFUL_API_CONNECT.format("IBM API Connect", str(response.status_code), self.get_oauth2_return().get_error())
+                    logger.error(msg)
+                    raise common.PAWException(msg)
+
+            else:
+                msg = messages.ERROR_AUTHENTICATION_NO_ACCESS_TOKEN.format("IBM API Connect", self.get_oauth2_return().to_json())
+                logger.error(msg)
+                raise common.PAWException(msg)
+
         else:
-            msg = messages.ERROR_AUTHENTICATION_PHOENIX_NOT_SUCCESSFUL.format("/connect/token", str(response))
+            oauth_error_json = {"error": str(iam_response.json()["errorCode"]) + ' ' + str(iam_response.json()["errorMessage"])}
+            self.set_oauth2_return(oauth2_return_from_json(oauth_error_json))
+            
+            msg = messages.ERROR_AUTHENTICATION_NOT_SUCCESSFUL_API_CONNECT.format("IBM Cloud IAM", str(iam_response.status_code), self.get_oauth2_return().get_error())
             logger.error(msg)
             raise common.PAWException(msg)
+
+    #
+    def api_connect_refresh_auth_token(self,
+                                       verify = constants.GLOBAL_SSL_VERIFY
+                                      ):
+        
+        """
+        The method performs a new api_connect_get_auth_token.
+
+        :param verify:       Verify ssl.
+        :type verify:        boolean
+        """
+        
+        self.api_connect_get_auth_token()
+        
+    #
+    def get_auth_token(self, 
+                       api_key      = None, 
+                       client_id    = None,
+                       endpoint     = None,
+                       verify       = constants.GLOBAL_SSL_VERIFY,
+                       iam_endpoint = None,
+                       org_id       = None,
+                       tenant_id    = None
+                      ):
+        
+        if self._legacy is True:
+            logger.info("Legacy Environment is True")
+            self.phoenix_get_auth_token(api_key   = api_key, 
+                                        client_id = client_id, 
+                                        endpoint  = endpoint,
+                                        verify    = verify
+                                       )
+        else:
+            logger.info("Legacy Environment is False")
+            self.api_connect_get_auth_token(api_key      = api_key, 
+                                            client_id    = client_id,
+                                            endpoint     = endpoint,
+                                            verify       = verify,
+                                            iam_endpoint = iam_endpoint,
+                                            org_id       = org_id,
+                                            tenant_id    = tenant_id
+                                           )
+            
+    #
+    def refresh_auth_token(self,
+                           verify = constants.GLOBAL_SSL_VERIFY
+                          ):
+        
+        if self._legacy is True:
+            self.phoenix_refresh_auth_token()
+        else:
+            self.api_connect_refresh_auth_token()
     
     #
     def from_dict(authentication_dict: Any):
         
         """
         Create a OAuth2 authentication object from a dictionary.
         
@@ -1023,14 +1448,18 @@
         host         = None
         username     = None
         api_key      = None
         api_key_file = None
         client_id    = None
         endpoint     = None
         jwt_token    = None
+        iam_endpoint = None
+        org_id       = None
+        tenant_id    = None
+        legacy       = None
         
         common.check_dict(authentication_dict)
         if "host" in authentication_dict:
             if authentication_dict.get("host") is not None:
                 host = common.check_str(authentication_dict.get("host"))
         if "username" in authentication_dict:
             if authentication_dict.get("username") is not None:
@@ -1046,22 +1475,44 @@
                 client_id = common.check_str(authentication_dict.get("client_id"))
         if "endpoint" in authentication_dict:
             if authentication_dict.get("endpoint") is not None:
                 endpoint = common.check_str(authentication_dict.get("endpoint"))
         if "jwt_token" in authentication_dict:
             if authentication_dict.get("jwt_token") is not None:
                 jwt_token = common.check_str(authentication_dict.get("jwt_token"))
+        if "iam_endpoint" in authentication_dict:
+            if authentication_dict.get("iam_endpoint") is not None:
+                iam_endpoint = common.check_str(authentication_dict.get("iam_endpoint"))
+        if "orgId" in authentication_dict:
+            if authentication_dict.get("orgId") is not None:
+                org_id = common.check_str(authentication_dict.get("orgId"))
+        elif "org_id" in authentication_dict:
+            if authentication_dict.get("org_id") is not None:
+                org_id = common.check_str(authentication_dict.get("org_id"))
+        if "tenantId" in authentication_dict:
+            if authentication_dict.get("tenantId") is not None:
+                tenant_id = common.check_str(authentication_dict.get("tenantId"))
+        elif "tenant_id" in authentication_dict:
+            if authentication_dict.get("tenant_id") is not None:
+                tenant_id = common.check_str(authentication_dict.get("tenant_id"))
+        if "legacy" in authentication_dict:
+            if authentication_dict.get("legacy") is not None:
+                legacy = common.check_str(authentication_dict.get("legacy"))
             
         return OAuth2(host,
                       username,
                       api_key,
                       api_key_file,
                       client_id,
                       endpoint,
-                      jwt_token
+                      jwt_token,
+                      iam_endpoint,
+                      org_id,
+                      tenant_id,
+                      legacy
                      )
 
     #
     def to_dict(self):
       
         """
         Create a dictionary from the objects structure.  
@@ -1082,23 +1533,31 @@
             authentication_dict["client_id"] = self._client_id
         if self._endpoint is not None:
             authentication_dict["endpoint"] = self._endpoint
         if self._jwt_token is not None:
             authentication_dict["jwt_token"] = self._jwt_token
         if self._oauth2_return is not None:
             authentication_dict["oauth2_return"] = common.class_to_dict(self._oauth2_return, OAuth2Return)
+        if self._iam_endpoint is not None:
+            authentication_dict["iam_endpoint"] = self._iam_endpoint
+        if self._org_id is not None:
+            authentication_dict["org_id"] = self._org_id
+        if self._tenant_id is not None:
+            authentication_dict["tenant_id"] = self._tenant_id
+        if self._legacy is not None:
+            authentication_dict["legacy"] = self._legacy
         return authentication_dict
     
     #
     def from_json(oauth2_json: Any):
 
         """
         Create an OAuth2 object from json (dictonary or str).
         
-        :param oauth2_dict: A json dictionary that contains the keys of an OAuth2 or a string representation of a json dictionary.
+        :param oauth2_dict: A json dictionary that contains the keys of a OAuth2 or a string representation of a json dictionary.
         :type oauth2_dict:  Any             
         :rtype:             ibmpairs.authentication.OAuth2
         :raises Exception:  if not a dictionary or a string.
         """
 
         if isinstance(oauth2_json, dict):
             oauth2 = OAuth2.from_dict(oauth2_json)
```

### Comparing `ibmpairs-0.2.7/ibmpairs/catalog.py` & `ibmpairs-0.2.8/ibmpairs/catalog.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.7/ibmpairs/client.py` & `ibmpairs-0.2.8/ibmpairs/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,14 +28,20 @@
 import requests
 from requests.auth import HTTPBasicAuth
 import aiohttp
 #}}}
 
 GLOBAL_PAIRS_CLIENT = None
 
+GLOBAL_LEGACY_ENVIRONMENT      = os.environ.get('GLOBAL_LEGACY_ENVIRONMENT', "True")
+if GLOBAL_LEGACY_ENVIRONMENT.lower() in ('true', 't', 'yes', 'y'):
+    GLOBAL_LEGACY_ENVIRONMENT  = True
+else:
+    GLOBAL_LEGACY_ENVIRONMENT  = False
+
 #
 class ClientResponse:
     #_status: int
     #_body: str
     
     """
     A representation of a client response.
@@ -141,30 +147,39 @@
             client_response_dict["status"] = self._status
         if self._body is not None:
             client_response_dict["body"] = self._body
         return client_response_dict
  
 #
 class Client:
-    #_host: str           = None
-    #_headers: dict       = None
-    #_authentication      = None
-    #_body                = None
+    #_host: str
+    #_headers: dict
+    #_authentication
+    #_body: str
+    #_client_id: str
+    #_tenant_id: str
+    #_legacy: bool
     
     """
     A client wrapper for interaction with IBM PAIRS.
     
     :param headers:            IBM PAIRS host.
     :type headers:             str
     :param headers:            A dictionary of request headers.
     :type headers:             dict
     :param authentication:     An authentication object.
     :type authentication:      ibmpairs.authentication.Oauth2 or ibmpairs.authentication.Basic
     :param body:               A message body.
     :type body:                str
+    :param client_id:          A client id for the authentication system, defaults to 'ibm-pairs' if legacy.
+    :type client_id:           str
+    :param tenant_id:          IBM EIS GA API Connect Tenant Id
+    :type tenant_id:           str
+    :param legacy:             IBM EIS GA Legacy Environment selector override
+    :type legacy:              bool
     """
     
     #
     def __str__(self):
         
         """
         The method creates a string representation of the internal class structure.
@@ -202,40 +217,98 @@
                 client_dict["authentication"] = common.class_to_dict(self._authentication, authentication.Basic)
             elif isinstance(self._authentication, authentication.OAuth2):
                 client_dict["authentication"] = common.class_to_dict(self._authentication, authentication.OAuth2)
             else:
                 client_dict["authentication"] = self._authentication
         if self._body is not None:
             client_dict["body"] = self._body
+        if self._client_id is not None:
+            client_dict["client_id"] = self._client_id
+        if self._tenant_id is not None:
+            client_dict["tenant_id"] = self._tenant_id
+        if self._legacy is not None:
+            client_dict["legacy"] = self._legacy
         return client_dict
 
     #
     def __init__(self,
-                 host = None,
-                 headers = None,
+                 host: str      = None,
+                 headers: dict  = None,
                  authentication = None,
-                 body = None
+                 body: str      = None,
+                 client_id: str = None, 
+                 tenant_id: str = None,
+                 legacy: bool   = None
                 ):
+            
+            self._authentication = authentication
+
+            if legacy is not None:
+                self._legacy = legacy
+            elif (self._authentication is not None) and (self._authentication.legacy is not None):
+                self._legacy = self._authentication.legacy
+            else:
+                self._legacy = GLOBAL_LEGACY_ENVIRONMENT
 
             if (headers is not None):
                 self._headers = headers
             else:
                 self._headers = constants.CLIENT_JSON_HEADER
-
-            self._authentication = authentication
             
             if (host is not None):
                 self._host = common.ensure_protocol(host)
             elif (host is None) and (self._authentication is not None) and (self._authentication.host is not None):
                 self._host = common.ensure_protocol(self._authentication.host)
             else:
-                self._host = common.ensure_protocol(constants.CLIENT_PAIRS_URL)
+                if self._legacy is True:
+                    self._host = common.ensure_protocol(constants.CLIENT_LEGACY_URL)
+                else:
+                    self._host = common.ensure_protocol(constants.CLIENT_URL)
+                    
+            logger.info("HOST: " + self._host)
             
             self._body = body
             
+            if self._legacy is True:
+                if client_id is not None:
+                    self._client_id = client_id
+                else:
+                    self._client_id = 'ibm-pairs'
+                self._tenant_id = tenant_id
+            else:
+                if (client_id is not None) and (tenant_id is not None):
+                    msg = messages.INFO_BOTH_CLIENT_ID_AND_TENANT_ID.format(client_id, tenant_id)
+                    logger.info(msg)
+                    if client_id.startswith('saascore-'):
+                        msg = messages.INFO_STARTS_WITH_SAASCORE
+                        logger.info(msg)
+                        self._client_id = 'geospatial-' + common.get_tenant_id(client_id)
+                    else:
+                        self._client_id = client_id
+                    self._tenant_id = common.get_tenant_id(client_id)
+                elif (client_id is not None) and (tenant_id is None):
+                    if client_id.startswith('saascore-'):
+                        msg = messages.INFO_STARTS_WITH_SAASCORE
+                        logger.info(msg)
+                        self._client_id = 'geospatial-' + common.get_tenant_id(client_id)
+                    else:
+                        self._client_id = client_id
+                    self._tenant_id = common.get_tenant_id(client_id)
+                elif (client_id is None) and (tenant_id is not None):
+                    self._tenant_id = common.get_tenant_id(tenant_id)
+                    self._client_id = 'geospatial-' + self._tenant_id
+                else:
+                    if (self._authentication is not None) and (self._authentication.tenant_id is not None):
+                        self._tenant_id = self._authentication.tenant_id
+                        self._client_id = 'geospatial-' + self._tenant_id
+                    else:
+                        msg = messages.ERROR_NO_CLIENT_OR_TENANT_ID
+                        logger.error(msg)
+                        raise common.PAWException(msg)
+            
             global GLOBAL_PAIRS_CLIENT 
             GLOBAL_PAIRS_CLIENT = self
     
     #       
     def get_host(self):
         return self._host
 
@@ -295,49 +368,93 @@
     #    
     def del_body(self): 
         del self._body
 
     #    
     body = property(get_body, set_body, del_body)
     
+    #       
+    def get_client_id(self):
+        return self._client_id
+    
+    #
+    def set_client_id(self, client_id):
+        self._client_id = client_id
+        
+    #    
+    def del_client_id(self): 
+        del self._client_id
+        
+    #    
+    client_id = property(get_client_id, set_client_id, del_client_id)
+    
+    #       
+    def get_tenant_id(self):
+        return self._tenant_id
+  
+    #
+    def set_tenant_id(self, tenant_id):
+        self._tenant_id = tenant_id
+      
+    #    
+    def del_tenant_id(self): 
+        del self._tenant_id
+      
+    #    
+    tenant_id = property(get_tenant_id, set_tenant_id, del_tenant_id)
+    
+    #
+    def get_legacy(self):
+        return self._legacy
+    
+    #
+    def set_legacy(self, legacy):
+        self._legacy = common.check_bool(legacy)
+        
+    #    
+    def del_legacy(self): 
+        del self._legacy
+        
+    #    
+    legacy = property(get_legacy, set_legacy, del_legacy)
+    
     def session(self,
                 authentication = None,
                 headers        = None,
-                ssl            = None,
-                verify_ssl     = True
+                verify         = None
                ):
         
         """
         A wrapper method around aiohttp.ClientSession.
         
         :param authentication:     A username for the user.
         :type authentication:      ibmpairs.authentication.Basic or ibmpairs.authentication.OAuth2
         :param headers:            A dictionary of request headers.
         :type headers:             dict
-        :param ssl:                SSL.
-        :type ssl:                 str
-        :param verify_ssl:         Verify SSL.
-        :type verify_ssl:          bool
+        :param verify:             Verify SSL.
+        :type verify:              bool
         :returns:                  A aiohttp.ClientSession using the attributes provided.
         :rtype:                    aiohttp.ClientSession
         """
         
         if headers is not None:
             self.set_headers(headers)
+            
+            if self._legacy is False:
+                self.append_header('x-ibm-client-id', self.get_client_id())
+                
             msg = messages.DEBUG_CLIENT_SET_HEADERS.format(headers)
             logger.debug(msg)
         
         if authentication is not None:
             self.set_authentication(authentication)
             msg = messages.DEBUG_CLIENT_SET_HEADERS.format(authentication)
-            logger.debug(msg)             
+            logger.debug(msg)
                         
-        connector = aiohttp.TCPConnector(ssl        = ssl,
-                                         verify_ssl = verify_ssl
-                                        )
+        connector = aiohttp.TCPConnector(ssl = verify)
                                         
         if self.authentication_mode(self._authentication) in ['Basic', 'None']:
             # If authentication.Basic then get set authenication tuple.
             if self.authentication_mode(self._authentication) in ['Basic']:
                 authentication = aiohttp.BasicAuth(self._authentication.username, self._authentication.password)
 
             timeout = aiohttp.ClientTimeout(constants.CLIENT_TIMEOUT)
@@ -347,15 +464,15 @@
                                             timeout   = timeout
                                            )
         elif self.authentication_mode(self._authentication) in ['OAuth2']:
             
             # Add bearer token to headers.
             token = 'Bearer ' + self._authentication.jwt_token
             self.append_header('Authorization', token)
-            
+
             timeout = aiohttp.ClientTimeout(constants.CLIENT_TIMEOUT)
             session = aiohttp.ClientSession(connector = connector, 
                                             headers   = self._headers,
                                             timeout   = timeout
                                            )
         else: 
             msg = messages.ERROR_CLIENT_AUTHENTICATION_MECHANISM.format(self.authentication_mode(self._authentication))
@@ -366,84 +483,85 @@
 
     #
     async def async_get(self,
                         url,
                         session: aiohttp.ClientSession = None,
                         authentication                 = None,
                         headers                        = None,
-                        ssl                            = None,
-                        verify                         = True,
+                        verify                         = None,
                         response_type                  = 'json'
                        ):
                         
         """
         A wrapper method around aiohttp.ClientSession.get.
         
         :param url:                A URL to GET.
         :type url:                 str
         :param session:            An aiohttp.ClientSession to use for a GET request.
         :type session:             aiohttp.ClientSession
         :param authentication:     A username for the user.
         :type authentication:      ibmpairs.authentication.Basic or ibmpairs.authentication.OAuth2
         :param headers:            A dictionary of request headers.
         :type headers:             dict
-        :param ssl:                SSL.
-        :type ssl:                 str
-        :param verify_ssl:         Verify SSL.
-        :type verify_ssl:          bool
+        :param verify:             Verify SSL.
+        :type verify:              bool
         :param response_type:      A response type, defaults to json.
         :type response_type:       str
         :returns:                  An ibmpairs.client.ClientResponse object.
         :rtype:                    ibmpairs.client.ClientResponse
         """
+    
+        retry: bool = False
 
         client_response = ClientResponse()
 
         if session is None:
             session = self.session(authentication, 
                                    headers,
-                                   ssl,
                                    verify
                                   )
 
         async with session.get(url = url
                               ) as response:
             
             client_response.status = response.status  
             if response_type == 'json':
                 client_response.body   = await response.text()
             else:
                 client_response.body   = await response.read()
 
             await session.close() 
-
-        if client_response.status in (401,403):
+            
+        if ((self._legacy is True) and (client_response.status in (401,403))):
             token_refresh_message = constants.CLIENT_TOKEN_REFRESH_MESSAGE
             if client_response.body is not None:
                 response_string = client_response.body
                 if token_refresh_message in response_string:
+                    retry = True
+        elif ((self._legacy is False) and (client_response.status == 500)):
+            retry = True
+
+        if retry is True:
+            self._authentication.refresh_auth_token()
                     
-                    self._authentication.refresh_auth_token()
-                    
-                    session = self.session(self._authentication, 
-                                           headers,
-                                           ssl,
-                                           verify
-                                          )
+            session = self.session(self._authentication, 
+                                   headers,
+                                   verify
+                                  )
 
-                    async with session.get(url = url
-                                          ) as response:
+            async with session.get(url = url
+                                  ) as response:
                             
-                        client_response.status = response.status  
-                        if response_type == 'json':
-                            client_response.body   = await response.text()
-                        else:
-                            client_response.body   = await response.read()
+                client_response.status = response.status  
+                if response_type == 'json':
+                    client_response.body   = await response.text()
+                else:
+                    client_response.body   = await response.read()
 
-                        await session.close()
+                await session.close()
         
         return client_response
     
     #
     def get(self, 
             url,
             headers = None,
@@ -459,18 +577,24 @@
         :type headers:             dict
         :param verify:             Verify SSL.
         :type verify:              bool
         :returns:                  A requests.Response object.
         :rtype:                    requests.Response
         """
         
+        retry: bool = False
+        
         response = None
         
         if headers is not None:
             self.set_headers(headers)
+            
+            if self._legacy is False:
+                self.append_header('x-ibm-client-id', self._get_client_id())
+                
             msg = messages.DEBUG_CLIENT_SET_HEADERS.format('GET', headers)
             logger.debug(msg)
         
         if self.authentication_mode(self._authentication) in ['Basic', 'tuple', 'Dict', 'None']:
             # If Basic, construct an authentication tuple.
             if self.authentication_mode(self._authentication) in ['Basic']:
                 authentication = self._authentication.get_credentials()
@@ -481,28 +605,33 @@
                                     verify  = verify)
         elif self.authentication_mode(self._authentication) in ['OAuth2']:
             token = 'Bearer ' + self._authentication.jwt_token
             self.append_header('Authorization', token)
             response = requests.get(url, 
                                     headers = self._headers,
                                     verify  = verify
-                                   )                
-            
-            if response.status_code in (401,403):
+                                   )
+                                    
+            if ((self._legacy is True) and (response.status_code in (401,403))):
                 token_refresh_message = constants.CLIENT_TOKEN_REFRESH_MESSAGE
                 if response.json() is not None:
                     response_string = json.dumps(response.json())
                     if token_refresh_message in response_string:
-                        self._authentication.refresh_auth_token()
-                        token = 'Bearer ' + self._authentication.jwt_token
-                        self.append_header('Authorization', token)
-                        response = requests.get(url, 
-                                                headers = self._headers,
-                                                verify  = verify
-                                               )
+                        retry = True
+            elif ((self._legacy is False) and (response.status_code == 500)):
+                retry = True
+            
+            if retry is True:
+                self._authentication.refresh_auth_token()
+                token = 'Bearer ' + self._authentication.jwt_token
+                self.append_header('Authorization', token)
+                response = requests.get(url, 
+                                        headers = self._headers,
+                                        verify  = verify
+                                       )
         else:
             msg = messages.ERROR_AUTHENTICATION_TYPE_NOT_RECOGNIZED.format(type(self._authentication))
             logger.error(msg)
             raise Exception(msg)
             
         return response
 
@@ -524,19 +653,25 @@
         :param headers:            A dictionary of request headers.
         :type headers:             dict
         :param verify:             Verify SSL.
         :type verify:              bool
         :returns:                  A requests.Response object.
         :rtype:                    requests.Response
         """
+        
+        retry: bool = False
             
         response = None
         
         if headers is not None:
             self.set_headers(headers)
+            
+            if self._legacy is False:
+                self.append_header('x-ibm-client-id', self._get_client_id())
+                
             msg = messages.DEBUG_CLIENT_SET_HEADERS.format('PUT', headers)
             logger.debug(msg)
         
         if self.authentication_mode(self._authentication) in ['Basic', 'tuple', 'Dict', 'None']:
             # If Basic, construct an authentication tuple.
             if self.authentication_mode(self._authentication) in ['Basic']:
                 authentication = self._authentication.get_credentials()
@@ -551,27 +686,33 @@
             token = 'Bearer ' + self._authentication.jwt_token
             self.append_header('Authorization', token)
             response = requests.put(url,
                                     headers = self._headers,
                                     data    = body,
                                     verify  = verify
                                    )
-            if response.status_code in (401,403):
+            
+            if ((self._legacy is True) and (response.status_code in (401,403))):
                 token_refresh_message = constants.CLIENT_TOKEN_REFRESH_MESSAGE
                 if response.json() is not None:
                     response_string = json.dumps(response.json())
                     if token_refresh_message in response_string:
-                        self._authentication.refresh_auth_token()
-                        token = 'Bearer ' + self._authentication.jwt_token
-                        self.append_header('Authorization', token)
-                        response = requests.put(url,
-                                                headers = self._headers,
-                                                data    = body,
-                                                verify  = verify
-                                               )
+                        retry = True
+            elif ((self._legacy is False) and (response.status_code == 500)):
+                retry = True
+            
+            if retry is True:
+                self._authentication.refresh_auth_token()
+                token = 'Bearer ' + self._authentication.jwt_token
+                self.append_header('Authorization', token)
+                response = requests.put(url,
+                                        headers = self._headers,
+                                        data    = body,
+                                        verify  = verify
+                                       )
 
         else:
             msg = messages.ERROR_AUTHENTICATION_TYPE_NOT_RECOGNIZED.format(type(self._authentication))
             logger.error(msg)
             raise Exception(msg)
                     
         return response
@@ -579,16 +720,15 @@
     #
     async def async_post(self,
                          url,
                          body,
                          session: aiohttp.ClientSession = None,
                          authentication                 = None,
                          headers                        = None,
-                         ssl                            = None,
-                         verify                         = True
+                         verify                         = None
                         ):
                           
         """
         A wrapper method around aiohttp.ClientSession.post.
         
         :param url:                A URL to POST.
         :type url:                 str
@@ -596,62 +736,64 @@
         :type body:                Any
         :param session:            An aiohttp.ClientSession to use for a get request.
         :type session:             aiohttp.ClientSession
         :param authentication:     A username for the user.
         :type authentication:      ibmpairs.authentication.Basic or ibmpairs.authentication.OAuth2
         :param headers:            A dictionary of request headers.
         :type headers:             dict
-        :param ssl:                SSL.
-        :type ssl:                 str
-        :param verify_ssl:         Verify SSL.
-        :type verify_ssl:          bool
+        :param verify:             Verify SSL.
+        :type verify:              bool
         :returns:                  An ibmpairs.client.ClientResponse object.
         :rtype:                    ibmpairs.client.ClientResponse
         """
+    
+        retry: bool = False
                             
         client_response = ClientResponse()
 
         if session is None:
             session = self.session(authentication, 
                                    headers,
-                                   ssl,
                                    verify
                                   )
 
         async with session.post(url  = url,
                                 json = body 
                                ) as response:
             
             client_response.status = response.status            
             client_response.body   = await response.text()
 
             await session.close()
-        
-        if client_response.status in (401,403):
+            
+        if ((self._legacy is True) and (client_response.status in (401,403))):
             token_refresh_message = constants.CLIENT_TOKEN_REFRESH_MESSAGE
             if client_response.body is not None:
                 response_string = client_response.body
                 if token_refresh_message in response_string:
+                    retry = True
+        elif ((self._legacy is False) and (client_response.status == 500)):
+            retry = True
+        
+        if retry is True:
+            self._authentication.refresh_auth_token()
                     
-                    self._authentication.refresh_auth_token()
-                    
-                    session = self.session(self._authentication, 
-                                           headers,
-                                           ssl,
-                                           verify
-                                          )
+            session = self.session(self._authentication, 
+                                   headers,
+                                   verify
+                                  )
 
-                    async with session.post(url  = url,
-                                            json = body 
-                                           ) as response:
+            async with session.post(url  = url,
+                                    json = body 
+                                   ) as response:
             
-                        client_response.status = response.status            
-                        client_response.body   = await response.text()
+                client_response.status = response.status            
+                client_response.body   = await response.text()
 
-                        await session.close()
+                await session.close()
         
         return client_response
 
     #
     def post(self, 
              url,
              body,
@@ -670,18 +812,24 @@
         :type headers:             dict
         :param verify:             Verify SSL.
         :type verify:              bool
         :returns:                  A requests.Response object.
         :rtype:                    requests.Response
         """
         
+        retry: bool = False
+        
         response = None
         
         if headers is not None:
             self.set_headers(headers)
+            
+            if self._legacy is False:
+                self.append_header('x-ibm-client-id', self._get_client_id())
+                
             msg = messages.DEBUG_CLIENT_SET_HEADERS.format('POST', headers)
             logger.debug(msg)
         
         auth_mode = self.authentication_mode(self._authentication)
         
         if auth_mode in ['Basic', 'tuple', 'Dict', 'None']:
             # If Basic, construct an authentication tuple.
@@ -700,28 +848,34 @@
             self.append_header('Authorization', token)
             logger.debug(messages.DEBUG_CLIENT_POST_OAUTH.format(body, url))
             response = requests.post(url,
                                      headers = self._headers,
                                      data    = body,
                                      verify  = verify
                                     )
-            if response.status_code in (401,403):
+            
+            if ((self._legacy is True) and (response.status_code in (401,403))):
                 token_refresh_message = constants.CLIENT_TOKEN_REFRESH_MESSAGE
                 if response.json() is not None:
                     response_string = json.dumps(response.json())
                     if token_refresh_message in response_string:
-                        self._authentication.refresh_auth_token()
-                        token = 'Bearer ' + self._authentication.jwt_token
-                        self.append_header('Authorization', token)
-                        logger.debug(messages.DEBUG_CLIENT_POST_OAUTH.format(body, url))
-                        response = requests.post(url,
-                                                 headers = self._headers,
-                                                 data    = body,
-                                                 verify  = verify
-                                                )
+                        retry = True
+            elif ((self._legacy is False) and (response.status_code == 500)):
+                retry = True
+            
+            if retry is True:
+                self._authentication.refresh_auth_token()
+                token = 'Bearer ' + self._authentication.jwt_token
+                self.append_header('Authorization', token)
+                logger.debug(messages.DEBUG_CLIENT_POST_OAUTH.format(body, url))
+                response = requests.post(url,
+                                         headers = self._headers,
+                                         data    = body,
+                                         verify  = verify
+                                        )
         else:
             msg = messages.ERROR_AUTHENTICATION_TYPE_NOT_RECOGNIZED.format(type(self._authentication))
             logger.error(msg)
             raise Exception(msg)
 
         return response
       
@@ -740,19 +894,25 @@
         :param headers:            A dictionary of request headers.
         :type headers:             dict
         :param verify:             Verify SSL.
         :type verify:              bool
         :returns:                  A requests.Response object.
         :rtype:                    requests.Response
         """
+        
+        retry: bool = False
                 
         response = None
         
         if headers is not None:
             self.set_headers(headers)
+            
+            if self._legacy is False:
+                self.append_header('x-ibm-client-id', self._get_client_id())
+                
             msg = messages.DEBUG_CLIENT_SET_HEADERS.format('DELETE', headers)
             logger.debug(msg)
         
         auth_mode = self.authentication_mode(self._authentication)
         
         if auth_mode in ['Basic', 'tuple', 'Dict', 'None']:
             # If Basic, construct an authentication tuple.
@@ -769,28 +929,33 @@
             token = 'Bearer ' + self._authentication.jwt_token
             self.append_header('Authorization', token)
             logger.debug(messages.DEBUG_CLIENT_DELETE_OAUTH.format(url))
             response = requests.delete(url,
                                        headers = self._headers,
                                        verify  = verify
                                       )
-          
-            if response.status_code in (401,403):
+                                        
+            if ((self._legacy is True) and (response.status_code in (401,403))):
                 token_refresh_message = constants.CLIENT_TOKEN_REFRESH_MESSAGE
                 if response.json() is not None:
                     response_string = json.dumps(response.json())
                     if token_refresh_message in response_string:
-                        self._authentication.refresh_auth_token()
-                        token = 'Bearer ' + self._authentication.jwt_token
-                        self.append_header('Authorization', token)
-                        logger.debug(messages.DEBUG_CLIENT_DELETE_OAUTH.format(url))
-                        response = requests.delete(url,
-                                                   headers = self._headers,
-                                                   verify  = verify
-                                                  )
+                        retry = True
+            elif ((self._legacy is False) and (response.status_code == 500)):
+                retry = True
+          
+            if retry is True:
+                self._authentication.refresh_auth_token()
+                token = 'Bearer ' + self._authentication.jwt_token
+                self.append_header('Authorization', token)
+                logger.debug(messages.DEBUG_CLIENT_DELETE_OAUTH.format(url))
+                response = requests.delete(url,
+                                           headers = self._headers,
+                                           verify  = verify
+                                          )
         else:
             msg = messages.ERROR_AUTHENTICATION_TYPE_NOT_RECOGNIZED.format(type(self._authentication))
             logger.error(msg)
             raise Exception(msg)
 
         return response
 
@@ -822,7 +987,94 @@
             authentication_mode = 'dict'
         else:
             msg = u'The authentication object was not recognized.'
 #            logger.warning(msg)
             raise Exception(msg)
         
         return authentication_mode
+  
+#
+def get_client(host: str          = None,
+               username: str      = None,
+               api_key: str       = None,
+               api_key_file: str  = "auth/oauth2.txt",
+               client_id: str     = None,
+               endpoint: str      = None,
+               jwt_token: str     = None,
+               iam_endpoint: str  = "iam.cloud.ibm.com",
+               org_id: str        = None, 
+               tenant_id: str     = None,
+               headers: dict      = None,
+               body: str          = None,
+               password: str      = None,
+               password_file: str = None,
+               legacy: bool       = None
+              ):
+    """
+    Gets either a authentication.Basic or authentication.OAuth2 from authentication credentials.
+    
+    :param host:          IBM PAIRS host
+    :type host:           str
+    :param username:      IBM PAIRS username
+    :type username:       str
+    :param api_key:       IBM PAIRS API key
+    :type api_key:        str
+    :param api_key_file:  IBM PAIRS API key file, defaults to auth/oauth2.txt
+    :type api_key_file:   str
+    :param client_id:     A client id for the authentication system, defaults to 'ibm-pairs' if legacy.
+    :type client_id:      str
+    :param endpoint:      The authentication endpoint.
+    :type endpoint:       str
+    :param jwt_token:     A jwt token for authentication.
+    :type jwt_token:      str
+    :param iam_endpoint:  IBM Cloud IAM Endpoint
+    :type iam_endpoint:   str
+    :param org_id:        IBM EIS GA API Connect Org Id
+    :type org_id:         str
+    :param tenant_id:     IBM EIS GA API Connect Tenant Id
+    :type tenant_id:      str
+    :param password:      IBM PAIRS password
+    :type password:       str
+    :param password_file: IBM PAIRS password file, defaults to auth/basic.txt
+    :type password_file:  str
+    :param legacy:        IBM EIS GA Legacy Environment selector override
+    :type legacy:         bool
+    :rtype:               authentication.Basic or authentication.OAuth2
+    :raises Exception:    if authentication.Basic or authentication.OAuth2 raise an error
+    """
+    
+    auth = None
+    
+    if (password is not None) or (password_file is not None):
+        msg = messages.INFO_BASIC_AUTH_ASSUMPTION
+        logger.info(msg)
+        
+        auth = authentication.Basic(host          = host,
+                                    username      = username,
+                                    password      = password,
+                                    password_file = password_file,
+                                    legacy        = legacy
+                                   )
+    
+    else:
+        msg = messages.INFO_0AUTH2_AUTH_ASSUMPTION
+        logger.info(msg)
+        
+        auth = authentication.OAuth2(host         = host,
+                                     username     = username,
+                                     api_key      = api_key,
+                                     api_key_file = api_key_file,
+                                     client_id    = client_id,
+                                     endpoint     = endpoint,
+                                     jwt_token    = jwt_token,
+                                     iam_endpoint = iam_endpoint,
+                                     org_id       = org_id, 
+                                     tenant_id    = tenant_id,
+                                     legacy        = legacy
+                                    )
+        
+    eis_client = Client(headers = headers,
+                        authentication = auth,
+                        body = body
+                       )
+    
+    return eis_client
```

### Comparing `ibmpairs-0.2.7/ibmpairs/common.py` & `ibmpairs-0.2.8/ibmpairs/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -438,7 +438,32 @@
     if host.startswith('pairs.res') or host.startswith('http://pairs.res'):
         return "https://" + strip_protocol(host)
     else:
         if host.startswith('http://'):
             return "http://" + strip_protocol(host)
         else:
             return "https://" + strip_protocol(host)
+
+#
+def get_tenant_id(client_id: str):
+    
+    """
+    Gets tenant id from client_id with 'saascore-', 'geospatial-' prefixes or without.
+
+    :param client_id: A client id for the authentication system.
+    :type client_id:  str
+    :returns:         The tenant id.
+    :rtype:           str
+    """ 
+    
+    tenant_id: str = None
+    
+    if client_id is not None:
+        tenant_id = client_id
+        if client_id.startswith('saascore-'):
+            tenant_id = client_id[9:len(client_id)]
+        elif client_id.startswith('geospatial-'):
+            tenant_id = client_id[11:len(client_id)]
+            
+        return tenant_id
+    else:
+        return None
```

### Comparing `ibmpairs-0.2.7/ibmpairs/config.py` & `ibmpairs-0.2.8/ibmpairs/config.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.7/ibmpairs/constants.py` & `ibmpairs-0.2.8/ibmpairs/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 Copyright 2019-2021 Physical Analytics, IBM Research All Rights Reserved.
 
 SPDX-License-Identifier: BSD-3-Clause
 """
 import os
 
 # global
-PAW_LOG_LEVEL              = os.environ.get('PAW_LOG_LEVEL', 'INFO')
-GLOBAL_JSON_REPR_INDENT    = int(os.environ.get('GLOBAL_JSON_REPR_INDENT', 4))
-GLOBAL_JSON_REPR_SORT_KEYS = os.environ.get('GLOBAL_JSON_REPR_SORT_KEYS', True)
-GLOBAL_SSL_VERIFY          = True
+GLOBAL_LEGACY_ENVIRONMENT     = os.environ.get('GLOBAL_LEGACY_ENVIRONMENT', "True")
+if GLOBAL_LEGACY_ENVIRONMENT.lower() in ('true', 't', 'yes', 'y', '1', 'on'):
+	GLOBAL_LEGACY_ENVIRONMENT = True
+else:
+	GLOBAL_LEGACY_ENVIRONMENT = False
+
+PAW_LOG_LEVEL                 = os.environ.get('PAW_LOG_LEVEL', 'INFO')
+GLOBAL_JSON_REPR_INDENT       = int(os.environ.get('GLOBAL_JSON_REPR_INDENT', 4))
+GLOBAL_JSON_REPR_SORT_KEYS    = os.environ.get('GLOBAL_JSON_REPR_SORT_KEYS', True)
+GLOBAL_SSL_VERIFY             = True
 
 # catalog
 CATALOG_DATA_SETS_API                   = '/v2/datasets/'
 CATALOG_DATA_SETS_API_FULL              = '/v2/datasets/full'
 CATALOG_DATA_SETS_LAYERS_API            = '/datalayers'
 
 CATALOG_DATA_LAYERS_API                 = '/v2/datalayers/'
@@ -26,15 +32,16 @@
 
 CATALOG_DATA_LAYER_DIMENSIONS_API       = '/v2/datalayer_dimensions/'
 CATALOG_DATA_LAYER_DIMENSION_VALUES_API = '/v2/datalayer_dimension_values/'
 
 CATALOG_DATA_LAYER_PROPERTIES_API       = '/v2/datalayer_properties/'
 
 # client
-CLIENT_PAIRS_URL                 = os.environ.get('CLIENT_PAIRS_URL', 'https://pairs.res.ibm.com')
+CLIENT_URL                       = os.environ.get('CLIENT_URL', 'https://api.ibm.com/geospatial/run/na/pairs-query')
+CLIENT_LEGACY_URL                = os.environ.get('CLIENT_LEGACY_URL', 'https://pairs.res.ibm.com')
 CLIENT_JSON_HEADER               = {"Content-Type": "application/json"}
 CLIENT_PUT_AND_POST_HEADER       = {'Content-Type': 'application/json', 'Accept': 'application/json'}
 CLIENT_PUT_AND_POST_HEADER_CSV   = {'Accept': 'text/csv'}
 CLIENT_GET_DEFAULT_RESPONSE_TYPE = 'json'
 CLIENT_TOKEN_REFRESH_MESSAGE     = 'claim expired'
 CLIENT_TIMEOUT                   = os.environ.get('CLIENT_TIMEOUT', 3600)
 
@@ -42,39 +49,41 @@
 UPLOAD_STATUS_API              = '/v2/uploader/upload/'
 UPLOAD_METADATA_FILE_EXTENTION = '.meta.json'
 
 UPLOAD_DEFAULT_WORKERS         = int(os.environ.get('UPLOAD_DEFAULT_WORKERS', 1))
 UPLOAD_MAX_WORKERS             = int(os.environ.get('UPLOAD_MAX_WORKERS', 8))
 UPLOAD_MIN_STATUS_INTERVAL     = int(os.environ.get('UPLOAD_MIN_STATUS_INTERVAL', 30))
 UPLOAD_STATUS_CHECK_INTERVAL   = int(os.environ.get('UPLOAD_STATUS_CHECK_INTERVAL', 60))
+UPLOAD_WORKER_DEBUG            = os.environ.get('UPLOAD_WORKER_DEBUG', "False")
 UPLOAD_WORKER_DEBUG            = False
 
 # woc
 EIS_V2_API_URL                 = os.environ.get('EIS_V2_API_URL', 'https://foundation.agtech.ibm.com/v2')
 EIS_REGISTER_QUERY_URL         = EIS_V2_API_URL + '/layer/analytics/metadata'
 
 # phoenix
-PHOENIX_V1_API_URL             =  os.environ.get('PHOENIX_V1_API_URL', 'https://api.auth-b2b-twc.ibm.com/api/v1')
+PHOENIX_V1_API_URL             = os.environ.get('PHOENIX_V1_API_URL', 'https://api.auth-b2b-twc.ibm.com/api/v1')
 PHOENIX_ADD_DASHBOARD_LAYER    = PHOENIX_V1_API_URL  + '/IMAP/put-layer-config-block'
 
 #query
-QUERY_API                      = '/v2/query/'
+QUERY_API                      = '/v2/query'
 QUERY_JOBS_API                 = '/v2/queryjobs/'
 QUERY_JOBS_DOWNLOAD_API        = '/v2/queryjobs/download/'
 QUERY_JOBS_API_MERGE           = '/merge/'
 QUERY_DATE_FORMAT              = '%Y-%m-%d'
 QUERY_DEFAULT_WORKERS          = int(os.environ.get('QUERY_DEFAULT_WORKERS', 1))
 QUERY_MAX_WORKERS              = int(os.environ.get('QUERY_MAX_WORKERS', 8))
 QUERY_MIN_STATUS_INTERVAL      = int(os.environ.get('QUERY_MIN_STATUS_INTERVAL', 15))
 QUERY_STATUS_CHECK_INTERVAL    = int(os.environ.get('QUERY_STATUS_CHECK_INTERVAL', 30))
-QUERY_WORKER_DEBUG             = False
 QUERY_STATUS_RUNNING_CODES     = [0, 1, 10, 11, 12]
 QUERY_STATUS_SUCCESS_CODES     = [20]
 QUERY_STATUS_FAILURE_CODES     = [21, 30, 31, 40, 41]
 QUERY_DOWNLOAD_DEFAULT_FOLDER  = 'download'
+QUERY_WORKER_DEBUG             = os.environ.get('QUERY_WORKER_DEBUG', "False")
+QUERY_WORKER_DEBUG             = False
 
 #
 IBM_CLOUD_OBJECT_STORE_CONTROL_URL = 'control.cloud-object-storage.cloud.ibm.com'
 IBM_CLOUD_OBJECT_STORE_ENDPOINTS   = '/v2/endpoints'
 
 # Used for conversion from degrees to metres / vice versa, and determining levels
 RASTER_DEGREE_STEPS = [268.435456,134.217728,67.108864,33.554432,16.777216,8.388608,4.194304,2.097152,1.048576,0.524288,0.262144,0.131072,0.065536,0.032768,0.016384,0.008192,0.004096,0.002048,0.001024,0.000512,0.000256,0.000128,0.000064,0.000032,0.000016,0.000008,0.000004,0.000002,0.000001]
```

### Comparing `ibmpairs-0.2.7/ibmpairs/dashboard.py` & `ibmpairs-0.2.8/ibmpairs/dashboard.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Copyright 2019-2021 Physical Analytics, IBM Research All Rights Reserved.
 
 SPDX-License-Identifier: BSD-3-Clause
 """
 
 # fold: Import Python Standard Library {{{
 # Python Standard Library:
+import os
 from datetime import datetime
 import json
 import re
 from typing import List, Any
 #}}}
 # fold: Import ibmpairs Modules {{{
 # ibmpairs Modules:
@@ -23,14 +24,20 @@
 import ibmpairs.messages as messages
 from ibmpairs.logger import logger
 #}}}
 # fold: Import Third Party Libraries {{{
 # Third Party Libraries:
 #}}}
 
+GLOBAL_LEGACY_ENVIRONMENT      = os.environ.get('GLOBAL_LEGACY_ENVIRONMENT', "True")
+if GLOBAL_LEGACY_ENVIRONMENT.lower() in ('true', 't', 'yes', 'y'):
+  GLOBAL_LEGACY_ENVIRONMENT  = True
+else:
+  GLOBAL_LEGACY_ENVIRONMENT  = False
+
 class QueryRegistrationReturn:
     #_analytics_uuid: str
     #_layer_id: str
     #_base_computation_id: str
     
     """
     An object to represent the return from an IBM Environmental Intelligence Suite (EIS) Query Registration call.
@@ -196,15 +203,16 @@
         
         return json.dumps(self.to_dict())
 
 #
 def register_query(query,
                    query_name: str,
                    client: client_module.Client = None,
-                   host: str                    = None
+                   host: str                    = None,
+                   legacy: bool                 = None
                   ):
                     
     """
     A method to register a PAIRS Query with the IBM Environmental Intelligence Suite (EIS) dashboard.
 
     :param query:        A PAIRS Query.
     :type query:         ibmpairs.query.Query or dict or str
@@ -217,14 +225,17 @@
     :returns:            A QueryRegistrationReturn and a Query.
     :rtype:              ibmpairs.dashboard.QueryRegistrationReturn, ibmpairs.query.Query
     :raises Exception:   If no client is provided or found Globally in the environment, 
                          if query type is not ibmpairs.query.Query or dict or str, 
                          if response is not 200, 
                          if object conversions fail.
     """        
+  
+    if legacy is None:
+        legacy = GLOBAL_LEGACY_ENVIRONMENT
                     
     if (host is None):
         host = constants.EIS_REGISTER_QUERY_URL
 
     if (client is None):
         client = common.set_client(input_client  = client,
                                    global_client = client_module.GLOBAL_PAIRS_CLIENT)
@@ -268,16 +279,18 @@
         query_obj.submit_response = query_return
         query_obj.id = query_registration.base_computation_id
         #query_result = query_module.QueryResult(client=client, query=query_obj, query_return=query_return)
         return query_registration, query_obj
     except Exception as ex:
         raise ex
     finally:
-        # set client back to pointing at PAIRS
-        client.set_host(constants.CLIENT_PAIRS_URL)
+        if legacy is True:
+          client.set_host = common.ensure_protocol(constants.CLIENT_LEGACY_URL)
+        else:
+          client.set_host = common.ensure_protocol(constants.CLIENT_URL)
 
 
 def add_dashboard_layer(query_registration: QueryRegistrationReturn,
                         name: str,
                         client         = None,
                         headers        = None,
                         host           = None,
@@ -291,15 +304,16 @@
                                                                        ] 
                                                        },
                                             'unit': 'C',
                                             'isInterpolated': True,
                                             'extendMinimumColor': False,
                                             'extendMaximumColor': True,
                                             'invalidDataValue': -9999
-                                           }
+                                           },
+                        legacy: bool                 = None
                         ):
     
     """
     A method to add a dashboard layer to the IBM Environmental Intelligence Suite (EIS) dashboard.
 
     :param query_registration: A query registration result from a successful EIS registration.
     :type query_registration:  ibmpairs.dashboard.QueryRegistrationReturn
@@ -312,14 +326,17 @@
     :param host:               (Optional) A host for the registration.
     :type host:                str
     :param style_properties:   (Optional) A dictionary of style properties for the dashboard layer.
     :type style_properties:    dict
     :raises Exception:         If no client is provided or found Globally in the environment, 
                                if response is not 200.
     """ 
+  
+    if legacy is None:
+        legacy = GLOBAL_LEGACY_ENVIRONMENT
 
     if (headers is None):
         headers = constants.CLIENT_JSON_HEADER
 
     if (host is None):
         host = constants.PHOENIX_ADD_DASHBOARD_LAYER
 
@@ -362,10 +379,13 @@
             except :
                 msg = str(response.status_code)
                 logger.error(msg)
             raise common.PAWException(msg)
     except Exception as ex:
         raise ex
     finally:
-        # set client back to pointing at PAIRS
-        client.set_host(constants.CLIENT_PAIRS_URL)
+        if legacy is True:
+            client.set_host = common.ensure_protocol(constants.CLIENT_LEGACY_URL)
+        else:
+            client.set_host = common.ensure_protocol(constants.CLIENT_URL)
 
+
```

### Comparing `ibmpairs-0.2.7/ibmpairs/external/ibm.py` & `ibmpairs-0.2.8/ibmpairs/external/ibm.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.7/ibmpairs/messages.py` & `ibmpairs-0.2.8/ibmpairs/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,29 @@
 INFO_AUTHENTICATION_API_KEY_NOT_FOUND_IN_FILE = 'The api key for the user \'{}\' in file \'{}\' could not be found or set for the host \'{}\'.'
 INFO_AUTHENTICATION_PASSWORD_NOT_FOUND_IN_FILE = 'The password for the user \'{}\' in file \'{}\' could not be found or set for the host \'{}\'.'
 INFO_AUTHENTICATION_COULD_NOT_GET_AUTH_TOKEN = 'The authentication failed with auth token \'{}\', exception: \'{}\''
 ERROR_AUTHENTICATION_FAILED = 'AUTHENTICATION FAILED: A {} could not be gathered from the provided attributes.'
 ERROR_AUTHENTICATION_COULD_NOT_FIND_API_KEY_FILE = 'The api key file \'{}\' could not be found.'
 ERROR_AUTHENTICATION_NO_API_KEY_OR_CLIENT_ID = 'The OAuth2 Authentication type requires an api_key and client_id to be set.'
 ERROR_AUTHENTICATION_NO_REFRESH_TOKEN_OR_CLIENT_ID = 'The OAuth2 Authentication refresh_auth_token() call requires a oauth2_response.refresh_token and client_id to be set. The method is intended to be called once a user has already authenticated but the jwt token has expired, try executing the get_auth_token() method.'
-ERROR_AUTHENTICATION_PHOENIX_RETURN_NOT_OAUTH2RETURN = 'The json returned by the {} service was not of type OAuth2Return. The returned json is: \'{}\', the exception: \'{}\''
-ERROR_AUTHENTICATION_PHOENIX_NOT_SUCCESSFUL = 'The call to the {} service was not successful, the status code is: \'{}\''
-ERROR_AUTHENTICATION_PHOENIX_200_RETURN_ERROR = 'The call to the {} service was successful but produced an error \'{}\', perhaps the api_key value is incorrect.'
-ERROR_AUTHENTICATION_PHOENIX_REFRESH_200_RETURN_ERROR = 'The call to the {} service was successful but produced an error \'{}\', perhaps the refresh_token value is incorrect or a temporary issue with the authentication system prevented the procurement of an authentication token.'
+ERROR_AUTHENTICATION_RETURN_NOT_OAUTH2RETURN = 'The json returned by the {} service was not of type OAuth2Return. The returned json is: \'{}\', the exception: \'{}\''
+ERROR_AUTHENTICATION_NOT_SUCCESSFUL = 'The call to the {} service was not successful, the status code is: \'{}\''
+ERROR_AUTHENTICATION_NOT_SUCCESSFUL_API_CONNECT = 'The call to the {} service was not successful, the status code is: \'{}\', message: \'{}\''
+ERROR_AUTHENTICATION_200_RETURN_ERROR = 'The call to the {} service was successful but produced an error \'{}\', perhaps the api_key value is incorrect.'
+ERROR_AUTHENTICATION_REFRESH_200_RETURN_ERROR = 'The call to the {} service was successful but produced an error \'{}\', perhaps the refresh_token value is incorrect or a temporary issue with the authentication system prevented the procurement of an authentication token.'
 INFO_AUTHENTICATION_TOKEN_REFRESH = 'Attempting to refresh authentication token.'
 INFO_AUTHENTICATION_TOKEN_REFRESH_SUCCESS = 'The token was successfully refreshed.'
 ERROR_AUTHENTICATION_TYPE_NOT_RECOGNIZED = 'The authentication type {} was not recognized.'
+ERROR_AUTHENTICATION_IAM_NO_API_KEY_OR_CLIENT_ID = 'The OAuth2 Authentication type, when using API Connect, requires an api_key, client_id and org_id to be set.'
+ERROR_AUTHENTICATION_NO_ACCESS_TOKEN = 'An access_token from {} the return could not be found, response \'{}\'.'
+INFO_BOTH_CLIENT_ID_AND_TENANT_ID = 'The client_id {} and the tenant_id {} have both been specified; the tenant_id entry will be derived from client_id.'
+ERROR_NO_CLIENT_OR_TENANT_ID = 'A client_id or tenant_id must be specified in order to authentication via IBM API Connect.'
+ERROR_NO_ORG_ID = 'An org_id must be specified in order to authentication via IBM API Connect.'
+INFO_STARTS_WITH_GEOSPATIAL = 'The string starts with geospatial, where it should start with saascore; correcting.'
+INFO_STARTS_WITH_SAASCORE = 'The string starts with saascore, where it should start with geospatial; correcting.'
 
 # catalog messages
 ERROR_CATALOG_RESPOSE_NOT_SUCCESSFUL = 'The {} {} call to {} failed with status code: {}, message: {}.'
 INFO_CATALOG_RESPOSE_NOT_SUCCESSFUL_NO_ERROR_MESSAGE = 'There was no error message produced in the output of the failed call.'
 
 ERROR_CATALOG_DATA_SET_ID = 'The DataSet object has no ID set and none was provided.'
 ERROR_CATALOG_DATA_LAYER_DATA_SET_ID = 'The DataLayer object has no Data Set ID set and none was provided.'
@@ -94,14 +102,16 @@
 DEBUG_CLIENT_DELETE_BASIC = 'DELETE of {} using basic auth.'
 DEBUG_CLIENT_DELETE_OAUTH = 'DELETE of {} using oauth.'
 ERROR_CLIENT_AUTHENTICATION_MECHANISM = 'The authentication mechanism {} was not recognized.'
 DEBUG_CLIENT_SET_HEADERS = 'The headers for the client set to {}.'
 DEBUG_CLIENT_SET_AUTHENTICATION = 'The authentication for the client was set to {}.'
 
 ERROR_CLIENT_UNSPECIFIED_ERROR = 'The {} {} to {} encountered an unspecified error contacting the server; the request was unsuccessful, error message: {}'
+INFO_BASIC_AUTH_ASSUMPTION = 'The client authentication method is assumed to be Basic auth as password, or password file was specified.'
+INFO_0AUTH2_AUTH_ASSUMPTION = 'The client authentication method is assumed to be OAuth2.'
 
 # common messages
 INFO_COMMON_CHECK_BOOL_CONVERSION = 'The \'{}\' value \'{}\' was converted to a boolean \'{}\'.'
 
 ERROR_COMMON_FROM_LIST = 'The input method \'{}\' could not be executed against the \'{}\' list.'
 ERROR_COMMON_CLASS_TO_DICT = 'The \'{}\' input object of type \'{}\' could not be cast to dict.'
 ERROR_COMMON_CHECK_BOOL = 'The type \'{}\' of \'{}\' is invalid, the type should be in [\'bool\', \'str\', \'int\'].'
```

### Comparing `ibmpairs-0.2.7/ibmpairs/paw.py` & `ibmpairs-0.2.8/ibmpairs/paw.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,41 +24,41 @@
 import copy
 # compatibility of code with Python 2 and 3
 from builtins import dict, range, map, filter, zip, input, chr, str
 from past.builtins import xrange, execfile, intern, apply, cmp
 from io import open
 from functools import reduce
 try:
-    from importlib import reload
+        from importlib import reload
 except:
-    from imp import reload
+        from imp import reload
 from future import standard_library
 standard_library.install_aliases()
 try:
-    string_type = basestring
+        string_type = basestring
 except NameError:
-    string_type = str
+        string_type = str
 # parallel processing
 import concurrent.futures
 # make reading file pointer streams in Python 2 and 3
 import codecs
 # modules needed
 import numpy
 import pandas
 import errno
 from requests.compat import urlparse, urljoin
 import requests
 import io
 import json, jsonschema
 HAS_GEOJSON = False
 try:
-    import geojson
-    HAS_GEOJSON = True
+        import geojson
+        HAS_GEOJSON = True
 except:
-    pass
+        pass
 import hashlib
 import time
 import datetime
 import dateutil, dateutil.parser
 import pytz
 from shapely.geometry import shape, box, Point
 import re
@@ -68,34 +68,34 @@
 # file system abstraction
 import fs
 from fs.osfs import OSFS
 from fs import zipfs
 # }}}
 # fold: optional packages#{{{
 try:
-    import geopandas
-    HAS_GEOPANDAS=True
+        import geopandas
+        HAS_GEOPANDAS=True
 except:
-    HAS_GEOPANDAS=False
+        HAS_GEOPANDAS=False
 try:
-    import coloredlogs
-    HAS_COLOREDLOGS=True
+        import coloredlogs
+        HAS_COLOREDLOGS=True
 except:
-    HAS_COLOREDLOGS=False
+        HAS_COLOREDLOGS=False
 try:
-    from osgeo import gdal
-    HAS_GDAL=True
+        from osgeo import gdal
+        HAS_GDAL=True
 except:
-    HAS_GDAL=False
-    try:
-        import PIL.Image
-        # adjust maximum size of pixels for image to load (1 TPix)
-        PIL.Image.MAX_IMAGE_PIXELS = 10**12
-    except Exception as e:
-        raise ImportError('Neither GDAL nor PIL could be imported.')
+        HAS_GDAL=False
+        try:
+                import PIL.Image
+                # adjust maximum size of pixels for image to load (1 TPix)
+                PIL.Image.MAX_IMAGE_PIXELS = 10**12
+        except Exception as e:
+                raise ImportError('Neither GDAL nor PIL could be imported.')
 import ibmpairs.authentication as authentication
 #}}}
 # fold: global parameters{{{
 ## PAIRS query meta data information file
 PAIRS_QUERY_METADATA_FILE_NAME      = u'output.info'
 ## PAIRS vector JSON file name
 PAIRS_VECTOR_CSV_FILE_NAME          = u'Vector_Data_Output.csv'
@@ -162,2514 +162,2514 @@
 # PAIRS time series parameters
 TIMESERIES_RESPONSE_FILE_SCHEMA     = '{layerID}_{lon}~{lat}_{t0}-{t1}.json'
 # load parameters from the command line
 PAW_LOG_LEVEL                       = logging.DEBUG #logging.INFO
 LOG_LEVEL_ENV                       = u''
 PAW_ENV_BASE_NAME                   = u'PAW'
 ENVIRONMENT_VARIABLES               = (
-    u'LOG_LEVEL_ENV',
-    u'CONFIGURE_LOGGING',
-    u'PAIRS_DEFAULT_SERVER',
-    u'PAIRS_DEFAULT_PROTOCOL',
-    u'PAIRS_DEFAULT_BASE_URI',
-    u'PAIRS_DEFAULT_USER',
-    u'PAIRS_DEFAULT_PASSWORD_FILE_NAME',
-    u'PAIRS_DEFAULT_PUBLISH_2_GUI',
-    u'PAIRS_DEFAULT_GUI_URL',
-    u'PAIRS_DEFAULT_GUI_TOKEN',
+        u'LOG_LEVEL_ENV',
+        u'CONFIGURE_LOGGING',
+        u'PAIRS_DEFAULT_SERVER',
+        u'PAIRS_DEFAULT_PROTOCOL',
+        u'PAIRS_DEFAULT_BASE_URI',
+        u'PAIRS_DEFAULT_USER',
+        u'PAIRS_DEFAULT_PASSWORD_FILE_NAME',
+        u'PAIRS_DEFAULT_PUBLISH_2_GUI',
+        u'PAIRS_DEFAULT_GUI_URL',
+        u'PAIRS_DEFAULT_GUI_TOKEN',
 )
 def load_environment_variables():
-    """
-    Some settings of this module can be set by environment variables. This function loads them.
+        """
+        Some settings of this module can be set by environment variables. This function loads them.
 
-    In particular, server credentials and connection details are set via
-    ``paw.ENVIRONMENT_VARIABLES`` prefixed by ``paw.PAW_ENV_BASE_NAME+'_'``, e.g. by
-    starting your Python shell with:
-
-    .. code-block:: bash
-
-       PAW_PAIRS_DEFAULT_USER='<your PAIRS user name>' PAW_PAIRS_DEFAULT_BASE_URI python
-    """
-    # set global variables reading from environment variables
-    for var in ENVIRONMENT_VARIABLES:
-        if PAW_ENV_BASE_NAME+'_'+var in os.environ:
-            exec(
-                "global {var}; {var} = os.environ['{pawBaseName}_{var}']".format(
-                    var=var, pawBaseName=PAW_ENV_BASE_NAME,
-                )
-            )
-    # adjust non-string variables
-    global PAW_LOG_LEVEL
-    if LOG_LEVEL_ENV == u"DEBUG":
-        PAW_LOG_LEVEL = logging.DEBUG
-    elif LOG_LEVEL_ENV == u"INFO":
-        PAW_LOG_LEVEL = logging.INFO
-    elif LOG_LEVEL_ENV == u"WARNING":
-        PAW_LOG_LEVEL = logging.WARNING
-    elif LOG_LEVEL_ENV == u"ERROR":
-        PAW_LOG_LEVEL = logging.ERROR
-    elif LOG_LEVEL_ENV == u"CRITICAL":
-        PAW_LOG_LEVEL = logging.CRITICAL
-    global CONFIGURE_LOGGING
-    if isinstance(CONFIGURE_LOGGING, str):
-        CONFIGURE_LOGGING = CONFIGURE_LOGGING.lower()=='true'
-    global PAIRS_DEFAULT_PUBLISH_2_GUI
-    if isinstance(CONFIGURE_LOGGING, str):
-        PAIRS_DEFAULT_PUBLISH_2_GUI = PAIRS_DEFAULT_PUBLISH_2_GUI.lower()=='true'
+        In particular, server credentials and connection details are set via
+        ``paw.ENVIRONMENT_VARIABLES`` prefixed by ``paw.PAW_ENV_BASE_NAME+'_'``, e.g. by
+        starting your Python shell with:
+
+        .. code-block:: bash
+
+             PAW_PAIRS_DEFAULT_USER='<your PAIRS user name>' PAW_PAIRS_DEFAULT_BASE_URI python
+        """
+        # set global variables reading from environment variables
+        for var in ENVIRONMENT_VARIABLES:
+                if PAW_ENV_BASE_NAME+'_'+var in os.environ:
+                        exec(
+                                "global {var}; {var} = os.environ['{pawBaseName}_{var}']".format(
+                                        var=var, pawBaseName=PAW_ENV_BASE_NAME,
+                                )
+                        )
+        # adjust non-string variables
+        global PAW_LOG_LEVEL
+        if LOG_LEVEL_ENV == u"DEBUG":
+                PAW_LOG_LEVEL = logging.DEBUG
+        elif LOG_LEVEL_ENV == u"INFO":
+                PAW_LOG_LEVEL = logging.INFO
+        elif LOG_LEVEL_ENV == u"WARNING":
+                PAW_LOG_LEVEL = logging.WARNING
+        elif LOG_LEVEL_ENV == u"ERROR":
+                PAW_LOG_LEVEL = logging.ERROR
+        elif LOG_LEVEL_ENV == u"CRITICAL":
+                PAW_LOG_LEVEL = logging.CRITICAL
+        global CONFIGURE_LOGGING
+        if isinstance(CONFIGURE_LOGGING, str):
+                CONFIGURE_LOGGING = CONFIGURE_LOGGING.lower()=='true'
+        global PAIRS_DEFAULT_PUBLISH_2_GUI
+        if isinstance(CONFIGURE_LOGGING, str):
+                PAIRS_DEFAULT_PUBLISH_2_GUI = PAIRS_DEFAULT_PUBLISH_2_GUI.lower()=='true'
 load_environment_variables()
 # }}}
 # fold: settings#{{{
 ## get (global) logger
 logger = logging.getLogger(__name__)
 ## set log level
 if CONFIGURE_LOGGING:
-    if HAS_COLOREDLOGS:
-        coloredlogs.install(
-            level       = PAW_LOG_LEVEL,
-            fmt='%(levelname)s - %(asctime)s: "%(message)s" [%(funcName)s]',
-            level_styles= {
-                'info':     {'color': 'green'},
-                'warning':  {'color': 'yellow'},
-                'error':    {'color': 'red'},
-                'critical': {'color': 'red', 'bold': True},
-            },
-            stream      = sys.stdout,
-            logger      = logger,
-        )
-    else:
-        logger.setLevel(PAW_LOG_LEVEL)
-        handler = logging.StreamHandler(sys.stdout)
-        handler.setFormatter(
-            logging.Formatter('%(levelname)s - %(asctime)s: "%(message)s" [%(funcName)s]'),
-        )
-        logger.addHandler(handler)
-    logging.debug("Log level set to: '{}'".format(logging.getLevelName(logger.getEffectiveLevel())))
+        if HAS_COLOREDLOGS:
+                coloredlogs.install(
+                        level       = PAW_LOG_LEVEL,
+                        fmt='%(levelname)s - %(asctime)s: "%(message)s" [%(funcName)s]',
+                        level_styles= {
+                                'info':     {'color': 'green'},
+                                'warning':  {'color': 'yellow'},
+                                'error':    {'color': 'red'},
+                                'critical': {'color': 'red', 'bold': True},
+                        },
+                        stream      = sys.stdout,
+                        logger      = logger,
+                )
+        else:
+                logger.setLevel(PAW_LOG_LEVEL)
+                handler = logging.StreamHandler(sys.stdout)
+                handler.setFormatter(
+                        logging.Formatter('%(levelname)s - %(asctime)s: "%(message)s" [%(funcName)s]'),
+                )
+                logger.addHandler(handler)
+        logging.debug("Log level set to: '{}'".format(logging.getLevelName(logger.getEffectiveLevel())))
 #}}}
 
 # fold: misc functions {{{
 def get_pairs_api_password(
-    server, user,
-    passFile=None,
+        server, user,
+        passFile=None,
 ):
-    '''
-    Tries to obtain the PAIRS API password for a given user on a given server.
+        '''
+        Tries to obtain the PAIRS API password for a given user on a given server.
 
-    :param server:      PAIRS API server name, e.g. 'pairs.res.ibm.com'
-    :type server:       str
-    :param user:        user name for which to obtain the corresponding password
-    :type user:         str
-    :param passFile:    path to file with password, it is expected to have the format
-                        `<server>:<user>:<password>`, colons in passwords need to be escaped
-    :type passFile:     str
-    :returns:           corresponding password if available, `None` otherwise
-                        *note*: if either user or server is `None`, no password searched
-                        for, and `None` is returned
-    :rtype:             str
-    :raises Exception:  if password file does not exist
-                        if password was not found
-    '''
-    # of either no user or server is provided
-    if server is None or user is None:
-        return None
-    # Search for a password file in (a) the current working directory and (b) $HOME
-    if passFile is None:
-        if os.path.isfile(os.path.join(os.getcwd(), PAIRS_DEFAULT_PASSWORD_FILE_NAME)):
-            passFile = os.path.join(os.getcwd(), PAIRS_DEFAULT_PASSWORD_FILE_NAME)
-        elif os.path.isfile(os.path.join(os.path.expanduser('~'), PAIRS_DEFAULT_PASSWORD_FILE_NAME)):
-            passFile = os.path.join(os.path.expanduser('~'), PAIRS_DEFAULT_PASSWORD_FILE_NAME)
-        else:
-            raise ValueError(
-                "passFile = None requires existence of a '{}' file in a default location.".format(
-                    PAIRS_DEFAULT_PASSWORD_FILE_NAME
-                )
-            )
+        :param server:      PAIRS API server name, e.g. 'pairs.res.ibm.com'
+        :type server:       str
+        :param user:        user name for which to obtain the corresponding password
+        :type user:         str
+        :param passFile:    path to file with password, it is expected to have the format
+                                                `<server>:<user>:<password>`, colons in passwords need to be escaped
+        :type passFile:     str
+        :returns:           corresponding password if available, `None` otherwise
+                                                *note*: if either user or server is `None`, no password searched
+                                                for, and `None` is returned
+        :rtype:             str
+        :raises Exception:  if password file does not exist
+                                                if password was not found
+        '''
+        # of either no user or server is provided
+        if server is None or user is None:
+                return None
+        # Search for a password file in (a) the current working directory and (b) $HOME
+        if passFile is None:
+                if os.path.isfile(os.path.join(os.getcwd(), PAIRS_DEFAULT_PASSWORD_FILE_NAME)):
+                        passFile = os.path.join(os.getcwd(), PAIRS_DEFAULT_PASSWORD_FILE_NAME)
+                elif os.path.isfile(os.path.join(os.path.expanduser('~'), PAIRS_DEFAULT_PASSWORD_FILE_NAME)):
+                        passFile = os.path.join(os.path.expanduser('~'), PAIRS_DEFAULT_PASSWORD_FILE_NAME)
+                else:
+                        raise ValueError(
+                                "passFile = None requires existence of a '{}' file in a default location.".format(
+                                        PAIRS_DEFAULT_PASSWORD_FILE_NAME
+                                )
+                        )
+
+        # Often the value to server is the same as some global variable PAIRS_SERVER
+        # That however if later handed to PAIRSQuery objects. The following code allows
+        # using PAIRS_SERVER='https://pairs.res.ibm.com' and avoids later use of
+        # 'https://'+PAIRS_SERVER
+        if server.startswith('https://'):
+                server = server[8:]
+
+        passFound = False
+        try:
+                # parse PAIRS API access password file
+                with open(passFile) as f:
+                        for line in f:
+                                if not re.match(PAIRS_PASSWORD_FILE_COMMENT_REG_EX, line):
+                                        serverF, userF, password  = re.split(r'(?<!\\):',line.strip())
+                                        password = password.replace(r'\:', ':')
+                                        if server == serverF and user == userF:
+                                                passFound = True
+                                                break
+        except EnvironmentError as e:
+                raise e
+        except Exception as e:
+                raise ValueError('Failed loading PAIRS password from {0}'.format(passFile))
 
-    # Often the value to server is the same as some global variable PAIRS_SERVER
-    # That however if later handed to PAIRSQuery objects. The following code allows
-    # using PAIRS_SERVER='https://pairs.res.ibm.com' and avoids later use of
-    # 'https://'+PAIRS_SERVER
-    if server.startswith('https://'):
-        server = server[8:]
-
-    passFound = False
-    try:
-        # parse PAIRS API access password file
-        with open(passFile) as f:
-            for line in f:
-                if not re.match(PAIRS_PASSWORD_FILE_COMMENT_REG_EX, line):
-                    serverF, userF, password  = re.split(r'(?<!\\):',line.strip())
-                    password = password.replace(r'\:', ':')
-                    if server == serverF and user == userF:
-                        passFound = True
-                        break
-    except EnvironmentError as e:
-        raise e
-    except Exception as e:
-        raise ValueError('Failed loading PAIRS password from {0}'.format(passFile))
-
-    # return password (if any)
-    if passFound:
-        return password
-    else:
-        raise ValueError('Unable to find PAIRS password for {0}@{1} in {2}.'.format(user, server, passFile))
+        # return password (if any)
+        if passFound:
+                return password
+        else:
+                raise ValueError('Unable to find PAIRS password for {0}@{1} in {2}.'.format(user, server, passFile))
 
 def getQueryHash(query):
-    return hashlib.md5(
-        json.dumps(query, sort_keys=True).encode('utf-8')
-    ).hexdigest()
+        return hashlib.md5(
+                json.dumps(query, sort_keys=True).encode('utf-8')
+        ).hexdigest()
 #}}}
 
 # fold: PAIRS query class for managing single queries {{{
 # set mocked query status
 class MockSubmitResponse():
-    """
-    Helper class for mocking a PAIRS query submit response.
+        """
+        Helper class for mocking a PAIRS query submit response.
 
-    It is useful to simulate a query submission when reloading a previously submitted
-    query based on a given PAIRS query ID.
-    """
-    def __init__(self, queryID, status_code=200):
-        self.status_code = status_code
-        self.queryID     = queryID
-        self.ok          = True
-    def json(self):
-        return {u'id': str(self.queryID)}
+        It is useful to simulate a query submission when reloading a previously submitted
+        query based on a given PAIRS query ID.
+        """
+        def __init__(self, queryID, status_code=200):
+                self.status_code = status_code
+                self.queryID     = queryID
+                self.ok          = True
+        def json(self):
+                return {u'id': str(self.queryID)}
 
 class PAIRSQuery(object):
-    """
-    Representation of a PAIRS query.
+        """
+        Representation of a PAIRS query.
 
-    :param query:               dictionary equivalent to PAIRS JSON load that defines a query or
-                                path that references a ZIP file identified with a PAIRS query or
-                                ID of existing (submitted) query
-    :type query:                dict or
-                                str
-    :param pairsHost:           base URL + scheme of PAIRS host to connect to,
-                                e.g. 'https://pairs.res.ibm.com'
-                                *note*: the initialization tries its best to autodetect
-                                even the `baseURI` and `port` if contained in `pairsHost` already
-    :type pairsHost:            str
-    :param auth:                user name and password as tuple for access to pairsHost
-    :type auth:                 (str, str) or authentication.OAuth2
-    :param port:                port to use for pairsHost
-    :type port:                 int
-    :param overwriteExisting:   destroy locally cached data, if existing, otherwise grab the latest
-                                locally cached data, `latest` is defined by alphanumerical ordering
-                                of the PAIRS query ID
-                                *note:* ignored in case of a file path (string) is provided as query
-    :type overwriteExisting:    bool
-    :param deleteDownload:      destroy downloaded data with destruction of class instance
-    :type deleteDownload:       bool
-    :param downloadDir:         directory where to store downloaded data
-                                note: ignored if the `query` is a string representing the
-                                PAIRS query ZIP directory
-    :type downloadDir:          str
-    :param baseURI:             PAIRS API base URI to append to the base URL (cf. `pairsHost`)
-    :type baseURI:              str
-    :param verifySSL:                          if SSL connections get verified
-    :type verifySSL:            bool
-    :param vectorFormat:        data format of the vector data
-    :type vectorFormat:         str
-    :param inMemory:            triggers storing files directly in memory
-                                note: ignored if query is loaded from existing ZIP file
-    :type inMemory:             bool
-    :param guiURL:              URL of PAIRS GUI to be used for publishing query result (if any)
-    :type guiURL:               str
-    :param publish2GUI:         determines whether or not the query result is automatically published
-                                to the PAIRS GUI
-    :type publish2GUI:          bool
-    :param guiPassword:         password to be used when PAIRS GUI password is different from
-                                PAIRS API password, note: the user is the same as for the PAIRS API
-                                (typically the user's e-mail address)
-    :type guiPassword:          str
-    :param authType:            'password' or 'api-key'
-    :type port:                 str
-    :raises Exception:          if an invalid URL was specified
-                                if the query defintion is not understood
-                                if a manually set PAIRS query ZIP directory does not exist
-    """
-    # class-wide constants/parameters
-    SUBMIT_API_STRING            = u'v2/query'
-    STATUS_API_STRING            = u'v2/queryjobs/'
-    DOWNLOAD_API_STRING          = u'v2/queryjobs/download/'
-    COS_UPLOAD_API_STRING        = u'v2/queryjobs/upload/'
-    COS_API_ENDPOINT             = u'https://s3.us.cloud-object-storage.appdomain.cloud'
-    COS_INFO_KEYS                = ('provider', 'endpoint', 'bucket', 'token')
-    GET_GEOJSON_API_STRING       = u'ws/queryaois/geojson/'
-    GET_AOI_INFO_API_STRING      = u'ws/queryaois/aoi/'
-    GET_QUERY_INFO               = u'v2/queryhistories/full/queryjob/'
-    LOGIN_2_GUI                  = u'users/login'
-    PUBLISH_QUERY_RESULT_2_GUI   = u'queryjobs/{queryID}/mapcorejob'
-    VECTOR_GEOJSON_DIR_IN_ZIP    = u''
-    DOWNLOAD_DIR                 = u'./downloads'
-    PAIRS_JUPYTER_QUERY_BASE_DIR = u'.'
-    STATUS_POLL_INTERVAL_SEC     = 10
-    PAIRS_FILES_TIMESTAMP_SCHEMA2= '%m_%d_%YT%H:%M:%S'
-    PAIRS_FILES_TIMESTAMP_SCHEMA = '%m_%d_%YT%H_%M_%S'
-    PAIRS_FILES_SPLITTING_CHAR   = '-'
-    RASTER_FILE_EXTENSION        = PAIRS_GEOTIFF_FILE_EXTENSION
-    VECTOR_FILE_EXTENSION        = PAIRS_CSV_FILE_EXTENSION
-    PAIRS_POINT_QUERY_RESP_FORMAT= 'text/csv' # 'application/json' # as alternative for JSON return
-
-    def __init__(
-        self, query,
-        pairsHost               = None,
-        auth                    = None,
-        port                    = None,
-        overwriteExisting       = True,
-        deleteDownload          = False,
-        downloadDir             = DOWNLOAD_DIR,
-        baseURI                 = None,
-        verifySSL               = True,
-        vectorFormat            = None,
-        inMemory                = False,
-        guiURL                  = None,
-        publish2GUI             = None,
-        guiPassword             = None,
-        authType                = 'password'
-    ):
-        self.authType = authType
-
-        # get default credentials
-        # check and set port for IBM PAIRS core API server
-        if port is not None:
-            if isinstance(port, int) and port > 0 and port < 65536:
-                self.pairsPort  = port
-            else:
-                logger.warning("Incorrect port number provided: {}, defaulting to port 80".format(port))
-                self.pairsPort  = 80
-        else:
-            self.pairsPort                  = None
-        # parse host URL serving PAIRS API to connect to
-        if pairsHost is None: pairsHost = '{}://{}'.format(
-            PAIRS_DEFAULT_PROTOCOL,
-            PAIRS_DEFAULT_SERVER,
-        )
-        self.pairsHost                  = urlparse(
-            u'' if pairsHost is None else pairsHost
-        )
-        if pairsHost is not None and self.pairsHost.scheme not in ['http', 'https']:
-            raise Exception(
-                "Invalid PAIRS host URL: {}\n correct example: 'https://pairs.res.ibm.com:80/'".format(pairsHost)
-            )
-        if self.pairsPort is not None:
-            if self.pairsHost.port is None:
-                self.pairsHost              = urlparse(
-                    '{}://{}:{}{}'.format(
-                        self.pairsHost.scheme, self.pairsHost.netloc, self.pairsPort, self.pairsHost.path
-                    )
-                )
-            elif self.pairsHost.port != self.pairsPort:
-                logger.warning(
-                    "Port explicitly specified by `port`='{}' clashes with `pairsHost`='{}' parsing, using spec from `pairsHost`.".format(
-                        port, pairsHost
-                    )
-                )
+        :param query:               dictionary equivalent to PAIRS JSON load that defines a query or
+                                                                path that references a ZIP file identified with a PAIRS query or
+                                                                ID of existing (submitted) query
+        :type query:                dict or
+                                                                str
+        :param pairsHost:           base URL + scheme of PAIRS host to connect to,
+                                                                e.g. 'https://pairs.res.ibm.com'
+                                                                *note*: the initialization tries its best to autodetect
+                                                                even the `baseURI` and `port` if contained in `pairsHost` already
+        :type pairsHost:            str
+        :param auth:                user name and password as tuple for access to pairsHost
+        :type auth:                 (str, str) or authentication.OAuth2
+        :param port:                port to use for pairsHost
+        :type port:                 int
+        :param overwriteExisting:   destroy locally cached data, if existing, otherwise grab the latest
+                                                                locally cached data, `latest` is defined by alphanumerical ordering
+                                                                of the PAIRS query ID
+                                                                *note:* ignored in case of a file path (string) is provided as query
+        :type overwriteExisting:    bool
+        :param deleteDownload:      destroy downloaded data with destruction of class instance
+        :type deleteDownload:       bool
+        :param downloadDir:         directory where to store downloaded data
+                                                                note: ignored if the `query` is a string representing the
+                                                                PAIRS query ZIP directory
+        :type downloadDir:          str
+        :param baseURI:             PAIRS API base URI to append to the base URL (cf. `pairsHost`)
+        :type baseURI:              str
+        :param verifySSL:                          if SSL connections get verified
+        :type verifySSL:            bool
+        :param vectorFormat:        data format of the vector data
+        :type vectorFormat:         str
+        :param inMemory:            triggers storing files directly in memory
+                                                                note: ignored if query is loaded from existing ZIP file
+        :type inMemory:             bool
+        :param guiURL:              URL of PAIRS GUI to be used for publishing query result (if any)
+        :type guiURL:               str
+        :param publish2GUI:         determines whether or not the query result is automatically published
+                                                                to the PAIRS GUI
+        :type publish2GUI:          bool
+        :param guiPassword:         password to be used when PAIRS GUI password is different from
+                                                                PAIRS API password, note: the user is the same as for the PAIRS API
+                                                                (typically the user's e-mail address)
+        :type guiPassword:          str
+        :param authType:            'password' or 'api-key'
+        :type port:                 str
+        :raises Exception:          if an invalid URL was specified
+                                                                if the query defintion is not understood
+                                                                if a manually set PAIRS query ZIP directory does not exist
+        """
+        # class-wide constants/parameters
+        SUBMIT_API_STRING            = u'v2/query'
+        STATUS_API_STRING            = u'v2/queryjobs/'
+        DOWNLOAD_API_STRING          = u'v2/queryjobs/download/'
+        COS_UPLOAD_API_STRING        = u'v2/queryjobs/upload/'
+        COS_API_ENDPOINT             = u'https://s3.us.cloud-object-storage.appdomain.cloud'
+        COS_INFO_KEYS                = ('provider', 'endpoint', 'bucket', 'token')
+        GET_GEOJSON_API_STRING       = u'ws/queryaois/geojson/'
+        GET_AOI_INFO_API_STRING      = u'ws/queryaois/aoi/'
+        GET_QUERY_INFO               = u'v2/queryhistories/full/queryjob/'
+        LOGIN_2_GUI                  = u'users/login'
+        PUBLISH_QUERY_RESULT_2_GUI   = u'queryjobs/{queryID}/mapcorejob'
+        VECTOR_GEOJSON_DIR_IN_ZIP    = u''
+        DOWNLOAD_DIR                 = u'./downloads'
+        PAIRS_JUPYTER_QUERY_BASE_DIR = u'.'
+        STATUS_POLL_INTERVAL_SEC     = 10
+        PAIRS_FILES_TIMESTAMP_SCHEMA2= '%m_%d_%YT%H:%M:%S'
+        PAIRS_FILES_TIMESTAMP_SCHEMA = '%m_%d_%YT%H_%M_%S'
+        PAIRS_FILES_SPLITTING_CHAR   = '-'
+        RASTER_FILE_EXTENSION        = PAIRS_GEOTIFF_FILE_EXTENSION
+        VECTOR_FILE_EXTENSION        = PAIRS_CSV_FILE_EXTENSION
+        PAIRS_POINT_QUERY_RESP_FORMAT= 'text/csv' # 'application/json' # as alternative for JSON return
+
+        def __init__(
+                self, query,
+                pairsHost               = None,
+                auth                    = None,
+                port                    = None,
+                overwriteExisting       = True,
+                deleteDownload          = False,
+                downloadDir             = DOWNLOAD_DIR,
+                baseURI                 = None,
+                verifySSL               = True,
+                vectorFormat            = None,
+                inMemory                = False,
+                guiURL                  = None,
+                publish2GUI             = None,
+                guiPassword             = None,
+                authType                = 'password'
+        ):
+                self.authType = authType
 
-        # make sure the baseURI has trailing and leading slash
-        if baseURI is None: baseURI = PAIRS_DEFAULT_BASE_URI
-        baseURIBeforeMerge = self.pairsHost.path
-        if len(baseURI)>0:
-            if baseURI[-1]!='/':    baseURI = baseURI+'/'
-            if baseURI[0]!='/':     baseURI = '/'+baseURI
-        # add baseURI to full PAIRS host specs (if any)
-        self.pairsHost = urlparse(
-            urljoin(
-                os.path.join(self.pairsHost.geturl(),''),
-                baseURI.lstrip('/')
-            )
-        )
-        # check merge vs. naive merge and inform user about deviation
-        if self.pairsHost.path != baseURIBeforeMerge+baseURI:
-            logger.warning(
-                "`pairsHost`='{}' and `baseURI`='{}' merged to: '{}'".format(
-                    pairsHost, baseURI, self.pairsHost.geturl(),
-                )
-            )
-        else:
-            logger.debug(
-                "The full PAIRS base URL reads: '{}'".format(self.pairsHost.geturl())
-            )
-
-        # use SSL verification
-        self.verifySSL                  = verifySSL
-        # PAIRS API authentication
-        if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-            if type(auth) is authentication.OAuth2:
-                self.auth = auth
-            else:
-                self.auth = authentication.OAuth2(host         = PAIRS_DEFAULT_SERVER,
-                                                  username     = PAIRS_DEFAULT_USER,
-                                                  api_key_file = PAIRS_DEFAULT_PASSWORD_FILE_NAME
-                                                 )
-        else:
-            self.auth                       = (
-                PAIRS_DEFAULT_USER,
-                get_pairs_api_password(
-                    server  = PAIRS_DEFAULT_SERVER,
-                    user    = PAIRS_DEFAULT_USER,
-                    passFile= PAIRS_DEFAULT_PASSWORD_FILE_NAME,
-                )
-            ) if auth is None else auth
+                # get default credentials
+                # check and set port for IBM PAIRS core API server
+                if port is not None:
+                        if isinstance(port, int) and port > 0 and port < 65536:
+                                self.pairsPort  = port
+                        else:
+                                logger.warning("Incorrect port number provided: {}, defaulting to port 80".format(port))
+                                self.pairsPort  = 80
+                else:
+                        self.pairsPort                  = None
+                # parse host URL serving PAIRS API to connect to
+                if pairsHost is None: pairsHost = '{}://{}'.format(
+                        PAIRS_DEFAULT_PROTOCOL,
+                        PAIRS_DEFAULT_SERVER,
+                )
+                self.pairsHost                  = urlparse(
+                        u'' if pairsHost is None else pairsHost
+                )
+                if pairsHost is not None and self.pairsHost.scheme not in ['http', 'https']:
+                        raise Exception(
+                                "Invalid PAIRS host URL: {}\n correct example: 'https://pairs.res.ibm.com:80/'".format(pairsHost)
+                        )
+                if self.pairsPort is not None:
+                        if self.pairsHost.port is None:
+                                self.pairsHost              = urlparse(
+                                        '{}://{}:{}{}'.format(
+                                                self.pairsHost.scheme, self.pairsHost.netloc, self.pairsPort, self.pairsHost.path
+                                        )
+                                )
+                        elif self.pairsHost.port != self.pairsPort:
+                                logger.warning(
+                                        "Port explicitly specified by `port`='{}' clashes with `pairsHost`='{}' parsing, using spec from `pairsHost`.".format(
+                                                port, pairsHost
+                                        )
+                                )
 
-        # set PAIRS GUI info for publishing query result
-        self.guiURL         = guiURL if guiURL is not None else PAIRS_DEFAULT_GUI_URL
-        if self.guiURL is not None and len(self.guiURL)>0:
-            if self.guiURL[-1]!='/': self.guiURL = self.guiURL+'/'
-        if self.guiURL is not None:
-            self.publish2GUI    = publish2GUI if publish2GUI is not None else PAIRS_DEFAULT_PUBLISH_2_GUI
-        else:
-            self.publish2GUI    = False
-        
-        # get PAIRS GUI token (for publishing PAIRS query result)
-        if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-            self.guiToken = self.auth.jwt_token
-        else:
-            self.guiPassword = guiPassword if guiPassword is not None else self.auth[1]
-            # get PAIRS GUI token (for publishing PAIRS query result)
-            if self.publish2GUI:
-                if PAIRS_DEFAULT_GUI_TOKEN is None:
-                    try:
-                        self.guiToken = requests.post(
-                            urljoin(self.guiURL, self.LOGIN_2_GUI),
-                            json    = {
-                                'email':    self.auth[0],
-                                'password': self.guiPassword,
-                            },
-                            headers = {
-                                'Content-Type': 'application/json',
-                                'Referer': 'http://localhost:80',
-                            },
-                            verify  = self.verifySSL,
-                        ).json()['token']
-                    except Exception as e:
-                        self.publish2GUI = False
+                # make sure the baseURI has trailing and leading slash
+                if baseURI is None: baseURI = PAIRS_DEFAULT_BASE_URI
+                baseURIBeforeMerge = self.pairsHost.path
+                if len(baseURI)>0:
+                        if baseURI[-1]!='/':    baseURI = baseURI+'/'
+                        if baseURI[0]!='/':     baseURI = '/'+baseURI
+                # add baseURI to full PAIRS host specs (if any)
+                self.pairsHost = urlparse(
+                        urljoin(
+                                os.path.join(self.pairsHost.geturl(),''),
+                                baseURI.lstrip('/')
+                        )
+                )
+                # check merge vs. naive merge and inform user about deviation
+                if self.pairsHost.path != baseURIBeforeMerge+baseURI:
                         logger.warning(
-                                "Ah, cannot get token for PAIRS GUI (publish query result disabled): {}".format(e)
+                                "`pairsHost`='{}' and `baseURI`='{}' merged to: '{}'".format(
+                                        pairsHost, baseURI, self.pairsHost.geturl(),
+                                )
                         )
                 else:
-                    self.guiToken = PAIRS_DEFAULT_GUI_TOKEN
+                        logger.debug(
+                                "The full PAIRS base URL reads: '{}'".format(self.pairsHost.geturl())
+                        )
 
-        # set base URI
-        self.baseURI                    = self.pairsHost.path
+                # use SSL verification
+                self.verifySSL                  = verifySSL
+                # PAIRS API authentication
+                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                        if type(auth) is authentication.OAuth2:
+                                self.auth = auth
+                        else:
+                                self.auth = authentication.OAuth2(host         = PAIRS_DEFAULT_SERVER,
+                                                                                                    username     = PAIRS_DEFAULT_USER,
+                                                                                                    api_key_file = PAIRS_DEFAULT_PASSWORD_FILE_NAME
+                                                                                                 )
+                else:
+                        self.auth                       = (
+                                PAIRS_DEFAULT_USER,
+                                get_pairs_api_password(
+                                        server  = PAIRS_DEFAULT_SERVER,
+                                        user    = PAIRS_DEFAULT_USER,
+                                        passFile= PAIRS_DEFAULT_PASSWORD_FILE_NAME,
+                                )
+                        ) if auth is None else auth
 
-        # query information retrieved via PAIRS API
-        self.queryInfo                  = None
-        # associated PAIRS query ID (found in the JSON load)
-        self.queryID                    = None
-
-        # variable for file system object
-        self.fs                         = None
-        # variable for file system of query result
-        self.queryFS                    = None
-        # variable for query result data stream
-        self._queryStream               = None
-        # define whether or not to use virtual disk in memory for query result
-        self.inMemory                   = inMemory
-
-        # define query (depending on what information is provided)
-        ## assumption on whether or not the query immediately returns
-        ## (e.g. for point query without batch processing)
-        self._isOnlineQuery             = False
-        ## submit of query
-        self.querySubmit                = None
-        # flag for how to handle downloaded data on object delete
-        self.deleteDownload             = deleteDownload
-        ## JSON load defining the query
-        if isinstance(query, dict):
-            # assign query JSON definition
-            self.query                  = query
-            self.zipFilePath            = None
-            # determine the query whether or not the query immediately returns (e.g. for point query)
-            self._isOnlineQuery         =  self.query['spatial']['type'] == PAIRS_POINT_QUERY_NAME \
-                and (not self.query['batch'] if 'batch' in self.query else True)
-            logger.info(
-                'PAIRS query JSON initialized{}.'.format(' as online query' if self._isOnlineQuery else '')
-            )
-        elif isinstance(query, string_type):
-            ## ZIP file path storing the PAIRS query result
-            # TODO: detect and incorporate case where string represents e.g. COS
-            #       to be abstracted by pyfilesystem2, i.e. split apart COS part
-            #       from zipFilePath
-            if os.path.exists(query):
-                self.zipFilePath        = str(query)
-                self.query              = None
-                # reset in memory user option, since contradicting
-                self.inMemory           = False
-                logger.info("Will load PAIRS query data from '{}'.".format(query))
-            else:
-                ## PAIRS query ID defining the query result
-                try:
-                    self.query          = self.get_query_JSON(query)
-                except Exception as e:
-                    self.query          = None
-                    logger.warning(
-                        "Unable to fetch query definition from PAIRS for query ID '{}': {}".format(query, e)
-                    )
-                self.queryID            = query
-                self.zipFilePath        = None
-                self.querySubmit        = MockSubmitResponse(self.queryID)
-                logger.info("Will load PAIRS query data from '{}'.".format(query))
-        else:
-            raise Exception(
-                "Query definition of type '{}' not an option.".format(type(query))
-            )
-
-        # folder to save query result
-        self.downloadDir         = str(
-            os.path.dirname(self.zipFilePath) if self.zipFilePath is not None else downloadDir
-        )
-        # separate ZIP file name from directory (if any)
-        # note: the download directory where the ZIP file is located gets abstracted
-        # away by self.fs
-        if self.zipFilePath is not None:
-            self.zipFilePath = os.path.basename(self.zipFilePath)
-        # overwriting download directory according to ZIP directory information given (if any)
-        if self.downloadDir is not None and not self.inMemory and not os.path.exists(self.downloadDir):
-            os.mkdir(self.downloadDir)
-            logger.info("Download directory '{}' created.".format(self.downloadDir))
-        # file system for query storage
-        self._openDataSource(force=True)
-        # hash of the JSON query
-        # (used as subfolder for saving files and to see if corresponding Tiff already exists)
-        self.qHash               = getQueryHash(query if isinstance(self.query, dict) else {})
-        # overwrite existing files
-        self.overwriteExisting   = overwriteExisting if (
-            isinstance(self.query, dict) or isinstance(self.querySubmit, MockSubmitResponse)
-        ) else False
-        # Query directory
-        self.queryDir            = None
-        # status of query
-        self.queryStatus         = None
-        # flag to indicate a failed Zip or GeoTiff generation. Used to re-issue the query
-        self.BadDownloadFile     = None
-        # general query metadata (based on `output.info`)
-        self.metadata            = None
-        # dict of in-memory data of the query result indexed by the file's name
-        self.data                = dict()
-        self.vectorFormat        = vectorFormat
-        # data frame of the vector data
-        self.vdf                 = None
-        # geo data frame with query polygon information
-        self.pdf                 = None
-        # keyword to indicate translation of timestamp column in the dataframe.
-        # data acknowledgement information
-        self.dataAcknowledgeText = None
-        # if loading data from existing ZIP, get the data acknowledgement
-        if isinstance(query, string_type):
-            try:
-                self.read_data_acknowledgement()
-            except Exception as e:
-                pass
-        if isinstance(self.fs, fs.memoryfs.MemoryFS):
-            logger.info('Just FYI: Local file system is in memory - no data saved on local disk.')
-        # add flag for IBM cloud object storage result specification
-        self.inIBMCOS            = False
-
-    def __del__(self):
-        # Delete the file and folder
-        if self.deleteDownload and (not self.queryDir is None):
-            if self.fs.exists(self.queryDir):
-                try:
-                    # Remove the folder with all its contents
-                    self.fs.removetree(self.queryDir)
-                except Exception as e:
-                    logger.warning(
-                        "Unable to delete query directory '{}': {}.".format(self.queryDir, e)
-                    )
+                # set PAIRS GUI info for publishing query result
+                self.guiURL         = guiURL if guiURL is not None else PAIRS_DEFAULT_GUI_URL
+                if self.guiURL is not None and len(self.guiURL)>0:
+                        if self.guiURL[-1]!='/': self.guiURL = self.guiURL+'/'
+                if self.guiURL is not None:
+                        self.publish2GUI    = publish2GUI if publish2GUI is not None else PAIRS_DEFAULT_PUBLISH_2_GUI
                 else:
-                    logger.info("Query directory '{}' delete.".format(self.queryDir))
-            # Remove the zip file
-            try:
-                self.fs.remove(self.queryDir + PAIRS_ZIP_FILE_EXTENSION)
-            except Exception as e:
-                logger.warning(
-                    "Unable to delete query result ZIP file '{}': {}.".format(self.queryDir, e)
-                )
-            else:
-                logger.info(
-                    "Query result ZIP file '{}' deleted.".format(self.queryDir)
-                )
-        # decouple from file system
-        try:
-            self._closeDataSource(force=True)
-        except Exception as e:
-            logger.error('Cannot properly close file system handlers: {}'.format(e))
+                        self.publish2GUI    = False
+                
+                # get PAIRS GUI token (for publishing PAIRS query result)
+                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                        self.guiToken = self.auth.jwt_token
+                else:
+                        self.guiPassword = guiPassword if guiPassword is not None else self.auth[1]
+                        # get PAIRS GUI token (for publishing PAIRS query result)
+                        if self.publish2GUI:
+                                if PAIRS_DEFAULT_GUI_TOKEN is None:
+                                        try:
+                                                self.guiToken = requests.post(
+                                                        urljoin(self.guiURL, self.LOGIN_2_GUI),
+                                                        json    = {
+                                                                'email':    self.auth[0],
+                                                                'password': self.guiPassword,
+                                                        },
+                                                        headers = {
+                                                                'Content-Type': 'application/json',
+                                                                'Referer': 'http://localhost:80',
+                                                        },
+                                                        verify  = self.verifySSL,
+                                                ).json()['token']
+                                        except Exception as e:
+                                                self.publish2GUI = False
+                                                logger.warning(
+                                                                "Ah, cannot get token for PAIRS GUI (publish query result disabled): {}".format(e)
+                                                )
+                                else:
+                                        self.guiToken = PAIRS_DEFAULT_GUI_TOKEN
 
-    def _openDataSource(self, force=False):
-        """
-        Wrapper function to properly open the data source associated with query.
+                # set base URI
+                self.baseURI                    = self.pairsHost.path
 
-        *notes*:
-            - Designed to be immutable. Use `self._closeDataSource()` to open the
-              data source from scratch.
-            - `KEEP_QUERY_SOURCE_DIR_OPEN` lets the function skip any operation
-              except for when it is forced.
-
-        :param force:   enforce to open data source, independent of global settings
-        :type force:    bool
-        :returns:       function actually attached and/or opened the data source
-        :rtype:         bool
-        """
-        if not KEEP_QUERY_SOURCE_DIR_OPEN or force:
-            if force: logger.debug("Enforcing data source to open.")
-            hasOpened=False
-            if self.fs is None or self.fs.isclosed():
-                try:
-                    if self.inMemory:
-                        # create in-memory file system
-                        self.fs = fs.open_fs(u'mem://')
-                        # ignore user set download directory
-                        self.downloadDir=u''
-                        logger.debug("Attached to virtual, volatile memory.")
-                    else:
-                        self.fs = fs.open_fs(self.downloadDir)
-                        logger.debug("Attached to directory '{}'".format(self.downloadDir))
-                    hasOpened = True
-                except Exception as e:
-                    raise Exception(
-                        "Unable to initialize download directory '{}': {}".format(self.downloadDir, e)
-                    )
-            # try to open the ZIP file (if any)
-            if self.zipFilePath is not None:
-                try:
-                    # get query stream if not existing or not open
-                    if self._queryStream is None or not self._queryStream.readable():
-                        # try to close unusable ZIP file stream
+                # query information retrieved via PAIRS API
+                self.queryInfo                  = None
+                # associated PAIRS query ID (found in the JSON load)
+                self.queryID                    = None
+
+                # variable for file system object
+                self.fs                         = None
+                # variable for file system of query result
+                self.queryFS                    = None
+                # variable for query result data stream
+                self._queryStream               = None
+                # define whether or not to use virtual disk in memory for query result
+                self.inMemory                   = inMemory
+
+                # define query (depending on what information is provided)
+                ## assumption on whether or not the query immediately returns
+                ## (e.g. for point query without batch processing)
+                self._isOnlineQuery             = False
+                ## submit of query
+                self.querySubmit                = None
+                # flag for how to handle downloaded data on object delete
+                self.deleteDownload             = deleteDownload
+                ## JSON load defining the query
+                if isinstance(query, dict):
+                        # assign query JSON definition
+                        self.query                  = query
+                        self.zipFilePath            = None
+                        # determine the query whether or not the query immediately returns (e.g. for point query)
+                        self._isOnlineQuery         =  self.query['spatial']['type'] == PAIRS_POINT_QUERY_NAME \
+                                and (not self.query['batch'] if 'batch' in self.query else True)
+                        logger.info(
+                                'PAIRS query JSON initialized{}.'.format(' as online query' if self._isOnlineQuery else '')
+                        )
+                elif isinstance(query, string_type):
+                        ## ZIP file path storing the PAIRS query result
+                        # TODO: detect and incorporate case where string represents e.g. COS
+                        #       to be abstracted by pyfilesystem2, i.e. split apart COS part
+                        #       from zipFilePath
+                        if os.path.exists(query):
+                                self.zipFilePath        = str(query)
+                                self.query              = None
+                                # reset in memory user option, since contradicting
+                                self.inMemory           = False
+                                logger.info("Will load PAIRS query data from '{}'.".format(query))
+                        else:
+                                ## PAIRS query ID defining the query result
+                                try:
+                                        self.query          = self.get_query_JSON(query)
+                                except Exception as e:
+                                        self.query          = None
+                                        logger.warning(
+                                                "Unable to fetch query definition from PAIRS for query ID '{}': {}".format(query, e)
+                                        )
+                                self.queryID            = query
+                                self.zipFilePath        = None
+                                self.querySubmit        = MockSubmitResponse(self.queryID)
+                                logger.info("Will load PAIRS query data from '{}'.".format(query))
+                else:
+                        raise Exception(
+                                "Query definition of type '{}' not an option.".format(type(query))
+                        )
+
+                # folder to save query result
+                self.downloadDir         = str(
+                        os.path.dirname(self.zipFilePath) if self.zipFilePath is not None else downloadDir
+                )
+                # separate ZIP file name from directory (if any)
+                # note: the download directory where the ZIP file is located gets abstracted
+                # away by self.fs
+                if self.zipFilePath is not None:
+                        self.zipFilePath = os.path.basename(self.zipFilePath)
+                # overwriting download directory according to ZIP directory information given (if any)
+                if self.downloadDir is not None and not self.inMemory and not os.path.exists(self.downloadDir):
+                        os.mkdir(self.downloadDir)
+                        logger.info("Download directory '{}' created.".format(self.downloadDir))
+                # file system for query storage
+                self._openDataSource(force=True)
+                # hash of the JSON query
+                # (used as subfolder for saving files and to see if corresponding Tiff already exists)
+                self.qHash               = getQueryHash(query if isinstance(self.query, dict) else {})
+                # overwrite existing files
+                self.overwriteExisting   = overwriteExisting if (
+                        isinstance(self.query, dict) or isinstance(self.querySubmit, MockSubmitResponse)
+                ) else False
+                # Query directory
+                self.queryDir            = None
+                # status of query
+                self.queryStatus         = None
+                # flag to indicate a failed Zip or GeoTiff generation. Used to re-issue the query
+                self.BadDownloadFile     = None
+                # general query metadata (based on `output.info`)
+                self.metadata            = None
+                # dict of in-memory data of the query result indexed by the file's name
+                self.data                = dict()
+                self.vectorFormat        = vectorFormat
+                # data frame of the vector data
+                self.vdf                 = None
+                # geo data frame with query polygon information
+                self.pdf                 = None
+                # keyword to indicate translation of timestamp column in the dataframe.
+                # data acknowledgement information
+                self.dataAcknowledgeText = None
+                # if loading data from existing ZIP, get the data acknowledgement
+                if isinstance(query, string_type):
                         try:
-                            self._queryStream.close()
-                        except:
-                            pass
-                        self._queryStream   = self.fs.open(self.zipFilePath, 'rb')
-                        # try to close any previous open file system
-                        if self.queryFS is not None:
-                            try:
-                                self.queryFS.close()
-                            except:
+                                self.read_data_acknowledgement()
+                        except Exception as e:
                                 pass
-                        # open file system
-                        self.queryFS        = zipfs.ZipFS(self._queryStream, write=False)
-                        logger.debug("Opened data source '{}'".format(self.zipFilePath))
-                    # test file system by listing contents
-                    self.queryFS.listdir(u'')
-                    hasOpened = True
+                if isinstance(self.fs, fs.memoryfs.MemoryFS):
+                        logger.info('Just FYI: Local file system is in memory - no data saved on local disk.')
+                # add flag for IBM cloud object storage result specification
+                self.inIBMCOS            = False
+
+        def __del__(self):
+                # Delete the file and folder
+                if self.deleteDownload and (not self.queryDir is None):
+                        if self.fs.exists(self.queryDir):
+                                try:
+                                        # Remove the folder with all its contents
+                                        self.fs.removetree(self.queryDir)
+                                except Exception as e:
+                                        logger.warning(
+                                                "Unable to delete query directory '{}': {}.".format(self.queryDir, e)
+                                        )
+                                else:
+                                        logger.info("Query directory '{}' delete.".format(self.queryDir))
+                        # Remove the zip file
+                        try:
+                                self.fs.remove(self.queryDir + PAIRS_ZIP_FILE_EXTENSION)
+                        except Exception as e:
+                                logger.warning(
+                                        "Unable to delete query result ZIP file '{}': {}.".format(self.queryDir, e)
+                                )
+                        else:
+                                logger.info(
+                                        "Query result ZIP file '{}' deleted.".format(self.queryDir)
+                                )
+                # decouple from file system
+                try:
+                        self._closeDataSource(force=True)
                 except Exception as e:
-                    raise Exception('Hm, cannot load data from ZIP file: {}'.format(e))
-                # flags prominently that query data is downloaded and available as files to be loaded
-                if force: self.downloaded = True
-            else:
-                # flag data is not downloaded, yet
-                if force: self.downloaded = False
-
-            if not hasOpened: logger.debug("Left data source open status untouched.")
-
-            return hasOpened
-        else:
-            return False
-
-    def _closeDataSource(self, force=False):
-        """
-        Wrapper function to properly close the data source associated with query.
-
-        After the call all file system descriptors are certainly detached from the
-        query object, except for the cases where
-            - the global variable `KEEP_QUERY_SOURCE_DIR_OPEN=True`
-            - the data source resides in (volatile) memory
-
-        Regardless, the `force=True` option can explicitly enforce the close.
-
-        :param force:   enforce to close data source, independent of global settings
-        :type force:    bool
-        :returns:       function performed closing
-        :rtype:         bool
-        """
-        if not (KEEP_QUERY_SOURCE_DIR_OPEN or self.inMemory) or force:
-            try:
-                self.queryFS.close()
-            except:
-                pass
-            finally:
-                self.queryFS = None
-            try:
-                self._queryStream.close()
-            except:
-                pass
-            finally:
-                self._queryStream = None
-            try:
-                self.fs.close()
-            except:
-                pass
-            finally:
-                self.fs = None
-            logger.debug("Data source closed{}.".format(' (enforced)' if force else ''))
-            return True
-        else:
-            logger.debug("Skipped closing data source.")
-            return False
+                        logger.error('Cannot properly close file system handlers: {}'.format(e))
 
+        def _openDataSource(self, force=False):
+                """
+                Wrapper function to properly open the data source associated with query.
+
+                *notes*:
+                        - Designed to be immutable. Use `self._closeDataSource()` to open the
+                            data source from scratch.
+                        - `KEEP_QUERY_SOURCE_DIR_OPEN` lets the function skip any operation
+                            except for when it is forced.
+
+                :param force:   enforce to open data source, independent of global settings
+                :type force:    bool
+                :returns:       function actually attached and/or opened the data source
+                :rtype:         bool
+                """
+                if not KEEP_QUERY_SOURCE_DIR_OPEN or force:
+                        if force: logger.debug("Enforcing data source to open.")
+                        hasOpened=False
+                        if self.fs is None or self.fs.isclosed():
+                                try:
+                                        if self.inMemory:
+                                                # create in-memory file system
+                                                self.fs = fs.open_fs(u'mem://')
+                                                # ignore user set download directory
+                                                self.downloadDir=u''
+                                                logger.debug("Attached to virtual, volatile memory.")
+                                        else:
+                                                self.fs = fs.open_fs(self.downloadDir)
+                                                logger.debug("Attached to directory '{}'".format(self.downloadDir))
+                                        hasOpened = True
+                                except Exception as e:
+                                        raise Exception(
+                                                "Unable to initialize download directory '{}': {}".format(self.downloadDir, e)
+                                        )
+                        # try to open the ZIP file (if any)
+                        if self.zipFilePath is not None:
+                                try:
+                                        # get query stream if not existing or not open
+                                        if self._queryStream is None or not self._queryStream.readable():
+                                                # try to close unusable ZIP file stream
+                                                try:
+                                                        self._queryStream.close()
+                                                except:
+                                                        pass
+                                                self._queryStream   = self.fs.open(self.zipFilePath, 'rb')
+                                                # try to close any previous open file system
+                                                if self.queryFS is not None:
+                                                        try:
+                                                                self.queryFS.close()
+                                                        except:
+                                                                pass
+                                                # open file system
+                                                self.queryFS        = zipfs.ZipFS(self._queryStream, write=False)
+                                                logger.debug("Opened data source '{}'".format(self.zipFilePath))
+                                        # test file system by listing contents
+                                        self.queryFS.listdir(u'')
+                                        hasOpened = True
+                                except Exception as e:
+                                        raise Exception('Hm, cannot load data from ZIP file: {}'.format(e))
+                                # flags prominently that query data is downloaded and available as files to be loaded
+                                if force: self.downloaded = True
+                        else:
+                                # flag data is not downloaded, yet
+                                if force: self.downloaded = False
 
-    def get_query_JSON(self, queryID, reloadData=False):
-        """
-        Obtain JSON load that defines a PAIRS query assigned a given ID.
+                        if not hasOpened: logger.debug("Left data source open status untouched.")
 
-        :param queryID:         PAIRS query ID for which to obtain the defining query JSON load
-        :type queryID:          str
-        :param reloadData:      triggers usage of already retrieved/cached data
-        :type reloadData:       bool
-        :returns:               PAIRS query defining JSON load
-        :rtype:                 dict
-        :raises Exception:      if the data cannot be obtained from PAIRS through an API call
-                                if cached data do not contain valid JSON load information
-        """
-        # use cached data (if any)
-        if not reloadData and self.queryInfo is not None:
-            try:
-                return self.queryInfo['apiJson']
-            except Exception as e:
-                logger.error(
-                    "Unable to extract query JSON load from PAIRS query info: '{}'.".format(e)
-                )
-                raise
-        # query data through PAIRS API
-        else:
-            # construct RESTful endpoint
-            queryInfoURL = urljoin(
-                urljoin(
-                    self.pairsHost.geturl(),
-                    self.GET_QUERY_INFO
-                ),
-                queryID
-            )
-            # query for information
-            try:
-                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-                    headers = {}
-                    token = 'Bearer ' + self.auth.jwt_token
-                    headers['Authorization'] = token
-                    resp = requests.get(
-                        queryInfoURL,
-                        verify  = self.verifySSL,
-                        headers = headers,
-                    )
+                        return hasOpened
                 else:
-                    resp = requests.get(
-                        queryInfoURL,
-                        auth    = self.auth,
-                        verify  = self.verifySSL,
-                    )
-                if resp.status_code != 200:
-                    raise Exception('Sorry, bad response with code: {}'.format(resp.status_code))
-                self.queryInfo = resp.json()
-                # convert string to dict
-                self.queryInfo['apiJson'] = json.loads(
-                    self.queryInfo['apiJson']
-                )
-
-                return self.queryInfo['apiJson']
-            except Exception as e:
-                logger.error(
-                    "Unable to fetch query information from PAIRS for ID '{}': '{}'".format(
-                        queryID, e
-                    )
-                )
-                raise
-
-
-    @classmethod
-    def from_query_result_dir(
-        cls, queryDir,
-        pairsHost    = None,
-        queryID      = None,
-        baseURI      = None,
-    ):
-        """
-        Generates a PAIRS query object from a native PAIRS query directory.
-
-        *Note*: Used for PAIRS query Jupyter notebook service.
-
-        :param queryDir:        query directory from which to load raster and vector data
-        :type queryDir:         str
-        :param pairsHost:       PAIRS host to be used for PAIRS API calls
-        :type pairsHost:        str
-        :param queryID:         PAIRS query ID associated with the data folder queryDir
-        :type queryID:          str
-        :param baseURI:         base URI to use for PAIRS API calls
-        :type baseURI:          str
-        :returns:               PAIRS API wrapper query object
-        :rtype:                 api_wrapper.PAIRSQuery
-        """
-        if baseURI is None: baseURI = PAIRS_DEFAULT_BASE_URI
-        clsInstance = cls(
-            query               = None,
-            pairsHost           = pairsHost,
-            baseURI             = baseURI,
-            auth                = None,
-            downloadDir         = None,
-            overwriteExisting   = False,
-        )
-        # indicate that the data does not need to be downloaded
-        clsInstance.downloaded  = True
-        # set PAIRS query base directory
-        # note: incorporates a hack due to a bug in the fs Python module (on parsing)
-        clsInstance.queryFS     = OSFS(queryDir)
-        # load all raster and vector data
-        logger.info('Loading query result into memory ...')
-        # load all queried layers
-        clsInstance.create_layers()
-        logger.info('... done.')
-
-        return clsInstance
-
-    def get_query_dir_name(self):
-        """
-        Compute query directory name by setting self.queryDir.
+                        return False
 
-        :raises Exception:  if required information is missing
-                            if the query hash cannot be constructed
-        """
-        # recompute query hash
-        try:
-            self.qHash = getQueryHash(self.query if isinstance(self.query, dict) else {})
-        except:
-            errMsg = u'Unable to determine query hash.'
-            logger.error(errMsg)
-            raise Exception(errMsg)
-
-        # construct query directory name
-        # note: download directory abstracted away by self.fs
-        if self.queryID is not None:
-            self.queryDir = str(
-                    self.queryID + '_' + self.qHash
-            )
-        elif self.zipFilePath is not None:
-            self.queryDir = str(os.path.dirname(self.zipFilePath))
-        else:
-            msg = u'Information to construct query directory incomplete.'
-            logger.warning(msg)
-            raise Exception(msg)
+        def _closeDataSource(self, force=False):
+                """
+                Wrapper function to properly close the data source associated with query.
+
+                After the call all file system descriptors are certainly detached from the
+                query object, except for the cases where
+                        - the global variable `KEEP_QUERY_SOURCE_DIR_OPEN=True`
+                        - the data source resides in (volatile) memory
+
+                Regardless, the `force=True` option can explicitly enforce the close.
+
+                :param force:   enforce to close data source, independent of global settings
+                :type force:    bool
+                :returns:       function performed closing
+                :rtype:         bool
+                """
+                if not (KEEP_QUERY_SOURCE_DIR_OPEN or self.inMemory) or force:
+                        try:
+                                self.queryFS.close()
+                        except:
+                                pass
+                        finally:
+                                self.queryFS = None
+                        try:
+                                self._queryStream.close()
+                        except:
+                                pass
+                        finally:
+                                self._queryStream = None
+                        try:
+                                self.fs.close()
+                        except:
+                                pass
+                        finally:
+                                self.fs = None
+                        logger.debug("Data source closed{}.".format(' (enforced)' if force else ''))
+                        return True
+                else:
+                        logger.debug("Skipped closing data source.")
+                        return False
 
-    def read_data_acknowledgement(self):
-        """
-        Extracts data acknowledge statement from PAIRS query result ZIP file.
 
-        :raises Exception:      if no acknowledgement is found
-        """
-        # attempt to extract only if not set already
-        self._openDataSource()
-        try:
-            if self.dataAcknowledgeText is None and self.queryFS is not None:
-                # check that there exists a file with the acknowledgement
-                if self.fs.exists(self.zipFilePath) and \
-                   PAIRS_DATA_ACK_FILE_NAME in self.queryFS.listdir(u''):
-                    # extract data acknowledgement from PAIRS query ZIP file
-                    try:
-                        with self.queryFS.open(PAIRS_DATA_ACK_FILE_NAME, 'rb') as f:
-                            self.dataAcknowledgeText = ''.join(codecs.getreader('utf-8')(f))
-                        logger.info('Data acknowledgement successfully loaded, print with `self.print_data_acknowledgement()`')
-                    except Exception as e:
-                        msg = u'Unable to read data acknowledgement from PAIRS query result ZIP file: {}'.format(e)
-                        logger.error(msg)
-                        raise Exception(msg)
+        def get_query_JSON(self, queryID, reloadData=False):
+                """
+                Obtain JSON load that defines a PAIRS query assigned a given ID.
+
+                :param queryID:         PAIRS query ID for which to obtain the defining query JSON load
+                :type queryID:          str
+                :param reloadData:      triggers usage of already retrieved/cached data
+                :type reloadData:       bool
+                :returns:               PAIRS query defining JSON load
+                :rtype:                 dict
+                :raises Exception:      if the data cannot be obtained from PAIRS through an API call
+                                                                if cached data do not contain valid JSON load information
+                """
+                # use cached data (if any)
+                if not reloadData and self.queryInfo is not None:
+                        try:
+                                return self.queryInfo['apiJson']
+                        except Exception as e:
+                                logger.error(
+                                        "Unable to extract query JSON load from PAIRS query info: '{}'.".format(e)
+                                )
+                                raise
+                # query data through PAIRS API
                 else:
-                    msg = u'No PAIRS query ZIP file identified, or no acknowledgement in ZIP file found. Did you run `self.download()`, yet?'
-                    logger.warning(msg)
-                    raise Exception(msg)
-            else:
-                logger.info('Data acknowledgement loaded already - print with `self.print_data_acknowledgement()`')
-        except:
-            raise
-        finally:
-            self._closeDataSource()
-
-    def print_data_acknowledgement(self):
-        """
-        Simply print out data acknowledgement statement.
+                        # construct RESTful endpoint
+                        queryInfoURL = urljoin(
+                                urljoin(
+                                        self.pairsHost.geturl(),
+                                        self.GET_QUERY_INFO
+                                ),
+                                queryID
+                        )
+                        # query for information
+                        try:
+                                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                                        headers = {}
+                                        token = 'Bearer ' + self.auth.jwt_token
+                                        headers['Authorization'] = token
+                                        resp = requests.get(
+                                                queryInfoURL,
+                                                verify  = self.verifySSL,
+                                                headers = headers,
+                                        )
+                                else:
+                                        resp = requests.get(
+                                                queryInfoURL,
+                                                auth    = self.auth,
+                                                verify  = self.verifySSL,
+                                        )
+                                if resp.status_code != 200:
+                                        raise Exception('Sorry, bad response with code: {}'.format(resp.status_code))
+                                self.queryInfo = resp.json()
+                                # convert string to dict
+                                self.queryInfo['apiJson'] = json.loads(
+                                        self.queryInfo['apiJson']
+                                )
 
-        """
-        try:
-            self.read_data_acknowledgement()
-        except:
-            pass
-        print("The data acknowledgement for self.data is:\n{}".format(self.dataAcknowledgeText))
+                                return self.queryInfo['apiJson']
+                        except Exception as e:
+                                logger.error(
+                                        "Unable to fetch query information from PAIRS for ID '{}': '{}'".format(
+                                                queryID, e
+                                        )
+                                )
+                                raise
 
 
-    def submit(self):
-        """
-        Submit query to PAIRS (if defined).
+        @classmethod
+        def from_query_result_dir(
+                cls, queryDir,
+                pairsHost    = None,
+                queryID      = None,
+                baseURI      = None,
+        ):
+                """
+                Generates a PAIRS query object from a native PAIRS query directory.
 
-        :raises Exception:  if no query is defined
-                            if no local cache is available which is requested to use
-                            if no PAIRS query ID can be identified from the return of the PAIRS server
-        """
+                *Note*: Used for PAIRS query Jupyter notebook service.
 
-        # get information for if-statement to follow from data source (if any)
-        locallyCachedZIP = False
-        try:
-            self._openDataSource()
-            locallyCachedZIP = self.fs.exists(self.zipFilePath)
-        except:
-            pass
-        finally:
-            self._closeDataSource()
-        if self.query is not None:
-            # fake submit for using existing cache
-            if not self.overwriteExisting:
-                logger.warning("Fake submit to PAIRS in order to use (latest) locally cached data.")
-                # check whether locally cache exists at all
-                self._openDataSource()
+                :param queryDir:        query directory from which to load raster and vector data
+                :type queryDir:         str
+                :param pairsHost:       PAIRS host to be used for PAIRS API calls
+                :type pairsHost:        str
+                :param queryID:         PAIRS query ID associated with the data folder queryDir
+                :type queryID:          str
+                :param baseURI:         base URI to use for PAIRS API calls
+                :type baseURI:          str
+                :returns:               PAIRS API wrapper query object
+                :rtype:                 api_wrapper.PAIRSQuery
+                """
+                if baseURI is None: baseURI = PAIRS_DEFAULT_BASE_URI
+                clsInstance = cls(
+                        query               = None,
+                        pairsHost           = pairsHost,
+                        baseURI             = baseURI,
+                        auth                = None,
+                        downloadDir         = None,
+                        overwriteExisting   = False,
+                )
+                # indicate that the data does not need to be downloaded
+                clsInstance.downloaded  = True
+                # set PAIRS query base directory
+                # note: incorporates a hack due to a bug in the fs Python module (on parsing)
+                clsInstance.queryFS     = OSFS(queryDir)
+                # load all raster and vector data
+                logger.info('Loading query result into memory ...')
+                # load all queried layers
+                clsInstance.create_layers()
+                logger.info('... done.')
+
+                return clsInstance
+
+        def get_query_dir_name(self):
+                """
+                Compute query directory name by setting self.queryDir.
+
+                :raises Exception:  if required information is missing
+                                                        if the query hash cannot be constructed
+                """
+                # recompute query hash
                 try:
-                    if isinstance(self.query, dict):
+                        self.qHash = getQueryHash(self.query if isinstance(self.query, dict) else {})
+                except:
+                        errMsg = u'Unable to determine query hash.'
+                        logger.error(errMsg)
+                        raise Exception(errMsg)
+
+                # construct query directory name
+                # note: download directory abstracted away by self.fs
+                if self.queryID is not None:
                         self.queryDir = str(
-                            os.path.splitext(
-                                os.path.abspath(
-                                    sorted(
-                                        [
-                                            g.path
-                                            for g in self.fs.glob(
-                                                os.path.join(
-                                                    '*_{}{}'.format(
-                                                        self.qHash,
-                                                        PAIRS_ZIP_FILE_EXTENSION
-                                                    )
-                                                )
-                                            )
-                                        ],
-                                    )[-1]
-                                )
-                            )[0]
-                        )
-                        self.queryID = str(
-                            os.path.basename(
-                                self.queryDir
-                            ).rsplit(PAW_QUERY_NAME_SEPARATOR, 1)[0]
+                                        self.queryID + '_' + self.qHash
                         )
-                        self.downloaded = True
-                        logger.info("Alright, using cache of PAIRS query with ID: '{}'".format(self.queryID))
-                except Exception as e:
-                    msg = "I am sorry, you asked for using the local cache, but your query does not match any existing. I am gonna query PAIRS instead: '{}'.".format(e)
-                    logger.warning(msg)
-                    self.overwriteExisting = True
-                    self.queryID = False
-                finally:
-                    self._closeDataSource()
-            # query PAIRS (if any)
-            if self.overwriteExisting:
-                # try to submit query to PAIRS
+                elif self.zipFilePath is not None:
+                        self.queryDir = str(os.path.dirname(self.zipFilePath))
+                else:
+                        msg = u'Information to construct query directory incomplete.'
+                        logger.warning(msg)
+                        raise Exception(msg)
+
+        def read_data_acknowledgement(self):
+                """
+                Extracts data acknowledge statement from PAIRS query result ZIP file.
+
+                :raises Exception:      if no acknowledgement is found
+                """
+                # attempt to extract only if not set already
+                self._openDataSource()
                 try:
-                    if (self.querySubmit is None) or (self.querySubmit.status_code not in (200, 201)):
-                        # compose query header
-                        headers = {'Content-Type': 'application/json'}
-                        if self._isOnlineQuery:
-                            headers['Accept']   = self.PAIRS_POINT_QUERY_RESP_FORMAT
-                        # submit query
-                        if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-                            token = 'Bearer ' + self.auth.jwt_token
-                            headers['Authorization'] = token
-                            self.querySubmit = requests.post(
-                                urljoin(
-                                    self.pairsHost.geturl(),
-                                    self.SUBMIT_API_STRING
-                                ),
-                                data    = json.dumps(self.query),
-                                headers = headers,
-                                verify  = self.verifySSL,
-                            )
+                        if self.dataAcknowledgeText is None and self.queryFS is not None:
+                                # check that there exists a file with the acknowledgement
+                                if self.fs.exists(self.zipFilePath) and \
+                                     PAIRS_DATA_ACK_FILE_NAME in self.queryFS.listdir(u''):
+                                        # extract data acknowledgement from PAIRS query ZIP file
+                                        try:
+                                                with self.queryFS.open(PAIRS_DATA_ACK_FILE_NAME, 'rb') as f:
+                                                        self.dataAcknowledgeText = ''.join(codecs.getreader('utf-8')(f))
+                                                logger.info('Data acknowledgement successfully loaded, print with `self.print_data_acknowledgement()`')
+                                        except Exception as e:
+                                                msg = u'Unable to read data acknowledgement from PAIRS query result ZIP file: {}'.format(e)
+                                                logger.error(msg)
+                                                raise Exception(msg)
+                                else:
+                                        msg = u'No PAIRS query ZIP file identified, or no acknowledgement in ZIP file found. Did you run `self.download()`, yet?'
+                                        logger.warning(msg)
+                                        raise Exception(msg)
                         else:
-                            self.querySubmit = requests.post(
-                                urljoin(
-                                    self.pairsHost.geturl(),
-                                    self.SUBMIT_API_STRING
-                                ),
-                                data    = json.dumps(self.query),
-                                headers = headers,
-                                auth    = self.auth,
-                                verify  = self.verifySSL,
-                            )
-                except Exception as e:
-                    raise Exception(
-                        'Sorry, I have trouble to submit your query: {}.'.format(e)
-                    )
-                # check that submission return is proper JSON
-                if not self._isOnlineQuery:
-                    try:
-                        _ = self.querySubmit.json()
-                    except Exception as e:
-                        logger.error(
-                            'Unable to extract query ID from submit JSON return - are you using the correct base URI ({})?'.format(self.baseURI)
-                        )
-                        logger.error(
-                            "Maybe your query definition is not right or PAIRS is temporarily unavailable? Here is the PAIRS server response:\n{}".format(self.querySubmit.text)
-                        )
+                                logger.info('Data acknowledgement loaded already - print with `self.print_data_acknowledgement()`')
+                except:
                         raise
+                finally:
+                        self._closeDataSource()
 
-                # obtain (and internally set) query ID, or ...
-                if not self._isOnlineQuery:
-                    try:
-                        self.queryID = self.querySubmit.json()['id']
-                    except Exception as e:
-                        logger.error(
-                            'Unable to extract query ID from submit JSON return, the JSON-load is: {}'.format(self.querySubmit.json())
-                        )
-                        raise
-                    logger.info("Query successfully submitted, reference ID: {}".format(self.queryID))
-                    # silently poll the PAIRS query status to populate self.queryStatus for user
-                    try:
-                        self.poll()
-                    except:
+        def print_data_acknowledgement(self):
+                """
+                Simply print out data acknowledgement statement.
+
+                """
+                try:
+                        self.read_data_acknowledgement()
+                except:
                         pass
-                # ... handle online (point) query that immediately returns
-                else:
-                    # set query status equal to submit status
-                    self.queryStatus = self.querySubmit
-                    # convert data into (vector) dataframe
-                    # catch empty return
-                    if self.queryStatus.text is None:
-                        logger.warning('No point data available to load/returned.')
-                    else:
-                        try:
-                            if self.queryStatus.status_code != 200:
-                                raise Exception(
-                                        "Querying PAIRS resulted in HTTP error code '{}': {}.".format(
-                                        self.queryStatus.status_code,
-                                        self.queryStatus.text,
-                                    )
-                                )
-                            else:
-                                if self.PAIRS_POINT_QUERY_RESP_FORMAT.lower()=='text/csv':
-                                    self.vdf = pandas.read_csv(
-                                        io.StringIO(self.queryStatus.text),
-                                        header      = 0,
-                                        index_col   = False,
-                                        quotechar   = PAIRS_VECTOR_CSV_QUOTE_CHAR,
-                                    )
-                                else:
-                                    self.vdf = pandas.DataFrame(
-                                        self.queryStatus.json()['data']
-                                    )
-                            logger.info('Point data successfully imported into self.vdf')
-                            # check for (default) timestamp column
-                            if PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME in self.vdf.columns:
-                                self.set_timestamp_column(PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME)
-                                logger.info("Timestamp column '{}' detected.".format(PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME))
-                            else:
-                                logger.warning("No timestamp column '{}' detected.".format(PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME))
-                            # check for (default) geo-coordinate columns
-                            if PAIRS_VECTOR_LONGITUDE_COLUMN_NAME in self.vdf.columns \
-                            and PAIRS_VECTOR_LATITUDE_COLUMN_NAME in self.vdf.columns:
-                                self.set_lat_lon_columns(
-                                    PAIRS_VECTOR_LATITUDE_COLUMN_NAME,
-                                    PAIRS_VECTOR_LONGITUDE_COLUMN_NAME,
-                                    PAIRS_VECTOR_GEOMETRY_COLUMN_NAME,
-                                )
-                                logger.info(
-                                    "Geo-coordinate columns '{}' and '{}' detected.".format(
-                                        PAIRS_VECTOR_LONGITUDE_COLUMN_NAME,
-                                        PAIRS_VECTOR_LATITUDE_COLUMN_NAME,
-                                    )
-                                )
-                            else:
-                                logger.warning(
-                                    "No geo-coordinate columns '{}' detected.".format(
-                                        [PAIRS_VECTOR_LONGITUDE_COLUMN_NAME, PAIRS_VECTOR_LATITUDE_COLUMN_NAME]
-                                    )
-                                )
-                        except Exception as e:
-                            logger.error(
-                                "Unable to load point data into dataframe employing format '{}': '{}'.".format(
-                                    self.PAIRS_POINT_QUERY_RESP_FORMAT, e,
-                                )
-                            )
-                            raise
-        # case of PAIRS cached query (previously run)
-        elif isinstance(self.querySubmit, MockSubmitResponse):
-            logger.info(
-                "Alright, using remotely cached PAIRS query with ID '{}'.".format(self.queryID)
-            )
-        # case of locally cached PAIRS query ZIP directory
-        elif locallyCachedZIP:
-            logger.info(
-                "Alright, using locally cached PAIRS query ZIP file '{}'.".format(self.zipFilePath)
-            )
-            self.downloaded = True
-        else:
-            raise Exception(
-                'Sorry, no query defined. You are probably using PAIRS Jupyter notebook?'
-            )
+                print("The data acknowledgement for self.data is:\n{}".format(self.dataAcknowledgeText))
 
-    def poll(self, passNonSubmitted=False):
-        """
-        Polls the status a single time and updating self.queryStatus.
 
-        :param passNonSubmitted:    allow the method to pass although no query has been submitted
-                                    (this is used for locally cached data)
-        :type passNonSubmitted:     bool
-        :raises Exception:  if query submit response is unsuccessful,
-                            if no query or query ID is defined,
-                            if the provided credentials are incorrect
-        """
-        # skip online (point) query
-        if isinstance(self.querySubmit, MockSubmitResponse) or self.query is None \
-        or not self._isOnlineQuery:
-            # in case the query is a local pointer to a directory, pass polling
-            if isinstance(self.query, string_type):
-                passNonSubmitted = True
-            if passNonSubmitted:
-                # Flag to allow poll() method to pass even though the query has not been submitted yet.
-                pass
-            elif (self.querySubmit is None) and self.queryID is not None and self.downloaded:
-                # poll PAIRS API even though we don't have a querySubmit status code.
-                # (Used to re-load old GeoTiffs).
-                pollURL = urljoin(
-                    urljoin(
-                        self.pairsHost.geturl(),
-                        self.STATUS_API_STRING
-                    ),
-                    self.queryID
-                )
+        def submit(self):
+                """
+                Submit query to PAIRS (if defined).
 
-                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-                    headers = {}
-                    token = 'Bearer ' + self.auth.jwt_token
-                    headers['Authorization'] = token
-                    self.queryStatus = requests.get(
-                        pollURL,
-                        verify  = self.verifySSL,
-                        headers = headers,
-                    )
-                else:
-                    self.queryStatus = requests.get(
-                        pollURL,
-                        auth    = self.auth,
-                        verify  = self.verifySSL,
-                    )
-            elif self.queryID is not None and \
-                (not self.querySubmit is None) and \
-                (self.querySubmit.status_code == 200) and \
-                ('data' not in self.querySubmit.json()):
-                # poll PAIRS API
-                pollURL = urljoin(
-                    urljoin(
-                        self.pairsHost.geturl(),
-                        self.STATUS_API_STRING
-                    ),
-                    self.queryID
-                )
+                :raises Exception:  if no query is defined
+                                                        if no local cache is available which is requested to use
+                                                        if no PAIRS query ID can be identified from the return of the PAIRS server
+                """
 
-                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-                    headers = {}
-                    token = 'Bearer ' + self.auth.jwt_token
-                    headers['Authorization'] = token
-                    self.queryStatus = requests.get(
-                        pollURL,
-                        verify  = self.verifySSL,
-                        headers = headers,
-                    )
-                else:
-                    self.queryStatus = requests.get(
-                        pollURL,
-                        auth    = self.auth,
-                        verify  = self.verifySSL,
-                    )
-            elif self.queryID is None and self.query is None:
-                raise Exception(
-                    'No query or query ID defined on record, so no submit possible, i.e. polling does not make sense. You are probably using PAIRS Jupyter notebook?'
-                )
-            else:
-                raise Exception('Query submit response: ' + str(self.querySubmit.status_code))
-
-            # raise an exception if credentials are wrong
-            if not passNonSubmitted and self.queryStatus is not None and self.queryStatus.status_code == 401:
-                raise Exception('ATTENTION: Provided credentials are incorrect!')
-
-    def poll_till_finished(
-        self,
-        pollIntSec  = None,
-        printStatus = False,
-        timeout     = -1,
-    ):
-        """
-        Polls the status until not running anymore. If successful the result is
-        published in the PAIRS GUI (given the user specified this on query generation).
+                # get information for if-statement to follow from data source (if any)
+                locallyCachedZIP = False
+                try:
+                        self._openDataSource()
+                        locallyCachedZIP = self.fs.exists(self.zipFilePath)
+                except:
+                        pass
+                finally:
+                        self._closeDataSource()
+                if self.query is not None:
+                        # fake submit for using existing cache
+                        if not self.overwriteExisting:
+                                logger.warning("Fake submit to PAIRS in order to use (latest) locally cached data.")
+                                # check whether locally cache exists at all
+                                self._openDataSource()
+                                try:
+                                        if isinstance(self.query, dict):
+                                                self.queryDir = str(
+                                                        os.path.splitext(
+                                                                os.path.abspath(
+                                                                        sorted(
+                                                                                [
+                                                                                        g.path
+                                                                                        for g in self.fs.glob(
+                                                                                                os.path.join(
+                                                                                                        '*_{}{}'.format(
+                                                                                                                self.qHash,
+                                                                                                                PAIRS_ZIP_FILE_EXTENSION
+                                                                                                        )
+                                                                                                )
+                                                                                        )
+                                                                                ],
+                                                                        )[-1]
+                                                                )
+                                                        )[0]
+                                                )
+                                                self.queryID = str(
+                                                        os.path.basename(
+                                                                self.queryDir
+                                                        ).rsplit(PAW_QUERY_NAME_SEPARATOR, 1)[0]
+                                                )
+                                                self.downloaded = True
+                                                logger.info("Alright, using cache of PAIRS query with ID: '{}'".format(self.queryID))
+                                except Exception as e:
+                                        msg = "I am sorry, you asked for using the local cache, but your query does not match any existing. I am gonna query PAIRS instead: '{}'.".format(e)
+                                        logger.warning(msg)
+                                        self.overwriteExisting = True
+                                        self.queryID = False
+                                finally:
+                                        self._closeDataSource()
+                        # query PAIRS (if any)
+                        if self.overwriteExisting:
+                                # try to submit query to PAIRS
+                                try:
+                                        if (self.querySubmit is None) or (self.querySubmit.status_code not in (200, 201)):
+                                                # compose query header
+                                                headers = {'Content-Type': 'application/json'}
+                                                if self._isOnlineQuery:
+                                                        headers['Accept']   = self.PAIRS_POINT_QUERY_RESP_FORMAT
+                                                # submit query
+                                                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                                                        token = 'Bearer ' + self.auth.jwt_token
+                                                        headers['Authorization'] = token
+                                                        self.querySubmit = requests.post(
+                                                                urljoin(
+                                                                        self.pairsHost.geturl(),
+                                                                        self.SUBMIT_API_STRING
+                                                                ),
+                                                                data    = json.dumps(self.query),
+                                                                headers = headers,
+                                                                verify  = self.verifySSL,
+                                                        )
+                                                else:
+                                                        self.querySubmit = requests.post(
+                                                                urljoin(
+                                                                        self.pairsHost.geturl(),
+                                                                        self.SUBMIT_API_STRING
+                                                                ),
+                                                                data    = json.dumps(self.query),
+                                                                headers = headers,
+                                                                auth    = self.auth,
+                                                                verify  = self.verifySSL,
+                                                        )
+                                except Exception as e:
+                                        raise Exception(
+                                                'Sorry, I have trouble to submit your query: {}.'.format(e)
+                                        )
+                                # check that submission return is proper JSON
+                                if not self._isOnlineQuery:
+                                        try:
+                                                _ = self.querySubmit.json()
+                                        except Exception as e:
+                                                logger.error(
+                                                        'Unable to extract query ID from submit JSON return - are you using the correct base URI ({})?'.format(self.baseURI)
+                                                )
+                                                logger.error(
+                                                        "Maybe your query definition is not right or PAIRS is temporarily unavailable? Here is the PAIRS server response:\n{}".format(self.querySubmit.text)
+                                                )
+                                                raise
 
-        :param pollIntSec:      seconds to idle between polls
-        :type pollIntSec:       float
-        :param printStatus:     triggers printing the poll status information
-        :type printStatus:      bool
-        :param timeout:         maximum (positive) time in seconds allowed to poll
-                                till finished, the default is infinitely polling
-        :type timeout:          int
-        :raises Exception:      if query submit response is unsuccessful or not existing,
-                                if no query or query ID is defined
-                                if a user set timeout has been reached
-        """
-        # skip online (point) query case
-        if isinstance(self.querySubmit, MockSubmitResponse) or self.query is None \
-        or not self._isOnlineQuery:
-            # poll in case no locally cached data is used, only
-            if not self.overwriteExisting:
-                self.poll(passNonSubmitted = True)
-            # report case where there is not enough information available to query PAIRS
-            elif self.queryID is None and self.query is None:
-                raise Exception(
-                    'No query or query ID defined on record, so no submit possible, i.e. polling does not make sense. You are probably using PAIRS Jupyter notebook?'
-                )
-            elif self.querySubmit.status_code is None:
-                raise Exception(
-                    'Sorry, no query submitted so far. Try: `PAIRSQuery.submit()`.'
-                )
-            elif self.querySubmit.status_code == 200:
-                # record start time of polling
-                startTime = time.time()
-                # wait for query to finish by constantly polling the API
-                while True:
-                    # check (user defined) timeout
-                    if timeout > 0:
-                        if time.time()-startTime > timeout:
-                            raise Exception("User defined poll timeout reached.")
-                    # poll PAIRS API (if not to use locally cached data)
-                    self.poll()
-                    # print polled status
-                    if printStatus:
-                        try:
-                            status = self.queryStatus.json()['status']
-                            progressPercent = float(self.queryStatus.json()['exPercent'])
-                            if progressPercent > 0:
-                                percMsg = ' ({}%)'.format(progressPercent)
-                            else:
-                                percMsg = u''
-                            logger.info("Query status is '{}'{}.".format(status, percMsg))
-                        except:
-                            pass
-                    # break if query not running any more
-                    try:
-                        statusCode = self.queryStatus.json()['statusCode']
-                    except Exception as e:
-                        logger.error(
-                            'Unable to extract query status code from poll JSON return - are you using the correct base URI ({})?'.format(self.baseURI)
-                        )
-                        raise
-                    if statusCode is not None and PAIRS_QUERY_RUN_STAT_REG_EX.match(str(statusCode)) is None:
-                        break
-                    # idle before polling again
-                    time.sleep(
-                        pollIntSec if pollIntSec is not None \
-                        else PAIRSQuery.STATUS_POLL_INTERVAL_SEC
-                    )
-                # publish PAIRS query result to PAIRS GUI (if any)
-                if self.publish2GUI and hasattr(self, 'guiToken'):
-                    resp = requests.post(
-                        urljoin(
-                            self.guiURL,
-                            self.PUBLISH_QUERY_RESULT_2_GUI.format(queryID=self.queryID),
-                        ),
-                        headers = {'Authorization': 'Bearer ' + self.guiToken},
-                        verify  = self.verifySSL,
-                    )
-                    if resp.status_code!=200:
-                        logger.warning(
-                            "Unfortunate, I could not publish your query result to the PAIRS GUI using '{}' got return code '{}': {}".format(
-                                self.guiURL, resp.status_code, resp.text,
-                            )
+                                # obtain (and internally set) query ID, or ...
+                                if not self._isOnlineQuery:
+                                        try:
+                                                self.queryID = self.querySubmit.json()['id']
+                                        except Exception as e:
+                                                logger.error(
+                                                        'Unable to extract query ID from submit JSON return, the JSON-load is: {}'.format(self.querySubmit.json())
+                                                )
+                                                raise
+                                        logger.info("Query successfully submitted, reference ID: {}".format(self.queryID))
+                                        # silently poll the PAIRS query status to populate self.queryStatus for user
+                                        try:
+                                                self.poll()
+                                        except:
+                                                pass
+                                # ... handle online (point) query that immediately returns
+                                else:
+                                        # set query status equal to submit status
+                                        self.queryStatus = self.querySubmit
+                                        # convert data into (vector) dataframe
+                                        # catch empty return
+                                        if self.queryStatus.text is None:
+                                                logger.warning('No point data available to load/returned.')
+                                        else:
+                                                try:
+                                                        if self.queryStatus.status_code != 200:
+                                                                raise Exception(
+                                                                                "Querying PAIRS resulted in HTTP error code '{}': {}.".format(
+                                                                                self.queryStatus.status_code,
+                                                                                self.queryStatus.text,
+                                                                        )
+                                                                )
+                                                        else:
+                                                                if self.PAIRS_POINT_QUERY_RESP_FORMAT.lower()=='text/csv':
+                                                                        self.vdf = pandas.read_csv(
+                                                                                io.StringIO(self.queryStatus.text),
+                                                                                header      = 0,
+                                                                                index_col   = False,
+                                                                                quotechar   = PAIRS_VECTOR_CSV_QUOTE_CHAR,
+                                                                        )
+                                                                else:
+                                                                        self.vdf = pandas.DataFrame(
+                                                                                self.queryStatus.json()['data']
+                                                                        )
+                                                        logger.info('Point data successfully imported into self.vdf')
+                                                        # check for (default) timestamp column
+                                                        if PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME in self.vdf.columns:
+                                                                self.set_timestamp_column(PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME)
+                                                                logger.info("Timestamp column '{}' detected.".format(PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME))
+                                                        else:
+                                                                logger.warning("No timestamp column '{}' detected.".format(PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME))
+                                                        # check for (default) geo-coordinate columns
+                                                        if PAIRS_VECTOR_LONGITUDE_COLUMN_NAME in self.vdf.columns \
+                                                        and PAIRS_VECTOR_LATITUDE_COLUMN_NAME in self.vdf.columns:
+                                                                self.set_lat_lon_columns(
+                                                                        PAIRS_VECTOR_LATITUDE_COLUMN_NAME,
+                                                                        PAIRS_VECTOR_LONGITUDE_COLUMN_NAME,
+                                                                        PAIRS_VECTOR_GEOMETRY_COLUMN_NAME,
+                                                                )
+                                                                logger.info(
+                                                                        "Geo-coordinate columns '{}' and '{}' detected.".format(
+                                                                                PAIRS_VECTOR_LONGITUDE_COLUMN_NAME,
+                                                                                PAIRS_VECTOR_LATITUDE_COLUMN_NAME,
+                                                                        )
+                                                                )
+                                                        else:
+                                                                logger.warning(
+                                                                        "No geo-coordinate columns '{}' detected.".format(
+                                                                                [PAIRS_VECTOR_LONGITUDE_COLUMN_NAME, PAIRS_VECTOR_LATITUDE_COLUMN_NAME]
+                                                                        )
+                                                                )
+                                                except Exception as e:
+                                                        logger.error(
+                                                                "Unable to load point data into dataframe employing format '{}': '{}'.".format(
+                                                                        self.PAIRS_POINT_QUERY_RESP_FORMAT, e,
+                                                                )
+                                                        )
+                                                        raise
+                # case of PAIRS cached query (previously run)
+                elif isinstance(self.querySubmit, MockSubmitResponse):
+                        logger.info(
+                                "Alright, using remotely cached PAIRS query with ID '{}'.".format(self.queryID)
                         )
-                    else:
+                # case of locally cached PAIRS query ZIP directory
+                elif locallyCachedZIP:
                         logger.info(
-                            "Query with ID '{}' successfully published to PAIRS GUI using '{}'.".format(
-                                self.queryID, self.guiURL,
-                            )
+                                "Alright, using locally cached PAIRS query ZIP file '{}'.".format(self.zipFilePath)
                         )
+                        self.downloaded = True
                 else:
-                    logger.debug(
-                        "Query won't be published to PAIRS GUI, because either it is not requested by user or there is no GUI API token available (cf. `self.guiToken` and `self.publish2GUI`)."
-                    )
-            else:
-                raise Exception('Query submit response: ' + str(self.querySubmit.status_code))
-
-    def download(
-        self,
-        cosInfoJSON     = None,
-        cosPollIntSec   = None,
-        cosTimeout      = -1,
-        printStatus     = False,
-    ):
-        """
-        Get the data previously queried and save the ZIP file.
-
-        :param cosInfoJSON:     IBM PAIRS with Cloud Object Storage bucket information like
-                                ```JSON
-                                {
-                                    "provider": "ibm",
-                                    "endpoint": "https://s3.us.cloud-object-storage.appdomain.cloud",
-                                    "bucket": "<your bucket name>",
-                                    "token": "<your secret token for bucket>"
-                                }
-                                ```
-                                if set, the query result is published in the cloud
-                                and not stored locally on your machine. It is a
-                                useful feature in combination with IBM Watson Studio notebooks
-        :type cosInfoJSON:      dict
-        :param cosPollIntSec:   seconds to idle between polls to IBM COS
-        :type cosPollIntSec:    float
-        :param printStatus:     triggers printing the poll status information
-        :type printStatus:      bool
-        :param cosTimeout:      maximum (positive) time in seconds allowed to poll
-                                till finished, the default is infinitely polling
-        :type cosTimeout:       int
-        """
-        # flag IBM COS usage
-        if cosInfoJSON is not None:
-            self.inIBMCOS = True
-        # skip online (point) query case (including reload query and cached query)
-        if isinstance(self.querySubmit, MockSubmitResponse) or self.query is None \
-        or not self._isOnlineQuery:
-            # one more time poll/try to get query status
-            if self.queryStatus is None and self.overwriteExisting:
-                self.poll()
-
-            # construct path
-            self.get_query_dir_name()
-
-            # check successful query
-            if not self.overwriteExisting:
-                # note: if the ZIP file path is set already, we deal with the case where
-                # there is a user specified PAIRS query directory, already
-                if self.zipFilePath is None:
-                    self.zipFilePath = str(self.queryDir + PAIRS_ZIP_FILE_EXTENSION)
+                        raise Exception(
+                                'Sorry, no query defined. You are probably using PAIRS Jupyter notebook?'
+                        )
 
-                # check if locally set path for downloaded PAIRS query ZIP file exists
-                # to confirm the download
-                self._openDataSource()
-                try:
-                    self.downloaded = self.fs.exists(self.zipFilePath)
-                except:
-                    raise
-                finally:
-                    self._closeDataSource()
-            else:
-                try:
-                    respJson    = self.queryStatus.json()
-                    statusCode  = respJson['statusCode']
-                    statusMsg   = str(respJson['status'])
-                except Exception as e:
-                    logger.error(
-                        'Unable to extract query status code from poll JSON return - are you using the correct base URI ({})?'.format(self.baseURI)
-                    )
-                    raise
-
-                # check that the data is ready for download
-                if int(statusCode) == PAIRS_QUERY_DOWNLOADABLE_STAT:
-                    # TODO: IS THIS STILL A VALID ASSUMPTION?
-                    # Save the query ID prominently. This ID also flags that the file
-                    # has been downloaded already
-                    if not self.downloaded:
-                        self.downloaded = True
-                        try:
-                            self.queryID = self.querySubmit.json()['id']
-                        except Exception as e:
-                            logger.error(
-                                'Unable to extract query ID from submit JSON return - are you using the correct base URI ({})?'.format(self.baseURI)
-                            )
-                            raise
-                    # note on streaming into memory
-                    # TODO: move COS upload to separate function
-                    if self.inIBMCOS:
-                        # publish query result to COS
-                        if isinstance(cosInfoJSON, dict) and \
-                           set(self.COS_INFO_KEYS) <= set(cosInfoJSON):
-                            try:
-                                # initialize upload to COS
-                                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-                                    headers = {'Content-Type': 'application/json'}
-                                    token = 'Bearer ' + self.auth.jwt_token
-                                    headers['Authorization'] = token
-                                    resp = requests.post(
+        def poll(self, passNonSubmitted=False):
+                """
+                Polls the status a single time and updating self.queryStatus.
+
+                :param passNonSubmitted:    allow the method to pass although no query has been submitted
+                                                                        (this is used for locally cached data)
+                :type passNonSubmitted:     bool
+                :raises Exception:  if query submit response is unsuccessful,
+                                                        if no query or query ID is defined,
+                                                        if the provided credentials are incorrect
+                """
+                # skip online (point) query
+                if isinstance(self.querySubmit, MockSubmitResponse) or self.query is None \
+                or not self._isOnlineQuery:
+                        # in case the query is a local pointer to a directory, pass polling
+                        if isinstance(self.query, string_type):
+                                passNonSubmitted = True
+                        if passNonSubmitted:
+                                # Flag to allow poll() method to pass even though the query has not been submitted yet.
+                                pass
+                        elif (self.querySubmit is None) and self.queryID is not None and self.downloaded:
+                                # poll PAIRS API even though we don't have a querySubmit status code.
+                                # (Used to re-load old GeoTiffs).
+                                pollURL = urljoin(
                                         urljoin(
-                                            urljoin(
                                                 self.pairsHost.geturl(),
-                                                self.COS_UPLOAD_API_STRING
-                                            ),
-                                            str(self.queryID)
+                                                self.STATUS_API_STRING
                                         ),
-                                        json=cosInfoJSON,
-                                        headers = headers,
-                                        verify  = self.verifySSL,
-                                    )
+                                        self.queryID
+                                )
+
+                                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                                        headers = {}
+                                        token = 'Bearer ' + self.auth.jwt_token
+                                        headers['Authorization'] = token
+                                        self.queryStatus = requests.get(
+                                                pollURL,
+                                                verify  = self.verifySSL,
+                                                headers = headers,
+                                        )
                                 else:
-                                    resp = requests.post(
+                                        self.queryStatus = requests.get(
+                                                pollURL,
+                                                auth    = self.auth,
+                                                verify  = self.verifySSL,
+                                        )
+                        elif self.queryID is not None and \
+                                (not self.querySubmit is None) and \
+                                (self.querySubmit.status_code == 200) and \
+                                ('data' not in self.querySubmit.json()):
+                                # poll PAIRS API
+                                pollURL = urljoin(
                                         urljoin(
-                                            urljoin(
                                                 self.pairsHost.geturl(),
-                                                self.COS_UPLOAD_API_STRING
-                                            ),
-                                            str(self.queryID)
+                                                self.STATUS_API_STRING
                                         ),
-                                        json=cosInfoJSON,
-                                        headers = {'Content-Type': 'application/json'},
-                                        auth    = self.auth,
-                                        verify  = self.verifySSL,
-                                    )
-                                if resp.status_code == 200:
-                                    logger.info('Upload of query result to IBM COS initialized.')
+                                        self.queryID
+                                )
+
+                                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                                        headers = {}
+                                        token = 'Bearer ' + self.auth.jwt_token
+                                        headers['Authorization'] = token
+                                        self.queryStatus = requests.get(
+                                                pollURL,
+                                                verify  = self.verifySSL,
+                                                headers = headers,
+                                        )
                                 else:
-                                    raise Exception(
-                                        'PAIRS failed publishing query result to COS: {}'.format(resp.text)
-                                    )
-                                # track progress of upload to COS
+                                        self.queryStatus = requests.get(
+                                                pollURL,
+                                                auth    = self.auth,
+                                                verify  = self.verifySSL,
+                                        )
+                        elif self.queryID is None and self.query is None:
+                                raise Exception(
+                                        'No query or query ID defined on record, so no submit possible, i.e. polling does not make sense. You are probably using PAIRS Jupyter notebook?'
+                                )
+                        else:
+                                raise Exception('Query submit response: ' + str(self.querySubmit.status_code))
+
+                        # raise an exception if credentials are wrong
+                        if not passNonSubmitted and self.queryStatus is not None and self.queryStatus.status_code == 401:
+                                raise Exception('ATTENTION: Provided credentials are incorrect!')
+
+        def poll_till_finished(
+                self,
+                pollIntSec  = None,
+                printStatus = False,
+                timeout     = -1,
+        ):
+                """
+                Polls the status until not running anymore. If successful the result is
+                published in the PAIRS GUI (given the user specified this on query generation).
+
+                :param pollIntSec:      seconds to idle between polls
+                :type pollIntSec:       float
+                :param printStatus:     triggers printing the poll status information
+                :type printStatus:      bool
+                :param timeout:         maximum (positive) time in seconds allowed to poll
+                                                                till finished, the default is infinitely polling
+                :type timeout:          int
+                :raises Exception:      if query submit response is unsuccessful or not existing,
+                                                                if no query or query ID is defined
+                                                                if a user set timeout has been reached
+                """
+                # skip online (point) query case
+                if isinstance(self.querySubmit, MockSubmitResponse) or self.query is None \
+                or not self._isOnlineQuery:
+                        # poll in case no locally cached data is used, only
+                        if not self.overwriteExisting:
+                                self.poll(passNonSubmitted = True)
+                        # report case where there is not enough information available to query PAIRS
+                        elif self.queryID is None and self.query is None:
+                                raise Exception(
+                                        'No query or query ID defined on record, so no submit possible, i.e. polling does not make sense. You are probably using PAIRS Jupyter notebook?'
+                                )
+                        elif self.querySubmit.status_code is None:
+                                raise Exception(
+                                        'Sorry, no query submitted so far. Try: `PAIRSQuery.submit()`.'
+                                )
+                        elif self.querySubmit.status_code == 200:
                                 # record start time of polling
                                 startTime = time.time()
                                 # wait for query to finish by constantly polling the API
-                                while resp.status_code==200:
-                                    # check (user defined) timeout
-                                    if cosTimeout > 0:
-                                        if time.time()-startTime > cosTimeout:
-                                            raise Exception(
-                                                "User defined poll timeout for IBM COS reached."
-                                            )
-                                    # poll PAIRS API for status of upload to COS
-                                    if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-                                        headers = {'Content-Type': 'application/json'}
-                                        token = 'Bearer ' + self.auth.jwt_token
-                                        headers['Authorization'] = token
-                                        resp = requests.get(
-                                            urljoin(
-                                                urljoin(
-                                                    self.pairsHost.geturl(),
-                                                    self.COS_UPLOAD_API_STRING
-                                                ),
-                                                str(self.queryID)
-                                            ),
-                                            headers = headers,
-                                            verify  = self.verifySSL,
+                                while True:
+                                        # check (user defined) timeout
+                                        if timeout > 0:
+                                                if time.time()-startTime > timeout:
+                                                        raise Exception("User defined poll timeout reached.")
+                                        # poll PAIRS API (if not to use locally cached data)
+                                        self.poll()
+                                        # print polled status
+                                        if printStatus:
+                                                try:
+                                                        status = self.queryStatus.json()['status']
+                                                        progressPercent = float(self.queryStatus.json()['exPercent'])
+                                                        if progressPercent > 0:
+                                                                percMsg = ' ({}%)'.format(progressPercent)
+                                                        else:
+                                                                percMsg = u''
+                                                        logger.info("Query status is '{}'{}.".format(status, percMsg))
+                                                except:
+                                                        pass
+                                        # break if query not running any more
+                                        try:
+                                                statusCode = self.queryStatus.json()['statusCode']
+                                        except Exception as e:
+                                                logger.error(
+                                                        'Unable to extract query status code from poll JSON return - are you using the correct base URI ({})?'.format(self.baseURI)
+                                                )
+                                                raise
+                                        if statusCode is not None and PAIRS_QUERY_RUN_STAT_REG_EX.match(str(statusCode)) is None:
+                                                break
+                                        # idle before polling again
+                                        time.sleep(
+                                                pollIntSec if pollIntSec is not None \
+                                                else PAIRSQuery.STATUS_POLL_INTERVAL_SEC
                                         )
-                                    else:
-                                        resp = requests.get(
-                                            urljoin(
+                                # publish PAIRS query result to PAIRS GUI (if any)
+                                if self.publish2GUI and hasattr(self, 'guiToken'):
+                                        resp = requests.post(
                                                 urljoin(
-                                                    self.pairsHost.geturl(),
-                                                    self.COS_UPLOAD_API_STRING
+                                                        self.guiURL,
+                                                        self.PUBLISH_QUERY_RESULT_2_GUI.format(queryID=self.queryID),
                                                 ),
-                                                str(self.queryID)
-                                            ),
-                                            headers = {'Content-Type': 'application/json'},
-                                            auth    = self.auth,
-                                            verify  = self.verifySSL,
+                                                headers = {'Authorization': 'Bearer ' + self.guiToken},
+                                                verify  = self.verifySSL,
                                         )
-                                    load = resp.json()
-                                    if resp.status_code == 200:
-                                        if printStatus:
-                                            logger.warning(
-                                                "Upload PAIRS query {} to IBM COS at {:0.1f}%.".format(
-                                                    self.queryID,
-                                                    100*float(load['sizeUploaded'])/float(load['sizeTotal'])
+                                        if resp.status_code!=200:
+                                                logger.warning(
+                                                        "Unfortunate, I could not publish your query result to the PAIRS GUI using '{}' got return code '{}': {}".format(
+                                                                self.guiURL, resp.status_code, resp.text,
+                                                        )
                                                 )
-                                            )
-                                    else:
-                                        raise Exception("Unsuccessful upload status request for COS.")
-                                    # check if upload is complete
-                                    if load['sizeUploaded']==load['sizeTotal'] \
-                                      or load['status'] not in ('initializing', 'uploading'):
-                                        break
-                                    # idle before polling again
-                                    time.sleep(
-                                        cosPollIntSec if cosPollIntSec is not None \
-                                        else PAIRSQuery.STATUS_POLL_INTERVAL_SEC
-                                    )
-                            except Exception as e:
-                                raise Exception(
-                                        'Sorry, I have trouble getting your query result to Cloud Object storage: {}.'.format(e)
-                                )
+                                        else:
+                                                logger.info(
+                                                        "Query with ID '{}' successfully published to PAIRS GUI using '{}'.".format(
+                                                                self.queryID, self.guiURL,
+                                                        )
+                                                )
+                                else:
+                                        logger.debug(
+                                                "Query won't be published to PAIRS GUI, because either it is not requested by user or there is no GUI API token available (cf. `self.guiToken` and `self.publish2GUI`)."
+                                        )
                         else:
-                            msg = u'Sorry, I do not know what to do based on the `cosInfoJSON` you provided.'
-                            logger.error(msg)
-                            raise Exception(msg)
-                    else:
-                        self._openDataSource()
+                                raise Exception('Query submit response: ' + str(self.querySubmit.status_code))
+
+        def download(
+                self,
+                cosInfoJSON     = None,
+                cosPollIntSec   = None,
+                cosTimeout      = -1,
+                printStatus     = False,
+        ):
+                """
+                Get the data previously queried and save the ZIP file.
+
+                :param cosInfoJSON:     IBM PAIRS with Cloud Object Storage bucket information like
+                                                                ```JSON
+                                                                {
+                                                                        "provider": "ibm",
+                                                                        "endpoint": "https://s3.us.cloud-object-storage.appdomain.cloud",
+                                                                        "bucket": "<your bucket name>",
+                                                                        "token": "<your secret token for bucket>"
+                                                                }
+                                                                ```
+                                                                if set, the query result is published in the cloud
+                                                                and not stored locally on your machine. It is a
+                                                                useful feature in combination with IBM Watson Studio notebooks
+                :type cosInfoJSON:      dict
+                :param cosPollIntSec:   seconds to idle between polls to IBM COS
+                :type cosPollIntSec:    float
+                :param printStatus:     triggers printing the poll status information
+                :type printStatus:      bool
+                :param cosTimeout:      maximum (positive) time in seconds allowed to poll
+                                                                till finished, the default is infinitely polling
+                :type cosTimeout:       int
+                """
+                # flag IBM COS usage
+                if cosInfoJSON is not None:
+                        self.inIBMCOS = True
+                # skip online (point) query case (including reload query and cached query)
+                if isinstance(self.querySubmit, MockSubmitResponse) or self.query is None \
+                or not self._isOnlineQuery:
+                        # one more time poll/try to get query status
+                        if self.queryStatus is None and self.overwriteExisting:
+                                self.poll()
+
+                        # construct path
+                        self.get_query_dir_name()
+
+                        # check successful query
+                        if not self.overwriteExisting:
+                                # note: if the ZIP file path is set already, we deal with the case where
+                                # there is a user specified PAIRS query directory, already
+                                if self.zipFilePath is None:
+                                        self.zipFilePath = str(self.queryDir + PAIRS_ZIP_FILE_EXTENSION)
+
+                                # check if locally set path for downloaded PAIRS query ZIP file exists
+                                # to confirm the download
+                                self._openDataSource()
+                                try:
+                                        self.downloaded = self.fs.exists(self.zipFilePath)
+                                except:
+                                        raise
+                                finally:
+                                        self._closeDataSource()
+                        else:
+                                try:
+                                        respJson    = self.queryStatus.json()
+                                        statusCode  = respJson['statusCode']
+                                        statusMsg   = str(respJson['status'])
+                                except Exception as e:
+                                        logger.error(
+                                                'Unable to extract query status code from poll JSON return - are you using the correct base URI ({})?'.format(self.baseURI)
+                                        )
+                                        raise
+
+                                # check that the data is ready for download
+                                if int(statusCode) == PAIRS_QUERY_DOWNLOADABLE_STAT:
+                                        # TODO: IS THIS STILL A VALID ASSUMPTION?
+                                        # Save the query ID prominently. This ID also flags that the file
+                                        # has been downloaded already
+                                        if not self.downloaded:
+                                                self.downloaded = True
+                                                try:
+                                                        self.queryID = self.querySubmit.json()['id']
+                                                except Exception as e:
+                                                        logger.error(
+                                                                'Unable to extract query ID from submit JSON return - are you using the correct base URI ({})?'.format(self.baseURI)
+                                                        )
+                                                        raise
+                                        # note on streaming into memory
+                                        # TODO: move COS upload to separate function
+                                        if self.inIBMCOS:
+                                                # publish query result to COS
+                                                if isinstance(cosInfoJSON, dict) and \
+                                                     set(self.COS_INFO_KEYS) <= set(cosInfoJSON):
+                                                        try:
+                                                                # initialize upload to COS
+                                                                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                                                                        headers = {'Content-Type': 'application/json'}
+                                                                        token = 'Bearer ' + self.auth.jwt_token
+                                                                        headers['Authorization'] = token
+                                                                        resp = requests.post(
+                                                                                urljoin(
+                                                                                        urljoin(
+                                                                                                self.pairsHost.geturl(),
+                                                                                                self.COS_UPLOAD_API_STRING
+                                                                                        ),
+                                                                                        str(self.queryID)
+                                                                                ),
+                                                                                json=cosInfoJSON,
+                                                                                headers = headers,
+                                                                                verify  = self.verifySSL,
+                                                                        )
+                                                                else:
+                                                                        resp = requests.post(
+                                                                                urljoin(
+                                                                                        urljoin(
+                                                                                                self.pairsHost.geturl(),
+                                                                                                self.COS_UPLOAD_API_STRING
+                                                                                        ),
+                                                                                        str(self.queryID)
+                                                                                ),
+                                                                                json=cosInfoJSON,
+                                                                                headers = {'Content-Type': 'application/json'},
+                                                                                auth    = self.auth,
+                                                                                verify  = self.verifySSL,
+                                                                        )
+                                                                if resp.status_code == 200:
+                                                                        logger.info('Upload of query result to IBM COS initialized.')
+                                                                else:
+                                                                        raise Exception(
+                                                                                'PAIRS failed publishing query result to COS: {}'.format(resp.text)
+                                                                        )
+                                                                # track progress of upload to COS
+                                                                # record start time of polling
+                                                                startTime = time.time()
+                                                                # wait for query to finish by constantly polling the API
+                                                                while resp.status_code==200:
+                                                                        # check (user defined) timeout
+                                                                        if cosTimeout > 0:
+                                                                                if time.time()-startTime > cosTimeout:
+                                                                                        raise Exception(
+                                                                                                "User defined poll timeout for IBM COS reached."
+                                                                                        )
+                                                                        # poll PAIRS API for status of upload to COS
+                                                                        if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                                                                                headers = {'Content-Type': 'application/json'}
+                                                                                token = 'Bearer ' + self.auth.jwt_token
+                                                                                headers['Authorization'] = token
+                                                                                resp = requests.get(
+                                                                                        urljoin(
+                                                                                                urljoin(
+                                                                                                        self.pairsHost.geturl(),
+                                                                                                        self.COS_UPLOAD_API_STRING
+                                                                                                ),
+                                                                                                str(self.queryID)
+                                                                                        ),
+                                                                                        headers = headers,
+                                                                                        verify  = self.verifySSL,
+                                                                                )
+                                                                        else:
+                                                                                resp = requests.get(
+                                                                                        urljoin(
+                                                                                                urljoin(
+                                                                                                        self.pairsHost.geturl(),
+                                                                                                        self.COS_UPLOAD_API_STRING
+                                                                                                ),
+                                                                                                str(self.queryID)
+                                                                                        ),
+                                                                                        headers = {'Content-Type': 'application/json'},
+                                                                                        auth    = self.auth,
+                                                                                        verify  = self.verifySSL,
+                                                                                )
+                                                                        load = resp.json()
+                                                                        if resp.status_code == 200:
+                                                                                if printStatus:
+                                                                                        logger.warning(
+                                                                                                "Upload PAIRS query {} to IBM COS at {:0.1f}%.".format(
+                                                                                                        self.queryID,
+                                                                                                        100*float(load['sizeUploaded'])/float(load['sizeTotal'])
+                                                                                                )
+                                                                                        )
+                                                                        else:
+                                                                                raise Exception("Unsuccessful upload status request for COS.")
+                                                                        # check if upload is complete
+                                                                        if load['sizeUploaded']==load['sizeTotal'] \
+                                                                            or load['status'] not in ('initializing', 'uploading'):
+                                                                                break
+                                                                        # idle before polling again
+                                                                        time.sleep(
+                                                                                cosPollIntSec if cosPollIntSec is not None \
+                                                                                else PAIRSQuery.STATUS_POLL_INTERVAL_SEC
+                                                                        )
+                                                        except Exception as e:
+                                                                raise Exception(
+                                                                                'Sorry, I have trouble getting your query result to Cloud Object storage: {}.'.format(e)
+                                                                )
+                                                else:
+                                                        msg = u'Sorry, I do not know what to do based on the `cosInfoJSON` you provided.'
+                                                        logger.error(msg)
+                                                        raise Exception(msg)
+                                        else:
+                                                self._openDataSource()
+                                                try:
+                                                        if isinstance(self.fs, fs.memoryfs.MemoryFS):
+                                                                logger.warning(
+                                                                        'Be aware: As directed, downloading query result into memory!'
+                                                                )
+
+                                                        if self.zipFilePath is None:
+                                                                self.zipFilePath = str(self.queryDir + PAIRS_ZIP_FILE_EXTENSION)
+                                                        if self.overwriteExisting or not self.fs.isfile(self.zipFilePath):
+                                                                # stream the query result (ZIP file)
+                                                                with self.fs.open(self.zipFilePath, 'wb') as f:
+                                                                        downloadURL = urljoin(
+                                                                                urljoin(
+                                                                                        self.pairsHost.geturl(),
+                                                                                        self.DOWNLOAD_API_STRING
+                                                                                ),
+                                                                                self.queryID
+                                                                        )
+                                                                        if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                                                                                headers = {}
+                                                                                token = 'Bearer ' + self.auth.jwt_token
+                                                                                headers['Authorization'] = token
+                                                                                downloadResponse = requests.get(
+                                                                                        downloadURL,
+                                                                                        stream  = True,
+                                                                                        verify  = self.verifySSL,
+                                                                                        headers = headers
+                                                                                )
+                                                                        else:
+                                                                                downloadResponse = requests.get(
+                                                                                        downloadURL,
+                                                                                        auth    = self.auth,
+                                                                                        stream  = True,
+                                                                                        verify  = self.verifySSL,
+                                                                                )
+                                                                        if not downloadResponse.ok:
+                                                                                self.BadDownloadFile = True
+                                                                                raise Exception('Sorry, downloading file failed.')
+
+                                                                        for block in downloadResponse.iter_content(1024):
+                                                                                f.write(block)
+                                                        else:
+                                                                logger.error('Aborted download: Zip file already present and overwriteExisting set to False')
+                                                except:
+                                                        raise
+                                                finally:
+                                                        self._closeDataSource()
+                                else:
+                                        if PAIRS_QUERY_ERR_STAT_REG_EX.match(str(statusCode)):
+                                                msg = "I am sorry, IBM PAIRS query failed, status code: '{}' ({})".format(statusCode, statusMsg)
+                                        elif PAIRS_QUERY_RUN_STAT_REG_EX.match(str(statusCode)):
+                                                msg = "Hold on, please, downloading data not an option yet, status code: '{}' ({})".format(statusCode, statusMsg)
+                                        elif PAIRS_QUERY_FINISH_STAT_REG_EX.match(str(statusCode)):
+                                                msg = "Bummer, the PAIRS query finished, but you'll never be able to download anything, status code: '{}' ({})".format(statusCode, statusMsg)
+                                        else:
+                                                msg = "Hm, not sure what is going on, status code from IBM PAIRS is '{}' ({})".format(statusCode, statusMsg)
+                                        logger.info(msg)
+                                        raise Exception(msg)
+
+                        # test if downloaded ZIP file is readable
                         try:
-                            if isinstance(self.fs, fs.memoryfs.MemoryFS):
-                                logger.warning(
-                                    'Be aware: As directed, downloading query result into memory!'
+                                self._closeDataSource()
+                                self._openDataSource()
+                        except Exception as e:
+                                # flag BadZipfile exception
+                                self.BadDownloadFile = True
+                                logger.error('Sorry, cannot read downloaded query ZIP file: {}'.format(e))
+                        else:
+                                self.BadDownloadFile = False
+                                logger.info(
+                                        "Here we go, PAIRS query result successfully downloaded as '{}'.".format(self.zipFilePath)
                                 )
-
-                            if self.zipFilePath is None:
-                                self.zipFilePath = str(self.queryDir + PAIRS_ZIP_FILE_EXTENSION)
-                            if self.overwriteExisting or not self.fs.isfile(self.zipFilePath):
-                                # stream the query result (ZIP file)
-                                with self.fs.open(self.zipFilePath, 'wb') as f:
-                                    downloadURL = urljoin(
-                                        urljoin(
-                                            self.pairsHost.geturl(),
-                                            self.DOWNLOAD_API_STRING
-                                        ),
-                                        self.queryID
-                                    )
-                                    if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-                                        headers = {}
-                                        token = 'Bearer ' + self.auth.jwt_token
-                                        headers['Authorization'] = token
-                                        downloadResponse = requests.get(
-                                            downloadURL,
-                                            stream  = True,
-                                            verify  = self.verifySSL,
-                                            headers = headers
-                                        )
-                                    else:
-                                        downloadResponse = requests.get(
-                                            downloadURL,
-                                            auth    = self.auth,
-                                            stream  = True,
-                                            verify  = self.verifySSL,
-                                        )
-                                    if not downloadResponse.ok:
-                                        self.BadDownloadFile = True
-                                        raise Exception('Sorry, downloading file failed.')
-
-                                    for block in downloadResponse.iter_content(1024):
-                                        f.write(block)
-                            else:
-                                logger.error('Aborted download: Zip file already present and overwriteExisting set to False')
-                        except:
-                            raise
                         finally:
-                            self._closeDataSource()
-                else:
-                    if PAIRS_QUERY_ERR_STAT_REG_EX.match(str(statusCode)):
-                        msg = "I am sorry, IBM PAIRS query failed, status code: '{}' ({})".format(statusCode, statusMsg)
-                    elif PAIRS_QUERY_RUN_STAT_REG_EX.match(str(statusCode)):
-                        msg = "Hold on, please, downloading data not an option yet, status code: '{}' ({})".format(statusCode, statusMsg)
-                    elif PAIRS_QUERY_FINISH_STAT_REG_EX.match(str(statusCode)):
-                        msg = "Bummer, the PAIRS query finished, but you'll never be able to download anything, status code: '{}' ({})".format(statusCode, statusMsg)
-                    else:
-                        msg = "Hm, not sure what is going on, status code from IBM PAIRS is '{}' ({})".format(statusCode, statusMsg)
-                    logger.info(msg)
-                    raise Exception(msg)
-
-            # test if downloaded ZIP file is readable
-            try:
-                self._closeDataSource()
-                self._openDataSource()
-            except Exception as e:
-                # flag BadZipfile exception
-                self.BadDownloadFile = True
-                logger.error('Sorry, cannot read downloaded query ZIP file: {}'.format(e))
-            else:
-                self.BadDownloadFile = False
-                logger.info(
-                    "Here we go, PAIRS query result successfully downloaded as '{}'.".format(self.zipFilePath)
-                )
-            finally:
-                self._closeDataSource()
-
-            # try to read data acknowledgement
-            try:
-                self.read_data_acknowledgement()
-            except:
-                pass
-
-            # silently try to list the rasters and vectors
-            try:
-                #TODO: incorporate COS mounting
-                self.list_layers()
-            except Exception as e:
-                logger.warning("Ah, implicitly running `list_layers()` did not work out: '{}'".format(e))
+                                self._closeDataSource()
 
+                        # try to read data acknowledgement
+                        try:
+                                self.read_data_acknowledgement()
+                        except:
+                                pass
 
-    def set_geometry_id_column(self, regionName):
-        """
-        Set geometry column for vector data.
+                        # silently try to list the rasters and vectors
+                        try:
+                                #TODO: incorporate COS mounting
+                                self.list_layers()
+                        except Exception as e:
+                                logger.warning("Ah, implicitly running `list_layers()` did not work out: '{}'".format(e))
 
-        :param regionName:  pandas dataframe column name of data with region information
-        :type regionName:   str
-        """
-        self.vdf_geom_col_name = regionName
 
-    def set_timestamp_column(self, timeName):
-        """
-        Set timestamp column for vector data and try to convert it to datetime objects.
+        def set_geometry_id_column(self, regionName):
+                """
+                Set geometry column for vector data.
+
+                :param regionName:  pandas dataframe column name of data with region information
+                :type regionName:   str
+                """
+                self.vdf_geom_col_name = regionName
+
+        def set_timestamp_column(self, timeName):
+                """
+                Set timestamp column for vector data and try to convert it to datetime objects.
+
+                :param timeName:    pandas dataframe column name of data with timestamps
+                :type timeName:     str
+                :raises Exception:  if it fails to convert timestamps
+                """
+                # is the data from an online (point) query?
+                if self._isOnlineQuery:
+                        try:
+                                if self.vdf is not None and isinstance(self.vdf, pandas.DataFrame) \
+                                and self.vdf[timeName].dtype in (numpy.float64, numpy.int64):
+                                        self.vdf[timeName] = self.vdf[timeName].apply(
+                                                lambda t: t if numpy.isnan(t) else datetime.datetime.fromtimestamp(
+                                                        t/1e3, tz=pytz.UTC
+                                                )
+                                        )
+                        except Exception as e:
+                                raise Exception(
+                                        "Sorry, failed to convert timestamps of column '{}' to datetime object: {}".format(timeName, e)
+                                )
+                else:
+                        # set meta data
+                        for meta in self.metadata.values():
+                                meta.update({'timestamp_col_name': timeName})
+                        if self.query['outputType'] == PAIRS_VECTOR_JSON_TYPE_NAME:
+                                # convert timestamp column
+                                try:
+                                        self.vdf[timeName].astype(str).apply(dateutil.parser.parse)
+                                        self.vdf[timeName].apply(lambda ts: pytz.UTC.localize(ts) if ts.tzinfo is None else ts)
+                                except Exception as e:
+                                        raise Exception(
+                                                'Sorry, failed to convert timestamps to datetime objects: {}'.format(e)
+                                        )
+                        elif self.query['outputType'] == PAIRS_VECTOR_CSV_TYPE_NAME:
+                                # convert timestamp column
+                                try:
+                                        if self.vdf is not None and isinstance(self.vdf, pandas.DataFrame) \
+                                        and self.vdf[timeName].dtype in (numpy.float64, numpy.int64):
+                                                self.vdf[timeName] = self.vdf[timeName].apply(
+                                                        lambda t: datetime.datetime.fromtimestamp(t, tz=pytz.UTC)
+                                                )
+                                except Exception as e:
+                                        raise Exception(
+                                                "Sorry, failed to convert timestamps to datetime objects: {}".format(e)
+                                        )
 
-        :param timeName:    pandas dataframe column name of data with timestamps
-        :type timeName:     str
-        :raises Exception:  if it fails to convert timestamps
-        """
-        # is the data from an online (point) query?
-        if self._isOnlineQuery:
-            try:
-                if self.vdf is not None and isinstance(self.vdf, pandas.DataFrame) \
-                and self.vdf[timeName].dtype in (numpy.float64, numpy.int64):
-                    self.vdf[timeName] = self.vdf[timeName].apply(
-                        lambda t: t if numpy.isnan(t) else datetime.datetime.fromtimestamp(
-                            t/1e3, tz=pytz.UTC
-                        )
-                    )
-            except Exception as e:
-                raise Exception(
-                    "Sorry, failed to convert timestamps of column '{}' to datetime object: {}".format(timeName, e)
-                )
-        else:
-            # set meta data
-            for meta in self.metadata.values():
-                meta.update({'timestamp_col_name': timeName})
-            if self.query['outputType'] == PAIRS_VECTOR_JSON_TYPE_NAME:
-                # convert timestamp column
-                try:
-                    self.vdf[timeName].astype(str).apply(dateutil.parser.parse)
-                    self.vdf[timeName].apply(lambda ts: pytz.UTC.localize(ts) if ts.tzinfo is None else ts)
-                except Exception as e:
-                    raise Exception(
-                        'Sorry, failed to convert timestamps to datetime objects: {}'.format(e)
-                    )
-            elif self.query['outputType'] == PAIRS_VECTOR_CSV_TYPE_NAME:
-                # convert timestamp column
+        def set_lat_lon_columns(self, latColName, lonColName, geomColName):
+                """
+                Set latitude and longitude columns in order to generate a GeoPandas dataframe.
+
+                :param latColName:  self.vdf Pandas data frame column name for latitude coordinate
+                :type latColName:   str
+                :param lonColName:  self.vdf Pandas data frame column name for longitude coordinate
+                :type lonColName:   str
+                :param geomColName: self.vdf GeoPandas data frame column name for point geometry
+                :type geomColName:  str
+                :raises Exception:  if it fails to generate a GeoPandas dataframe
+                """
                 try:
-                    if self.vdf is not None and isinstance(self.vdf, pandas.DataFrame) \
-                    and self.vdf[timeName].dtype in (numpy.float64, numpy.int64):
-                        self.vdf[timeName] = self.vdf[timeName].apply(
-                            lambda t: datetime.datetime.fromtimestamp(t, tz=pytz.UTC)
+                        # generate column with shapely point objects
+                        self.vdf[geomColName] = pandas.Series(
+                                [
+                                        Point(lon, lat)
+                                        for lon, lat in zip(
+                                                self.vdf[lonColName],
+                                                self.vdf[latColName]
+                                        )
+                                ]
                         )
+                        # convert Pandas dataframe to GeoPandas dataframe (if any)
+                        if HAS_GEOPANDAS:
+                                self.vdf = geopandas.GeoDataFrame(
+                                        self.vdf,
+                                        crs         = PAIRS_GEOREFERENCE_SYSTEM_NAME,
+                                        geometry    = geomColName,
+                                )
+                        else:
+                                logger.warning("GeoPandas not available on your system. Cannot convert vector dataframe to GeoPandas dataframe.")
                 except Exception as e:
-                    raise Exception(
-                        "Sorry, failed to convert timestamps to datetime objects: {}".format(e)
-                    )
-
-    def set_lat_lon_columns(self, latColName, lonColName, geomColName):
-        """
-        Set latitude and longitude columns in order to generate a GeoPandas dataframe.
-
-        :param latColName:  self.vdf Pandas data frame column name for latitude coordinate
-        :type latColName:   str
-        :param lonColName:  self.vdf Pandas data frame column name for longitude coordinate
-        :type lonColName:   str
-        :param geomColName: self.vdf GeoPandas data frame column name for point geometry
-        :type geomColName:  str
-        :raises Exception:  if it fails to generate a GeoPandas dataframe
-        """
-        try:
-            # generate column with shapely point objects
-            self.vdf[geomColName] = pandas.Series(
-                [
-                    Point(lon, lat)
-                    for lon, lat in zip(
-                        self.vdf[lonColName],
-                        self.vdf[latColName]
-                    )
-                ]
-            )
-            # convert Pandas dataframe to GeoPandas dataframe (if any)
-            if HAS_GEOPANDAS:
-                self.vdf = geopandas.GeoDataFrame(
-                    self.vdf,
-                    crs         = PAIRS_GEOREFERENCE_SYSTEM_NAME,
-                    geometry    = geomColName,
-                )
-            else:
-                logger.warning("GeoPandas not available on your system. Cannot convert vector dataframe to GeoPandas dataframe.")
-        except Exception as e:
-            raise Exception(
-                "Unable to convert Pandas dataframe to GeoDataframe: '{}'".format(e)
-            )
-
-    def split_property_string_column(self):
-        """
-        Split the property string into multiple pandas vector dataframe columns.
-
-        *note:* Applies with CSV vector data import only.
-
-        :raises Exception:  if existing columns clash with the generation of property
-                            columns produced here
-        """
-        # determine if there is property columns to operate on (if any)
-        propertyCols = list(
-            set(
-                self.vdf.columns.intersection(
-                    [PROPERTY_STRING_COL_NAME, PROPERTY_STRING_COL_NAME_POINT]
-                )
-            )
-        )
-        if len(propertyCols)>0:
-            # split the property column (assumption: there is just one)
-            split = pandas.DataFrame(
-                self.vdf[propertyCols[0]].apply(
-                    lambda x: dict(
-                        item.split(PROPERTY_STRING_SPLIT_CHAR2, 1)
-                        for item in x.split(PROPERTY_STRING_SPLIT_CHAR1)
-                    ) if isinstance(x, string_type) else {}
-                ).tolist()
-            )
-            # check that there was no previous call of this function or there
-            # is no column existing with the name of any property split
-            doubledCols = list(set(self.vdf.columns.intersection(split.columns)))
-            if len(doubledCols) == 0:
-                # concatenate property columns
-                self.vdf = pandas.concat([self.vdf, split], axis=1)
-            # most likely this function ran before
-            elif len(doubledCols) == len(split.columns):
-                logger.warning('FYI: Looks like you ran this functon before?')
-                for col in doubledCols:
-                    self.vdf[col] = split[col]
-            # most likely there is a clash between existing columns not previously
-            # generated by this function
-            else:
-                msg = "Oops, it looks like the columns {} exist, sorry, won't overwrite.".format(doubledCols)
-                logger.error(msg)
-                raise Exception(msg)
-
-    def query_pairs_polygon(self, polyID):
-        """
-        Uses PAIRS API to obtain the polygon that corresponds to a given AoI ID.
-
-        :param polyID:  PAIRS AoI ID to query data for
-        :type polyID:   int
-        :returns:       shapely.geometry.shape of the polygon associated with polyID
-                        if there is an error on retrieval, `None` is returned
-        """
-        try:
-            if not HAS_GEOJSON:
-                raise Exception('Sorry, you have not installed the GeoJSON Python module (e.g. via `pip install geojson`)')
-
-            if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-                headers = {}
-                token = 'Bearer ' + self.auth.jwt_token
-                headers['Authorization'] = token
-                polygon = requests.get(
-                    urljoin(
-                        urljoin(
-                            self.pairsHost.geturl(),
-                            self.GET_GEOJSON_API_STRING
-                        ),
-                        str(polyID)
-                    ),
-                    verify = self.verifySSL,
-                    headers = headers,
-                ).json()
-            else:
-                polygon = requests.get(
-                    urljoin(
-                        urljoin(
-                            self.pairsHost.geturl(),
-                            self.GET_GEOJSON_API_STRING
-                        ),
-                        str(polyID)
-                    ),
-                    auth   = self.auth,
-                    verify = self.verifySSL,
-                ).json()
-
-            return shape(
-                geojson.loads(
-                    polygon
-                )
-            )
-        except Exception as e:
-            logger.error(str(e))
-            return None
-
-
-    def query_pairs_polygon_meta(self, polyID):
-        """
-        Uses PAIRS API to obtain polygon meta-information that corresponds to a given AoI ID.
-
-        :param polyID:  PAIRS AoI ID to query data for
-        :type polyID:   int
-        :returns:       dict of polygon meta-data associated with polyID
-                        if there is an error on retrieval, `None` is returned
-        """
-        try:
-            if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-                headers = {}
-                token = 'Bearer ' + self.auth.jwt_token
-                headers['Authorization'] = token
-                query = requests.get(
-                    urljoin(
-                        urljoin(
-                            self.pairsHost.geturl(),
-                            self.GET_AOI_INFO_API_STRING
-                        ),
-                        str(polyID)
-                    ),
-                    verify = self.verifySSL,
-                    headers = headers,
-                ).json()['name']
-            else:
-                query = requests.get(
-                    urljoin(
-                        urljoin(
-                            self.pairsHost.geturl(),
-                            self.GET_AOI_INFO_API_STRING
-                        ),
-                        str(polyID)
-                    ),
-                    auth   = self.auth,
-                    verify = self.verifySSL,
-                ).json()['name']
-            return query
-        except Exception as e:
-            logger.error(e)
-            return None
-
-
-    def get_vector_polygon_table(self, includeGeometry=False):
-        """
-        For vector data obtain polygon geometry information from PAIRS.
+                        raise Exception(
+                                "Unable to convert Pandas dataframe to GeoDataframe: '{}'".format(e)
+                        )
 
-        :param includeGeometry:     triggers whether to include the geometrys of the polygons or not
-        :type includeGeometry:      bool
-        :raises Exception:          if there is no polygon geometry specified,
-                                    if it fails to retrieve vector geometries or info from PAIRS
-        """
-        # define vector polygon information dataframe
-        if self.pdf is None:
-            if HAS_GEOPANDAS:
-                self.pdf = geopandas.GeoDataFrame(
-                    [],
-                    columns=['polygon_id', 'polygon_name'],
-                    geometry=[],
-                )
-            else:
-                self.pdf = pandas.DataFrame(
-                    [],
-                    columns=['polygon_id', 'polygon_name'],
-                )
-        # get JSON IDs that have geometry information
-        try:
-            polyColName = self.vdf_geom_col_name
-            if polyColName is not None:
-                polyIDs = pandas.Series(
-                    self.vdf.get(
-                        polyColName,
-                    ).unique()
+        def split_property_string_column(self):
+                """
+                Split the property string into multiple pandas vector dataframe columns.
+
+                *note:* Applies with CSV vector data import only.
+
+                :raises Exception:  if existing columns clash with the generation of property
+                                                        columns produced here
+                """
+                # determine if there is property columns to operate on (if any)
+                propertyCols = list(
+                        set(
+                                self.vdf.columns.intersection(
+                                        [PROPERTY_STRING_COL_NAME, PROPERTY_STRING_COL_NAME_POINT]
+                                )
+                        )
                 )
-        except Exception as e:
-            raise Exception(
-                'Sorry, no polygon ID columns specified yet, cf. PAIRSQuery.set_geometry_id_column().'
-            )
-        # remove existing polyIDs
-        polyIDs = polyIDs[
-            ~polyIDs.isin(self.pdf.polygon_id)
-        ]
-        # get polygons from PAIRS
-        if includeGeometry:
-            logger.info(
-                'Alright, start fetching {} polygons from PAIRS, stay tuned ...'.format(len(polyIDs))
-            )
-            polys = [
-                self.query_pairs_polygon(polyID)
-                for polyID in polyIDs
-            ]
-            if None in polys:
-                logger.warning('Sorry, failed to retrieve (some) vector geometries from PAIRS.')
-        # get polygon names/info from PAIRS
-        logger.info('Let me get the polygon meta data information for you ...')
-        polyNameIDs = [
-            [
-                polyID,
-                self.query_pairs_polygon_meta(polyID)
-            ]
-            for polyID in polyIDs
-        ]
-        if None in polyNameIDs:
-            logger.warning('Sorry, failed to retrieve (some) vector meta data from PAIRS.')
-        # append information to pandas dataframe
-        if HAS_GEOPANDAS:
-            self.pdf = self.pdf.append(
-                geopandas.GeoDataFrame(
-                    polyNameIDs,
-                    columns=['polygon_id', 'polygon_name'],
-                    geometry = polys if includeGeometry else None
-                ),
-                ignore_index=True,
-            )
-        else:
-            self.pdf = self.pdf.append(
-                pandas.DataFrame(
-                    polyNameIDs,
-                    columns=['polygon_id', 'polygon_name'],
-                ),
-                ignore_index=True,
-            )
-            if includeGeometry:
-                self.pdf[PAIRS_VECTOR_GEOMETRY_COLUMN_NAME] = pandas.Series(polys)
-        logger.info('Here you go, checkout your query object, property `pdf` for the result I assembled for you.')
-
-    def list_layers(self, defaultExtension=u'', refresh=False):
-        """
-        Get general metadata information for data of the query.
+                if len(propertyCols)>0:
+                        # split the property column (assumption: there is just one)
+                        split = pandas.DataFrame(
+                                self.vdf[propertyCols[0]].apply(
+                                        lambda x: dict(
+                                                item.split(PROPERTY_STRING_SPLIT_CHAR2, 1)
+                                                for item in x.split(PROPERTY_STRING_SPLIT_CHAR1)
+                                        ) if isinstance(x, string_type) else {}
+                                ).tolist()
+                        )
+                        # check that there was no previous call of this function or there
+                        # is no column existing with the name of any property split
+                        doubledCols = list(set(self.vdf.columns.intersection(split.columns)))
+                        if len(doubledCols) == 0:
+                                # concatenate property columns
+                                self.vdf = pandas.concat([self.vdf, split], axis=1)
+                        # most likely this function ran before
+                        elif len(doubledCols) == len(split.columns):
+                                logger.warning('FYI: Looks like you ran this functon before?')
+                                for col in doubledCols:
+                                        self.vdf[col] = split[col]
+                        # most likely there is a clash between existing columns not previously
+                        # generated by this function
+                        else:
+                                msg = "Oops, it looks like the columns {} exist, sorry, won't overwrite.".format(doubledCols)
+                                logger.error(msg)
+                                raise Exception(msg)
+
+        def query_pairs_polygon(self, polyID):
+                """
+                Uses PAIRS API to obtain the polygon that corresponds to a given AoI ID.
+
+                :param polyID:  PAIRS AoI ID to query data for
+                :type polyID:   int
+                :returns:       shapely.geometry.shape of the polygon associated with polyID
+                                                if there is an error on retrieval, `None` is returned
+                """
+                try:
+                        if not HAS_GEOJSON:
+                                raise Exception('Sorry, you have not installed the GeoJSON Python module (e.g. via `pip install geojson`)')
 
-        :param defaultExtension:    sets default extension for data layer types not specified
-        :type defaultExtension:     str
-        :param refresh:             triggers the reload of the meta data from scratch
-        :type refresh:              bool
-        :raises Exception:          if no PAIRS meta data can be found to list layer information
-                                    if there is an issue reading the meta data information
-        """
-        # define path of main PAIRS query meta file
-        pairsMetaInfoPath = PAIRS_QUERY_METADATA_FILE_NAME
-        # load meta data just once (and if no point query)
-        if (self.metadata is None or refresh) and (
-            self.queryStatus is not self.querySubmit if self.queryStatus is not None else True
-        ):
-            self._openDataSource()
-            try:
-                # check if required main meta data info exists
-                if pairsMetaInfoPath not in self.queryFS.listdir(u''):
-                    msg = "No PAIRS meta data file '{}' found".format(
-                        os.path.basename(pairsMetaInfoPath)
-                    )
-                    # ATTENTION: temporarily allow missing `output.info` for pure vector data
-                    if PAIRS_VECTOR_CSV_FILE_NAME in self.queryFS.listdir(u''):
-                        logger.warning(msg)
-                    else:
-                        logger.error(msg)
-                        raise Exception(msg)
-                # ATTENTION: temporarily allow missing `output.info` for pure vector data
-                if pairsMetaInfoPath in self.queryFS.listdir(u''):
-                    with self.queryFS.open(pairsMetaInfoPath, 'rb') as j:
-                        outputJson = json.load(codecs.getreader('utf-8')(j))
-                    # format meta data as dictionary with key the file name (without extension)
-                    # ATTENTION: temporary hack for file name and name mismatch
-                    self.metadata = {
-                        fileDict['name'].replace(':', '_'): {
-                             k: v for k, v in fileDict.items() if k != 'name'
-                        }
-                        for fileDict in outputJson['files']
-                    }
-                    logger.info(
-                        "PAIRS meta data loaded from '{}'.".format(os.path.basename(pairsMetaInfoPath))
-                    )
-                else:
-                    self.metadata = {}
-                    logger.info("Initializing empty meta data dictionary.")
-                # load (optional) detailed layer information (based on the existence of
-                # a file with same name plus PAIRS file name extension for JSON files)
-                for fileName, metaData in self.metadata.items():
-                    metaPath = fileName + (
-                        defaultExtension if 'layerType' not in metaData \
-                        else self.RASTER_FILE_EXTENSION if metaData['layerType'] == PAIRS_RASTER_QUERY_NAME \
-                        else self.VECTOR_FILE_EXTENSION if metaData['layerType'] == PAIRS_VECTOR_QUERY_NAME \
-                        else u''
-                    ) + PAIRS_JSON_FILE_EXTENSION
-                    if metaPath in self.queryFS.listdir(u''):
-                        try:
-                            with self.queryFS.open(metaPath, 'rb') as j:
-                                metaData.update(
-                                    {
-                                        'details': json.load(codecs.getreader('utf-8')(j))
-                                    }
-                                )
-                            logger.debug(
-                                "Detailed meta information for data file name '{}' loaded.".format(metaPath)
-                            )
-                        except Exception as e:
-                            logger.debug(
-                                "Unable to read detailed meta information for file '{}': {}.".format(metaPath, e)
-                            )
-                # note: special treatment of default vector data file name
-                if PAIRS_VECTOR_CSV_FILE_NAME in self.queryFS.listdir(u''):
-                    self.metadata[os.path.splitext(PAIRS_VECTOR_CSV_FILE_NAME)[0]] = {
-                        'layerType': 'vector',
-                    }
-            except:
-                raise
-            finally:
-                self._closeDataSource()
+                        if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                                headers = {}
+                                token = 'Bearer ' + self.auth.jwt_token
+                                headers['Authorization'] = token
+                                polygon = requests.get(
+                                        urljoin(
+                                                urljoin(
+                                                        self.pairsHost.geturl(),
+                                                        self.GET_GEOJSON_API_STRING
+                                                ),
+                                                str(polyID)
+                                        ),
+                                        verify = self.verifySSL,
+                                        headers = headers,
+                                ).json()
+                        else:
+                                polygon = requests.get(
+                                        urljoin(
+                                                urljoin(
+                                                        self.pairsHost.geturl(),
+                                                        self.GET_GEOJSON_API_STRING
+                                                ),
+                                                str(polyID)
+                                        ),
+                                        auth   = self.auth,
+                                        verify = self.verifySSL,
+                                ).json()
+
+                        return shape(
+                                geojson.loads(
+                                        polygon
+                                )
+                        )
+                except Exception as e:
+                        logger.error(str(e))
+                        return None
 
-    def create_layer(self, fileName, layerMeta, defaultExtension=u''):
-        """
-        Load layer data such as raster or vector data.
 
-        :param fileName:            the key to identify a data layer, associated with the
-                                    corresponding file's name
-        :type fileName:             str
-        :param layerMeta:           meta information of layer to load
-        :type layerMeta:            dict
-        :param defaultExtension:    sets default extension for data layer types not specified
-        :type defaultExtension:     str
-        :raises Exception:          if layer data cannot be loaded from query ZIP file
-        """
-        # convert timestamp information (if any)
-        if PAIRS_META_TIMESTAMP_NAME in layerMeta.keys() \
-        and not isinstance(layerMeta[PAIRS_META_TIMESTAMP_NAME], datetime.datetime):
-            layerMeta[PAIRS_META_TIMESTAMP_NAME] = datetime.datetime.fromtimestamp(
-                int(layerMeta[PAIRS_META_TIMESTAMP_NAME])/1000.,
-                tz=pytz.UTC
-            )
-        # load raster data
-        # construct file path to load data from
-        layerDataPath = fileName + (
-            defaultExtension if 'layerType' not in layerMeta \
-            else self.RASTER_FILE_EXTENSION if layerMeta['layerType'] == PAIRS_RASTER_QUERY_NAME and PAIRS_JSON_SPAT_AGG_KEY not in layerMeta \
-            else self.VECTOR_FILE_EXTENSION if layerMeta['layerType'] == PAIRS_VECTOR_QUERY_NAME or PAIRS_JSON_SPAT_AGG_KEY in layerMeta \
-            else u''
-        )
-        # extract data to temporary file from ZIP (if any)
-        # get raster data
-        # ATTENTION: temporary hack in order to circumvent issue
-        if layerMeta['layerType'] == PAIRS_RASTER_QUERY_NAME \
-           and not PAIRS_JSON_SPAT_AGG_KEY in layerMeta:
-            if HAS_GDAL:
-                # note: Unforetunately GDAL does not allow to directly take Python
-                # binary file streams, thus one needs to inefficiently write back
-                # to local temporary file to get a physical file name one can and over
-                # with a file name string
-                self._openDataSource()
+        def query_pairs_polygon_meta(self, polyID):
+                """
+                Uses PAIRS API to obtain polygon meta-information that corresponds to a given AoI ID.
+
+                :param polyID:  PAIRS AoI ID to query data for
+                :type polyID:   int
+                :returns:       dict of polygon meta-data associated with polyID
+                                                if there is an error on retrieval, `None` is returned
+                """
                 try:
-                    # extract data to temporary file from ZIP
-                    # note: it looks like having the delete option causes issues on Windows machines
-                    # therefore we extract to the standard temporary directory and hope for the OS
-                    # to clean up, and that sufficient disk space is provided in the temporary directory
-                    tempFilePath = None
-                    with tempfile.NamedTemporaryFile('wb', delete=False,) as tf: #dir=self.downloadDir)
-                        with self.queryFS.open(layerDataPath, 'rb') as zf:
-                            tf.write(zf.read())
-                        tf.flush()
-                        # record path of temporary file
-                        tempFilePath = tf.name
-                        # directly read from data path
-                        ds = gdal.Open(tf.name)
-                        a  = numpy.array(ds.GetRasterBand(1).ReadAsArray(), dtype=numpy.float64)
-                        ds = None
-                    # try to expliticly remove the temporary file used to load the data
-                    if tempFilePath is not None:
-                        try:
-                            os.remove(tempFilePath)
-                        except:
-                            pass
+                        if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                                headers = {}
+                                token = 'Bearer ' + self.auth.jwt_token
+                                headers['Authorization'] = token
+                                query = requests.get(
+                                        urljoin(
+                                                urljoin(
+                                                        self.pairsHost.geturl(),
+                                                        self.GET_AOI_INFO_API_STRING
+                                                ),
+                                                str(polyID)
+                                        ),
+                                        verify = self.verifySSL,
+                                        headers = headers,
+                                ).json()['name']
+                        else:
+                                query = requests.get(
+                                        urljoin(
+                                                urljoin(
+                                                        self.pairsHost.geturl(),
+                                                        self.GET_AOI_INFO_API_STRING
+                                                ),
+                                                str(polyID)
+                                        ),
+                                        auth   = self.auth,
+                                        verify = self.verifySSL,
+                                ).json()['name']
+                        return query
                 except Exception as e:
-                    logger.error(
-                        "Unable to load '{}' from '{}' into NumPy array using GDAL: {}".format(fileName, self.zipFilePath, e)
-                    )
-                finally:
-                    self._closeDataSource()
-            else:
-                self._openDataSource()
+                        logger.error(e)
+                        return None
+
+
+        def get_vector_polygon_table(self, includeGeometry=False):
+                """
+                For vector data obtain polygon geometry information from PAIRS.
+
+                :param includeGeometry:     triggers whether to include the geometrys of the polygons or not
+                :type includeGeometry:      bool
+                :raises Exception:          if there is no polygon geometry specified,
+                                                                        if it fails to retrieve vector geometries or info from PAIRS
+                """
+                # define vector polygon information dataframe
+                if self.pdf is None:
+                        if HAS_GEOPANDAS:
+                                self.pdf = geopandas.GeoDataFrame(
+                                        [],
+                                        columns=['polygon_id', 'polygon_name'],
+                                        geometry=[],
+                                )
+                        else:
+                                self.pdf = pandas.DataFrame(
+                                        [],
+                                        columns=['polygon_id', 'polygon_name'],
+                                )
+                # get JSON IDs that have geometry information
                 try:
-                    logger.warning(
-                        "GDAL is not available for proper GeoTiff loading, default to standard PIL module to load raster data."
-                    )
-                    # note: it seems we (unfortunately) have to temporarily write/export
-                    # the image to load to the local file system first, because directly
-                    # reading the multi-wrapped virtual file handler with PIL.Image.open()
-                    # is extremely slow
-                    # TODO: explore more elegant options (problem with stream-buffer size?)
-                    tempFilePath = None
-                    with tempfile.NamedTemporaryFile('wb', delete=False,) as tf:
-                        # write raster data/image to temporary file
-                        with self.queryFS.open(layerDataPath, 'rb') as zf:
-                            tf.write(zf.read())
-                        tf.flush()
-                        # load temporary file with PIL into NumPy array
-                        with open(tf.name, 'rb') as f:
-                            im = PIL.Image.open(f)
-                            if 'details' in layerMeta and 'pixelType' in layerMeta['details']:
-                                if layerMeta['details']['pixelType'] in PAIRS_RASTER_INT_PIX_TYPE_CLASS:
-                                    im.mode=u'I'
-                                elif layerMeta['details']['pixelType'] in PAIRS_RASTER_FLOAT_PIX_TYPE_CLASS:
-                                    im.mode=u'F'
-                            else:
-                                logger.warning(
-                                    "No pixel data type identified from query meta data, default to 4 bytes floating point numbers."
+                        polyColName = self.vdf_geom_col_name
+                        if polyColName is not None:
+                                polyIDs = pandas.Series(
+                                        self.vdf.get(
+                                                polyColName,
+                                        ).unique()
                                 )
-                                im.mode=u'F'
-                            a = numpy.array(im).astype(numpy.float64)
-                    # try to expliticly remove the temporary file used to load the data
-                    if tempFilePath is not None:
-                        try:
-                            os.remove(tempFilePath)
-                        except:
-                            pass
                 except Exception as e:
-                    logger.error(
-                        "Unable to load '{}' from '{}' into NumPy array using PIL: {}".format(fileName, self.zipFilePath, e)
-                    )
-                finally:
-                    self._closeDataSource()
-            # mask no-data value
-            if 'details' in layerMeta and 'pixelNoDataVal' in layerMeta['details']:
-                a[a==numpy.float64(layerMeta['details']['pixelNoDataVal'])] = numpy.nan
-            else:
-                logger.warning(
-                        "Unable to identify pixel no-data value, using default '{}'.".format(PAIRS_DEFAULT_NODATA_VALUE)
-                )
-                a[a==numpy.float64(PAIRS_DEFAULT_NODATA_VALUE)] = numpy.nan
-            # assign loaded data to object's data dictionary
-            self.data[fileName] = a
-        # load vector data (note: CSV file format assumed)
-        elif layerMeta['layerType'] == PAIRS_VECTOR_QUERY_NAME \
-            or PAIRS_JSON_SPAT_AGG_KEY in layerMeta:
-            self._openDataSource()
-            try:
-                with self.queryFS.open(layerDataPath, 'rb') as f:
-                    # spatial aggregation vector data
-                    if PAIRS_JSON_SPAT_AGG_KEY in layerMeta:
-                        logger.info('Identified spatial aggregation data.')
-                        self.data[fileName] = pandas.read_csv(
-                            f,
-                            header      = 0,
-                            index_col   = False,
-                            quotechar   = PAIRS_VECTOR_CSV_QUOTE_CHAR,
+                        raise Exception(
+                                'Sorry, no polygon ID columns specified yet, cf. PAIRSQuery.set_geometry_id_column().'
                         )
-                    # *conventional* PAIRS vector data
-                    else:
-                        try:
-                            self.data[fileName] = pandas.read_csv(
-                                f,
-                                header      = 0,
-                                index_col   = False,
-                                quotechar   = PAIRS_VECTOR_CSV_QUOTE_CHAR,
-                                parse_dates = {
-                                    PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME: [PAIRS_VECTOR_CSV_TIMESTAMP_COL_NUM]
-                                },
-                            )
-                        except:
-                            # catch clash due to same timestamp column naming (Pandas bug)
-                            with self.queryFS.open(layerDataPath, 'rb') as f2:
-                                self.data[fileName] = pandas.read_csv(
-                                    f2,
-                                    header      = 0,
-                                    index_col   = False,
-                                    quotechar   = PAIRS_VECTOR_CSV_QUOTE_CHAR,
-                                    parse_dates = [PAIRS_VECTOR_CSV_TIMESTAMP_COL_NUM],
-                                )
+                # remove existing polyIDs
+                polyIDs = polyIDs[
+                        ~polyIDs.isin(self.pdf.polygon_id)
+                ]
+                # get polygons from PAIRS
+                if includeGeometry:
                         logger.info(
-                            "'{}' from '{}' loaded into Pandas dataframe.".format(layerDataPath, self.zipFilePath)
+                                'Alright, start fetching {} polygons from PAIRS, stay tuned ...'.format(len(polyIDs))
+                        )
+                        polys = [
+                                self.query_pairs_polygon(polyID)
+                                for polyID in polyIDs
+                        ]
+                        if None in polys:
+                                logger.warning('Sorry, failed to retrieve (some) vector geometries from PAIRS.')
+                # get polygon names/info from PAIRS
+                logger.info('Let me get the polygon meta data information for you ...')
+                polyNameIDs = [
+                        [
+                                polyID,
+                                self.query_pairs_polygon_meta(polyID)
+                        ]
+                        for polyID in polyIDs
+                ]
+                if None in polyNameIDs:
+                        logger.warning('Sorry, failed to retrieve (some) vector meta data from PAIRS.')
+                # append information to pandas dataframe
+                if HAS_GEOPANDAS:
+                        self.pdf = self.pdf.append(
+                                geopandas.GeoDataFrame(
+                                        polyNameIDs,
+                                        columns=['polygon_id', 'polygon_name'],
+                                        geometry = polys if includeGeometry else None
+                                ),
+                                ignore_index=True,
+                        )
+                else:
+                        self.pdf = self.pdf.append(
+                                pandas.DataFrame(
+                                        polyNameIDs,
+                                        columns=['polygon_id', 'polygon_name'],
+                                ),
+                                ignore_index=True,
                         )
-                        # check if timestamp column is completely empty, and if so,
-                        # assign the timestamp from the meta data
+                        if includeGeometry:
+                                self.pdf[PAIRS_VECTOR_GEOMETRY_COLUMN_NAME] = pandas.Series(polys)
+                logger.info('Here you go, checkout your query object, property `pdf` for the result I assembled for you.')
+
+        def list_layers(self, defaultExtension=u'', refresh=False):
+                """
+                Get general metadata information for data of the query.
+
+                :param defaultExtension:    sets default extension for data layer types not specified
+                :type defaultExtension:     str
+                :param refresh:             triggers the reload of the meta data from scratch
+                :type refresh:              bool
+                :raises Exception:          if no PAIRS meta data can be found to list layer information
+                                                                        if there is an issue reading the meta data information
+                """
+                # define path of main PAIRS query meta file
+                pairsMetaInfoPath = PAIRS_QUERY_METADATA_FILE_NAME
+                # load meta data just once (and if no point query)
+                if (self.metadata is None or refresh) and (
+                        self.queryStatus is not self.querySubmit if self.queryStatus is not None else True
+                ):
+                        self._openDataSource()
                         try:
-                            if self.data[fileName][PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME].apply(
-                                lambda t: isinstance(t, pandas._libs.tslibs.nattype.NaTType)
-                            ).all() and PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME in layerMeta.keys():
-                                self.data[fileName][PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME] = layerMeta[PAIRS_META_TIMESTAMP_NAME]
-                                logger.info(
-                                    "Successfully populated timestamp column '{}' with '{}'.".format(
-                                        PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME,
-                                        layerMeta[PAIRS_META_TIMESTAMP_NAME]
-                                    )
-                                )
+                                # check if required main meta data info exists
+                                if pairsMetaInfoPath not in self.queryFS.listdir(u''):
+                                        msg = "No PAIRS meta data file '{}' found".format(
+                                                os.path.basename(pairsMetaInfoPath)
+                                        )
+                                        # ATTENTION: temporarily allow missing `output.info` for pure vector data
+                                        if PAIRS_VECTOR_CSV_FILE_NAME in self.queryFS.listdir(u''):
+                                                logger.warning(msg)
+                                        else:
+                                                logger.error(msg)
+                                                raise Exception(msg)
+                                # ATTENTION: temporarily allow missing `output.info` for pure vector data
+                                if pairsMetaInfoPath in self.queryFS.listdir(u''):
+                                        with self.queryFS.open(pairsMetaInfoPath, 'rb') as j:
+                                                outputJson = json.load(codecs.getreader('utf-8')(j))
+                                        # format meta data as dictionary with key the file name (without extension)
+                                        # ATTENTION: temporary hack for file name and name mismatch
+                                        self.metadata = {
+                                                fileDict['name'].replace(':', '_'): {
+                                                         k: v for k, v in fileDict.items() if k != 'name'
+                                                }
+                                                for fileDict in outputJson['files']
+                                        }
+                                        logger.info(
+                                                "PAIRS meta data loaded from '{}'.".format(os.path.basename(pairsMetaInfoPath))
+                                        )
+                                else:
+                                        self.metadata = {}
+                                        logger.info("Initializing empty meta data dictionary.")
+                                # load (optional) detailed layer information (based on the existence of
+                                # a file with same name plus PAIRS file name extension for JSON files)
+                                for fileName, metaData in self.metadata.items():
+                                        metaPath = fileName + (
+                                                defaultExtension if 'layerType' not in metaData \
+                                                else self.RASTER_FILE_EXTENSION if metaData['layerType'] == PAIRS_RASTER_QUERY_NAME \
+                                                else self.VECTOR_FILE_EXTENSION if metaData['layerType'] == PAIRS_VECTOR_QUERY_NAME \
+                                                else u''
+                                        ) + PAIRS_JSON_FILE_EXTENSION
+                                        if metaPath in self.queryFS.listdir(u''):
+                                                try:
+                                                        with self.queryFS.open(metaPath, 'rb') as j:
+                                                                metaData.update(
+                                                                        {
+                                                                                'details': json.load(codecs.getreader('utf-8')(j))
+                                                                        }
+                                                                )
+                                                        logger.debug(
+                                                                "Detailed meta information for data file name '{}' loaded.".format(metaPath)
+                                                        )
+                                                except Exception as e:
+                                                        logger.debug(
+                                                                "Unable to read detailed meta information for file '{}': {}.".format(metaPath, e)
+                                                        )
+                                # note: special treatment of default vector data file name
+                                if PAIRS_VECTOR_CSV_FILE_NAME in self.queryFS.listdir(u''):
+                                        self.metadata[os.path.splitext(PAIRS_VECTOR_CSV_FILE_NAME)[0]] = {
+                                                'layerType': 'vector',
+                                        }
                         except:
-                            # silently pass if this bonus option does not work
-                            pass
-            except Exception as e:
-                logger.error(
-                    "Unable to load '{}' from '{}' into Pandas dataframe: {}".format(layerDataPath, self.zipFilePath, e)
-                )
-            finally:
-                self._closeDataSource()
-        else:
-            msg = "Sorry, I do not know how to load PAIRS query data of type '{}'".format(layerMeta['layerType'])
-            logger.error(msg)
-            raise Exception(msg)
+                                raise
+                        finally:
+                                self._closeDataSource()
 
-    def create_layers(self, defaultExtension=u''):
-        """
-        From PAIRS query ZIP file generate Python data structures for layers in memory.
+        def create_layer(self, fileName, layerMeta, defaultExtension=u''):
+                """
+                Load layer data such as raster or vector data.
+
+                :param fileName:            the key to identify a data layer, associated with the
+                                                                        corresponding file's name
+                :type fileName:             str
+                :param layerMeta:           meta information of layer to load
+                :type layerMeta:            dict
+                :param defaultExtension:    sets default extension for data layer types not specified
+                :type defaultExtension:     str
+                :raises Exception:          if layer data cannot be loaded from query ZIP file
+                """
+                # convert timestamp information (if any)
+                if PAIRS_META_TIMESTAMP_NAME in layerMeta.keys() \
+                and not isinstance(layerMeta[PAIRS_META_TIMESTAMP_NAME], datetime.datetime):
+                        layerMeta[PAIRS_META_TIMESTAMP_NAME] = datetime.datetime.fromtimestamp(
+                                int(layerMeta[PAIRS_META_TIMESTAMP_NAME])/1000.,
+                                tz=pytz.UTC
+                        )
+                # load raster data
+                # construct file path to load data from
+                layerDataPath = fileName + (
+                        defaultExtension if 'layerType' not in layerMeta \
+                        else self.RASTER_FILE_EXTENSION if layerMeta['layerType'] == PAIRS_RASTER_QUERY_NAME and PAIRS_JSON_SPAT_AGG_KEY not in layerMeta \
+                        else self.VECTOR_FILE_EXTENSION if layerMeta['layerType'] == PAIRS_VECTOR_QUERY_NAME or PAIRS_JSON_SPAT_AGG_KEY in layerMeta \
+                        else u''
+                )
+                # extract data to temporary file from ZIP (if any)
+                # get raster data
+                # ATTENTION: temporary hack in order to circumvent issue
+                if layerMeta['layerType'] == PAIRS_RASTER_QUERY_NAME \
+                     and not PAIRS_JSON_SPAT_AGG_KEY in layerMeta:
+                        if HAS_GDAL:
+                                # note: Unforetunately GDAL does not allow to directly take Python
+                                # binary file streams, thus one needs to inefficiently write back
+                                # to local temporary file to get a physical file name one can and over
+                                # with a file name string
+                                self._openDataSource()
+                                try:
+                                        # extract data to temporary file from ZIP
+                                        # note: it looks like having the delete option causes issues on Windows machines
+                                        # therefore we extract to the standard temporary directory and hope for the OS
+                                        # to clean up, and that sufficient disk space is provided in the temporary directory
+                                        tempFilePath = None
+                                        with tempfile.NamedTemporaryFile('wb', delete=False,) as tf: #dir=self.downloadDir)
+                                                with self.queryFS.open(layerDataPath, 'rb') as zf:
+                                                        tf.write(zf.read())
+                                                tf.flush()
+                                                # record path of temporary file
+                                                tempFilePath = tf.name
+                                                # directly read from data path
+                                                ds = gdal.Open(tf.name)
+                                                a  = numpy.array(ds.GetRasterBand(1).ReadAsArray(), dtype=numpy.float64)
+                                                ds = None
+                                        # try to expliticly remove the temporary file used to load the data
+                                        if tempFilePath is not None:
+                                                try:
+                                                        os.remove(tempFilePath)
+                                                except:
+                                                        pass
+                                except Exception as e:
+                                        logger.error(
+                                                "Unable to load '{}' from '{}' into NumPy array using GDAL: {}".format(fileName, self.zipFilePath, e)
+                                        )
+                                finally:
+                                        self._closeDataSource()
+                        else:
+                                self._openDataSource()
+                                try:
+                                        logger.warning(
+                                                "GDAL is not available for proper GeoTiff loading, default to standard PIL module to load raster data."
+                                        )
+                                        # note: it seems we (unfortunately) have to temporarily write/export
+                                        # the image to load to the local file system first, because directly
+                                        # reading the multi-wrapped virtual file handler with PIL.Image.open()
+                                        # is extremely slow
+                                        # TODO: explore more elegant options (problem with stream-buffer size?)
+                                        tempFilePath = None
+                                        with tempfile.NamedTemporaryFile('wb', delete=False,) as tf:
+                                                # write raster data/image to temporary file
+                                                with self.queryFS.open(layerDataPath, 'rb') as zf:
+                                                        tf.write(zf.read())
+                                                tf.flush()
+                                                # load temporary file with PIL into NumPy array
+                                                with open(tf.name, 'rb') as f:
+                                                        im = PIL.Image.open(f)
+                                                        if 'details' in layerMeta and 'pixelType' in layerMeta['details']:
+                                                                if layerMeta['details']['pixelType'] in PAIRS_RASTER_INT_PIX_TYPE_CLASS:
+                                                                        im.mode=u'I'
+                                                                elif layerMeta['details']['pixelType'] in PAIRS_RASTER_FLOAT_PIX_TYPE_CLASS:
+                                                                        im.mode=u'F'
+                                                        else:
+                                                                logger.warning(
+                                                                        "No pixel data type identified from query meta data, default to 4 bytes floating point numbers."
+                                                                )
+                                                                im.mode=u'F'
+                                                        a = numpy.array(im).astype(numpy.float64)
+                                        # try to expliticly remove the temporary file used to load the data
+                                        if tempFilePath is not None:
+                                                try:
+                                                        os.remove(tempFilePath)
+                                                except:
+                                                        pass
+                                except Exception as e:
+                                        logger.error(
+                                                "Unable to load '{}' from '{}' into NumPy array using PIL: {}".format(fileName, self.zipFilePath, e)
+                                        )
+                                finally:
+                                        self._closeDataSource()
+                        # mask no-data value
+                        if 'details' in layerMeta and 'pixelNoDataVal' in layerMeta['details']:
+                                a[a==numpy.float64(layerMeta['details']['pixelNoDataVal'])] = numpy.nan
+                        else:
+                                logger.warning(
+                                                "Unable to identify pixel no-data value, using default '{}'.".format(PAIRS_DEFAULT_NODATA_VALUE)
+                                )
+                                a[a==numpy.float64(PAIRS_DEFAULT_NODATA_VALUE)] = numpy.nan
+                        # assign loaded data to object's data dictionary
+                        self.data[fileName] = a
+                # load vector data (note: CSV file format assumed)
+                elif layerMeta['layerType'] == PAIRS_VECTOR_QUERY_NAME \
+                        or PAIRS_JSON_SPAT_AGG_KEY in layerMeta:
+                        self._openDataSource()
+                        try:
+                                with self.queryFS.open(layerDataPath, 'rb') as f:
+                                        # spatial aggregation vector data
+                                        if PAIRS_JSON_SPAT_AGG_KEY in layerMeta:
+                                                logger.info('Identified spatial aggregation data.')
+                                                self.data[fileName] = pandas.read_csv(
+                                                        f,
+                                                        header      = 0,
+                                                        index_col   = False,
+                                                        quotechar   = PAIRS_VECTOR_CSV_QUOTE_CHAR,
+                                                )
+                                        # *conventional* PAIRS vector data
+                                        else:
+                                                try:
+                                                        self.data[fileName] = pandas.read_csv(
+                                                                f,
+                                                                header      = 0,
+                                                                index_col   = False,
+                                                                quotechar   = PAIRS_VECTOR_CSV_QUOTE_CHAR,
+                                                                parse_dates = {
+                                                                        PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME: [PAIRS_VECTOR_CSV_TIMESTAMP_COL_NUM]
+                                                                },
+                                                        )
+                                                except:
+                                                        # catch clash due to same timestamp column naming (Pandas bug)
+                                                        with self.queryFS.open(layerDataPath, 'rb') as f2:
+                                                                self.data[fileName] = pandas.read_csv(
+                                                                        f2,
+                                                                        header      = 0,
+                                                                        index_col   = False,
+                                                                        quotechar   = PAIRS_VECTOR_CSV_QUOTE_CHAR,
+                                                                        parse_dates = [PAIRS_VECTOR_CSV_TIMESTAMP_COL_NUM],
+                                                                )
+                                                logger.info(
+                                                        "'{}' from '{}' loaded into Pandas dataframe.".format(layerDataPath, self.zipFilePath)
+                                                )
+                                                # check if timestamp column is completely empty, and if so,
+                                                # assign the timestamp from the meta data
+                                                try:
+                                                        if self.data[fileName][PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME].apply(
+                                                                lambda t: isinstance(t, pandas._libs.tslibs.nattype.NaTType)
+                                                        ).all() and PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME in layerMeta.keys():
+                                                                self.data[fileName][PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME] = layerMeta[PAIRS_META_TIMESTAMP_NAME]
+                                                                logger.info(
+                                                                        "Successfully populated timestamp column '{}' with '{}'.".format(
+                                                                                PAIRS_VECTOR_TIMESTAMP_COLUMN_NAME,
+                                                                                layerMeta[PAIRS_META_TIMESTAMP_NAME]
+                                                                        )
+                                                                )
+                                                except:
+                                                        # silently pass if this bonus option does not work
+                                                        pass
+                        except Exception as e:
+                                logger.error(
+                                        "Unable to load '{}' from '{}' into Pandas dataframe: {}".format(layerDataPath, self.zipFilePath, e)
+                                )
+                        finally:
+                                self._closeDataSource()
+                else:
+                        msg = "Sorry, I do not know how to load PAIRS query data of type '{}'".format(layerMeta['layerType'])
+                        logger.error(msg)
+                        raise Exception(msg)
 
-        :param defaultExtension:    sets default extension for data layer types not specified
-        :type defaultExtension:     str
-        """
-        # Make sure that the layer listing exists
-        if self.metadata is None:
-            self.list_layers()
-        # no raster data availabile?
-        if self.metadata is not None:
-            for fileName, layerMeta in self.metadata.items():
-                self.create_layer(fileName, layerMeta, defaultExtension=defaultExtension)
+        def create_layers(self, defaultExtension=u''):
+                """
+                From PAIRS query ZIP file generate Python data structures for layers in memory.
+
+                :param defaultExtension:    sets default extension for data layer types not specified
+                :type defaultExtension:     str
+                """
+                # Make sure that the layer listing exists
+                if self.metadata is None:
+                        self.list_layers()
+                # no raster data availabile?
+                if self.metadata is not None:
+                        for fileName, layerMeta in self.metadata.items():
+                                self.create_layer(fileName, layerMeta, defaultExtension=defaultExtension)
 
 # }}}
 
 # fold: class optimized for PAIRS timeseries queries{{{
 class PAIRSTimeSeries(object):
-    """
-    Assemble time series data from PAIRS data layers.
+        """
+        Assemble time series data from PAIRS data layers.
 
-    :param querySpecs:                              defines layers and spatio-temporal intervals to pull from PAIRS,
-                                                    the JSON schema is defined by PAIRSTimeSeries.QUERY_INPUT_JSON_SCHEMA
-    :type querySpecs:                               dict
-    :raises jsonschema.exceptions.ValidationError:  in case the input `querySpecs` does not conform to the required format
-    """
-    # general settings
-    UNIX_EPOCH_ZERO_TIME            = datetime.datetime(1970,1,1,0,0,0, tzinfo=pytz.UTC)
-    # time series dataframe related settings
-    DATAFRAME_LATITUDE_NAME         = 'latitude'
-    DATAFRAME_LONGITUDE_NAME        = 'longitude'
-    DATAFRAME_TIMESTAMP_NAME        = 'timestamp'
-    # PAIRS related configuration settings
-    PAIRS_TIMESERIES_ENDPOINT       = 'v2/timeseries'
-    PAIRS_QUERY_RETRIES             = 10
-    PAIRS_QUERY_RETRY_BACKOFF_FACTOR= 3
-    PAIRS_JSON_VALUE_KEY_NAME       = 'value'
-    PAIRS_JSON_TIMESTAMP_NAME       = 'timestamp'
-    PAIRS_NUM_PARALLEL_QUERIES      = 2
-    PAIRS_QUERY_SUCCESS_CODES       = [200, 201]
-    # define class variables
-    QUERY_INPUT_JSON_SCHEMA = {
-        "$schema": "http://json-schema.org/draft-07/schema#",
-        "type": "object",
-        "properties": {
-            "layers": {
-                "type": "array",
-                "items": {
-                    "type": "object",
-                    "properties": {
-                        "pairs-layer-id":   {"type": "string"},
-                        "column-name":      {"type": "string"},
-                        "dimensions": {
-                            "type": "array",
-                            "items": {
-                                "type": "object",
-                                "properties": {
-                                    "name": {"type": "string"},
-                                    "value": {"type": "string"},
-                                },
-                            },
-                        },
-                    },
-                    "required": ["pairs-layer-id", "column-name",],
-                }
-            },
-            "spatio-temporal-queries": {
-                "type": "array",
-                "items": {
-                    "type": "object",
-                    "properties": {
-                        "longitude":{"type": "number"},
-                        "latitude": {"type": "number"},
-                        "temporal": {
-                            "type": "array",
-                            "items": {
-                                "type": "object",
-                                "properties": {
-                                    "start": {"type": "string"},
-                                    "end": {"type": "string"},
-                                },
-                                "required": ["start", "end",],
-                            }
+        :param querySpecs:                              defines layers and spatio-temporal intervals to pull from PAIRS,
+                                                                                                        the JSON schema is defined by PAIRSTimeSeries.QUERY_INPUT_JSON_SCHEMA
+        :type querySpecs:                               dict
+        :raises jsonschema.exceptions.ValidationError:  in case the input `querySpecs` does not conform to the required format
+        """
+        # general settings
+        UNIX_EPOCH_ZERO_TIME            = datetime.datetime(1970,1,1,0,0,0, tzinfo=pytz.UTC)
+        # time series dataframe related settings
+        DATAFRAME_LATITUDE_NAME         = 'latitude'
+        DATAFRAME_LONGITUDE_NAME        = 'longitude'
+        DATAFRAME_TIMESTAMP_NAME        = 'timestamp'
+        # PAIRS related configuration settings
+        PAIRS_TIMESERIES_ENDPOINT       = 'v2/timeseries'
+        PAIRS_QUERY_RETRIES             = 10
+        PAIRS_QUERY_RETRY_BACKOFF_FACTOR= 3
+        PAIRS_JSON_VALUE_KEY_NAME       = 'value'
+        PAIRS_JSON_TIMESTAMP_NAME       = 'timestamp'
+        PAIRS_NUM_PARALLEL_QUERIES      = 2
+        PAIRS_QUERY_SUCCESS_CODES       = [200, 201]
+        # define class variables
+        QUERY_INPUT_JSON_SCHEMA = {
+                "$schema": "http://json-schema.org/draft-07/schema#",
+                "type": "object",
+                "properties": {
+                        "layers": {
+                                "type": "array",
+                                "items": {
+                                        "type": "object",
+                                        "properties": {
+                                                "pairs-layer-id":   {"type": "string"},
+                                                "column-name":      {"type": "string"},
+                                                "dimensions": {
+                                                        "type": "array",
+                                                        "items": {
+                                                                "type": "object",
+                                                                "properties": {
+                                                                        "name": {"type": "string"},
+                                                                        "value": {"type": "string"},
+                                                                },
+                                                        },
+                                                },
+                                        },
+                                        "required": ["pairs-layer-id", "column-name",],
+                                }
                         },
-                    },
-                    "required": ["longitude", "latitude", "temporal",],
-                }
-            }
-        },
-        "required": ["layers", "spatio-temporal-queries",],
-    }
-
-
-
-    def __init__(
-        self, querySpecs,
-    ):
-        # save input
-        self.querySpecs = copy.deepcopy(querySpecs)
-        # check input for correct schema
-        jsonschema.validate(
-            instance    = self.querySpecs,
-            schema      = self.QUERY_INPUT_JSON_SCHEMA,
-        )
-        # reformat input
-        ## transform input (simplify layer information in preparation for query string)
-        self.querySpecs['layers'] = {
-            layer["column-name"]: '{layerID}{dimensionList}'.format(
-                layerID         = layer["pairs-layer-id"],
-                dimensionList   = '&dimension='+','.join(
-                    [
-                        '{name}%3D{value}'.format(name=dimension['name'], value=dimension['value'])
-                        for dimension in layer['dimensions']
-                    ]
-                ) if 'dimensions' in layer else '',
-            )
-            for layer in self.querySpecs['layers']
+                        "spatio-temporal-queries": {
+                                "type": "array",
+                                "items": {
+                                        "type": "object",
+                                        "properties": {
+                                                "longitude":{"type": "number"},
+                                                "latitude": {"type": "number"},
+                                                "temporal": {
+                                                        "type": "array",
+                                                        "items": {
+                                                                "type": "object",
+                                                                "properties": {
+                                                                        "start": {"type": "string"},
+                                                                        "end": {"type": "string"},
+                                                                },
+                                                                "required": ["start", "end",],
+                                                        }
+                                                },
+                                        },
+                                        "required": ["longitude", "latitude", "temporal",],
+                                }
+                        }
+                },
+                "required": ["layers", "spatio-temporal-queries",],
         }
 
-        ## convert timestamps of input to UNIX epoch
-        try:
-            for entry in self.querySpecs['spatio-temporal-queries']:
-                entry['temporal'] = [
-                    {
-                        'start':int(1e3*(dateutil.parser.isoparse(item['start'])-self.UNIX_EPOCH_ZERO_TIME).total_seconds()),
-                        'end':  int(1e3*(dateutil.parser.isoparse(item['end'])-self.UNIX_EPOCH_ZERO_TIME).total_seconds()),
-                    }
-                    for item in entry['temporal']
-                ]
-        except Exception as e:
-            raise Exception('Invalid `querySpecs` given: {}'.format(e))
-        # print reformatted input for debugging
-        logger.debug(json.dumps(self.querySpecs, indent=2))
 
 
+        def __init__(
+                self, querySpecs,
+        ):
+                # save input
+                self.querySpecs = copy.deepcopy(querySpecs)
+                # check input for correct schema
+                jsonschema.validate(
+                        instance    = self.querySpecs,
+                        schema      = self.QUERY_INPUT_JSON_SCHEMA,
+                )
+                # reformat input
+                ## transform input (simplify layer information in preparation for query string)
+                self.querySpecs['layers'] = {
+                        layer["column-name"]: '{layerID}{dimensionList}'.format(
+                                layerID         = layer["pairs-layer-id"],
+                                dimensionList   = '&dimension='+','.join(
+                                        [
+                                                '{name}%3D{value}'.format(name=dimension['name'], value=dimension['value'])
+                                                for dimension in layer['dimensions']
+                                        ]
+                                ) if 'dimensions' in layer else '',
+                        )
+                        for layer in self.querySpecs['layers']
+                }
 
-    def _get_pairs_timeseries(
-        self, lon, lat, t0, t1, layerID, auth,
-        requestFunction     = requests.get,
-        rawDataDumpDir      = None,
-        authType            = 'password'
-    ):
-        """
-        Extracts time series of point location from PAIRS through time series API endpoint.
+                ## convert timestamps of input to UNIX epoch
+                try:
+                        for entry in self.querySpecs['spatio-temporal-queries']:
+                                entry['temporal'] = [
+                                        {
+                                                'start':int(1e3*(dateutil.parser.isoparse(item['start'])-self.UNIX_EPOCH_ZERO_TIME).total_seconds()),
+                                                'end':  int(1e3*(dateutil.parser.isoparse(item['end'])-self.UNIX_EPOCH_ZERO_TIME).total_seconds()),
+                                        }
+                                        for item in entry['temporal']
+                                ]
+                except Exception as e:
+                        raise Exception('Invalid `querySpecs` given: {}'.format(e))
+                # print reformatted input for debugging
+                logger.debug(json.dumps(self.querySpecs, indent=2))
 
-        :param lon:             longitude of point of interest
-        :type lon:              float
-        :param lat:             latitude of point of interest
-        :type lat:              float
-        :param t0:              UNIX epoch time in milliseconds to start time series
-        :type t0:               int
-        :param t1:              UNIX epoch time in milliseconds to end time series
-        :type t1:               int
-        :param layerID:         PAIRS layer ID to query, potentially with URL-compatible
-                                dimension specification in format:
-                                `&dimension=<name1>%D3<value1>,<name1>%D3<value1>...`
-        :type layerID:          str
-        :param auth:            PAIRS credentials for authentication
-        :type auth:             (str, str) or authentication.OAuth2
-        :param requestFunction: request function to be used for GET call to PAIRS
-        :type requestFunction:  function
-        :param rawDataDumpDir:  if set, the PAIRS query result is dumped as JSON
-                                file into the given directory
-        :type rawDataDumpDir:   str
-        :param authType:        'password' or 'api-key'
-        :type authType:         str
-        :returns:               time series data queried from PAIRS for layer `layerID`
-                                and dictionary of time series summary information
-                                - temporal interval: [`"first-timestamp"`, `"last-timestamp"`]
-                                - number of timestamps in `"number-data-points"`
-        :rtype:                 pandas.DataFrame, dict
-        :raises Exception:      if `t0` is smaller than `t1` or if the JSON data
-                                dump directory does not exist
-        """
 
-        # make temporal interval inclusive
-        t0 = copy.copy(t0)-1000
-        # check inputs
-        try:
-            assert t0 < t1
-        except Exception as e:
-            raise Exception('start of time interval is later than its end.: {}'.format(e))
-        if rawDataDumpDir is not None and not os.path.isdir(rawDataDumpDir):
-            raise Exception(
-                "The directory path '{}' does not exist.".format(rawDataDumpDir)
-            )
-
-        # compose PAIRS query URL
-        url="{baseURL}{timeseriesEndpoint}?start={startUNIXEpochMS}&end={endUNIXEpochMS}&lon={longitude}&lat={latitude}&layer={layerID}".format(
-            baseURL             = self.pairsBaseURL,
-            timeseriesEndpoint  = self.PAIRS_TIMESERIES_ENDPOINT,
-            # adjust for the fact that the starting timestamp (in milliseconds)
-            # is exlusive, i.e. a timestamp in PAIRS with exactly t0 would not get returned
-            startUNIXEpochMS    = t0,
-            endUNIXEpochMS      = t1,
-            longitude           = lon,
-            latitude            = lat,
-            layerID             = layerID,
-        )
-        logger.debug(url)
-        if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-            headers = {}
-            token = 'Bearer ' + self.auth.jwt_token
-            headers['Authorization'] = token
-            response = requestFunction(url=url, verify=self.verifySSL, headers=headers,)
-        else:
-            response = requestFunction(url=url, auth=auth, verify=self.verifySSL,)
-        # check that the response is valid
-        if response.status_code not in self.PAIRS_QUERY_SUCCESS_CODES:
-            raise requests.HTTPError(response.status_code)
-        # convert response into Pandas dataframe
-        try:
-            # make Pandas dataframe from PAIRS query JSON
-            responseJSON = response.json()
-            df = pandas.DataFrame(responseJSON['data'])
-            # format Pandas dataframe
-            if len(df)==0:
-                logger.warning("{} returned no data: {}".format(url,response.text))
-                return None, None
-            # convert timestamp
-            df[self.PAIRS_JSON_TIMESTAMP_NAME]  = pandas.to_datetime(
-                df[self.PAIRS_JSON_TIMESTAMP_NAME], unit='ms', utc=True,
-            )
-            # add layer information column
-            df['layerID']                       = layerID
-            df[self.DATAFRAME_LONGITUDE_NAME]   = lon
-            df[self.DATAFRAME_LATITUDE_NAME]    = lat
-        except Exception as e:
-            raise Exception('Unable to convert PAIRS data into Pandas dataframe.: {}'.format(e))
-        # write raw data queried to file (if any)
-        if rawDataDumpDir is not None:
-            with open(
-                os.path.join(
-                    rawDataDumpDir,
-                    TIMESERIES_RESPONSE_FILE_SCHEMA.format(
-                        layerID=layerID, lon=lon, lat=lat, t0=t0, t1=t1,
-                    )
-            ), 'w') as fp:
-                try:
-                    # Python 3
-                    json.dump(responseJSON, fp)
-                except:
-                    # Python 2
-                    fp.write(json.dumps(responseJSON, ensure_ascii=False,))
 
-        return df, {
-            'first-timestamp':      responseJSON['start'],
-            'last-timestamp':       responseJSON['end'],
-            'number-data-points':   responseJSON['count'],
-        }
+        def _get_pairs_timeseries(
+                self, lon, lat, t0, t1, layerID, auth,
+                requestFunction     = requests.get,
+                rawDataDumpDir      = None,
+                authType            = 'password'
+        ):
+                """
+                Extracts time series of point location from PAIRS through time series API endpoint.
 
+                :param lon:             longitude of point of interest
+                :type lon:              float
+                :param lat:             latitude of point of interest
+                :type lat:              float
+                :param t0:              UNIX epoch time in milliseconds to start time series
+                :type t0:               int
+                :param t1:              UNIX epoch time in milliseconds to end time series
+                :type t1:               int
+                :param layerID:         PAIRS layer ID to query, potentially with URL-compatible
+                                                                dimension specification in format:
+                                                                `&dimension=<name1>%D3<value1>,<name1>%D3<value1>...`
+                :type layerID:          str
+                :param auth:            PAIRS credentials for authentication
+                :type auth:             (str, str) or authentication.OAuth2
+                :param requestFunction: request function to be used for GET call to PAIRS
+                :type requestFunction:  function
+                :param rawDataDumpDir:  if set, the PAIRS query result is dumped as JSON
+                                                                file into the given directory
+                :type rawDataDumpDir:   str
+                :param authType:        'password' or 'api-key'
+                :type authType:         str
+                :returns:               time series data queried from PAIRS for layer `layerID`
+                                                                and dictionary of time series summary information
+                                                                - temporal interval: [`"first-timestamp"`, `"last-timestamp"`]
+                                                                - number of timestamps in `"number-data-points"`
+                :rtype:                 pandas.DataFrame, dict
+                :raises Exception:      if `t0` is smaller than `t1` or if the JSON data
+                                                                dump directory does not exist
+                """
+
+                # make temporal interval inclusive
+                t0 = copy.copy(t0)-1000
+                # check inputs
+                try:
+                        assert t0 < t1
+                except Exception as e:
+                        raise Exception('start of time interval is later than its end.: {}'.format(e))
+                if rawDataDumpDir is not None and not os.path.isdir(rawDataDumpDir):
+                        raise Exception(
+                                "The directory path '{}' does not exist.".format(rawDataDumpDir)
+                        )
 
+                # compose PAIRS query URL
+                url="{baseURL}{timeseriesEndpoint}?start={startUNIXEpochMS}&end={endUNIXEpochMS}&lon={longitude}&lat={latitude}&layer={layerID}".format(
+                        baseURL             = self.pairsBaseURL,
+                        timeseriesEndpoint  = self.PAIRS_TIMESERIES_ENDPOINT,
+                        # adjust for the fact that the starting timestamp (in milliseconds)
+                        # is exlusive, i.e. a timestamp in PAIRS with exactly t0 would not get returned
+                        startUNIXEpochMS    = t0,
+                        endUNIXEpochMS      = t1,
+                        longitude           = lon,
+                        latitude            = lat,
+                        layerID             = layerID,
+                )
+                logger.debug(url)
+                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                        headers = {}
+                        token = 'Bearer ' + self.auth.jwt_token
+                        headers['Authorization'] = token
+                        response = requestFunction(url=url, verify=self.verifySSL, headers=headers,)
+                else:
+                        response = requestFunction(url=url, auth=auth, verify=self.verifySSL,)
+                # check that the response is valid
+                if response.status_code not in self.PAIRS_QUERY_SUCCESS_CODES:
+                        raise requests.HTTPError(response.status_code)
+                # convert response into Pandas dataframe
+                try:
+                        # make Pandas dataframe from PAIRS query JSON
+                        responseJSON = response.json()
+                        df = pandas.DataFrame(responseJSON['data'])
+                        # format Pandas dataframe
+                        if len(df)==0:
+                                logger.warning("{} returned no data: {}".format(url,response.text))
+                                return None, None
+                        # convert timestamp
+                        df[self.PAIRS_JSON_TIMESTAMP_NAME]  = pandas.to_datetime(
+                                df[self.PAIRS_JSON_TIMESTAMP_NAME], unit='ms', utc=True,
+                        )
+                        # add layer information column
+                        df['layerID']                       = layerID
+                        df[self.DATAFRAME_LONGITUDE_NAME]   = lon
+                        df[self.DATAFRAME_LATITUDE_NAME]    = lat
+                except Exception as e:
+                        raise Exception('Unable to convert PAIRS data into Pandas dataframe.: {}'.format(e))
+                # write raw data queried to file (if any)
+                if rawDataDumpDir is not None:
+                        with open(
+                                os.path.join(
+                                        rawDataDumpDir,
+                                        TIMESERIES_RESPONSE_FILE_SCHEMA.format(
+                                                layerID=layerID, lon=lon, lat=lat, t0=t0, t1=t1,
+                                        )
+                        ), 'w') as fp:
+                                try:
+                                        # Python 3
+                                        json.dump(responseJSON, fp)
+                                except:
+                                        # Python 2
+                                        fp.write(json.dumps(responseJSON, ensure_ascii=False,))
+
+                return df, {
+                        'first-timestamp':      responseJSON['start'],
+                        'last-timestamp':       responseJSON['end'],
+                        'number-data-points':   responseJSON['count'],
+                }
 
-    def get_dataframe(
-        self,
-        pairsBaseURL        = None,
-        verifySSL           = True,
-        auth                = None,
-        spatioTemporalIndex = False,
-        authType            = 'password'
-    ):
-        """
-        Function to query point data from PAIRS.
 
-        :param pairsBaseURL:                       PAIRS base URL to be used for API endpoint,
-                                                   example: `https://pairs.res.ibm.com:443`
-        :type pairsBaseURL:                        str
-        :param verifySSL:                          if SSL connections get verified
-        :type verifySSL:                           bool
-        :param auth:                               PAIRS API credentials in (user, password) format
-        :type auth:                                (str, str)
-        :param spatioTemporalIndex:                whether or not to spatio-temorally index the Pandas dataframe to be returned,
-                                                   *note*: temporal index comes last for time series optimization
-        :type spatioTemporalIndex                  bool
-        :param authType:                           'password' or 'api-key'
-        :type port:                                str
-        :returns:                                  table with PAIRS data
-        :rtype:                                    pandas.DataFrame
-        :raises urllib3.exceptions.MaxRetryError:  in case PAIRS is unreachable
-        :raises requests.HTTPError:                in case the PAIRS HTTP response code is not 200
-        """
 
-        self.authType = authType
+        def get_dataframe(
+                self,
+                pairsBaseURL        = None,
+                verifySSL           = True,
+                auth                = None,
+                spatioTemporalIndex = False,
+                authType            = 'password'
+        ):
+                """
+                Function to query point data from PAIRS.
 
-        # set PAIRS connection details
-        ## PAIRS URL (guarantee trailing slash)
-        self.pairsBaseURL = '{}://{}{}'.format(
-            PAIRS_DEFAULT_PROTOCOL,
-            PAIRS_DEFAULT_SERVER,
-            PAIRS_DEFAULT_BASE_URI,
-        ) if pairsBaseURL is None else pairsBaseURL
-        if len(self.pairsBaseURL)>0 and self.pairsBaseURL[-1]!='/':
-            self.pairsBaseURL += '/'
-        ## authentication
-        if self.authType.lower() in ['api-key', 'apikey', 'api key']:
-            if type(auth) is authentication.OAuth2:
-                self.auth = auth
-            else:
-                self.auth = authentication.OAuth2(
-                    host = PAIRS_DEFAULT_SERVER,
-                    username     = PAIRS_DEFAULT_USER,
-                    api_key_file = PAIRS_DEFAULT_PASSWORD_FILE_NAME,
-                )
-        else:
-            self.auth   = (
-                PAIRS_DEFAULT_USER,
-                get_pairs_api_password(
-                    server  = PAIRS_DEFAULT_SERVER,
-                    user    = PAIRS_DEFAULT_USER,
-                    passFile= PAIRS_DEFAULT_PASSWORD_FILE_NAME,
-                )
-            ) if auth is None else auth
+                :param pairsBaseURL:                       PAIRS base URL to be used for API endpoint,
+                                                                                                     example: `https://pairs.res.ibm.com:443`
+                :type pairsBaseURL:                        str
+                :param verifySSL:                          if SSL connections get verified
+                :type verifySSL:                           bool
+                :param auth:                               PAIRS API credentials in (user, password) format
+                :type auth:                                (str, str)
+                :param spatioTemporalIndex:                whether or not to spatio-temorally index the Pandas dataframe to be returned,
+                                                                                                     *note*: temporal index comes last for time series optimization
+                :type spatioTemporalIndex                  bool
+                :param authType:                           'password' or 'api-key'
+                :type port:                                str
+                :returns:                                  table with PAIRS data
+                :rtype:                                    pandas.DataFrame
+                :raises urllib3.exceptions.MaxRetryError:  in case PAIRS is unreachable
+                :raises requests.HTTPError:                in case the PAIRS HTTP response code is not 200
+                """
+
+                self.authType = authType
+
+                # set PAIRS connection details
+                ## PAIRS URL (guarantee trailing slash)
+                self.pairsBaseURL = '{}://{}{}'.format(
+                        PAIRS_DEFAULT_PROTOCOL,
+                        PAIRS_DEFAULT_SERVER,
+                        PAIRS_DEFAULT_BASE_URI,
+                ) if pairsBaseURL is None else pairsBaseURL
+                if len(self.pairsBaseURL)>0 and self.pairsBaseURL[-1]!='/':
+                        self.pairsBaseURL += '/'
+                ## authentication
+                if self.authType.lower() in ['api-key', 'apikey', 'api key']:
+                        if type(auth) is authentication.OAuth2:
+                                self.auth = auth
+                        else:
+                                self.auth = authentication.OAuth2(
+                                        host = PAIRS_DEFAULT_SERVER,
+                                        username     = PAIRS_DEFAULT_USER,
+                                        api_key_file = PAIRS_DEFAULT_PASSWORD_FILE_NAME,
+                                )
+                else:
+                        self.auth   = (
+                                PAIRS_DEFAULT_USER,
+                                get_pairs_api_password(
+                                        server  = PAIRS_DEFAULT_SERVER,
+                                        user    = PAIRS_DEFAULT_USER,
+                                        passFile= PAIRS_DEFAULT_PASSWORD_FILE_NAME,
+                                )
+                        ) if auth is None else auth
 
-        ## SSL verification
-        self.verifySSL = verifySSL
+                ## SSL verification
+                self.verifySSL = verifySSL
 
-        # set up requests session
-        ## set retry rules for PAIRS queries
-        retryRules = requests.packages.urllib3.util.retry.Retry(
-            total           = self.PAIRS_QUERY_RETRIES,
-            backoff_factor  = self.PAIRS_QUERY_RETRY_BACKOFF_FACTOR,
-        )
-
-        ## instantiate requests session and parallel execution
-        adapter = requests.adapters.HTTPAdapter(max_retries=retryRules)
-        with requests.Session() as http, \
-             concurrent.futures.ThreadPoolExecutor(
-                 max_workers=self.PAIRS_NUM_PARALLEL_QUERIES
-             ) as pool:
-            # register requests session
-            http.mount("https://", adapter)
-            http.mount("http://", adapter)
-            # compile list of arguments for parallel PAIRS query jobs
-            try:
-                parallelExecuteList = [
-                    {
-                        "t0":               interval['start'],
-                        "t1":               interval['end'],
-                        "lon":              query['longitude'],
-                        "lat":              query['latitude'],
-                        "layerID":          layerID,
-                        "requestFunction":  http.get,
-                    }
-                    for layerName, layerID in self.querySpecs['layers'].items()
-                    for query in self.querySpecs['spatio-temporal-queries']
-                    for interval in query['temporal']
-                ]
-            except Exception as e:
-                raise Exception('Unable to generate PAIRS queries from `querySpecs`: {}'.format(e))
-            # fetch data from PAIRS
-            pairsQueryDataFrames = [
-                df
-                for df, _ in pool.map(
-                    lambda x: self._get_pairs_timeseries(auth=auth, authType=authType, **x),
-                    parallelExecuteList
-                )
-                if df is not None
-            ]
-            logger.debug(
-                'There has been {} PAIRS time series queries with no data available.'.format(
-                    len(parallelExecuteList) - len(pairsQueryDataFrames)
-                )
-            )
+                # set up requests session
+                ## set retry rules for PAIRS queries
+                retryRules = requests.packages.urllib3.util.retry.Retry(
+                        total           = self.PAIRS_QUERY_RETRIES,
+                        backoff_factor  = self.PAIRS_QUERY_RETRY_BACKOFF_FACTOR,
+                )
+
+                ## instantiate requests session and parallel execution
+                adapter = requests.adapters.HTTPAdapter(max_retries=retryRules)
+                with requests.Session() as http, \
+                         concurrent.futures.ThreadPoolExecutor(
+                                 max_workers=self.PAIRS_NUM_PARALLEL_QUERIES
+                         ) as pool:
+                        # register requests session
+                        http.mount("https://", adapter)
+                        http.mount("http://", adapter)
+                        # compile list of arguments for parallel PAIRS query jobs
+                        try:
+                                parallelExecuteList = [
+                                        {
+                                                "t0":               interval['start'],
+                                                "t1":               interval['end'],
+                                                "lon":              query['longitude'],
+                                                "lat":              query['latitude'],
+                                                "layerID":          layerID,
+                                                "requestFunction":  http.get,
+                                        }
+                                        for layerName, layerID in self.querySpecs['layers'].items()
+                                        for query in self.querySpecs['spatio-temporal-queries']
+                                        for interval in query['temporal']
+                                ]
+                        except Exception as e:
+                                raise Exception('Unable to generate PAIRS queries from `querySpecs`: {}'.format(e))
+                        # fetch data from PAIRS
+                        pairsQueryDataFrames = [
+                                df
+                                for df, _ in pool.map(
+                                        lambda x: self._get_pairs_timeseries(auth=auth, authType=authType, **x),
+                                        parallelExecuteList
+                                )
+                                if df is not None
+                        ]
+                        logger.debug(
+                                'There has been {} PAIRS time series queries with no data available.'.format(
+                                        len(parallelExecuteList) - len(pairsQueryDataFrames)
+                                )
+                        )
 
-            # concatenate PAIRS query results
-            fullDf = pandas.concat(pairsQueryDataFrames, axis=0, ignore_index=True)
+                        # concatenate PAIRS query results
+                        fullDf = pandas.concat(pairsQueryDataFrames, axis=0, ignore_index=True)
 
 
-            # reshape Pandas dataframe for final output
-            ## instantiate empty, auxiliary dataframe for iterative joining
-            auxDf = pandas.DataFrame(
-                [],
-                columns=[
-                    self.DATAFRAME_LONGITUDE_NAME,
-                    self.DATAFRAME_LATITUDE_NAME,
-                    self.PAIRS_JSON_TIMESTAMP_NAME,
-                    self.PAIRS_JSON_VALUE_KEY_NAME,
-                ],
-            )
-            ## prepare function to infer column name from PAIRS layer ID (with dimension)
-            inverseLayerDict = { v: k for k, v in self.querySpecs['layers'].items() }
-            ## join groups of data from full query result
-            for layerID, layerData in fullDf.groupby('layerID'):
-                layerData.drop('layerID', inplace=True, axis=1)
-                auxDf = auxDf.merge(
-                    layerData.rename(
-                        columns={self.PAIRS_JSON_VALUE_KEY_NAME: inverseLayerDict[layerID],},
-                    ),
-                    how = 'outer',
-                    on  = [
-                        self.DATAFRAME_LATITUDE_NAME,
-                        self.DATAFRAME_LONGITUDE_NAME,
-                        self.PAIRS_JSON_TIMESTAMP_NAME,
-                    ],
-                )
-            ## reformat data frame include indexing and timestamp column renaming
-            fullDf = auxDf.reset_index(drop=True).drop(
-                self.PAIRS_JSON_VALUE_KEY_NAME, axis=1
-            ).rename(
-                columns = {
-                    self.PAIRS_JSON_TIMESTAMP_NAME: self.DATAFRAME_TIMESTAMP_NAME,
-                }
-            )
+                        # reshape Pandas dataframe for final output
+                        ## instantiate empty, auxiliary dataframe for iterative joining
+                        auxDf = pandas.DataFrame(
+                                [],
+                                columns=[
+                                        self.DATAFRAME_LONGITUDE_NAME,
+                                        self.DATAFRAME_LATITUDE_NAME,
+                                        self.PAIRS_JSON_TIMESTAMP_NAME,
+                                        self.PAIRS_JSON_VALUE_KEY_NAME,
+                                ],
+                        )
+                        ## prepare function to infer column name from PAIRS layer ID (with dimension)
+                        inverseLayerDict = { v: k for k, v in self.querySpecs['layers'].items() }
+                        ## join groups of data from full query result
+                        for layerID, layerData in fullDf.groupby('layerID'):
+                                layerData.drop('layerID', inplace=True, axis=1)
+                                auxDf = auxDf.merge(
+                                        layerData.rename(
+                                                columns={self.PAIRS_JSON_VALUE_KEY_NAME: inverseLayerDict[layerID],},
+                                        ),
+                                        how = 'outer',
+                                        on  = [
+                                                self.DATAFRAME_LATITUDE_NAME,
+                                                self.DATAFRAME_LONGITUDE_NAME,
+                                                self.PAIRS_JSON_TIMESTAMP_NAME,
+                                        ],
+                                )
+                        ## reformat data frame include indexing and timestamp column renaming
+                        fullDf = auxDf.reset_index(drop=True).drop(
+                                self.PAIRS_JSON_VALUE_KEY_NAME, axis=1
+                        ).rename(
+                                columns = {
+                                        self.PAIRS_JSON_TIMESTAMP_NAME: self.DATAFRAME_TIMESTAMP_NAME,
+                                }
+                        )
 
-            ## spatio-temporal indexing if requested
-            if spatioTemporalIndex:
-                fullDf = fullDf.set_index([
-                    self.DATAFRAME_LONGITUDE_NAME,
-                    self.DATAFRAME_LATITUDE_NAME,
-                    self.DATAFRAME_TIMESTAMP_NAME,
-                ])
+                        ## spatio-temporal indexing if requested
+                        if spatioTemporalIndex:
+                                fullDf = fullDf.set_index([
+                                        self.DATAFRAME_LONGITUDE_NAME,
+                                        self.DATAFRAME_LATITUDE_NAME,
+                                        self.DATAFRAME_TIMESTAMP_NAME,
+                                ])
 
 
-            return fullDf
+                        return fullDf
 #}}}
```

### Comparing `ibmpairs-0.2.7/ibmpairs/query.py` & `ibmpairs-0.2.8/ibmpairs/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -6161,15 +6161,15 @@
             logger.info(msg)
             
             qj = QueryJob(status = msg)
             query.status_response = qj
             poll       = False
             incomplete = False
             
-    #    
+    #
     async def async_download(self,
                              query,
                              client: cl.Client    = None,
                              status_interval: int = QUERY_STATUS_CHECK_INTERVAL,
                              download_folder      = None,
                              download_file_name   = None,
                              verify: bool         = constants.GLOBAL_SSL_VERIFY
```

### Comparing `ibmpairs-0.2.7/ibmpairs/upload.py` & `ibmpairs-0.2.8/ibmpairs/upload.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.7/ibmpairs/utils.py` & `ibmpairs-0.2.8/ibmpairs/utils.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.7/ibmpairs.egg-info/PKG-INFO` & `ibmpairs-0.2.8/ibmpairs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmpairs
-Version: 0.2.7
+Version: 0.2.8
 Summary: open source Python modules for the IBM PAIRS Geoscope platform
 Home-page: https://ibmpairs.mybluemix.net
 Author: Physical Analytics, IBM Research
 Author-email: pairs@us.ibm.com
 Maintainer: cmalbrec
 License: BSD-Clause-3
 Project-URL: Documentation, https://pairs.res.ibm.com/tutorial
```

### Comparing `ibmpairs-0.2.7/ibmpairs.egg-info/SOURCES.txt` & `ibmpairs-0.2.8/ibmpairs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.7/setup.py` & `ibmpairs-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 # define package version
-version = '0.2.7'
+version = '0.2.8'
 # ... and record it for ibmpairs package
 with open("ibmpairs/version.py", 'w') as f:
     f.write('# generated by setup.py\nversion = "{}"\n'.format(version))
 
 def readme():
     try:
         with open('README.md') as f:
```

