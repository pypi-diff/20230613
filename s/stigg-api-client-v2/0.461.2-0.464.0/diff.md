# Comparing `tmp/stigg_api_client_v2-0.461.2.tar.gz` & `tmp/stigg_api_client_v2-0.464.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.461.2.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.464.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.461.2.tar` & `stigg_api_client_v2-0.464.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0     1644 2023-06-11 15:33:37.053950 stigg_api_client_v2-0.461.2/README.md
--rw-r--r--   0        0        0      653 2023-06-11 15:34:17.538161 stigg_api_client_v2-0.461.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-11 15:33:37.053950 stigg_api_client_v2-0.461.2/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-11 15:33:37.053950 stigg_api_client_v2-0.461.2/stigg/client.py
--rw-r--r--   0        0        0    39294 2023-06-11 15:34:15.654152 stigg_api_client_v2-0.461.2/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-11 15:34:15.282150 stigg_api_client_v2-0.461.2/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-11 15:34:15.282150 stigg_api_client_v2-0.461.2/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-11 15:34:14.286145 stigg_api_client_v2-0.461.2/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-11 15:34:14.306146 stigg_api_client_v2-0.461.2/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    68793 2023-06-11 15:34:15.502151 stigg_api_client_v2-0.461.2/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-11 15:34:14.322146 stigg_api_client_v2-0.461.2/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-11 15:34:14.418146 stigg_api_client_v2-0.461.2/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23730 2023-06-11 15:34:11.802134 stigg_api_client_v2-0.461.2/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-11 15:34:14.294145 stigg_api_client_v2-0.461.2/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-11 15:34:14.302145 stigg_api_client_v2-0.461.2/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-11 15:34:15.282150 stigg_api_client_v2-0.461.2/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53088 2023-06-11 15:34:15.282150 stigg_api_client_v2-0.461.2/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-11 15:34:14.354146 stigg_api_client_v2-0.461.2/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-11 15:34:14.362146 stigg_api_client_v2-0.461.2/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-11 15:34:14.346146 stigg_api_client_v2-0.461.2/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-11 15:34:14.402146 stigg_api_client_v2-0.461.2/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-11 15:34:14.378146 stigg_api_client_v2-0.461.2/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-11 15:34:14.374146 stigg_api_client_v2-0.461.2/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-11 15:34:14.410146 stigg_api_client_v2-0.461.2/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-11 15:34:14.366146 stigg_api_client_v2-0.461.2/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-11 15:34:14.386146 stigg_api_client_v2-0.461.2/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-11 15:34:14.394146 stigg_api_client_v2-0.461.2/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-11 15:34:14.254145 stigg_api_client_v2-0.461.2/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-11 15:34:14.250145 stigg_api_client_v2-0.461.2/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-11 15:34:14.274145 stigg_api_client_v2-0.461.2/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   125303 2023-06-11 15:34:14.230145 stigg_api_client_v2-0.461.2/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-11 15:34:14.338146 stigg_api_client_v2-0.461.2/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-11 15:34:14.242145 stigg_api_client_v2-0.461.2/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-11 15:34:14.270145 stigg_api_client_v2-0.461.2/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-11 15:34:14.318146 stigg_api_client_v2-0.461.2/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      637 2023-06-11 15:34:14.314145 stigg_api_client_v2-0.461.2/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-11 15:34:15.286150 stigg_api_client_v2-0.461.2/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-11 15:34:14.258145 stigg_api_client_v2-0.461.2/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-11 15:34:14.282145 stigg_api_client_v2-0.461.2/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      451 2023-06-11 15:34:14.422146 stigg_api_client_v2-0.461.2/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.461.2/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-13 12:40:08.904076 stigg_api_client_v2-0.464.0/README.md
+-rw-r--r--   0        0        0      653 2023-06-13 12:40:52.951066 stigg_api_client_v2-0.464.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-13 12:40:08.904076 stigg_api_client_v2-0.464.0/stigg/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-13 12:40:08.904076 stigg_api_client_v2-0.464.0/stigg/client.py
+-rw-r--r--   0        0        0    39351 2023-06-13 12:40:50.982933 stigg_api_client_v2-0.464.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-13 12:40:50.550903 stigg_api_client_v2-0.464.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-13 12:40:50.554903 stigg_api_client_v2-0.464.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-13 12:40:49.542834 stigg_api_client_v2-0.464.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-13 12:40:49.562836 stigg_api_client_v2-0.464.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    69337 2023-06-13 12:40:50.802920 stigg_api_client_v2-0.464.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-13 12:40:49.590838 stigg_api_client_v2-0.464.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      541 2023-06-13 12:40:49.686844 stigg_api_client_v2-0.464.0/stigg/generated/entitlements_updated.py
+-rw-r--r--   0        0        0    23730 2023-06-13 12:40:46.902654 stigg_api_client_v2-0.464.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-13 12:40:49.550835 stigg_api_client_v2-0.464.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-13 12:40:49.558835 stigg_api_client_v2-0.464.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-13 12:40:50.554903 stigg_api_client_v2-0.464.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53088 2023-06-13 12:40:50.550903 stigg_api_client_v2-0.464.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-13 12:40:49.614839 stigg_api_client_v2-0.464.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-13 12:40:49.622840 stigg_api_client_v2-0.464.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-13 12:40:49.606839 stigg_api_client_v2-0.464.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-13 12:40:49.666843 stigg_api_client_v2-0.464.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-13 12:40:49.642841 stigg_api_client_v2-0.464.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-13 12:40:49.634841 stigg_api_client_v2-0.464.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-13 12:40:49.678844 stigg_api_client_v2-0.464.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-13 12:40:49.630840 stigg_api_client_v2-0.464.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-13 12:40:49.650842 stigg_api_client_v2-0.464.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-13 12:40:49.658842 stigg_api_client_v2-0.464.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-13 12:40:49.502832 stigg_api_client_v2-0.464.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-13 12:40:49.498831 stigg_api_client_v2-0.464.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-13 12:40:49.530833 stigg_api_client_v2-0.464.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   125303 2023-06-13 12:40:49.478830 stigg_api_client_v2-0.464.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-13 12:40:49.598838 stigg_api_client_v2-0.464.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-13 12:40:49.490831 stigg_api_client_v2-0.464.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-13 12:40:49.522833 stigg_api_client_v2-0.464.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-13 12:40:49.582837 stigg_api_client_v2-0.464.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-06-13 12:40:49.578837 stigg_api_client_v2-0.464.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-06-13 12:40:49.570836 stigg_api_client_v2-0.464.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-13 12:40:50.558904 stigg_api_client_v2-0.464.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-13 12:40:49.510832 stigg_api_client_v2-0.464.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-13 12:40:49.534834 stigg_api_client_v2-0.464.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      451 2023-06-13 12:40:49.690844 stigg_api_client_v2-0.464.0/stigg/generated/usage_updated.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.464.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.461.2/README.md` & `stigg_api_client_v2-0.464.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.461.2/pyproject.toml` & `stigg_api_client_v2-0.464.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "0.461.2"
+version = "0.464.0"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/__init__.py` & `stigg_api_client_v2-0.464.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
@@ -591,14 +591,15 @@
 )
 from .provision_subscription import (
     ProvisionSubscription,
     ProvisionSubscriptionProvisionSubscription,
     ProvisionSubscriptionProvisionSubscriptionSubscription,
 )
 from .report_entitlement_check_requested import ReportEntitlementCheckRequested
