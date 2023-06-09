# Comparing `tmp/martin-binance-1.3.0b22.tar.gz` & `tmp/martin-binance-1.3.0b23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin-binance-1.3.0b22.tar", last modified: Tue Jun  6 19:02:43 2023, max compression
+gzip compressed data, was "martin-binance-1.3.0b23.tar", last modified: Thu Jun  8 07:35:21 2023, max compression
```

## Comparing `martin-binance-1.3.0b22.tar` & `martin-binance-1.3.0b23.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.0b22/.deepsource.toml
--rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.0b22/.dockerignore
--rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.0b22/.github/FUNDING.yml
--rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.0b22/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.0b22/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.0b22/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.0b22/.gitignore
--rwxr-xr-x   0        0        0    17691 2023-06-06 16:49:15.643997 martin-binance-1.3.0b22/CHANGELOG.md
--rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.0b22/Dockerfile
--rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.0b22/LICENSE
--rwxr-xr-x   0        0        0    35437 2023-05-30 12:20:07.843798 martin-binance-1.3.0b22/README.md
--rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.0b22/doc/Create_strategy.png
--rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.0b22/doc/Model of logarithmic grid.ods
--rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.0b22/doc/Modified martingale.svg
--rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.0b22/doc/graf1.png
--rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.0b22/doc/tlg_notify.png
--rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.0b22/doc/tmux.png
--rw-r--r--   0        0        0     2004 2023-06-06 19:02:16.703877 martin-binance-1.3.0b22/martin_binance/__init__.py
--rw-r--r--   0        0        0     2218 2023-06-05 19:37:24.375292 martin-binance-1.3.0b22/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2949 2023-06-03 09:17:19.879857 martin-binance-1.3.0b22/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    12323 2023-06-04 14:26:32.096258 martin-binance-1.3.0b22/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6474 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6469 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6475 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4710 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/client.py
--rw-r--r--   0        0        0   181595 2023-06-06 19:02:16.719858 martin-binance-1.3.0b22/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.0b22/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.0b22/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.0b22/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.0b22/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    79598 2023-06-06 16:41:38.089871 martin-binance-1.3.0b22/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.0b22/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.0b22/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.0b22/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16185 2023-05-30 12:20:07.847793 martin-binance-1.3.0b22/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-05-30 12:20:07.847793 martin-binance-1.3.0b22/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.3.0b22/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.0b22/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.0b22/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1203 2023-06-03 20:53:44.166165 martin-binance-1.3.0b22/pyproject.toml
--rw-r--r--   0        0        0      320 2023-06-03 20:53:44.162164 martin-binance-1.3.0b22/requirements.txt
--rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.0b22/uml/architecture.puml
--rw-r--r--   0        0        0    36614 1970-01-01 00:00:00.000000 martin-binance-1.3.0b22/PKG-INFO
+-rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.0b23/.deepsource.toml
+-rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.0b23/.dockerignore
+-rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.0b23/.github/FUNDING.yml
+-rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.0b23/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.0b23/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.0b23/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.0b23/.gitignore
+-rwxr-xr-x   0        0        0    17766 2023-06-08 07:01:31.585733 martin-binance-1.3.0b23/CHANGELOG.md
+-rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.0b23/Dockerfile
+-rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.0b23/LICENSE
+-rwxr-xr-x   0        0        0    35437 2023-05-30 12:20:07.843798 martin-binance-1.3.0b23/README.md
+-rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.0b23/doc/Create_strategy.png
+-rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.0b23/doc/Model of logarithmic grid.ods
+-rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.0b23/doc/Modified martingale.svg
+-rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.0b23/doc/graf1.png
+-rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.0b23/doc/tlg_notify.png
+-rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.0b23/doc/tmux.png
+-rw-r--r--   0        0        0     2050 2023-06-07 08:37:58.500647 martin-binance-1.3.0b23/martin_binance/__init__.py
+-rw-r--r--   0        0        0     2218 2023-06-05 19:37:24.375292 martin-binance-1.3.0b23/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2949 2023-06-03 09:17:19.879857 martin-binance-1.3.0b23/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    12323 2023-06-04 14:26:32.096258 martin-binance-1.3.0b23/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6474 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6469 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6475 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4710 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/client.py
+-rw-r--r--   0        0        0   181684 2023-06-07 16:41:03.333036 martin-binance-1.3.0b23/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.0b23/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.0b23/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.0b23/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.0b23/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    79598 2023-06-06 16:41:38.089871 martin-binance-1.3.0b23/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.0b23/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.0b23/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.0b23/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16185 2023-05-30 12:20:07.847793 martin-binance-1.3.0b23/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-05-30 12:20:07.847793 martin-binance-1.3.0b23/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.3.0b23/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.0b23/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.0b23/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1203 2023-06-03 20:53:44.166165 martin-binance-1.3.0b23/pyproject.toml
+-rw-r--r--   0        0        0      320 2023-06-03 20:53:44.162164 martin-binance-1.3.0b23/requirements.txt
+-rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.0b23/uml/architecture.puml
+-rw-r--r--   0        0        0    36614 1970-01-01 00:00:00.000000 martin-binance-1.3.0b23/PKG-INFO
```

### Comparing `martin-binance-1.3.0b22/.github/ISSUE_TEMPLATE/bug_report.md` & `martin-binance-1.3.0b23/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/.github/ISSUE_TEMPLATE/feature_request.md` & `martin-binance-1.3.0b23/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/.github/workflows/codeql.yml` & `martin-binance-1.3.0b23/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/CHANGELOG.md` & `martin-binance-1.3.0b23/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+## v1.3.0b22-23 2023-06-08
+### Fix
+* correct funding check in start()
+
 ## v1.3.0b18-21 2023-06-06
 ### Fix
 * #59
 
 ### Update
 * Sync record/play
