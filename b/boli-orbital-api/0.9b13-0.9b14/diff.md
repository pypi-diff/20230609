# Comparing `tmp/boli_orbital_api-0.9b13.tar.gz` & `tmp/boli_orbital_api-0.9b14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boli_orbital_api-0.9b13.tar", max compression
+gzip compressed data, was "boli_orbital_api-0.9b14.tar", max compression
```

## Comparing `boli_orbital_api-0.9b13.tar` & `boli_orbital_api-0.9b14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6414 2023-06-05 20:24:45.320328 boli_orbital_api-0.9b13/.gitignore
--rw-r--r--   0        0        0      541 2023-06-05 19:49:57.553690 boli_orbital_api-0.9b13/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-06-05 20:23:02.778565 boli_orbital_api-0.9b13/LICENSE
--rw-r--r--   0        0        0     2772 2023-06-03 22:55:11.905218 boli_orbital_api-0.9b13/README.md
--rw-r--r--   0        0        0     2922 2023-06-03 22:55:11.858554 boli_orbital_api-0.9b13/README_ES.md
--rw-r--r--   0        0        0     1305 2023-06-05 20:18:34.246061 boli_orbital_api-0.9b13/TODO.md
--rw-r--r--   0        0        0       42 2023-06-03 22:49:39.137192 boli_orbital_api-0.9b13/boli_orbital_api/__init__.py
--rw-r--r--   0        0        0     3476 2023-06-05 19:46:20.983826 boli_orbital_api-0.9b13/boli_orbital_api/logger.py
--rw-r--r--   0        0        0    62893 2023-06-05 19:46:40.680170 boli_orbital_api-0.9b13/boli_orbital_api/rpc.py
--rw-r--r--   0        0        0       14 2023-06-02 00:43:19.185603 boli_orbital_api-0.9b13/docs/using.md
--rw-r--r--   0        0        0     1255 2023-06-05 20:13:20.047751 boli_orbital_api-0.9b13/pyproject.toml
--rw-r--r--   0        0        0       16 2023-06-01 22:31:09.954549 boli_orbital_api-0.9b13/requirements.txt
--rw-r--r--   0        0        0      100 2023-06-05 19:52:15.081557 boli_orbital_api-0.9b13/requirements_freezed.txt
--rw-r--r--   0        0        0        0 2023-05-31 19:36:48.526207 boli_orbital_api-0.9b13/tests/__init__.py
--rw-r--r--   0        0        0      409 2023-06-05 19:41:08.195877 boli_orbital_api-0.9b13/tests/test.py
--rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 boli_orbital_api-0.9b13/PKG-INFO
+-rw-r--r--   0        0        0     6425 2023-06-07 13:34:10.219390 boli_orbital_api-0.9b14/.gitignore
+-rw-r--r--   0        0        0      541 2023-06-05 19:49:57.553690 boli_orbital_api-0.9b14/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-06-05 20:23:02.778565 boli_orbital_api-0.9b14/LICENSE
+-rw-r--r--   0        0        0     2772 2023-06-03 22:55:11.905218 boli_orbital_api-0.9b14/README.md
+-rw-r--r--   0        0        0     2922 2023-06-03 22:55:11.858554 boli_orbital_api-0.9b14/README_ES.md
+-rw-r--r--   0        0        0     1305 2023-06-05 20:18:34.246061 boli_orbital_api-0.9b14/TODO.md
+-rw-r--r--   0        0        0       42 2023-06-07 13:32:45.641287 boli_orbital_api-0.9b14/boli_orbital_api/__init__.py
+-rw-r--r--   0        0        0     2724 2023-06-09 18:45:51.900962 boli_orbital_api-0.9b14/boli_orbital_api/logger.py
+-rw-r--r--   0        0        0    62361 2023-06-09 18:45:51.784297 boli_orbital_api-0.9b14/boli_orbital_api/rpc.py
+-rw-r--r--   0        0        0       14 2023-06-02 00:43:19.185603 boli_orbital_api-0.9b14/docs/using.md
+-rw-r--r--   0        0        0     1255 2023-06-09 18:45:51.830963 boli_orbital_api-0.9b14/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-06-01 22:31:09.954549 boli_orbital_api-0.9b14/requirements.txt
+-rw-r--r--   0        0        0      100 2023-06-09 18:43:19.823212 boli_orbital_api-0.9b14/requirements_freezed.txt
+-rw-r--r--   0        0        0        0 2023-05-31 19:36:48.526207 boli_orbital_api-0.9b14/tests/__init__.py
+-rw-r--r--   0        0        0      409 2023-06-05 19:41:08.195877 boli_orbital_api-0.9b14/tests/test.py
+-rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 boli_orbital_api-0.9b14/PKG-INFO
```

### Comparing `boli_orbital_api-0.9b13/.gitignore` & `boli_orbital_api-0.9b14/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -304,7 +304,8 @@
 # LSP config files
 pyrightconfig.json
 
 # End of https://www.toptal.com/developers/gitignore/api/pycharm,linux,python
 
 /poetry.lock
 
