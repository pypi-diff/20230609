# Comparing `tmp/duckduckgo_search-3.8.2.tar.gz` & `tmp/duckduckgo_search-3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.8.2.tar", last modified: Thu Jun  8 08:22:30 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.8.3.tar", last modified: Fri Jun  9 13:20:52 2023, max compression
```

## Comparing `duckduckgo_search-3.8.2.tar` & `duckduckgo_search-3.8.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    14271 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16474 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    31995 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14813 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 13:20:52.000000 duckduckgo_search-3.8.3/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:20:52.943625 duckduckgo_search-3.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-09 13:20:32.000000 duckduckgo_search-3.8.3/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.8.2/LICENSE.md` & `duckduckgo_search-3.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.2/PKG-INFO` & `duckduckgo_search-3.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.8.2
+Version: 3.8.3
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -58,26 +58,34 @@
 python -m duckduckgo_search --help
 ```
 
 CLI examples:
 ```python3
 # text search
 ddgs text -k 'ayrton senna'
+# text search via proxy (example: Tor Browser)
+ddgs text -k 'china is a global threat' -p socks5://localhost:9150
 # find and download pdf files
 ddgs text -k "russia filetype:pdf" -m 50 -d
+# find in es-es region and download pdf files via proxy (example: Tor browser)
+ddgs text -k "embajada a tamorlán filetype:pdf" -r es-es -m 50 -d -p socks5://localhost:9150
 # find and download xls files from a specific site
 ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
-# find and download any xls files from a specific site
-ddgs text -k 'filetype:xls site:mos.ru' -m 50 -d
+# find and download any doc(x) files from a specific site
+ddgs text -k 'filetype:doc site:mos.ru' -m 50 -d
 # find and download images
 ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
+# find in br-br region and download images via proxy (example: Tor browser) in 10 threads
+ddgs images -k 'rio carnival' -r br-br -s off -m 500 -d -th 10 -p socks5://localhost:9150
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
 # get last day's news and save it to a csv file
 ddgs news -k "hubble telescope" -t d -m 50 -o csv
+# get answers and save to a json file
+ddgs answers -k holocaust -o json
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
 | Keywords example |	Result|
 | ---     | ---   |
```

### Comparing `duckduckgo_search-3.8.2/README.md` & `duckduckgo_search-3.8.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,26 +33,34 @@
 python -m duckduckgo_search --help
 ```
 
 CLI examples:
 ```python3
 # text search
 ddgs text -k 'ayrton senna'
+# text search via proxy (example: Tor Browser)
+ddgs text -k 'china is a global threat' -p socks5://localhost:9150
 # find and download pdf files
 ddgs text -k "russia filetype:pdf" -m 50 -d
+# find in es-es region and download pdf files via proxy (example: Tor browser)
+ddgs text -k "embajada a tamorlán filetype:pdf" -r es-es -m 50 -d -p socks5://localhost:9150
 # find and download xls files from a specific site
 ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
-# find and download any xls files from a specific site
-ddgs text -k 'filetype:xls site:mos.ru' -m 50 -d
+# find and download any doc(x) files from a specific site
+ddgs text -k 'filetype:doc site:mos.ru' -m 50 -d
 # find and download images
 ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
+# find in br-br region and download images via proxy (example: Tor browser) in 10 threads
+ddgs images -k 'rio carnival' -r br-br -s off -m 500 -d -th 10 -p socks5://localhost:9150
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
 # get last day's news and save it to a csv file
 ddgs news -k "hubble telescope" -t d -m 50 -o csv
+# get answers and save to a json file
+ddgs answers -k holocaust -o json
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
 | Keywords example |	Result|
 | ---     | ---   |
```

### Comparing `duckduckgo_search-3.8.2/duckduckgo_search/__init__.py` & `duckduckgo_search-3.8.3/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.2/duckduckgo_search/cli.py` & `duckduckgo_search-3.8.3/duckduckgo_search/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import csv
 import json
 import logging
 import os
+import ssl
 from datetime import datetime
 from random import choice
 from urllib.parse import unquote
 
 import aiofiles
 import click
 import httpx
@@ -91,50 +92,61 @@
         .replace("/", "_")
         .replace("\\", "_")
         .replace(" ", "")
     )
     return keywords
 
 
-async def download_file(url, dir_path, filename, sem):
+async def download_file(url, dir_path, filename, sem, proxy):
     headers = {"User-Agent": choice(USERAGENTS)}
