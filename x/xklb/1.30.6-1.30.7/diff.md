# Comparing `tmp/xklb-1.30.6.tar.gz` & `tmp/xklb-1.30.7.tar.gz`

## Comparing `xklb-1.30.6.tar` & `xklb-1.30.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.6/.gitattributes
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 xklb-1.30.6/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.6/Windows.md
--rw-r--r--   0        0        0   490403 2020-02-02 00:00:00.000000 xklb-1.30.6/pdm.lock
--rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 xklb-1.30.6/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.6/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.30.6/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.6/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/__init__.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/books.py
--rw-r--r--   0        0        0     7790 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/consts.py
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/dl_config.py
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/dl_extract.py
--rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/hn_extract.py
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/lb.py
--rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/play_actions.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/playback.py
--rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/player.py
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/praw_extract.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/search.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/tabs_extract.py
--rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/tube_backend.py
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/tube_extract.py
--rw-r--r--   0        0        0    77219 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/usage.py
--rw-r--r--   0        0        0    37021 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.6/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.6/LICENSE
--rw-r--r--   0        0        0    99569 2020-02-02 00:00:00.000000 xklb-1.30.6/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.6/pyproject.toml
--rw-r--r--   0        0        0   103165 2020-02-02 00:00:00.000000 xklb-1.30.6/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.7/.gitattributes
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.30.7/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.7/Windows.md
+-rw-r--r--   0        0        0   490403 2020-02-02 00:00:00.000000 xklb-1.30.7/pdm.lock
+-rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 xklb-1.30.7/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.30.7/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.7/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/__init__.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/books.py
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/consts.py
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/dl_config.py
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/lb.py
+-rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/play_actions.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/playback.py
+-rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/player.py
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/search.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/tube_extract.py
+-rw-r--r--   0        0        0    77219 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/usage.py
+-rw-r--r--   0        0        0    36215 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.7/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.7/LICENSE
+-rw-r--r--   0        0        0    99569 2020-02-02 00:00:00.000000 xklb-1.30.7/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.7/pyproject.toml
+-rw-r--r--   0        0        0   103165 2020-02-02 00:00:00.000000 xklb-1.30.7/PKG-INFO
```

### Comparing `xklb-1.30.6/TODO` & `xklb-1.30.7/TODO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-- use rowid alias instead of string pks: playlists table: switch playlist_path fk to integer id
-
-- wt/lt/search join and use fts on both tables, threading ?
+- use rowid alias instead of string pks: playlists table: switch playlist_path nullable fk to integer id
 
 - POIs CLI -- save your trip plans and see places to go with automated day trip itineraries, geopandas buffer
 
-- upscale command -- download higher quality videos; use webpath, PURL, comment to get URL
-
-- move time_played, playhead, and other ephemeral data to its own table
+- wt/lt/search join and use fts on both tables, threading ?
 
-add time_first_played, time_last_played; remove time_played instead use play_count
+- upscale command -- download higher quality videos; use webpath, PURL, comment to get URL
 
 - move mpv specific playhead code to a script subcommand
 
 option to delete mpv watch_later file if media file does not exist
 
-- improve block subcommand
+- move time_played, playhead, and other ephemeral data to its own table
 
-add support for domains, specific combinations
+add time_first_played, time_last_played; remove time_played instead use play_count
 
 - improve playlists subcommand
 
 - make generic printer. support --json or --csv for most subcommands
 
-SELECT \* FROM playlists p WHERE PATH NOT IN (SELECT DISTINCT playlist_path FROM media WHERE playlist_path NOT NULL )
-
 - improve dlstatus subcommand
 
 - scan bpm and key sig  https://github.com/aubio/aubio https://github.com/tyiannak/pyAudioAnalysis
 
+- cluster images
+
+https://github.com/HughKu/Im2txt
+https://github.com/immich-app/immich/tree/main/machine-learning/app
+
 - CLI EDA tool
 
 - CLI incremental diff (SQLITE, NDJSON, CSV)
 
     compare 100 rows at a time using primary key
 
     show the differences between files
```

### Comparing `xklb-1.30.6/Windows.md` & `xklb-1.30.7/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/pdm.lock` & `xklb-1.30.7/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -881,15 +881,15 @@
     "markdown-it-py<3.0.0,>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.271"
