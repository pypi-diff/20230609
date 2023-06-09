# Comparing `tmp/ufbt-0.2.3rc0.tar.gz` & `tmp/ufbt-0.2.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.3rc0.tar", last modified: Thu Jun  8 21:16:01 2023, max compression
+gzip compressed data, was "ufbt-0.2.4rc0.tar", last modified: Fri Jun  9 15:42:29 2023, max compression
```

## Comparing `ufbt-0.2.3rc0.tar` & `ufbt-0.2.4rc0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:16:01.197437 ufbt-0.2.3rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-08 21:15:44.000000 ufbt-0.2.3rc0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-08 21:16:01.197437 ufbt-0.2.3rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-08 21:15:44.000000 ufbt-0.2.3rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-08 21:15:44.000000 ufbt-0.2.3rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 21:16:01.197437 ufbt-0.2.3rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:16:01.197437 ufbt-0.2.3rc0/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-08 21:15:44.000000 ufbt-0.2.3rc0/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-08 21:15:44.000000 ufbt-0.2.3rc0/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26452 2023-06-08 21:15:44.000000 ufbt-0.2.3rc0/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:16:01.197437 ufbt-0.2.3rc0/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-08 21:16:01.000000 ufbt-0.2.3rc0/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 21:16:01.000000 ufbt-0.2.3rc0/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 21:16:01.000000 ufbt-0.2.3rc0/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 21:16:01.000000 ufbt-0.2.3rc0/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 21:16:01.000000 ufbt-0.2.3rc0/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26503 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.3rc0/LICENSE.md` & `ufbt-0.2.4rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.3rc0/PKG-INFO` & `ufbt-0.2.4rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.3rc0
+Version: 0.2.4rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

### Comparing `ufbt-0.2.3rc0/README.md` & `ufbt-0.2.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.3rc0/pyproject.toml` & `ufbt-0.2.4rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.3rc0/ufbt/__init__.py` & `ufbt-0.2.4rc0/ufbt/__init__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.3rc0/ufbt/__main__.py` & `ufbt-0.2.4rc0/ufbt/__main__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.3rc0/ufbt/bootstrap.py` & `ufbt-0.2.4rc0/ufbt/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
     """
 
     hw_target: str = None
     force: bool = False
     mode: str = None
     all_params: Dict[str, str] = field(default_factory=dict)
 
-    DEFAULT_HW_TARGET: ClassVar[str] = ""
+    DEFAULT_HW_TARGET: ClassVar[str] = "f7"
 
     def update_from(self, other: "SdkDeployTask") -> None:
         log.debug(f"deploy task update from {other=}")
         if other.hw_target:
             self.hw_target = other.hw_target
 
         if other.mode:
@@ -450,15 +450,15 @@
         task.mode = "channel"
         task.all_params["channel"] = UpdateChannelSdkLoader.UpdateChannel.RELEASE.value
         return task
 
     @staticmethod
     def from_args(args: argparse.Namespace) -> "SdkDeployTask":
         task = SdkDeployTask()
-        task.hw_target = args.hw_target or SdkDeployTask.DEFAULT_HW_TARGET
+        task.hw_target = args.hw_target
         task.force = args.force
         for loader_cls in all_boostrap_loader_cls:
             task.all_params.update(loader_cls.args_namespace_to_metadata(args))
             if getattr(args, loader_cls.LOADER_MODE_KEY):
                 task.mode = loader_cls.LOADER_MODE_KEY
                 break
         log.debug(f"deploy task from args: {task=}")
@@ -603,15 +603,15 @@
         if previous_task := sdk_deployer.get_previous_task():
             previous_task.update_from(current_task)
             task_to_deploy = previous_task
         else:
             if current_task.mode:
                 task_to_deploy = current_task
             else:
-                log.error("No previous SDK state was found, fetching latest release")
+                log.warn("No previous SDK state was found, fetching latest release")
                 task_to_deploy = SdkDeployTask.default()
 
         if not sdk_deployer.deploy(task_to_deploy):
             return 1
         return 0
 
 
@@ -633,14 +633,15 @@
             help="Purge whole ufbt state",
             action="store_true",
             default=False,
         )
 
     def _func(self, args) -> int:
         sdk_deployer = UfbtSdkDeployer(args.ufbt_home)
+        log.info("If you want to clean build artifacts, use 'ufbt -c', not 'clean'")
         if args.purge:
             log.info(f"Cleaning complete ufbt state in {sdk_deployer.ufbt_state_dir}")
             shutil.rmtree(sdk_deployer.ufbt_state_dir, ignore_errors=True)
             log.info("Done")
             return
 
         if args.downloads:
```

### Comparing `ufbt-0.2.3rc0/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.4rc0/ufbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.3rc0
+Version: 0.2.4rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

