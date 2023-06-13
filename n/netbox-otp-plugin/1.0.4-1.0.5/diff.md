# Comparing `tmp/netbox_otp_plugin-1.0.4-py3-none-any.whl.zip` & `tmp/netbox_otp_plugin-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5858 bytes, number of entries: 12
+Zip file size: 7326 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx     1338 b- defN 23-Jan-09 19:35 netbox_otp_plugin/__init__.py
--rw-rw-r--  2.0 unx     1036 b- defN 22-Dec-26 19:18 netbox_otp_plugin/forms.py
+-rw-rw-r--  2.0 unx     1075 b- defN 23-Apr-13 16:38 netbox_otp_plugin/forms.py
 -rw-rw-r--  2.0 unx      453 b- defN 23-Jan-10 18:38 netbox_otp_plugin/middleware.py
--rw-rw-r--  2.0 unx      222 b- defN 22-Dec-22 08:06 netbox_otp_plugin/urls.py
--rw-rw-r--  2.0 unx      117 b- defN 22-Dec-22 08:06 netbox_otp_plugin/views.py
+-rw-rw-r--  2.0 unx      141 b- defN 23-Apr-13 16:38 netbox_otp_plugin/urls.py
+-rw-rw-r--  2.0 unx     4417 b- defN 23-Apr-13 16:38 netbox_otp_plugin/views.py
 -rw-rw-r--  2.0 unx      880 b- defN 22-Dec-22 08:06 netbox_otp_plugin/management/commands/addtotp.py
 -rw-rw-r--  2.0 unx      831 b- defN 23-Jan-10 18:38 netbox_otp_plugin/management/commands/resettotp.py
--rw-rw-r--  2.0 unx     2054 b- defN 22-Dec-22 08:06 netbox_otp_plugin/templates/otp_login.html
--rw-rw-r--  2.0 unx      312 b- defN 23-Jan-10 18:42 netbox_otp_plugin-1.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-10 18:42 netbox_otp_plugin-1.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Jan-10 18:42 netbox_otp_plugin-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1065 b- defN 23-Jan-10 18:42 netbox_otp_plugin-1.0.4.dist-info/RECORD
-12 files, 8418 bytes uncompressed, 4034 bytes compressed:  52.1%
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Apr-13 16:38 netbox_otp_plugin/templates/otp_login.html
+-rw-rw-r--  2.0 unx      312 b- defN 23-Apr-13 16:50 netbox_otp_plugin-1.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-13 16:50 netbox_otp_plugin-1.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-13 16:50 netbox_otp_plugin-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-13 16:50 netbox_otp_plugin-1.0.5.dist-info/RECORD
+12 files, 13057 bytes uncompressed, 5502 bytes compressed:  57.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: netbox_otp_plugin/management/commands/resettotp.py
 Comment: 
 
 Filename: netbox_otp_plugin/templates/otp_login.html
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.4.dist-info/METADATA
+Filename: netbox_otp_plugin-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.4.dist-info/WHEEL
+Filename: netbox_otp_plugin-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.4.dist-info/top_level.txt
+Filename: netbox_otp_plugin-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.4.dist-info/RECORD
+Filename: netbox_otp_plugin-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netbox_otp_plugin/forms.py

```diff
@@ -3,15 +3,15 @@
 from django.contrib.auth.forms import AuthenticationForm
 from django_otp.forms import OTPAuthenticationFormMixin
 from django_otp import user_has_device
 from utilities.forms import BootstrapMixin
 
 class OTPAuthenticationForm(OTPAuthenticationFormMixin, AuthenticationForm):
     otp_device = forms.CharField(required=False, widget=forms.Select)
-    otp_token = forms.CharField(required=False, widget=forms.TextInput(attrs={'autocomplete': 'off'}))
+    otp_token = forms.CharField(required=False, widget=forms.TextInput(attrs={'autocomplete': 'off', 'class': 'rounded'}), label="OTP Token")
     otp_challenge = forms.CharField(required=False)
 
     def clean(self):
         self.cleaned_data = super().clean()
         user = self.get_user()
         # use get_plugin_config from extras.plugins better
         plugin_config = settings.PLUGINS_CONFIG['netbox_otp_plugin']
```

