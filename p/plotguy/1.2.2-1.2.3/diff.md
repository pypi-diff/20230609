# Comparing `tmp/plotguy-1.2.2.tar.gz` & `tmp/plotguy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.2.2.tar", last modified: Wed Jun  7 04:53:31 2023, max compression
+gzip compressed data, was "plotguy-1.2.3.tar", last modified: Fri Jun  9 03:04:52 2023, max compression
```

## Comparing `plotguy-1.2.2.tar` & `plotguy-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:53:31.418426 plotguy-1.2.2/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-07 04:53:31.418259 plotguy-1.2.2/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.2/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:53:31.417334 plotguy-1.2.2/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    25831 2023-06-07 04:50:28.000000 plotguy-1.2.2/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16884 2023-05-22 09:16:53.000000 plotguy-1.2.2/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    65949 2023-06-07 04:51:18.000000 plotguy-1.2.2/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    38123 2023-06-06 21:38:06.000000 plotguy-1.2.2/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.2.2/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:53:31.418063 plotguy-1.2.2/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-07 04:53:31.418477 plotguy-1.2.2/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-07 04:53:23.000000 plotguy-1.2.2/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-09 03:04:52.730259 plotguy-1.2.3/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-09 03:04:52.730090 plotguy-1.2.3/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.3/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-09 03:04:52.729066 plotguy-1.2.3/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    25651 2023-06-09 02:59:05.000000 plotguy-1.2.3/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16885 2023-06-09 02:59:56.000000 plotguy-1.2.3/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    65962 2023-06-09 02:59:05.000000 plotguy-1.2.3/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    38129 2023-06-09 02:59:05.000000 plotguy-1.2.3/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.2.3/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-09 03:04:52.729898 plotguy-1.2.3/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-09 03:04:52.730313 plotguy-1.2.3/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-09 03:04:10.000000 plotguy-1.2.3/setup.py
```

### Comparing `plotguy-1.2.2/plotguy/__init__.py` & `plotguy-1.2.3/plotguy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 
     for year in year_list:
         win_rate_dict[year] = calculate_win_rate_info(df.loc[df['year'] == year])
 
     return win_rate_dict
 
 
-def calculate_sharp_ratio(df, col, risk_free_rate):
+def calculate_sharpe_ratio(df, col, risk_free_rate):
     holding_period_day = (df.loc[df.index[-1], 'date'] - df.loc[df.index[0], 'date']).days
     net_profit = df.at[df.index[-1], col] - df.at[df.index[0], col]
 
     initial_capital = df.loc[df.index[0], col]
 
     # To avoid power error below
     if net_profit < 0 and abs(net_profit) > initial_capital:
@@ -527,28 +527,29 @@
         result_dict['annualized_sr'] = 0
         result_dict['mdd_dollar'] = 0
         result_dict['mdd_pct'] = 0
         result_dict['num_of_trade'] = 0
         result_dict['win_rate'] = 0
         result_dict['loss_rate'] = 0
         result_dict['net_profit_to_mdd'] = np.inf
-        result_dict['cov'] = 0
+        result_dict['cov_count'] = 0
+        result_dict['cov_return'] = 0
 
         # Win rate by year
         for year in year_list:
             result_dict[str(year)] = 0
             result_dict[f'{year}_win_rate'] = '--'
             result_dict[f'{year}_return'] = 0
 
     else:
         df['date'] = pd.to_datetime(df['date'], format='%Y-%m-%d')
         df['year'] = pd.DatetimeIndex(df['date']).year
 
         # Strategy Performance
