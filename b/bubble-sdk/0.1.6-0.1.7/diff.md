# Comparing `tmp/bubble-sdk-0.1.6.tar.gz` & `tmp/bubble-sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bubble-sdk-0.1.6.tar", last modified: Wed May 31 10:59:11 2023, max compression
+gzip compressed data, was "bubble-sdk-0.1.7.tar", last modified: Tue Jun 13 03:21:00 2023, max compression
```

## Comparing `bubble-sdk-0.1.6.tar` & `bubble-sdk-0.1.7.tar`

### file list

```diff
@@ -1,249 +1,249 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/
--rw-rw-rw-   0        0        0     1101 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     2240 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.330139 bubble-sdk-0.1.6/bubble/
--rw-rw-rw-   0        0        0      802 2023-05-29 02:03:27.000000 bubble-sdk-0.1.6/bubble/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.345772 bubble-sdk-0.1.6/bubble/_utils/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/__init__.py
--rw-rw-rw-   0        0        0    29754 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/abi.py
--rw-rw-rw-   0        0        0      477 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/async_caching.py
--rw-rw-rw-   0        0        0     7956 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/async_transactions.py
--rw-rw-rw-   0        0        0     2136 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/blocks.py
--rw-rw-rw-   0        0        0     1028 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/caching.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.361400 bubble-sdk-0.1.6/bubble/_utils/compat/
--rw-rw-rw-   0        0        0      337 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/compat/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/compat/compat_py2.py
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/compat/compat_py3.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.361400 bubble-sdk-0.1.6/bubble/_utils/contract_sources/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/__init__.py
--rw-rw-rw-   0        0        0     6598 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/compile_contracts.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.361400 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/__init__.py
--rw-rw-rw-   0        0        0      538 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/_custom_contract_data.py
--rw-rw-rw-   0        0        0     5375 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/address_reflector.py
--rw-rw-rw-   0        0        0    18951 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/arrays_contract.py
--rw-rw-rw-   0        0        0    14866 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/bytes_contracts.py
--rw-rw-rw-   0        0        0     6169 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/constructor_contracts.py
--rw-rw-rw-   0        0        0     6395 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/contract_caller_tester.py
--rw-rw-rw-   0        0        0    38386 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/emitter_contract.py
--rw-rw-rw-   0        0        0     5670 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/event_contracts.py
--rw-rw-rw-   0        0        0    15916 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/extended_resolver.py
--rw-rw-rw-   0        0        0     1677 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/fallback_function_contract.py
--rw-rw-rw-   0        0        0     7712 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/math_contract.py
--rw-rw-rw-   0        0        0    16770 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/offchain_lookup.py
--rw-rw-rw-   0        0        0    32747 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/offchain_resolver.py
--rw-rw-rw-   0        0        0     1856 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/payable_tester.py
--rw-rw-rw-   0        0        0    17352 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/receive_function_contracts.py
--rw-rw-rw-   0        0        0     5295 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/reflector_contracts.py
--rw-rw-rw-   0        0        0     4324 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/revert_contract.py
--rw-rw-rw-   0        0        0     3586 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/simple_resolver.py
--rw-rw-rw-   0        0        0    11630 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/string_contract.py
--rw-rw-rw-   0        0        0    23337 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/tuple_contracts.py
--rw-rw-rw-   0        0        0    15485 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/contracts.py
--rw-rw-rw-   0        0        0     1701 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/datatypes.py
--rw-rw-rw-   0        0        0     1796 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/decorators.py
--rw-rw-rw-   0        0        0      157 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/empty.py
--rw-rw-rw-   0        0        0     9376 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/encoding.py
--rw-rw-rw-   0        0        0     2218 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/ens.py
--rw-rw-rw-   0        0        0    17730 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/events.py
--rw-rw-rw-   0        0        0     2176 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/fee_utils.py
--rw-rw-rw-   0        0        0    12297 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/filters.py
--rw-rw-rw-   0        0        0     3344 2023-05-23 08:51:59.000000 bubble-sdk-0.1.6/bubble/_utils/formatters.py
--rw-rw-rw-   0        0        0       61 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/function_identifiers.py
--rw-rw-rw-   0        0        0      204 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/http.py
--rw-rw-rw-   0        0        0      219 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/hypothesis.py
--rw-rw-rw-   0        0        0     1088 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/math.py
--rw-rw-rw-   0        0        0    33265 2023-05-25 08:40:49.000000 bubble-sdk-0.1.6/bubble/_utils/method_formatters.py
--rw-rw-rw-   0        0        0     3249 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.361400 bubble-sdk-0.1.6/bubble/_utils/module_testing/
--rw-rw-rw-   0        0        0      560 2023-05-22 07:05:55.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/__init__.py
--rw-rw-rw-   0        0        0   170862 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/eth_module.py
--rw-rw-rw-   0        0        0     3519 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_admin_module.py
--rw-rw-rw-   0        0        0    10645 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_personal_module.py
--rw-rw-rw-   0        0        0     1209 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_txpool_module.py
--rw-rw-rw-   0        0        0     4995 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/module_testing_utils.py
--rw-rw-rw-   0        0        0     1329 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/net_module.py
--rw-rw-rw-   0        0        0     9640 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/web3_module.py
--rw-rw-rw-   0        0        0     7132 2023-05-26 01:35:35.000000 bubble-sdk-0.1.6/bubble/_utils/normalizers.py
--rw-rw-rw-   0        0        0     9102 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/_utils/request.py
--rw-rw-rw-   0        0        0     8800 2023-05-25 08:41:34.000000 bubble-sdk-0.1.6/bubble/_utils/rpc_abi.py
--rw-rw-rw-   0        0        0     4374 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/_utils/threads.py
--rw-rw-rw-   0        0        0     9032 2023-05-26 02:16:43.000000 bubble-sdk-0.1.6/bubble/_utils/transactions.py
--rw-rw-rw-   0        0        0      846 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/type_conversion.py
--rw-rw-rw-   0        0        0     1727 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/_utils/utility_methods.py
--rw-rw-rw-   0        0        0     6509 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/validation.py
--rw-rw-rw-   0        0        0     1032 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/windows.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/auto/
--rw-rw-rw-   0        0        0       51 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/auto/__init__.py
--rw-rw-rw-   0        0        0      282 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/auto/gethdev.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/beacon/
--rw-rw-rw-   0        0        0       93 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/beacon/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-05-22 02:41:30.000000 bubble-sdk-0.1.6/bubble/beacon/api_endpoints.py
--rw-rw-rw-   0        0        0     5586 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/beacon/async_beacon.py
--rw-rw-rw-   0        0        0     4927 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/beacon/main.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/bub/
--rw-rw-rw-   0        0        0      176 2023-05-22 02:55:48.000000 bubble-sdk-0.1.6/bubble/bub/__init__.py
--rw-rw-rw-   0        0        0    19802 2023-05-25 08:16:36.000000 bubble-sdk-0.1.6/bubble/bub/async_bub.py
--rw-rw-rw-   0        0        0     6143 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/bub/base_bub.py
--rw-rw-rw-   0        0        0    17985 2023-05-25 08:17:34.000000 bubble-sdk-0.1.6/bubble/bub/bub.py
--rw-rw-rw-   0        0        0      406 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/contract/
--rw-rw-rw-   0        0        0      228 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/contract/__init__.py
--rw-rw-rw-   0        0        0    20413 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/contract/async_contract.py
--rw-rw-rw-   0        0        0    36847 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/contract/base_contract.py
--rw-rw-rw-   0        0        0    19453 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/contract/contract.py
--rw-rw-rw-   0        0        0    12794 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/contract/utils.py
--rw-rw-rw-   0        0        0     9390 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/datastructures.py
--rw-rw-rw-   0        0        0      827 2023-05-31 10:46:14.000000 bubble-sdk-0.1.6/bubble/debug.py
--rw-rw-rw-   0        0        0      257 2023-05-24 07:10:11.000000 bubble-sdk-0.1.6/bubble/dpos.py
--rw-rw-rw-   0        0        0     6563 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/gas_strategies/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/gas_strategies/__init__.py
--rw-rw-rw-   0        0        0      459 2023-05-25 08:17:34.000000 bubble-sdk-0.1.6/bubble/gas_strategies/rpc.py
--rw-rw-rw-   0        0        0     9277 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/gas_strategies/time_based.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/inner_contract/
--rw-rw-rw-   0        0        0      503 2023-05-25 02:11:17.000000 bubble-sdk-0.1.6/bubble/inner_contract/__init__.py
--rw-rw-rw-   0        0        0     3597 2023-05-24 07:08:55.000000 bubble-sdk-0.1.6/bubble/inner_contract/delegate.py
--rw-rw-rw-   0        0        0     5983 2023-05-23 10:08:11.000000 bubble-sdk-0.1.6/bubble/inner_contract/error_code.py
--rw-rw-rw-   0        0        0     6694 2023-05-31 09:47:08.000000 bubble-sdk-0.1.6/bubble/inner_contract/formatters.py
--rw-rw-rw-   0        0        0    10622 2023-05-31 09:47:30.000000 bubble-sdk-0.1.6/bubble/inner_contract/inner_contract.py
--rw-rw-rw-   0        0        0     9264 2023-05-31 10:37:37.000000 bubble-sdk-0.1.6/bubble/inner_contract/proposal.py
--rw-rw-rw-   0        0        0     1486 2023-05-24 07:26:08.000000 bubble-sdk-0.1.6/bubble/inner_contract/restricting.py
--rw-rw-rw-   0        0        0     1076 2023-05-24 07:26:26.000000 bubble-sdk-0.1.6/bubble/inner_contract/reward.py
--rw-rw-rw-   0        0        0     1747 2023-05-24 07:08:55.000000 bubble-sdk-0.1.6/bubble/inner_contract/slashing.py
--rw-rw-rw-   0        0        0     7134 2023-05-24 07:27:18.000000 bubble-sdk-0.1.6/bubble/inner_contract/staking.py
--rw-rw-rw-   0        0        0      208 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/logs.py
--rw-rw-rw-   0        0        0    13900 2023-05-25 09:00:17.000000 bubble-sdk-0.1.6/bubble/main.py
--rw-rw-rw-   0        0        0     8140 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/manager.py
--rw-rw-rw-   0        0        0     8699 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/method.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/middleware/
--rw-rw-rw-   0        0        0     3857 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/middleware/__init__.py
--rw-rw-rw-   0        0        0      252 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/middleware/abi.py
--rw-rw-rw-   0        0        0     2860 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/async_cache.py
--rw-rw-rw-   0        0        0     1858 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/middleware/attrdict.py
--rw-rw-rw-   0        0        0     1736 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/middleware/bub_poa.py
--rw-rw-rw-   0        0        0     1853 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/middleware/buffered_gas_estimate.py
--rw-rw-rw-   0        0        0    13010 2023-05-25 08:17:34.000000 bubble-sdk-0.1.6/bubble/middleware/cache.py
--rw-rw-rw-   0        0        0     1220 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/exception_handling.py
--rw-rw-rw-   0        0        0     3249 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/middleware/exception_retry_request.py
--rw-rw-rw-   0        0        0    21799 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/filter.py
--rw-rw-rw-   0        0        0     4742 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/middleware/fixture.py
--rw-rw-rw-   0        0        0     4929 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/middleware/formatting.py
--rw-rw-rw-   0        0        0     4345 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/middleware/gas_price_strategy.py
--rw-rw-rw-   0        0        0      628 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/names.py
--rw-rw-rw-   0        0        0      259 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/middleware/normalize_request_parameters.py
--rw-rw-rw-   0        0        0      367 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/pythonic.py
--rw-rw-rw-   0        0        0     4635 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/middleware/signing.py
--rw-rw-rw-   0        0        0     1061 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/middleware/simulate_unmined_transaction.py
--rw-rw-rw-   0        0        0     3865 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/middleware/stalecheck.py
--rw-rw-rw-   0        0        0     4757 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/middleware/validation.py
--rw-rw-rw-   0        0        0     3757 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/module.py
--rw-rw-rw-   0        0        0     1643 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/net.py
--rw-rw-rw-   0        0        0    11907 2023-05-25 08:37:41.000000 bubble-sdk-0.1.6/bubble/node.py
--rw-rw-rw-   0        0        0    22263 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/pm.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/providers/
--rw-rw-rw-   0        0        0      387 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/providers/__init__.py
--rw-rw-rw-   0        0        0     4320 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/providers/async_base.py
--rw-rw-rw-   0        0        0     2567 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/providers/async_rpc.py
--rw-rw-rw-   0        0        0     3576 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/providers/auto.py
--rw-rw-rw-   0        0        0     4254 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/providers/base.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/providers/bub_tester/
--rw-rw-rw-   0        0        0       99 2023-05-22 06:53:52.000000 bubble-sdk-0.1.6/bubble/providers/bub_tester/__init__.py
--rw-rw-rw-   0        0        0    14864 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/providers/bub_tester/defaults.py
--rw-rw-rw-   0        0        0     5690 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/providers/bub_tester/main.py
--rw-rw-rw-   0        0        0    13288 2023-05-26 02:23:29.000000 bubble-sdk-0.1.6/bubble/providers/bub_tester/middleware.py
--rw-rw-rw-   0        0        0     6758 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/providers/ipc.py
--rw-rw-rw-   0        0        0     2796 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/providers/rpc.py
--rw-rw-rw-   0        0        0     4062 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/providers/websocket.py
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/scripts/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/scripts/release/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/scripts/release/__init__.py
--rw-rw-rw-   0        0        0     1594 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/scripts/release/test_package.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/tools/
--rw-rw-rw-   0        0        0       75 2023-05-22 03:56:23.000000 bubble-sdk-0.1.6/bubble/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/tools/benchmark/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/__init__.py
--rw-rw-rw-   0        0        0     6098 2023-05-25 08:17:34.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/main.py
--rw-rw-rw-   0        0        0     3542 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/node.py
--rw-rw-rw-   0        0        0      951 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/reporting.py
--rw-rw-rw-   0        0        0     1791 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.408275 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/__init__.py
--rw-rw-rw-   0        0        0     4307 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/_utils.py
--rw-rw-rw-   0        0        0     1471 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/deployer.py
--rw-rw-rw-   0        0        0      402 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/exceptions.py
--rw-rw-rw-   0        0        0     4053 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/linker.py
--rw-rw-rw-   0        0        0      680 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/plugins.py
--rw-rw-rw-   0        0        0     3302 2023-05-25 08:43:00.000000 bubble-sdk-0.1.6/bubble/tracing.py
--rw-rw-rw-   0        0        0    13659 2023-05-24 07:08:55.000000 bubble-sdk-0.1.6/bubble/types.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.408275 bubble-sdk-0.1.6/bubble/utils/
--rw-rw-rw-   0        0        0      472 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/utils/__init__.py
--rw-rw-rw-   0        0        0      521 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/utils/abi.py
--rw-rw-rw-   0        0        0     1008 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/utils/address.py
--rw-rw-rw-   0        0        0     3199 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/utils/async_exception_handling.py
--rw-rw-rw-   0        0        0     1569 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/utils/caching.py
--rw-rw-rw-   0        0        0     3157 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/utils/exception_handling.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.408275 bubble-sdk-0.1.6/bubble_sdk.egg-info/
--rw-rw-rw-   0        0        0     2240 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6916 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-31 10:56:52.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1174 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ens/
--rw-rw-rw-   0        0        0      305 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/__init__.py
--rw-rw-rw-   0        0        0    24627 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/abis.py
--rw-rw-rw-   0        0        0    21480 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/ens/async_ens.py
--rw-rw-rw-   0        0        0       46 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/auto.py
--rw-rw-rw-   0        0        0     3412 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/ens/base_ens.py
--rw-rw-rw-   0        0        0      629 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/constants.py
--rw-rw-rw-   0        0        0   199146 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/ens/contract_data.py
--rw-rw-rw-   0        0        0    20613 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/ens/ens.py
--rw-rw-rw-   0        0        0     2511 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/exceptions.py
--rw-rw-rw-   0        0        0     9333 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/ens/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/
--rw-rw-rw-   0        0        0      775 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/_utils/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/__init__.py
--rw-rw-rw-   0        0        0     2604 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/_utils/backend.py
--rw-rw-rw-   0        0        0     1521 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/cache.py
--rw-rw-rw-   0        0        0     2969 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/ethpm/_utils/chains.py
--rw-rw-rw-   0        0        0     1065 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/contract.py
--rw-rw-rw-   0        0        0     5410 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/ethpm/_utils/deployments.py
--rw-rw-rw-   0        0        0     2835 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/ethpm/_utils/ipfs.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/_utils/protobuf/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/protobuf/__init__.py
--rw-rw-rw-   0        0        0     1971 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/protobuf/ipfs_file_pb2.py
--rw-rw-rw-   0        0        0     1517 2023-05-22 02:41:29.000000 bubble-sdk-0.1.6/ethpm/_utils/registry.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/assets/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/backends/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/backends/__init__.py
--rw-rw-rw-   0        0        0      999 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/backends/base.py
--rw-rw-rw-   0        0        0     3114 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/backends/http.py
--rw-rw-rw-   0        0        0     6772 2023-05-23 08:08:32.000000 bubble-sdk-0.1.6/ethpm/backends/ipfs.py
--rw-rw-rw-   0        0        0     4332 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/ethpm/backends/registry.py
--rw-rw-rw-   0        0        0      422 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/constants.py
--rw-rw-rw-   0        0        0     6448 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/ethpm/contract.py
--rw-rw-rw-   0        0        0     1948 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/dependencies.py
--rw-rw-rw-   0        0        0     2218 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/ethpm/deployments.py
--rw-rw-rw-   0        0        0     1262 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/exceptions.py
--rw-rw-rw-   0        0        0    14939 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/ethpm/package.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/ethpm/tools/
--rw-rw-rw-   0        0        0      107 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/tools/__init__.py
--rw-rw-rw-   0        0        0    27981 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/ethpm/tools/builder.py
--rw-rw-rw-   0        0        0    10687 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/ethpm/tools/checker.py
--rw-rw-rw-   0        0        0      494 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/tools/get_manifest.py
--rw-rw-rw-   0        0        0     4513 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/ethpm/uri.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/ethpm/validation/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/validation/__init__.py
--rw-rw-rw-   0        0        0     4862 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/validation/manifest.py
--rw-rw-rw-   0        0        0     1115 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/ethpm/validation/misc.py
--rw-rw-rw-   0        0        0     2397 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/validation/package.py
--rw-rw-rw-   0        0        0     5038 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/ethpm/validation/uri.py
--rw-rw-rw-   0        0        0       42 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     3300 2023-05-31 10:59:05.000000 bubble-sdk-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.217649 bubble-sdk-0.1.7/
+-rw-rw-rw-   0        0        0     1101 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2240 2023-06-13 03:21:00.216650 bubble-sdk-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.098855 bubble-sdk-0.1.7/bubble/
+-rw-rw-rw-   0        0        0      802 2023-05-29 02:03:27.000000 bubble-sdk-0.1.7/bubble/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.119135 bubble-sdk-0.1.7/bubble/_utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/__init__.py
+-rw-rw-rw-   0        0        0    29754 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/_utils/abi.py
+-rw-rw-rw-   0        0        0      477 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/async_caching.py
+-rw-rw-rw-   0        0        0     7956 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/_utils/async_transactions.py
+-rw-rw-rw-   0        0        0     2136 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/_utils/blocks.py
+-rw-rw-rw-   0        0        0     1028 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/caching.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.120136 bubble-sdk-0.1.7/bubble/_utils/compat/
+-rw-rw-rw-   0        0        0      337 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/_utils/compat/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/compat/compat_py2.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/compat/compat_py3.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.121135 bubble-sdk-0.1.7/bubble/_utils/contract_sources/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/__init__.py
+-rw-rw-rw-   0        0        0     6598 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/compile_contracts.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.137066 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/_custom_contract_data.py
+-rw-rw-rw-   0        0        0     5375 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/address_reflector.py
+-rw-rw-rw-   0        0        0    18951 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/arrays_contract.py
+-rw-rw-rw-   0        0        0    14866 2023-05-23 08:08:30.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/bytes_contracts.py
+-rw-rw-rw-   0        0        0     6169 2023-05-23 08:08:30.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/constructor_contracts.py
+-rw-rw-rw-   0        0        0     6395 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/contract_caller_tester.py
+-rw-rw-rw-   0        0        0    38386 2023-05-23 08:08:30.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/emitter_contract.py
+-rw-rw-rw-   0        0        0     5670 2023-05-23 08:08:20.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/event_contracts.py
+-rw-rw-rw-   0        0        0    15916 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/extended_resolver.py
+-rw-rw-rw-   0        0        0     1677 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/fallback_function_contract.py
+-rw-rw-rw-   0        0        0     7712 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/math_contract.py
+-rw-rw-rw-   0        0        0    16770 2023-05-23 08:08:24.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/offchain_lookup.py
+-rw-rw-rw-   0        0        0    32747 2023-05-23 08:08:24.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/offchain_resolver.py
+-rw-rw-rw-   0        0        0     1856 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/payable_tester.py
+-rw-rw-rw-   0        0        0    17352 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/receive_function_contracts.py
+-rw-rw-rw-   0        0        0     5295 2023-05-23 08:08:24.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/reflector_contracts.py
+-rw-rw-rw-   0        0        0     4324 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/revert_contract.py
+-rw-rw-rw-   0        0        0     3586 2023-05-23 08:08:20.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/simple_resolver.py
+-rw-rw-rw-   0        0        0    11630 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/string_contract.py
+-rw-rw-rw-   0        0        0    23337 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/tuple_contracts.py
+-rw-rw-rw-   0        0        0    15485 2023-05-23 08:08:30.000000 bubble-sdk-0.1.7/bubble/_utils/contracts.py
+-rw-rw-rw-   0        0        0     1701 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/datatypes.py
+-rw-rw-rw-   0        0        0     1796 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/decorators.py
+-rw-rw-rw-   0        0        0      157 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/_utils/empty.py
+-rw-rw-rw-   0        0        0     9376 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/_utils/encoding.py
+-rw-rw-rw-   0        0        0     2218 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/_utils/ens.py
+-rw-rw-rw-   0        0        0    17730 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/_utils/events.py
+-rw-rw-rw-   0        0        0     2176 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/_utils/fee_utils.py
+-rw-rw-rw-   0        0        0    12297 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/_utils/filters.py
+-rw-rw-rw-   0        0        0     3344 2023-05-23 08:51:59.000000 bubble-sdk-0.1.7/bubble/_utils/formatters.py
+-rw-rw-rw-   0        0        0       61 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/function_identifiers.py
+-rw-rw-rw-   0        0        0      204 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/_utils/http.py
+-rw-rw-rw-   0        0        0      219 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/hypothesis.py
+-rw-rw-rw-   0        0        0     1088 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/_utils/math.py
+-rw-rw-rw-   0        0        0    33273 2023-06-13 03:16:03.000000 bubble-sdk-0.1.7/bubble/_utils/method_formatters.py
+-rw-rw-rw-   0        0        0     3249 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/_utils/module.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.142065 bubble-sdk-0.1.7/bubble/_utils/module_testing/
+-rw-rw-rw-   0        0        0      560 2023-05-22 07:05:55.000000 bubble-sdk-0.1.7/bubble/_utils/module_testing/__init__.py
+-rw-rw-rw-   0        0        0   170862 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/_utils/module_testing/eth_module.py
+-rw-rw-rw-   0        0        0     3519 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/_utils/module_testing/go_ethereum_admin_module.py
+-rw-rw-rw-   0        0        0    10645 2023-05-23 08:08:25.000000 bubble-sdk-0.1.7/bubble/_utils/module_testing/go_ethereum_personal_module.py
+-rw-rw-rw-   0        0        0     1209 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/_utils/module_testing/go_ethereum_txpool_module.py
+-rw-rw-rw-   0        0        0     4995 2023-05-23 08:08:20.000000 bubble-sdk-0.1.7/bubble/_utils/module_testing/module_testing_utils.py
+-rw-rw-rw-   0        0        0     1329 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/_utils/module_testing/net_module.py
+-rw-rw-rw-   0        0        0     9640 2023-05-23 08:08:30.000000 bubble-sdk-0.1.7/bubble/_utils/module_testing/web3_module.py
+-rw-rw-rw-   0        0        0     7132 2023-05-26 01:35:35.000000 bubble-sdk-0.1.7/bubble/_utils/normalizers.py
+-rw-rw-rw-   0        0        0     9102 2023-05-23 08:08:25.000000 bubble-sdk-0.1.7/bubble/_utils/request.py
+-rw-rw-rw-   0        0        0     8944 2023-06-05 06:31:36.000000 bubble-sdk-0.1.7/bubble/_utils/rpc_abi.py
+-rw-rw-rw-   0        0        0     4374 2023-05-23 08:08:24.000000 bubble-sdk-0.1.7/bubble/_utils/threads.py
+-rw-rw-rw-   0        0        0     9032 2023-05-26 02:16:43.000000 bubble-sdk-0.1.7/bubble/_utils/transactions.py
+-rw-rw-rw-   0        0        0      846 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/type_conversion.py
+-rw-rw-rw-   0        0        0     1727 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/_utils/utility_methods.py
+-rw-rw-rw-   0        0        0     6509 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/_utils/validation.py
+-rw-rw-rw-   0        0        0     1032 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/_utils/windows.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.143070 bubble-sdk-0.1.7/bubble/auto/
+-rw-rw-rw-   0        0        0       51 2023-05-23 08:08:20.000000 bubble-sdk-0.1.7/bubble/auto/__init__.py
+-rw-rw-rw-   0        0        0      282 2023-05-23 08:08:20.000000 bubble-sdk-0.1.7/bubble/auto/gethdev.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.145064 bubble-sdk-0.1.7/bubble/beacon/
+-rw-rw-rw-   0        0        0       93 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/beacon/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-05-22 02:41:30.000000 bubble-sdk-0.1.7/bubble/beacon/api_endpoints.py
+-rw-rw-rw-   0        0        0     5586 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/beacon/async_beacon.py
+-rw-rw-rw-   0        0        0     4927 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/beacon/main.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.146065 bubble-sdk-0.1.7/bubble/bub/
+-rw-rw-rw-   0        0        0      176 2023-05-22 02:55:48.000000 bubble-sdk-0.1.7/bubble/bub/__init__.py
+-rw-rw-rw-   0        0        0    19802 2023-05-25 08:16:36.000000 bubble-sdk-0.1.7/bubble/bub/async_bub.py
+-rw-rw-rw-   0        0        0     6143 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/bub/base_bub.py
+-rw-rw-rw-   0        0        0    17985 2023-05-25 08:17:34.000000 bubble-sdk-0.1.7/bubble/bub/bub.py
+-rw-rw-rw-   0        0        0      406 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.149069 bubble-sdk-0.1.7/bubble/contract/
+-rw-rw-rw-   0        0        0      228 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/contract/__init__.py
+-rw-rw-rw-   0        0        0    20413 2023-05-23 08:08:25.000000 bubble-sdk-0.1.7/bubble/contract/async_contract.py
+-rw-rw-rw-   0        0        0    36847 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/contract/base_contract.py
+-rw-rw-rw-   0        0        0    19453 2023-05-23 08:08:20.000000 bubble-sdk-0.1.7/bubble/contract/contract.py
+-rw-rw-rw-   0        0        0    12794 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/contract/utils.py
+-rw-rw-rw-   0        0        0     9390 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/datastructures.py
+-rw-rw-rw-   0        0        0      827 2023-05-31 10:46:14.000000 bubble-sdk-0.1.7/bubble/debug.py
+-rw-rw-rw-   0        0        0      257 2023-05-24 07:10:11.000000 bubble-sdk-0.1.7/bubble/dpos.py
+-rw-rw-rw-   0        0        0     6563 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.150071 bubble-sdk-0.1.7/bubble/gas_strategies/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/gas_strategies/__init__.py
+-rw-rw-rw-   0        0        0      459 2023-05-25 08:17:34.000000 bubble-sdk-0.1.7/bubble/gas_strategies/rpc.py
+-rw-rw-rw-   0        0        0     9277 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/gas_strategies/time_based.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.155071 bubble-sdk-0.1.7/bubble/inner_contract/
+-rw-rw-rw-   0        0        0      503 2023-05-25 02:11:17.000000 bubble-sdk-0.1.7/bubble/inner_contract/__init__.py
+-rw-rw-rw-   0        0        0     3553 2023-06-06 07:37:18.000000 bubble-sdk-0.1.7/bubble/inner_contract/delegate.py
+-rw-rw-rw-   0        0        0     5983 2023-05-23 10:08:11.000000 bubble-sdk-0.1.7/bubble/inner_contract/error_code.py
+-rw-rw-rw-   0        0        0     6694 2023-05-31 09:47:08.000000 bubble-sdk-0.1.7/bubble/inner_contract/formatters.py
+-rw-rw-rw-   0        0        0    10622 2023-05-31 09:47:30.000000 bubble-sdk-0.1.7/bubble/inner_contract/inner_contract.py
+-rw-rw-rw-   0        0        0     9246 2023-06-06 07:37:23.000000 bubble-sdk-0.1.7/bubble/inner_contract/proposal.py
+-rw-rw-rw-   0        0        0     1486 2023-05-24 07:26:08.000000 bubble-sdk-0.1.7/bubble/inner_contract/restricting.py
+-rw-rw-rw-   0        0        0     1032 2023-06-06 07:37:28.000000 bubble-sdk-0.1.7/bubble/inner_contract/reward.py
+-rw-rw-rw-   0        0        0     1703 2023-06-06 07:37:13.000000 bubble-sdk-0.1.7/bubble/inner_contract/slashing.py
+-rw-rw-rw-   0        0        0     7134 2023-05-24 07:27:18.000000 bubble-sdk-0.1.7/bubble/inner_contract/staking.py
+-rw-rw-rw-   0        0        0      208 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/logs.py
+-rw-rw-rw-   0        0        0    13900 2023-05-25 09:00:17.000000 bubble-sdk-0.1.7/bubble/main.py
+-rw-rw-rw-   0        0        0     8140 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/manager.py
+-rw-rw-rw-   0        0        0     8699 2023-05-23 08:08:20.000000 bubble-sdk-0.1.7/bubble/method.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.162807 bubble-sdk-0.1.7/bubble/middleware/
+-rw-rw-rw-   0        0        0     3857 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/middleware/__init__.py
+-rw-rw-rw-   0        0        0      252 2023-05-23 08:08:25.000000 bubble-sdk-0.1.7/bubble/middleware/abi.py
+-rw-rw-rw-   0        0        0     2860 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/middleware/async_cache.py
+-rw-rw-rw-   0        0        0     1858 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/middleware/attrdict.py
+-rw-rw-rw-   0        0        0     1736 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/middleware/bub_poa.py
+-rw-rw-rw-   0        0        0     1853 2023-05-23 08:08:24.000000 bubble-sdk-0.1.7/bubble/middleware/buffered_gas_estimate.py
+-rw-rw-rw-   0        0        0    13010 2023-05-25 08:17:34.000000 bubble-sdk-0.1.7/bubble/middleware/cache.py
+-rw-rw-rw-   0        0        0     1220 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/middleware/exception_handling.py
+-rw-rw-rw-   0        0        0     3249 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/middleware/exception_retry_request.py
+-rw-rw-rw-   0        0        0    21799 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/middleware/filter.py
+-rw-rw-rw-   0        0        0     4742 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/middleware/fixture.py
+-rw-rw-rw-   0        0        0     4929 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/middleware/formatting.py
+-rw-rw-rw-   0        0        0     4345 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/middleware/gas_price_strategy.py
+-rw-rw-rw-   0        0        0      628 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/middleware/names.py
+-rw-rw-rw-   0        0        0      259 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/middleware/normalize_request_parameters.py
+-rw-rw-rw-   0        0        0      367 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/middleware/pythonic.py
+-rw-rw-rw-   0        0        0     4635 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/middleware/signing.py
+-rw-rw-rw-   0        0        0     1061 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/middleware/simulate_unmined_transaction.py
+-rw-rw-rw-   0        0        0     3865 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/middleware/stalecheck.py
+-rw-rw-rw-   0        0        0     4757 2023-06-13 03:20:35.000000 bubble-sdk-0.1.7/bubble/middleware/validation.py
+-rw-rw-rw-   0        0        0     3757 2023-05-23 08:08:25.000000 bubble-sdk-0.1.7/bubble/module.py
+-rw-rw-rw-   0        0        0     1643 2023-05-23 08:08:24.000000 bubble-sdk-0.1.7/bubble/net.py
+-rw-rw-rw-   0        0        0    12176 2023-06-05 06:30:47.000000 bubble-sdk-0.1.7/bubble/node.py
+-rw-rw-rw-   0        0        0    22263 2023-05-23 08:08:30.000000 bubble-sdk-0.1.7/bubble/pm.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.166124 bubble-sdk-0.1.7/bubble/providers/
+-rw-rw-rw-   0        0        0      387 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/providers/__init__.py
+-rw-rw-rw-   0        0        0     4320 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/bubble/providers/async_base.py
+-rw-rw-rw-   0        0        0     2567 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/providers/async_rpc.py
+-rw-rw-rw-   0        0        0     3576 2023-05-23 08:08:25.000000 bubble-sdk-0.1.7/bubble/providers/auto.py
+-rw-rw-rw-   0        0        0     4254 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/providers/base.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.169133 bubble-sdk-0.1.7/bubble/providers/bub_tester/
+-rw-rw-rw-   0        0        0       99 2023-05-22 06:53:52.000000 bubble-sdk-0.1.7/bubble/providers/bub_tester/__init__.py
+-rw-rw-rw-   0        0        0    14864 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/providers/bub_tester/defaults.py
+-rw-rw-rw-   0        0        0     5690 2023-05-23 08:08:25.000000 bubble-sdk-0.1.7/bubble/providers/bub_tester/main.py
+-rw-rw-rw-   0        0        0    13288 2023-05-26 02:23:29.000000 bubble-sdk-0.1.7/bubble/providers/bub_tester/middleware.py
+-rw-rw-rw-   0        0        0     6758 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/providers/ipc.py
+-rw-rw-rw-   0        0        0     2796 2023-05-23 08:08:30.000000 bubble-sdk-0.1.7/bubble/providers/rpc.py
+-rw-rw-rw-   0        0        0     4062 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/providers/websocket.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.169133 bubble-sdk-0.1.7/bubble/scripts/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.170138 bubble-sdk-0.1.7/bubble/scripts/release/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/scripts/release/__init__.py
+-rw-rw-rw-   0        0        0     1594 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/scripts/release/test_package.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.171130 bubble-sdk-0.1.7/bubble/tools/
+-rw-rw-rw-   0        0        0       75 2023-05-22 03:56:23.000000 bubble-sdk-0.1.7/bubble/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.173131 bubble-sdk-0.1.7/bubble/tools/benchmark/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/tools/benchmark/__init__.py
+-rw-rw-rw-   0        0        0     6098 2023-05-25 08:17:34.000000 bubble-sdk-0.1.7/bubble/tools/benchmark/main.py
+-rw-rw-rw-   0        0        0     3542 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/tools/benchmark/node.py
+-rw-rw-rw-   0        0        0      951 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/tools/benchmark/reporting.py
+-rw-rw-rw-   0        0        0     1791 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/tools/benchmark/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.175131 bubble-sdk-0.1.7/bubble/tools/pytest_bubble/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/tools/pytest_bubble/__init__.py
+-rw-rw-rw-   0        0        0     4307 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/bubble/tools/pytest_bubble/_utils.py
+-rw-rw-rw-   0        0        0     1471 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/tools/pytest_bubble/deployer.py
+-rw-rw-rw-   0        0        0      402 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/tools/pytest_bubble/exceptions.py
+-rw-rw-rw-   0        0        0     4053 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/bubble/tools/pytest_bubble/linker.py
+-rw-rw-rw-   0        0        0      680 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/bubble/tools/pytest_bubble/plugins.py
+-rw-rw-rw-   0        0        0     3302 2023-05-25 08:43:00.000000 bubble-sdk-0.1.7/bubble/tracing.py
+-rw-rw-rw-   0        0        0    13659 2023-05-24 07:08:55.000000 bubble-sdk-0.1.7/bubble/types.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.178132 bubble-sdk-0.1.7/bubble/utils/
+-rw-rw-rw-   0        0        0      472 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/utils/__init__.py
+-rw-rw-rw-   0        0        0      521 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/utils/abi.py
+-rw-rw-rw-   0        0        0     1008 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/bubble/utils/address.py
+-rw-rw-rw-   0        0        0     3199 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/bubble/utils/async_exception_handling.py
+-rw-rw-rw-   0        0        0     1569 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/bubble/utils/caching.py
+-rw-rw-rw-   0        0        0     3157 2023-05-23 08:08:25.000000 bubble-sdk-0.1.7/bubble/utils/exception_handling.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.189131 bubble-sdk-0.1.7/bubble_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2240 2023-06-13 03:20:59.000000 bubble-sdk-0.1.7/bubble_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6916 2023-06-13 03:21:00.000000 bubble-sdk-0.1.7/bubble_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 03:20:59.000000 bubble-sdk-0.1.7/bubble_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-13 03:20:59.000000 bubble-sdk-0.1.7/bubble_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-13 03:20:59.000000 bubble-sdk-0.1.7/bubble_sdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     1174 2023-06-13 03:20:59.000000 bubble-sdk-0.1.7/bubble_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-13 03:20:59.000000 bubble-sdk-0.1.7/bubble_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.195130 bubble-sdk-0.1.7/ens/
+-rw-rw-rw-   0        0        0      305 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ens/__init__.py
+-rw-rw-rw-   0        0        0    24627 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ens/abis.py
+-rw-rw-rw-   0        0        0    21480 2023-05-23 08:08:30.000000 bubble-sdk-0.1.7/ens/async_ens.py
+-rw-rw-rw-   0        0        0       46 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ens/auto.py
+-rw-rw-rw-   0        0        0     3412 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/ens/base_ens.py
+-rw-rw-rw-   0        0        0      629 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ens/constants.py
+-rw-rw-rw-   0        0        0   199146 2023-05-23 08:08:30.000000 bubble-sdk-0.1.7/ens/contract_data.py
+-rw-rw-rw-   0        0        0    20613 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/ens/ens.py
+-rw-rw-rw-   0        0        0     2511 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ens/exceptions.py
+-rw-rw-rw-   0        0        0     9333 2023-05-23 08:08:27.000000 bubble-sdk-0.1.7/ens/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.199133 bubble-sdk-0.1.7/ethpm/
+-rw-rw-rw-   0        0        0      775 2023-05-22 03:42:55.000000 bubble-sdk-0.1.7/ethpm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.205134 bubble-sdk-0.1.7/ethpm/_utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/_utils/__init__.py
+-rw-rw-rw-   0        0        0     2604 2023-05-22 03:42:55.000000 bubble-sdk-0.1.7/ethpm/_utils/backend.py
+-rw-rw-rw-   0        0        0     1521 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/_utils/cache.py
+-rw-rw-rw-   0        0        0     2969 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/ethpm/_utils/chains.py
+-rw-rw-rw-   0        0        0     1065 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/_utils/contract.py
+-rw-rw-rw-   0        0        0     5410 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/ethpm/_utils/deployments.py
+-rw-rw-rw-   0        0        0     2835 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/ethpm/_utils/ipfs.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.206131 bubble-sdk-0.1.7/ethpm/_utils/protobuf/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/_utils/protobuf/__init__.py
+-rw-rw-rw-   0        0        0     1971 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/_utils/protobuf/ipfs_file_pb2.py
+-rw-rw-rw-   0        0        0     1517 2023-05-22 02:41:29.000000 bubble-sdk-0.1.7/ethpm/_utils/registry.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.207130 bubble-sdk-0.1.7/ethpm/assets/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.210649 bubble-sdk-0.1.7/ethpm/backends/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/backends/__init__.py
+-rw-rw-rw-   0        0        0      999 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/backends/base.py
+-rw-rw-rw-   0        0        0     3114 2023-05-22 03:42:55.000000 bubble-sdk-0.1.7/ethpm/backends/http.py
+-rw-rw-rw-   0        0        0     6772 2023-05-23 08:08:32.000000 bubble-sdk-0.1.7/ethpm/backends/ipfs.py
+-rw-rw-rw-   0        0        0     4332 2023-05-23 08:08:25.000000 bubble-sdk-0.1.7/ethpm/backends/registry.py
+-rw-rw-rw-   0        0        0      422 2023-05-22 03:42:55.000000 bubble-sdk-0.1.7/ethpm/constants.py
+-rw-rw-rw-   0        0        0     6448 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/ethpm/contract.py
+-rw-rw-rw-   0        0        0     1948 2023-05-22 03:42:55.000000 bubble-sdk-0.1.7/ethpm/dependencies.py
+-rw-rw-rw-   0        0        0     2218 2023-05-23 08:08:29.000000 bubble-sdk-0.1.7/ethpm/deployments.py
+-rw-rw-rw-   0        0        0     1262 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/exceptions.py
+-rw-rw-rw-   0        0        0    14939 2023-05-23 08:08:20.000000 bubble-sdk-0.1.7/ethpm/package.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.212650 bubble-sdk-0.1.7/ethpm/tools/
+-rw-rw-rw-   0        0        0      107 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/tools/__init__.py
+-rw-rw-rw-   0        0        0    27981 2023-05-23 08:08:21.000000 bubble-sdk-0.1.7/ethpm/tools/builder.py
+-rw-rw-rw-   0        0        0    10687 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/ethpm/tools/checker.py
+-rw-rw-rw-   0        0        0      494 2023-05-22 03:42:55.000000 bubble-sdk-0.1.7/ethpm/tools/get_manifest.py
+-rw-rw-rw-   0        0        0     4513 2023-05-23 08:08:26.000000 bubble-sdk-0.1.7/ethpm/uri.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:00.215650 bubble-sdk-0.1.7/ethpm/validation/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.7/ethpm/validation/__init__.py
+-rw-rw-rw-   0        0        0     4862 2023-05-22 03:42:55.000000 bubble-sdk-0.1.7/ethpm/validation/manifest.py
+-rw-rw-rw-   0        0        0     1115 2023-05-23 08:08:31.000000 bubble-sdk-0.1.7/ethpm/validation/misc.py
+-rw-rw-rw-   0        0        0     2397 2023-05-22 03:42:55.000000 bubble-sdk-0.1.7/ethpm/validation/package.py
+-rw-rw-rw-   0        0        0     5038 2023-05-23 08:08:28.000000 bubble-sdk-0.1.7/ethpm/validation/uri.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 03:21:00.217649 bubble-sdk-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     3300 2023-06-13 03:17:45.000000 bubble-sdk-0.1.7/setup.py
```

### Comparing `bubble-sdk-0.1.6/LICENSE` & `bubble-sdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/PKG-INFO` & `bubble-sdk-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Bubble sdk
 Home-page: https://github.com/shinnng/bubble.py
 Author: Shing
 Author-email: Shinnng@outlook.com
 License: MIT
 Keywords: bubble
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bubble-sdk-0.1.6/README.md` & `bubble-sdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/__init__.py` & `bubble-sdk-0.1.7/bubble/__init__.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/abi.py` & `bubble-sdk-0.1.7/bubble/_utils/abi.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/async_transactions.py` & `bubble-sdk-0.1.7/bubble/_utils/async_transactions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/blocks.py` & `bubble-sdk-0.1.7/bubble/_utils/blocks.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/caching.py` & `bubble-sdk-0.1.7/bubble/_utils/caching.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/compile_contracts.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/compile_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/_custom_contract_data.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/_custom_contract_data.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/address_reflector.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/address_reflector.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/arrays_contract.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/arrays_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/bytes_contracts.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/bytes_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/constructor_contracts.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/constructor_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/contract_caller_tester.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/contract_caller_tester.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/emitter_contract.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/event_contracts.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/event_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/extended_resolver.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/extended_resolver.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/fallback_function_contract.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/fallback_function_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/math_contract.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/math_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/offchain_lookup.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/offchain_lookup.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/offchain_resolver.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/offchain_resolver.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/payable_tester.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/payable_tester.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/receive_function_contracts.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/receive_function_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/reflector_contracts.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/reflector_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/revert_contract.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/revert_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/simple_resolver.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/simple_resolver.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/string_contract.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/string_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/tuple_contracts.py` & `bubble-sdk-0.1.7/bubble/_utils/contract_sources/contract_data/tuple_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/contracts.py` & `bubble-sdk-0.1.7/bubble/_utils/contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/datatypes.py` & `bubble-sdk-0.1.7/bubble/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/decorators.py` & `bubble-sdk-0.1.7/bubble/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/encoding.py` & `bubble-sdk-0.1.7/bubble/_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/ens.py` & `bubble-sdk-0.1.7/bubble/_utils/ens.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/events.py` & `bubble-sdk-0.1.7/bubble/_utils/events.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/fee_utils.py` & `bubble-sdk-0.1.7/bubble/_utils/fee_utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/filters.py` & `bubble-sdk-0.1.7/bubble/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/formatters.py` & `bubble-sdk-0.1.7/bubble/_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/math.py` & `bubble-sdk-0.1.7/bubble/_utils/math.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/method_formatters.py` & `bubble-sdk-0.1.7/bubble/_utils/method_formatters.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,23 +129,23 @@
 is_false = partial(operator.is_, False)
 is_not_false = complement(is_false)
 is_not_null = complement(is_null)
 
 
 @curry
 def to_hexbytes(
-    num_bytes: int, val: Union[str, int, bytes], variable_length: bool = False
+        num_bytes: int, val: Union[str, int, bytes], variable_length: bool = False
 ) -> HexBytes:
     if isinstance(val, (str, int, bytes)):
         result = HexBytes(val)
     else:
         raise TypeError(f"Cannot convert {val!r} to HexBytes")
 
     extra_bytes = len(result) - num_bytes
