# Comparing `tmp/biliarchiver-0.0.13.tar.gz` & `tmp/biliarchiver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biliarchiver-0.0.13.tar", max compression
+gzip compressed data, was "biliarchiver-0.0.9.tar", max compression
```

## Comparing `biliarchiver-0.0.13.tar` & `biliarchiver-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0      429 2023-06-06 20:05:41.529385 biliarchiver-0.0.13/README.md
--rw-r--r--   0        0        0     7931 2023-06-09 05:44:19.446941 biliarchiver-0.0.13/biliarchiver/_biliarchiver_upload_bvid.py
--rw-r--r--   0        0        0     7157 2023-06-06 19:12:07.431306 biliarchiver-0.0.13/biliarchiver/archive_bvid.py
--rw-r--r--   0        0        0     6003 2023-06-09 05:59:03.621791 biliarchiver-0.0.13/biliarchiver/bili_archive_bvids.py
--rw-r--r--   0        0        0     4133 2023-06-06 19:45:06.489235 biliarchiver-0.0.13/biliarchiver/bili_get_bvids.py
--rw-r--r--   0        0        0     1490 2023-06-07 12:25:53.093261 biliarchiver-0.0.13/biliarchiver/bili_upload.py
--rw-r--r--   0        0        0     2139 2023-06-07 14:08:15.117924 biliarchiver-0.0.13/biliarchiver/config.py
--rw-r--r--   0        0        0      194 2023-06-09 04:15:33.665307 biliarchiver-0.0.13/biliarchiver/exception.py
--rw-r--r--   0        0        0     2724 2023-06-06 05:53:18.324384 biliarchiver-0.0.13/biliarchiver/utils/dirLock.py
--rw-r--r--   0        0        0      237 2023-06-07 06:29:29.311341 biliarchiver-0.0.13/biliarchiver/utils/ffmpeg.py
--rw-r--r--   0        0        0     1278 2023-06-05 16:41:54.082484 biliarchiver-0.0.13/biliarchiver/utils/string.py
--rw-r--r--   0        0        0       32 2023-06-09 05:48:56.174093 biliarchiver-0.0.13/biliarchiver/version.py
--rw-r--r--   0        0        0      529 2023-06-09 05:49:02.370253 biliarchiver-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 biliarchiver-0.0.13/setup.py
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 biliarchiver-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-06 20:05:41.529385 biliarchiver-0.0.9/README.md
+-rw-r--r--   0        0        0     7575 2023-06-06 19:48:46.123664 biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py
+-rw-r--r--   0        0        0     7157 2023-06-06 19:12:07.431306 biliarchiver-0.0.9/biliarchiver/archive_bvid.py
+-rw-r--r--   0        0        0     4734 2023-06-07 04:48:33.598085 biliarchiver-0.0.9/biliarchiver/bili_archive_bvids.py
+-rw-r--r--   0        0        0     4133 2023-06-06 19:45:06.489235 biliarchiver-0.0.9/biliarchiver/bili_get_bvids.py
+-rw-r--r--   0        0        0     1490 2023-06-07 04:52:11.184454 biliarchiver-0.0.9/biliarchiver/bili_uploade.py
+-rw-r--r--   0        0        0     2018 2023-06-06 19:20:55.302758 biliarchiver-0.0.9/biliarchiver/config.py
+-rw-r--r--   0        0        0     2724 2023-06-06 05:53:18.324384 biliarchiver-0.0.9/biliarchiver/utils/dirLock.py
+-rw-r--r--   0        0        0     1278 2023-06-05 16:41:54.082484 biliarchiver-0.0.9/biliarchiver/utils/string.py
+-rw-r--r--   0        0        0       31 2023-06-06 19:35:41.648702 biliarchiver-0.0.9/biliarchiver/version.py
+-rw-r--r--   0        0        0      530 2023-06-07 04:58:02.482737 biliarchiver-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/setup.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/PKG-INFO
```

### Comparing `biliarchiver-0.0.13/biliarchiver/_biliarchiver_upload_bvid.py` & `biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 import json
 import os
 from pathlib import Path
 import time
 from internetarchive import get_item
 from requests import Response
 from rich import print
-from biliarchiver.exception import VideosBasePathNotFoundError
 
 from biliarchiver.utils.string import human_readable_upper_part_map
 from biliarchiver.config import BILIBILI_IDENTIFIER_PERFIX, config
 from biliarchiver.utils.dirLock import UploadLock, AlreadyRunningError
 from biliarchiver.version import BILI_ARCHIVER_VERSION
 
 def upload_bvid(bvid):
     try:
         lock_dir = config.storage_home_dir / '.locks' / bvid
         os.makedirs(lock_dir, exist_ok=True)
         with UploadLock(lock_dir): # type: ignore
             _upload_bvid(bvid)
     except AlreadyRunningError:
         print(f'已经有一个上传 {bvid} 的进程在运行，跳过')
