# Comparing `tmp/roadtx-1.3.1.tar.gz` & `tmp/roadtx-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadtx-1.3.1.tar", last modified: Fri Jun  2 13:39:09 2023, max compression
+gzip compressed data, was "roadtx-1.3.2.tar", last modified: Tue Jun 13 13:32:20 2023, max compression
```

## Comparing `roadtx-1.3.1.tar` & `roadtx-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 13:39:09.951048 roadtx-1.3.1/
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-06-02 13:39:09.951048 roadtx-1.3.1/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 13:39:09.951048 roadtx-1.3.1/roadtools/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 13:39:09.951048 roadtx-1.3.1/roadtools/roadtx/
--rw-r--r--   0 vsts      (1001) docker     (123)     7865 2023-06-02 13:37:39.000000 roadtx-1.3.1/roadtools/roadtx/keepass.py
--rw-r--r--   0 vsts      (1001) docker     (123)    52146 2023-06-02 13:37:39.000000 roadtx-1.3.1/roadtools/roadtx/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12028 2023-06-02 13:37:39.000000 roadtx-1.3.1/roadtools/roadtx/selenium.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 13:39:09.951048 roadtx-1.3.1/roadtx.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      301 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 13:39:07.000000 roadtx-1.3.1/roadtx.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       66 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-02 13:39:09.951048 roadtx-1.3.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-06-02 13:37:39.000000 roadtx-1.3.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:32:20.272841 roadtx-1.3.2/
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-06-13 13:32:20.272841 roadtx-1.3.2/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:32:20.272841 roadtx-1.3.2/roadtools/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:32:20.272841 roadtx-1.3.2/roadtools/roadtx/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7865 2023-06-13 13:30:49.000000 roadtx-1.3.2/roadtools/roadtx/keepass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    52771 2023-06-13 13:30:49.000000 roadtx-1.3.2/roadtools/roadtx/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14364 2023-06-13 13:30:49.000000 roadtx-1.3.2/roadtools/roadtx/selenium.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:32:20.272841 roadtx-1.3.2/roadtx.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      301 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 13:32:17.000000 roadtx-1.3.2/roadtx.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       66 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-13 13:32:20.272841 roadtx-1.3.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-06-13 13:30:49.000000 roadtx-1.3.2/setup.py
```

### Comparing `roadtx-1.3.1/PKG-INFO` & `roadtx-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.3.1
+Version: 1.3.2
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.3.1/roadtools/roadtx/keepass.py` & `roadtx-1.3.2/roadtools/roadtx/keepass.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.3.1/roadtools/roadtx/main.py` & `roadtx-1.3.2/roadtools/roadtx/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,14 +236,17 @@
     urlhelp = 'Url to initiate browsing. Will be constructed from below parameters if not supplied.'
     intauth_parser = subparsers.add_parser('interactiveauth', help='Interactive authentication in Selenium browser window, optional autofill')
     intauth_parser.add_argument('-u', '--username', action='store', metavar='USER', help='User to authenticate')
     intauth_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password of the user')
     intauth_parser.add_argument('--krbtoken',
                                 action='store',
                                 help='Kerberos auth data from krbsso.py')
