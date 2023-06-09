# Comparing `tmp/clenv-0.0.4.tar.gz` & `tmp/clenv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clenv-0.0.4.tar", last modified: Wed Apr 26 10:21:01 2023, max compression
+gzip compressed data, was "clenv-0.0.6.tar", last modified: Fri Jun  9 20:16:03 2023, max compression
```

## Comparing `clenv-0.0.4.tar` & `clenv-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-04-26 10:21:01.319038 clenv-0.0.4/
--rw-r--r--   0 brainco    (501) staff       (20)     1067 2023-04-26 09:03:52.000000 clenv-0.0.4/LICENSE
--rw-r--r--   0 brainco    (501) staff       (20)     2623 2023-04-26 10:21:01.318635 clenv-0.0.4/PKG-INFO
--rw-r--r--   0 brainco    (501) staff       (20)     1940 2023-04-26 08:28:28.000000 clenv-0.0.4/README.md
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-04-26 10:21:01.311910 clenv-0.0.4/clenv/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 09:54:11.000000 clenv-0.0.4/clenv/__init__.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-04-26 10:21:01.315229 clenv-0.0.4/clenv/cli/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:03:58.000000 clenv-0.0.4/clenv/cli/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)      316 2023-04-26 10:12:55.000000 clenv-0.0.4/clenv/cli/__main__.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-04-26 10:21:01.317007 clenv-0.0.4/clenv/cli/config/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:04:34.000000 clenv-0.0.4/clenv/cli/config/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)    13596 2023-04-26 07:35:54.000000 clenv-0.0.4/clenv/cli/config/config_manager.py
--rw-r--r--   0 brainco    (501) staff       (20)     5224 2023-04-26 10:09:13.000000 clenv-0.0.4/clenv/cli/config/config_subcommand.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-04-26 10:21:01.317970 clenv-0.0.4/clenv/cli/user/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:05:30.000000 clenv-0.0.4/clenv/cli/user/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)     2636 2023-04-26 10:05:45.000000 clenv-0.0.4/clenv/cli/user/user_subcommand.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-04-26 10:21:01.314395 clenv-0.0.4/clenv.egg-info/
--rw-r--r--   0 brainco    (501) staff       (20)     2623 2023-04-26 10:21:01.000000 clenv-0.0.4/clenv.egg-info/PKG-INFO
--rw-r--r--   0 brainco    (501) staff       (20)      427 2023-04-26 10:21:01.000000 clenv-0.0.4/clenv.egg-info/SOURCES.txt
--rw-r--r--   0 brainco    (501) staff       (20)        1 2023-04-26 10:21:01.000000 clenv-0.0.4/clenv.egg-info/dependency_links.txt
--rw-r--r--   0 brainco    (501) staff       (20)       50 2023-04-26 10:21:01.000000 clenv-0.0.4/clenv.egg-info/entry_points.txt
--rw-r--r--   0 brainco    (501) staff       (20)       59 2023-04-26 10:21:01.000000 clenv-0.0.4/clenv.egg-info/requires.txt
--rw-r--r--   0 brainco    (501) staff       (20)        6 2023-04-26 10:21:01.000000 clenv-0.0.4/clenv.egg-info/top_level.txt
--rw-r--r--   0 brainco    (501) staff       (20)       38 2023-04-26 10:21:01.319149 clenv-0.0.4/setup.cfg
--rw-r--r--   0 brainco    (501) staff       (20)     1147 2023-04-26 10:20:37.000000 clenv-0.0.4/setup.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.788407 clenv-0.0.6/
+-rw-r--r--   0 brainco    (501) staff       (20)     1067 2023-04-26 09:03:52.000000 clenv-0.0.6/LICENSE
+-rw-r--r--   0 brainco    (501) staff       (20)     4138 2023-06-09 20:16:03.787797 clenv-0.0.6/PKG-INFO
+-rw-r--r--   0 brainco    (501) staff       (20)     3455 2023-06-09 19:54:28.000000 clenv-0.0.6/README.md
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.776973 clenv-0.0.6/clenv/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 09:54:11.000000 clenv-0.0.6/clenv/__init__.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.780617 clenv-0.0.6/clenv/cli/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:03:58.000000 clenv-0.0.6/clenv/cli/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)      390 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/__main__.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.783058 clenv-0.0.6/clenv/cli/config/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:04:34.000000 clenv-0.0.6/clenv/cli/config/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)      828 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/config/config_loader.py
+-rw-r--r--   0 brainco    (501) staff       (20)    14187 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/config/config_manager.py
+-rw-r--r--   0 brainco    (501) staff       (20)     5650 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/config/config_subcommand.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.784275 clenv-0.0.6/clenv/cli/queue/
+-rw-r--r--   0 brainco    (501) staff       (20)       13 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/queue/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)     2182 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/queue/queue_manager.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.785563 clenv-0.0.6/clenv/cli/task/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/task/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)     8320 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/task/task_subcommand.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.786888 clenv-0.0.6/clenv/cli/user/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:05:30.000000 clenv-0.0.6/clenv/cli/user/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)     2724 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/user/user_subcommand.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.779948 clenv-0.0.6/clenv.egg-info/
+-rw-r--r--   0 brainco    (501) staff       (20)     4138 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/PKG-INFO
+-rw-r--r--   0 brainco    (501) staff       (20)      583 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/SOURCES.txt
+-rw-r--r--   0 brainco    (501) staff       (20)        1 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/dependency_links.txt
+-rw-r--r--   0 brainco    (501) staff       (20)       50 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/entry_points.txt
+-rw-r--r--   0 brainco    (501) staff       (20)       59 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/requires.txt
+-rw-r--r--   0 brainco    (501) staff       (20)        6 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/top_level.txt
+-rw-r--r--   0 brainco    (501) staff       (20)       38 2023-06-09 20:16:03.788598 clenv-0.0.6/setup.cfg
+-rw-r--r--   0 brainco    (501) staff       (20)     1147 2023-06-09 19:36:56.000000 clenv-0.0.6/setup.py
```

### Comparing `clenv-0.0.4/LICENSE` & `clenv-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clenv-0.0.4/PKG-INFO` & `clenv-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clenv
-Version: 0.0.4
+Version: 0.0.6
 Summary: ClearML config profile manager
 Home-page: https://github.com/DavidSonoda/clenv
 Author: Juewei Dong
 Author-email: juewei.dong@brainco.tech
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# clenv - Clearml environment profile manager
+# clenv - Unofficial ClearML CLI helper
 
 
 
 ## Pre-requisites
 
 - `clearml` installed, please refer to [ClearML installation guide](https://clear.ml/docs/latest/docs/getting_started/ds/ds_first_steps) for more details.
 - Run `clearml-init` and initialize your first ever config file.
@@ -32,15 +32,14 @@
 ## Installation
 
 ```bash
 pip install clenv
 ```
 
 
-
 ## Usage
 
 ### Subcommand `config`
 Note: All config files must be in the format of `clearml-<profile_name>.conf`
 
 #### List all config profiles
 ```bash
@@ -72,47 +71,80 @@
 ### Subcommand `user`
 
 #### Generate user/password hocon config
 ```bash
 clenv user genpass <user_name>
 ```
 
+### Subcommand `task`
+
+> Note: This command only support git repos for now. The project name of the task created on the ClearML server will be the same as the git repo name. So please make sure you have a meaningful, easy to read git repo name.
+
+#### Execute a task remotely on ClearML server
+
+```bash
+clenv task exec
+```
+
+It will prompt you to select an available queue, correct task type, your entrypoint script path and input the task name.
+
+![clenv-task-exec-1](./static/clenv-task-exec-1.png)
+
+After inputting all the required configs, it will ask you whether to save the configs. By typing 'y', the config will be saved. When you execute `clenv task exec` next time in the same repo, it will load the saved configs and skip the config input process. However, it will still ask you for confirmation before submitting the task.
+
+#### Ignore the saved run configs when starting a new execution
+
+If you want to ignore the old run configs and freshly start a new execution, you can run:
+
+```bash
+clenv task exec -N
+```
+
+The `-N` option will tell `clenv` to ignore the config file you have, and prompt you to input all the configs again.
 
+An alternative way of doing that is to delete the config file manually, which is located at `./.clenv/task_template.json`. Then running `clenv task exec` again will start a fresh execution as well.
 
 ## Examples
 
 ### Create a new clearml config profile for privately hosted clearml server 
 
 #### Initialize profiles
 
 ```bash
-$ ./clearenvoy.bin config list
+$ clenv config list
 # Input a name for your current profile
 ```
 
 #### Create a new profile
 
 ```bash
-$ ./clearenvoy.bin config create brainco
+$ clenv config create brainco
 ```
 
 #### Reinit the profile credentials
 
 ```bash
-$ ./clearenvoy.bin config reinit brainco
+$ clenv config reinit brainco
 ```
 
 #### Checkout the new profile
 
 ```bash
-$ ./clearenvoy.bin config checkout brainco
+$ clenv config checkout brainco
 ```
 
 ## Roadmap
-- [x] Config profile management
-- [x] BCrypt password generation
-- [ ] Support custom config file path
-- [ ] Server side utils and config management
-- [ ] ClearML Agent side utils and config management
+- Config management
+  - [x] Config profile management
+  - [ ] Support custom config file path
+- Privately hosted server management
+  - [x] BCrypt password generation (Feature to be deprecated when more sophisticated user management is implemented)
+  - [ ] Server side utils and config management
+  - [ ] ClearML Agent side utils and config management
+- Remote task management
+  - [x] A user friendly remote task execution wizard
+
+
+
 
 ## Disclaimer & License
 This project is not affiliated with Allegro AI, Inc. in any way. It is an independent and unofficial software. It's licensed under the MIT license.
```

### Comparing `clenv-0.0.4/clenv/cli/config/config_manager.py` & `clenv-0.0.6/clenv/cli/config/config_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,32 +8,39 @@
 import re
 import shutil
 from pyhocon import ConfigFactory, HOCONConverter
 
 
 class ConfigManager:
     def __init__(self, index_file_path, save_index=True):
+        """
+        Initialize a new index for the given index file path.
+        :param index_file_path: The file path of the index file.
+        :param save_index: Whether to save the index after refreshing it. Defaults to True.
+        """
         self.__index_file_path = index_file_path
         self.__EMPTY_INDEX_JSON = {"profiles": {"active": [], "non_active": []}}
         index_json = self.__load_index_file(index_file_path)
         self.__new_index_json = self.__refresh_index(index_json)
         if save_index:
             self.save_index()
 
     # Return a list of object, each object has 2 keys:
     # - profile_name
     # - file_path
     # The list should contain all the profiles in the index file, including the active profile
     # and the non-active profiles
     # Solution
     def get_all_profiles(self):
-        return (
-            self.__new_index_json["profiles"]["active"]
-            + self.__new_index_json["profiles"]["non_active"]
-        )
+        # Get all active profiles
+        active_profiles = self.__new_index_json["profiles"]["active"]
+        # Get all non active profiles
+        non_active_profiles = self.__new_index_json["profiles"]["non_active"]
+        # Concatenate both lists and return
+        return active_profiles + non_active_profiles
 
     # Get active profile. Return a list of object, each object has 2 keys:
     # - profile_name
     # - file_path
     def get_active_profile(self):
         return self.__new_index_json["profiles"]["active"]
 
@@ -57,33 +64,38 @@
         ):
             if profile["profile_name"] == "untitled":
                 return False
         return True
 
     # Rename a profile, the old_profile_name could be in both non_active and active list
     def rename_profile(self, old_profile_name, new_profile_name):
