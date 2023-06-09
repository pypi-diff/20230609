# Comparing `tmp/veetility-0.1.80.tar.gz` & `tmp/veetility-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.80.tar", last modified: Fri Jun  9 17:16:21 2023, max compression
+gzip compressed data, was "veetility-0.1.9.tar", last modified: Fri Jan 27 12:16:41 2023, max compression
```

## Comparing `veetility-0.1.80.tar` & `veetility-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,14 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-09 17:16:21.559850 veetility-0.1.80/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-09 17:16:21.559701 veetility-0.1.80/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.80/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-06-09 17:16:21.559912 veetility-0.1.80/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-06-09 17:16:12.000000 veetility-0.1.80/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-09 17:16:21.554746 veetility-0.1.80/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.80/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.80/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.80/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-09 17:16:21.558578 veetility-0.1.80/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.80/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    16067 2023-06-09 17:16:03.000000 veetility-0.1.80/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.80/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1613 2023-05-18 16:58:17.000000 veetility-0.1.80/veetility/matched_qa.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.80/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    30168 2023-06-05 13:28:11.000000 veetility-0.1.80/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.80/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    53170 2023-06-05 13:25:13.000000 veetility-0.1.80/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.80/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7555 2023-06-09 16:58:39.000000 veetility-0.1.80/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-09 17:16:21.559475 veetility-0.1.80/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-09 17:16:21.000000 veetility-0.1.80/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      581 2023-06-09 17:16:21.000000 veetility-0.1.80/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-06-09 17:16:21.000000 veetility-0.1.80/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-06-09 17:16:21.000000 veetility-0.1.80/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-06-09 17:16:21.000000 veetility-0.1.80/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-27 12:16:41.142082 veetility-0.1.9/
+-rw-r--r--   0 willbutler   (502) staff       (20)      822 2023-01-27 12:16:41.141929 veetility-0.1.9/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      166 2023-01-04 11:21:38.000000 veetility-0.1.9/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-01-27 12:16:41.142139 veetility-0.1.9/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1424 2023-01-27 12:16:27.000000 veetility-0.1.9/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-27 12:16:41.140419 veetility-0.1.9/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-01-16 18:08:11.000000 veetility-0.1.9/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    32811 2023-01-27 12:11:54.000000 veetility-0.1.9/veetility/utility_functions.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-27 12:16:41.141660 veetility-0.1.9/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)      822 2023-01-27 12:16:40.000000 veetility-0.1.9/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      235 2023-01-27 12:16:41.000000 veetility-0.1.9/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-01-27 12:16:40.000000 veetility-0.1.9/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       90 2023-01-27 12:16:41.000000 veetility-0.1.9/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-01-27 12:16:41.000000 veetility-0.1.9/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.80/setup.py` & `veetility-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.80",
+    version="0.1.9",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
@@ -32,12 +32,12 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["veetility"],
     include_package_data=True,
-    install_requires=["fuzzywuzzy", 'gspread',
-                        "gspread_dataframe", "numpy",
-                        "pandas", "psycopg2-binary", "regex",
-                        "requests", "SQLAlchemy", "tqdm"]
+    install_requires=["fuzzywuzzy",'gspread',
+                        "gspread_dataframe","numpy",
+                        "pandas","psycopg2","regex",
+                        "requests","SQLAlchemy","tqdm"]
 )
```

### Comparing `veetility-0.1.80/veetility/quality_assessments.py` & `veetility-0.1.9/veetility/utility_functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,467 +1,672 @@
+import requests
+import json
 import pandas as pd
 import regex as re
 import numpy as np
-from datetime import date, datetime
+from datetime import datetime,timedelta
+import time
+from fuzzywuzzy import fuzz
 from tqdm.auto import tqdm
-import os
-import logging
+import psycopg2 as pg
 import sys
-today = pd.to_datetime(date.today())
+import logging
+import gspread
+import pickle
+import gspread_dataframe as gd
+import os
+import sqlalchemy as sa
 
-#%%-----------------------------
-# Initialise Logger
-# ------------------------------
+emoji_pattern = re.compile("["
+                           u"\U0001F600-\U0001F64F"  # emoticons
+                           u"\U0001F300-\U0001F5FF"  # symbols & pictographs
+                           u"\U0001F680-\U0001F6FF"  # transport & map symbols
+                           u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
+                           "]+", flags=re.UNICODE)
 
-logger = logging.getLogger('QAFunctions')
+logger = logging.getLogger('UtilityFunctions')
 if logger.hasHandlers():
     logger.handlers = []
 if os.path.isdir('logs') == False:
     os.mkdir('logs')
 logger.setLevel(logging.INFO)
 logger.addHandler(logging.StreamHandler(sys.stdout))
 formatter = logging.Formatter('%(levelname)s %(asctime)s - %(message)s')
 
-file_handler = logging.FileHandler(f'./logs/QAFunctions.log')
+file_handler = logging.FileHandler(f'./logs/UtilityFunctions.log')
 file_handler.setFormatter(formatter)
 logger.addHandler(file_handler)
 
-class QualityAssessments:
-
-    def __init__(self, util_object=None):
+class UtilityFunctions():
 
-        if util_object != None:
-            self.util = util_object
+    def __init__(self, gspread_auth_dict=None,db_user=None,db_password=None,db_host=None,
+                        db_port=None,db_name=None):
+        """Initialise a gspread email account from reading from a json file contaning authorisation details
+        and provide login details for a postgreSQL table
+        This means you can only connect to one google account and one database per instance 
+        of the UtilityFunctions class
+        
+        Parameters 
+        -----------------
+        gspread_filepath : str
+
+            """
+        if gspread_auth_dict != None:
+            self.sa = gspread.service_account_from_dict(gspread_auth_dict)         
+        if db_user != None:
+            self.db_user, self.db_password, self.db_host, self.db_port, self.db_name = \
+            db_user, db_password, db_host, db_port, db_name
+            postgres_str = f'postgresql://{self.db_user}:{self.db_password}@{self.db_host}:{self.db_port}/{self.db_name}'
+            self.postgresql_engine = sa.create_engine(postgres_str)
+        #if root_path != None:
+        if os.path.isdir('logs') == False:
+            os.mkdir('logs')
+        logger = logging.getLogger('UtilLog')
+        if logger.hasHandlers():
+            logger.handlers = []
+        # if os.path.isdir(f'{root_path}/logs') == False:
+        #     os.mkdir(f'{root_path}/logs')
+        logger.setLevel(logging.INFO)
+        logger.addHandler(logging.StreamHandler(sys.stdout))
+        formatter = logging.Formatter('%(levelname)s %(asctime)s - %(message)s')
+        #file_handler = logging.FileHandler(f'{root_path}/logs/UtilLog.log')
+        file_handler = logging.FileHandler(f'./logs/UtilLog.log')
+        file_handler.setFormatter(formatter)
+        logger.addHandler(file_handler)
+        self.logger = logger
     
