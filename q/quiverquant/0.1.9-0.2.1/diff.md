# Comparing `tmp/quiverquant-0.1.9.tar.gz` & `tmp/quiverquant-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quiverquant-0.1.9.tar", last modified: Tue Feb  2 18:02:07 2021, max compression
+gzip compressed data, was "dist/quiverquant-0.2.1.tar", last modified: Fri Jun  9 16:53:10 2023, max compression
```

## Comparing `quiverquant-0.1.9.tar` & `quiverquant-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 ckardatzke   (501) staff       (20)        0 2021-02-02 18:02:07.000000 quiverquant-0.1.9/
--rw-r--r--   0 ckardatzke   (501) staff       (20)     3015 2021-02-02 18:02:07.000000 quiverquant-0.1.9/PKG-INFO
--rw-r--r--   0 ckardatzke   (501) staff       (20)     1975 2021-01-03 00:53:15.000000 quiverquant-0.1.9/README.md
-drwxr-xr-x   0 ckardatzke   (501) staff       (20)        0 2021-02-02 18:02:07.000000 quiverquant-0.1.9/quiverquant.egg-info/
--rw-r--r--   0 ckardatzke   (501) staff       (20)     3015 2021-02-02 18:02:07.000000 quiverquant-0.1.9/quiverquant.egg-info/PKG-INFO
--rw-r--r--   0 ckardatzke   (501) staff       (20)      207 2021-02-02 18:02:07.000000 quiverquant-0.1.9/quiverquant.egg-info/SOURCES.txt
--rw-r--r--   0 ckardatzke   (501) staff       (20)        1 2021-02-02 18:02:07.000000 quiverquant-0.1.9/quiverquant.egg-info/dependency_links.txt
--rw-r--r--   0 ckardatzke   (501) staff       (20)       16 2021-02-02 18:02:07.000000 quiverquant-0.1.9/quiverquant.egg-info/requires.txt
--rw-r--r--   0 ckardatzke   (501) staff       (20)       12 2021-02-02 18:02:07.000000 quiverquant-0.1.9/quiverquant.egg-info/top_level.txt
--rw-r--r--   0 ckardatzke   (501) staff       (20)     4093 2021-02-02 18:00:50.000000 quiverquant-0.1.9/quiverquant.py
--rw-r--r--   0 ckardatzke   (501) staff       (20)       38 2021-02-02 18:02:07.000000 quiverquant-0.1.9/setup.cfg
--rw-r--r--   0 ckardatzke   (501) staff       (20)      733 2021-02-02 18:01:51.000000 quiverquant-0.1.9/setup.py
+drwxr-xr-x   0 ckardatzke   (501) staff       (20)        0 2023-06-09 16:53:10.000000 quiverquant-0.2.1/
+-rw-r--r--   0 ckardatzke   (501) staff       (20)     1068 2023-06-09 16:42:18.000000 quiverquant-0.2.1/LICENSE
+-rw-r--r--   0 ckardatzke   (501) staff       (20)     4364 2023-06-09 16:53:10.000000 quiverquant-0.2.1/PKG-INFO
+-rw-r--r--   0 ckardatzke   (501) staff       (20)     3004 2023-06-09 16:42:18.000000 quiverquant-0.2.1/README.md
+drwxr-xr-x   0 ckardatzke   (501) staff       (20)        0 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/
+-rw-r--r--   0 ckardatzke   (501) staff       (20)     4364 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/PKG-INFO
+-rw-r--r--   0 ckardatzke   (501) staff       (20)      215 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/SOURCES.txt
+-rw-r--r--   0 ckardatzke   (501) staff       (20)        1 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/dependency_links.txt
+-rw-r--r--   0 ckardatzke   (501) staff       (20)       16 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/requires.txt
+-rw-r--r--   0 ckardatzke   (501) staff       (20)       12 2023-06-09 16:53:10.000000 quiverquant-0.2.1/quiverquant.egg-info/top_level.txt
+-rw-r--r--   0 ckardatzke   (501) staff       (20)    15959 2023-06-09 16:46:47.000000 quiverquant-0.2.1/quiverquant.py
+-rw-r--r--   0 ckardatzke   (501) staff       (20)       38 2023-06-09 16:53:10.000000 quiverquant-0.2.1/setup.cfg
+-rw-r--r--   0 ckardatzke   (501) staff       (20)      735 2023-06-09 16:52:49.000000 quiverquant-0.2.1/setup.py
```

### Comparing `quiverquant-0.1.9/README.md` & `quiverquant-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # Quiver Quantitative Alternative Data
 This package allows you to access several alternative data sources which are updated daily and mapped to tickers. These include:
 - Trading by US congressmen
 - Corporate Lobbying
 - Government Contracts
