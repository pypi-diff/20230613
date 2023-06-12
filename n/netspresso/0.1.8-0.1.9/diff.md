# Comparing `tmp/netspresso-0.1.8-py3-none-any.whl.zip` & `tmp/netspresso-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 20290 bytes, number of entries: 24
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-12 22:40 netspresso/__init__.py
+Zip file size: 20286 bytes, number of entries: 24
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-12 22:51 netspresso/__init__.py
 -rw-rw-rw-  2.0 fat    23322 b- defN 23-Jun-12 20:25 netspresso/compressor/__init__.py
 -rw-rw-rw-  2.0 fat     8456 b- defN 23-Jun-05 06:16 netspresso/compressor/client/__init__.py
--rw-rw-rw-  2.0 fat      586 b- defN 23-Jun-12 22:38 netspresso/compressor/client/config.py
+-rw-rw-rw-  2.0 fat      535 b- defN 23-Jun-12 22:51 netspresso/compressor/client/config.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 02:41 netspresso/compressor/client/schemas/__init__.py
 -rw-rw-rw-  2.0 fat     2644 b- defN 23-Jun-05 02:41 netspresso/compressor/client/schemas/auth.py
 -rw-rw-rw-  2.0 fat      482 b- defN 23-Jun-05 02:41 netspresso/compressor/client/schemas/common.py
 -rw-rw-rw-  2.0 fat     4108 b- defN 23-Jun-12 20:25 netspresso/compressor/client/schemas/compression.py
 -rw-rw-rw-  2.0 fat     5681 b- defN 23-Jun-12 20:25 netspresso/compressor/client/schemas/model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 02:41 netspresso/compressor/client/utils/__init__.py
 -rw-rw-rw-  2.0 fat      481 b- defN 23-Jun-05 02:41 netspresso/compressor/client/utils/common.py
@@ -14,13 +14,13 @@
 -rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-05 02:41 netspresso/compressor/client/utils/validator.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 02:41 netspresso/compressor/core/__init__.py
 -rw-rw-rw-  2.0 fat     1900 b- defN 23-Jun-12 20:25 netspresso/compressor/core/compression.py
 -rw-rw-rw-  2.0 fat     2966 b- defN 23-Jun-12 20:25 netspresso/compressor/core/model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 02:41 netspresso/compressor/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2035 b- defN 23-Jun-12 20:25 netspresso/compressor/utils/model.py
 -rw-rw-rw-  2.0 fat      236 b- defN 23-Jun-05 02:41 netspresso/compressor/utils/token.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-12 22:42 netspresso-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      769 b- defN 23-Jun-12 22:42 netspresso-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 22:42 netspresso-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-12 22:42 netspresso-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2237 b- defN 23-Jun-12 22:42 netspresso-0.1.8.dist-info/RECORD
-24 files, 72241 bytes uncompressed, 16554 bytes compressed:  77.1%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-12 22:51 netspresso-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      769 b- defN 23-Jun-12 22:51 netspresso-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 22:51 netspresso-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-12 22:51 netspresso-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2237 b- defN 23-Jun-12 22:51 netspresso-0.1.9.dist-info/RECORD
+24 files, 72190 bytes uncompressed, 16550 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -51,23 +51,23 @@
 
 Filename: netspresso/compressor/utils/model.py
 Comment: 
 
 Filename: netspresso/compressor/utils/token.py
 Comment: 
 
-Filename: netspresso-0.1.8.dist-info/LICENSE
+Filename: netspresso-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: netspresso-0.1.8.dist-info/METADATA
+Filename: netspresso-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: netspresso-0.1.8.dist-info/WHEEL
+Filename: netspresso-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: netspresso-0.1.8.dist-info/top_level.txt
+Filename: netspresso-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: netspresso-0.1.8.dist-info/RECORD
+Filename: netspresso-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netspresso/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## netspresso/compressor/client/config.py

```diff
@@ -1,18 +1,18 @@
 import configparser
 import os
 from pathlib import Path
 
 from loguru import logger
+from pydantic import BaseSettings
 
+BASE_DIR = Path(__file__).resolve().parent
+config = configparser.ConfigParser()
+DEPLOYMENT_MODE = os.getenv("DEPLOYMENT_MODE", "PROD")
+logger.info(f"Read {DEPLOYMENT_MODE} config")
+config.read(f"{BASE_DIR}/configs/config-{DEPLOYMENT_MODE.lower()}.ini")
 
-class Config:
-    def __init__(self) -> None:
-        BASE_DIR = Path(__file__).resolve().parent
-        config = configparser.ConfigParser()
-        DEPLOYMENT_MODE = os.getenv("DEPLOYMENT_MODE", "PROD")
-        logger.info(f"Read {DEPLOYMENT_MODE} config")
-        config.read(f"{BASE_DIR}/configs/config-{DEPLOYMENT_MODE.lower()}.ini")
 
-        self.API_PREFIX: str = "/api/v2"
-        self.IP: str = config["GENERAL"]["IP"]
-        self.PORT: int = int(config["GENERAL"]["PORT"])
+class Config(BaseSettings):
+    API_PREFIX: str = "/api/v2"
+    IP: str = config["GENERAL"]["IP"]
+    PORT: int = int(config["GENERAL"]["PORT"])
```

