# Comparing `tmp/certbot-dns-easydns-0.1.1.tar.gz` & `tmp/certbot-dns-easydns-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-easydns-0.1.1.tar", last modified: Fri Mar  3 19:38:39 2023, max compression
+gzip compressed data, was "certbot-dns-easydns-0.1.2.tar", last modified: Tue Jun 13 18:16:50 2023, max compression
```

## Comparing `certbot-dns-easydns-0.1.1.tar` & `certbot-dns-easydns-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ccullen   (1000) ccullen   (1000)        0 2023-03-03 19:38:39.748560 certbot-dns-easydns-0.1.1/
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)    10801 2023-03-02 20:20:39.000000 certbot-dns-easydns-0.1.1/LICENSE
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     6848 2023-03-03 19:38:39.748560 certbot-dns-easydns-0.1.1/PKG-INFO
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     5216 2023-03-03 19:38:30.000000 certbot-dns-easydns-0.1.1/README.rst
-drwxrwxr-x   0 ccullen   (1000) ccullen   (1000)        0 2023-03-03 19:38:39.748560 certbot-dns-easydns-0.1.1/certbot_dns_easydns/
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       73 2023-03-02 20:56:27.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns/__init__.py
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       22 2023-03-03 19:30:52.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns/_version.py
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     3885 2023-03-03 18:29:47.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns/dns_easydns.py
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     2057 2023-03-03 18:29:47.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns/dns_easydns_test.py
-drwxrwxr-x   0 ccullen   (1000) ccullen   (1000)        0 2023-03-03 19:38:39.748560 certbot-dns-easydns-0.1.1/certbot_dns_easydns.egg-info/
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     6848 2023-03-03 19:38:39.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns.egg-info/PKG-INFO
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)      436 2023-03-03 19:38:39.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns.egg-info/SOURCES.txt
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)        1 2023-03-03 19:38:39.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns.egg-info/dependency_links.txt
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       78 2023-03-03 19:38:39.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns.egg-info/entry_points.txt
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       99 2023-03-03 19:38:39.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns.egg-info/requires.txt
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       20 2023-03-03 19:38:39.000000 certbot-dns-easydns-0.1.1/certbot_dns_easydns.egg-info/top_level.txt
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)      379 2023-03-03 19:38:39.748560 certbot-dns-easydns-0.1.1/setup.cfg
--rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     2527 2023-03-03 18:29:47.000000 certbot-dns-easydns-0.1.1/setup.py
+drwxrwxr-x   0 ccullen   (1000) ccullen   (1000)        0 2023-06-13 18:16:50.988572 certbot-dns-easydns-0.1.2/
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)    10801 2023-03-02 20:20:39.000000 certbot-dns-easydns-0.1.2/LICENSE
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     7995 2023-06-13 18:16:50.988572 certbot-dns-easydns-0.1.2/PKG-INFO
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     6363 2023-06-13 18:06:02.000000 certbot-dns-easydns-0.1.2/README.rst
+drwxrwxr-x   0 ccullen   (1000) ccullen   (1000)        0 2023-06-13 18:16:50.988572 certbot-dns-easydns-0.1.2/certbot_dns_easydns/
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       73 2023-03-02 20:56:27.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns/__init__.py
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       22 2023-06-13 18:14:01.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns/_version.py
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     3885 2023-03-03 18:29:47.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns/dns_easydns.py
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     2057 2023-03-03 18:29:47.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns/dns_easydns_test.py
+drwxrwxr-x   0 ccullen   (1000) ccullen   (1000)        0 2023-06-13 18:16:50.988572 certbot-dns-easydns-0.1.2/certbot_dns_easydns.egg-info/
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     7995 2023-06-13 18:16:50.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns.egg-info/PKG-INFO
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)      436 2023-06-13 18:16:50.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns.egg-info/SOURCES.txt
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)        1 2023-06-13 18:16:50.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns.egg-info/dependency_links.txt
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       78 2023-06-13 18:16:50.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns.egg-info/entry_points.txt
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       99 2023-06-13 18:16:50.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns.egg-info/requires.txt
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)       20 2023-06-13 18:16:50.000000 certbot-dns-easydns-0.1.2/certbot_dns_easydns.egg-info/top_level.txt
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)      379 2023-06-13 18:16:50.988572 certbot-dns-easydns-0.1.2/setup.cfg
+-rw-rw-r--   0 ccullen   (1000) ccullen   (1000)     2527 2023-03-03 18:29:47.000000 certbot-dns-easydns-0.1.2/setup.py
```

### Comparing `certbot-dns-easydns-0.1.1/LICENSE` & `certbot-dns-easydns-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `certbot-dns-easydns-0.1.1/PKG-INFO` & `certbot-dns-easydns-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-easydns
-Version: 0.1.1
+Version: 0.1.2
 Summary: EasyDNS Authenticator plugin for Certbot
 Home-page: https://github.com/easydns/certbot-dns-easydns
 Author: Caleb S. Cullen
 Author-email: certbot-dev@easydns.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/easydns/certbot-dns-easydns/issues
 Project-URL: Documentation, https://github.com/easydns/certbot-dns-easydns/
@@ -91,27 +91,48 @@
                                       | (Default: 120, Recommended: >= 600)
 ===================================== ==============================================
 
 
 Credentials
 -----------
 
+Credentials for access to the EasyDNS REST API are required in order
+for this plugin to work.  The credentials are stored in a separate INI
+file which should have mode 0600 for security (see below).  The file
+is often stored in a location such as ``/root/.secrets`` or
+``/etc/letsencrypt/.secrets`` and perhaps named for the authenticator,
+e.g. ``/root/.secrets/easydns.ini``.  Henceforth we shall refer to
+this file as ``credentials.ini``.
+
 An example ``credentials.ini`` file:
 
 .. code-block:: ini
 
    dns_easydns_usertoken = myremoteuser
    dns_easydns_userkey = verysecureremoteuserpassword
    dns_easydns_endpoint = https://rest.easydns.net
 
 
-The path to this file can be provided interactively or using the
-``--certbot-dns-easydns:dns-easydns-credentials`` command-line
-argument. Certbot records the path to this file for use during
-renewal, but does not store the file's contents.
+The full path to this file can be provided interactively or by using
+the ``--dns-easydns-credentials`` command-line argument; that value
+appears in the ``domain.conf`` which Certbot creates to describe the
+domain which is the subject of the cert.  Certbot records the absolute
+path to this file for use during renewal, but does not store the
+file's contents.
+
+The ``domain.conf`` file is created by ``certbot`` if it is not
+present, when the SSL cert is first provisioned by running the
+``certbot certonly`` command (example below).  If the
+``--dns-easydns-credentials`` option is used, the resulting
+``domain.conf`` file should reflect the location provided without any
+need for editing by the user.  However, if the credentials file
+changes locations, then the ``domain.conf`` file will need to be
+updated to reflect the new location.  It is worthy of note that in the
+``domain.conf`` file, the parameter uses underscores in place of
+hyphens.
 
 .. note::
 
    Please note that providing the endpoint is required, though it is
    currently always the same; this is for forward compatibility.
 
 .. caution::
```

