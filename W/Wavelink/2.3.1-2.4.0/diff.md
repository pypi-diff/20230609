# Comparing `tmp/Wavelink-2.3.1.tar.gz` & `tmp/Wavelink-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Wavelink-2.3.1.tar", last modified: Sun May 21 00:10:17 2023, max compression
+gzip compressed data, was "Wavelink-2.4.0.tar", last modified: Fri Jun  9 02:56:36 2023, max compression
```

## Comparing `Wavelink-2.3.1.tar` & `Wavelink-2.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.462276 Wavelink-2.3.1/
--rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.3.1/LICENSE
--rw-rw-rw-   0        0        0     5772 2023-05-21 00:10:17.461774 Wavelink-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.3.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.377169 Wavelink-2.3.1/Wavelink.egg-info/
--rw-rw-rw-   0        0        0     5772 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1006 2023-05-21 00:09:01.000000 Wavelink-2.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 00:10:17.462776 Wavelink-2.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.436127 Wavelink-2.3.1/wavelink/
--rw-rw-rw-   0        0        0     1495 2023-05-21 00:09:01.000000 Wavelink-2.3.1/wavelink/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/backoff.py
--rw-rw-rw-   0        0        0     2225 2023-05-20 08:30:58.000000 Wavelink-2.3.1/wavelink/enums.py
--rw-rw-rw-   0        0        0     1995 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.351676 Wavelink-2.3.1/wavelink/ext/
-drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.442187 Wavelink-2.3.1/wavelink/ext/spotify/
--rw-rw-rw-   0        0        0    16455 2023-04-01 01:28:43.000000 Wavelink-2.3.1/wavelink/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/filters.py
--rw-rw-rw-   0        0        0    17765 2023-04-04 07:37:42.000000 Wavelink-2.3.1/wavelink/node.py
--rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.3.1/wavelink/payloads.py
--rw-rw-rw-   0        0        0    20971 2023-05-21 00:07:39.000000 Wavelink-2.3.1/wavelink/player.py
--rw-rw-rw-   0        0        0    12384 2023-03-15 08:08:05.000000 Wavelink-2.3.1/wavelink/queue.py
--rw-rw-rw-   0        0        0    10102 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/tracks.py
-drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.460773 Wavelink-2.3.1/wavelink/types/
--rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/types/events.py
--rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/types/request.py
--rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/types/state.py
--rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/types/track.py
--rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.3.1/wavelink/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.083344 Wavelink-2.4.0/
+-rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0     5772 2023-06-09 02:56:36.083344 Wavelink-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.069282 Wavelink-2.4.0/Wavelink.egg-info/
+-rw-rw-rw-   0        0        0     5772 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1006 2023-06-05 09:48:12.000000 Wavelink-2.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 02:56:36.083344 Wavelink-2.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.078839 Wavelink-2.4.0/wavelink/
+-rw-rw-rw-   0        0        0     1495 2023-06-05 09:48:12.000000 Wavelink-2.4.0/wavelink/__init__.py
+-rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/backoff.py
+-rw-rw-rw-   0        0        0     3689 2023-06-05 10:25:32.000000 Wavelink-2.4.0/wavelink/enums.py
+-rw-rw-rw-   0        0        0     3028 2023-06-05 09:44:43.000000 Wavelink-2.4.0/wavelink/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.052882 Wavelink-2.4.0/wavelink/ext/
+drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.079340 Wavelink-2.4.0/wavelink/ext/spotify/
+-rw-rw-rw-   0        0        0    17854 2023-06-05 11:43:40.000000 Wavelink-2.4.0/wavelink/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/filters.py
+-rw-rw-rw-   0        0        0    17836 2023-06-05 08:54:30.000000 Wavelink-2.4.0/wavelink/node.py
+-rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.4.0/wavelink/payloads.py
+-rw-rw-rw-   0        0        0    21928 2023-06-05 13:30:06.000000 Wavelink-2.4.0/wavelink/player.py
+-rw-rw-rw-   0        0        0    12384 2023-03-15 08:08:05.000000 Wavelink-2.4.0/wavelink/queue.py
+-rw-rw-rw-   0        0        0    10222 2023-06-05 10:36:36.000000 Wavelink-2.4.0/wavelink/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.082342 Wavelink-2.4.0/wavelink/types/
+-rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/types/events.py
+-rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/types/request.py
+-rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/types/state.py
+-rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/types/track.py
+-rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.4.0/wavelink/websocket.py
```

### Comparing `Wavelink-2.3.1/LICENSE` & `Wavelink-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.1/PKG-INFO` & `Wavelink-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.3.1
+Version: 2.4.0
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.3.1/README.rst` & `Wavelink-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.1/Wavelink.egg-info/PKG-INFO` & `Wavelink-2.4.0/Wavelink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.3.1
+Version: 2.4.0
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.3.1/Wavelink.egg-info/SOURCES.txt` & `Wavelink-2.4.0/Wavelink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.1/pyproject.toml` & `Wavelink-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Wavelink"
-version = "2.3.1"
+version = "2.4.0"
 authors = [
   { name="EvieePy", email="evieepy@gmail.com" },
 ]
 dynamic = ["dependencies"]
 description = "A robust and powerful Lavalink wrapper for discord.py"
 readme = "README.rst"
 requires-python = ">=3.10"
