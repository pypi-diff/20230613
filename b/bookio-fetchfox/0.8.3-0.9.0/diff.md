# Comparing `tmp/bookio_fetchfox-0.8.3.tar.gz` & `tmp/bookio_fetchfox-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.8.3.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.9.0.tar", max compression
```

## Comparing `bookio_fetchfox-0.8.3.tar` & `bookio_fetchfox-0.9.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3723 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/README.md
--rw-r--r--   0        0        0        0 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2156 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      604 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1357 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1780 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      600 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2658 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      793 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1647 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/cardano/jpgstore.py
--rwxr-xr-x   0        0        0      683 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      966 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4277 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2725 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-13 09:13:52.486652 bookio_fetchfox-0.8.3/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     9405 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      501 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     2596 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    13947 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1043 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0     1505 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0    10224 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      616 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0     1512 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      146 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0       82 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/constants/cardano.py
--rw-r--r--   0        0        0      112 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0       66 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/constants/evm.py
--rw-r--r--   0        0        0      296 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      216 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     3194 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     3435 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      463 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1586 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      365 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1969 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1895 2023-06-13 09:13:52.490653 bookio_fetchfox-0.8.3/fetchfox/rest.py
--rw-r--r--   0        0        0     1148 2023-06-13 09:13:52.502654 bookio_fetchfox-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.8.3/setup.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     3723 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2156 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      604 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1357 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1780 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      600 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2659 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      793 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1647 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/cardano/jpgstore.py
+-rwxr-xr-x   0        0        0      683 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      966 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4939 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2725 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     9601 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      501 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     2744 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-13 09:35:04.913481 bookio_fetchfox-0.9.0/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    14141 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1043 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0     1505 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0    10793 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      616 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0     1512 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      146 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0       82 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/constants/cardano.py
+-rw-r--r--   0        0        0      112 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0       66 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/constants/evm.py
+-rw-r--r--   0        0        0      296 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      216 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     3194 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3435 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      463 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1586 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      365 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1969 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1895 2023-06-13 09:35:04.917481 bookio_fetchfox-0.9.0/fetchfox/rest.py
+-rw-r--r--   0        0        0     1148 2023-06-13 09:35:04.929481 bookio_fetchfox-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.9.0/setup.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.9.0/PKG-INFO
```

### Comparing `bookio_fetchfox-0.8.3/README.md` & `bookio_fetchfox-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/cardano/blockfrostio.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         yield from response
 
 
 def get_owner(asset_id: str, project_id: str) -> dict:
     check_str(asset_id, "blockfrost.asset_id")
 
     response, status_code = get(
-        "assets/{asset_id}/addresses",
+        f"assets/{asset_id}/addresses",
         project_id=project_id,
     )
 
     for item in response:
         if item["quantity"] == "1":
             return {
                 "asset_id": asset_id,
```

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/cardano/cnfttools.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/cardano/cnfttools.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/coingeckocom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/evm/moralisio.py`

 * *Files 12% similar despite different names*

```diff
@@ -150,7 +150,27 @@
                 "amount": holding["amount"],
             }
 
         cursor = response.get("cursor")
 
         if not cursor:
             break
+
+
+def get_owner(contract_address: str, asset_id: str, blockchain: str, api_key: str) -> dict:
+    check_str(contract_address, "moralisio.contract_address")
+    check_str(asset_id, "moralisio.asset_id")
+    contract_address = contract_address.strip().lower()
+
+    response, status_code = get(
+        f"nft/{contract_address}/{asset_id}/owners",
+        blockchain=blockchain,
+        api_key=api_key,
+    )
+
+    for holding in response["result"]:
+        return {
+            "contract_address": holding["token_address"],
+            "asset_id": holding["token_id"],
+            "address": holding["owner_of"],
+            "amount": holding["amount"],
+        }
```

### Comparing `bookio_fetchfox-0.8.3/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.9.0/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.9.0/fetchfox/blockchains/algorand/blockchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,24 +149,30 @@
                 quantity=quantity,
             )
 
     def get_snapshot(self, collection_id: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_collection_id(collection_id)
 
         for asset in self.get_assets(collection_id, fetch_metadata=False):
-            holding = algonodecloud.get_owner(
-                str(asset.asset_id),
-            )
+            yield self.get_owner(collection_id, asset.asset_id)
 
-            yield HoldingDTO(
-                collection_id=asset.collection_id,
-                asset_id=holding["asset_id"],
-                address=holding["address"],
-                quantity=holding["amount"],
-            )
+    def get_owner(self, collection_id: str, asset_id: str, *args, **kwargs) -> HoldingDTO:
+        self.check_collection_id(collection_id)
+        self.check_asset_id(asset_id)
+
+        holding = algonodecloud.get_owner(
+            str(asset_id),
+        )
+
+        return HoldingDTO(
+            collection_id=collection_id,
+            asset_id=holding["asset_id"],
+            address=holding["address"],
+            quantity=holding["amount"],
+        )
 
     def get_listings(self, collection_id: str, *args, **kwargs) -> Iterable[ListingDTO]:
         self.check_collection_id(collection_id)
 
         listings = randswapcom.get_listings(collection_id)
 
         for listing in listings:
```

### Comparing `bookio_fetchfox-0.8.3/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.9.0/fetchfox/blockchains/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,7 +78,11 @@
     @abstractmethod
     def get_snapshot(self, collection_id: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_sales(self, collection_id: str, *args, **kwargs) -> Iterable[SaleDTO]:
         raise NotImplementedError()
+
+    @abstractmethod
+    def get_owner(self, collection_id: str, asset_id: str, *args, **kwargs) -> HoldingDTO:
+        raise NotImplementedError()
```

### Comparing `bookio_fetchfox-0.8.3/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.9.0/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,27 +255,33 @@
             rank=int(rank),
         )
 
     def get_snapshot(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_collection_id(collection_id)
 
         for asset in self.get_assets(collection_id, discriminator=discriminator, fetch_metadata=False):
-            holding = blockfrostio.get_owner(
-                asset.asset_id,
-                project_id=self.blockfrostio_project_id,
-            )
-
-            stake_address = self.get_stake_key(holding["address"])
-
-            yield HoldingDTO(
-                collection_id=collection_id,
-                asset_id=holding["asset_id"],
-                address=stake_address,
-                quantity=holding["amount"],
-            )
+            yield self.get_owner(collection_id, asset.asset_id)
+
+    def get_owner(self, collection_id: str, asset_id: str, *args, **kwargs) -> HoldingDTO:
+        self.check_collection_id(collection_id)
+        self.check_asset_id(asset_id)
+
+        holding = blockfrostio.get_owner(
+            asset_id,
+            project_id=self.blockfrostio_project_id,
+        )
+
+        stake_address = self.get_stake_key(holding["address"])
+
+        return HoldingDTO(
+            collection_id=collection_id,
+            asset_id=holding["asset_id"],
+            address=stake_address,
+            quantity=holding["amount"],
+        )
 
     def get_listings(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Iterable[ListingDTO]:
         self.check_collection_id(collection_id)
 
         if discriminator:
             discriminator = discriminator.lower()
```

### Comparing `bookio_fetchfox-0.8.3/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.9.0/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-0.9.0/fetchfox/blockchains/ethereum/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.9.0/fetchfox/blockchains/evm/blockchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,32 @@
             yield HoldingDTO(
                 collection_id=asset["contract_address"],
                 asset_id=asset["asset_id"],
                 address=asset["address"],
                 quantity=asset["amount"],
             )
 
+    def get_owner(self, collection_id: str, asset_id: str, *args, **kwargs) -> HoldingDTO:
+        self.check_collection_id(collection_id)
+        self.check_asset_id(asset_id)
+
+        asset = moralisio.get_owner(
+            collection_id,
+            asset_id=asset_id,
+            blockchain=self.name,
+            api_key=self.moralisio_api_key,
+        )
+
+        return HoldingDTO(
+            collection_id=asset["contract_address"],
+            asset_id=asset["asset_id"],
+            address=asset["address"],
+            quantity=asset["amount"],
+        )
+
     def get_listings(self, collection_id: str, slug: str = None, *args, **kwargs) -> Iterable[ListingDTO]:
         self.check_collection_id(collection_id)
 
         listings = openseaio.get_listings(
             collection_id,
             api_key=self.openseaio_api_key,
             slug=slug,
```

### Comparing `bookio_fetchfox-0.8.3/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.9.0/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/blockchains/polygon/blockchain.py` & `bookio_fetchfox-0.9.0/fetchfox/blockchains/polygon/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.9.0/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.9.0/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.9.0/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/dtos/sale.py` & `bookio_fetchfox-0.9.0/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/fetchfox/rest.py` & `bookio_fetchfox-0.9.0/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.8.3/pyproject.toml` & `bookio_fetchfox-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.8.3"
+version = "0.9.0"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-0.8.3/setup.py` & `bookio_fetchfox-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.8.3',
+    'version': '0.9.0',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-0.8.3/PKG-INFO` & `bookio_fetchfox-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.8.3
+Version: 0.9.0
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```