-    def null_values_checker(self,df,cols_to_group,gsheet_name,tab_name,cols_to_ignore=None,
-                            null_definitions=[np.nan,'N/A','','None'],output_method='gsheet'):
-        """Takes in a dataframe and columns to groupby and checks how many null values or null equivalents
-        there are in the rest of the columns.
+    def prepare_string_matching(self,string, is_url=False):
+        """Prepare strings for matching say in a merge function by removing unnecessary 
+        detail, whitespaces and converting to lower case
+        Remove emojis as sometimes they can not come through properly in Tracer data
+
+        Parameters
+        -----------------
+        string : str
+            The string to be cleaned
+        is_url : bool
+            If True then remove characters after the '?' which are utm parameters
+            These can be present in some urls we recieve
+        
+        Returns
+        -----------------
+        string : The cleaned string containing no spaces, punctuation or utm parameters
+        """
+        string = string.lower()
+        if is_url:
+            # get rid of everything after they start to be utm parameters
+            string = string.split('?')[0]
+        string = emoji_pattern.sub(r'', string)
+        string = string.replace(' ', '',)
+        string = re.sub(r'[^\w\s]', '', string)
+        return string
+
+    def match_ads(self,df_1, df_2, df_1_exact_col, df_2_exact_col,
+                df_1_fuzzy_col=None, df_2_fuzzy_col=None, is_exact_col_link=True, 
+                matched_col_name='boosted', merge=False,cols_to_merge =['platform'],pickle_name='NoStore'):
+
+        """Match row items in df_2 onto row items in df_1 based on two sets of columns, first the dataframes will be tried to match
+        using the first set of columns using an exact match
+        Then for the row items that haven't matched then use the second set of columns and try to match them 
+        using fuzzy matching
+        
+        Parameters
+        -----------------
+        df_1 : DataFrame
+            The Dataframe that will be searched to see if any corresponding values in df_2, if merge=True df_2 will be left joined onto df_1
+        df_2 : df 
+            The Dataframe that if merge = True will be left joined onto df_1
+        df_1_exact_col : str
+            The Column name from df_1 that will be first attempted to find exact matches
+        df_2_exact_col : str
+            The Column name from df_2 that will be first attempted to find exact matches
+        df_1_fuzzy_col : str
+            The Column name from df_1 that will be attempted to fuzzy match if there was no exact match before
+        df_2_fuzzy_col : str
+            The Column name from df_2 that will be attempted to fuzzy match if there was no exact match before
+        is_exact_col_link : bool
+            Boolean Flag, is the set of columns to be exact matched hyperlinks? If so they will be cleaned to remove utm parameters
+        matched_col_name : str
+            String to name the column which will contain boolean values to indicate whether row items in df_1 found a match in df_2
+        merge : bool
+            Boolean Flag, if true then df_2 will be left joined onto df_1. Else df_1 will be left unchanged apart from column indicating whether there is a match
+        cols_to_merge : list, str
+            List of strings to merge on if 'merge' = True
+        pickle_name : 
+            Name of the dictionary of best matches found by fuzzy matching to be stored as a pickle file. The next time the function is 
+            run with the same pickle_name, the pickle file is used to find matches without having to do slow fuzzy matching from scratch
             
-        Args:
-            df (pandas.DataFrame): The Input Dataframe of any type where you want to check for nulls.
-            cols_to_group (list of str): The list of columns to perform a groupby operation with the null 
-                                        percentage counts will be a percentage of nulls in these groupbys.
-            cols_to_ignore (list of str): The list of columns to ignore when checking for nulls. Default is None.
-            gsheet_name (str): The name of the google sheet workbook to pass to the google sheet function.
-            tab_name (str): The name of the tab in the google sheet workbook to pass to the google sheet function.
-                                            The google sheet must be setup with this tab already created.
-            null_definitions (list): A list containing elements to be defined as a null value.
-            output_method (str): A string identifying whether the output is to be sent to a Google sheet 
-                                        ('gsheet') or returned as a dataframe ('Dataframe').
-                             
-        Returns:
-            null_count_df (pandas.DataFrame): Dataframe showing the percentage of nulls in each column grouped 
-                                           by the 'cols_to_group'."""
+        Returns
+        ----------------
+        df_1 : DataFrame
+            The original df_1 with just a column to indicate whether a match has occured if merge = False else df_1 will have df_2 left joined on
+        df_2 : DataFrame
+            The original df_2 with cleaned columns and 'Match String' column to help quality check why some rows have or haven't matched
+        df_2_no_match : DataFrame
+            A dataframe of df_2 row items that haven't found a match in df_1
+            """
+                
+        df_1_num_rows = df_1.shape[0] #Used later to check we don't lose of rows by merging
+        if df_1_fuzzy_col == None:
+            df_1_fuzzy_col = df_1_exact_col
+            df_2_fuzzy_col = df_2_exact_col
+
+        #create new columns for the columns to match on, the text in the column will get cleaned later
+        df_1_fuzzy_col_clean = df_1_fuzzy_col + '_clean'
+        df_2_fuzzy_col_clean = df_2_fuzzy_col + '_clean'
+        df_1_exact_col_clean = df_1_exact_col + '_clean'
+        df_2_exact_col_clean = df_2_exact_col + '_clean'
+
+        df_1[df_1_fuzzy_col] = df_1[df_1_fuzzy_col].astype(str)
+        df_2[df_2_fuzzy_col] = df_2[df_2_fuzzy_col].astype(str)
+        df_1[df_1_exact_col] = df_1[df_1_exact_col].astype(str)
+        df_2[df_2_exact_col] = df_2[df_2_exact_col].astype(str)
+
+        df_1['message'] = df_1['message'].replace('None','NoValuePresent') # this stops multiple none values in df_2 being written onto ever y null value in df_1
+
+        # prepare strings in a raw form with no spaces or punctuation in order to increase chance of matching
+        df_1['match_string'] = df_1[df_1_exact_col].apply(lambda x: self.prepare_string_matching(x, is_url=is_exact_col_link))
+        df_2['match_string'] = df_2[df_2_exact_col].apply(lambda x: self.prepare_string_matching(x, is_url=is_exact_col_link))
+        df_1[df_1_fuzzy_col_clean] = df_1[df_1_fuzzy_col].apply(lambda x: self.prepare_string_matching(x))
+        df_2[df_2_fuzzy_col_clean] = df_2[df_2_fuzzy_col].apply(lambda x: self.prepare_string_matching(x))
+
+        #find out the number of unique values of the first cleaned column to match by
+        df_2_unique_exact = df_2['match_string'].unique().tolist()
+        df_1_unique_exact = df_1['match_string'].unique().tolist()
+
+        #find out whether there is an exact match on the first cleaned column by using the list of unique values from df_2
+        df_1['matched_exact?'] = df_1['match_string'].apply(lambda x: True if x in df_2_unique_exact else False)
+        df_1[matched_col_name] = False
+        df_1['matched_fuzzy?'] = False
+        # Split Dataframes up into rows that had a URL match and one where the rows didn't match
+        # Then the ones that didn't match will try and be matched with the cleaned caption
+        df_1_match = df_1[df_1['matched_exact?'] == True]
+        df_1_no_match = df_1[df_1['matched_exact?'] == False]
+
+        df_1_match_rows = df_1_match.shape[0] #this is used to find out the change in the number of rows of the left df after the merge
+        cols_to_merge.append('match_string') #from the cols_to_merge specified as an input argument add the matchstring
+        if merge:
+            df_1_match = pd.merge(df_1_match, df_2.drop(df_2_fuzzy_col_clean, axis=1),
+                                left_on=cols_to_merge, right_on=cols_to_merge, how='left',indicator=True)
+            #Indicate whether a post has matched using the exact column (the first merge) if the result of the indcator is "both"
+            df_1_match['matched_exact?'] = df_1_match['_merge'].apply(lambda x: True if x == 'both' else False)
+        else:
+            df_1['matched_exact?'] = df_1['match_string'].apply(lambda x: True if x in df_2_unique_exact else False)
         
-        if cols_to_ignore == None:
-            cols_to_ignore = []
+        logger.info(f'Rows count change after df_1_match merge {df_1_match.shape[0] - df_1_match_rows}')
+        # Find the unique instances of cleaned captions to be passed to the fuzzy matching function
+        df_1_no_match_unique = df_1_no_match[df_1_fuzzy_col_clean].unique().tolist()
+        df_2_fuzzy_unique = df_2[df_2_fuzzy_col_clean].unique().tolist()
 
