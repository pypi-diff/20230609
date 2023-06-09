# Comparing `tmp/mindmate-0.1.5.tar.gz` & `tmp/mindmate-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindmate-0.1.5.tar", last modified: Tue Jun  6 20:06:25 2023, max compression
+gzip compressed data, was "mindmate-0.1.6.tar", last modified: Fri Jun  9 20:40:50 2023, max compression
```

## Comparing `mindmate-0.1.5.tar` & `mindmate-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:25.198553 mindmate-0.1.5/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2084 2023-06-06 20:06:25.194554 mindmate-0.1.5/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      759 2023-06-06 20:02:53.000000 mindmate-0.1.5/README.md
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:24.553437 mindmate-0.1.5/mindmate/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.5/mindmate/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      551 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/cli.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:24.870542 mindmate-0.1.5/mindmate/commands/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.5/mindmate/commands/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3968 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/commands/ai.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2816 2023-06-06 20:02:53.000000 mindmate-0.1.5/mindmate/commands/chat.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      756 2023-04-26 02:15:41.000000 mindmate-0.1.5/mindmate/commands/configure.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      143 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/commands/version.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       17 2023-06-06 20:02:53.000000 mindmate-0.1.5/mindmate/meta.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:25.012052 mindmate-0.1.5/mindmate/services/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/services/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1457 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/services/directory.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3545 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/services/models.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     4452 2023-06-06 20:02:53.000000 mindmate-0.1.5/mindmate/services/openai.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:25.166075 mindmate-0.1.5/mindmate/utils/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.5/mindmate/utils/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      790 2023-06-06 20:02:53.000000 mindmate-0.1.5/mindmate/utils/conf.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      619 2023-04-24 05:58:07.000000 mindmate-0.1.5/mindmate/utils/env.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      312 2023-04-26 01:29:16.000000 mindmate-0.1.5/mindmate/utils/helper.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1862 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/utils/utils.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:24.712522 mindmate-0.1.5/mindmate.egg-info/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2084 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      644 2023-06-06 20:06:23.000000 mindmate-0.1.5/mindmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/entry_points.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       41 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/requires.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/top_level.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-06-06 20:06:25.200554 mindmate-0.1.5/setup.cfg
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2260 2023-06-03 16:28:25.000000 mindmate-0.1.5/setup.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.865685 mindmate-0.1.6/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2083 2023-06-09 20:40:50.862176 mindmate-0.1.6/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      759 2023-06-06 20:02:53.000000 mindmate-0.1.6/README.md
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.074108 mindmate-0.1.6/mindmate/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.6/mindmate/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      637 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/cli.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.473520 mindmate-0.1.6/mindmate/commands/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.6/mindmate/commands/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2538 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/commands/chat.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      768 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/commands/configure.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     4038 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/commands/directory.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1680 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/commands/image.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      143 2023-06-03 16:28:25.000000 mindmate-0.1.6/mindmate/commands/version.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1216 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/error.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       17 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/meta.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.667514 mindmate-0.1.6/mindmate/services/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:28:25.000000 mindmate-0.1.6/mindmate/services/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1457 2023-06-03 16:28:25.000000 mindmate-0.1.6/mindmate/services/directory.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1500 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/services/generic.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3545 2023-06-03 16:28:25.000000 mindmate-0.1.6/mindmate/services/models.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     4957 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/services/openai.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.832785 mindmate-0.1.6/mindmate/utils/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.6/mindmate/utils/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      773 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/utils/conf.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      657 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/utils/env.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      328 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/utils/helper.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2461 2023-06-09 20:37:05.000000 mindmate-0.1.6/mindmate/utils/utils.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-09 20:40:50.250293 mindmate-0.1.6/mindmate.egg-info/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2083 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      725 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       41 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/requires.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-06-09 20:40:48.000000 mindmate-0.1.6/mindmate.egg-info/top_level.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-06-09 20:40:50.866686 mindmate-0.1.6/setup.cfg
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2259 2023-06-08 18:06:48.000000 mindmate-0.1.6/setup.py
```

### Comparing `mindmate-0.1.5/PKG-INFO` & `mindmate-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindmate
-Version: 0.1.5
+Version: 0.1.6
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: # install package
@@ -41,15 +41,15 @@
         
         # compatibility
         
         __Not tested__ yet, but should be compatible with any Python >= 3.8
         
 Keywords: cli,ai,nlp,ml,developers,productivity,openai,directory,manifest
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
```

### Comparing `mindmate-0.1.5/README.md` & `mindmate-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.5/mindmate/cli.py` & `mindmate-0.1.6/mindmate/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import click
 from mindmate.utils import helper
 from mindmate.commands.configure import configure
 from mindmate.commands.chat import chat
