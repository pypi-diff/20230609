# Comparing `tmp/twelvedata-1.2.8-py2.py3-none-any.whl.zip` & `tmp/twelvedata-1.2.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 44876 bytes, number of entries: 17
+Zip file size: 45067 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      392 b- defN 21-Jan-02 09:28 twelvedata/__init__.py
 -rw-r--r--  2.0 unx    17643 b- defN 21-Nov-11 14:32 twelvedata/client.py
 -rw-r--r--  2.0 unx      750 b- defN 21-Nov-05 17:30 twelvedata/context.py
 -rw-r--r--  2.0 unx   284041 b- defN 22-Jun-27 11:43 twelvedata/endpoints.py
 -rw-r--r--  2.0 unx      338 b- defN 21-Jan-02 09:28 twelvedata/exceptions.py
 -rw-r--r--  2.0 unx     1681 b- defN 21-Mar-22 08:27 twelvedata/http_client.py
 -rw-r--r--  2.0 unx     2544 b- defN 21-Nov-11 20:13 twelvedata/mixins.py
 -rw-r--r--  2.0 unx    11023 b- defN 21-Jun-17 11:29 twelvedata/renders.py
 -rw-r--r--  2.0 unx   286496 b- defN 22-Jun-22 14:18 twelvedata/time_series.py
 -rw-r--r--  2.0 unx     5848 b- defN 22-Jun-27 11:43 twelvedata/utils.py
--rw-r--r--  2.0 unx     7676 b- defN 22-Mar-21 08:06 twelvedata/websocket.py
--rw-r--r--  2.0 unx       39 b- defN 22-Jun-27 11:43 twelvedata-1.2.8.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx     1077 b- defN 22-Jun-27 11:43 twelvedata-1.2.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    19224 b- defN 22-Jun-27 11:43 twelvedata-1.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Jun-27 11:43 twelvedata-1.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 22-Jun-27 11:43 twelvedata-1.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1373 b- defN 22-Jun-27 11:43 twelvedata-1.2.8.dist-info/RECORD
-17 files, 640266 bytes uncompressed, 42644 bytes compressed:  93.3%
+-rw-r--r--  2.0 unx     7966 b- defN 22-Sep-09 08:58 twelvedata/websocket.py
+-rw-r--r--  2.0 unx       39 b- defN 22-Sep-09 08:58 twelvedata-1.2.9.dist-info/AUTHORS.rst
+-rw-r--r--  2.0 unx     1077 b- defN 22-Sep-09 08:58 twelvedata-1.2.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    19386 b- defN 22-Sep-09 08:58 twelvedata-1.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 22-Sep-09 08:58 twelvedata-1.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 22-Sep-09 08:58 twelvedata-1.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1373 b- defN 22-Sep-09 08:58 twelvedata-1.2.9.dist-info/RECORD
+17 files, 640718 bytes uncompressed, 42835 bytes compressed:  93.3%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: twelvedata/utils.py
 Comment: 
 
 Filename: twelvedata/websocket.py
 Comment: 
 
-Filename: twelvedata-1.2.8.dist-info/AUTHORS.rst
+Filename: twelvedata-1.2.9.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: twelvedata-1.2.8.dist-info/LICENSE.txt
+Filename: twelvedata-1.2.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: twelvedata-1.2.8.dist-info/METADATA
+Filename: twelvedata-1.2.9.dist-info/METADATA
 Comment: 
 
-Filename: twelvedata-1.2.8.dist-info/WHEEL
+Filename: twelvedata-1.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: twelvedata-1.2.8.dist-info/top_level.txt
+Filename: twelvedata-1.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: twelvedata-1.2.8.dist-info/RECORD
+Filename: twelvedata-1.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## twelvedata/websocket.py

