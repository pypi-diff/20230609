# Comparing `tmp/plex-tvdb-alt-orderer-0.1.0.tar.gz` & `tmp/plex-tvdb-alt-orderer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-tvdb-alt-orderer-0.1.0.tar", last modified: Thu Jun  8 19:16:41 2023, max compression
+gzip compressed data, was "plex-tvdb-alt-orderer-0.2.0.tar", last modified: Fri Jun  9 21:23:43 2023, max compression
```

## Comparing `plex-tvdb-alt-orderer-0.1.0.tar` & `plex-tvdb-alt-orderer-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 19:16:41.168238 plex-tvdb-alt-orderer-0.1.0/
--rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2980 2023-06-08 19:16:41.168238 plex-tvdb-alt-orderer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2360 2023-06-08 19:08:55.000000 plex-tvdb-alt-orderer-0.1.0/README.md
--rw-rw-rw-   0        0        0      850 2023-06-08 19:16:22.000000 plex-tvdb-alt-orderer-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 19:16:41.169237 plex-tvdb-alt-orderer-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-08 19:16:41.133675 plex-tvdb-alt-orderer-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 19:16:41.137674 plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer/
--rw-rw-rw-   0        0        0     6006 2023-06-08 18:47:25.000000 plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer/main.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:16:41.167236 plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer.egg-info/
--rw-rw-rw-   0        0        0     2980 2023-06-08 19:16:41.000000 plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-08 19:16:41.000000 plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 19:16:41.000000 plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-08 19:16:41.000000 plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-06-08 19:16:41.000000 plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-08 19:16:41.000000 plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 21:23:43.819000 plex-tvdb-alt-orderer-0.2.0/
+-rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5612 2023-06-09 21:23:43.817480 plex-tvdb-alt-orderer-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4992 2023-06-09 21:17:45.000000 plex-tvdb-alt-orderer-0.2.0/README.md
+-rw-rw-rw-   0        0        0      877 2023-06-09 21:00:18.000000 plex-tvdb-alt-orderer-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 21:23:43.819000 plex-tvdb-alt-orderer-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 21:23:43.712391 plex-tvdb-alt-orderer-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 21:23:43.746446 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer/
+-rw-rw-rw-   0        0        0     8107 2023-06-09 21:17:11.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 21:23:43.807482 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/
+-rw-rw-rw-   0        0        0     5612 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-09 21:23:43.000000 plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
```

### Comparing `plex-tvdb-alt-orderer-0.1.0/LICENSE` & `plex-tvdb-alt-orderer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-tvdb-alt-orderer-0.1.0/pyproject.toml` & `plex-tvdb-alt-orderer-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "plex-tvdb-alt-orderer"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="bpoxy" },
 ]
 description = "A utility that applies alternate TVDB orders to Plex."
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = ["click", "inquirer", "plexapi", "progress", "tvdb_v4_official"]
+dependencies = ["click", "inquirer", "plexapi", "progress", "termcolor", "tvdb_v4_official", "validators"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Multimedia :: Video",
 ]
```

### Comparing `plex-tvdb-alt-orderer-0.1.0/src/plex_tvdb_alt_orderer/main.py` & `plex-tvdb-alt-orderer-0.2.0/src/plex_tvdb_alt_orderer/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,133 @@
 import click
 import inquirer
 import re
-from plexapi.myplex import MyPlexAccount, MyPlexResource
+import validators
+from plexapi.myplex import MyPlexAccount, PlexServer
 from plexapi.library import ShowSection
 from plexapi.video import Episode, Show
 from progress.bar import Bar
+from termcolor import colored
 from tvdb_v4_official import TVDB
 