-        for null in null_definitions: 
-            df = df.replace(null, 'NullValue')
+        # the fuzzy match function will return a dictionary of matches for each caption from df_1 that wasn't
+        # matched by link and a list of captions from df_2 that didn't match
+        best_match_dict = self.best_fuzzy_match(df_1_no_match_unique, df_2_fuzzy_unique, 90,pickle_name)
 
-        null_count_df = pd.DataFrame(index=df[cols_to_group].value_counts().index).reset_index()
-        other_cols = list(set(df.columns) - set(cols_to_group) - set(cols_to_ignore))
-
-        for col in other_cols:
-            col_groupby = df.groupby(cols_to_group)[col].apply(lambda x: round(100 * x[x == 'NullValue'].count()/x.shape[0],1)).reset_index()
-            null_count_df = pd.merge(null_count_df, col_groupby)
-
-        if output_method == 'gsheet':
-            self.util.write_to_gsheet(gsheet_name, tab_name, null_count_df)
-        elif output_method == 'Dataframe': 
-            return null_count_df
-    
-    def check_data_recency(self, df, cols_to_group, gsheet_name, tab_name='DataRecency',
-                            three_days_for_monday= True, date_col='date',
-                            dayfirst='EnterValue', yearfirst='EnterValue', format=None, errors='raise'):
-        """Post a google sheet showing how many days since different channels have been active.
-        Also return a list of channels that have been inactive for more than 2 days which
-        might be indicative of an error
-        
-        Args:
-            df (pandas.DataFrame): Dataframe of data containing a 'date' column
-            cols_to_group (list or str): Columns to groupby effectively creating the 'channels'
-            gsheet_name (str): Name of the google sheet to write to
-            tab_name (str): Name of the tab in the Google sheet
-            three_days_for_monday (bool): If the check is run on a Monday, give 3 days before declaring a channel as inactive because of the weekend.
-            date_col (str): Column name for the date to find the maximum value for based on grouping by `cols_to_group`. If 'created' is used when working with Tracer data, then this will find out when the data was last updated by Tracer, regardless of whether the actual date of the post was 30 days ago.
-            dayfirst (bool): If True, parses dates with the day first, eg 10/11/12 is parsed as 2012-11-10. If False, parses dates with the month first, eg 10/11/12 is parsed as 2010-11-12. If None, this is set to True if the day is in the first position in the format string, False otherwise. If dayfirst is set to True, parsing will be faster, but will fail for ambiguous dates, such as 01/02/03.
-            yearfirst (bool): If True parses dates with the year first, eg 10/11/12 is parsed as 2010-11-12. If both dayfirst and yearfirst are True, yearfirst is preceded (same as dateutil). If False, parses dates with the month first, eg 10/11/12 is parsed as 2012-11-10. If None, this defaults to False. Setting yearfirst to True is not recommended, as it can result in ambiguous dates.
-            format (str): Format to use for strptime. If None, the format is inferred from the first non-NaN element of the column. If the format is inferred, it will be used in subsequent parsing, even if the format changes. To specify a format string that will be used in parsing regardless of the inferred format, use pd.to_datetime with format.
-            errors (str): If 'raise', then invalid parsing will raise an exception. If 'coerce', then invalid parsing will be set as NaT. If 'ignore', then invalid parsing will return the input.
+        # create a column that is the closest match in df_2 for every caption in df_1
+        # This will be used to merge df_2 onto the remainder of none matching df_1
+        df_1_no_match['match_string'] = df_1_no_match[df_1_fuzzy_col_clean].map(best_match_dict)
 
-        Returns:
-            error_message (str): String error message describing which channels are recently inactive. This message can then be sent
-                                to a slack function"""
+        df_1_no_match['match_string'].fillna(False, inplace=True)
+        #Idnetify whether a post has matched using the fuzzy matching function by whether there is a value there
+        df_1_no_match['matched_fuzzy?'] = df_1_no_match['match_string'].apply(lambda x: False if ((x == 'None') or (x == '')) else True)
+        df_2['match_string'] = df_2.apply(lambda x: x['match_string'] if x['match_string'] in df_1_unique_exact else x[df_2_fuzzy_col_clean], axis=1)
 
-        error_message = ''
-        organic_or_paid = self.util.identify_paid_or_organic(df)
-        print(organic_or_paid)
-        buffer_days_since_active = 2
-        #remove any timezone information from the date_col and check the date is being read in in correct format
-        df[date_col] = pd.to_datetime(df[date_col].dt.date, dayfirst=dayfirst,
-                                      yearfirst=yearfirst, format=format, errors=errors)
-
-        data_recency = pd.DataFrame(df.groupby(cols_to_group)[date_col].max().apply(lambda x: (today - x).days)).reset_index().rename(columns={date_col:'DaysSinceActive'})  
-    
-        self.util.write_to_gsheet(gsheet_name, tab_name, data_recency, sheet_prefix=organic_or_paid)
-
-        #create a tag string to identify a channel, a concatenation of all the column values specified in 'cols_to_group'
-        def concat_cols(x):
-            result = ''
-            for col in cols_to_group:
-                result += x[col] + '-'
-            return result.rstrip('-')
-            
-        data_recency['Channel'] = data_recency.apply(lambda x: concat_cols(x),axis=1)
+        #Now try and merge the rows that didn't match on the exact column
+        df_1_no_match_num_rows = df_1_no_match.shape[0]
+        if merge:
+            df_1_no_match = pd.merge(df_1_no_match, df_2.drop(df_2_fuzzy_col, axis=1), left_on=cols_to_merge,
+                                    right_on=cols_to_merge, how='left',indicator=True)
+        
+            df_1_no_match['matched_fuzzy?'] = df_1_no_match['_merge'].apply(lambda x: True if x == 'both' else False)
+        
 
-        #The option for giving 3 days of buffer for monday is available in case no advertising/posting is done 
-        #over the weekend and you don't want many channels appearing as if they are inactive on Monday morning
-        if today.day_of_week == 0 and three_days_for_monday: 
-            buffer_days_since_active = 3
-
-        channels_recently_inactive = data_recency.query(f'DaysSinceActive >{buffer_days_since_active} and DaysSinceActive <=6')
-        channels_recently_inactive_list = channels_recently_inactive['Channel'].unique().tolist()
-        if len(channels_recently_inactive_list) != 0:
-            error_message = f'{organic_or_paid} Channels Recently that are recently inactive {" , ".join(channels_recently_inactive_list)}\n'
+        logger.info(f'Rows Lost after no match merge {df_1_no_match_num_rows - df_1_no_match.shape[0]}')
 
-        return error_message
-    
-    def boosted_function_qa(self, paid_df, organic_df, gsheet_name, tab_name='OrganicWithBigImpressions', impressions_threshold=100000):
-        """Takes in organic data and paid data and reports how many are mislabelled as boosted
-            
-        Args:
-            paid_df (pandas.DataFrame): Daily ad spend, boosted posts identified in the 'workstream' column
-            organic_df (pandas.DataFrame): Organic Post performance Data 
-            impressions_threshold (pandas.DataFrame): The number of impressions above which it is unlikely the post is purely organic
-            
-        Returns:
-            error_message (str): A string detailing what the error is so that it can be passed to a notification service like slack"""
-        error_message = ''
-        organic_df['Error'] = False
+        df_1 = pd.concat([df_1_match, df_1_no_match], ignore_index=True)
 