```diff
@@ -90,17 +90,16 @@
         self.subscribed_symbols = set()
 
         if self.ws:
             self.ws.close()
             time.sleep(1)
 
     def keep_alive(self):
-        while True:
-            time.sleep(10)
-            self.heartbeat()
+        self.logger.info('Method keep_alive is deprecated, use heartbeat method instead')
+        self.heartbeat()
 
     def heartbeat(self):
         if not self.ready:
             return
 
         try:
             self.ws.send('{"action": "heartbeat"}')
@@ -188,32 +187,38 @@
             "params": {
                 "symbols": ",".join(list(symbols))
             }
         }
 
 
 class EventReceiver(threading.Thread):
-    def __init__(self, client):
+    def __init__(self, client, ping_interval=15, ping_timeout=10):
         threading.Thread.__init__(self)
         self.daemon = True
         self.client = client
         self.enabled = True
+        self.ping_interval = ping_interval
+        self.ping_timeout = ping_timeout
 
     def run(self):
         import websocket
         self.client.ws = websocket.WebSocketApp(
             self.client.url,
             on_open=self.on_open,
             on_close=self.on_close,
             on_message=self.on_message,
             on_error=self.on_error
         )
 
         self.client.logger.debug("EventReceiver ready")
-        self.client.ws.run_forever()
+        self.client.ws.run_forever(
+            ping_interval=self.ping_interval,
+            ping_timeout=self.ping_timeout,
+            ping_payload='ping',
+        )
         self.client.logger.debug("EventReceiver exiting")
 
     def on_open(self, _):
         self.client.logger.info("TDWebSocket opened!")
         self.client.on_connect()
 
     def on_close(self, _, close_status_code, close_msg):
```

## Comparing `twelvedata-1.2.8.dist-info/LICENSE.txt` & `twelvedata-1.2.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `twelvedata-1.2.8.dist-info/METADATA` & `twelvedata-1.2.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twelvedata
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python client for Twelve Data
 Home-page: https://github.com/twelvedata/twelvedata-python
 Author: Twelve Data
 Author-email: info@twelvedata.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -336,25 +336,35 @@
 
 #### Features
 * Real-time low latency stream of financial quotes.
 * You might subscribe to stocks, forex, and crypto.
 
 #### Example
 ```python
+import time
 from twelvedata import TDClient
 
+
+messages_history = []
+
+
 def on_event(e):
     # do whatever is needed with data
     print(e)
+    messages_history.append(e)
 
-td = TDClient(apikey="YOUR_API_KEY_HERE")
+
+td = TDClient(apikey="02fb2924fc9e468e99a30decbe1259b7")
 ws = td.websocket(symbols="BTC/USD", on_event=on_event)
 ws.subscribe(['ETH/BTC', 'AAPL'])
 ws.connect()
-ws.keep_alive()
+while True:
+    print('messages received: ', len(messages_history))
+    ws.heartbeat()
+    time.sleep(10)
 ```
 
 Parameters accepted by the `.websocket()` object:
 * **symbols** list of symbols to subscribe
 * **on_event** function that invokes when event from server is received
 * **logger** instance of logger, otherwise set to default
 * **max_queue_size** maximum size of queue, default `12000`
@@ -362,15 +372,15 @@
 
 Applicable methods on `.websocket()` object:
 * `ws.subscribe([list of symbols])`: get data from the symbols passed
 * `ws.unsubscribe([list of symbols])`: stop receiving data from the symbols passed
 * `ws.reset()`: unsubscribe from all symbols
 * `ws.connect()`: establish connection with WebSocket server
 * `ws.disconnect()`: close connection with WebSocket server