```

### Comparing `Wavelink-2.3.1/wavelink/__init__.py` & `Wavelink-2.4.0/wavelink/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __title__ = "WaveLink"
 __author__ = "PythonistaGuild, EvieePy"
 __license__ = "MIT"
 __copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.3.1"
+__version__ = "2.4.0"
 
 from .enums import *
 from .exceptions import *
 from .node import *
 from .payloads import *
 from .player import Player as Player
 from .tracks import *
```

### Comparing `Wavelink-2.3.1/wavelink/backoff.py` & `Wavelink-2.4.0/wavelink/backoff.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.1/wavelink/ext/spotify/__init__.py` & `Wavelink-2.4.0/wavelink/ext/spotify/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,20 +99,24 @@
 
     return None
 
 
 class SpotifySearchType(enum.Enum):
     """An enum specifying which type to search for with a given Spotify ID.
 
+    Attributes
+    ----------
     track
         Default search type. Unless specified otherwise this will always be the search type.
     album
-        Search for an album.
+        Album search type.
     playlist
-        Search for a playlist.
+        Playlist search type.
+    unusable
+        Unusable type. This type is returned when Wavelink can not be used to play this track.
     """
     track = 0
     album = 1
     playlist = 2
     unusable = 3
 
 
@@ -257,24 +261,46 @@
 
         Search for tracks with the given query.
 
         Parameters
         ----------
         query: str
             The song to search for.
-        type: Optional[:class:`spotify.SpotifySearchType`]
+        type: Optional[:class:`~SpotifySearchType`]
             An optional enum value to use when searching with Spotify. Defaults to track.
         node: Optional[:class:`wavelink.Node`]
             An optional Node to use to make the search with.
         return_first: Optional[bool]
             An optional bool which when set to True will return only the first track found. Defaults to False.
 
         Returns
         -------
