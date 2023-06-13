# Comparing `tmp/vcsc_data_common-0.1.8.tar.gz` & `tmp/vcsc_data_common-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.1.8.tar", last modified: Mon May 15 03:19:38 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.2.1.tar", last modified: Tue Jun 13 08:26:36 2023, max compression
```

## Comparing `vcsc_data_common-0.1.8.tar` & `vcsc_data_common-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.822515 vcsc_data_common-0.1.8/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-15 03:19:38.822623 vcsc_data_common-0.1.8/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.8/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.8/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-05-15 03:19:38.822986 vcsc_data_common-0.1.8/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.812908 vcsc_data_common-0.1.8/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.8/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.814097 vcsc_data_common-0.1.8/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.8/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.8/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.820332 vcsc_data_common-0.1.8/vcsc_data_common/backtest/
--rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.1.8/vcsc_data_common/backtest/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.820831 vcsc_data_common-0.1.8/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.1.8/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.821129 vcsc_data_common-0.1.8/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.8/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.821400 vcsc_data_common-0.1.8/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3777 2023-05-15 03:18:50.000000 vcsc_data_common-0.1.8/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.821635 vcsc_data_common-0.1.8/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     3660 2023-05-11 09:51:24.000000 vcsc_data_common-0.1.8/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.813726 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      565 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.556051 vcsc_data_common-0.2.1/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-06-13 08:26:36.556152 vcsc_data_common-0.2.1/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.2.1/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.2.1/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-06-13 08:26:36.556492 vcsc_data_common-0.2.1/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.552465 vcsc_data_common-0.2.1/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.2.1/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.553740 vcsc_data_common-0.2.1/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.2.1/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5081 2023-06-08 06:24:22.000000 vcsc_data_common-0.2.1/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.554047 vcsc_data_common-0.2.1/vcsc_data_common/backtest/
+-rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.2.1/vcsc_data_common/backtest/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.554340 vcsc_data_common-0.2.1/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.2.1/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.554685 vcsc_data_common-0.2.1/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.2.1/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.554979 vcsc_data_common-0.2.1/vcsc_data_common/oneday_portfolio/
+-rw-r--r--   0 pd         (501) staff       (20)      516 2023-05-24 09:25:19.000000 vcsc_data_common-0.2.1/vcsc_data_common/oneday_portfolio/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.555261 vcsc_data_common-0.2.1/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3875 2023-06-08 02:36:37.000000 vcsc_data_common-0.2.1/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.555542 vcsc_data_common-0.2.1/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3868 2023-06-13 08:25:14.000000 vcsc_data_common-0.2.1/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.555812 vcsc_data_common-0.2.1/vcsc_data_common/signals/
+-rw-r--r--   0 pd         (501) staff       (20)     1513 2023-06-01 10:35:44.000000 vcsc_data_common-0.2.1/vcsc_data_common/signals/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.553348 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      648 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.1.8/pyproject.toml` & `vcsc_data_common-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.8/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.2.1/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,36 +39,41 @@
             self.offline_data_fetchers.append(offline_data_fetcher)
 
             self.offline_data_dfs.append(pd.DataFrame())
             self.live_data_dfs.append(pd.DataFrame())
 
     def start(self):
         self.offline_data_df = self.fetch_all_offline_data()
-
+        
         while True:
 
             self.fetch_all_live_data()
 
             if(self.is_new_live_data):
 
                 # union all df & return
                 data_arr: list[pd.DataFrame] = []
 
                 for index in range(self.fetching_time_frame_configs.__len__()):
                     offline_data_df = self.offline_data_dfs[index]
                     live_data_df = self.live_data_dfs[index]
+
+                    if(live_data_df.empty == True):
+                        self.is_ignore_call_back = True
+
                     union_df = pd.concat([offline_data_df, live_data_df])
 
                     data_arr.append(union_df)
 
                 market_status_df = self.live_data_fetchers[0].get_market_status(
                 )
 
                 self.callback(*data_arr, market_status_df,
-                              self.live_modification_time)
+                            self.live_modification_time)
+                
 
             else:
                 logging.debug('data has no change')
 
             self.is_new_live_data = False
             time.sleep(self.interval)
```

### Comparing `vcsc_data_common-0.1.8/vcsc_data_common/backtest/__init__.py` & `vcsc_data_common-0.2.1/vcsc_data_common/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.8/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.2.1/vcsc_data_common/live_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.8/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.2.1/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.8/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.2.1/vcsc_data_common/order/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 import logging
 import pandas as pd
 
 
 class OrderException(Exception):
     pass
 
-
+from datetime import datetime
 class Order:
     def __init__(self, paper_trading_api_end_point: str):
         self.paper_trading_api_end_point = paper_trading_api_end_point
 
