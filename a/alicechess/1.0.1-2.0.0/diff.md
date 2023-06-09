# Comparing `tmp/alicechess-1.0.1.tar.gz` & `tmp/alicechess-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicechess-1.0.1.tar", max compression
+gzip compressed data, was "alicechess-2.0.0.tar", max compression
```

## Comparing `alicechess-1.0.1.tar` & `alicechess-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-1.0.1/LICENSE
--rw-r--r--   0        0        0     4076 2023-06-09 04:14:15.807338 alicechess-1.0.1/README.md
--rw-r--r--   0        0        0     1042 2023-06-09 04:14:27.253727 alicechess-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      164 2023-06-09 04:07:30.904920 alicechess-1.0.1/src/alicechess/__init__.py
--rw-r--r--   0        0        0      388 2023-06-07 21:32:17.245811 alicechess-1.0.1/src/alicechess/__main__.py
--rw-r--r--   0        0        0       65 2023-06-09 04:13:56.560979 alicechess-1.0.1/src/alicechess/__version__.py
--rw-r--r--   0        0        0     3329 2023-06-07 21:31:30.165561 alicechess-1.0.1/src/alicechess/bots.py
--rw-r--r--   0        0        0     1808 2023-06-09 00:07:47.640400 alicechess-1.0.1/src/alicechess/game.py
--rw-r--r--   0        0        0    36219 2023-06-07 21:30:47.973855 alicechess-1.0.1/src/alicechess/game_state.py
--rw-r--r--   0        0        0    15232 2023-06-07 15:42:54.161860 alicechess-1.0.1/src/alicechess/moves_calculator.py
--rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-1.0.1/src/alicechess/pictures/BB.png
--rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-1.0.1/src/alicechess/pictures/BK.png
--rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-1.0.1/src/alicechess/pictures/BN.png
--rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-1.0.1/src/alicechess/pictures/BP.png
--rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-1.0.1/src/alicechess/pictures/BQ.png
--rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-1.0.1/src/alicechess/pictures/BR.png
--rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-1.0.1/src/alicechess/pictures/WB.png
--rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-1.0.1/src/alicechess/pictures/WK.png
--rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-1.0.1/src/alicechess/pictures/WN.png
--rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-1.0.1/src/alicechess/pictures/WP.png
--rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-1.0.1/src/alicechess/pictures/WQ.png
--rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-1.0.1/src/alicechess/pictures/WR.png
--rw-r--r--   0        0        0     2152 2023-06-03 13:02:01.873732 alicechess-1.0.1/src/alicechess/pieces/__init__.py
--rw-r--r--   0        0        0     2539 2023-06-03 13:02:40.681380 alicechess-1.0.1/src/alicechess/pieces/king.py
--rw-r--r--   0        0        0     1369 2023-06-04 02:35:41.836367 alicechess-1.0.1/src/alicechess/pieces/pawn.py
--rw-r--r--   0        0        0     8067 2023-06-07 21:17:23.344370 alicechess-1.0.1/src/alicechess/pieces/piece.py
--rw-r--r--   0        0        0     2171 2023-05-27 03:42:56.855167 alicechess-1.0.1/src/alicechess/player.py
--rw-r--r--   0        0        0     9925 2023-06-04 00:33:15.176040 alicechess-1.0.1/src/alicechess/position.py
--rw-r--r--   0        0        0      376 2023-06-07 21:30:52.032950 alicechess-1.0.1/src/alicechess/test.py
--rw-r--r--   0        0        0     2644 2023-06-07 21:21:10.031159 alicechess-1.0.1/src/alicechess/utils.py
--rw-r--r--   0        0        0    21708 2023-06-07 21:31:05.844394 alicechess-1.0.1/src/alicechess/window.py
--rw-r--r--   0        0        0     4963 1970-01-01 00:00:00.000000 alicechess-1.0.1/setup.py
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 alicechess-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3740 2023-06-09 04:29:05.322145 alicechess-2.0.0/README.md
+-rw-r--r--   0        0        0     1042 2023-06-09 04:40:57.176153 alicechess-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-06-09 04:36:24.042041 alicechess-2.0.0/src/alicechess/__init__.py
+-rw-r--r--   0        0        0      410 2023-06-09 04:36:08.864143 alicechess-2.0.0/src/alicechess/__main__.py
+-rw-r--r--   0        0        0       65 2023-06-09 04:40:41.830358 alicechess-2.0.0/src/alicechess/__version__.py
+-rw-r--r--   0        0        0    15265 2023-06-09 04:36:45.923112 alicechess-2.0.0/src/alicechess/_moves_calculator.py
+-rw-r--r--   0        0        0     3520 2023-06-09 04:37:00.369033 alicechess-2.0.0/src/alicechess/bots.py
+-rw-r--r--   0        0        0     1950 2023-06-09 04:38:27.983773 alicechess-2.0.0/src/alicechess/game.py
+-rw-r--r--   0        0        0    36291 2023-06-09 04:37:28.559970 alicechess-2.0.0/src/alicechess/game_state.py
+-rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-2.0.0/src/alicechess/pictures/BB.png
+-rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-2.0.0/src/alicechess/pictures/BK.png
+-rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-2.0.0/src/alicechess/pictures/BN.png
+-rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-2.0.0/src/alicechess/pictures/BP.png
+-rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-2.0.0/src/alicechess/pictures/BQ.png
+-rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-2.0.0/src/alicechess/pictures/BR.png
+-rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-2.0.0/src/alicechess/pictures/WB.png
+-rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-2.0.0/src/alicechess/pictures/WK.png
+-rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-2.0.0/src/alicechess/pictures/WN.png
+-rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-2.0.0/src/alicechess/pictures/WP.png
+-rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-2.0.0/src/alicechess/pictures/WQ.png
+-rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-2.0.0/src/alicechess/pictures/WR.png
+-rw-r--r--   0        0        0     2129 2023-06-09 04:32:36.557471 alicechess-2.0.0/src/alicechess/pieces/__init__.py
+-rw-r--r--   0        0        0     2566 2023-06-09 04:32:19.713301 alicechess-2.0.0/src/alicechess/pieces/king.py
+-rw-r--r--   0        0        0     1396 2023-06-09 04:32:48.125403 alicechess-2.0.0/src/alicechess/pieces/pawn.py
+-rw-r--r--   0        0        0     8089 2023-06-09 04:32:57.403280 alicechess-2.0.0/src/alicechess/pieces/piece.py
+-rw-r--r--   0        0        0     2178 2023-06-09 04:37:41.423231 alicechess-2.0.0/src/alicechess/player.py
+-rw-r--r--   0        0        0     9936 2023-06-09 04:37:46.484148 alicechess-2.0.0/src/alicechess/position.py
+-rw-r--r--   0        0        0     2644 2023-06-09 04:26:49.101173 alicechess-2.0.0/src/alicechess/utils.py
+-rw-r--r--   0        0        0    21874 2023-06-09 04:39:18.703016 alicechess-2.0.0/src/alicechess/window.py
+-rw-r--r--   0        0        0     4620 1970-01-01 00:00:00.000000 alicechess-2.0.0/setup.py
+-rw-r--r--   0        0        0     4496 1970-01-01 00:00:00.000000 alicechess-2.0.0/PKG-INFO
```

### Comparing `alicechess-1.0.1/LICENSE` & `alicechess-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/README.md` & `alicechess-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Alice Chess
 
 This project allows you to play Alice Chess, a variant of chess.
 
