# Comparing `tmp/libretrofuzz-2.9.9.tar.gz` & `tmp/libretrofuzz-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.9.9.tar", max compression
+gzip compressed data, was "libretrofuzz-3.0.0.tar", max compression
```

## Comparing `libretrofuzz-2.9.9.tar` & `libretrofuzz-3.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/LICENSE
--rw-r--r--   0        0        0     7900 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/README.rst
--rw-r--r--   0        0        0       22 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    55098 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/pyproject.toml
--rw-r--r--   0        0        0     9078 2023-06-08 04:41:07.833858 libretrofuzz-2.9.9/setup.py
--rw-r--r--   0        0        0     9088 2023-06-08 04:41:07.835004 libretrofuzz-2.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-08 19:57:51.975392 libretrofuzz-3.0.0/LICENSE
+-rw-r--r--   0        0        0     8014 2023-06-08 19:57:51.975392 libretrofuzz-3.0.0/README.rst
+-rw-r--r--   0        0        0       22 2023-06-08 19:57:51.975392 libretrofuzz-3.0.0/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    54633 2023-06-08 19:57:51.975392 libretrofuzz-3.0.0/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-08 19:57:51.975392 libretrofuzz-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9194 2023-06-08 19:58:06.674284 libretrofuzz-3.0.0/setup.py
+-rw-r--r--   0        0        0     9202 2023-06-08 19:58:06.675262 libretrofuzz-3.0.0/PKG-INFO
```

### Comparing `libretrofuzz-2.9.9/LICENSE` & `libretrofuzz-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.9/README.rst` & `libretrofuzz-3.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 False positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
 
 Example:
   ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``
 
   The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.
 
+To debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.
+
 libretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]
   :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.
 
                         Linux default:   ``~/.config/retroarch/retroarch.cfg``
 
                         Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``
 
@@ -54,26 +56,26 @@
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
   --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
                         | [1<=x<=30]
   --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=30]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
-  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.
+  --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.
                         | [default: 200; 0<=x<=200]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
-  --verbose N           | Show length N list: score, mininame, emoji hyperlinks.
+  --verbose N           | Show length N list: score, name, emoji hyperlinks.
                         | [x>=1]
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
```

### Comparing `libretrofuzz-2.9.9/libretrofuzz/__main__.py` & `libretrofuzz-3.0.0/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 #! /usr/bin/env python3
 
 # this downloads thumbnails for retroarch playlists
-# it uses fuzzy matching to find the most similar name to the names, based on the playlist description.
-# there may be false positives, especially if the thumbnail server does not have the game but does have
-# another similarly named game - happens on series or playlists where multiple versions of a game coexist.
-
-# Although a game playlist entry may have a different db this script doesn't handle that to simplify
-# the caching of names, since it's rare, so it assumes all entries in a playlist will have the same system.
+# it uses fuzzy matching to find the most similar name
+# to the server names, based on the playlist description.
+# there may be false positives, especially if the thumbnail
+# server does not have the game but does have another similarly
+# named game - happens often on series or playlists where
+# multiple versions of a game coexist.
+
+# Although a game playlist entry may have a different db this
+# script doesn't handle that to simplify the caching of names,
+# since it's rare, it assumes all entries in a playlist will
+# have the same system.
 
 from pathlib import Path
 from typing import Optional, List
 from urllib.request import unquote, quote
 from tempfile import TemporaryDirectory
 from contextlib import asynccontextmanager, contextmanager
+from functools import partial
 from itertools import chain
 from struct import unpack
 import json
 import os
 import sys
 import io
 import regex
@@ -25,15 +31,14 @@
 import collections
 import shutil
 import unicodedata
 import asyncio
 import subprocess
 import configparser
 import platform
-from functools import partial
 
 # external libraries
 from PIL import Image, ImageOps
 from rapidfuzz import process, fuzz
 from bs4 import BeautifulSoup
 from questionary import Style, select
 from httpx import RequestError, HTTPStatusError, Client, AsyncClient