-    if extra_bytes == 0 or (variable_length and extra_bytes < 0):
+    if extra_bytes == 0 or not variable_length:
         return result
     elif all(byte == 0 for byte in result[:extra_bytes]):
         return HexBytes(result[extra_bytes:])
     else:
         raise ValueError(
             f"The value {result!r} is {len(result)} bytes, but should be {num_bytes}"
         )
@@ -153,32 +153,32 @@
 
 def is_attrdict(val: Any) -> bool:
     return isinstance(val, AttributeDict)
 
 
 @curry
 def type_aware_apply_formatters_to_dict(
-    formatters: Formatters,
-    value: Union[AttributeDict[str, Any], Dict[str, Any]],
+        formatters: Formatters,
+        value: Union[AttributeDict[str, Any], Dict[str, Any]],
 ) -> Union[ReadableAttributeDict[str, Any], Dict[str, Any]]:
     """
     Preserve ``AttributeDict`` types if original ``value`` was an ``AttributeDict``.
     """
     formatted_dict: Dict[str, Any] = apply_formatters_to_dict(formatters, dict(value))
     return (
         AttributeDict.recursive(formatted_dict)
         if is_attrdict(value)
         else formatted_dict
     )
 
 
 def type_aware_apply_formatters_to_dict_keys_and_values(
-    key_formatters: Callable[[Any], Any],
-    value_formatters: Callable[[Any], Any],
-    dict_like_object: Union[AttributeDict[str, Any], Dict[str, Any]],
+        key_formatters: Callable[[Any], Any],
+        value_formatters: Callable[[Any], Any],
+        dict_like_object: Union[AttributeDict[str, Any], Dict[str, Any]],
 ) -> Union[ReadableAttributeDict[str, Any], Dict[str, Any]]:
     """
     Preserve ``AttributeDict`` types if original ``value`` was an ``AttributeDict``.
     """
     formatted_dict = dict(
         (key_formatters(k), value_formatters(v)) for k, v in dict_like_object.items()
     )
