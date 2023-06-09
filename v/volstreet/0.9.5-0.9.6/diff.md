# Comparing `tmp/volstreet-0.9.5.tar.gz` & `tmp/volstreet-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-0.9.5.tar", last modified: Thu Jun  8 12:57:22 2023, max compression
+gzip compressed data, was "volstreet-0.9.6.tar", last modified: Fri Jun  9 10:18:52 2023, max compression
```

## Comparing `volstreet-0.9.5.tar` & `volstreet-0.9.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 12:57:22.019606 volstreet-0.9.5/
--rw-rw-rw-   0        0        0      497 2023-06-08 12:57:22.019606 volstreet-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-0.9.5/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0     1375 2023-06-08 12:57:22.021819 volstreet-0.9.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-08 12:57:22.006535 volstreet-0.9.5/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-0.9.5/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-0.9.5/volstreet/__init__.py
--rw-rw-rw-   0        0        0     8133 2023-06-07 07:39:33.000000 volstreet-0.9.5/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2694 2023-06-07 14:47:58.000000 volstreet-0.9.5/volstreet/constants.py
--rw-rw-rw-   0        0        0    24214 2023-06-07 14:47:58.000000 volstreet-0.9.5/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   157692 2023-06-08 12:56:39.000000 volstreet-0.9.5/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-0.9.5/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-0.9.5/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-0.9.5/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    14536 2023-06-07 14:47:58.000000 volstreet-0.9.5/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:57:22.017640 volstreet-0.9.5/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-06-08 12:57:21.000000 volstreet-0.9.5/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-06-08 12:57:21.000000 volstreet-0.9.5/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 12:57:21.000000 volstreet-0.9.5/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      787 2023-06-08 12:57:21.000000 volstreet-0.9.5/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-08 12:57:21.000000 volstreet-0.9.5/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 10:18:52.505343 volstreet-0.9.6/
+-rw-rw-rw-   0        0        0      497 2023-06-09 10:18:52.505343 volstreet-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-0.9.6/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-0.9.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1375 2023-06-09 10:18:52.506838 volstreet-0.9.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 10:18:52.496495 volstreet-0.9.6/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-0.9.6/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-0.9.6/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     8133 2023-06-07 07:39:33.000000 volstreet-0.9.6/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2694 2023-06-07 14:47:58.000000 volstreet-0.9.6/volstreet/constants.py
+-rw-rw-rw-   0        0        0    24214 2023-06-07 14:47:58.000000 volstreet-0.9.6/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   161941 2023-06-09 10:14:18.000000 volstreet-0.9.6/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-0.9.6/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-0.9.6/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-0.9.6/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    14536 2023-06-07 14:47:58.000000 volstreet-0.9.6/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-09 10:18:52.504342 volstreet-0.9.6/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      787 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-0.9.5/setup.cfg` & `volstreet-0.9.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 302e 392e 350d 0a61  rsion = 0.9.5..a
+00000020: 7273 696f 6e20 3d20 302e 392e 360d 0a61  rsion = 0.9.6..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-0.9.5/volstreet/SmartWebSocketV2.py` & `volstreet-0.9.6/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.5/volstreet/blackscholes.py` & `volstreet-0.9.6/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.5/volstreet/constants.py` & `volstreet-0.9.6/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.5/volstreet/datamodule.py` & `volstreet-0.9.6/volstreet/datamodule.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.5/volstreet/dealingroom.py` & `volstreet-0.9.6/volstreet/dealingroom.py`

 * *Files 2% similar despite different names*

```diff
@@ -482,24 +482,31 @@
 
     def fetch_ltp(self):
         return fetchltp("NFO", self.symbol, self.token)
 
     def fetch_symbol_token(self):
         return self.symbol, self.token
 