-    try:
-        async with sem:
-            async with httpx.AsyncClient(headers=headers) as client:
-                async with client.stream("GET", url) as resp:
-                    if resp.status_code == 200:
-                        async with aiofiles.open(
-                            os.path.join(dir_path, filename), "wb"
-                        ) as file:
-                            async for chunk in resp.aiter_bytes():
-                                await file.write(chunk)
-                logger.info(f"File downloaded {url}")
-    except Exception as ex:
-        logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
+    for i in range(2):
+        try:
+            async with sem:
+                async with httpx.AsyncClient(headers=headers, proxies=proxy) as client:
+                    async with client.stream("GET", url) as resp:
+                        if resp.status_code == 200:
+                            async with aiofiles.open(
+                                os.path.join(dir_path, filename[:200]), "wb"
+                            ) as file:
+                                async for chunk in resp.aiter_bytes():
+                                    await file.write(chunk)
+                            break
+        except (
+            httpx.ConnectTimeout,
+            httpx.ConnectError,
+            httpx.ProxyError,
+            httpx.ReadTimeout,
+            ssl.SSLCertVerificationError,
+            ssl.SSLError,
+        ) as ex:
+            logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
+        except ValueError as ex:
+            raise ex
 
 
-async def _download_results(keywords, results, images=False):
+async def _download_results(keywords, results, images=False, proxy=None, threads=None):
     if images:
         path = f"images_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     else:
         path = f"text_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     os.makedirs(path, exist_ok=True)
 
     tasks = []
