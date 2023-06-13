# Comparing `tmp/btclib-2023.2.3.tar.gz` & `tmp/btclib-2023.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btclib-2023.2.3.tar", last modified: Thu Feb  2 19:11:15 2023, max compression
+gzip compressed data, was "btclib-2023.5.30.tar", last modified: Tue Jun 13 15:49:25 2023, max compression
```

## Comparing `btclib-2023.2.3.tar` & `btclib-2023.5.30.tar`

### file list

```diff
@@ -1,260 +1,260 @@
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.986217 btclib-2023.2.3/
--rw-r--r--   0 ferdi      (501) staff       (20)      741 2023-01-08 13:31:15.000000 btclib-2023.2.3/.flake8
--rw-r--r--   0 ferdi      (501) staff       (20)      485 2023-01-29 11:04:07.000000 btclib-2023.2.3/.markdownlint.jsonc
--rw-r--r--   0 ferdi      (501) staff       (20)     4895 2023-02-02 18:58:20.000000 btclib-2023.2.3/.pre-commit-config.yaml
--rw-r--r--   0 ferdi      (501) staff       (20)     1657 2023-01-08 13:31:15.000000 btclib-2023.2.3/.sourcery.yaml
--rw-r--r--   0 ferdi      (501) staff       (20)      303 2023-01-04 12:58:11.000000 btclib-2023.2.3/AUTHORS.md
--rw-r--r--   0 ferdi      (501) staff       (20)      207 2023-01-04 12:58:11.000000 btclib-2023.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 ferdi      (501) staff       (20)     5855 2023-01-08 13:31:15.000000 btclib-2023.2.3/CONTRIBUTING.md
--rw-r--r--   0 ferdi      (501) staff       (20)      341 2023-01-08 13:31:15.000000 btclib-2023.2.3/COPYRIGHT
--rw-r--r--   0 ferdi      (501) staff       (20)    11181 2023-02-02 19:01:28.000000 btclib-2023.2.3/HISTORY.md
--rw-r--r--   0 ferdi      (501) staff       (20)     1108 2023-01-08 13:31:15.000000 btclib-2023.2.3/LICENSE
--rw-r--r--   0 ferdi      (501) staff       (20)      943 2023-01-29 11:04:07.000000 btclib-2023.2.3/MANIFEST.in
--rw-r--r--   0 ferdi      (501) staff       (20)    10315 2023-02-02 19:11:15.985574 btclib-2023.2.3/PKG-INFO
--rw-r--r--   0 ferdi      (501) staff       (20)     8530 2023-01-29 11:59:25.000000 btclib-2023.2.3/README.md
--rw-r--r--   0 ferdi      (501) staff       (20)     1371 2023-01-29 11:04:07.000000 btclib-2023.2.3/RELEASE.md
--rw-r--r--   0 ferdi      (501) staff       (20)      187 2023-01-08 13:31:15.000000 btclib-2023.2.3/SECURITY.md
--rw-r--r--   0 ferdi      (501) staff       (20)     1639 2023-01-08 13:31:15.000000 btclib-2023.2.3/TODO.md
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.541886 btclib-2023.2.3/btclib/
--rw-r--r--   0 ferdi      (501) staff       (20)      620 2023-02-02 19:02:25.000000 btclib-2023.2.3/btclib/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.545735 btclib-2023.2.3/btclib/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)      598 2023-01-08 13:31:15.000000 btclib-2023.2.3/btclib/_data/mainnet.json
--rw-r--r--   0 ferdi      (501) staff       (20)      600 2023-01-08 13:31:15.000000 btclib-2023.2.3/btclib/_data/regtest.json
--rw-r--r--   0 ferdi      (501) staff       (20)      598 2023-01-08 13:31:15.000000 btclib-2023.2.3/btclib/_data/testnet.json
--rw-r--r--   0 ferdi      (501) staff       (20)     3543 2023-02-02 18:10:53.000000 btclib-2023.2.3/btclib/alias.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3901 2023-01-29 11:04:07.000000 btclib-2023.2.3/btclib/amount.py
--rw-r--r--   0 ferdi      (501) staff       (20)     6479 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/b32.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4567 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/b58.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4308 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/base58.py
--rw-r--r--   0 ferdi      (501) staff       (20)     5727 2023-02-02 17:51:50.000000 btclib-2023.2.3/btclib/bech32.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.549437 btclib-2023.2.3/btclib/bip32/
--rw-r--r--   0 ferdi      (501) staff       (20)     1380 2023-01-29 20:16:00.000000 btclib-2023.2.3/btclib/bip32/__init__.py
--rw-r--r--   0 ferdi      (501) staff       (20)    16540 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/bip32/bip32.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3737 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/bip32/der_path.py
--rw-r--r--   0 ferdi      (501) staff       (20)     5735 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/bip32/key_origin.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3879 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/bip32/slip132.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.551626 btclib-2023.2.3/btclib/block/
--rw-r--r--   0 ferdi      (501) staff       (20)      515 2023-01-29 20:16:06.000000 btclib-2023.2.3/btclib/block/__init__.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4968 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/block/block.py
--rw-r--r--   0 ferdi      (501) staff       (20)     7448 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/block/block_header.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.557340 btclib-2023.2.3/btclib/ec/
--rw-r--r--   0 ferdi      (501) staff       (20)     1553 2023-01-29 20:16:06.000000 btclib-2023.2.3/btclib/ec/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.560952 btclib-2023.2.3/btclib/ec/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)     4102 2023-01-08 13:31:15.000000 btclib-2023.2.3/btclib/ec/_data/ec_Brainpool.json
--rw-r--r--   0 ferdi      (501) staff       (20)     3105 2023-01-08 13:31:15.000000 btclib-2023.2.3/btclib/ec/_data/ec_NIST.json
--rw-r--r--   0 ferdi      (501) staff       (20)     2403 2023-01-08 13:31:15.000000 btclib-2023.2.3/btclib/ec/_data/ec_SEC2v1_insecure.json
--rw-r--r--   0 ferdi      (501) staff       (20)     4233 2023-01-08 13:31:15.000000 btclib-2023.2.3/btclib/ec/_data/ec_SEC2v2.json
--rw-r--r--   0 ferdi      (501) staff       (20)     8771 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/ec/curve.py
--rw-r--r--   0 ferdi      (501) staff       (20)    25183 2023-02-01 10:31:36.000000 btclib-2023.2.3/btclib/ec/curve_group.py
--rw-r--r--   0 ferdi      (501) staff       (20)     8183 2023-01-29 11:04:07.000000 btclib-2023.2.3/btclib/ec/curve_group_2.py
--rw-r--r--   0 ferdi      (501) staff       (20)     1727 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/ec/curve_group_f.py
--rw-r--r--   0 ferdi      (501) staff       (20)     2495 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/ec/libsecp256k1.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3069 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/ec/sec_point.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.570250 btclib-2023.2.3/btclib/ecc/
--rw-r--r--   0 ferdi      (501) staff       (20)      633 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/ecc/__init__.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3593 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/ecc/bip340_nonce.py
--rw-r--r--   0 ferdi      (501) staff       (20)    14412 2023-01-29 11:59:25.000000 btclib-2023.2.3/btclib/ecc/bms.py
--rw-r--r--   0 ferdi      (501) staff       (20)     6124 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/ecc/borromean.py
--rw-r--r--   0 ferdi      (501) staff       (20)     2615 2023-02-01 10:31:36.000000 btclib-2023.2.3/btclib/ecc/dh.py
--rw-r--r--   0 ferdi      (501) staff       (20)    19859 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/ecc/dsa.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4291 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/ecc/libsecp256k1.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3272 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/ecc/pedersen.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4441 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/ecc/rfc6979_nonce.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4466 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/ecc/sign_to_contract.py
--rw-r--r--   0 ferdi      (501) staff       (20)    15087 2023-01-29 11:59:25.000000 btclib-2023.2.3/btclib/ecc/ssa.py
--rw-r--r--   0 ferdi      (501) staff       (20)      795 2023-01-08 22:03:08.000000 btclib-2023.2.3/btclib/exceptions.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3126 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/hashes.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.575422 btclib-2023.2.3/btclib/mnemonic/
--rw-r--r--   0 ferdi      (501) staff       (20)     1389 2023-01-08 19:50:07.000000 btclib-2023.2.3/btclib/mnemonic/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.577299 btclib-2023.2.3/btclib/mnemonic/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)    13116 2023-01-04 12:58:11.000000 btclib-2023.2.3/btclib/mnemonic/_data/english.txt
--rw-r--r--   0 ferdi      (501) staff       (20)    16033 2023-01-04 12:58:11.000000 btclib-2023.2.3/btclib/mnemonic/_data/italian.txt
--rw-r--r--   0 ferdi      (501) staff       (20)     5312 2023-01-15 17:27:11.000000 btclib-2023.2.3/btclib/mnemonic/bip39.py
--rw-r--r--   0 ferdi      (501) staff       (20)     5430 2023-01-15 17:27:17.000000 btclib-2023.2.3/btclib/mnemonic/electrum.py
--rw-r--r--   0 ferdi      (501) staff       (20)    11856 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/mnemonic/entropy.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4287 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/mnemonic/mnemonic.py
--rw-r--r--   0 ferdi      (501) staff       (20)     9348 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/network.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4972 2023-02-01 10:31:36.000000 btclib-2023.2.3/btclib/number_theory.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.583828 btclib-2023.2.3/btclib/psbt/
--rw-r--r--   0 ferdi      (501) staff       (20)     1237 2023-01-09 19:07:38.000000 btclib-2023.2.3/btclib/psbt/__init__.py
--rw-r--r--   0 ferdi      (501) staff       (20)    20538 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/psbt/psbt.py
--rw-r--r--   0 ferdi      (501) staff       (20)    16086 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/psbt/psbt_in.py
--rw-r--r--   0 ferdi      (501) staff       (20)     5294 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/psbt/psbt_out.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4837 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/psbt/psbt_utils.py
--rw-r--r--   0 ferdi      (501) staff       (20)       27 2023-01-04 12:58:11.000000 btclib-2023.2.3/btclib/py.typed
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.589130 btclib-2023.2.3/btclib/script/
--rw-r--r--   0 ferdi      (501) staff       (20)     1565 2023-01-08 14:26:09.000000 btclib-2023.2.3/btclib/script/__init__.py
--rw-r--r--   0 ferdi      (501) staff       (20)    11000 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/script/script.py
--rw-r--r--   0 ferdi      (501) staff       (20)    17561 2023-02-02 17:59:04.000000 btclib-2023.2.3/btclib/script/script_pub_key.py
--rw-r--r--   0 ferdi      (501) staff       (20)     9678 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/script/sig_hash.py
--rw-r--r--   0 ferdi      (501) staff       (20)     5502 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/script/taproot.py
--rw-r--r--   0 ferdi      (501) staff       (20)     2305 2023-02-02 18:06:50.000000 btclib-2023.2.3/btclib/script/witness.py
--rw-r--r--   0 ferdi      (501) staff       (20)     7024 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/to_prv_key.py
--rw-r--r--   0 ferdi      (501) staff       (20)     7908 2023-01-16 13:28:33.000000 btclib-2023.2.3/btclib/to_pub_key.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.593673 btclib-2023.2.3/btclib/tx/
--rw-r--r--   0 ferdi      (501) staff       (20)      597 2023-01-09 19:07:38.000000 btclib-2023.2.3/btclib/tx/__init__.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3263 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/tx/out_point.py
--rw-r--r--   0 ferdi      (501) staff       (20)    10197 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/tx/tx.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4582 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/tx/tx_in.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4045 2023-02-02 18:58:20.000000 btclib-2023.2.3/btclib/tx/tx_out.py
--rw-r--r--   0 ferdi      (501) staff       (20)     6075 2023-01-29 11:59:25.000000 btclib-2023.2.3/btclib/utils.py
--rw-r--r--   0 ferdi      (501) staff       (20)     1237 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/var_bytes.py
--rw-r--r--   0 ferdi      (501) staff       (20)     2702 2023-01-09 16:39:32.000000 btclib-2023.2.3/btclib/var_int.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.544299 btclib-2023.2.3/btclib.egg-info/
--rw-r--r--   0 ferdi      (501) staff       (20)    10315 2023-02-02 19:11:15.000000 btclib-2023.2.3/btclib.egg-info/PKG-INFO
--rw-r--r--   0 ferdi      (501) staff       (20)     5778 2023-02-02 19:11:15.000000 btclib-2023.2.3/btclib.egg-info/SOURCES.txt
--rw-r--r--   0 ferdi      (501) staff       (20)        1 2023-02-02 19:11:15.000000 btclib-2023.2.3/btclib.egg-info/dependency_links.txt
--rw-r--r--   0 ferdi      (501) staff       (20)       20 2023-02-02 19:11:15.000000 btclib-2023.2.3/btclib.egg-info/requires.txt
--rw-r--r--   0 ferdi      (501) staff       (20)        7 2023-02-02 19:11:15.000000 btclib-2023.2.3/btclib.egg-info/top_level.txt
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.597206 btclib-2023.2.3/docs/
--rw-r--r--   0 ferdi      (501) staff       (20)      638 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/Makefile
--rw-r--r--   0 ferdi      (501) staff       (20)     1777 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/README.rst
--rw-r--r--   0 ferdi      (501) staff       (20)      804 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/make.bat
--rw-r--r--   0 ferdi      (501) staff       (20)       43 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/requirements.txt
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.611445 btclib-2023.2.3/docs/source/
--rw-r--r--   0 ferdi      (501) staff       (20)      788 2023-01-17 08:50:31.000000 btclib-2023.2.3/docs/source/btclib.bip32.rst
--rw-r--r--   0 ferdi      (501) staff       (20)      491 2023-01-17 08:50:31.000000 btclib-2023.2.3/docs/source/btclib.block.rst
--rw-r--r--   0 ferdi      (501) staff       (20)     1088 2023-01-17 08:50:31.000000 btclib-2023.2.3/docs/source/btclib.ec.rst
--rw-r--r--   0 ferdi      (501) staff       (20)     1647 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/source/btclib.ecc.rst
--rw-r--r--   0 ferdi      (501) staff       (20)      823 2023-01-17 08:50:31.000000 btclib-2023.2.3/docs/source/btclib.mnemonic.rst
--rw-r--r--   0 ferdi      (501) staff       (20)      772 2023-01-17 08:50:31.000000 btclib-2023.2.3/docs/source/btclib.psbt.rst
--rw-r--r--   0 ferdi      (501) staff       (20)     2325 2023-01-17 09:45:30.000000 btclib-2023.2.3/docs/source/btclib.rst
--rw-r--r--   0 ferdi      (501) staff       (20)      972 2023-01-17 08:50:31.000000 btclib-2023.2.3/docs/source/btclib.script.rst
--rw-r--r--   0 ferdi      (501) staff       (20)      721 2023-01-17 08:50:31.000000 btclib-2023.2.3/docs/source/btclib.tx.rst
--rw-r--r--   0 ferdi      (501) staff       (20)     2147 2023-02-02 19:02:25.000000 btclib-2023.2.3/docs/source/conf.py
--rw-r--r--   0 ferdi      (501) staff       (20)      157 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/source/contributing_link.md
--rw-r--r--   0 ferdi      (501) staff       (20)      105 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/source/history_link.md
--rw-r--r--   0 ferdi      (501) staff       (20)      508 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/source/index.rst
--rw-r--r--   0 ferdi      (501) staff       (20)       55 2023-01-28 20:20:32.000000 btclib-2023.2.3/docs/source/modules.rst
--rw-r--r--   0 ferdi      (501) staff       (20)      151 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/source/readme_link.md
--rw-r--r--   0 ferdi      (501) staff       (20)      153 2023-01-29 11:04:07.000000 btclib-2023.2.3/docs/source/security_link.md
--rw-r--r--   0 ferdi      (501) staff       (20)     1380 2023-02-02 18:58:20.000000 btclib-2023.2.3/pyproject.toml
--rw-r--r--   0 ferdi      (501) staff       (20)      318 2023-01-08 13:31:15.000000 btclib-2023.2.3/readthedocs.yml
--rw-r--r--   0 ferdi      (501) staff       (20)      299 2023-01-09 00:56:27.000000 btclib-2023.2.3/requirements-dev.txt
--rw-r--r--   0 ferdi      (501) staff       (20)       41 2023-02-01 10:13:56.000000 btclib-2023.2.3/requirements.txt
--rw-r--r--   0 ferdi      (501) staff       (20)       38 2023-02-02 19:11:15.986357 btclib-2023.2.3/setup.cfg
--rw-r--r--   0 ferdi      (501) staff       (20)     2705 2023-02-02 18:58:20.000000 btclib-2023.2.3/setup.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.629548 btclib-2023.2.3/tests/
--rw-r--r--   0 ferdi      (501) staff       (20)     1036 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/README.md
--rw-r--r--   0 ferdi      (501) staff       (20)      405 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.633396 btclib-2023.2.3/tests/_generated_files/
--rw-r--r--   0 ferdi      (501) staff       (20)      598 2023-02-02 19:07:44.000000 btclib-2023.2.3/tests/_generated_files/mainnet.json
--rw-r--r--   0 ferdi      (501) staff       (20)      600 2023-02-02 19:07:44.000000 btclib-2023.2.3/tests/_generated_files/regtest.json
--rw-r--r--   0 ferdi      (501) staff       (20)      598 2023-02-02 19:07:44.000000 btclib-2023.2.3/tests/_generated_files/testnet.json
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.643345 btclib-2023.2.3/tests/bip32/
--rw-r--r--   0 ferdi      (501) staff       (20)      411 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/bip32/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.648409 btclib-2023.2.3/tests/bip32/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)     3151 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/bip32/_data/bip32_invalid_keys.json
--rw-r--r--   0 ferdi      (501) staff       (20)     5515 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/bip32/_data/bip32_test_vectors.json
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.651335 btclib-2023.2.3/tests/bip32/_generated_files/
--rw-r--r--   0 ferdi      (501) staff       (20)       73 2023-02-02 19:07:44.000000 btclib-2023.2.3/tests/bip32/_generated_files/key_origin.json
--rw-r--r--   0 ferdi      (501) staff       (20)      625 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/bip32/_generated_files/key_paths.json
--rw-r--r--   0 ferdi      (501) staff       (20)    13984 2023-01-29 11:04:07.000000 btclib-2023.2.3/tests/bip32/test_bip32.py
--rw-r--r--   0 ferdi      (501) staff       (20)     5027 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/bip32/test_der_path.py
--rw-r--r--   0 ferdi      (501) staff       (20)     5185 2023-01-09 19:07:38.000000 btclib-2023.2.3/tests/bip32/test_key_origin.py
--rw-r--r--   0 ferdi      (501) staff       (20)     9595 2023-02-02 18:58:20.000000 btclib-2023.2.3/tests/bip32/test_slip132.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.653720 btclib-2023.2.3/tests/block/
--rw-r--r--   0 ferdi      (501) staff       (20)      411 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/block/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.663763 btclib-2023.2.3/tests/block/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)      215 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/block/_data/block_1.bin
--rw-r--r--   0 ferdi      (501) staff       (20)      490 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/block/_data/block_170.bin
--rw-r--r--   0 ferdi      (501) staff       (20)   247533 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/block/_data/block_200000.bin
--rw-r--r--   0 ferdi      (501) staff       (20)   988519 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/block/_data/block_481824.bin
--rw-r--r--   0 ferdi      (501) staff       (20)   989323 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/block/_data/block_481824_complete.bin
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.730062 btclib-2023.2.3/tests/block/_generated_files/
--rw-r--r--   0 ferdi      (501) staff       (20)  5738930 2023-02-02 19:07:48.000000 btclib-2023.2.3/tests/block/_generated_files/block_481824.json
--rw-r--r--   0 ferdi      (501) staff       (20)      419 2023-02-02 19:07:49.000000 btclib-2023.2.3/tests/block/_generated_files/block_header_481824.json
--rw-r--r--   0 ferdi      (501) staff       (20)    10561 2023-01-29 11:04:07.000000 btclib-2023.2.3/tests/block/test_block.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.759691 btclib-2023.2.3/tests/ec/
--rw-r--r--   0 ferdi      (501) staff       (20)      408 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/ec/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.764455 btclib-2023.2.3/tests/ec/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)   126364 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/ec/_data/pubkey.json
--rw-r--r--   0 ferdi      (501) staff       (20)    15648 2023-02-02 18:58:20.000000 btclib-2023.2.3/tests/ec/test_curve.py
--rw-r--r--   0 ferdi      (501) staff       (20)    15426 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/ec/test_curve_group.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4271 2023-01-08 19:50:07.000000 btclib-2023.2.3/tests/ec/test_curve_group_2.py
--rw-r--r--   0 ferdi      (501) staff       (20)     2179 2023-01-08 19:50:07.000000 btclib-2023.2.3/tests/ec/test_curve_group_f.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4813 2023-02-02 18:58:20.000000 btclib-2023.2.3/tests/ec/test_sec_point.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.815813 btclib-2023.2.3/tests/ecc/
--rw-r--r--   0 ferdi      (501) staff       (20)      409 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/ecc/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.824405 btclib-2023.2.3/tests/ecc/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)     5161 2023-01-04 12:58:11.000000 btclib-2023.2.3/tests/ecc/_data/bip340_test_vectors.csv
--rw-r--r--   0 ferdi      (501) staff       (20)    50597 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/ecc/_data/bms.json
--rw-r--r--   0 ferdi      (501) staff       (20)    89766 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/ecc/_data/ecdsa_custom_nonce_sig.json
--rw-r--r--   0 ferdi      (501) staff       (20)    72463 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/ecc/_data/ecdsa_sig.json
--rw-r--r--   0 ferdi      (501) staff       (20)    31685 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/ecc/_data/rfc6979.json
--rw-r--r--   0 ferdi      (501) staff       (20)    27857 2023-01-29 11:04:07.000000 btclib-2023.2.3/tests/ecc/test_bms.py
--rw-r--r--   0 ferdi      (501) staff       (20)     1484 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/ecc/test_borromean.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3887 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/ecc/test_der.py
--rw-r--r--   0 ferdi      (501) staff       (20)    29798 2023-01-29 11:04:07.000000 btclib-2023.2.3/tests/ecc/test_dh.py
--rw-r--r--   0 ferdi      (501) staff       (20)    13268 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/ecc/test_dsa.py
--rw-r--r--   0 ferdi      (501) staff       (20)     2002 2023-01-29 11:04:07.000000 btclib-2023.2.3/tests/ecc/test_pedersen.py
--rw-r--r--   0 ferdi      (501) staff       (20)     2925 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/ecc/test_rfc6979.py
--rw-r--r--   0 ferdi      (501) staff       (20)     1508 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/ecc/test_sign_to_contract.py
--rw-r--r--   0 ferdi      (501) staff       (20)    25964 2023-01-29 11:04:07.000000 btclib-2023.2.3/tests/ecc/test_ssa.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.831714 btclib-2023.2.3/tests/mnemonic/
--rw-r--r--   0 ferdi      (501) staff       (20)      414 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/mnemonic/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.836678 btclib-2023.2.3/tests/mnemonic/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)    12193 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/mnemonic/_data/bip39_test_vectors.json
--rw-r--r--   0 ferdi      (501) staff       (20)     2751 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/mnemonic/_data/electrum_test_vectors.json
--rw-r--r--   0 ferdi      (501) staff       (20)    13116 2023-01-04 12:58:11.000000 btclib-2023.2.3/tests/mnemonic/_data/english.txt
--rw-r--r--   0 ferdi      (501) staff       (20)    13108 2023-01-04 12:58:11.000000 btclib-2023.2.3/tests/mnemonic/_data/fakeenglish.txt
--rw-r--r--   0 ferdi      (501) staff       (20)     3001 2023-01-15 18:09:45.000000 btclib-2023.2.3/tests/mnemonic/test_bip39.py
--rw-r--r--   0 ferdi      (501) staff       (20)     5192 2023-01-29 11:04:07.000000 btclib-2023.2.3/tests/mnemonic/test_electrum.py
--rw-r--r--   0 ferdi      (501) staff       (20)    10689 2023-01-15 18:09:45.000000 btclib-2023.2.3/tests/mnemonic/test_entropy.py
--rw-r--r--   0 ferdi      (501) staff       (20)     1952 2023-01-08 19:50:07.000000 btclib-2023.2.3/tests/mnemonic/test_mnemonic.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.842058 btclib-2023.2.3/tests/psbt/
--rw-r--r--   0 ferdi      (501) staff       (20)      410 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/psbt/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.843207 btclib-2023.2.3/tests/psbt/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)    29762 2023-01-04 12:58:11.000000 btclib-2023.2.3/tests/psbt/_data/bip174_test_vectors.json
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.847493 btclib-2023.2.3/tests/psbt/_generated_files/
--rw-r--r--   0 ferdi      (501) staff       (20)     8273 2023-02-02 19:07:47.000000 btclib-2023.2.3/tests/psbt/_generated_files/psbt.json
--rw-r--r--   0 ferdi      (501) staff       (20)     2943 2023-02-02 19:07:47.000000 btclib-2023.2.3/tests/psbt/_generated_files/psbt_in.json
--rw-r--r--   0 ferdi      (501) staff       (20)      294 2023-02-02 19:07:47.000000 btclib-2023.2.3/tests/psbt/_generated_files/psbt_out.json
--rw-r--r--   0 ferdi      (501) staff       (20)    70300 2023-01-29 11:04:07.000000 btclib-2023.2.3/tests/psbt/test_psbt.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3597 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/psbt/test_psbt_in.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4404 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/psbt/test_psbt_out.py
--rw-r--r--   0 ferdi      (501) staff       (20)      736 2023-01-09 00:56:27.000000 btclib-2023.2.3/tests/psbt/test_psbt_utils.py
--rw-r--r--   0 ferdi      (501) staff       (20)       27 2023-01-08 19:50:07.000000 btclib-2023.2.3/tests/py.typed
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.916539 btclib-2023.2.3/tests/script/
--rw-r--r--   0 ferdi      (501) staff       (20)      412 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/script/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.945887 btclib-2023.2.3/tests/script/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)     1648 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/script/_data/bip67_test_vectors.json
--rw-r--r--   0 ferdi      (501) staff       (20)   210483 2023-01-04 12:58:11.000000 btclib-2023.2.3/tests/script/_data/sig_hash_legacy_test_vectors.json
--rw-r--r--   0 ferdi      (501) staff       (20)    29296 2023-01-04 12:58:11.000000 btclib-2023.2.3/tests/script/_data/taproot_test_vector.json
--rw-r--r--   0 ferdi      (501) staff       (20)  9242563 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/script/_data/tapscript_test_vector.json
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.968982 btclib-2023.2.3/tests/script/_generated_files/
--rw-r--r--   0 ferdi      (501) staff       (20)     1100 2023-02-02 19:07:48.000000 btclib-2023.2.3/tests/script/_generated_files/witness.json
--rw-r--r--   0 ferdi      (501) staff       (20)     8330 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/script/test_script.py
--rw-r--r--   0 ferdi      (501) staff       (20)    23479 2023-02-02 18:58:20.000000 btclib-2023.2.3/tests/script/test_script_pub_key.py
--rw-r--r--   0 ferdi      (501) staff       (20)     8217 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/script/test_sig_hash_legacy.py
--rw-r--r--   0 ferdi      (501) staff       (20)     6958 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/script/test_sig_hash_segwitv0.py
--rw-r--r--   0 ferdi      (501) staff       (20)     8476 2023-02-02 18:58:20.000000 btclib-2023.2.3/tests/script/test_sig_hash_taproot.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4300 2023-02-02 18:58:20.000000 btclib-2023.2.3/tests/script/test_taproot.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4368 2023-01-08 19:50:07.000000 btclib-2023.2.3/tests/script/test_witness.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3719 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/test_amount.py
--rw-r--r--   0 ferdi      (501) staff       (20)    12407 2023-02-02 18:58:20.000000 btclib-2023.2.3/tests/test_b32.py
--rw-r--r--   0 ferdi      (501) staff       (20)    10234 2023-02-02 18:58:20.000000 btclib-2023.2.3/tests/test_b58.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3725 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/test_base58.py
--rw-r--r--   0 ferdi      (501) staff       (20)     6531 2023-01-29 11:04:07.000000 btclib-2023.2.3/tests/test_bech32.py
--rw-r--r--   0 ferdi      (501) staff       (20)      847 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/test_hashes.py
--rw-r--r--   0 ferdi      (501) staff       (20)     2761 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/test_network.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3615 2023-01-09 00:56:27.000000 btclib-2023.2.3/tests/test_number_theory.py
--rw-r--r--   0 ferdi      (501) staff       (20)    11489 2023-01-08 22:03:08.000000 btclib-2023.2.3/tests/test_to_key.py
--rw-r--r--   0 ferdi      (501) staff       (20)     5844 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/test_to_prv_key.py
--rw-r--r--   0 ferdi      (501) staff       (20)     9749 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/test_to_pub_key.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3073 2023-01-16 13:28:33.000000 btclib-2023.2.3/tests/test_utils.py
--rw-r--r--   0 ferdi      (501) staff       (20)     2060 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/test_var_int.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.977537 btclib-2023.2.3/tests/tx/
--rw-r--r--   0 ferdi      (501) staff       (20)      408 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/tx/__init__.py
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.978067 btclib-2023.2.3/tests/tx/_data/
--rw-r--r--   0 ferdi      (501) staff       (20)     4740 2023-01-04 12:58:11.000000 btclib-2023.2.3/tests/tx/_data/d4f3c2c3c218be868c77ae31bedb497e2f908d6ee5bbbe91e4933e6da680c970.bin
-drwxr-xr-x   0 ferdi      (501) staff       (20)        0 2023-02-02 19:11:15.984556 btclib-2023.2.3/tests/tx/_generated_files/
--rw-r--r--   0 ferdi      (501) staff       (20)       98 2023-02-02 19:07:48.000000 btclib-2023.2.3/tests/tx/_generated_files/out_point.json
--rw-r--r--   0 ferdi      (501) staff       (20)    12973 2023-02-02 19:07:48.000000 btclib-2023.2.3/tests/tx/_generated_files/tx.json
--rw-r--r--   0 ferdi      (501) staff       (20)     1392 2023-02-02 19:07:48.000000 btclib-2023.2.3/tests/tx/_generated_files/tx_in.json
--rw-r--r--   0 ferdi      (501) staff       (20)      289 2023-02-02 19:07:48.000000 btclib-2023.2.3/tests/tx/_generated_files/tx_out.json
--rw-r--r--   0 ferdi      (501) staff       (20)     3440 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/tx/test_out_point.py
--rw-r--r--   0 ferdi      (501) staff       (20)    20493 2023-01-09 19:07:38.000000 btclib-2023.2.3/tests/tx/test_tx.py
--rw-r--r--   0 ferdi      (501) staff       (20)     4547 2023-01-08 13:31:15.000000 btclib-2023.2.3/tests/tx/test_tx_in.py
--rw-r--r--   0 ferdi      (501) staff       (20)     3558 2023-01-09 16:39:32.000000 btclib-2023.2.3/tests/tx/test_tx_out.py
--rw-r--r--   0 ferdi      (501) staff       (20)      409 2023-02-02 18:58:20.000000 btclib-2023.2.3/tox.ini
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:25.001772 btclib-2023.5.30/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      741 2023-02-07 11:12:07.000000 btclib-2023.5.30/.flake8
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      485 2023-02-07 11:12:07.000000 btclib-2023.5.30/.markdownlint.jsonc
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4894 2023-06-13 15:45:45.000000 btclib-2023.5.30/.pre-commit-config.yaml
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1657 2023-02-07 11:12:07.000000 btclib-2023.5.30/.sourcery.yaml
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      303 2022-07-04 10:37:33.000000 btclib-2023.5.30/AUTHORS.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      207 2022-07-04 10:37:33.000000 btclib-2023.5.30/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5855 2023-02-07 11:12:07.000000 btclib-2023.5.30/CONTRIBUTING.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      341 2023-02-07 11:12:07.000000 btclib-2023.5.30/COPYRIGHT
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    11354 2023-06-13 15:39:58.000000 btclib-2023.5.30/HISTORY.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1108 2023-02-07 11:12:07.000000 btclib-2023.5.30/LICENSE
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      943 2023-02-07 11:12:07.000000 btclib-2023.5.30/MANIFEST.in
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10316 2023-06-13 15:49:25.001772 btclib-2023.5.30/PKG-INFO
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8530 2023-02-07 11:12:07.000000 btclib-2023.5.30/README.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1371 2023-02-07 11:12:07.000000 btclib-2023.5.30/RELEASE.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      187 2023-02-07 11:12:07.000000 btclib-2023.5.30/SECURITY.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1639 2023-06-13 15:39:52.000000 btclib-2023.5.30/TODO.md
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.889772 btclib-2023.5.30/btclib/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      621 2023-06-13 15:39:58.000000 btclib-2023.5.30/btclib/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.889772 btclib-2023.5.30/btclib/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/_data/mainnet.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      600 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/_data/regtest.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/_data/testnet.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3823 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/alias.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3901 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/amount.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6291 2023-06-13 15:39:58.000000 btclib-2023.5.30/btclib/b32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4567 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/b58.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4308 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/base58.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5727 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bech32.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.893772 btclib-2023.5.30/btclib/bip32/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1380 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    16582 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/bip32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3737 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/der_path.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5735 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/key_origin.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3879 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/bip32/slip132.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.893772 btclib-2023.5.30/btclib/block/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      515 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/block/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4968 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/block/block.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     7448 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/block/block_header.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.893772 btclib-2023.5.30/btclib/ec/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1553 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.893772 btclib-2023.5.30/btclib/ec/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4102 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/_data/ec_Brainpool.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3105 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/_data/ec_NIST.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2403 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/_data/ec_SEC2v1_insecure.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4233 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/_data/ec_SEC2v2.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8771 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/curve.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    25244 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/curve_group.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8183 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/curve_group_2.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1727 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/curve_group_f.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2495 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/libsecp256k1.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3069 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ec/sec_point.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.897772 btclib-2023.5.30/btclib/ecc/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      633 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3593 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/bip340_nonce.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    14412 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/bms.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6124 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/borromean.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2615 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/dh.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    19859 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/dsa.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4291 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/libsecp256k1.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3272 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/pedersen.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4441 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/rfc6979_nonce.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4466 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/sign_to_contract.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    15087 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/ecc/ssa.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      795 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/exceptions.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3089 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/hashes.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.897772 btclib-2023.5.30/btclib/mnemonic/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1389 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.897772 btclib-2023.5.30/btclib/mnemonic/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13116 2022-07-04 10:37:33.000000 btclib-2023.5.30/btclib/mnemonic/_data/english.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    16033 2022-07-04 10:37:33.000000 btclib-2023.5.30/btclib/mnemonic/_data/italian.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5312 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/bip39.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5430 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/electrum.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    11856 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/entropy.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4287 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/mnemonic/mnemonic.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     9348 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/network.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4972 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/number_theory.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.897772 btclib-2023.5.30/btclib/psbt/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1237 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/psbt/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    20538 2023-05-11 14:15:22.000000 btclib-2023.5.30/btclib/psbt/psbt.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    16086 2023-06-13 15:39:52.000000 btclib-2023.5.30/btclib/psbt/psbt_in.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5294 2023-06-13 15:39:52.000000 btclib-2023.5.30/btclib/psbt/psbt_out.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4837 2023-06-13 15:39:52.000000 btclib-2023.5.30/btclib/psbt/psbt_utils.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       27 2022-07-04 10:37:33.000000 btclib-2023.5.30/btclib/py.typed
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.901772 btclib-2023.5.30/btclib/script/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1565 2023-06-13 15:39:58.000000 btclib-2023.5.30/btclib/script/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    11000 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/script/script.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    17561 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/script/script_pub_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     9678 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/script/sig_hash.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5270 2023-06-13 15:39:52.000000 btclib-2023.5.30/btclib/script/taproot.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2305 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/script/witness.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     7024 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/to_prv_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     7908 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/to_pub_key.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.901772 btclib-2023.5.30/btclib/tx/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      597 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/__init__.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3263 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/out_point.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10363 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/tx.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4582 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/tx_in.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4045 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/tx/tx_out.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6075 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/utils.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1237 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/var_bytes.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2702 2023-02-07 11:12:07.000000 btclib-2023.5.30/btclib/var_int.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.889772 btclib-2023.5.30/btclib.egg-info/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10316 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/PKG-INFO
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5778 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/SOURCES.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)        1 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/dependency_links.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       20 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/requires.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)        7 2023-06-13 15:49:24.000000 btclib-2023.5.30/btclib.egg-info/top_level.txt
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.901772 btclib-2023.5.30/docs/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      638 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/Makefile
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1777 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/README.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      804 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/make.bat
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       43 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/requirements.txt
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.909772 btclib-2023.5.30/docs/source/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      788 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/btclib.bip32.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      491 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.block.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1088 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.ec.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1647 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.ecc.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      823 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/btclib.mnemonic.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      772 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/btclib.psbt.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2325 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      972 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/btclib.script.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      721 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/btclib.tx.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2148 2023-06-13 15:39:58.000000 btclib-2023.5.30/docs/source/conf.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      157 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/contributing_link.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      105 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/history_link.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      508 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/index.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       55 2022-07-04 10:37:33.000000 btclib-2023.5.30/docs/source/modules.rst
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      151 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/readme_link.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      153 2023-02-07 11:12:07.000000 btclib-2023.5.30/docs/source/security_link.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1380 2023-02-07 11:12:07.000000 btclib-2023.5.30/pyproject.toml
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      318 2023-02-07 11:12:07.000000 btclib-2023.5.30/readthedocs.yml
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      299 2023-02-07 11:12:07.000000 btclib-2023.5.30/requirements-dev.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       41 2023-02-07 11:12:07.000000 btclib-2023.5.30/requirements.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       38 2023-06-13 15:49:25.001772 btclib-2023.5.30/setup.cfg
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2705 2023-02-07 11:12:07.000000 btclib-2023.5.30/setup.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.913772 btclib-2023.5.30/tests/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1036 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/README.md
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      405 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.913772 btclib-2023.5.30/tests/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-05-11 14:09:52.000000 btclib-2023.5.30/tests/_generated_files/mainnet.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      600 2023-05-11 14:09:52.000000 btclib-2023.5.30/tests/_generated_files/regtest.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      598 2023-05-11 14:09:52.000000 btclib-2023.5.30/tests/_generated_files/testnet.json
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.917772 btclib-2023.5.30/tests/bip32/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      411 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.917772 btclib-2023.5.30/tests/bip32/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3151 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/_data/bip32_invalid_keys.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5515 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/_data/bip32_test_vectors.json
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.917772 btclib-2023.5.30/tests/bip32/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       73 2023-05-11 14:09:52.000000 btclib-2023.5.30/tests/bip32/_generated_files/key_origin.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      625 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/_generated_files/key_paths.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    14054 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/test_bip32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5027 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/test_der_path.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5185 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/test_key_origin.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     9595 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/bip32/test_slip132.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.917772 btclib-2023.5.30/tests/block/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      411 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.925772 btclib-2023.5.30/tests/block/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      215 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_1.bin
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      490 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_170.bin
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   247533 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_200000.bin
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   988519 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_481824.bin
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   989323 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/_data/block_481824_complete.bin
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.945772 btclib-2023.5.30/tests/block/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)  5738930 2023-05-11 14:09:55.000000 btclib-2023.5.30/tests/block/_generated_files/block_481824.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      419 2023-05-11 14:09:55.000000 btclib-2023.5.30/tests/block/_generated_files/block_header_481824.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10561 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/block/test_block.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.949772 btclib-2023.5.30/tests/ec/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      408 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.949772 btclib-2023.5.30/tests/ec/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   126364 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/_data/pubkey.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    15648 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_curve.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    15426 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_curve_group.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4271 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_curve_group_2.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2179 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_curve_group_f.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4813 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ec/test_sec_point.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.953772 btclib-2023.5.30/tests/ecc/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      409 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.957772 btclib-2023.5.30/tests/ecc/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5161 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/ecc/_data/bip340_test_vectors.csv
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    50597 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/_data/bms.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    89766 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/_data/ecdsa_custom_nonce_sig.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    72463 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/_data/ecdsa_sig.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    31685 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/_data/rfc6979.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    27857 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_bms.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1484 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_borromean.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3887 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_der.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    29798 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_dh.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13268 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_dsa.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2002 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_pedersen.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2925 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_rfc6979.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1508 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_sign_to_contract.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    25964 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/ecc/test_ssa.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.957772 btclib-2023.5.30/tests/mnemonic/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      414 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.961772 btclib-2023.5.30/tests/mnemonic/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    12193 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/_data/bip39_test_vectors.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2751 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/_data/electrum_test_vectors.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13116 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/mnemonic/_data/english.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    13108 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/mnemonic/_data/fakeenglish.txt
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3001 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/test_bip39.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5192 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/test_electrum.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10689 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/test_entropy.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1952 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/mnemonic/test_mnemonic.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.961772 btclib-2023.5.30/tests/psbt/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      410 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/psbt/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.961772 btclib-2023.5.30/tests/psbt/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    29762 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/psbt/_data/bip174_test_vectors.json
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.961772 btclib-2023.5.30/tests/psbt/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8273 2023-06-13 15:39:52.000000 btclib-2023.5.30/tests/psbt/_generated_files/psbt.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2943 2023-06-13 15:39:52.000000 btclib-2023.5.30/tests/psbt/_generated_files/psbt_in.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      294 2023-06-13 15:39:52.000000 btclib-2023.5.30/tests/psbt/_generated_files/psbt_out.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    70300 2023-06-13 15:39:52.000000 btclib-2023.5.30/tests/psbt/test_psbt.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3597 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/psbt/test_psbt_in.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4404 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/psbt/test_psbt_out.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      736 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/psbt/test_psbt_utils.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       27 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/py.typed
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.965772 btclib-2023.5.30/tests/script/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      412 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.969772 btclib-2023.5.30/tests/script/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1648 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/_data/bip67_test_vectors.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)   210483 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/script/_data/sig_hash_legacy_test_vectors.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    29296 2022-07-04 10:37:33.000000 btclib-2023.5.30/tests/script/_data/taproot_test_vector.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)  9242563 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/_data/tapscript_test_vector.json
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.993772 btclib-2023.5.30/tests/script/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1100 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/script/_generated_files/witness.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8330 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_script.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    23491 2023-06-13 15:39:58.000000 btclib-2023.5.30/tests/script/test_script_pub_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8217 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_sig_hash_legacy.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6958 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_sig_hash_segwitv0.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     8476 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_sig_hash_taproot.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4287 2023-06-13 15:39:58.000000 btclib-2023.5.30/tests/script/test_taproot.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4368 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/script/test_witness.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3719 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_amount.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    12411 2023-06-13 15:39:58.000000 btclib-2023.5.30/tests/test_b32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    10234 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_b58.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3725 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_base58.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     6531 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_bech32.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      847 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_hashes.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2761 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_network.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3615 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_number_theory.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    11489 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_to_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     5844 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_to_prv_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     9749 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_to_pub_key.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3073 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_utils.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     2060 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/test_var_int.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.997772 btclib-2023.5.30/tests/tx/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      408 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/__init__.py
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.997772 btclib-2023.5.30/tests/tx/_data/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4740 2022-07-04 10:37:34.000000 btclib-2023.5.30/tests/tx/_data/d4f3c2c3c218be868c77ae31bedb497e2f908d6ee5bbbe91e4933e6da680c970.bin
+drwxrwxr-x   0 kappa     (1000) kappa     (1000)        0 2023-06-13 15:49:24.997772 btclib-2023.5.30/tests/tx/_generated_files/
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)       98 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/tx/_generated_files/out_point.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    12973 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/tx/_generated_files/tx.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     1392 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/tx/_generated_files/tx_in.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      289 2023-05-11 14:09:54.000000 btclib-2023.5.30/tests/tx/_generated_files/tx_out.json
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3440 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/test_out_point.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)    20879 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/test_tx.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     4547 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/test_tx_in.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)     3558 2023-02-07 11:12:07.000000 btclib-2023.5.30/tests/tx/test_tx_out.py
+-rw-rw-r--   0 kappa     (1000) kappa     (1000)      409 2023-06-13 15:39:52.000000 btclib-2023.5.30/tox.ini
```

### Comparing `btclib-2023.2.3/.flake8` & `btclib-2023.5.30/.flake8`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/.pre-commit-config.yaml` & `btclib-2023.5.30/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -25,40 +25,40 @@
       - id: detect-private-key
       - id: debug-statements
       - id: requirements-txt-fixer
       - id: check-docstring-first
       # - id: name-tests-test
       - id: check-toml
   - repo: https://github.com/DavidAnson/markdownlint-cli2
-    rev: v0.6.0
+    rev: v0.8.1
     hooks:
       - id: markdownlint-cli2-fix
         name: markdownlint-cli2-fix (in place fixes)
   - repo: https://github.com/leoll2/copyright_notice_precommit
     rev: 0.1.1
     hooks:
       - id: copyright-notice
         args: [--notice=COPYRIGHT]
         files: python
   - repo: https://github.com/PyCQA/autoflake
-    rev: v2.0.1
+    rev: v2.1.1
     hooks:
       - id: autoflake
         args:
           - --in-place
           - --expand-star-imports
           - --remove-all-unused-imports
           - --ignore-init-module-imports
           - --remove-duplicate-keys
           - --remove-unused-variables
           - --remove-rhs-for-unused-variables
         language: python
         types: [python]
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.6.0
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
         # exclude: *fixtures
         language: python
         types: [python]
   - repo: https://github.com/pycqa/isort
@@ -66,15 +66,15 @@
     hooks:
       - id: isort
         name: isort (black profile, in place fixes)
         args: ["--profile", "black", "--filter-files"]
         language: python
         types: [python]
   - repo: https://github.com/PyCQA/docformatter
-    rev: v1.5.1
+    rev: v1.7.2
     hooks:
       - id: docformatter
         description: "Formats docstrings to follow PEP 257."
         language: python
         types: [python]
         args: ["--in-place"]
   - repo: https://github.com/DanielNoord/pydocstringformatter
@@ -87,80 +87,80 @@
     rev: 6.3.0
     hooks:
       - id: pydocstyle
         additional_dependencies: [tomli]
         language: python
         types: [python]
   - repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
+    rev: v1.5.0
     hooks:
       - id: yesqa
         language: python
         types: [python]
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         language: python
         types: [python]
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black (in place fixes)
         # args: [--diff, --check]
         # It is recommended to specify the latest version of Python
         # supported by your project here, or alternatively use
         # pre-commit's default_language_version, see
         # https://pre-commit.com/#top_level-default_language_version
         # language_version: python3.11
         language: python
         types: [python]
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         name: bandit (btclib)
         args: []
         exclude: test_*
         language: python
         types: [python]
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         name: bandit (tests)
         # for the test folder disable
         # B101, Test for use of assert
         # B311, Standard pseudo-random generators are not suitable
         #       for security/cryptographic purposes
         args: ["--skip", "B101,B311"]
         exclude: btclib
         language: python
         types: [python]
   - repo: https://github.com/pycqa/pylint
-    rev: v2.16.0b1
+    rev: v3.0.0a6
     hooks:
       - id: pylint
         args: [
             "--disable=E0401", # import-error
           ]
         language: python
         types: [python]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.3.0
     hooks:
       - id: mypy
         language: python
         types: [python]
   - repo: https://github.com/mgedmin/check-manifest
     rev: "0.49"
     hooks:
       - id: check-manifest
         description: Check the completeness of MANIFEST.in for Python packages.
         language: python
         pass_filenames: false
         always_run: true
   - repo: https://github.com/regebro/pyroma
-    rev: "4.1"
+    rev: "4.2"
     hooks:
       - id: pyroma
```

