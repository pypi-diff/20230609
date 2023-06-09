# Comparing `tmp/yt-fts-0.1.8.tar.gz` & `tmp/yt-fts-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-fts-0.1.8.tar", last modified: Mon May 29 17:46:11 2023, max compression
+gzip compressed data, was "yt-fts-0.1.9.tar", last modified: Mon May 29 21:32:43 2023, max compression
```

## Comparing `yt-fts-0.1.8.tar` & `yt-fts-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 17:46:11.124924 yt-fts-0.1.8/
--rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 20:45:24.000000 yt-fts-0.1.8/LICENSE
--rw-r--r--   0 home       (501) staff       (20)     4705 2023-05-29 17:46:11.124205 yt-fts-0.1.8/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     4162 2023-05-29 17:04:59.000000 yt-fts-0.1.8/README.md
--rw-r--r--   0 home       (501) staff       (20)       38 2023-05-29 17:46:11.125157 yt-fts-0.1.8/setup.cfg
--rw-r--r--   0 home       (501) staff       (20)      969 2023-05-29 17:46:03.000000 yt-fts-0.1.8/setup.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 17:46:11.116939 yt-fts-0.1.8/tests/
--rw-r--r--   0 home       (501) staff       (20)      325 2023-05-29 14:19:36.000000 yt-fts-0.1.8/tests/test_search_all.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 17:46:11.119100 yt-fts-0.1.8/yt_fts/
--rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 20:45:24.000000 yt-fts-0.1.8/yt_fts/__init__.py
--rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 20:45:24.000000 yt-fts-0.1.8/yt_fts/__main__.py
--rw-r--r--   0 home       (501) staff       (20)     3204 2023-05-29 17:38:10.000000 yt-fts-0.1.8/yt_fts/db_scripts.py
--rw-r--r--   0 home       (501) staff       (20)    10975 2023-05-29 17:41:42.000000 yt-fts-0.1.8/yt_fts/yt_fts.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 17:46:11.123252 yt-fts-0.1.8/yt_fts.egg-info/
--rw-r--r--   0 home       (501) staff       (20)     4705 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)      309 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       45 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/entry_points.txt
--rw-r--r--   0 home       (501) staff       (20)      288 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)        7 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/top_level.txt
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 21:32:43.110380 yt-fts-0.1.9/
+-rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 20:45:24.000000 yt-fts-0.1.9/LICENSE
+-rw-r--r--   0 home       (501) staff       (20)     4786 2023-05-29 21:32:43.109696 yt-fts-0.1.9/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     4243 2023-05-29 18:37:41.000000 yt-fts-0.1.9/README.md
+-rw-r--r--   0 home       (501) staff       (20)       38 2023-05-29 21:32:43.110573 yt-fts-0.1.9/setup.cfg
+-rw-r--r--   0 home       (501) staff       (20)      969 2023-05-29 21:32:35.000000 yt-fts-0.1.9/setup.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 21:32:43.096424 yt-fts-0.1.9/tests/
+-rw-r--r--   0 home       (501) staff       (20)      325 2023-05-29 14:19:36.000000 yt-fts-0.1.9/tests/test_search_all.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 21:32:43.102287 yt-fts-0.1.9/yt_fts/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 20:45:24.000000 yt-fts-0.1.9/yt_fts/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 20:45:24.000000 yt-fts-0.1.9/yt_fts/__main__.py
+-rw-r--r--   0 home       (501) staff       (20)     3204 2023-05-29 19:58:12.000000 yt-fts-0.1.9/yt_fts/db_scripts.py
+-rw-r--r--   0 home       (501) staff       (20)     4654 2023-05-29 20:57:03.000000 yt-fts-0.1.9/yt_fts/download_scripts.py
+-rw-r--r--   0 home       (501) staff       (20)     1592 2023-05-29 20:50:33.000000 yt-fts-0.1.9/yt_fts/utils.py
+-rw-r--r--   0 home       (501) staff       (20)     5873 2023-05-29 20:47:14.000000 yt-fts-0.1.9/yt_fts/yt_fts.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 21:32:43.108544 yt-fts-0.1.9/yt_fts.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)     4786 2023-05-29 21:32:43.000000 yt-fts-0.1.9/yt_fts.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)      352 2023-05-29 21:32:43.000000 yt-fts-0.1.9/yt_fts.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-05-29 21:32:43.000000 yt-fts-0.1.9/yt_fts.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       45 2023-05-29 21:32:43.000000 yt-fts-0.1.9/yt_fts.egg-info/entry_points.txt
+-rw-r--r--   0 home       (501) staff       (20)      288 2023-05-29 21:32:43.000000 yt-fts-0.1.9/yt_fts.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)        7 2023-05-29 21:32:43.000000 yt-fts-0.1.9/yt_fts.egg-info/top_level.txt
```

### Comparing `yt-fts-0.1.8/LICENSE` & `yt-fts-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.8/PKG-INFO` & `yt-fts-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-fts
-Version: 0.1.8
+Version: 0.1.9
 Summary: yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.
 Home-page: https://github.com/NotJoeMartinez/yt-fts
 Author: NotJoeMartinez
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,122 +45,130 @@
 brew install yt-dlp
 ```
 **Windows/winget**
 ```bash
 winget install yt-dlp
 ```
 
-### Usage 
+## Usage 
 ```
 Usage: yt-fts [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   delete    delete [channel id]
   download  download [channel url]
   export    export [search text] [channel id]
   list      Lists channels
   search    search [search text] [channel id]
 ```
 
-### `download`
+## `download`
 Will download all of a channels vtt files into your database 
 ```bash
 yt-fts download "https://www.youtube.com/@TimDillonShow/videos"
 ```
 
-**`--channel-id [youtube channel id]`**
+`--channel-id [channel_id]`
 
 If `download` fails you can manually input the channel id with the `--channel-id` flag.
 The channel url should still be an argument 
 ```bash
 yt-fts download --channel-id "UC4woSp8ITBoYDmjkukhEhxg" "https://www.youtube.com/@TimDillonShow/videos" 
 ```
 
-**`--language [en/fr/es/etc..]`**
+`--language [en/fr/es/etc..]`
 
 Specify subtitles language 
 ```bash
 yt-fts download --language de "https://www.youtube.com/@TimDillonShow/videos" 
 ```
 
-**`--number-of-jobs [number]`**
+`--number-of-jobs [num_threads]`
 
 Speed up downloads with multi threading 
 ```bash
 yt-fts download --number-of-jobs 6 "https://www.youtube.com/@TimDillonShow/videos"
 ```
 
-### `list`
+## `list`
 List all of your downloaded channels 
 ```bash
 yt-fts list
 ```
 
 output:
 ```
 Listing channels
 channel_id                channel_name         channel_url
 ------------------------  -------------------  ---------------------------------------------------------------
 UC4woSp8ITBoYDmjkukhEhxg  The Tim Dillon Show  https://www.youtube.com/channel/UC4woSp8ITBoYDmjkukhEhxg/videos
 ```
 
-### `search`
+## `search`
 Search a channel for text based off the channel id you give it and 
 print a url to that point in the video. The search string does not 
 have to be a word for word and match is limited to 40 characters. 
 
 ```bash
 yt-fts search "text you want to find" [channel_id]
 ```
 **Ex:**
 ```bash
 yt-fts search "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 output:
 ```
-Video Title: "164 - Life In The Big City - YouTube"
+The Tim Dillon Show: "164 - Life In The Big City - YouTube"
 
     Quote: "van in the driveway life in the big city"
     Time Stamp: 00:30:44.580
     Link: https://youtu.be/dqGyCTbzYmc?t=1841
+```
 
-Video Title: "154 - The 3 AM Episode - YouTube"
+### Search all channels 
+Use `--all` to search all channels in your database 
 
-    Quote: "Dennis would go hey life in the big city"
-    Time Stamp: 00:58:53.789
-    Link: https://youtu.be/MhaG3Yfv1cU?t=3530
+**Ex:**
+```bash
+yt-fts search "text to search" --all
 ```
 
 ### Advanced Search Syntax
 
 The search string supports sqlite [Enhanced Query Syntax](https://www.sqlite.org/fts3.html#full_text_index_queries).
 which includes things like [prefix queries](https://www.sqlite.org/fts3.html#termprefix) which you can use to match parts of a word.  
 
 **Ex:**
 
 ```bash
 yt-fts search "rea* kni* Mali*" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 output:
 ```
-Video Title: "#200 - Knife Fights In Malibu | The Tim Dillon Show - YouTube"
+The Tim Dillon Show: "#200 - Knife Fights In Malibu | The Tim Dillon Show - YouTube"
 
     Quote: "real knife fight down here in Malibu I"
     Time Stamp: 00:45:39.420
     Link: https://youtu.be/e79H5nxS65Q?t=2736
 ```
 
-### `Export`
+## `Export`
 Similar to `search` except it will export all of the search results to a csv 
-with the format: `Video Title,Quote,Time Stamp,Link` as it's headers
+with the format: `Channel Name,Video Title,Quote,Time Stamp,Link` as it's headers
+
 ```bash
 yt-fts export "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 
-### `Delete` 
+You can export from all channels in your database as well
+```bash
+yt-fts export "life in the big city" --all
+```
+
+## `Delete` 
 Will delete a channel from your database 
 ```bash
 yt-fts delete [channel_id]
 ```
```

### Comparing `yt-fts-0.1.8/README.md` & `yt-fts-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,122 +35,130 @@
 brew install yt-dlp
 ```
 **Windows/winget**
 ```bash
 winget install yt-dlp
 ```
 
-### Usage 
+## Usage 
 ```
 Usage: yt-fts [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   delete    delete [channel id]
   download  download [channel url]
   export    export [search text] [channel id]
   list      Lists channels
   search    search [search text] [channel id]
 ```
 
-### `download`
+## `download`
 Will download all of a channels vtt files into your database 
 ```bash
 yt-fts download "https://www.youtube.com/@TimDillonShow/videos"
 ```
 
-**`--channel-id [youtube channel id]`**
+`--channel-id [channel_id]`
 
 If `download` fails you can manually input the channel id with the `--channel-id` flag.
 The channel url should still be an argument 
 ```bash
 yt-fts download --channel-id "UC4woSp8ITBoYDmjkukhEhxg" "https://www.youtube.com/@TimDillonShow/videos" 
 ```
 
-**`--language [en/fr/es/etc..]`**
+`--language [en/fr/es/etc..]`
 
 Specify subtitles language 
 ```bash
 yt-fts download --language de "https://www.youtube.com/@TimDillonShow/videos" 
 ```
 
-**`--number-of-jobs [number]`**
+`--number-of-jobs [num_threads]`
 
 Speed up downloads with multi threading 
 ```bash
 yt-fts download --number-of-jobs 6 "https://www.youtube.com/@TimDillonShow/videos"
 ```
 
-### `list`
+## `list`
 List all of your downloaded channels 
 ```bash
 yt-fts list
 ```
 
 output:
 ```
 Listing channels
 channel_id                channel_name         channel_url
 ------------------------  -------------------  ---------------------------------------------------------------
 UC4woSp8ITBoYDmjkukhEhxg  The Tim Dillon Show  https://www.youtube.com/channel/UC4woSp8ITBoYDmjkukhEhxg/videos
 ```
 
-### `search`
+## `search`
 Search a channel for text based off the channel id you give it and 
 print a url to that point in the video. The search string does not 
 have to be a word for word and match is limited to 40 characters. 
 
 ```bash
 yt-fts search "text you want to find" [channel_id]
 ```
 **Ex:**
 ```bash
 yt-fts search "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 output:
 ```
-Video Title: "164 - Life In The Big City - YouTube"
+The Tim Dillon Show: "164 - Life In The Big City - YouTube"
 
     Quote: "van in the driveway life in the big city"
     Time Stamp: 00:30:44.580
     Link: https://youtu.be/dqGyCTbzYmc?t=1841
+```
 
-Video Title: "154 - The 3 AM Episode - YouTube"
+### Search all channels 
+Use `--all` to search all channels in your database 
 
-    Quote: "Dennis would go hey life in the big city"
-    Time Stamp: 00:58:53.789
-    Link: https://youtu.be/MhaG3Yfv1cU?t=3530
+**Ex:**
+```bash
+yt-fts search "text to search" --all
 ```
 
 ### Advanced Search Syntax
 
 The search string supports sqlite [Enhanced Query Syntax](https://www.sqlite.org/fts3.html#full_text_index_queries).
 which includes things like [prefix queries](https://www.sqlite.org/fts3.html#termprefix) which you can use to match parts of a word.  
 
 **Ex:**
 
 ```bash
 yt-fts search "rea* kni* Mali*" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 output:
 ```
-Video Title: "#200 - Knife Fights In Malibu | The Tim Dillon Show - YouTube"
+The Tim Dillon Show: "#200 - Knife Fights In Malibu | The Tim Dillon Show - YouTube"
 
     Quote: "real knife fight down here in Malibu I"
     Time Stamp: 00:45:39.420
     Link: https://youtu.be/e79H5nxS65Q?t=2736
 ```
 
-### `Export`
+## `Export`
 Similar to `search` except it will export all of the search results to a csv 
-with the format: `Video Title,Quote,Time Stamp,Link` as it's headers
+with the format: `Channel Name,Video Title,Quote,Time Stamp,Link` as it's headers
+
 ```bash
 yt-fts export "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 
-### `Delete` 
+You can export from all channels in your database as well
+```bash
+yt-fts export "life in the big city" --all
+```
+
+## `Delete` 
 Will delete a channel from your database 
 ```bash
 yt-fts delete [channel_id]
 ```
```

### Comparing `yt-fts-0.1.8/setup.py` & `yt-fts-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'console_scripts': [
         'yt-fts=yt_fts.yt_fts:cli',
     ],
 }
 
 setup(
     name='yt-fts', 
-    version='0.1.8',
+    version='0.1.9',
     description='yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     author='NotJoeMartinez',
     url='https://github.com/NotJoeMartinez/yt-fts',  
     packages=find_packages(),
     install_requires=dependencies,
```

### Comparing `yt-fts-0.1.8/yt_fts/db_scripts.py` & `yt-fts-0.1.9/yt_fts/db_scripts.py`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.8/yt_fts.egg-info/PKG-INFO` & `yt-fts-0.1.9/yt_fts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-fts
-Version: 0.1.8
+Version: 0.1.9
 Summary: yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.
 Home-page: https://github.com/NotJoeMartinez/yt-fts
 Author: NotJoeMartinez
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,122 +45,130 @@
 brew install yt-dlp
 ```
 **Windows/winget**
 ```bash
 winget install yt-dlp
 ```
 
-### Usage 
+## Usage 
 ```
 Usage: yt-fts [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   delete    delete [channel id]
   download  download [channel url]
   export    export [search text] [channel id]
   list      Lists channels
   search    search [search text] [channel id]
 ```
 
-### `download`
+## `download`
 Will download all of a channels vtt files into your database 
 ```bash
 yt-fts download "https://www.youtube.com/@TimDillonShow/videos"
 ```
 
-**`--channel-id [youtube channel id]`**
+`--channel-id [channel_id]`
 
 If `download` fails you can manually input the channel id with the `--channel-id` flag.
 The channel url should still be an argument 
 ```bash
 yt-fts download --channel-id "UC4woSp8ITBoYDmjkukhEhxg" "https://www.youtube.com/@TimDillonShow/videos" 
 ```
 
-**`--language [en/fr/es/etc..]`**
+`--language [en/fr/es/etc..]`
 
 Specify subtitles language 
 ```bash
 yt-fts download --language de "https://www.youtube.com/@TimDillonShow/videos" 
 ```
 
-**`--number-of-jobs [number]`**
+`--number-of-jobs [num_threads]`
 
 Speed up downloads with multi threading 
 ```bash
 yt-fts download --number-of-jobs 6 "https://www.youtube.com/@TimDillonShow/videos"
 ```
 
-### `list`
+## `list`
 List all of your downloaded channels 
 ```bash
 yt-fts list
 ```
 
 output:
 ```
 Listing channels
 channel_id                channel_name         channel_url
 ------------------------  -------------------  ---------------------------------------------------------------
 UC4woSp8ITBoYDmjkukhEhxg  The Tim Dillon Show  https://www.youtube.com/channel/UC4woSp8ITBoYDmjkukhEhxg/videos
 ```
 
-### `search`
+## `search`
 Search a channel for text based off the channel id you give it and 
 print a url to that point in the video. The search string does not 
 have to be a word for word and match is limited to 40 characters. 
 
 ```bash
 yt-fts search "text you want to find" [channel_id]
 ```
 **Ex:**
 ```bash
 yt-fts search "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 output:
 ```
-Video Title: "164 - Life In The Big City - YouTube"
+The Tim Dillon Show: "164 - Life In The Big City - YouTube"
 
     Quote: "van in the driveway life in the big city"
     Time Stamp: 00:30:44.580
     Link: https://youtu.be/dqGyCTbzYmc?t=1841
+```
 
-Video Title: "154 - The 3 AM Episode - YouTube"
+### Search all channels 
+Use `--all` to search all channels in your database 
 
-    Quote: "Dennis would go hey life in the big city"
-    Time Stamp: 00:58:53.789
-    Link: https://youtu.be/MhaG3Yfv1cU?t=3530
+**Ex:**
+```bash
+yt-fts search "text to search" --all
 ```
 
 ### Advanced Search Syntax
 
 The search string supports sqlite [Enhanced Query Syntax](https://www.sqlite.org/fts3.html#full_text_index_queries).
 which includes things like [prefix queries](https://www.sqlite.org/fts3.html#termprefix) which you can use to match parts of a word.  
 
 **Ex:**
 
 ```bash
 yt-fts search "rea* kni* Mali*" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 output:
 ```
-Video Title: "#200 - Knife Fights In Malibu | The Tim Dillon Show - YouTube"
+The Tim Dillon Show: "#200 - Knife Fights In Malibu | The Tim Dillon Show - YouTube"
 
     Quote: "real knife fight down here in Malibu I"
     Time Stamp: 00:45:39.420
     Link: https://youtu.be/e79H5nxS65Q?t=2736
 ```
 
-### `Export`
+## `Export`
 Similar to `search` except it will export all of the search results to a csv 
-with the format: `Video Title,Quote,Time Stamp,Link` as it's headers
+with the format: `Channel Name,Video Title,Quote,Time Stamp,Link` as it's headers
+
 ```bash
 yt-fts export "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 
-### `Delete` 
+You can export from all channels in your database as well
+```bash
+yt-fts export "life in the big city" --all
+```
+
+## `Delete` 
 Will delete a channel from your database 
 ```bash
 yt-fts delete [channel_id]
 ```
```

