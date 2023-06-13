# Comparing `tmp/tsetmc_api-5.0.5.tar.gz` & `tmp/tsetmc_api-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsetmc_api-5.0.5.tar", max compression
+gzip compressed data, was "tsetmc_api-5.1.0.tar", max compression
```

## Comparing `tsetmc_api-5.0.5.tar` & `tsetmc_api-5.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1098 2023-05-27 16:19:22.412208 tsetmc_api-5.0.5/LICENSE.md
--rw-r--r--   0        0        0     2767 2023-05-27 16:19:22.412208 tsetmc_api-5.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/__init__.py
--rw-r--r--   0        0        0       36 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/__init__.py
--rw-r--r--   0        0        0     9279 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/_core.py
--rw-r--r--   0        0        0     5877 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/day_details.py
--rw-r--r--   0        0        0      438 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/orderbook.py
--rw-r--r--   0        0        0      460 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/price.py
--rw-r--r--   0        0        0     1842 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/shareholder.py
--rw-r--r--   0        0        0      114 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/threshold.py
--rw-r--r--   0        0        0      215 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/trade.py
--rw-r--r--   0        0        0      368 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/traders_type.py
--rw-r--r--   0        0        0       36 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/group/__init__.py
--rw-r--r--   0        0        0      481 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/group/_core.py
--rw-r--r--   0        0        0      739 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/group/group.py
--rw-r--r--   0        0        0       36 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_map/__init__.py
--rw-r--r--   0        0        0     1373 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_map/_core.py
--rw-r--r--   0        0        0     1628 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_map/map.py
--rw-r--r--   0        0        0       31 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/__init__.py
--rw-r--r--   0        0        0    17109 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/_core.py
--rw-r--r--   0        0        0      224 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/daily_history.py
--rw-r--r--   0        0        0      227 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/orderbook.py
--rw-r--r--   0        0        0      514 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/price.py
--rw-r--r--   0        0        0      321 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/traders_type.py
--rw-r--r--   0        0        0     5043 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/watch.py
--rw-r--r--   0        0        0       27 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/__init__.py
--rw-r--r--   0        0        0    12382 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/_core.py
--rw-r--r--   0        0        0      164 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/group.py
--rw-r--r--   0        0        0      366 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/identification.py
--rw-r--r--   0        0        0      219 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/notification.py
--rw-r--r--   0        0        0      247 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/orderbook.py
--rw-r--r--   0        0        0      920 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/price.py
--rw-r--r--   0        0        0     1887 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/shareholder.py
--rw-r--r--   0        0        0      221 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/state_change.py
--rw-r--r--   0        0        0      240 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/supervisor_message.py
--rw-r--r--   0        0        0     9574 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/symbol.py
--rw-r--r--   0        0        0      343 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/traders_type.py
--rw-r--r--   0        0        0      874 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/utils.py
--rw-r--r--   0        0        0      745 2023-05-27 16:19:22.456208 tsetmc_api-5.0.5/pyproject.toml
--rw-r--r--   0        0        0     3725 1970-01-01 00:00:00.000000 tsetmc_api-5.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-06-13 09:21:30.533244 tsetmc_api-5.1.0/LICENSE.md
+-rw-r--r--   0        0        0     2705 2023-06-13 09:21:30.533244 tsetmc_api-5.1.0/README.md
+-rw-r--r--   0        0        0       18 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/__init__.py
+-rw-r--r--   0        0        0     9279 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/_core.py
+-rw-r--r--   0        0        0     5877 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/day_details.py
+-rw-r--r--   0        0        0      438 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/orderbook.py
+-rw-r--r--   0        0        0      460 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/price.py
+-rw-r--r--   0        0        0     1842 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/shareholder.py
+-rw-r--r--   0        0        0      114 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/threshold.py
+-rw-r--r--   0        0        0      215 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/trade.py
+-rw-r--r--   0        0        0      368 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/traders_type.py
+-rw-r--r--   0        0        0       36 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/group/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/group/_core.py
+-rw-r--r--   0        0        0      739 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/group/group.py
+-rw-r--r--   0        0        0       36 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_map/__init__.py
+-rw-r--r--   0        0        0     1373 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_map/_core.py
+-rw-r--r--   0        0        0     1628 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_map/map.py
+-rw-r--r--   0        0        0       31 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/__init__.py
+-rw-r--r--   0        0        0    17109 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/_core.py
+-rw-r--r--   0        0        0      224 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/daily_history.py
+-rw-r--r--   0        0        0      227 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/orderbook.py
+-rw-r--r--   0        0        0      514 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/price.py
+-rw-r--r--   0        0        0      321 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/traders_type.py
+-rw-r--r--   0        0        0     5043 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/watch.py
+-rw-r--r--   0        0        0       27 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/__init__.py
+-rw-r--r--   0        0        0    12706 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/_core.py
+-rw-r--r--   0        0        0      164 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/group.py
+-rw-r--r--   0        0        0      366 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/identification.py
+-rw-r--r--   0        0        0      219 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/notification.py
+-rw-r--r--   0        0        0      247 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/orderbook.py
+-rw-r--r--   0        0        0     1004 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/price.py
+-rw-r--r--   0        0        0     1887 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/shareholder.py
+-rw-r--r--   0        0        0      221 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/state_change.py
+-rw-r--r--   0        0        0      240 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/supervisor_message.py
+-rw-r--r--   0        0        0     9693 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/symbol.py
+-rw-r--r--   0        0        0      453 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/traders_type.py
+-rw-r--r--   0        0        0      874 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/utils.py
+-rw-r--r--   0        0        0      745 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 tsetmc_api-5.1.0/PKG-INFO
```

### Comparing `tsetmc_api-5.0.5/LICENSE.md` & `tsetmc_api-5.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/README.md` & `tsetmc_api-5.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 
 ### Errors
 
 Tsetmc sometimes returns 403 and you should retry.
 
 ### TODO
 
