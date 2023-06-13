# Comparing `tmp/dsm-django-socialauth-1.0.8.tar.gz` & `tmp/dsm-django-socialauth-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsm-django-socialauth-1.0.8.tar", last modified: Fri Feb  3 08:16:25 2023, max compression
+gzip compressed data, was "dsm-django-socialauth-1.0.9.tar", last modified: Mon Feb  6 07:50:59 2023, max compression
```

## Comparing `dsm-django-socialauth-1.0.8.tar` & `dsm-django-socialauth-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-02-03 08:16:25.955868 dsm-django-socialauth-1.0.8/
--rw-r--r--   0 naii       (501) staff       (20)     1090 2021-06-11 03:56:18.000000 dsm-django-socialauth-1.0.8/LICENSE
--rw-r--r--   0 naii       (501) staff       (20)       33 2021-06-11 03:48:24.000000 dsm-django-socialauth-1.0.8/MANIFEST.in
--rw-r--r--   0 naii       (501) staff       (20)     4266 2023-02-03 08:16:25.954797 dsm-django-socialauth-1.0.8/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)     3400 2023-01-12 08:14:18.000000 dsm-django-socialauth-1.0.8/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-02-03 08:16:25.944573 dsm-django-socialauth-1.0.8/dsm_django_socialauth.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)     4266 2023-02-03 08:16:25.000000 dsm-django-socialauth-1.0.8/dsm_django_socialauth.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      371 2023-02-03 08:16:25.000000 dsm-django-socialauth-1.0.8/dsm_django_socialauth.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-02-03 08:16:25.000000 dsm-django-socialauth-1.0.8/dsm_django_socialauth.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       53 2023-02-03 08:16:25.000000 dsm-django-socialauth-1.0.8/dsm_django_socialauth.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)        8 2023-02-03 08:16:25.000000 dsm-django-socialauth-1.0.8/dsm_django_socialauth.egg-info/top_level.txt
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-02-03 08:16:25.951050 dsm-django-socialauth-1.0.8/dsmauth/
--rw-r--r--   0 naii       (501) staff       (20)      181 2023-02-03 08:16:16.000000 dsm-django-socialauth-1.0.8/dsmauth/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     2112 2022-11-14 08:01:37.000000 dsm-django-socialauth-1.0.8/dsmauth/backend.py
--rw-r--r--   0 naii       (501) staff       (20)     1908 2023-01-12 04:22:01.000000 dsm-django-socialauth-1.0.8/dsmauth/complete.py
--rw-r--r--   0 naii       (501) staff       (20)      352 2023-02-03 08:13:21.000000 dsm-django-socialauth-1.0.8/dsmauth/urls.py
--rw-r--r--   0 naii       (501) staff       (20)      130 2023-01-12 04:21:59.000000 dsm-django-socialauth-1.0.8/dsmauth/utils.py
--rw-r--r--   0 naii       (501) staff       (20)      825 2023-02-03 08:08:55.000000 dsm-django-socialauth-1.0.8/dsmauth/views.py
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-02-03 08:16:25.956070 dsm-django-socialauth-1.0.8/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1537 2023-02-03 08:14:15.000000 dsm-django-socialauth-1.0.8/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-02-06 07:50:59.600268 dsm-django-socialauth-1.0.9/
+-rw-r--r--   0 naii       (501) staff       (20)     1090 2021-06-11 03:56:18.000000 dsm-django-socialauth-1.0.9/LICENSE
+-rw-r--r--   0 naii       (501) staff       (20)       33 2021-06-11 03:48:24.000000 dsm-django-socialauth-1.0.9/MANIFEST.in
+-rw-r--r--   0 naii       (501) staff       (20)     4801 2023-02-06 07:50:59.599921 dsm-django-socialauth-1.0.9/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)     3935 2023-02-06 07:47:42.000000 dsm-django-socialauth-1.0.9/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-02-06 07:50:59.594306 dsm-django-socialauth-1.0.9/dsm_django_socialauth.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     4801 2023-02-06 07:50:59.000000 dsm-django-socialauth-1.0.9/dsm_django_socialauth.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      371 2023-02-06 07:50:59.000000 dsm-django-socialauth-1.0.9/dsm_django_socialauth.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-02-06 07:50:59.000000 dsm-django-socialauth-1.0.9/dsm_django_socialauth.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       53 2023-02-06 07:50:59.000000 dsm-django-socialauth-1.0.9/dsm_django_socialauth.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)        8 2023-02-06 07:50:59.000000 dsm-django-socialauth-1.0.9/dsm_django_socialauth.egg-info/top_level.txt
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-02-06 07:50:59.599174 dsm-django-socialauth-1.0.9/dsmauth/
+-rw-r--r--   0 naii       (501) staff       (20)      181 2023-02-06 07:47:54.000000 dsm-django-socialauth-1.0.9/dsmauth/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)     2112 2022-11-14 08:01:37.000000 dsm-django-socialauth-1.0.9/dsmauth/backend.py
+-rw-r--r--   0 naii       (501) staff       (20)     1908 2023-01-12 04:22:01.000000 dsm-django-socialauth-1.0.9/dsmauth/complete.py
+-rw-r--r--   0 naii       (501) staff       (20)      352 2023-02-03 08:13:21.000000 dsm-django-socialauth-1.0.9/dsmauth/urls.py
+-rw-r--r--   0 naii       (501) staff       (20)      130 2023-01-12 04:21:59.000000 dsm-django-socialauth-1.0.9/dsmauth/utils.py
+-rw-r--r--   0 naii       (501) staff       (20)      962 2023-02-06 07:37:15.000000 dsm-django-socialauth-1.0.9/dsmauth/views.py
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-02-06 07:50:59.600384 dsm-django-socialauth-1.0.9/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     1537 2023-02-06 07:48:00.000000 dsm-django-socialauth-1.0.9/setup.py
```

### Comparing `dsm-django-socialauth-1.0.8/LICENSE` & `dsm-django-socialauth-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dsm-django-socialauth-1.0.8/PKG-INFO` & `dsm-django-socialauth-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsm-django-socialauth
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple way to use Custom authentication in django application. for dsm
 Home-page: https://gitlab.com/public-project2/dsm-django-oauth
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -131,14 +131,17 @@
 ```
 
 ## Authentication step
 
 <img src="_docs/authenflow.png" height="400px">
 
 1. frontend href to ```<BACKEND_URL>/oauth/login/dsmauth```
+    - optional ```<BACKEND_URL>/oauth/login/dsmauth/?callback=<FRONTEND_URI>```
+        - FRONTEND_URI : domain frontend or localhost:xxxx
+        - default: use in backend settings ```BASE_FRONTEND_URL``` and ```BASE_BACKEND_URL```
 2. backend authentication with oauth server
 3. if authen complete backend callback to frontend ```<BASE_FRONTEND_URL>/callback?token=<REFRESH_TOKEN>```
  - note BASE_FRONTEND_URL in backend/settings.py previous step
 4. frontend request access token with refresh token via 
     - request
 
     ```
