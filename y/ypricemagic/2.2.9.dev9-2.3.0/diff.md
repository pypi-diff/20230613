# Comparing `tmp/ypricemagic-2.2.9.dev9.tar.gz` & `tmp/ypricemagic-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.2.9.dev9.tar", last modified: Sat May  6 19:20:36 2023, max compression
+gzip compressed data, was "ypricemagic-2.3.0.tar", last modified: Tue Jun 13 02:14:06 2023, max compression
```

## Comparing `ypricemagic-2.2.9.dev9.tar` & `ypricemagic-2.3.0.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.184718 ypricemagic-2.2.9.dev9/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.172718 ypricemagic-2.2.9.dev9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.176718 ypricemagic-2.2.9.dev9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-06 19:20:36.184718 ypricemagic-2.2.9.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-06 19:20:36.184718 ypricemagic-2.2.9.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.176718 ypricemagic-2.2.9.dev9/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.176718 ypricemagic-2.2.9.dev9/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.176718 ypricemagic-2.2.9.dev9/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.176718 ypricemagic-2.2.9.dev9/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.176718 ypricemagic-2.2.9.dev9/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.176718 ypricemagic-2.2.9.dev9/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.176718 ypricemagic-2.2.9.dev9/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.176718 ypricemagic-2.2.9.dev9/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     9930 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20058 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19844 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.180718 ypricemagic-2.2.9.dev9/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11223 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.184718 ypricemagic-2.2.9.dev9/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    21947 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.184718 ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.184718 ypricemagic-2.2.9.dev9/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     7901 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4332 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.184718 ypricemagic-2.2.9.dev9/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.184718 ypricemagic-2.2.9.dev9/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-06 19:20:25.000000 ypricemagic-2.2.9.dev9/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:20:36.184718 ypricemagic-2.2.9.dev9/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-06 19:20:36.000000 ypricemagic-2.2.9.dev9/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-05-06 19:20:36.000000 ypricemagic-2.2.9.dev9/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 19:20:36.000000 ypricemagic-2.2.9.dev9/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-06 19:20:36.000000 ypricemagic-2.2.9.dev9/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-06 19:20:36.000000 ypricemagic-2.2.9.dev9/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.353175 ypricemagic-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.333172 ypricemagic-2.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.333172 ypricemagic-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-13 02:14:06.353175 ypricemagic-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-13 02:14:06.353175 ypricemagic-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.333172 ypricemagic-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.333172 ypricemagic-2.3.0/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/y/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9930 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20162 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.337172 ypricemagic-2.3.0/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.345173 ypricemagic-2.3.0/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19844 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.345173 ypricemagic-2.3.0/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.345173 ypricemagic-2.3.0/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10744 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.349174 ypricemagic-2.3.0/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.349174 ypricemagic-2.3.0/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.349174 ypricemagic-2.3.0/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11225 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.349174 ypricemagic-2.3.0/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22171 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.349174 ypricemagic-2.3.0/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.349174 ypricemagic-2.3.0/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7924 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.353175 ypricemagic-2.3.0/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.353175 ypricemagic-2.3.0/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-13 02:13:45.000000 ypricemagic-2.3.0/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 02:14:06.353175 ypricemagic-2.3.0/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-13 02:14:06.000000 ypricemagic-2.3.0/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-06-13 02:14:06.000000 ypricemagic-2.3.0/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 02:14:06.000000 ypricemagic-2.3.0/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-13 02:14:06.000000 ypricemagic-2.3.0/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-13 02:14:06.000000 ypricemagic-2.3.0/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.2.9.dev9/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.3.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/.github/workflows/pytest.yaml` & `ypricemagic-2.3.0/.github/workflows/pytest.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -14,17 +14,19 @@
       - '**/pytest.yaml'
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     #timeout-minutes: 10
     strategy:
+      fail-fast: false
       matrix:
         os: [ ubuntu-latest, macos-latest, windows-latest ]
