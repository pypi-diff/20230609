# Comparing `tmp/Signal8-3.3.tar.gz` & `tmp/Signal8-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-3.3.tar", last modified: Thu Jun  8 18:55:07 2023, max compression
+gzip compressed data, was "Signal8-3.4.tar", last modified: Fri Jun  9 16:58:06 2023, max compression
```

## Comparing `Signal8-3.3.tar` & `Signal8-3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 18:55:07.207450 Signal8-3.3/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.3/LICENSE
--rw-rw-rw-   0        0        0     5556 2023-06-08 18:55:07.193449 Signal8-3.3/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 18:55:07.128451 Signal8-3.3/Signal8/
--rw-rw-rw-   0        0        0    11051 2023-06-08 18:54:13.000000 Signal8-3.3/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-3.3/Signal8/__init__.py
--rw-rw-rw-   0        0        0     1989 2023-06-08 18:53:56.000000 Signal8-3.3/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-08 18:55:07.167451 Signal8-3.3/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.3/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5809 2023-06-06 17:48:52.000000 Signal8-3.3/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2783 2023-06-08 18:19:36.000000 Signal8-3.3/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-3.3/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.3/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-3.3/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.3/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-08 18:55:07.152452 Signal8-3.3/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5556 2023-06-08 18:55:06.000000 Signal8-3.3/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-08 18:55:06.000000 Signal8-3.3/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 18:55:06.000000 Signal8-3.3/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-08 18:55:06.000000 Signal8-3.3/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 18:55:07.208450 Signal8-3.3/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-08 18:54:23.000000 Signal8-3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:58:06.890635 Signal8-3.4/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.4/LICENSE
+-rw-rw-rw-   0        0        0     5556 2023-06-09 16:58:06.887635 Signal8-3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 16:58:06.792201 Signal8-3.4/Signal8/
+-rw-rw-rw-   0        0        0    11061 2023-06-09 16:56:47.000000 Signal8-3.4/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-3.4/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-06-09 16:49:06.000000 Signal8-3.4/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:58:06.881635 Signal8-3.4/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.4/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     6036 2023-06-09 16:47:11.000000 Signal8-3.4/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2826 2023-06-09 16:43:50.000000 Signal8-3.4/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-3.4/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.4/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-3.4/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.4/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:58:06.826197 Signal8-3.4/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5556 2023-06-09 16:58:06.000000 Signal8-3.4/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-09 16:58:06.000000 Signal8-3.4/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 16:58:06.000000 Signal8-3.4/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 16:58:06.000000 Signal8-3.4/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 16:58:06.891633 Signal8-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-09 16:57:19.000000 Signal8-3.4/setup.py
```

### Comparing `Signal8-3.3/LICENSE` & `Signal8-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-3.3/PKG-INFO` & `Signal8-3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.3
+Version: 3.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-3.3/README.md` & `Signal8-3.4/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-3.3/Signal8/Signal8.py` & `Signal8-3.4/Signal8/Signal8.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,43 +193,44 @@
         if goal_dist <= max_observable_dist:
             observed_goal = relative_goal_pos
         
         return np.concatenate((agent_pos, agent_vel, np.concatenate(observed_obstacles, axis=0), observed_goal))
             
     # Run a thread for each scripted obstacle
     def run_scripted_obstacle(self, world, obstacle):
-        sensitivity = 2.0
         while self.scripted_obstacle_running:
-            with obstacle.lock:
-                # self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
-                action = self._action_callback(obstacle, world)
-                obstacle.action = action * sensitivity
-                obstacle.move()
-                time.sleep(0.25)
+            self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
+            action, size = self._action_callback(obstacle, world)
+            obstacle.update(action, size)
+            time.sleep(0.5)
         
     # disaster response: increase obstacle size to resemble increasing size of fire
     # precision farming: move obstacle in a zig-zag pattern to resemble a tractor
-    def _action_callback(self, obs, world):
-        action = np.zeros(world.dim_p)
+    def _action_callback(self, obstacle, world):
+        size = None
+        action = None
         instance = world.problem_instance
         if world.problem_type == 'disaster_response':
             if instance == 'instance_0':
-                obs.size += 0.005
+                size = 0.005
             elif instance == 'instance_1':
-                obs.size += 0.0075
+                size = 0.0075
             elif instance == 'instance_2':
-                obs.size += 0.01
+                size = 0.01
             elif instance == 'instance_3':
-                obs.size += 0.0125
+                size = 0.0125
         else:
-            obs_num = int(obs.name.split('_')[-1])
+            action = np.zeros(world.dim_p)
+            obstacle_num = int(obstacle.name.split('_')[-1])
             instance_num = int(instance.split('_')[-1])
-            action = self.npc[obs_num].get_scripted_action(obs, instance_num)
+            action = self.npc[obstacle_num].get_scripted_action(obstacle, instance_num)
+            sensitivity = 2.0
+            action *= sensitivity
 
-        return action
+        return action, size
 
     # Stop all threads for scripted obstacles
     def stop_scripted_obstacles(self):
         self.scripted_obstacle_running = False
         for t in self.scripted_obstacle_threads:
             t.join()
         self.scripted_obstacle_threads.clear()