-        Union[Optional[Track], List[Track]]
+        Union[Optional[:class:`SpotifyTrack`], List[:class:`SpotifyTrack`]]
+
+        Examples
+        --------
+        Searching for a singular tack to play...
+
+        .. code:: python3
+
+            track: spotify.SpotifyTrack = await spotify.SpotifyTrack.search(query=SPOTIFY_URL)
+
+
+        Searching for all tracks in an album...
+
+        .. code:: python3
+
+            tracks: list[spotify.SpotifyTrack] =
+            await spotify.SpotifyTrack.search(query=SPOTIFY_URL, type=spotify.SpotifySearchType.album)
+
+
+        .. note::
+
+            See :func:`~.decode_url` for gathering information about the supplied URL, including search type.
+            Before using this method.
         """
         if node is None:
             node: Node = NodePool.get_connected_node()
 
         if type == SpotifySearchType.track:
             tracks = await node._spotify._search(query=query, type=type)
 
@@ -295,55 +321,69 @@
 
         Parameters
         ----------
         query: str
             The Spotify URL or ID to search for. Must be of type Playlist or Album.
         limit: Optional[int]
             Limit the amount of tracks returned.
-        type: :class:`SpotifySearchType`
+        type: :class:`~SpotifySearchType`
             The type of search. Must be either playlist or album. Defaults to playlist.
-        node: Optional[:class:`Node`]
-            An optional node to use when querying for tracks. Defaults to best available.
+        node: Optional[:class:`wavelink.Node`]
+            An optional node to use when querying for tracks. Defaults to the best available.
 
         Examples
         --------
 
         .. code:: python3
 
                 async for track in spotify.SpotifyTrack.iterator(query=..., type=spotify.SpotifySearchType.playlist):
                     ...
+
+
+        .. note::
+
+            See :func:`~.decode_url` for gathering information about the supplied URL, including search type.
+            Before using this method.
         """
 
         if type is not SpotifySearchType.album and type is not SpotifySearchType.playlist:
             raise TypeError("Iterator search type must be either album or playlist.")
 
         if node is None:
             node = NodePool.get_connected_node()
 
         return SpotifyAsyncIterator(query=query, limit=limit, node=node, type=type)
 
     @classmethod
     async def convert(cls: Type[ST], ctx: commands.Context, argument: str) -> ST:
         """Converter which searches for and returns the first track.
 
-        Used as a type hint in a discord.py command.
+        Used as a type hint in a
+        `discord.py command <https://discordpy.readthedocs.io/en/stable/ext/commands/commands.html>`_.
         """
         results = await cls.search(argument)
 
         if not results:
             raise commands.BadArgument("Could not find any songs matching that query.")
 
         return results[0]
 
     async def fulfill(self, *, player: Player, cls: Playable, populate: bool) -> Playable:
-        """
+        """Used to fulfill the :class:`wavelink.Player` Auto Play Queue.
+
+        .. warning::
+
+            Usually you would not call this directly. Instead you would set :attr:`wavelink.Player.autoplay` to true,
+            and allow the player to fulfill this request automatically.
+
+
         Parameters
         ----------
         player: :class:`wavelink.player.Player`
-            If Player.autoplay is enabled, this search will fill the AutoPlay Queue.
+            If :attr:`wavelink.Player.autoplay` is enabled, this search will fill the AutoPlay Queue with more tracks.
         cls
             The class to convert this Spotify Track to.
         """
         try:
             tracks: list[cls] = await cls.search(f'"{self.isrc}"')
         except wavelink.NoTracksError:
             tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
@@ -376,15 +416,15 @@
 
             await player.auto_queue.put_wait(reco)
 
         return tracks[0]
 
 
 class SpotifyClient:
-    """Spotify client passed to Nodes for searching via Spotify.
+    """Spotify client passed to :class:`wavelink.Node` for searching via Spotify.
 
     Parameters
     ----------
     client_id: str
         Your spotify application client ID.
     client_secret: str
         Your spotify application secret.
```

### Comparing `Wavelink-2.3.1/wavelink/filters.py` & `Wavelink-2.4.0/wavelink/filters.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.1/wavelink/node.py` & `Wavelink-2.4.0/wavelink/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,16 @@
         Raises
         ------
         ValueError
             Loading the playlist failed.
         WavelinkException
             An unspecified error occurred when loading the playlist.
         """
-        data = await self._send(method='GET', path='loadtracks', query=f'identifier={query}')
+        encoded_query = urllib.parse.quote(query)
+        data = await self._send(method='GET', path='loadtracks', query=f'identifier={encoded_query}')
 
         load_type = try_enum(LoadType, data.get("loadType"))
 
         if load_type is LoadType.load_failed:
             # TODO Proper exception...
             raise ValueError('Tracks failed to Load.')
 
