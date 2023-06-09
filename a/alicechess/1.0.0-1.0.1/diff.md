# Comparing `tmp/alicechess-1.0.0.tar.gz` & `tmp/alicechess-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicechess-1.0.0.tar", max compression
+gzip compressed data, was "alicechess-1.0.1.tar", max compression
```

## Comparing `alicechess-1.0.0.tar` & `alicechess-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-1.0.0/LICENSE
--rw-r--r--   0        0        0     4066 2023-06-09 03:49:05.608049 alicechess-1.0.0/README.md
--rw-r--r--   0        0        0     1042 2023-06-09 04:04:00.998758 alicechess-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      164 2023-06-09 04:00:12.882743 alicechess-1.0.0/src/alicechess/__init__.py
--rw-r--r--   0        0        0      388 2023-06-07 21:32:17.245811 alicechess-1.0.0/src/alicechess/__main__.py
--rw-r--r--   0        0        0     3329 2023-06-07 21:31:30.165561 alicechess-1.0.0/src/alicechess/bots.py
--rw-r--r--   0        0        0     1808 2023-06-09 00:07:47.640400 alicechess-1.0.0/src/alicechess/game.py
--rw-r--r--   0        0        0    36219 2023-06-07 21:30:47.973855 alicechess-1.0.0/src/alicechess/game_state.py
--rw-r--r--   0        0        0    15232 2023-06-07 15:42:54.161860 alicechess-1.0.0/src/alicechess/moves_calculator.py
--rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-1.0.0/src/alicechess/pictures/BB.png
--rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-1.0.0/src/alicechess/pictures/BK.png
--rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-1.0.0/src/alicechess/pictures/BN.png
--rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-1.0.0/src/alicechess/pictures/BP.png
--rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-1.0.0/src/alicechess/pictures/BQ.png
--rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-1.0.0/src/alicechess/pictures/BR.png
--rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-1.0.0/src/alicechess/pictures/WB.png
--rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-1.0.0/src/alicechess/pictures/WK.png
--rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-1.0.0/src/alicechess/pictures/WN.png
--rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-1.0.0/src/alicechess/pictures/WP.png
--rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-1.0.0/src/alicechess/pictures/WQ.png
--rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-1.0.0/src/alicechess/pictures/WR.png
--rw-r--r--   0        0        0     2152 2023-06-03 13:02:01.873732 alicechess-1.0.0/src/alicechess/pieces/__init__.py
--rw-r--r--   0        0        0     2539 2023-06-03 13:02:40.681380 alicechess-1.0.0/src/alicechess/pieces/king.py
--rw-r--r--   0        0        0     1369 2023-06-04 02:35:41.836367 alicechess-1.0.0/src/alicechess/pieces/pawn.py
--rw-r--r--   0        0        0     8067 2023-06-07 21:17:23.344370 alicechess-1.0.0/src/alicechess/pieces/piece.py
--rw-r--r--   0        0        0     2171 2023-05-27 03:42:56.855167 alicechess-1.0.0/src/alicechess/player.py
--rw-r--r--   0        0        0     9925 2023-06-04 00:33:15.176040 alicechess-1.0.0/src/alicechess/position.py
--rw-r--r--   0        0        0      376 2023-06-07 21:30:52.032950 alicechess-1.0.0/src/alicechess/test.py
--rw-r--r--   0        0        0     2644 2023-06-07 21:21:10.031159 alicechess-1.0.0/src/alicechess/utils.py
--rw-r--r--   0        0        0    21708 2023-06-07 21:31:05.844394 alicechess-1.0.0/src/alicechess/window.py
--rw-r--r--   0        0        0     4953 1970-01-01 00:00:00.000000 alicechess-1.0.0/setup.py
--rw-r--r--   0        0        0     4822 1970-01-01 00:00:00.000000 alicechess-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4076 2023-06-09 04:14:15.807338 alicechess-1.0.1/README.md
+-rw-r--r--   0        0        0     1042 2023-06-09 04:14:27.253727 alicechess-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      164 2023-06-09 04:07:30.904920 alicechess-1.0.1/src/alicechess/__init__.py
+-rw-r--r--   0        0        0      388 2023-06-07 21:32:17.245811 alicechess-1.0.1/src/alicechess/__main__.py
+-rw-r--r--   0        0        0       65 2023-06-09 04:13:56.560979 alicechess-1.0.1/src/alicechess/__version__.py
+-rw-r--r--   0        0        0     3329 2023-06-07 21:31:30.165561 alicechess-1.0.1/src/alicechess/bots.py
+-rw-r--r--   0        0        0     1808 2023-06-09 00:07:47.640400 alicechess-1.0.1/src/alicechess/game.py
+-rw-r--r--   0        0        0    36219 2023-06-07 21:30:47.973855 alicechess-1.0.1/src/alicechess/game_state.py
+-rw-r--r--   0        0        0    15232 2023-06-07 15:42:54.161860 alicechess-1.0.1/src/alicechess/moves_calculator.py
+-rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-1.0.1/src/alicechess/pictures/BB.png
+-rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-1.0.1/src/alicechess/pictures/BK.png
+-rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-1.0.1/src/alicechess/pictures/BN.png
+-rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-1.0.1/src/alicechess/pictures/BP.png
+-rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-1.0.1/src/alicechess/pictures/BQ.png
+-rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-1.0.1/src/alicechess/pictures/BR.png
+-rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-1.0.1/src/alicechess/pictures/WB.png
+-rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-1.0.1/src/alicechess/pictures/WK.png
+-rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-1.0.1/src/alicechess/pictures/WN.png
+-rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-1.0.1/src/alicechess/pictures/WP.png
+-rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-1.0.1/src/alicechess/pictures/WQ.png
+-rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-1.0.1/src/alicechess/pictures/WR.png
+-rw-r--r--   0        0        0     2152 2023-06-03 13:02:01.873732 alicechess-1.0.1/src/alicechess/pieces/__init__.py
+-rw-r--r--   0        0        0     2539 2023-06-03 13:02:40.681380 alicechess-1.0.1/src/alicechess/pieces/king.py
+-rw-r--r--   0        0        0     1369 2023-06-04 02:35:41.836367 alicechess-1.0.1/src/alicechess/pieces/pawn.py
+-rw-r--r--   0        0        0     8067 2023-06-07 21:17:23.344370 alicechess-1.0.1/src/alicechess/pieces/piece.py
+-rw-r--r--   0        0        0     2171 2023-05-27 03:42:56.855167 alicechess-1.0.1/src/alicechess/player.py
+-rw-r--r--   0        0        0     9925 2023-06-04 00:33:15.176040 alicechess-1.0.1/src/alicechess/position.py
+-rw-r--r--   0        0        0      376 2023-06-07 21:30:52.032950 alicechess-1.0.1/src/alicechess/test.py
+-rw-r--r--   0        0        0     2644 2023-06-07 21:21:10.031159 alicechess-1.0.1/src/alicechess/utils.py
+-rw-r--r--   0        0        0    21708 2023-06-07 21:31:05.844394 alicechess-1.0.1/src/alicechess/window.py
+-rw-r--r--   0        0        0     4963 1970-01-01 00:00:00.000000 alicechess-1.0.1/setup.py
+-rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 alicechess-1.0.1/PKG-INFO
```

### Comparing `alicechess-1.0.0/LICENSE` & `alicechess-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/README.md` & `alicechess-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,8 +100,8 @@
 
 ## Credit
 
 Thank you to Artyom Lisitsyn for inspiring me to pursue this project and to
 Trung Phan for being my chess consultant and answering all my questions on rules
 and technicalities.
 