-    def place_order(self, transaction_type, quantity_in_lots, price="LIMIT", order_tag=""):
-        if price.upper() == "LIMIT":
-            price = self.fetch_ltp()
-            modifier = 1.05 if transaction_type.upper() == "BUY" else 0.95
-            price = price * modifier
+    def place_order(self, transaction_type, quantity_in_lots, price="LIMIT", stop_loss_order=False, order_tag=""):
+        if isinstance(price, str):
+            if price.upper() == "LIMIT":
+                price = self.fetch_ltp()
+                modifier = 1.05 if transaction_type.upper() == "BUY" else 0.95
+                price = price * modifier
         spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
         order_ids = []
         for qty in spliced_orders:
             order_id = place_order(
-                self.symbol, self.token, qty * self.lot_size, transaction_type, price, order_tag=order_tag
+                self.symbol,
+                self.token,
+                qty * self.lot_size,
+                transaction_type,
+                price,
+                stop_loss_order=stop_loss_order,
+                order_tag=order_tag
             )
             order_ids.append(order_id)
         self.order_id_log.append(order_ids)
         return order_ids
 
 
 class Strangle:
@@ -2579,20 +2586,22 @@
     def intraday_strangle(
         self,
         quantity_in_lots,
         call_strike_offset=0,
         put_strike_offset=0,
         stop_loss=1.6,
         exit_time=(15, 29),
-        sleep_time=60,
+        sleep_time=5,
         catch_trend=False,
         trend_qty_ratio=1,
         trend_strike_offset=0,
-        trend_sl=0.003
+        trend_sl=0.003,
+        place_sl_orders=False
     ):
+
         """Intraday strangle strategy. Trades strangle with  stop loss. All offsets are in percentage terms.
         Parameters
         ----------
         quantity_in_lots : int
             Quantity in lots
         call_strike_offset : float, optional
             Call strike offset in percentage terms, by default 0
@@ -2608,318 +2617,385 @@
             Catch trend or not, by default False
         trend_qty_ratio : int, optional
             Ratio of trend quantity to strangle quantity, by default 1
         trend_strike_offset : float, optional
             Strike offset for trend order in percentage terms, by default 0
         trend_sl : float, optional
             Stop loss for trend order, by default 0.003
+        place_sl_orders : bool, optional
+            Place stop loss orders or not, by default False
         """
 
-        order_tag = "Intraday Strangle"
-        underlying_ltp = self.fetch_ltp()
-        call_strike = underlying_ltp * (1 + call_strike_offset)
-        put_strike = underlying_ltp * (1 - put_strike_offset)
-        call_strike = findstrike(call_strike, self.base)
-        put_strike = findstrike(put_strike, self.base)
-        expiry = self.current_expiry
-
-        strangle = Strangle(call_strike=call_strike, put_strike=put_strike, underlying=self.name, expiry=expiry)
-
-        call_order_ids, put_order_ids = strangle.place_order(
-            "SELL", quantity_in_lots, prices="LIMIT", order_tag=order_tag
-        )
-
-        orderbook = fetch_book('orderbook')
-        order_statuses = lookup_and_return(orderbook, 'orderid', call_order_ids+put_order_ids, 'status')
-        check_and_notify_order_statuses(
-            order_statuses,
-            self.webhook_url,
-            order_tag=order_tag,
-            Underlying=self.name,
-            Action="SELL",
-            Strikes=[call_strike, put_strike],
-            Expiry=expiry,
-            Quantity=quantity_in_lots
-        )
-
-        call_avg_price = lookup_and_return(orderbook, 'orderid', call_order_ids, 'averageprice').astype(float).mean()
-        put_avg_price = lookup_and_return(orderbook, 'orderid', put_order_ids, 'averageprice').astype(float).mean()
-        total_avg_price = call_avg_price + put_avg_price
-
-        call_stop_loss_price = call_avg_price * stop_loss
-        put_stop_loss_price = put_avg_price * stop_loss
-
-        self.log_combined_order(
-            call_strike=call_strike,
-            put_strike=put_strike,
-            expiry=expiry,
-            buy_or_sell="SELL",
-            call_price=call_avg_price,
-            put_price=put_avg_price,
-            order_tag=order_tag
-        )
-
-        summary_message = "\n".join(
-            f"{k}: {v}" for k, v in self.order_log[order_tag][0].items()
-        )
-
-        traded_call_iv, traded_put_iv, traded_avg_iv = strangle_iv(
-            callprice=call_avg_price,
-            putprice=put_avg_price,
-            callstrike=call_strike,
-            putstrike=put_strike,
-            spot=underlying_ltp,
-            timeleft=timetoexpiry(expiry)
-        )
-
-        summary_message += f"\nTraded IVs: {traded_call_iv}, {traded_put_iv}, {traded_avg_iv}"
-        summary_message += f"\nCall SL: {call_stop_loss_price}, Put SL: {put_stop_loss_price}"
-        notifier(summary_message, self.webhook_url)
-
-        def position_monitor():
+        @log_errors
+        def position_monitor(info_dict):
 
