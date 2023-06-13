# Comparing `tmp/bookio_fetchfox-0.7.8.tar.gz` & `tmp/bookio_fetchfox-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.7.8.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.8.0.tar", max compression
```

## Comparing `bookio_fetchfox-0.7.8.tar` & `bookio_fetchfox-0.8.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
--rw-r--r--   0        0        0     3723 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/README.md
--rw-r--r--   0        0        0        0 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2156 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      604 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1357 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1780 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      600 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2658 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      734 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1647 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/cardano/jpgstore.py
--rwxr-xr-x   0        0        0      683 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      963 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4277 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2725 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     8903 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      501 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     2459 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    12945 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1043 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0     9864 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      616 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0     1398 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      146 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      112 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0      296 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      216 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     2815 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     3435 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      463 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1586 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      365 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1969 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1895 2023-06-12 23:32:01.112907 bookio_fetchfox-0.7.8/fetchfox/rest.py
--rw-r--r--   0        0        0     1148 2023-06-12 23:32:01.124907 bookio_fetchfox-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.8/setup.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     3723 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2156 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      604 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1357 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1780 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      600 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2658 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      734 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1647 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/cardano/jpgstore.py
+-rwxr-xr-x   0        0        0      683 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      966 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4277 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2725 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     9291 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      501 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     2575 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    13799 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1043 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0    10224 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      616 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0     1398 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      146 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0       82 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/constants/cardano.py
+-rw-r--r--   0        0        0      112 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0       66 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/constants/evm.py
+-rw-r--r--   0        0        0      296 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-13 00:17:18.033765 bookio_fetchfox-0.8.0/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      216 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3435 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      463 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1586 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      365 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1969 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1895 2023-06-13 00:17:18.037765 bookio_fetchfox-0.8.0/fetchfox/rest.py
+-rw-r--r--   0        0        0     1148 2023-06-13 00:17:18.049765 bookio_fetchfox-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.8.0/setup.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.8.0/PKG-INFO
```

### Comparing `bookio_fetchfox-0.7.8/README.md` & `bookio_fetchfox-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/cardano/blockfrostio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/cardano/cnfttools.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/cardano/cnfttools.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/coingeckocom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/evm/ensideascom.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 
     ens_domain = response.get("name")
 
     if not ens_domain:
         return None
 
     logger.info("resolved %s to %s", address, ens_domain)
-    return address
+    return ens_domain
```

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.8.0/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.8.0/fetchfox/blockchains/algorand/blockchain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from datetime import datetime
+from functools import lru_cache
 from typing import Iterable
 
 import pytz
 
 from fetchfox.apis.algorand import (
     algonodecloud,
     nfdomains,
@@ -56,14 +57,29 @@
             return f"https://algoexplorer.io/address/{collection_id.upper()}"
 
         if tx_hash:
             return f"https://algoexplorer.io/tx/{tx_hash.upper()}"
 
         return None
 
+    @lru_cache
+    def format_wallet(self, wallet: str) -> str:
+        self.check_wallet(wallet)
+
+        if utils.is_nf_domain(wallet):
+            return wallet
+
+        if utils.is_address(wallet):
+            domain = nfdomains.get_nf_domain(wallet)
+
+            if domain:
+                return domain
+
+        return super().format_wallet(wallet)
+
     def marketplace_url(self, collection_id: str = None, asset_id: str = None) -> str:
         if asset_id:
             return f"https://www.randgallery.com/algo-collection/?address={asset_id}"
 
         if collection_id:
             return f"https://randgallery.com/algo-collection/?address={collection_id}"
```

### Comparing `bookio_fetchfox-0.7.8/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.8.0/fetchfox/blockchains/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         raise NotImplementedError()
 
     @abstractmethod
     def explorer_url(self, collection_id: str = None, asset_id: str = None, tx_hash: str = None) -> str:
         raise NotImplementedError()
 
     @abstractmethod
+    def format_wallet(self, wallet: str) -> str:
+        return f"{wallet[:5]}..{wallet[-5:]}"
+
+    @abstractmethod
     def marketplace_url(self, collection_id: str = None, asset_id: str = None) -> str:
         raise NotImplementedError()
 
     @abstractmethod
     def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         raise NotImplementedError()
```

### Comparing `bookio_fetchfox-0.7.8/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.8.0/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import pytz
 
 from fetchfox.apis import bookio
 from fetchfox.apis.cardano import blockfrostio, cnfttools, handleme, jpgstore
 from fetchfox.blockchains.base import Blockchain
 from fetchfox.constants.blockchains import CARDANO