@@ -159,7 +162,14 @@
 - request to backend
 ```
 URL : <BACKEND>/api/xxx
 HEADER : {
     'Authorization': "Bearer <ACCESS_TOKEN>"
 }
 ```
+
+## logout / sign out
+
+- logout href to ```<BACKEND_URL>/authen/logout/```
+    - optional ```<BACKEND_URL>/authen/logout/?callback=<FRONTEND_URI>```
+        - FRONTEND_URI : domain frontend or localhost:xxxx
+        - default: use in backend settings ```BASE_FRONTEND_URL``` and ```BASE_BACKEND_URL```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dsm-django-socialauth Version: 1.0.8 Summary: A
+Metadata-Version: 2.1 Name: dsm-django-socialauth Version: 1.0.9 Summary: A
 simple way to use Custom authentication in django application. for dsm Home-
 page: https://gitlab.com/public-project2/dsm-django-oauth Author:
 DigitalStoreMesh Co.,Ltd Author-email: contact@storemesh.com License: MIT
 License Classifier: Environment :: Web Environment Classifier: Framework ::
 Django Classifier: Framework :: Django :: 4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
@@ -40,14 +40,21 @@
 dsmauth.views import logout urlpatterns = [ ... path('oauth/complete//',
 complete, name='complete'), path('oauth/', include('social_django.urls',
 namespace='social')), # in django2 path('authen/', include('dsmauth.urls')) ...
 ] ``` ### in template ``` ... Login_with_DSM LOGOUT ... ``` # If use backend-
 frontend (Client Site Render) can use authentication with JWT ### in
 settings.py ```python BASE_FRONTEND_URL='http://localhost:3000/' ``` ##
 Authentication step [_docs/authenflow.png] 1. frontend href to ```/oauth/login/
