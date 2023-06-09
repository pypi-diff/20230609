# Comparing `tmp/lasvegas-0.1.4.tar.gz` & `tmp/lasvegas-0.2.0.tar.gz`

## Comparing `lasvegas-0.1.4.tar` & `lasvegas-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 lasvegas-0.1.4/changelog.md
--rw-r--r--   0        0        0  5286809 2020-02-02 00:00:00.000000 lasvegas-0.1.4/rules.pdf
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 lasvegas-0.1.4/todo.md
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 lasvegas-0.1.4/lasvegas/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 lasvegas-0.1.4/lasvegas/_custom_imports.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 lasvegas-0.1.4/lasvegas/game.py
--rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 lasvegas-0.1.4/lasvegas/interactive.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 lasvegas-0.1.4/lasvegas/policies.py
--rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 lasvegas-0.1.4/lasvegas/ui.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 lasvegas-0.1.4/lasvegas/core/__init__.py
--rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 lasvegas-0.1.4/lasvegas/core/env.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 lasvegas-0.1.4/lasvegas/core/rules.py
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 lasvegas-0.1.4/perf/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 lasvegas-0.1.4/perf/__main__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 lasvegas-0.1.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lasvegas-0.1.4/LICENSE
--rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 lasvegas-0.1.4/README.md
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 lasvegas-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    12834 2020-02-02 00:00:00.000000 lasvegas-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 lasvegas-0.2.0/changelog.md
+-rw-r--r--   0        0        0  5286809 2020-02-02 00:00:00.000000 lasvegas-0.2.0/rules.pdf
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 lasvegas-0.2.0/todo.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/__init__.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/game.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/interactive.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/act/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/act/_utils.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/act/player.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/act/policy.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/act/rollicy.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/core/__init__.py
+-rw-r--r--   0        0        0    38722 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/core/env.py
+-rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 lasvegas-0.2.0/lasvegas/core/rules.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 lasvegas-0.2.0/perf/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 lasvegas-0.2.0/perf/__main__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 lasvegas-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lasvegas-0.2.0/LICENSE
+-rw-r--r--   0        0        0    17283 2020-02-02 00:00:00.000000 lasvegas-0.2.0/README.md
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 lasvegas-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    19116 2020-02-02 00:00:00.000000 lasvegas-0.2.0/PKG-INFO
```

### Comparing `lasvegas-0.1.4/rules.pdf` & `lasvegas-0.2.0/rules.pdf`

 * *Files identical despite different names*

### Comparing `lasvegas-0.1.4/lasvegas/interactive.py` & `lasvegas-0.2.0/lasvegas/interactive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,143 +1,185 @@
-""" Module adding interactive functionality.
+""" Module adding interactive functionalities to the package.
 
 Exported functions:
 -------------------
     confront: Confront policies in multiple games.
     play_vs: Play in CLI against humans and/or policies.
 """
 
 __all__ = ['confront', 'play_vs']
 
+import itertools
+
+from numpy.typing import NDArray
 from tqdm import tqdm
 import numpy as np
+import tabulate
 
-from .game import Game, Player, Policy
-from .policies import cli
-from .ui import display_confront, display_game_state
+from .act import BasePlayer, Human, Policy
+from .game import Game, _width
 
 
 def play_vs(
         num_players: int | None = None,
         /,
         *,
-        policies: list[Policy | None] = [],
         humans: int | list[str] = 1,
-        out: bool = False) -> None:
+        policies: list[Policy | None] = [],
+        out: bool = False,
+        **gameargs) -> Game | None:
     """ Play a game in CLI.
 
     If `num_players` is not `None`, humans or policies may be omitted or
-    added to match the number of players. This function priorities
+    added to match the number of players. This function prioritizes
     playing with humans over policies. If `num_players` is `None`, it is
-    inferred from `humans` and `policies` and locally defined
-    `_min_players`.
+    inferred from `humans` and `policies` and locally defined.
 
     Arguments:
     ----------