-        network: [ mainnet, bsc-main, polygon-main, ftm-main ]
+        pyversion: [ "3.8", "3.9", "3.10" ]
+        network: [ mainnet, bsc-main, polygon-main, ftm-main, arbitrum-main, optimism-main ]
         include:
         - os: ubuntu-latest
           path: ~/.cache/pip
         - os: macos-latest
           path: ~/Library/Caches/pip
         - os: windows-latest
           path: ~\AppData\Local\pip\Cache
@@ -32,24 +34,27 @@
           provider: WEB3_PROVIDER
         - network: bsc-main
           provider: BSC_WEB3_PROVIDER
         - network: polygon-main
           provider: POLY_WEB3_PROVIDER
         - network: ftm-main
           provider: FTM_WEB3_PROVIDER
-
+        - network: arbitrum-main
+          provider: ARBI_WEB3_PROVIDER
+        - network: optimism-main
+          provider: OPTI_WEB3_PROVIDER
 
     steps:
       - name: Check out repository code
         uses: actions/checkout@v2
 
       - name: Setup Python (faster than using Python container)
         uses: actions/setup-python@v2
         with:
-          python-version: "3.9"
+          python-version: ${{ matrix.pyversion }}
 
       - name: Cache dependencies
         uses: actions/cache@v3
         with:
           key: ${{ runner.os }}-pip-${{ hashFiles('**/requirements.txt') }}-${{ hashFiles('**/requirements-dev.txt') }}
           path: |
             ${{ matrix.path }}
@@ -85,10 +90,11 @@
         env:
           BROWNIE_NETWORK: ${{ matrix.network }}
           # Explorer tokens for all chains:
           ETHERSCAN_TOKEN: ${{ secrets.ETHERSCAN_TOKEN }}
           BSCSCAN_TOKEN: ${{ secrets.BSCSCAN_TOKEN }}
           POLYGONSCAN_TOKEN: ${{ secrets.POLYGONSCAN_TOKEN }}
           FTMSCAN_TOKEN: ${{ secrets.FTMSCAN_TOKEN }}
+          ARBISCAN_TOKEN: ${{ secrets.ARBISCAN_TOKEN }}
+          OPTISCAN_TOKEN: ${{ secrets.OPTISCAN_TOKEN }}
         run: make test
-        continue-on-error: true
```

### Comparing `ypricemagic-2.2.9.dev9/.github/workflows/release.yaml` & `ypricemagic-2.3.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/LICENSE.txt` & `ypricemagic-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/README.md` & `ypricemagic-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/setup.py` & `ypricemagic-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/classes/test_erc20.py` & `ypricemagic-2.3.0/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/classes/test_singleton.py` & `ypricemagic-2.3.0/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/fixtures.py` & `ypricemagic-2.3.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.3.0/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/prices/lending/test_aave.py` & `ypricemagic-2.3.0/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/prices/lending/test_compound.py` & `ypricemagic-2.3.0/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/prices/test_chainlink.py` & `ypricemagic-2.3.0/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/prices/test_magic.py` & `ypricemagic-2.3.0/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/prices/test_popsicle.py` & `ypricemagic-2.3.0/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/prices/test_synthetix.py` & `ypricemagic-2.3.0/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/prices/test_yearn.py` & `ypricemagic-2.3.0/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/tests/prices/utils/test_buckets.py` & `ypricemagic-2.3.0/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/__init__.py` & `ypricemagic-2.3.0/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/classes/common.py` & `ypricemagic-2.3.0/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/classes/singleton.py` & `ypricemagic-2.3.0/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/constants.py` & `ypricemagic-2.3.0/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/contracts.py` & `ypricemagic-2.3.0/y/contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from y import convert
 from y.datatypes import Address, AnyAddressType, Block
 from y.exceptions import (ContractNotVerified, NodeNotSynced, call_reverted,
                           contract_not_verified)
 from y.interfaces.ERC20 import ERC20ABI
 from y.networks import Network