-            nonlocal strangle, call_avg_price, put_avg_price, call_stop_loss_price, put_stop_loss_price, exit_price_dict
-            nonlocal call_sl, put_sl, underlying_ltp, call_ltp, put_ltp, profit_in_pts
-            nonlocal in_trade
+            c_avg_price = info_dict["call_avg_price"]
+            p_avg_price = info_dict["put_avg_price"]
+            traded_strangle = info_dict["traded_strangle"]
 
             last_print_time = currenttime()
             last_log_time = currenttime()
             last_notify_time = currenttime()
             print_interval = timedelta(seconds=5)
             log_interval = timedelta(minutes=5)
             notify_interval = timedelta(minutes=60)
-            while in_trade:
-                underlying_ltp = self.fetch_ltp()
-                call_ltp, put_ltp = strangle.fetch_ltp()
+            while not info_dict["exit_triggers"]["trade_complete"]:
+                spot_price = self.fetch_ltp()
+                c_ltp, p_ltp = traded_strangle.fetch_ltp()
+                info_dict["underlying_ltp"] = spot_price
+                info_dict["call_ltp"] = c_ltp
+                info_dict["put_ltp"] = p_ltp
                 call_iv, put_iv, avg_iv = strangle_iv(
-                    callprice=call_ltp,
-                    putprice=put_ltp,
+                    callprice=c_ltp,
+                    putprice=p_ltp,
                     callstrike=call_strike,
                     putstrike=put_strike,
-                    spot=underlying_ltp,
+                    spot=spot_price,
                     timeleft=timetoexpiry(expiry)
                 )
-
-                if call_sl is False:
-                    call_sl = call_ltp > call_stop_loss_price
-                if put_sl is False:
-                    put_sl = put_ltp > put_stop_loss_price
+                info_dict["call_iv"] = call_iv
+                info_dict["put_iv"] = put_iv
+                info_dict["avg_iv"] = avg_iv
 
                 # Calculate mtm price
-                call_exit_price = exit_price_dict.get('call', call_ltp)
-                put_exit_price = exit_price_dict.get('put', put_ltp)
+                call_exit_price = info_dict.get('call_exit_price', c_ltp)
+                put_exit_price = info_dict.get('put_exit_price', p_ltp)
                 mtm_price = call_exit_price + put_exit_price
 
                 # Calculate profit
-                profit_in_pts = (call_avg_price + put_avg_price) - mtm_price
+                profit_in_pts = (c_avg_price + p_avg_price) - mtm_price
                 profit_in_rs = profit_in_pts * self.lot_size * quantity_in_lots