-        # count number of unique paid posts wi  th workstream organic minus oranic posts labelled as boosted
-        # number of boosted post from paid naming convention Tags
-        paid_boosted_count = len(paid_df[paid_df['workstream'] == 'boosted']['post_id'].unique())
-
-        # number of posts our boosted matching function has identified as boosted
-        organic_boosted_count = len(organic_df[organic_df['workstream'] == 'boosted']['post_id'].unique())
-        missing_boosted = paid_boosted_count-organic_boosted_count
-
-        if (missing_boosted) != 0:
-            error_message = error_message + '  ' + \
-                f'There are {missing_boosted}({round(missing_boosted*100/paid_boosted_count, 2)}%) posts mislabelled as Pure Organic\n'
-            logger.warning(error_message)
-
-        # A post that is labelled as organic but has impressions over the impressions_threshold may actually be boosted 
-        # but hasn't been identified as such
-        misslabelled_og_rows = organic_df[(organic_df['workstream'] == 'Pure Organic') & \
-                                        ((organic_df['impressions'] >= impressions_threshold) | \
-                                        (organic_df['video_views'] >= impressions_threshold))]
-
-        if len(misslabelled_og_rows.index.values) > 0:
-            error_message = error_message + '  ' + \
-                f'There are {len(misslabelled_og_rows.index.values)} Pure Organic posts with over {impressions_threshold} impressions or video views\n'
-            logger.warning(error_message)
-            self.util.write_to_gsheet(gsheet_name, tab_name, misslabelled_og_rows)
-        # return TT or IG values with empty message field
-        # for the date function exlude the dates we paused for the queen
+        df_1[matched_col_name] = df_1.apply(lambda x: True if ((x['matched_exact?'] == True) or (x['matched_fuzzy?'] == True)) else False, axis=1)
 
-        logger.warning(error_message)
-        return error_message
-    
-    def comparison_with_previous_data(self, df, name_of_df, cols_to_check=['impressions','likes'], perc_increase_threshold=20,
-                                   perc_decrease_threshold=0.5, check_cols_set=True, raise_exceptions=False):
-        """ This function stores the high level sums for a datatable from the previous run of the script
-        and if they have reduced or increased too sharply an error is raised.
-
-        A JSON file is created which stores historical data about the dataframe, the columns present and the
-        sum of the columns specified in cols_to_check. This can then be used for reference purposes to see if any changes in the totals are
-        caused by code changes or errors. 
-
-        Args:
-            df (pd.DataFrame): Input dataframe that the historic checks are going to be performed on.
-            name_of_df (str): Name of the dataframe, this will be used to name a file to save for future comparison.
-            cols_to_check (List[str]): A list of strings that detail the columns to be totaled which will then 
-                be compared with previous data.
-            perc_increase_threshold (float): A number between 0 and 100, the percentage increase threshold above 
-                which it is deemed that the totals have raised too rapidly and an error has occured.
-            perc_decrease_threshold (float): A number between 0 and 100, the percentage decrease threshold below 
-                which it is deemed that the totals decreased and an error has occured.
-            check_cols_set (bool): If true, store the set of columns present for comparison to see if any new 
-                columns have been added or removed next time, in which case it is deemed an error has occured.
-            raise_exceptions (bool): If true, then raise an exception if an error has occured instead of just returning an error message.
+        df_2_no_match = df_2[~df_2['match_string'].isin(df_1['match_string'].unique().tolist())]
 
-        Returns:
-            error_message (str): String detailing what the error is so that it can be passed to a notification service like slack."""
-        
-        error_message, error_occured = '', False
-        new_dict = {}
-        new_dict['datetime'] = str(datetime.now())
-        for col in cols_to_check:
-            new_dict[col] = int(df[col].sum())
-
-        if check_cols_set == True:
-            new_dict['Columns'] = df.columns.tolist()
-
-        if os.path.isdir('Historic df Comparison (Do Not Delete)') == False:
-            os.mkdir('Historic df Comparison (Do Not Delete)')
-        if os.path.exists(f'Historic df Comparison (Do Not Delete)/{name_of_df}_previous_totals.json') ==False:
-            self.util.write_json(new_dict, f'{name_of_df}_previous_totals', file_type='append', folder='Historic df Comparison (Do Not Delete)/')
-            logger.info(f"Creation of {name_of_df}_previous_totals")
-            logger.info(new_dict)
-            return error_message
-        else:
-            #old_dict = self.util.unpickle_data(f'{name_of_df}_previous_totals', folder='Historic df Comparison (Do Not Delete)')
-            old_dict_file = self.util.read_json(f'{name_of_df}_previous_totals', folder='Historic df Comparison (Do Not Delete)',
-                                                    file_type='append')
-            old_dict = old_dict_file[-1] # Grab the lastest entry in the json file, descending date order
-        
-        for key, value in old_dict.items():
-            if key == 'Columns':
-                if set(value) != set(new_dict['Columns']):
-                    error_occured = True
-                    columns_removed = list(set(value) - set(new_dict['Columns']))
-                    columns_added = list(set(new_dict['Columns']) - set(value))
-                    error_message = error_message + '  ' + f'The columns seems to have changed from last time,\n'\
-                                            f' Columns that were added = {columns_added}\n' \
-                                            f' Columns that were removed = {columns_removed}\n'
-            elif key == 'datetime':
-                continue
-            elif new_dict[key] *(1+perc_decrease_threshold/100) < value:
-                error_occured = True
-                error_message = error_message + '  ' + f'The total of {key} seems to have decreased from last time\n'\
-                                        f' Prev Value = {old_dict[key]} , New Value = {new_dict[key]}\n'
-            elif new_dict[key] > value*(1 +perc_increase_threshold/100):
-                error_occured = True
-                error_message = error_message + '  ' + f'The total of {key} has increased by more than\n'\
-                                    f'{perc_increase_threshold}% from last time\n'\
-                                        f' Prev Value = {old_dict[key]}, New Value = {new_dict[key]}\n'
-
-        if error_occured:
-            error_message = f'Comparison with historic df {name_of_df}: ' + error_message +'\n'
-            logger.info('ERROR' + error_message) # If error messages has been added to then log it
-        if raise_exceptions and error_occured:
-            raise Exception(error_message)
-        #self.util.pickle_data(new_dict, f'{name_of_df}_previous_totals', folder='Historic df Comparison (Do Not Delete)/')
-        self.util.write_json(new_dict, f'{name_of_df}_previous_totals', file_type='append',
-                             folder='Historic df Comparison (Do Not Delete)/')
-        
-        return error_message
-    
-    def duplicates_qa(self, df: pd.DataFrame, df_name: str, subset= None, drop_duplicates: bool = True):
-        """Checks for duplicates and optionally drops duplicates in a dataframe.
-        
-        Args:
-            df (pd.DataFrame): The Dataframe to be checked for duplicates
-            df_name (str): The name of the dataframe to be used for logging purposes
-            subset (Optional[Union[list, str]], optional): Only consider certain columns for identifying duplicates, by default use all of the columns
-            drop_duplicates (bool, optional): If true remove duplicate values
-            
-        Returns:
-            df (pd.DataFrame): Returns original dataframe without duplicates if 'drop_duplicates' = True"""
+        logger.info(f'df_1 row numbers change = {df_1_num_rows - df_1.shape[0]}')
 