-        net_profit, holding_period_day, return_on_capital, annualized_return, annualized_std, annualized_sr = calculate_sharp_ratio(
+        net_profit, holding_period_day, return_on_capital, annualized_return, annualized_std, annualized_sr = calculate_sharpe_ratio(
             df, 'equity_value', risk_free_rate)
         mdd_pct, mdd_dollar = calculate_mdd(df, 'equity_value')
         mdd_pct = mdd_pct * -100
         mdd_dollar = mdd_dollar * -1
 
         # Win Rate (need to use df_backtest directly)
 
@@ -579,37 +580,33 @@
         result_dict['loss_rate'] = loss_rate
 
         if mdd_dollar == 0:
             result_dict['net_profit_to_mdd'] = np.inf
         else:
             result_dict['net_profit_to_mdd'] = net_profit / mdd_dollar
 
-        # Cov
-        # df3 = df[df['action'] == 'open']
-        df3 = df[df['action'].notnull()]
-        df3 = df3.set_index('date')
-        signal_year_count = df3.groupby(lambda x: x.year).size()
-
-        signal_year_std = np.std(signal_year_count)
-        signal_year_mean = np.mean(signal_year_count)
-        cov = round(signal_year_std / signal_year_mean, 3)
 
-        result_dict['cov_count'] = cov
-
-        # Win rate by year
+        # Count and Win rate by year
+        year_count = []
         for year in year_list:
             try:
                 result_dict[str(year)] = win_rate_dict[year][0]
                 result_dict[f'{year}_win_rate'] = win_rate_dict[year][3]
 
             except Exception as e:
                 # print(e)
                 result_dict[str(year)] = 0
                 result_dict[f'{year}_win_rate'] = '--'
 
+            year_count.append(result_dict[str(year)])
+
+
+        result_dict['cov_count'] = round(np.std(year_count) / np.mean(year_count), 3)
+
+
         # Performance by year
         first_equity_value = 0
         last_equity_value = 0
         year_return_list = []
         for year in year_list:
             if not df.loc[df['year'] == year].empty:  # if trade
                 if first_equity_value == 0:  # if 1st year, set beginning as the first equity_value
@@ -638,15 +635,15 @@
             cov_return = round(return_year_std / return_year_mean, 3)
         result_dict['cov_return'] = cov_return
 
     result_dict['risk_free_rate'] = risk_free_rate
 
     # BaH Performance
     bah_net_return, holding_period_day, bah_return, \
-    bah_annualized_return, bah_annualized_std, bah_annualized_sr = calculate_sharp_ratio(df, 'close',
+    bah_annualized_return, bah_annualized_std, bah_annualized_sr = calculate_sharpe_ratio(df, 'close',
                                                                                          risk_free_rate)
     initial_capital = df.loc[df.index[0], 'equity_value']
     df['bah_equity_curve'] = df['close'] * initial_capital // df.loc[df.index[0], 'close']
     bah_mdd_pct, bah_mdd_dollar = calculate_mdd(df, 'bah_equity_curve')
     bah_mdd_pct = bah_mdd_pct * -100
     bah_mdd_dollar = bah_mdd_dollar * -1
```

### Comparing `plotguy-1.2.2/plotguy/aggregate.py` & `plotguy-1.2.3/plotguy/aggregate.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
                     d['initial_capital'] = d['initial_capital'] / (initial_capital / 100000)
                     d['net_profit'] = d['net_profit'] / (initial_capital / 100000)
                     d['total_commission'] = d['total_commission'] / (initial_capital / 100000)
                 d.pop('net_profit_to_mdd')
                 d.pop('mdd_dollar')
                 d.pop('mdd_pct')
                 d.pop('return_on_capital')
-                d.pop('sharp_ratio')
+                d.pop('sharpe_ratio')
                 dicts.append(d.copy())
 
             df_performance = pd.DataFrame.from_dict(dicts)
 
             total_dict = {}
             for element in df_performance.columns:
                 total_dict[element] = df_performance[element].sum()
```

### Comparing `plotguy-1.2.2/plotguy/components.py` & `plotguy-1.2.3/plotguy/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
                                                        {'label': 'Exclude Stock', 'value': 'exclude'},
                                                        {'label': 'Return on Capital >', 'value': 'return_on_capital>'},
                                                        {'label': 'Return on Capital <', 'value': 'return_on_capital<'},
                                                        {'label': 'Annualized Return >', 'value': 'annualized_return>'},
                                                        {'label': 'Annualized Return <', 'value': 'annualized_return<'},
                                                        {'label': 'Return-BaH % Diff. >', 'value': 'return_to_bah>'},
                                                        {'label': 'Return-BaH % Diff. <', 'value': 'return_to_bah<'},
-                                                       {'label': 'Sharp Ratio >', 'value': 'annualized_sr>'},
-                                                       {'label': 'Sharp Ratio <', 'value': 'annualized_sr<'},
+                                                       {'label': 'Sharpe Ratio >', 'value': 'annualized_sr>'},
+                                                       {'label': 'Sharpe Ratio <', 'value': 'annualized_sr<'},
                                                        {'label': 'MDD Percentage >', 'value': 'mdd_pct>'},
                                                        {'label': 'MDD Percentage <', 'value': 'mdd_pct<'},
                                                        {'label': 'Trade Count >', 'value': 'num_of_trade>'},
                                                        {'label': 'Trade Count <', 'value': 'num_of_trade<'},
                                                        {'label': 'COV (Count) >', 'value': 'cov_count>'},
                                                        {'label': 'COV (Count) <', 'value': 'cov_count<'},
                                                        {'label': 'COV (Return) >', 'value': 'cov_return>'},
@@ -74,15 +74,15 @@
     def __init__(self,number_of_curves):
         self.sort_method_dropdown = html.Div(
             dbc.Select(id='sort_method',
                        placeholder="Select Sorting Method",
                        value=f'Top Net Profit',
                        options=[{'label': f'Top {number_of_curves} Net Profit', 'value': 'Top Net Profit'},
                                 {'label': f'Top {number_of_curves} Return-BaH % Difference', 'value': 'Top Return to BaH Ratio'},
-                                {'label': f'Top {number_of_curves} Sharp Ratio', 'value': 'Top Sharp Ratio'}, ],
+                                {'label': f'Top {number_of_curves} Sharpe Ratio', 'value': 'Top Sharpe Ratio'}, ],
                        style={'border-radius': '5px', 'font-size': '12px', }),
             style={'padding-left': '15px', 'width': '235px'})
 
 
     def empty_line_chart(self):
         chart_bg = self.chart_bg
         fig_line = px.line()
@@ -288,15 +288,15 @@
         per_col_1_1.append(html.Div('COV (Return)'))
         per_col_1_1.append(html.Div('Total Commission'))
         per_col_1_1.append(html.Div('Risk Free Rate'))
 
         per_col_2_1.append(html.Div('Return on Capital'))
         per_col_2_1.append(html.Div('Ann. Return'))
         per_col_2_1.append(html.Div('Ann. Std'))
-        per_col_2_1.append(html.Div('Ann. Sharp Ratio'))
+        per_col_2_1.append(html.Div('Ann. Sharpe Ratio'))
         per_col_2_1.append(html.Div('MDD Dollar'))
         per_col_2_1.append(html.Div('MDD Percentage'))
 
         for i in range(8):
             per_col_1_2.append(html.Div(df[keys[i]], style={'text-align': 'center'}))
         try:
             per_col_1_2.append(html.Div( "{:.2%}".format(risk_free_rate / 100) , style={'text-align': 'center'}))
@@ -400,15 +400,15 @@
         return matrix_div
 
 
     filter_options = {
         'num_of_trade':'Trade Count',
         'return_on_capital': 'Return on Capital',
         'annualized_return': 'Annualized Return',
-        'annualized_sr': 'Sharp Ratio',
+        'annualized_sr': 'Sharpe Ratio',
         'mdd_pct':'MDD Percentage',
         'cov_count':'COV (Count)',
         'cov_return': 'COV (Return)',
         'win_rate':'Win Rate',
         'return_to_bah': 'Return/BnH % Diff.',
         'exclude': 'Exclude',
         }
@@ -435,15 +435,15 @@
 
         return filter_button
 
 
     def sort_method_df(self, sort_method, result_df, number_of_curves):
         if sort_method == 'Top Net Profit':
             df_sorted = result_df.sort_values(by='net_profit', ascending=False).head(number_of_curves).copy()
-        elif sort_method == 'Top Sharp Ratio':
+        elif sort_method == 'Top Sharpe Ratio':
             df_sorted = result_df.sort_values(by='annualized_sr', ascending=False).head(number_of_curves).copy()
         elif sort_method == 'Top Return to BaH Ratio':
             df_sorted = result_df.sort_values(by='return_to_bah', ascending=False).head(number_of_curves).copy()
         else:
             df_sorted = result_df.copy()
 
         df_sorted = df_sorted.reset_index(drop=True)
@@ -606,15 +606,15 @@
 
 
             hovertemplate = hovertemplate + "<br>"
 
 
             hovertemplate = hovertemplate + "Return on Capital : " + "{:.0%}".format(graph_df.iloc[i]['return_on_capital']/100) + "<br>"
             hovertemplate = hovertemplate + "Annual Return : " + "{:.0%}".format(graph_df.iloc[i]['annualized_return'] / 100) + "<br>"
-            hovertemplate = hovertemplate + "Sharp Ratio : " + str(graph_df.iloc[i]['annualized_sr']) + "<br>"
+            hovertemplate = hovertemplate + "Sharpe Ratio : " + str(graph_df.iloc[i]['annualized_sr']) + "<br>"
             hovertemplate = hovertemplate + "MDD Percentage : " + "{:.0%}".format(graph_df.iloc[i]['mdd_pct'] / 100) + "<br>"
 
             hovertemplate = hovertemplate + "<br>"
 
             # para_combination for save_path generation
             reference_index = graph_df.iloc[i].reference_index
             para_combination = df_all_para_combination.loc[df_all_para_combination['reference_index'] == reference_index].to_dict('records')[0]
@@ -1097,15 +1097,15 @@
                     'net_profit': row['net_profit'],
                     'mdd_dollar': row['mdd_dollar'],
                     'mdd_pct': row['mdd_pct'],
                     'num_of_trade': row['num_of_trade'],
                     'num_of_win': row['num_of_win'],
                     'return_on_capital': row['return_on_capital'],
                     'total_commission': row['total_commission'],
-                    'sharp_ratio': row['sharp'],
+                    'sharpe_ratio': row['sharpe'],
                 }
                 dict['format'] = file_format
                 dict['ref'] = ref_code
 
 
                 start_date_year = datetime.datetime.strptime(parameters['startdate'], '%Y%m%d').year
                 end_date_year = datetime.datetime.strptime(parameters['enddate'], '%Y%m%d').year