+                info_dict["profit_in_pts"] = profit_in_pts
+                info_dict["profit_in_rs"] = profit_in_rs
 
                 message = (
                     f"\nUnderlying: {self.name}\n"
                     f"Time: {currenttime():%d-%m-%Y %H:%M:%S}\n"
-                    f"Underlying LTP: {underlying_ltp}\n"
+                    f"Underlying LTP: {spot_price}\n"
                     f"Call Strike: {call_strike}\n"
                     f"Put Strike: {put_strike}\n"
-                    f"Call Price: {call_ltp}\n"
-                    f"Put Price: {put_ltp}\n"
+                    f"Call Price: {c_ltp}\n"
+                    f"Put Price: {p_ltp}\n"
                     f"MTM Price: {mtm_price}\n"
                     f"IVs: {call_iv}, {put_iv}, {avg_iv}\n"
-                    f"Call SL: {call_sl}\n"
-                    f"Put SL: {put_sl}\n"
-                    f"Profit Pts: {profit_in_pts:.2f}\n"
-                    f"Profit: {profit_in_rs:.2f}\n"
+                    f"Call SL: {info_dict['call_sl']}\n"
+                    f"Put SL: {info_dict['put_sl']}\n"
+                    f"Profit Pts: {info_dict['profit_in_pts']:.2f}\n"
+                    f"Profit: {info_dict['profit_in_rs']:.2f}\n"
                 )
                 if currenttime() - last_print_time > print_interval:
                     print(message)
                     last_print_time = currenttime()
                 if currenttime() - last_log_time > log_interval:
                     logger.info(message)
                     last_log_time = currenttime()
                 if currenttime() - last_notify_time > notify_interval:
                     notifier(message, self.webhook_url)
                     last_notify_time = currenttime()
                 sleep(sleep_time)
 
-        def trend_catcher(sl_type, qty_ratio, stoploss, strike_offset):
-            nonlocal underlying_ltp, in_trade
+        @log_errors
+        def trend_catcher(info_dict, sl_type, qty_ratio, sl, strike_offset):
 
             offset = 1-strike_offset if sl_type == "call" else 1+strike_offset
-            trend = "Up" if sl_type == "call" else "Down"
+
+            spot_price = info_dict["underlying_ltp"]
 
             # Setting up the trend option
-            strike = underlying_ltp * offset
+            strike = spot_price * offset
             strike = findstrike(strike, self.base)
             opt_type = "PE" if sl_type == "call" else "CE"
             qty_in_lots = max(int(quantity_in_lots * qty_ratio), 1)
             trend_option = Option(strike, opt_type, self.name, expiry)
 
             # Placing the trend option order
             place_option_order_and_notify(
-                trend_option, "SELL", qty_in_lots, "Intraday Strangle Trend Catcher", self.webhook_url
+                trend_option, "SELL", qty_in_lots, "LIMIT", "Intraday Strangle Trend Catcher", self.webhook_url
             )
 
             # Setting up the stop loss
-            sl_multiplier = 1 - stoploss if sl_type == "call" else 1 + stoploss
-            sl_price = underlying_ltp * sl_multiplier
+            sl_multiplier = 1 - sl if sl_type == "call" else 1 + sl
+            sl_price = spot_price * sl_multiplier
             trend_sl_hit = False
 
             last_print_time = currenttime()
             print_interval = timedelta(seconds=10)
-            while all([currenttime().time() < time(*exit_time), in_trade]):
-                trend_sl_hit = underlying_ltp < sl_price if sl_type == "call" else underlying_ltp > sl_price
+            while all([currenttime().time() < time(*exit_time), not info_dict["exit_triggers"]["trade_complete"]]):
+                spot_price = info_dict["underlying_ltp"]
+                trend_sl_hit = spot_price < sl_price if sl_type == "call" else spot_price > sl_price
                 if trend_sl_hit:
                     break
                 sleep(1)
                 if currenttime() - last_print_time > print_interval:
                     last_print_time = currenttime()
                     print(
                         f"{self.name} {sl_type} trend catcher running.\n"
-                        + f"Stoploss price: {sl_price}, Underlying Price: {underlying_ltp}\n"
+                        + f"Stoploss price: {sl_price}, Underlying Price: {spot_price}\n"
                         + f"Stoploss hit: {trend_sl_hit}.\n"
                     )
 
             if trend_sl_hit:
                 notifier(
-                    f"{self.name} strangle {trend} trend catcher stoploss hit.", self.webhook_url
+                    f"{self.name} strangle {sl_type} trend catcher stoploss hit.", self.webhook_url
                 )
             else:
                 notifier(
-                    f"{self.name} strangle {trend} trend catcher exiting.", self.webhook_url
+                    f"{self.name} strangle {sl_type} trend catcher exiting.", self.webhook_url
                 )
 
             # Buying the trend option back
             place_option_order_and_notify(
-                trend_option, "BUY", qty_in_lots, "Intraday Strangle Trend Catcher", self.webhook_url
+                trend_option, "BUY", qty_in_lots, "LIMIT", "Intraday Strangle Trend Catcher", self.webhook_url
             )
 