@@ -208,15 +208,14 @@
     "hash": to_hexbytes(32),
     "v": apply_formatter_if(is_not_null, to_integer_if_hex),
     "standardV": apply_formatter_if(is_not_null, to_integer_if_hex),
     "type": apply_formatter_if(is_not_null, to_integer_if_hex),
     "chainId": apply_formatter_if(is_not_null, to_integer_if_hex),
 }
 
-
 transaction_result_formatter = type_aware_apply_formatters_to_dict(
     TRANSACTION_RESULT_FORMATTERS
 )
 
 WITHDRAWAL_RESULT_FORMATTERS = {
     "index": to_integer_if_hex,
     "validatorIndex": to_integer_if_hex,
@@ -239,18 +238,16 @@
     "transactionHash": apply_formatter_if(is_not_null, to_hexbytes(32)),
     "logIndex": to_integer_if_hex,
     "address": to_checksum_address,
     "topics": apply_list_to_array_formatter(to_hexbytes(32)),
     "data": HexBytes,
 }
 
-
 log_entry_formatter = type_aware_apply_formatters_to_dict(LOG_ENTRY_FORMATTERS)
 
-
 RECEIPT_FORMATTERS = {
     "blockHash": apply_formatter_if(is_not_null, to_hexbytes(32)),
     "blockNumber": apply_formatter_if(is_not_null, to_integer_if_hex),
     "transactionIndex": apply_formatter_if(is_not_null, to_integer_if_hex),
     "transactionHash": to_hexbytes(32),
     "cumulativeGasUsed": to_integer_if_hex,
     "status": to_integer_if_hex,
@@ -260,20 +257,19 @@
     "logsBloom": to_hexbytes(256, variable_length=True),
     "from": apply_formatter_if(is_not_null, to_checksum_address),
     "to": apply_formatter_if(is_address, to_checksum_address),
     "effectiveGasPrice": to_integer_if_hex,
     "type": to_integer_if_hex,
 }
 
