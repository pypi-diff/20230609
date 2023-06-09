# Comparing `tmp/nonebot_plugin_manga_translator-0.1.2.tar.gz` & `tmp/nonebot_plugin_manga_translator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_manga_translator-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_manga_translator-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_manga_translator-0.1.2.tar` & `nonebot_plugin_manga_translator-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/LICENSE
--rw-r--r--   0        0        0     7701 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/README.md
--rw-r--r--   0        0        0     3999 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/nonebot_plugin_manga_translator/__init__.py
--rw-r--r--   0        0        0     8774 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/nonebot_plugin_manga_translator/utils.py
--rw-r--r--   0        0        0      529 2023-05-02 16:20:44.784722 nonebot_plugin_manga_translator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8499 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/LICENSE
+-rw-r--r--   0        0        0     8272 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/README.md
+-rw-r--r--   0        0        0     4167 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/nonebot_plugin_manga_translator/__init__.py
+-rw-r--r--   0        0        0     8819 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/nonebot_plugin_manga_translator/utils.py
+-rw-r--r--   0        0        0      529 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9070 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_manga_translator-0.1.2/LICENSE` & `nonebot_plugin_manga_translator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_manga_translator-0.1.2/README.md` & `nonebot_plugin_manga_translator-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,29 @@
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
 # nonebot-plugin-manga-translator
 
 ✨*基于Nonebot2的图片/漫画翻译插件*✨
-  
+
+<a href="https://github.com/nonebot/nonebot2">
+  <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
+</a> 
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/maoxig/nonebot-plugin-manga-translator" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-manga-translator">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-manga-translator" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+
 <div align="left">
-  
+
 ## 💿安装
 通过`pip`或`nb`安装；
 
 - 使用nb:
   在机器人目录下命令行使用
   `nb plugin install nonebot_plugin_manga_translator`
 - 使用pip(不推荐):
@@ -26,15 +38,15 @@
 
 请在机器人目录下的.env.*里填写以下选项(至少填一个平台的)，获取方式已整理好，见下方
 
 ~~个人感觉就漫画翻译而言,这几家API的效果大致为有道>=百度≈离线>=火山,且火山翻译对竖版日文的翻译效果很差~~
 
 |          配置项           | 类型  | 默认值 |                示例                 | 说明              | API定价                                           |
 | :-----------------------: | :---: | :----: | :---------------------------------: | :---------------- | :------------------------------------------------ |
-|        有道翻译API        |   -   |   -    |                  -                  | -                 | 梯度收费，0<月调用量<100w时,0.04元/张                   |
+|        有道翻译API        |   -   |   -    |                  -                  | -                 | 新用户送一定额度,梯度收费，0<月调用量<100w时,0.04元/张                   |
 |      youdao_app_key       |  str  |   ""   |       youdao_app_key="xxxxx"        | 应用ID            |                                                   |
 |     youdao_app_secret     |  str  |   ""   |     youdao_app_secret="xxxxxx"      | 应用秘钥          |                                                   |
 |        百度翻译API        |   -   |   -    |                  -                  | -                 | 每月1万次免费调用量，之后按梯度收费,最高0.04元/次 |
 |       baidu_app_id        |  str  |   ""   |        baidu_app_id="66666"         | APP ID            |                                                   |
 |       baidu_app_key       |  str  |   ""   |       baidu_app_key="xxxxxx"        | 密钥              |                                                   |
 |        火山翻译API        |   -   |   -    |                  -                  | -                 | 每月前100张免费，之后0.04元/张                    |
 |   huoshan_access_key_id   |  str  |   ""   |    huoshan_access_key_id="AK***"    | Access Key ID     |                                                   |