+        # Iterate over all profiles
         for profile in (
             self.__new_index_json["profiles"]["active"]
             + self.__new_index_json["profiles"]["non_active"]
         ):
+            # If the profile is found, rename it
             if profile["profile_name"] == old_profile_name:
                 profile["profile_name"] = new_profile_name
                 # If the profile is active, do not rename the config file path
                 # If the profile is non-active, rename the config file path
                 if profile in self.__new_index_json["profiles"]["non_active"]:
+                    # Rename the config file path
                     new_file_path = os.path.expanduser(
                         profile["file_path"].replace(
                             f"clearml-{old_profile_name}.conf",
                             f"clearml-{new_profile_name}.conf",
                         )
                     )
                     os.rename(os.path.expanduser(profile["file_path"]), new_file_path)
                     profile["file_path"] = new_file_path
+                # Save the new index
                 self.save_index()
                 return
+        # If the profile is not found, raise an error
         raise Exception(f"Profile {old_profile_name} does not exist")
 
     def initialize_profile(self, profile_name):
         self.rename_profile("untitled", profile_name)
 
     def is_active_profile(self, profile_name):
         return (
@@ -210,70 +222,68 @@
                 f.write(HOCONConverter.convert(clearml_config))
         except:
             raise Exception("Invalid api_config_str")
 
     def __refresh_index(self, index_json):
         # Scan the home directory
         new_index_json = self.__scan_home_dir()
+
         # If the default profile in index_json is not empty, update the new_index_json with the default profile
         # in index_json
         if len(index_json["profiles"]["active"]) > 0:
             new_index_json["profiles"]["active"] = index_json["profiles"]["active"]
+
         return new_index_json
 
     # Load the json content of the index file, return the json object. If the file
     # is empty or malformed, return an empty json object.
     def __load_index_file(self, file_path):
-        index_file = os.path.expanduser(file_path)
-        if not os.path.exists(index_file) or os.stat(index_file).st_size == 0:
+        index_file_path = os.path.expanduser(file_path)
+        if not os.path.exists(index_file_path) or os.stat(index_file_path).st_size == 0:
             # return an empty json object
             return self.__EMPTY_INDEX_JSON
         else:
             try:
-                with open(index_file, "r") as f:
+                with open(index_file_path, "r") as f:
                     return json.load(f)
             except:
                 return self.__EMPTY_INDEX_JSON
 
-    # Scan the home directory for files that match the criteria:
-    # - the file name ends with .conf
-    # - the file is not a directory
-    # - the file is not a symbolic link
-    # - the file name contains the word clearml
-    # - the file content is in hocon format, using pyhocon library to detect if it is hocon format, throw
-    #   an exception if it is not hocon format
-    # Create a json object for each file, it got 2 keys
-    # - profile name
-    # - file path
-    #
-    # Return a list of json objects. Do not read the index file, just scan the home directory.
-    #
-    # Solution
     def __scan_home_dir(self):
+        # get the home directory
         home_dir = os.path.expanduser("~")
+        # get the list of files in the home directory
         files = os.listdir(home_dir)
+        # create lists to store the active and non-active profiles
         active_profile_list = []
         non_active_profile_list = []
+        # for each file in the home directory
         for file in files:
+            # if the file is a config file
             if (
                 file.endswith(".conf")
                 and not os.path.isdir(file)
                 and not os.path.islink(file)
                 and "clearml" in file
             ):
                 try:
+                    # parse the file
                     ConfigFactory.parse_file(f"{home_dir}/{file}")
+                    # if the file is the active profile
                     if file == "clearml.conf":
+                        # add the file to the list of active profiles
                         active_profile_list.append(
                             {
                                 "profile_name": self.__extract_profile_name(file),
                                 "file_path": f"{home_dir}/{file}",
                             }
                         )
+                    # if the file is not the active profile
                     else:
+                        # add the file to the list of non-active profiles
                         non_active_profile_list.append(
                             {
                                 "profile_name": self.__extract_profile_name(file),
                                 "file_path": f"{home_dir}/{file}",
                             }
                         )
                 except:
@@ -288,13 +298,12 @@
                 "non_active": non_active_profile_list,
             }
         }
 
     # Extract profile name from the file name, if the file name is clearml.conf, the profile name should be default
     # If the file name is clearml-<profile_name>.conf, the profile name should be <profile_name>
     # Use regex to extract the profile name