+from y.time import check_node, check_node_async
 from y.utils.cache import memory
 from y.utils.dank_mids import dank_w3
 from y.utils.logging import yLazyLogger
 
 logger = logging.getLogger(__name__)
 
 contract_threads = PruningThreadPoolExecutor(16)
@@ -73,14 +74,16 @@
     logger.debug(f"contract creation block {address}")
     height = chain.height
 
     if height == 0:
         raise NodeNotSynced(f'''
             `chain.height` returns 0 on your node, which means it is not fully synced.
             You can only use this function on a fully synced node.''')
+    
+    check_node()
 
     lo, hi = 0, height
     barrier = 0
     warned = False
     while hi - lo > 1:
         mid = lo + (hi - lo) // 2
         # TODO rewrite this so we can get deploy blocks for some contracts deployed on correct side of barrier
@@ -124,14 +127,16 @@
     logger.debug(f"contract creation block {address}")
     height = await dank_w3.eth.block_number
 
     if height == 0:
         raise NodeNotSynced(f'''
             `chain.height` returns 0 on your node, which means it is not fully synced.
             You can only use this function on a fully synced node.''')
+    
+    await check_node_async()
 
     lo, hi = 0, height
     barrier = 0
     warned = False
     while hi - lo > 1:
         mid = lo + (hi - lo) // 2
         # TODO rewrite this so we can get deploy blocks for some contracts deployed on correct side of barrier
```

### Comparing `ypricemagic-2.2.9.dev9/y/datatypes.py` & `ypricemagic-2.3.0/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/decorators.py` & `ypricemagic-2.3.0/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/erc20.py` & `ypricemagic-2.3.0/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/exceptions.py` & `ypricemagic-2.3.0/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/interfaces/ERC20.py` & `ypricemagic-2.3.0/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.3.0/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/interfaces/compound/unitroller.py` & `ypricemagic-2.3.0/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.3.0/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/interfaces/multicall2.py` & `ypricemagic-2.3.0/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.3.0/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.3.0/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/networks.py` & `ypricemagic-2.3.0/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/band.py` & `ypricemagic-2.3.0/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/chainlink.py` & `ypricemagic-2.3.0/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/convex.py` & `ypricemagic-2.3.0/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.3.0/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/balancer/v1.py` & `ypricemagic-2.3.0/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/balancer/v2.py` & `ypricemagic-2.3.0/y/prices/dex/balancer/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 import a_sync
 from brownie import chain
 from brownie.convert.datatypes import EthAddress
 from hexbytes import HexBytes
 from multicall import Call
 
+from y import constants, contracts
 from y.classes.common import ERC20, ContractBase, WeiBalance
-from y.constants import STABLECOINS, WRAPPED_GAS_COIN
-from y.contracts import build_name, contract_creation_block_async, has_methods
 from y.datatypes import Address, AnyAddressType, Block, UsdPrice, UsdValue
 from y.networks import Network
 from y.utils.events import decode_logs, get_logs_asap
 from y.utils.raw_calls import raw_call
 
 logger = logging.getLogger(__name__)
 
@@ -58,32 +57,38 @@
         topics = ['0x3c13bc30b8e878c53fd2a36b679409c073afd75950be43d8858768e956fbc20e']
         #try:
         events = decode_logs(await get_logs_asap(self.address, topics, to_block=block, sync=False))
         #except TypeError as e:
         #    if "Start must be less than or equal to stop" in str(e):
         #        return {}
         #    raise
-        return {event['poolId'].hex():event['poolAddress'] for event in events}
+        return {
+            event['poolId'].hex(): event['poolAddress'] for event in events
+            # NOTE: For some reason the Balancer fork on Fantom lists "0x3e522051A9B1958Aa1e828AC24Afba4a551DF37d"
+            #       as a pool, but it is not a contract. This handler will prevent it and future cases from causing problems.
+            if contracts.is_contract(event['poolAddress'])
+        }
     
     @a_sync.a_sync(ram_cache_maxsize=10)
     async def get_pool_info(self, poolids: Tuple[HexBytes,...], block: Optional[Block] = None) -> List[Tuple]:
         return await asyncio.gather(*[
             self.contract.getPoolTokens.coroutine(poolId, block_identifier=block)
             for poolId in poolids
         ])
     
     #yLazyLogger(logger)
     async def deepest_pool_for(self, token_address: Address, block: Optional[Block] = None) -> Tuple[Optional[EthAddress],int]:
+        # sourcery skip: simplify-len-comparison
         pools = await self.list_pools(block=block, sync=False)
         is_standard_pool = await asyncio.gather(*[_is_standard_pool(pool) for pool in pools.values()])
         
         if block is None:
             poolids = (poolid for (poolid, pool), is_standard in zip(pools.items(), is_standard_pool) if is_standard)
         else:
-            deploy_blocks = await asyncio.gather(*[contract_creation_block_async(pool, True) for pool in pools.values()])
+            deploy_blocks = await asyncio.gather(*[contracts.contract_creation_block_async(pool, True) for pool in pools.values()])
             poolids = (poolid for (poolid, pool), is_standard, deploy_block in zip(pools.items(), is_standard_pool, deploy_blocks) if is_standard and deploy_block <= block)
 
         pools_info = await self.get_pool_info(poolids, block=block, sync=False)
         all_pools = await self.list_pools(block=block, sync=False)
         pools_info = {all_pools[poolid]: info for poolid, info in zip(poolids, pools_info) if str(info) != "((), (), 0)"}
         
         deepest_pool = {'pool': None, 'balance': 0}
@@ -127,31 +132,31 @@
         return UsdValue(sum(await asyncio.gather(*[
             balance.__value_usd__(sync=False) for balance in balances.values()
             if balance.token.address != self.address  # NOTE: to prevent an infinite loop for tokens that include themselves in the pool (e.g. bb-a-USDC)
         ])))
 
     async def get_balances(self, block: Optional[Block] = None) -> Dict[ERC20, WeiBalance]:
         tokens = await self.tokens(block=block, sync=False)
-        return {token: balance for token, balance in tokens.items()}
+        return dict(tokens.items())
 
     async def get_token_price(self, token_address: AnyAddressType, block: Optional[Block] = None) -> Optional[UsdPrice]:
         token_balances, weights = await asyncio.gather(
             self.get_balances(block=block, sync=False),
             self.weights(block=block, sync=False),
         )
         pool_token_info = list(zip(token_balances.keys(),token_balances.values(), weights))
         for pool_token, balance, weight in pool_token_info:
             if pool_token == token_address:
                 token_balance, token_weight = balance, weight
 
         for pool_token, balance, weight in pool_token_info:
-            if pool_token in STABLECOINS:
+            if pool_token in constants.STABLECOINS:
                 paired_token_balance, paired_token_weight = balance, weight
                 break
-            elif pool_token == WRAPPED_GAS_COIN:
+            elif pool_token == constants.WRAPPED_GAS_COIN:
                 paired_token_balance, paired_token_weight = balance, weight
                 break
             elif len(pool_token_info) == 2 and pool_token != token_address:
                 paired_token_balance, paired_token_weight = balance, weight
                 break
 
         try:
@@ -178,28 +183,28 @@
 async def _is_standard_pool(pool: EthAddress) -> bool:
     '''
     Returns `False` if `build_name(pool) in ['ConvergentCurvePool','MetaStablePool']`, else `True`
     '''
     
     # With `return_None_on_failure=True`, if `build_name(pool)` fails,
     # we can't know for sure that its a standard pool, but... it probably is.