## Comparing `netspresso-0.1.8.dist-info/LICENSE` & `netspresso-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netspresso-0.1.8.dist-info/METADATA` & `netspresso-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netspresso
-Version: 0.1.8
+Version: 0.1.9
 Summary: NetsPresso Python Package
 Home-page: https://github.com/Nota-NetsPresso/netspresso-python
 Author: NetsPresso
 Author-email: bmlee@nota.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `netspresso-0.1.8.dist-info/RECORD` & `netspresso-0.1.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-netspresso/__init__.py,sha256=0xngvyws52ELzKEHKt7iPFCbLG7K2r7U7qtbX9gCyQM,23
+netspresso/__init__.py,sha256=eV1qXt5ItBAELF1kU226t6-A_4Kn4s7Ddf8OiUuc04c,23
 netspresso/compressor/__init__.py,sha256=8nccEoi_l_5HaBse4tqOnHqGtdsRq52FqjlMET2VGeY,23322
 netspresso/compressor/client/__init__.py,sha256=pgYngRDyZBTc3vTDNeZPHpSc86KJ_122J-jdKFArpT0,8456
-netspresso/compressor/client/config.py,sha256=K-xQ7TPo3cTQLA9aLsSyx4CPU2mdNJ3zCM_0NpkWVTk,586
+netspresso/compressor/client/config.py,sha256=CjYFS5hAQ7ZjUTE0utCKNOboT7LV1FiGKk_FcsrjPXY,535
 netspresso/compressor/client/schemas/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/client/schemas/auth.py,sha256=NGudVfx4Q7E8XppeDgcKmQlU_3UwKDu3YjYiIwsii1g,2644
 netspresso/compressor/client/schemas/common.py,sha256=w1rR-jqIvjQ6UqMRZ5KYWW8bQrlXMSrAdWXCzA3tQuk,482
 netspresso/compressor/client/schemas/compression.py,sha256=0OwRemHeFQy4wZBWHzwcYuf0T2w8fN7Hb39fHWyPM0k,4108
 netspresso/compressor/client/schemas/model.py,sha256=hprc5AQ3gFe8hjtoHEcyKM8HoQCYn53LJwQJ_QsBUHA,5681
 netspresso/compressor/client/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/client/utils/common.py,sha256=gAHVbvzBGmoYNExaGOEgaqJHTszXuMOSwCFpyH_xEwc,481
@@ -13,12 +13,12 @@
 netspresso/compressor/client/utils/validator.py,sha256=0pONKSTlxTWcpSIiUw3P2ItPARoLXvu5YSGGxhUFPNU,3814
 netspresso/compressor/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/core/compression.py,sha256=OMrI-SsDXmwzZdz_1jRmv30KTGRRluRszJPqcXFQOwU,1900
 netspresso/compressor/core/model.py,sha256=kH0VBvcpwyxO9QsUpaQZXLB-IZXfw3T-mp613qX3_mE,2966
 netspresso/compressor/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/utils/model.py,sha256=tPojNWMvvHTNT8EgLIJfq_3EWIOIb0HuZHDbF1ANBc0,2035
 netspresso/compressor/utils/token.py,sha256=zWKx6olb8N2c3nSQhUS22IRG7ILQZYIERScETEFeUXY,236
-netspresso-0.1.8.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-netspresso-0.1.8.dist-info/METADATA,sha256=o3zGj-UWAJYjOG80oKNPDYPVGhLs5DOnjrO99CQusz4,769
-netspresso-0.1.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-netspresso-0.1.8.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
-netspresso-0.1.8.dist-info/RECORD,,
+netspresso-0.1.9.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+netspresso-0.1.9.dist-info/METADATA,sha256=Xm8m70PAVTWaF15PnvzuNBzTqbbjYHsABlMFECdBWck,769
+netspresso-0.1.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+netspresso-0.1.9.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
+netspresso-0.1.9.dist-info/RECORD,,
```