-        num_players (int | None): Number of players if not `None`.
-        policies (list[Policy | None]): List of policies to play against,
-            `None` corresponding to `Game`'s builtin default policy.
         humans (int | list[str]): Number of human players or list of
             human player names.
+        num_players (int | None): Number of players if not `None`.
         out (bool): Whether or not to return the game at the end.
+        policies (list[Policy | None]): List of policies to play against,
+            `None` corresponding to `Game.default policy`.
+        **gameargs: Passed to `Game` after `num_players` processing.
+
+    Returns:
+    --------
+        game (Game | None): If not `None`, the `Game` instance that was
+            used to play.
     """
-    _min_players = 2  # Arbitrary.
     players = []
     # Human players
     if isinstance(humans, int):
         for i in range(humans):
-            players.append(Player(play_func=cli, name=f"Human {i}"))
+            players.append(Human(f"Human {i}"))
     else:  # Names list
-        for i, name in enumerate(humans):
-            players.append(Player(play_func=cli, name=name))
+        for name in humans:
+            players.append(Human(name))
     # Policy players
     for i, policy in enumerate(policies):
-        players.append(Player(play_func=policy,
-                              name=f"Policy {i}: {policy.__name__}"))
+        players.append(
+            BasePlayer(play_func=policy,
+                       name=f"Policy {i}: {policy and policy.__name__}"))
     # Setup game
-    if num_players is None:
-        g = Game(players, num_players=max(_min_players, len(players)))
-    else:
-        g = Game(players[:num_players], num_players=num_players)
-    # Play and end
-    g()
-    print("Game ended in the following state:")
-    display_game_state(g)
+    if num_players is not None:
+        gameargs["num_players"] = num_players
+    game = Game(players, **gameargs)
+    game.run()
+    msg = "Game ended in the following state:"
+    print(f"\n{msg}\n" + '-' * _width(msg), end='')
+
+    game.env.show(show_roll=False, show_infos=False)
     if out:
-        return g
+        return game
 
 
 def confront(
         *policies: Policy | None,
         games: int = 100,
         show: bool = True,
-        out: bool = False) -> tuple | None:
-    """ Confronts different policies in a `games`-games match.
+        out: bool = False,
+        **gameargs) -> tuple | None:
+    """ Confronts different policies in a multiple-games match.
 
     Results can be displayed in CLI and or output.
     If during a game several policies are ex-aequo, they all share the
     best of their ranks (e.g. 2nd, 3rd and 4th ex-aequo all become 2nd).
 
     Example of console output:
     ```
-    >>> confront(None, lasvegas.policies.greedy_shy)
     Match in 100 games:
-    ╭──────────────────────┬─────┬────────┬─────┬────────╮
-    │ Policy               │ 1st │   with │ 2nd │   with │
-    ├──────────────────────┼─────┼────────┼─────┼────────┤
-    │ Policy 0: None       │  35 │ 506000 │  65 │ 381846 │
-    │ Policy 1: greedy_shy │  66 │ 529848 │  34 │ 397059 │
-    ╰──────────────────────┴─────┴────────┴─────┴────────╯
+    ╭────────────────────────┬─────┬───────────────┬─────┬──────────────╮
+    │ Policy                 │ 1st │ with          │ 2nd │ with         │
+    ├────────────────────────┼─────┼───────────────┼─────┼──────────────┤
+    │ Policy 0: greedy_first │  71 │ 596338 (10.0) │  29 │ 416207 (7.3) │
+    │ Policy 1: greedy_score │  29 │ 527586 (8.7)  │  71 │ 398028 (7.1) │
+    ╰────────────────────────┴─────┴───────────────┴─────┴──────────────╯
     ```
 
     Arguments:
     ----------
-        *policies (Policy | None): Policies to confront.
         games (int): Number of games the match is played over.
         out (bool): Whether or not to return the results.
         show (bool): Whether or not to show the results in CLI.
+        *policies (Policy | None): Policies to confront.
+        **gameargs: Passed to `Game` after `num_players` processing.
 
     Returns:
     --------
         results (tuple | None): If not `None`, `(rankings, avg_scores)`,
             where the `i`th line of `rankings` is the number of times
             `i`th policy finished in each place (from 1st to last), and
             corresponding value in `avg_scores` is its average score
-            at this rank.
+            at this rank as `[avg_tot_bills, avg_num_bills]`
     """
