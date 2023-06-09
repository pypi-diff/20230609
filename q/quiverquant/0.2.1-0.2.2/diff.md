# Comparing `tmp/quiverquant-0.2.1.tar.gz` & `tmp/quiverquant-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quiverquant-0.2.1.tar", last modified: Fri Jun  9 16:53:10 2023, max compression
+gzip compressed data, was "dist/quiverquant-0.2.2.tar", last modified: Fri Jun  9 16:58:05 2023, max compression
```

## Comparing `quiverquant-0.2.1.tar` & `quiverquant-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ckardatzke   (501) staff       (20)        0 2023-06-09 16:53:10.000000 quiverquant-0.2.1/
--rw-r--r--   0 ckardatzke   (501) staff       (20)     1068 2023-06-09 16:42:18.000000 quiverquant-0.2.1/LICENSE
--rw-r--r--   0 ckardatzke   (501) staff       (20)     4364 2023-06-09 16:53:10.000000 quiverquant-0.2.1/PKG-INFO
--rw-r--r--   0 ckardatzke   (501) staff       (20)     3004 2023-06-09 16:42:18.000000 quiverquant-0.2.1/README.md
-drwxr-xr-x   0 ckardatzke   (501) staff       (20)        0 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/
--rw-r--r--   0 ckardatzke   (501) staff       (20)     4364 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/PKG-INFO
--rw-r--r--   0 ckardatzke   (501) staff       (20)      215 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/SOURCES.txt
--rw-r--r--   0 ckardatzke   (501) staff       (20)        1 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/dependency_links.txt
--rw-r--r--   0 ckardatzke   (501) staff       (20)       16 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/requires.txt
--rw-r--r--   0 ckardatzke   (501) staff       (20)       12 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/top_level.txt
--rw-r--r--   0 ckardatzke   (501) staff       (20)    15959 2023-06-09 16:46:47.000000 quiverquant-0.2.1/quiverquant.py
--rw-r--r--   0 ckardatzke   (501) staff       (20)       38 2023-06-09 16:53:10.000000 quiverquant-0.2.1/setup.cfg
--rw-r--r--   0 ckardatzke   (501) staff       (20)      735 2023-06-09 16:52:49.000000 quiverquant-0.2.1/setup.py
+drwxr-xr-x   0 ckardatzke   (501) staff       (20)        0 2023-06-09 16:58:05.000000 quiverquant-0.2.2/
+-rw-r--r--   0 ckardatzke   (501) staff       (20)     1068 2023-06-09 16:42:18.000000 quiverquant-0.2.2/LICENSE
+-rw-r--r--   0 ckardatzke   (501) staff       (20)     4364 2023-06-09 16:58:05.000000 quiverquant-0.2.2/PKG-INFO
+-rw-r--r--   0 ckardatzke   (501) staff       (20)     3004 2023-06-09 16:42:18.000000 quiverquant-0.2.2/README.md
+drwxr-xr-x   0 ckardatzke   (501) staff       (20)        0 2023-06-09 16:58:05.000000 quiverquant-0.2.2/quiverquant.egg-info/
+-rw-r--r--   0 ckardatzke   (501) staff       (20)     4364 2023-06-09 16:58:05.000000 quiverquant-0.2.2/quiverquant.egg-info/PKG-INFO
+-rw-r--r--   0 ckardatzke   (501) staff       (20)      215 2023-06-09 16:58:05.000000 quiverquant-0.2.2/quiverquant.egg-info/SOURCES.txt
+-rw-r--r--   0 ckardatzke   (501) staff       (20)        1 2023-06-09 16:58:05.000000 quiverquant-0.2.2/quiverquant.egg-info/dependency_links.txt
+-rw-r--r--   0 ckardatzke   (501) staff       (20)       16 2023-06-09 16:58:05.000000 quiverquant-0.2.2/quiverquant.egg-info/requires.txt
+-rw-r--r--   0 ckardatzke   (501) staff       (20)       12 2023-06-09 16:58:05.000000 quiverquant-0.2.2/quiverquant.egg-info/top_level.txt
+-rw-r--r--   0 ckardatzke   (501) staff       (20)    18139 2023-06-09 16:57:55.000000 quiverquant-0.2.2/quiverquant.py
+-rw-r--r--   0 ckardatzke   (501) staff       (20)       38 2023-06-09 16:58:05.000000 quiverquant-0.2.2/setup.cfg
+-rw-r--r--   0 ckardatzke   (501) staff       (20)      735 2023-06-09 16:58:00.000000 quiverquant-0.2.2/setup.py
```

### Comparing `quiverquant-0.2.1/LICENSE` & `quiverquant-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quiverquant-0.2.1/PKG-INFO` & `quiverquant-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiverquant
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quiver Quantitative Alternative Data
 Home-page: https://github.com/Quiver-Quantitative/python-api
 Author: Chris Kardatzke
 Author-email: chris@quiverquant.com
 License: UNKNOWN
 Description: # Quiver Quantitative Alternative Data
         This package allows you to access several alternative data sources which are updated daily and mapped to tickers. These include:
```

### Comparing `quiverquant-0.2.1/README.md` & `quiverquant-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `quiverquant-0.2.1/quiverquant.egg-info/PKG-INFO` & `quiverquant-0.2.2/quiverquant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiverquant
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quiver Quantitative Alternative Data
 Home-page: https://github.com/Quiver-Quantitative/python-api
 Author: Chris Kardatzke
 Author-email: chris@quiverquant.com
 License: UNKNOWN
 Description: # Quiver Quantitative Alternative Data
         This package allows you to access several alternative data sources which are updated daily and mapped to tickers. These include:
```

### Comparing `quiverquant-0.2.1/quiverquant.py` & `quiverquant-0.2.2/quiverquant.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,93 +15,115 @@
         else:
             urlStart = 'https://api.quiverquant.com/beta/bulk/congresstrading'
         if politician:
             ticker = ticker.replace(" ", "%20")
             url = urlStart+"?representative="+ticker
             
         elif len(ticker)>0:
+            urlStart = 'https://api.quiverquant.com/beta/historical/congresstrading'
             url = urlStart+"/"+ticker
         else:
             url = urlStart
         print(url)
         r = requests.get(url, headers=self.headers)
         j = json.loads(r.content)
         df = pd.DataFrame(j)
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df["ReportDate"] = pd.to_datetime(df["ReportDate"])
         df["TransactionDate"] = pd.to_datetime(df["TransactionDate"])
+
         return df
    
 
     def senate_trading(self, ticker=""):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/historical/senatetrading/"+ticker
         else:
             url = "https://api.quiverquant.com/beta/live/senatetrading"
         r = requests.get(url, headers=self.headers)
         j = json.loads(r.content)
         df = pd.DataFrame(j)
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df["Date"] = pd.to_datetime(df["Date"])
         return df
 
     def house_trading(self, ticker=""):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/historical/housetrading/"+ticker
         else:
             url = "https://api.quiverquant.com/beta/live/housetrading"
         r = requests.get(url, headers=self.headers)
         j = json.loads(r.content)
         df = pd.DataFrame(j)
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df["Date"] = pd.to_datetime(df["Date"])
         return df    
     
     def offexchange(self, ticker=""):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/historical/offexchange/"+ticker
         else:
             url = "https://api.quiverquant.com/beta/live/offexchange"
         r = requests.get(url, headers=self.headers)
         j = json.loads(r.content)
         df = pd.DataFrame(j)
-        
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         if len(ticker)>0:
             df["Date"] = pd.to_datetime(df["Date"])
             
         return df
     
     def gov_contracts(self, ticker=""):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/historical/govcontractsall/"+ticker
         else:
             url = "https://api.quiverquant.com/beta/live/govcontractsall"
 
         r = requests.get(url, headers=self.headers)
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         return df
 
     
     def lobbying(self, ticker=""):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/historical/lobbying/"+ticker
         else:
             url = "https://api.quiverquant.com/beta/live/lobbying"
 
         r = requests.get(url, headers=self.headers)
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df["Date"] = pd.to_datetime(df["Date"])
         return df
         
     def insiders(self, ticker=""):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/live/insiders?ticker="+ticker
         else:
             url = "https://api.quiverquant.com/beta/live/insiders"
          
         print("Drawing from: ", url)
         r = requests.get(url, headers=self.headers)
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
        # df["Date"] = pd.to_datetime(df["Date"])
         return df     
             
             
             
     def wikipedia(self, ticker=""):
         if len(ticker)>0:
@@ -111,14 +133,17 @@
 
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         return df
     
     def wallstreetbets(self, ticker="",date_from = "", date_to = "", yesterday=False):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/historical/wallstreetbets/"+ticker
 
         else:
@@ -136,15 +161,18 @@
         print(url)
         r = requests.get(url, headers=self.headers)
 
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset.')
 
         df = pd.DataFrame(json.loads(r.content))
