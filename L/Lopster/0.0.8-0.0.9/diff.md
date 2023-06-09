# Comparing `tmp/Lopster-0.0.8.tar.gz` & `tmp/Lopster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.0.8.tar", last modified: Fri Jun  9 16:38:02 2023, max compression
+gzip compressed data, was "Lopster-0.0.9.tar", last modified: Fri Jun  9 17:23:16 2023, max compression
```

## Comparing `Lopster-0.0.8.tar` & `Lopster-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 16:38:02.545329 Lopster-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-06-09 16:38:02.514085 Lopster-0.0.8/Lopster/
--rw-rw-rw-   0        0        0     7996 2023-06-09 16:37:40.000000 Lopster-0.0.8/Lopster/Lopster.py
--rw-rw-rw-   0        0        0     7920 2023-06-09 16:29:07.000000 Lopster-0.0.8/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 16:38:02.545329 Lopster-0.0.8/Lopster.egg-info/
--rw-rw-rw-   0        0        0      235 2023-06-09 16:38:02.000000 Lopster-0.0.8/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-09 16:38:02.000000 Lopster-0.0.8/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 16:38:02.000000 Lopster-0.0.8/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 16:38:02.000000 Lopster-0.0.8/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 16:38:02.000000 Lopster-0.0.8/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-06-09 16:38:02.545329 Lopster-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-09 16:38:02.545329 Lopster-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-06-09 16:37:58.000000 Lopster-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:23:16.052857 Lopster-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-09 17:23:16.016335 Lopster-0.0.9/Lopster/
+-rw-rw-rw-   0        0        0     7795 2023-06-09 17:22:44.000000 Lopster-0.0.9/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:23:16.048856 Lopster-0.0.9/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-06-09 17:23:15.000000 Lopster-0.0.9/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-09 17:23:15.000000 Lopster-0.0.9/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 17:23:15.000000 Lopster-0.0.9/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 17:23:15.000000 Lopster-0.0.9/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 17:23:15.000000 Lopster-0.0.9/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-06-09 17:23:16.050856 Lopster-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-09 17:23:16.052857 Lopster-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-06-09 17:23:11.000000 Lopster-0.0.9/setup.py
```

### Comparing `Lopster-0.0.8/Lopster/Lopster.py` & `Lopster-0.0.9/Lopster/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 import inspect
 import pygame
 import pygame.font
 
+
 class Enemy:
     _object = []
     typ = "Enemy"
 
     def __init__(self, _x, _y, _h, _w, _update):
         self._object.append(self)
         self.x = _x
@@ -29,28 +30,29 @@
         text = []
 
         text.append("Enemy\n")
         text.append("x = " + self.x + "\n")
         text.append("y = " + self.y + "\n")
         text.append("h = " + self.h + "\n")
         text.append("w = " + self.w + "\n")
-        text.append("func update = " + inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
+        text.append("func update = " +
+                    inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
         text.append("init @x @y @h @w @update\n")
         text.append(";")
 
         return "".join(text)
 
 
 class FakeEnemy:
     typ = "Enemy"
     x = 0
     y = 0
     h = 0
     w = 0
-    update = lambda: print()
+    def update(): return print()
 
     def __init__(self, _x, _y, _h, _w, _update):
         self.x = _x
         self.y = _y
         self.h = _h
         self.w = _w
         self.update = _update
@@ -65,15 +67,16 @@
         text = []
 
         text.append("FakeEnemy\n")
         text.append("x = " + self.x + "\n")
         text.append("y = " + self.y + "\n")
         text.append("h = " + self.h + "\n")
         text.append("w = " + self.w + "\n")
-        text.append("func update = " + inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
+        text.append("func update = " +
+                    inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
         text.append("init @x @y @h @w @update\n")
         text.append(";")
 
         return "".join(text)
 
 
 class Player(Enemy):
@@ -113,41 +116,35 @@
 
         text.append("Player\n")
         text.append("x = " + str(self.x) + "\n")
         text.append("y = " + str(self.y) + "\n")
         text.append("h = " + str(self.h) + "\n")
         text.append("w = " + str(self.w) + "\n")
         text.append("speed = " + str(self.speed) + "\n")
-        text.append("func update = " + inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
+        text.append("func update = " +
+                    inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
         text.append("init @x @y @h @w @speed @update\n")
         text.append(";")
 
         return "".join(text)
 
+
 class Text(Enemy):
-    def __init__(self, x, y, text, font_name, font_size, color, _x, _y, _h, _w, _update):
+    def __init__(self, _x, _y, _h, _w, _update):
         super().__init__(_x, _y, _h, _w, _update)
-        self.x = x
-        self.y = y
-        self.text = text
-        self.font = pygame.font.Font(font_name, font_size)
-        self.color = color
-
-    def set_text(self, text):
-        self.text = text
-
-    def set_font(self, font_name, font_size):
-        self.font = pygame.font.Font(font_name, font_size)
-
-    def set_color(self, color):
-        self.color = color
-
-    def draw(self, window):
-        text_surface = self.font.render(self.text, True, self.color)
-        window.blit(text_surface, (self.x, self.y))
+
+    def draw(self, window, fontName, fontSize, text, color):
+        font = pygame.font.Font(fontName, fontSize)
+        _text = font.render(text, True, color)
+        text_rect = _text.get_rect()
+        text_rect.x = self.x
+        text_rect.y = self.y
+        window.blit(_text, text_rect)
+
+
 
 class MathMap:
     h = 0
     w = 0
 
     def __init__(self, height, width):
         self._h = height
@@ -281,8 +278,8 @@
                     obj.update(window, obj)
 
             pygame.display.update()
 
         pygame.quit()
 
 
-__all__ = ['Enemy', 'FakeEnemy', 'Player', 'MathMap', 'Map', 'RunLopster']
+__all__ = ['Enemy', 'FakeEnemy', 'Player', 'MathMap', 'Map', 'RunLopster']
```

