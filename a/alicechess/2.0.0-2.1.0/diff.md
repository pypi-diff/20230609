# Comparing `tmp/alicechess-2.0.0.tar.gz` & `tmp/alicechess-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicechess-2.0.0.tar", max compression
+gzip compressed data, was "alicechess-2.1.0.tar", max compression
```

## Comparing `alicechess-2.0.0.tar` & `alicechess-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-2.0.0/LICENSE
--rw-r--r--   0        0        0     3740 2023-06-09 04:29:05.322145 alicechess-2.0.0/README.md
--rw-r--r--   0        0        0     1042 2023-06-09 04:40:57.176153 alicechess-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      208 2023-06-09 04:36:24.042041 alicechess-2.0.0/src/alicechess/__init__.py
--rw-r--r--   0        0        0      410 2023-06-09 04:36:08.864143 alicechess-2.0.0/src/alicechess/__main__.py
--rw-r--r--   0        0        0       65 2023-06-09 04:40:41.830358 alicechess-2.0.0/src/alicechess/__version__.py
--rw-r--r--   0        0        0    15265 2023-06-09 04:36:45.923112 alicechess-2.0.0/src/alicechess/_moves_calculator.py
--rw-r--r--   0        0        0     3520 2023-06-09 04:37:00.369033 alicechess-2.0.0/src/alicechess/bots.py
--rw-r--r--   0        0        0     1950 2023-06-09 04:38:27.983773 alicechess-2.0.0/src/alicechess/game.py
--rw-r--r--   0        0        0    36291 2023-06-09 04:37:28.559970 alicechess-2.0.0/src/alicechess/game_state.py
--rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-2.0.0/src/alicechess/pictures/BB.png
--rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-2.0.0/src/alicechess/pictures/BK.png
--rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-2.0.0/src/alicechess/pictures/BN.png
--rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-2.0.0/src/alicechess/pictures/BP.png
--rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-2.0.0/src/alicechess/pictures/BQ.png
--rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-2.0.0/src/alicechess/pictures/BR.png
--rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-2.0.0/src/alicechess/pictures/WB.png
--rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-2.0.0/src/alicechess/pictures/WK.png
--rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-2.0.0/src/alicechess/pictures/WN.png
--rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-2.0.0/src/alicechess/pictures/WP.png
--rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-2.0.0/src/alicechess/pictures/WQ.png
--rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-2.0.0/src/alicechess/pictures/WR.png
--rw-r--r--   0        0        0     2129 2023-06-09 04:32:36.557471 alicechess-2.0.0/src/alicechess/pieces/__init__.py
--rw-r--r--   0        0        0     2566 2023-06-09 04:32:19.713301 alicechess-2.0.0/src/alicechess/pieces/king.py
--rw-r--r--   0        0        0     1396 2023-06-09 04:32:48.125403 alicechess-2.0.0/src/alicechess/pieces/pawn.py
--rw-r--r--   0        0        0     8089 2023-06-09 04:32:57.403280 alicechess-2.0.0/src/alicechess/pieces/piece.py
--rw-r--r--   0        0        0     2178 2023-06-09 04:37:41.423231 alicechess-2.0.0/src/alicechess/player.py
--rw-r--r--   0        0        0     9936 2023-06-09 04:37:46.484148 alicechess-2.0.0/src/alicechess/position.py
--rw-r--r--   0        0        0     2644 2023-06-09 04:26:49.101173 alicechess-2.0.0/src/alicechess/utils.py
--rw-r--r--   0        0        0    21874 2023-06-09 04:39:18.703016 alicechess-2.0.0/src/alicechess/window.py
--rw-r--r--   0        0        0     4620 1970-01-01 00:00:00.000000 alicechess-2.0.0/setup.py
--rw-r--r--   0        0        0     4496 1970-01-01 00:00:00.000000 alicechess-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4279 2023-06-09 07:07:55.894301 alicechess-2.1.0/README.md
+-rw-r--r--   0        0        0     1042 2023-06-09 17:42:29.149110 alicechess-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-06-09 04:36:24.042041 alicechess-2.1.0/src/alicechess/__init__.py
+-rw-r--r--   0        0        0      593 2023-06-09 17:41:11.497466 alicechess-2.1.0/src/alicechess/__main__.py
+-rw-r--r--   0        0        0       65 2023-06-09 17:42:56.232815 alicechess-2.1.0/src/alicechess/__version__.py
+-rw-r--r--   0        0        0    15265 2023-06-09 04:36:45.923112 alicechess-2.1.0/src/alicechess/_moves_calculator.py
+-rw-r--r--   0        0        0     3520 2023-06-09 04:37:00.369033 alicechess-2.1.0/src/alicechess/bots.py
+-rw-r--r--   0        0        0     1950 2023-06-09 04:38:27.983773 alicechess-2.1.0/src/alicechess/game.py
+-rw-r--r--   0        0        0    36291 2023-06-09 04:37:28.559970 alicechess-2.1.0/src/alicechess/game_state.py
+-rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-2.1.0/src/alicechess/pictures/BB.png
+-rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-2.1.0/src/alicechess/pictures/BK.png
+-rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-2.1.0/src/alicechess/pictures/BN.png
+-rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-2.1.0/src/alicechess/pictures/BP.png
+-rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-2.1.0/src/alicechess/pictures/BQ.png
+-rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-2.1.0/src/alicechess/pictures/BR.png
+-rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-2.1.0/src/alicechess/pictures/WB.png
+-rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-2.1.0/src/alicechess/pictures/WK.png
+-rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-2.1.0/src/alicechess/pictures/WN.png
+-rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-2.1.0/src/alicechess/pictures/WP.png
+-rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-2.1.0/src/alicechess/pictures/WQ.png
+-rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-2.1.0/src/alicechess/pictures/WR.png
+-rw-r--r--   0        0        0     2129 2023-06-09 04:32:36.557471 alicechess-2.1.0/src/alicechess/pieces/__init__.py
+-rw-r--r--   0        0        0     2566 2023-06-09 04:32:19.713301 alicechess-2.1.0/src/alicechess/pieces/king.py
+-rw-r--r--   0        0        0     1396 2023-06-09 04:32:48.125403 alicechess-2.1.0/src/alicechess/pieces/pawn.py
+-rw-r--r--   0        0        0     8089 2023-06-09 04:32:57.403280 alicechess-2.1.0/src/alicechess/pieces/piece.py
+-rw-r--r--   0        0        0     2178 2023-06-09 04:37:41.423231 alicechess-2.1.0/src/alicechess/player.py
+-rw-r--r--   0        0        0    10036 2023-06-09 07:12:48.581884 alicechess-2.1.0/src/alicechess/position.py
+-rw-r--r--   0        0        0     2644 2023-06-09 04:26:49.101173 alicechess-2.1.0/src/alicechess/utils.py
+-rw-r--r--   0        0        0    24426 2023-06-09 17:41:56.223271 alicechess-2.1.0/src/alicechess/window.py
+-rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 alicechess-2.1.0/setup.py
+-rw-r--r--   0        0        0     5035 1970-01-01 00:00:00.000000 alicechess-2.1.0/PKG-INFO
```

### Comparing `alicechess-2.0.0/LICENSE` & `alicechess-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/README.md` & `alicechess-2.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -87,14 +87,38 @@
 
 The code is factored in a way to make it very easy for you to code your own bots
 to play against. Simply extend the `Player` class and implement the two abstract
 methods for making a move and promoting a pawn. This class (not an instance) can
 then be passed into the `Game` constructor to start a game. See the
 [API Documentation][docs] for more information.
 
