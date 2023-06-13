# Comparing `tmp/rns-0.5.4.tar.gz` & `tmp/rns-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rns-0.5.4.tar", last modified: Sat Jun  3 13:54:29 2023, max compression
+gzip compressed data, was "rns-0.5.5.tar", last modified: Tue Jun 13 17:22:49 2023, max compression
```

## Comparing `rns-0.5.4.tar` & `rns-0.5.5.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.426787 rns-0.5.4/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rns-0.5.4/LICENSE
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-06-03 13:54:29.423453 rns-0.5.4/PKG-INFO
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    17959 2023-05-05 09:14:48.000000 rns-0.5.4/README.md
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.410120 rns-0.5.4/RNS/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10926 2023-05-18 23:54:43.000000 rns-0.5.4/RNS/Buffer.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24736 2023-05-18 23:37:50.000000 rns-0.5.4/RNS/Channel.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.410120 rns-0.5.4/RNS/Cryptography/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/AES.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/Ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/Fernet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rns-0.5.4/RNS/Cryptography/HKDF.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/HMAC.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/Hashes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/PKCS7.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/Provider.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/Proxies.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/SHA256.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/SHA512.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/X25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.413453 rns-0.5.4/RNS/Cryptography/aes/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/aes/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/aes/aes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/aes/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.413453 rns-0.5.4/RNS/Cryptography/pure25519/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/pure25519/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/pure25519/_ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/pure25519/basic.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/pure25519/ed25519_oop.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Cryptography/pure25519/eddsa.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rns-0.5.4/RNS/Destination.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24048 2023-05-31 13:38:00.000000 rns-0.5.4/RNS/Identity.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.416787 rns-0.5.4/RNS/Interfaces/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Interfaces/AX25KISSInterface.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.416787 rns-0.5.4/RNS/Interfaces/Android/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rns-0.5.4/RNS/Interfaces/Android/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49037 2023-05-02 15:44:28.000000 rns-0.5.4/RNS/Interfaces/Android/RNodeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rns-0.5.4/RNS/Interfaces/Android/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rns-0.5.4/RNS/Interfaces/Android/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    20327 2023-05-11 17:33:15.000000 rns-0.5.4/RNS/Interfaces/AutoInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rns-0.5.4/RNS/Interfaces/I2PInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Interfaces/Interface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Interfaces/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12932 2023-05-10 13:51:28.000000 rns-0.5.4/RNS/Interfaces/LocalInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Interfaces/PipeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30633 2023-05-02 15:44:01.000000 rns-0.5.4/RNS/Interfaces/RNodeInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Interfaces/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21620 2023-05-04 21:14:01.000000 rns-0.5.4/RNS/Interfaces/TCPInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4206 2023-05-04 21:15:49.000000 rns-0.5.4/RNS/Interfaces/UDPInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rns-0.5.4/RNS/Interfaces/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    53160 2023-06-02 19:22:06.000000 rns-0.5.4/RNS/Link.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    22263 2023-05-18 14:48:32.000000 rns-0.5.4/RNS/Packet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45887 2023-05-10 13:26:58.000000 rns-0.5.4/RNS/Resource.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65220 2023-05-05 08:37:31.000000 rns-0.5.4/RNS/Reticulum.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   129986 2023-05-18 19:32:45.000000 rns-0.5.4/RNS/Transport.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.420120 rns-0.5.4/RNS/Utilities/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Utilities/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    15089 2023-05-31 13:39:02.000000 rns-0.5.4/RNS/Utilities/rncp.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-05-09 18:30:37.000000 rns-0.5.4/RNS/Utilities/rnid.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)   208368 2023-05-31 19:25:17.000000 rns-0.5.4/RNS/Utilities/rnodeconf.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Utilities/rnpath.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/Utilities/rnprobe.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12818 2023-05-02 14:47:11.000000 rns-0.5.4/RNS/Utilities/rnsd.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rns-0.5.4/RNS/Utilities/rnstatus.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rns-0.5.4/RNS/Utilities/rnx.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7088 2023-03-04 17:36:37.000000 rns-0.5.4/RNS/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-06-03 13:52:32.000000 rns-0.5.4/RNS/_version.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.420120 rns-0.5.4/RNS/vendor/
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/__init__.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/configobj.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.423453 rns-0.5.4/RNS/vendor/i2plib/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/i2plib/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/i2plib/__version__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/i2plib/aiosam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/i2plib/exceptions.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/i2plib/log.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/i2plib/sam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/i2plib/tunnel.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/i2plib/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.423453 rns-0.5.4/RNS/vendor/ifaddr/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rns-0.5.4/RNS/vendor/ifaddr/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rns-0.5.4/RNS/vendor/ifaddr/_posix.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rns-0.5.4/RNS/vendor/ifaddr/_shared.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rns-0.5.4/RNS/vendor/ifaddr/_win32.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rns-0.5.4/RNS/vendor/ifaddr/niwrapper.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rns-0.5.4/RNS/vendor/platformutils.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/six.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rns-0.5.4/RNS/vendor/umsgpack.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-03 13:54:29.423453 rns-0.5.4/rns.egg-info/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-06-03 13:54:29.000000 rns-0.5.4/rns.egg-info/PKG-INFO
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2237 2023-06-03 13:54:29.000000 rns-0.5.4/rns.egg-info/SOURCES.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-06-03 13:54:29.000000 rns-0.5.4/rns.egg-info/dependency_links.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-06-03 13:54:29.000000 rns-0.5.4/rns.egg-info/entry_points.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       34 2023-06-03 13:54:29.000000 rns-0.5.4/rns.egg-info/requires.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-06-03 13:54:29.000000 rns-0.5.4/rns.egg-info/top_level.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-06-03 13:54:29.426787 rns-0.5.4/setup.cfg
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1970 2023-05-04 15:54:21.000000 rns-0.5.4/setup.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.632865 rns-0.5.5/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rns-0.5.5/LICENSE
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-06-13 17:22:49.632865 rns-0.5.5/PKG-INFO
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    17959 2023-05-05 09:14:48.000000 rns-0.5.5/README.md
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.626198 rns-0.5.5/RNS/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10926 2023-05-18 23:54:43.000000 rns-0.5.5/RNS/Buffer.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24736 2023-05-18 23:37:50.000000 rns-0.5.5/RNS/Channel.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.626198 rns-0.5.5/RNS/Cryptography/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/AES.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Fernet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rns-0.5.5/RNS/Cryptography/HKDF.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/HMAC.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Hashes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/PKCS7.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Provider.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Proxies.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/SHA256.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/SHA512.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/X25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.626198 rns-0.5.5/RNS/Cryptography/aes/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/aes/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/aes/aes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/aes/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.626198 rns-0.5.5/RNS/Cryptography/pure25519/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/_ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/basic.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/ed25519_oop.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/eddsa.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rns-0.5.5/RNS/Destination.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24048 2023-05-31 13:38:00.000000 rns-0.5.5/RNS/Identity.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.629532 rns-0.5.5/RNS/Interfaces/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/AX25KISSInterface.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.629532 rns-0.5.5/RNS/Interfaces/Android/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rns-0.5.5/RNS/Interfaces/Android/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49069 2023-06-13 14:11:28.000000 rns-0.5.5/RNS/Interfaces/Android/RNodeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rns-0.5.5/RNS/Interfaces/Android/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rns-0.5.5/RNS/Interfaces/Android/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    20327 2023-05-11 17:33:15.000000 rns-0.5.5/RNS/Interfaces/AutoInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rns-0.5.5/RNS/Interfaces/I2PInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/Interface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12932 2023-05-10 13:51:28.000000 rns-0.5.5/RNS/Interfaces/LocalInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/PipeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30665 2023-06-13 14:11:28.000000 rns-0.5.5/RNS/Interfaces/RNodeInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21620 2023-05-04 21:14:01.000000 rns-0.5.5/RNS/Interfaces/TCPInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4206 2023-05-04 21:15:49.000000 rns-0.5.5/RNS/Interfaces/UDPInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rns-0.5.5/RNS/Interfaces/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    53726 2023-06-13 17:05:12.000000 rns-0.5.5/RNS/Link.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    22263 2023-05-18 14:48:32.000000 rns-0.5.5/RNS/Packet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45887 2023-05-10 13:26:58.000000 rns-0.5.5/RNS/Resource.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65220 2023-05-05 08:37:31.000000 rns-0.5.5/RNS/Reticulum.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   130124 2023-06-13 17:09:12.000000 rns-0.5.5/RNS/Transport.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.629532 rns-0.5.5/RNS/Utilities/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Utilities/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    15089 2023-05-31 13:39:02.000000 rns-0.5.5/RNS/Utilities/rncp.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-05-09 18:30:37.000000 rns-0.5.5/RNS/Utilities/rnid.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)   208368 2023-05-31 19:25:17.000000 rns-0.5.5/RNS/Utilities/rnodeconf.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Utilities/rnpath.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Utilities/rnprobe.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12818 2023-05-02 14:47:11.000000 rns-0.5.5/RNS/Utilities/rnsd.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rns-0.5.5/RNS/Utilities/rnstatus.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rns-0.5.5/RNS/Utilities/rnx.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7088 2023-03-04 17:36:37.000000 rns-0.5.5/RNS/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-06-13 12:55:02.000000 rns-0.5.5/RNS/_version.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.629532 rns-0.5.5/RNS/vendor/
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/__init__.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/configobj.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.632865 rns-0.5.5/RNS/vendor/i2plib/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/__version__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/aiosam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/exceptions.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/log.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/sam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/tunnel.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.632865 rns-0.5.5/RNS/vendor/ifaddr/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rns-0.5.5/RNS/vendor/ifaddr/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rns-0.5.5/RNS/vendor/ifaddr/_posix.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rns-0.5.5/RNS/vendor/ifaddr/_shared.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rns-0.5.5/RNS/vendor/ifaddr/_win32.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rns-0.5.5/RNS/vendor/ifaddr/niwrapper.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rns-0.5.5/RNS/vendor/platformutils.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/six.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/umsgpack.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.632865 rns-0.5.5/rns.egg-info/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/PKG-INFO
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2237 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/SOURCES.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/dependency_links.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/entry_points.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       34 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/requires.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/top_level.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-06-13 17:22:49.632865 rns-0.5.5/setup.cfg
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1970 2023-05-04 15:54:21.000000 rns-0.5.5/setup.py
```

### Comparing `rns-0.5.4/LICENSE` & `rns-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/PKG-INFO` & `rns-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rns
-Version: 0.5.4
+Version: 0.5.5
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rns-0.5.4/README.md` & `rns-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Buffer.py` & `rns-0.5.5/RNS/Buffer.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Channel.py` & `rns-0.5.5/RNS/Channel.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/AES.py` & `rns-0.5.5/RNS/Cryptography/AES.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/Ed25519.py` & `rns-0.5.5/RNS/Cryptography/Ed25519.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/Fernet.py` & `rns-0.5.5/RNS/Cryptography/Fernet.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/HKDF.py` & `rns-0.5.5/RNS/Cryptography/HKDF.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/HMAC.py` & `rns-0.5.5/RNS/Cryptography/HMAC.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/Hashes.py` & `rns-0.5.5/RNS/Cryptography/Hashes.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/PKCS7.py` & `rns-0.5.5/RNS/Cryptography/PKCS7.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/Provider.py` & `rns-0.5.5/RNS/Cryptography/Provider.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/Proxies.py` & `rns-0.5.5/RNS/Cryptography/Proxies.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/SHA256.py` & `rns-0.5.5/RNS/Cryptography/SHA256.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/SHA512.py` & `rns-0.5.5/RNS/Cryptography/SHA512.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/X25519.py` & `rns-0.5.5/RNS/Cryptography/X25519.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/__init__.py` & `rns-0.5.5/RNS/Cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/aes/aes.py` & `rns-0.5.5/RNS/Cryptography/aes/aes.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/aes/utils.py` & `rns-0.5.5/RNS/Cryptography/aes/utils.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/pure25519/_ed25519.py` & `rns-0.5.5/RNS/Cryptography/pure25519/_ed25519.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/pure25519/basic.py` & `rns-0.5.5/RNS/Cryptography/pure25519/basic.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/pure25519/ed25519_oop.py` & `rns-0.5.5/RNS/Cryptography/pure25519/ed25519_oop.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Cryptography/pure25519/eddsa.py` & `rns-0.5.5/RNS/Cryptography/pure25519/eddsa.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Destination.py` & `rns-0.5.5/RNS/Destination.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Identity.py` & `rns-0.5.5/RNS/Identity.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/AX25KISSInterface.py` & `rns-0.5.5/RNS/Interfaces/AX25KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/Android/KISSInterface.py` & `rns-0.5.5/RNS/Interfaces/Android/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/Android/RNodeInterface.py` & `rns-0.5.5/RNS/Interfaces/Android/RNodeInterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,14 +391,15 @@
         self.r_sf        = None
         self.r_cr        = None
         self.r_state     = None
         self.r_lock      = None
         self.r_stat_rx   = None
         self.r_stat_tx   = None
         self.r_stat_rssi = None