+/recursos/
```

### Comparing `boli_orbital_api-0.9b13/CHANGELOG.md` & `boli_orbital_api-0.9b14/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b13/LICENSE` & `boli_orbital_api-0.9b14/LICENSE`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b13/README.md` & `boli_orbital_api-0.9b14/README.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b13/README_ES.md` & `boli_orbital_api-0.9b14/README_ES.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b13/TODO.md` & `boli_orbital_api-0.9b14/TODO.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b13/boli_orbital_api/logger.py` & `boli_orbital_api-0.9b14/boli_orbital_api/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,83 +18,83 @@
 
 
 logs_dir = Path(__file__).resolve().parent / 'logs'
 logs_dir.mkdir(parents=True, exist_ok=True)
 LOG_FILE = Path(logs_dir / 'orbitalapi.log')
 
 LOGGING_CONFIG = {
-        "version": 1,
-        "disable_existing_loggers": False,
-        "loggers": {
-                "root": {
-                        "level": "INFO",
-                        "propagate": False,
-                        # "handlers": ["stream_handler", "rotating_file_handler"],
-                        "handlers": ["stream_handler"],
-                        },
-
-                "urllib3": {
-                        "level": "WARNING",
-                        "propagate": False,
-                        # "handlers": ["stream_handler", "rotating_file_handler"],
-                        "handlers": ["stream_handler"],
-                        },
-
-                },
-        "handlers": {
-                "stream_handler": {
-                        "class": "logging.StreamHandler",
-                        "stream": "ext://sys.stdout",
-                        "level": "DEBUG",
-                        "filters": ["only_debug"],
-                        "formatter": "default_formatter",
-                        },
-                "file_handler": {
-                        "class": "logging.FileHandler",
-                        "filename": LOG_FILE,
-                        "mode": "a",
-                        "level": "DEBUG",
-                        "formatter": "file_formatter",
-                        },
-                "rotating_file_handler": {
-                        "class": "logging.handlers.RotatingFileHandler",
-                        'maxBytes': 2097152,  # 2Mb
-                        'backupCount': 5,
-                        "filename": LOG_FILE,
-                        "filters": ["only_warning"],
-                        "mode": "a",
-                        "level": "DEBUG",
-                        "formatter": "file_formatter",
-                        },
-                },
-        "filters": {
-                "only_warning": {
-                        "()": LevelOnlyFilter,
-                        "level": logging.WARNING,
-                        },
-                "only_info": {
-                        "()": LevelOnlyFilter,
-                        "level": logging.INFO,
-                        },
-                "only_debug": {
-                        "()": LevelOnlyFilter,
-                        "level": logging.DEBUG,
-                        },
-                },
-        "formatters": {
-                "default_formatter": {
-                        "format": "%(levelname)s - %(name)s - %(funcName)s - %(message)s",
-                        "datefmt": "%Y-%m-%d %H:%M:%S",
-                        },
-                "file_formatter": {
-                        "format": "%(asctime)s - %(levelname)s - %(name)s - %(funcName)s - %(message)s",
-                        "datefmt": "%Y-%m-%d %H:%M:%S",
-                        },
-                },
-        }
+    "version": 1,
+    "disable_existing_loggers": False,
+    "loggers": {
+        "root": {
+            "level": "INFO",
+            "propagate": False,
+            # "handlers": ["stream_handler", "rotating_file_handler"],
+            "handlers": ["stream_handler"],
+        },
+
+        "urllib3": {
+            "level": "WARNING",
+            "propagate": False,
+            # "handlers": ["stream_handler", "rotating_file_handler"],
+            "handlers": ["stream_handler"],
+        },
+
+    },
+    "handlers": {
+        "stream_handler": {
+            "class": "logging.StreamHandler",
+            "stream": "ext://sys.stdout",
+            "level": "DEBUG",
+            "filters": ["only_debug"],
+            "formatter": "default_formatter",
+        },
+        "file_handler": {
+            "class": "logging.FileHandler",
+            "filename": LOG_FILE,
+            "mode": "a",
+            "level": "DEBUG",
+            "formatter": "file_formatter",
+        },
+        "rotating_file_handler": {
+            "class": "logging.handlers.RotatingFileHandler",
+            'maxBytes': 2097152,  # 2Mb
+            'backupCount': 5,
+            "filename": LOG_FILE,
+            "filters": ["only_warning"],
+            "mode": "a",
+            "level": "DEBUG",
+            "formatter": "file_formatter",
+        },
+    },
+    "filters": {
+        "only_warning": {
+            "()": LevelOnlyFilter,
+            "level": logging.WARNING,
+        },
+        "only_info": {
+            "()": LevelOnlyFilter,
+            "level": logging.INFO,
+        },
+        "only_debug": {
+            "()": LevelOnlyFilter,
+            "level": logging.DEBUG,
+        },
+    },
+    "formatters": {
+        "default_formatter": {
+            "format": "%(levelname)s - %(name)s - %(funcName)s - %(message)s",
+            "datefmt": "%Y-%m-%d %H:%M:%S",
+        },
+        "file_formatter": {
+            "format": "%(asctime)s - %(levelname)s - %(name)s - %(funcName)s - %(message)s",
+            "datefmt": "%Y-%m-%d %H:%M:%S",
+        },
+    },
+}
 
 
 def setup_logger(name: str):
     """
         Setup a logger using defaults
     Args:
         name:
```