-
 receipt_formatter = type_aware_apply_formatters_to_dict(RECEIPT_FORMATTERS)
 
 BLOCK_FORMATTERS = {
     "baseFeePerGas": to_integer_if_hex,
-    "extraData": apply_formatter_if(is_not_null, to_hexbytes(32, variable_length=True)),
+    "extraData": apply_formatter_if(is_not_null, to_hexbytes(97)),
     "gasLimit": to_integer_if_hex,
     "gasUsed": to_integer_if_hex,
     "size": to_integer_if_hex,
     "timestamp": to_integer_if_hex,
     "hash": apply_formatter_if(is_not_null, to_hexbytes(32)),
     "logsBloom": apply_formatter_if(
         is_not_null, to_hexbytes(256, variable_length=True)
@@ -301,53 +297,46 @@
     "transactionsRoot": apply_formatter_if(is_not_null, to_hexbytes(32)),
     "withdrawals": apply_formatter_if(
         is_not_null, apply_list_to_array_formatter(withdrawal_result_formatter)
     ),
     "withdrawalsRoot": apply_formatter_if(is_not_null, to_hexbytes(32)),
 }
 
-
 block_formatter = type_aware_apply_formatters_to_dict(BLOCK_FORMATTERS)
 
-
 SYNCING_FORMATTERS = {
     "startingBlock": to_integer_if_hex,
     "currentBlock": to_integer_if_hex,
     "highestBlock": to_integer_if_hex,
     "knownStates": to_integer_if_hex,
     "pulledStates": to_integer_if_hex,
 }
 
-
 syncing_formatter = type_aware_apply_formatters_to_dict(SYNCING_FORMATTERS)
 
-
 TRANSACTION_POOL_CONTENT_FORMATTERS = {
     "pending": compose(
         curried.keymap(to_ascii_if_bytes),
         curried.valmap(transaction_result_formatter),
     ),
     "queued": compose(
         curried.keymap(to_ascii_if_bytes),
         curried.valmap(transaction_result_formatter),
     ),
 }
 
-
 transaction_pool_content_formatter = type_aware_apply_formatters_to_dict(
     TRANSACTION_POOL_CONTENT_FORMATTERS
 )
 
-
 TRANSACTION_POOL_INSPECT_FORMATTERS = {
     "pending": curried.keymap(to_ascii_if_bytes),
     "queued": curried.keymap(to_ascii_if_bytes),
 }
 
-
 transaction_pool_inspect_formatter = type_aware_apply_formatters_to_dict(
     TRANSACTION_POOL_INSPECT_FORMATTERS
 )
 
 FEE_HISTORY_FORMATTERS = {
     "baseFeePerGas": apply_formatter_to_array(to_integer_if_hex),
     "gasUsedRatio": apply_formatter_if(is_not_null, apply_formatter_to_array(float)),
@@ -381,31 +370,28 @@
 proof_formatter = type_aware_apply_formatters_to_dict(ACCOUNT_PROOF_FORMATTERS)
 
 FILTER_PARAMS_FORMATTERS = {
     "fromBlock": apply_formatter_if(is_integer, integer_to_hex),
     "toBlock": apply_formatter_if(is_integer, integer_to_hex),
 }
 
-
 filter_params_formatter = type_aware_apply_formatters_to_dict(FILTER_PARAMS_FORMATTERS)
 
-
 filter_result_formatter = apply_one_of_formatters(
     (
         (is_array_of_dicts, apply_list_to_array_formatter(log_entry_formatter)),
         (is_array_of_strings, apply_list_to_array_formatter(to_hexbytes(32))),
     )
 )
 
 transaction_param_formatter = compose(
     remove_key_if("to", lambda txn: txn["to"] in {"", b"", None}),
     remove_key_if("gasPrice", lambda txn: txn["gasPrice"] in {"", b"", None}),
 )
 
-
 call_without_override: Callable[
     [Tuple[TxParams, BlockIdentifier]], Tuple[Dict[str, Any], int]
 ] = apply_formatters_to_sequence(
     [
         transaction_param_formatter,
         to_hex_if_integer,
     ]
@@ -427,15 +413,14 @@
             to_checksum_address,
             type_aware_apply_formatters_to_dict(CALL_OVERRIDE_FORMATTERS),
             val,
         ),
     ]
 )
 