-    n = len(policies)
-    rankings = np.zeros((n, n))
-    avg_scores = np.zeros((n, n))
-    players = [
-        Player(play_func=policy,
-               name=f"Policy {i}: {policy and policy.__name__}")
-        for i, policy in enumerate(policies)]
+    P = len(policies)
+    gameargs["num_players"] = P
+    players = [BasePlayer(play_func=policy,
+                          name=f"Policy {i}: {policy and policy.__name__}")
+               for i, policy in enumerate(policies)]
     # Match:
     # Loop over games
+    game = Game(players, **gameargs)
+    rankings = np.zeros((P, game.env.num_collectors))
+    avg_scores = np.zeros((P, game.env.num_collectors, 2))
     for _ in tqdm(range(games)):
-        g = Game(players)
-        g()
+        game.run()
         # Find winner
-        scores = [(0, 0)] * n
-        for i in range(n):
-            bills = g.players_bills[i]
-            scores[g.players_permutation[i]] = (sum(bills), len(bills))
-        order = sorted(range(n), key=lambda i: scores[i], reverse=True)
-        ranks = sorted(range(n), key=lambda i: order[i])
-        # Reajust draws (if 2nd == 3rd, both 2nd)
-        for s, i in list(enumerate(order)):
-            if i == 0:
-                continue
-            if scores[i] == scores[order[s-1]]:
-                ranks[i] = ranks[order[s-1]]
-        # Update ranking: `i` reresents  policy index and `r` its rank.
-        for i, r in enumerate(ranks):
-            rankings[i][r] += 1
-            avg_scores[i][r] += scores[i][0]
-    avg_scores /= rankings
+        order = game.env.rank_order()
+        ordered_scores = game.env.scores[order]
+        ranks = np.arange(game.env.num_collectors)
+        for i, (s, ss) in enumerate(itertools.pairwise(ordered_scores)):
+            if np.all(s == ss):
+                ranks[i+1] = ranks[i]
+        for score, rank, i_pol in zip(ordered_scores, ranks, order):
+            if i_pol < P:
+                rankings[i_pol, rank] += 1
+                avg_scores[i_pol, rank] += score  # (tot, num)
+    avg_scores /= np.expand_dims(rankings, axis=-1)
     result = rankings, avg_scores
     # Show (?)
     if show:
-        display_confront(players, result, games)
+        gameargs.pop("num_players")
+        _display_confront(game,
+                          result,
+                          games,
+                          gameargs_str=str(gameargs or ''))
     # Out (?)
     if out:
         return result