```

### Comparing `Signal8-3.3/Signal8/main.py` & `Signal8-3.4/Signal8/utils/test_dynamic_obs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,28 @@
-# import Signal8
-# import time
-
-# env = Signal8.env('disaster_response')
-# env.reset(options={"instance_num": 0})
-# observation, _, terminations, truncations, _ = env.last()
-# entities = env.unwrapped.get_start_state()
-# time.sleep(1)
-# time.sleep(1)
-# env.step(1)
-# env.close()
-
 import pygame
 import numpy as np
 from utils.npc import NPC
 
 pygame.init()
 scale_factor = 400
 window_size = (800, 800)
 window = pygame.display.set_mode(window_size)
 
 start = (0.9, 0.9)
 npc = NPC(start)
 scenario_num = 0
 
-
 class State:
     def __init__(self, start):
         self.p_pos = np.array(start)
 
-
 class Obs:
     def __init__(self, start):
         self.state = State(start)
 
-
 obs = Obs(start)
 
 running = True
 while running:
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
             running = False
@@ -46,27 +31,24 @@
     # Adjust this value to change the speed of the NPC
     obs.state.p_pos += action * 0.005
 
     # Draw the NPC
     window.fill((0, 0, 0))  # Clear the window
 
     # Draw the start point as a blue circle
-    x_start, y_start = np.array(
-        start) * scale_factor + np.array(window_size) / 2
+    x_start, y_start = np.array(start) * scale_factor + np.array(window_size) / 2
     pygame.draw.circle(window, (0, 0, 255), (int(x_start), int(y_start)), 10)
 
     # Draw the destination as a red rectangle
     bounds = npc.farming_instances[scenario_num]['bounds']
-    x_bounds, y_bounds = np.array(
-        bounds) * scale_factor + np.array(window_size) / 2
+    x_bounds, y_bounds = np.array(bounds) * scale_factor + np.array(window_size) / 2
     width = x_bounds[1] - x_bounds[0]
     height = y_bounds[1] - y_bounds[0]
-    pygame.draw.rect(window, (255, 0, 0), pygame.Rect(
-        x_bounds[0], y_bounds[0], width, height))
+    pygame.draw.rect(window, (255, 0, 0), pygame.Rect(x_bounds[0], y_bounds[0], width, height))
 
     # Convert NPC coordinates to Pygame coordinates
     x, y = obs.state.p_pos * scale_factor + np.array(window_size) / 2
     # Draw the NPC as a white circle
     pygame.draw.circle(window, (255, 255, 255), (int(x), int(y)), 10)
     pygame.display.flip()  # Update the window
 
-pygame.quit()
+pygame.quit()
```

### Comparing `Signal8-3.3/Signal8/utils/core.py` & `Signal8-3.4/Signal8/utils/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,25 +42,29 @@
 
 
 class Obstacle(Entity):  # properties of obstacles entities
     def __init__(self):
         super().__init__()
         # entity can be moved / pushed
         self.movable = False
-        # action
-        self.action = None
         # script behavior to execute
         self.action_callback = None
         self.lock = None
     
     # updates the state of the obstacle
-    def move(self, dt=0.1, damping=0.25):
-        self.state.p_vel = self.state.p_vel * (1 - damping)
-        self.state.p_vel += (self.action / self.mass) * dt
-        self.state.p_pos += self.state.p_vel * dt
+    def update(self, action=None, size=None, dt=0.1, damping=0.25):
+        with self.lock:
+            if action is not None:
+                self.state.p_vel = self.state.p_vel * (1 - damping)
+                self.state.p_vel += (action / self.mass) * dt
+                self.state.p_pos += self.state.p_vel * dt
+            elif size is not None:
+                self.size += size
+            else:
+                raise ValueError("Either action or size must be specified")
         
 
 class Agent(Entity):  # properties of agent entities
     def __init__(self):
         super().__init__()
         # agents are movable by default
         self.movable = True
```

### Comparing `Signal8-3.3/Signal8/utils/npc.py` & `Signal8-3.4/Signal8/utils/npc.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,22 @@
         self.farming_instances = {
             0: {'destination': (-0.9, -0.9), 'direction': [-1, 1], 'bounds': [(-1, -0.4), (-1, 1)]},
             1: {'destination': (0.9, 0.9), 'direction': [-1, -1], 'bounds': [(-1, 1), (0.4, 1)]},
             2: {'destination': (0, 1), 'direction': [1, -1], 'bounds': [(-0.25, 0.25), (-1, 1)]},
             3: {'destination': (-0.75, -0.90), 'direction': [1, 1], 'bounds': [(-1, 1), (-1, -0.4)]},
         }
     
-    def get_scripted_action(self, obs, instance_num):
+    def get_scripted_action(self, obstacle, instance_num):
         destination = self.farming_instances[instance_num]['destination']
         direction = self.farming_instances[instance_num]['direction']
         bounds = self.farming_instances[instance_num]['bounds']
         
         action = np.array([0, 0])
-        x, y, = obs.state.p_pos
+        with obstacle.lock:
+            x, y, = obstacle.state.p_pos
         
         if self.status == 'moving_to_destination':
             if np.allclose([x, y], destination, atol=0.05):
                 self.status = 'zigzagging'
                 self.direction = direction
             else:
                 action = self._move_towards_point(x, y, destination)
```

### Comparing `Signal8-3.3/Signal8/utils/problems.py` & `Signal8-3.4/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.3/Signal8/utils/simple_env.py` & `Signal8-3.4/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.3/Signal8.egg-info/PKG-INFO` & `Signal8-3.4/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.3
+Version: 3.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-3.3/Signal8.egg-info/SOURCES.txt` & `Signal8-3.4/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-3.3/setup.py` & `Signal8-3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="3.3",
+    version="3.4",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