-## Installastion
+## Installation
 
 The package may be installed through `pip`:
 
 ```bash
 $ pip install alicechess
 ```
 
@@ -87,21 +87,14 @@
 
 The code is factored in a way to make it very easy for you to code your own bots
 to play against. Simply extend the `Player` class and implement the two abstract
 methods for making a move and promoting a pawn. This class (not an instance) can
 then be passed into the `Game` constructor to start a game. See the
 [API Documentation][docs] for more information.
 
-## Advanced Usage
-
-The only dependency for this project is `Pillow` to use the images in the
-interactive window. As such, you could technically clone the repository and run
-it without the window with only the Python builtins. Not sure why you would want
-to do that, but that is another alternative option to installing through `pip`.
+[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md
 
 ## Credit
 
 Thank you to Artyom Lisitsyn for inspiring me to pursue this project and to
 Trung Phan for being my chess consultant and answering all my questions on rules
 and technicalities.
-
-[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md
```

### Comparing `alicechess-1.0.1/pyproject.toml` & `alicechess-2.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 profile = "black"
 # Just setting the profile will use the `black` default line length of 88, so
 # need to override line length as well
 line_length = 79
 
 [tool.poetry]
 name = "alicechess"
-version = "1.0.1"
+version = "2.0.0"
 description = "A Python package to play Alice Chess"
 authors = ["Joseph Lou <joseph.d.lou@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/josephlou5/alicechess"
 repository = "https://github.com/josephlou5/alicechess"
 classifiers = [
```

### Comparing `alicechess-1.0.1/src/alicechess/bots.py` & `alicechess-2.0.0/src/alicechess/bots.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,25 @@
 """
 
 # =============================================================================
 
 import random
 from typing import Dict
 
-from game_state import GameState
-from player import Player
-from position import Move
-from utils import PieceType, PromoteType
+from alicechess.game_state import GameState
+from alicechess.player import Player
+from alicechess.position import Move
+from alicechess.utils import PieceType, PromoteType
+
+# =============================================================================
+
+__all__ = (
+    "RandomPlayer",
+    "PrioritizedRandomPlayer",
+)
 
 # =============================================================================
 
 
 class RandomPlayer(Player):
     """A bot that picks a random move to make."""
```

### Comparing `alicechess-1.0.1/src/alicechess/game.py` & `alicechess-2.0.0/src/alicechess/game.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 Game class.
 """
 
 # =============================================================================
 
 from typing import Type
 
-from game_state import GameState
-from player import AnyPlayer, _PlayerBase
+from alicechess.game_state import GameState
+from alicechess.player import AnyPlayer, _PlayerBase
+
+# =============================================================================
+
+__all__ = ("Game",)
 
 # =============================================================================
 
 
 class Game:
     """Represents a game of Alice Chess."""
 
@@ -45,12 +49,13 @@
         """Starts the game in a window.
 
         Any keyword arguments will be passed to the `Window`
         constructor.
         """
         # import here so that games that don't use the window don't need
         # to be run in a virtual environment (requires Pillow)
-        from window import Window  # pylint: disable=import-outside-toplevel
+        # pylint: disable=import-outside-toplevel
+        from alicechess.window import Window
 
         game_state = self.new()
         window = Window(game_state, **kwargs)
         window.run()
```

### Comparing `alicechess-1.0.1/src/alicechess/game_state.py` & `alicechess-2.0.0/src/alicechess/game_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 # =============================================================================
 
 import math
 from itertools import count, zip_longest
 from typing import Dict, Iterable, Iterator, Optional, Self, Type
 
-import pieces
-from moves_calculator import BoardDict, MovesCalculator
-from pieces import Piece, make_promoted
-from player import AnyPlayer
-from position import Move, PieceMove, PieceMoved, Position
-from utils import Color, EndGameState, PieceType, PromoteType
+from alicechess import pieces
+from alicechess._moves_calculator import BoardDict, MovesCalculator
+from alicechess.pieces import Piece, make_promoted
+from alicechess.player import AnyPlayer
+from alicechess.position import Move, PieceMove, PieceMoved, Position
+from alicechess.utils import Color, EndGameState, PieceType, PromoteType
 
 # =============================================================================
 
 __all__ = ("GameState",)
 
 # =============================================================================
```

### Comparing `alicechess-1.0.1/src/alicechess/moves_calculator.py` & `alicechess-2.0.0/src/alicechess/_moves_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 # =============================================================================
 
 from functools import partial
 from typing import Dict, Iterator, List, Optional, Sequence, Tuple
 
-from pieces import King, Pawn, Piece, Rook
-from position import BoardPosition, Position
-from utils import Color, PieceType, check_brc, check_brc_bool
+from alicechess.pieces import King, Pawn, Piece, Rook
+from alicechess.position import BoardPosition, Position
+from alicechess.utils import Color, PieceType, check_brc, check_brc_bool
 
 # =============================================================================
 
 BoardDict = Dict[BoardPosition, Piece]
 
 # =============================================================================
```

### Comparing `alicechess-1.0.1/src/alicechess/pictures/BB.png` & `alicechess-2.0.0/src/alicechess/pictures/BB.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/BK.png` & `alicechess-2.0.0/src/alicechess/pictures/BK.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/BN.png` & `alicechess-2.0.0/src/alicechess/pictures/BN.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/BP.png` & `alicechess-2.0.0/src/alicechess/pictures/BP.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/BQ.png` & `alicechess-2.0.0/src/alicechess/pictures/BQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/BR.png` & `alicechess-2.0.0/src/alicechess/pictures/BR.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/WB.png` & `alicechess-2.0.0/src/alicechess/pictures/WB.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/WK.png` & `alicechess-2.0.0/src/alicechess/pictures/WK.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/WN.png` & `alicechess-2.0.0/src/alicechess/pictures/WN.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/WP.png` & `alicechess-2.0.0/src/alicechess/pictures/WP.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/WQ.png` & `alicechess-2.0.0/src/alicechess/pictures/WQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pictures/WR.png` & `alicechess-2.0.0/src/alicechess/pictures/WR.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/pieces/__init__.py` & `alicechess-2.0.0/src/alicechess/pieces/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 Pieces submodule.
 """
 
 # =============================================================================
 
 import typing as _t
 
-from utils import Color as _Color
-from utils import PieceType as _PieceType
-from utils import PromoteType as _PromoteType
-
-from .king import King
-from .pawn import Pawn
-from .piece import Piece
+from alicechess.pieces.king import King
+from alicechess.pieces.pawn import Pawn
+from alicechess.pieces.piece import Piece
+from alicechess.utils import Color, PieceType, PromoteType
 
 # =============================================================================
 
 __all__ = (
     "Piece",
     "King",
     "Queen",
@@ -36,15 +33,15 @@
 
     class Subclass(Piece):
         _type = piece_type
 
         def _check_start_position(self) -> bool:
             if self._pos.bn != 0:
                 return False
-            if self._color is _Color.WHITE:
+            if self._color is Color.WHITE:
                 row = rows[0]
             else:
                 row = rows[1]
             if self._pos.r != row:
                 return False
             if columns is not None and self._pos.c not in columns:
                 return False
@@ -54,27 +51,27 @@
     Subclass.__name__ = piece_name
     Subclass.__doc__ = f"{piece_name} piece."
 
     return Subclass
 
 
 # queen is always on the left for this particular board setup
-Queen = _make_simple_piece(_PieceType.QUEEN, (7, 0), (3,))
-Rook = _make_simple_piece(_PieceType.ROOK, (7, 0), (0, 7))
-Knight = _make_simple_piece(_PieceType.KNIGHT, (7, 0), (1, 6))
-Bishop = _make_simple_piece(_PieceType.BISHOP, (7, 0), (2, 5))
+Queen = _make_simple_piece(PieceType.QUEEN, (7, 0), (3,))
+Rook = _make_simple_piece(PieceType.ROOK, (7, 0), (0, 7))
+Knight = _make_simple_piece(PieceType.KNIGHT, (7, 0), (1, 6))
+Bishop = _make_simple_piece(PieceType.BISHOP, (7, 0), (2, 5))
 
 # =============================================================================
 
 
 def make_promoted(
-    pawn: Pawn, promote_type: _PromoteType
+    pawn: Pawn, promote_type: PromoteType
 ) -> _t.Union[Queen, Rook, Knight, Bishop]:
     PROMOTE_CLASSES = {
-        _PromoteType.QUEEN: Queen,
-        _PromoteType.ROOK: Rook,
-        _PromoteType.KNIGHT: Knight,
-        _PromoteType.BISHOP: Bishop,
+        PromoteType.QUEEN: Queen,
+        PromoteType.ROOK: Rook,
+        PromoteType.KNIGHT: Knight,
+        PromoteType.BISHOP: Bishop,
     }
     return PROMOTE_CLASSES[promote_type](
         pawn.id, pawn.color, pawn.pos, has_moved=pawn.has_moved
     )
```

### Comparing `alicechess-1.0.1/src/alicechess/pieces/king.py` & `alicechess-2.0.0/src/alicechess/pieces/king.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 King piece.
 """
 
 # =============================================================================
 
-from utils import Color, PieceType
-
-from .piece import Piece
+from alicechess.pieces.piece import Piece
+from alicechess.utils import Color, PieceType
 
 # =============================================================================
 
 
 class King(Piece):
     """King piece.
```

### Comparing `alicechess-1.0.1/src/alicechess/pieces/pawn.py` & `alicechess-2.0.0/src/alicechess/pieces/pawn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 Pawn piece.
 """
 
 # =============================================================================
 
-from utils import Color, PieceType
-
-from .piece import Piece
+from alicechess.pieces.piece import Piece
+from alicechess.utils import Color, PieceType
 
 # =============================================================================
 
 
 class Pawn(Piece):
     """Pawn piece.
```

### Comparing `alicechess-1.0.1/src/alicechess/pieces/piece.py` & `alicechess-2.0.0/src/alicechess/pieces/piece.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Piece abstract class.
 """
 
 # =============================================================================
 
 from typing import Iterator, Optional, Set
 
-from position import BoardPosition, PieceMove, Position
-from utils import Color, PieceType, check_brc
+from alicechess.position import BoardPosition, PieceMove, Position
+from alicechess.utils import Color, PieceType, check_brc
 
 # =============================================================================
 
 __all__ = ("Piece",)
 
 # =============================================================================
```

### Comparing `alicechess-1.0.1/src/alicechess/player.py` & `alicechess-2.0.0/src/alicechess/player.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Player class.
 """
 
 # =============================================================================
 
-import typing as _t
+from typing import Union
 
-import utils as _utils
-from position import Move as _Move
+from alicechess.position import Move
+from alicechess.utils import Color, PromoteType
 
 # =============================================================================
 
 __all__ = (
     "Player",
     "HumanPlayer",
 )
@@ -20,20 +20,20 @@
 
 
 class _PlayerBase:
     """Base class for a player.."""
 
     is_human = False
 
-    def __init__(self, color: _utils.Color):
+    def __init__(self, color: Color):
         """Initializes a player."""
         self._color = color
 
     @property
-    def color(self) -> _utils.Color:
+    def color(self) -> Color:
         """The player color."""
         return self._color
 
 
 class Player(_PlayerBase):
     """Represents a player.
 
@@ -44,28 +44,28 @@
     Methods:
         make_move(game_state) -> Move
             Called when this player should make their next move.
         promote(game_state) -> PromoteType
             Called when this player can promote a pawn.
     """
 
-    def make_move(self, game_state: "GameState") -> _Move:
+    def make_move(self, game_state: "GameState") -> Move:
         """Called when this player should make their next move.
 
         Args:
             game_state (GameState): The current game state.
 
         Returns:
             Move: The move to make.
         """
         raise NotImplementedError(
             f"{self.__class__.__name__}: method `make_move()` not implemented"
         )
 
-    def promote(self, game_state: "GameState") -> _utils.PromoteType:
+    def promote(self, game_state: "GameState") -> PromoteType:
         """Called when this player can promote a pawn.
 
         The move being made is accessible through `game_state.move`.
 
         Args:
             game_state (GameState): The current game state.
 
@@ -81,8 +81,8 @@
     """Represents a human player."""
 
     is_human = True
 
 
 # =============================================================================
 
-AnyPlayer = _t.Union[Player, HumanPlayer]
+AnyPlayer = Union[Player, HumanPlayer]
```

### Comparing `alicechess-1.0.1/src/alicechess/position.py` & `alicechess-2.0.0/src/alicechess/position.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # =============================================================================
 
 from functools import total_ordering
 from typing import Iterable, Optional, Self, Tuple
 
-from utils import check_brc
+from alicechess.utils import check_brc
 
 # =============================================================================
 
 __all__ = (
     "Position",
     "BoardPosition",
     "Move",
```

### Comparing `alicechess-1.0.1/src/alicechess/utils.py` & `alicechess-2.0.0/src/alicechess/utils.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.1/src/alicechess/window.py` & `alicechess-2.0.0/src/alicechess/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,22 @@
         """\
 Pillow must be installed to run a game in a window:
 
   $ python -m pip install Pillow
 """
     ) from ex
 
-from game_state import GameState
-from pieces import Piece
-from position import BoardPosition, Position
-from utils import Color, PieceType, PromoteType, check_brc_bool
+from alicechess.game_state import GameState
+from alicechess.pieces import Piece
+from alicechess.position import BoardPosition, Position
+from alicechess.utils import Color, PieceType, PromoteType, check_brc_bool
+
+# =============================================================================
+
+__all__ = ("Window",)
 
 # =============================================================================
 
 # The size of a square cell.
 SQUARE_SIZE = 70
 HALF_SQUARE_SIZE = SQUARE_SIZE / 2
 # The padding between the two boards.
@@ -59,15 +63,15 @@
 POSSIBLE_COLOR = "blue"
 LAST_MOVE_COLOR = "#" + "".join(f"{x:02x}" for x in (102, 255, 178))
 
 # The fonts to use.
 FONTS = ("SF Pro",)
 
 # Images
-PICTURE_FOLDER = Path("pictures")
+PICTURE_FOLDER = Path(__file__).parent / "pictures"
 PICTURE_EXT = ".png"
 
 # =============================================================================
 
 
 def _black_on_button(game_state: GameState) -> bool:
     # black should only be on the bottom if white is not a human but
```

### Comparing `alicechess-1.0.1/setup.py` & `alicechess-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*'], 'alicechess': ['pictures/*']}
 
 install_requires = \
 ['Pillow>=9.5.0,<10.0.0']
 
 setup_kwargs = {
     'name': 'alicechess',
-    'version': '1.0.1',
+    'version': '2.0.0',
     'description': 'A Python package to play Alice Chess',
-    'long_description': '# Alice Chess\n\nThis project allows you to play Alice Chess, a variant of chess.\n\n## Installastion\n\nThe package may be installed through `pip`:\n\n```bash\n$ pip install alicechess\n```\n\n## Rules\n\nHere is a [description of the concept and rules][rules].\n\n[rules]: https://www.chessvariants.com/other.dir/alice.html\n\nNotable game rules:\n\n- **Castling**: A king and rook may only castle if neither has moved already,\n  the king is not in check, all squares between them are vacant on both boards,\n  and the king does not move through check or into check. After the castle, both\n  pieces will teleport to the other board.\n- **En passant**: A pawn may capture another pawn through en passant if your\n  pawn is on board B and the enemy pawn advances two spaces, teleporting to the\n  space right next to yours on board B. (This results in a situation that looks\n  like regular en passant.) Note that due to teleporting to the other board\n  after each move, this can only be achieved by a pawn that _does not_ advance\n  two squares on its first move.\n- **Fifty move rule**: If both players have made 50 moves each where no piece\n  has been captured or no pawn moved, then a player may claim a draw. However,\n  to simplify this case, the game will be automatically ended with a draw\n  (rather than allowing a player to claim a draw), although this is not the\n  official rule. This therefore overshadows the 75-move rule, where a draw is\n  automatically applied after 75 moves by both players with no captures or pawn\n  movements.\n\n## How to play\n\nTo start a game between two human players, you can easily just run the package\non the command line:\n\n```bash\n$ python -m alicechess\n```\n\nA window will come up where the game can be played.\n\n## Playing against bots\n\nTo play a game against a bot or between bots, you must write your own script.\nYou should initialize a `Game` object with the appropriate players, then call\neither the `start()` or `start_window()` method. To write your own bot, see the\n[Writing a bot](#writing-a-bot) section.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot that plays randomly.\n"""\n\nfrom alicechess import Game, HumanPlayer\nfrom alicechess.bots import RandomPlayer\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=RandomPlayer).start_window()\n```\n\nNote that the class names (not instances) are passed to the `Game` constructor.\n\nThe `start_window()` method will, as implied, start an interactive window where\nthe game can be played. However, you can also opt to use the `start()` method\ninstead, which will return the first `GameState` of the game, and then use\nanother way to ask the user for input and play the game; for instance, you could\nmake the game entirely textual with user input provided with the keyboard. See\nthe [API Documentation][docs] for more information.\n\nIn the interactive window, there is a 3 second delay for non-human player moves,\nto simulate realism. This can be changed by passing a value for\n`non_human_player_delay` to the `start_window()` method.\n\nIt is also possible for two bots to play against each other.\n\n### Writing a bot\n\nThe code is factored in a way to make it very easy for you to code your own bots\nto play against. Simply extend the `Player` class and implement the two abstract\nmethods for making a move and promoting a pawn. This class (not an instance) can\nthen be passed into the `Game` constructor to start a game. See the\n[API Documentation][docs] for more information.\n\n## Advanced Usage\n\nThe only dependency for this project is `Pillow` to use the images in the\ninteractive window. As such, you could technically clone the repository and run\nit without the window with only the Python builtins. Not sure why you would want\nto do that, but that is another alternative option to installing through `pip`.\n\n## Credit\n\nThank you to Artyom Lisitsyn for inspiring me to pursue this project and to\nTrung Phan for being my chess consultant and answering all my questions on rules\nand technicalities.\n\n[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md\n',
+    'long_description': '# Alice Chess\n\nThis project allows you to play Alice Chess, a variant of chess.\n\n## Installation\n\nThe package may be installed through `pip`:\n\n```bash\n$ pip install alicechess\n```\n\n## Rules\n\nHere is a [description of the concept and rules][rules].\n\n[rules]: https://www.chessvariants.com/other.dir/alice.html\n\nNotable game rules:\n\n- **Castling**: A king and rook may only castle if neither has moved already,\n  the king is not in check, all squares between them are vacant on both boards,\n  and the king does not move through check or into check. After the castle, both\n  pieces will teleport to the other board.\n- **En passant**: A pawn may capture another pawn through en passant if your\n  pawn is on board B and the enemy pawn advances two spaces, teleporting to the\n  space right next to yours on board B. (This results in a situation that looks\n  like regular en passant.) Note that due to teleporting to the other board\n  after each move, this can only be achieved by a pawn that _does not_ advance\n  two squares on its first move.\n- **Fifty move rule**: If both players have made 50 moves each where no piece\n  has been captured or no pawn moved, then a player may claim a draw. However,\n  to simplify this case, the game will be automatically ended with a draw\n  (rather than allowing a player to claim a draw), although this is not the\n  official rule. This therefore overshadows the 75-move rule, where a draw is\n  automatically applied after 75 moves by both players with no captures or pawn\n  movements.\n\n## How to play\n\nTo start a game between two human players, you can easily just run the package\non the command line:\n\n```bash\n$ python -m alicechess\n```\n\nA window will come up where the game can be played.\n\n## Playing against bots\n\nTo play a game against a bot or between bots, you must write your own script.\nYou should initialize a `Game` object with the appropriate players, then call\neither the `start()` or `start_window()` method. To write your own bot, see the\n[Writing a bot](#writing-a-bot) section.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot that plays randomly.\n"""\n\nfrom alicechess import Game, HumanPlayer\nfrom alicechess.bots import RandomPlayer\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=RandomPlayer).start_window()\n```\n\nNote that the class names (not instances) are passed to the `Game` constructor.\n\nThe `start_window()` method will, as implied, start an interactive window where\nthe game can be played. However, you can also opt to use the `start()` method\ninstead, which will return the first `GameState` of the game, and then use\nanother way to ask the user for input and play the game; for instance, you could\nmake the game entirely textual with user input provided with the keyboard. See\nthe [API Documentation][docs] for more information.\n\nIn the interactive window, there is a 3 second delay for non-human player moves,\nto simulate realism. This can be changed by passing a value for\n`non_human_player_delay` to the `start_window()` method.\n\nIt is also possible for two bots to play against each other.\n\n### Writing a bot\n\nThe code is factored in a way to make it very easy for you to code your own bots\nto play against. Simply extend the `Player` class and implement the two abstract\nmethods for making a move and promoting a pawn. This class (not an instance) can\nthen be passed into the `Game` constructor to start a game. See the\n[API Documentation][docs] for more information.\n\n[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md\n\n## Credit\n\nThank you to Artyom Lisitsyn for inspiring me to pursue this project and to\nTrung Phan for being my chess consultant and answering all my questions on rules\nand technicalities.\n',
     'author': 'Joseph Lou',
     'author_email': 'joseph.d.lou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josephlou5/alicechess',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `alicechess-1.0.1/PKG-INFO` & `alicechess-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicechess
-Version: 1.0.1
+Version: 2.0.0
 Summary: A Python package to play Alice Chess
 Home-page: https://github.com/josephlou5/alicechess
 License: MIT
 Author: Joseph Lou
 Author-email: joseph.d.lou@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Project-URL: Repository, https://github.com/josephlou5/alicechess
 Description-Content-Type: text/markdown
 
 # Alice Chess
 
 This project allows you to play Alice Chess, a variant of chess.
 
-## Installastion
+## Installation
 
 The package may be installed through `pip`:
 
 ```bash
 $ pip install alicechess
 ```
 
@@ -107,22 +107,15 @@
 
 The code is factored in a way to make it very easy for you to code your own bots
 to play against. Simply extend the `Player` class and implement the two abstract
 methods for making a move and promoting a pawn. This class (not an instance) can
 then be passed into the `Game` constructor to start a game. See the
 [API Documentation][docs] for more information.
 
-## Advanced Usage
-
-The only dependency for this project is `Pillow` to use the images in the
-interactive window. As such, you could technically clone the repository and run
-it without the window with only the Python builtins. Not sure why you would want
-to do that, but that is another alternative option to installing through `pip`.
+[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md
 
 ## Credit
 
 Thank you to Artyom Lisitsyn for inspiring me to pursue this project and to
 Trung Phan for being my chess consultant and answering all my questions on rules
 and technicalities.
 
-[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md
-
```