### Comparing `boli_orbital_api-0.9b13/boli_orbital_api/rpc.py` & `boli_orbital_api-0.9b14/boli_orbital_api/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         BOLICOIN COMPATIBLE VERSION: v2.0.0.2-g
         Bolicoin/Bolivarcoin platform and cryptocurrency from http://bolis.info
 
     __author__: "Asdrúbal Velásquez Lagrave - Twitter/Telegram: @Visionario"
     __copyright__: "2018-2023"
     __credits__: [""]
     __license__: "MIT"
-    __version__: 0.9b13
+    __version__: 0.9b14
     __maintainer__: "Asdrúbal Velásquez Lagrave"
     __email__: "hello@orbital.center"
     __status__: "BETA"
     __app_name__: "Node API Rpc main class for Bolivarcoin/Bolicoin blockchain (Layer 1)",
     __url__: "https://orbital.center"
 
 """
@@ -20,24 +20,24 @@
 
 from orjson import dumps
 from requests import Response, exceptions as request_exceptions, post
 
 from .logger import setup_logger
 
 __all__ = [
-        "Node",
-        "GobjectListSignals",
-        "GobjectListTypes",
-        "MasternodeCountOptions",
-        "MasternodeStartModes",
-        "About",
-        "VERSION",
-        ]
+    "Node",
+    "GobjectListSignals",
+    "GobjectListTypes",
+    "MasternodeCountOptions",
+    "MasternodeStartModes",
+    "About",
+    "VERSION",
+]
 
-VERSION = "0.9b13"
+VERSION = "0.9b14"
 
 # LOGGER
 logger = setup_logger(__name__)
 
 
 class GobjectListSignals:
     """See gobject_list()"""
@@ -209,15 +209,15 @@
     def sendtoaddress(
             self,
             address: str,
             amount: float,
             comment: str = '',
             comment_to: str = '',
             subtractfeefromamount: bool = False
-            ) -> dict:
+    ) -> dict:
         """
             sendtoaddress "bolivarcoinaddress" amount ( "comment" "comment-to" subtractfeefromamount use_is use_ps )
 
             Send an amount to a given address.
 
             Arguments:
             1. "bolivarcoinaddress" (string, required) The bolivarcoin address to send to.