-
 estimate_gas_without_block_id: Callable[[Dict[str, Any]], Dict[str, Any]]
 estimate_gas_without_block_id = apply_formatter_at_index(transaction_param_formatter, 0)
 estimate_gas_with_block_id: Callable[
     [Tuple[Dict[str, Any], Union[str, int]]], Tuple[Dict[str, Any], int]
 ]
 estimate_gas_with_block_id = apply_formatters_to_sequence(
     [
@@ -451,15 +436,14 @@
 
 signed_tx_formatter = type_aware_apply_formatters_to_dict(SIGNED_TX_FORMATTER)
 
 FILTER_PARAM_NORMALIZERS = type_aware_apply_formatters_to_dict(
     {"address": apply_formatter_if(is_string, lambda x: [x])}
 )
 
-
 BUB_WALLET_FORMATTER = {"address": to_checksum_address}
 
 bub_wallet_formatter = type_aware_apply_formatters_to_dict(BUB_WALLET_FORMATTER)
 
 BUB_WALLETS_FORMATTER = {
     "accounts": apply_list_to_array_formatter(bub_wallet_formatter),
 }
@@ -681,15 +665,14 @@
 STANDARD_NORMALIZERS = [
     abi_bytes_to_hex,
     abi_int_to_hex,
     abi_string_to_hex,
     abi_address_to_hex,
 ]
 
-
 ABI_REQUEST_FORMATTERS: Formatters = abi_request_formatters(
     STANDARD_NORMALIZERS, RPC_ABIS
 )
 
 # the first 4 bytes of keccak hash for:
 # "OffchainLookup(address,string[],bytes,bytes4,bytes)"
 OFFCHAIN_LOOKUP_FUNC_SELECTOR = "0x556f1830"
@@ -735,16 +718,16 @@
                 revert_reason = bytes.fromhex(receipt).decode("utf-8")
                 raise ContractLogicError(
                     f"execution reverted: {revert_reason}", data=data
                 )
             else:
                 raise ContractLogicError("execution reverted", data=data)
 
-        reason_length = int(data[len(prefix) : len(prefix) + 64], 16)
-        reason = data[len(prefix) + 64 : len(prefix) + 64 + reason_length * 2]
+        reason_length = int(data[len(prefix): len(prefix) + 64], 16)
+        reason = data[len(prefix) + 64: len(prefix) + 64 + reason_length * 2]
         raise ContractLogicError(
             f'execution reverted: {bytes.fromhex(reason).decode("utf8")}',
             data=data,
         )
 
     # --- EIP-3668 | CCIP Read --- #
     # 0x556f1830 is the function selector for:
@@ -784,24 +767,24 @@
     RPC.bub_estimateGas: raise_contract_logic_error_on_revert,
     RPC.bub_call: raise_contract_logic_error_on_revert,
 }
 
 
 @to_tuple
 def combine_formatters(
-    formatter_maps: Collection[Dict[RPCEndpoint, Callable[..., TReturn]]],
-    method_name: RPCEndpoint,
+        formatter_maps: Collection[Dict[RPCEndpoint, Callable[..., TReturn]]],
+        method_name: RPCEndpoint,
 ) -> Iterable[Callable[..., TReturn]]:
     for formatter_map in formatter_maps:
         if method_name in formatter_map:
             yield formatter_map[method_name]
 
 
 def get_request_formatters(
-    method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]]
+        method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]]
 ) -> Dict[str, Callable[..., Any]]:
     request_formatter_maps = (
         ABI_REQUEST_FORMATTERS,
         # METHOD_NORMALIZERS needs to be after ABI_REQUEST_FORMATTERS
         # so that bub_getLogs's apply_formatter_at_index formatter
         # is applied to the whole address
         # rather than on the first byte of the address
@@ -819,15 +802,15 @@
     except IndexError:
         message = "Unknown block identifier"
 
     raise BlockNotFound(message)
 
 
 def raise_block_not_found_for_uncle_at_index(
-    params: Tuple[BlockIdentifier, Union[HexStr, int]]
+        params: Tuple[BlockIdentifier, Union[HexStr, int]]
 ) -> NoReturn:
     try:
         block_identifier = params[0]
         uncle_index = to_integer_if_hex(params[1])
         message = (
             f"Uncle at index: {uncle_index} of block with id: "
             f"{block_identifier!r} not found."
@@ -845,15 +828,15 @@
     except IndexError:
         message = "Unknown transaction hash"
 
     raise TransactionNotFound(message)
 
 
 def raise_transaction_not_found_with_index(
-    params: Tuple[BlockIdentifier, int]
+        params: Tuple[BlockIdentifier, int]
 ) -> NoReturn:
     try:
         block_identifier = params[0]
         transaction_index = to_integer_if_hex(params[1])
         message = (
             f"Transaction index: {transaction_index} "
             f"on block id: {block_identifier!r} not found."
@@ -876,17 +859,17 @@
     RPC.bub_getRawTransactionByBlockHashAndIndex: raise_transaction_not_found_with_index,  # noqa: E501
     RPC.bub_getRawTransactionByBlockNumberAndIndex: raise_transaction_not_found_with_index,  # noqa: E501
     RPC.bub_getRawTransactionByHash: raise_transaction_not_found,
 }
 
 
 def filter_wrapper(
-    module: Union["AsyncBub", "Bub"],
-    method: RPCEndpoint,
-    filter_id: HexStr,
+        module: Union["AsyncBub", "Bub"],
+        method: RPCEndpoint,
+        filter_id: HexStr,
 ) -> Union[
     AsyncBlockFilter,
     AsyncTransactionFilter,
     AsyncLogFilter,
     BlockFilter,
     TransactionFilter,
     LogFilter,
@@ -921,45 +904,45 @@
     RPC.bub_newBlockFilter: filter_wrapper,
     RPC.bub_newFilter: filter_wrapper,
 }
 
 
 @to_tuple
 def apply_module_to_formatters(
-    formatters: Tuple[Callable[..., TReturn]],
-    module: "Module",
-    method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]],
+        formatters: Tuple[Callable[..., TReturn]],
+        module: "Module",
+        method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]],
 ) -> Iterable[Callable[..., TReturn]]:
     for f in formatters:
         yield partial(f, module, method_name)
 
 
 def get_result_formatters(
-    method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]],
-    module: "Module",
+        method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]],
+        module: "Module",
 ) -> Dict[str, Callable[..., Any]]:
     formatters = combine_formatters((PYTHONIC_RESULT_FORMATTERS,), method_name)
     formatters_requiring_module = combine_formatters(
         (FILTER_RESULT_FORMATTERS,), method_name
     )
     partial_formatters = apply_module_to_formatters(
         formatters_requiring_module, module, method_name
     )
     return compose(*partial_formatters, *formatters)
 
 
 def get_error_formatters(
-    method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]]
+        method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]]
 ) -> Callable[..., Any]:
     #  Note error formatters work on the full response dict
     error_formatter_maps = (ERROR_FORMATTERS,)
     formatters = combine_formatters(error_formatter_maps, method_name)
 
     return compose(*formatters)
 
 
 def get_null_result_formatters(
-    method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]]
+        method_name: Union[RPCEndpoint, Callable[..., RPCEndpoint]]
 ) -> Callable[..., Any]:
     formatters = combine_formatters((NULL_RESULT_FORMATTERS,), method_name)
 
     return compose(*formatters)