@@ -334,16 +335,16 @@
         Parameters
         ----------
         cls: type[PlayableT]
             The type of Playable track that should be returned.
         encoded: str
             The Tracks unique encoded string.
         """
-        encoded = urllib.parse.quote(encoded)
-        data = await self._send(method='GET', path='decodetrack', query=f'encodedTrack={encoded}')
+        encoded_query = urllib.parse.quote(encoded)
+        data = await self._send(method='GET', path='decodetrack', query=f'encodedTrack={encoded_query}')
 
         return cls(data=data)
 
 
 # noinspection PyShadowingBuiltins
 class NodePool:
     """The Wavelink NodePool is responsible for keeping track of all :class:`Node`.
```

### Comparing `Wavelink-2.3.1/wavelink/payloads.py` & `Wavelink-2.4.0/wavelink/payloads.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.1/wavelink/player.py` & `Wavelink-2.4.0/wavelink/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import logging
 from typing import TYPE_CHECKING, Any, Union
 
 import discord
 from discord.utils import MISSING
 
 from .enums import *
-from .exceptions import InvalidLavalinkResponse, QueueEmpty
+from .exceptions import *
 from .ext import spotify
 from .filters import Filter
 from .node import Node, NodePool
 from .payloads import TrackEventPayload
 from .queue import Queue
 from .tracks import *
 
@@ -58,15 +58,15 @@
     discord.VoiceChannel, discord.StageChannel
 ]  # todo: VocalGuildChannel?
 
 
 class Player(discord.VoiceProtocol):
     """Wavelink Player class.
 
-    This class is used as a :class:`discord.VoiceProtocol` and inherits all its members.
+    This class is used as a :class:`~discord.VoiceProtocol` and inherits all its members.
 
 
     .. note::
 
         The Player class come with an in-built queue. See :class:`queue.Queue`.
 
     Parameters
@@ -76,15 +76,15 @@
         the best connected Node will be used.
     swap_node_on_disconnect: bool
         If a list of :class:`node.Node` is provided the Player will swap Nodes on Node disconnect.
         Defaults to True.
 
     Attributes
     ----------
-    client: :class:discord.Client`
+    client: :class:`discord.Client`
         The discord Client or Bot associated with this Player.
     channel: :class:`discord.VoiceChannel`
         The channel this player is currently connected to.
     nodes: list[:class:`node.Node`]
         The list of Nodes this player is currently using.
     current_node: :class:`node.Node`
         The Node this player is currently using.
@@ -115,17 +115,19 @@
         self.client: discord.Client = client
         self.channel: VoiceChannel | None = channel
 
         self.nodes: list[Node]
         self.current_node: Node
 
         if swap_node_on_disconnect and not nodes:
-            self.nodes = list(NodePool.nodes.values())
+            nodes = list(NodePool.nodes.values())
+            self.nodes = sorted(nodes, key=lambda n: len(n.players))
             self.current_node = self.nodes[0]
         elif nodes:
+            nodes = sorted(nodes, key=lambda n: len(n.players))
             self.current_node = nodes[0]
             self.nodes = nodes
         else:
             self.current_node = NodePool.get_connected_node()
             self.nodes = [self.current_node]
 
         if not self.client:
@@ -328,15 +330,35 @@
                                                              guild_id=self._guild.id,
                                                              data=voice)
 
         logger.debug(f'Dispatching VOICE_UPDATE: {resp}')
 
     async def connect(self, *, timeout: float, reconnect: bool, **kwargs: Any) -> None:
         if self.channel is None:
-            raise RuntimeError('')
+            self._invalidate()
+
+            msg: str = 'Please use the method "discord.VoiceChannel.connect" and pass this player to cls='
+            raise InvalidChannelStateError(msg)
+
+        if not self.channel.permissions_for(self.channel.guild.me).connect:
+            self._invalidate()
+
+            raise InvalidChannelPermissions('You do not have connect permissions to join this channel.')
+
+        limit: int = self.channel.user_limit
+        total: int = len(self.channel.members)
+
+        if limit == 0:
+            pass
+
+        elif total >= limit:
+            self._invalidate()
+
+            msg: str = f'There are currently too many users in this channel. <{total}/{limit}>'
+            raise InvalidChannelPermissions(msg)
 
         if not self._guild:
             self._guild = self.channel.guild
             self.current_node._players[self._guild.id] = self
 
         await self.channel.guild.change_voice_state(channel=self.channel, **kwargs)
 
@@ -552,14 +574,19 @@
                                                              guild_id=self._guild.id,
                                                              data=data)        
 
         if self.is_playing() and seek:
             await self.seek(int(self.position))
         logger.debug(f"Set filter:: {self._filter} ({self.channel.id})")
 
+    def _invalidate(self) -> None:
+        self._voice_state = {}
+        self._player_state = {}
+        self.channel = None
+
     async def _destroy(self) -> None:
         self.autoplay = False
         self._voice_state = {}
         self._player_state = {}
 
         self.cleanup()
         self.channel = None
```

### Comparing `Wavelink-2.3.1/wavelink/queue.py` & `Wavelink-2.4.0/wavelink/queue.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.1/wavelink/tracks.py` & `Wavelink-2.4.0/wavelink/tracks.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         The length of the track in milliseconds.
     duration: int
         An alias for length.
     position: int
         The position the track will start in milliseconds. Defaults to 0.
     title: str
         The Track title.
-    source: :class:`TrackSource`
+    source: :class:`wavelink.TrackSource`
         The source this Track was fetched from.
     uri: Optional[str]
         The URI of this track. Could be None.
     author: Optional[str]
         The author of this track. Could be None.
     identifier: Optional[str]
         The Youtube/YoutubeMusic identifier for this track. Could be None.
@@ -188,17 +188,17 @@
 
         Parameters
         ----------
         query: str
             The query to search for.
         return_first: Optional[bool]
             Whether to return the first track from the search results. Defaults to False.
-        node: Optional[:class:`Node`]
-            The node to use when searching for tracks. If no :class:`Node` is passed,
-            one will be fetched via the :class:`NodePool`.
+        node: Optional[:class:`wavelink.Node`]
+            The node to use when searching for tracks. If no :class:`wavelink.Node` is passed,
+            one will be fetched via the :class:`wavelink.NodePool`.
         """
 
         check = yarl.URL(query)
 
         if str(check.host) == 'youtube.com' or str(check.host) == 'www.youtube.com' and check.query.get("list") or \
                 cls.PREFIX == 'ytpl:':
 