+        self.r_stat_snr  = None
         self.r_random    = None
 
         self.packet_queue    = []
         self.flow_control    = flow_control
         self.interface_ready = False
         self.announce_rate_target = None
         self.last_port_io = 0
```

### Comparing `rns-0.5.4/RNS/Interfaces/Android/SerialInterface.py` & `rns-0.5.5/RNS/Interfaces/Android/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/Android/__init__.py` & `rns-0.5.5/RNS/Interfaces/Android/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/AutoInterface.py` & `rns-0.5.5/RNS/Interfaces/AutoInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/I2PInterface.py` & `rns-0.5.5/RNS/Interfaces/I2PInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/Interface.py` & `rns-0.5.5/RNS/Interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/KISSInterface.py` & `rns-0.5.5/RNS/Interfaces/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/LocalInterface.py` & `rns-0.5.5/RNS/Interfaces/LocalInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/PipeInterface.py` & `rns-0.5.5/RNS/Interfaces/PipeInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/RNodeInterface.py` & `rns-0.5.5/RNS/Interfaces/RNodeInterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,14 +153,15 @@
         self.r_sf        = None
         self.r_cr        = None
         self.r_state     = None
         self.r_lock      = None
         self.r_stat_rx   = None
         self.r_stat_tx   = None
         self.r_stat_rssi = None