-    return await build_name(pool, return_None_on_failure=True, sync=False) not in ['ConvergentCurvePool','MetaStablePool']
+    return await contracts.build_name(pool, return_None_on_failure=True, sync=False) not in ['ConvergentCurvePool','MetaStablePool']
 
 
 class BalancerV2(a_sync.ASyncGenericSingleton):
     def __init__(self, asynchronous: bool = False) -> None:
         self.asynchronous = asynchronous
         self.vaults = [BalancerV2Vault(vault, asynchronous=self.asynchronous) for vault in BALANCER_V2_VAULTS]
     
     def __str__(self) -> str:
         return "BalancerV2()"
 
     async def is_pool(self, token_address: AnyAddressType) -> bool:
         methods = ('getPoolId()(bytes32)','getPausedState()((bool,uint,uint))','getSwapFeePercentage()(uint)')
-        return await has_methods(token_address, methods, sync=False)
+        return await contracts.has_methods(token_address, methods, sync=False)
     
     async def get_pool_price(self, pool_address: AnyAddressType, block: Optional[Block] = None) -> UsdPrice:
         return await BalancerV2Pool(pool_address, asynchronous=True).get_pool_price(block=block)
 
     async def get_token_price(self, token_address: Address, block: Optional[Block] = None) -> UsdPrice:
         deepest_pool: Optional[BalancerV2Pool] = await self.deepest_pool_for(token_address, block=block, sync=False)
         if deepest_pool is None:
```

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/genericamm.py` & `ypricemagic-2.3.0/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/mooniswap.py` & `ypricemagic-2.3.0/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.3.0/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.3.0/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.3.0/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.3.0/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.3.0/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/eth_derivs/creth.py` & `ypricemagic-2.3.0/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.3.0/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/gearbox.py` & `ypricemagic-2.3.0/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/lending/aave.py` & `ypricemagic-2.3.0/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/lending/compound.py` & `ypricemagic-2.3.0/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/lending/ib.py` & `ypricemagic-2.3.0/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/magic.py` & `ypricemagic-2.3.0/y/prices/magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,11 +233,11 @@
         if `silent == True`, ypricemagic will print an error message using standard python logging
         if `silent == False`, ypricemagic will not log any error
         if `fail_to_None == True`, ypricemagic will return `None`
         if `fail_to_None == False`, ypricemagic will raise a PriceError
     '''
 
     if not silent:
-        logger.error(f"failed to get price for {token_string} on {Network.printable()}")
+        logger.warning(f"failed to get price for {token_string} on {Network.printable()}")
 
     if not fail_to_None:
         raise PriceError(f'could not fetch price for {token_string} on {Network.printable()}')
```

### Comparing `ypricemagic-2.2.9.dev9/y/prices/one_to_one.py` & `ypricemagic-2.3.0/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/popsicle.py` & `ypricemagic-2.3.0/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/stable_swap/belt.py` & `ypricemagic-2.3.0/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/stable_swap/curve.py` & `ypricemagic-2.3.0/y/prices/stable_swap/curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     # On other chains, "cryptopool factory" is id 6.
     # On Polygon, id 6 is "crypto factory".
     # I've only seen this on Mainnet and Polygon so far, for now will treat `7` == `6`.
     Cryptopool_Factory = 7
     crvUSD_Plain_Pools_deprecated_1 = 8
     crvUSD_Plain_Pools_deprecated_2 = 9
     crvUSD_Plain_Pools = 10
+    Curve_Tricrypto_Factory = 11
 
 
 class CurvePool(ERC20): # this shouldn't be ERC20 but works for inheritance for now
     @a_sync.aka.cached_property
     async def factory(self) -> Contract:
         return await curve.get_factory(self, sync=False)
 
@@ -178,17 +179,20 @@
                 return None
             raise
 
     async def get_tvl(self, block: Optional[Block] = None) -> Optional[UsdValue]:
         """
         Get total value in Curve pool.
         """
-        balances = await self.get_balances(block=block, sync=False)
-        if balances is None:
-            return None
+        try:
+            balances = await self.get_balances(block=block, sync=False)
+        except ValueError as e:
+            if str(e).startswith("could not fetch balances "):
+                return None
+            raise e
         
         prices = await asyncio.gather(*[coin.price(block=block, sync=False) for coin in balances])
 
         return UsdValue(
             sum(balance * price for balance, price in zip(balances.values(),prices))
         )
     