@@ -55,29 +60,31 @@
 ########### SCRIPT SETTINGS ###############
 ###########################################
 
 ADDRESS = "https://thumbnails.libretro.com"
 MAX_SCORE = 200
 MAX_RETRIES = 3
 MAX_WAIT_SECS = 30
-# 00-1f are ascii control codes, rest is 'normal' illegal windows filename chars according to powershell + &
+# 00-1f are ascii control codes, rest are illegal windows filename chars according to powershell + &
 forbidden = regex.compile(
     r"[\u0022\u003c\u003e\u007c\u0000\u0001\u0002\u0003\u0004\u0005\u0006\u0007\u0008"
     + r"\u0009\u000a\u000b\u000c\u000d\u000e\u000f\u0010\u0011\u0012\u0013\u0014\u0015"
     + r"\u0016\u0017\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f\u003a\u002a\u003f\u005c\u002f\u0026]"
 )
 # external terminal image viewer application
 viewer = None
 
-# makes a class with these fields, which are the subdir names on the server system dir of the types of thumbnails
+# makes a class with these fields, the subdir names on the server system dir of the types of thumbnails
 Thumbs = collections.namedtuple("Thumbs", ["Named_Boxarts", "Named_Titles", "Named_Snaps"])
 # this is for 64 bits too
 if sys.platform == "win32":
-    # this order is to make 'portable' installs have priority in windows, a concept that doesn't exist in linux or macosx
-    # these are the default 32 and 64 bits installer paths, since there is no way to know what the user choses, check the defaults only.
+    # this order is to make 'portable' installs have priority in windows
+    # a concept that doesn't exist in linux or macosx
+    # these are the default 32 and 64 bits installer paths, since there
+    # is no way to know what the user choses, check the defaults only.
     CONFIG = Path(r"C:/RetroArch-Win64/retroarch.cfg")
     if not CONFIG.exists():
         CONFIG = Path(r"C:/RetroArch/retroarch.cfg")
         if not CONFIG.exists():
             echo("Portable install default location config not found, trying with APPDATA location")
             var = os.getenv("APPDATA")
             if var:
@@ -150,16 +157,18 @@
     if skip:
         raise StopDownload()
     if enter:
         raise ContinueDownload()
 
 
 def checkEscape():
-    """only called when it doesn't matter if a escape will happen, usually at the start of a iteration or the preparation phase"""
-    # so we can reset skip here, since it wont matter either way and will help remove false skip positives from the key event loop
+    """only called when it doesn't matter if a escape will happen,
+    usually at the start of a iteration or the preparation phase"""
+    # we can reset variables here, since it wont matter either way and
+    # will help remove false skip positives from the key event loop
     global skip
     skip = False
     global enter
     enter = False
     global escape
     if escape:
         raise StopProgram()
@@ -167,24 +176,20 @@
 
 @asynccontextmanager
 async def lock_keys():
     """blocks key echoing for this console and recognizes most keys
     including many combinations, user kill still works, alt+tab...
     it also serves as a quit program and skip download shortcut
     from: https://python-prompt-toolkit.readthedocs.io/en/master/pages/asking_for_input.html
-    Since this is decorated with a asynccontextmanager, it's guarded by async with
+    Since this is decorated with a asynccontextmanager, it's guarded with
     https://docs.python.org/3/reference/compound_stmts.html#async-with
 
-    since prompt_toolkit (3.0) input.attach attaches to a already running event asyncio event loop,
-    these key checks run essentially 'forever' in the same thread as the main one.
-
-    This is event loop is not cooperative (although it's thread safe, since it's a single thread)
-    so stale 'skip' (not ctrl-c or escape, since those exit right away) can be set to 'True' with a
-    logical check error of set while a nondownload iteration was running then check on a unrelated one.
-    So then you should reset skip on the 'checkescape' function at the start of every iteration
+    since prompt_toolkit (3.0) input.attach attaches to the running asyncio event loop
+    check asyncio.sleep(0) and reset the global variables here when appropriate to prevent
+    stale keys being used, probably on the same function checking for escape to exit
     """
     input = create_input()
 
     def keys_ready():
         global skip
         global escape
         global enter