@@ -241,23 +241,23 @@
             > bolivarcoin-cli sendtoaddress "AJw5Dqdh47muwzqN1tsmhAiFrvoKqCpna8" 0.1 "" "" true
             > curl --user myusername --data-binary '{"jsonrpc": "1.0", "id":"curltest", "method": "sendtoaddress", "params": ["AJw5Dqdh47muwzqN1tsmhAiFrvoKqCpna8", 0.1, "donation", "seans outpost"] }' -H 'content-type: text/plain;' http://127.0.0.1:14776/
 
         """
         if amount <= 0:
             return {"result": None, "error": "amount <= 0"}
         return _process_result(
-                self.raw_call(
-                        "sendtoaddress", params=[
-                                address,
-                                amount,
-                                comment,
-                                comment_to,
-                                subtractfeefromamount]
-                        )
-                )
+            self.raw_call(
+                "sendtoaddress", params=[
+                    address,
+                    amount,
+                    comment,
+                    comment_to,
+                    subtractfeefromamount]
+            )
+        )
 
 
 # ╻ ╻╺┳╸╻╻
 # ┃ ┃ ┃ ┃┃
 # ┗━┛ ╹ ╹┗━╸
 class _Utils:
     """Utils methods"""
@@ -453,15 +453,15 @@
 
     def getlisttransactions(
             self,
             account: str = "*",
             count: int = 10,
             from_number: int = 0,
             includewatchonly: bool = False
-            ) -> dict:
+    ) -> dict:
         """
         Bolicoin uses "*" as default account
 
             listtransactions    ( "account" count from includeWatchonly)
 
             Returns up to 'count' most recent transactions skipping the first 'from' transactions for account 'account'.
 
@@ -522,23 +522,23 @@
 
             As a json rpc call
             > curl --user myusername --data-binary '{"jsonrpc": "1.0", "id":"curltest", "method": "listtransactions", "params": ["*", 20, 100] }' -H 'content-type: text/plain;' http://127.0.0.1:14776/
 
 
         """
         return _process_result(
-                self.raw_call(
-                        "listtransactions", params=[
-                                account,
-                                count,
-                                from_number,
-                                includewatchonly
-                                ]
-                        )
-                )
+            self.raw_call(
+                "listtransactions", params=[
+                    account,
+                    count,
+                    from_number,
+                    includewatchonly
+                ]
+            )
+        )
 
 
 # ┏┳┓╻┏┓╻╻┏┓╻┏━╸
 # ┃┃┃┃┃┗┫┃┃┗┫┃╺┓
 # ╹ ╹╹╹ ╹╹╹ ╹┗━┛
 class _Mining:
     """Mining methods"""
@@ -996,15 +996,15 @@
 
         return _process_result(self.raw_call("gobject", params=['count']))
 
     def gobject_list(
             self,
             signal: GobjectListSignals = GobjectListSignals.ALL,
             type: GobjectListTypes = GobjectListTypes.ALL
-            ) -> dict:
+    ) -> dict:
         """
         List governance objects (can be filtered by signal and/or object type)
 
         :param signal: should be 'valid', 'funding', 'delete', 'endorsed' or 'all'
         :param type: should be 'proposals', 'triggers', 'watchdogs' or 'all'
         :return:
 
@@ -1091,23 +1091,23 @@
         return _process_result(self.raw_call("getdifficulty"))
 
 
 # ┏┓╻┏━┓╺┳┓┏━╸
 # ┃┗┫┃ ┃ ┃┃┣╸
 # ╹ ╹┗━┛╺┻┛┗━╸
 class Node(
-        _Utils,
-        _Wallet,
-        _BlockChain,
-        _Network,
-        _Transactions,
-        _Governance,
-        _Masternode,
-        _Help
-        ):
+    _Utils,
+    _Wallet,
+    _BlockChain,
+    _Network,
+    _Transactions,
+    _Governance,
+    _Masternode,
+    _Help
+):
     """ Main RPC/API Class
 
         Communicate with nodes via RPC
 
         BOLICOIN COMPATIBLE VERSION: v2.0.0.2-g
     """
 
@@ -1119,15 +1119,15 @@
             server_ip: str = "127.0.0.1",
             scheme: str = 'http',
             core_type: int = 1,
             name: str = '',
             ticker: str = 'BOLI',
             is_masternode: bool = False,
             app_id: str = 'standard',
-            ):
+    ):
 
         self.server_ip = server_ip
         self.rpc_port = rpc_port
         self.rpc_user = rpc_user
         self.rpc_password = rpc_password
         self.scheme = scheme
         self.core_type = core_type
