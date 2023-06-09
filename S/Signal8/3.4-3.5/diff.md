# Comparing `tmp/Signal8-3.4.tar.gz` & `tmp/Signal8-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-3.4.tar", last modified: Fri Jun  9 16:58:06 2023, max compression
+gzip compressed data, was "Signal8-3.5.tar", last modified: Fri Jun  9 17:03:05 2023, max compression
```

## Comparing `Signal8-3.4.tar` & `Signal8-3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 16:58:06.890635 Signal8-3.4/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.4/LICENSE
--rw-rw-rw-   0        0        0     5556 2023-06-09 16:58:06.887635 Signal8-3.4/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 16:58:06.792201 Signal8-3.4/Signal8/
--rw-rw-rw-   0        0        0    11061 2023-06-09 16:56:47.000000 Signal8-3.4/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-3.4/Signal8/__init__.py
--rw-rw-rw-   0        0        0      268 2023-06-09 16:49:06.000000 Signal8-3.4/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 16:58:06.881635 Signal8-3.4/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.4/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     6036 2023-06-09 16:47:11.000000 Signal8-3.4/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2826 2023-06-09 16:43:50.000000 Signal8-3.4/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-3.4/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.4/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-3.4/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.4/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-09 16:58:06.826197 Signal8-3.4/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5556 2023-06-09 16:58:06.000000 Signal8-3.4/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-09 16:58:06.000000 Signal8-3.4/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 16:58:06.000000 Signal8-3.4/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 16:58:06.000000 Signal8-3.4/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 16:58:06.891633 Signal8-3.4/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-09 16:57:19.000000 Signal8-3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:03:05.162217 Signal8-3.5/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.5/LICENSE
+-rw-rw-rw-   0        0        0     5556 2023-06-09 17:03:05.160218 Signal8-3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 17:03:05.091228 Signal8-3.5/Signal8/
+-rw-rw-rw-   0        0        0    11063 2023-06-09 17:02:14.000000 Signal8-3.5/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-3.5/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-06-09 16:49:06.000000 Signal8-3.5/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:03:05.155218 Signal8-3.5/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.5/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     6036 2023-06-09 16:47:11.000000 Signal8-3.5/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2826 2023-06-09 16:43:50.000000 Signal8-3.5/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-3.5/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.5/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-3.5/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.5/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:03:05.135219 Signal8-3.5/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5556 2023-06-09 17:03:04.000000 Signal8-3.5/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-09 17:03:04.000000 Signal8-3.5/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 17:03:04.000000 Signal8-3.5/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 17:03:04.000000 Signal8-3.5/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 17:03:05.162217 Signal8-3.5/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-09 17:02:41.000000 Signal8-3.5/setup.py
```

### Comparing `Signal8-3.4/LICENSE` & `Signal8-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-3.4/PKG-INFO` & `Signal8-3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.4
+Version: 3.5
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-3.4/README.md` & `Signal8-3.5/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-3.4/Signal8/Signal8.py` & `Signal8-3.5/Signal8/Signal8.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             observed_goal = relative_goal_pos
         
         return np.concatenate((agent_pos, agent_vel, np.concatenate(observed_obstacles, axis=0), observed_goal))
             
     # Run a thread for each scripted obstacle
     def run_scripted_obstacle(self, world, obstacle):
         while self.scripted_obstacle_running:
-            self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
+            # self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
             action, size = self._action_callback(obstacle, world)
             obstacle.update(action, size)
             time.sleep(0.5)
         
     # disaster response: increase obstacle size to resemble increasing size of fire
     # precision farming: move obstacle in a zig-zag pattern to resemble a tractor
     def _action_callback(self, obstacle, world):
```

### Comparing `Signal8-3.4/Signal8/utils/core.py` & `Signal8-3.5/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.4/Signal8/utils/npc.py` & `Signal8-3.5/Signal8/utils/npc.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.4/Signal8/utils/problems.py` & `Signal8-3.5/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.4/Signal8/utils/simple_env.py` & `Signal8-3.5/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.4/Signal8/utils/test_dynamic_obs.py` & `Signal8-3.5/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.4/Signal8.egg-info/PKG-INFO` & `Signal8-3.5/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.4
+Version: 3.5
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-3.4/Signal8.egg-info/SOURCES.txt` & `Signal8-3.5/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-3.4/setup.py` & `Signal8-3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="3.4",
+    version="3.5",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