+    intauth_parser.add_argument('--estscookie',
+                                action='store',
+                                help='ESTSAUTHPERSISTENT cookie from browser')
     intauth_parser.add_argument('-url', '--auth-url', action='store', metavar='URL', help=urlhelp)
     intauth_parser.add_argument('-c',
                                 '--client',
                                 action='store',
                                 help=clienthelptext,
                                 default='1b730954-1685-4b74-9bfd-dac224a7b894')
     intauth_parser.add_argument('-r',
@@ -434,14 +437,15 @@
     enrauth_parser.add_argument('-kp', '--keepass', action='store', metavar='KPFILE', default='roadtx.kdbx', help='KeePass file (default: roadtx.kdbx)')
     enrauth_parser.add_argument('-kpp', '--keepass-password', action='store', metavar='KPPASS', help='KeePass file password. Can also be provided via KPPASS environment variable.')
     enrauth_parser.add_argument('-d', '--driver-path',
                                 action='store',
                                 help='Path to geckodriver file on disk (download from: https://github.com/mozilla/geckodriver/releases)',
                                 default='geckodriver')
     enrauth_parser.add_argument('-f', '--prt-file', default="roadtx.prt", action='store', metavar='FILE', help='PRT storage file (default: roadtx.prt)')
+    enrauth_parser.add_argument('--no-prt', action='store_true', help='Perform the flow without a PRT')
     enrauth_parser.add_argument('--prt',
                                 action='store',
                                 help='Primary Refresh Token')
     enrauth_parser.add_argument('--prt-sessionkey',
                                 action='store',
                                 help='Primary Refresh Token session key (as hex key)')
     enrauth_parser.add_argument('--ngcmfa-drs-auth', action='store_true', help="Don't request PRT with MFA claim but get access token with ngcmfa claim for DRS instead.")
@@ -456,14 +460,16 @@
     if len(sys.argv) < 2:
         parser.print_help()
         sys.exit(1)
         return
 
     deviceauth = DeviceAuthentication()
     args = parser.parse_args()
+    seleniumproxy = None
+
     if args.command in ('auth', 'gettokens', 'gettoken'):
         auth.parse_args(args)
         res = auth.get_tokens(args)
         if not res:
             return
         auth.save_tokens(args)
     elif args.command == 'device':
@@ -605,38 +611,40 @@
         print()
         for alias, resourceurl in WELLKNOWN_RESOURCES.items():
             print(f"{alias} - {resourceurl}")
     elif args.command == 'interactiveauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.tenant = args.tenant
-        selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url)
+        selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url, proxy=seleniumproxy)
         if args.auth_url:
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
         service = selauth.get_service(args.driver_path)
         if not service:
             return
         selauth.driver = selauth.get_webdriver(service, intercept=True)
         if args.krbtoken:
             result = selauth.selenium_login_with_kerberos(url, args.username, args.password, capture=args.capture_code, krbdata=args.krbtoken)
+        elif args.estscookie:
+            result = selauth.selenium_login_with_estscookie(url, args.username, args.password, capture=args.capture_code, estscookie=args.estscookie)
         else:
             result = selauth.selenium_login(url, args.username, args.password, capture=args.capture_code)
         if args.capture_code:
             if result:
                 print(f'Captured auth code: {result}')
             return
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'keepassauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.tenant = args.tenant
-        selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url)
+        selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url, proxy=seleniumproxy)
         password, otpseed = selauth.get_keepass_cred(args.username, args.keepass, args.keepass_password)
         if args.auth_url:
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
         service = selauth.get_service(args.driver_path)
         if not service:
@@ -658,15 +666,15 @@
         elif args.prt_cookie:
             pass
         elif args.prt_file and deviceauth.loadprt(args.prt_file):
             pass
         else:
             print('You must either supply a PRT and session key on the command line or a file that contains them')
             return
-        selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url)
+        selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url, proxy=seleniumproxy)
         if args.auth_url:
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
         service = selauth.get_service(args.driver_path)
         if not service:
             return
@@ -711,36 +719,37 @@
             return
         selauth.driver = selauth.get_webdriver(service, intercept=True)
         if not selauth.selenium_login_with_prt(url, identity=args.username, password=password, otpseed=otpseed, keep=args.keep_open):
             return
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'prtenrich':
-        if args.prt and args.prt_sessionkey:
-            deviceauth.setprt(args.prt, args.prt_sessionkey)
-        elif args.prt_file and deviceauth.loadprt(args.prt_file):
-            pass
-        else:
-            print('You must either supply a PRT and session key on the command line or a file that contains them')
-            return
+        if not args.no_prt:
+            if args.prt and args.prt_sessionkey:
+                deviceauth.setprt(args.prt, args.prt_sessionkey)
+            elif args.prt_file and deviceauth.loadprt(args.prt_file):
+                pass
+            else:
+                print('You must either supply a PRT and session key on the command line or a file that contains them')
+                return
         auth.set_client_id('29d9ed98-a469-4536-ade2-f981bc1d605e')
         if args.username:
             hint = '&login_hint=' + quote_plus(args.username)
         else:
             hint = ''
         replyurl = "ms-appx-web://Microsoft.AAD.BrokerPlugin/DRS"
         url = f'https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&client_id=29d9ed98-a469-4536-ade2-f981bc1d605e&redirect_uri=ms-appx-web%3a%2f%2fMicrosoft.AAD.BrokerPlugin%2fDRS&resource=urn%3aaad%3atb%3aupdate%3aprt&add_account=noheadsup&scope=openid{hint}&response_mode=form_post&windows_api_version=2.0&amr_values=ngcmfa'
 
         if args.ngcmfa_drs_auth:
             # Get ngcmfa token for device registration service
             auth.set_client_id('dd762716-544d-4aeb-a526-687b73838a22')
             replyurl = "ms-appx-web://Microsoft.AAD.BrokerPlugin/dd762716-544d-4aeb-a526-687b73838a22"
             url = f'https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&client_id=dd762716-544d-4aeb-a526-687b73838a22&redirect_uri=ms-appx-web%3a%2f%2fMicrosoft.AAD.BrokerPlugin%2fdd762716-544d-4aeb-a526-687b73838a22&resource=urn%3ams-drs%3aenterpriseregistration.windows.net&add_account=noheadsup&scope=openid{hint}&response_mode=form_post&windows_api_version=2.0&amr_values=ngcmfa'
 