-        num_duplicates = df.duplicated(subset=subset).sum()
-        if num_duplicates >= 0:
-            logger.warning(f'{num_duplicates} duplicates found in the {df_name}. Subset = {subset}')
-            if drop_duplicates:
-                df.drop_duplicates(subset=subset, inplace=True)
-        return df
-    
-    def duplicates_qa_plus(self, df, name_of_df, perc_dupes_thresh=3, cols_to_check=None, 
-                        cols_to_add=None, return_type='duplicates', raise_exceptions=True):
-        """Checks for duplicates in a dataframe and returns the duplicates or the dataframe without duplicates.
+        logger.info(f"Num unique exact col values in df_1: {df_1[df_1_exact_col].nunique()},\
+                Num unique fuzzy col values in df_1: {df_1[df_1_fuzzy_col].nunique()}")
+        logger.info(f"Num unique exact col values in df_2: {df_2[df_2_exact_col].nunique()},\
+                Num unique fuzzy col values in df_2: {df_2[df_2_fuzzy_col].nunique()}")
 
-        The function first checks to see whether the input dataframe is paid or organic data. If it is paid data then the columns to check for duplicates are
-        ['date','platform','country','media_type','cohort','message','ad_name','spend'].
+        logger.info(f"Num Matched df_1 exact col ={df_1['matched_exact?'].sum()}")
+        logger.info(f"Num Matched df_1 fuzzy col ={df_1['matched_fuzzy?'].sum()}")
+        logger.info(f"Num df_2 exact that didn't match= {df_2_no_match[df_2_exact_col].nunique()}")
 
-        For organic data the standard columns it will check for are ['platform', 'country','media_type' ,'message','url']
+        matched_df_1_nunique = df_1[df_1[matched_col_name]==True].drop_duplicates(subset=cols_to_merge).shape[0]
+        logger.info(f"Number of df_1 that have matched = {matched_df_1_nunique}")
+        num_df_2_to_match = df_2.drop_duplicates(subset=cols_to_merge).shape[0]
+        logger.info(f"Number of df_2 that need to match {num_df_2_to_match}")
+        logger.info(f"Percentage of df_2 that were matched = {round((matched_df_1_nunique * 100)/num_df_2_to_match,2)}")
 
-        You can specify other columns to check for duplicates by passing a list to the cols_to_check argument. You can also add to the standard columns by passing
-        a list to the cols_to_add argument.
+        return df_1, df_2, df_2_no_match
 
-        You can specify whether to return the original dataframe with duplicates removed or just the duplicates by passing 'duplicates' or 'duplicates_removed' to the
-        return_type argument.
+    def best_fuzzy_match(self,list_1, list_2, threshold, pickle_name):
+        """Takes in two lists of strings and every string in list_1 is fuzzy matched onto every item in list_2
+        The fuzzy match of a string in list_1 with a string in list_2 with the highest score will count as the 
+        match as long as it is above the threshold. The match is then stored as a key value pair in a dictionary
 
-        If the return type is duplicates_removed, an error message will also be returned, with the error message being blank if no duplicates are found. This can be passed
-        to a notification function for example.
+        The dictionary of matches will be saved as a pickle file to be used next time the function is run to save
+        having to do searches on a string if we've already found a match in the past
 
-        
-        Args:
-            df (pd.DataFrame): The Dataframe to be checked for duplicates
-            name_of_df (str): The name of the dataframe to be used for logging purposes
-            perc_dupes_thresh (int, optional): The percentage of duplicates that are allowed before an error is raised. Defaults to 3.
-            cols_to_check (Optional[list], optional): The columns to check for duplicates. Defaults to None.
-            cols_to_add (Optional[list], optional): The columns to add to the standard cols_to_check to duplicates check. Defaults to None.
-            return_type (str, optional): The type of return. Either 'duplicates' or 'duplicates_removed'. Defaults to 'duplicates'.
-            raise_exceptions (bool, optional): If true raise an exception if duplicates are found. Defaults to True.
-        
-        Raises:
-            Exception: If raise_exceptions = True and duplicates are found
+        Paramaters
+        -------------------
+        list_1 : list
+            First List of strings, every item will be searched for a fuzzy match in list_2
+        list_2 : list
+            Second List of strings, every item in list_1 will be fuzzy matched with every item in list 2 and best fuzzy match score wins
+        threshold : integer between 0 and 100
+            value between 0 and 100 signifying percentage fuzzy match score at which a match is considered sufficiently close
+        pickle_name : str 
+            name of pickle_file to create or add to if a pickle of the dictionary already exists
         
         Returns:
-            pd.DataFrame: Returns the duplicates or the dataframe without duplicates depending on the return_type"""
-
-        num_rows = len(df)
-        logger.info(f'Num of rows in {name_of_df} = {num_rows}')
-        paid_or_organic = self.util.identify_paid_or_organic(df)
-        
-        if cols_to_check == None:
-            if paid_or_organic == 'Paid':
-                #Include date in paid duplicate check because the same ad is repeated across consequitve days
-                #Spend is a good indicator of duplicates in paid data
-                cols_to_check = ['date', 'platform', 'country', 'media_type', 'cohort', 'message', 'ad_name', 'spend']
-                
-            elif paid_or_organic == 'Organic':
-                cols_to_check = ['platform', 'country', 'media_type' , 'message', 'url']
-                if 'date_row_added' in df.columns:
-                    cols_to_check.append('date_row_added')
-        
-        if cols_to_add != None:
-            cols_to_check = cols_to_check + cols_to_add
-        
-        for i in range(2, len(cols_to_check)+1):
-            num_duplicates = df.duplicated(subset=cols_to_check[:i]).sum()
-            logger.info(f'{num_duplicates} - {name_of_df} - {cols_to_check[:i]}')
+        best_match_dict : Dictionary
+            Dictionary of matches (with highest fuzzy match score) between strings in list_1 and list_2 
+            key = string in list_1, value = string in list_2 """
+
+        best_match_dict = {} 
+        stored_best_dict = {} #
+        if pickle_name != 'NoStore':
+            if os.path.isfile(f'Pickled Files/best_match_dict_{pickle_name}'):
+                stored_best_dict = self.unpickle_data(f'best_match_dict_{pickle_name}')
+                logger.info(f"loaded dict of len :{len(stored_best_dict)}")
+
+        for string_1 in tqdm(list_1):
+            temp_match_dict = {}
+            # If there is an exact match then just put the match as itself and no need to go through list
+            if string_1 in list_2:  
+                best_match_dict[string_1] = string_1
+                continue
+            
+            #If there is a match in the stored dictionary then use that
+            if string_1 in list(stored_best_dict.keys()): 
+                best_match_dict[string_1] = stored_best_dict[string_1]
+                continue
+            
+            #Then go through every string in the second list and fuzzy match to produce a score
+            #If the score is below the threshold then set the score to 0
+            #start = time.time()
+            for string_2 in list_2:
+                score = fuzz.ratio(string_1, string_2)
+                if score < threshold:
+                    score = 0
+                temp_match_dict[string_2] = score
+            # end = time.time()
+            # logger.info(end - start)
+            
+            #if there were no matches above the threshold then return a match for that 
+            #string in list_1 equal to "none"
+            if max(temp_match_dict.values()) == 0:
+                best_match_dict[string_1] = 'None'
+            else:
+                # find the match with the highest matching score and save that to the
+                # best match dictionary
+                best_match = max(temp_match_dict.items(), key=lambda k: k[1])[0]
+                best_match_dict[string_1] = best_match
+
+        if pickle_name!= 'NoStore':
+            # Remove matches that didn't find anythign as that will let new values be discovered
+            # if new data comes in
+            #best_match_dict_none_removed = {k:v for k,v in best_match_dict.items() if v != 'None'}
+            self.pickle_data(best_match_dict,f'best_match_dict_{pickle_name}')
+
+        return best_match_dict
+
+    def write_to_postgresql(self,df,table_name, if_exists='replace'):
+        """Writes a dataframe to a PostgreSQL database table using a SQLalchemy engine defined elsewhere.
+        If writing fails it waits 10 seconds then trys again
+            
+        Paramaters
+        --------------
+        df : DataFrame
+            The Dataframe to send to the PostGreSQL table
+        table_name : str
+            The name of the table to write the dataframe to
+        if_exists : str
+            Either 'replace' or 'append' which describes what to do if a table with
+            that name already exists
+                                    
+        Returns
+        --------------
+        error_message : str
+            An error message saying that the connection has failed """
+        # create a SQL alchemy engine to write the data to the database after cleaning
         