-    def place_mp_buy_order_with_ratio(self, username: str, portfolio_cycle_id: int, symbol: str, ratio: float, tradingDate: str = None):
+    def place_mp_buy_order_with_ratio(self, username: str, portfolio_cycle_id: int, symbol: str, ratio: float, tradingDate: str = datetime.today().strftime('%Y-%m-%d')):
         logging.info('start place_mp_buy_order_with_ratio')
         url = f"{self.paper_trading_api_end_point}/order/placeOrderWithRatio"
 
         payload = json.dumps({
             "username": username,
             "symbol": symbol,
             "orderType": "MP",
             "ratio": ratio,
             "side": "B",
             'tradingDate': tradingDate
-        })
+        }) 
+
         headers = {
             'Content-Type': 'application/json'
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
 
         if(response.status_code != 200):
@@ -35,25 +36,26 @@
                 f'place_mp_buy_order_with_ratio: http code: {response.status_code} --> {response.text}')
 
             raise OrderException('place_mp_buy_order_with_ratio api error')
 
         logging.info(
             f'place_mp_buy_order_with_ratio {username} - {portfolio_cycle_id} - {symbol} - {ratio}: ')
 
-    def place_mp_sell_order_with_ratio(self, username: str, portfolio_cycle_id: int, symbol: str, ratio: float, tradingDate: str = None):
+    def place_mp_sell_order_with_ratio(self, username: str, portfolio_cycle_id: int, symbol: str, ratio: float, tradingDate: str = datetime.today().strftime('%Y-%m-%d')):
         url = f"{self.paper_trading_api_end_point}/order/placeOrderWithRatio"
 
         payload = json.dumps({
             "username": username,
             "symbol": symbol,
             "orderType": "MP",
             "ratio": ratio,
             "side": "S",
             'tradingDate': tradingDate
         })
+
         headers = {
             'Content-Type': 'application/json'
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
 
         if(response.status_code != 200):
```

### Comparing `vcsc_data_common-0.1.8/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.2.1/vcsc_data_common/portfolio_info/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,31 +19,41 @@
         paper_trading_db_connection_str = f'postgresql://{paper_trading_db_username}:{paper_trading_db_password}@{paper_trading_db_host}:{paper_trading_db_port}/{paper_trading_db_name}'
         self.paper_trading_db_connection = create_engine(
             paper_trading_db_connection_str).connect()
 
     def get_all_portfolio(self):
         return pd.read_sql(f""" 
             select t1."portfolioConfigId",t4."tradingModel",t4."portfolioModel",t1.username,t1.symbol,COALESCE("latestMatchPrice",0) as "latestMatchPrice",
-                "totalAmount",CASE WHEN "forceSellAmount" > "availableAmount" THEN 0 ELSE "availableAmount" - "forceSellAmount"  END as "availableAmount",
+                "totalAmount","availableAmount",
                 "scheduledAmount", "averageMatchedPrice","targetPercent",
-                "balance","initBalance", t1."cutoffDate", "forceSellAmount" , t1."portfolioType"
+                "balance","initBalance", t1."cutoffDate", "forceSellAmount" , t1."portfolioType",t1."diffBalanceRemain"
                 from "portfolio" t1
                 left join "symbol_info" t2 on t1.symbol = t2.symbol
                 left join "portfolio_config" t4 on t1."portfolioConfigId" = t4.id
 				WHERE t4.status = 'RUNNING'
         """, con=self.paper_trading_db_connection)
 
-    def update_target_percent_portfolio(self, portfolio_data: dict, cycle_length: int, portfolioModel: int):
+    def update_target_percent_portfolio(self, portfolio_data: dict, portfolio_model: int,signals:dict,trading_model:int,trading_date:str=None):
 
         url = f"{self.paper_trading_api_end_point}/portfolioRatio/updateNewRatio"
 
-        payload = json.dumps({
+        payload_data = {
             "ratio": portfolio_data,
-            "portfolioModel": portfolioModel
-        })
+            "portfolioModel": portfolio_model,
+            "tradingDate": trading_date,
+            "signals":signals,
+            'tradingModel':trading_model
+        } if trading_date != None else {
+            "ratio": portfolio_data,
+            "portfolioModel": portfolio_model,
+            "signals":signals,
+            'tradingModel':trading_model
+        }
+
+        payload = json.dumps(payload_data)
         headers = {
             'Content-Type': 'application/json'
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
 
         if(response.status_code == 200):
@@ -54,18 +64,15 @@
                 f'update_target_percent_portfolio ==> {response.text}')
             raise Exception('update_target_percent_portfolio failed')
 
         ### hard code backtest môi trường dev ###
         try:
             url = f"http://10.11.0.99:31377/portfolioRatio/updateNewRatio"
 
-            payload = json.dumps({
-                "ratio": portfolio_data,
-                "portfolioModel": portfolioModel
-            })
+            payload = json.dumps(payload_data)
             headers = {
                 'Content-Type': 'application/json'
             }
 
             response = requests.request(
                 "POST", url, headers=headers, data=payload)
```