+- Patents
+- Off-exchange short volume
 - Companies' Wikipedia page views
-- Discussions on Reddit's /r/WallStreetBets
+- Discussion on Reddit's r/wallstreetbets
+- Discussion on Reddit's r/SPACs
+- Companies' Twitter followings
+- Flights by corporate private jets
+- Political Beta
+- Insider Transactions
 
 This data can be used for backtesting and implementing trading strategies.
 
 ### Receiving API Token
 You can sign up for a Quiver API token [here](https://api.quiverquant.com). 
 
-The cost is $10/month, please [e-mail me](mailto:chris@quiverquant.com) if that is an issue and I may be able to help cover.
+The pricing starts at $10/month, please [e-mail me](mailto:chris@quiverquant.com) if that is an issue and I may be able to help cover.
 
 ## Getting Started
 #### Prerequisites
 - Python version 3 installed locally
 - Pip installed locally
 
 #### Installation
@@ -29,42 +36,75 @@
 #Import the package
 import quiverquant
 
 #Connect to the API using your token
 #Replace <TOKEN> with your token
 quiver = quiverquant.quiver("<TOKEN>")
 
+#Get data on WallStreetBets discussion
+dfWSB = quiver.wallstreetbets()
+
+#Get data on WallStreetBets discussion of GameStop
+dfWSB_GameStop = quiver.wallstreetbets("GME")
+
 #Get recent trades by members of U.S. Congress
 dfCongress = quiver.congress_trading()
 
 #Get trades of a Tesla by members of congress
 dfCongress_Tesla = quiver.congress_trading("TSLA")
 
 #Get trades made by U.S. Senator Richard Burr
 dfCongress_Burr = quiver.congress_trading("Richard Burr", politician=True)
 
-#Get data on WallStreetBets discussion
-dfWSB = quiver.wallstreetbets()
-
-#Get data on WallStreetBets discussion of Virgin Galactic
-dfWSB_Virgin = quiver.wallstreetbets("SPCE")
-
 #Get recent corporate lobbying
 dfLobbying = quiver.lobbying()
 
 #Get corporate lobbying by Apple
 dfLobbying_Apple = quiver.lobbying("AAPL")
 
 #Get data on government contracts
 dfContracts = quiver.gov_contracts()
 
 #Get data on government contracts to Lockheed Martin
 dfContracts_Lockheed = quiver.gov_contracts("LMT")
 
+#Get data on off-exchange short volume
+dfOTC = quiver.offexchange()
+
+#Get data on off-exchange short volume for AMC
+dfOTC_AMC = quiver.offexchange("AMC")
+
 #Get data on Wikipedia page views
 dfWiki = quiver.wikipedia()
 
 #Get data on Wikipedia page views of Microsoft
 dfWiki_Microsoft = quiver.wikipedia("MSFT")
+
+#Get data on companies' Twitter following
+dfTwitter = quiver.twitter()
+
+#Get data on GE's Twitter following
+dfTwitter_GE = quiver.twitter("GE")
+
+#Get data on r/SPACs discussion
+dfSPACs = quiver.spacs()
+
+#Get data on r/SPACs discussion of CCIV
+dfSPACs_CCIV = quiver.spacs("CCIV")
+
+#Get data on recent corporate private jet flights
+dfFlights = quiver.flights()
+
+#Get data on private jet flights by Target
+dfFlights_Target = quiver.flights("TGT")
+
+#Get data on patents by Apple
+dfPatents_Apple = quiver.patents("AAPL")
+
+#Get data on recent insider transactions
+dfInsiders = quiver.insiders()
+
+#Get data on recent insider transactions by Tesla insiders
+dfInsiders_Tesla = quiver.insiders("TSLA")
 ```
```

### Comparing `quiverquant-0.1.9/setup.py` & `quiverquant-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quiverquant",
-    version="0.1.9",
+    version="0.2.01",
     author="Chris Kardatzke",
     author_email="chris@quiverquant.com",
     description="Quiver Quantitative Alternative Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Quiver-Quantitative/python-api",
     py_modules = ["quiverquant"],
@@ -19,8 +19,8 @@
 ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-)
+)
```

