# Comparing `tmp/wclone-1.0.0.tar.gz` & `tmp/wclone-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wclone-1.0.0.tar", last modified: Sat Jun  3 13:34:13 2023, max compression
+gzip compressed data, was "wclone-1.0.1.tar", last modified: Fri Jun  9 16:19:42 2023, max compression
```

## Comparing `wclone-1.0.0.tar` & `wclone-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-03 13:34:13.565583 wclone-1.0.0/
--rw-rw----   0 root         (0) everybody  (9997)     2402 2023-06-03 13:34:13.533583 wclone-1.0.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1650 2023-06-03 13:13:22.000000 wclone-1.0.0/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-03 13:34:13.569583 wclone-1.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1103 2023-06-03 12:33:01.000000 wclone-1.0.0/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-03 13:34:13.265583 wclone-1.0.0/wclone/
--rw-rw----   0 root         (0) everybody  (9997)      178 2023-06-03 13:30:40.000000 wclone-1.0.0/wclone/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       28 2023-06-03 12:31:36.000000 wclone-1.0.0/wclone/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     9335 2023-06-03 13:12:00.000000 wclone-1.0.0/wclone/app.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-03 13:34:13.513583 wclone-1.0.0/wclone.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2402 2023-06-03 13:34:12.000000 wclone-1.0.0/wclone.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      252 2023-06-03 13:34:12.000000 wclone-1.0.0/wclone.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-03 13:34:12.000000 wclone-1.0.0/wclone.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       43 2023-06-03 13:34:12.000000 wclone-1.0.0/wclone.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       13 2023-06-03 13:34:12.000000 wclone-1.0.0/wclone.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-06-03 13:34:12.000000 wclone-1.0.0/wclone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:19:42.568390 wclone-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-09 16:19:42.568390 wclone-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-09 16:19:26.000000 wclone-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:19:42.568390 wclone-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-09 16:19:26.000000 wclone-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:19:42.568390 wclone-1.0.1/wclone/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 16:19:26.000000 wclone-1.0.1/wclone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 16:19:26.000000 wclone-1.0.1/wclone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-06-09 16:19:26.000000 wclone-1.0.1/wclone/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:19:42.568390 wclone-1.0.1/wclone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 16:19:42.000000 wclone-1.0.1/wclone.egg-info/top_level.txt
```

### Comparing `wclone-1.0.0/PKG-INFO` & `wclone-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wclone
-Version: 1.0.0
+Version: 1.0.1
 Summary: Basic website cloner written in Python
 Home-page: https://github.com/ZKAW/website-cloner
 Author: ZKAW
 Maintainer: Smartwa
 Maintainer-email: smartwacaleb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/ZKAW/website-cloner/issues/new
```

### Comparing `wclone-1.0.0/README.md` & `wclone-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wclone-1.0.0/setup.py` & `wclone-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     author=__author__,
     maintainer=__maintainer__,
     maintainer_email="smartwacaleb@gmail.com",
     description=__description__,
     packages=["wclone"],
     url=__repo__,
     project_urls={"Bug Report": f"{__repo__}/issues/new"},
