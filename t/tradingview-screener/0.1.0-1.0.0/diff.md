# Comparing `tmp/tradingview_screener-0.1.0.tar.gz` & `tmp/tradingview_screener-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingview_screener-0.1.0.tar", max compression
+gzip compressed data, was "tradingview_screener-1.0.0.tar", max compression
```

## Comparing `tradingview_screener-0.1.0.tar` & `tradingview_screener-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-03-09 22:58:53.153717 tradingview_screener-0.1.0/LICENSE
--rw-r--r--   0        0        0      474 2023-04-25 15:57:55.400009 tradingview_screener-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7233 2023-04-25 15:33:55.393746 tradingview_screener-0.1.0/README.md
--rw-r--r--   0        0        0      104 2023-04-25 15:09:19.384141 tradingview_screener-0.1.0/tradingview_screener/__init__.py
--rw-r--r--   0        0        0    16703 2023-04-25 15:10:38.040451 tradingview_screener-0.1.0/tradingview_screener/screener.py
--rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 tradingview_screener-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-03-09 22:58:53.153717 tradingview_screener-1.0.0/LICENSE
+-rw-r--r--   0        0        0      972 2023-06-09 06:58:04.567288 tradingview_screener-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    16020 2023-04-30 17:05:47.164356 tradingview_screener-1.0.0/README.md
+-rw-r--r--   0        0        0      138 2023-04-26 22:23:30.233994 tradingview_screener-1.0.0/tradingview_screener/__init__.py
+-rw-r--r--   0        0        0     5218 2023-06-09 07:05:40.082819 tradingview_screener-1.0.0/tradingview_screener/query.py
+-rw-r--r--   0        0        0    16921 2023-04-30 15:08:06.151572 tradingview_screener-1.0.0/tradingview_screener/screener.py
+-rw-r--r--   0        0        0    16776 1970-01-01 00:00:00.000000 tradingview_screener-1.0.0/setup.py
+-rw-r--r--   0        0        0    16585 1970-01-01 00:00:00.000000 tradingview_screener-1.0.0/PKG-INFO
```

### Comparing `tradingview_screener-0.1.0/LICENSE` & `tradingview_screener-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tradingview_screener-0.1.0/tradingview_screener/screener.py` & `tradingview_screener-1.0.0/tradingview_screener/screener.py`

 * *Files 5% similar despite different names*

```diff
@@ -277,24 +277,27 @@
     'Volume Weighted Average Price': 'VWAP',
     'Volume Weighted Moving Average (20)': 'VWMA',
     'Volume*Price': 'Value.Traded',
     'Weekly Performance': 'Perf.W',
     'Williams Percent Range (14)': 'W.R',
     'Yearly Performance': 'Perf.Y',
     'YTD Performance': 'Perf.YTD',
+    'type': 'type',
+    'subtype': 'subtype',
+    'name': 'name',
+    'logoid': 'logoid',
 }  # TODO: test all columns
 API_SETTINGS = {
     'filter': [{'left': 'type', 'operation': 'equal', 'right': 'stock'},
                {'left': 'subtype', 'operation': 'in_range', 'right': ['common', 'foreign-issuer']},
                {'left': 'exchange', 'operation': 'in_range', 'right': ['AMEX', 'NASDAQ', 'NYSE']}],
-    'options': {'active_symbols_only': True, 'lang': 'en'},
+    'options': {'lang': 'en'},
     'markets': ['america'],
     'symbols': {'query': {'types': []}, 'tickers': []},
     'columns': ['name', 'close', 'volume', 'market_cap_basic'],
-    # TODO: change the default columns
     # 'sort': {},  # the sortBy value should be replaced with a column name
     'range': [0, 50]
 }
 
 
 class Scanner(dict, Enum):
     premarket_gainers = {'sortBy': 'premarket_change', 'sortOrder': 'desc'}
@@ -310,32 +313,37 @@
     def names(cls) -> list[str]:
         return [x.name for x in cls]
 
     def get_data(self, **kwargs) -> pd.DataFrame:
         cols = API_SETTINGS['columns'].copy()
         cols.insert(1, self.value['sortBy'])  # insert the column that we are sorting by, right after the symbol column
         kwargs.setdefault('columns', cols)  # use `setdefault()` so the user can override this
-        return get_scanner_data(sort=self.value, **kwargs)
+        return get_scanner_data(sort=self.value, **kwargs)[1]
 
 
-def get_scanner_data(**kwargs) -> pd.DataFrame:
+def get_scanner_data(**kwargs) -> tuple[int, pd.DataFrame]:
     """
     Get a dataframe with the scanner data directly from the API
 
     :param kwargs: kwargs to override fields in the `local_settings` dictionary
     :return: Pandas DataFrame
     """
     local_settings = API_SETTINGS.copy()  # copy() to avoid modifying the global settings
     local_settings.update(**kwargs)
 
     r = requests.post(URL, headers=HEADERS, data=json.dumps(local_settings))
     r.raise_for_status()
 
-    data = r.json()['data']
-    return pd.DataFrame(data=(row['d'] for row in data), columns=local_settings['columns'])
+    json_obj = r.json()
+    rows_count = json_obj['totalCount']
+    data = json_obj['data']
+
+    if data is None:
+        return rows_count, pd.DataFrame(columns=local_settings['columns'])
+    return rows_count, pd.DataFrame(data=(row['d'] for row in data), columns=local_settings['columns'])
 
 
 def get_all_symbols(exchanges: Iterable[str] = ('AMEX', 'OTC', 'NYSE', 'NASDAQ')) -> list[str]:
     """
     Get a list with all the symbols filtered by a given exchange.
 
     Valid exchanges: {'AMEX', 'OTC', 'NYSE', 'NASDAQ'}
```