@@ -217,15 +217,16 @@
 
         return tracks
 
     @classmethod
     async def convert(cls, ctx: commands.Context, argument: str) -> Self:
         """Converter which searches for and returns the first track.
 
-        Used as a type hint in a discord.py command.
+        Used as a type hint in a
+        `discord.py command <https://discordpy.readthedocs.io/en/stable/ext/commands/commands.html>`_.
         """
         results = await cls.search(argument)
 
         if not results:
             raise commands.BadArgument("Could not find any songs matching that query.")
 
         if issubclass(cls, YouTubePlaylist):
@@ -249,15 +250,15 @@
     @property
     def thumbnail(self) -> str:
         """The URL to the thumbnail of this video.
 
         .. note::
 
             Due to YouTube limitations this may not always return a valid thumbnail.
-            Use :func:`.fetch_thumbnail` to fallback.
+            Use :meth:`.fetch_thumbnail` to fallback.
 
         Returns
         -------
         str
             The URL to the video thumbnail.
         """
         return f"https://img.youtube.com/vi/{self.identifier}/maxresdefault.jpg"
```

### Comparing `Wavelink-2.3.1/wavelink/types/events.py` & `Wavelink-2.4.0/wavelink/types/events.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.1/wavelink/types/request.py` & `Wavelink-2.4.0/wavelink/types/request.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.1/wavelink/websocket.py` & `Wavelink-2.4.0/wavelink/websocket.py`

 * *Files identical despite different names*