+from fetchfox.constants.cardano import ADA_HANDLE_POLICY_ID
 from fetchfox.constants.currencies import ADA
 from fetchfox.constants.marketplaces import JPG_STORE
 from fetchfox.dtos import (
     AssetDTO,
     CampaignDTO,
     FloorDTO,
     HoldingDTO,
@@ -59,14 +60,41 @@
             return f"https://cardanoscan.io/tokenPolicy/{collection_id.lower()}"
 
         if tx_hash:
             return f"https://cardanoscan.io/transaction/{collection_id.lower()}"
 
         return None
 
+    @lru_cache
+    def format_wallet(self, wallet: str) -> str:
+        self.check_wallet(wallet)
+
+        if utils.is_ada_handle(wallet):
+            return wallet
+
+        handles = []
+
+        for holding in self.get_holdings(wallet):
+            if holding.collection_id != ADA_HANDLE_POLICY_ID:
+                continue
+
+            _, name = utils.split_asset_id(holding.asset_id)
+            handles.append(name)
+
+        if handles:
+            handle = sorted(handles, key=len)[0]
+            punycode = handle.encode().decode("idna")
+
+            if handle != punycode:
+                return f"{punycode} (${handle})"
+
+            return f"${handle}"
+
+        return super().format_wallet(wallet)
+
     def marketplace_url(self, collection_id: str = None, asset_id: str = None) -> str:
         if asset_id:
             return f"https://www.jpg.store/asset/{asset_id.lower()}"
 
         if collection_id:
             return f"https://jpg.store/collection/{collection_id.lower()}"
 
@@ -176,15 +204,18 @@
             asset_id = holding["unit"]
 
             if asset_id == "lovelace":
                 continue
 
             quantity = int(holding["quantity"])
 
-            policy_id, _ = utils.split_asset_id(asset_id)
+            try:
+                policy_id, _ = utils.split_asset_id(asset_id)
+            except UnicodeDecodeError:
+                continue
 
             yield HoldingDTO(
                 collection_id=policy_id,
                 asset_id=asset_id,
                 address=stake_address,
                 quantity=quantity,
             )
```

### Comparing `bookio_fetchfox-0.7.8/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.8.0/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-0.8.0/fetchfox/blockchains/ethereum/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.8.0/fetchfox/blockchains/evm/blockchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 from datetime import datetime
+from functools import lru_cache
 from typing import Iterable
 
 import pytz
 
 from fetchfox.apis import bookio
 from fetchfox.apis.evm import moralisio, ensideascom, openseaio
 from fetchfox.blockchains.base import Blockchain
@@ -32,14 +33,29 @@
         if not utils.is_asset_id(asset_id):
             raise ValueError(f"{asset_id} is not a valid {self.name} asset id")
 
     def check_wallet(self, wallet: str):
         if not utils.is_wallet(wallet):
             raise ValueError(f"{wallet} is not a valid {self.name} address or ens domain")
 
+    @lru_cache
+    def format_wallet(self, wallet: str) -> str:
+        self.check_wallet(wallet)
+
+        if utils.is_ens_domain(wallet):
+            return wallet
+
+        if utils.is_address(wallet):
+            domain = ensideascom.get_ens_domain(wallet)
+
+            if domain:
+                return domain
+
+        return super().format_wallet(wallet)
+
     def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         self.check_collection_id(collection_id)
 
         if fetch_metadata:
             asset_id = -1
 
             while True:
@@ -267,13 +283,13 @@
                 asset_ids=[asset_id],
                 asset_names=[asset_name],
                 tx_hash=tx_hash,
                 marketplace=OPENSEA_IO,
                 price=float(int(sale["total_price"]) / 10 ** sale["payment_token"]["decimals"]),
                 currency=sale["payment_token"]["symbol"].replace("WETH", "ETH"),
                 confirmed_at=confirmed_at,
-                sold_by=sale["transaction"]["from_account"]["address"],
-                bought_by=sale["transaction"]["to_account"]["address"],
+                sold_by=sale["seller"]["address"],
+                bought_by=sale["winner_account"]["address"],
                 sale_id=sale["id"],
                 marketplace_url=marketplace_url,
                 explorer_url=explorer_url,
             )
```

### Comparing `bookio_fetchfox-0.7.8/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.8.0/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/blockchains/polygon/blockchain.py` & `bookio_fetchfox-0.8.0/fetchfox/blockchains/polygon/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.8.0/fetchfox/dtos/asset.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 class AssetDTO:
     def __init__(self, collection_id: str, asset_id: str, metadata: dict):
         self.collection_id: str = collection_id
         self.asset_id: str = asset_id
         self.metadata: dict = metadata
 
     @property
+    def name(self) -> str:
+        if "Book Title" in self.metadata:
+            return self.metadata["Book Title"][0]
+
+        return self.metadata["name"]
+
+    @property
     def title(self) -> str:
         if "Book Title" in self.metadata:
             return self.metadata["Book Title"][0]
 
         return self.metadata["name"].split(" #")[0]
 
     @property
```

### Comparing `bookio_fetchfox-0.7.8/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.8.0/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.8.0/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/dtos/sale.py` & `bookio_fetchfox-0.8.0/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/fetchfox/rest.py` & `bookio_fetchfox-0.8.0/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.8/pyproject.toml` & `bookio_fetchfox-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.7.8"
+version = "0.8.0"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-0.7.8/setup.py` & `bookio_fetchfox-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.7.8',
+    'version': '0.8.0',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-0.7.8/PKG-INFO` & `bookio_fetchfox-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.7.8
+Version: 0.8.0
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```