@@ -254,18 +258,19 @@
             await asyncio.sleep(15)
             
         async for logs in get_logs_asap_generator(str(self.address_provider), None, from_block=block+1, chronological=True, run_forever=True):
             for event in decode_logs(logs):
                 self._load_address_provider_event(event)
     
     async def _load_registry_event(self, registry: Contract, event) -> None:
-        if event.name == 'PoolAdded':
-            lp_token = await registry.get_lp_token.coroutine(event['pool'])
-            self.registries[event.address].add(event['pool'])
-            self.token_to_pool[lp_token] = event['pool']
+        if event.name in ['PoolAdded', 'TricryptoPoolDeployed']:
+            pool = event['pool']
+            lp_token = pool if event.name == 'TricryptoPoolDeployed' else await registry.get_lp_token.coroutine(pool)
+            self.registries[event.address].add(pool)
+            self.token_to_pool[lp_token] = pool
         elif event.name == 'PoolRemoved':
             self.registries[event.address].discard(event['pool'])
 
     async def _load_registry(self, registry: Address) -> NoReturn:
         """ Fetch all pools from a particular registry. """ 
         contract, block = await asyncio.gather(Contract.coroutine(registry), dank_w3.eth.block_number)
         async for logs in get_logs_asap_generator(registry, to_block=block, chronological=True):
```

### Comparing `ypricemagic-2.2.9.dev9/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.3.0/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/stable_swap/froyo.py` & `ypricemagic-2.3.0/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.3.0/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/stable_swap/saddle.py` & `ypricemagic-2.3.0/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/synthetix.py` & `ypricemagic-2.3.0/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.3.0/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.3.0/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.3.0/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.3.0/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/utils/buckets.py` & `ypricemagic-2.3.0/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/utils/sense_check.py` & `ypricemagic-2.3.0/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/prices/utils/ypriceapi.py` & `ypricemagic-2.3.0/y/prices/utils/ypriceapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import logging
 import os
 from collections import defaultdict
 from http import HTTPStatus
 from random import randint
 from time import time
-from typing import Any, Callable, List, Optional
+from typing import Any, Callable, Dict, List, Optional
 
 from aiohttp import BasicAuth, ClientResponse, ClientSession, TCPConnector
 from aiohttp.client_exceptions import ClientError, ContentTypeError
 from async_lru import alru_cache
 from brownie import chain
 
 from y import constants
@@ -29,14 +29,15 @@
 
 # old
 YPRICEAPI_USER = os.environ.get("YPRICEAPI_USER")
 YPRICEAPI_PASS = os.environ.get("YPRICEAPI_PASS")
 OLD_AUTH = BasicAuth(YPRICEAPI_USER, YPRICEAPI_PASS) if YPRICEAPI_USER and YPRICEAPI_PASS else None
 
 ONE_MINUTE = 60  # some arbitrary amount of time in case the header is missing on unexpected 5xx responses
+ONE_HOUR = ONE_MINUTE * 60
 FALLBACK_STR = "Falling back to your node for pricing."
 YPRICEAPI_SEMAPHORE = asyncio.Semaphore(int(os.environ.get("YPRICEAPI_SEMAPHORE", 100)))
 
 if any(AUTH_HEADERS.values()) and not AUTH_HEADERS_PRESENT:
     for header in AUTH_HEADERS:
         if not AUTH_HEADERS[header]:
             raise EnvironmentError(f'You must also pass in a value for {header_env_names[header]} in order to use ypriceAPI.')
