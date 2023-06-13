# Comparing `tmp/dploot-2.1.8.tar.gz` & `tmp/dploot-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dploot-2.1.8.tar", last modified: Mon Feb  6 11:15:45 2023, max compression
+gzip compressed data, was "dploot-2.1.9.tar", last modified: Mon Feb  6 13:52:42 2023, max compression
```

## Comparing `dploot-2.1.8.tar` & `dploot-2.1.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 11:15:45.709861 dploot-2.1.8/
--rw-rw-r--   0 tse       (1000) tse       (1000)     1066 2023-02-06 11:11:26.000000 dploot-2.1.8/LICENSE
--rw-rw-r--   0 tse       (1000) tse       (1000)      317 2023-02-06 11:15:45.709861 dploot-2.1.8/PKG-INFO
--rwxrwxr-x   0 tse       (1000) tse       (1000)    29201 2023-02-06 11:11:26.000000 dploot-2.1.8/README.md
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 11:15:45.701861 dploot-2.1.8/dploot/
--rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/__init__.py
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 11:15:45.705860 dploot-2.1.8/dploot/action/
--rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/__init__.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     2959 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/backupkey.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     4439 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/browser.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     4558 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/certificates.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3973 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/credentials.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     4276 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/machinecertificates.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3719 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/machinecredentials.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3369 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/machinemasterkeys.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     6095 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/machinetriage.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3641 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/machinevaults.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     5163 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/masterkeys.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     4511 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/rdg.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     7843 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/triage.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3873 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/vaults.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3800 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/action/wifi.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     1818 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/entry.py
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 11:15:45.705860 dploot-2.1.8/dploot/lib/
--rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/lib/__init__.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)    11877 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/lib/crypto.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)    10464 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/lib/dpapi.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     6554 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/lib/smb.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     5823 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/lib/target.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     1870 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/lib/utils.py
--rw-rw-r--   0 tse       (1000) tse       (1000)     1909 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/lib/wmi.py
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 11:15:45.709861 dploot-2.1.8/dploot/triage/
--rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/triage/__init__.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3068 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/triage/backupkey.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)    10478 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/triage/browser.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)    13447 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/triage/certificates.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     5912 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/triage/credentials.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     8548 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/triage/masterkeys.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     8935 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/triage/rdg.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     9102 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/triage/vaults.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     9875 2023-02-06 11:11:26.000000 dploot-2.1.8/dploot/triage/wifi.py
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 11:15:45.701861 dploot-2.1.8/dploot.egg-info/
--rw-rw-r--   0 tse       (1000) tse       (1000)      317 2023-02-06 11:15:45.000000 dploot-2.1.8/dploot.egg-info/PKG-INFO
--rw-rw-r--   0 tse       (1000) tse       (1000)     1042 2023-02-06 11:15:45.000000 dploot-2.1.8/dploot.egg-info/SOURCES.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)        1 2023-02-06 11:15:45.000000 dploot-2.1.8/dploot.egg-info/dependency_links.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)       46 2023-02-06 11:15:45.000000 dploot-2.1.8/dploot.egg-info/entry_points.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)       61 2023-02-06 11:15:45.000000 dploot-2.1.8/dploot.egg-info/requires.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)        7 2023-02-06 11:15:45.000000 dploot-2.1.8/dploot.egg-info/top_level.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)       38 2023-02-06 11:15:45.709861 dploot-2.1.8/setup.cfg
--rwxrwxr-x   0 tse       (1000) tse       (1000)      698 2023-02-06 11:11:26.000000 dploot-2.1.8/setup.py
+drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.998914 dploot-2.1.9/
+-rw-rw-r--   0 tse       (1000) tse       (1000)     1066 2023-02-06 11:11:26.000000 dploot-2.1.9/LICENSE
+-rw-rw-r--   0 tse       (1000) tse       (1000)      317 2023-02-06 13:52:41.998914 dploot-2.1.9/PKG-INFO
+-rwxrwxr-x   0 tse       (1000) tse       (1000)    29201 2023-02-06 11:11:26.000000 dploot-2.1.9/README.md
+drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.990914 dploot-2.1.9/dploot/
+-rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/__init__.py
+drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.994914 dploot-2.1.9/dploot/action/
+-rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/__init__.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     2959 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/backupkey.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     4439 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/browser.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     4558 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/certificates.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     3973 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/credentials.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     4276 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinecertificates.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     3719 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinecredentials.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     3369 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinemasterkeys.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     6095 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinetriage.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     3641 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinevaults.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     5370 2023-02-06 13:49:08.000000 dploot-2.1.9/dploot/action/masterkeys.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     4511 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/rdg.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     7843 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/triage.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     3873 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/vaults.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     3800 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/wifi.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     1818 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/entry.py
+drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.998914 dploot-2.1.9/dploot/lib/
+-rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/__init__.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)    11877 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/crypto.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)    10464 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/dpapi.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     6554 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/smb.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     5823 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/target.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     1870 2023-02-06 13:47:25.000000 dploot-2.1.9/dploot/lib/utils.py
+-rw-rw-r--   0 tse       (1000) tse       (1000)     1909 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/wmi.py
+drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.998914 dploot-2.1.9/dploot/triage/
+-rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/__init__.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     3068 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/backupkey.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)    10478 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/browser.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)    13447 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/certificates.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     5912 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/credentials.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     8580 2023-02-06 13:41:52.000000 dploot-2.1.9/dploot/triage/masterkeys.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     8935 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/rdg.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     9102 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/vaults.py
+-rwxrwxr-x   0 tse       (1000) tse       (1000)     9875 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/wifi.py
+drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.990914 dploot-2.1.9/dploot.egg-info/
+-rw-rw-r--   0 tse       (1000) tse       (1000)      317 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/PKG-INFO
+-rw-rw-r--   0 tse       (1000) tse       (1000)     1042 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/SOURCES.txt
+-rw-rw-r--   0 tse       (1000) tse       (1000)        1 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/dependency_links.txt
+-rw-rw-r--   0 tse       (1000) tse       (1000)       46 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/entry_points.txt
+-rw-rw-r--   0 tse       (1000) tse       (1000)       61 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/requires.txt
+-rw-rw-r--   0 tse       (1000) tse       (1000)        7 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/top_level.txt
+-rw-rw-r--   0 tse       (1000) tse       (1000)       38 2023-02-06 13:52:41.998914 dploot-2.1.9/setup.cfg
+-rwxrwxr-x   0 tse       (1000) tse       (1000)      698 2023-02-06 13:51:22.000000 dploot-2.1.9/setup.py
```

### Comparing `dploot-2.1.8/LICENSE` & `dploot-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/README.md` & `dploot-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/backupkey.py` & `dploot-2.1.9/dploot/action/backupkey.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/browser.py` & `dploot-2.1.9/dploot/action/browser.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/certificates.py` & `dploot-2.1.9/dploot/action/certificates.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/credentials.py` & `dploot-2.1.9/dploot/action/credentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/machinecertificates.py` & `dploot-2.1.9/dploot/action/machinecertificates.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/machinecredentials.py` & `dploot-2.1.9/dploot/action/machinecredentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/machinemasterkeys.py` & `dploot-2.1.9/dploot/action/machinemasterkeys.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/machinetriage.py` & `dploot-2.1.9/dploot/action/machinetriage.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/machinevaults.py` & `dploot-2.1.9/dploot/action/machinevaults.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/masterkeys.py` & `dploot-2.1.9/dploot/action/masterkeys.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,15 +101,21 @@
         if passwords is None:
             passwords = dict()
         passwords[target.username] = target.password
 
     if target.nthash != '':
         if nthashes is None:
             nthashes = dict()