+Here is an example:
+
+```python
+"""
+Plays a game between a human and a bot (that I wrote).
+"""
+
+from alicechess import Game, HumanPlayer, Player, PromoteType
+
+class Bot(Player):
+    """A very good bot that I wrote."""
+
+    def make_move(self, game_state):
+        for piece in game_state.yield_player_pieces():
+            for move in piece.yield_moves():
+                return move
+
+    def promote(self, game_state):
+        return PromoteType.QUEEN
+
+if __name__ == "__main__":
+    Game(white=HumanPlayer, black=Bot).start_window()
+```
+
 [docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md
 
 ## Credit
 
 Thank you to Artyom Lisitsyn for inspiring me to pursue this project and to
 Trung Phan for being my chess consultant and answering all my questions on rules
 and technicalities.
```

### Comparing `alicechess-2.0.0/pyproject.toml` & `alicechess-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 profile = "black"
 # Just setting the profile will use the `black` default line length of 88, so
 # need to override line length as well
 line_length = 79
 
 [tool.poetry]
 name = "alicechess"
-version = "2.0.0"
+version = "2.1.0"
 description = "A Python package to play Alice Chess"
 authors = ["Joseph Lou <joseph.d.lou@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/josephlou5/alicechess"
 repository = "https://github.com/josephlou5/alicechess"
 classifiers = [
```

### Comparing `alicechess-2.0.0/src/alicechess/_moves_calculator.py` & `alicechess-2.1.0/src/alicechess/_moves_calculator.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/bots.py` & `alicechess-2.1.0/src/alicechess/bots.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/game.py` & `alicechess-2.1.0/src/alicechess/game.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/game_state.py` & `alicechess-2.1.0/src/alicechess/game_state.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/BB.png` & `alicechess-2.1.0/src/alicechess/pictures/BB.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/BK.png` & `alicechess-2.1.0/src/alicechess/pictures/BK.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/BN.png` & `alicechess-2.1.0/src/alicechess/pictures/BN.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/BP.png` & `alicechess-2.1.0/src/alicechess/pictures/BP.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/BQ.png` & `alicechess-2.1.0/src/alicechess/pictures/BQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/BR.png` & `alicechess-2.1.0/src/alicechess/pictures/BR.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/WB.png` & `alicechess-2.1.0/src/alicechess/pictures/WB.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/WK.png` & `alicechess-2.1.0/src/alicechess/pictures/WK.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/WN.png` & `alicechess-2.1.0/src/alicechess/pictures/WN.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/WP.png` & `alicechess-2.1.0/src/alicechess/pictures/WP.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/WQ.png` & `alicechess-2.1.0/src/alicechess/pictures/WQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pictures/WR.png` & `alicechess-2.1.0/src/alicechess/pictures/WR.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pieces/__init__.py` & `alicechess-2.1.0/src/alicechess/pieces/__init__.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pieces/king.py` & `alicechess-2.1.0/src/alicechess/pieces/king.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pieces/pawn.py` & `alicechess-2.1.0/src/alicechess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/pieces/piece.py` & `alicechess-2.1.0/src/alicechess/pieces/piece.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/player.py` & `alicechess-2.1.0/src/alicechess/player.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/position.py` & `alicechess-2.1.0/src/alicechess/position.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,16 +67,21 @@
 
     @classmethod
     def of(cls, obj) -> Self:
         if obj is None:
             return None
         if isinstance(obj, cls):
             return obj
-        if isinstance(obj, (tuple, list)):
-            return cls(*obj)
+        try:
+            args = tuple(obj)
+        except TypeError:
+            pass
+        else:
+            # if iterable, use it as args
+            return cls(*args)
         raise TypeError(
             f"Cannot create {cls.__name__} from {obj.__class__.__name__}"
         )
 
     @classmethod
     def to_str(cls, iterable: Iterable[Self], sep: str = " ") -> str:
         """Returns the objs in the given iterable as a string."""
```

### Comparing `alicechess-2.0.0/src/alicechess/utils.py` & `alicechess-2.1.0/src/alicechess/utils.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.0.0/src/alicechess/window.py` & `alicechess-2.1.0/src/alicechess/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 Y_OFFSET_BOT = 180
 
 # Calculated dimensions of the entire window.
 WIDTH = X_OFFSET + SQUARE_SIZE * 8 + BOARD_PADDING + SQUARE_SIZE * 8 + X_OFFSET
 HALF_WIDTH = WIDTH / 2
 HEIGHT = Y_OFFSET + SQUARE_SIZE * 8 + Y_OFFSET_BOT
 
-RESET_BUTTON_COORDS = (10, 10, 70, 40)
-UNDO_BUTTON_COORDS = (WIDTH - 70, 10, WIDTH - 10, 40)
+BUTTON_PADDING = 5
+
 POSSIBLE_DOT_RADIUS = 5
 
 # Board colors
 WHITE_COLOR = "white"
 BLACK_COLOR = "gray"
 SELECT_COLOR = "green"
 POSSIBLE_COLOR = "blue"
@@ -69,14 +69,26 @@
 # Images
 PICTURE_FOLDER = Path(__file__).parent / "pictures"
 PICTURE_EXT = ".png"
 
 # =============================================================================
 
 
+def _button_width(font: _TkFont.Font, text: str) -> int:
+    return BUTTON_PADDING + font.measure(text) + BUTTON_PADDING
+
+
+def _button_middle(coords) -> Tuple[float, float]:
+    x1, y1, x2, y2 = coords
+    return (x1 + x2) / 2, (y1 + y2) / 2
+
+
+# =============================================================================
+
+
 def _black_on_button(game_state: GameState) -> bool:
     # black should only be on the bottom if white is not a human but
     # black is a human
     # otherwise, default to white on bottom
     return not game_state.white.is_human and game_state.black.is_human
 
 
@@ -257,15 +269,15 @@
         families = set(_TkFont.families())
         for font in FONTS:
             if font in families:
                 self._font = font
                 break
         font30 = (self._font, 30)
         font20 = (self._font, 20)
-        font15 = (self._font, 15)
+        self._font15 = _TkFont.Font(self._tk, (self._font, 15))
 
         self._canvas = canvas = _tk.Canvas(
             self._tk, width=WIDTH, height=HEIGHT
         )
         canvas.pack()
 
         # title
@@ -343,33 +355,56 @@
         self._hide("promotions")
 
         # state text
         self._state_text = canvas.create_text(
             HALF_WIDTH, bottom_y, font=font20
         )
 
+        def _create_button(coords, text, **kwargs):
+            tags_kwargs = {}
+            if "tags" in kwargs:
+                tags_kwargs["tags"] = kwargs["tags"]
+            button_id = canvas.create_rectangle(*coords, **tags_kwargs)
+            text_id = canvas.create_text(
+                *_button_middle(coords), text=text, **kwargs
+            )
+            return button_id, text_id
+
         # reset button
-        canvas.create_rectangle(*RESET_BUTTON_COORDS)
-        x1, y1, x2, y2 = RESET_BUTTON_COORDS
-        canvas.create_text(
-            (x1 + x2) / 2, (y1 + y2) / 2, text="Reset", font=font15
+        self._reset_button_coords = (
+            10,
+            10,
+            10 + _button_width(self._font15, "Reset"),
+            40,
         )
+        _create_button(self._reset_button_coords, "Reset")
 
         # undo button
-        canvas.create_rectangle(*UNDO_BUTTON_COORDS, tags=("undo",))
-        x1, y1, x2, y2 = UNDO_BUTTON_COORDS
-        canvas.create_text(
-            (x1 + x2) / 2,
-            (y1 + y2) / 2,
-            text="Undo",
-            font=font15,
-            tags=("undo",),
+        self._undo_button_coords = (
+            WIDTH - (10 + _button_width(self._font15, "Undo")),
+            10,
+            WIDTH - 10,
+            40,
         )
+        _create_button(self._undo_button_coords, "Undo", tags=("undo",))
         self._hide("undo")
 
+        # pause button
+        self._pause_button_coords = (
+            WIDTH - (10 + _button_width(self._font15, "Pause")),
+            10,
+            WIDTH - 10,
+            40,
+        )
+        self._pause_button, self._pause_text = _create_button(
+            self._pause_button_coords, "Pause", tags=("pause",)
+        )
+        self._hide("pause")
+        self._paused = False
+
         # for manually playing with human players
         self._last_move = None
         self._selected = None
         self._other_player_callback = None
 
     def _show(self, element, **kwargs):
         self._canvas.itemconfig(element, **kwargs, state="normal")
@@ -400,14 +435,19 @@
             square.reset()
 
         # reset other visual stuff
         self._hide("undo")
         self._hide("promotions")
         self._hide(self._state_text)
 
+        if self._has_human_player:
+            self._hide("pause")
+        else:
+            self._show("pause")
+
         # update piece images
         self._update_pieces()
 
     def _update_piece_image(
         self,
         piece: Piece,
         img_id: Optional[int] = None,
@@ -482,26 +522,30 @@
                 self._undo_state = grand_prev
 
     def _click(self, event: _tk.Event):
         """Handles a click event."""
         x, y = event.x, event.y
 
         # check reset button
-        if _within_coords(RESET_BUTTON_COORDS, x, y):
+        if _within_coords(self._reset_button_coords, x, y):
             self._reset()
             # initialize a non-human turn, if possible
             self._non_human_turn(True)
             return
 
         if not self._has_human_player:
-            # no other clicks to check for
+            # check pause button
+            if _within_coords(self._pause_button_coords, x, y):
+                self._pause_unpause()
+
+            # nothing else to check
             return
 
         # check undo button
-        if _within_coords(UNDO_BUTTON_COORDS, x, y):
+        if _within_coords(self._undo_button_coords, x, y):
             if self._undo_state is not None:
                 self._stop_non_human_player()
                 self._game = self._undo_state
                 self._update_pieces()
                 self._end_turn()
             return
 
@@ -591,17 +635,56 @@
                 self._squares[move.capture_pos].reset_possible()
             # show promotion images
             self._show(f"{self._selected.color.name.lower()}_promotions")
             return
 
         self._end_turn()
 
+    def _pause_unpause(self):
+        if self._game.is_game_over():
+            # do nothing
+            return
+
+        if self._paused:
+            # unpause
+            button_text = "Pause"
+            # initialize a non-human turn
+            self._non_human_turn()
+        else:
+            # pause
+            button_text = "Unpause"
+            # stop the current turn
+            self._stop_non_human_player()
+            # update the state text
+            if self._game.is_in_check():
+                state_text = f"{self._game.current_color.title()} is in check."
+                self._canvas.itemconfig(self._state_text, text=state_text)
+            else:
+                self._hide(self._state_text)
+
+        # update button text
+        self._pause_button_coords = (
+            WIDTH - (10 + _button_width(self._font15, button_text)),
+            10,
+            WIDTH - 10,
+            40,
+        )
+        self._canvas.coords(self._pause_button, self._pause_button_coords)
+        self._canvas.coords(
+            self._pause_text, _button_middle(self._pause_button_coords)
+        )
+        self._canvas.itemconfig(self._pause_text, text=button_text)
+
+        self._paused = not self._paused
+
     def _non_human_turn(self, first_move: bool = False):
         if self._game.current_player.is_human:
             return
+        if self._game.is_game_over():
+            return
 
         def make_turn():
             self._game = self._game.step()
             print("non-human player made move:", self._game.move)
             self._other_player_callback = None
             self._end_turn()
 
@@ -642,16 +725,16 @@
             self._squares[last_pos].last_move()
             self._last_move = last_pos
 
         game = self._game
         game.debug()
         # check for game over
         if game.is_game_over():
-            # no more undo
-            # self._hide("undo")
+            # no more pause
+            self._hide("pause")
             if game.is_in_checkmate():
                 text = f"Checkmate. {game.winner().title()} won!"
             elif game.is_in_stalemate():
                 text = "Stalemate."
             elif game.is_kings_draw():
                 text = "Draw."
             elif game.is_draw():
```

### Comparing `alicechess-2.0.0/setup.py` & `alicechess-2.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*'], 'alicechess': ['pictures/*']}
 
 install_requires = \
 ['Pillow>=9.5.0,<10.0.0']
 
 setup_kwargs = {
     'name': 'alicechess',
-    'version': '2.0.0',
+    'version': '2.1.0',
     'description': 'A Python package to play Alice Chess',
-    'long_description': '# Alice Chess\n\nThis project allows you to play Alice Chess, a variant of chess.\n\n## Installation\n\nThe package may be installed through `pip`:\n\n```bash\n$ pip install alicechess\n```\n\n## Rules\n\nHere is a [description of the concept and rules][rules].\n\n[rules]: https://www.chessvariants.com/other.dir/alice.html\n\nNotable game rules:\n\n- **Castling**: A king and rook may only castle if neither has moved already,\n  the king is not in check, all squares between them are vacant on both boards,\n  and the king does not move through check or into check. After the castle, both\n  pieces will teleport to the other board.\n- **En passant**: A pawn may capture another pawn through en passant if your\n  pawn is on board B and the enemy pawn advances two spaces, teleporting to the\n  space right next to yours on board B. (This results in a situation that looks\n  like regular en passant.) Note that due to teleporting to the other board\n  after each move, this can only be achieved by a pawn that _does not_ advance\n  two squares on its first move.\n- **Fifty move rule**: If both players have made 50 moves each where no piece\n  has been captured or no pawn moved, then a player may claim a draw. However,\n  to simplify this case, the game will be automatically ended with a draw\n  (rather than allowing a player to claim a draw), although this is not the\n  official rule. This therefore overshadows the 75-move rule, where a draw is\n  automatically applied after 75 moves by both players with no captures or pawn\n  movements.\n\n## How to play\n\nTo start a game between two human players, you can easily just run the package\non the command line:\n\n```bash\n$ python -m alicechess\n```\n\nA window will come up where the game can be played.\n\n## Playing against bots\n\nTo play a game against a bot or between bots, you must write your own script.\nYou should initialize a `Game` object with the appropriate players, then call\neither the `start()` or `start_window()` method. To write your own bot, see the\n[Writing a bot](#writing-a-bot) section.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot that plays randomly.\n"""\n\nfrom alicechess import Game, HumanPlayer\nfrom alicechess.bots import RandomPlayer\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=RandomPlayer).start_window()\n```\n\nNote that the class names (not instances) are passed to the `Game` constructor.\n\nThe `start_window()` method will, as implied, start an interactive window where\nthe game can be played. However, you can also opt to use the `start()` method\ninstead, which will return the first `GameState` of the game, and then use\nanother way to ask the user for input and play the game; for instance, you could\nmake the game entirely textual with user input provided with the keyboard. See\nthe [API Documentation][docs] for more information.\n\nIn the interactive window, there is a 3 second delay for non-human player moves,\nto simulate realism. This can be changed by passing a value for\n`non_human_player_delay` to the `start_window()` method.\n\nIt is also possible for two bots to play against each other.\n\n### Writing a bot\n\nThe code is factored in a way to make it very easy for you to code your own bots\nto play against. Simply extend the `Player` class and implement the two abstract\nmethods for making a move and promoting a pawn. This class (not an instance) can\nthen be passed into the `Game` constructor to start a game. See the\n[API Documentation][docs] for more information.\n\n[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md\n\n## Credit\n\nThank you to Artyom Lisitsyn for inspiring me to pursue this project and to\nTrung Phan for being my chess consultant and answering all my questions on rules\nand technicalities.\n',
+    'long_description': '# Alice Chess\n\nThis project allows you to play Alice Chess, a variant of chess.\n\n## Installation\n\nThe package may be installed through `pip`:\n\n```bash\n$ pip install alicechess\n```\n\n## Rules\n\nHere is a [description of the concept and rules][rules].\n\n[rules]: https://www.chessvariants.com/other.dir/alice.html\n\nNotable game rules:\n\n- **Castling**: A king and rook may only castle if neither has moved already,\n  the king is not in check, all squares between them are vacant on both boards,\n  and the king does not move through check or into check. After the castle, both\n  pieces will teleport to the other board.\n- **En passant**: A pawn may capture another pawn through en passant if your\n  pawn is on board B and the enemy pawn advances two spaces, teleporting to the\n  space right next to yours on board B. (This results in a situation that looks\n  like regular en passant.) Note that due to teleporting to the other board\n  after each move, this can only be achieved by a pawn that _does not_ advance\n  two squares on its first move.\n- **Fifty move rule**: If both players have made 50 moves each where no piece\n  has been captured or no pawn moved, then a player may claim a draw. However,\n  to simplify this case, the game will be automatically ended with a draw\n  (rather than allowing a player to claim a draw), although this is not the\n  official rule. This therefore overshadows the 75-move rule, where a draw is\n  automatically applied after 75 moves by both players with no captures or pawn\n  movements.\n\n## How to play\n\nTo start a game between two human players, you can easily just run the package\non the command line:\n\n```bash\n$ python -m alicechess\n```\n\nA window will come up where the game can be played.\n\n## Playing against bots\n\nTo play a game against a bot or between bots, you must write your own script.\nYou should initialize a `Game` object with the appropriate players, then call\neither the `start()` or `start_window()` method. To write your own bot, see the\n[Writing a bot](#writing-a-bot) section.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot that plays randomly.\n"""\n\nfrom alicechess import Game, HumanPlayer\nfrom alicechess.bots import RandomPlayer\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=RandomPlayer).start_window()\n```\n\nNote that the class names (not instances) are passed to the `Game` constructor.\n\nThe `start_window()` method will, as implied, start an interactive window where\nthe game can be played. However, you can also opt to use the `start()` method\ninstead, which will return the first `GameState` of the game, and then use\nanother way to ask the user for input and play the game; for instance, you could\nmake the game entirely textual with user input provided with the keyboard. See\nthe [API Documentation][docs] for more information.\n\nIn the interactive window, there is a 3 second delay for non-human player moves,\nto simulate realism. This can be changed by passing a value for\n`non_human_player_delay` to the `start_window()` method.\n\nIt is also possible for two bots to play against each other.\n\n### Writing a bot\n\nThe code is factored in a way to make it very easy for you to code your own bots\nto play against. Simply extend the `Player` class and implement the two abstract\nmethods for making a move and promoting a pawn. This class (not an instance) can\nthen be passed into the `Game` constructor to start a game. See the\n[API Documentation][docs] for more information.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot (that I wrote).\n"""\n\nfrom alicechess import Game, HumanPlayer, Player, PromoteType\n\nclass Bot(Player):\n    """A very good bot that I wrote."""\n\n    def make_move(self, game_state):\n        for piece in game_state.yield_player_pieces():\n            for move in piece.yield_moves():\n                return move\n\n    def promote(self, game_state):\n        return PromoteType.QUEEN\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=Bot).start_window()\n```\n\n[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md\n\n## Credit\n\nThank you to Artyom Lisitsyn for inspiring me to pursue this project and to\nTrung Phan for being my chess consultant and answering all my questions on rules\nand technicalities.\n',
     'author': 'Joseph Lou',
     'author_email': 'joseph.d.lou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josephlou5/alicechess',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `alicechess-2.0.0/PKG-INFO` & `alicechess-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicechess
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Python package to play Alice Chess
 Home-page: https://github.com/josephlou5/alicechess
 License: MIT
 Author: Joseph Lou
 Author-email: joseph.d.lou@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -107,14 +107,38 @@
 
 The code is factored in a way to make it very easy for you to code your own bots
 to play against. Simply extend the `Player` class and implement the two abstract
 methods for making a move and promoting a pawn. This class (not an instance) can
 then be passed into the `Game` constructor to start a game. See the
 [API Documentation][docs] for more information.
 
+Here is an example:
+
+```python
+"""
+Plays a game between a human and a bot (that I wrote).
+"""
+
+from alicechess import Game, HumanPlayer, Player, PromoteType
+
+class Bot(Player):
+    """A very good bot that I wrote."""
+
+    def make_move(self, game_state):
+        for piece in game_state.yield_player_pieces():
+            for move in piece.yield_moves():
+                return move
+
+    def promote(self, game_state):
+        return PromoteType.QUEEN
+
+if __name__ == "__main__":
+    Game(white=HumanPlayer, black=Bot).start_window()
+```
+
 [docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md
 
 ## Credit
 
 Thank you to Artyom Lisitsyn for inspiring me to pursue this project and to
 Trung Phan for being my chess consultant and answering all my questions on rules
 and technicalities.
```

