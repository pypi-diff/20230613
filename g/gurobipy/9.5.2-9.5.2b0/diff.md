# Comparing `tmp/gurobipy-9.5.2-cp39-cp39-win_amd64.whl.zip` & `tmp/gurobipy-9.5.2b0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8944386 bytes, number of entries: 8
+Zip file size: 8944407 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       24 b- defN 22-Mar-07 11:14 gurobipy/__init__.py
--rw-rw-rw-  2.0 fat       89 b- defN 22-Jun-28 07:51 gurobipy/gurobi.lic
--rw-rw-rw-  2.0 fat 34562920 b- defN 22-Jun-28 07:51 gurobipy/gurobi95.dll
--rw-rw-rw-  2.0 fat  2527744 b- defN 22-Jun-28 07:52 gurobipy/gurobipy.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    15674 b- defN 22-Jun-28 07:52 gurobipy-9.5.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      105 b- defN 22-Jun-28 07:52 gurobipy-9.5.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Jun-28 07:52 gurobipy-9.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      630 b- defN 22-Jun-28 07:52 gurobipy-9.5.2.dist-info/RECORD
-8 files, 37107195 bytes uncompressed, 8943300 bytes compressed:  75.9%
+-rw-rw-rw-  2.0 fat       89 b- defN 22-Jun-16 19:55 gurobipy/gurobi.lic
+-rw-rw-rw-  2.0 fat 34562920 b- defN 22-Jun-16 19:55 gurobipy/gurobi95.dll
+-rw-rw-rw-  2.0 fat  2527744 b- defN 22-Jun-16 19:56 gurobipy/gurobipy.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    15676 b- defN 22-Jun-16 19:56 gurobipy-9.5.2b0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      105 b- defN 22-Jun-16 19:56 gurobipy-9.5.2b0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 22-Jun-16 19:56 gurobipy-9.5.2b0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      638 b- defN 22-Jun-16 19:56 gurobipy-9.5.2b0.dist-info/RECORD
+8 files, 37107205 bytes uncompressed, 8943305 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gurobipy/gurobi95.dll
 Comment: 
 
 Filename: gurobipy/gurobipy.cp39-win_amd64.pyd
 Comment: 
 
-Filename: gurobipy-9.5.2.dist-info/METADATA
+Filename: gurobipy-9.5.2b0.dist-info/METADATA
 Comment: 
 
-Filename: gurobipy-9.5.2.dist-info/WHEEL
+Filename: gurobipy-9.5.2b0.dist-info/WHEEL
 Comment: 
 
-Filename: gurobipy-9.5.2.dist-info/top_level.txt
+Filename: gurobipy-9.5.2b0.dist-info/top_level.txt
 Comment: 
 
-Filename: gurobipy-9.5.2.dist-info/RECORD
+Filename: gurobipy-9.5.2b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gurobipy-9.5.2.dist-info/METADATA` & `gurobipy-9.5.2b0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobipy
-Version: 9.5.2
+Version: 9.5.2b0
 Summary: Python interface to Gurobi
 Home-page: https://www.gurobi.com
 Author: Gurobi Optimization, LLC
 License: Proprietary
 Keywords: optimization,mip,lp
 Platform: Windows
 Platform: Linux
```

## Comparing `gurobipy-9.5.2.dist-info/RECORD` & `gurobipy-9.5.2b0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gurobipy/__init__.py,sha256=paXoGzzB0Scc7jnJU2aHaO5OGE2iayIlyn97lPwBPeo,24
 gurobipy/gurobi.lic,sha256=9UC_NsmlVglbynO2YJYRaYp1cyvNfr-pnOoasKV_pv0,89
 gurobipy/gurobi95.dll,sha256=ysMgjsSxGp69HPpv7rcWqUyHv5pf_ItMPYzGTx3M79g,34562920
-gurobipy/gurobipy.cp39-win_amd64.pyd,sha256=i34xkaojpFRlv4GDIib9BwM8i1ExkcTXkgcRk1pSVz8,2527744
-gurobipy-9.5.2.dist-info/METADATA,sha256=fiHAdI1PiGtCokyEg2gXn5iKZaLI_8NCjBE_kH8S9wE,15674
-gurobipy-9.5.2.dist-info/WHEEL,sha256=2Kg4PzfJLrLEnxRV1e1jZf0TVEjxVcXZXjp8WtjE4tI,105
-gurobipy-9.5.2.dist-info/top_level.txt,sha256=lI8imVf2_cKV2kVT6NVXJ4sH0ib8oAKeh06ysN_0_Bg,9
-gurobipy-9.5.2.dist-info/RECORD,,
+gurobipy/gurobipy.cp39-win_amd64.pyd,sha256=TZ7-qrUj9IkEbA6huCjelgH_lUbgK-FilTpVeRCffq8,2527744
+gurobipy-9.5.2b0.dist-info/METADATA,sha256=DJXwnfCify35girf50MXwRW7ZhcFo4SqRZCPJciAnqo,15676
+gurobipy-9.5.2b0.dist-info/WHEEL,sha256=2Kg4PzfJLrLEnxRV1e1jZf0TVEjxVcXZXjp8WtjE4tI,105
+gurobipy-9.5.2b0.dist-info/top_level.txt,sha256=lI8imVf2_cKV2kVT6NVXJ4sH0ib8oAKeh06ysN_0_Bg,9
+gurobipy-9.5.2b0.dist-info/RECORD,,
```