-        nthashes[target.username] = target.nthash
+        nthashes[target.username] = target.nthash.lower()
+
+    if nthashes is not None:
+        nthashes = {k.lower():v.lower() for k, v in nthashes.items()}
+    
+    if passwords is not None:
+        passwords = {k.lower():v for k, v in passwords.items()}
 
     return pvkbytes, passwords, nthashes
 
 def add_masterkeys_argument_group(group: argparse._ArgumentGroup) -> None:
 
     group.add_argument(
         "-pvk",
```

### Comparing `dploot-2.1.8/dploot/action/rdg.py` & `dploot-2.1.9/dploot/action/rdg.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/triage.py` & `dploot-2.1.9/dploot/action/triage.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/vaults.py` & `dploot-2.1.9/dploot/action/vaults.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/action/wifi.py` & `dploot-2.1.9/dploot/action/wifi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/entry.py` & `dploot-2.1.9/dploot/entry.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/lib/crypto.py` & `dploot-2.1.9/dploot/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/lib/dpapi.py` & `dploot-2.1.9/dploot/lib/dpapi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/lib/smb.py` & `dploot-2.1.9/dploot/lib/smb.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/lib/target.py` & `dploot-2.1.9/dploot/lib/target.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/lib/utils.py` & `dploot-2.1.9/dploot/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/lib/wmi.py` & `dploot-2.1.9/dploot/lib/wmi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/triage/backupkey.py` & `dploot-2.1.9/dploot/triage/backupkey.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/triage/browser.py` & `dploot-2.1.9/dploot/triage/browser.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/triage/certificates.py` & `dploot-2.1.9/dploot/triage/certificates.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/triage/credentials.py` & `dploot-2.1.9/dploot/triage/credentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/triage/masterkeys.py` & `dploot-2.1.9/dploot/triage/masterkeys.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,16 +129,16 @@
                         masterkey_bytes = self.conn.readFile(self.share, filepath)
                         if masterkey_bytes is not None:
                             self.looted_files[guid] = masterkey_bytes
                             key = decrypt_masterkey(
                                 masterkey=masterkey_bytes,
                                 domain_backupkey=self.pvkbytes,
                                 sid=sid, 
-                                password=self.passwords[user] if self.passwords is not None and user in self.passwords else None,
-                                nthash=self.nthashes[user] if self.nthashes is not None and user in self.nthashes else None,
+                                password=self.passwords[user.lower()] if self.passwords is not None and user.lower() in self.passwords else None,
+                                nthash=self.nthashes[user.lower()] if self.nthashes is not None and user.lower() in self.nthashes else None,
                                 )
                             if key is not None:
                                 masterkeys.append(Masterkey(guid=guid, sha1=hexlify(SHA1.new(key).digest()).decode('latin-1'), user=user))
         return masterkeys
 
     def getDPAPI_SYSTEM(self,secretType, secret) -> None:
         if secret.startswith("dpapi_machinekey:"):
```

### Comparing `dploot-2.1.8/dploot/triage/rdg.py` & `dploot-2.1.9/dploot/triage/rdg.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/triage/vaults.py` & `dploot-2.1.9/dploot/triage/vaults.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot/triage/wifi.py` & `dploot-2.1.9/dploot/triage/wifi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/dploot.egg-info/SOURCES.txt` & `dploot-2.1.9/dploot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dploot-2.1.8/setup.py` & `dploot-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="dploot",
-    version="2.1.8",
+    version="2.1.9",
     author="zblurx",
     author_email="seigneuret.thomas@pm.me",
     description="DPAPI looting remotely in Python",
     long_description="README.md",
     long_description_content_type="text/markdown",
     url="https://github.com/zblurx/dploot",
     license="MIT",
```