+        self.r_stat_snr  = None
         self.r_random    = None
 
         self.packet_queue    = []
         self.flow_control    = flow_control
         self.interface_ready = False
         self.announce_rate_target = None
```

### Comparing `rns-0.5.4/RNS/Interfaces/SerialInterface.py` & `rns-0.5.5/RNS/Interfaces/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/TCPInterface.py` & `rns-0.5.5/RNS/Interfaces/TCPInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/UDPInterface.py` & `rns-0.5.5/RNS/Interfaces/UDPInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Interfaces/__init__.py` & `rns-0.5.5/RNS/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Link.py` & `rns-0.5.5/RNS/Link.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,49 +260,58 @@
         proof_data = packet.packet_hash + signature
 
         proof = RNS.Packet(self, proof_data, RNS.Packet.PROOF)
         proof.send()
         self.had_outbound()
 
     def validate_proof(self, packet):
-        if self.status == Link.PENDING:
-            if self.initiator and len(packet.data) == RNS.Identity.SIGLENGTH//8+Link.ECPUBSIZE//2:
-                peer_pub_bytes = packet.data[RNS.Identity.SIGLENGTH//8:RNS.Identity.SIGLENGTH//8+Link.ECPUBSIZE//2]
-                peer_sig_pub_bytes = self.destination.identity.get_public_key()[Link.ECPUBSIZE//2:Link.ECPUBSIZE]
-                self.load_peer(peer_pub_bytes, peer_sig_pub_bytes)
-                self.handshake()
-
-                self.establishment_cost += len(packet.raw)
-                signed_data = self.link_id+self.peer_pub_bytes+self.peer_sig_pub_bytes
-                signature = packet.data[:RNS.Identity.SIGLENGTH//8]
-                
-                if self.destination.identity.validate(signature, signed_data):
-                    self.rtt = time.time() - self.request_time
-                    self.attached_interface = packet.receiving_interface
-                    self.__remote_identity = self.destination.identity
-                    self.status = Link.ACTIVE
-                    self.activated_at = time.time()
-                    self.last_proof = self.activated_at
-                    RNS.Transport.activate_link(self)
-                    RNS.log("Link "+str(self)+" established with "+str(self.destination)+", RTT is "+str(round(self.rtt, 3))+"s", RNS.LOG_VERBOSE)
+        try:
+            if self.status == Link.PENDING:
+                if self.initiator and len(packet.data) == RNS.Identity.SIGLENGTH//8+Link.ECPUBSIZE//2:
+                    peer_pub_bytes = packet.data[RNS.Identity.SIGLENGTH//8:RNS.Identity.SIGLENGTH//8+Link.ECPUBSIZE//2]
+                    peer_sig_pub_bytes = self.destination.identity.get_public_key()[Link.ECPUBSIZE//2:Link.ECPUBSIZE]
+                    self.load_peer(peer_pub_bytes, peer_sig_pub_bytes)
+                    self.handshake()
+
+                    self.establishment_cost += len(packet.raw)
+                    signed_data = self.link_id+self.peer_pub_bytes+self.peer_sig_pub_bytes
+                    signature = packet.data[:RNS.Identity.SIGLENGTH//8]
                     
-                    if self.rtt != None and self.establishment_cost != None and self.rtt > 0 and self.establishment_cost > 0:
-                        self.establishment_rate = self.establishment_cost/self.rtt
+                    if self.destination.identity.validate(signature, signed_data):
+                        if self.status != Link.HANDSHAKE:
+                            raise IOError("Invalid link state for proof validation: "+str(self.status))
+
+                        self.rtt = time.time() - self.request_time
+                        self.attached_interface = packet.receiving_interface
+                        self.__remote_identity = self.destination.identity
+                        self.status = Link.ACTIVE
+                        self.activated_at = time.time()
+                        self.last_proof = self.activated_at
+                        RNS.Transport.activate_link(self)
+                        RNS.log("Link "+str(self)+" established with "+str(self.destination)+", RTT is "+str(round(self.rtt, 3))+"s", RNS.LOG_VERBOSE)
+                        
+                        if self.rtt != None and self.establishment_cost != None and self.rtt > 0 and self.establishment_cost > 0:
+                            self.establishment_rate = self.establishment_cost/self.rtt
 
-                    rtt_data = umsgpack.packb(self.rtt)
-                    rtt_packet = RNS.Packet(self, rtt_data, context=RNS.Packet.LRRTT)
-                    rtt_packet.send()
-                    self.had_outbound()
-
-                    if self.callbacks.link_established != None:
-                        thread = threading.Thread(target=self.callbacks.link_established, args=(self,))
-                        thread.daemon = True
-                        thread.start()
-                else:
-                    RNS.log("Invalid link proof signature received by "+str(self)+". Ignoring.", RNS.LOG_DEBUG)
+                        rtt_data = umsgpack.packb(self.rtt)
+                        rtt_packet = RNS.Packet(self, rtt_data, context=RNS.Packet.LRRTT)
+                        rtt_packet.send()
+                        self.had_outbound()
+
+                        if self.callbacks.link_established != None:
+                            thread = threading.Thread(target=self.callbacks.link_established, args=(self,))
+                            thread.daemon = True
+                            thread.start()
+                    else:
+                        RNS.log("Invalid link proof signature received by "+str(self)+". Ignoring.", RNS.LOG_DEBUG)
+        
+        except Exception as e:
+            self.status = Link.CLOSED
+            RNS.log("An error ocurred while validating link request proof on "+str(self)+".", RNS.LOG_ERROR)
+            RNS.log("The contained exception was: "+str(e), RNS.LOG_ERROR)
 
 
     def identify(self, identity):
         """
         Identifies the initiator of the link to the remote peer. This can only happen
         once the link has been established, and is carried out over the encrypted link.
         The identity is only revealed to the remote peer, and initiator anonymity is
@@ -516,24 +525,24 @@
                         self.link_closed()
                         sleep_time = 0.001
 
                 elif self.status == Link.HANDSHAKE:
                     next_check = self.request_time + self.establishment_timeout
                     sleep_time = next_check - time.time()
                     if time.time() >= self.request_time + self.establishment_timeout:
-                        if self.initiator:
-                            RNS.log("Timeout waiting for link request proof", RNS.LOG_DEBUG)
-                        else:
-                            RNS.log("Timeout waiting for RTT packet from link initiator", RNS.LOG_DEBUG)
-
                         self.status = Link.CLOSED
                         self.teardown_reason = Link.TIMEOUT
                         self.link_closed()
                         sleep_time = 0.001
 
+                        if self.initiator:
+                            RNS.log("Timeout waiting for link request proof", RNS.LOG_DEBUG)
+                        else:
+                            RNS.log("Timeout waiting for RTT packet from link initiator", RNS.LOG_DEBUG)
+
                 elif self.status == Link.ACTIVE:
                     activated_at = self.activated_at if self.activated_at != None else 0
                     last_inbound = max(max(self.last_inbound, self.last_proof), activated_at)
 
                     if time.time() >= last_inbound + self.keepalive:
                         if self.initiator:
                             self.send_keepalive()
@@ -843,15 +852,15 @@
 
     def encrypt(self, plaintext):
         try:
             if not self.fernet:
                 try:
                     self.fernet = Fernet(self.derived_key)
                 except Exception as e:
-                    RNS.log("Could not "+str(self)+" instantiate Fernet while performin encryption on link. The contained exception was: "+str(e), RNS.LOG_ERROR)
+                    RNS.log("Could not instantiate Fernet while performin encryption on link "+str(self)+". The contained exception was: "+str(e), RNS.LOG_ERROR)
                     raise e
 
             return self.fernet.encrypt(plaintext)
 
         except Exception as e:
             RNS.log("Encryption on link "+str(self)+" failed. The contained exception was: "+str(e), RNS.LOG_ERROR)
             raise e
```

### Comparing `rns-0.5.4/RNS/Packet.py` & `rns-0.5.5/RNS/Packet.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Resource.py` & `rns-0.5.5/RNS/Resource.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Reticulum.py` & `rns-0.5.5/RNS/Reticulum.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Transport.py` & `rns-0.5.5/RNS/Transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1737,14 +1737,16 @@
         else:
             Transport.active_links.append(link)
 
     @staticmethod
     def activate_link(link):
         RNS.log("Activating link "+str(link), RNS.LOG_EXTREME)
         if link in Transport.pending_links:
+            if link.status != RNS.Link.ACTIVE:
+                raise IOError("Invalid link state for link activation: "+str(link.status))
             Transport.pending_links.remove(link)
             Transport.active_links.append(link)
             link.status = RNS.Link.ACTIVE
         else:
             RNS.log("Attempted to activate a link that was not in the pending table", RNS.LOG_ERROR)
 
     @staticmethod
```

### Comparing `rns-0.5.4/RNS/Utilities/__init__.py` & `rns-0.5.5/RNS/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Utilities/rncp.py` & `rns-0.5.5/RNS/Utilities/rncp.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Utilities/rnid.py` & `rns-0.5.5/RNS/Utilities/rnid.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Utilities/rnodeconf.py` & `rns-0.5.5/RNS/Utilities/rnodeconf.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Utilities/rnpath.py` & `rns-0.5.5/RNS/Utilities/rnpath.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Utilities/rnprobe.py` & `rns-0.5.5/RNS/Utilities/rnprobe.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Utilities/rnsd.py` & `rns-0.5.5/RNS/Utilities/rnsd.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Utilities/rnstatus.py` & `rns-0.5.5/RNS/Utilities/rnstatus.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/Utilities/rnx.py` & `rns-0.5.5/RNS/Utilities/rnx.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/__init__.py` & `rns-0.5.5/RNS/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/configobj.py` & `rns-0.5.5/RNS/vendor/configobj.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/i2plib/__init__.py` & `rns-0.5.5/RNS/vendor/i2plib/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/i2plib/aiosam.py` & `rns-0.5.5/RNS/vendor/i2plib/aiosam.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/i2plib/exceptions.py` & `rns-0.5.5/RNS/vendor/i2plib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/i2plib/sam.py` & `rns-0.5.5/RNS/vendor/i2plib/sam.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/i2plib/tunnel.py` & `rns-0.5.5/RNS/vendor/i2plib/tunnel.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/i2plib/utils.py` & `rns-0.5.5/RNS/vendor/i2plib/utils.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/ifaddr/__init__.py` & `rns-0.5.5/RNS/vendor/ifaddr/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/ifaddr/_posix.py` & `rns-0.5.5/RNS/vendor/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/ifaddr/_shared.py` & `rns-0.5.5/RNS/vendor/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/ifaddr/_win32.py` & `rns-0.5.5/RNS/vendor/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/ifaddr/niwrapper.py` & `rns-0.5.5/RNS/vendor/ifaddr/niwrapper.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/platformutils.py` & `rns-0.5.5/RNS/vendor/platformutils.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/six.py` & `rns-0.5.5/RNS/vendor/six.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/RNS/vendor/umsgpack.py` & `rns-0.5.5/RNS/vendor/umsgpack.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/rns.egg-info/PKG-INFO` & `rns-0.5.5/rns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rns
-Version: 0.5.4
+Version: 0.5.5
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rns-0.5.4/rns.egg-info/SOURCES.txt` & `rns-0.5.5/rns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rns-0.5.4/setup.py` & `rns-0.5.5/setup.py`

 * *Files identical despite different names*