+version = "0.0.272"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 
 [[package]]
 name = "scalene"
 version = "1.5.19"
 requires_python = ">=3.8"
@@ -1206,15 +1206,15 @@
 name = "websockets"
 version = "11.0.3"
 requires_python = ">=3.7"
 summary = "An implementation of the WebSocket Protocol (RFC 6455 & 7692)"
 
 [[package]]
 name = "werkzeug"
-version = "2.3.4"
+version = "2.3.6"
 requires_python = ">=3.8"
 summary = "The comprehensive WSGI web application library."
 dependencies = [
     "MarkupSafe>=2.1.1",
 ]
 
 [[package]]
@@ -2900,32 +2900,32 @@
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
 "rich 13.4.1" = [
     {url = "https://files.pythonhosted.org/packages/02/97/0046b5e3c6a5057b5817e5e6c51a776d410b953e6a9c67ae249dafdd2999/rich-13.4.1.tar.gz", hash = "sha256:76f6b65ea7e5c5d924ba80e322231d7cb5b5981aa60bfc1e694f1bc097fe6fe1"},
     {url = "https://files.pythonhosted.org/packages/ea/93/c68645c689d10a035010e3ae314b6b2855d040ce0d11fdfdfbb8be416581/rich-13.4.1-py3-none-any.whl", hash = "sha256:d204aadb50b936bf6b1a695385429d192bc1fdaf3e8b907e8e26f4c4e4b5bf75"},
 ]