-        perc_dupes = df.duplicated(subset=cols_to_check).sum()*100 / num_rows
-        exceed_thresh = perc_dupes > perc_dupes_thresh
+        error_message = ''
+        try:
+            now = time.time()
+            df.to_sql(table_name, con=self.postgresql_engine, index=False, if_exists=if_exists)
+            time_taken = round(time.time() - now,2)
+            logger.info(f"Time Taken to write {table_name} = {time_taken}secs")
+            logger.info(f"Sent Data to {table_name}")
+        except ConnectionError as error_message:
+            logger.info(f"Connection error {error_message}")
+            time.sleep(10) # wait for 10 seconds then try again
+            try:
+                now = time.time()
+                df.to_sql(table_name, con=self.postgresql_engine, index=False, if_exists=if_exists)
+                time_taken = round(time.time() - now,2)
+                logger.info(f"Time Taken to write {table_name} = {time_taken}secs")
+            except Exception as error_message:
+                logger.error(f'Connection failed again {error_message}',exc_info=True)
+                return f'{table_name} error: ' + error_message
+        return error_message
+    
+    def table_exists(self,table_name):
+        """Determine whether a table called 'table_name' exists"""
+        all_table_names = sa.inspect(self.postgresql_engine).get_table_names()
+        return (table_name in all_table_names)
+    
+    def store_daily_organic_data(self,df,output_table_name,num_days_to_store=30,date_column_name='date',
+                                    check_created_col=True,created_col='created',refresh_lag=1):
+        """Takes in an organic data table with each row item reflecting an organic post with the metric totals
+        updating and increasing in the same row item each day rather than creating a new row item each day.
+        Returns an organic table which has a row item  
+            
+        Parameters
+        ----------------
+        df : DataFrame
+            The Dataframe source of organic data
+        output_table : str
+            The name of the output table to write the data to
+        num_days_to_store : integer
+            The number of days to look back
+        date_column_name : str
+            The name of the column which contains the date that the post was originally posted
+        check_created_col : bool
+            If true then we should check whether the created column in Tracer is up to date, because 
+            there is no point sending a days worth of data if the row items have not been refreshed
+        created_col : str
+            The name of the column in the dataset which indicates the date that it was last updated
+        Returns
+        ----------------
+        df : DataFrame
+            Outputs a table to the 'output_table_name', appends if already exists or creates from scratch if not"""
+        today_datetime = datetime.today()
+        today_date = today_datetime.date() 
+        if today_datetime.hour < 15: #Before 3 o'clock in the afternoon
+            logger.info("It may be better to run the API later on in the day to make sure the USA data has had time to refresh")
+        #Check Tracer data has actually updated
+        if self.table_exists(output_table_name):
+
+            old_df = self.read_from_postgresql(output_table_name)
+            if old_df['date_updated'].max().date() == today_date:
+                logger.info(f"It looks data has already pushed to {output_table_name} today")
+            else:
+                if (df[created_col].max().date() < today_date - timedelta(days=refresh_lag)) and (check_created_col):
+                    error_message = "It looks like the input df has not been updated yesterday. Therefore there is no fresh data to add on."
+                    logger.info(error_message)
+                    raise Exception(error_message)
+                cutoff_date = today_date - timedelta(days=num_days_to_store)
+                #create temporary date column that you can change the date format, that you then delete so it doesn't affect original date format
+                df['datetemp'] = pd.to_datetime(df[date_column_name]).dt.date
+                df = df[df['datetemp']>=(cutoff_date)]#filter data only after the cutoff date
+                df['date_updated'] = today_datetime
+                df = df.drop(columns=['datetemp']) #drop temporary date column used for filtering dates
+                self.write_to_postgresql(df,output_table_name,if_exists='append')
+        else: #if the table doesn't exist create it with the whole dataset for the first time
+            df['date_updated'] = today_datetime
+            self.write_to_postgresql(df,output_table_name,if_exists='replace')
+
+
+    def read_from_postgresql(self,table_name,clean_date=True,date_col='EnterValue',
+                                dayfirst='EnterValue',yearfirst='EnterValue',format=None,errors='raise'):
+        """Reads a table from a PostgreSQL database table using a pscopg2 connection.
+            If fails it waits 10 seconds and tries again"""
+        conn = pg.connect(dbname=self.db_name, host=self.db_host,
+                    port=self.db_port, user=self.db_user, password=self.db_password)
+        try:
+            now = time.time()
+            df = pd.read_sql_query(f"SELECT * FROM {table_name}", conn)
+            time_taken = round(time.time() - now,2)
+            logger.info(f"Time Taken to read {table_name} = {time_taken}secs")
+
+        except Exception as error_message:
+            logger.error(f"Read {table_name} error: {error_message}",exc_info=True)
+            time.sleep(10)
+        
+            now = time.time()
+            df = pd.read_sql_query(f"SELECT * FROM {table_name}", conn)
+            time_taken = round(time.time() - now,2)
+            logger.info(f"Time Taken to read {table_name} = {time_taken}secs")
+
+        conn.close()
+        if clean_date:
+            df[date_col] = pd.to_datetime(df[date_col],dayfirst=dayfirst,yearfirst=yearfirst,
+                                        format=format,errors=errors)
+        return df
 
-        logger.info(f'% Dupes of whole subset - {name_of_df} = {perc_dupes}')
+    def write_to_gsheet(self,workbook_name, sheet_name, df, if_exists='replace', sheet_prefix=''):
+        """Write dataframe to google sheet
 
-        if exceed_thresh:
-            error_message = f'% Dupes in {name_of_df} exceeds {perc_dupes_thresh}%'
+        Parameters
+        ----------
+        workbook_name : str
+            The name of the google sheet workbook.
+        sheet_name : str
+            The name of the sheet to write data to.
+        df : pandas.DataFrame
+            The dataframe to be written to the google sheet.
+        if_exists : str, optional (default='replace')
+            Determines the behavior when the sheet already exists, options are 'replace' or 'append'.
+        sheet_prefix : str, optional (default='')
+            A prefix to be added to the sheet name.
+
+        Returns
+        -------
+        None"""
+        now = datetime.now()
+        dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
+        df['SheetUpdated'] = dt_string
+        try:
+            # Adding the sheet prefix to the sheet name
+            sheet_name = sheet_prefix + sheet_name
+            # Open the worksheet
+            sheet = self.sa.open(workbook_name).worksheet(sheet_name)
+            if if_exists == 'replace': 
+                # Clear the sheet if if_exists is set to 'replace'
+                sheet.clear()
+            now = time.time()
+            # Write the dataframe to the sheet
+            gd.set_with_dataframe(sheet, df)
+            time_taken = round(time.time() - now,2)
+            logger.info(f"Time Taken to write to google sheet {sheet_name} = {time_taken}secs")
+        except Exception as error_message:
+            logger.error(error_message,exc_info=True)
+            time.sleep(10)
+            gd.set_with_dataframe(sheet, df)
+
+
+    def read_from_gsheet(self,workbook_name, sheet_name,clean_date=True,date_col='EnterValue',
+                            dayfirst='EnterValue',yearfirst='EnterValue',format=None,errors='raise'):
+        try:
+            spreadsheet = self.sa.open(workbook_name)
+        except Exception as error_message:
+            logger.info(error_message)
+            time.sleep(10)
+            spreadsheet = self.sa.open(workbook_name)
+        worksheet = spreadsheet.worksheet(sheet_name)
+        df = pd.DataFrame(worksheet.get_all_records())
+        if clean_date:
+            df[date_col] = pd.to_datetime(df[date_col],dayfirst=dayfirst,yearfirst=yearfirst,
+                                        format=format,errors=errors)
+        return df
+    
+    def identify_paid_or_organic(self,df):
+        """Identify whether a given dataframe contains paid data"""
+        paid_or_organic = 'Organic'
+        #make columns to check lower case so can work on
+        # columns that have or haven't been cleaned
+        col_list = [x.lower() for x in df.columns]
+        if 'spend' in col_list:
+            paid_or_organic = 'Paid'
+        return paid_or_organic
+
+    def pickle_data(self,data, filename,folder="Pickled Files"):
+        if os.path.isdir(folder) == False:
+            os.mkdir(folder)
+        pickle.dump(data, open(folder + '/' + filename, "wb"))
+    
+    def unpickle_data(self,filename,folder ="Pickled Files"):
+        return pickle.load(open(folder + '/' + filename, "rb"))
+    
+    def write_json(self,object,file_name,file_type):
+        if file_type == 'DataFrame':
+            object.to_json(file_name+'.json',orient='split')
+        elif file_type == 'List' or file_type == 'Dictionary':
+            with open(f"{file_name}.json","w") as outfile:
+                json.dump(object,outfile)
         else:
-            error_message = ''
-
-        if raise_exceptions and exceed_thresh:
-            raise Exception(error_message)
-        
-        elif return_type == 'duplicates': 
-            return df[df.duplicated(subset=cols_to_check, keep=False)].sort_values(by=cols_to_check)
-
-        elif return_type == 'duplicates_removed':
-            return df.drop_duplicates(subset=cols_to_check, inplace=False), error_message
-
+            logger.error('JSON write error, file_type error')
     
-    def check_impressions_no_engagements(self, df, gsheet_name, tab_name='NoImpressionsButEngagements', raise_exceptions=False):
-        """Function to check if a row item has engagements but no impressions and no video views. 
-        This shouldn't happen and is indicative of an error with Tracer but can be valid as some 
-        platforms count viral engagements differently.
-
-        Args:
-            df (DataFrame): Input dataframe of advertising data with columns 'impressions' or 'video_views'
-            gsheet_name (str): name of the google sheet
-            tab_name (str, optional): name of the tab. Defaults to 'NoImpressionsButEngagements'.
-            raise_exceptions (bool, optional): Boolean flag if set to true will raise an exception if an offending row item is discovered. Defaults to False.
+    def read_json(self,file_name, file_type):
+        if file_type == 'DataFrame':
+            return pd.read_json(f'{file_name}.json',orient='split')
+        elif file_type == 'List' or file_type == 'Dictionary':
+            return json.load(open(f'{file_name}.json'))
+        else:
+            logger.error('JSON read error, file_type error')
 
-        Returns:
-            error_message (str): String detailing what the error is so that it can be passed to a notification service like slack."""
+    def remove_vvm_stage(self,creative_name):
+        creative_name = re.sub(r'Level 2 - ','', creative_name)
+        creative_name = re.sub(r'Level2 -','', creative_name)
+        creative_name = re.sub(r'Level_2-','', creative_name)
+        creative_name = re.sub(r'Level2_','', creative_name)
+        return creative_name
+
+    def calc_tiktok_vtr_rates(self,df):
+        df['Engagements'] = df['likes'] + df['comments'] + df['shares']
+        df['EngagementRate'] = round(
+            df['Engagements'] * 100 / df['impressions'], 2)
+        df['25%VTR'] = round(df['Video Views P 25'] * 100 / df['impressions'], 2)
+        df['50%VTR'] = round(df['Video Views P 50'] * 100 / df['impressions'], 2)
+        df['75%VTR'] = round(df['Video Views P 75'] * 100 / df['impressions'], 2)
+        df['100%VTR'] = round(df['Video Completions'] * 100 / df['impressions'], 2)
+        return df
+    
+    def columnnames_to_lowercase(self,df):
+        df.columns = df.columns.str.lower()
+        df.columns = df.columns.str.replace(' ','_')
+        df.columns = df.columns.str.strip()
+        return df
 
-        paid_or_organic = self.util.identify_paid_or_organic(df)
-        # https://docs.google.com/spreadsheets/d/1refbPLje6B48qvSRNXrK3U_OAfzjzeuTrzgfqq9O-yw/edit#gid=0
-        df['date'] = pd.to_datetime(df['date'])
-        error_message = f'{paid_or_organic} Data Quality Check Function Failed'
-        engagements_cols = ['likes', 'comments', 'shares']
-        engagements_mask = ((df[engagements_cols] != 0).any(1))
-        # Check for zeros in impression columns but non zeros in likes, impressions, and other metrics
-        no_impr_but_engage = list(df[(df['impressions'] == 0) & engagements_mask].index.values)
-
-        # TikTok organic doesn't have impressions, instead it has video views. There is an error if
-        # Video views is equal to zero but there are engagements
-        tiktok_org_no_impr_but_engage = list(df[((df['platform'] == 'TikTok') & (df['workstream'] == 'boosted') &
-                                                (df['video_views'] == 0) & engagements_mask)].index.values)
-
-        reels_org_no_impr_but_engage = list(df[((df['placement'] == 'Reels') & (df['workstream'] == 'boosted') &
-                                                (df['video_views'] == 0) & engagements_mask)].index.values)
-
-        # paid with  impressions but has engagements
-        no_impressions_but_engage_rows = set(no_impr_but_engage + tiktok_org_no_impr_but_engage 
-                                            + reels_org_no_impr_but_engage)
-
-        if len(no_impressions_but_engage_rows) > 0:
-            error_message = error_message + '  ' + f'There are {len(no_impressions_but_engage_rows)} rows with'\
-                ' zeros in impressions columns but non-zeros in likes, comments, shares and video_views\n'
-
-            df.loc[no_impressions_but_engage_rows, 'Error'] = True
-            # error_message = error_message + " " + "Split By platform"
-            # error_message = error_message + " " + pd.crosstab(erroneous_df['platform'],erroneous_df['media_type'],margins=True,dropna=False)
-            self.util.write_to_gsheet(gsheet_name, tab_name, df.loc[no_impressions_but_engage_rows],
-                            sheet_prefix=paid_or_organic)
-            exception_occurred = True
-
-        logger.warning(error_message)
-        if raise_exceptions and exception_occurred:
-            raise Exception(error_message)
-        
-        return error_message
 