### Comparing `certbot-dns-easydns-0.1.1/README.rst` & `certbot-dns-easydns-0.1.2/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -54,27 +54,48 @@
                                       | (Default: 120, Recommended: >= 600)
 ===================================== ==============================================
 
 
 Credentials
 -----------
 
+Credentials for access to the EasyDNS REST API are required in order
+for this plugin to work.  The credentials are stored in a separate INI
+file which should have mode 0600 for security (see below).  The file
+is often stored in a location such as ``/root/.secrets`` or
+``/etc/letsencrypt/.secrets`` and perhaps named for the authenticator,
+e.g. ``/root/.secrets/easydns.ini``.  Henceforth we shall refer to
+this file as ``credentials.ini``.
+
 An example ``credentials.ini`` file:
 
 .. code-block:: ini
 
    dns_easydns_usertoken = myremoteuser
    dns_easydns_userkey = verysecureremoteuserpassword
    dns_easydns_endpoint = https://rest.easydns.net
 
 
-The path to this file can be provided interactively or using the
-``--certbot-dns-easydns:dns-easydns-credentials`` command-line
-argument. Certbot records the path to this file for use during
-renewal, but does not store the file's contents.
+The full path to this file can be provided interactively or by using
+the ``--dns-easydns-credentials`` command-line argument; that value
+appears in the ``domain.conf`` which Certbot creates to describe the
+domain which is the subject of the cert.  Certbot records the absolute
+path to this file for use during renewal, but does not store the
+file's contents.
+
+The ``domain.conf`` file is created by ``certbot`` if it is not
+present, when the SSL cert is first provisioned by running the
+``certbot certonly`` command (example below).  If the
+``--dns-easydns-credentials`` option is used, the resulting
+``domain.conf`` file should reflect the location provided without any
+need for editing by the user.  However, if the credentials file
+changes locations, then the ``domain.conf`` file will need to be
+updated to reflect the new location.  It is worthy of note that in the
+``domain.conf`` file, the parameter uses underscores in place of
+hyphens.
 
 .. note::
 
    Please note that providing the endpoint is required, though it is
    currently always the same; this is for forward compatibility.
 
 .. caution::