+from .report_event import ReportEvent
 from .report_usage import ReportUsage, ReportUsageCreateUsageMeasurement
 from .update_customer import UpdateCustomer, UpdateCustomerUpdateCustomer
 from .update_subscription import (
     UpdateSubscription,
     UpdateSubscriptionUpdateSubscription,
 )
 from .usage_updated import UsageUpdated, UsageUpdatedUsageUpdated
@@ -1010,14 +1011,15 @@
     "RemoveBasePlanFromPlanInput",
     "RemoveCompatibleAddonsFromPlanInput",
     "RemoveCouponFromCustomerInput",
     "RemoveCouponFromCustomerSubscriptionInput",
     "RemoveExperimentFromCustomerInput",
     "RemoveExperimentFromCustomerSubscriptionInput",
     "ReportEntitlementCheckRequested",
+    "ReportEvent",
     "ReportUsage",
     "ReportUsageCreateUsageMeasurement",
     "ReportUsageInput",
     "ResyncIntegrationInput",
     "SetBasePlanOnPlanInput",
     "SetCompatibleAddonsOnPlanInput",
     "SetCouponOnCustomerInput",
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.464.0/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/base_model.py` & `stigg_api_client_v2-0.464.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.464.0/stigg/generated/cancel_subscription.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/client.py` & `stigg_api_client_v2-0.464.0/stigg/generated/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import AsyncIterator
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
@@ -40,20 +40,22 @@
     ProvisionSubscriptionInput,
     SubscriptionCancellationInput,
     SubscriptionInput,
     SubscriptionMigrationInput,
     SubscriptionUpdateScheduleCancellationInput,
     UpdateCustomerInput,
     UpdateSubscriptionInput,