-"ruff 0.0.271" = [
-    {url = "https://files.pythonhosted.org/packages/00/6a/eb0f14b8942522797b3bcaa468528ab9492b7d200a76af222d76dd3a89ea/ruff-0.0.271-py3-none-win32.whl", hash = "sha256:403e8f9de18b2279d65015a45e0e0d98d60ad878d52f46904f502a4d09465815"},
-    {url = "https://files.pythonhosted.org/packages/05/3a/4cf1193c3fef061cf719e6e60291796ed189f251843e0b2c88479da8e596/ruff-0.0.271-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9e5de841e09ea75a26956a2cda930d1260c9d8d94cbe57c13b3e881d96526860"},
-    {url = "https://files.pythonhosted.org/packages/09/42/4a175bfb99a1db67bd0ce2e9f18afa0b82f804b9dbc572a099931d4f86ae/ruff-0.0.271-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:cd43c1aff3eefb2193a125a12124438f65a8d1a6da0e86f8545141d48f6a39fa"},
-    {url = "https://files.pythonhosted.org/packages/0e/55/e6c1af8dc0ac3ea8e078ab7323567ff58ce02c8205b87716e156e5f48f9b/ruff-0.0.271-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:f3fd9e7c7afb7740d2734af3348e6c88226b42acba2e10a3d1e449caa67e4652"},
-    {url = "https://files.pythonhosted.org/packages/48/9a/99858a13725552d2364ba8ae7f89b35a7b974e4ad8eba7bf9965469dbe39/ruff-0.0.271-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5a73ffda5548ea8e28e0afcfa698a8675bb17f7048299327f4c1a1287b6e36a2"},
-    {url = "https://files.pythonhosted.org/packages/5c/99/11d8d05cd4186fd6e852d46f47a27de5c6da9f0c2045e6eeb24db136bad5/ruff-0.0.271-py3-none-musllinux_1_2_i686.whl", hash = "sha256:efdfe7fea656eb2ed54f123135c04f71744ad6e4c0c6be156d46e7a2f4730d48"},
-    {url = "https://files.pythonhosted.org/packages/86/35/8a339e8740a7988bdab0adcb016ff0b4a390ee9e7801e2fa071e944e4885/ruff-0.0.271-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f445c56cdc8c12fc28a0b16588ba33abebb6340cb5b1b5a7d5668d4c0b31ad33"},
-    {url = "https://files.pythonhosted.org/packages/86/54/39c28366ee871c955a9beeb092aed3b632a466b8811865aaa78aa7d94cd3/ruff-0.0.271-py3-none-win_amd64.whl", hash = "sha256:140e912a18a662062b04b489861e5aebdbe1a1668bf416e5a951f2347aa65907"},
-    {url = "https://files.pythonhosted.org/packages/9b/50/cd5fec53ae4670b9d409a3f9e99c85016980fb594fb5e1ab354f3171853c/ruff-0.0.271-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:1a627978df924635f7d1a169a98abb2ea488c2d409da56a3f9e44a82d30606ac"},
-    {url = "https://files.pythonhosted.org/packages/a0/e8/1f5116a0b4d6349b8682497287a22ea7b3c13c01b82aab407f213f8289fa/ruff-0.0.271-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:191cdddfc82165afd63ab29ad671419a90a5e699b026ac2d9c61232543965de6"},
-    {url = "https://files.pythonhosted.org/packages/a6/c0/359fa555e0a5ce87e66319c4b6f4035bba75626d39ae133deeff86ca5769/ruff-0.0.271-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:fca503741f4b23a7179fd7a9bc50fc2cca637e9a4da027776f38690c50ae559f"},
-    {url = "https://files.pythonhosted.org/packages/ae/e5/8d3c2a3a507ecb6b161a7838da601d623bb25f2b366f0aadd2f2ddeabfc4/ruff-0.0.271-py3-none-win_arm64.whl", hash = "sha256:45b3c3551a798d9786779c6dd7ad2224af6e06162e17f4a0e7678d3e9115ae56"},
-    {url = "https://files.pythonhosted.org/packages/b2/95/99f3884f93dbc909662362253b84d29923e379f5ad6032f7720ea69c12b0/ruff-0.0.271-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:f47d8a192f6869e95896dc5bb7e825a4f9c554136b9c3bddd38389e43d4db08b"},
-    {url = "https://files.pythonhosted.org/packages/b9/6c/5353a2267cc1a4b72fba83ea4093a57a10a1bcf058f0fbf2557f5c6fff65/ruff-0.0.271-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7e34ca86329a542ab5d31f4fc2702f556d62748f4217e2f6951aef93176190f0"},
-    {url = "https://files.pythonhosted.org/packages/eb/d0/bc63f1baa7e6d7698a857591fe215cc3bac174b309de15bdd2e1b3fe0bd4/ruff-0.0.271-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:7543b8a32e000ed30727ca6e570a90ab26f8899ee23dffb28806dfc2618782fb"},
-    {url = "https://files.pythonhosted.org/packages/f9/39/2888b3baad15b7930c084da2a2c6f3cac669c4add9b98ac2f74c8378d64a/ruff-0.0.271.tar.gz", hash = "sha256:be4590137a31c47e7f6ef4488d60102c68102f842453355d8073193a30199aa7"},
-    {url = "https://files.pythonhosted.org/packages/fb/de/7647175d1889f29ffbfa7dcbc8a0ed3e007ecc955a01a158d562a6ad37ec/ruff-0.0.271-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:67525aa821ff0f8371eaa28c73dc467b8eea18931a8bd749775ad538fe1f35e6"},
+"ruff 0.0.272" = [
+    {url = "https://files.pythonhosted.org/packages/1f/12/1b0b513ccf7a0ea19430843bf3a82b51704a1c8001900ca99066b69270ec/ruff-0.0.272-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:691d72a00a99707a4e0b2846690961157aef7b17b6b884f6b4420a9f25cd39b5"},
+    {url = "https://files.pythonhosted.org/packages/2e/96/1a4b3b9c658bf2a04ba7820aefa24d8561f73379bf0d79c2f01321c4dd84/ruff-0.0.272-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:d5a208f8ef0e51d4746930589f54f9f92f84bb69a7d15b1de34ce80a7681bc00"},
+    {url = "https://files.pythonhosted.org/packages/48/cb/2e8b7d690eec62a16971f15ca018248bc9058fb2d6abf0588f1fcc9fafb4/ruff-0.0.272-py3-none-win_arm64.whl", hash = "sha256:06b8ee4eb8711ab119db51028dd9f5384b44728c23586424fd6e241a5b9c4a3b"},
+    {url = "https://files.pythonhosted.org/packages/4a/8f/66590b978ceeb3d62eee4f46eeabff4a4967cde81c05e9d4e8a28ca18f7d/ruff-0.0.272-py3-none-win_amd64.whl", hash = "sha256:a37ec80e238ead2969b746d7d1b6b0d31aa799498e9ba4281ab505b93e1f4b28"},
+    {url = "https://files.pythonhosted.org/packages/4b/f8/50874f1992355a8c565bc6322659abf7cc86ce2e929ea4930d14768a022b/ruff-0.0.272-py3-none-musllinux_1_2_i686.whl", hash = "sha256:19643d448f76b1eb8a764719072e9c885968971bfba872e14e7257e08bc2f2b7"},
+    {url = "https://files.pythonhosted.org/packages/67/d5/ce76ab5f37f647bdbed63b857c47c275620ad34b1a062529c5514675c5ee/ruff-0.0.272.tar.gz", hash = "sha256:273a01dc8c3c4fd4c2af7ea7a67c8d39bb09bce466e640dd170034da75d14cab"},
+    {url = "https://files.pythonhosted.org/packages/6a/cd/5ef249cd71029d869edb858171d108ea001c98baab7c1e88123d7a49c86b/ruff-0.0.272-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:1609b864a8d7ee75a8c07578bdea0a7db75a144404e75ef3162e0042bfdc100d"},
+    {url = "https://files.pythonhosted.org/packages/6e/41/8d0ceacc7e5be1f54f9c5cf22ad80541e8751ffa4b6870d801ad082257e7/ruff-0.0.272-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:677284430ac539bb23421a2b431b4ebc588097ef3ef918d0e0a8d8ed31fea216"},
+    {url = "https://files.pythonhosted.org/packages/6e/ff/6864326dc773a5467a06369cb1125391424b86478ed8f242bffb835b10a8/ruff-0.0.272-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:905ff8f3d6206ad56fcd70674453527b9011c8b0dc73ead27618426feff6908e"},
+    {url = "https://files.pythonhosted.org/packages/74/a8/c6a072ae54cb9144086b0437e9febc638e52d7c4e4520e197395cf6b1e7a/ruff-0.0.272-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:48eccf225615e106341a641f826b15224b8a4240b84269ead62f0afd6d7e2d95"},
+    {url = "https://files.pythonhosted.org/packages/91/81/5d65b3ed9a0e02f14275df6e2e1e1d95495af0a429256ab998a35d2de104/ruff-0.0.272-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:ae9b57546e118660175d45d264b87e9b4c19405c75b587b6e4d21e6a17bf4fdf"},
+    {url = "https://files.pythonhosted.org/packages/98/9c/932d41fe80ec408a8a618b61ee7f36a99d67b99b70de480f8ab1d2771af0/ruff-0.0.272-py3-none-win32.whl", hash = "sha256:dc406e5d756d932da95f3af082814d2467943631a587339ee65e5a4f4fbe83eb"},
+    {url = "https://files.pythonhosted.org/packages/98/b7/478cf23d492f07ca13b45b7efa2c43660e3a4a229623f3f196022631e387/ruff-0.0.272-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ee76b4f05fcfff37bd6ac209d1370520d509ea70b5a637bdf0a04d0c99e13dff"},
+    {url = "https://files.pythonhosted.org/packages/c5/74/25a315f9020f05e5f8508467d930bff61667514260ab03505397fb293cf0/ruff-0.0.272-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:9c4bfb75456a8e1efe14c52fcefb89cfb8f2a0d31ed8d804b82c6cf2dc29c42c"},
+    {url = "https://files.pythonhosted.org/packages/d6/ae/8018ccae4f6757d1b6c0e3b1c6ca5fbe2f0a9c83474b9abc468b76b2ba26/ruff-0.0.272-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:86bc788245361a8148ff98667da938a01e1606b28a45e50ac977b09d3ad2c538"},
+    {url = "https://files.pythonhosted.org/packages/e2/1a/c0e7f3b10550f53113bdb671b509171f54e7c3fbec99b7114561c99c5cc2/ruff-0.0.272-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:27b2ea68d2aa69fff1b20b67636b1e3e22a6a39e476c880da1282c3e4bf6ee5a"},
+    {url = "https://files.pythonhosted.org/packages/e3/f8/c8242e21cd82e0e2d6403e54d62d2dff66a6bf5f221455ba3496363de0a3/ruff-0.0.272-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bd2bbe337a3f84958f796c77820d55ac2db1e6753f39d1d1baed44e07f13f96d"},
 ]
 "scalene 1.5.19" = [
     {url = "https://files.pythonhosted.org/packages/11/19/c973ecc43b18076df6c7efff7bec280d02d48d8245f46d94b7e90cf306f2/scalene-1.5.19-cp39-cp39-win_amd64.whl", hash = "sha256:d1fd5d83f3c022ddc46049f29823351b8dbdb8590f5803358fa6034784601f24"},
     {url = "https://files.pythonhosted.org/packages/19/54/d89426ab970f1cb3850b0374967ae22d831d0091efeb2c1d8e8d02ac2a19/scalene-1.5.19-cp39-cp39-macosx_11_7_universal2.whl", hash = "sha256:6c08f3bc0b6355db3c34f0e9aea1b291e64675bb832e19758ee751918787cac0"},
     {url = "https://files.pythonhosted.org/packages/49/11/5a2fa4567eee217609e0a627534f5fb60d0c1f768b43a93145a2ea24e39b/scalene-1.5.19-cp38-cp38-manylinux_2_24_x86_64.whl", hash = "sha256:f67f39321548c06de440319bdd70c41c14b6c50d4748226a101402995677cade"},
     {url = "https://files.pythonhosted.org/packages/5e/3c/b1f159a11f0949f3f27b18af1cc68ee301088a7337efc7d961684bdd3f46/scalene-1.5.19-cp37-cp37m-macosx_10_15_universal2.whl", hash = "sha256:58fb40d031081a55e813f292b2d85b64d7558a372832d8e456f7fe2113adf182"},
     {url = "https://files.pythonhosted.org/packages/65/c3/ebaf00eef807b8da6c5b0c4eb6627f0a67538a25ac7e3858347e15c55d22/scalene-1.5.19-cp38-cp38-win_amd64.whl", hash = "sha256:7a1d452ad4d32cf8adb8b86cae4e5b9c7bff866fff1c43618f9ad114b9ecac32"},
@@ -3219,17 +3219,17 @@
     {url = "https://files.pythonhosted.org/packages/e9/26/1dfaa81788f61c485b4d65f1b28a19615e39f9c45100dce5e2cbf5ad1352/websockets-11.0.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:f467ba0050b7de85016b43f5a22b46383ef004c4f672148a8abf32bc999a87f0"},
     {url = "https://files.pythonhosted.org/packages/eb/fb/2af7fc3ce2c3f1378d48a15802b4ff2caf6c0dfac13291e73c557caf04f7/websockets-11.0.3-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:42cc5452a54a8e46a032521d7365da775823e21bfba2895fb7b77633cce031bb"},
     {url = "https://files.pythonhosted.org/packages/ec/3f/0c5cae14e9e86401105833383405787ae4caddd476a8fc5561259253dab7/websockets-11.0.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1a073fc9ab1c8aff37c99f11f1641e16da517770e31a37265d2755282a5d28aa"},
     {url = "https://files.pythonhosted.org/packages/ed/45/466944e00b324ae3a1fddb305b4abf641f582e131548f07bcd970971b154/websockets-11.0.3-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:ed058398f55163a79bb9f06a90ef9ccc063b204bb346c4de78efc5d15abfe602"},
     {url = "https://files.pythonhosted.org/packages/f3/82/2d1f3395d47fab65fa8b801e2251b324300ed8db54753b6fb7919cef0c11/websockets-11.0.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:84d27a4832cc1a0ee07cdcf2b0629a8a72db73f4cf6de6f0904f6661227f256f"},
     {url = "https://files.pythonhosted.org/packages/f4/3f/65dfa50084a06ab0a05f3ca74195c2c17a1c075b8361327d831ccce0a483/websockets-11.0.3-cp39-cp39-win_amd64.whl", hash = "sha256:c792ea4eabc0159535608fc5658a74d1a81020eb35195dd63214dcf07556f67e"},
 ]
-"werkzeug 2.3.4" = [
-    {url = "https://files.pythonhosted.org/packages/2d/bf/5a00bb4a70028f7c6000bc9394492154fa9ae3f5226187e3ddcd0aa5eca1/Werkzeug-2.3.4.tar.gz", hash = "sha256:1d5a58e0377d1fe39d061a5de4469e414e78ccb1e1e59c0f5ad6fa1c36c52b76"},
-    {url = "https://files.pythonhosted.org/packages/c2/2f/f0dc628295bd23571c962d5a349307d9c8796a05bfca6571659eaded38e2/Werkzeug-2.3.4-py3-none-any.whl", hash = "sha256:48e5e61472fee0ddee27ebad085614ebedb7af41e88f687aaf881afb723a162f"},
+"werkzeug 2.3.6" = [
+    {url = "https://files.pythonhosted.org/packages/ba/d6/8040faecaba2feb84e1647af174b3243c9b90c163c7ea407820839931efe/Werkzeug-2.3.6-py3-none-any.whl", hash = "sha256:935539fa1413afbb9195b24880778422ed620c0fc09670945185cce4d91a8890"},
+    {url = "https://files.pythonhosted.org/packages/d1/7e/c35cea5749237d40effc50ed1a1c7518d9f2e768fcf30b4e9ea119e74975/Werkzeug-2.3.6.tar.gz", hash = "sha256:98c774df2f91b05550078891dee5f0eb0cb797a522c757a2452b9cee5b202330"},
 ]
 "wheel 0.40.0" = [
     {url = "https://files.pythonhosted.org/packages/61/86/cc8d1ff2ca31a312a25a708c891cf9facbad4eae493b3872638db6785eb5/wheel-0.40.0-py3-none-any.whl", hash = "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"},
     {url = "https://files.pythonhosted.org/packages/fc/ef/0335f7217dd1e8096a9e8383e1d472aa14717878ffe07c4772e68b6e8735/wheel-0.40.0.tar.gz", hash = "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873"},
 ]
 "xlrd 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/aa/05/ec9d4fcbbb74bbf4da9f622b3b61aec541e4eccf31d3c60c5422ec027ce2/xlrd-1.2.0.tar.gz", hash = "sha256:546eb36cee8db40c3eaa46c351e67ffee6eeb5fa2650b71bc4c758a29a1b29b2"},
```

### Comparing `xklb-1.30.6/readme.py` & `xklb-1.30.7/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.30.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.30.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/.github/workflows/push.yaml` & `xklb-1.30.7/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/sql/transfer.sql` & `xklb-1.30.7/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/av.py` & `xklb-1.30.7/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/books.py` & `xklb-1.30.7/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/consts.py` & `xklb-1.30.7/xklb/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
     if speech_recognition:
         extensions.extend(SPEECH_RECOGNITION_EXTENSIONS)
 
     return get_files(path, extensions)
 
 
 time_facets = [
+    "all",
     "watching",
     "watched",
     "deleted",
     "created",
     "modified",
     "downloaded",
 ]
```

### Comparing `xklb-1.30.6/xklb/db.py` & `xklb-1.30.7/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/dl_config.py` & `xklb-1.30.7/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/dl_extract.py` & `xklb-1.30.7/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/fs_extract.py` & `xklb-1.30.7/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/gui.py` & `xklb-1.30.7/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/hn_extract.py` & `xklb-1.30.7/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/lb.py` & `xklb-1.30.7/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/play_actions.py` & `xklb-1.30.7/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/playback.py` & `xklb-1.30.7/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/player.py` & `xklb-1.30.7/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/praw_extract.py` & `xklb-1.30.7/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/search.py` & `xklb-1.30.7/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/subtitle.py` & `xklb-1.30.7/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/tabs_actions.py` & `xklb-1.30.7/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/tabs_extract.py` & `xklb-1.30.7/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/tube_backend.py` & `xklb-1.30.7/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/tube_extract.py` & `xklb-1.30.7/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/usage.py` & `xklb-1.30.7/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/utils.py` & `xklb-1.30.7/xklb/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -959,14 +959,22 @@
     try:
         print(x, flush=True)
     except BrokenPipeError:
         sys.stdout = None
         sys.exit(141)
 
 
+def pipe_lines(x) -> None:
+    try:
+        sys.stdout.writelines(x)
+    except BrokenPipeError:
+        sys.stdout = None
+        sys.exit(141)
+
+
 def random_string() -> str:
     return "".join(random.choices(string.ascii_uppercase + string.digits, k=5))
 
 
 def random_filename(path) -> str:
     ext = Path(path).suffix
     path = str(Path(path).with_suffix(""))
@@ -1068,61 +1076,25 @@
             if entry.is_file():
                 files.append(entry.path)
                 if len(files) == limit:
                     break
     return sorted(files)
 
 
-def load_spacy_model(model=None):
-    try:
-        import spacy
-    except ModuleNotFoundError:
-        log.error("Install spaCy and sklearn to use:")
-        log.error("pip install spacy sklearn")
-        log.error("python -m spacy download en_core_web_sm")
-        sys.exit(1)
-
-    if model:
-        return spacy.load(model)
-
-    model_sizes = ["lg", "md", "sm"]
-    loaded_model = None
-
-    for size in model_sizes:
-        try:
-            loaded_model = spacy.load(f"en_core_web_{size}")
-            log.info(f"Loaded 'en_core_web_{size}'")
-        except OSError:
-            pass
-
-    if loaded_model:
-        return loaded_model
-
-    log.error("Language model not found. Download a model first using the following commands:")
-    log.error("python -m spacy download en_core_web_sm")
-    sys.exit(1)
-
-
-def cluster_paths(paths, model=None, n_clusters=None):
-    nlp = load_spacy_model(model)
-
+def cluster_paths(paths, n_clusters=None):
     from sklearn.cluster import KMeans
     from sklearn.feature_extraction.text import TfidfVectorizer
 
     sentence_strings = (path_to_sentence(s) for s in paths)
 
-    joined_strings = []
-    for doc in nlp.pipe(sentence_strings, n_process=4):
-        joined_strings.append(" ".join([token.lower_ for token in doc if not token.is_stop]))
-
-    vectorizer = TfidfVectorizer()
-    X = vectorizer.fit_transform(joined_strings)
+    vectorizer = TfidfVectorizer(min_df=2, strip_accents="unicode", stop_words="english")
+    X = vectorizer.fit_transform(sentence_strings)
 
-    kmeans = KMeans(n_clusters=n_clusters or int(X.shape[0] ** 0.5), random_state=0).fit(X)
-    clusters = kmeans.labels_
+    clusterizer = KMeans(n_clusters=n_clusters or int(X.shape[0] ** 0.5), random_state=0, n_init=10).fit(X)
+    clusters = clusterizer.labels_
 
     grouped_strings = {}
     for i, string in enumerate(paths):
         cluster_id = clusters[i]
 
         if cluster_id not in grouped_strings:
             grouped_strings[cluster_id] = []
```

### Comparing `xklb-1.30.6/xklb/scripts/bigdirs.py` & `xklb-1.30.7/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/block.py` & `xklb-1.30.7/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/christen.py` & `xklb-1.30.7/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/cluster_sort.py` & `xklb-1.30.7/xklb/scripts/cluster_sort.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from xklb import usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library cluster-sort", usage=usage.cluster_sort)
-    parser.add_argument("--model", "-m", help="Use a specific spaCy model")
     parser.add_argument("--clusters", "--n-clusters", "-c", type=int, help="Number of KMeans clusters")
     parser.add_argument("--groups", "-g", action="store_true", help="Show groups")
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("input_path", nargs="?", type=argparse.FileType("r"), default=sys.stdin)
     parser.add_argument("output_path", nargs="?")
     args = parser.parse_args()
@@ -21,25 +20,25 @@
 
 def cluster_sort() -> None:
     args = parse_args()
 
     lines = args.input_path.readlines()
     args.input_path.close()
 
-    groups = utils.cluster_paths(lines, args.model, args.clusters)
+    groups = utils.cluster_paths(lines, args.clusters)
     groups = sorted(groups, key=lambda d: (len(d["grouped_paths"]), -len(d["common_prefix"])))
 
     if args.groups:
         from rich import print
 
         print(groups)
     else:
         lines = utils.flatten(d["grouped_paths"] for d in groups)
         if args.output_path:
             with open(args.output_path, "w") as output_fd:
                 output_fd.writelines(lines)
         else:
-            sys.stdout.writelines(lines)
+            utils.pipe_lines(lines)
 
 
 if __name__ == "__main__":
     cluster_sort()
```

### Comparing `xklb-1.30.6/xklb/scripts/copy_play_counts.py` & `xklb-1.30.7/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/dedupe.py` & `xklb-1.30.7/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/download_status.py` & `xklb-1.30.7/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/history.py` & `xklb-1.30.7/xklb/scripts/history.py`

 * *Files 23% similar despite different names*

```diff
@@ -79,43 +79,46 @@
     tbl = utils.col_resize(tbl, "duration", 5)
     tbl = utils.col_resize(tbl, "playhead", 5)
     tbl = utils.list_dict_filter_bool(tbl)
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
 
 def recent_media(args, time_column):
+    m_columns = args.db["media"].columns_dict
     query = f"""
     SELECT
         path
-        , title
-        , duration
-        , subtitle_count
+        {', title' if 'title' in m_columns else ''}
+        {', duration' if 'duration' in m_columns else ''}
+        {', subtitle_count' if 'subtitle_count' in m_columns else ''}
         , {time_column}
     FROM media
     WHERE coalesce({time_column}, 0)>0
     ORDER BY {time_column} desc
     LIMIT {args.limit or 5}
     """
     return list(args.db.query(query))
 
 
 def history() -> None:
     args = parse_args()
 
+    m_columns = args.db["media"].columns_dict
+
     if args.facet.startswith(("all", "watching")):
         print("Partially watched:")
         tbl = player.historical_usage(args, args.frequency, "time_played", "and coalesce(play_count, 0)=0")
         print_history(tbl)
         query = f"""SELECT
                 path
-                , title
-                , duration
-                , subtitle_count
-                , time_played
-                , playhead
+                {', title' if 'title' in m_columns else ''}
+                {', duration' if 'duration' in m_columns else ''}
+                {', subtitle_count' if 'subtitle_count' in m_columns else ''}
+                {', time_played' if 'time_played' in m_columns else ''}
+                {', playhead' if 'playhead' in m_columns else ''}
             FROM media
             WHERE coalesce(time_deleted, 0) = 0
                 and coalesce(playhead, 0) > 60
                 and coalesce(play_count, 0) = 0
             ORDER BY time_played desc, playhead desc
             LIMIT {args.limit or 5}
         """
@@ -124,18 +127,18 @@
 
     elif args.facet.startswith(("all", "watched")):
         print("Finished watching:")
         tbl = player.historical_usage(args, args.frequency, "time_played", "and coalesce(play_count, 0)>0")
         print_history(tbl)
         query = f"""SELECT
                 path
-                , title
-                , duration
-                , subtitle_count
-                , time_played
+                {', title' if 'title' in m_columns else ''}
+                {', duration' if 'duration' in m_columns else ''}
+                {', subtitle_count' if 'subtitle_count' in m_columns else ''}
+                {', time_played' if 'time_played' in m_columns else ''}
             FROM media
             WHERE coalesce(play_count, 0)>0
             ORDER BY time_played desc, path
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
         print_recent(tbl, "time_played")
```

### Comparing `xklb-1.30.6/xklb/scripts/merge_dbs.py` & `xklb-1.30.7/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/merge_online_local.py` & `xklb-1.30.7/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/move_list.py` & `xklb-1.30.7/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/optimize_db.py` & `xklb-1.30.7/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/playlists.py` & `xklb-1.30.7/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/redownload.py` & `xklb-1.30.7/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/relmv.py` & `xklb-1.30.7/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/scatter.py` & `xklb-1.30.7/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/streaming_tab_loader.py` & `xklb-1.30.7/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/mining/data.py` & `xklb-1.30.7/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/mining/extract_links.py` & `xklb-1.30.7/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/mining/nouns.py` & `xklb-1.30.7/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/mining/pushshift.py` & `xklb-1.30.7/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.30.7/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/xklb/assets/kotobago.png` & `xklb-1.30.7/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/.gitignore` & `xklb-1.30.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/LICENSE` & `xklb-1.30.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/README.md` & `xklb-1.30.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.30.006)
+    xk media library subcommands (v1.30.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.30.6/pyproject.toml` & `xklb-1.30.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.30.6/PKG-INFO` & `xklb-1.30.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.30.6
+Version: 1.30.7
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -223,15 +223,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.30.006)
+    xk media library subcommands (v1.30.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