-    except VideosBasePathNotFoundError:
-        print(f'没有找到 {bvid} 对应的文件夹。可能是因已存在 IA item 而跳过了下载，或者你传入了错误的 bvid')
     except Exception as e:
         print(f'上传 {bvid} 时出错：')
         raise e
 
 def _upload_bvid(bvid: str):
     access_key, secret_key = read_ia_keys(config.ia_key_file)
 
     # identifier format: BiliBili-{bvid}_p{pid}-{upper_part} 
     upper_part = human_readable_upper_part_map(string=bvid, backward=True)
     OLD_videos_basepath: Path = config.storage_home_dir / 'videos' / bvid
     videos_basepath: Path = config.storage_home_dir / 'videos' / f'{bvid}-{upper_part}'
-
     if os.path.exists(OLD_videos_basepath):
         print(f'检测到旧的视频主目录 {OLD_videos_basepath}，将其重命名为 {videos_basepath}...')
         os.rename(OLD_videos_basepath, videos_basepath)
-
-    if not os.path.exists(videos_basepath):
-        raise VideosBasePathNotFoundError(f'{videos_basepath}')
     for local_identifier in os.listdir(videos_basepath):
         remote_identifier = f'{local_identifier}-{upper_part}'
         if os.path.exists(f'{videos_basepath}/{local_identifier}/_uploaded.mark'):
             print(f'{local_identifier} => {remote_identifier} 已经上传过了(_uploaded.mark)')
             continue
         if local_identifier.startswith('_') :
             print(f'跳过 {local_identifier}')
```

### Comparing `biliarchiver-0.0.13/biliarchiver/archive_bvid.py` & `biliarchiver-0.0.9/biliarchiver/archive_bvid.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.13/biliarchiver/bili_archive_bvids.py` & `biliarchiver-0.0.9/biliarchiver/bili_archive_bvids.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,78 @@
 import asyncio
 import os
 import argparse
-from pathlib import Path
-from typing import Union
-
-from internetarchive import get_item
 
 from biliarchiver.archive_bvid import archive_bvid
-from biliarchiver.config import config
+from biliarchiver.config import Config
 
 from bilix.sites.bilibili.downloader import DownloaderBilibili
 from rich.console import Console
 from httpx import AsyncClient, Client
 from rich.traceback import install
-install()
 
 from biliarchiver.utils.string import human_readable_upper_part_map
-from biliarchiver.utils.ffmpeg import check_ffmpeg
+install()
 
 from biliarchiver.config import BILIBILI_IDENTIFIER_PERFIX
 
 from dataclasses import dataclass
 
 @dataclass
 class Args:
+    cookies: str
     bvids: str
     skip_ia: bool
 
 def parse_args():
 
     parser = argparse.ArgumentParser()
+    parser.add_argument('--cookies', dest='cookies', type=str, default='~/.cookies.txt')
     parser.add_argument('--bvids', dest='bvids', type=str, help='bvids 列表的文件路径', required=True)
     parser.add_argument('-s', '--skip-ia-check', dest='skip_ia', action='store_true',
                         help='不检查 IA 上是否已存在对应 BVID 的 item ，直接开始下载')
     
     args = Args(**vars(parser.parse_args()))
 
     return args
 
 def check_ia_item_exist(client: Client, identifier: str) -> bool:
-    cache_dir = config.storage_home_dir / 'ia_item_exist_cache'
-    cache_dir.mkdir(parents=True, exist_ok=True)
-    def create_item_exist_cache_file(identifier: str) -> Path:
-        with open(cache_dir / f'{identifier}.mark', 'w', encoding='utf-8') as f:
-            f.write('')
-        return cache_dir / f'{identifier}.mark'
-    def check_ia_item_exist_from_cache_file(identifier: str) -> bool:
-        return (cache_dir / f'{identifier}.mark').exists()
-
-
-    if check_ia_item_exist_from_cache_file(identifier):
-        return True
-
-    # params = {
-    #     'identifier': identifier,
-    #     'output': 'json',
-    # }
-    # r = client.get('https://archive.org/services/check_identifier.php' ,params=params)
-    # r.raise_for_status()
-    # r_json = r.json()
-    # assert r_json['type'] =='success'
-    # if r_json['code'] == 'available':
-    #     return False
-    # elif r_json['code'] == 'not_available':
-    #     return True
-    # else:
-    #     raise ValueError(f'Unexpected code: {r_json["code"]}')
-    item = get_item(identifier)
-    if item.exists:
-        create_item_exist_cache_file(identifier)
+    params = {
+        'identifier': identifier,
+        'output': 'json',
+    }
+    r = client.get('https://archive.org/services/check_identifier.php' ,params=params)
+    r.raise_for_status()
+    r_json = r.json()
+    assert r_json['type'] =='success'
+    if r_json['code'] == 'available':
+        return False
+    elif r_json['code'] == 'not_available':
         return True
