# Comparing `tmp/fabric-mgmt-cli-1.4.0b4.tar.gz` & `tmp/fabric-mgmt-cli-1.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-mgmt-cli-1.4.0b4.tar", last modified: Sat Jan 14 02:15:42 2023, max compression
+gzip compressed data, was "fabric-mgmt-cli-1.5.0b1.tar", last modified: Fri Jun  9 20:57:53 2023, max compression
```

## Comparing `fabric-mgmt-cli-1.4.0b4.tar` & `fabric-mgmt-cli-1.5.0b1.tar`

### file list

```diff
@@ -1,36 +1,25 @@
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-14 02:15:42.024435 fabric-mgmt-cli-1.4.0b4/
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/LICENSE
--rw-r--r--   0 kthare10   (503) staff       (20)      143 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/MANIFEST.in
--rw-r--r--   0 kthare10   (503) staff       (20)     9878 2023-01-14 02:15:42.023821 fabric-mgmt-cli-1.4.0b4/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     9378 2022-12-20 22:42:50.000000 fabric-mgmt-cli-1.4.0b4/README.md
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-14 02:15:42.006730 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/
--rw-r--r--   0 kthare10   (503) staff       (20)       24 2023-01-14 02:14:48.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-14 02:15:42.016674 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2002 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/command.py
--rw-r--r--   0 kthare10   (503) staff       (20)     9832 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/config_processor.py
--rw-r--r--   0 kthare10   (503) staff       (20)     7461 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/configuration.py
--rw-r--r--   0 kthare10   (503) staff       (20)     9946 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/kafka_processor.py
--rw-r--r--   0 kthare10   (503) staff       (20)    26203 2023-01-13 22:08:00.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/manage_command.py
--rw-r--r--   0 kthare10   (503) staff       (20)    23725 2023-01-14 01:57:30.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/managecli.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-14 02:15:42.021245 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8830 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/commands.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3657 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/nso.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1072 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/resources.py
--rw-r--r--   0 kthare10   (503) staff       (20)     6728 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/services.py
--rw-r--r--   0 kthare10   (503) staff       (20)      535 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/util.py
--rw-r--r--   0 kthare10   (503) staff       (20)    16640 2023-01-14 01:57:36.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/show_command.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-14 02:15:42.022680 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/test/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/test/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8401 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/test/test_managecli.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-14 02:15:42.009361 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli.egg-info/
--rw-r--r--   0 kthare10   (503) staff       (20)     9878 2023-01-14 02:15:41.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli.egg-info/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)      989 2023-01-14 02:15:41.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kthare10   (503) staff       (20)        1 2023-01-14 02:15:41.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       82 2023-01-14 02:15:41.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli.egg-info/entry_points.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       87 2023-01-14 02:15:41.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli.egg-info/requires.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       16 2023-01-14 02:15:41.000000 fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli.egg-info/top_level.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       87 2023-01-14 02:14:42.000000 fabric-mgmt-cli-1.4.0b4/requirements.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       38 2023-01-14 02:15:42.024566 fabric-mgmt-cli-1.4.0b4/setup.cfg
--rw-r--r--   0 kthare10   (503) staff       (20)     1250 2022-10-13 16:37:50.000000 fabric-mgmt-cli-1.4.0b4/setup.py
+-rw-r--r--   0        0        0     1806 2023-06-09 20:57:01.647957 fabric-mgmt-cli-1.5.0b1/.gitignore
+-rw-r--r--   0        0        0     1071 2022-10-13 16:37:50.489741 fabric-mgmt-cli-1.5.0b1/LICENSE
+-rw-r--r--   0        0        0     9452 2023-01-19 19:01:44.980822 fabric-mgmt-cli-1.5.0b1/README.md
+-rw-r--r--   0        0        0     2046 2022-10-13 16:37:50.490228 fabric-mgmt-cli-1.5.0b1/config.yml
+-rw-r--r--   0        0        0       51 2023-06-09 20:57:43.829971 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-13 16:37:50.490498 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/__init__.py
+-rw-r--r--   0        0        0     2002 2022-10-13 16:37:50.490695 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/command.py
+-rw-r--r--   0        0        0     9832 2022-10-13 16:37:50.490796 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/config_processor.py
+-rw-r--r--   0        0        0     7461 2022-10-13 16:37:50.490934 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/configuration.py
+-rw-r--r--   0        0        0     9957 2023-01-19 18:49:45.717500 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/kafka_processor.py
+-rw-r--r--   0        0        0    45398 2023-05-22 15:02:49.188025 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/manage_command.py
+-rw-r--r--   0        0        0    27720 2023-05-17 03:26:00.969252 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/managecli.py
+-rw-r--r--   0        0        0        0 2022-10-13 16:37:50.491613 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/__init__.py
+-rw-r--r--   0        0        0     8830 2022-10-13 16:37:50.491743 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/commands.py
+-rw-r--r--   0        0        0     3657 2022-10-13 16:37:50.491891 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/nso.py
+-rw-r--r--   0        0        0     1072 2022-10-13 16:37:50.492004 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/resources.py
+-rw-r--r--   0        0        0     6728 2023-05-09 13:25:27.691022 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/services.py
+-rw-r--r--   0        0        0      535 2022-10-13 16:37:50.492246 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/util.py
+-rw-r--r--   0        0        0    19237 2023-06-04 20:42:05.646655 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/show_command.py
+-rw-r--r--   0        0        0        0 2022-10-13 16:37:50.492509 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/test/__init__.py
+-rw-r--r--   0        0        0     1828 2022-10-13 16:37:50.492603 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/test/config.yml
+-rw-r--r--   0        0        0     8401 2022-10-13 16:37:50.492732 fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/test/test_managecli.py
+-rw-r--r--   0        0        0      983 2022-10-13 16:37:50.492848 fabric-mgmt-cli-1.5.0b1/net_inventory.yml
+-rw-r--r--   0        0        0     1067 2023-06-09 20:55:59.298191 fabric-mgmt-cli-1.5.0b1/pyproject.toml
+-rw-r--r--   0        0        0    10351 1970-01-01 00:00:00.000000 fabric-mgmt-cli-1.5.0b1/PKG-INFO
```

### Comparing `fabric-mgmt-cli-1.4.0b4/LICENSE` & `fabric-mgmt-cli-1.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.4.0b4/PKG-INFO` & `fabric-mgmt-cli-1.5.0b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: fabric-mgmt-cli
-Version: 1.4.0b4
-Summary: Fabric Control Framework
-Home-page: https://github.com/fabric-testbed/ManagementCli
-Author: Komal Thareja
-Author-email: kthare10@renci.org
-Keywords: Swagger,Fabric Control Framework Management Cli
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Requirements Status](https://requires.io/github/fabric-testbed/ManagementCli/requirements.svg?branch=main)](https://requires.io/github/fabric-testbed/ManagementCli/requirements/?branch=main)
 
 [![PyPI](https://img.shields.io/pypi/v/fabric-mgmt-cli?style=plastic)](https://pypi.org/project/fabric-mgmt-cli/)
 
 # ManagementCli
 Fabric Control Framework Management CLI for administrative operations over Kafka
 
@@ -258,19 +243,19 @@
 ##### Change Worker Maintenance Mode
 Move Worker in Pre-Maintenance Mode.
 ```
 $ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode PreMaint --deadline '2022-12-26T22:29:51.214418+00:00' --end '2022-12-30T22:29:51.214418+00:00' --workers renc-w1.fabric-testbed.net
 ```
 Move Worker in Maintenance Mode.
 ```
-$ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode Maint
+$ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode Maint --workers renc-w1.fabric-testbed.net
 ```
 Move Worker in Active Mode
 ```
-$ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode Active
+$ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode Active --workers renc-w1.fabric-testbed.net
 ```
 
 ### Network Management Commands
 List of the Network Management commands supported can be found below:
 ```
 $ fabric-mgmt-cli net
 Usage: fabric-mgmt-cli net [OPTIONS] COMMAND [ARGS]...
@@ -281,8 +266,8 @@
   --help  Show this message and exit.
 
 Commands:
   create  Create a new network service
   delete  Delete an existing network service by name
   show    Subgroup for network information commands
   sync    Control NSO device synchronization
-```
+```
```

### Comparing `fabric-mgmt-cli-1.4.0b4/README.md` & `fabric-mgmt-cli-1.5.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: fabric-mgmt-cli
+Version: 1.5.0b1
+Summary: FABRIC Management CLI
+Keywords: Swagger,Fabric Management Cli
+Author-email: Komal Thareja <kthare10@renci.org>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Dist: click==7.1.2
+Requires-Dist: pytest==7.1.1
+Requires-Dist: fabric-cf==1.4.0
+Requires-Dist: fabric-credmgr-client==1.5.0b4
+Requires-Dist: coverage>=4.0.3 ; extra == "test"
+Requires-Dist: nose>=1.3.7 ; extra == "test"
+Requires-Dist: pluggy>=0.3.1 ; extra == "test"
+Requires-Dist: py>=1.4.31 ; extra == "test"
+Requires-Dist: randomize>=0.13 ; extra == "test"
+Project-URL: Home, https://fabric-testbed.net/
+Project-URL: Sources, https://github.com/fabric-testbed/ManagementCli
+Provides-Extra: test
+
 [![Requirements Status](https://requires.io/github/fabric-testbed/ManagementCli/requirements.svg?branch=main)](https://requires.io/github/fabric-testbed/ManagementCli/requirements/?branch=main)
 
 [![PyPI](https://img.shields.io/pypi/v/fabric-mgmt-cli?style=plastic)](https://pypi.org/project/fabric-mgmt-cli/)
 
 # ManagementCli
 Fabric Control Framework Management CLI for administrative operations over Kafka
 
@@ -243,19 +267,19 @@
 ##### Change Worker Maintenance Mode
 Move Worker in Pre-Maintenance Mode.
 ```
 $ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode PreMaint --deadline '2022-12-26T22:29:51.214418+00:00' --end '2022-12-30T22:29:51.214418+00:00' --workers renc-w1.fabric-testbed.net
 ```
 Move Worker in Maintenance Mode.
 ```
-$ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode Maint
+$ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode Maint --workers renc-w1.fabric-testbed.net
 ```
 Move Worker in Active Mode
 ```
-$ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode Active
+$ fabric-mgmt-cli maintenance site --name RENC --actor orchestrator --mode Active --workers renc-w1.fabric-testbed.net
 ```
 
 ### Network Management Commands
 List of the Network Management commands supported can be found below:
 ```
 $ fabric-mgmt-cli net
 Usage: fabric-mgmt-cli net [OPTIONS] COMMAND [ARGS]...
@@ -266,8 +290,8 @@
   --help  Show this message and exit.
 
 Commands:
   create  Create a new network service
   delete  Delete an existing network service by name
   show    Subgroup for network information commands
   sync    Control NSO device synchronization
-```
+```
```

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/command.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/command.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/config_processor.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/config_processor.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/configuration.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/kafka_processor.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/kafka_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,27 +189,27 @@
         tokens = None
         if refresh_token is None:
             refresh_token = os.getenv('FABRIC_REFRESH_TOKEN', None)
 
         if refresh_token is not None:
             try:
                 proxy = CredmgrProxy(credmgr_host=self.config_processor.get_credmgr_host())
-                tokens = proxy.refresh(project_name="all", scope="all", refresh_token=refresh_token)
+                tokens = proxy.refresh(project_id=None, scope="all", refresh_token=refresh_token)
                 id_token = tokens.get('id_token', None)
             except Exception as e:
                 raise TokenException('Not a valid refresh_token! Error: {}'.format(e))
 
         if id_token is None:
             id_token = os.getenv('FABRIC_ID_TOKEN', None)
             raise TokenException('Either id_token or refresh_token must be specified! Alternatively, '
                                  'set the environment variables FABRIC_ID_TOKEN and FABRIC_REFRESH_TOKEN')
 
         return id_token
 
-    def start(self, id_token: str, refresh_token: str, ignore_tokens: bool = False) -> str:
+    def start(self, id_token: str = None, refresh_token: str = None, ignore_tokens: bool = False) -> str:
         """
         Start Synchronous Kafka Processor
         @param id_token identity token
         @param refresh_token refresh token
         @param ignore_tokens flag  to indicate to ignore tokens
         @return token if ignore_tokens is False; None otherwise
         """
```

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/managecli.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/managecli.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import os
 import click
 
 from fabric_mgmt_cli.managecli.kafka_processor import KafkaProcessorSingleton
 from fabric_mgmt_cli.managecli.manage_command import ManageCommand
 from fabric_mgmt_cli.managecli.show_command import ShowCommand
 from fabric_mgmt_cli.managecli.net import commands as netcommands
-
+import traceback
 
 @click.group()
 @click.option('-v', '--verbose', is_flag=True)
 @click.pass_context
 def managecli(ctx, verbose):
     ctx.ensure_object(dict)
     ctx.obj['VERBOSE'] = verbose
@@ -72,14 +72,33 @@
         # traceback.print_exc()
         click.echo('Error occurred: {}'.format(e))
 
 
 @slices.command()
 @click.option('--sliceid', help='Slice Id', required=True)
 @click.option('--actor', help='Actor Name', required=True)
+@click.option('--endtime', help='New Lease End Time', required=True)
+@click.pass_context
+def renew(ctx, sliceid, actor, endtime):
+    """ Renews slice for an actor
+    """
+    try:
+        KafkaProcessorSingleton.get().start(ignore_tokens=True)
+        mgmt_command = ManageCommand(logger=KafkaProcessorSingleton.get().logger)
+        mgmt_command.renew_slice(slice_id=sliceid, actor_name=actor, end_time=endtime,
+                                 callback_topic=KafkaProcessorSingleton.get().get_callback_topic())
+        KafkaProcessorSingleton.get().stop()
+    except Exception as e:
+        # traceback.print_exc()
+        click.echo('Error occurred: {}'.format(e))
+
+
+@slices.command()
+@click.option('--sliceid', help='Slice Id', required=True)
+@click.option('--actor', help='Actor Name', required=True)
 @click.option('--idtoken', default=None, help='Fabric Identity Token', required=False)
 @click.option('--refreshtoken', default=None, help='Fabric Refresh Token', required=False)
 @click.pass_context
 def remove(ctx, sliceid, actor, idtoken, refreshtoken):
     """ Removes slice for an actor
     """
     try:
@@ -92,24 +111,23 @@
         # traceback.print_exc()
         click.echo('Error occurred: {}'.format(e))
 
 
 @slices.command()
 @click.option('--email', help='User Email', required=True)
 @click.option('--actor', help='Actor Name', required=True)
-@click.option('--idtoken', default=None, help='Fabric Identity Token', required=False)
-@click.option('--refreshtoken', default=None, help='Fabric Refresh Token', required=False)
+@click.option('--sliceid', help='Slice Id', required=False)
 @click.pass_context
-def removealldead(ctx, email, actor, idtoken, refreshtoken):
+def removealldead(ctx, email, actor, sliceid):
     """ Removes slice for an actor
     """
     try:
-        idtoken = KafkaProcessorSingleton.get().start(id_token=idtoken, refresh_token=refreshtoken, ignore_tokens=True)
+        idtoken = KafkaProcessorSingleton.get().start(ignore_tokens=True)
         mgmt_command = ManageCommand(logger=KafkaProcessorSingleton.get().logger)
-        mgmt_command.delete_dead_slices(email=email, actor_name=actor, id_token=idtoken,
+        mgmt_command.delete_dead_slices(email=email, actor_name=actor, id_token=idtoken, slice_id=sliceid,
                                         callback_topic=KafkaProcessorSingleton.get().get_callback_topic())
         KafkaProcessorSingleton.get().stop()
     except Exception as e:
         # traceback.print_exc()
         click.echo('Error occurred: {}'.format(e))
 
 
@@ -135,32 +153,34 @@
                                 slice_id=sliceid, slice_name=slicename, id_token=idtoken, email=email, states=states,
                                 format=format)
         KafkaProcessorSingleton.get().stop()
     except Exception as e:
         # traceback.print_exc()
         click.echo('Error occurred: {}'.format(e))
 
+'''
 @slices.command()
-@click.option('--email', help='User Email', required=True)
-@click.option('--actor', help='Actor Name', required=True)
-@click.option('--idtoken', default=None, help='Fabric Identity Token', required=False)
-@click.option('--refreshtoken', default=None, help='Fabric Refresh Token', required=False)
+@click.option('--actor', default=None, help='Actor Name', required=True)
+@click.option('--sliceid', default=None, help='Slice ID', required=False)
+@click.option('--slicename', default=None, help='Slice Name', required=False)
 @click.pass_context
-def removealldead(ctx, email, actor, idtoken, refreshtoken):
-    """ Removes slice for an actor
+def create(ctx, actor, sliceid, slicename):
+    """ Get slice(s) from an actor
     """
     try:
-        idtoken = KafkaProcessorSingleton.get().start(id_token=idtoken, refresh_token=refreshtoken, ignore_tokens=True)
+        idtoken = KafkaProcessorSingleton.get().start(ignore_tokens=True)
         mgmt_command = ManageCommand(logger=KafkaProcessorSingleton.get().logger)
-        mgmt_command.delete_dead_slices(email=email, actor_name=actor, id_token=idtoken,
-                                        callback_topic=KafkaProcessorSingleton.get().get_callback_topic())
+        mgmt_command.create_slice(actor_name=actor, callback_topic=KafkaProcessorSingleton.get().get_callback_topic(),
+                                  slice_id=sliceid, slice_name=slicename)
         KafkaProcessorSingleton.get().stop()
     except Exception as e:
         # traceback.print_exc()
         click.echo('Error occurred: {}'.format(e))
+'''
+
 
 @click.group()
 @click.pass_context
 def slivers(ctx):
     """ Sliver management
     """
     config = os.getenv('FABRIC_MGMT_CLI_CONFIG_PATH')
@@ -379,15 +399,15 @@
     if config is None or config == "":
         ctx.fail('FABRIC_MGMT_CLI_CONFIG_PATH is not set')
 
     return
 
 
 @maintenance.command()
-@click.option('--actor', help='Actor Name', required=True)
+@click.option('--actors', help='Comma separated list of Actor names', required=True)
 @click.option('--mode', help='Mode value, i.e. PreMaint, Maint, Active', required=True)
 @click.option('--projects', help='Comma separated list of Project Ids allowed to use TestBed in Maintenance mode',
               required=False, default=None)
 @click.option('--users', help='Comma separated list of User emails allowed to use TestBed in Maintenance mode',
               required=False, default=None)
 @click.option('--deadline',
               help='Start time that allows new resources to be created or extended up '
@@ -395,33 +415,37 @@
               required=False, default=None)
 @click.option('--end',
               help='Expected End for the Maintainenance in formt: %Y-%m-%d %H:%M:%S %z',
               required=False, default=None)
 @click.option('--idtoken', default=None, help='Fabric Identity Token', required=False)
 @click.option('--refreshtoken', default=None, help='Fabric Refresh Token', required=False)
 @click.pass_context
-def testbed(ctx, actor: str, mode: str, projects: str, users: str, deadline: str, end: str, idtoken: str,
+def testbed(ctx, actors: str, mode: str, projects: str, users: str, deadline: str, end: str, idtoken: str,
             refreshtoken: str):
     """ Change Maintenance modes (PreMaint, Maint, Active) for the Testbed
     """
     try:
         idtoken = KafkaProcessorSingleton.get().start(id_token=idtoken, refresh_token=refreshtoken, ignore_tokens=True)
         mgmt_command = ManageCommand(logger=KafkaProcessorSingleton.get().logger)
-        mgmt_command.toggle_maintenance_mode(actor_name=actor,
-                                             callback_topic=KafkaProcessorSingleton.get().get_callback_topic(),
-                                             state=mode, projects=projects, users=users, id_token=idtoken,
-                                             deadline=deadline, expected_end=end)
+        actors = actors.strip()
+        actor_list = actors.split(",")
+        for actor in actor_list:
+            actor = actor.strip()
+            mgmt_command.toggle_maintenance_mode(actor_name=actor,
+                                                 callback_topic=KafkaProcessorSingleton.get().get_callback_topic(),
+                                                 state=mode, projects=projects, users=users, id_token=idtoken,
+                                                 deadline=deadline, expected_end=end)
         KafkaProcessorSingleton.get().stop()
     except Exception as e:
         # traceback.print_exc()
         click.echo('Error occurred: {}'.format(e))
 
 
 @maintenance.command()
-@click.option('--actor', help='Actor Name', required=True)
+@click.option('--actors', help='Comma separated list of Actor names', required=True)
 @click.option('--name', help='Site Name', required=True)
 @click.option('--mode', help='Mode value, i.e. PreMaint, Maint, Active', required=True)
 @click.option('--projects', help='Comma separated list of Project Ids allowed to use TestBed in Maintenance mode',
               required=False, default=None)
 @click.option('--users', help='Comma separated list of User emails allowed to use TestBed in Maintenance mode',
               required=False, default=None)
 @click.option('--workers', help='Comma separated list of workers to be marked in Maintenance mode',
@@ -432,50 +456,113 @@
               required=False, default=None)
 @click.option('--end',
               help='Expected End for the Maintainenance in formt: %Y-%m-%d %H:%M:%S %z',
               required=False, default=None)
 @click.option('--idtoken', default=None, help='Fabric Identity Token', required=False)
 @click.option('--refreshtoken', default=None, help='Fabric Refresh Token', required=False)
 @click.pass_context
-def site(ctx, actor: str, name: str, mode: str, projects, users, workers: str, deadline: str, end: str,
+def site(ctx, actors: str, name: str, mode: str, projects, users, workers: str, deadline: str, end: str,
          idtoken: str, refreshtoken: str):
     """ Change Maintenance modes (PreMaint, Maint, Active) for a specific Site or a specific worker
     """
     try:
         idtoken = KafkaProcessorSingleton.get().start(id_token=idtoken, refresh_token=refreshtoken, ignore_tokens=True)
         mgmt_command = ManageCommand(logger=KafkaProcessorSingleton.get().logger)
-        mgmt_command.toggle_maintenance_mode(actor_name=actor,
-                                             callback_topic=KafkaProcessorSingleton.get().get_callback_topic(),
-                                             state=mode, projects=projects, users=users, expected_end=end,
-                                             site_name=name, workers=workers, deadline=deadline, id_token=idtoken)
+        actors = actors.strip()
+        actor_list = actors.split(",")
+        for actor in actor_list:
+            actor = actor.strip()
+            mgmt_command.toggle_maintenance_mode(actor_name=actor,
+                                                 callback_topic=KafkaProcessorSingleton.get().get_callback_topic(),
+                                                 state=mode, projects=projects, users=users, expected_end=end,
+                                                 site_name=name, workers=workers, deadline=deadline, id_token=idtoken)
 
         KafkaProcessorSingleton.get().stop()
     except Exception as e:
         # traceback.print_exc()
         click.echo('Error occurred: {}'.format(e))
-'''
+
 
 @maintenance.command()
-@click.option('--actor', help='Actor Name', required=True)
-@click.option('--site', help='Site Name', required=False)
+@click.option('--actors', help='Comma separated list of Actor names', required=True)
+@click.option('--sites', help='Site Names, Comma separated list of the site names or ALL for entire testbed', required=False)
+@click.option('--format', default='text', help='Output Format Type: text or json', required=False)
 @click.pass_context
-def query(ctx, actor: str, site: str):
+def query(ctx, actors: str, sites: str, format:str):
     """ Query Maintenance Status for Testbed/Site
     """
     try:
         idtoken = KafkaProcessorSingleton.get().start(ignore_tokens=True)
-        mgmt_command = ManageCommand(logger=KafkaProcessorSingleton.get().logger)
-        mgmt_command.get_maintenance_mode(actor_name=actor,
-                                          callback_topic=KafkaProcessorSingleton.get().get_callback_topic(),
-                                          site=site)
+        mgmt_command = ShowCommand(logger=KafkaProcessorSingleton.get().logger)
+        actors = actors.strip()
+        actor_list = actors.split(",")
+        for actor in actor_list:
+            actor = actor.strip()
+            mgmt_command.get_sites(actor_name=actor,
+                                   callback_topic=KafkaProcessorSingleton.get().get_callback_topic(),
+                                   sites=sites, format=format)
 
         KafkaProcessorSingleton.get().stop()
     except Exception as e:
         # traceback.print_exc()
         click.echo('Error occurred: {}'.format(e))
-'''
+
+
+@maintenance.command()
+@click.option('--oc', help='Orchestrator Name', required=True)
+@click.option('--broker', help='Broker Name', required=True)
+@click.option('--am', help='Am Name', required=True)
+@click.option('--sliceid', help='Slice Id', required=False)
+@click.option('--sliverid', help='Sliver Id', required=False)
+@click.option('--site', help='Site Name', required=False)
+@click.option('--type', default=None,
+              help='Sliver Type, possible allowed values: '
+                   '[VM, L2Bridge, L2STS, L2PTP, FABNetv4, FABNetv6, FABNetv4Ext, '
+                   'FABNetv6Ext, PortMirror, Facility, L3VPN]',
+              required=False)
+@click.pass_context
+def audit(ctx, oc: str, broker: str, am: str, sliceid: str, sliverid: str, site: str, type: str):
+    """ Audit Sliver state across various Control Framework actors, report discrepancies found.
+    """
+    try:
+        KafkaProcessorSingleton.get().start(ignore_tokens=True)
+        mgmt_command = ManageCommand(logger=KafkaProcessorSingleton.get().logger)
+        mgmt_command.do_audit(oc_name=oc, br_name=broker, am_name=am, slice_id=sliceid,
+                              sliver_id=sliverid, site_name=site, sliver_type=type,
+                              callback_topic=KafkaProcessorSingleton.get().get_callback_topic())
+        KafkaProcessorSingleton.get().stop()
+    except Exception as e:
+        traceback.print_exc()
+        click.echo('Error occurred: {}'.format(e))
+
+
+@maintenance.command()
+@click.option('--am', help='Am Name', required=True)
+@click.option('--sliceid', help='Slice Id', required=False)
+@click.option('--sliverid', help='Sliver Id', required=False)
+@click.option('--site', help='Site Name', required=False)
+@click.option('--type', default=None,
+              help='Sliver Type, possible allowed values: '
+                   '[VM, L2Bridge, L2STS, L2PTP, FABNetv4, FABNetv6, FABNetv4Ext, '
+                   'FABNetv6Ext, PortMirror, Facility, L3VPN]',
+              required=False)
+@click.pass_context
+def audit_infra(ctx, am: str, sliceid: str, sliverid: str, site: str, type: str):
+    """ Audit AM Sliver state against the underlying infrastructure, report discrepancies found.
+    """
+    try:
+        KafkaProcessorSingleton.get().start(ignore_tokens=True)
+        mgmt_command = ManageCommand(logger=KafkaProcessorSingleton.get().logger)
+        mgmt_command.do_audit_infra(am_name=am, slice_id=sliceid,
+                                    sliver_id=sliverid, site_name=site, sliver_type=type,
+                                    callback_topic=KafkaProcessorSingleton.get().get_callback_topic())
+        KafkaProcessorSingleton.get().stop()
+    except Exception as e:
+        traceback.print_exc()
+        click.echo('Error occurred: {}'.format(e))
+
 
 managecli.add_command(slices)
 managecli.add_command(slivers)
 managecli.add_command(delegations)
 managecli.add_command(maintenance)
 managecli.add_command(netcommands.net)
```

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/commands.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/commands.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/nso.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/nso.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/resources.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/services.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/services.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/net/util.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/net/util.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/show_command.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/show_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 from fabric_cf.actor.core.kernel.reservation_states import ReservationStates, ReservationPendingStates
 from fabric_cf.actor.core.kernel.slice_state_machine import SliceState
 from fabric_cf.actor.core.manage.error import Error
 from fabric_cf.actor.core.time.actor_clock import ActorClock
 from fabric_cf.actor.core.util.id import ID
 from fabric_cf.actor.core.util.utils import sliver_to_str
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
+from fabric_mb.message_bus.messages.lease_reservation_avro import LeaseReservationAvro
 from fabric_mb.message_bus.messages.reservation_mng import ReservationMng
+from fabric_mb.message_bus.messages.site_avro import SiteAvro
 from fabric_mb.message_bus.messages.slice_avro import SliceAvro
 from fim.graph.abc_property_graph import ABCPropertyGraph
 from fim.slivers.network_node import NodeSliver
 from fim.slivers.network_service import NetworkServiceSliver
 
 from fabric_mgmt_cli.managecli.command import Command
 
@@ -100,14 +102,15 @@
             sid = ID(uid=slice_id) if slice_id is not None else None
             slice_states = None
             if states is not None:
                 states_list = states.split(",")
                 for x in states_list:
                     if slice_states is None:
                         slice_states = []
+                    x = x.strip()
                     slice_states.append(SliceState.translate(state_name=x).value)
 
             result = actor.get_slices(slice_id=sid, slice_name=slice_name, email=email, states=slice_states)
             return result, actor.get_last_error()
         except Exception:
             ex_str = traceback.format_exc()
             self.logger.error(ex_str)
@@ -124,16 +127,17 @@
             actor.prepare(callback_topic=callback_topic)
             sid = ID(uid=slice_id) if slice_id is not None else None
             reservation_id = ID(uid=rid) if rid is not None else None
             reservation_states = None
             if states is not None:
                 states_list = states.split(",")
                 for x in states_list:
-                    if reservation_states is not None:
+                    if reservation_states is None:
                         reservation_states = []
+                    x = x.strip()
                     reservation_states.append(ReservationStates.translate(state_name=x).value)
             return actor.get_reservations(slice_id=sid, rid=reservation_id, states=reservation_states, email=email,
                                           site=site, type=type), actor.get_last_error()
         except Exception as e:
             ex_str = traceback.format_exc()
             self.logger.error(ex_str)
         return None, actor.get_last_error()
@@ -150,14 +154,15 @@
             if slice_id is not None:
                 sid = ID(uid=slice_id)
             delegation_states = None
             if states is not None:
                 for x in states:
                     if delegation_states is None:
                         delegation_states = []
+                    x = x.strip()
                     delegation_states.append(DelegationState.translate(state_name=x).value)
             return actor.get_delegations(delegation_id=did, slice_id=sid,
                                          states=delegation_states), actor.get_last_error()
         except Exception as e:
             self.logger.error(f"Exception occurred while fetching delegations: e {e}")
             self.logger.error(traceback.format_exc())
             traceback.print_exc()
@@ -178,21 +183,21 @@
             if reservation.rtype is not None and (field_list is None or 'type' in field_list):
                 res_dict['type'] = reservation.rtype
 
             if reservation.rtype is not None and (field_list is None or 'notices' in field_list):
                 res_dict['notices'] = reservation.notices
 
             if reservation.start is not None and (field_list is None or 'start' in field_list):
-                res_dict['start'] = ShowCommand.__time_string(milliseconds=reservation.start)
+                res_dict['start'] = ShowCommand.time_string(milliseconds=reservation.start)
 
             if reservation.end is not None and (field_list is None or 'end' in field_list):
-                res_dict['end'] = ShowCommand.__time_string(milliseconds=reservation.end)
+                res_dict['end'] = ShowCommand.time_string(milliseconds=reservation.end)
 
             if reservation.requested_end is not None and (field_list is None or 'requested_end' in field_list):
-                res_dict['requested_end'] = ShowCommand.__time_string(milliseconds=reservation.requested_end)
+                res_dict['requested_end'] = ShowCommand.time_string(milliseconds=reservation.requested_end)
 
             if reservation.units is not None and (field_list is None or 'units' in field_list):
                 res_dict['units'] = reservation.units
 
             if reservation.state is not None and (field_list is None or 'state' in field_list):
                 res_dict['state'] = reservation.state
 
@@ -221,22 +226,27 @@
         """
         print("")
         print(f"Reservation ID: {reservation.reservation_id} Slice ID: {reservation.slice_id}")
         if reservation.rtype is not None or reservation.notices is not None:
             print(f"Resource Type: {reservation.rtype} Notices: {reservation.notices}")
 
         if reservation.start is not None or reservation.end is not None or reservation.requested_end is not None:
-            print(f"Start: {ShowCommand.__time_string(milliseconds=reservation.start)} "
-                  f"End: {ShowCommand.__time_string(milliseconds=reservation.end)} "
-                  f"Requested End: {ShowCommand.__time_string(milliseconds=reservation.requested_end)}")
+            print(f"Start: {ShowCommand.time_string(milliseconds=reservation.start)} "
+                  f"End: {ShowCommand.time_string(milliseconds=reservation.end)} "
+                  f"Requested End: {ShowCommand.time_string(milliseconds=reservation.requested_end)}")
 
         if reservation.units is not None or reservation.state is not None or reservation.pending_state is not None:
             print(f"Units: {reservation.units} State: {ReservationStates(reservation.state)} "
                   f"Pending State: {ReservationPendingStates(reservation.pending_state)}")
 
+        if isinstance(reservation, LeaseReservationAvro) and reservation.redeem_processors is not None:
+            print(f"Predecessors")
+            for x in reservation.redeem_processors:
+                print(x.get_reservation_id())
+
         sliver = reservation.get_sliver()
         if sliver is not None:
             print(f"Sliver: {sliver_to_str(sliver=sliver)}")
         print("")
 
     @staticmethod
     def __print_node_sliver(*, sliver: NodeSliver):
@@ -247,26 +257,26 @@
     @staticmethod
     def __print_ns_sliver(*, sliver: NetworkServiceSliver):
         if sliver.interface_info is not None:
             for c in sliver.interface_info.interfaces.values():
                 print(c)
 
     @staticmethod
-    def __time_string(*, milliseconds):
+    def time_string(*, milliseconds):
         time_obj = ActorClock.from_milliseconds(milli_seconds=milliseconds)
         return time_obj.strftime(Constants.LEASE_TIME_FORMAT)
 
     @staticmethod
     def __print_slice(*, slice_object: SliceAvro):
         """
         Prints Slice Object
         """
         print("")
         print(f"Slice Name: {slice_object.get_slice_name()} Slice ID: {slice_object.get_slice_id()} "
-              f"Project ID: {slice_object.get_slice_id()}")
+              f"Project ID: {slice_object.get_project_id()} Project Name: {slice_object.get_project_name()} ")
         if slice_object.get_graph_id() is not None:
             print(f"Graph ID: {slice_object.get_graph_id()}")
 
         if slice_object.get_owner() is not None:
             print(f"Slice owner: {slice_object.get_owner()}")
 
         if slice_object.get_state() is not None:
@@ -282,14 +292,15 @@
         Prints Slice Object
         """
         slc_list = []
         for slice_object in slices:
             slc_dict = {'name': slice_object.get_slice_name(),
                         'slice_id': slice_object.get_slice_id(),
                         'project_id': slice_object.get_project_id(),
+                        'project_name': slice_object.get_project_name(),
                         'graph_id': slice_object.get_graph_id(),
                         'owner': slice_object.get_owner().get_email(),
                         'state': str(SliceState(slice_object.get_state())),
                         'lease_start_time': str(slice_object.get_lease_start()),
                         'lease_end_time': str(slice_object.get_lease_end())
                         }
             slc_list.append(slc_dict)
@@ -308,14 +319,16 @@
         """
         Prints the Delegation Object
         """
         print("")
         print("Delegation ID: {} Slice ID: {}".format(dlg_object.delegation_id, dlg_object.slice.get_slice_id()))
         if dlg_object.delegation_name is not None:
             print("Delegation Name: {}".format(dlg_object.delegation_name))
+        if dlg_object.site is not None:
+            print("Site Name: {}".format(dlg_object.site))
         if dlg_object.sequence is not None:
             print("Sequence: {}".format(dlg_object.sequence))
         if dlg_object.state is not None:
             print(f"State: {DelegationState(dlg_object.state)}")
         if dlg_object.graph is not None:
             print("Graph: {}".format(dlg_object.graph))
         print("")
@@ -339,8 +352,50 @@
         print(json.dumps(dlg_list, indent=4))
 
     def __print_delegations(self, *, delegations: List[DelegationAvro], format: str):
         if format == 'text':
             for d in delegations:
                 self.__print_delegation(dlg_object=d)
         else:
-            self.__print_delegations_json(delegations=delegations)
+            self.__print_delegations_json(delegations=delegations)
+
+    def do_get_sites(self, *, actor_name: str, callback_topic: str, sites: str) -> Tuple[List[SiteAvro] or None, Error]:
+        actor = self.get_actor(actor_name=actor_name)
+
+        if actor is None:
+            raise Exception("Invalid arguments actor {} not found".format(actor_name))
+        try:
+            actor.prepare(callback_topic=callback_topic)
+            return actor.get_sites(site=sites.upper()), actor.get_last_error()
+        except Exception as e:
+            self.logger.error(f"Exception occurred while fetching delegations: e {e}")
+            self.logger.error(traceback.format_exc())
+            traceback.print_exc()
+        return None, actor.get_last_error()
+
+    def get_sites(self, *, actor_name: str, callback_topic: str, sites:str, format: str):
+        try:
+            sites, error = self.do_get_sites(actor_name=actor_name, callback_topic=callback_topic, sites=sites)
+            if sites is not None and len(sites) > 0:
+                self.__print_sites(sites=sites, format=format, actor_name=actor_name)
+            else:
+                print(f"Status of {actor_name}: {error.get_status()}")
+        except Exception as e:
+            ex_str = traceback.format_exc()
+            self.logger.error(ex_str)
+            print("Exception occurred while processing get_delegations {}".format(e))
+
+    def __print_sites(self, *, sites: List[SiteAvro], format: str, actor_name:str):
+        if format == 'text':
+            print(f"Actor: {actor_name}")
+            for s in sites:
+                print(s)
+        else:
+            site_list = []
+            for s in sites:
+                s_dict = {
+                    'name': s.get_name(),
+                    'maint_info': s.get_maint_info().to_json()
+                }
+                site_list.append(s_dict)
+            maint_info = {actor_name: site_list}
+            print(json.dumps(maint_info, indent=4))
```

### Comparing `fabric-mgmt-cli-1.4.0b4/fabric_mgmt_cli/managecli/test/test_managecli.py` & `fabric-mgmt-cli-1.5.0b1/fabric_mgmt_cli/managecli/test/test_managecli.py`

 * *Files identical despite different names*

