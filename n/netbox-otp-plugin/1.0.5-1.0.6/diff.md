# Comparing `tmp/netbox_otp_plugin-1.0.5-py3-none-any.whl.zip` & `tmp/netbox_otp_plugin-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7326 bytes, number of entries: 12
--rw-rw-r--  2.0 unx     1338 b- defN 23-Jan-09 19:35 netbox_otp_plugin/__init__.py
--rw-rw-r--  2.0 unx     1075 b- defN 23-Apr-13 16:38 netbox_otp_plugin/forms.py
--rw-rw-r--  2.0 unx      453 b- defN 23-Jan-10 18:38 netbox_otp_plugin/middleware.py
--rw-rw-r--  2.0 unx      141 b- defN 23-Apr-13 16:38 netbox_otp_plugin/urls.py
--rw-rw-r--  2.0 unx     4417 b- defN 23-Apr-13 16:38 netbox_otp_plugin/views.py
--rw-rw-r--  2.0 unx      880 b- defN 22-Dec-22 08:06 netbox_otp_plugin/management/commands/addtotp.py
--rw-rw-r--  2.0 unx      831 b- defN 23-Jan-10 18:38 netbox_otp_plugin/management/commands/resettotp.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Apr-13 16:38 netbox_otp_plugin/templates/otp_login.html
--rw-rw-r--  2.0 unx      312 b- defN 23-Apr-13 16:50 netbox_otp_plugin-1.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-13 16:50 netbox_otp_plugin-1.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Apr-13 16:50 netbox_otp_plugin-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-13 16:50 netbox_otp_plugin-1.0.5.dist-info/RECORD
-12 files, 13057 bytes uncompressed, 5502 bytes compressed:  57.9%
+Zip file size: 7372 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx     1456 b- defN 23-Jun-13 05:28 netbox_otp_plugin/__init__.py
+-rw-rw-r--  2.0 unx     1075 b- defN 23-May-29 18:20 netbox_otp_plugin/forms.py
+-rw-rw-r--  2.0 unx      453 b- defN 23-Jun-12 06:53 netbox_otp_plugin/middleware.py
+-rw-rw-r--  2.0 unx      141 b- defN 23-May-29 18:20 netbox_otp_plugin/urls.py
+-rw-rw-r--  2.0 unx     4417 b- defN 23-May-29 18:20 netbox_otp_plugin/views.py
+-rw-rw-r--  2.0 unx      880 b- defN 23-May-29 18:20 netbox_otp_plugin/management/commands/addtotp.py
+-rw-rw-r--  2.0 unx      831 b- defN 23-May-29 18:20 netbox_otp_plugin/management/commands/resettotp.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-May-29 18:20 netbox_otp_plugin/templates/otp_login.html
+-rw-rw-r--  2.0 unx      312 b- defN 23-Jun-13 10:35 netbox_otp_plugin-1.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 10:35 netbox_otp_plugin-1.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jun-13 10:35 netbox_otp_plugin-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-13 10:35 netbox_otp_plugin-1.0.6.dist-info/RECORD
+12 files, 13175 bytes uncompressed, 5548 bytes compressed:  57.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: netbox_otp_plugin/management/commands/resettotp.py
 Comment: 
 
 Filename: netbox_otp_plugin/templates/otp_login.html
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.5.dist-info/METADATA
+Filename: netbox_otp_plugin-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.5.dist-info/WHEEL
+Filename: netbox_otp_plugin-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.5.dist-info/top_level.txt
+Filename: netbox_otp_plugin-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.5.dist-info/RECORD
+Filename: netbox_otp_plugin-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netbox_otp_plugin/__init__.py

```diff
@@ -7,20 +7,21 @@
 if importlib.util.find_spec('django_otp') is None:
     raise ImproperlyConfigured(
         f"netbox_otp_plugin is enabled but django_otp is not present. It can be "
         f"installed by running 'pip install django_otp qrcode'." 
     )
 
 netbox_settings.INSTALLED_APPS.extend(['django_otp','django_otp.plugins.otp_totp'])
+netbox_settings.AUTH_EXEMPT_PATHS = netbox_settings.AUTH_EXEMPT_PATHS + (f'/{netbox_settings.BASE_PATH}plugins/otp',)
 
 class OTPPluginConfig(PluginConfig):
     name = 'netbox_otp_plugin'
     verbose_name = 'OTP Login'
     description = 'OTP Login plugin'
-    version = '1.0.4'
+    version = '1.0.6'
     author = 'Andrey Shalashov'
     author_email = 'avshalashov@yandex.ru'
     base_url = 'otp'
     required_settings = []
     default_settings = {
         'otp_required': True,
         'issuer': 'Netbox'
```

## Comparing `netbox_otp_plugin-1.0.5.dist-info/RECORD` & `netbox_otp_plugin-1.0.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-netbox_otp_plugin/__init__.py,sha256=RCdH7RiQDf-vmQMPicjCEB-XKetM6zGv17QR9KtkeVg,1338
+netbox_otp_plugin/__init__.py,sha256=VWQkYAJJNFvXzhXXH24xfcdTgEihSxnZyiKnx6jTd1k,1456
 netbox_otp_plugin/forms.py,sha256=dbQkE1P8Q8zsHPWs46QxJxKlIyUZilR2_6swMxdqoxE,1075
 netbox_otp_plugin/middleware.py,sha256=Pja6J7oTsIpY96MsF_VG2P742GRsC9NWkg7R2ySDDlw,453
 netbox_otp_plugin/urls.py,sha256=Y9px4QUdp6URAa6gzwckIAGVkvMleLy6Bihtxfbszyc,141
 netbox_otp_plugin/views.py,sha256=zrDaMQyv3YCoEiF6igzgtgQu3QvvNEx2VbTZ6Hz7i1A,4417
 netbox_otp_plugin/management/commands/addtotp.py,sha256=45ydKm7XtDhBnFOh1x2qRZzCAexYNQxHQKsdOZapIys,880
 netbox_otp_plugin/management/commands/resettotp.py,sha256=zuQVQwsTVDcumDFoolOkVcPinZ9kwwTy4zUXBnqp_Lg,831
 netbox_otp_plugin/templates/otp_login.html,sha256=Qjkx2tL_UjPvU00ynlD7WpJF0iQoUTn-Chl8iFaNHjM,2434
-netbox_otp_plugin-1.0.5.dist-info/METADATA,sha256=HbU_9P208p0IdX1HmclzkySKcFEOp4vbDfv0OBwkNLc,312
-netbox_otp_plugin-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-netbox_otp_plugin-1.0.5.dist-info/top_level.txt,sha256=T322x6_TOk3lbaU-efVeIjMvWZQ5QiqFTFIeGhX8JlE,18
-netbox_otp_plugin-1.0.5.dist-info/RECORD,,
+netbox_otp_plugin-1.0.6.dist-info/METADATA,sha256=610EVA-DUY3nnhYzl9cMeMKaf9Xgrr-np3D6qByqAAo,312
+netbox_otp_plugin-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+netbox_otp_plugin-1.0.6.dist-info/top_level.txt,sha256=T322x6_TOk3lbaU-efVeIjMvWZQ5QiqFTFIeGhX8JlE,18
+netbox_otp_plugin-1.0.6.dist-info/RECORD,,
```