-        def process_stop_loss(sl_type):
+        def check_for_stop_loss(info_dict, side, sl_order_ids=None):
+
+            if sl_order_ids is None:  # Not using SL orders
+                sl = info_dict[f"{side}_ltp"] > info_dict[f"{side}_stop_loss_price"]
+
+            else:  # Using SL orders
+                sl = False
+                pass  # TODO: Implement fetching order status and checking for SL
+
+            info_dict[f"{side}_sl"] = sl
 
-            nonlocal strangle, call_sl, put_sl, exit_price_dict
+        def process_stop_loss(info_dict, sl_type):
 
-            if call_sl and put_sl:  # Check to avoid double processing
+            if info_dict["call_sl"] and info_dict["put_sl"]:  # Check to avoid double processing
                 return
 
+            traded_strangle = info_dict["traded_strangle"]
             # Buying the stop loss option back
             notifier(f'{self.name} strangle {sl_type} stop loss hit.', self.webhook_url)
-            option_to_buy = strangle.call_option if sl_type == "call" else strangle.put_option
+            option_to_buy = traded_strangle.call_option if sl_type == "call" else traded_strangle.put_option
             exit_price = place_option_order_and_notify(
-                option_to_buy, "BUY", quantity_in_lots, order_tag, self.webhook_url
+                option_to_buy, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
             )
-            exit_price_dict[sl_type] = exit_price
+            info_dict[f'{sl_type}_exit_price'] = exit_price
 
             # Starting the trend catcher
             if catch_trend:
                 trend_thread = Thread(
                     target=trend_catcher,
-                    args=(sl_type, trend_qty_ratio, trend_sl, trend_strike_offset)
+                    args=(info_dict, sl_type, trend_qty_ratio, trend_sl, trend_strike_offset),
                 )
                 trend_thread.start()
 
             # Wait for exit or other stop loss to hit
+            other_sl_type = "put" if sl_type == "call" else "call"
             while all([currenttime().time() < time(*exit_time)]):
-                sleep(1)
-                if call_sl and put_sl:
-                    other_sl_option = strangle.put_option if sl_type == "call" else strangle.call_option
-                    other_sl_type = "put" if sl_type == "call" else "call"
+                check_for_stop_loss(info_dict, other_sl_type)
+                if info_dict[f"{other_sl_type}_sl"]:
+                    other_sl_option = traded_strangle.put_option if sl_type == "call" else traded_strangle.call_option
                     notifier(f'{self.name} strangle {other_sl_type} stop loss hit.', self.webhook_url)
                     other_exit_price = place_option_order_and_notify(
-                        other_sl_option, "BUY", quantity_in_lots, order_tag, self.webhook_url
+                        other_sl_option, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
                     )
-                    exit_price_dict[other_sl_type] = other_exit_price
+                    info_dict[f'{other_sl_type}_exit_price'] = other_exit_price
                     break
+                sleep(sleep_time)
 