-    # Solution
     def __extract_profile_name(self, file_name):
         if file_name == "clearml.conf":
             return "untitled"
         else:
             return re.match(r"clearml-(.+)\.conf", file_name).group(1)
```

### Comparing `clenv-0.0.4/clenv/cli/config/config_subcommand.py` & `clenv-0.0.6/clenv/cli/config/config_subcommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,29 +14,32 @@
 
 @click.option(
     "--showpath", "-v", is_flag=True, help="Show config file path for the profile"
 )
 @config.command(help="List all config profiles")
 def list(showpath):
     config_manager = ConfigManager(INDEX_FILE_PATH)
+
+    # If the profile has not been initialized, prompt the user to input a profile name
+    # The default profile name is 'default'
     if not config_manager.profile_has_initialized():
-        # Prompt the user to initalize the profile by inputting a profile name, the default is 'default'
-        # Solution
         profile_name = click.prompt("Please input a profile name", default="default")
         config_manager.initialize_profile(profile_name)
 
     active_profiles = config_manager.get_active_profile()
     non_active_profiles = config_manager.get_non_active_profiles()
+
+    # Print the active profiles
     for profile in active_profiles:
-        # Print the active profile name with '(active)' at the end, print it in green color
         click.echo(click.style(f'{profile["profile_name"]} [active]', fg="green"))
         if showpath:
             click.echo(click.style(f'  {profile["file_path"]}'))