@@ -1275,15 +1275,15 @@
         net_profit = "{:,}".format(int(round(total_dict['net_profit'],0)) )
         net_profit_to_mdd = round(total_dict['net_profit_to_mdd'],2)
         try:
             win_rate = "{:.0%}".format( float(total_dict['win_rate']) )
         except:
             win_rate = '--'
 
-        # Sharp Ratio
+        # Sharpe Ratio
         annualized_std = total_dict['annualized_std']
         annualized_return = total_dict['annualized_return']
 
         if isinstance(risk_free_rate, str):
             try:
                 if risk_free_rate == 'geometric_mean':
                     start_date_year = year_list[0]
@@ -1331,14 +1331,15 @@
 
             try:
                 year_return_list.append(float(year_return))
             except:
                 year_return_list.append(0)
 
         cov_count = round(np.std(year_count) / np.mean(year_count), 2)
+
         if np.mean(year_return_list) == 0:
             cov_return = 0
         else:
             cov_return = round(np.std(year_return_list) / np.mean(year_return_list), 2)
 
         div = html.Div([
 
@@ -1355,15 +1356,15 @@
                          html.Div('COV (Return)'),
                          html.Div('Total Commission'),
                          html.Div('Risk Free Rate'),
                          html.Div(style={'height': '10px'}),
                          html.Div('Return on Capital'),
                          html.Div('Ann. Return'),
                          html.Div('Ann. Std'),
-                         html.Div('Ann. Sharp Ratio'),
+                         html.Div('Ann. Sharpe Ratio'),
                          html.Div('MDD Dollar'),
                          html.Div('MDD Percentage')
                          ],
                         style={'padding-left':'13px'},
                         width=7),
                 dbc.Col([html.Div(num_of_trade),
                          html.Div(net_profit),
```

### Comparing `plotguy-1.2.2/plotguy/equity_curves.py` & `plotguy-1.2.3/plotguy/equity_curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,29 @@
     chart_type = 1
     relayoutData = []
     init = True
     save_path = ''
     initial_capital = 0
     return_in_capital = 0
     mdd = 0
-    sharp = 0
+    sharpe = 0
 
     start_date_datetime = 0
     end_date_datetime = 0
 
     para_combination = {}
     save_path = 'save_path'
     net_profit_to_mdd = 0
     net_profit = 0
     mdd_dollar = 0
     mdd_pct = 0
     num_of_trade = 0
     num_of_win = 0
     return_on_capital = 0
-    sharp = 0
+    sharpe = 0
     total_commission = 0
     year_list = []
     year_count = []
     year_win_count = []
 
 
     def __new__(self, all_para_combination, result_df, settings, number_of_curves):
@@ -605,15 +605,15 @@
                     self.mdd_pct = df['mdd_pct']
                     self.num_of_trade = df['num_of_trade']
                     try:
                         self.num_of_win = round(int(df['num_of_trade'])*float(df['win_rate'])/100)
                     except:
                         self.num_of_win = '--'
                     self.return_on_capital = df['return_on_capital']
-                    self.sharp = df['annualized_sr']
+                    self.sharpe = df['annualized_sr']
                     self.total_commission = df['total_commission']
                     self.total_commission = df['total_commission']
                     year_count = []
                     year_win_count = []
                     for year in self.year_list:
                         if not df[f'{year}_win_rate'] == '--':
                             win_count = round(int(df[str(year)])*float(df[f'{year}_win_rate'])/100)
@@ -634,15 +634,15 @@
             Output('save_button', "style"),
             Input('save_button', "n_clicks"),
         )
         def save_button(save_clicks):
             if not os.path.isfile('saved_strategies.csv'):
                 columns = ['path','initial','net_profit_to_mdd','net_profit',
                                       'mdd_dollar','mdd_pct','num_of_trade','num_of_win',
-                                      'return_on_capital','total_commission','sharp'
+                                      'return_on_capital','total_commission','sharpe'
                                       ]
                 for year in self.year_list:
                     columns.append(year)
                     columns.append(f'{year}_win_count')
                 columns.append('para_combination')
                 pd.DataFrame(columns=columns).to_csv('saved_strategies.csv', index=False)
             else:
@@ -698,15 +698,15 @@
                                            'net_profit_to_mdd': self.net_profit_to_mdd,
                                            'net_profit': self.net_profit,
                                            'mdd_dollar':self.mdd_dollar,
                                            'mdd_pct':self.mdd_pct,
                                            'num_of_trade':self.num_of_trade,
                                            'num_of_win': self.num_of_win,
                                            'return_on_capital': self.return_on_capital,
-                                           'sharp': self.sharp,
+                                           'sharpe': self.sharpe,
                                            'total_commission': self.total_commission,
                                            }
                                 for i, year in enumerate(self.year_list):
                                     df_dict[str(year)] = self.year_count[i]
                                     df_dict[f'{year}_win_count'] = self.year_win_count[i]
 
                                 saved_df = pd.concat([saved_df, pd.DataFrame(df_dict,index=[10])],
```

### Comparing `plotguy-1.2.2/plotguy/signals.py` & `plotguy-1.2.3/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.2/setup.py` & `plotguy-1.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.2.2",
+    version="1.2.3",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',
```

