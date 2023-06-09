# Comparing `tmp/edudraw-1.3.2.tar.gz` & `tmp/edudraw-1.4.0.tar.gz`

## Comparing `edudraw-1.3.2.tar` & `edudraw-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,8 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/.name
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/Edu-Draw-Python.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/misc.xml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/vcs.xml
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/workspace.xml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edudraw-1.3.2/src/EduDraw/__init__.py
--rw-r--r--   0        0        0    38253 2020-02-02 00:00:00.000000 edudraw-1.3.2/src/EduDraw/edudraw.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 edudraw-1.3.2/src/EduDraw/requirements.txt
--rw-r--r--   0        0        0    14696 2020-02-02 00:00:00.000000 edudraw-1.3.2/tests/edudraw_tests.py
--rw-r--r--   0        0        0    27030 2020-02-02 00:00:00.000000 edudraw-1.3.2/LICENSE
--rw-r--r--   0        0        0    32176 2020-02-02 00:00:00.000000 edudraw-1.3.2/README.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 edudraw-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    31647 2020-02-02 00:00:00.000000 edudraw-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edudraw-1.4.0/src/EduDraw/__init__.py
+-rw-r--r--   0        0        0    66011 2020-02-02 00:00:00.000000 edudraw-1.4.0/src/EduDraw/edudraw.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 edudraw-1.4.0/src/EduDraw/requirements.txt
+-rw-r--r--   0        0        0    17985 2020-02-02 00:00:00.000000 edudraw-1.4.0/tests/edudraw_tests.py
+-rw-r--r--   0        0        0    27030 2020-02-02 00:00:00.000000 edudraw-1.4.0/LICENSE
+-rw-r--r--   0        0        0    39773 2020-02-02 00:00:00.000000 edudraw-1.4.0/README.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 edudraw-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    38938 2020-02-02 00:00:00.000000 edudraw-1.4.0/PKG-INFO
```

### Comparing `edudraw-1.3.2/tests/edudraw_tests.py` & `edudraw-1.4.0/tests/edudraw_tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import gc
 
 import pygame.image
 
 from src.EduDraw import edudraw
 import time
 
-s = edudraw.EduDraw(500, 500)
+s = edudraw.EduDraw(500, 500, False)
 d = edudraw.EduDraw(250, 250, True)
 
 flag_done = False
 tests = []
 
 end = 0
 start = time.time()
 
 antialias = False
 
+# Note: This is just a test picture, nothing special
+img = pygame.image.load(r"Image\path\goes\here")
+
 def pressed(data):
     global antialias
     antialias = not antialias
 
 
 def setup():
+    # s.frame_rate(50)
+    s.deltatime = 0
     s.set_controls(key_down=pressed)
 
 flag_has_null = False
 
 def draw():
     global flag_done, start, end, flag_has_null
 
@@ -36,14 +41,15 @@
 
     if len(tests) == 0:
         # d.quit()
         if flag_done:
             s.quit()
             end = time.time()
             print(f"Test done: {str(test_null_mode)}, Elapsed time: {end - start}, Avg. FPS: {s.frame_count / (end - start)}")
+            print(f"Avg. fps for inner instance: {d.frame_count / (end - start)}")
             print("All tests done.")
             return
         else:
             if not flag_has_null:
                 start = time.time()
                 d.start(dummy, inner_drawing, "This should not appear")
                 flag_has_null = True
