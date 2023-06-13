# Comparing `tmp/mollie-api-python-3.2.0.tar.gz` & `tmp/mollie-api-python-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mollie-api-python-3.2.0.tar", last modified: Tue Apr 11 07:15:20 2023, max compression
+gzip compressed data, was "mollie-api-python-3.3.0.tar", last modified: Tue Jun 13 07:15:24 2023, max compression
```

## Comparing `mollie-api-python-3.2.0.tar` & `mollie-api-python-3.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.305022 mollie-api-python-3.2.0/mollie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.305022 mollie-api-python-3.2.0/mollie/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.309022 mollie-api-python-3.2.0/mollie/api/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/balance_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/chargeback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/issuer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/order_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/refund.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/settlement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/shipment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/mollie/api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/balances.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/captures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/chargebacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/customers.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/invoices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/mandates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/order_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/payment_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/refunds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/settlements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/shipments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/mollie_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:23.995721 mollie-api-python-3.3.0/mollie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:23.999721 mollie-api-python-3.3.0/mollie/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:24.003722 mollie-api-python-3.3.0/mollie/api/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/balance_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/chargeback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/issuer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/order_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/settlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/mollie/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/captures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/chargebacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/mandates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/order_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/payment_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/settlements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/mollie_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/setup.py
```

### Comparing `mollie-api-python-3.2.0/LICENSE.txt` & `mollie-api-python-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/PKG-INFO` & `mollie-api-python-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mollie-api-python
-Version: 3.2.0
+Version: 3.3.0
 Summary: Mollie API client for Python
 Home-page: https://github.com/mollie/mollie-api-python
 Author: Mollie B.V.
 Author-email: info@mollie.com
 Maintainer: Four Digits B.V.
 Maintainer-email: info@fourdigits.nl
 License: BSD
@@ -21,18 +21,18 @@
 <p align="center">
   <img src="https://info.mollie.com/hubfs/github/python/logo.png" width="128" height="128"/>
 </p>
 <h1 align="center">Mollie API client for Python</h1>
 
 <img src="https://info.mollie.com/hubfs/github/python/editor-1.png" />
 