### Comparing `btclib-2023.2.3/.sourcery.yaml` & `btclib-2023.5.30/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/CONTRIBUTING.md` & `btclib-2023.5.30/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/HISTORY.md` & `btclib-2023.5.30/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Release notes
 
 Notable changes to the codebase are documented here.
 
 Release names follow *[calendar versioning](https://calver.org/)*:
 full year, short month, short day (YYYY-M-D)
 
+## v2023.6 (work in progress, not released yet)
+
+Major changes include:
+
+- TBD
+
+## v2023.5.30
+
+Major changes include:
+
+- Fix circular import between ``script`` and ``b32``
+
 ## v2023.2.3
 
 Major changes include:
 
 - enabled libsecp256k1 by default
 - improved documentation
 - used generic containers (Sequence instead of list, Mapping instead of dict)
```

### Comparing `btclib-2023.2.3/LICENSE` & `btclib-2023.5.30/LICENSE`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/MANIFEST.in` & `btclib-2023.5.30/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/PKG-INFO` & `btclib-2023.5.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btclib
-Version: 2023.2.3
+Version: 2023.5.30
 Summary: A library for 'bitcoin cryptography'
 Home-page: https://btclib.org
 Author: The btclib developers
 Author-email: devs@btclib.org
 License: MIT License
 Project-URL: Download, https://github.com/btclib-org/btclib/releases
 Project-URL: Documentation, https://btclib.readthedocs.io/
```

### Comparing `btclib-2023.2.3/README.md` & `btclib-2023.5.30/README.md`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/RELEASE.md` & `btclib-2023.5.30/RELEASE.md`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/TODO.md` & `btclib-2023.5.30/TODO.md`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/__init__.py` & `btclib-2023.5.30/btclib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 #
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
 
 """__init__ module for the btclib package."""
 
 name = "btclib"
-__version__ = "2023.2.3"
+__version__ = "2023.5.30"
 __author__ = "The btclib developers"
 __author_email__ = "devs@btclib.org"
 __copyright__ = "Copyright (C) 2017-2023 The btclib developers"
 __license__ = "MIT License"
```

### Comparing `btclib-2023.2.3/btclib/_data/mainnet.json` & `btclib-2023.5.30/btclib/_data/mainnet.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/_data/regtest.json` & `btclib-2023.5.30/btclib/_data/regtest.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/_data/testnet.json` & `btclib-2023.5.30/btclib/_data/testnet.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/alias.py` & `btclib-2023.5.30/btclib/alias.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 # hex-string or bytes representation of an int
 # Integer = Union[Octets, int]
 Integer = Union[bytes, str, int]
 
 # Hash digest constructor: it may be any name suitable to hashlib.new()
 HashF = Callable[[], Any]
 # HashF = Callable[[Any], Any]
+H160_Net = Tuple[bytes, str]
 
 # Elliptic curve point in affine coordinates.
 # Warning: to make Point a NamedTuple would slow down the code
 Point = Tuple[int, int]
 
 # Note that the infinity point in affine coordinates is INF = (int, 0)
 # (no affine point has y=0 coordinate in a group of prime order).
@@ -93,7 +94,14 @@
 # It can be checked with 'INF[2] == 0'
 # The default x and y coordinates are arbitrary:
 # 7, 0 are used because those are what one would obtain
 # from the generic affine to Jacobian transformation
 # of the INF Point
 # QJ = Q[0], Q[1], 1 if Q[1] else 0
 INFJ = 7, 0, 0
+
+# TODO add type hinting to script_tree
+# unfortunately recursive type hinting is not supported
+# https://github.com/python/mypy/issues/731
+# TaprootLeaf = Tuple[int, Script]
+# TaprootScriptTree = List[Union[Any, TaprootLeaf]]
+TaprootScriptTree = Any
```

### Comparing `btclib-2023.2.3/btclib/amount.py` & `btclib-2023.5.30/btclib/amount.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/b32.py` & `btclib-2023.5.30/btclib/b32.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 from typing import Iterable
 
 from btclib.alias import Octets, String
 from btclib.bech32 import decode, encode
 from btclib.exceptions import BTClibValueError
 from btclib.hashes import hash160, sha256
 from btclib.network import NETWORKS, network_from_key_value
-from btclib.script import TaprootScriptTree, output_pubkey
 from btclib.to_pub_key import Key, pub_keyinfo_from_key
 from btclib.utils import bytes_from_octets
 
 # 0. bech32 facilities
 
 
 def has_segwit_prefix(addr: String) -> bool:
@@ -166,15 +165,10 @@
 
 def p2wsh(script_pub_key: Octets, network: str = "mainnet") -> str:
     """Return the p2wsh bech32 address corresponding to a script_pub_key."""
     h256 = sha256(script_pub_key)
     return address_from_witness(0, h256, network)
 
 
-def p2tr(
-    internal_key: Key | None = None,
-    script_path: TaprootScriptTree | None = None,
-    network: str = "mainnet",
-) -> str:
+def p2tr(output_key: Octets, network: str = "mainnet") -> str:
     """Return the p2tr bech32 address corresponding to a taproot output key."""
-    pub_key = output_pubkey(internal_key, script_path)[0]
-    return address_from_witness(1, pub_key, network)
+    return address_from_witness(1, output_key, network)
```

### Comparing `btclib-2023.2.3/btclib/b58.py` & `btclib-2023.5.30/btclib/b58.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/base58.py` & `btclib-2023.5.30/btclib/base58.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/bech32.py` & `btclib-2023.5.30/btclib/bech32.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/bip32/__init__.py` & `btclib-2023.5.30/btclib/bip32/__init__.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/bip32/bip32.py` & `btclib-2023.5.30/btclib/bip32/bip32.py`

 * *Files 9% similar despite different names*

```diff
@@ -273,15 +273,15 @@
     transactions).
     """
     xkey = _xpub_from_xprv(xprv)
     return xkey.b58encode()
 
 
 @dataclass
-class _ExtendedBIP32KeyData(BIP32KeyData):
+class _BIP32KeyData(BIP32KeyData):
     # extensions used to cache intermediate results
     # in multi-level derivation: do not rely on them elsewhere
 
     prv_key_int: int  # non-zero for private key only
     pub_key_point: Point  # non-Infinity for public key only
 
     def __init__(
@@ -305,24 +305,16 @@
             self.prv_key_int = 0
             self.pub_key_point = point_from_octets(self.key, ec)
 
         if check_validity:
             self.assert_valid()
 
 
-def __child_key_derivation(xkey: _ExtendedBIP32KeyData, index: int) -> None:
-    xkey.depth += 1
+def __prv_key_derivation(xkey: _BIP32KeyData, index: int) -> None:
     xkey.index = index
-    if xkey.is_private:
-        __private_key_derivation(xkey, index)
-    else:
-        __public_key_derivation(xkey, index)
-
-
-def __private_key_derivation(xkey: _ExtendedBIP32KeyData, index: int) -> None:
     Q_bytes = bytes_from_point(mult(xkey.prv_key_int))
     xkey.parent_fingerprint = hash160(Q_bytes)[:4]
     hmac_ = (
         hmac.new(
             xkey.chain_code,
             xkey.key + index.to_bytes(4, byteorder="big", signed=False),
             "sha512",
@@ -337,18 +329,17 @@
     xkey.chain_code = hmac_[32:]
     offset = int.from_bytes(hmac_[:32], byteorder="big", signed=False)
     xkey.prv_key_int = (xkey.prv_key_int + offset) % ec.n
     xkey.key = b"\x00" + xkey.prv_key_int.to_bytes(32, byteorder="big", signed=False)
     xkey.pub_key_point = INF
 
 
-def __public_key_derivation(xkey: _ExtendedBIP32KeyData, index: int) -> None:
+def __pub_key_derivation(xkey: _BIP32KeyData, index: int) -> None:
+    xkey.index = index
     xkey.parent_fingerprint = hash160(xkey.key)[:4]
-    if xkey.is_hardened:
-        raise BTClibValueError("invalid hardened derivation from public key")
     hmac_ = hmac.new(
         xkey.chain_code,
         xkey.key + index.to_bytes(4, byteorder="big", signed=False),
         "sha512",
     ).digest()
     xkey.chain_code = hmac_[32:]
     offset = int.from_bytes(hmac_[:32], byteorder="big", signed=False)
@@ -366,37 +357,44 @@
     indexes = indexes_from_bip32_path(der_path)
 
     final_depth = xkey.depth + len(indexes)
     if final_depth > 255:
         err_msg = f"final depth greater than 255: {final_depth}"
         raise BTClibValueError(err_msg)
 
-    xkey = _ExtendedBIP32KeyData(
+    xkey = _BIP32KeyData(
         version=xkey.version,
-        depth=xkey.depth,
+        depth=final_depth,
         parent_fingerprint=xkey.parent_fingerprint,
         index=xkey.index,
         chain_code=xkey.chain_code,
         key=xkey.key,
     )
-    for index in indexes:
-        __child_key_derivation(xkey, index)
 
     if forced_version:
         if xkey.version in XPRV_VERSIONS_ALL:
             allowed_versions = XPRV_VERSIONS_ALL
         else:
             allowed_versions = XPUB_VERSIONS_ALL
         fversion = bytes_from_octets(forced_version, 4)
         if fversion not in allowed_versions:
             err_msg = "invalid version forced on the extended key"
             err_msg += f"{hex_string(fversion)}"
             raise BTClibValueError(err_msg)
         xkey.version = fversion
 
+    if xkey.is_private:
+        for index in indexes:
+            __prv_key_derivation(xkey, index)
+    else:
+        if any(index >= 0x80000000 for index in indexes):
+            raise BTClibValueError("invalid hardened derivation from public key")
+        for index in indexes:
+            __pub_key_derivation(xkey, index)
+
     return xkey
 
 
 def derive(
     xkey: BIP32Key, der_path: BIP32DerPath, forced_version: Octets | None = None
 ) -> str:
     """Derive a BIP32 key across a path spanning multiple depth levels.
