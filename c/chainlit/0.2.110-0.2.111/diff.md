# Comparing `tmp/chainlit-0.2.110.tar.gz` & `tmp/chainlit-0.2.111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-0.2.110.tar", max compression
+gzip compressed data, was "chainlit-0.2.111.tar", max compression
```

## Comparing `chainlit-0.2.110.tar` & `chainlit-0.2.111.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2477 2023-06-08 15:36:12.422187 chainlit-0.2.110/README.md
--rw-r--r--   0        0        0     6620 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/__main__.py
--rw-r--r--   0        0        0     1234 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/action.py
--rw-r--r--   0        0        0     3773 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/cli/__init__.py
--rw-r--r--   0        0        0     4093 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/cli/auth.py
--rw-r--r--   0        0        0     2594 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/cli/deploy.py
--rw-r--r--   0        0        0      716 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/cli/utils.py
--rw-r--r--   0        0        0     8578 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/client.py
--rw-r--r--   0        0        0     6548 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/config.py
--rw-r--r--   0        0        0     5068 2023-06-08 15:35:16.514063 chainlit-0.2.110/chainlit/element.py
--rw-r--r--   0        0        0  2074648 2023-06-08 15:36:49.346337 chainlit-0.2.110/chainlit/frontend/dist/assets/index-36bf9cab.js
--rw-r--r--   0        0        0     4317 2023-06-08 15:36:49.342337 chainlit-0.2.110/chainlit/frontend/dist/assets/index-bdffdaa0.css
--rw-r--r--   0        0        0     8889 2023-06-08 15:36:49.342337 chainlit-0.2.110/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
--rw-r--r--   0        0        0     8891 2023-06-08 15:36:49.342337 chainlit-0.2.110/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
--rw-r--r--   0        0        0     6455 2023-06-08 15:36:47.674335 chainlit-0.2.110/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0      791 2023-06-08 15:36:49.342337 chainlit-0.2.110/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      399 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/hello.py
--rw-r--r--   0        0        0        0 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/lc/__init__.py
--rw-r--r--   0        0        0     8467 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/lc/chainlit_handler.py
--rw-r--r--   0        0        0      863 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/lc/monkey.py
--rw-r--r--   0        0        0     5388 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/lc/new_monkey.py
--rw-r--r--   0        0        0     4129 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/lc/old_monkey.py
--rw-r--r--   0        0        0     1068 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/lc/utils.py
--rw-r--r--   0        0        0      398 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/logger.py
--rw-r--r--   0        0        0     1623 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/markdown.py
--rw-r--r--   0        0        0    12016 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/message.py
--rw-r--r--   0        0        0     5227 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/sdk.py
--rw-r--r--   0        0        0    11230 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/server.py
--rw-r--r--   0        0        0      800 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/session.py
--rw-r--r--   0        0        0     2342 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/telemetry.py
--rw-r--r--   0        0        0     1064 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/types.py
--rw-r--r--   0        0        0     1145 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/user_session.py
--rw-r--r--   0        0        0      196 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/version.py
--rw-r--r--   0        0        0     1551 2023-06-08 15:35:16.518063 chainlit-0.2.110/chainlit/watch.py
--rw-r--r--   0        0        0     1031 2023-06-08 15:35:16.522063 chainlit-0.2.110/pyproject.toml
--rw-r--r--   0        0        0     3906 1970-01-01 00:00:00.000000 chainlit-0.2.110/PKG-INFO
+-rw-r--r--   0        0        0     2477 2023-06-09 16:20:19.169145 chainlit-0.2.111/README.md
+-rw-r--r--   0        0        0     6620 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/__main__.py
+-rw-r--r--   0        0        0     1234 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/action.py
+-rw-r--r--   0        0        0     4728 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0     4093 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/cli/auth.py
+-rw-r--r--   0        0        0     2594 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/cli/deploy.py
+-rw-r--r--   0        0        0      716 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/cli/utils.py
+-rw-r--r--   0        0        0     8578 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/client.py
+-rw-r--r--   0        0        0     6548 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/config.py
+-rw-r--r--   0        0        0     5068 2023-06-09 16:19:40.032612 chainlit-0.2.111/chainlit/element.py
+-rw-r--r--   0        0        0  2074675 2023-06-09 16:20:46.073502 chainlit-0.2.111/chainlit/frontend/dist/assets/index-4d8f8873.js
+-rw-r--r--   0        0        0     4317 2023-06-09 16:20:46.073502 chainlit-0.2.111/chainlit/frontend/dist/assets/index-bdffdaa0.css
+-rw-r--r--   0        0        0     8889 2023-06-09 16:20:46.065502 chainlit-0.2.111/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
+-rw-r--r--   0        0        0     8891 2023-06-09 16:20:46.073502 chainlit-0.2.111/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
+-rw-r--r--   0        0        0     6455 2023-06-09 16:20:44.793486 chainlit-0.2.111/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0      791 2023-06-09 16:20:46.073502 chainlit-0.2.111/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      399 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/hello.py
+-rw-r--r--   0        0        0        0 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/lc/__init__.py
+-rw-r--r--   0        0        0     8467 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/lc/chainlit_handler.py
+-rw-r--r--   0        0        0      863 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/lc/monkey.py
+-rw-r--r--   0        0        0     5388 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/lc/new_monkey.py
+-rw-r--r--   0        0        0     4129 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/lc/old_monkey.py
+-rw-r--r--   0        0        0     1068 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/lc/utils.py
+-rw-r--r--   0        0        0      398 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/logger.py
+-rw-r--r--   0        0        0     1623 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/markdown.py
+-rw-r--r--   0        0        0    12016 2023-06-09 16:19:40.036612 chainlit-0.2.111/chainlit/message.py
+-rw-r--r--   0        0        0     5227 2023-06-09 16:19:40.040612 chainlit-0.2.111/chainlit/sdk.py
+-rw-r--r--   0        0        0    11230 2023-06-09 16:19:40.040612 chainlit-0.2.111/chainlit/server.py
+-rw-r--r--   0        0        0      800 2023-06-09 16:19:40.040612 chainlit-0.2.111/chainlit/session.py
+-rw-r--r--   0        0        0     2342 2023-06-09 16:19:40.040612 chainlit-0.2.111/chainlit/telemetry.py
+-rw-r--r--   0        0        0     1064 2023-06-09 16:19:40.040612 chainlit-0.2.111/chainlit/types.py
+-rw-r--r--   0        0        0     1145 2023-06-09 16:19:40.040612 chainlit-0.2.111/chainlit/user_session.py
+-rw-r--r--   0        0        0      196 2023-06-09 16:19:40.040612 chainlit-0.2.111/chainlit/version.py
+-rw-r--r--   0        0        0     1551 2023-06-09 16:19:40.040612 chainlit-0.2.111/chainlit/watch.py
+-rw-r--r--   0        0        0     1031 2023-06-09 16:19:40.040612 chainlit-0.2.111/pyproject.toml
+-rw-r--r--   0        0        0     3906 1970-01-01 00:00:00.000000 chainlit-0.2.111/PKG-INFO
```

### Comparing `chainlit-0.2.110/README.md` & `chainlit-0.2.111/README.md`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/__init__.py` & `chainlit-0.2.111/chainlit/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/action.py` & `chainlit-0.2.111/chainlit/action.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/cli/__init__.py` & `chainlit-0.2.111/chainlit/cli/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,14 +71,49 @@
     if host:
         os.environ["CHAINLIT_HOST"] = host
     if port:
         os.environ["CHAINLIT_PORT"] = port
     if ci:
         logger.info("Running in CI mode")
         config.enable_telemetry = False
+
+        # Set the openai api key to a fake value
+        import os
+
+        os.environ["OPENAI_API_KEY"] = "sk-FAKE-OPENAI-API-KEY"
+
+        # Mock the openai api
+        import responses
+
+        responses.start()
+        jsonReply = {
+            "id": "cmpl-uqkvlQyYK7bGYrRHQ0eXlWi7",
+            "object": "text_completion",
+            "created": 1589478378,
+            "model": "text-davinci-003",
+            "choices": [
+                {
+                    "text": "\n\n```text\n3*3\n```",
+                    "index": 0,
+                    "logprobs": None,
+                    "finish_reason": "length",
+                }
+            ],
+            "usage": {
+                "prompt_tokens": 5,
+                "completion_tokens": 7,
+                "total_tokens": 12,
+            },
+        }
+        responses.add(
+            responses.POST,
+            "https://api.openai.com/v1/completions",
+            json=jsonReply,
+        )
+
     else:
         trace_event("chainlit run")
 
     run_chainlit(target, watch, headless, debug)
 
 
 @cli.command("deploy")
```