-        in_trade = True
-        call_sl = False
-        put_sl = False
-        profit_in_pts = 0
+        # Setting strikes and expiry
+        order_tag = "Intraday Strangle"
+        underlying_ltp = self.fetch_ltp()
+        call_strike = underlying_ltp * (1 + call_strike_offset)
+        put_strike = underlying_ltp * (1 - put_strike_offset)
+        call_strike = findstrike(call_strike, self.base)
+        put_strike = findstrike(put_strike, self.base)
+        expiry = self.current_expiry
+
+        # Placing the main order
+        strangle = Strangle(call_strike=call_strike, put_strike=put_strike, underlying=self.name, expiry=expiry)
+        call_order_ids, put_order_ids = strangle.place_order(
+            "SELL", quantity_in_lots, prices="LIMIT", order_tag=order_tag
+        )
+        orderbook = fetch_book('orderbook')
+        order_statuses = lookup_and_return(orderbook, 'orderid', call_order_ids+put_order_ids, 'status')
+        check_and_notify_order_statuses(
+            order_statuses,
+            self.webhook_url,
+            target_status="complete",
+            order_tag=order_tag,
+            Underlying=self.name,
+            Action="SELL",
+            Strikes=[call_strike, put_strike],
+            Expiry=expiry,
+            Quantity=quantity_in_lots
+        )
+
+        # Calculating average prices
+        call_avg_price = lookup_and_return(orderbook, 'orderid', call_order_ids, 'averageprice').astype(float).mean()
+        put_avg_price = lookup_and_return(orderbook, 'orderid', put_order_ids, 'averageprice').astype(float).mean()
+        total_avg_price = call_avg_price + put_avg_price
+
+        call_stop_loss_price = call_avg_price * stop_loss
+        put_stop_loss_price = put_avg_price * stop_loss
+
+        # Logging information and sending notification
+        self.log_combined_order(
+            call_strike=call_strike,
+            put_strike=put_strike,
+            expiry=expiry,
+            buy_or_sell="SELL",
+            call_price=call_avg_price,
+            put_price=put_avg_price,
+            order_tag=order_tag
+        )
+
+        summary_message = "\n".join(
+            f"{k}: {v}" for k, v in self.order_log[order_tag][-1].items()
+        )
+
+        traded_call_iv, traded_put_iv, traded_avg_iv = strangle_iv(
+            callprice=call_avg_price,
+            putprice=put_avg_price,
+            callstrike=call_strike,
+            putstrike=put_strike,
+            spot=underlying_ltp,
+            timeleft=timetoexpiry(expiry)
+        )
+
+        summary_message += f"\nTraded IVs: {traded_call_iv}, {traded_put_iv}, {traded_avg_iv}"
+        summary_message += f"\nCall SL: {call_stop_loss_price}, Put SL: {put_stop_loss_price}"
+        notifier(summary_message, self.webhook_url)
+
+        if place_sl_orders:
+            call_stop_loss_order_ids = place_option_order_and_notify(
+                option=strangle.call_option,
+                action="BUY",
+                qty_in_lots=quantity_in_lots,
+                price=call_stop_loss_price,
+                order_tag="Call SL Strangle",
+                webhook_url=self.webhook_url,
+                stop_loss_order=True,
+                target_status="trigger pending",
+                return_avg_price=False
+            )
+            put_stop_loss_order_ids = place_option_order_and_notify(
+                option=strangle.put_option,
+                action="BUY",
+                qty_in_lots=quantity_in_lots,
+                price=put_stop_loss_price,
+                order_tag="Put SL Strangle",
+                webhook_url=self.webhook_url,
+                stop_loss_order=True,
+                target_status="trigger pending",
+                return_avg_price=False
+            )
+        else:
+            call_stop_loss_order_ids = None
+            put_stop_loss_order_ids = None
+
+        # Setting up shared info dict
         call_ltp, put_ltp = strangle.fetch_ltp()
-        exit_price_dict = {}
+        shared_info_dict = {
+            "traded_strangle": strangle,
+            "call_avg_price": call_avg_price,
+            "put_avg_price": put_avg_price,
+            "call_stop_loss_price": call_stop_loss_price,
+            "put_stop_loss_price": put_stop_loss_price,
+            "call_stop_loss_order_ids": call_stop_loss_order_ids,
+            "put_stop_loss_order_ids": put_stop_loss_order_ids,
+            "call_ltp": call_ltp,
+            "put_ltp": put_ltp,
+            "underlying_ltp": underlying_ltp,
+            "call_sl": False,
+            "put_sl": False,
+            "exit_triggers": {"trade_complete": False}
+        }
 