## netbox_otp_plugin/urls.py

```diff
@@ -1,9 +1,8 @@
 from django.urls import path
-from netbox_otp_plugin.forms import OTPLoginForm
 
 from . import views
 
 app_name = 'otp'
 urlpatterns = [
-    path('', views.OTPLoginView.as_view(authentication_form=OTPLoginForm), name='otp')
+    path('', views.OTPLoginView.as_view(), name='otp')
 ]
```

## netbox_otp_plugin/views.py

```diff
@@ -1,4 +1,110 @@
+import logging
+
 from django.contrib.auth.views import LoginView
+from django.contrib.auth import login as auth_login
+from django.utils.http import url_has_allowed_host_and_scheme, urlencode
+from django.urls import reverse
+from django.conf import settings
+from social_core.backends.utils import load_backends
+from django.shortcuts import render
+from django.contrib.auth.models import update_last_login
+from django.contrib.auth.signals import user_logged_in
+from django.contrib import messages
+from django.http import HttpResponseRedirect
+
+from netbox.authentication import get_auth_backend_display, get_saml_idps
+from netbox.config import get_config
+from users.models import  UserConfig
+
+from netbox_otp_plugin.forms import OTPLoginForm
 
 class OTPLoginView(LoginView):
     template_name = 'otp_login.html'
+    authentication_form = OTPLoginForm
+
+    def gen_auth_data(self, name, url, params):
+        display_name, icon_name = get_auth_backend_display(name)
+        return {
+            'display_name': display_name,
+            'icon_name': icon_name,
+            'url': f'{url}?{urlencode(params)}',
+        }
+
+    def get_auth_backends(self, request):
+        auth_backends = []
+        saml_idps = get_saml_idps()
+
+        for name in load_backends(settings.AUTHENTICATION_BACKENDS).keys():
+            url = reverse('social:begin', args=[name])
+            params = {}
+            if next := request.GET.get('next'):
+                params['next'] = next
+            if name.lower() == 'saml' and saml_idps:
+                for idp in saml_idps:
+                    params['idp'] = idp
+                    data = self.gen_auth_data(name, url, params)
+                    data['display_name'] = f'{data["display_name"]} ({idp})'
+                    auth_backends.append(data)
+            else:
+                auth_backends.append(self.gen_auth_data(name, url, params))
+
+        return auth_backends
+
+    def get(self, request):
+        form = self.authentication_form(request)
+
+        if request.user.is_authenticated:
+            logger = logging.getLogger('netbox.auth.login')
+            return self.redirect_to_next(request, logger)
+
+        return render(request, self.template_name, {
+            'form': form,
+            'auth_backends': self.get_auth_backends(request),
+        })
+
+    def post(self, request):
+        logger = logging.getLogger('netbox.auth.login')
+        form = self.authentication_form(request, data=request.POST)
+
+        if form.is_valid():
+            logger.debug("Login form validation was successful")
+
+            # If maintenance mode is enabled, assume the database is read-only, and disable updating the user's
+            # last_login time upon authentication.
+            if get_config().MAINTENANCE_MODE:
+                logger.warning("Maintenance mode enabled: disabling update of most recent login time")
+                user_logged_in.disconnect(update_last_login, dispatch_uid='update_last_login')
+
+            # Authenticate user
+            auth_login(request, form.get_user())
+            logger.info(f"User {request.user} successfully authenticated")
+            messages.info(request, f"Logged in as {request.user}.")
+
+            # Ensure the user has a UserConfig defined. (This should normally be handled by
+            # create_userconfig() on user creation.)
+            if not hasattr(request.user, 'config'):
+                config = get_config()
+                UserConfig(user=request.user, data=config.DEFAULT_USER_PREFERENCES).save()
+
+            return self.redirect_to_next(request, logger)
+
+        else:
+            logger.debug(f"Login form validation failed for username: {form['username'].value()}")
+
+        return render(request, self.template_name, {
+            'form': form,
+            'auth_backends': self.get_auth_backends(request),
+        })
+
+    def redirect_to_next(self, request, logger):
+        data = request.POST if request.method == "POST" else request.GET
+        redirect_url = data.get('next', settings.LOGIN_REDIRECT_URL)
+
+        if redirect_url and url_has_allowed_host_and_scheme(redirect_url, allowed_hosts=None):
+            logger.debug(f"Redirecting user to {redirect_url}")
+        else:
+            if redirect_url:
+                logger.warning(f"Ignoring unsafe 'next' URL passed to login form: {redirect_url}")
+            redirect_url = reverse('home')
+
+        return HttpResponseRedirect(redirect_url)
```