```

### Comparing `certbot-dns-easydns-0.1.1/certbot_dns_easydns/dns_easydns.py` & `certbot-dns-easydns-0.1.2/certbot_dns_easydns/dns_easydns.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-easydns-0.1.1/certbot_dns_easydns/dns_easydns_test.py` & `certbot-dns-easydns-0.1.2/certbot_dns_easydns/dns_easydns_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-easydns-0.1.1/certbot_dns_easydns.egg-info/PKG-INFO` & `certbot-dns-easydns-0.1.2/certbot_dns_easydns.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-easydns
-Version: 0.1.1
+Version: 0.1.2
 Summary: EasyDNS Authenticator plugin for Certbot
 Home-page: https://github.com/easydns/certbot-dns-easydns
 Author: Caleb S. Cullen
 Author-email: certbot-dev@easydns.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/easydns/certbot-dns-easydns/issues
 Project-URL: Documentation, https://github.com/easydns/certbot-dns-easydns/
@@ -91,27 +91,48 @@
                                       | (Default: 120, Recommended: >= 600)
 ===================================== ==============================================
 
 
 Credentials
 -----------
 
+Credentials for access to the EasyDNS REST API are required in order
+for this plugin to work.  The credentials are stored in a separate INI
+file which should have mode 0600 for security (see below).  The file
+is often stored in a location such as ``/root/.secrets`` or
+``/etc/letsencrypt/.secrets`` and perhaps named for the authenticator,
+e.g. ``/root/.secrets/easydns.ini``.  Henceforth we shall refer to
+this file as ``credentials.ini``.
+
 An example ``credentials.ini`` file:
 
 .. code-block:: ini
 
    dns_easydns_usertoken = myremoteuser
    dns_easydns_userkey = verysecureremoteuserpassword
    dns_easydns_endpoint = https://rest.easydns.net
 
 
-The path to this file can be provided interactively or using the
-``--certbot-dns-easydns:dns-easydns-credentials`` command-line
-argument. Certbot records the path to this file for use during
-renewal, but does not store the file's contents.
+The full path to this file can be provided interactively or by using
+the ``--dns-easydns-credentials`` command-line argument; that value
+appears in the ``domain.conf`` which Certbot creates to describe the
+domain which is the subject of the cert.  Certbot records the absolute
+path to this file for use during renewal, but does not store the
+file's contents.
+
+The ``domain.conf`` file is created by ``certbot`` if it is not
+present, when the SSL cert is first provisioned by running the
+``certbot certonly`` command (example below).  If the
+``--dns-easydns-credentials`` option is used, the resulting
+``domain.conf`` file should reflect the location provided without any
+need for editing by the user.  However, if the credentials file
+changes locations, then the ``domain.conf`` file will need to be
+updated to reflect the new location.  It is worthy of note that in the
+``domain.conf`` file, the parameter uses underscores in place of
+hyphens.
 
 .. note::
 
    Please note that providing the endpoint is required, though it is
    currently always the same; this is for forward compatibility.
 
 .. caution::
```

### Comparing `certbot-dns-easydns-0.1.1/setup.py` & `certbot-dns-easydns-0.1.2/setup.py`

 * *Files identical despite different names*