-    install_requires=["bs4", "requests"],
+    install_requires=["bs4", "requests","cloudscraper==1.2.69"],
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `wclone-1.0.0/wclone/app.py` & `wclone-1.0.1/wclone/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,259 +2,370 @@
 import requests
 import functools
 import shutil
 import codecs
 import sys
 import os
 import logging
-
+import cloudscraper
 from bs4 import BeautifulSoup
 from urllib.parse import urljoin, urlparse
-from . import __version__,__description__
+from . import __version__, __description__
+
+platforms = ["darwin", "ios", "android", "windows", "linux"]
+browsers = ["chrome", "firefox"]
+
 
 class Extractor:
     def __init__(self, url):
         self.url = url
         self.soup = BeautifulSoup(self.get_page_content(url), "html.parser")
 
         self.scraped_urls = self.scrap_all_urls()
-    
+
     def run(self):
         self.save_files(self.scraped_urls)
         self.save_html()
-    
+
     def get_page_content(self, url):
-        try: 
+        try:
             content = session.get(url)
-            content.encoding = 'utf-8'
+            content.encoding = "utf-8"
             return content.text
         except Exception as e:
-        	sys.exit(logging.critical(get_excep(e)))
+            sys.exit(logging.critical(get_excep(e)))
 
-    # get the script files    
+    # get the script files
     def scrap_scripts(self):
         script_urls = []
         for script_tag in self.soup.find_all("script"):
             # if the tag has the attribute 'script'
             script_url = script_tag.attrs.get("src")
             if script_url:
-                if not script_url.startswith('http'): script_url = urljoin(self.url, script_url)
-                else: continue
+                if not script_url.startswith("http"):
+                    script_url = urljoin(self.url, script_url)
+                else:
+                    continue
 
                 new_url = self.url_to_local_path(script_url, keepQuery=True)
 
                 if new_url:
-                    script_tag['src'] = new_url
-                    script_urls.append(script_url.split('?')[0])
-        
+                    script_tag["src"] = new_url
+                    script_urls.append(script_url.split("?")[0])
+
         return list(dict.fromkeys(script_urls))
 
     #  get attributes
     def scrap_form_attr(self):
         urls = []
         for form_tag in self.soup.find_all("form"):
             # if the tag has the attribute 'action'
             form_url = form_tag.attrs.get("action")
             if form_url:
-                if not form_url.startswith('http'): form_url = urljoin(self.url, form_tag.attrs.get("action"))
+                if not form_url.startswith("http"):
+                    form_url = urljoin(self.url, form_tag.attrs.get("action"))
 
                 new_url = self.url_to_local_path(form_url, keepQuery=True)
 
                 if new_url:
-                    form_tag['action'] = new_url
+                    form_tag["action"] = new_url
 
-                    urls.append(form_url.split('?')[0])
+                    urls.append(form_url.split("?")[0])
 
         return list(dict.fromkeys(urls))
 
     def scrap_a_attr(self):
         urls = []
-        for link_tag in self.soup.find_all('a'):
+        for link_tag in self.soup.find_all("a"):
             # if the tag has the attribute 'href'
-            link_url = link_tag.attrs.get('href')
+            link_url = link_tag.attrs.get("href")
             if link_url:
-                if not link_url.startswith('http'): link_url = urljoin(self.url, link_tag.attrs.get('href'))
+                if not link_url.startswith("http"):
+                    link_url = urljoin(self.url, link_tag.attrs.get("href"))
 
                 new_url = self.url_to_local_path(link_url, keepQuery=True)
                 if new_url:
-                    link_tag['href'] = new_url
-                    urls.append(link_url.split('?')[0])
+                    link_tag["href"] = new_url
+                    urls.append(link_url.split("?")[0])
 
-        return list(dict.fromkeys(urls))          
-                
+        return list(dict.fromkeys(urls))
 
     def scrap_img_attr(self):
         urls = []
-        for img_tag in self.soup.find_all('img'):
+        for img_tag in self.soup.find_all("img"):
             # if the tag has the attribute 'src'
-            img_url = img_tag.attrs.get('src')
+            img_url = img_tag.attrs.get("src")
             if img_url:
-                if not img_url.startswith('http'): img_url = urljoin(self.url, img_tag.attrs.get('src'))
+                if not img_url.startswith("http"):
+                    img_url = urljoin(self.url, img_tag.attrs.get("src"))
 
                 new_url = self.url_to_local_path(img_url, keepQuery=True)
                 if new_url:
-                    img_tag['src'] = new_url
-                    urls.append(img_url.split('?')[0])
+                    img_tag["src"] = new_url
+                    urls.append(img_url.split("?")[0])
 
         return list(dict.fromkeys(urls))
-    
+
     def scrap_link_attr(self):
         urls = []
-        for link_tag in self.soup.find_all('link'):
+        for link_tag in self.soup.find_all("link"):
             # if the tag has the attribute 'href'
-            link_url = link_tag.attrs.get('href')
+            link_url = link_tag.attrs.get("href")
             if link_url:
-                if not link_url.startswith('http'): link_url = urljoin(self.url, link_tag.attrs.get('href'))
+                if not link_url.startswith("http"):
+                    link_url = urljoin(self.url, link_tag.attrs.get("href"))
 
                 new_url = self.url_to_local_path(link_url, keepQuery=True)
                 if new_url:
-                    link_tag['href'] = new_url
-                    urls.append(link_url.split('?')[0])
+                    link_tag["href"] = new_url
+                    urls.append(link_url.split("?")[0])
 
         return list(dict.fromkeys(urls))
-    
+
     def scrap_btn_attr(self):
         urls = []
-        for buttons in self.soup.find_all('button'):
-            button_url = buttons.attrs.get('onclick')
-            if not button_url: return None
-
-            button_url = button_url.replace(' ','')
-            button_url = button_url[button_url.find('location.href='):].replace('location.href=','')
-            button_url = button_url.replace('\'', '')
-            button_url = button_url.replace('\"', '')
-            button_url = button_url.replace('`', '')
-
-            if button_url and button_url.startswith('/'):
-                if not button_url.startswith('http'): button_url = urljoin(self.url, buttons.get('onclick'))
+        for buttons in self.soup.find_all("button"):
+            button_url = buttons.attrs.get("onclick")
+            if not button_url:
+                return None
+
+            button_url = button_url.replace(" ", "")
+            button_url = button_url[button_url.find("location.href=") :].replace(
+                "location.href=", ""
+            )
+            button_url = button_url.replace("'", "")
+            button_url = button_url.replace('"', "")
+            button_url = button_url.replace("`", "")
+
+            if button_url and button_url.startswith("/"):
+                if not button_url.startswith("http"):
+                    button_url = urljoin(self.url, buttons.get("onclick"))
 
                 new_url = self.url_to_local_path(button_url, keepQuery=True)
                 if new_url:
-                    buttons['onclick'] = new_url
-                    urls.append(button_url.split('?')[0])
+                    buttons["onclick"] = new_url
+                    urls.append(button_url.split("?")[0])
 
         return list(dict.fromkeys(urls))
-                
 
     # get assets (img and more)
     def scrap_assets(self):
         assets_urls = []
 
         form_attr = self.scrap_form_attr()
         a_attr = self.scrap_a_attr()
         img_attr = self.scrap_img_attr()
         link_attr = self.scrap_link_attr()
         btn_attr = self.scrap_btn_attr()
-        
-        if form_attr: assets_urls = list(set(assets_urls + form_attr))
-        if a_attr: assets_urls = list(set(assets_urls + a_attr))
-        if img_attr: assets_urls = list(set(assets_urls + img_attr))
-        if link_attr: assets_urls = list(set(assets_urls + link_attr))
-        if btn_attr: assets_urls = list(set(assets_urls + btn_attr))
+
+        if form_attr:
+            assets_urls = list(set(assets_urls + form_attr))
+        if a_attr:
+            assets_urls = list(set(assets_urls + a_attr))
+        if img_attr:
+            assets_urls = list(set(assets_urls + img_attr))
+        if link_attr:
+            assets_urls = list(set(assets_urls + link_attr))
+        if btn_attr:
+            assets_urls = list(set(assets_urls + btn_attr))
 
         return assets_urls
 
     # scrap every urls
     def scrap_all_urls(self):
         urls = []
         urls.extend(self.scrap_scripts())
         urls.extend(self.scrap_assets())
         return list(dict.fromkeys(urls))
-    
+
     # convert url to into local path
     def url_to_local_path(self, url, keepQuery=False):
         try:
             new_url = urlparse(url).path
             query = urlparse(url).query
-            if keepQuery and query: new_url += '?' + urlparse(url).query
-            if (new_url[0] == '/') or (new_url[0] == '\\'): new_url = new_url[1:]
+            if keepQuery and query:
+                new_url += "?" + urlparse(url).query
+            if (new_url[0] == "/") or (new_url[0] == "\\"):
+                new_url = new_url[1:]
         except:
             return None
 
         return new_url
 
     # download file from URL
-    def download_file(self, url, output_path):
+    def download_file(self, url, output_path, count=0):
 
         # Remove query string and http from URL