+
+    # Print the non-active profiles
     for profile in non_active_profiles:
-        # Print the non-active profile name, print it in yellow color
         click.echo(click.style(f'{profile["profile_name"]}', fg="yellow"))
         if showpath:
             click.echo(click.style(f'  {profile["file_path"]}'))
 
 
 # Checkout the profile name specified by the user, and set it as the default profile.
 # If the profile name is not found in the index file, print an error message and exit
@@ -55,15 +58,14 @@
     else:
         config_manager.set_active_profile(profile_name)
         click.echo(f'Profile "{profile_name}" is now active')
 
 
 # Create a new profile, the profile name is specified by the user
 # If the profile name is already in the index file, print an error message and exit
-# Solution
 @click.argument("profile_name", required=True)
 @click.option("--base", "-b", help="Base profile name")
 @config.command(help="Create a new profile")
 def create(profile_name, base):
     config_manager = ConfigManager(INDEX_FILE_PATH)
     if config_manager.has_profile(profile_name=profile_name):
         click.echo(f"Profile {profile_name} already exists")
@@ -75,54 +77,65 @@
 # Delete the profile specified by the user, if the profile is the default profile, print an error
 # message and exit. If the profile is not found in the index file, print an error message and exit.
 # Solution
 @click.argument("profile_name", required=True)
 @config.command(name="del", help="Delete a profile")
 def delete(profile_name):
     config_manager = ConfigManager(INDEX_FILE_PATH)