-from mindmate.commands.ai import ai
+from mindmate.commands.directory import directory
+from mindmate.commands.image import image
 from mindmate.commands.version import version
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def cli():
     """hi to mindmate cli, try option --help for more information"""
     pass
 
 cli.add_command(configure)
 cli.add_command(chat)
-cli.add_command(ai)
+cli.add_command(directory)
+cli.add_command(image)
 cli.add_command(version)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `mindmate-0.1.5/mindmate/commands/ai.py` & `mindmate-0.1.6/mindmate/commands/directory.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     # Print the keys and values in the table
     for key, value in content.items():
         row = f'{str(key):<{max_key_length}} {value}'
         yield row + '\n'
 
 @click.group()
-def ai():
+def directory():
     """Returns related functionalities to AI platforms"""
     pass
 
 @click.group()
 def chat():
     """Returns related functionalities to chat-based AI platforms"""
     pass
@@ -129,16 +129,16 @@
 @click.command(name='list')
 def list_coding():
     """a list of AI platforms that offer code-based responses"""
     click.echo_via_pager(_generate_output(manifest.list_development()))
 
 coding.add_command(list_coding)
 
-ai.add_command(chat)
-ai.add_command(image)
-ai.add_command(video)
-ai.add_command(prompting)
-ai.add_command(design)
-ai.add_command(presentation)
-ai.add_command(no_code)
-ai.add_command(data)
-ai.add_command(coding)
+directory.add_command(chat)
+directory.add_command(image)
+directory.add_command(video)
+directory.add_command(prompting)
+directory.add_command(design)
+directory.add_command(presentation)
+directory.add_command(no_code)
+directory.add_command(data)
+directory.add_command(coding)
```

### Comparing `mindmate-0.1.5/mindmate/commands/chat.py` & `mindmate-0.1.6/mindmate/commands/chat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 import click
 import sys
 from mindmate.utils.utils import utility
 from mindmate.utils.helper import help
 from mindmate.utils.conf import constants
 from mindmate.services.openai import OpenAIManager
+from mindmate.services.generic import Prompt
 
 
-def stream_response(completion):
-    """Stream the messages generated by the OpenAI API to the user."""
-    for choice in completion.choices:
-        if 'message' in choice and 'content' in choice.message:
-            return choice.message['content']
-
 def model_option_callback(ctx, param, value):
     try:
         platform = ctx.params['platform']
     except KeyError:
         click.echo(f"{constants.SYS_ROLE}: You can't specify a platform/model alone, you need to specify them both or don't specify both.")
         click.echo(f"{constants.HINT_ROLE}: try to re-order to the options and starts with --platform/-P then --model/-m and then --prompt/-p")
         sys.exit(1)
     if platform == 'openai':
         return value if value in constants.MODEL_OPTIONS['openai'] else None
-    elif platform == 'aws':
-        return value if value in constants.MODEL_OPTIONS['aws'] else None
     else:
         return None
 
 @click.command()
 @click.option('-P', '--platform', required=True, default='openai', show_default=False, type=click.Choice(constants.PLATFORM_OPTIONS), help='use platform as an underlying technology')
 @click.option('-m', '--model', required=True, default='text-davinci-003', show_default=True, type=str, callback=model_option_callback, help='select targeted model to utilize')
 @click.option('-p', '--prompt', required=True, show_default=False, type=str, help='Your prompt to AI')