-* Add SAVE_DS = True  # Save session result data (ticker, orders) for compare
+* Add SAVE_DS = True  # Save session result snapshot (ticker, orders) for compare
 * up requirements for exchanges-wrapper to 1.3.0-1
 * refactoring class StrategyBase
 * + backtest_data_control()
  
 ## v1.3.0b12 2023-06-02
 ### Fix
 * deepsource issues
```

### Comparing `martin-binance-1.3.0b22/Dockerfile` & `martin-binance-1.3.0b23/Dockerfile`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/LICENSE` & `martin-binance-1.3.0b23/LICENSE`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/README.md` & `martin-binance-1.3.0b23/README.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/doc/Create_strategy.png` & `martin-binance-1.3.0b23/doc/Create_strategy.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/doc/Model of logarithmic grid.ods` & `martin-binance-1.3.0b23/doc/Model of logarithmic grid.ods`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/doc/Modified martingale.svg` & `martin-binance-1.3.0b23/doc/Modified martingale.svg`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/doc/graf1.png` & `martin-binance-1.3.0b23/doc/graf1.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/doc/tlg_notify.png` & `martin-binance-1.3.0b23/doc/tlg_notify.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/doc/tmux.png` & `martin-binance-1.3.0b23/doc/tmux.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/__init__.py` & `martin-binance-1.3.0b23/martin_binance/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b22"
+__version__ = "1.3.0b23"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 #
 import platform
@@ -48,8 +48,9 @@
     copy(Path(Path(__file__).parent.absolute(), "cli_2_TESTBTCTESTUSDT.py.template"),
          Path(WORK_PATH, "cli_2_TESTBTCTESTUSDT.py"))
     print(f"Before the first run, set the parameters in {CONFIG_FILE}")
     if STANDALONE:
         raise SystemExit(1)
     raise UserWarning()
 
-# TODO Add parameter for not record analytics data in 'S' MODE
+# TODO GRID_ONLY mode: after depositing asset refresh balance
+# TODO 'S' mode - use last_state for start ???
```

### Comparing `martin-binance-1.3.0b22/martin_binance/backtest/OoTSP.py` & `martin-binance-1.3.0b23/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/backtest/VCoSEL.py` & `martin-binance-1.3.0b23/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/backtest/exchange_simulator.py` & `martin-binance-1.3.0b23/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/cli_0_BTCUSDT.py.template` & `martin-binance-1.3.0b23/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/cli_1_BTCUSDT.py.template` & `martin-binance-1.3.0b23/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin-binance-1.3.0b23/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/client.py` & `martin-binance-1.3.0b23/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/executor.py` & `martin-binance-1.3.0b23/martin_binance/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b22"
+__version__ = "1.3.0b23"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -1355,22 +1355,22 @@
         if self.first_run:
             if MODE in ('T', 'TC'):
                 self.start_process()
             self.save_init_assets(ff, fs)
         if self.restart:
             # Check refunding before restart
             if self.cycle_buy:
-                go_trade = fs >= self.initial_reverse_second if self.reverse else self.initial_second
+                go_trade = fs >= (self.initial_reverse_second if self.reverse else self.initial_second)
                 if go_trade:
                     if FEE_IN_PAIR and FEE_MAKER:
                         fs = self.initial_reverse_second if self.reverse else self.initial_second
                     _ff = ff
                     _fs = fs - profit_s
             else:
-                go_trade = ff >= self.initial_reverse_first if self.reverse else self.initial_first
+                go_trade = ff >= (self.initial_reverse_first if self.reverse else self.initial_first)
                 if go_trade:
                     if FEE_IN_PAIR and FEE_MAKER:
                         ff = self.initial_reverse_first if self.reverse else self.initial_first
                     _ff = ff - profit_f
                     _fs = fs
             if go_trade:
                 self.wait_refunding_for_start = False
@@ -1403,27 +1403,29 @@
                         self.queue_to_db.put(data_to_db)
                 self.save_init_assets(ff, fs)
                 if STANDALONE and COLLECT_ASSETS:
                     _ff, _fs = self.collect_assets()
                     ff -= _ff
                     fs -= _fs
             else:
+                self.first_run = False
                 self.wait_refunding_for_start = True
                 self.message_log(f"Wait refunding for start, having now: first: {ff}, second: {fs}")
                 return
         self.avg_rate = f2d(self.get_buffered_ticker().last_price)
         if GRID_ONLY:
             if USE_ALL_FUND and not self.start_after_shift:
                 if self.cycle_buy:
                     self.deposit_second = fs
                     self.message_log(f'Use all available funds: {self.deposit_second} {self.s_currency}')
                 else:
                     self.deposit_first = ff
                     self.message_log(f'Use all available funds: {self.deposit_first} {self.f_currency}')
             if not self.check_min_amount(for_tp=False) and self.command is None:
+                self.first_run = False
                 self.grid_only_restart = True
                 self.message_log("Waiting funding for convert", color=Style.B_WHITE)
                 return
         if not self.first_run and not self.start_after_shift and not self.reverse and not GRID_ONLY:
             self.message_log(f"Complete {self.cycle_buy_count} buy cycle and {self.cycle_sell_count} sell cycle\n"
                              f"For all cycles profit:\n"
                              f"First: {self.sum_profit_first}\n"
@@ -3026,19 +3028,19 @@
         # print(f"on_new_funds.funds: {funds}")
         ff = funds.get(self.f_currency, 0)
         fs = funds.get(self.s_currency, 0)
         if self.wait_refunding_for_start:
             ff = f2d(ff.total_for_currency) if ff else Decimal('0.0')
             fs = f2d(fs.total_for_currency) if fs else Decimal('0.0')
             if self.cycle_buy:
-                go_trade = fs >= self.initial_reverse_second if self.reverse else self.initial_second
+                go_trade = fs >= (self.initial_reverse_second if self.reverse else self.initial_second)
             else:
-                go_trade = ff >= self.initial_reverse_first if self.reverse else self.initial_first
+                go_trade = ff >= (self.initial_reverse_first if self.reverse else self.initial_first)
             if go_trade:
-                self.message_log("Start after on_new_funds())")
+                self.message_log("Started after receipt of funds")
                 self.start()
                 return
         if self.tp_order_hold:
             if self.tp_order_hold['buy_side']:
                 available_fund = f2d(fs.available) if fs else Decimal('0.0')
             else:
                 available_fund = f2d(ff.available) if ff else Decimal('0.0')
```

### Comparing `martin-binance-1.3.0b22/martin_binance/funds_rate.db.template` & `martin-binance-1.3.0b23/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin-binance-1.3.0b23/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/margin_wrapper.py` & `martin-binance-1.3.0b23/martin_binance/margin_wrapper.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/ms_cfg.toml.template` & `martin-binance-1.3.0b23/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/service/funds_rate_exporter.py` & `martin-binance-1.3.0b23/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/service/grafana.json` & `martin-binance-1.3.0b23/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/martin_binance/service/relaunch.py` & `martin-binance-1.3.0b23/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/pyproject.toml` & `martin-binance-1.3.0b23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/uml/architecture.puml` & `martin-binance-1.3.0b23/uml/architecture.puml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b22/PKG-INFO` & `martin-binance-1.3.0b23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.0b22
+Version: 1.3.0b23
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.0b22 Summary: Free
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.0b23 Summary: Free
 trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: exchanges-wrapper==1.3.0.post1 Requires-Dist: margin-strategy-sdk==0.0.11
```

