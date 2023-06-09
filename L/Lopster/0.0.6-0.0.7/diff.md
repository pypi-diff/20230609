# Comparing `tmp/Lopster-0.0.6.tar.gz` & `tmp/Lopster-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.0.6.tar", last modified: Fri Jun  9 15:58:31 2023, max compression
+gzip compressed data, was "Lopster-0.0.7.tar", last modified: Fri Jun  9 16:29:42 2023, max compression
```

## Comparing `Lopster-0.0.6.tar` & `Lopster-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:58:31.823288 Lopster-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-06-09 15:58:31.792029 Lopster-0.0.6/Lopster/
--rw-rw-rw-   0        0        0     7201 2023-06-09 15:29:02.000000 Lopster-0.0.6/Lopster/Lopster.py
--rw-rw-rw-   0        0        0     7350 2023-06-09 15:58:27.000000 Lopster-0.0.6/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:58:31.823288 Lopster-0.0.6/Lopster.egg-info/
--rw-rw-rw-   0        0        0      235 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-06-09 15:58:31.823288 Lopster-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-09 15:58:31.823288 Lopster-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-06-09 15:58:27.000000 Lopster-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:29:42.371939 Lopster-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-09 16:29:42.340600 Lopster-0.0.7/Lopster/
+-rw-rw-rw-   0        0        0     7920 2023-06-09 16:29:33.000000 Lopster-0.0.7/Lopster/Lopster.py
+-rw-rw-rw-   0        0        0     7920 2023-06-09 16:29:07.000000 Lopster-0.0.7/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:29:42.371939 Lopster-0.0.7/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-06-09 16:29:42.000000 Lopster-0.0.7/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-09 16:29:42.000000 Lopster-0.0.7/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 16:29:42.000000 Lopster-0.0.7/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 16:29:42.000000 Lopster-0.0.7/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 16:29:42.000000 Lopster-0.0.7/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-06-09 16:29:42.371939 Lopster-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-09 16:29:42.371939 Lopster-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-06-09 16:12:56.000000 Lopster-0.0.7/setup.py
```

### Comparing `Lopster-0.0.6/Lopster/Lopster.py` & `Lopster-0.0.7/Lopster/Lopster.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import inspect
 import pygame
-
+import pygame.font
 
 class Enemy:
     _object = []
     typ = "Enemy"
 
     def __init__(self, _x, _y, _h, _w, _update):
         self._object.append(self)
@@ -25,24 +25,25 @@
     def visible(self, typ):
         self.typ = typ
 
     def cash(self):
         text = []
 
         text.append("Enemy\n")