+
+
+def _display_confront(
+        game: Game,
+        result: tuple[NDArray[int], NDArray[float]],
+        games: int,
+        *,
+        gameargs_str: str = '') -> None:
+    """ Prints human-readable results of policy confrontation.
+
+    Example of output can be found in `.interactive.confront` doc.
+    """
+    headers = ["Policy"] + [x
+                            for i in range(game.env.num_collectors)
+                            for x in [game.env._ordinal(i + 1), 'with']]
+    lines = []
+    for player, ranks_occ, avg_scores in zip(game.players, *result):
+        line = [player.name]
+        for rank_occ, (avg_tot, avg_num) in zip(ranks_occ, avg_scores):
+            if np.isnan(avg_tot):
+                line += [rank_occ, "- (-)"]
+            else:
+                line += [rank_occ,
+                         f'{round(avg_tot)} ({round(avg_num, ndigits=1)})']
+        lines.append(line)
+    # Tabulate
+    PADDING_bak = tabulate.MIN_PADDING
+    tabulate.MIN_PADDING = 0
+    table = tabulate.tabulate(lines, headers, "rounded_outline")
+    tabulate.MIN_PADDING = PADDING_bak
+    # Print
+    print(f"Match in {games} games"
+          f"{' with ' + gameargs_str + ':' if gameargs_str else ':'}")
+    print(table)
```

### Comparing `lasvegas-0.1.4/perf/__init__.py` & `lasvegas-0.2.0/perf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,145 +3,155 @@
 Exported functions:
 -------------------
     main: Runs multiple games and times execution.
 """
 
 __all__ = ['main']
 
-from typing import Any, Iterable
-
 from math import ceil, log10
 from time import perf_counter
+from typing import Any, Sequence
+
 from tqdm import tqdm
 import numpy as np
 import tabulate
 
-from lasvegas.core import GameRules
-from lasvegas.game import Player, Policy, Game
+from lasvegas.act import BasePlayer, Policy
+from lasvegas.core import RuleBook
+from lasvegas.game import Game
 
 
 TimeStat = tuple[float, float, float, float]
 
 
 def main(policy: Policy | None = None,
-         games: int = 1000,
+         games: int = 100,
          out: bool = False,
          /,
-         **ruleset: Any) -> list[TimeStat] | None:
+         **gameargs: Any) -> list[TimeStat] | None:
     """ Runs multiple games and times execution before displaying stats.
 
     Arguments:
     ----------
+        games (int): Number of games to run and gather stats over.
         policy (Policy | None): Policy used as all players in the game.
             If `None`, `Game` will use default -- uniformly random.
-        games (int): Number of games to run and gather stats over.
         out (bool): Default is `False`, meaning results are only
             displayed. If `True`, results are only returned.
-        **ruleset (Any): Ruleset to use for performance measure. If
+        **gameargs (Any): Ruleset to use for performance measure. If
             `num_players` is not specified, all values from
             `GameRules.rulebook_min_players` to
             `GameRules.rulebook_max_players` will be tested.
 
     Returns:
     --------
         results (list[TimeStat] | None): If `out`, list of all
             `(mean, stdv, min_, max_)` game time for every number of
             players tested.
     """
     all_num_players = (
-        [ruleset.pop("num_players")]
-        if "num_players" in ruleset
-        else range(GameRules.rulebook_min_players,
-                   GameRules.rulebook_max_players + 1))
+        [gameargs.pop("num_players")]
+        if "num_players" in gameargs
+        else set(RuleBook.xtr_rules))
     results = [
-        run_ruleset(policy, games, num_players=num_players, **ruleset)
+        run_gameset(policy, games, num_players=num_players, **gameargs)
         for num_players in all_num_players]
     if out:
         return results
     else:
         print(f"Game time for policy '{policy and policy.__name__}' "
-              f"over {games} games:")
+              f"{'with ' + str(gameargs) + ' ' if gameargs else ''}"
+              f"(over {games} games):")
         display_results(all_num_players, results)
 
 
-def run_ruleset(
+def run_gameset(
         policy: Policy | None,
         games: int,
-        **ruleset: Any) -> TimeStat:
-    """ Perf measurement logic, given a oplicy and ruleset.
+        **gameargs: Any) -> TimeStat:
+    """ Perf measurement logic, given a oplicy and gameargs.
 
     Elapsed time starts before `Game` instance creation and ends when
     the game is over:
     ```
     START                                                   END
       |game-instanciation-----game-is-played-----game-is-over|
     ```
 
     Arguments:
     ----------
-        policy (Policy | None): Policy used for all players in the game.
         games (int): Number of games to run and time.
-        **ruleset (Any): The ruleset used for measured game.
+        policy (Policy | None): Policy used for all players in the game.
+        **gameargs (Any): Passed to `Game`.
 
     Returns:
     --------
         mean, stdv, min_, max_ (TimeStat): Respectively, the mean,
-            standard deviation, min and max elapsed time over `games`
-            games, in `ms`.
+            standard deviation, min and max elapsed time over
+            `games` games, in `ms`.
 
     Raises:
     -------
         `AssertionError` if `not games > 0`.
     """
     assert games > 0
     durations = np.zeros(games)