-        selauth = SeleniumAuthentication(auth, deviceauth, replyurl)
+        selauth = SeleniumAuthentication(auth, deviceauth, replyurl, proxy=seleniumproxy)
         if args.username and args.keepass and (args.keepass_password or 'KPPASS' in os.environ or args.keepass.endswith('.xml')):
             _, otpseed = selauth.get_keepass_cred(args.username, args.keepass, args.keepass_password)
         else:
             otpseed = None
         service = selauth.get_service(args.driver_path)
         if not service:
             return
```

### Comparing `roadtx-1.3.1/roadtools/roadtx/selenium.py` & `roadtx-1.3.2/roadtools/roadtx/selenium.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import os
 import sys
 from urllib.parse import urlparse, parse_qs, quote_plus
 from roadtools.roadlib.auth import Authentication, AuthenticationException, get_data, WELLKNOWN_CLIENTS, WELLKNOWN_RESOURCES
 from roadtools.roadlib.deviceauth import DeviceAuthentication
 from roadtools.roadtx.keepass import HackyKeePassFileReader
 from seleniumwire import webdriver as webdriver_wire
+from seleniumwire.thirdparty.mitmproxy.net.http import encoding
 from selenium import webdriver
 from selenium.webdriver.firefox.service import Service
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.common.exceptions import TimeoutException
 import pyotp
 
 class SeleniumAuthentication():
     def __init__(self, auth, deviceauth, redirurl, proxy=None):
+        if proxy and proxy.startswith('http'):
+            proxy = proxy.replace('http://','').replace('https://','')
         self.proxy = proxy
         self.auth = auth
         self.deviceauth = deviceauth
         self.driver = None
         self.redirurl = redirurl
 
     def get_service(self, driverpath):