-
-    return False
+    else:
+        raise ValueError(f'Unexpected code: {r_json["code"]}')
 
 def _main():
     args = parse_args()
-    assert check_ffmpeg() is True, 'ffmpeg 未安装'
 
     assert args.bvids is not None, '必须指定 bvids 列表的文件路径'
     with open(args.bvids, 'r', encoding='utf-8') as f:
         bvids_from_file = f.read().splitlines()
 
+    config = Config()
+
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
 
     d = DownloaderBilibili(hierarchy=True, sess_data=None, # sess_data 将在后面装载 cookies 时装载 # type: ignore
         video_concurrency=config.video_concurrency,
         part_concurrency=config.part_concurrency,
         stream_retry=config.stream_retry,
     )
-    update_cookies_from_file(d.client, config.cookies_file)
+    update_cookies_from_file(d.client, args.cookies)
     client = Client(cookies=d.client.cookies, headers=d.client.headers)
     logined = is_login(client)
     if not logined:
         return
 
     d.progress.start()
     for index, bvid in enumerate(bvids_from_file):
@@ -112,52 +91,44 @@
         task = loop.create_task(archive_bvid(d, bvid, logined=logined))
     
     while len(asyncio.all_tasks(loop)) > 0:
         loop.run_until_complete(asyncio.sleep(1))
     
 
 
-def update_cookies_from_file(client: AsyncClient, cookies_path: Union[str, Path]):
-    if isinstance(cookies_path, Path):
-        cookies_path = cookies_path.expanduser()
-    elif isinstance(cookies_path, str):
-        cookies_path = Path(cookies_path).expanduser()
-    else:
-        raise TypeError(f'cookies_path: {type(cookies_path)}')
-
+def update_cookies_from_file(client: AsyncClient, cookies_path: str):
+    cookies_path = os.path.expanduser(cookies_path)
     assert os.path.exists(cookies_path), f'cookies 文件不存在: {cookies_path}'
     from http.cookiejar import MozillaCookieJar
     cj = MozillaCookieJar()
-    cj.load(f'{cookies_path}', ignore_discard=True, ignore_expires=True)
+    cj.load(cookies_path, ignore_discard=True, ignore_expires=True)
     loadded_cookies = 0
     for cookie in cj:
         # only load bilibili cookies
         if 'bilibili' in cookie.domain:
             assert cookie.value is not None
             client.cookies.set(
                 cookie.name, cookie.value, domain=cookie.domain, path=cookie.path
                 )
             loadded_cookies += 1
-    print(f'从 {cookies_path} 品尝了 {loadded_cookies} 块 cookies')
+    print(f'从 {cookies_path} 加载了 {loadded_cookies} 块 cookies')
     if loadded_cookies > 100:
-        print('吃了过多的 cookies，可能导致 httpx.Client 怠工，响应非常缓慢')
+        print('可能加载了过多的 cookies，可能导致 httpx.Client 响应非常慢')
 
     assert client.cookies.get('SESSDATA') is not None, 'SESSDATA 不存在'
     # print(f'SESS_DATA: {client.cookies.get("SESSDATA")}')
 
 def is_login(cilent: Client) -> bool:
     r = cilent.get('https://api.bilibili.com/x/member/web/account')
     r.raise_for_status()
     nav_json = r.json()
     if nav_json['code'] == 0:
-        print('BiliBili 登录成功，饼干真香。')
-        print('NOTICE: 存档过程中请不要在 cookies 的源浏览器访问 B 站，避免 B 站刷新'
-              ' cookies 导致我们半路全下到的视频全是 480P 的优酷土豆级醇享画质。')
+        print('用户登录成功')
         return True
-    print('未登录/SESSDATA无效/过期，你这饼干它保真吗？')
+    print('未登录/SESSDATA无效/过期')
     return False
 
 def main():
     try:
         _main()
     except KeyboardInterrupt:
         print('KeyboardInterrupt')