```

### Comparing `bubble-sdk-0.1.6/bubble/_utils/module.py` & `bubble-sdk-0.1.7/bubble/_utils/module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/module_testing/__init__.py` & `bubble-sdk-0.1.7/bubble/_utils/module_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/module_testing/eth_module.py` & `bubble-sdk-0.1.7/bubble/_utils/module_testing/eth_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_admin_module.py` & `bubble-sdk-0.1.7/bubble/_utils/module_testing/go_ethereum_admin_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_personal_module.py` & `bubble-sdk-0.1.7/bubble/_utils/module_testing/go_ethereum_personal_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_txpool_module.py` & `bubble-sdk-0.1.7/bubble/_utils/module_testing/go_ethereum_txpool_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/module_testing/module_testing_utils.py` & `bubble-sdk-0.1.7/bubble/_utils/module_testing/module_testing_utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/module_testing/net_module.py` & `bubble-sdk-0.1.7/bubble/_utils/module_testing/net_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/module_testing/web3_module.py` & `bubble-sdk-0.1.7/bubble/_utils/module_testing/web3_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/normalizers.py` & `bubble-sdk-0.1.7/bubble/_utils/normalizers.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/request.py` & `bubble-sdk-0.1.7/bubble/_utils/request.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/rpc_abi.py` & `bubble-sdk-0.1.7/bubble/_utils/rpc_abi.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     admin_datadir = RPCEndpoint("admin_datadir")
     admin_nodeInfo = RPCEndpoint("admin_nodeInfo")
     admin_peers = RPCEndpoint("admin_peers")
     admin_startHTTP = RPCEndpoint("admin_startHTTP")
     admin_startWS = RPCEndpoint("admin_startWS")
     admin_stopHTTP = RPCEndpoint("admin_stopHTTP")
     admin_stopWS = RPCEndpoint("admin_stopWS")