@@ -39,18 +42,19 @@
         '''
         if self.proxy:
             options = {
                 'proxy': {
                     'http': f'http://{self.proxy}',
                     'https': f'https://{self.proxy}',
                     'no_proxy': 'localhost,127.0.0.1'
-                }
+                },
+                'request_storage': 'memory'
             }
         else:
-            options = {}
+            options = {'request_storage': 'memory'}
         if intercept:
             driver = webdriver_wire.Firefox(service=service, seleniumwire_options=options)
         else:
             driver = webdriver.Firefox(service=service)
         return driver
 
     def get_keepass_cred(self, identity, filepath, password):
@@ -189,14 +193,34 @@
 
                     # Force single cookie injection
                     request.headers['Authorization'] = f'Negotiate {krbdata}'
 
         self.driver.request_interceptor = interceptor
         return self.selenium_login(url, identity, password, otpseed, keep=keep, capture=capture)
 
+    def selenium_login_with_estscookie(self, url, identity=None, password=None, otpseed=None, keep=False, capture=False, estscookie=None):
+        '''
+        Selenium login with Kerberos auth header injection.
+        '''
+        def interceptor(request):
+            del request.headers['User-Agent']
+            request.headers['User-Agent'] = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/103.0.5060.134 Safari/537.36 Edg/103.0.1264.71'
+            request.headers['Sec-Ch-Ua'] = '" Not;A Brand";v="99", "Microsoft Edge";v="103", "Chromium";v="103"'
+            request.headers['Sec-Ch-Ua-Mobile'] =  '?0'
+            request.headers['Sec-Ch-Ua-Platform'] =  '"Windows"'
+            request.headers['Sec-Ch-Ua-Platform-Version'] = '"10.0.0"'
+            if request.headers['Cookie']:
+                existing = request.headers['Cookie']
+            else:
+                existing = ''
+            request.headers['Cookie'] = f'ESTSAUTHPERSISTENT={estscookie}; ' + existing
+
+        self.driver.request_interceptor = interceptor
+        return self.selenium_login(url, identity, password, otpseed, keep=keep, capture=capture)
+
     def selenium_enrich_prt(self, url, otpseed=None):
         '''
         Selenium authentication to add NGC MFA claim to a PRT or token.
         Single factor auth is handled via PRT injection, MFA seed can come
         from keepass or manually. Result is refresh token that can be used to request
         a new PRT, or an access token to the desired resource (depends on supplied url).
         '''
@@ -204,27 +228,42 @@
             del request.headers['User-Agent']
             request.headers['User-Agent'] = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; WebView/3.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36 Edge/18.19044'
             request.headers['Sec-Ch-Ua'] = '" Not;A Brand";v="99", "Microsoft Edge";v="103", "Chromium";v="103"'
             request.headers['Sec-Ch-Ua-Mobile'] =  '?0'
             request.headers['Sec-Ch-Ua-Platform'] =  '"Windows"'
             request.headers['Sec-Ch-Ua-Platform-Version'] = '"10.0.0"'
 
-            if request.url.startswith('https://login.microsoftonline.com'):
+            if request.url.startswith('https://login.microsoftonline.com') and self.deviceauth.prt:
                 if '/authorize' in request.url or '/login' in request.url or '/kmsi' in request.url or '/reprocess' in request.url or '/resume' in request.url:
                     if 'sso_nonce' in request.url:
                         res = urlparse(request.url)
                         params = parse_qs(res.query)
                         cookie = self.auth.create_prt_cookie_kdf_ver_2(self.deviceauth.prt,
                                                                        self.deviceauth.session_key,
                                                                        params['sso_nonce'][0])
                     else:
                         cookie = self.auth.create_prt_cookie_kdf_ver_2(self.deviceauth.prt,
                                                                        self.deviceauth.session_key)
                     request.headers['X-Ms-Refreshtokencredential'] = cookie
+
+        def response_interceptor(request, response):
+            '''
+            Intercept response to prevent automatic form submission to a non-handled URL scheme so
+            selenium has time to extract the data
+            '''
+            if request.url.startswith('https://login.microsoftonline.com'):
+                body = encoding.decode(response.body, response.headers.get('Content-Encoding', 'identity'))
+                if b'SwitchToProgressPage();' in body:
+                    body = body.replace(b'SwitchToProgressPage();',b'/*SwitchToProgressPage();*/')
+                    response.body = encoding.encode(body, response.headers.get('Content-Encoding', 'identity'))
+                    del response.headers['Content-Length']
+                    response.headers['Content-Length'] = len(response.body)
+
         self.driver.request_interceptor = interceptor
+        self.driver.response_interceptor = response_interceptor
 
         driver = self.driver
         driver.get(url)
         if otpseed:
             try:
                 els = WebDriverWait(driver, 4).until(lambda d: d.find_element(By.CSS_SELECTOR, '[data-value="PhoneAppOTP"]'))
                 els.click()
```

### Comparing `roadtx-1.3.1/roadtx.egg-info/PKG-INFO` & `roadtx-1.3.2/roadtx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.3.1
+Version: 1.3.2
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.3.1/setup.py` & `roadtx-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='roadtx',
-      version='1.3.1',
+      version='1.3.2',
       description='ROADtools Token eXchange',
       author='Dirk-jan Mollema',
       author_email='dirkjan@outsidersecurity.nl',
       url='https://github.com/dirkjanm/ROADtools/',
       license='MIT',
       classifiers=[
           'Intended Audience :: Information Technology',
```

