# Comparing `tmp/volstreet-0.9.7.tar.gz` & `tmp/volstreet-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-0.9.7.tar", last modified: Mon Jun 12 13:05:09 2023, max compression
+gzip compressed data, was "volstreet-0.9.8.tar", last modified: Tue Jun 13 08:25:51 2023, max compression
```

## Comparing `volstreet-0.9.7.tar` & `volstreet-0.9.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 13:05:09.174687 volstreet-0.9.7/
--rw-rw-rw-   0        0        0      497 2023-06-12 13:05:09.174687 volstreet-0.9.7/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-0.9.7/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-0.9.7/pyproject.toml
--rw-rw-rw-   0        0        0     1375 2023-06-12 13:05:09.176046 volstreet-0.9.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 13:05:09.166493 volstreet-0.9.7/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-0.9.7/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-0.9.7/volstreet/__init__.py
--rw-rw-rw-   0        0        0     8133 2023-06-07 07:39:33.000000 volstreet-0.9.7/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2694 2023-06-07 14:47:58.000000 volstreet-0.9.7/volstreet/constants.py
--rw-rw-rw-   0        0        0    25475 2023-06-12 13:04:14.000000 volstreet-0.9.7/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   167244 2023-06-12 13:04:14.000000 volstreet-0.9.7/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-0.9.7/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-0.9.7/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-0.9.7/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    14536 2023-06-07 14:47:58.000000 volstreet-0.9.7/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:05:09.173654 volstreet-0.9.7/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      787 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 08:25:51.362784 volstreet-0.9.8/
+-rw-rw-rw-   0        0        0      497 2023-06-13 08:25:51.362784 volstreet-0.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-0.9.8/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-0.9.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1375 2023-06-13 08:25:51.364780 volstreet-0.9.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 08:25:51.355502 volstreet-0.9.8/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-0.9.8/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-0.9.8/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     8133 2023-06-07 07:39:33.000000 volstreet-0.9.8/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2694 2023-06-07 14:47:58.000000 volstreet-0.9.8/volstreet/constants.py
+-rw-rw-rw-   0        0        0    25475 2023-06-12 13:04:14.000000 volstreet-0.9.8/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   167555 2023-06-13 08:04:56.000000 volstreet-0.9.8/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-0.9.8/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-0.9.8/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-0.9.8/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    14536 2023-06-07 14:47:58.000000 volstreet-0.9.8/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:25:51.362784 volstreet-0.9.8/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      787 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-0.9.7/setup.cfg` & `volstreet-0.9.8/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 302e 392e 370d 0a61  rsion = 0.9.7..a
+00000020: 7273 696f 6e20 3d20 302e 392e 380d 0a61  rsion = 0.9.8..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-0.9.7/volstreet/SmartWebSocketV2.py` & `volstreet-0.9.8/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.7/volstreet/blackscholes.py` & `volstreet-0.9.8/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.7/volstreet/constants.py` & `volstreet-0.9.8/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.7/volstreet/datamodule.py` & `volstreet-0.9.8/volstreet/datamodule.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.7/volstreet/dealingroom.py` & `volstreet-0.9.8/volstreet/dealingroom.py`

 * *Files 0% similar despite different names*

```diff
@@ -2814,14 +2814,15 @@
         put_strike = underlying_ltp * (1 - put_strike_offset)
         call_strike = findstrike(call_strike, self.base)
         put_strike = findstrike(put_strike, self.base)
         expiry = self.current_expiry
 
         # Placing the main order
         strangle = Strangle(call_strike=call_strike, put_strike=put_strike, underlying=self.name, expiry=expiry)
+        call_ltp, put_ltp = strangle.fetch_ltp()
         call_order_ids, put_order_ids = strangle.place_order(
             "SELL", quantity_in_lots, prices="LIMIT", order_tag=order_tag
         )
         orderbook = fetch_book('orderbook')
         order_statuses = lookup_and_return(orderbook, 'orderid', call_order_ids+put_order_ids, 'status')
         check_and_notify_order_statuses(
             order_statuses,
@@ -2832,16 +2833,20 @@
             Action="SELL",
             Strikes=[call_strike, put_strike],
             Expiry=expiry,
             Quantity=quantity_in_lots
         )
 
         # Calculating average prices
-        call_avg_price = lookup_and_return(orderbook, 'orderid', call_order_ids, 'averageprice').astype(float).mean()
-        put_avg_price = lookup_and_return(orderbook, 'orderid', put_order_ids, 'averageprice').astype(float).mean()
+        def get_avg_price(book, order_ids, ltp):
+            prices = lookup_and_return(book, ['orderid', 'status'], [order_ids, 'complete'], 'averageprice')
+            return ltp if not isinstance(prices, np.ndarray) else prices.astype(float).mean()
+
+        call_avg_price = get_avg_price(orderbook, call_order_ids, call_ltp)
+        put_avg_price = get_avg_price(orderbook, put_order_ids, put_ltp)
         total_avg_price = call_avg_price + put_avg_price
 
         call_stop_loss_price = call_avg_price * call_stop_loss if call_stop_loss else call_avg_price * stop_loss
         put_stop_loss_price = put_avg_price * put_stop_loss if put_stop_loss else put_avg_price * stop_loss
 
         # Logging information and sending notification
         self.log_combined_order(
@@ -2895,15 +2900,14 @@
                 return_avg_price=False
             )
         else:
             call_stop_loss_order_ids = None
             put_stop_loss_order_ids = None
 
         # Setting up shared info dict
-        call_ltp, put_ltp = strangle.fetch_ltp()
         shared_info_dict = {
             "traded_strangle": strangle,
             "call_avg_price": call_avg_price,
             "put_avg_price": put_avg_price,
             "call_stop_loss_price": call_stop_loss_price,
             "put_stop_loss_price": put_stop_loss_price,
             "call_stop_loss_order_ids": call_stop_loss_order_ids,
@@ -3871,14 +3875,21 @@
 
 # Finding ATM strike
 def findstrike(x, base):
     number = base * round(x / base)
     return int(number)
 
 
+def custom_round(x, base=0.05):
+    num = base * round(x / base)
+    if num == 0:
+        num = base
+    return round(num, 2)
+
+
 def splice_orders(quantity_in_lots, freeze_qty):
     if quantity_in_lots > freeze_qty:
         loops = int(quantity_in_lots / freeze_qty)
         if loops > large_order_threshold:
             raise Exception(
                 "Order too big. This error was raised to prevent accidental large order placement."
             )
@@ -4147,15 +4158,15 @@
         if order_type == "LIMIT":
             if execution_price < 10 and qty < 4000:
                 execution_price = np.ceil(price) if action == "BUY" else max(np.floor(price), 0.05)
 
         params.update({
             "variety": "NORMAL",
             "ordertype": order_type,
-            "price": round(execution_price, 1)
+            "price": custom_round(execution_price)
         })
 
     for attempt in range(1, 4):
         try:
             return obj.placeOrder(params)
         except Exception as e:
             if attempt == 3:
```

### Comparing `volstreet-0.9.7/volstreet/discord_bot.py` & `volstreet-0.9.8/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.7/volstreet/nsefunctions.py` & `volstreet-0.9.8/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.7/volstreet/strategies.py` & `volstreet-0.9.8/volstreet/strategies.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.7/volstreet.egg-info/requires.txt` & `volstreet-0.9.8/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