+    # Check if the profile exists
     if not config_manager.has_profile(profile_name=profile_name):
         click.echo(f"Profile {profile_name} does not exist")
         return
+    # Check if the profile is active
     if config_manager.is_active_profile(profile_name):
         click.echo(
             f"Profile {profile_name} is active, only non-active profiles can be deleted"
         )
         return
+    # Delete the profile
     config_manager.delete_profile(profile_name)
     click.echo(f"Profile {profile_name} deleted")
 
 
 # Rename profile
 @config.command(help="Rename a profile")
 @click.argument("old_profile_name", required=True)
 @click.argument("new_profile_name", required=True)
 def rename(old_profile_name, new_profile_name):
+    # Define a ConfigManager object for the index file
     config_manager = ConfigManager(INDEX_FILE_PATH)
+    # If the old profile doesn't exist, print an error message
     if not config_manager.has_profile(profile_name=old_profile_name):
         click.echo(f"Profile {old_profile_name} does not exist")
         return
+    # If the new profile already exists, print an error message
     if config_manager.has_profile(profile_name=new_profile_name):
         click.echo(f"Profile {new_profile_name} already exists")
         return
+    # Rename the profile
     config_manager.rename_profile(old_profile_name, new_profile_name)
+    # Print a message confirming the rename
     click.echo(f"Profile {old_profile_name} renamed to {new_profile_name}")
 
 
 # Reinitialize the api section of the config file. The argument is the hocon formatted
 # string that will be used to replace the api section of the config file.
 @click.argument("base_profile", required=True)
 @config.command(help="Reinitialize the api section of the config file")
 def reinit(base_profile):
+    # Get the configuration from the user.
     click.echo("Please paste your multi-line configuration and press Enter:")
     config = read_multiline()
 
+    # Reinitialize the api section of the config file.
     config_manager = ConfigManager(INDEX_FILE_PATH)
     config_manager.reinitialize_api_config(base_profile, config)
 
 
+# Reads multiple lines of input from the user and returns them as a string.
 def read_multiline():
     lines = []
     while True:
         try:
             line = input()
             if not line:
                 break
```

### Comparing `clenv-0.0.4/clenv/cli/user/user_subcommand.py` & `clenv-0.0.6/clenv/cli/user/user_subcommand.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import click
 
 # Import generate_password from user.user_manager
 import bcrypt
 import os, re
 import json
+import base64
 from pyhocon import ConfigFactory, HOCONConverter
 
 
-@click.group(help="user management")
+@click.group(help="Privately hosted clearml server user helper tools")
 def user():
     pass
 
 
 # Write a command to generate a user config file ending with .conf in hocon format
 # The command should take a username and a password as arguments,
 # Encrypt the password using UserManager.generate_password() and write the username and encrypted password to the config file
 # The config file should be named after the username and saved to home directory
-# Solution
 @user.command(help="Generate a user password")
 @click.argument("username", required=True)
 @click.argument("password", required=False)
 def genpass(username, password):
     try:
         if password is None:
             password = click.prompt("Create a password for the user", hide_input=True)
         cipher_pw = generate_password(password)
 