-[ ] Migrate `symbol` component to use new tsetmc.
-[ ] Migrate `market_watch` component to use new tsetmc.
-[x] Migrate `day_details` component to use new tsetmc.
-[x] Migrate `market_map` component to use new tsetmc.
-[x] Migrate `group` component to use new tsetmc.
+- [ ] Migrate `symbol` component to use new tsetmc.
+- [ ] Migrate `market_watch` component to use new tsetmc.
+- [x] Migrate `day_details` component to use new tsetmc.
+- [x] Migrate `market_map` component to use new tsetmc.
+- [x] Migrate `group` component to use new tsetmc.
+- [ ] Support asyncio.
 
 ## Support and Donation
 
 If this repository helped you, please support it by giving a star (:star:).
-For donation please contact me at [mahdi74sadeghi@gmail.com](mailto:mahdi74sadeghi@gmail.com).
```

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/day_details/_core.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/day_details/_core.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/day_details/day_details.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/day_details/day_details.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/day_details/shareholder.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/day_details/shareholder.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/group/group.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/group/group.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/market_map/_core.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/market_map/_core.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/market_map/map.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/market_map/map.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/_core.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/_core.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/price.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/price.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/watch.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/watch.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/symbol/_core.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/symbol/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ast
 import locale
+from datetime import datetime
 
 import requests
 from bs4 import BeautifulSoup
 from jdatetime import time as jtime, date as jdate, datetime as jdatetime
 
 from ..utils import convert_deven_to_jdate
 
@@ -49,14 +50,16 @@
     response.raise_for_status()
     response = response.text
 
     all_sections = response.split(';')
 
     # price section
     data = all_sections[0].split(',')
+    gregorian_datetime = datetime.strptime(f"{data[12]}{data[0]}", '%Y%m%d%H:%M:%S')
+    jalali_datetime = jdatetime.fromgregorian(datetime=gregorian_datetime)
     price_data = {
         'last': int(data[2]),
         'close': int(data[3]),
         'open': int(data[4]),
         'yesterday': int(data[5]),
         'high': int(data[6]),
         'low': int(data[7]),
@@ -133,14 +136,15 @@
             'close': int(close),
             'count': int(count),
             'volume': int(volume),
             'value': int(value),
         })
 
     return {
+        'datetime': jalali_datetime,
         'price_data': price_data,
         'orderbook_data': orderbook,
         'traders_type_data': traders_type,
         'group_data': group_data,
     }
 
 
@@ -312,61 +316,55 @@
     }
 
     return result
 
 
 def get_symbol_traders_type_history(symbol_id: str) -> list[dict]:
     response = requests.get(
-        url='http://old.tsetmc.com/tsev2/data/clienttype.aspx',
+        url=f'http://cdn.tsetmc.com/api/ClientType/GetClientTypeHistory/{symbol_id}',
         params={
             'i': symbol_id,
         },
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
-    response = response.text
+    response = response.json()
 
     traders_type_history = []
-    raw_data = response.split(';')
+    raw_data = response['clientType']
     for row in raw_data:
-        (
-            dt,
-            r_buy_c, l_buy_c, r_sell_c, l_sell_c,
-            r_buy_v, l_buy_v, r_sell_v, l_sell_v,
-            r_buy_vl, l_buy_vl, r_sell_vl, l_sell_vl
-        ) = row.split(',')
+        gregorian_date = datetime.strptime(str(row['recDate']), '%Y%m%d').date()
         traders_type_history.append({
-            'date': jdate.fromgregorian(
-                year=int(dt[:4]),
-                month=int(dt[4:6]),
-                day=int(dt[6:]),
-            ),
+            'date': jdate.fromgregorian(date=gregorian_date),
             'legal': {
                 'buy': {
-                    'value': l_buy_vl,
-                    'volume': l_buy_v,
-                    'count': l_buy_c,
+                    'value': row['buy_N_Value'],
+                    'volume': row['buy_N_Volume'],
+                    'count': row['buy_N_Count'],
                 },
                 'sell': {
-                    'value': l_sell_vl,
-                    'volume': l_sell_v,
-                    'count': l_sell_c,
+                    'value': row['sell_N_Value'],
+                    'volume': row['sell_N_Volume'],
+                    'count': row['sell_N_Count'],
                 }
             },
             'real': {
                 'buy': {
-                    'value': r_buy_vl,
-                    'volume': r_buy_v,
-                    'count': r_buy_c,
+                    'value': row['buy_I_Value'],
+                    'volume': row['buy_I_Volume'],
+                    'count': row['buy_I_Count'],
                 },
                 'sell': {
-                    'value': r_sell_vl,
-                    'volume': r_sell_v,
-                    'count': r_sell_c,
+                    'value': row['sell_I_Value'],
+                    'volume': row['sell_I_Volume'],
+                    'count': row['sell_I_Count'],
                 }
             },
         })
 
     return traders_type_history
```

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/symbol/price.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/symbol/price.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from jdatetime import date as jdate
-from jdatetime import time as jtime
+from jdatetime import date as jdate, datetime as jdatetime, time as jtime
 from pydantic import BaseModel
 
 from .group import SymbolGroupDataRow
 from .orderbook import SymbolOrderBookData
 from .traders_type import SymbolTradersTypeDataRow
 
 