## netbox_otp_plugin/templates/otp_login.html

```diff
@@ -83,47 +83,71 @@
 00000520: 653d 2273 7562 6d69 7422 2063 6c61 7373  e="submit" class
 00000530: 3d22 6274 6e20 6274 6e2d 7072 696d 6172  ="btn btn-primar
 00000540: 7920 6274 6e2d 6c67 2077 2d31 3030 206d  y btn-lg w-100 m
 00000550: 742d 3422 3e0a 2020 2020 2020 2020 2020  t-4">.          
 00000560: 5369 676e 2049 6e0a 2020 2020 2020 2020  Sign In.        
 00000570: 3c2f 6275 7474 6f6e 3e0a 2020 2020 2020  </button>.      
 00000580: 3c2f 666f 726d 3e0a 2020 2020 3c2f 6469  </form>.    </di
-00000590: 763e 0a0a 2020 3c2f 6d61 696e 3e0a 0a20  v>..  </main>.. 
-000005a0: 207b 2320 5061 6765 2066 6f6f 7465 7220   {# Page footer 
-000005b0: 237d 0a20 203c 666f 6f74 6572 2063 6c61  #}.  <footer cla
-000005c0: 7373 3d22 666f 6f74 6572 2063 6f6e 7461  ss="footer conta
-000005d0: 696e 6572 2d66 6c75 6964 206c 6f67 696e  iner-fluid login
-000005e0: 2d66 6f6f 7465 7220 702d 3322 3e0a 2020  -footer p-3">.  
-000005f0: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
-00000600: 7720 616c 6967 6e2d 6974 656d 732d 6365  w align-items-ce
-00000610: 6e74 6572 2077 2d31 3030 223e 0a20 2020  nter w-100">.   
-00000620: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-00000630: 6f6c 2d32 2063 6f6c 2d6d 642d 3120 6d62  ol-2 col-md-1 mb
-00000640: 2d30 223e 0a20 2020 2020 2020 203c 6275  -0">.        <bu
-00000650: 7474 6f6e 2074 7970 653d 2262 7574 746f  tton type="butto
-00000660: 6e22 2063 6c61 7373 3d22 6274 6e20 6274  n" class="btn bt
-00000670: 6e2d 736d 2063 6f6c 6f72 2d6d 6f64 652d  n-sm color-mode-
-00000680: 746f 6767 6c65 2220 7469 746c 653d 2254  toggle" title="T
-00000690: 6f67 676c 6520 436f 6c6f 7220 4d6f 6465  oggle Color Mode
-000006a0: 223e 0a20 2020 2020 2020 2020 203c 6920  ">.          <i 
-000006b0: 636c 6173 733d 2263 6f6c 6f72 2d6d 6f64  class="color-mod
-000006c0: 652d 6963 6f6e 206d 6469 206d 6469 2d6c  e-icon mdi mdi-l
-000006d0: 6967 6874 6275 6c62 223e 3c2f 693e 266e  ightbulb"></i>&n
-000006e0: 6273 703b 0a20 2020 2020 2020 203c 2f62  bsp;.        </b
-000006f0: 7574 746f 6e3e 0a20 2020 2020 203c 2f64  utton>.      </d
-00000700: 6976 3e0a 2020 2020 2020 3c64 6976 2063  iv>.      <div c
-00000710: 6c61 7373 3d22 636f 6c2d 3120 636f 6c2d  lass="col-1 col-
-00000720: 6d64 2d61 7574 6f20 6d62 2d30 223e 3c2f  md-auto mb-0"></
-00000730: 6469 763e 0a20 2020 2020 203c 6469 7620  div>.      <div 
-00000740: 636c 6173 733d 2263 6f6c 2074 6578 742d  class="col text-
-00000750: 656e 6420 6d62 2d30 223e 0a20 2020 2020  end mb-0">.     
-00000760: 2020 203c 736d 616c 6c20 636c 6173 733d     <small class=
-00000770: 2274 6578 742d 6d75 7465 6422 3e0a 2020  "text-muted">.  
-00000780: 2020 2020 2020 2020 7b7b 2073 6574 7469          {{ setti
-00000790: 6e67 732e 484f 5354 4e41 4d45 207d 7d20  ngs.HOSTNAME }} 
-000007a0: 2876 7b7b 2073 6574 7469 6e67 732e 5645  (v{{ settings.VE
-000007b0: 5253 494f 4e20 7d7d 290a 2020 2020 2020  RSION }}).      
-000007c0: 2020 3c2f 736d 616c 6c3e 0a20 2020 2020    </small>.     
-000007d0: 203c 2f64 6976 3e0a 2020 2020 3c2f 6469   </div>.    </di
-000007e0: 763e 0a20 203c 2f66 6f6f 7465 723e 0a0a  v>.  </footer>..
-000007f0: 7b25 2065 6e64 626c 6f63 6b20 6c61 796f  {% endblock layo
-00000800: 7574 2025 7d0a                           ut %}.
+00000590: 763e 0a20 2020 207b 2520 6966 2061 7574  v>.    {% if aut
+000005a0: 685f 6261 636b 656e 6473 2025 7d0a 2020  h_backends %}.  
+000005b0: 2020 2020 3c68 3620 636c 6173 733d 226d      <h6 class="m
+000005c0: 742d 3420 6d62 2d33 223e 4f72 2075 7365  t-4 mb-3">Or use
+000005d0: 2061 2073 696e 676c 6520 7369 676e 2d6f   a single sign-o
+000005e0: 6e20 2853 534f 2920 7072 6f76 6964 6572  n (SSO) provider
+000005f0: 3a3c 2f68 363e 0a20 2020 2020 207b 2520  :</h6>.      {% 
+00000600: 666f 7220 6261 636b 656e 6420 696e 2061  for backend in a
+00000610: 7574 685f 6261 636b 656e 6473 2025 7d0a  uth_backends %}.
+00000620: 2020 2020 2020 2020 3c68 353e 0a20 2020          <h5>.   
+00000630: 2020 2020 2020 207b 2520 6966 2062 6163         {% if bac
+00000640: 6b65 6e64 2e69 636f 6e5f 6e61 6d65 2025  kend.icon_name %
+00000650: 7d3c 6920 636c 6173 733d 226d 6469 206d  }<i class="mdi m
+00000660: 6469 2d7b 7b20 6261 636b 656e 642e 6963  di-{{ backend.ic
+00000670: 6f6e 5f6e 616d 6520 7d7d 223e 3c2f 693e  on_name }}"></i>
+00000680: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000690: 2020 2020 2020 3c61 2068 7265 663d 227b        <a href="{
+000006a0: 7b20 6261 636b 656e 642e 7572 6c20 7d7d  { backend.url }}
+000006b0: 2220 636c 6173 733d 226d 792d 3222 3e7b  " class="my-2">{
+000006c0: 7b20 6261 636b 656e 642e 6469 7370 6c61  { backend.displa
+000006d0: 795f 6e61 6d65 207d 7d3c 2f61 3e0a 2020  y_name }}</a>.  
+000006e0: 2020 2020 2020 3c2f 6835 3e0a 2020 2020        </h5>.    
+000006f0: 2020 7b25 2065 6e64 666f 7220 257d 0a20    {% endfor %}. 
+00000700: 2020 207b 2520 656e 6469 6620 257d 0a0a     {% endif %}..
+00000710: 2020 3c2f 6d61 696e 3e0a 0a20 207b 2320    </main>..  {# 
+00000720: 5061 6765 2066 6f6f 7465 7220 237d 0a20  Page footer #}. 
+00000730: 203c 666f 6f74 6572 2063 6c61 7373 3d22   <footer class="
+00000740: 666f 6f74 6572 2063 6f6e 7461 696e 6572  footer container
+00000750: 2d66 6c75 6964 206c 6f67 696e 2d66 6f6f  -fluid login-foo
+00000760: 7465 7220 702d 3322 3e0a 2020 2020 3c64  ter p-3">.    <d
+00000770: 6976 2063 6c61 7373 3d22 726f 7720 616c  iv class="row al
+00000780: 6967 6e2d 6974 656d 732d 6365 6e74 6572  ign-items-center
+00000790: 2077 2d31 3030 223e 0a20 2020 2020 203c   w-100">.      <
+000007a0: 6469 7620 636c 6173 733d 2263 6f6c 2d32  div class="col-2
+000007b0: 2063 6f6c 2d6d 642d 3120 6d62 2d30 223e   col-md-1 mb-0">
+000007c0: 0a20 2020 2020 2020 203c 6275 7474 6f6e  .        <button
+000007d0: 2074 7970 653d 2262 7574 746f 6e22 2063   type="button" c
+000007e0: 6c61 7373 3d22 6274 6e20 6274 6e2d 736d  lass="btn btn-sm
+000007f0: 2063 6f6c 6f72 2d6d 6f64 652d 746f 6767   color-mode-togg
+00000800: 6c65 2220 7469 746c 653d 2254 6f67 676c  le" title="Toggl
+00000810: 6520 436f 6c6f 7220 4d6f 6465 223e 0a20  e Color Mode">. 
+00000820: 2020 2020 2020 2020 203c 6920 636c 6173           <i clas
+00000830: 733d 2263 6f6c 6f72 2d6d 6f64 652d 6963  s="color-mode-ic
+00000840: 6f6e 206d 6469 206d 6469 2d6c 6967 6874  on mdi mdi-light
+00000850: 6275 6c62 223e 3c2f 693e 266e 6273 703b  bulb"></i>&nbsp;
+00000860: 0a20 2020 2020 2020 203c 2f62 7574 746f  .        </butto
+00000870: 6e3e 0a20 2020 2020 203c 2f64 6976 3e0a  n>.      </div>.
+00000880: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000890: 3d22 636f 6c2d 3120 636f 6c2d 6d64 2d61  ="col-1 col-md-a
+000008a0: 7574 6f20 6d62 2d30 223e 3c2f 6469 763e  uto mb-0"></div>
+000008b0: 0a20 2020 2020 203c 6469 7620 636c 6173  .      <div clas
+000008c0: 733d 2263 6f6c 2074 6578 742d 656e 6420  s="col text-end 
+000008d0: 6d62 2d30 223e 0a20 2020 2020 2020 203c  mb-0">.        <
+000008e0: 736d 616c 6c20 636c 6173 733d 2274 6578  small class="tex
+000008f0: 742d 6d75 7465 6422 3e0a 2020 2020 2020  t-muted">.      
+00000900: 2020 2020 7b7b 2073 6574 7469 6e67 732e      {{ settings.
+00000910: 484f 5354 4e41 4d45 207d 7d20 2876 7b7b  HOSTNAME }} (v{{
+00000920: 2073 6574 7469 6e67 732e 5645 5253 494f   settings.VERSIO
+00000930: 4e20 7d7d 290a 2020 2020 2020 2020 3c2f  N }}).        </
+00000940: 736d 616c 6c3e 0a20 2020 2020 203c 2f64  small>.      </d
+00000950: 6976 3e0a 2020 2020 3c2f 6469 763e 0a20  iv>.    </div>. 
+00000960: 203c 2f66 6f6f 7465 723e 0a0a 7b25 2065   </footer>..{% e
+00000970: 6e64 626c 6f63 6b20 6c61 796f 7574 2025  ndblock layout %
+00000980: 7d0a                                     }.
```