### Comparing `chainlit-0.2.110/chainlit/cli/auth.py` & `chainlit-0.2.111/chainlit/cli/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/cli/deploy.py` & `chainlit-0.2.111/chainlit/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/cli/utils.py` & `chainlit-0.2.111/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/client.py` & `chainlit-0.2.111/chainlit/client.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/config.py` & `chainlit-0.2.111/chainlit/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/element.py` & `chainlit-0.2.111/chainlit/element.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/frontend/dist/assets/index-36bf9cab.js` & `chainlit-0.2.111/chainlit/frontend/dist/assets/index-4d8f8873.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -82797,15 +82797,15 @@
                 ...Lpt(e)
             },
             ...!t && {
                 ...Fpt(e)
             }
         })),
         cie = () => {
-            const [e, t] = ga(vM);
+            const [e, t] = ga(vM), n = k.useMemo(() => e ? uie(e) : null, [e]);
             return O.jsxs(Mpt, {
                 open: !!e,
                 children: [O.jsxs(Hn, {
                     direction: "row",
                     alignItems: "center",
                     children: [O.jsx(jn, {
                         noWrap: !0,
@@ -82823,15 +82823,15 @@
                     })]
                 }), O.jsx(Mt, {
                     mt: "1.5rem",
                     id: "side-view-content",
                     sx: {
                         height: "100%"
                     },
-                    children: e && uie(e)
+                    children: n
                 })]
             })
         };
 
     function Ppt() {
         const [e, t] = ga(vv), n = Yt(Ap);
         if (!e) return null;
```

### Comparing `chainlit-0.2.110/chainlit/frontend/dist/assets/index-bdffdaa0.css` & `chainlit-0.2.111/chainlit/frontend/dist/assets/index-bdffdaa0.css`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg` & `chainlit-0.2.111/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg` & `chainlit-0.2.111/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/frontend/dist/favicon.svg` & `chainlit-0.2.111/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/frontend/dist/index.html` & `chainlit-0.2.111/chainlit/frontend/dist/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     <link
       href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap"
       rel="stylesheet"
     />
     <script>
       const global = globalThis;
     </script>
-    <script type="module" crossorigin src="/assets/index-36bf9cab.js"></script>
+    <script type="module" crossorigin src="/assets/index-4d8f8873.js"></script>
     <link rel="stylesheet" href="/assets/index-bdffdaa0.css">
   </head>
   <body>
     <div id="root"></div>
     
   </body>
 </html>
```

### Comparing `chainlit-0.2.110/chainlit/lc/chainlit_handler.py` & `chainlit-0.2.111/chainlit/lc/chainlit_handler.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/lc/monkey.py` & `chainlit-0.2.111/chainlit/lc/monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/lc/new_monkey.py` & `chainlit-0.2.111/chainlit/lc/new_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/lc/old_monkey.py` & `chainlit-0.2.111/chainlit/lc/old_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/lc/utils.py` & `chainlit-0.2.111/chainlit/lc/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/markdown.py` & `chainlit-0.2.111/chainlit/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/message.py` & `chainlit-0.2.111/chainlit/message.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/sdk.py` & `chainlit-0.2.111/chainlit/sdk.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/server.py` & `chainlit-0.2.111/chainlit/server.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/session.py` & `chainlit-0.2.111/chainlit/session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/telemetry.py` & `chainlit-0.2.111/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/types.py` & `chainlit-0.2.111/chainlit/types.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/user_session.py` & `chainlit-0.2.111/chainlit/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/chainlit/watch.py` & `chainlit-0.2.111/chainlit/watch.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.110/pyproject.toml` & `chainlit-0.2.111/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlit"
-version = "0.2.110"
+version = "0.2.111"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'langchain']
 description = "A faster way to build chatbot UIs."
 authors = ["Chainlit"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
```

### Comparing `chainlit-0.2.110/PKG-INFO` & `chainlit-0.2.111/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 0.2.110
+Version: 0.2.111
 Summary: A faster way to build chatbot UIs.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,langchain
 Author: Chainlit
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