@@ -427,22 +425,24 @@
 
     if not mxkey.is_hardened:
         raise BTClibValueError("unhardened account/master key")
 
     if branch >= 0x80000000:
         raise BTClibValueError("invalid private derivation at branch level")
     if branch > max_index:
-        raise BTClibValueError(f"too high branch: {branch}")
+        err_msg = f"invalid branch number: {branch} is higher than {max_index}."
+        raise BTClibValueError(err_msg)
     if branches_0_1_only and branch not in (0, 1):
-        raise BTClibValueError(f"invalid branch: {branch} not in (0, 1)")
+        raise BTClibValueError(f"invalid branch number: {branch} not in (0, 1)")
 
     if address_index >= 0x80000000:
         raise BTClibValueError("invalid private derivation at address index level")
     if address_index > max_index:
-        raise BTClibValueError(f"too high address index: {branch}")
+        err_msg = f"invalid address index: {address_index} is higher than {max_index}."
+        raise BTClibValueError(err_msg)
 
     return _derive(mxkey, f"m/{branch}/{address_index}")
 
 
 def derive_from_account(
     mxkey: BIP32Key,
     branch: int,
```

### Comparing `btclib-2023.2.3/btclib/bip32/der_path.py` & `btclib-2023.5.30/btclib/bip32/der_path.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/bip32/key_origin.py` & `btclib-2023.5.30/btclib/bip32/key_origin.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/bip32/slip132.py` & `btclib-2023.5.30/btclib/bip32/slip132.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/block/__init__.py` & `btclib-2023.5.30/btclib/block/__init__.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/block/block.py` & `btclib-2023.5.30/btclib/block/block.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/block/block_header.py` & `btclib-2023.5.30/btclib/block/block_header.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/__init__.py` & `btclib-2023.5.30/btclib/ec/__init__.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/_data/ec_Brainpool.json` & `btclib-2023.5.30/btclib/ec/_data/ec_Brainpool.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/_data/ec_NIST.json` & `btclib-2023.5.30/btclib/ec/_data/ec_NIST.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/_data/ec_SEC2v1_insecure.json` & `btclib-2023.5.30/btclib/ec/_data/ec_SEC2v1_insecure.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/_data/ec_SEC2v2.json` & `btclib-2023.5.30/btclib/ec/_data/ec_SEC2v2.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/curve.py` & `btclib-2023.5.30/btclib/ec/curve.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/curve_group.py` & `btclib-2023.5.30/btclib/ec/curve_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,24 +477,24 @@
 
     return T
 
 
 MAX_W = 5
 
 
-@functools.lru_cache()  # least recently used cache
+@functools.lru_cache()  # results are cached to increase efficiency
 def cached_multiples(Q: JacPoint, ec: CurveGroup) -> list[JacPoint]:
     T = [INFJ, Q]
     for i in range(3, 2**MAX_W, 2):
         T.append(ec.double_jac(T[(i - 1) // 2]))
         T.append(ec.add_jac(T[-1], Q))
     return T
 
 
-@functools.lru_cache()
+@functools.lru_cache()  # results are cached to increase efficiency
 def cached_multiples_fixwind(
     Q: JacPoint, ec: CurveGroup, w: int = 4
 ) -> list[list[JacPoint]]:
     """Made to precompute values for mult_fixed_window_cached.
 
     Do not use it for other functions. Made to be used for w=4, do not
     use w.
```

### Comparing `btclib-2023.2.3/btclib/ec/curve_group_2.py` & `btclib-2023.5.30/btclib/ec/curve_group_2.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/curve_group_f.py` & `btclib-2023.5.30/btclib/ec/curve_group_f.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/libsecp256k1.py` & `btclib-2023.5.30/btclib/ec/libsecp256k1.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ec/sec_point.py` & `btclib-2023.5.30/btclib/ec/sec_point.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/__init__.py` & `btclib-2023.5.30/btclib/ecc/__init__.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/bip340_nonce.py` & `btclib-2023.5.30/btclib/ecc/bip340_nonce.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/bms.py` & `btclib-2023.5.30/btclib/ecc/bms.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/borromean.py` & `btclib-2023.5.30/btclib/ecc/borromean.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/dh.py` & `btclib-2023.5.30/btclib/ecc/dh.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/dsa.py` & `btclib-2023.5.30/btclib/ecc/dsa.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/libsecp256k1.py` & `btclib-2023.5.30/btclib/ecc/libsecp256k1.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/pedersen.py` & `btclib-2023.5.30/btclib/ecc/pedersen.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/rfc6979_nonce.py` & `btclib-2023.5.30/btclib/ecc/rfc6979_nonce.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/sign_to_contract.py` & `btclib-2023.5.30/btclib/ecc/sign_to_contract.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/ecc/ssa.py` & `btclib-2023.5.30/btclib/ecc/ssa.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/exceptions.py` & `btclib-2023.5.30/btclib/exceptions.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/hashes.py` & `btclib-2023.5.30/btclib/hashes.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 # No part of btclib including this file, may be copied, modified, propagated,
 # or distributed except according to the terms contained in the LICENSE file.
 
 """Hash based helper functions."""
 from __future__ import annotations
 
 import hashlib
-from typing import Callable, Sequence, Tuple
+from typing import Callable, Sequence
 
 from btclib.alias import HashF, Octets
 from btclib.utils import bytes_from_octets
 
-H160_Net = Tuple[bytes, str]
-
 # see https://bugs.python.org/issue47101
 # With OpenSSL 3.x, hashlib still includes ripemd160
 # but it is not usable unless the legacy provider is loaded.
 try:
     hashlib.new("ripemd160")
 except ValueError:  # pragma: no cover
     import ctypes
```

### Comparing `btclib-2023.2.3/btclib/mnemonic/__init__.py` & `btclib-2023.5.30/btclib/mnemonic/__init__.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/mnemonic/_data/english.txt` & `btclib-2023.5.30/btclib/mnemonic/_data/english.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/mnemonic/_data/italian.txt` & `btclib-2023.5.30/btclib/mnemonic/_data/italian.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/mnemonic/bip39.py` & `btclib-2023.5.30/btclib/mnemonic/bip39.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/mnemonic/electrum.py` & `btclib-2023.5.30/btclib/mnemonic/electrum.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/mnemonic/entropy.py` & `btclib-2023.5.30/btclib/mnemonic/entropy.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/mnemonic/mnemonic.py` & `btclib-2023.5.30/btclib/mnemonic/mnemonic.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/network.py` & `btclib-2023.5.30/btclib/network.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/number_theory.py` & `btclib-2023.5.30/btclib/number_theory.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/psbt/__init__.py` & `btclib-2023.5.30/btclib/psbt/__init__.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/psbt/psbt.py` & `btclib-2023.5.30/btclib/psbt/psbt.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -97,20 +97,20 @@
         self.unknown = dict(sorted(decode_dict_bytes_bytes(unknown).items()))
 
         if check_validity:
             self.assert_valid()
 
     def assert_valid(self) -> None:
         """Assert logical self-consistency."""
-        self.tx.assert_valid()
-
         # ensure a non-null tx has been included
         if not (self.tx.vin and self.tx.vout):
             raise BTClibValueError("null transaction")
 
+        self.tx.assert_valid()
+
         # ensure the tx is unsigned
         if any(tx_in.script_sig or tx_in.script_witness for tx_in in self.tx.vin):
             raise BTClibValueError("non empty script_sig or witness")
 
         if len(self.tx.vin) != len(self.inputs):
             err_msg = "mismatched number of psb.tx.vin and psb.inputs: "
             err_msg += f"{len(self.tx.vin)} vs {len(self.inputs)}"
```

### Comparing `btclib-2023.2.3/btclib/psbt/psbt_in.py` & `btclib-2023.5.30/btclib/psbt/psbt_in.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/psbt/psbt_out.py` & `btclib-2023.5.30/btclib/psbt/psbt_out.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/psbt/psbt_utils.py` & `btclib-2023.5.30/btclib/psbt/psbt_utils.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/script/__init__.py` & `btclib-2023.5.30/btclib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/script/script.py` & `btclib-2023.5.30/btclib/script/script.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/script/script_pub_key.py` & `btclib-2023.5.30/btclib/script/script_pub_key.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/script/sig_hash.py` & `btclib-2023.5.30/btclib/script/sig_hash.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/script/taproot.py` & `btclib-2023.5.30/btclib/script/taproot.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,23 @@
 """Taproot related functions."""
 
 from __future__ import annotations
 
 from typing import Any
 
 from btclib import var_bytes
-from btclib.alias import Octets
+from btclib.alias import Octets, TaprootScriptTree
 from btclib.ec import Curve, mult, secp256k1
 from btclib.exceptions import BTClibValueError
 from btclib.hashes import tagged_hash
 from btclib.script.script import serialize
 from btclib.to_prv_key import PrvKey, int_from_prv_key
 from btclib.to_pub_key import Key, pub_keyinfo_from_key
 from btclib.utils import bytes_from_octets
 
-# TODO add type hinting to script_tree
-# unfortunately recursive type hinting is not supported
-# https://github.com/python/mypy/issues/731
-# TaprootLeaf = Tuple[int, Script]
-# TaprootScriptTree = List[Union[Any, TaprootLeaf]]
-TaprootScriptTree = Any
-
 
 def tree_helper(script_tree: TaprootScriptTree) -> tuple[Any, bytes]:
     if len(script_tree) == 1:
         return _tree_helper(script_tree)
     left, left_h = tree_helper(script_tree[0])
     right, right_h = tree_helper(script_tree[1])
     info = [(leaf, c + right_h) for leaf, c in left]
```

### Comparing `btclib-2023.2.3/btclib/script/witness.py` & `btclib-2023.5.30/btclib/script/witness.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/to_prv_key.py` & `btclib-2023.5.30/btclib/to_prv_key.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/to_pub_key.py` & `btclib-2023.5.30/btclib/to_pub_key.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/tx/__init__.py` & `btclib-2023.5.30/btclib/tx/__init__.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/tx/out_point.py` & `btclib-2023.5.30/btclib/tx/out_point.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/tx/tx.py` & `btclib-2023.5.30/btclib/tx/tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from math import ceil
 from typing import Any, Mapping, Sequence
 
 from btclib import var_int
 from btclib.alias import BinaryData
 from btclib.exceptions import BTClibValueError
 from btclib.hashes import hash256
-from btclib.script import Witness
+from btclib.script.witness import Witness
 from btclib.tx.tx_in import TX_IN_COMPARES_WITNESS, TxIn
 from btclib.tx.tx_out import TxOut
 from btclib.utils import bytesio_from_binarydata
 
 _SEGWIT_MARKER = b"\x00\x01"
 
 
@@ -189,17 +189,21 @@
         if not 0 <= self.version <= 0xFFFFFFFF:
             raise BTClibValueError(f"invalid version: {self.version}")
 
         # must be a 4-bytes int
         if not 0 <= self.lock_time <= 0xFFFFFFFF:
             raise BTClibValueError(f"invalid lock time: {self.lock_time}")
 
+        if not self.vin:
+            raise BTClibValueError("Missing inputs")
         for tx_in in self.vin:
             tx_in.assert_valid()
 
+        if not self.vout:
+            raise BTClibValueError("Missing outputs")
         for tx_out in self.vout:
             tx_out.assert_valid()
 
     def serialize(self, include_witness: bool, check_validity: bool = True) -> bytes:
         if check_validity:
             self.assert_valid()
```

### Comparing `btclib-2023.2.3/btclib/tx/tx_in.py` & `btclib-2023.5.30/btclib/tx/tx_in.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/tx/tx_out.py` & `btclib-2023.5.30/btclib/tx/tx_out.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/utils.py` & `btclib-2023.5.30/btclib/utils.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/var_bytes.py` & `btclib-2023.5.30/btclib/var_bytes.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib/var_int.py` & `btclib-2023.5.30/btclib/var_int.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/btclib.egg-info/PKG-INFO` & `btclib-2023.5.30/btclib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btclib
-Version: 2023.2.3
+Version: 2023.5.30
 Summary: A library for 'bitcoin cryptography'
 Home-page: https://btclib.org
 Author: The btclib developers
 Author-email: devs@btclib.org
 License: MIT License
 Project-URL: Download, https://github.com/btclib-org/btclib/releases
 Project-URL: Documentation, https://btclib.readthedocs.io/
```

### Comparing `btclib-2023.2.3/btclib.egg-info/SOURCES.txt` & `btclib-2023.5.30/btclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/Makefile` & `btclib-2023.5.30/docs/Makefile`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/README.rst` & `btclib-2023.5.30/docs/README.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/make.bat` & `btclib-2023.5.30/docs/make.bat`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/source/btclib.bip32.rst` & `btclib-2023.5.30/docs/source/btclib.bip32.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/source/btclib.ec.rst` & `btclib-2023.5.30/docs/source/btclib.ec.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/source/btclib.ecc.rst` & `btclib-2023.5.30/docs/source/btclib.ecc.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/source/btclib.mnemonic.rst` & `btclib-2023.5.30/docs/source/btclib.mnemonic.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/source/btclib.psbt.rst` & `btclib-2023.5.30/docs/source/btclib.psbt.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/source/btclib.rst` & `btclib-2023.5.30/docs/source/btclib.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/source/btclib.script.rst` & `btclib-2023.5.30/docs/source/btclib.script.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/source/btclib.tx.rst` & `btclib-2023.5.30/docs/source/btclib.tx.rst`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/docs/source/conf.py` & `btclib-2023.5.30/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "btclib"
 project_copyright = "2017-2023 The btclib developers"
 author = "The btclib developers"
-release = "2023.2.3"
+release = "2023.5.30"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     # "m2r2",
     "myst_parser",
```

### Comparing `btclib-2023.2.3/pyproject.toml` & `btclib-2023.5.30/pyproject.toml`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/setup.py` & `btclib-2023.5.30/setup.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/README.md` & `btclib-2023.5.30/tests/README.md`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/_generated_files/mainnet.json` & `btclib-2023.5.30/tests/_generated_files/mainnet.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/_generated_files/regtest.json` & `btclib-2023.5.30/tests/_generated_files/regtest.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/_generated_files/testnet.json` & `btclib-2023.5.30/tests/_generated_files/testnet.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/bip32/_data/bip32_invalid_keys.json` & `btclib-2023.5.30/tests/bip32/_data/bip32_invalid_keys.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/bip32/_data/bip32_test_vectors.json` & `btclib-2023.5.30/tests/bip32/_data/bip32_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/bip32/_generated_files/key_paths.json` & `btclib-2023.5.30/tests/bip32/_generated_files/key_paths.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/bip32/test_bip32.py` & `btclib-2023.5.30/tests/bip32/test_bip32.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,27 +292,27 @@
         addr = p2pkh(derive(rmxprv, full_path))
         assert addr == p2pkh(derive_from_account(mxpub, branch, index))
 
     err_msg = "invalid private derivation at branch level"
     with pytest.raises(BTClibValueError, match=err_msg):
         derive_from_account(mxpub, 0x80000000, 0, True)
 
-    err_msg = "too high branch: "
+    err_msg = "invalid branch number: 65536"
     with pytest.raises(BTClibValueError, match=err_msg):
-        derive_from_account(mxpub, 0xFFFF + 1, 0)
+        derive_from_account(mxpub, 0xFFFF + 1, 0, branches_0_1_only=False)
 
-    err_msg = "invalid branch: "
+    err_msg = "invalid branch number: 2"
     with pytest.raises(BTClibValueError, match=err_msg):
         derive_from_account(mxpub, 2, 0)
 
     err_msg = "invalid private derivation at address index level"
     with pytest.raises(BTClibValueError, match=err_msg):
-        derive_from_account(mxpub, 0, 0x80000000)
+        derive_from_account(mxpub, 0, 0x80000000, max_index=0xFFFFFFFF)
 
-    err_msg = "too high address index: "
+    err_msg = "invalid address index: 65536"
     with pytest.raises(BTClibValueError, match=err_msg):
         derive_from_account(mxpub, 0, 0xFFFF + 1)
 
     der_path = "m / 44 h / 0"
     mxpub = xpub_from_xprv(derive(rmxprv, der_path))
     err_msg = "unhardened account/master key"
     with pytest.raises(BTClibValueError, match=err_msg):
```

### Comparing `btclib-2023.2.3/tests/bip32/test_der_path.py` & `btclib-2023.5.30/tests/bip32/test_der_path.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/bip32/test_key_origin.py` & `btclib-2023.5.30/tests/bip32/test_key_origin.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/bip32/test_slip132.py` & `btclib-2023.5.30/tests/bip32/test_slip132.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/block/_data/block_200000.bin` & `btclib-2023.5.30/tests/block/_data/block_200000.bin`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/block/_data/block_481824.bin` & `btclib-2023.5.30/tests/block/_data/block_481824.bin`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/block/_data/block_481824_complete.bin` & `btclib-2023.5.30/tests/block/_data/block_481824_complete.bin`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/block/_generated_files/block_481824.json` & `btclib-2023.5.30/tests/block/_generated_files/block_481824.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/block/test_block.py` & `btclib-2023.5.30/tests/block/test_block.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ec/_data/pubkey.json` & `btclib-2023.5.30/tests/ec/_data/pubkey.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ec/test_curve.py` & `btclib-2023.5.30/tests/ec/test_curve.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ec/test_curve_group.py` & `btclib-2023.5.30/tests/ec/test_curve_group.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ec/test_curve_group_2.py` & `btclib-2023.5.30/tests/ec/test_curve_group_2.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ec/test_curve_group_f.py` & `btclib-2023.5.30/tests/ec/test_curve_group_f.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ec/test_sec_point.py` & `btclib-2023.5.30/tests/ec/test_sec_point.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/_data/bip340_test_vectors.csv` & `btclib-2023.5.30/tests/ecc/_data/bip340_test_vectors.csv`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/_data/bms.json` & `btclib-2023.5.30/tests/ecc/_data/bms.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/_data/ecdsa_custom_nonce_sig.json` & `btclib-2023.5.30/tests/ecc/_data/ecdsa_custom_nonce_sig.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/_data/ecdsa_sig.json` & `btclib-2023.5.30/tests/ecc/_data/ecdsa_sig.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/_data/rfc6979.json` & `btclib-2023.5.30/tests/ecc/_data/rfc6979.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/test_bms.py` & `btclib-2023.5.30/tests/ecc/test_bms.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/test_borromean.py` & `btclib-2023.5.30/tests/ecc/test_borromean.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/test_der.py` & `btclib-2023.5.30/tests/ecc/test_der.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/test_dh.py` & `btclib-2023.5.30/tests/ecc/test_dh.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/test_dsa.py` & `btclib-2023.5.30/tests/ecc/test_dsa.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/test_pedersen.py` & `btclib-2023.5.30/tests/ecc/test_pedersen.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/test_rfc6979.py` & `btclib-2023.5.30/tests/ecc/test_rfc6979.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/test_sign_to_contract.py` & `btclib-2023.5.30/tests/ecc/test_sign_to_contract.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/ecc/test_ssa.py` & `btclib-2023.5.30/tests/ecc/test_ssa.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/mnemonic/_data/bip39_test_vectors.json` & `btclib-2023.5.30/tests/mnemonic/_data/bip39_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/mnemonic/_data/electrum_test_vectors.json` & `btclib-2023.5.30/tests/mnemonic/_data/electrum_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/mnemonic/_data/english.txt` & `btclib-2023.5.30/tests/mnemonic/_data/english.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/mnemonic/_data/fakeenglish.txt` & `btclib-2023.5.30/tests/mnemonic/_data/fakeenglish.txt`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/mnemonic/test_bip39.py` & `btclib-2023.5.30/tests/mnemonic/test_bip39.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/mnemonic/test_electrum.py` & `btclib-2023.5.30/tests/mnemonic/test_electrum.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/mnemonic/test_entropy.py` & `btclib-2023.5.30/tests/mnemonic/test_entropy.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/mnemonic/test_mnemonic.py` & `btclib-2023.5.30/tests/mnemonic/test_mnemonic.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/psbt/_data/bip174_test_vectors.json` & `btclib-2023.5.30/tests/psbt/_data/bip174_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/psbt/_generated_files/psbt.json` & `btclib-2023.5.30/tests/psbt/_generated_files/psbt.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/psbt/_generated_files/psbt_in.json` & `btclib-2023.5.30/tests/psbt/_generated_files/psbt_in.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/psbt/test_psbt.py` & `btclib-2023.5.30/tests/psbt/test_psbt.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/psbt/test_psbt_in.py` & `btclib-2023.5.30/tests/psbt/test_psbt_in.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/psbt/test_psbt_out.py` & `btclib-2023.5.30/tests/psbt/test_psbt_out.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/psbt/test_psbt_utils.py` & `btclib-2023.5.30/tests/psbt/test_psbt_utils.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/_data/bip67_test_vectors.json` & `btclib-2023.5.30/tests/script/_data/bip67_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/_data/sig_hash_legacy_test_vectors.json` & `btclib-2023.5.30/tests/script/_data/sig_hash_legacy_test_vectors.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/_data/taproot_test_vector.json` & `btclib-2023.5.30/tests/script/_data/taproot_test_vector.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/_data/tapscript_test_vector.json` & `btclib-2023.5.30/tests/script/_data/tapscript_test_vector.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/_generated_files/witness.json` & `btclib-2023.5.30/tests/script/_generated_files/witness.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/test_script.py` & `btclib-2023.5.30/tests/script/test_script.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/test_script_pub_key.py` & `btclib-2023.5.30/tests/script/test_script_pub_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,21 +576,21 @@
 
     assert addr == b32.address_from_witness(0, sha256(redeem_script), network)
     assert script_pub_key == ScriptPubKey.p2wsh(redeem_script)
 
 
 def test_p2tr() -> None:
     pub_key = "cc71eb30d653c0c3163990c47b976f3fb3f37cccdcbedb169a1dfef58bbfbfaf"
-    payload = output_pubkey(pub_key)[0]
-    script_pub_key = serialize(["OP_1", payload])
+    out_pubkey = output_pubkey(pub_key)[0]
+    script_pub_key = serialize(["OP_1", out_pubkey])
     assert_p2tr(script_pub_key)
-    assert ("p2tr", payload) == type_and_payload(script_pub_key)
+    assert ("p2tr", out_pubkey) == type_and_payload(script_pub_key)
 
     network = "mainnet"
-    addr = b32.p2tr(pub_key, network=network)
+    addr = b32.p2tr(out_pubkey, network=network)
     assert addr == address(script_pub_key, network)
 
     assert script_pub_key == ScriptPubKey.from_address(addr).script
     assert script_pub_key == ScriptPubKey.p2tr(pub_key).script
 
     err_msg = "invalid redeem script hash length marker: "
     with pytest.raises(BTClibValueError, match=err_msg):
```

### Comparing `btclib-2023.2.3/tests/script/test_sig_hash_legacy.py` & `btclib-2023.5.30/tests/script/test_sig_hash_legacy.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/test_sig_hash_segwitv0.py` & `btclib-2023.5.30/tests/script/test_sig_hash_segwitv0.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/test_sig_hash_taproot.py` & `btclib-2023.5.30/tests/script/test_sig_hash_taproot.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/script/test_taproot.py` & `btclib-2023.5.30/tests/script/test_taproot.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,11 +127,11 @@
         data = json.load(file_)["scriptPubKey"]
 
     for test in data:
         pub_key = test["given"]["internalPubkey"]
         script_tree = convert_script_tree(test["given"]["scriptTree"])
 
         tweaked_pubkey = output_pubkey(f"02{pub_key}", script_tree)[0]
-        address = b32.p2tr(f"02{pub_key}", script_tree)
+        address = b32.p2tr(tweaked_pubkey)
 
         assert tweaked_pubkey.hex() == test["intermediary"]["tweakedPubkey"]
         assert address == test["expected"]["bip350Address"]
```

### Comparing `btclib-2023.2.3/tests/script/test_witness.py` & `btclib-2023.5.30/tests/script/test_witness.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_amount.py` & `btclib-2023.5.30/tests/test_amount.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_b32.py` & `btclib-2023.5.30/tests/test_b32.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,11 +310,11 @@
     with pytest.raises(BTClibValueError, match=err_msg):
         b32.address_from_witness(0, witness_script_bytes)
 
 
 def test_p2tr() -> None:
     key = 1
     pub_key = output_pubkey(key)[0]
-    addr = b32.p2tr(key)
+    addr = b32.p2tr(pub_key)
     _, wit_prg, _ = b32.witness_from_address(addr)
 
     assert wit_prg == pub_key
```

### Comparing `btclib-2023.2.3/tests/test_b58.py` & `btclib-2023.5.30/tests/test_b58.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_base58.py` & `btclib-2023.5.30/tests/test_base58.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_bech32.py` & `btclib-2023.5.30/tests/test_bech32.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_hashes.py` & `btclib-2023.5.30/tests/test_hashes.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_network.py` & `btclib-2023.5.30/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_number_theory.py` & `btclib-2023.5.30/tests/test_number_theory.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_to_key.py` & `btclib-2023.5.30/tests/test_to_key.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_to_prv_key.py` & `btclib-2023.5.30/tests/test_to_prv_key.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_to_pub_key.py` & `btclib-2023.5.30/tests/test_to_pub_key.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_utils.py` & `btclib-2023.5.30/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/test_var_int.py` & `btclib-2023.5.30/tests/test_var_int.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/tx/_data/d4f3c2c3c218be868c77ae31bedb497e2f908d6ee5bbbe91e4933e6da680c970.bin` & `btclib-2023.5.30/tests/tx/_data/d4f3c2c3c218be868c77ae31bedb497e2f908d6ee5bbbe91e4933e6da680c970.bin`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/tx/_generated_files/tx.json` & `btclib-2023.5.30/tests/tx/_generated_files/tx.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/tx/_generated_files/tx_in.json` & `btclib-2023.5.30/tests/tx/_generated_files/tx_in.json`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/tx/test_out_point.py` & `btclib-2023.5.30/tests/tx/test_out_point.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/tx/test_tx.py` & `btclib-2023.5.30/tests/tx/test_tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from btclib.exceptions import BTClibValueError
 from btclib.script import Witness
 from btclib.tx import OutPoint, Tx, TxIn, TxOut, join_txs
 
 
 def test_tx() -> None:
     # default constructor
-    tx = Tx()
+    tx = Tx(check_validity=False)
     assert not tx.is_segwit()
     assert not any(bool(w) for w in tx.vwitness)
     assert not any(bool(tx_in.script_witness) for tx_in in tx.vin)
     assert not tx.is_coinbase()
     assert tx.version == 1
     assert tx.lock_time == 0
     assert not tx.vin
@@ -36,34 +36,45 @@
     tx_id = "d21633ba23f70118185227be58a63527675641ad37967e2aa461559f577aec43"
     assert tx.id.hex() == tx_id
     assert tx.hash == tx.id
     assert tx.size == 10
     assert tx.vsize == tx.size
     assert tx.weight == tx.size * 4
 
-    tx_2 = Tx.from_dict(tx.to_dict())
+    with pytest.raises(BTClibValueError, match="Missing inputs"):
+        tx.assert_valid()
+
+    tx_2 = Tx.from_dict(tx.to_dict(check_validity=False), check_validity=False)
     assert tx_2.is_segwit() == tx.is_segwit()
     assert tx_2 == tx
 
-    tx_2 = Tx.parse(tx.serialize(include_witness=True))
+    tx_2 = Tx.parse(
+        tx.serialize(include_witness=True, check_validity=False), check_validity=False
+    )
     assert tx_2.is_segwit() == tx.is_segwit()
     assert tx_2 == tx
 
-    tx_2 = Tx.parse(tx.serialize(include_witness=False))
+    tx_2 = Tx.parse(
+        tx.serialize(include_witness=False, check_validity=False), check_validity=False
+    )
     assert not tx_2.is_segwit()
     assert tx_2 == tx
 
     # non-default constructor, no segwit
     prev_out = OutPoint(
         "9dcfdb5836ecfe146bdaa896605ba21222f83cd014dd47adde14fab2aba7de9b", 1
     )
     script_sig = b""
     sequence = 0xFFFFFFFF
     tx_in = TxIn(prev_out, script_sig, sequence)
 
+    tx.vin = [tx_in]
+    with pytest.raises(BTClibValueError, match="Missing outputs"):
+        tx.assert_valid()
+
     tx_out1 = TxOut(2500000, "a914f987c321394968be164053d352fc49763b2be55c87")
     tx_out2 = TxOut(
         6381891, "0020701a8d401c84fb13e6baf169d59684e17abd9fa216c8cc5b9fc63d622ff8c58d"
     )
     version = 1
     lock_time = 0
     tx = Tx(version, lock_time, [tx_in], [tx_out1, tx_out2])
```

### Comparing `btclib-2023.2.3/tests/tx/test_tx_in.py` & `btclib-2023.5.30/tests/tx/test_tx_in.py`

 * *Files identical despite different names*

### Comparing `btclib-2023.2.3/tests/tx/test_tx_out.py` & `btclib-2023.5.30/tests/tx/test_tx_out.py`

 * *Files identical despite different names*