-        url = url.split('?')[0]
-        file_name = url.split('/')[-1]
+        url = url.split("?")[0]
+        file_name = url.split("/")[-1]
 
-        if len(file_name) == 0: return False
+        if len(file_name) == 0:
+            return False
 
         # Create output directory
         if not os.path.exists(os.path.dirname(output_path)):
             os.makedirs(os.path.dirname(output_path))
 
         # Get file content and save it
-        response = session.get(url)
-        with open(output_path, "wb") as file:
-            file.write(response.content)
-            logging.info(f"Downloaded {file_name} to {os.path.relpath(output_path)}")
-        
+        try:
+            response = session.get(url, stream=True)
+            if not response.ok:
+                logging.warning(f"Failed to get resource in URI '{url}'")
+                return True
+            with open(output_path, "wb") as file:
+                for chunk in response.iter_content(chunk_size=2048):
+                    file.write(chunk)
+                logging.info(
+                    f"Downloaded {file_name} to {os.path.relpath(output_path)}"
+                )
+        except requests.exceptions.ConnectionError as e:
+            if count < 1:
+                logging.warning(f"{get_excep(e)} with uri '{url}' retrying once...")
+                count += 1
+                return self.download_file(url, output_path, count)
+            else:
+                logging.error(f"{get_excep(e)} with uri '{url}'")
+
         return True
-    
+
     def save_files(self, urls):
         shutil.rmtree(os.path.join(workspace, output_folder), ignore_errors=True)
         for url in urls:
             output_path = self.url_to_local_path(url, keepQuery=False)
             output_path = os.path.join(workspace, output_folder, output_path)
 
             self.download_file(url, output_path)
-        
+
         return True
-    
+
     # save the HTML file
     def save_html(self):
-        output_path = os.path.join(workspace, output_folder,'index.html')
+        output_path = os.path.join(workspace, output_folder, "index.html")
         prettyHTML = self.soup.prettify()
-        with codecs.open(output_path, 'w', 'utf-8') as file:
+        with codecs.open(output_path, "w", "utf-8") as file:
             file.write(prettyHTML)
             file.close()
             logging.info(f"Saved index.html to {os.path.relpath(output_path)}")
-        
+
         return True
 
+
+def error_handler():
+    def decorator(func):
+        def main(*args, **kwargs):
+            try:
+                return func(*args, **kwargs)
+            except (KeyboardInterrupt, EOFError) as e:
+                logging.warning(f'^{e} - Exitting"')
+            except Exception as e:
+                # logging.exception(e)
+                logging.critical(get_excep(e))
+
+        return main
+
+    return decorator
+
+
+@error_handler()
 def main():