@@ -1166,15 +1166,15 @@
         logger.debug("Connecting node...")
         self._check_online_status()
 
     def raw_call(
             self,
             method: str,
             params=None,
-            ) -> Any:
+    ) -> Any:
         """ Rpc communication raw_call main method
 
         It will return:
         # OK
         {"result": response.json()['result'], 'errors': None} When OK
 
         # Server responds but NOT OK
@@ -1191,19 +1191,19 @@
 
         logger.debug(f"raw_call: method:{method} params:{params}")
 
         response: Response = Response()
         try:
             # print(self._data, dumps(self._data), sep="\n")
             response = post(
-                    url=f'{self.scheme}://{self.server_ip}:{self.rpc_port}/',
-                    headers=self._headers,
-                    data=dumps(self._data),
-                    auth=(self.rpc_user, self.rpc_password)
-                    )
+                url=f'{self.scheme}://{self.server_ip}:{self.rpc_port}/',
+                headers=self._headers,
+                data=dumps(self._data),
+                auth=(self.rpc_user, self.rpc_password)
+            )
 
             # print("raw_call_result", response.status_code, response.json())
 
             if response.status_code == 200:
                 self._valid_node = True
                 return {"result": response.json()['result'], 'errors': None}
 
@@ -1223,43 +1223,43 @@
             return {"result": None, 'errors': f'{e}'}
 
     # OBLIGATORIO ENTENDER PREREQUISITOS
     # https://github.com/BlockchainCommons/Learning-Bitcoin-from-the-Command-Line/blob/master/04_5_Sending_Coins_with_Automated_Raw_Transactions.md
     def fundrawtransaction(
             self,
             recipients_with_amounts: dict,  # {"address..1":amount..1,"address..2":amount..2,...}
-            ):
+    ):
         """Sending Coins with Automated Raw Transactions"""
 
         # Step one: Get unfinished TX with createrawtransaction
         try:
             # {'result': '01000000000100d2496b000000001976a9144486f188fd5361906cf9a0c1cd1105f913a080f488ac00000000', 'errors': None}
             rawtransaction = self.raw_call(
-                    method='createrawtransaction',
-                    params=[
-                            [],
-                            recipients_with_amounts,
-                            ]
-                    )
+                method='createrawtransaction',
+                params=[
+                    [],
+                    recipients_with_amounts,
+                ]
+            )
 
             if rawtransaction['errors'] is not None:
                 return {"result": rawtransaction.get('result', None), "errors": rawtransaction.get('errors', True)}
 
             # print("rawtransaction", rawtransaction)
 
         except BaseException as e:
             logger.critical(f'{self.name} fundrawtransaction BaseException "rawtransaction" error: {e}')
             return {"result": None, "errors": e}
 
         # Step two: Fund that bare-bones transaction
         try:
             fund = self.raw_call(
-                    method='fundrawtransaction',
-                    params=[rawtransaction['result']]
-                    )
+                method='fundrawtransaction',
+                params=[rawtransaction['result']]
+            )
 
             # print(f"fund {fund}")
 
             if fund['errors'] is not None:
                 return {"result": fund.get('result', None), "errors": fund.get('errors', True)}
 
             hex = fund['result']['hex']
@@ -1278,32 +1278,32 @@
         except BaseException as e:
             logger.critical(f'{self.name} fundrawtransaction BaseException "fund" error: {e}')
             return {"result": None, "errors": e}
 
         # Decode decoderawtransaction
         try:
             decoded = self.raw_call(
-                    method='decoderawtransaction',
-                    params=[hex]
-                    )
+                method='decoderawtransaction',
+                params=[hex]
+            )
             # print(f"decoded {decoded}")
 
             if decoded['errors'] is not None:
                 return {"result": decoded.get('result', None), "errors": decoded.get('errors', True)}
 
         except BaseException as e:
             logger.critical(f'{self.name} fundrawtransaction BaseException "decoded" error: {e}')
             return {"result": None, "errors": e}
 
         # Step 3: Signs the transaction signrawtransaction
         try:
             signed = self.raw_call(
-                    method='signrawtransaction',
-                    params=[hex]
-                    )
+                method='signrawtransaction',
+                params=[hex]
+            )
 
             # print(f"signed {signed}")
 
             if signed['errors'] is not None:
                 return {"result": signed.get('result', None), "errors": signed.get('errors', True)}
 
             signedhex = signed['result']['hex']
@@ -1312,17 +1312,17 @@
         except BaseException as e:
             logger.critical(f'{self.name} fundrawtransaction BaseException "signed" error: {e}')
             return {"result": None, "errors": e}
 
         # Step 4: Send RAW Transaction sendrawtransaction
         try:
             sent = self.raw_call(
-                    method='sendrawtransaction',
-                    params=[signedhex]
-                    )
+                method='sendrawtransaction',
+                params=[signedhex]
+            )
 
             # print(f"sent {sent}")
 
             if sent['errors'] is not None:
                 return {"result": sent.get('result', None), "errors": sent.get('errors', True)}
 
         except BaseException as e:
@@ -1330,18 +1330,18 @@
             return {"result": None, "errors": e}
 
         # SUCCESS TXID Acquired
         # SUCCESS TXID Acquired
         # SUCCESS TXID Acquired
         # SUCCESS TXID Acquired
         return {
-                "txid": sent['result'],
-                "fee": fee,
-                "errors": sent['errors']
-                }
+            "txid": sent['result'],
+            "fee": fee,
+            "errors": sent['errors']
+        }
 
     @property
     def is_online(self) -> bool:
         self._check_online_status()
         return self._valid_node
 
     @property
@@ -1362,33 +1362,33 @@
                   "params": [1],
                   "id": "foo2"
                 }
               ]''' \
               --header 'Content-Type: text/plain;' localhost:62026
         """
         return {
-                "getblockchaininfo": self.getblockchaininfo(),
-                "getnetworkinfo": self.getnetworkinfo(),
-                "getwalletinfo": self.getwalletinfo()
-                }
+            "getblockchaininfo": self.getblockchaininfo(),
+            "getnetworkinfo": self.getnetworkinfo(),
+            "getwalletinfo": self.getwalletinfo()
+        }
 
     @property
     def api_version(self) -> str:
         return VERSION
 
 
 class About:
 
     @classmethod
     def about(cls):
         return {
-                '__author__': "Asdrúbal Velásquez Lagrave - Twitter/Telegram: @Visionario",
-                '__copyright__': "2018-2023",
-                '__credits__': [""],
-                '__license__': "MIT",
-                '__version__': VERSION,
-                '__maintainer__': "Asdrúbal Velásquez Lagrave",
-                '__email__': "hello@orbital.center",
-                '__status__': "BETA",
-                '__app_name__': "API RPC main class for Bolivarcoin/Bolicoin nodes (Layer 1)",
-                '__url__': "https://orbital.center",
-                }
+            '__author__': "Asdrúbal Velásquez Lagrave - Twitter/Telegram: @Visionario",
+            '__copyright__': "2018-2023",
+            '__credits__': [""],
+            '__license__': "MIT",
+            '__version__': VERSION,
+            '__maintainer__': "Asdrúbal Velásquez Lagrave",
+            '__email__': "hello@orbital.center",
+            '__status__': "BETA",
+            '__app_name__': "API RPC main class for Bolivarcoin/Bolicoin nodes (Layer 1)",
+            '__url__': "https://orbital.center",
+        }
```

### Comparing `boli_orbital_api-0.9b13/pyproject.toml` & `boli_orbital_api-0.9b14/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boli_orbital_api"
-version = "0.9b13"
+version = "0.9b14"
 description = "Orbital API RPC for Bolivarcoin/Bolicoin blockchain"
 authors = ["Asdrubal Velasquez Lagrave <hello@orbital.center>"]
 maintainers = ["Asdrubal Velasquez Lagrave <hello@orbital.center>"]
 repository = "https://github.com/Visionario/BoliOrbitalAPI"
 homepage = "https://orbital.center"
 keywords = ["bolicoin", "bolivarcoin", "criptocurrency", "blockchain", "api"]
 classifiers = [
```

### Comparing `boli_orbital_api-0.9b13/PKG-INFO` & `boli_orbital_api-0.9b14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boli-orbital-api
-Version: 0.9b13
+Version: 0.9b14
 Summary: Orbital API RPC for Bolivarcoin/Bolicoin blockchain
 Home-page: https://orbital.center
 License: MIT
 Keywords: bolicoin,bolivarcoin,criptocurrency,blockchain,api
 Author: Asdrubal Velasquez Lagrave
 Author-email: hello@orbital.center
 Maintainer: Asdrubal Velasquez Lagrave
```