## Comparing `netbox_otp_plugin-1.0.4.dist-info/RECORD` & `netbox_otp_plugin-1.0.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 netbox_otp_plugin/__init__.py,sha256=RCdH7RiQDf-vmQMPicjCEB-XKetM6zGv17QR9KtkeVg,1338
-netbox_otp_plugin/forms.py,sha256=C1mpg9Glk-5XM_6I2VfTlDGBwq75eYOMEJm8Skiv0NE,1036
+netbox_otp_plugin/forms.py,sha256=dbQkE1P8Q8zsHPWs46QxJxKlIyUZilR2_6swMxdqoxE,1075
 netbox_otp_plugin/middleware.py,sha256=Pja6J7oTsIpY96MsF_VG2P742GRsC9NWkg7R2ySDDlw,453
-netbox_otp_plugin/urls.py,sha256=zu36IZWT2rtYu7euIiWADdpfkLrryP_SXVY215sCwjY,222
-netbox_otp_plugin/views.py,sha256=FKlXg9dObLANFbpUn6raCB8MtOCsLYN5RLKmLfWxnV8,117
+netbox_otp_plugin/urls.py,sha256=Y9px4QUdp6URAa6gzwckIAGVkvMleLy6Bihtxfbszyc,141
+netbox_otp_plugin/views.py,sha256=zrDaMQyv3YCoEiF6igzgtgQu3QvvNEx2VbTZ6Hz7i1A,4417
 netbox_otp_plugin/management/commands/addtotp.py,sha256=45ydKm7XtDhBnFOh1x2qRZzCAexYNQxHQKsdOZapIys,880
 netbox_otp_plugin/management/commands/resettotp.py,sha256=zuQVQwsTVDcumDFoolOkVcPinZ9kwwTy4zUXBnqp_Lg,831