+    admin_getProgramVersion = RPCEndpoint("admin_getProgramVersion")
+    admin_getSchnorrNIZKProve = RPCEndpoint("admin_getSchnorrNIZKProve")
     # deprecated
     admin_startRPC = RPCEndpoint("admin_startRPC")
     admin_stopRPC = RPCEndpoint("admin_stopRPC")
 
     # bub
     bub_accounts = RPCEndpoint("bub_accounts")
     bub_blockNumber = RPCEndpoint("bub_blockNumber")
```

### Comparing `bubble-sdk-0.1.6/bubble/_utils/threads.py` & `bubble-sdk-0.1.7/bubble/_utils/threads.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/transactions.py` & `bubble-sdk-0.1.7/bubble/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/type_conversion.py` & `bubble-sdk-0.1.7/bubble/_utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/utility_methods.py` & `bubble-sdk-0.1.7/bubble/_utils/utility_methods.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/validation.py` & `bubble-sdk-0.1.7/bubble/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/_utils/windows.py` & `bubble-sdk-0.1.7/bubble/_utils/windows.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/beacon/api_endpoints.py` & `bubble-sdk-0.1.7/bubble/beacon/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/beacon/async_beacon.py` & `bubble-sdk-0.1.7/bubble/beacon/async_beacon.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/beacon/main.py` & `bubble-sdk-0.1.7/bubble/beacon/main.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/bub/async_bub.py` & `bubble-sdk-0.1.7/bubble/bub/async_bub.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/bub/base_bub.py` & `bubble-sdk-0.1.7/bubble/bub/base_bub.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/bub/bub.py` & `bubble-sdk-0.1.7/bubble/bub/bub.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/contract/async_contract.py` & `bubble-sdk-0.1.7/bubble/contract/async_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/contract/base_contract.py` & `bubble-sdk-0.1.7/bubble/contract/base_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/contract/contract.py` & `bubble-sdk-0.1.7/bubble/contract/contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/contract/utils.py` & `bubble-sdk-0.1.7/bubble/contract/utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/datastructures.py` & `bubble-sdk-0.1.7/bubble/datastructures.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/debug.py` & `bubble-sdk-0.1.7/bubble/debug.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/exceptions.py` & `bubble-sdk-0.1.7/bubble/exceptions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/gas_strategies/time_based.py` & `bubble-sdk-0.1.7/bubble/gas_strategies/time_based.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/inner_contract/delegate.py` & `bubble-sdk-0.1.7/bubble/inner_contract/delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,14 @@
         :param staking_block_identifier: the identifier of the staking block when delegate
         """
         block = self.web3.bub.get_block(staking_block_identifier)
         return self.function(InnerFunction.delegate_getDelegateInfo,
                              block_number=block['number'],
                              address=address,
                              node_id=node_id,
-                             is_call=True,
                              )
 
     def get_delegate_lock_info(self, address: Address):
         """
         Get locked delegate information of the address.
         """
         return self.function(InnerFunction.delegate_getDelegateLockInfo, address=address)
```

### Comparing `bubble-sdk-0.1.6/bubble/inner_contract/error_code.py` & `bubble-sdk-0.1.7/bubble/inner_contract/error_code.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/inner_contract/formatters.py` & `bubble-sdk-0.1.7/bubble/inner_contract/formatters.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/inner_contract/inner_contract.py` & `bubble-sdk-0.1.7/bubble/inner_contract/inner_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/inner_contract/proposal.py` & `bubble-sdk-0.1.7/bubble/inner_contract/proposal.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,14 @@
         :param proposal_id: hash id of the proposal
         :param block_identifier: block identifier
         """
         block = self.web3.bub.get_block(block_identifier)
         return self.function(InnerFunction.proposal_getProposalVotes,
                              proposal_id=proposal_id,
                              block_hash=block['hash'],
-                             is_call=True,
                              )
 
     def get_proposal_result(self, proposal_id: Union[bytes, HexStr]):
         """
         Get proposal results, you can query only after the proposal is complete.
         use 'self.get_proposal_votes' to get current voting information.
 
@@ -200,15 +199,15 @@
         """
         Get the current value of the governable parameter
         Use 'self.govern_param_list' to get all governable parameters.
 
         :param module: the module to which the parameter belongs
         :param name: parameter name
         """
-        return self.function(InnerFunction.proposal_getGovernParam)
+        return self.function(InnerFunction.proposal_getGovernParam, module=module, name=name)
 
     def govern_param_list(self, module: str = ''):
         """
         get all governable parameters.
 
         :param module: optionally, specify a module name
         """
```

### Comparing `bubble-sdk-0.1.6/bubble/inner_contract/restricting.py` & `bubble-sdk-0.1.7/bubble/inner_contract/restricting.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/inner_contract/reward.py` & `bubble-sdk-0.1.7/bubble/inner_contract/reward.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,9 +22,8 @@
                             ):
         """
         Get the delegate reward information of the address, it can be filtered by node id.
         """
         return self.function(InnerFunction.reward_getDelegateReward,
                              address=address,
                              node_ids=[bytes.fromhex(remove_0x_prefix(node_id)) for node_id in node_ids],
-                             is_call=True,
                              )
```

### Comparing `bubble-sdk-0.1.6/bubble/inner_contract/slashing.py` & `bubble-sdk-0.1.7/bubble/inner_contract/slashing.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,9 +40,8 @@
         :param block_identifier: duplicate-signed block identifier
         """
         block = self.web3.bub.get_block(block_identifier)
         return self.function(InnerFunction.slashing_checkDuplicateSign,
                              report_type=report_type,
                              node_id=node_id,
                              block_number=block['number'],
-                             is_call=True,
                              )