@@ -63,29 +69,31 @@
 
 def dummy():
     pass
 
 position = [d.width/2, d.height//2]
 velocity = [3, 4]
 def inner_drawing():
-    # d.background((200, 200, 200))
     global position, velocity
     if position[0] < 0 or position[0] > d.width:
         velocity[0] *= -1
 
     if position[1] < 0 or position[1] > d.height:
         velocity[1] *= -1
 
     position[0] += velocity[0]
     position[1] += velocity[1]
 
     d.fill((255, 0, 0))
     d.stroke((0, 0, 255))
     d.circle(position[0], position[1], 5)
 
+    d.rect_mode('CENTER')
+    d.image(img, d.width // 2, s.height // 2, d.width // 2, s.height // 2, True)
+
 
 def test_rect_mode():
     global flag_done
     s.background((200, 200, 200))
 
     s.no_fill()
 
@@ -676,16 +684,15 @@
     if s.frame_count > 40:
         flag_done = True
 
 
 tests.append(test_polygon)
 
 # Note: This is just a test picture, nothing special
-img = pygame.image.load(r"C:\Users\Murilo Luis\Desktop\logo.png")
-
+img = pygame.image.load(r"File\path\goes\here")
 
 def test_image():
     global flag_done
 
     s.scale(0.75, 1.25)
     s.background((200, 200, 200))
     s.image(img, 50, 50, 200, 200)
@@ -694,28 +701,156 @@
     s.translate(s.width // 2, s.height // 2)
     s.image(img, 0, 0, 200, 200, force_transparency=True)
 
     if s.frame_count > 60:
         flag_done = True
 
 
-
-
 tests.append(test_image)
 
 
 def test_null_mode():
     global flag_done
     s.background((255, 255, 255))
     s.rotate(s.frame_count)
     s.rect_mode("CENTER")
     s.translate(s.width // 2, s.height // 2)
-    s.image(d.screen, 0, 0)
+    s.image(d.retrieve_frame(), 0, 0)
+
+    if s.frame_count > 150:
+        flag_done = True
+
+
+control_points = [(100, 100), (150, 500), (450, 500), (500, 150)]
+
+
+def test_bezier():
+    global flag_done
+    s.background((255, 255, 255))
+    s.stroke((255, 0, 0))
+    s.stroke_weight(3)
+    s.bezier_curve(control_points, s.frame_count)
+
+    s.stroke((0, 0, 255))
+    s.fill((0, 0, 255))
+    for point in control_points:
+        s.circle(point[0], point[1], 5)
 
     if s.frame_count > 150:
         flag_done = True
 
 
-# tests.append(test_null_mode)
+tests.append(test_bezier)
+
+
+def test_pie():
+    global flag_done
+    # This is so trippy
+    s.background((200, 200, 200))
+    s.no_fill()
+    s.rotate(s.frame_count * 1.1)
+    s.scale(1.25, 0.75)
+    s.translate(s.width//2, s.height//2)
+    s.stroke((255, 255, 255))
+    s.stroke_weight(3)
+    s.fill((255, 0, 0))
+
+    s.stroke((0, 0, 255))
+    s.arc_pie(s.frame_count + 150, s.frame_count * 2, 0, 0, s.width//2, s.height//2)
+
+    if s.frame_count > 180:
+        flag_done = True
+
+
+tests.append(test_pie)
+
+
+def test_arc_closed():
+    global flag_done
+    s.background((200, 200, 200))
+    s.no_fill()
+    s.rotate(s.frame_count * 1.1)
+    s.scale(1.25, 0.75)
+    s.translate(s.width//2, s.height//2)
+    s.stroke((255, 255, 255))
+    s.stroke_weight(3)
+    s.fill((255, 0, 0))
+
+    s.stroke((0, 0, 255))
+    s.arc_closed(s.frame_count + 150, s.frame_count * 2, 0, 0, s.width//2, s.height//2)
+
+    if s.frame_count > 180:
+        flag_done = True
+
+
+tests.append(test_arc_closed)
+
+
+def test_arc_open():
+    global flag_done
+    s.background((200, 200, 200))
+    s.no_fill()
+    s.rotate(s.frame_count * 1.1)
+    s.scale(1.25, 0.75)
+    s.translate(s.width//2, s.height//2)
+    s.stroke((255, 255, 255))
+    s.stroke_weight(3)
+    s.fill((255, 0, 0))
+
+    s.stroke((0, 0, 255))
+    s.arc_open(s.frame_count + 150, s.frame_count * 2, 0, 0, s.width//2, s.height//2)
+
+    if s.frame_count > 180:
+        flag_done = True
+
+
+tests.append(test_arc_open)
+
+
+def test_erase():
+    global flag_done
+    s.background((200, 200, 200))
+    s.fill((255, 0, 0))
+    s.circle(s.width//2, s.height//2, s.width//2)
+    s.fill((0, 0, 255))
+    s.erase()
+    s.rect(0, s.height//3, s.width, s.height//3 + 40)
+    s.no_erase()
+    s.rect(s.width//3, 0, s.width//3 + 40, s.height)
+    s.erase()
+    s.translate(90, 90)
+    s.triangle(120, 120, 180, 240, 240, 120)
+    s.no_erase()
+
+    if s.frame_count > 160:
+        flag_done = True
+
+
+tests.append(test_erase)
+
+
+def test_lerp():
+    global flag_done
+    s.stroke((255, 255, 255))
+    s.background((51, 51, 51))
+    color_a = (218, 165, 32)
+    color_b = (72, 61, 139)
+    inter_a = s.lerp_color(color_a, color_b, 0.33)
+    inter_b = s.lerp_color(color_a, color_b, 0.66)
+    s.fill(color_a)
+    s.rect(10, 20, 20, 60)
+    s.fill(inter_a)
+    s.rect(30, 20, 20, 60)
+    s.fill(inter_b)
+    s.rect(50, 20, 20, 60)
+    s.fill(color_b)
+    s.rect(70, 20, 20, 60)
+
+    if s.frame_count > 160:
+        flag_done = True
+
+
+tests.append(test_lerp)
+
 
 s.start(setup, draw, "Running tests")
```

### Comparing `edudraw-1.3.2/LICENSE` & `edudraw-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edudraw-1.3.2/README.md` & `edudraw-1.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -172,37 +172,40 @@
 
 # Documentation
 
 ## State methods
 
 These methods don't directly draw onto the screen, but rather control aspects of the simulation.
 
-### EduDraw(width: int, height: int, null_mode: bool = False)
+### EduDraw(width: int, height: int, null_mode: bool = False) -> EduDraw
 
 Initializer for the EduDraw class.
 
 Parameters:
 
 width, height: The width and height of the window to be created
 
 null_mode: Whether null mode should be used or not. Default: False. See more about null mode at the end.
 
 Returns a new instance of the EduDraw class.
 
+
 ### EduDraw.start(setup, draw, window_title: str)
 
 Starts the simulation.
 
 Parameters:
 
 setup: The setup() function written by the user
 
 draw: The draw() function written by the user
 
-window_title: A string to be used as a title for the window running the simulation. Note: This parameter is unused for null mode instances.
+window_title: A string to be used as a title for the window running the simulation. 
+Note: This parameter is unused for null mode instances.
+
 
 ### EduDraw.rect_mode(mode: str)
 
 Changes the current mode for drawing squares, rectangles and images.
 
 If ```mode``` is ```'TOP_LEFT'``` (which is the default), the (X,Y) coordinates passed in for the ```rect()``` and ```square()``` methods will represent the top left coordinate of the rectangle.
 
@@ -273,14 +276,15 @@
 ```
 
 ![circlemode](https://user-images.githubusercontent.com/88753590/233815073-8bb60f23-9c03-4c0d-982e-fc4e8a2319fc.png)
 
 
 ---
 
+
 ### EduDraw.fill(color: tuple)
 
 Makes all shapes drawn after this call to be filled in with a given color.
 
 Parameters:
 
 color: A tuple containing the (R, G, B) values of the color to fill the subsequent shapes.
@@ -297,18 +301,20 @@
 
         s.fill((255, 255, 0))
         s.circle(100, 150, 25)
 ```
 
 ![fill](https://user-images.githubusercontent.com/88753590/233815075-ed143b96-8cae-4f8d-ba53-338467a036d9.png)
 
+
 ### EduDraw.no_fill()
 
 Makes all shapes drawn after this call to not be filled in.
 
+
 ### EduDraw.font(new_font: str, font_size: int = 12, bold=False, italic=False, underline=False)
 
 Changes the font to be used when writing text. When the font is changed, all text will have it's font size, so the parameter for size in the `text()` method is not used. Note: This is a costly method, if possible, it's recommended to use it once in `setup()` instead of every frame in `draw()`. If you need to change font mid-drawing, it's recommended to use `font_from_instance()` instead with a preloaded font.
 
 Parameters:
 
 new_font: The name of the font to be used. See [Pygame fonts](https://www.pygame.org/docs/ref/font.html#pygame.font.get_fonts)
@@ -317,31 +323,35 @@
 
 bold: Whether the font should be bold or not. Default: False
 
 italic: Whether the font should be italic or not. Default: False
 
 underline: Whether the font should have an underline or not. Default: False
 
+
 ### EduDraw.font_from_instance(new_font: pygame.font.Font)
 
 Sets the font to be used when writing text to a premade instance of a `pygame.font.Font` object. It is recommended that, if you need to change fonts mid-drawing, you preload those fonts once before in your program and use this method to change them, instead of using the normal `font()` method, since it's costly to keep creating new instances every frame and the effect this has on performance is noticeable.
 
 Parameters:
 
 new_font: A `pygame.font.Font` instance to be used for text.
 
+
 ### EduDraw.change_default_font(new_font: str, font_size: int = 12, bold=False, italic=False, underline=False)
 
 Changes the default font to be used. This method is meant to be called in `setup()`, and is the preferred way of changing the font.
 The parameters are the same as `font()`.
 
+
 ### EduDraw.reset_font()
 
 Resets the font used to the default one.
 
+
 ### EduDraw.stroke(color: tuple)
 
 Makes all shapes drawn after this call to have their outlines drawn with a given color.
 
 Parameters:
 
 color: A tuple containing the (R, G, B) values of the color to draw the outlines of the subsequent shapes.
@@ -362,18 +372,20 @@
     s.stroke((0, 0, 255))
 
     s.triangle(200, 200, 300, 300, 350, 150)
 ```
 
 ![stroke](https://user-images.githubusercontent.com/88753590/233815081-9336437f-1eb6-41d9-81a2-15ecfcc8d0b4.png)
 
+
 ### EduDraw.no_stroke()
 
 Makes all subsequent shapes not have their outlines drawn. 
 
+
 ### EduDraw.stroke_weight(new_weight: int)
 
 Changes how thick or thin the stroke lines are, smaller numbers means thinner outlines, bigger numbers mean thicker outlines.
 
 Note: Due to the way antialiasing works with `gfxdraw`, the stroke weight has NO effect when drawing antialiased primitives and is always 1px.
 
 Parameters:
@@ -401,14 +413,15 @@
 ![strokeweight](https://user-images.githubusercontent.com/88753590/233815088-a628b74a-5d95-4188-bcd0-14c96c4ac359.png)
 
 
 ### EduDraw.push() 
 
 Toggles the temporary state on. All color, font and weight changes made while this mode is on will be reverted once it is left.
 
+
 ### EduDraw.pop()
 
 Toggles the temporary state off.
 
 Example:
 ```
     def draw():
@@ -467,15 +480,14 @@
         # Leave second state
         s.circle(200, 50, 25)
 ```
 
 ![pushpop2](https://user-images.githubusercontent.com/88753590/236652838-d6181f0e-9349-4437-bf7e-9cc1ae241e12.png)
 
 
-
 ### EduDraw.mouse_pos()-> tuple
 
 Gets the current mouse position (relative to the top left corner of the canvas).
 Returns a tuple with the X,Y position of the cursor.
 
 Returns:
 
@@ -493,17 +505,17 @@
         if 75 <= mouse_y <= 150:
             s.fill((255, 255, 0))
 
     s.circle(mouse_x, mouse_y, 3)
 
     s.square(75, 75, 75)
 
-    s.stroke((0, 255, 0))
+    s.fill((0, 255, 0))
     s.text(f"X: {mouse_x}", 10, 10)
-    s.stroke((255, 0, 0))
+    s.fill((255, 0, 0))
     s.text(f"Y: {mouse_y}", 10, 30)
 ```
 
 ![mousepos](https://user-images.githubusercontent.com/88753590/233815197-3eb81842-bb44-4e51-95ad-f4e4ffe52be4.gif)
 
 You can set whether this function should or not revert transformations to retrieve the perceived position by using
 `EduDraw.set_account_for_transformations(True)`, the example below illustrates the difference:
@@ -613,15 +625,14 @@
     s.pop()
     s.circle(80, 0, 10)
 ```
 
 ![advancedexample](https://user-images.githubusercontent.com/88753590/236653135-d38838d1-518c-4b70-a664-ea121cf71315.gif)
 
 
-
 ### EduDraw.scale(scale_x: float, scale_y: float) 
 
 Scales the drawing's axis by the desired multipliers
 Note: Is cumulative with other scalars.
 
 Parameters:
 
@@ -682,34 +693,39 @@
 ![translate](https://user-images.githubusercontent.com/88753590/236652958-1b89304d-9cb0-4104-9806-82dc0c8e9f3c.png)
 
 
 ### EduDraw.reset_transformations()
 
 Resets all transformations applied.
 
+
 ### EduDraw.reset_scaling() 
 
 Resets all scaling transformations applied.
 
+
 ### EduDraw.reset_translation() 
 
 Resets all translation transformations applied.
 
+
 ### EduDraw.reset_rotation() 
 
 Resets all rotation transformations applied.
 
+
 ### EduDraw.set_account_for_transformations(state: bool) 
 
 Changes wether `mouse_pos()` should yield the real or perceived position of the mouse.
 
 Parameters:
 
 state: The state to apply to this setting. `True` yields the perceived position, whereas `False` (the default) yields the real position.
 
+
 ### EduDraw.set_controls(key_down=None, key_up=None, mouse_motion=None, mouse_button_up=None, mouse_button_down=None, mouse_wheel=None)
 
 Sets functions to be ran on each specific Pygame event. `None` means that nothing will occur on those events.
 Each function must have a parameter to receive a dictionary containing the data related to that event (such
 as which key was pressed, where the mouse is, etc.)
 
 Parameters:
@@ -786,26 +802,57 @@
 ### EduDraw.toggle_antialising()
 
 Toggles antialiasing on or off. It's off by default.
 
 Note: Antialiasing needs more processing, especially when the number of shapes and their complexity is higher. Also, antialised shapes do not take
 into account the stroke weight of the lines, and all lines are drawn with the weight of 1px.
 
+
+### EduDraw.erase()
+
+Makes drawings erase from the canvas instead of drawing normally. This has the same effect has
+drawing with the same colors as the background color.
+
+
+### EduDraw.no_erase()
+
+Stops erasing shapes.
+
+Example:
+
+```
+def draw():
+    s.background((200, 200, 200))
+    s.fill((255, 255, 100))
+    s.triangle(0, s.height, s.width//2, 0, s.width, s.height)
+
+    s.fill((255, 0, 0))
+    s.erase()
+    s.circle(s.width//2, s.height//2, 50)
+    s.no_erase()
+
+    s.circle(s.width//2, s.height//2 - 65, 15)
+```
+
+![erasing](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/64debd22-9f24-49ef-86cf-94c7b8060444)
+
+
 ## Drawing methods
 
 These methods draw onto the canvas.
 
 ### EduDraw.point(x: int, y: int)
 
 Draws a point at coordinates (x,y)
 
 Parameters:
 
 x, y: The x,y coordinates to draw the point onto.
 
+
 ### EduDraw.text(string: str, x: int, y: int)
 
 Writes a string of text onto the screen.
 
 Parameters:
 
 string: The text to be written
@@ -817,24 +864,26 @@
 
 Sets a new background color and clears the canvas to it.
 
 Parameters:
 
 color: A tuple containing the (R, G, B) values of the desired color.
 
+
 ### EduDraw.circle(x: int, y: int, radius: int)
 
 Draws a circle onto the screen.
 
 Parameters:
 
 x, y: The coordinates of the top-left part of the rectangle that contains the circle if circle_mode is 'TOP_LEFT', or the center of the circle if circle_mode is 'CENTER'.
 
 r: The radius of the circle.
 
+
 ### EduDraw.ellipse(x: int, y: int, width: int, height: int)
 
 Draws an ellipse onto the screen.
 
 Parameters:
 
 x, y: The coordinates of the top-left part of the rectange that contains the ellipse if circle_mode is 'TOP_LEFT', or the center of the ellipse if circle_mode is 'CENTER'.
@@ -973,15 +1022,14 @@
     s.triangle(120, 40, 200, 40, 160, 120)
     s.triangle(80, 120, 160, 120, 120, 200)
 ```
 
 ![triangle](https://user-images.githubusercontent.com/88753590/233815214-5f44f6b7-4d0a-41f8-88f8-3b384e1d117f.png)
 
 
-
 ### EduDraw.polygon(points: list)
 
 Draws any polygon onto the screen.
 
 Parameters:
 
 points: An array containing tuples with all of the vertices of the polygon.
@@ -1004,14 +1052,15 @@
 ```
 
 ![polygon](https://user-images.githubusercontent.com/88753590/233815221-2da1f919-571f-40a2-ad96-cb4e4084875b.png)
 
 
 ---
 
+
 ### EduDraw.image(img: pygame.surface.Surface, x: int, y: int, width: int = None, height: int = None, force_transparency: bool = False):
     
 Displays an image onto the screen on the (x,y) position. If specified a width or height, the image will be resized to those sizes, otherwise, the image will be drawn to it's original size.
     
 Parameters:
 
 img: The image to be drawn onto the canvas
@@ -1040,14 +1089,159 @@
 Note that some images may not have transparency when transformed into `pygame.Surface` objects through the
 `pygame.image.load()` method. Should this be the case, like the one below, you can use the `force_transparency`
 parameter to force that.
 
 ![example](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/c350c788-3cc4-491e-94f9-67c1a7aa8a78)
 
 
+### EduDraw.bezier_curve(self, control_points: list, num_points: int | None = None)
+
+Draws a bezier curve from a set of control points
+
+Parameters:
+
+control_points: A list of tuples containing the coordinates of the control points for the curve
+
+num_points (optional): The number of points to be used as steps for the lines. Default: 30
+
+Example:
+
+```
+control_points = [(100, 100), (150, 500), (450, 500), (500, 150)]
+
+def draw():
+    s.background((255, 255, 255))
+    s.stroke((255, 0, 0))
+    s.stroke_weight(3)
+    s.bezier_curve(control_points, 70)
+
+    # Drawing the control points for visibility
+    for point in control_points:
+        s.circle(point[0], point[1], 5)
+```
+
+
+### EduDraw.arc_open(self, start_angle: int, stop_angle: int, x: int, y: int, width: int, height: int)
+
+Draws an open arc onto the canvas.
+
+Parameters:
+
+start_angle: The starting angle (in degrees) of the arc
+
+stop_angle: The stopping angle (in degrees) of the arc
+
+x: The x coordinate to draw the arc, if circle mode is top_left, it's the top left of the rectangle
+containing the ellipse, else it's the center of the ellipse
+
+y: The y coordinate to draw the arc
+
+width: The width of the ellipse to create the arc
+
+height: The height of the ellipse to create the arc
+
+```
+def draw():
+    s.background((200, 200, 200))
+    s.stroke_weight(3)
+
+    s.fill((255, 0, 0))
+    # Circular red pie that starts at 60 degrees and ends at 300
+    s.arc_open(60, 300, s.width // 4 + 5, s.height//2, s.width//2, s.height//2)
+
+    s.fill((0, 255, 0))
+    # Elliptical green pie that starts at 300 degrees and ends at 60
+    s.arc_open(300, 60, int(s.width * 0.75) - 5, s.height//2, s.width//2, s.height)
+```
+
+![open_arcs](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/35c47f31-e9c9-4e57-a5e0-ab74e5dd035e)
+
+
+
+### EduDraw.arc_pie(start_angle: int, stop_angle: int, x: int, y: int, width: int, height: int, close_edges: bool = True)
+
+Draws a pie-like arc in a counter-clockwise direction from the starting angle up to the stopping angle.
+
+Parameters:
+
+start_angle: The starting angle to draw the pie
+
+stop_angle: The angle to stop the pie
+
+x: The x coordinate to draw the ellipse of the pie
+
+y: The y coordinate to draw the ellipse of the pie
+
+width: The horizontal diameter of the ellipse
+
+height: The vertical diameter of the ellipse
+
+close_edges (optional): Whether the lines from the edges of the pie should be drawn. Default: True
+
+Example:
+
+```
+def draw():
+    s.background((200, 200, 200))
+    s.stroke_weight(3)
+
+    s.fill((255, 0, 0))
+    # Circular red pie that starts at 60 degrees and ends at 300
+    s.arc_pie(60, 300, s.width // 4 + 5, s.height//2, s.width//2, s.height//2)
+
+    s.fill((0, 255, 0))
+    # Elliptical green pie that starts at 300 degrees and ends at 60
+    s.arc_pie(300, 60, int(s.width * 0.75) - 5, s.height//2, s.width//2, s.height)
+```
+
+![pie](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/3ace4d82-2e7f-435a-897d-cd9194ccd00c)
+
+
+### EduDraw.arc_closed(start_angle: int, stop_angle: int, x: int, y: int, width: int, height: int, close_edges: bool = True)
+
+Draws a closed arc between two angles in an ellipse
+
+Parameters: 
+
+start_angle: The starting angle of the arc
+
+stop_angle: The stopping angle of the arc
+
+x: The x coordinate to place the arc's ellipse
+
+y: The y coordinate to place the arc's ellipse
+
+width: The width of the ellipse
+
+height: The height of the ellipse
+
+close_edges (optional): Whether the edges between the starting and stopping angles should be connected.
+Default: True
+
+Example:
+
+```
+def draw():
+    s.background((200, 200, 200))
+    s.stroke_weight(3)
+
+    s.fill((255, 0, 0))
+    # Circular red arc that starts at 60 degrees and ends at 300
+    s.arc_closed(60, 300, s.width // 4 + 5, s.height//2, s.width//2, s.height//2)
+
+    s.fill((0, 255, 0))
+    # Elliptical green arc that starts at 300 degrees and ends at 60
+    s.arc_closed(300, 60, int(s.width * 0.75) - 5, s.height//2, s.width//2, s.height)
+```
+
+![arcs_closed](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/4d096234-b456-454e-a1a7-5c692b561555)
+
+
+## Other methods
+
 ### EduDraw.frame_rate(fps: int)
 
 Changes the framerate of the simulation. Must be called in ```setup()```.
 Note that in the Python version the simulation does not run as fast as the C# one, to run the simulation as fast as possible set the EduDraw.deltatime to zero.
 
 Parameters:
 
@@ -1060,15 +1254,128 @@
 If filename is empty, the name will be the frame count of when the photo was saved.
 
 
 ### EduDraw.quit()
 
 Quits the simulation.
 
-### Null mode
+
+### EduDraw.load_sound(file: str) -> pygame.mixer.Sound
+
+Loads a sound from a file and turns it into a `pygame.mixer.Sound` instance.
+
+Parameters:
+
+file: A string with the path to the file to be loaded
+
+Returns a new Sound class instance.
+
+
+### EduDraw.play_sound(sound: pygame.mixer.Sound, loops: int = 0, max_time: int = 0, fade_time: int = 0)
+
+Plays a loaded sound.
+
+Parameters:
+
+sound: A loaded `pygame.mixer.Sound` instance to be played.
+
+loops (optional): The amount of times to loop the audio
+
+max_time (optional): The maximum time (ms) to play the audio
+
+fade_time (optional): The fading time of the audio (in ms)
+
+
+### EduDraw.remove_icon()
+
+Removes the current icon from window
+
+
+### EduDraw.change_icon(self, image: pygame.surface.Surface)
+
+Changes icon to a user-defined image
+
+Parameters:
+
+image: The image to be used as icon
+
+
+### EduDraw.retrieve_frame() -> pygame.surface.Surface
+
+Retrieves the current frame of the simulation as a pygame Surface image.
+
+Returns the currently drawn frame from when this method was called.
+
+
+### EduDraw.lerp_color(color_1: tuple, color_2: tuple, amount: float = 0.5) -> tuple
+
+Mixes two color to find an intermediary color between them
+
+Parameters:
+
+color_1: The color to lerp from
+
+color_2: The color to lerp to
+
+amount (optional): How close the resulting color should be to the two colors to be mixed.
+Default: 0.5
+
+Example:
+
+```
+def draw():
+    s.stroke((255, 255, 255))
+    s.background((51, 51, 51))
+    color_a = (218, 165, 32)  # Starting color
+    color_b = (72, 61, 139)  # Destination color
+    inter_a = s.lerp_color(color_a, color_b, 0.33)
+    inter_b = s.lerp_color(color_a, color_b, 0.66)
+    s.fill(color_a)
+    s.rect(10, 20, 20, 60)
+    s.fill(inter_a)
+    s.rect(30, 20, 20, 60)
+    s.fill(inter_b)
+    s.rect(50, 20, 20, 60)
+    s.fill(color_b)
+    s.rect(70, 20, 20, 60)
+```
+
+![lerp_image](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/fa6defc4-69d5-489a-82c8-2fb6d19c2500)
+
+
+### EduDraw.get_color_from_pos(x: int, y: int) -> tuple
+
+Retrieves the color from a given position in the current frame
+
+Parameters:
+
+x: The x coordinate to retrieve the color from
+
+y: The y coordinate to retrieve the color from
+
+Returns a (r,g,b,a) tuple with the color at that position
+
+
+### EduDraw.is_focused() -> bool
+
+Gets whether the display is focused or not.
+
+Returns True if display is focused, False if not
+
+
+### EduDraw.set_mouse_visibility(visible: bool)
+
+Changes the visibility of the cursor
+
+Parameters:
+
+visible: Whether the mouse should be visible or hidden
+
+
+## Null mode
 
 Null mode is a mode in which you can run an instance of a simulation without having it running directly onto the canvas. You can do this for many reasons, including using EduDraw in a different context or application, creating multiple drawings inside of one another, among other things.
 
 To initialize an EduDraw instance in null mode, you can use the optional parameter for it in the `start()` method.
 
 Example of null mode:
 
@@ -1132,8 +1439,7 @@
     s.image(d.screen, 0, 0)
     
 d.start(setup, inner_drawing, "This does not appear")
 s.start(setup, draw, "My drawing :D")
 ```
 
 ![nullmode](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/5026c565-f081-49cf-8bfd-55fe487bada6)
-
```

### Comparing `edudraw-1.3.2/pyproject.toml` & `edudraw-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EduDraw"
-version = "1.3.2"
+version = "1.4.0"
 authors = [
   { name="Murilo Luis Calvo Neves", email="muriloluiscalvoneves2004@hotmail.com" },
 ]
 description = "A simple interface for using 2D graphics in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `edudraw-1.3.2/PKG-INFO` & `edudraw-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduDraw
-Version: 1.3.2
+Version: 1.4.0
 Summary: A simple interface for using 2D graphics in python
 Project-URL: Homepage, https://github.com/MuriloLCN/Edu-Draw-Python
 Project-URL: Bug Tracker, https://github.com/MuriloLCN/Edu-Draw-Python/issues
 Author-email: Murilo Luis Calvo Neves <muriloluiscalvoneves2004@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -186,37 +186,40 @@
 
 # Documentation
 
 ## State methods
 
 These methods don't directly draw onto the screen, but rather control aspects of the simulation.
 
-### EduDraw(width: int, height: int, null_mode: bool = False)
+### EduDraw(width: int, height: int, null_mode: bool = False) -> EduDraw
 
 Initializer for the EduDraw class.
 
 Parameters:
 
 width, height: The width and height of the window to be created
 
 null_mode: Whether null mode should be used or not. Default: False. See more about null mode at the end.
 
 Returns a new instance of the EduDraw class.
 
+
 ### EduDraw.start(setup, draw, window_title: str)
 
 Starts the simulation.
 
 Parameters:
 
 setup: The setup() function written by the user
 
 draw: The draw() function written by the user
 
-window_title: A string to be used as a title for the window running the simulation. Note: This parameter is unused for null mode instances.
+window_title: A string to be used as a title for the window running the simulation. 
+Note: This parameter is unused for null mode instances.
+
 
 ### EduDraw.rect_mode(mode: str)
 
 Changes the current mode for drawing squares, rectangles and images.
 
 If ```mode``` is ```'TOP_LEFT'``` (which is the default), the (X,Y) coordinates passed in for the ```rect()``` and ```square()``` methods will represent the top left coordinate of the rectangle.
 
@@ -287,14 +290,15 @@
 ```
 
 ![circlemode](https://user-images.githubusercontent.com/88753590/233815073-8bb60f23-9c03-4c0d-982e-fc4e8a2319fc.png)
 
 
 ---
 
+
 ### EduDraw.fill(color: tuple)
 
 Makes all shapes drawn after this call to be filled in with a given color.
 
 Parameters:
 
 color: A tuple containing the (R, G, B) values of the color to fill the subsequent shapes.
@@ -311,18 +315,20 @@
 
         s.fill((255, 255, 0))
         s.circle(100, 150, 25)
 ```
 
 ![fill](https://user-images.githubusercontent.com/88753590/233815075-ed143b96-8cae-4f8d-ba53-338467a036d9.png)
 
+
 ### EduDraw.no_fill()
 
 Makes all shapes drawn after this call to not be filled in.
 
+
 ### EduDraw.font(new_font: str, font_size: int = 12, bold=False, italic=False, underline=False)
 
 Changes the font to be used when writing text. When the font is changed, all text will have it's font size, so the parameter for size in the `text()` method is not used. Note: This is a costly method, if possible, it's recommended to use it once in `setup()` instead of every frame in `draw()`. If you need to change font mid-drawing, it's recommended to use `font_from_instance()` instead with a preloaded font.
 
 Parameters:
 
 new_font: The name of the font to be used. See [Pygame fonts](https://www.pygame.org/docs/ref/font.html#pygame.font.get_fonts)
@@ -331,31 +337,35 @@
 
 bold: Whether the font should be bold or not. Default: False
 
 italic: Whether the font should be italic or not. Default: False
 
 underline: Whether the font should have an underline or not. Default: False
 
+
 ### EduDraw.font_from_instance(new_font: pygame.font.Font)
 
 Sets the font to be used when writing text to a premade instance of a `pygame.font.Font` object. It is recommended that, if you need to change fonts mid-drawing, you preload those fonts once before in your program and use this method to change them, instead of using the normal `font()` method, since it's costly to keep creating new instances every frame and the effect this has on performance is noticeable.
 
 Parameters:
 
 new_font: A `pygame.font.Font` instance to be used for text.
 
+
 ### EduDraw.change_default_font(new_font: str, font_size: int = 12, bold=False, italic=False, underline=False)
 
 Changes the default font to be used. This method is meant to be called in `setup()`, and is the preferred way of changing the font.
 The parameters are the same as `font()`.
 
+
 ### EduDraw.reset_font()
 
 Resets the font used to the default one.
 
+
 ### EduDraw.stroke(color: tuple)
 
 Makes all shapes drawn after this call to have their outlines drawn with a given color.
 
 Parameters:
 
 color: A tuple containing the (R, G, B) values of the color to draw the outlines of the subsequent shapes.
@@ -376,18 +386,20 @@
     s.stroke((0, 0, 255))
 
     s.triangle(200, 200, 300, 300, 350, 150)
 ```
 
 ![stroke](https://user-images.githubusercontent.com/88753590/233815081-9336437f-1eb6-41d9-81a2-15ecfcc8d0b4.png)
 
+
 ### EduDraw.no_stroke()
 
 Makes all subsequent shapes not have their outlines drawn. 
 
+
 ### EduDraw.stroke_weight(new_weight: int)
 
 Changes how thick or thin the stroke lines are, smaller numbers means thinner outlines, bigger numbers mean thicker outlines.
 
 Note: Due to the way antialiasing works with `gfxdraw`, the stroke weight has NO effect when drawing antialiased primitives and is always 1px.
 
 Parameters:
@@ -415,14 +427,15 @@
 ![strokeweight](https://user-images.githubusercontent.com/88753590/233815088-a628b74a-5d95-4188-bcd0-14c96c4ac359.png)
 
 
 ### EduDraw.push() 
 
 Toggles the temporary state on. All color, font and weight changes made while this mode is on will be reverted once it is left.
 
+
 ### EduDraw.pop()
 
 Toggles the temporary state off.
 
 Example:
 ```
     def draw():
@@ -481,15 +494,14 @@
         # Leave second state
         s.circle(200, 50, 25)
 ```
 
 ![pushpop2](https://user-images.githubusercontent.com/88753590/236652838-d6181f0e-9349-4437-bf7e-9cc1ae241e12.png)
 
 
-
 ### EduDraw.mouse_pos()-> tuple
 
 Gets the current mouse position (relative to the top left corner of the canvas).
 Returns a tuple with the X,Y position of the cursor.
 
 Returns:
 
@@ -507,17 +519,17 @@
         if 75 <= mouse_y <= 150:
             s.fill((255, 255, 0))
 
     s.circle(mouse_x, mouse_y, 3)
 
     s.square(75, 75, 75)
 
-    s.stroke((0, 255, 0))
+    s.fill((0, 255, 0))
     s.text(f"X: {mouse_x}", 10, 10)
-    s.stroke((255, 0, 0))
+    s.fill((255, 0, 0))
     s.text(f"Y: {mouse_y}", 10, 30)
 ```
 
 ![mousepos](https://user-images.githubusercontent.com/88753590/233815197-3eb81842-bb44-4e51-95ad-f4e4ffe52be4.gif)
 
 You can set whether this function should or not revert transformations to retrieve the perceived position by using
 `EduDraw.set_account_for_transformations(True)`, the example below illustrates the difference:
@@ -627,15 +639,14 @@
     s.pop()
     s.circle(80, 0, 10)
 ```
 
 ![advancedexample](https://user-images.githubusercontent.com/88753590/236653135-d38838d1-518c-4b70-a664-ea121cf71315.gif)
 
 
-
 ### EduDraw.scale(scale_x: float, scale_y: float) 
 
 Scales the drawing's axis by the desired multipliers
 Note: Is cumulative with other scalars.
 
 Parameters:
 
@@ -696,34 +707,39 @@
 ![translate](https://user-images.githubusercontent.com/88753590/236652958-1b89304d-9cb0-4104-9806-82dc0c8e9f3c.png)
 
 
 ### EduDraw.reset_transformations()
 
 Resets all transformations applied.
 
+
 ### EduDraw.reset_scaling() 
 
 Resets all scaling transformations applied.
 
+
 ### EduDraw.reset_translation() 
 
 Resets all translation transformations applied.
 
+
 ### EduDraw.reset_rotation() 
 
 Resets all rotation transformations applied.
 
+
 ### EduDraw.set_account_for_transformations(state: bool) 
 
 Changes wether `mouse_pos()` should yield the real or perceived position of the mouse.
 
 Parameters:
 
 state: The state to apply to this setting. `True` yields the perceived position, whereas `False` (the default) yields the real position.
 
+
 ### EduDraw.set_controls(key_down=None, key_up=None, mouse_motion=None, mouse_button_up=None, mouse_button_down=None, mouse_wheel=None)
 
 Sets functions to be ran on each specific Pygame event. `None` means that nothing will occur on those events.
 Each function must have a parameter to receive a dictionary containing the data related to that event (such
 as which key was pressed, where the mouse is, etc.)
 
 Parameters:
@@ -800,26 +816,57 @@
 ### EduDraw.toggle_antialising()
 
 Toggles antialiasing on or off. It's off by default.
 
 Note: Antialiasing needs more processing, especially when the number of shapes and their complexity is higher. Also, antialised shapes do not take
 into account the stroke weight of the lines, and all lines are drawn with the weight of 1px.
 
+
+### EduDraw.erase()
+
+Makes drawings erase from the canvas instead of drawing normally. This has the same effect has
+drawing with the same colors as the background color.
+
+
+### EduDraw.no_erase()
+
+Stops erasing shapes.
+
+Example:
+
+```
+def draw():
+    s.background((200, 200, 200))
+    s.fill((255, 255, 100))
+    s.triangle(0, s.height, s.width//2, 0, s.width, s.height)
+
+    s.fill((255, 0, 0))
+    s.erase()
+    s.circle(s.width//2, s.height//2, 50)
+    s.no_erase()
+
+    s.circle(s.width//2, s.height//2 - 65, 15)
+```
+
+![erasing](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/64debd22-9f24-49ef-86cf-94c7b8060444)
+
+
 ## Drawing methods
 
 These methods draw onto the canvas.
 
 ### EduDraw.point(x: int, y: int)
 
 Draws a point at coordinates (x,y)
 
 Parameters:
 
 x, y: The x,y coordinates to draw the point onto.
 
+
 ### EduDraw.text(string: str, x: int, y: int)
 
 Writes a string of text onto the screen.
 
 Parameters:
 
 string: The text to be written
@@ -831,24 +878,26 @@
 
 Sets a new background color and clears the canvas to it.
 
 Parameters:
 
 color: A tuple containing the (R, G, B) values of the desired color.
 
+
 ### EduDraw.circle(x: int, y: int, radius: int)
 
 Draws a circle onto the screen.
 
 Parameters:
 
 x, y: The coordinates of the top-left part of the rectangle that contains the circle if circle_mode is 'TOP_LEFT', or the center of the circle if circle_mode is 'CENTER'.
 
 r: The radius of the circle.
 
+
 ### EduDraw.ellipse(x: int, y: int, width: int, height: int)
 
 Draws an ellipse onto the screen.
 
 Parameters:
 
 x, y: The coordinates of the top-left part of the rectange that contains the ellipse if circle_mode is 'TOP_LEFT', or the center of the ellipse if circle_mode is 'CENTER'.
@@ -987,15 +1036,14 @@
     s.triangle(120, 40, 200, 40, 160, 120)
     s.triangle(80, 120, 160, 120, 120, 200)
 ```
 
 ![triangle](https://user-images.githubusercontent.com/88753590/233815214-5f44f6b7-4d0a-41f8-88f8-3b384e1d117f.png)
 
 
-
 ### EduDraw.polygon(points: list)
 
 Draws any polygon onto the screen.
 
 Parameters:
 
 points: An array containing tuples with all of the vertices of the polygon.
@@ -1018,14 +1066,15 @@
 ```
 
 ![polygon](https://user-images.githubusercontent.com/88753590/233815221-2da1f919-571f-40a2-ad96-cb4e4084875b.png)
 
 
 ---
 
+
 ### EduDraw.image(img: pygame.surface.Surface, x: int, y: int, width: int = None, height: int = None, force_transparency: bool = False):
     
 Displays an image onto the screen on the (x,y) position. If specified a width or height, the image will be resized to those sizes, otherwise, the image will be drawn to it's original size.
     
 Parameters:
 
 img: The image to be drawn onto the canvas
@@ -1054,14 +1103,159 @@
 Note that some images may not have transparency when transformed into `pygame.Surface` objects through the
 `pygame.image.load()` method. Should this be the case, like the one below, you can use the `force_transparency`
 parameter to force that.
 
 ![example](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/c350c788-3cc4-491e-94f9-67c1a7aa8a78)
 
 
+### EduDraw.bezier_curve(self, control_points: list, num_points: int | None = None)
+
+Draws a bezier curve from a set of control points
+
+Parameters:
+
+control_points: A list of tuples containing the coordinates of the control points for the curve
+
+num_points (optional): The number of points to be used as steps for the lines. Default: 30
+
+Example:
+
+```
+control_points = [(100, 100), (150, 500), (450, 500), (500, 150)]
+
+def draw():
+    s.background((255, 255, 255))
+    s.stroke((255, 0, 0))
+    s.stroke_weight(3)
+    s.bezier_curve(control_points, 70)
+
+    # Drawing the control points for visibility
+    for point in control_points:
+        s.circle(point[0], point[1], 5)
+```
+
+
+### EduDraw.arc_open(self, start_angle: int, stop_angle: int, x: int, y: int, width: int, height: int)
+
+Draws an open arc onto the canvas.
+
+Parameters:
+
+start_angle: The starting angle (in degrees) of the arc
+
+stop_angle: The stopping angle (in degrees) of the arc
+
+x: The x coordinate to draw the arc, if circle mode is top_left, it's the top left of the rectangle
+containing the ellipse, else it's the center of the ellipse
+
+y: The y coordinate to draw the arc
+
+width: The width of the ellipse to create the arc
+
+height: The height of the ellipse to create the arc
+
+```
+def draw():
+    s.background((200, 200, 200))
+    s.stroke_weight(3)
+
+    s.fill((255, 0, 0))
+    # Circular red pie that starts at 60 degrees and ends at 300
+    s.arc_open(60, 300, s.width // 4 + 5, s.height//2, s.width//2, s.height//2)
+
+    s.fill((0, 255, 0))
+    # Elliptical green pie that starts at 300 degrees and ends at 60
+    s.arc_open(300, 60, int(s.width * 0.75) - 5, s.height//2, s.width//2, s.height)
+```
+
+![open_arcs](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/35c47f31-e9c9-4e57-a5e0-ab74e5dd035e)
+
+
+
+### EduDraw.arc_pie(start_angle: int, stop_angle: int, x: int, y: int, width: int, height: int, close_edges: bool = True)
+
+Draws a pie-like arc in a counter-clockwise direction from the starting angle up to the stopping angle.
+
+Parameters:
+
+start_angle: The starting angle to draw the pie
+
+stop_angle: The angle to stop the pie
+
+x: The x coordinate to draw the ellipse of the pie
+
+y: The y coordinate to draw the ellipse of the pie
+
+width: The horizontal diameter of the ellipse
+
+height: The vertical diameter of the ellipse
+
+close_edges (optional): Whether the lines from the edges of the pie should be drawn. Default: True
+
+Example:
+
+```
+def draw():
+    s.background((200, 200, 200))
+    s.stroke_weight(3)
+
+    s.fill((255, 0, 0))
+    # Circular red pie that starts at 60 degrees and ends at 300
+    s.arc_pie(60, 300, s.width // 4 + 5, s.height//2, s.width//2, s.height//2)
+
+    s.fill((0, 255, 0))
+    # Elliptical green pie that starts at 300 degrees and ends at 60
+    s.arc_pie(300, 60, int(s.width * 0.75) - 5, s.height//2, s.width//2, s.height)
+```
+
+![pie](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/3ace4d82-2e7f-435a-897d-cd9194ccd00c)
+
+
+### EduDraw.arc_closed(start_angle: int, stop_angle: int, x: int, y: int, width: int, height: int, close_edges: bool = True)
+
+Draws a closed arc between two angles in an ellipse
+
+Parameters: 
+
+start_angle: The starting angle of the arc
+
+stop_angle: The stopping angle of the arc
+
+x: The x coordinate to place the arc's ellipse
+
+y: The y coordinate to place the arc's ellipse
+
+width: The width of the ellipse
+
+height: The height of the ellipse
+
+close_edges (optional): Whether the edges between the starting and stopping angles should be connected.
+Default: True
+
+Example:
+
+```
+def draw():
+    s.background((200, 200, 200))
+    s.stroke_weight(3)
+
+    s.fill((255, 0, 0))
+    # Circular red arc that starts at 60 degrees and ends at 300
+    s.arc_closed(60, 300, s.width // 4 + 5, s.height//2, s.width//2, s.height//2)
+
+    s.fill((0, 255, 0))
+    # Elliptical green arc that starts at 300 degrees and ends at 60
+    s.arc_closed(300, 60, int(s.width * 0.75) - 5, s.height//2, s.width//2, s.height)
+```
+
+![arcs_closed](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/4d096234-b456-454e-a1a7-5c692b561555)
+
+
+## Other methods
+
 ### EduDraw.frame_rate(fps: int)
 
 Changes the framerate of the simulation. Must be called in ```setup()```.
 Note that in the Python version the simulation does not run as fast as the C# one, to run the simulation as fast as possible set the EduDraw.deltatime to zero.
 
 Parameters:
 
@@ -1074,15 +1268,128 @@
 If filename is empty, the name will be the frame count of when the photo was saved.
 
 
 ### EduDraw.quit()
 
 Quits the simulation.
 
-### Null mode
+
+### EduDraw.load_sound(file: str) -> pygame.mixer.Sound
+
+Loads a sound from a file and turns it into a `pygame.mixer.Sound` instance.
+
+Parameters:
+
+file: A string with the path to the file to be loaded
+
+Returns a new Sound class instance.
+
+
+### EduDraw.play_sound(sound: pygame.mixer.Sound, loops: int = 0, max_time: int = 0, fade_time: int = 0)
+
+Plays a loaded sound.
+
+Parameters:
+
+sound: A loaded `pygame.mixer.Sound` instance to be played.
+
+loops (optional): The amount of times to loop the audio
+
+max_time (optional): The maximum time (ms) to play the audio
+
+fade_time (optional): The fading time of the audio (in ms)
+
+
+### EduDraw.remove_icon()
+
+Removes the current icon from window
+
+
+### EduDraw.change_icon(self, image: pygame.surface.Surface)
+
+Changes icon to a user-defined image
+
+Parameters:
+
+image: The image to be used as icon
+
+
+### EduDraw.retrieve_frame() -> pygame.surface.Surface
+
+Retrieves the current frame of the simulation as a pygame Surface image.
+
+Returns the currently drawn frame from when this method was called.
+
+
+### EduDraw.lerp_color(color_1: tuple, color_2: tuple, amount: float = 0.5) -> tuple
+
+Mixes two color to find an intermediary color between them
+
+Parameters:
+
+color_1: The color to lerp from
+
+color_2: The color to lerp to
+
+amount (optional): How close the resulting color should be to the two colors to be mixed.
+Default: 0.5
+
+Example:
+
+```
+def draw():
+    s.stroke((255, 255, 255))
+    s.background((51, 51, 51))
+    color_a = (218, 165, 32)  # Starting color
+    color_b = (72, 61, 139)  # Destination color
+    inter_a = s.lerp_color(color_a, color_b, 0.33)
+    inter_b = s.lerp_color(color_a, color_b, 0.66)
+    s.fill(color_a)
+    s.rect(10, 20, 20, 60)
+    s.fill(inter_a)
+    s.rect(30, 20, 20, 60)
+    s.fill(inter_b)
+    s.rect(50, 20, 20, 60)
+    s.fill(color_b)
+    s.rect(70, 20, 20, 60)
+```
+
+![lerp_image](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/fa6defc4-69d5-489a-82c8-2fb6d19c2500)
+
+
+### EduDraw.get_color_from_pos(x: int, y: int) -> tuple
+
+Retrieves the color from a given position in the current frame
+
+Parameters:
+
+x: The x coordinate to retrieve the color from
+
+y: The y coordinate to retrieve the color from
+
+Returns a (r,g,b,a) tuple with the color at that position
+
+
+### EduDraw.is_focused() -> bool
+
+Gets whether the display is focused or not.
+
+Returns True if display is focused, False if not
+
+
+### EduDraw.set_mouse_visibility(visible: bool)
+
+Changes the visibility of the cursor
+
+Parameters:
+
+visible: Whether the mouse should be visible or hidden
+
+
+## Null mode
 
 Null mode is a mode in which you can run an instance of a simulation without having it running directly onto the canvas. You can do this for many reasons, including using EduDraw in a different context or application, creating multiple drawings inside of one another, among other things.
 
 To initialize an EduDraw instance in null mode, you can use the optional parameter for it in the `start()` method.
 
 Example of null mode:
 
@@ -1146,8 +1453,7 @@
     s.image(d.screen, 0, 0)
     
 d.start(setup, inner_drawing, "This does not appear")
 s.start(setup, draw, "My drawing :D")
 ```
 
 ![nullmode](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/5026c565-f081-49cf-8bfd-55fe487bada6)
-
```