```

### Comparing `biliarchiver-0.0.13/biliarchiver/bili_get_bvids.py` & `biliarchiver-0.0.9/biliarchiver/bili_get_bvids.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.13/biliarchiver/bili_upload.py` & `biliarchiver-0.0.9/biliarchiver/bili_uploade.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.13/biliarchiver/config.py` & `biliarchiver-0.0.9/biliarchiver/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,28 @@
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 @dataclass
-class _Config(metaclass=singleton):
+class Config(metaclass=singleton):
     video_concurrency: int = 3 
     part_concurrency: int = 10
     stream_retry: int = 20
     storage_home_dir: Path = Path('bilibili_archive_dir/').expanduser()
     ia_key_file: Path = Path('~/.bili_ia_keys.txt').expanduser()
-    cookies_file: Path = Path('~/.cookies.txt').expanduser()
 
     def __init__(self):
         self.is_right_pwd()
         if not os.path.exists(CONFIG_FILE):
             print(f'{CONFIG_FILE} 不存在，创建中...')
             self.save()
         with open(CONFIG_FILE, 'r', encoding='utf-8') as f:
-            print(f'Loading {CONFIG_FILE} ...')
+            print(f'读取 {CONFIG_FILE}...')
             config_file = json.load(f)
 
         self.video_concurrency: int = config_file['video_concurrency']
         self.part_concurrency: int = config_file['part_concurrency']
         self.stream_retry: int = config_file['stream_retry']
 
         self.storage_home_dir: Path = Path(config_file['storage_home_dir']).expanduser()
@@ -44,15 +43,14 @@
         with open(CONFIG_FILE, 'w', encoding='utf-8') as f:
             json.dump({
                 'video_concurrency': self.video_concurrency,
                 'part_concurrency': self.part_concurrency,
                 'stream_retry': self.stream_retry,
                 'storage_home_dir': str(self.storage_home_dir),
                 'ia_key_file': str(self.ia_key_file),
-                'cookies_file': str(self.cookies_file),
             }, f, ensure_ascii=False, indent=4)
 
     def is_right_pwd(self):
         if not os.path.exists('biliarchiver.home'):
             raise Exception('先在当前工作目录创建 biliarchiver.home 文件')
 
-config = _Config()
+config = Config()
```

### Comparing `biliarchiver-0.0.13/biliarchiver/utils/dirLock.py` & `biliarchiver-0.0.9/biliarchiver/utils/dirLock.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.13/biliarchiver/utils/string.py` & `biliarchiver-0.0.9/biliarchiver/utils/string.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.13/pyproject.toml` & `biliarchiver-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "biliarchiver"
-version = "0.0.13"
+version = "0.0.9"
 description = ""
 authors = ["yzqzss <yzqzss@yandex.com>"]
 readme = "README.md"
 packages = [{include = "biliarchiver"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bilix = "0.18.3"
 internetarchive = "^3.5.0"
 
 [tool.poetry.scripts]
 bili_archive_bvids = "biliarchiver:bili_archive_bvids.main"
-bili_upload = "biliarchiver:bili_upload.main"
+bili_uploade = "biliarchiver:bili_uploade.main"
 bili_get_bvids = "biliarchiver:bili_get_bvids.main"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `biliarchiver-0.0.13/setup.py` & `biliarchiver-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 install_requires = \
 ['bilix==0.18.3', 'internetarchive>=3.5.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['bili_archive_bvids = '
                      'biliarchiver:bili_archive_bvids.main',
                      'bili_get_bvids = biliarchiver:bili_get_bvids.main',
-                     'bili_upload = biliarchiver:bili_upload.main']}
+                     'bili_uploade = biliarchiver:bili_uploade.main']}
 
 setup_kwargs = {
     'name': 'biliarchiver',
-    'version': '0.0.13',
+    'version': '0.0.9',
     'description': '',
     'long_description': '# biliarchiver\n\n## 基于 bilix 的 BiliBili 存档工具\n\n~~ IA iteam identifier 格式兼容 tubeup ~~。  \n现在不兼容了，Tubeup 不适合存 B 站视频，它的 identifier 设计不科学，大规模存档必定会撞车。\n\n目前，我可能随时 commit 乱飞且动不动就 git push -f 这个仓库。（为了在我的 vps 和本地之间同步代码）\n\nuserscript.js 还没适配新换的 identifier 格式。\n',
     'author': 'yzqzss',
     'author_email': 'yzqzss@yandex.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `biliarchiver-0.0.13/PKG-INFO` & `biliarchiver-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biliarchiver
-Version: 0.0.13
+Version: 0.0.9
 Summary: 
 Author: yzqzss
 Author-email: yzqzss@yandex.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