-Accepting [iDEAL](https://www.mollie.com/en/payments/ideal/), [Bancontact/Mister Cash](https://www.mollie.com/en/payments/bancontact/), [SOFORT Banking](https://www.mollie.com/en/payments/sofort/), [Creditcard](https://www.mollie.com/en/payments/credit-card/), [SEPA Bank transfer](https://www.mollie.com/en/payments/bank-transfer/), [SEPA Direct debit](https://www.mollie.com/en/payments/direct-debit/), [PayPal](https://www.mollie.com/en/payments/paypal/), [Belfius Direct Net](https://www.mollie.com/en/payments/belfius/), [KBC/CBC](https://www.mollie.com/en/payments/kbc-cbc/), Klarna [Pay later](https://www.mollie.com/en/payments/klarna-pay-later/)/[Pay now](https://www.mollie.com/en/payments/klarna-pay-now/)/[Slice it](https://www.mollie.com/en/payments/klarna-slice-it/), [paysafecard](https://www.mollie.com/en/payments/paysafecard/), [Giftcards](https://www.mollie.com/en/payments/gift-cards/), [Giropay](https://www.mollie.com/en/payments/giropay/), [EPS](https://www.mollie.com/en/payments/eps/) and [Przelewy24](https://www.mollie.com/en/payments/przelewy24) online payments without fixed monthly costs or any punishing registration procedures. Just use the Mollie API to receive payments directly on your website or easily refund transactions to your customers.
+Accepting [iDEAL](https://www.mollie.com/en/payments/ideal/), [Bancontact/Mister Cash](https://www.mollie.com/en/payments/bancontact/), [SOFORT Banking](https://www.mollie.com/en/payments/sofort/), [Creditcard](https://www.mollie.com/en/payments/credit-card/), [SEPA Bank transfer](https://www.mollie.com/en/payments/bank-transfer/), [SEPA Direct debit](https://www.mollie.com/en/payments/direct-debit/), [PayPal](https://www.mollie.com/en/payments/paypal/), [Belfius Direct Net](https://www.mollie.com/en/payments/belfius/), [KBC/CBC](https://www.mollie.com/en/payments/kbc-cbc/), Klarna [Pay later](https://www.mollie.com/en/payments/klarna-pay-later/)/[Pay now](https://www.mollie.com/en/payments/klarna-pay-now/)/[Slice it](https://www.mollie.com/en/payments/klarna-slice-it/), [paysafecard](https://www.mollie.com/en/payments/paysafecard/), [Giftcards](https://www.mollie.com/en/payments/gift-cards/), [Giropay](https://www.mollie.com/en/payments/giropay/), [EPS](https://www.mollie.com/en/payments/eps/), [Przelewy24](https://www.mollie.com/en/payments/przelewy24) and [Billie](https://www.mollie.com/en/payments/billie) online payments without fixed monthly costs or any punishing registration procedures. Just use the Mollie API to receive payments directly on your website or easily refund transactions to your customers.
 
 [![PyPI version](https://badge.fury.io/py/mollie-api-python.svg)](http://badge.fury.io/py/mollie-api-python)
-[![Build Status](https://travis-ci.org/mollie/mollie-api-python.svg?branch=master)](https://travis-ci.org/mollie/mollie-api-python)
+![Tests](https://github.com/mollie/mollie-api-python/actions/workflows/tests.yaml/badge.svg)
 
 ## Requirements ##
 To use the Mollie API client, the following things are required:
 
 + Get yourself a free [Mollie account](https://www.mollie.com/signup). No sign up costs.
 + Create a new [Website profile](https://www.mollie.com/dashboard/settings/profiles) to generate API keys and setup your webhook.
 + Now you're ready to use the Mollie API client in test mode.
```

### Comparing `mollie-api-python-3.2.0/README.md` & `mollie-api-python-3.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <p align="center">
   <img src="https://info.mollie.com/hubfs/github/python/logo.png" width="128" height="128"/>
 </p>
 <h1 align="center">Mollie API client for Python</h1>
 
 <img src="https://info.mollie.com/hubfs/github/python/editor-1.png" />
 
-Accepting [iDEAL](https://www.mollie.com/en/payments/ideal/), [Bancontact/Mister Cash](https://www.mollie.com/en/payments/bancontact/), [SOFORT Banking](https://www.mollie.com/en/payments/sofort/), [Creditcard](https://www.mollie.com/en/payments/credit-card/), [SEPA Bank transfer](https://www.mollie.com/en/payments/bank-transfer/), [SEPA Direct debit](https://www.mollie.com/en/payments/direct-debit/), [PayPal](https://www.mollie.com/en/payments/paypal/), [Belfius Direct Net](https://www.mollie.com/en/payments/belfius/), [KBC/CBC](https://www.mollie.com/en/payments/kbc-cbc/), Klarna [Pay later](https://www.mollie.com/en/payments/klarna-pay-later/)/[Pay now](https://www.mollie.com/en/payments/klarna-pay-now/)/[Slice it](https://www.mollie.com/en/payments/klarna-slice-it/), [paysafecard](https://www.mollie.com/en/payments/paysafecard/), [Giftcards](https://www.mollie.com/en/payments/gift-cards/), [Giropay](https://www.mollie.com/en/payments/giropay/), [EPS](https://www.mollie.com/en/payments/eps/) and [Przelewy24](https://www.mollie.com/en/payments/przelewy24) online payments without fixed monthly costs or any punishing registration procedures. Just use the Mollie API to receive payments directly on your website or easily refund transactions to your customers.
+Accepting [iDEAL](https://www.mollie.com/en/payments/ideal/), [Bancontact/Mister Cash](https://www.mollie.com/en/payments/bancontact/), [SOFORT Banking](https://www.mollie.com/en/payments/sofort/), [Creditcard](https://www.mollie.com/en/payments/credit-card/), [SEPA Bank transfer](https://www.mollie.com/en/payments/bank-transfer/), [SEPA Direct debit](https://www.mollie.com/en/payments/direct-debit/), [PayPal](https://www.mollie.com/en/payments/paypal/), [Belfius Direct Net](https://www.mollie.com/en/payments/belfius/), [KBC/CBC](https://www.mollie.com/en/payments/kbc-cbc/), Klarna [Pay later](https://www.mollie.com/en/payments/klarna-pay-later/)/[Pay now](https://www.mollie.com/en/payments/klarna-pay-now/)/[Slice it](https://www.mollie.com/en/payments/klarna-slice-it/), [paysafecard](https://www.mollie.com/en/payments/paysafecard/), [Giftcards](https://www.mollie.com/en/payments/gift-cards/), [Giropay](https://www.mollie.com/en/payments/giropay/), [EPS](https://www.mollie.com/en/payments/eps/), [Przelewy24](https://www.mollie.com/en/payments/przelewy24) and [Billie](https://www.mollie.com/en/payments/billie) online payments without fixed monthly costs or any punishing registration procedures. Just use the Mollie API to receive payments directly on your website or easily refund transactions to your customers.
 
 [![PyPI version](https://badge.fury.io/py/mollie-api-python.svg)](http://badge.fury.io/py/mollie-api-python)
-[![Build Status](https://travis-ci.org/mollie/mollie-api-python.svg?branch=master)](https://travis-ci.org/mollie/mollie-api-python)
+![Tests](https://github.com/mollie/mollie-api-python/actions/workflows/tests.yaml/badge.svg)
 
 ## Requirements ##
 To use the Mollie API client, the following things are required:
 
 + Get yourself a free [Mollie account](https://www.mollie.com/signup). No sign up costs.
 + Create a new [Website profile](https://www.mollie.com/dashboard/settings/profiles) to generate API keys and setup your webhook.
 + Now you're ready to use the Mollie API client in test mode.
```

### Comparing `mollie-api-python-3.2.0/mollie/api/client.py` & `mollie-api-python-3.3.0/mollie/api/client.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/error.py` & `mollie-api-python-3.3.0/mollie/api/error.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,34 +74,51 @@
             return ConflictError(resp, idempotency_key=idempotency_key)
         elif status == 422:
             return UnprocessableEntityError(resp, idempotency_key=idempotency_key)
         else:
             # generic fallback
             return ResponseError(resp, idempotency_key=idempotency_key)
 
+    def __reduce__(self):
+        """
+        Customize the pickling routine.
+
+        Exceptions have a custom __reduce__() routine, but that doesn't work
+        since we override the __init__ method here.
+        """
+
+        callable_ = self.__class__
+        args = (
+            {
+                "detail": self.args[0],
+                "status": self.status,
+                "field": self.field,
+            },
+            self.idempotency_key,
+        )
+        return (callable_, args)
+
 
 class UnauthorizedError(ResponseError):
     """Your request wasn't executed due to failed authentication. Check your API key."""
 
     pass
 
 
 class NotFoundError(ResponseError):
     """The object referenced by your API request does not exist."""
 
     pass
 
 
 class BadRequestError(ResponseError):
-
     pass
 
 
 class ConflictError(ResponseError):
-
     pass
 
 
 class UnprocessableEntityError(ResponseError):
     """We could not process your request due to another reason than the ones listed above.
 
     The response usually contains a field property to indicate which field is causing the issue.
```

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/balance.py` & `mollie-api-python-3.3.0/mollie/api/objects/balance.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/balance_report.py` & `mollie-api-python-3.3.0/mollie/api/objects/balance_report.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/balance_transaction.py` & `mollie-api-python-3.3.0/mollie/api/objects/balance_transaction.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/base.py` & `mollie-api-python-3.3.0/mollie/api/objects/base.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/capture.py` & `mollie-api-python-3.3.0/mollie/api/objects/capture.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/chargeback.py` & `mollie-api-python-3.3.0/mollie/api/objects/chargeback.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/client.py` & `mollie-api-python-3.3.0/mollie/api/objects/client.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/customer.py` & `mollie-api-python-3.3.0/mollie/api/objects/customer.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/invoice.py` & `mollie-api-python-3.3.0/mollie/api/objects/invoice.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/issuer.py` & `mollie-api-python-3.3.0/mollie/api/objects/issuer.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/list.py` & `mollie-api-python-3.3.0/mollie/api/objects/list.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/mandate.py` & `mollie-api-python-3.3.0/mollie/api/objects/mandate.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/method.py` & `mollie-api-python-3.3.0/mollie/api/objects/method.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     PAYSAFECARD = "paysafecard"
     SOFORT = "sofort"
 
     # Payment methods for Payments only
     # (none)
 
     # Payment methods for Orders only
+    BILLIE = "billie"
     IN3 = "in3"
     KLARNAPAYLATER = "klarnapaylater"
     KLARNAPAYNOW = "klarnapaynow"
     KLARNASLICEIT = "klarnasliceit"
     VOUCHER = "voucher"
 
     @property
```

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/onboarding.py` & `mollie-api-python-3.3.0/mollie/api/objects/onboarding.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/order.py` & `mollie-api-python-3.3.0/mollie/api/objects/order.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/order_line.py` & `mollie-api-python-3.3.0/mollie/api/objects/order_line.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/organization.py` & `mollie-api-python-3.3.0/mollie/api/objects/organization.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/payment.py` & `mollie-api-python-3.3.0/mollie/api/objects/payment.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/payment_link.py` & `mollie-api-python-3.3.0/mollie/api/objects/payment_link.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/permission.py` & `mollie-api-python-3.3.0/mollie/api/objects/permission.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/profile.py` & `mollie-api-python-3.3.0/mollie/api/objects/profile.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/refund.py` & `mollie-api-python-3.3.0/mollie/api/objects/refund.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/settlement.py` & `mollie-api-python-3.3.0/mollie/api/objects/settlement.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/shipment.py` & `mollie-api-python-3.3.0/mollie/api/objects/shipment.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/objects/subscription.py` & `mollie-api-python-3.3.0/mollie/api/objects/subscription.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/__init__.py` & `mollie-api-python-3.3.0/mollie/api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/balances.py` & `mollie-api-python-3.3.0/mollie/api/resources/balances.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/base.py` & `mollie-api-python-3.3.0/mollie/api/resources/base.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/captures.py` & `mollie-api-python-3.3.0/mollie/api/resources/captures.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/chargebacks.py` & `mollie-api-python-3.3.0/mollie/api/resources/chargebacks.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/clients.py` & `mollie-api-python-3.3.0/mollie/api/resources/clients.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/customers.py` & `mollie-api-python-3.3.0/mollie/api/resources/customers.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/invoices.py` & `mollie-api-python-3.3.0/mollie/api/resources/invoices.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/mandates.py` & `mollie-api-python-3.3.0/mollie/api/resources/mandates.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/methods.py` & `mollie-api-python-3.3.0/mollie/api/resources/methods.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/onboarding.py` & `mollie-api-python-3.3.0/mollie/api/resources/onboarding.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import warnings
 from typing import Any, Dict
 
-from ..error import IdentifierError
+from ..error import APIDeprecationWarning, IdentifierError
 from ..objects.onboarding import Onboarding as OnboardingObject
 from .base import ResourceGetMixin
 
 __all__ = [
     "Onboarding",
 ]
 
@@ -17,11 +18,17 @@
 
     def get(self, resource_id: str, **params: Any) -> OnboardingObject:
         if resource_id != "me":
             raise IdentifierError(f"Invalid onboarding ID: '{resource_id}'. The onboarding ID should be 'me'.")
         return super().get(resource_id, **params)
 
     def create(self, data: Dict[str, Any], **params: Any) -> OnboardingObject:
+        warnings.warn(
+            "Submission of onboarding data is deprecated, see "
+            "https://docs.mollie.com/reference/v2/onboarding-api/submit-onboarding-data",
+            APIDeprecationWarning,
+        )
+
         resource_path = self.get_resource_path()
         path = f"{resource_path}/me"
         result = self.perform_api_call(self.REST_CREATE, path, data, params)
         return self.get_resource_object(result)
```

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/order_lines.py` & `mollie-api-python-3.3.0/mollie/api/resources/order_lines.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/orders.py` & `mollie-api-python-3.3.0/mollie/api/resources/orders.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/organizations.py` & `mollie-api-python-3.3.0/mollie/api/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/payment_links.py` & `mollie-api-python-3.3.0/mollie/api/resources/payment_links.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/payments.py` & `mollie-api-python-3.3.0/mollie/api/resources/payments.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/permissions.py` & `mollie-api-python-3.3.0/mollie/api/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/profiles.py` & `mollie-api-python-3.3.0/mollie/api/resources/profiles.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/refunds.py` & `mollie-api-python-3.3.0/mollie/api/resources/refunds.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/settlements.py` & `mollie-api-python-3.3.0/mollie/api/resources/settlements.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/shipments.py` & `mollie-api-python-3.3.0/mollie/api/resources/shipments.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie/api/resources/subscriptions.py` & `mollie-api-python-3.3.0/mollie/api/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/mollie_api_python.egg-info/PKG-INFO` & `mollie-api-python-3.3.0/mollie_api_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mollie-api-python
-Version: 3.2.0
+Version: 3.3.0
 Summary: Mollie API client for Python
 Home-page: https://github.com/mollie/mollie-api-python
 Author: Mollie B.V.
 Author-email: info@mollie.com
 Maintainer: Four Digits B.V.
 Maintainer-email: info@fourdigits.nl
 License: BSD
@@ -21,18 +21,18 @@
 <p align="center">
   <img src="https://info.mollie.com/hubfs/github/python/logo.png" width="128" height="128"/>
 </p>
 <h1 align="center">Mollie API client for Python</h1>
 
 <img src="https://info.mollie.com/hubfs/github/python/editor-1.png" />
 
-Accepting [iDEAL](https://www.mollie.com/en/payments/ideal/), [Bancontact/Mister Cash](https://www.mollie.com/en/payments/bancontact/), [SOFORT Banking](https://www.mollie.com/en/payments/sofort/), [Creditcard](https://www.mollie.com/en/payments/credit-card/), [SEPA Bank transfer](https://www.mollie.com/en/payments/bank-transfer/), [SEPA Direct debit](https://www.mollie.com/en/payments/direct-debit/), [PayPal](https://www.mollie.com/en/payments/paypal/), [Belfius Direct Net](https://www.mollie.com/en/payments/belfius/), [KBC/CBC](https://www.mollie.com/en/payments/kbc-cbc/), Klarna [Pay later](https://www.mollie.com/en/payments/klarna-pay-later/)/[Pay now](https://www.mollie.com/en/payments/klarna-pay-now/)/[Slice it](https://www.mollie.com/en/payments/klarna-slice-it/), [paysafecard](https://www.mollie.com/en/payments/paysafecard/), [Giftcards](https://www.mollie.com/en/payments/gift-cards/), [Giropay](https://www.mollie.com/en/payments/giropay/), [EPS](https://www.mollie.com/en/payments/eps/) and [Przelewy24](https://www.mollie.com/en/payments/przelewy24) online payments without fixed monthly costs or any punishing registration procedures. Just use the Mollie API to receive payments directly on your website or easily refund transactions to your customers.
+Accepting [iDEAL](https://www.mollie.com/en/payments/ideal/), [Bancontact/Mister Cash](https://www.mollie.com/en/payments/bancontact/), [SOFORT Banking](https://www.mollie.com/en/payments/sofort/), [Creditcard](https://www.mollie.com/en/payments/credit-card/), [SEPA Bank transfer](https://www.mollie.com/en/payments/bank-transfer/), [SEPA Direct debit](https://www.mollie.com/en/payments/direct-debit/), [PayPal](https://www.mollie.com/en/payments/paypal/), [Belfius Direct Net](https://www.mollie.com/en/payments/belfius/), [KBC/CBC](https://www.mollie.com/en/payments/kbc-cbc/), Klarna [Pay later](https://www.mollie.com/en/payments/klarna-pay-later/)/[Pay now](https://www.mollie.com/en/payments/klarna-pay-now/)/[Slice it](https://www.mollie.com/en/payments/klarna-slice-it/), [paysafecard](https://www.mollie.com/en/payments/paysafecard/), [Giftcards](https://www.mollie.com/en/payments/gift-cards/), [Giropay](https://www.mollie.com/en/payments/giropay/), [EPS](https://www.mollie.com/en/payments/eps/), [Przelewy24](https://www.mollie.com/en/payments/przelewy24) and [Billie](https://www.mollie.com/en/payments/billie) online payments without fixed monthly costs or any punishing registration procedures. Just use the Mollie API to receive payments directly on your website or easily refund transactions to your customers.
 
 [![PyPI version](https://badge.fury.io/py/mollie-api-python.svg)](http://badge.fury.io/py/mollie-api-python)
-[![Build Status](https://travis-ci.org/mollie/mollie-api-python.svg?branch=master)](https://travis-ci.org/mollie/mollie-api-python)
+![Tests](https://github.com/mollie/mollie-api-python/actions/workflows/tests.yaml/badge.svg)
 
 ## Requirements ##
 To use the Mollie API client, the following things are required:
 
 + Get yourself a free [Mollie account](https://www.mollie.com/signup). No sign up costs.
 + Create a new [Website profile](https://www.mollie.com/dashboard/settings/profiles) to generate API keys and setup your webhook.
 + Now you're ready to use the Mollie API client in test mode.
```

### Comparing `mollie-api-python-3.2.0/mollie_api_python.egg-info/SOURCES.txt` & `mollie-api-python-3.3.0/mollie_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.2.0/setup.py` & `mollie-api-python-3.3.0/setup.py`

 * *Files identical despite different names*