-        config_dict = {"user": {"username": username, "password": cipher_pw.decode()}}
+        config_dict = {
+            "username": username,
+            "password": base64.b64encode(cipher_pw).decode("utf-8"),
+        }
         config = ConfigFactory.from_dict(config_dict)
         # Save the clearml-user.conf file in the home directory
         path = os.path.expanduser(f"~/clearml-server-{username}.conf")
         with open(path, "w") as f:
             f.write(HOCONConverter.to_hocon(config))
+
         click.echo(json.dumps(config_dict, indent=4))
         # Print the file path in green color
         click.echo(
             click.style(
                 f"User name and cipher password config saved to {path}, please send the config file to server admin",
                 fg="green",
             )
```

### Comparing `clenv-0.0.4/clenv.egg-info/PKG-INFO` & `clenv-0.0.6/clenv.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clenv
-Version: 0.0.4
+Version: 0.0.6
 Summary: ClearML config profile manager
 Home-page: https://github.com/DavidSonoda/clenv
 Author: Juewei Dong
 Author-email: juewei.dong@brainco.tech
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# clenv - Clearml environment profile manager
+# clenv - Unofficial ClearML CLI helper
 
 
 
 ## Pre-requisites
 
 - `clearml` installed, please refer to [ClearML installation guide](https://clear.ml/docs/latest/docs/getting_started/ds/ds_first_steps) for more details.
 - Run `clearml-init` and initialize your first ever config file.
@@ -32,15 +32,14 @@
 ## Installation
 
 ```bash
 pip install clenv
 ```
 
 
-
 ## Usage
 
 ### Subcommand `config`
 Note: All config files must be in the format of `clearml-<profile_name>.conf`
 
 #### List all config profiles
 ```bash
@@ -72,47 +71,80 @@
 ### Subcommand `user`
 
 #### Generate user/password hocon config
 ```bash
 clenv user genpass <user_name>
 ```
 
+### Subcommand `task`
+
+> Note: This command only support git repos for now. The project name of the task created on the ClearML server will be the same as the git repo name. So please make sure you have a meaningful, easy to read git repo name.
+
+#### Execute a task remotely on ClearML server
+
+```bash
+clenv task exec
+```
+
+It will prompt you to select an available queue, correct task type, your entrypoint script path and input the task name.
+
+![clenv-task-exec-1](./static/clenv-task-exec-1.png)
+
+After inputting all the required configs, it will ask you whether to save the configs. By typing 'y', the config will be saved. When you execute `clenv task exec` next time in the same repo, it will load the saved configs and skip the config input process. However, it will still ask you for confirmation before submitting the task.
+
+#### Ignore the saved run configs when starting a new execution
+
+If you want to ignore the old run configs and freshly start a new execution, you can run:
+
+```bash
+clenv task exec -N
+```
+
+The `-N` option will tell `clenv` to ignore the config file you have, and prompt you to input all the configs again.
 
+An alternative way of doing that is to delete the config file manually, which is located at `./.clenv/task_template.json`. Then running `clenv task exec` again will start a fresh execution as well.
 
 ## Examples
 
 ### Create a new clearml config profile for privately hosted clearml server 
 
 #### Initialize profiles
 
 ```bash
-$ ./clearenvoy.bin config list
+$ clenv config list
 # Input a name for your current profile
 ```
 
 #### Create a new profile
 
 ```bash
-$ ./clearenvoy.bin config create brainco
+$ clenv config create brainco
 ```
 
 #### Reinit the profile credentials
 
 ```bash
-$ ./clearenvoy.bin config reinit brainco
+$ clenv config reinit brainco
 ```
 
 #### Checkout the new profile
 
 ```bash
-$ ./clearenvoy.bin config checkout brainco
+$ clenv config checkout brainco
 ```
 
 ## Roadmap
-- [x] Config profile management
-- [x] BCrypt password generation
-- [ ] Support custom config file path
-- [ ] Server side utils and config management
-- [ ] ClearML Agent side utils and config management
+- Config management
+  - [x] Config profile management
+  - [ ] Support custom config file path
+- Privately hosted server management
+  - [x] BCrypt password generation (Feature to be deprecated when more sophisticated user management is implemented)
+  - [ ] Server side utils and config management
+  - [ ] ClearML Agent side utils and config management
+- Remote task management
+  - [x] A user friendly remote task execution wizard
+
+
+
 
 ## Disclaimer & License
 This project is not affiliated with Allegro AI, Inc. in any way. It is an independent and unofficial software. It's licensed under the MIT license.
```