@@ -23,19 +22,23 @@
     date: jdate
 
     class Config:
         arbitrary_types_allowed = True
 
 
 class SymbolPriceOverview(BaseModel):
+    datetime: jdatetime
     price_data: SymbolPriceData
     orderbook: SymbolOrderBookData
     traders_type: SymbolTradersTypeDataRow
     group_data: list[SymbolGroupDataRow]
 
+    class Config:
+        arbitrary_types_allowed = True
+
 
 class SymbolIntraDayPriceChartDataRow(BaseModel):
     time: jtime
     high: int
     low: int
     open: int
     close: int
```

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/symbol/shareholder.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/symbol/shareholder.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/symbol/symbol.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/symbol/symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         ) for row in raw_data['orderbook_data']['buy_rows']]
         orderbook = SymbolOrderBookData(
             sell_rows=sell_rows,
             buy_rows=buy_rows,
         )
 
         traders_type = SymbolTradersTypeDataRow(
+            date=raw_data['datetime'].date(),
             legal=SymbolTradersTypeInfo(
                 buy=SymbolTradersTypeSubInfo(
                     count=raw_data['traders_type_data']['legal']['buy']['count'],
                     volume=raw_data['traders_type_data']['legal']['buy']['volume'],
                     value=raw_data['traders_type_data']['legal']['buy']['value'],
                 ),
                 sell=SymbolTradersTypeSubInfo(
@@ -81,14 +82,15 @@
             close=row['close'],
             count=row['count'],
             volume=row['volume'],
             value=row['value'],
         ) for row in raw_data['group_data']]
 
         return SymbolPriceOverview(
+            datetime=raw_data['datetime'],
             price_data=tick,
             orderbook=orderbook,
             traders_type=traders_type,
             group_data=group_data,
         )
 
     def get_intraday_price_chart_data(self) -> list[SymbolIntraDayPriceChartDataRow]:
@@ -208,14 +210,15 @@
         """
         returns daily traders type history (in "haghihi-hoghooghi" tab)
         """
 
         raw_data = _core.get_symbol_traders_type_history(symbol_id=self.symbol_id)
 
         traders_type_history = [SymbolTradersTypeDataRow(
+            date=row['date'],
             legal=SymbolTradersTypeInfo(
                 buy=SymbolTradersTypeSubInfo(
                     count=row['legal']['buy']['count'],
                     volume=row['legal']['buy']['volume'],
                     value=row['legal']['buy']['value'],
                 ),
                 sell=SymbolTradersTypeSubInfo(
```