-    def naming_convention_checker(self, df, gsheet_name, naming_convention, campaignname_dict=None, adgroupname_dict=None, 
-                                    adname_dict=None, campaign_col='campaign_name', adgroup_col='group_name', adname_col='name',
-                                    start_char='_', middle_char=':', end_char='_'):
-        """Checks for naming convention errors in a given DataFrame and outputs the errors to a Google Sheet.
-
-        The function takes in a DataFrame containing paid data with columns for campaign name, ad group name, and ad name, 
-        as well as a DataFrame containing the accepted tags and values for each level of naming (campaign, ad group, ad name). 
-        Dictionarys for each level fo checking are required this specifies what tags should be checked for, e.g. should a check
-        for the correct values in 'platform' be performed. If a dictionary for a certain level is not provided that level will
-        not be checked. The function will output a table in a Google Sheet showing all errors in naming conventions, 
-        with a tab for each level of errors.
-
-        The Google Sheet should be set up with a tab name for each level of errors to check for, 
-        i.e. 'CampaignNameErrors', 'AdGroupNameErrors', 'AdNameErrors'.
-
-        Args:
-            df (DataFrame): The DataFrame containing paid data with campaign name, ad group name, and ad name columns.
-            naming_convention (DataFrame): The DataFrame containing the accepted tags and values for each level of naming.
-            campaignname_dict (dict, optional): A dictionary of the tags to be checked for the campaign name, with the column label as the key and the shortcode as the value.
-            adgroupname_dict (dict, optional): A dictionary of the tags to be checked for the ad group name, with the column label as the key and the shortcode as the value.
-            adname_dict (dict, optional): A dictionary of the tags to be checked for the ad name, with the column label as the key and the shortcode as the value.
-            campaign_col (str, optional): The column in the input DataFrame that corresponds to the campaign name. Defaults to 'campaign_name'.
-            adgroup_col (str, optional): The column in the input DataFrame that corresponds to the ad group name. Defaults to 'group_name'.
-            adname_col (str, optional): The column in the input DataFrame that corresponds to the ad name. Defaults to 'name'.
-            start_char (str, optional): The starting character for the tag in the naming convention. Defaults to '_'.
-            middle_char (str, optional): The character that separates the tag from the value in the naming convention. Defaults to ':'.
-            end_char (str, optional): The ending character for the tag in the naming convention. Defaults to '_'.
+    def group_by_asset(self,x):
+        d = {}
 
-        Returns:
-            Writes to a Google Sheet a table with the index being a unique instance of the campaign."""
-        
-        conv_level_tuple = ((campaignname_dict, campaign_col, 'CampaignNameErrors'), (adgroupname_dict, adgroup_col, 'AdGroupNameErrors'),
-                            (adname_dict, adname_col, 'AdNameErrors'))
-        # df = clean.clean_column_names(df)
-        #Obtain the column names of all the Keys available in the convention tracker sheet
-        #https://docs.google.com/spreadsheets/d/1Wtwd6xT9zRLhPICWSWDNZ2mXBy74_xszLVX2ZqO_odo/edit#gid=605935420
-        key_values_conv_cols = [x.replace(' Key', '') for x in naming_convention.columns if ' Key' in x]
-
-        def remove_empties_from_list(input_list):
-            '''Obtaining a list of keys from the tracker sheet column often results in multiple empty
-                strings, this function removes them from the list'''
-            return list(filter(lambda x: x != '', input_list))
-
-        def return_value(string, tag, acceptable_values):
-            """This checks for each campaign, group_name or ad_name string, for a certain tag e.g.'pl'
-            whether the tag is even present and if so whether a correct value is present"""
-            search_string = f'{start_char}{tag}{middle_char}(.*?){end_char}'
-            search_result = re.search(search_string, string + '_') #add a underscore at so search string has an endpoint to find
-            if search_result == None:
-                return 'NoKey'
-            elif search_result.group(1).strip(' ') == '':
-                return 'NoKey'
-            else:
-                if search_result.group(1).upper() in acceptable_values:
-                    return "Correct"
-                else:
-                    return 'Incorrect Value'
-
-        for level in conv_level_tuple:
-            #For each level of the naming convention, i.e. campaign, adgroup, adname
-            output_df = round(df.groupby(level[1])['spend'].sum().reset_index(),1)
-            if level[0] == None: continue #no convention dict provided therefore ignore
-            for label,tag in level[0].items():
-                #For each label and tag in the required set 
-                if label in key_values_conv_cols:
-                    acceptable_values= remove_empties_from_list(naming_convention[label+' Key'].str.upper().unique().tolist())
-                    output_df[f'{label} ("{tag}")'] = output_df[level[1]].apply(lambda x: return_value(x, tag, acceptable_values))
-            self.util.write_to_gsheet(workbook_name = gsheet_name, sheet_name= level[2], df = output_df)
+        d['Engagements'] = x['Engagements'].sum()
+        d['impressions'] = x['impressions'].sum()
+        d['EngagementRate'] = round(d['Engagements'] * 100 / d['impressions'], 2)
+        d['25%VTR'] = round(x['25%VTR'].mean(), 2)
+        d['50%VTR'] = round(x['50%VTR'].mean(), 2)
+        d['75%VTR'] = round(x['75%VTR'].mean(), 2)
+        d['100%VTR'] = round(x['100%VTR'].mean(), 2)
+        d['Video Length'] = round(x['Video Length'].iloc[0], 2)
+
+        return pd.Series(d, index=list(d.keys()))
+class Logger:
+
+    def __init__(self,name_of_log):
+        self.name_of_log = name_of_log
+        logger = logging.getLogger(__name__)
+        if logger.hasHandlers():
+            logger.handlers = []
+        if os.path.isdir('logs') == False:
+            os.mkdir('logs')
+        logger.setLevel(logging.INFO)
+        logger.addHandler(logging.StreamHandler(sys.stdout))
+        formatter = logging.Formatter('%(levelname)s %(asctime)s - %(message)s')
+
+        file_handler = logging.FileHandler(f'./logs/{name_of_log}.log')
+        file_handler.setFormatter(formatter)
+        logger.addHandler(file_handler)
+        self.logger = logger
+        
+
+class SlackNotifier:
+    """A class that notifies slack given a webhook
+        """
+
+    def __init__(self, slack_webhook_url: str, title = "Update" ,link_1 = '', link_1_name='No Url',
+                    link_2 ='', link_2_name = 'No Url', link_3 = '', link_3_name = 'No Url',
+                    link_4='', link_4_name='No Url'):
     
+        self.slack_webhook_url, self.title = slack_webhook_url, title
+        self.link_1,self.link_2,self.link_3,self.link_4 = link_1,link_2,link_3,link_4
+        self.link_1_name,self.link_2_name,self.link_3_name,self.link_4_name = link_1_name,link_2_name,link_3_name,link_4_name
+        
+    def send_slack_message(self, message:str):
+        payload = {
+        "blocks":
+        [
+            {
+                  "type": "header",
+                  "text": {
+                      "type": "plain_text",
+                      "text": f"{self.title}",
+                        }
+            },
+
+            {
+                  "type": "divider"
+            },
+
+            {
+                  "type": "section",
+                  "fields": [
+                      {
+                          "type": "mrkdwn",
+                          "text": message
+                      },
+
+                    ],
+            },
+
+            {
+                  "type": "divider"
+            },
+
+            {
+                  "type": "section",
+                  "text": {
+                      "type": "mrkdwn",
+                      "text": f"<{self.link_1}|{self.link_1_name}>"
+                  }
+            },
+
+            {
+                  "type": "section",
+                  "text": {
+                      "type": "mrkdwn",
+                      "text": f"<{self.link_2}|View {self.link_2_name}>"
+                        }
+            },
+
+            {
+                  "type": "section",
+                  "text": {
+                      "type": "mrkdwn",
+                      "text": f"<{self.link_3}|View {self.link_3_name}>"
+                        }
+            },
+
+            {
+                  "type": "section",
+                  "text": {
+                      "type": "mrkdwn",
+                      "text": f"<{self.link_4}|View {self.link_4_name}>"
+                        }
+            },
+
+        ]
+        }
+        try:
+            requests.post(self.slack_webhook_url, data=json.dumps(payload))
+        except Exception as e:
+            logger.error(f"Failed To Send Slack messafe {e}",exc_info=True)
```