@@ -77,15 +89,16 @@
 <summary>离线翻译</summary>
 (该方案对设备配置要求较高，建议在有足够的硬盘空间、内存、显存，或有一台能为bot处理请求的服务器时考虑使用该方案)
 
    1. 参考[manga-image-translator](https://github.com/zyddnys/manga-image-translator)的说明，克隆仓库，并安装相关依赖(可能需要额外安装`pydensecrf`)
    2. 安装好依赖后，在仓库目录下运行
 
       ```python
-      python -m manga_translator -v --mode web --use-cuda# the demo will be serving on http://127.0.0.1:5003
+      python -m manga_translator -v --mode web --use-cuda
+      # the demo will be serving on http://127.0.0.1:5003
       ```
 
    3. 如果你的设备没有成功安装cuda(要求pytorch的版本和cuda对应，不对应请重装)，请去掉参数`--use-cuda`，如果图片处理过程中爆显存，请改成`--use-cuda-limited`
 
    4. 你可以访问控制台给出的网址，尝试先本地翻译一张图片，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
    5. 如果bot和翻译器在同一台设备，那么.env填写`offline_url="http://127.0.0.1:5003"`即可，如果不在同一台设备，你**可能**还需要放行防火墙、端口转发等，并且填写内容也会有所变化
    6. 最后你**可能**还需要修改一下本插件的代码，找到本插件`utils.py`的`offline`函数，根据注释和[文档](https://github.com/zyddnys/manga-image-translator/blob/main/README.md),修改字典`data`，从而指定你想要的OCR模型和翻译模型(目前是用了offline模型,你可以改成别的)
@@ -116,14 +129,18 @@
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图4.PNG" width="300" height="300">
 
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
+- 2023-06-09:
+
+  - 更新插件元数据
+
 - 2023-05-03:
 
   - 更新说明文档
   - 适配[火山翻译api](https://translate.volcengine.com/api),你可以选择接入火山翻译提供的API
 
 - 2023-05-01:
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
                                    [nonebot]
         # nonebot-plugin-manga-translator â¨*åºäºNonebot2çå¾ç/
-                            æ¼«ç»ç¿»è¯æä»¶*â¨
+          æ¼«ç»ç¿»è¯æä»¶*â¨ [nonebot] [license] [pypi] [python]
 ## ð¿å®è£ éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb:
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨ `nb plugin install
 nonebot_plugin_manga_translator` - ä½¿ç¨pip(ä¸æ¨è):
 ~~ä¸æ¨èå°±æ¯ä¸æ¨èï¼ç¥ç¥ç¥~~ ## ðç®ä» 1.
 ééå¤ç§api,å°æ¶å°çå¾çç¿»è¯å¹¶åéç¿»è¯åçå¾çï¼æ¯ææ¹éæä½
 2. âï¸æä»¶éç½® è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
 (è³å°å¡«ä¸ä¸ªå¹³å°ç)ï¼è·åæ¹å¼å·²æ´çå¥½ï¼è§ä¸æ¹
 ~~ä¸ªäººæè§å°±æ¼«ç»ç¿»è¯èè¨,è¿å å®¶APIçææå¤§è´ä¸ºæé>=ç¾åº¦âç¦»çº¿>=ç«å±±,ä¸ç«å±±ç¿»è¯å¯¹ç«çæ¥æçç¿»è¯ææå¾å·®~~
 | éç½®é¡¹ | ç±»å | é»è®¤å¼ | ç¤ºä¾ | è¯´æ | APIå®ä»· | | :-----------
 ------------: | :---: | :----: | :---------------------------------: | :-------
 --------- | :------------------------------------------------ | |
 æéç¿»è¯API | - | - | - | - |
-æ¢¯åº¦æ¶è´¹ï¼0<æè°ç¨é<100wæ¶,0.04å/å¼  | | youdao_app_key | str | ""
-| youdao_app_key="xxxxx" | åºç¨ID | | | youdao_app_secret | str | "" |
-youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | | | ç¾åº¦ç¿»è¯API | - | - | - | -
-| æ¯æ1ä¸æ¬¡åè´¹è°ç¨éï¼ä¹åææ¢¯åº¦æ¶è´¹,æé«0.04å/æ¬¡ | |
+æ°ç¨æ·éä¸å®é¢åº¦,æ¢¯åº¦æ¶è´¹ï¼0<æè°ç¨é<100wæ¶,0.04å/å¼  | |
+youdao_app_key | str | "" | youdao_app_key="xxxxx" | åºç¨ID | | |
+youdao_app_secret | str | "" | youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | | |
+ç¾åº¦ç¿»è¯API | - | - | - | - |
+æ¯æ1ä¸æ¬¡åè´¹è°ç¨éï¼ä¹åææ¢¯åº¦æ¶è´¹,æé«0.04å/æ¬¡ | |
 baidu_app_id | str | "" | baidu_app_id="66666" | APP ID | | | baidu_app_key |
 str | "" | baidu_app_key="xxxxxx" | å¯é¥ | | | ç«å±±ç¿»è¯API | - | - | - |
 - | æ¯æå100å¼ åè´¹ï¼ä¹å0.04å/å¼  | | huoshan_access_key_id | str |
 "" | huoshan_access_key_id="AK***" | Access Key ID | | |
 huoshan_secret_access_key | str | "" | huoshan_secret_access_key="UT**" |
 Secret Access Key | | | ç¦»çº¿ç¿»è¯API | - | - | - | - | å¯è½æ¯çµè´¹? | |
 offline_url | str | "" | offline_url="http://127.0.0.1:5003" | è§ä¸æ¹è¯´æ
@@ -41,16 +42,16 @@
 Key`ï¼ç¶åç¹å»`Secret Access Key`ä¸çæé®æ¾ç¤ºåºå¯é¥ 3.
 åå«æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶   ç¦»çº¿ç¿»è¯
 (è¯¥æ¹æ¡å¯¹è®¾å¤éç½®è¦æ±è¾é«ï¼å»ºè®®å¨æè¶³å¤çç¡¬çç©ºé´ãåå­ãæ¾å­ï¼ææä¸å°è½ä¸ºbotå¤çè¯·æ±çæå¡å¨æ¶èèä½¿ç¨è¯¥æ¹æ¡)
 1. åè[manga-image-translator](https://github.com/zyddnys/manga-image-
 translator)çè¯´æï¼åéä»åºï¼å¹¶å®è£ç¸å³ä¾èµ
 (å¯è½éè¦é¢å¤å®è£`pydensecrf`) 2.
 å®è£å¥½ä¾èµåï¼å¨ä»åºç®å½ä¸è¿è¡ ```python python -
-m manga_translator -v --mode web --use-cuda# the demo will be serving on http:/
-/127.0.0.1:5003 ``` 3. å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
+m manga_translator -v --mode web --use-cuda # the demo will be serving on http:
+//127.0.0.1:5003 ``` 3. å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
 (è¦æ±pytorchççæ¬åcudaå¯¹åºï¼ä¸å¯¹åºè¯·éè£)ï¼è¯·å»æåæ°`--
 use-cuda`ï¼å¦æå¾çå¤çè¿ç¨ä¸­çæ¾å­ï¼è¯·æ¹æ`--use-cuda-
 limited` 4.
 ä½ å¯ä»¥è®¿é®æ§å¶å°ç»åºçç½åï¼å°è¯åæ¬å°ç¿»è¯ä¸å¼ å¾çï¼æ­¤æ¶ä¼æ ¹æ®éé¡¹ä¸è½½éè¦çæ¨¡å
 (ä¸ºé²æ­¢ä¸è½½å¤±è´¥ï¼ä¹å¯ä»¥æåæå¨ä¸è½½) 5.
 å¦æbotåç¿»è¯å¨å¨åä¸å°è®¾å¤ï¼é£ä¹.envå¡«å`offline_url="http://
 127.0.0.1:
@@ -67,18 +68,18 @@
 1. åæå­ï¼åå¤å¼ å¾ç 2. æå­+å¾ç*n 3. åæ¢ç¿»è¯api [api]:
 å°è¯¥apiä¼åçº§æå°æé«ï¼ç®åæ`youdao baidu huoshan offline`
 æªå®å¾ç»­ ## â­ææå¾ [https://github.com/maoxig/nonebot-plugin-manga-
 translator/blob/main/resource/ææå¾1.jpg] [https://github.com/maoxig/
 nonebot-plugin-manga-translator/blob/main/resource/ææå¾2.jpg] [https://
 github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
 ææå¾3.jpg] [https://github.com/maoxig/nonebot-plugin-manga-translator/
-blob/main/resource/ææå¾4.PNG] ## ðæ´æ°æ¥å¿  ç¹å»å±å¼ - 2023-05-
-03: - æ´æ°è¯´æææ¡£ - éé[ç«å±±ç¿»è¯api](https://
-translate.volcengine.com/api),ä½ å¯ä»¥éæ©æ¥å¥ç«å±±ç¿»è¯æä¾çAPI -
-2023-05-01: -
+blob/main/resource/ææå¾4.PNG] ## ðæ´æ°æ¥å¿  ç¹å»å±å¼ - 2023-06-
+09: - æ´æ°æä»¶åæ°æ® - 2023-05-03: - æ´æ°è¯´æææ¡£ - éé
+[ç«å±±ç¿»è¯api](https://translate.volcengine.com/
+api),ä½ å¯ä»¥éæ©æ¥å¥ç«å±±ç¿»è¯æä¾çAPI - 2023-05-01: -
 æ·»å åæ¢apiçåè½ï¼ä½ å¯ä»¥å°æä¸ªapiä¼åçº§è®¾ä¸ºæé« -
 ééç¦»çº¿ç¿»è¯api[manga-image-translator](https://github.com/zyddnys/manga-
 image-translator),ç°å¨ä½ å¯ä»¥ä½éªæ¬å°çç¿»è¯ - 2023-04-28: -
 æä»¶åå¸  ## ð¦è®¡å - [x] ééç¦»çº¿ç¿»è¯æ¨¡å[manga-image-
 translator](https://github.com/zyddnys/manga-image-translator) - [x]
 æ¯ææ´å¤API - [ ] å®åæä»¶ ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

### Comparing `nonebot_plugin_manga_translator-0.1.2/nonebot_plugin_manga_translator/__init__.py` & `nonebot_plugin_manga_translator-0.1.3/nonebot_plugin_manga_translator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from nonebot.exception import MatcherException
 from nonebot.params import CommandArg,Arg,ArgPlainText
 from nonebot.plugin import PluginMetadata
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot import on_command,logger,get_driver
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent,helpers,MessageSegment,Message,GroupMessageEvent
-from .utils import MangaTranslator 
+from .utils import MangaTranslator,Config
 
 __plugin_meta__ = PluginMetadata(
     name="图片翻译",
     description="利用api翻译图片并返回翻译后的图片",
     usage="""指令：
         图片翻译 [图片] --翻译并返回翻译后的图片
         多图片翻译 [图片]*n --翻译并返回多张翻译后的图片
         切换翻译api [api] --将该api的优先级设为最高
 """,
+    type="application",
+    homepage="https://github.com/maoxig/nonebot-plugin-manga-translator",
+    config=Config,
+    supported_adapters={"~onebot.v11"},
+    
 )
 
 pictrans= on_command("图片翻译", priority=5, block=False,aliases={"翻译图片"})
 mul_pictrans=on_command("多图片翻译",priority=5,block=False)
 api_change=on_command("翻译api切换",priority=5,aliases={"翻译API切换","切换翻译api","切换翻译API"})
 
 manga_trans=MangaTranslator(get_driver().config.dict())
```

### Comparing `nonebot_plugin_manga_translator-0.1.2/nonebot_plugin_manga_translator/utils.py` & `nonebot_plugin_manga_translator-0.1.3/nonebot_plugin_manga_translator/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             logger.info("检测到火山API")
             
     async def call_api(self,imageUrl):
         for api in self.api:
             try:
                 result=await api(imageUrl)
                 return result
-            except Exception as e:
+            except httpx.HTTPError as e:
                 logger.warning(f"API[{api.__name__}]不可用：{e}尝试切换下一个")
         return None,"无可用API"
    
  
     async def youdao(self,imageUrl):
         """有道翻译"""
         salt = str(uuid.uuid1())
@@ -93,15 +93,15 @@
             baidu_res=await client.post(url='http://api.fanyi.baidu.com/api/trans/sdk/picture',params=payload,files=image)
             img_base64=baidu_res.json()["data"]["pasteImg"]
             pic=base64.b64decode(img_base64)
         return pic,"百度"
     
 
     async def offline(self, imgUrl, timeout=60):
-        """离线翻译"""
+        """离线翻译,这里写的有点烂，求pr"""
         async with httpx.AsyncClient() as client:
             res = await client.get(imgUrl)
             img_content = res.content
             form = {"file": ("image.png", img_content, 'image/png')}
             response = await client.post(self.config.offline_url + "/submit", files=form,data={"translator":"offline"})#改为本地翻译器
             #这里的填写请参考文档，根据自己情况填写，例如data={"translator":"youdao","tgt_lang":"CHS"},如果是有道、百度、gpt等，请确保填写了key
             response.raise_for_status()  # 检查响应状态
@@ -124,15 +124,15 @@
             if img_data.status_code == 200 and img_data.content:
                 return img_data.content, "离线"
             else:
                 return None, "离线"
 
 
     async def huoshan(self,imageUrl):
-        """火山引擎翻译，90%在构建签名"""
+        """火山引擎翻译，构建签名"""
         async with httpx.AsyncClient() as client:
             res=await client.get(imageUrl)
             data=json.dumps({"Image":str(base64.b64encode(res.content),encoding='utf-8'),'TargetLanguage': "zh"})
             x_content_sha256=self.hash_sha256(data)
             now_time=datetime.datetime.utcnow()#
             x_date=now_time.strftime("%Y%m%dT%H%M%SZ")
             credential_scope = "/".join([x_date[:8], "cn-north-1", 'translate', "request"])
@@ -175,24 +175,27 @@
             return input.getvalue()
         
     @staticmethod
     def encrypt(signStr):
         hash_algorithm = md5()
         hash_algorithm.update(signStr.encode('utf-8'))
         return hash_algorithm.hexdigest()
+    
     @staticmethod
     def hash_sha256(content: str):
         return hashlib.sha256(content.encode("utf-8")).hexdigest()
+    
     @staticmethod
     def norm_query(params):
         query = ""
         for key in sorted(params.keys()):
             if type(params[key]) == list:
                 for k in params[key]:
                     query = (query + quote(key, safe="-_.~") + "=" + quote(k, safe="-_.~") + "&")
             else:
                 query = (query + quote(key, safe="-_.~") + "=" + quote(params[key], safe="-_.~") + "&")
         query = query[:-1]
         return query.replace("+", "%20")
+    
     @staticmethod
     def hmac_sha256(key: bytes, content: str):
         return hmac.new(key, content.encode("utf-8"), hashlib.sha256).digest()
```

### Comparing `nonebot_plugin_manga_translator-0.1.2/pyproject.toml` & `nonebot_plugin_manga_translator-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-manga-translator"
-version = "0.1.2"
+version = "0.1.3"
 description = "基于nonebot2的适配多种api的图片/漫画翻译插件"
 authors = ["xenophon <674550338@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_manga_translator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_manga_translator-0.1.2/PKG-INFO` & `nonebot_plugin_manga_translator-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-manga-translator
-Version: 0.1.2
+Version: 0.1.3
 Summary: 基于nonebot2的适配多种api的图片/漫画翻译插件
 License: MIT
 Author: xenophon
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,17 +23,29 @@
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
 # nonebot-plugin-manga-translator
 
 ✨*基于Nonebot2的图片/漫画翻译插件*✨
-  
+
+<a href="https://github.com/nonebot/nonebot2">
+  <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
+</a> 
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/maoxig/nonebot-plugin-manga-translator" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-manga-translator">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-manga-translator" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+
 <div align="left">
-  
+
 ## 💿安装
 通过`pip`或`nb`安装；
 
 - 使用nb:
   在机器人目录下命令行使用
   `nb plugin install nonebot_plugin_manga_translator`
 - 使用pip(不推荐):
@@ -47,15 +59,15 @@
 
 请在机器人目录下的.env.*里填写以下选项(至少填一个平台的)，获取方式已整理好，见下方
 
 ~~个人感觉就漫画翻译而言,这几家API的效果大致为有道>=百度≈离线>=火山,且火山翻译对竖版日文的翻译效果很差~~
 
 |          配置项           | 类型  | 默认值 |                示例                 | 说明              | API定价                                           |
 | :-----------------------: | :---: | :----: | :---------------------------------: | :---------------- | :------------------------------------------------ |
-|        有道翻译API        |   -   |   -    |                  -                  | -                 | 梯度收费，0<月调用量<100w时,0.04元/张                   |
+|        有道翻译API        |   -   |   -    |                  -                  | -                 | 新用户送一定额度,梯度收费，0<月调用量<100w时,0.04元/张                   |
 |      youdao_app_key       |  str  |   ""   |       youdao_app_key="xxxxx"        | 应用ID            |                                                   |
 |     youdao_app_secret     |  str  |   ""   |     youdao_app_secret="xxxxxx"      | 应用秘钥          |                                                   |
 |        百度翻译API        |   -   |   -    |                  -                  | -                 | 每月1万次免费调用量，之后按梯度收费,最高0.04元/次 |
 |       baidu_app_id        |  str  |   ""   |        baidu_app_id="66666"         | APP ID            |                                                   |
 |       baidu_app_key       |  str  |   ""   |       baidu_app_key="xxxxxx"        | 密钥              |                                                   |
 |        火山翻译API        |   -   |   -    |                  -                  | -                 | 每月前100张免费，之后0.04元/张                    |
 |   huoshan_access_key_id   |  str  |   ""   |    huoshan_access_key_id="AK***"    | Access Key ID     |                                                   |
@@ -98,15 +110,16 @@
 <summary>离线翻译</summary>
 (该方案对设备配置要求较高，建议在有足够的硬盘空间、内存、显存，或有一台能为bot处理请求的服务器时考虑使用该方案)
 
    1. 参考[manga-image-translator](https://github.com/zyddnys/manga-image-translator)的说明，克隆仓库，并安装相关依赖(可能需要额外安装`pydensecrf`)
    2. 安装好依赖后，在仓库目录下运行
 
       ```python
-      python -m manga_translator -v --mode web --use-cuda# the demo will be serving on http://127.0.0.1:5003
+      python -m manga_translator -v --mode web --use-cuda
+      # the demo will be serving on http://127.0.0.1:5003
       ```
 
    3. 如果你的设备没有成功安装cuda(要求pytorch的版本和cuda对应，不对应请重装)，请去掉参数`--use-cuda`，如果图片处理过程中爆显存，请改成`--use-cuda-limited`
 
    4. 你可以访问控制台给出的网址，尝试先本地翻译一张图片，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
    5. 如果bot和翻译器在同一台设备，那么.env填写`offline_url="http://127.0.0.1:5003"`即可，如果不在同一台设备，你**可能**还需要放行防火墙、端口转发等，并且填写内容也会有所变化
    6. 最后你**可能**还需要修改一下本插件的代码，找到本插件`utils.py`的`offline`函数，根据注释和[文档](https://github.com/zyddnys/manga-image-translator/blob/main/README.md),修改字典`data`，从而指定你想要的OCR模型和翻译模型(目前是用了offline模型,你可以改成别的)
@@ -137,14 +150,18 @@
 <img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图4.PNG" width="300" height="300">
 
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
+- 2023-06-09:
+
+  - 更新插件元数据
+
 - 2023-05-03:
 
   - 更新说明文档
   - 适配[火山翻译api](https://translate.volcengine.com/api),你可以选择接入火山翻译提供的API
 
 - 2023-05-01:
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.1.2
+Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.1.3
 Summary: åºäºnonebot2çééå¤ç§apiçå¾ç/æ¼«ç»ç¿»è¯æä»¶ License:
 MIT Author: xenophon Author-email: 674550338@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.1.1,<10.0.0) Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0) Requires-Dist: nonebot2
 (>=2.0.0rc1,<3.0.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Description-
 Content-Type: text/markdown
                                    [nonebot]
         # nonebot-plugin-manga-translator â¨*åºäºNonebot2çå¾ç/
-                            æ¼«ç»ç¿»è¯æä»¶*â¨
+          æ¼«ç»ç¿»è¯æä»¶*â¨ [nonebot] [license] [pypi] [python]
 ## ð¿å®è£ éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb:
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨ `nb plugin install
 nonebot_plugin_manga_translator` - ä½¿ç¨pip(ä¸æ¨è):
 ~~ä¸æ¨èå°±æ¯ä¸æ¨èï¼ç¥ç¥ç¥~~ ## ðç®ä» 1.
 ééå¤ç§api,å°æ¶å°çå¾çç¿»è¯å¹¶åéç¿»è¯åçå¾çï¼æ¯ææ¹éæä½
 2. âï¸æä»¶éç½® è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
 (è³å°å¡«ä¸ä¸ªå¹³å°ç)ï¼è·åæ¹å¼å·²æ´çå¥½ï¼è§ä¸æ¹
 ~~ä¸ªäººæè§å°±æ¼«ç»ç¿»è¯èè¨,è¿å å®¶APIçææå¤§è´ä¸ºæé>=ç¾åº¦âç¦»çº¿>=ç«å±±,ä¸ç«å±±ç¿»è¯å¯¹ç«çæ¥æçç¿»è¯ææå¾å·®~~
 | éç½®é¡¹ | ç±»å | é»è®¤å¼ | ç¤ºä¾ | è¯´æ | APIå®ä»· | | :-----------
 ------------: | :---: | :----: | :---------------------------------: | :-------
 --------- | :------------------------------------------------ | |
 æéç¿»è¯API | - | - | - | - |
-æ¢¯åº¦æ¶è´¹ï¼0<æè°ç¨é<100wæ¶,0.04å/å¼  | | youdao_app_key | str | ""
-| youdao_app_key="xxxxx" | åºç¨ID | | | youdao_app_secret | str | "" |
-youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | | | ç¾åº¦ç¿»è¯API | - | - | - | -
-| æ¯æ1ä¸æ¬¡åè´¹è°ç¨éï¼ä¹åææ¢¯åº¦æ¶è´¹,æé«0.04å/æ¬¡ | |
+æ°ç¨æ·éä¸å®é¢åº¦,æ¢¯åº¦æ¶è´¹ï¼0<æè°ç¨é<100wæ¶,0.04å/å¼  | |
+youdao_app_key | str | "" | youdao_app_key="xxxxx" | åºç¨ID | | |
+youdao_app_secret | str | "" | youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | | |
+ç¾åº¦ç¿»è¯API | - | - | - | - |
+æ¯æ1ä¸æ¬¡åè´¹è°ç¨éï¼ä¹åææ¢¯åº¦æ¶è´¹,æé«0.04å/æ¬¡ | |
 baidu_app_id | str | "" | baidu_app_id="66666" | APP ID | | | baidu_app_key |
 str | "" | baidu_app_key="xxxxxx" | å¯é¥ | | | ç«å±±ç¿»è¯API | - | - | - |
 - | æ¯æå100å¼ åè´¹ï¼ä¹å0.04å/å¼  | | huoshan_access_key_id | str |
 "" | huoshan_access_key_id="AK***" | Access Key ID | | |
 huoshan_secret_access_key | str | "" | huoshan_secret_access_key="UT**" |
 Secret Access Key | | | ç¦»çº¿ç¿»è¯API | - | - | - | - | å¯è½æ¯çµè´¹? | |
 offline_url | str | "" | offline_url="http://127.0.0.1:5003" | è§ä¸æ¹è¯´æ
@@ -52,16 +53,16 @@
 Key`ï¼ç¶åç¹å»`Secret Access Key`ä¸çæé®æ¾ç¤ºåºå¯é¥ 3.
 åå«æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶   ç¦»çº¿ç¿»è¯
 (è¯¥æ¹æ¡å¯¹è®¾å¤éç½®è¦æ±è¾é«ï¼å»ºè®®å¨æè¶³å¤çç¡¬çç©ºé´ãåå­ãæ¾å­ï¼ææä¸å°è½ä¸ºbotå¤çè¯·æ±çæå¡å¨æ¶èèä½¿ç¨è¯¥æ¹æ¡)
 1. åè[manga-image-translator](https://github.com/zyddnys/manga-image-
 translator)çè¯´æï¼åéä»åºï¼å¹¶å®è£ç¸å³ä¾èµ
 (å¯è½éè¦é¢å¤å®è£`pydensecrf`) 2.
 å®è£å¥½ä¾èµåï¼å¨ä»åºç®å½ä¸è¿è¡ ```python python -
-m manga_translator -v --mode web --use-cuda# the demo will be serving on http:/
-/127.0.0.1:5003 ``` 3. å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
+m manga_translator -v --mode web --use-cuda # the demo will be serving on http:
+//127.0.0.1:5003 ``` 3. å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
 (è¦æ±pytorchççæ¬åcudaå¯¹åºï¼ä¸å¯¹åºè¯·éè£)ï¼è¯·å»æåæ°`--
 use-cuda`ï¼å¦æå¾çå¤çè¿ç¨ä¸­çæ¾å­ï¼è¯·æ¹æ`--use-cuda-
 limited` 4.
 ä½ å¯ä»¥è®¿é®æ§å¶å°ç»åºçç½åï¼å°è¯åæ¬å°ç¿»è¯ä¸å¼ å¾çï¼æ­¤æ¶ä¼æ ¹æ®éé¡¹ä¸è½½éè¦çæ¨¡å
 (ä¸ºé²æ­¢ä¸è½½å¤±è´¥ï¼ä¹å¯ä»¥æåæå¨ä¸è½½) 5.
 å¦æbotåç¿»è¯å¨å¨åä¸å°è®¾å¤ï¼é£ä¹.envå¡«å`offline_url="http://
 127.0.0.1:
@@ -78,18 +79,18 @@
 1. åæå­ï¼åå¤å¼ å¾ç 2. æå­+å¾ç*n 3. åæ¢ç¿»è¯api [api]:
 å°è¯¥apiä¼åçº§æå°æé«ï¼ç®åæ`youdao baidu huoshan offline`
 æªå®å¾ç»­ ## â­ææå¾ [https://github.com/maoxig/nonebot-plugin-manga-
 translator/blob/main/resource/ææå¾1.jpg] [https://github.com/maoxig/
 nonebot-plugin-manga-translator/blob/main/resource/ææå¾2.jpg] [https://
 github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
 ææå¾3.jpg] [https://github.com/maoxig/nonebot-plugin-manga-translator/
-blob/main/resource/ææå¾4.PNG] ## ðæ´æ°æ¥å¿  ç¹å»å±å¼ - 2023-05-
-03: - æ´æ°è¯´æææ¡£ - éé[ç«å±±ç¿»è¯api](https://
-translate.volcengine.com/api),ä½ å¯ä»¥éæ©æ¥å¥ç«å±±ç¿»è¯æä¾çAPI -
-2023-05-01: -
+blob/main/resource/ææå¾4.PNG] ## ðæ´æ°æ¥å¿  ç¹å»å±å¼ - 2023-06-
+09: - æ´æ°æä»¶åæ°æ® - 2023-05-03: - æ´æ°è¯´æææ¡£ - éé
+[ç«å±±ç¿»è¯api](https://translate.volcengine.com/
+api),ä½ å¯ä»¥éæ©æ¥å¥ç«å±±ç¿»è¯æä¾çAPI - 2023-05-01: -
 æ·»å åæ¢apiçåè½ï¼ä½ å¯ä»¥å°æä¸ªapiä¼åçº§è®¾ä¸ºæé« -
 ééç¦»çº¿ç¿»è¯api[manga-image-translator](https://github.com/zyddnys/manga-
 image-translator),ç°å¨ä½ å¯ä»¥ä½éªæ¬å°çç¿»è¯ - 2023-04-28: -
 æä»¶åå¸  ## ð¦è®¡å - [x] ééç¦»çº¿ç¿»è¯æ¨¡å[manga-image-
 translator](https://github.com/zyddnys/manga-image-translator) - [x]
 æ¯ææ´å¤API - [ ] å®åæä»¶ ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