@@ -54,26 +55,26 @@
 #########################
 # YPRICEAPI PUBLIC BETA #
 #########################
     
 _you_get = [
     "access to your desired price data more quickly...",
     "...from nodes run by yearn-affiliated big brains...",
-    "on all the networks "
+    "...on all the networks Yearn supports."
 ]
 _testimonials = [
-    "I can now get prices for all of my useless shitcoins without waiting all day for ypricemagic to load logs."
+    "I can now get prices for all of my useless shitcoins without waiting all day for ypricemagic to load logs.",
     "I don't need to maintain an archive node anymore and that's saving me money.", 
     "Wow, so fast!",
 ]
 beta_announcement = "ypriceAPI is now in beta!\n\n"
 beta_announcement += "Head to ypriceapi-beta.yearn.finance and sign up for access. You get:\n"
 for you_get in _you_get:
     beta_announcement += f" - {you_get}\n"
-beta_announcement += "\nCheck out some testimonials from our close frens:"
+beta_announcement += "\nCheck out some testimonials from our close frens:\n"
 for testimonial in _testimonials:
     beta_announcement += f' - from anon{randint(0, 9999)}, "{testimonial}"\n'
 
 def announce_beta() -> None:
     spam_your_logs_fn = logger.info if logger.isEnabledFor(logging.INFO) else print
     spam_your_logs_fn(beta_announcement)
     global should_use
@@ -101,22 +102,22 @@
 async def get_session() -> ClientSession:
     return ClientSession(
         "https://ypriceapi-beta.yearn.finance",
         connector=TCPConnector(verify_ssl=False),
         headers=AUTH_HEADERS,
     )
 
-@alru_cache(maxsize=1, ttl=ONE_MINUTE * 60)
-async def get_chains() -> List[int]:
+@alru_cache(ttl=ONE_HOUR)
+async def get_chains() -> Dict[int, str]:
     session = await get_session()
     async with session.get("/chains") as response:
-        chains = await read_response(response)
-    return [] if chains is None else list(chains.keys())
+        chains = await read_response(response) or {}
+    return {int(k): v for k, v in chains.items()}
 