-        text.append("x = "+self.x+"\n")
-        text.append("y = "+self.y+"\n")
-        text.append("h = "+self.h+"\n")
-        text.append("w = "+self.w+"\n")
-        text.append("func update = "+inspect.getsource(self.update).replace("\n", "/../+o+/../")+"\n")
+        text.append("x = " + self.x + "\n")
+        text.append("y = " + self.y + "\n")
+        text.append("h = " + self.h + "\n")
+        text.append("w = " + self.w + "\n")
+        text.append("func update = " + inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
         text.append("init @x @y @h @w @update\n")
         text.append(";")
 
         return "".join(text)
 
+
 class FakeEnemy:
     typ = "Enemy"
     x = 0
     y = 0
     h = 0
     w = 0
     update = lambda: print()
@@ -60,19 +61,19 @@
     def visible(self, typ):
         self.typ = typ
 
     def cash(self):
         text = []
 
         text.append("FakeEnemy\n")
-        text.append("x = "+self.x+"\n")
-        text.append("y = "+self.y+"\n")
-        text.append("h = "+self.h+"\n")
-        text.append("w = "+self.w+"\n")
-        text.append("func update = "+inspect.getsource(self.update).replace("\n", "/../+o+/../")+"\n")
+        text.append("x = " + self.x + "\n")
+        text.append("y = " + self.y + "\n")
+        text.append("h = " + self.h + "\n")
+        text.append("w = " + self.w + "\n")
+        text.append("func update = " + inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
         text.append("init @x @y @h @w @update\n")
         text.append(";")
 
         return "".join(text)
 
 
 class Player(Enemy):
@@ -96,48 +97,69 @@
             obj.y += speed
 
     def addMoveWithBorder(self, up, down, left, right, obj, w, h):
         speed = self.speed
         keys = pygame.key.get_pressed()
         if keys[left] and obj.x >= self.w:
             obj.x -= speed
-        if keys[right] and obj.x <= w-self.w:
+        if keys[right] and obj.x <= w - self.w:
             obj.x += speed
         if keys[up] and obj.y >= self.h:
             obj.y -= speed
-        if keys[down] and obj.y <= h-self.h:
+        if keys[down] and obj.y <= h - self.h:
             obj.y += speed
 
     def cash(self):
         text = []
 
         text.append("Player\n")
-        text.append("x = "+str(self.x)+"\n")
-        text.append("y = "+str(self.y)+"\n")
-        text.append("h = "+str(self.h)+"\n")
-        text.append("w = "+str(self.w)+"\n")
-        text.append("speed = "+str(self.speed)+"\n")
-        text.append("func update = "+inspect.getsource(self.update).replace("\n", "/../+o+/../")+"\n")
+        text.append("x = " + str(self.x) + "\n")
+        text.append("y = " + str(self.y) + "\n")
+        text.append("h = " + str(self.h) + "\n")
+        text.append("w = " + str(self.w) + "\n")
+        text.append("speed = " + str(self.speed) + "\n")
+        text.append("func update = " + inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
         text.append("init @x @y @h @w @speed @update\n")
         text.append(";")
 
         return "".join(text)
 
+class Text(Enemy):
+    def __init__(self, x, y, text, font_name, font_size, color):
+        self.x = x
+        self.y = y
+        self.text = text
+        self.font = pygame.font.Font(font_name, font_size)
+        self.color = color
+
+    def set_text(self, text):
+        self.text = text
+
+    def set_font(self, font_name, font_size):
+        self.font = pygame.font.Font(font_name, font_size)
+
+    def set_color(self, color):
+        self.color = color
+
+    def draw(self, window):
+        text_surface = self.font.render(self.text, True, self.color)
+        window.blit(text_surface, (self.x, self.y))
+
 class MathMap:
     h = 0
     w = 0
 
     def __init__(self, height, width):
         self._h = height
         self._w = width
 
     def Distance(x, y, x1, y1):
         distance = math.sqrt((x1 - x) ** 2 + (y1 - y) ** 2)
         return distance
-    
+
     def Side(x, y, x1, y1):
         if x1 > x:
             return "right"
         elif x1 < x:
             return "left"
         elif y1 > y:
             return "bottom"
@@ -156,14 +178,15 @@
     def getTouch(self, obj):
         for obj2 in obj._object:
             if obj != obj2:
                 if obj.x < obj2.x + obj2.w and obj.x + obj.w > obj2.x and obj.y < obj2.y + obj2.h and obj.y + obj.h > obj2.y:
                     return obj2
         return None
 
+
 class Map:
     def __init__(self, window, drawingMap):
         self.map = drawingMap
         self.window = window
 
     def draw(self, map):
         drawMap = self.map
@@ -171,14 +194,15 @@
         for card in map:
             if not type(card) == "tuple":
                 drawMap[card](self.window, "NoN")
             else:
                 for subCard in card:
                     drawMap[subCard](self.window, card)
 
+
 # class Bank:
 #     def __init__(self, src):
 #         self.src = src
 #
 #     def cash(self):
 #         text = []
 #         for obj in Enemy._object:
@@ -214,14 +238,15 @@
 #                                 print("Unknown value '"+com+"' in cache '"+self.src+"'")
 #                     y += 1
 #                     print(var)
 #                 i += 1
 
 class RunLopster:
     _fps = 16
+
     def __init__(self, window_size, title, icon, update, fps):
         self._window_size = window_size
         self._title = title
         self._update = update
         self._fps = fps
         self._icon = icon
 
@@ -254,8 +279,9 @@
                 if obj.typ != "NoN":
                     obj.update(window, obj)
 
             pygame.display.update()
 
         pygame.quit()
 
+
 __all__ = ['Enemy', 'FakeEnemy', 'Player', 'MathMap', 'Map', 'RunLopster']
```

### Comparing `Lopster-0.0.6/Lopster/__init__.py` & `Lopster-0.0.7/Lopster/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from .Lopster import Enemy, FakeEnemy, Player, MathMap, Map, RunLopster
 import math
 import inspect
 import pygame
-
+import pygame.font
 
 class Enemy:
     _object = []
     typ = "Enemy"
 
     def __init__(self, _x, _y, _h, _w, _update):
         self._object.append(self)
@@ -120,14 +119,34 @@
         text.append("speed = " + str(self.speed) + "\n")
         text.append("func update = " + inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
         text.append("init @x @y @h @w @speed @update\n")
         text.append(";")
 
         return "".join(text)
 
+class Text(Enemy):
+    def __init__(self, x, y, text, font_name, font_size, color):
+        self.x = x
+        self.y = y
+        self.text = text
+        self.font = pygame.font.Font(font_name, font_size)
+        self.color = color
+
+    def set_text(self, text):
+        self.text = text
+
+    def set_font(self, font_name, font_size):
+        self.font = pygame.font.Font(font_name, font_size)
+
+    def set_color(self, color):
+        self.color = color
+
+    def draw(self, window):
+        text_surface = self.font.render(self.text, True, self.color)
+        window.blit(text_surface, (self.x, self.y))
 
 class MathMap:
     h = 0
     w = 0
 
     def __init__(self, height, width):
         self._h = height
```