-
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
+        
         if not yesterday:
             try:
                 df["Date"] = pd.to_datetime(df["Time"], unit='ms')
             except:
                 df["Date"] = pd.to_datetime(df["Date"]) 
             if len(date_from)>0:
                 df = df[df["Date"]>=pd.to_datetime(date_from)]
@@ -161,42 +189,51 @@
 
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         return df 
     
     def spacs(self, ticker = ""):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/historical/spacs/"+ticker
         else:
             url = "https://api.quiverquant.com/beta/live/spacs"
 
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         return df 
     
     def flights(self, ticker = ""):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/historical/flights/"+ticker
         else:
             url = "https://api.quiverquant.com/beta/live/flights"
 
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         return df 
         
         
     def political_beta(self, ticker = ""):
         if len(ticker)>0:
             url = "https://api.quiverquant.com/beta/historical/politicalbeta/"+ticker
         else:
@@ -204,14 +241,17 @@
 
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         return df 
     
     def patents(self, ticker = ""):
         if len(ticker)<1:
             url = "https://api.quiverquant.com/beta/live/allpatents"
         else:
             url = "https://api.quiverquant.com/beta/historical/allpatents/"+ticker
@@ -219,14 +259,17 @@
         print("Pulling data from: ", url)
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset.')
         
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df["Date"] = pd.to_datetime(df["Date"])
         
         return df
     
     ## Contact chris@quiverquant.com about access to these functions
     def sec13F(self, ticker="", date="", owner="", period=""):
         separator = "?"
@@ -247,14 +290,17 @@
         print("Pulling data from: ", url)     
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df["ReportPeriod"] = pd.to_datetime(df["ReportPeriod"], unit='ms')
 #         #Can edit this out once we get past May 25th
 #         values = []
 #         for val in df["Value"]:
 #             if len(val)>=900:
 #                 values.append(val[:len(val)//1000])
 #             else:
@@ -289,14 +335,17 @@
         print("Pulling data from: ", url)     
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df["ReportPeriod"] = pd.to_datetime(df["ReportPeriod"], unit='ms')
 #         #Can edit this out once we get past May 25th
 #         values = []
 #         for val in df["Value"]:
 #             if len(val)>=900:
 #                 values.append(val[:len(val)//1000])
 #             else:
@@ -331,14 +380,17 @@
         print("Pulling data from: ", url)
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset. Contact chris@quiverquant.com with questions.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         #df['Datetime'] = pd.to_datetime(df["Time"], unit='ms')
         return df 
     
     def wallstreetbetsCommentsFull(self, ticker="", freq="", date_from = "", date_to = ""):
         separator = "?"
         url = "https://api.quiverquant.com/beta/live/wsbcommentsfull"
         if len(ticker)>0:
@@ -357,14 +409,17 @@
         print("Pulling data from: ", url)
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset. Contact chris@quiverquant.com with questions.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df['Datetime'] = pd.to_datetime(df["Time"], unit='ms')
         return df 
     
        
     def cryptoComments(self, ticker="", freq="", date_from = "", date_to = ""):
         separator = "?"
         url = "https://api.quiverquant.com/beta/live/cryptocomments"
@@ -384,14 +439,17 @@
         print("Pulling data from: ", url)
         r = requests.get(url, headers=self.headers)
         
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset. Contact chris@quiverquant.com with questions.')
             
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df['Datetime'] = pd.to_datetime(df["Time"], unit='ms')
         return df 
     
     def cryptoCommentsHistorical(self, ticker="", freq="", date_from = "", date_to = ""):
         separator = "?"
         url = "https://api.quiverquant.com/beta/live/cryptocommentsfull"
         if len(ticker)>0:
@@ -410,12 +468,12 @@
         print("Pulling data from: ", url)
         r = requests.get(url, headers=self.headers)
 
         if r.text == '"Upgrade your subscription plan to access this dataset."':
             raise NameError('Upgrade your subscription plan to access this dataset. Contact chris@quiverquant.com with questions.')
 
         df = pd.DataFrame(json.loads(r.content))
+        if (len(df)==0) or (df.shape[0]==0):
+            print("No results found")
+            return df
         df['Datetime'] = pd.to_datetime(df["Time"], unit='ms')
         return df 
-
-
-
```

### Comparing `quiverquant-0.2.1/setup.py` & `quiverquant-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quiverquant",
-    version="0.2.01",
+    version="0.2.02",
     author="Chris Kardatzke",
     author_email="chris@quiverquant.com",
     description="Quiver Quantitative Alternative Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Quiver-Quantitative/python-api",
     py_modules = ["quiverquant"],
```