-	import argparse
-	parser = argparse.ArgumentParser(description=__description__)
-	parser.add_argument('host',help="URL pointing to a website")
-	parser.add_argument('-v','---version',action="version",version=f"%(prog)s {__version__}") 
-	parser.add_argument("-tp","--tor-proxy",metavar="PROXY",help="Proxy server url without schema - %(default)s",default="localhost:9050")
-	parser.add_argument("-o","--output",metavar="FOLDER",help="Folder for saving contents - host")
-	parser.add_argument("-w","--workspace",metavar="PATH",help="Directory for saving contents - %(default)s",default=os.getcwd())
-	parser.add_argument('--use-tor',action='store_true',help="Use tor proxy - %(default)s")	
-	args = parser.parse_args()	
-	
-	global url,workspace,get_excep,output_folder,session
-	
-	logging.basicConfig(format="[%(asctime)s : %(levelname)s] - %(message)s",datefmt="%H:%M:%S",level=logging.INFO)
-	# URL of the web page you want to extract data from
-	url = args.host
-	if not url.startswith('http'):
-		url="https://"+url
-	
-	#define workspace from script location
-	workspace = args.workspace	
-	
-	get_excep = lambda e: e.args[1] if len(e.args)>1 else e
-	
-	output_folder = args.output or urlparse(url).netloc
-	# initialize a session
-	session = requests.session()
-	if args.use_tor:
-	   session.request = functools.partial(session.request, timeout=30)
-	   session.proxies = {'http':  f'socks5h://{args.tor_proxy}','https': f'socks5h://{args.tor_proxy}'}
-	   
-	try:
-		logging.info(f"Extracting files from '{url}'")
-		extractor = Extractor(url)
-		extractor.run()
-		logging.info(f"\nTotal extracted files: {len(extractor.scraped_urls)}")
-	except (KeyboardInterrupt,EOFError) as e:
-		logging.warning(f'^{e} - Exitting"')
-	except Exception as e:
-		#logging.exception(e)
-		logging.critical(get_excep(e))
+    import argparse
+
+    parser = argparse.ArgumentParser(description=__description__)
+    parser.add_argument("host", help="URL pointing to a website")
+    parser.add_argument(
+        "-v", "---version", action="version", version=f"%(prog)s {__version__}"
+    )
+    parser.add_argument(
+        "-tp",
+        "--tor-proxy",
+        metavar="PROXY",
+        help="Proxy server url without schema - %(default)s",
+        default="localhost:9050",
+    )
+    parser.add_argument(
+        "-o", "--output", metavar="FOLDER", help="Folder for saving contents - host"
+    )
+    parser.add_argument(
+        "--headers", help="Path to .json file containing request headers"
+    )
+    parser.add_argument(
+        "--browser",
+        help="Browser name to be used - %(default)s",
+        choices=browsers,
+        default="firefox",
+        metavar="|".join(browsers),
+    )
+    parser.add_argument(
+        "--platform",
+        help="OS name to be used - %(default)s",
+        choices=platforms,
+        default="linux",
+        metavar="|".join(platforms),
+    )
+    parser.add_argument(
+        "-w",
+        "--workspace",
+        metavar="PATH",
+        help="Directory for saving contents - %(default)s",
+        default=os.getcwd(),
+    )
+    parser.add_argument(
+        "--use-tor", action="store_true", help="Use tor proxy - %(default)s"
+    )
+    args = parser.parse_args()
+
+    global url, workspace, get_excep, output_folder, session
+
+    logging.basicConfig(
+        format="[%(asctime)s : %(levelname)s] - %(message)s",
+        datefmt="%H:%M:%S",
+        level=logging.INFO,
+    )
+    # URL of the web page you want to extract data from
+    url = args.host
+    if not url.startswith("http"):
+        url = "https://" + url
+
+    # define workspace from script location
+    workspace = args.workspace
+
+    get_excep = lambda e: e.args[1] if len(e.args) > 1 else e
+
+    output_folder = args.output or urlparse(url).netloc
+    # initialize a session
+    session_def = requests.session()
+    if args.use_tor:
+        session_def.request = functools.partial(session.request, timeout=30)
+        session_def.proxies = {
+            "http": f"socks5h://{args.tor_proxy}",
+            "https": f"socks5h://{args.tor_proxy}",
+        }
+
+    if args.headers:
+        from json import load
+
+        with open(args.headers) as fh:
+            session_def.headers = load(fh)
+    else:
+        session_def.headers = {
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+            "User-Agent": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Mobile Safari/537.36",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Accept-Language": "en-US,en;q=0.9",
+        }
+
+    session = cloudscraper.create_scraper(
+        sess=session_def,
+        browser={
+            "browser": args.browser,
+            "platform": args.platform,
+            "desktop": True,
+        },
+    )
+    logging.info(f"Extracting files from '{url}'")
+    extractor = Extractor(url)
+    extractor.run()
+    logging.info(f"Total extracted files: {len(extractor.scraped_urls)}")
+
 
-if __name__=="__main__":
-	main()
+if __name__ == "__main__":
+    main()
```

### Comparing `wclone-1.0.0/wclone.egg-info/PKG-INFO` & `wclone-1.0.1/wclone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wclone
-Version: 1.0.0
+Version: 1.0.1
 Summary: Basic website cloner written in Python
 Home-page: https://github.com/ZKAW/website-cloner
 Author: ZKAW
 Maintainer: Smartwa
 Maintainer-email: smartwacaleb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/ZKAW/website-cloner/issues/new
```