-        position_monitor_thread = Thread(target=position_monitor)
+        position_monitor_thread = Thread(target=position_monitor, args=(shared_info_dict,))
         position_monitor_thread.start()
 
         # Wait for exit time or both stop losses to hit (Main Loop)
         while all([currenttime().time() < time(*exit_time)]):
-            sleep(2)
-            if call_sl or put_sl:
-                if call_sl:
-                    process_stop_loss("call")
-                if put_sl:
-                    process_stop_loss("put")
+            check_for_stop_loss(shared_info_dict, 'call')
+            if shared_info_dict["call_sl"]:
+                process_stop_loss(shared_info_dict, "call")
+                break
+            check_for_stop_loss(shared_info_dict, 'put')
+            if shared_info_dict["put_sl"]:
+                process_stop_loss(shared_info_dict, "put")
                 break
+            sleep(sleep_time)
 
         # Out of the while loop, so exit time reached or both stop losses hit
 
+        call_sl = shared_info_dict["call_sl"]
+        put_sl = shared_info_dict["put_sl"]
+
         if not call_sl and not put_sl:
             call_order_ids, put_order_ids = strangle.place_order("BUY", quantity_in_lots, "LIMIT", order_tag)
             order_book = fetch_book('orderbook')
             order_statuses_ = lookup_and_return(order_book, 'orderid', call_order_ids + put_order_ids, 'status')
             check_and_notify_order_statuses(
                 order_statuses_,
                 self.webhook_url,
+                target_status="complete",
                 order_tag='Strangle Exit',
                 Underlying=self.name,
                 Action='BUY',
-                Strike=strangle.call_option.strike,
+                Strikes=[strangle.call_option.strike, strangle.put_option.strike],
                 Expiry=strangle.call_option.expiry,
                 Qty=quantity_in_lots,
             )
 