-[docs]: https://github.com/josephlou5/alicechess/Documentation.md
+[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md
```

### Comparing `alicechess-1.0.0/pyproject.toml` & `alicechess-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 profile = "black"
 # Just setting the profile will use the `black` default line length of 88, so
 # need to override line length as well
 line_length = 79
 
 [tool.poetry]
 name = "alicechess"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python package to play Alice Chess"
 authors = ["Joseph Lou <joseph.d.lou@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/josephlou5/alicechess"
 repository = "https://github.com/josephlou5/alicechess"
 classifiers = [
```

### Comparing `alicechess-1.0.0/src/alicechess/bots.py` & `alicechess-1.0.1/src/alicechess/bots.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/game.py` & `alicechess-1.0.1/src/alicechess/game.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/game_state.py` & `alicechess-1.0.1/src/alicechess/game_state.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/moves_calculator.py` & `alicechess-1.0.1/src/alicechess/moves_calculator.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/BB.png` & `alicechess-1.0.1/src/alicechess/pictures/BB.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/BK.png` & `alicechess-1.0.1/src/alicechess/pictures/BK.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/BN.png` & `alicechess-1.0.1/src/alicechess/pictures/BN.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/BP.png` & `alicechess-1.0.1/src/alicechess/pictures/BP.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/BQ.png` & `alicechess-1.0.1/src/alicechess/pictures/BQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/BR.png` & `alicechess-1.0.1/src/alicechess/pictures/BR.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/WB.png` & `alicechess-1.0.1/src/alicechess/pictures/WB.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/WK.png` & `alicechess-1.0.1/src/alicechess/pictures/WK.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/WN.png` & `alicechess-1.0.1/src/alicechess/pictures/WN.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/WP.png` & `alicechess-1.0.1/src/alicechess/pictures/WP.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/WQ.png` & `alicechess-1.0.1/src/alicechess/pictures/WQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pictures/WR.png` & `alicechess-1.0.1/src/alicechess/pictures/WR.png`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pieces/__init__.py` & `alicechess-1.0.1/src/alicechess/pieces/__init__.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pieces/king.py` & `alicechess-1.0.1/src/alicechess/pieces/king.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pieces/pawn.py` & `alicechess-1.0.1/src/alicechess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/pieces/piece.py` & `alicechess-1.0.1/src/alicechess/pieces/piece.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/player.py` & `alicechess-1.0.1/src/alicechess/player.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/position.py` & `alicechess-1.0.1/src/alicechess/position.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/utils.py` & `alicechess-1.0.1/src/alicechess/utils.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/src/alicechess/window.py` & `alicechess-1.0.1/src/alicechess/window.py`

 * *Files identical despite different names*

### Comparing `alicechess-1.0.0/setup.py` & `alicechess-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*'], 'alicechess': ['pictures/*']}
 
 install_requires = \
 ['Pillow>=9.5.0,<10.0.0']
 
 setup_kwargs = {
     'name': 'alicechess',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'A Python package to play Alice Chess',
-    'long_description': '# Alice Chess\n\nThis project allows you to play Alice Chess, a variant of chess.\n\n## Installastion\n\nThe package may be installed through `pip`:\n\n```bash\n$ pip install alicechess\n```\n\n## Rules\n\nHere is a [description of the concept and rules][rules].\n\n[rules]: https://www.chessvariants.com/other.dir/alice.html\n\nNotable game rules:\n\n- **Castling**: A king and rook may only castle if neither has moved already,\n  the king is not in check, all squares between them are vacant on both boards,\n  and the king does not move through check or into check. After the castle, both\n  pieces will teleport to the other board.\n- **En passant**: A pawn may capture another pawn through en passant if your\n  pawn is on board B and the enemy pawn advances two spaces, teleporting to the\n  space right next to yours on board B. (This results in a situation that looks\n  like regular en passant.) Note that due to teleporting to the other board\n  after each move, this can only be achieved by a pawn that _does not_ advance\n  two squares on its first move.\n- **Fifty move rule**: If both players have made 50 moves each where no piece\n  has been captured or no pawn moved, then a player may claim a draw. However,\n  to simplify this case, the game will be automatically ended with a draw\n  (rather than allowing a player to claim a draw), although this is not the\n  official rule. This therefore overshadows the 75-move rule, where a draw is\n  automatically applied after 75 moves by both players with no captures or pawn\n  movements.\n\n## How to play\n\nTo start a game between two human players, you can easily just run the package\non the command line:\n\n```bash\n$ python -m alicechess\n```\n\nA window will come up where the game can be played.\n\n## Playing against bots\n\nTo play a game against a bot or between bots, you must write your own script.\nYou should initialize a `Game` object with the appropriate players, then call\neither the `start()` or `start_window()` method. To write your own bot, see the\n[Writing a bot](#writing-a-bot) section.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot that plays randomly.\n"""\n\nfrom alicechess import Game, HumanPlayer\nfrom alicechess.bots import RandomPlayer\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=RandomPlayer).start_window()\n```\n\nNote that the class names (not instances) are passed to the `Game` constructor.\n\nThe `start_window()` method will, as implied, start an interactive window where\nthe game can be played. However, you can also opt to use the `start()` method\ninstead, which will return the first `GameState` of the game, and then use\nanother way to ask the user for input and play the game; for instance, you could\nmake the game entirely textual with user input provided with the keyboard. See\nthe [API Documentation][docs] for more information.\n\nIn the interactive window, there is a 3 second delay for non-human player moves,\nto simulate realism. This can be changed by passing a value for\n`non_human_player_delay` to the `start_window()` method.\n\nIt is also possible for two bots to play against each other.\n\n### Writing a bot\n\nThe code is factored in a way to make it very easy for you to code your own bots\nto play against. Simply extend the `Player` class and implement the two abstract\nmethods for making a move and promoting a pawn. This class (not an instance) can\nthen be passed into the `Game` constructor to start a game. See the\n[API Documentation][docs] for more information.\n\n## Advanced Usage\n\nThe only dependency for this project is `Pillow` to use the images in the\ninteractive window. As such, you could technically clone the repository and run\nit without the window with only the Python builtins. Not sure why you would want\nto do that, but that is another alternative option to installing through `pip`.\n\n## Credit\n\nThank you to Artyom Lisitsyn for inspiring me to pursue this project and to\nTrung Phan for being my chess consultant and answering all my questions on rules\nand technicalities.\n\n[docs]: https://github.com/josephlou5/alicechess/Documentation.md\n',
+    'long_description': '# Alice Chess\n\nThis project allows you to play Alice Chess, a variant of chess.\n\n## Installastion\n\nThe package may be installed through `pip`:\n\n```bash\n$ pip install alicechess\n```\n\n## Rules\n\nHere is a [description of the concept and rules][rules].\n\n[rules]: https://www.chessvariants.com/other.dir/alice.html\n\nNotable game rules:\n\n- **Castling**: A king and rook may only castle if neither has moved already,\n  the king is not in check, all squares between them are vacant on both boards,\n  and the king does not move through check or into check. After the castle, both\n  pieces will teleport to the other board.\n- **En passant**: A pawn may capture another pawn through en passant if your\n  pawn is on board B and the enemy pawn advances two spaces, teleporting to the\n  space right next to yours on board B. (This results in a situation that looks\n  like regular en passant.) Note that due to teleporting to the other board\n  after each move, this can only be achieved by a pawn that _does not_ advance\n  two squares on its first move.\n- **Fifty move rule**: If both players have made 50 moves each where no piece\n  has been captured or no pawn moved, then a player may claim a draw. However,\n  to simplify this case, the game will be automatically ended with a draw\n  (rather than allowing a player to claim a draw), although this is not the\n  official rule. This therefore overshadows the 75-move rule, where a draw is\n  automatically applied after 75 moves by both players with no captures or pawn\n  movements.\n\n## How to play\n\nTo start a game between two human players, you can easily just run the package\non the command line:\n\n```bash\n$ python -m alicechess\n```\n\nA window will come up where the game can be played.\n\n## Playing against bots\n\nTo play a game against a bot or between bots, you must write your own script.\nYou should initialize a `Game` object with the appropriate players, then call\neither the `start()` or `start_window()` method. To write your own bot, see the\n[Writing a bot](#writing-a-bot) section.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot that plays randomly.\n"""\n\nfrom alicechess import Game, HumanPlayer\nfrom alicechess.bots import RandomPlayer\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=RandomPlayer).start_window()\n```\n\nNote that the class names (not instances) are passed to the `Game` constructor.\n\nThe `start_window()` method will, as implied, start an interactive window where\nthe game can be played. However, you can also opt to use the `start()` method\ninstead, which will return the first `GameState` of the game, and then use\nanother way to ask the user for input and play the game; for instance, you could\nmake the game entirely textual with user input provided with the keyboard. See\nthe [API Documentation][docs] for more information.\n\nIn the interactive window, there is a 3 second delay for non-human player moves,\nto simulate realism. This can be changed by passing a value for\n`non_human_player_delay` to the `start_window()` method.\n\nIt is also possible for two bots to play against each other.\n\n### Writing a bot\n\nThe code is factored in a way to make it very easy for you to code your own bots\nto play against. Simply extend the `Player` class and implement the two abstract\nmethods for making a move and promoting a pawn. This class (not an instance) can\nthen be passed into the `Game` constructor to start a game. See the\n[API Documentation][docs] for more information.\n\n## Advanced Usage\n\nThe only dependency for this project is `Pillow` to use the images in the\ninteractive window. As such, you could technically clone the repository and run\nit without the window with only the Python builtins. Not sure why you would want\nto do that, but that is another alternative option to installing through `pip`.\n\n## Credit\n\nThank you to Artyom Lisitsyn for inspiring me to pursue this project and to\nTrung Phan for being my chess consultant and answering all my questions on rules\nand technicalities.\n\n[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md\n',
     'author': 'Joseph Lou',
     'author_email': 'joseph.d.lou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josephlou5/alicechess',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `alicechess-1.0.0/PKG-INFO` & `alicechess-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicechess
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to play Alice Chess
 Home-page: https://github.com/josephlou5/alicechess
 License: MIT
 Author: Joseph Lou
 Author-email: joseph.d.lou@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -120,9 +120,9 @@
 
 ## Credit
 
 Thank you to Artyom Lisitsyn for inspiring me to pursue this project and to
 Trung Phan for being my chess consultant and answering all my questions on rules
 and technicalities.
 
-[docs]: https://github.com/josephlou5/alicechess/Documentation.md
+[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md
```