-netbox_otp_plugin/templates/otp_login.html,sha256=3OtKC4LBXlm4DR2-dK-ajnlioF-pbeduwFATlzC2rw0,2054
-netbox_otp_plugin-1.0.4.dist-info/METADATA,sha256=-D0ZCkQe2Pe0QFaRkG6JW1qZAyQJugiw2atgkbOKAq8,312
-netbox_otp_plugin-1.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-netbox_otp_plugin-1.0.4.dist-info/top_level.txt,sha256=T322x6_TOk3lbaU-efVeIjMvWZQ5QiqFTFIeGhX8JlE,18
-netbox_otp_plugin-1.0.4.dist-info/RECORD,,
+netbox_otp_plugin/templates/otp_login.html,sha256=Qjkx2tL_UjPvU00ynlD7WpJF0iQoUTn-Chl8iFaNHjM,2434
+netbox_otp_plugin-1.0.5.dist-info/METADATA,sha256=HbU_9P208p0IdX1HmclzkySKcFEOp4vbDfv0OBwkNLc,312
+netbox_otp_plugin-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+netbox_otp_plugin-1.0.5.dist-info/top_level.txt,sha256=T322x6_TOk3lbaU-efVeIjMvWZQ5QiqFTFIeGhX8JlE,18
+netbox_otp_plugin-1.0.5.dist-info/RECORD,,
```