```

### Comparing `bubble-sdk-0.1.6/bubble/inner_contract/staking.py` & `bubble-sdk-0.1.7/bubble/inner_contract/staking.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/main.py` & `bubble-sdk-0.1.7/bubble/main.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/manager.py` & `bubble-sdk-0.1.7/bubble/manager.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/method.py` & `bubble-sdk-0.1.7/bubble/method.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/__init__.py` & `bubble-sdk-0.1.7/bubble/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/async_cache.py` & `bubble-sdk-0.1.7/bubble/middleware/async_cache.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/attrdict.py` & `bubble-sdk-0.1.7/bubble/middleware/attrdict.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/bub_poa.py` & `bubble-sdk-0.1.7/bubble/middleware/bub_poa.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/buffered_gas_estimate.py` & `bubble-sdk-0.1.7/bubble/middleware/buffered_gas_estimate.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/cache.py` & `bubble-sdk-0.1.7/bubble/middleware/cache.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/exception_handling.py` & `bubble-sdk-0.1.7/bubble/middleware/exception_handling.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/exception_retry_request.py` & `bubble-sdk-0.1.7/bubble/middleware/exception_retry_request.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/filter.py` & `bubble-sdk-0.1.7/bubble/middleware/filter.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/fixture.py` & `bubble-sdk-0.1.7/bubble/middleware/fixture.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/formatting.py` & `bubble-sdk-0.1.7/bubble/middleware/formatting.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/gas_price_strategy.py` & `bubble-sdk-0.1.7/bubble/middleware/gas_price_strategy.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/names.py` & `bubble-sdk-0.1.7/bubble/middleware/names.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/signing.py` & `bubble-sdk-0.1.7/bubble/middleware/signing.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/simulate_unmined_transaction.py` & `bubble-sdk-0.1.7/bubble/middleware/simulate_unmined_transaction.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/stalecheck.py` & `bubble-sdk-0.1.7/bubble/middleware/stalecheck.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/middleware/validation.py` & `bubble-sdk-0.1.7/bubble/middleware/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 if TYPE_CHECKING:
     from bubble import (  # noqa: F401
         AsyncWeb3,
         Web3,
     )
 
-MAX_EXTRADATA_LENGTH = 32
+MAX_EXTRADATA_LENGTH = 97
 
 is_not_null = complement(is_null)
 to_integer_if_hex = apply_formatter_if(is_string, hex_to_integer)
 
 
 @curry
 def _validate_chain_id(web3_chain_id: int, chain_id: int) -> int:
```

### Comparing `bubble-sdk-0.1.6/bubble/module.py` & `bubble-sdk-0.1.7/bubble/module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/net.py` & `bubble-sdk-0.1.7/bubble/net.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/node.py` & `bubble-sdk-0.1.7/bubble/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,24 @@
     )
 
     stop_ws: Method[Callable[[], bool]] = Method(
         RPC.admin_stopWS,
         is_property=True,
     )
 
+    get_program_version: Method[Callable[[], str]] = Method(
+        RPC.admin_getProgramVersion,
+        mungers=None,
+    )
+
+    get_schnorr_NIZK_prove: Method[Callable[[], str]] = Method(
+        RPC.admin_getSchnorrNIZKProve,
+        mungers=None,
+    )
+
 
 class Node(Module):
     personal: NodePersonal
     admin: NodeAdmin
     txpool: NodeTxPool
```

### Comparing `bubble-sdk-0.1.6/bubble/pm.py` & `bubble-sdk-0.1.7/bubble/pm.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/async_base.py` & `bubble-sdk-0.1.7/bubble/providers/async_base.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/async_rpc.py` & `bubble-sdk-0.1.7/bubble/providers/async_rpc.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/auto.py` & `bubble-sdk-0.1.7/bubble/providers/auto.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/base.py` & `bubble-sdk-0.1.7/bubble/providers/base.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/bub_tester/defaults.py` & `bubble-sdk-0.1.7/bubble/providers/bub_tester/defaults.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/bub_tester/main.py` & `bubble-sdk-0.1.7/bubble/providers/bub_tester/main.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/bub_tester/middleware.py` & `bubble-sdk-0.1.7/bubble/providers/bub_tester/middleware.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/ipc.py` & `bubble-sdk-0.1.7/bubble/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/rpc.py` & `bubble-sdk-0.1.7/bubble/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/providers/websocket.py` & `bubble-sdk-0.1.7/bubble/providers/websocket.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/scripts/release/test_package.py` & `bubble-sdk-0.1.7/bubble/scripts/release/test_package.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/tools/benchmark/main.py` & `bubble-sdk-0.1.7/bubble/tools/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/tools/benchmark/node.py` & `bubble-sdk-0.1.7/bubble/tools/benchmark/node.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/tools/benchmark/reporting.py` & `bubble-sdk-0.1.7/bubble/tools/benchmark/reporting.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/tools/benchmark/utils.py` & `bubble-sdk-0.1.7/bubble/tools/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/tools/pytest_bubble/_utils.py` & `bubble-sdk-0.1.7/bubble/tools/pytest_bubble/_utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/tools/pytest_bubble/deployer.py` & `bubble-sdk-0.1.7/bubble/tools/pytest_bubble/deployer.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/tools/pytest_bubble/linker.py` & `bubble-sdk-0.1.7/bubble/tools/pytest_bubble/linker.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/tools/pytest_bubble/plugins.py` & `bubble-sdk-0.1.7/bubble/tools/pytest_bubble/plugins.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/tracing.py` & `bubble-sdk-0.1.7/bubble/tracing.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/types.py` & `bubble-sdk-0.1.7/bubble/types.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/utils/abi.py` & `bubble-sdk-0.1.7/bubble/utils/abi.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/utils/address.py` & `bubble-sdk-0.1.7/bubble/utils/address.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/utils/async_exception_handling.py` & `bubble-sdk-0.1.7/bubble/utils/async_exception_handling.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/utils/caching.py` & `bubble-sdk-0.1.7/bubble/utils/caching.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble/utils/exception_handling.py` & `bubble-sdk-0.1.7/bubble/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble_sdk.egg-info/PKG-INFO` & `bubble-sdk-0.1.7/bubble_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Bubble sdk
 Home-page: https://github.com/shinnng/bubble.py
 Author: Shing
 Author-email: Shinnng@outlook.com
 License: MIT
 Keywords: bubble
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bubble-sdk-0.1.6/bubble_sdk.egg-info/SOURCES.txt` & `bubble-sdk-0.1.7/bubble_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/bubble_sdk.egg-info/requires.txt` & `bubble-sdk-0.1.7/bubble_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ens/abis.py` & `bubble-sdk-0.1.7/ens/abis.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ens/async_ens.py` & `bubble-sdk-0.1.7/ens/async_ens.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ens/base_ens.py` & `bubble-sdk-0.1.7/ens/base_ens.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ens/constants.py` & `bubble-sdk-0.1.7/ens/constants.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ens/contract_data.py` & `bubble-sdk-0.1.7/ens/contract_data.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ens/ens.py` & `bubble-sdk-0.1.7/ens/ens.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ens/exceptions.py` & `bubble-sdk-0.1.7/ens/exceptions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ens/utils.py` & `bubble-sdk-0.1.7/ens/utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/__init__.py` & `bubble-sdk-0.1.7/ethpm/__init__.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/_utils/backend.py` & `bubble-sdk-0.1.7/ethpm/_utils/backend.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/_utils/cache.py` & `bubble-sdk-0.1.7/ethpm/_utils/cache.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/_utils/chains.py` & `bubble-sdk-0.1.7/ethpm/_utils/chains.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/_utils/contract.py` & `bubble-sdk-0.1.7/ethpm/_utils/contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/_utils/deployments.py` & `bubble-sdk-0.1.7/ethpm/_utils/deployments.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/_utils/ipfs.py` & `bubble-sdk-0.1.7/ethpm/_utils/ipfs.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/_utils/protobuf/ipfs_file_pb2.py` & `bubble-sdk-0.1.7/ethpm/_utils/protobuf/ipfs_file_pb2.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/_utils/registry.py` & `bubble-sdk-0.1.7/ethpm/_utils/registry.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/backends/base.py` & `bubble-sdk-0.1.7/ethpm/backends/base.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/backends/http.py` & `bubble-sdk-0.1.7/ethpm/backends/http.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/backends/ipfs.py` & `bubble-sdk-0.1.7/ethpm/backends/ipfs.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/backends/registry.py` & `bubble-sdk-0.1.7/ethpm/backends/registry.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/contract.py` & `bubble-sdk-0.1.7/ethpm/contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/dependencies.py` & `bubble-sdk-0.1.7/ethpm/dependencies.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/deployments.py` & `bubble-sdk-0.1.7/ethpm/deployments.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/exceptions.py` & `bubble-sdk-0.1.7/ethpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/package.py` & `bubble-sdk-0.1.7/ethpm/package.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/tools/builder.py` & `bubble-sdk-0.1.7/ethpm/tools/builder.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/tools/checker.py` & `bubble-sdk-0.1.7/ethpm/tools/checker.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/uri.py` & `bubble-sdk-0.1.7/ethpm/uri.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/validation/manifest.py` & `bubble-sdk-0.1.7/ethpm/validation/manifest.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/validation/misc.py` & `bubble-sdk-0.1.7/ethpm/validation/misc.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/validation/package.py` & `bubble-sdk-0.1.7/ethpm/validation/package.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/ethpm/validation/uri.py` & `bubble-sdk-0.1.7/ethpm/validation/uri.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.6/setup.py` & `bubble-sdk-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="bubble-sdk",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="0.1.6",
+    version="0.1.7",
     description="""Bubble sdk""",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Shing",
     author_email="Shinnng@outlook.com",
     url="https://github.com/shinnng/bubble.py",
     include_package_data=True,
```