-* `ws.keep_alive()`: run connection forever until closed
+* `ws.heartbeat()`: send heartbeat to server
 
 **Important**. Do not forget that WebSockets are only available for Twelve Data users on the [Pro plan](https://twelvedata.com/pricing) and above. Checkout the trial [here](https://support.twelvedata.com/en/articles/5335783-trial).
 
 ### Advanced
 
 #### Custom endpoint
 This method is used to request unrepresented endpoints on this package, but which are available at Twelve Data.
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twelvedata Version: 1.2.8 Summary: Python client
+Metadata-Version: 2.1 Name: twelvedata Version: 1.2.9 Summary: Python client
 for Twelve Data Home-page: https://github.com/twelvedata/twelvedata-python
 Author: Twelve Data Author-email: info@twelvedata.com License: MIT Platform:
 any Classifier: Development Status :: 4 - Beta Classifier: Programming Language
 :: Python Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7
 Description-Content-Type: text/markdown Requires-Dist: pytimeparse (<2,>=1.1)
 Requires-Dist: requests (<3,>=2.22) Provides-Extra: matplotlib Requires-Dist:
 matplotlib (<3,>=2.2) ; (python_version < "3") and extra == 'matplotlib'
@@ -186,42 +186,45 @@
 + MACD(close, 12, 26, 9) ts.with_ema(time_period=7).with_mama().with_mom
 ().with_macd().as_plotly_figure().show() ``` ### WebSocket With the WebSocket,
 a duplex communication channel with the server is established. Make sure to
 have `websocket_client` package [installed](https://pypi.org/project/
 websocket_client/). ![websocket example](https://res.cloudinary.com/dnz8pwg9r/
 image/upload/v1599349899/ws-example.gif) #### Features * Real-time low latency
 stream of financial quotes. * You might subscribe to stocks, forex, and crypto.
-#### Example ```python from twelvedata import TDClient def on_event(e): # do
-whatever is needed with data print(e) td = TDClient(apikey="YOUR_API_KEY_HERE")
-ws = td.websocket(symbols="BTC/USD", on_event=on_event) ws.subscribe(['ETH/
-BTC', 'AAPL']) ws.connect() ws.keep_alive() ``` Parameters accepted by the
-`.websocket()` object: * **symbols** list of symbols to subscribe *
-**on_event** function that invokes when event from server is received *
-**logger** instance of logger, otherwise set to default * **max_queue_size**
-maximum size of queue, default `12000` * **log_level** accepts `debug` or
-`info`, otherwise not set Applicable methods on `.websocket()` object: *
-`ws.subscribe([list of symbols])`: get data from the symbols passed *
-`ws.unsubscribe([list of symbols])`: stop receiving data from the symbols
-passed * `ws.reset()`: unsubscribe from all symbols * `ws.connect()`: establish
-connection with WebSocket server * `ws.disconnect()`: close connection with
-WebSocket server * `ws.keep_alive()`: run connection forever until closed
-**Important**. Do not forget that WebSockets are only available for Twelve Data
-users on the [Pro plan](https://twelvedata.com/pricing) and above. Checkout the
-trial [here](https://support.twelvedata.com/en/articles/5335783-trial). ###
-Advanced #### Custom endpoint This method is used to request unrepresented
-endpoints on this package, but which are available at Twelve Data. ```python
-endpoint = td.custom_endpoint( name="quote", symbol="AAPL", ) endpoint.as_json
-() ``` The only required parameter is `name` which should be identical to the
-endpoint used at Twelve Data. All others can be custom and will vary according
-to the method. #### Debugging When the method doesn't return the desired data
-or throws an error, it might be helpful to understand and analyze the API query
-behind it. Add `.as_url()` to any method or chain of methods, and it will
-return the list of used URLs. ```python ts = td.time_series( symbol="AAPL",
-interval="1min", outputsize=10, timezone="America/New_York", ).with_bbands
-().with_ema() ts.as_url() # ['https://api.twelvedata.com/
+#### Example ```python import time from twelvedata import TDClient
+messages_history = [] def on_event(e): # do whatever is needed with data print
+(e) messages_history.append(e) td = TDClient
+(apikey="02fb2924fc9e468e99a30decbe1259b7") ws = td.websocket(symbols="BTC/
+USD", on_event=on_event) ws.subscribe(['ETH/BTC', 'AAPL']) ws.connect() while
+True: print('messages received: ', len(messages_history)) ws.heartbeat()
+time.sleep(10) ``` Parameters accepted by the `.websocket()` object: *
+**symbols** list of symbols to subscribe * **on_event** function that invokes
+when event from server is received * **logger** instance of logger, otherwise
+set to default * **max_queue_size** maximum size of queue, default `12000` *
+**log_level** accepts `debug` or `info`, otherwise not set Applicable methods
+on `.websocket()` object: * `ws.subscribe([list of symbols])`: get data from
+the symbols passed * `ws.unsubscribe([list of symbols])`: stop receiving data
+from the symbols passed * `ws.reset()`: unsubscribe from all symbols *
+`ws.connect()`: establish connection with WebSocket server * `ws.disconnect()`:
+close connection with WebSocket server * `ws.heartbeat()`: send heartbeat to
+server **Important**. Do not forget that WebSockets are only available for
+Twelve Data users on the [Pro plan](https://twelvedata.com/pricing) and above.
+Checkout the trial [here](https://support.twelvedata.com/en/articles/5335783-
+trial). ### Advanced #### Custom endpoint This method is used to request
+unrepresented endpoints on this package, but which are available at Twelve
+Data. ```python endpoint = td.custom_endpoint( name="quote", symbol="AAPL", )
+endpoint.as_json() ``` The only required parameter is `name` which should be
+identical to the endpoint used at Twelve Data. All others can be custom and
+will vary according to the method. #### Debugging When the method doesn't
+return the desired data or throws an error, it might be helpful to understand
+and analyze the API query behind it. Add `.as_url()` to any method or chain of
+methods, and it will return the list of used URLs. ```python ts =
+td.time_series( symbol="AAPL", interval="1min", outputsize=10,
+timezone="America/New_York", ).with_bbands().with_ema() ts.as_url() # ['https:/
+/api.twelvedata.com/
 time_series?symbol=AAPL&interval=1min&outputsize=10&dp=5&timezone=America/
 New_York&order=desc&prepost=false&format=JSON&apikey=demo', # 'https://
 api.twelvedata.com/
 bbands?symbol=AAPL&interval=1min&series_type=close&time_period=20&sd=2&ma_type=SMA&outputsize=10&dp=5&timezone=America/
 New_York&order=desc&prepost=false&format=JSON&apikey=demo', # 'https://
 api.twelvedata.com/
 ema?symbol=AAPL&interval=1min&series_type=close&time_period=9&outputsize=10&dp=5&timezone=America/
```

## Comparing `twelvedata-1.2.8.dist-info/RECORD` & `twelvedata-1.2.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 twelvedata/endpoints.py,sha256=c8-UqVg3omPigfRxZnCu1DCpad8awIvpHVgHe213q_Q,284041
 twelvedata/exceptions.py,sha256=fHrDQ7UFf2g_4fYMAO_BkOqicsbxOflJcwalmcB7-WI,338
 twelvedata/http_client.py,sha256=-GIR_ydG8l1ImTOcZYGyRzCzNdNJdf9VrR-PsYOEYgk,1681
 twelvedata/mixins.py,sha256=6KGBQ5ubJPZM98v1GycSNYmFf-wHSGMF_i25nM6j8uY,2544
 twelvedata/renders.py,sha256=dYCPJcrV9N1D0R8KrZvzPYQzxA0PJsK5nkYGAhM_lbs,11023
 twelvedata/time_series.py,sha256=2pd5bNvj1IAlCon3G7iVQqcGN5w3vgP5w05HPq9Gow0,286496
 twelvedata/utils.py,sha256=7HaU6JeoecBQ4pqQ29AHmMly2AWIoGrfbRHDqnJSOfs,5848
-twelvedata/websocket.py,sha256=30_Qd6Mbc4uCJdFgphYe9CMGYbn2YQe052hHtTi4jrA,7676
-twelvedata-1.2.8.dist-info/AUTHORS.rst,sha256=bY7GQkErn8ie8aYrkBhU1SNZwsihup-Ou4w-oqKxdqQ,39
-twelvedata-1.2.8.dist-info/LICENSE.txt,sha256=JVefiIjGZCXgYLmij5ZmYoCmGuO0YI074JKyxswNO1Y,1077
-twelvedata-1.2.8.dist-info/METADATA,sha256=1aC8aqvw3tTGlDkJspE01Mz1yZcylP-yEePeAi4IYSM,19224
-twelvedata-1.2.8.dist-info/WHEEL,sha256=oh0NKYrTcu1i1-wgrI1cnhkjYIi8WJ-8qd9Jrr5_y4E,110
-twelvedata-1.2.8.dist-info/top_level.txt,sha256=jZMc4A1CQ1AL72ksuvNOoOabXQH3NdVOx4GPxnhwpZU,11
-twelvedata-1.2.8.dist-info/RECORD,,
+twelvedata/websocket.py,sha256=dS7ck9GyuA0qICDJO6OFrtsblEv0WHMBYbSzgnJTtHY,7966
+twelvedata-1.2.9.dist-info/AUTHORS.rst,sha256=bY7GQkErn8ie8aYrkBhU1SNZwsihup-Ou4w-oqKxdqQ,39
+twelvedata-1.2.9.dist-info/LICENSE.txt,sha256=JVefiIjGZCXgYLmij5ZmYoCmGuO0YI074JKyxswNO1Y,1077
+twelvedata-1.2.9.dist-info/METADATA,sha256=NMsDQ7GP84QwJ3NdIdHROrW-Xy7zNCLLDN_uhi33G00,19386
+twelvedata-1.2.9.dist-info/WHEEL,sha256=oh0NKYrTcu1i1-wgrI1cnhkjYIi8WJ-8qd9Jrr5_y4E,110
+twelvedata-1.2.9.dist-info/top_level.txt,sha256=jZMc4A1CQ1AL72ksuvNOoOabXQH3NdVOx4GPxnhwpZU,11
+twelvedata-1.2.9.dist-info/RECORD,,
```