+    UsageEventsReportInput,
     UsageMeasurementCreateInput,
 )
 from .migrate_subscription_to_latest import MigrateSubscriptionToLatest
 from .provision_customer import ProvisionCustomer
 from .provision_subscription import ProvisionSubscription
 from .report_entitlement_check_requested import ReportEntitlementCheckRequested
+from .report_event import ReportEvent
 from .report_usage import ReportUsage
 from .update_customer import UpdateCustomer
 from .update_subscription import UpdateSubscription
 from .usage_updated import UsageUpdated
 
 
 def gql(q: str) -> str:
@@ -745,14 +747,27 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return ReportUsage.parse_obj(data)
 
+    async def report_event(self, input: UsageEventsReportInput) -> ReportEvent:
+        query = gql(
+            """
+            mutation ReportEvent($input: UsageEventsReportInput!) {
+              reportEvent(events: $input)
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return ReportEvent.parse_obj(data)
+
     async def report_entitlement_check_requested(
         self, entitlement_check_requested: EntitlementCheckRequested
     ) -> ReportEntitlementCheckRequested:
         query = gql(
             """
             mutation ReportEntitlementCheckRequested($entitlementCheckRequested: EntitlementCheckRequested!) {
               reportEntitlementCheckRequested(
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.464.0/stigg/generated/create_subscription.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/entitlements_updated.py` & `stigg_api_client_v2-0.464.0/stigg/generated/entitlements_updated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import EntitlementsUpdatedPayload
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/enums.py` & `stigg_api_client_v2-0.464.0/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.464.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .fragments import SubscriptionPreviewFragment
 
 
-class EstimateSubscription(BaseModel):
-    estimate_subscription: "EstimateSubscriptionEstimateSubscription" = Field(
-        alias="estimateSubscription"
+class MigrateSubscriptionToLatest(BaseModel):
+    migrate_subscription_to_latest: "MigrateSubscriptionToLatestMigrateSubscriptionToLatest" = Field(
+        alias="migrateSubscriptionToLatest"
     )
 
 
-class EstimateSubscriptionEstimateSubscription(SubscriptionPreviewFragment):
-    pass
+class MigrateSubscriptionToLatestMigrateSubscriptionToLatest(BaseModel):
+    subscription_id: str = Field(alias="subscriptionId")
 
 
-EstimateSubscription.update_forward_refs()
-EstimateSubscriptionEstimateSubscription.update_forward_refs()
+MigrateSubscriptionToLatest.update_forward_refs()
+MigrateSubscriptionToLatestMigrateSubscriptionToLatest.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.464.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.464.0/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/fragments.py` & `stigg_api_client_v2-0.464.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,14 +32,36 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -55,36 +77,14 @@
 class PriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -328,21 +328,16 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -471,16 +466,21 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
 
 
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
@@ -517,14 +517,29 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
+
+
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
 class SubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
@@ -568,29 +583,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
-
-
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -1268,19 +1268,19 @@
 
 
 class SubscriptionPreviewFragmentProrationNetAmount(BaseModel):
     amount: float
     currency: Currency
 
 
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
 SlimCustomerFragment.update_forward_refs()
@@ -1303,15 +1303,15 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
@@ -1321,30 +1321,30 @@
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.464.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.464.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.464.0/stigg/generated/get_customer_by_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.464.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.464.0/stigg/generated/get_mock_paywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/get_products.py` & `stigg_api_client_v2-0.464.0/stigg/generated/get_products.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.464.0/stigg/generated/get_sdk_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/input_types.py` & `stigg_api_client_v2-0.464.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.464.0/stigg/generated/update_subscription.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
+from .fragments import SlimSubscriptionFragment
 
 
-class MigrateSubscriptionToLatest(BaseModel):
-    migrate_subscription_to_latest: "MigrateSubscriptionToLatestMigrateSubscriptionToLatest" = Field(
-        alias="migrateSubscriptionToLatest"
+class UpdateSubscription(BaseModel):
+    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
+        alias="updateSubscription"
     )
 
 
-class MigrateSubscriptionToLatestMigrateSubscriptionToLatest(BaseModel):
-    subscription_id: str = Field(alias="subscriptionId")
+class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
+    pass
 
 
-MigrateSubscriptionToLatest.update_forward_refs()
-MigrateSubscriptionToLatestMigrateSubscriptionToLatest.update_forward_refs()
+UpdateSubscription.update_forward_refs()
+UpdateSubscriptionUpdateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.464.0/stigg/generated/provision_customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.464.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.461.2/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.464.0/stigg/generated/report_usage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 15:34
+# Generated by ariadne-codegen on 2023-06-13 12:40
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.461.2/PKG-INFO` & `stigg_api_client_v2-0.464.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.461.2
+Version: 0.464.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