-@alru_cache(maxsize=1, ttl=ONE_MINUTE * 60)
+@alru_cache(ttl=ONE_HOUR)
 async def chain_supported(chainid: int) -> bool:
     if chainid in await get_chains():
         return True
     logger.info(f'ypriceAPI does not support {Network.name()} at this time.')
     return False
 
 async def get_price(
@@ -201,8 +202,8 @@
     return f"[{response.status} {ascii_encodable_reason}]"
     
 def _set_resume_at(retry_after: float) -> None:
     global resume_at
     logger.info(f"Falling back to your node for {int(retry_after/60)} minutes.")
     resume_from_this_err_at = time() + retry_after
     if resume_from_this_err_at > resume_at:
-        resume_at = resume_from_this_err_at
+        resume_at = resume_from_this_err_at
```

### Comparing `ypricemagic-2.2.9.dev9/y/prices/yearn.py` & `ypricemagic-2.3.0/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/time.py` & `ypricemagic-2.3.0/y/time.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import asyncio
 import datetime
 import logging
 import time
 from typing import NewType, Union
 
-from brownie import chain, web3
 from a_sync import a_sync
-from y.exceptions import NoBlockFound
+from async_lru import alru_cache
+from brownie import chain, web3
+from cachetools.func import ttl_cache
+
+from y.exceptions import NoBlockFound, NodeNotSynced
 from y.networks import Network
 from y.utils.cache import memory
 from y.utils.client import get_ethereum_client, get_ethereum_client_async
 from y.utils.dank_mids import dank_w3
 from y.utils.logging import yLazyLogger
 
 logger = logging.getLogger(__name__)
@@ -67,39 +70,42 @@
 class UnixTimestamp(int):
     pass
 
 Timestamp = Union[UnixTimestamp, datetime.datetime]
 
 def _parse_timestamp(timestamp: Timestamp) -> UnixTimestamp:
     if isinstance(timestamp, datetime.datetime):
-        timestamp = timestamp.timestamp()
+        timestamp = int(timestamp.timestamp())
     elif not isinstance(timestamp, int):
         raise TypeError("You may only pass in a unix timestamp or a datetime object.")
     return UnixTimestamp(timestamp)
 
 #yLazyLogger(logger)
 def closest_block_after_timestamp(timestamp: Timestamp, wait_for_block_if_needed: bool = False) -> int:
     timestamp = _parse_timestamp(timestamp)
     while wait_for_block_if_needed:
         try:
             return closest_block_after_timestamp(timestamp)
         except NoBlockFound:
             time.sleep(.2)
+    check_node()
     block = _closest_block_after_timestamp_cached(timestamp)
     logger.debug(f'closest {Network.name()} block after timestamp {timestamp} -> {block}')
     return block
 
 @a_sync(cache_type='memory')
 async def closest_block_after_timestamp_async(timestamp: Timestamp, wait_for_block_if_needed: bool = False) -> int:
     timestamp = _parse_timestamp(timestamp)
     while wait_for_block_if_needed:
         try:
             return await closest_block_after_timestamp_async(timestamp)
         except NoBlockFound:
             await asyncio.sleep(0.2)
+    
+    await check_node_async()
 
     height = await dank_w3.eth.block_number
     lo, hi = 0, height
     while hi - lo > 1:
         mid = lo + (hi - lo) // 2
         if await get_block_timestamp_async(mid) > timestamp:
             hi = mid
@@ -119,7 +125,23 @@
         if get_block_timestamp(mid) > timestamp:
             hi = mid
         else:
             lo = mid
     if hi == height:
         raise NoBlockFound(f"No block found after timestamp {timestamp}")
     return hi
+
+
+@ttl_cache(ttl=60)
+def check_node() -> None:
+    node_timestamp = web3.eth.get_block('latest').timestamp
+    current_time = time.time()
+    if current_time - node_timestamp > 5 * 60:
+        raise NodeNotSynced(f"current time: {current_time}  latest block time: {node_timestamp}  discrepancy: {round((current_time - node_timestamp) / 60, 2)} minutes")
+
+@alru_cache(ttl=60)
+async def check_node_async() -> None:
+    latest = await dank_w3.eth.get_block('latest')
+    node_timestamp = latest.timestamp
+    current_time = time.time()
+    if current_time - node_timestamp > 5 * 60:
+        raise NodeNotSynced(f"current time: {current_time}  latest block time: {node_timestamp}  discrepancy: {round((current_time - node_timestamp) / 60, 2)} minutes")
```

### Comparing `ypricemagic-2.2.9.dev9/y/utils/client.py` & `ypricemagic-2.3.0/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/utils/events.py` & `ypricemagic-2.3.0/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/utils/fakes.py` & `ypricemagic-2.3.0/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/utils/logging.py` & `ypricemagic-2.3.0/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/utils/middleware.py` & `ypricemagic-2.3.0/y/utils/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import eth_retry
 from brownie import chain, web3
 from requests import Session
 from requests.adapters import HTTPAdapter
 from web3 import HTTPProvider, Web3
 from web3.middleware import filter
+from web3.middleware.geth_poa import geth_poa_middleware
 
 from y.networks import Network
 from y.utils.cache import memory
 
 logger = logging.getLogger(__name__)
 
 provider_specific_batch_sizes = {
@@ -71,11 +72,14 @@
             else:
                 raise
 
     # patch and inject local filter middleware
     filter.MAX_BLOCK_REQUEST = BATCH_SIZE
     web3.middleware_onion.add(filter.local_filter_middleware)
     web3.middleware_onion.add(cache_middleware)
+    
+    if chain.id == Network.Optimism:
+        web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
 def ensure_middleware() -> None:
     setup_middleware()
```

### Comparing `ypricemagic-2.2.9.dev9/y/utils/multicall.py` & `ypricemagic-2.3.0/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/y/utils/raw_calls.py` & `ypricemagic-2.3.0/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/ypricemagic/magic.py` & `ypricemagic-2.3.0/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.9.dev9/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.3.0/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