-    sem = asyncio.Semaphore(20)
+    threads = 20 if threads is None else threads
+    sem = asyncio.Semaphore(threads)
     for i, res in enumerate(results, start=1):
         if images:
             filename = unquote(res["image"].split("/")[-1].split("?")[0])
             task = asyncio.create_task(
-                download_file(res["image"], path, f"{i}_{filename}", sem)
+                download_file(res["image"], path, f"{i}_{filename}", sem, proxy)
             )
         else:
             filename = unquote(res["href"].split("/")[-1].split("?")[0])
             task = asyncio.create_task(
-                download_file(res["href"], path, f"{i}_{filename}", sem)
+                download_file(res["href"], path, f"{i}_{filename}", sem, proxy)
             )
         tasks.append(task)
 
     with click.progressbar(
         length=len(tasks),
         label="Downloading",
         show_percent=True,
@@ -144,16 +156,16 @@
         for future in asyncio.as_completed(tasks):
             await future
             bar.update(1)
 
     await asyncio.gather(*tasks)
 
 
-def download_results(keywords, results, images=False):
-    asyncio.run(_download_results(keywords, results, images))
+def download_results(keywords, results, images=False, proxy=None, threads=None):
+    asyncio.run(_download_results(keywords, results, images, proxy))
 
 
 @click.group(chain=True)
 def cli():
     pass
 
 
@@ -207,30 +219,58 @@
 @click.option(
     "-b",
     "--backend",
     default="api",
     type=click.Choice(["api", "html", "lite"]),
     help="which backend to use, default=api",
 )
-def text(keywords, output, download, max_results, *args, **kwargs):
+@click.option(
+    "-th",
+    "--threads",
+    default=20,
+    help="download threads, default=20",
+)
+@click.option(
+    "-p",
+    "--proxy",
+    help="proxy server for download, example: socks5://localhost:9150",
+)
+def text(
+    keywords,
+    region,
+    safesearch,
+    timelimit,
+    backend,
+    output,
+    download,
+    threads,
+    max_results,
+    proxy,
+):
     data = []
-    for r in DDGS().text(keywords=keywords, *args, **kwargs):
+    for r in DDGS(proxies=proxy).text(
+        keywords=keywords,
+        region=region,
+        safesearch=safesearch,
+        timelimit=timelimit,
+        backend=backend,
+    ):
         if len(data) >= max_results:
             break
         data.append(r)
     keywords = sanitize_keywords(keywords)
     filename = f"text_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print" and not download:
         print_data(data)
     elif output == "csv":
         save_csv(f"{filename}.csv", data)
     elif output == "json":
         save_json(f"{filename}.json", data)
     if download:
-        download_results(keywords, data)
+        download_results(keywords, data, proxy=proxy, threads=threads)
 
 
 @cli.command()
 @click.option(
     "-k", "--keywords", required=True, help="answers search, keywords for query"
 )
 @click.option(
@@ -337,30 +377,66 @@
 @click.option(
     "-d",
     "--download",
     is_flag=True,
     default=False,
     help="download and save images to 'keywords' folder",
 )
-def images(keywords, output, download, max_results, *args, **kwargs):
+@click.option(
+    "-th",
+    "--threads",
+    default=20,
+    help="download threads, default=20",
+)
+@click.option(
+    "-p",
+    "--proxy",
+    help="proxy server for download, example: socks5://localhost:9150",
+)
+def images(
+    keywords,
+    region,
+    safesearch,
+    timelimit,
+    size,
+    color,
+    type_image,
+    layout,
+    license_image,
+    download,
+    threads,
+    max_results,
+    output,
+    proxy,
+):
     data = []
-    for r in DDGS().images(keywords=keywords, *args, **kwargs):
+    for r in DDGS(proxies=proxy).images(
+        keywords=keywords,
+        region=region,
+        safesearch=safesearch,
+        timelimit=timelimit,
+        size=size,
+        color=color,
+        type_image=type_image,
+        layout=layout,
+        license_image=license_image,
+    ):
         if len(data) >= max_results:
             break
         data.append(r)
     keywords = sanitize_keywords(keywords)
     filename = f"images_{sanitize_keywords(keywords)}_{datetime.now():%Y%m%d_%H%M%S}"
     if output == "print" and not download:
         print_data(data)
     elif output == "csv":
         save_csv(f"{filename}.csv", data)
     elif output == "json":
         save_json(f"{filename}.json", data)
     if download:
-        download_results(keywords, data, images=True)
+        download_results(keywords, data, images=True, proxy=proxy, threads=threads)
 
 
 @cli.command()
 @click.option("-k", "--keywords", required=True, help="keywords for query")
 @click.option(
     "-r",
     "--region",
```

### Comparing `duckduckgo_search-3.8.2/duckduckgo_search/compat.py` & `duckduckgo_search-3.8.3/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.2/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.8.3/duckduckgo_search/duckduckgo_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import re
 from collections import deque
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from html import unescape
-from itertools import cycle
+from itertools import cycle, islice
 from random import choice
 from time import sleep
 from typing import Deque, Dict, Iterator, Optional, Set, Tuple
 from urllib.parse import unquote
 
 import httpx
 from lxml import html
@@ -336,26 +336,28 @@
 
             if b"No more results." in resp.content:
                 return
 
             tree = html.fromstring(resp.content)
 
             result_exists = False
-            for i, e in zip(cycle(range(1, 5)), tree.xpath("//table[last()]//tr")):
+            data = zip(cycle(range(1, 5)), tree.xpath("//table[last()]//tr"))
+            for i, e in data:
                 if i == 1:
                     href = e.xpath(".//a//@href")
                     href = href[0] if href else None
                     if (
                         href is None
                         or href in cache
                         or href == f"http://www.google.com/search?q={keywords}"
                     ):
-                        continue
-                    cache.add(href)
-                    title = e.xpath(".//a//text()")[0]
+                        [next(data, None) for _ in range(3)]  # skip block(i=1,2,3,4)
+                    else:
+                        cache.add(href)
+                        title = e.xpath(".//a//text()")[0]
                 elif i == 2:
                     body = e.xpath(".//td[@class='result-snippet']//text()")
                     body = "".join(body).strip()
                 elif i == 3:
                     result_exists = True
                     yield {
                         "title": self._normalize(title),
```

### Comparing `duckduckgo_search-3.8.2/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.8.3/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.8.2
+Version: 3.8.3
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -58,26 +58,34 @@
 python -m duckduckgo_search --help
 ```
 
 CLI examples:
 ```python3
 # text search
 ddgs text -k 'ayrton senna'
+# text search via proxy (example: Tor Browser)
+ddgs text -k 'china is a global threat' -p socks5://localhost:9150
 # find and download pdf files
 ddgs text -k "russia filetype:pdf" -m 50 -d
+# find in es-es region and download pdf files via proxy (example: Tor browser)
+ddgs text -k "embajada a tamorlán filetype:pdf" -r es-es -m 50 -d -p socks5://localhost:9150
 # find and download xls files from a specific site
 ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
-# find and download any xls files from a specific site
-ddgs text -k 'filetype:xls site:mos.ru' -m 50 -d
+# find and download any doc(x) files from a specific site
+ddgs text -k 'filetype:doc site:mos.ru' -m 50 -d
 # find and download images
 ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
+# find in br-br region and download images via proxy (example: Tor browser) in 10 threads
+ddgs images -k 'rio carnival' -r br-br -s off -m 500 -d -th 10 -p socks5://localhost:9150
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
 # get last day's news and save it to a csv file
 ddgs news -k "hubble telescope" -t d -m 50 -o csv
+# get answers and save to a json file
+ddgs answers -k holocaust -o json
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
 | Keywords example |	Result|
 | ---     | ---   |
```

### Comparing `duckduckgo_search-3.8.2/pyproject.toml` & `duckduckgo_search-3.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.2/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.8.3/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