@@ -208,18 +213,17 @@
                         "Press escape to quit, enter to continue and most other non-meta keys to skip downloads",
                         bold=True,
                     )
                 )
                 yield
     finally:
         # in windows 7 and python 3.8 for some reason prompt_toolkit
-        # tries to send a 'handle ready' not 'remove' event after detaching (the with above)
-        # not sure if it happens in python later than 3.8.
-        # This throws a 'RuntimeError: Event Loop is closed'
-        # the sleep avoids it
+        # tries to send a 'handle ready' not 'remove' event after
+        # detaching (the with above) not sure if it happens in python
+        # later than 3.8. The sleep avoids a 'RuntimeError: Event Loop is closed'
         if sys.platform == "win32":
             await asyncio.sleep(0.1)
 
 
 # ----------------non contextual str manipulation------------------------
 def link(uri, label=None, parameters=""):
     """
@@ -249,15 +253,16 @@
 
 
 spatterns = {" - ": regex.compile(r".*( - .*)"), ": ": regex.compile(r".*(: .*)")}
 before_metadata = regex.compile(r"(^[^[({]*)")
 
 
 def nosubtitle_aux(t, subtitle_marker=" - "):
-    # last subtitle marker and everything there until the end (last because i noticed that 'subsubtitles' exist,
+    # last subtitle marker and everything there until the
+    # end, last because i noticed that 'subsubtitles' exist
     # for instance, ultima 7 - part 1|2 - subtitle
     try:
         pattern = spatterns[subtitle_marker]
     except:
         pattern = regex.compile(rf".*({subtitle_marker}.*)")
         spatterns[subtitle_marker] = pattern
     name_without_meta = regex.search(before_metadata, t)
@@ -279,27 +284,28 @@
 
 def removeprefix(name: str, pre: str):
     if name.startswith(pre):
         return name[len(pre) :]
     return name
 
 
-# ----------------Used to check the existence of a sixtel compatible terminal image viewer-------------------------------
+# Used to check the existence of a sixtel compatible terminal image viewer
 def which(executable):
     flips = shutil.which(executable)
     if not flips:
         flips = shutil.which(executable, path=os.path.dirname(__file__))
     if not flips:
         flips = shutil.which(executable, path=os.getcwd())
     return flips
 
 
-# -----------------------------------------------------------------------------------------------------------------------
-# The heart of the program, what orders titles to be 'more similar' or less to the local labels (after the normalization)
-# -----------------------------------------------------------------------------------------------------------------------
+# -------------------------------------------------------------------
+# The heart of the program, what orders titles to be 'more similar'
+# or less to the local labels (after the normalization)
+# -------------------------------------------------------------------
 class TitleScorer(object):
     def __init__(self):
         # rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way)
         # so it uses internal api to prevent a possible early exit at == 100
         self._RF_ScorerPy = {
             "get_scorer_flags": lambda **kwargs: {
                 "optimal_score": MAX_SCORE,
@@ -311,32 +317,33 @@
     def __call__(self, s1, s2, processor=None, score_cutoff=None):
         if (min(len(s1), len(s2)) / max(len(s1), len(s2))) < 0.2:
             # ideally this branch wouldn't exist, but since many games do not have
             # images, they get caught up on a short title being completely contained in another
             # token_set_ratio gives that 100. Skip if the smaller name length is less than 20%
             return 0
         # names are whitespace and case normalized, but they keep spaces
-        # for token_set_ratio. But still test this case.
+        # for token_set_ratio. But still test this case, since it's common
         if s1 == s2 or "".join(s1.split()) == "".join(s2.split()):
             return MAX_SCORE
         prefix = len(os.path.commonprefix([s1, s2]))
         # score_cutoff needs to be 0 from a combination of 3 factors that create a bug:
         # 1. the caller of this, extract passes the 'current best score' as score_cutoff
         # 2. the token_set_ratio function returns 0 if the calculated score < score_cutoff
         # 3. 'current best score' includes the prefix, which this call can't include in 2.
         similarity = fuzz.token_set_ratio(s1, s2, processor=None, score_cutoff=0)
         # Combine the scorer with a common prefix heuristic to give priority to longer similar
         # names, this helps prevents false positives for shorter strings which token set ratio
         # is prone because it sets score to 100 if one string words are completely on the other.
         return min(MAX_SCORE - 1, similarity + prefix)
 
 
-# -----------------------------------------------------------------------------------------------------------------------------
-# Normalization functions, part of the functions that change both local labels and remote names to be more similar to compare
-# -----------------------------------------------------------------------------------------------------------------------------
+# ---------------------------------------------------------------
+# Normalization functions, part of the functions that change both
+# local labels and remote names to be more similar to compare
+# ---------------------------------------------------------------
 camelcase_pattern = regex.compile(r"(\p{Lu}[\p{Ll},'“”\"]+)")
 # number sequences in the middle (not start or end) of a string that start with 0
 zero_lead_pattern = regex.compile(r"([^\d])0+([1-9])")
 
 
 def normalizer(t, nometa, hack):
     if nometa:
@@ -347,15 +354,15 @@
     t = replacemany(t, '_()[]{}-.!?#"', "")
     # strips just because the user may have made a mistake naming the source
     # (or the replacement above introduce boundary spaces)
     t = t.strip()
     # remove any number leading 0, except at the end or the start of the string
     # where it is likely a important part of the name, not a file manager sort workaround
     t = regex.sub(zero_lead_pattern, r"\1\2", t)
-    # CamelCaseNames for local labels are common when there are no spaces,
+    # CamelCaseNames for local labels are common when there are no spaces, split them
     # do this to normalize definite articles in normalization with spaces only (minimizes changes)
     t = " ".join([s.strip() for s in regex.split(camelcase_pattern, t) if s])
     # normalize case
     t = t.lower()
     # beginning and end definite articles in several european languages (people move them)
     # make sure we're only removing the start and end forms with spaces
     t = removefirst(t, ", the")
@@ -385,21 +392,21 @@
     t = removeprefix(t, "os ")
     t = removefirst(t, ", as")
     t = removeprefix(t, "as ")
     t = removefirst(t, ", o")
     t = removeprefix(t, "o ")
     t = removefirst(t, ", a")
     t = removeprefix(t, "a ")
-    # remove the symbols used in the definite article normalization
+    # remove the symbols used in the definite article normalization and word splitting
     t = replacemany(t, ",'“”\"", "")
     # this makes sure that if a remote name has ' and ' instead of ' _ ' to replace ' & ' it works
     #': ' doesn't need this because ':' is a forbidden character and both '_' and '-' turn to ''
     t = t.replace(" and ", " ")
     # Tries to make roman numerals in the range 1-20 equivalent to normal numbers.
-    # If both sides are roman numerals there is no harm done if XXIV gets turned into 204 in both sides.
+    # If both str tested have roman numerals no harm done if XXIV gets turned into 204.
     t = t.replace("xviii", "18")
     t = t.replace("xvii", "17")
     t = t.replace("xvi", "16")
     t = t.replace("xiii", "13")
     t = t.replace("xii", "12")
     t = t.replace("xiv", "14")
     t = t.replace("xv", "15")
@@ -412,17 +419,17 @@
     t = t.replace("iii", "3")
     t = t.replace("ii", "2")
     t = t.replace("iv", "4")
     t = t.replace("v", "5")
     t = t.replace("ix", "9")
     t = t.replace("x", "10")
     t = t.replace("i", "1")
-    # remove diacritics (does nothing to asian languages diacritics, only for 2 to 1 character combinations)
+    # remove diacritics (not to asian languages diacritics, only for 2 to 1 character combinations)
     t = "".join([c for c in unicodedata.normalize("NFKD", t) if not unicodedata.combining(c)])
-    # normalize spaces (don't remove them for other later score methods to be able to reorder tokens
+    # normalize spaces (don't remove them for other later score methods to be able to reorder tokens)
     return " ".join(t.split())
 
 
 def nosubtitle_normalizer(t, nometa, hack):
     return normalizer(nosubtitle_aux(t), nometa, hack)
 
 
@@ -533,15 +540,20 @@
 
 
 def error(error: str):
     echo(style(error, fg=RED, bold=True))
 
 
 def common_errors(cfg: Path, playlist: str, system: str, address: str):
-    """returns a tuple with (playlist_dir: Path, thumbnail_dir: Path, playlists: [Path], systems: [str])"""
+    """returns tuple (
+    nub_verbose: bool,    #hint to turn off emoji hyperlinks and images
+    thumbnail_dir: Path,  #RA thumbnail dir from the config file
+    playlists: [Path],    #sorted list of playlists in the playlist dir
+    systems: [str])       #sorted list of available systems on the thumbnail server
+    """
     global ADDRESS
     ADDRESS = address.rstrip("/")
     global viewer
     viewer = which("chafa")
     if not viewer:
         echo("Shell image viewer chafa was not found")
     if not cfg or not cfg.is_file():
@@ -562,19 +574,19 @@
     playlists = [pl for pl in playlist_dir.glob("./*.lpl") if pl.is_file() and os.access(pl, os.R_OK)]
     if not playlists:
         error(f"Invalid playlist files in playlist directory: {playlist_dir}")
         raise Exit(code=1)
     if playlist and Path(playlist_dir, playlist) not in playlists:
         error(f"Invalid user provided playlist: {playlist}")
         raise Exit(code=1)
+
     # windows can only print images and urls in windows 10 up (requires a better console)
-    # since python 3.8 is the very minimum of this application, it can only be used on windows 7 and up
-    # ie: we only have to disallow 7, 8
+    # since python 3.8 is the very minimum of this application, and it's for windows 7 and up
+    # we only have to disallow 7, 8
     nub_verbose = False
-
     if sys.platform == "win32" and platform.release() in ("7", "8", "8.1"):
         echo("Disabling rich verbose and image output because your windows does not support it")
         nub_verbose = True
     try:
         with Client() as client:
             page = client.get(ADDRESS, timeout=15)
             soup = BeautifulSoup(page.text, "html.parser")
@@ -635,15 +647,15 @@
     ),
     score: int = Option(
         MAX_SCORE,
         "--min",
         min=0,
         max=MAX_SCORE,
         metavar="SCORE",
-        help=f"0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.",
+        help=f"0=any, 100=fuzzy match, {MAX_SCORE}=equal,default. No-op with --no-fail.",
     ),
     nofail: bool = Option(False, "--no-fail", help="Download any score. Equivalent to --score 0."),
     noimage: bool = Option(False, "--no-image", help="Don't show images even with chafa installed."),
     nomerge: bool = Option(
         False,
         "--no-merge",
         help="Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.",
@@ -669,15 +681,15 @@
     ),
     address: Optional[str] = Option(
         ADDRESS,
         metavar="URL",
         help="URL with libretro-thumbnails server. For local files, git clone/unzip packs, run 'python3 -m http.server' in parent dir, and use --address 'http://localhost:8000'.",
     ),
     verbose: Optional[int] = Option(
-        None, "--verbose", min=1, metavar="N", help="Show length N list: score, mininame, emoji hyperlinks."
+        None, "--verbose", min=1, metavar="N", help="Show length N list: score, name, emoji hyperlinks."
     ),
 ):
     if playlist and not playlist.lower().endswith(".lpl"):
         playlist = playlist + ".lpl"
 
     (nub_verbose, playlist_dir, thumbnails_dir, playlists, systems) = common_errors(
         cfg, playlist, system, address
@@ -782,15 +794,15 @@
     ),
     score: int = Option(
         MAX_SCORE,
         "--min",
         min=0,
         max=MAX_SCORE,
         metavar="SCORE",
-        help=f"0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.",
+        help=f"0=any, 100=fuzzy match, {MAX_SCORE}=equal,default. No-op with --no-fail.",
     ),
     nofail: bool = Option(False, "--no-fail", help="Download any score. Equivalent to --score 0."),
     noimage: bool = Option(False, "--no-image", help="Don't show images even with chafa installed."),
     nomerge: bool = Option(
         False,
         "--no-merge",
         help="Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.",
@@ -816,18 +828,18 @@
     ),
     address: Optional[str] = Option(
         ADDRESS,
         metavar="URL",
         help="URL with libretro-thumbnails server. For local files, git clone/unzip packs, run 'python3 -m http.server' in parent dir, and use --address 'http://localhost:8000'.",
     ),
     verbose: Optional[int] = Option(
-        None, "--verbose", min=1, metavar="N", help="Show length N list: score, mininame, emoji hyperlinks."
+        None, "--verbose", min=1, metavar="N", help="Show length N list: score, name, emoji hyperlinks."
     ),
 ):
-    (nub_verbose, playlist_dir, thumbnails_dir, playlists, systems) = common_errors(cfg, None, None, address)
+    (nub_verbose, _, thumbnails_dir, playlists, systems) = common_errors(cfg, None, None, address)
     if nub_verbose:
         noimage = True
 
     notInSystems = [
         (playlist, os.path.basename(playlist)[:-4])
         for playlist in playlists
         if os.path.basename(playlist)[:-4] not in systems
@@ -889,15 +901,15 @@
         for tdir in ["/Named_Boxarts/", "/Named_Titles/", "/Named_Snaps/"]:
             lr_thumb = lr_thumbs + tdir
             response = ""
             async with client.stream("GET", lr_thumb, timeout=15) as r:
                 async for chunk in r.aiter_text(4096):
                     checkEscape()
                     response += chunk
-            # not found is ok, since some server system directories do not have all the subdirectories
+            # not found is ok, some server system directories don't have all the subdirectories
             if r.status_code == 404:
                 l1 = {}
             elif r.status_code == 521:
                 raise StopPlaylist()
             else:
                 # will go to except if there is a another error
                 r.raise_for_status()
@@ -934,83 +946,86 @@
     thumbnails_dir: Path,
     client: AsyncClient,
 ):
     # not a error to pass a empty playlist
     if len(names) == 0:
         return
     thumbs = Thumbs._make(await downloadgamenames(client, system))
-    # before implies that the names of the playlists may be cut, so the hack and meta matching must be disabled
+    # before implies that the names of the playlists may be cut,
+    # so the hack and meta matching must be disabled
     if before:
         hack = False
         nometa = True
     # no-fail is equivalent to max fuzz
     if nofail:
         score = 0
 
-    # built the function that will be called to print data, filling in some fixed arguments
-    strfy_runtime = partial(strfy, score, verbose, nub_verbose)
+    # build the function that will be called to print data,
+    # filling in some fixed arguments
+    short_names = os.getenv("SHORT")
+    short_names = True if short_names and short_names != "0" else False
+    strfy_runtime = partial(strfy, score, short_names, nub_verbose)
 
     # preprocess data so it's not redone every loop iteration.
     title_scorer = TitleScorer()
-    # normalize with or without subtitles, besides the remote_names this is used on the iterated local names later
+    # normalize with or without subtitles, besides the
+    # remote_names this is used on the iterated local names later
     norm = nosubtitle_normalizer if nosubtitle else normalizer
     # we choose the highest similarity of all 3 directories, since no mixed matches are allowed
     remote_names = set()
     remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
     # turn into a set, original key and normalized value.
     remote_names = {x: norm(x, nometa, hack) for x in remote_names}
     for name, destination in names:
         await asyncio.sleep(0)  # update key status
         checkEscape()  # check key status
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
-        # to simplify this code, the forbidden characters are replaced twice,
-        # on the string that is going to be the filename and the modified string copy of that that is going to be matched.
-        # it could be done only once, but that would require separating the colon character for subtitle matching,
-        # and the 'before' operation would have to find the index before the match to apply it after. A mess.
 
+        # to simplify this code, the forbidden characters are replaced twice, on the string
+        # that is going to be the filename and the string copy that is going to be matched.
         nameaux = name
 
         #'before' has priority over subtitle removal
         if before:
             # Ignore metadata and get the string before it
             name_without_meta = regex.search(before_metadata, nameaux)
             if name_without_meta:
                 before_index = name_without_meta.group(1).find(before)
                 if before_index != -1:
                     nameaux = nameaux[0:before_index]
 
         # there is a second form of subtitles, which doesn't appear in the thumbnail server
         # but can appear in linux game names. It uses the colon character, which is forbidden
-        # in windows. Note that this does mean that if the servername has 'Name_ subtitle.png'
-        # and not 'Name - subtitle.png' there is less chance of a match, but that is rarer than opposite.
+        # in windows. Note that this means that if the servername has 'Name_ subtitle.png',
+        # not 'Name - subtitle.png' it has little chance of a match, but that's rarer than opposite.
         # not to mention that this only applies if the user signals 'no-subtitle',
         # which presumably means they tried without it - which does match.
         if nosubtitle:
             nameaux = nosubtitle_aux(nameaux, ": ")
 
         # only the local names should have forbidden characters
         name = regex.sub(forbidden, "_", name)
         nameaux = regex.sub(forbidden, "_", nameaux)
 
         # unlike the server thumbnails, normalization wasn't done yet
         nameaux = norm(nameaux, nometa, hack)
 
         # operate on cache (to speed up by not applying normalization every iteration)
-        # the normalization can make it so that the winner has the same score as the runner up(s)
+        # normalization can make it so that the winner has the same score as the runner up(s)
         # so to make sure we catch at least two candidates for cases where that happens
         # it's a improvement because sometimes server thumbnail types have case letter typos
         result = process.extract(
             nameaux, remote_names, scorer=title_scorer, processor=None, limit=verbose or 2, score_cutoff=None
         )
         _, max_score, _ = (result and result[0]) or (None, -1, None)
         winners = [x for x in result if x[1] == max_score and x[1] >= score]
         show = result if verbose else winners
-        name_format = style(nameaux + ": ", bold=True) if verbose else style(name + ": ", bold=True)
+        name_format = style((nameaux if short_names else name) + ": ", bold=True)
 
         if winners:
             allow = True
             # these parent directories were created when reading the playlist
             # more efficient than doing it a playlist game loop
             real_thumb_dir = Path(thumbnails_dir, destination)
             down_thumb_dir = Path(tmpdir, destination)
@@ -1056,15 +1071,16 @@
                         for winner in winners:
                             t_norm, t_score, t_name = winner
                             # something to download
                             url = getattr(thumbs, dirname).get(t_name, None)
                             if not url:
                                 continue
 
-                            # with filters/reset you always download, and without only if it doesn't exist already.
+                            # with filters/reset you always download, and
+                            # without only if it doesn't exist already.
                             if filters or not real.exists():
                                 if await download(
                                     client,
                                     url,
                                     temp,
                                     getting_format,
                                     waiting_format,
@@ -1073,30 +1089,30 @@
                                     MAX_RETRIES,
                                 ):
                                     first_wait = False
                                     downloaded_once = True
                                     urls[(dirname, winner)] = url
                                     break
                     # Delete old images in the case of --filter.
-                    # this assumes internet is on, which is fair because
-                    # to get here you needed to have downloaded things
-                    # but it will skip if the user cancels, as is logical
-                    # this needs to be before image display
+                    # internet not available will exit the program
+                    # so this won't happen in a loop in that case
+                    # broken/not found server links WILL get deleted
+                    # it will also skip if the user cancels
+                    # as is logical this is before image display
                     if filters:
                         for old, _ in downloaded_dict.values():
                             old.unlink(missing_ok=True)
                     if not noimage and viewer and downloaded_once:
                         displayImages(downloaded_dict)
                         if wait_after is not None:
                             await printwait(wait_after, waiting_format)
                     if downloaded_once:
                         for old, new in downloaded_dict.values():
                             if new.exists():
                                 shutil.move(new, old)
-
                         name_format = name_format + ", ".join((strfy_runtime(x, urls) for x in show))
                         success_format = f'{style("Success",   fg=GREEN, bold=True)}: {name_format}'
                         echo(success_format)
                 except StopProgram as e:
                     name_format = name_format + ", ".join((strfy_runtime(x) for x in show))
                     skipped_format = f'{style("Skipped",     fg=(135,135,135), bold=True)}: {name_format}'
                     echo(skipped_format)
@@ -1122,29 +1138,29 @@
     count = int(wait / 0.1)
     with handleContinueDownload():
         for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, leave=False):
             checkDownload()
             await asyncio.sleep(0.1)
 
 
-def strfy(required_score, verbose, nub_verbose, r, urlsdict=None):
+def strfy(required_score, short_names, nub_verbose, r, urlsdict=None):
     thumb_norm, thumb_score, thumb_name = r
     score_color = RED if thumb_score < required_score else GREEN
     score_text = style(f"{int(thumb_score)}", fg=f"{score_color}", bold=True)
     if nub_verbose:
         return f"{score_text} {thumb_norm}"
     elif urlsdict:
         url1 = urlsdict.get((Thumbs._fields[0], r), None)
         url2 = urlsdict.get((Thumbs._fields[1], r), None)
         url3 = urlsdict.get((Thumbs._fields[2], r), None)
     else:
         url1 = None
         url2 = None
         url3 = None
-    thumb_text = thumb_norm if verbose else thumb_name
+    thumb_text = thumb_norm if short_names else thumb_name
     linked1 = style(link(url1, "🎴")) if url1 else ""
     linked2 = style(link(url2, "🎬")) if url2 else ""
     linked3 = style(link(url3, "📸")) if url3 else ""
     return f"{score_text} {thumb_text}{linked1}{linked2}{linked3}"
 
 
 async def download(
@@ -1222,15 +1238,16 @@
     # (added after the resizes, so they look the same)
     wanted_box_y = max([i.size[1] for i in imgs.values()])
     x, y = box.size
     if y != wanted_box_y:
         x = max(round(x * wanted_box_y / y), 1)
         y = wanted_box_y
     box = box.resize((x, y))
-    # the right side will adjust the width until title and snap are the same width and the desired height is reached (minus inner borders).
+    # the right side will adjust the width until title and snap are the
+    # same width and the desired height is reached (minus inner borders).
     wanted_y = wanted_box_y - BORDER_SIZE * 2
     x1, y1 = title.size
     x2, y2 = snap.size
     # Formulas to derive the value of samex (same width they need to reach wanted_y):
     # wanted_y = yx1 + yx2 and yx1 = y1 * samex / x1 and yx2 = y2 * samex / x2
     # then:
     # wanted_y = y1/x1 * samex + y2/x2 * samex <=>
```

### Comparing `libretrofuzz-2.9.9/pyproject.toml` & `libretrofuzz-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.9.9"
+version = "3.0.0"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.9.9/setup.py` & `libretrofuzz-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.9.9',
+    'version': '3.0.0',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list: score, mininame, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-2.9.9/PKG-INFO` & `libretrofuzz-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.9.9
+Version: 3.0.0
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -65,14 +65,16 @@
 False positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
 
 Example:
   ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``
 
   The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.
 
+To debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.
+
 libretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]
   :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.
 
                         Linux default:   ``~/.config/retroarch/retroarch.cfg``
 
                         Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``
 
@@ -83,26 +85,26 @@
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
   --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
                         | [1<=x<=30]
   --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=30]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
-  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.
+  --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.
                         | [default: 200; 0<=x<=200]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
-  --verbose N           | Show length N list: score, mininame, emoji hyperlinks.
+  --verbose N           | Show length N list: score, name, emoji hyperlinks.
                         | [x>=1]
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
```