-@click.option('-s', '--stream', required=False, default=False, show_default=True, type=bool, help='stream AI response on your terminal')
+@click.option('-s', '--stream', required=False, default=True, show_default=True, type=bool, help='stream AI response on your terminal')
 @click.option('--max-tokens', required=False, default=100, show_default=True, type=int, help='stream AI response on your terminal')
 def chat(platform, model, prompt, stream, max_tokens):
     """offers text-based response to your prompt"""
     click.echo(help.generic_message())
     # click.echo(click.get_current_context().params)
-    KEYS = utility.set_yaml_state(constants.FILE_PATH+'/'+constants.FILE_NAME)['keys']
+    KEYS = utility.get_yaml_state(constants.FILE_PATH+'/'+constants.FILE_NAME)['keys']
     if platform == 'openai':
         openai_client = OpenAIManager(id=KEYS['openai_id'], token=KEYS['openai_token'])
         openai_client.check_model(model)
+        prompt = Prompt(prompt)
         if stream == False:
             response = openai_client.ask_ai(prompt=prompt, model=model, max_tokens=max_tokens)
             click.echo(f'{constants.AI_ROLE}: {response}')
         elif stream == True:
             click.echo(f'{constants.AI_ROLE}: ', nl=False)
             for response in openai_client.ask_ai_with_stream(prompt=prompt, model=model, max_tokens=max_tokens): click.echo(response, nl=False)
     else:
```

### Comparing `mindmate-0.1.5/mindmate/commands/configure.py` & `mindmate-0.1.6/mindmate/commands/configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 from mindmate.utils.utils import utility
 from mindmate.utils.conf import constants
 
 @click.command()
 def configure():
     """collect keys from user and save it into state file as yaml"""
 
-    file = utility.set_yaml_state(constants.FILE_PATH+'/'+constants.FILE_NAME)
+    file = utility.get_yaml_state(constants.FILE_PATH+'/'+constants.FILE_NAME)
     #TODO: check environment variable first before setting values into yaml file. If exist, then skip yaml update
     openai_value = file['keys']['openai_token']
     openai_user_token = click.prompt(f'OPENAI TOKEN [****************{openai_value[-4:]}]', type=str)
     file['keys']['openai_token'] = openai_user_token
-    file['keys']['openai_id'] = str(uuid.uuid4())
+    file['keys']['openai_id'] = 'mindmate-'+str(uuid.uuid4())
     utility.update_yaml_state(state=file, file_path=constants.FILE_PATH+'/'+constants.FILE_NAME)
```

### Comparing `mindmate-0.1.5/mindmate/services/directory.py` & `mindmate-0.1.6/mindmate/services/directory.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.5/mindmate/services/models.py` & `mindmate-0.1.6/mindmate/services/models.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.1.5/mindmate/utils/conf.py` & `mindmate-0.1.6/mindmate/utils/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     FILE_PATH = '~/.mindmate'
     FILE_NAME = 'environment.yaml'
     SYS_ROLE = 'system'
     AI_ROLE = 'AI bot'
     HINT_ROLE = 'HINT'
     PLATFORM_OPTIONS = ['openai']
     MODEL_OPTIONS = {
-        'openai': ['gpt-3.5-turbo', 'text-davinci-003', 'text-davinci-002'],
+        'openai': ['text-davinci-003', 'text-davinci-002'],
     }
```

### Comparing `mindmate-0.1.5/mindmate/utils/utils.py` & `mindmate-0.1.6/mindmate/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 import yaml
 import os
+import string, random
 from mindmate.utils.conf import constants, mongo
 
 class utility:
     def create_yaml_state(file: str) -> dict:
         while not os.path.isfile(constants.FILE_PATH+'/'+constants.FILE_NAME):
             os.makedirs(constants.FILE_PATH, exist_ok=True)
             data = {
                 'version':1,
                 'keys': {
                     'openai_token':'xxxx',
                     'openai_id':'xxxx',
+                },
+                'prompt': {
+                    'last_prompt': None,
+                    'expires_at': None,
                 }
             }
             with open(constants.FILE_PATH+'/'+constants.FILE_NAME, 'w') as outputfile:
                 yaml.dump(data, outputfile, default_flow_style=False)
             return data