### Comparing `tsetmc_api-5.0.5/lib/tsetmc_api/utils.py` & `tsetmc_api-5.1.0/lib/tsetmc_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.5/pyproject.toml` & `tsetmc_api-5.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsetmc-api"
-version = "5.0.5"
+version = "5.1.0"
 description = "simple package to communicate and crawl data from tsetmc.com (Tehran Stock Exchange Website)"
 license = "MIT"
 repository = "https://github.com/mahs4d/tsetmc-api"
 authors = ["Mahdi Sadeghi <mahdi74sadeghi@gmail.com>"]
 packages = [
     { include = "tsetmc_api", from = "lib" },
 ]
```

### Comparing `tsetmc_api-5.0.5/PKG-INFO` & `tsetmc_api-5.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsetmc-api
-Version: 5.0.5
+Version: 5.1.0
 Summary: simple package to communicate and crawl data from tsetmc.com (Tehran Stock Exchange Website)
 Home-page: https://github.com/mahs4d/tsetmc-api
 License: MIT
 Keywords: tsetmc,stocks,tehran stock exchange
 Author: Mahdi Sadeghi
 Author-email: mahdi74sadeghi@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -76,18 +76,18 @@
 
 ### Errors
 
 Tsetmc sometimes returns 403 and you should retry.
 
 ### TODO
 
-[ ] Migrate `symbol` component to use new tsetmc.
-[ ] Migrate `market_watch` component to use new tsetmc.
-[x] Migrate `day_details` component to use new tsetmc.
-[x] Migrate `market_map` component to use new tsetmc.
-[x] Migrate `group` component to use new tsetmc.
+- [ ] Migrate `symbol` component to use new tsetmc.
+- [ ] Migrate `market_watch` component to use new tsetmc.
+- [x] Migrate `day_details` component to use new tsetmc.
+- [x] Migrate `market_map` component to use new tsetmc.
+- [x] Migrate `group` component to use new tsetmc.
+- [ ] Support asyncio.
 
 ## Support and Donation
 
 If this repository helped you, please support it by giving a star (:star:).
-For donation please contact me at [mahdi74sadeghi@gmail.com](mailto:mahdi74sadeghi@gmail.com).
```

