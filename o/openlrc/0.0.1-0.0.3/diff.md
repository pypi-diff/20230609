# Comparing `tmp/openlrc-0.0.1.tar.gz` & `tmp/openlrc-0.0.3.tar.gz`

## Comparing `openlrc-0.0.1.tar` & `openlrc-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openlrc-0.0.1/test_other.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 openlrc-0.0.1/openlrc/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 openlrc-0.0.1/openlrc/exceptions.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 openlrc-0.0.1/openlrc/logger.py
--rw-r--r--   0        0        0    10564 2020-02-02 00:00:00.000000 openlrc-0.0.1/openlrc/lrc.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 openlrc-0.0.1/openlrc/openlrc.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 openlrc-0.0.1/openlrc/prompter.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 openlrc-0.0.1/openlrc/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openlrc-0.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 openlrc-0.0.1/LICENSE
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 openlrc-0.0.1/README.md
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openlrc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 openlrc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/exceptions.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/logger.py
+-rw-r--r--   0        0        0    10941 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/lrc.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/openlrc.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/prompter.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openlrc-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 openlrc-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 openlrc-0.0.3/README.md
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 openlrc-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 openlrc-0.0.3/PKG-INFO
```

### Comparing `openlrc-0.0.1/openlrc/lrc.py` & `openlrc-0.0.3/openlrc/lrc.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,18 @@
         json_content = {'total_number': 0, 'list': []}
 
         system_prompt = str(prompter).format(
             source_lang=Language.get(self.lang if not source_lang else source_lang).display_name('en'),
             target_lang=Language.get(target_lang).display_name('en')
         )
 
+        # Prevent translating text into Traditional Chinese
+        if target_lang == 'zh-cn':
+            system_prompt.replace(Language.get(target_lang).display_name('en'), 'Mandarin Chinese')
+
         for chunk in chunks:
             # Format the input
             raw_content = format_texts(chunk)
 
             logger.info(f'Raw content: {raw_content}')
             token_number = get_token_number(raw_content + system_prompt)
             logger.info(f'Total token number: {token_number}')
@@ -139,14 +143,17 @@
                             }
                         ]
                     )
                     break
                 except openai.error.RateLimitError:
                     logger.warning('Rate limit exceeded. Wait 10s before retry.')
                     time.sleep(10)
+                except openai.error.APIConnectionError:
+                    logger.warning('API connection error. Wait 30s before retry.')
+                    time.sleep(30)
 
             target_content = response.choices[0].message.content
             logger.info(f'Target content: {target_content}')
 
             chunk_json_content = json2dict(target_content)
             logger.info(f'Length of the translated chunk: {len(chunk_json_content["list"])}')
```

### Comparing `openlrc-0.0.1/openlrc/openlrc.py` & `openlrc-0.0.3/openlrc/openlrc.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.0.1/openlrc/prompter.py` & `openlrc-0.0.3/openlrc/prompter.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 'Do not merge or eliminate any sentence.
 'Keep the number of the translated sentence in the returned list identical to that of the original list.
 'Ensure that the correspondence between the original and translated list is maintained.
 'Utilize context to rectify any inappropriate words.
 'If a sentence is not suitable for translation, please do not translate it, but you need to complete the translation of other suitable sentences.
 'If you are not sure whether a sentence is suitable for translation, please translate it.
 'Even if encountering sentences that are not suitable for translation, please maintain the output format.'
-'Even if only one sentence is translated, please maintain the output format. Dont add any other words.'''
+'Even if only one sentence is translated, please maintain the output format. Dont add any other words.
+'Use '<' and '>' to replace the double quote in the translated sentences.'''
 
 
 class LovelyPrompter(BaseTranslatePrompter):
     def __str__(self):
         return str(super()) + 'Use lovely colloquial expressions to translate each sentence.'
```

### Comparing `openlrc-0.0.1/openlrc/utils.py` & `openlrc-0.0.3/openlrc/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,27 +8,52 @@
 
 
 def json2dict(json_str):
     """ Convert json string to python dict. """
 
     try:
         result = json.loads(json_str)
+        return result
     except json.decoder.JSONDecodeError as e:
-        logger.warning(f'Error: Trying to convert into json: \n {json_str}\n')
+        logger.warning(f'Fail to convert into json: \n {json_str}\n')
 
-        # Try to fix the json string, only keep the content from first '{' to last '}'
-        result = json_str[json_str.find('{'):json_str.rfind('}') + 1]
-        logger.warning(f'Error: Trying to fix the json string: \n {result}\n Into: \n {result}\n')
-        try:
-            result = json.loads(result)
-        except json.decoder.JSONDecodeError:
-            logger.error(f'Error: Failed to convert into json: \n {json_str}\n')
-            raise e
+    # Try to fix the json string, only keep the content from first '{' to last '}'
+    fixed_json_str1 = json_str[json_str.find('{'):json_str.rfind('}') + 1]
+    logger.warning(
+        f'Trying to fix the json string by keep only "{{content}}": \n {json_str}\n Into: \n {fixed_json_str1}\n')
+    try:
+        result = json.loads(fixed_json_str1)
+        return result
+    except json.decoder.JSONDecodeError:
+        logger.warning(f'Failed to convert into json: \n {json_str}\n')
+
+    # Try to replace chinese "，" with english ","
+    fixed_json_str2 = fixed_json_str1.replace('，', ',')
+    logger.warning(
+        f'Trying to fix the json string by replace chinese quote with eng quote: \n {fixed_json_str1}\n Into: \n {fixed_json_str2}\n'
+    )
+    try:
+        result = json.loads(fixed_json_str2)
+        return result
+    except json.decoder.JSONDecodeError:
+        logger.warning(f'Failed to convert into json: \n {fixed_json_str2}\n')
+
+    # The content after last found " should be "}]"
+    fixed_json_str3 = fixed_json_str2[:fixed_json_str2.rfind('"') + 1] + ']}'
+    try:
+        result = json.loads(fixed_json_str3)
+        return result
+    except json.decoder.JSONDecodeError as e:
+        logger.error(f'Failed to convert into json: \n {fixed_json_str3}\n')
+
+        # Save the json string to file
+        with open('error.json', 'w', encoding='utf-8') as f:
+            f.write(fixed_json_str3)
 
-    return result
+        raise e
 
 
 def get_token_number(text):
     encoder = tiktoken.encoding_for_model("gpt-3.5-turbo")
 
     return len(encoder.encode(text))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlrc-0.0.1/LICENSE` & `openlrc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.0.1/pyproject.toml` & `openlrc-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openlrc"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
     { name = "Hao Zheng", email = "zhenghaosustc@gmail.com" },
 ]
 description = "Transcribe and translate voice into LRC file."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -30,10 +30,18 @@
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.11',
     "Operating System :: OS Independent",
 ]
 
+[tool.hatch.build]
+exclude = [
+    "test*",
+    "/promotion",
+    "/docs",
+    "/tests",
+]
+
 [project.urls]
 "Homepage" = "https://github.com/zh-plus/Open-Lyrics"
 "Bug Tracker" = "https://github.com/zh-plus/Open-Lyrics/issues"
```