-@click.command()
-@click.option("--plex-library", "plex_section_name", type=str, help="Your Plex TV show library name. Omit to choose from a list interactively or if your Plex server has a single TV show library.")
-@click.option("--plex-password", type=str, help="Your Plex password. Omit to enter interactively.")
-@click.option("--plex-server", type=str, help="Your Plex server name. Omit to enter interactively.")
-@click.option("--plex-show", "plex_show_name", type=str, help="The name of the show in Plex. Omit to enter interactively.")
-@click.option("--plex-user", type=str, help="Your Plex username. Omit to enter interactively.")
-@click.option("--tvdb-order", "tvdb_order_name", type=str, help="The TVDB order name (as specified for API-connected systems). Omit to choose from a list interactively.")
-@click.option("--tvdb-pin", type=str, help="Your TVDB subscriber PIN. Omit to enter interactively.")
-
-def main(plex_section_name: str, plex_password: str, plex_server: str, plex_show_name: str, plex_user: str, tvdb_order_name: str, tvdb_pin: str):
-    questions = []
-
-    if not tvdb_pin:
-        questions.append(inquirer.Text("tvdb_pin", message="Enter your TVDB subscriber PIN"))
-    if not plex_user:
-        questions.append(inquirer.Text("plex_user", message="Enter your Plex username"))
-    if not plex_password:
-        questions.append(inquirer.Text("plex_password", message="Enter your Plex password"))
-    if not plex_server:
-        questions.append(inquirer.Text("plex_server", message="Enter your Plex server name"))
-
-    answers = inquirer.prompt(questions)
+UPDATE_ENTIRE_SERIES = -1
 
-    plex_account = MyPlexAccount(plex_user or answers["plex_user"], plex_password or answers["plex_password"])
-    plex = plex_account.resource(plex_server or answers["plex_server"]).connect()
-
-    plex_section = get_plex_section(plex, plex_section_name)
+@click.command()
+@click.option("--plex-library", "plex_section_name", type=str, envvar="ALT_ORDERER_PLEX_LIBRARY",
+              help="Your Plex TV show library name. Omit to use the ALT_ORDERER_PLEX_LIBRARY environment variable, choose from a list interactively or if your Plex server has a sole TV show library.")
+@click.option("--plex-password", type=str, envvar="ALT_ORDERER_PLEX_PASSWORD",
+              help="Your Plex password. Omit to use the ALT_ORDERER_PLEX_PASSWORD environment variable or enter interactively.")
+@click.option("--plex-server", "plex_server_identifier", type=str, envvar="ALT_ORDERER_PLEX_SERVER",
+              help="Your Plex server name (user/password authentication) or URL (token authentication). Omit to use the ALT_ORDERER_PLEX_SERVER environment variable or enter interactively.")
+@click.option("--plex-show", "plex_show_name", type=str, envvar="ALT_ORDERER_PLEX_SHOW",
+              help="The name of the show in Plex. Omit to use the ALT_ORDERER_PLEX_SHOW environment variable or enter interactively.")
+@click.option("--plex-token", type=str, envvar="ALT_ORDERER_PLEX_TOKEN",
+              help="Your Plex token. Omit to use the ALT_ORDERER_PLEX_TOKEN environment variable or enter interactively.")
+@click.option("--plex-user", type=str, envvar="ALT_ORDERER_PLEX_USER",
+              help="Your Plex username. Omit to use the ALT_ORDERER_PLEX_USER environment variable or enter interactively.")
+@click.option("--season", type=int, envvar="ALT_ORDERER_SEASON",
+              help=f"The season to update ({UPDATE_ENTIRE_SERIES} to update the entire series). Omit to use the ALT_ORDERER_SEASON environment variable or enter interactively.")
+@click.option("--tvdb-order", "tvdb_order_name", type=str, envvar="ALT_ORDERER_TVDB_ORDER",
+              help="The TVDB order name (as specified for API-connected systems). Omit to use the ALT_ORDERER_TVDB_ORDER environment variable or choose from a list interactively.")
+@click.option("--tvdb-pin", type=str, envvar="ALT_ORDERER_TVDB_PIN",
+              help="Your TVDB subscriber PIN. Omit to use the ALT_ORDERER_TVDB_PIN environment variable or enter interactively.")
+
+def main(plex_section_name: str, plex_password: str, plex_server_identifier: str, plex_show_name: str, plex_token: str, plex_user: str, season: int, tvdb_order_name: str, tvdb_pin: str):
+    plex_server = get_plex_server(plex_password, plex_server_identifier, plex_token, plex_user)
+    plex_section = get_plex_section(plex_server, plex_section_name)
     plex_show = get_plex_show(plex_section, plex_show_name)
     plex_episodes = plex_show.episodes()