-    num_players = ruleset["num_players"]
-    players = [Player(play_func=policy) for _ in range(num_players)]
-    for i in tqdm(range(games), desc=f"{num_players} players", leave=False):
+    num_players = gameargs["num_players"]
+    players = [BasePlayer(play_func=policy) for _ in range(num_players)]
+    game = Game(players, **gameargs)
+    for i in tqdm(range(games),
+                  desc=f"{num_players} players",
+                  leave=False):
         # Start
         start = perf_counter()
-        Game(players)()
+        game.run()
         # End
         end = perf_counter()
         durations[i] = end - start
     mean = np.mean(durations)
     stdv = np.std(durations)
     min_ = np.min(durations)
     max_ = np.max(durations)
     return mean, stdv, min_, max_
 
 
 def display_results(
-        all_num_players: Iterable[int],
+        all_num_players: Sequence[int],
         results: list[TimeStat]) -> None:
-    """ Displays results from multiple `run_ruleset` calls.
+    """ Displays results from multiple `run_gameset` calls.
 
     Arguments:
     ----------
-        all_num_players (Iterable[int]): All number of players tested.
+        all_num_players (Sequence[int]): All number of players tested.
         results: (list[TimeStat]): The corresponding perf results.
 
     Example of output:
     ```
-    Game time for policy 'None' over 1000 games:
     ╭─────────────┬──────────┬──────────┬──────────┬──────────╮
     │ Num players │ Mean     │ Std      │ Min      │ Max      │
     ├─────────────┼──────────┼──────────┼──────────┼──────────┤
-    │           2 │ 674.6 us │ 112.9 us │ 533.4 us │ 1.566 ms │
-    │           3 │ 776.3 us │ 64.76 us │ 670.5 us │ 1.223 ms │
-    │           4 │ 1.007 ms │ 152.7 us │ 841.8 us │ 2.440 ms │
-    │           5 │ 918.3 us │ 75.86 us │ 809.7 us │ 1.457 ms │
+    │           1 │ 5.791 ms │ 662.2 us │ 4.940 ms │ 8.902 ms │
+    │           2 │ 1.636 ms │ 184.3 us │ 1.377 ms │ 2.310 ms │
+    │           3 │ 2.064 ms │ 178.5 us │ 1.752 ms │ 2.582 ms │
+    │           4 │ 2.718 ms │ 269.3 us │ 2.355 ms │ 3.807 ms │
+    │           5 │ 2.791 ms │ 250.8 us │ 2.457 ms │ 3.742 ms │
     ╰─────────────┴──────────┴──────────┴──────────┴──────────╯
     ```
     """
     headers = ["Num players", "Mean", "Std", "Min", "Max"]
     lines = [
         [num_players] + list(map(format_time, result))
         for num_players, result in zip(all_num_players, results)]
-    print(tabulate.tabulate(lines, headers, "rounded_outline"))
+    # Table
+    PADDING_bak = tabulate.MIN_PADDING
+    tabulate.MIN_PADDING = 0
+    table = tabulate.tabulate(lines, headers, "rounded_outline")
+    tabulate.MIN_PADDING = PADDING_bak
+    # Print
+    print(table)
 
 
 def format_time(duration: float, num_digits: int = 4) -> str:
     """ Formats a `float` duration in seconds to a readable `str`.
 
     A few examples with `num_digits = 4` are given below, showcasing
     some special cases.
```

### Comparing `lasvegas-0.1.4/LICENSE` & `lasvegas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lasvegas-0.1.4/pyproject.toml` & `lasvegas-0.2.0/pyproject.toml`

 * *Files identical despite different names*