-    def set_yaml_state(file: str) -> dict:
+    def get_yaml_state(file: str) -> dict:
         """Read YAML file and return data as dictionary."""
         try:
             with open(file, 'r') as f:
                 data_dict = yaml.load(f, Loader=yaml.FullLoader)
             return data_dict
         except FileNotFoundError as f:
             return utility.create_yaml_state(file)
     def update_yaml_state(state: dict, file_path: str) -> None:
         """update new yaml state with only changed keys and maintain unchanged values"""
+        existing_state = utility.get_yaml_state(constants.FILE_PATH+'/'+constants.FILE_NAME)
+        existing_state.update(state)
         with open(file_path, 'w') as outputfile:
-            yaml.dump(state, outputfile, default_flow_style=False)
+            yaml.dump(existing_state, outputfile, default_flow_style=False)
 
     #TODO: below implementation is not associated with any functionality yet, require implementation to be completed
-    def override_with_environment_variables(data: dict) -> dict:
-        """Override YAML data with environment variables."""
-        for key in data:
-            if key in os.environ:
-                data[key] = os.environ[key]
-        return data
+    # def override_with_environment_variables(data: dict) -> dict:
+    #     """Override YAML data with environment variables."""
+    #     for key in data:
+    #         if key in os.environ:
+    #             data[key] = os.environ[key]
+    #     return data
 
     def extract_results(result: dict) -> dict:
         final = {}
         for object in result:
             for key, value in object.items():
                 if key != '_id':
                     final.update({key: value})
-        return final
+        return final
+    def generate_random_string() -> str:
+        length = random.randint(5, 10)
+        letters = string.ascii_letters
+        random_string = ''.join(random.choice(letters) for _ in range(length))
+        return random_string
+    def get_the_current_path() -> str:
+        return os.getenv('PWD')
```

### Comparing `mindmate-0.1.5/mindmate.egg-info/PKG-INFO` & `mindmate-0.1.6/mindmate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindmate
-Version: 0.1.5
+Version: 0.1.6
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: # install package
@@ -41,15 +41,15 @@
         
         # compatibility
         
         __Not tested__ yet, but should be compatible with any Python >= 3.8
         
 Keywords: cli,ai,nlp,ml,developers,productivity,openai,directory,manifest
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
```

### Comparing `mindmate-0.1.5/mindmate.egg-info/SOURCES.txt` & `mindmate-0.1.6/mindmate.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 README.md
 setup.py
 mindmate/__init__.py
 mindmate/cli.py
+mindmate/error.py
 mindmate/meta.py
 mindmate.egg-info/PKG-INFO
 mindmate.egg-info/SOURCES.txt
 mindmate.egg-info/dependency_links.txt
 mindmate.egg-info/entry_points.txt
 mindmate.egg-info/requires.txt
 mindmate.egg-info/top_level.txt
 mindmate/commands/__init__.py
-mindmate/commands/ai.py
 mindmate/commands/chat.py
 mindmate/commands/configure.py
+mindmate/commands/directory.py
+mindmate/commands/image.py
 mindmate/commands/version.py
 mindmate/services/__init__.py
 mindmate/services/directory.py
+mindmate/services/generic.py
 mindmate/services/models.py
 mindmate/services/openai.py
 mindmate/utils/__init__.py
 mindmate/utils/conf.py
 mindmate/utils/env.py
 mindmate/utils/helper.py
 mindmate/utils/utils.py
```

### Comparing `mindmate-0.1.5/setup.py` & `mindmate-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     entry_points={
         'console_scripts': [
             'mindmate = mindmate.cli:cli',  # Update with your CLI entry point
         ],
     },
     # reference: https://pypi.org/classifiers/
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Environment :: Other Environment',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Information Technology',
```