+    
+    tvdb_pin = text_prompt_if_unspecified(tvdb_pin, "your TVDB subscriber PIN")
+    tvdb = TVDB(apikey="5f119e31-f9c5-4f0c-b1c3-064b3225e7d9", pin=tvdb_pin)
     tvdb_id = next(match.group("id") for match in [re.match(r"tvdb://(?P<id>\d+)", guid.id) for guid in plex_show.guids] if match)
-
-    tvdb = TVDB(apikey="5f119e31-f9c5-4f0c-b1c3-064b3225e7d9", pin=tvdb_pin or answers["tvdb_pin"])
     tvdb_season_type = get_tvdb_season_type(tvdb, tvdb_id, tvdb_order_name)
     tvdb_episodes = tvdb.get_series_episodes(tvdb_id, season_type=tvdb_season_type, lang="eng")["episodes"]
     
-    update_plex(plex_episodes, tvdb_episodes)
+    update_plex(season, plex_episodes, tvdb_episodes)
 
-def get_plex_section(plex: MyPlexResource, section_name: str) -> ShowSection:
-    sections = list(filter(lambda s: s.TYPE == "show", plex.library.sections()))
+def dict_to_tuple(dict: dict):
+    return [(key, value) for key, value in dict.items()]
 
-    if section_name:
-        section = next(filter(lambda s: s.title == section_name, sections), None)
-        
-        if not section:
-            raise ValueError(f"Your Plex server doesn't contain a TV show library named '{section_name}'.")
+def error_exit(text: str):
+    print(colored(text, "red"))
+    exit()
+
+def get_plex_section(plex_server: PlexServer, section_name: str) -> ShowSection:
+    sections = list(filter(lambda s: s.TYPE == "show", plex_server.library.sections()))
+    sections_dict = {s.title: s for s in sections}
 
-        return section
+    if section_name:
+        return sections_dict.get(section_name, None) or error_exit(f"Your Plex server doesn't contain a TV show library named '{section_name}'.")
 
     if len(sections) == 0:
-        raise ValueError(f"Your Plex server doesn't contain a TV show library.")
+        error_exit(f"Your Plex server doesn't contain a TV show library.")
     elif len(sections) == 1:
-        section = sections[0]
+        return sections[0]
     else:
-        sections_dict = {s.title: s for s in sections}
-        section_title = inquirer.prompt([inquirer.List("section_title", message="Select the library to update", choices=sections_dict.keys())])["section_title"]
-        section = sections_dict[section_title]
+        return inquirer.prompt([inquirer.List("section", message="Select the library to update", choices=dict_to_tuple(sections_dict))])["section"]
+
+def get_plex_server(plex_password: str, plex_server_identifier: str, plex_token: str, plex_user: str) -> PlexServer:
+    plex_server_identifier = text_prompt_if_unspecified(plex_server_identifier, "your Plex server name (user/password authentication) or URL (token authentication)")
+
+    if validators.url(plex_server_identifier):
+        return PlexServer(plex_server_identifier, text_prompt_if_unspecified(plex_token, "your Plex token"))
 
-    return section
+    plex_user = text_prompt_if_unspecified(plex_user, "your Plex username")
+    plex_password = plex_password or inquirer.prompt([inquirer.Password("password", message=f"Enter your Plex password")])["password"]
+    plex_account = MyPlexAccount(plex_user, plex_password)
+    return plex_account.resource(plex_server_identifier).connect()
 
 def get_plex_show(section: ShowSection, show_name: str) -> Show:
-    show_name = show_name or inquirer.prompt([inquirer.Text("show_name", message="Enter the name of the show")])["show_name"]
+    show_name = text_prompt_if_unspecified(show_name, "the name of the show")
     shows = section.search(title=show_name)
 
     if len(shows) == 0:
-        raise ValueError(f"Your TV show library doesn't contain a show with name '{show_name}'.")
+         error_exit(f"Your TV show library doesn't contain a show with name '{show_name}'.")
     elif len(shows) == 1:
-        show = shows[0]
+        return shows[0]
     else:
         shows_dict = {s.title: s for s in shows}
-        show_title = inquirer.prompt([inquirer.List("show_title", message="Select the show to update", choices=shows_dict.keys())])["show_title"]
-        show = shows_dict[show_title]
-
-    return show
+        return inquirer.prompt([inquirer.List("show", message="Select the show to update", choices=dict_to_tuple(shows_dict))])["show"]
 
 def get_tvdb_season_type(tvdb: TVDB, tvdb_id: int, order_name: str) -> str:
     season_types = tvdb.get_season_types(tvdb_id)
     season_types_dict = {s["name"]: s["type"] for s in season_types}
 
-    if order_name and order_name not in season_types_dict:
-        raise ValueError(f"TVDB doesn't define an order with name '{order_name}'.")
+    if order_name:
+        return season_types_dict.get(order_name, None) or error_exit(f"TVDB doesn't define an order with name '{order_name}'.")
+
+    return inquirer.prompt([inquirer.List("season_type", message="Select the order to apply", choices=dict_to_tuple(season_types_dict))])["season_type"]
+
+def text_prompt_if_unspecified(value: str, description: str):
+    return value or inquirer.prompt([inquirer.Text("answer", message=f"Enter {description}")])["answer"]
 
-    season_type_name = order_name or inquirer.prompt([inquirer.List("season_type_name", message="Select the order to apply", choices=season_types_dict.keys())])["season_type_name"]
-    return season_types_dict[season_type_name]
+def update_plex(season: int, plex_episodes: list[Episode], tvdb_episodes: list[dict]):
+    plex_seasons_dict = {"Entire Series": UPDATE_ENTIRE_SERIES}
+    plex_seasons_dict.update({f"Season {e.parentIndex}": e.parentIndex for e in plex_episodes})
+    season = season or inquirer.prompt([inquirer.List("season", message="Select the season to update", choices=dict_to_tuple(plex_seasons_dict))])["season"]
+
+    if season != UPDATE_ENTIRE_SERIES:
+        plex_episodes = list(filter(lambda e: e.parentIndex == season, plex_episodes))
+        tvdb_episodes = list(filter(lambda e: e["seasonNumber"] == season, tvdb_episodes))
 
-def update_plex(plex_episodes: list[Episode], tvdb_episodes: list[dict]):
     tvdb_episode_dict = {}
 
     for e in tvdb_episodes:
         episode_number = e["number"]
         season_number = e["seasonNumber"]
 
         if season_number not in tvdb_episode_dict:
             tvdb_episode_dict[season_number] = {}
 
         tvdb_episode_dict[season_number][episode_number] = e
 
     for e in plex_episodes:
         if e.parentIndex not in tvdb_episode_dict or e.index not in tvdb_episode_dict[e.parentIndex]:
-            raise KeyError(f"S{e.parentIndex:02}E{e.index:02} doesn't exist in the selected TVDB order.")
+            error_exit(f"S{e.parentIndex:02}E{e.index:02} doesn't exist in the selected TVDB order.")
 
     progress = Bar("Updating Plex", max=len(plex_episodes))
 
     for e in plex_episodes:
         tvdb_episode = tvdb_episode_dict[e.parentIndex][e.index]
 
         e.editOriginallyAvailable(tvdb_episode["aired"])
```