-            exit_price_dict['call'] = lookup_and_return(
+            shared_info_dict['call_exit_price'] = lookup_and_return(
                 order_book, 'orderid', call_order_ids, 'averageprice'
             ).astype(float).mean()
-            exit_price_dict['put'] = lookup_and_return(
+            shared_info_dict['put_exit_price'] = lookup_and_return(
                 order_book, 'orderid', put_order_ids, 'averageprice'
             ).astype(float).mean()
 
         elif (call_sl or put_sl) and not (call_sl and put_sl):  # Only one stop loss hit
             exit_option = strangle.put_option if call_sl else strangle.call_option
             non_sl_exit_price = place_option_order_and_notify(
-                exit_option, "BUY", quantity_in_lots, order_tag, self.webhook_url
+                exit_option, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
             )
             exit_option = "put" if call_sl else "call"
-            exit_price_dict[exit_option] = non_sl_exit_price
+            shared_info_dict[f"{exit_option}_exit_price"] = non_sl_exit_price
 
         else:  # Both stop losses hit
             pass
 
         # Calculate profit
-        total_exit_price = sum(exit_price_dict.values())
+        total_exit_price = shared_info_dict["call_exit_price"] + shared_info_dict["put_exit_price"]
         exit_message = (
             f"{self.name} strangle exited.\n"
             f"Time: {currenttime():%d-%m-%Y %H:%M:%S}\n"
             f"Underlying LTP: {underlying_ltp}\n"
             f"Call Price: {call_ltp}\n"
             f"Put Price: {put_ltp}\n"
             f"Call SL: {call_sl}\n"
             f"Put SL: {put_sl}\n"
-            f"Call Exit Price: {exit_price_dict['call']}\n"
-            f"Put Exit Price: {exit_price_dict['put']}\n"
+            f"Call Exit Price: {shared_info_dict['call_exit_price']}\n"
+            f"Put Exit Price: {shared_info_dict['put_exit_price']}\n"
             f"Total Exit Price: {total_exit_price}\n"
             f"Total Entry Price: {total_avg_price}\n"
             f"Profit Pts: {total_avg_price - total_exit_price}\n"
         )
         exit_dict = {
-            "Call exit price": exit_price_dict["call"],
-            "Put exit price": exit_price_dict["put"],
+            "Call exit price": shared_info_dict["call_exit_price"],
+            "Put exit price": shared_info_dict["put_exit_price"],
             "Total exit price": total_exit_price,
             "Points captured": total_avg_price - total_exit_price,
             "Call SL": call_sl,
             "Put SL": put_sl,
         }
         try:
             self.order_log[order_tag][0].update(exit_dict)
         except Exception as e:
             notifier(
                 f"{self.name}: Error updating order list with exit details. {e}",
                 self.webhook_url,
             )
         notifier(exit_message, self.webhook_url)
-        in_trade = False
+        shared_info_dict["exit_triggers"] = {"trade_complete": True}
         position_monitor_thread.join()
+        return shared_info_dict
 
     def intraday_straddle_delta_hedged(
         self,
         quantity_in_lots,
         exit_time=(15, 30),
         websocket=None,
         wait_for_equality=False,
@@ -3268,21 +3344,21 @@
             data=json.dumps(data),
             headers={"Content-Type": "application/json"},
         )
         print(message)
     return
 
 
-def check_and_notify_order_statuses(statuses, webhook_url=None, **kwargs):
+def check_and_notify_order_statuses(statuses, webhook_url=None, target_status="complete", **kwargs):
 
     order_prefix = f"{kwargs['order_tag']}: " if "order_tag" in kwargs else ""
     order_message = [f"{k}-{v}" for k, v in kwargs.items() if k != "order_tag"]
     order_message = ", ".join(order_message)
 
-    if all(statuses == "complete"):
+    if all(statuses == target_status):
         notifier(
             f"{order_prefix}Order(s) placed successfully for {order_message}",
             webhook_url
         )
     elif all(statuses == "rejected"):
         notifier(
             f"{order_prefix}All orders rejected for {order_message}",
@@ -3303,31 +3379,56 @@
         notifier(
             f"{order_prefix}ERROR. Order statuses uncertain for {order_message}",
             webhook_url
         )
         raise Exception("Order statuses uncertain")
 
 
-def place_option_order_and_notify(option, action, qty_in_lots, order_tag, webhook_url=None):
-    order_ids = option.place_order(action, qty_in_lots, "LIMIT", order_tag)
+def place_option_order_and_notify(
+        option: Option,
+        action: str,
+        qty_in_lots,
+        price="LIMIT",
+        order_tag="",
+        webhook_url=None,
+        stop_loss_order=False,
+        target_status="complete",
+        return_avg_price=True
+):
+
+    if stop_loss_order:
+        assert isinstance(price, (int, float)), "Stop loss order requires a price"
+
+    order_ids = option.place_order(
+        transaction_type=action,
+        quantity_in_lots=qty_in_lots,
+        price=price,
+        stop_loss_order=stop_loss_order,
+        order_tag=order_tag
+    )
     order_book = fetch_book('orderbook')
     order_statuses_ = lookup_and_return(order_book, 'orderid', order_ids, 'status')
     check_and_notify_order_statuses(
         order_statuses_,
         webhook_url,
+        target_status=target_status,
         order_tag=order_tag,
         Underlying=option.underlying,
         Action=action,
         Strike=option.strike,
         OptionType=option.option_type,
         Expiry=option.expiry,
         Qty=qty_in_lots
     )
-    avg_price = lookup_and_return(order_book, 'orderid', order_ids, 'averageprice').astype(float).mean()
-    return avg_price
+
+    if return_avg_price:
+        avg_price = lookup_and_return(order_book, 'orderid', order_ids, 'averageprice').astype(float).mean()
+        return avg_price
+
+    return order_ids
 
 
 # Market Hours
 def markethours():
     if time(9, 10) < currenttime().time() < time(15, 30):
         return True
     else:
```

### Comparing `volstreet-0.9.5/volstreet/discord_bot.py` & `volstreet-0.9.6/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.5/volstreet/nsefunctions.py` & `volstreet-0.9.6/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.5/volstreet/strategies.py` & `volstreet-0.9.6/volstreet/strategies.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.5/volstreet.egg-info/requires.txt` & `volstreet-0.9.6/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