-dsmauth``` 2. backend authentication with oauth server 3. if authen complete
-backend callback to frontend ```/callback?token=``` - note BASE_FRONTEND_URL in
-backend/settings.py previous step 4. frontend request access token with refresh
-token via - request ``` [POST] : /authen/token/refresh/ body : { "refresh" : "
+dsmauth``` - optional ```/oauth/login/dsmauth/?callback=``` - FRONTEND_URI :
+domain frontend or localhost:xxxx - default: use in backend settings
+```BASE_FRONTEND_URL``` and ```BASE_BACKEND_URL``` 2. backend authentication
+with oauth server 3. if authen complete backend callback to frontend ```/
+callback?token=``` - note BASE_FRONTEND_URL in backend/settings.py previous
+step 4. frontend request access token with refresh token via - request ```
+[POST] : /authen/token/refresh/ body : { "refresh" : "
 >" } ``` - reponse ``` { "access": "eyJ0eXAiOiJKV1Qi...ifZOpwg" } ``` 5.
 frontend collect access(access token) for request api ## How to use - request
-to backend ``` URL : /api/xxx HEADER : { 'Authorization': "Bearer " } ```
+to backend ``` URL : /api/xxx HEADER : { 'Authorization': "Bearer " } ``` ##
+logout / sign out - logout href to ```/authen/logout/``` - optional ```/authen/
+logout/?callback=``` - FRONTEND_URI : domain frontend or localhost:xxxx -
+default: use in backend settings ```BASE_FRONTEND_URL``` and
+```BASE_BACKEND_URL```
```

### Comparing `dsm-django-socialauth-1.0.8/README.md` & `dsm-django-socialauth-1.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -109,14 +109,17 @@
 ```
 
 ## Authentication step
 
 <img src="_docs/authenflow.png" height="400px">
 
 1. frontend href to ```<BACKEND_URL>/oauth/login/dsmauth```
+    - optional ```<BACKEND_URL>/oauth/login/dsmauth/?callback=<FRONTEND_URI>```
+        - FRONTEND_URI : domain frontend or localhost:xxxx
+        - default: use in backend settings ```BASE_FRONTEND_URL``` and ```BASE_BACKEND_URL```
 2. backend authentication with oauth server
 3. if authen complete backend callback to frontend ```<BASE_FRONTEND_URL>/callback?token=<REFRESH_TOKEN>```
  - note BASE_FRONTEND_URL in backend/settings.py previous step
 4. frontend request access token with refresh token via 
     - request
 
     ```
@@ -136,8 +139,15 @@
 ## How to use
 - request to backend
 ```
 URL : <BACKEND>/api/xxx
 HEADER : {
     'Authorization': "Bearer <ACCESS_TOKEN>"
 }
-```
+```
+
+## logout / sign out
+
+- logout href to ```<BACKEND_URL>/authen/logout/```
+    - optional ```<BACKEND_URL>/authen/logout/?callback=<FRONTEND_URI>```
+        - FRONTEND_URI : domain frontend or localhost:xxxx
+        - default: use in backend settings ```BASE_FRONTEND_URL``` and ```BASE_BACKEND_URL```
```

#### html2text {}

```diff
@@ -28,14 +28,21 @@
 dsmauth.views import logout urlpatterns = [ ... path('oauth/complete//',
 complete, name='complete'), path('oauth/', include('social_django.urls',
 namespace='social')), # in django2 path('authen/', include('dsmauth.urls')) ...
 ] ``` ### in template ``` ... Login_with_DSM LOGOUT ... ``` # If use backend-
 frontend (Client Site Render) can use authentication with JWT ### in
 settings.py ```python BASE_FRONTEND_URL='http://localhost:3000/' ``` ##
 Authentication step [_docs/authenflow.png] 1. frontend href to ```/oauth/login/
-dsmauth``` 2. backend authentication with oauth server 3. if authen complete
-backend callback to frontend ```/callback?token=``` - note BASE_FRONTEND_URL in
-backend/settings.py previous step 4. frontend request access token with refresh
-token via - request ``` [POST] : /authen/token/refresh/ body : { "refresh" : "
+dsmauth``` - optional ```/oauth/login/dsmauth/?callback=``` - FRONTEND_URI :
+domain frontend or localhost:xxxx - default: use in backend settings
+```BASE_FRONTEND_URL``` and ```BASE_BACKEND_URL``` 2. backend authentication
+with oauth server 3. if authen complete backend callback to frontend ```/
+callback?token=``` - note BASE_FRONTEND_URL in backend/settings.py previous
+step 4. frontend request access token with refresh token via - request ```
+[POST] : /authen/token/refresh/ body : { "refresh" : "
 >" } ``` - reponse ``` { "access": "eyJ0eXAiOiJKV1Qi...ifZOpwg" } ``` 5.
 frontend collect access(access token) for request api ## How to use - request
-to backend ``` URL : /api/xxx HEADER : { 'Authorization': "Bearer " } ```
+to backend ``` URL : /api/xxx HEADER : { 'Authorization': "Bearer " } ``` ##
+logout / sign out - logout href to ```/authen/logout/``` - optional ```/authen/
+logout/?callback=``` - FRONTEND_URI : domain frontend or localhost:xxxx -
+default: use in backend settings ```BASE_FRONTEND_URL``` and
+```BASE_BACKEND_URL```
```

### Comparing `dsm-django-socialauth-1.0.8/dsm_django_socialauth.egg-info/PKG-INFO` & `dsm-django-socialauth-1.0.9/dsm_django_socialauth.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsm-django-socialauth
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple way to use Custom authentication in django application. for dsm
 Home-page: https://gitlab.com/public-project2/dsm-django-oauth
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -131,14 +131,17 @@
 ```
 
 ## Authentication step
 
 <img src="_docs/authenflow.png" height="400px">
 
 1. frontend href to ```<BACKEND_URL>/oauth/login/dsmauth```
+    - optional ```<BACKEND_URL>/oauth/login/dsmauth/?callback=<FRONTEND_URI>```
+        - FRONTEND_URI : domain frontend or localhost:xxxx
+        - default: use in backend settings ```BASE_FRONTEND_URL``` and ```BASE_BACKEND_URL```
 2. backend authentication with oauth server
 3. if authen complete backend callback to frontend ```<BASE_FRONTEND_URL>/callback?token=<REFRESH_TOKEN>```
  - note BASE_FRONTEND_URL in backend/settings.py previous step
 4. frontend request access token with refresh token via 
     - request
 
     ```
@@ -159,7 +162,14 @@
 - request to backend
 ```
 URL : <BACKEND>/api/xxx
 HEADER : {
     'Authorization': "Bearer <ACCESS_TOKEN>"
 }
 ```
+
+## logout / sign out
+
+- logout href to ```<BACKEND_URL>/authen/logout/```
+    - optional ```<BACKEND_URL>/authen/logout/?callback=<FRONTEND_URI>```
+        - FRONTEND_URI : domain frontend or localhost:xxxx
+        - default: use in backend settings ```BASE_FRONTEND_URL``` and ```BASE_BACKEND_URL```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dsm-django-socialauth Version: 1.0.8 Summary: A
+Metadata-Version: 2.1 Name: dsm-django-socialauth Version: 1.0.9 Summary: A
 simple way to use Custom authentication in django application. for dsm Home-
 page: https://gitlab.com/public-project2/dsm-django-oauth Author:
 DigitalStoreMesh Co.,Ltd Author-email: contact@storemesh.com License: MIT
 License Classifier: Environment :: Web Environment Classifier: Framework ::
 Django Classifier: Framework :: Django :: 4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
@@ -40,14 +40,21 @@
 dsmauth.views import logout urlpatterns = [ ... path('oauth/complete//',
 complete, name='complete'), path('oauth/', include('social_django.urls',
 namespace='social')), # in django2 path('authen/', include('dsmauth.urls')) ...
 ] ``` ### in template ``` ... Login_with_DSM LOGOUT ... ``` # If use backend-
 frontend (Client Site Render) can use authentication with JWT ### in
 settings.py ```python BASE_FRONTEND_URL='http://localhost:3000/' ``` ##
 Authentication step [_docs/authenflow.png] 1. frontend href to ```/oauth/login/
-dsmauth``` 2. backend authentication with oauth server 3. if authen complete
-backend callback to frontend ```/callback?token=``` - note BASE_FRONTEND_URL in
-backend/settings.py previous step 4. frontend request access token with refresh
-token via - request ``` [POST] : /authen/token/refresh/ body : { "refresh" : "
+dsmauth``` - optional ```/oauth/login/dsmauth/?callback=``` - FRONTEND_URI :
+domain frontend or localhost:xxxx - default: use in backend settings
+```BASE_FRONTEND_URL``` and ```BASE_BACKEND_URL``` 2. backend authentication
+with oauth server 3. if authen complete backend callback to frontend ```/
+callback?token=``` - note BASE_FRONTEND_URL in backend/settings.py previous
+step 4. frontend request access token with refresh token via - request ```
+[POST] : /authen/token/refresh/ body : { "refresh" : "
 >" } ``` - reponse ``` { "access": "eyJ0eXAiOiJKV1Qi...ifZOpwg" } ``` 5.
 frontend collect access(access token) for request api ## How to use - request
-to backend ``` URL : /api/xxx HEADER : { 'Authorization': "Bearer " } ```
+to backend ``` URL : /api/xxx HEADER : { 'Authorization': "Bearer " } ``` ##
+logout / sign out - logout href to ```/authen/logout/``` - optional ```/authen/
+logout/?callback=``` - FRONTEND_URI : domain frontend or localhost:xxxx -
+default: use in backend settings ```BASE_FRONTEND_URL``` and
+```BASE_BACKEND_URL```
```

### Comparing `dsm-django-socialauth-1.0.8/dsmauth/backend.py` & `dsm-django-socialauth-1.0.9/dsmauth/backend.py`

 * *Files identical despite different names*

### Comparing `dsm-django-socialauth-1.0.8/dsmauth/complete.py` & `dsm-django-socialauth-1.0.9/dsmauth/complete.py`

 * *Files identical despite different names*

### Comparing `dsm-django-socialauth-1.0.8/dsmauth/views.py` & `dsm-django-socialauth-1.0.9/dsmauth/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,14 @@
 _uri = getattr(settings, 'OAUTH_DSM_SERVER_BASEURL', None)
 _scheme = getattr(settings, 'OAUTH_DSM_SCHEME', None)
 if _uri is None:
     raise Exception("Please input `OAUTH_DSM_SERVER_BASEURL` in settings.py")
 
 def logout(request):
     logout_view(request)
-    REDIRECT_FRONTEND = utils.append_slash(url=_REDIRECT_FRONTEND)
+    callback_uri = request.GET.get('callback', None)
+    REDIRECT_FRONTEND = _REDIRECT_FRONTEND if callback_uri == None else callback_uri
+    REDIRECT_FRONTEND = utils.append_slash(url=REDIRECT_FRONTEND)
     if REDIRECT_FRONTEND is not None:
         return HttpResponseRedirect(f"{_scheme}://{_uri}/logout?next={REDIRECT_FRONTEND}")
     return HttpResponseRedirect(f"{_scheme}://{_uri}/logout?next={_REDIRECT_BACKEND}")
```

### Comparing `dsm-django-socialauth-1.0.8/setup.py` & `dsm-django-socialauth-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='dsm-django-socialauth',
-    version='1.0.8',
+    version='1.0.9',
     url='https://gitlab.com/public-project2/dsm-django-oauth',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple way to use Custom authentication in django application. for dsm',
     long_description=README,
     long_description_content_type='text/markdown',
```

